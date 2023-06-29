# Comparing `tmp/haruka-bot-1.6.0.post2.tar.gz` & `tmp/haruka-bot-1.6.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka-bot-1.6.0.post2.tar", last modified: Tue Jun 27 09:32:59 2023, max compression
+gzip compressed data, was "haruka-bot-1.6.0.post3.tar", last modified: Thu Jun 29 08:06:01 2023, max compression
```

## Comparing `haruka-bot-1.6.0.post2.tar` & `haruka-bot-1.6.0.post3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0    34522 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post2/LICENSE
--rw-r--r--   0        0        0     2790 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post2/README.md
--rw-r--r--   0        0        0      695 2023-06-27 09:30:10.174866 haruka-bot-1.6.0.post2/haruka_bot/__init__.py
--rw-r--r--   0        0        0       61 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/__main__.py
--rw-r--r--   0        0        0      189 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/cli/__init__.py
--rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/cli/bot.py
--rw-r--r--   0        0        0     1170 2023-06-27 09:18:39.724159 haruka-bot-1.6.0.post2/haruka_bot/cli/utils.py
--rw-r--r--   0        0        0     1390 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/config.py
--rw-r--r--   0        0        0       49 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/database/__init__.py
--rw-r--r--   0        0        0    10155 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/database/db.py
--rw-r--r--   0        0        0     1936 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/database/models.py
--rw-r--r--   0        0        0       30 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/libs/__init__.py
--rw-r--r--   0        0        0     1466 2023-06-27 09:18:39.708160 haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/__init__.py
--rw-r--r--   0        0        0     1085 2023-06-27 09:18:39.696161 haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/card.py
--rw-r--r--   0        0        0      598 2023-06-27 09:18:39.684162 haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/desc.py
--rw-r--r--   0        0        0     1024 2023-06-27 09:18:39.708160 haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/display.py
--rw-r--r--   0        0        0      816 2023-06-27 09:18:39.696161 haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/user_profile.py
--rw-r--r--   0        0        0      456 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/at/__init__.py
--rw-r--r--   0        0        0     1430 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/at/at_off.py
--rw-r--r--   0        0        0     1421 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/at/at_on.py
--rw-r--r--   0        0        0      678 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/auto_agree.py
--rw-r--r--   0        0        0      875 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/auto_delete.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/dynamic/__init__.py
--rw-r--r--   0        0        0     1048 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/dynamic/dynamic_off.py
--rw-r--r--   0        0        0     1039 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/dynamic/dynamic_on.py
--rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/help.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/live/__init__.py
--rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/live/live_off.py
--rw-r--r--   0        0        0     1012 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/live/live_on.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/permission/__init__.py
--rw-r--r--   0        0        0     1180 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/permission/permission_off.py
--rw-r--r--   0        0        0     1201 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/permission/permission_on.py
--rw-r--r--   0        0        0       58 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/pusher/__init__.py
--rw-r--r--   0        0        0     4710 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/pusher/dynamic_pusher.py
--rw-r--r--   0        0        0     2296 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/pusher/live_pusher.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/add_sub.py
--rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/delete_sub.py
--rw-r--r--   0        0        0     1551 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/sub_list.py
--rw-r--r--   0        0        0     8200 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/utils/__init__.py
--rw-r--r--   0        0        0     6922 2023-06-27 09:18:54.507058 haruka-bot-1.6.0.post2/haruka_bot/utils/browser.py
--rw-r--r--   0        0        0     5004 2023-06-27 09:31:40.804190 haruka-bot-1.6.0.post2/haruka_bot/utils/captcha.py
--rw-r--r--   0        0        0      702 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/utils/fonts_provider.py
--rw-r--r--   0        0        0     7316 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post2/haruka_bot/utils/mobile.js
--rw-r--r--   0        0        0       97 2023-06-27 09:32:29.010855 haruka-bot-1.6.0.post2/haruka_bot/version.py
--rw-r--r--   0        0        0     1545 2023-06-27 09:03:26.103394 haruka-bot-1.6.0.post2/pyproject.toml
--rw-r--r--   0        0        0     3345 1970-01-01 00:00:00.000000 haruka-bot-1.6.0.post2/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post3/LICENSE
+-rw-r--r--   0        0        0     2790 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post3/README.md
+-rw-r--r--   0        0        0      695 2023-06-27 12:36:22.037779 haruka-bot-1.6.0.post3/haruka_bot/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/__main__.py
+-rw-r--r--   0        0        0      189 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/cli/__init__.py
+-rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/cli/bot.py
+-rw-r--r--   0        0        0     1170 2023-06-27 12:36:22.037779 haruka-bot-1.6.0.post3/haruka_bot/cli/utils.py
+-rw-r--r--   0        0        0     1704 2023-06-29 07:51:56.377586 haruka-bot-1.6.0.post3/haruka_bot/config.py
+-rw-r--r--   0        0        0       49 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/database/__init__.py
+-rw-r--r--   0        0        0    10155 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/database/db.py
+-rw-r--r--   0        0        0     1936 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/database/models.py
+-rw-r--r--   0        0        0       30 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/libs/__init__.py
+-rw-r--r--   0        0        0     1466 2023-06-27 12:36:22.037779 haruka-bot-1.6.0.post3/haruka_bot/libs/dynamic/__init__.py
+-rw-r--r--   0        0        0     1085 2023-06-27 12:36:22.037779 haruka-bot-1.6.0.post3/haruka_bot/libs/dynamic/card.py
+-rw-r--r--   0        0        0      598 2023-06-27 12:36:22.037779 haruka-bot-1.6.0.post3/haruka_bot/libs/dynamic/desc.py
+-rw-r--r--   0        0        0     1024 2023-06-27 12:36:22.037779 haruka-bot-1.6.0.post3/haruka_bot/libs/dynamic/display.py
+-rw-r--r--   0        0        0      816 2023-06-27 12:36:22.037779 haruka-bot-1.6.0.post3/haruka_bot/libs/dynamic/user_profile.py
+-rw-r--r--   0        0        0      466 2023-06-28 01:28:28.418748 haruka-bot-1.6.0.post3/haruka_bot/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/at/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/at/at_off.py
+-rw-r--r--   0        0        0     1421 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/at/at_on.py
+-rw-r--r--   0        0        0      678 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/auto_agree.py
+-rw-r--r--   0        0        0      875 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/auto_delete.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/dynamic/__init__.py
+-rw-r--r--   0        0        0     1048 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/dynamic/dynamic_off.py
+-rw-r--r--   0        0        0     1039 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/dynamic/dynamic_on.py
+-rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/help.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/live/__init__.py
+-rw-r--r--   0        0        0      848 2023-06-28 01:33:02.285143 haruka-bot-1.6.0.post3/haruka_bot/plugins/live/live_now.py
+-rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/live/live_off.py
+-rw-r--r--   0        0        0     1012 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/live/live_on.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/permission/__init__.py
+-rw-r--r--   0        0        0     1180 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/permission/permission_off.py
+-rw-r--r--   0        0        0     1201 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/permission/permission_on.py
+-rw-r--r--   0        0        0       58 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/pusher/__init__.py
+-rw-r--r--   0        0        0     4979 2023-06-29 02:44:29.765587 haruka-bot-1.6.0.post3/haruka_bot/plugins/pusher/dynamic_pusher.py
+-rw-r--r--   0        0        0     2676 2023-06-28 02:22:02.465196 haruka-bot-1.6.0.post3/haruka_bot/plugins/pusher/live_pusher.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/sub/__init__.py
+-rw-r--r--   0        0        0     2039 2023-06-28 01:07:12.684442 haruka-bot-1.6.0.post3/haruka_bot/plugins/sub/add_sub.py
+-rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/sub/delete_sub.py
+-rw-r--r--   0        0        0     1551 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/plugins/sub/sub_list.py
+-rw-r--r--   0        0        0    11045 2023-06-28 02:20:18.900580 haruka-bot-1.6.0.post3/haruka_bot/utils/__init__.py
+-rw-r--r--   0        0        0     8714 2023-06-29 07:45:52.149895 haruka-bot-1.6.0.post3/haruka_bot/utils/browser.py
+-rw-r--r--   0        0        0     4947 2023-06-29 07:21:35.327692 haruka-bot-1.6.0.post3/haruka_bot/utils/captcha.py
+-rw-r--r--   0        0        0      702 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post3/haruka_bot/utils/fonts_provider.py
+-rw-r--r--   0        0        0     9451 2023-06-29 02:10:51.370603 haruka-bot-1.6.0.post3/haruka_bot/utils/mobile.js
+-rw-r--r--   0        0        0       97 2023-06-27 13:07:46.881260 haruka-bot-1.6.0.post3/haruka_bot/version.py
+-rw-r--r--   0        0        0     1579 2023-06-27 16:51:47.955635 haruka-bot-1.6.0.post3/pyproject.toml
+-rw-r--r--   0        0        0     3345 1970-01-01 00:00:00.000000 haruka-bot-1.6.0.post3/PKG-INFO
```

### Comparing `haruka-bot-1.6.0.post2/LICENSE` & `haruka-bot-1.6.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/README.md` & `haruka-bot-1.6.0.post3/README.md`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/__init__.py` & `haruka-bot-1.6.0.post3/haruka_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/cli/bot.py` & `haruka-bot-1.6.0.post3/haruka_bot/cli/bot.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/cli/utils.py` & `haruka-bot-1.6.0.post3/haruka_bot/cli/utils.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/config.py` & `haruka-bot-1.6.0.post3/haruka_bot/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List, Optional
 
+from loguru import logger
 from nonebot import get_driver
 from pydantic import BaseSettings, validator
 from pydantic.fields import ModelField
 
 
 # 其他地方出现的类似 from .. import config，均是从 __init__.py 导入的 Config 实例
 class Config(BaseSettings):
@@ -14,27 +15,33 @@
     haruka_proxy: Optional[str] = None
     haruka_interval: int = 10
     haruka_live_interval: int = haruka_interval
     haruka_dynamic_interval: int = 0
     haruka_dynamic_at: bool = False
     haruka_screenshot_style: str = "mobile"
     haruka_captcha_address: str = "https://captcha-cd.ngworks.cn"
+    haruka_browser_ua: Optional[str] = None
     haruka_dynamic_timeout: int = 30
     haruka_dynamic_font_source: str = "system"
     haruka_dynamic_font: Optional[str] = "Noto Sans CJK SC"
+    haruka_dynamic_big_image: bool = False
     haruka_command_prefix: str = ""
     # 频道管理员身份组
     haruka_guild_admin_roles: List[str] = ["频道主", "超级管理员"]
 
     @validator("haruka_interval", "haruka_live_interval", "haruka_dynamic_interval")
     def non_negative(cls, v: int, field: ModelField):
         """定时器为负返回默认值"""
-        if v < 1:
-            return field.default
-        return v
+        return field.default if v < 1 else v
+
+    @validator("haruka_screenshot_style")
+    def screenshot_style(cls, v: str):
+        if v != "mobile":
+            logger.warning("截图样式目前只支持 mobile，pc 样式现已被弃用")
+        return "mobile"
 
     class Config:
         extra = "ignore"
 
 
 global_config = get_driver().config
 plugin_config = Config.parse_obj(global_config)
```

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/database/db.py` & `haruka-bot-1.6.0.post3/haruka_bot/database/db.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/database/models.py` & `haruka-bot-1.6.0.post3/haruka_bot/database/models.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/__init__.py` & `haruka-bot-1.6.0.post3/haruka_bot/libs/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/card.py` & `haruka-bot-1.6.0.post3/haruka_bot/libs/dynamic/card.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/desc.py` & `haruka-bot-1.6.0.post3/haruka_bot/libs/dynamic/desc.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/display.py` & `haruka-bot-1.6.0.post3/haruka_bot/libs/dynamic/display.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/libs/dynamic/user_profile.py` & `haruka-bot-1.6.0.post3/haruka_bot/libs/dynamic/user_profile.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/at/at_off.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/at/at_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/at/at_on.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/at/at_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/auto_agree.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/auto_agree.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/auto_delete.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/auto_delete.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/dynamic/dynamic_off.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/dynamic/dynamic_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/dynamic/dynamic_on.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/dynamic/dynamic_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/help.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/help.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/live/live_off.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/live/live_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/live/live_on.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/live/live_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/permission/permission_off.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/permission/permission_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/permission/permission_on.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/permission/permission_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/pusher/dynamic_pusher.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/pusher/dynamic_pusher.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 uid,
                 timeout=plugin_config.haruka_dynamic_timeout,
                 proxy=plugin_config.haruka_proxy,
             )
         ).list
     except AioRpcError as e:
         if e.code() == StatusCode.DEADLINE_EXCEEDED:
-            logger.error("爬取动态超时，将在下个轮询中重试")
+            logger.error(f"爬取动态超时，将在下个轮询中重试：{e.code()} {e.details()}")
             return
         raise
 
     if not dynamics:  # 没发过动态
         if uid in offset and offset[uid] == -1:  # 不记录会导致第一次发动态不推送
             offset[uid] = 0
         return
@@ -66,36 +66,42 @@
         return
 
     dynamic = None
     for dynamic in sorted(dynamics, key=lambda x: int(x.extend.dyn_id_str)):  # 动态从旧到新排列
         dynamic_id = int(dynamic.extend.dyn_id_str)
         if dynamic_id > offset[uid]:
             logger.info(f"检测到新动态（{dynamic_id}）：{name}（{uid}）")
+            image, err = await get_dynamic_screenshot(dynamic_id)
             url = f"https://t.bilibili.com/{dynamic_id}"
-            image = await get_dynamic_screenshot(dynamic_id)
             if image is None:
                 logger.debug(f"动态不存在，已跳过：{url}")
                 return
-            elif dynamic.card_type == DynamicType.live_rcmd:
-                logger.debug(f"直播推荐动态，已跳过：{url}")
+            elif dynamic.card_type in [
+                DynamicType.live_rcmd,
+                DynamicType.live,
+                DynamicType.ad,
+                DynamicType.banner,
+            ]:
+                logger.debug(f"无需推送的动态 {dynamic.card_type}，已跳过：{url}")
+                offset[uid] = dynamic_id
                 return
 
             type_msg = {
                 0: "发布了新动态",
                 DynamicType.forward: "转发了一条动态",
                 DynamicType.word: "发布了新文字动态",
                 DynamicType.draw: "发布了新图文动态",
                 DynamicType.av: "发布了新投稿",
                 DynamicType.article: "发布了新专栏",
                 DynamicType.music: "发布了新音频",
             }
             message = (
                 f"{name} {type_msg.get(dynamic.card_type, type_msg[0])}：\n"
-                + MessageSegment.image(image)
-                + f"\n{url}"
+                f"{f'动态图片可能截图异常：{err}' if err else ''}\n"
+                f"{MessageSegment.image(image)}\n{url}"
             )
 
             push_list = await db.get_push_list(uid, "dynamic")
             for sets in push_list:
                 await safe_send(
                     bot_id=sets.bot_id,
                     send_type=sets.type,
@@ -119,18 +125,15 @@
             dy_sched, id="dynamic_sched", next_run_time=datetime.now(scheduler.timezone)
         )
 
 
 if plugin_config.haruka_dynamic_interval == 0:
     scheduler.add_listener(
         dynamic_lisener,
-        EVENT_JOB_EXECUTED
-        | EVENT_JOB_ERROR
-        | EVENT_JOB_MISSED
-        | EVENT_SCHEDULER_STARTED,
+        EVENT_JOB_EXECUTED | EVENT_JOB_ERROR | EVENT_JOB_MISSED | EVENT_SCHEDULER_STARTED,
     )
 else:
     scheduler.add_job(
         dy_sched,
         "interval",
         seconds=plugin_config.haruka_dynamic_interval,
         id="dynamic_sched",
```

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/pusher/live_pusher.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/pusher/live_pusher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import time
+
 from bilireq.live import get_rooms_info_by_uids
 from nonebot.adapters.onebot.v11.message import MessageSegment
 from nonebot.log import logger
 
 from ...config import plugin_config
 from ...database import DB as db
-from ...utils import PROXIES, safe_send, scheduler
+from ...utils import PROXIES, safe_send, scheduler, calc_time_total
 
 status = {}
+live_time = {}
 
 
 @scheduler.scheduled_job(
     "interval", seconds=plugin_config.haruka_live_interval, id="live_sched"
 )
 async def live_sched():
     """直播推送"""
@@ -30,30 +33,36 @@
         old_status = status[uid]
         if new_status == old_status:  # 直播间状态无变化
             continue
         status[uid] = new_status
 
         name = info["uname"]
         if new_status:  # 开播
-            room_id = info["short_id"] if info["short_id"] else info["room_id"]
-            url = "https://live.bilibili.com/" + str(room_id)
+            live_time[uid] = info["live_time"]
+            room_id = info["short_id"] or info["room_id"]
+            url = f"https://live.bilibili.com/{room_id}"
             title = info["title"]
-            cover = (
-                info["cover_from_user"] if info["cover_from_user"] else info["keyframe"]
-            )
+            cover = info["cover_from_user"] or info["keyframe"]
+            area_parent = info["area_v2_parent_name"]
+            area = info["area_v2_name"]
+            room_area = f"{area_parent} / {area}"
             logger.info(f"检测到开播：{name}（{uid}）")
-
             live_msg = (
-                f"{name} 正在直播：\n{title}\n" + MessageSegment.image(cover) + f"\n{url}"
+                f"{name} 开播啦！\n分区：{room_area}\n标题：{title}\n{MessageSegment.image(cover)}\n{url}"
             )
         else:  # 下播
             logger.info(f"检测到下播：{name}（{uid}）")
             if not plugin_config.haruka_live_off_notify:  # 没开下播推送
                 continue
-            live_msg = f"{name} 下播了"
+            live_time_msg = (
+                f"，本次直播时长 {calc_time_total(time.time() - live_time[uid])}。"
+                if live_time[uid]
+                else "。"
+            )
+            live_msg = f"{name} 下播了{live_time_msg}"
 
         # 推送
         push_list = await db.get_push_list(uid, "live")
         for sets in push_list:
             await safe_send(
                 bot_id=sets.bot_id,
                 send_type=sets.type,
```

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/add_sub.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/sub/add_sub.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """根据 UID 订阅 UP 主"""
     user = await db.get_user(uid=uid)
     name = user and user.name
     if not name:
         try:
             name = (await get_user_info(uid, reqtype="web", proxies=PROXIES))["name"]
         except ResponseCodeError as e:
-            if e.code == -400 or e.code == -404:
+            if e.code in [-400, -404]:
                 await add_sub.finish("UID不存在，注意UID不是房间号")
             elif e.code == -412:
                 await add_sub.finish("操作过于频繁IP暂时被风控，请半小时后再尝试")
             else:
                 await add_sub.finish(
                     f"未知错误，请联系开发者反馈，错误内容：\n\
                                     {str(e)}"
```

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/delete_sub.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/sub/delete_sub.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/plugins/sub/sub_list.py` & `haruka-bot-1.6.0.post3/haruka_bot/plugins/sub/sub_list.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/utils/__init__.py` & `haruka-bot-1.6.0.post3/haruka_bot/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import asyncio
 import sys
+import re
+import contextlib
+import datetime
 from pathlib import Path
 from typing import Union
+from bilireq.utils import get
 
 import httpx
 import nonebot
 from nonebot import on_command as _on_command
 from nonebot import require
 from nonebot.adapters.onebot.v11 import (
     ActionFailed,
@@ -19,18 +23,20 @@
 from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import ArgPlainText, CommandArg, RawCommand
 from nonebot.permission import SUPERUSER, Permission
 from nonebot.rule import Rule
-from nonebot_plugin_guild_patch import ChannelDestroyedNoticeEvent, GuildMessageEvent
 
 from ..config import plugin_config
 
+require("nonebot_plugin_guild_patch")
+from nonebot_plugin_guild_patch import ChannelDestroyedNoticeEvent, GuildMessageEvent  # noqa
+
 
 def get_path(*other):
     """获取数据文件绝对路径"""
     if plugin_config.haruka_dir:
         dir_path = Path(plugin_config.haruka_dir).resolve()
     else:
         dir_path = Path.cwd().joinpath("data")
@@ -38,38 +44,98 @@
     return str(dir_path.joinpath(*other))
 
 
 async def handle_uid(
     matcher: Matcher,
     command_arg: Message = CommandArg(),
 ):
-    uid = command_arg.extract_plain_text().strip()
-    if uid:
+    if command_arg.extract_plain_text().strip():
         matcher.set_arg("uid", command_arg)
 
 
 async def uid_check(
     matcher: Matcher,
     uid: str = ArgPlainText("uid"),
 ):
     uid = uid.strip()
-    if not uid.isdecimal():
-        await matcher.finish("UID 必须为纯数字")
+    if extract := await uid_extract(uid):
+        uid = extract
+    else:
+        await matcher.finish("未找到该 UP，请输入正确的 UP 群内昵称、UP 名、UP UID或 UP 首页链接")
     matcher.set_arg("uid", Message(uid))
 
 
+async def b23_extract(text: str):
+    if "b23.tv" not in text and "b23.wtf" not in text:
+        return None
+    if not (b23 := re.compile(r"b23.(tv|wtf)[\\/]+(\w+)").search(text)):
+        return None
+    try:
+        url = f"https://b23.tv/{b23[2]}"
+        for _ in range(3):
+            with contextlib.suppress(Exception):
+                resp = await httpx.AsyncClient().get(url, follow_redirects=True)
+                break
+        else:
+            return None
+        url = resp.url
+        logger.debug(f"b23.tv url: {url}")
+        return str(url)
+    except TypeError:
+        return None
+
+
+async def search_user(keyword: str):
+    """
+    搜索用户
+    """
+    url = "https://api.bilibili.com/x/web-interface/search/type"
+    data = {"keyword": keyword, "search_type": "bili_user"}
+    resp = await get(url, params=data)
+    logger.debug(resp)
+    return resp
+
+
+async def uid_extract(text: str):
+    logger.debug(f"[UID Extract] Original Text: {text}")
+    b23_msg = await b23_extract(text) if "b23.tv" in text else None
+    message = b23_msg or text
+    logger.debug(f"[UID Extract] b23 extract: {message}")
+    pattern = re.compile("^[0-9]*$|bilibili.com/([0-9]*)")
+    if match := pattern.search(message):
+        logger.debug(f"[UID Extract] Digit or Url: {match}")
+        match = match[1] or match[0]
+        return str(match)
+    elif message.startswith("UID:"):
+        pattern = re.compile("^\\d+")
+        if match := pattern.search(message[4:]):
+            logger.debug(f"[UID Extract] UID: {match}")
+            return str(match[0])
+    else:
+        text_u = text.strip(""""'“”‘’""")
+        if text_u != text:
+            logger.debug(f"[UID Extract] Text is a Quoted Digit: {text_u}")
+        logger.debug(f"[UID Extract] Searching UID in BiliBili: {text_u}")
+        resp = await search_user(text_u)
+        logger.debug(f"[UID Extract] Search result: {resp}")
+        if resp and resp["numResults"]:
+            for result in resp["result"]:
+                if result["uname"] == text_u:
+                    logger.debug(f"[UID Extract] Found User: {result}")
+                    return str(result["mid"])
+        logger.debug("[UID Extract] No User found")
+
+
 async def _guild_admin(bot: Bot, event: GuildMessageEvent):
-    roles = set(
+    roles = {
         role["role_name"]
         for role in (
-            await bot.get_guild_member_profile(
-                guild_id=event.guild_id, user_id=event.user_id
-            )
+            await bot.get_guild_member_profile(guild_id=event.guild_id, user_id=event.user_id)
         )["roles"]
-    )
+    }
     return bool(roles & set(plugin_config.haruka_guild_admin_roles))
 
 
 GUILD_ADMIN: Permission = Permission(_guild_admin)
 
 
 async def permission_check(
@@ -91,17 +157,15 @@
             return
         if await (GUILD_ADMIN | SUPERUSER)(bot, event):
             return
     await bot.send(event, "权限不足，目前只有管理员才能使用")
     raise FinishedException
 
 
-async def group_only(
-    matcher: Matcher, event: PrivateMessageEvent, command: str = RawCommand()
-):
+async def group_only(matcher: Matcher, event: PrivateMessageEvent, command: str = RawCommand()):
     await matcher.finish(f"只有群里才能{command}")
 
 
 def to_me():
     if plugin_config.haruka_to_me:
         from nonebot.rule import to_me
 
@@ -109,14 +173,35 @@
 
     async def _to_me() -> bool:
         return True
 
     return Rule(_to_me)
 
 
+def calc_time_total(t):
+    t = int(t * 1000)
+    if t < 5000:
+        return f"{t} 毫秒"
+
+    timedelta = datetime.timedelta(seconds=t // 1000)
+    day = timedelta.days
+    hour, mint, sec = tuple(int(n) for n in str(timedelta).split(",")[-1].split(":"))
+
+    total = ""
+    if day:
+        total += f"{day} 天 "
+    if hour:
+        total += f"{hour} 小时 "
+    if mint:
+        total += f"{mint} 分钟 "
+    if sec and not day and not hour:
+        total += f"{sec} 秒 "
+    return total
+
+
 async def safe_send(bot_id, send_type, type_id, message, at=False):
     """发送出现错误时, 尝试重新发送, 并捕获异常且不会中断运行"""
 
     async def _safe_send(bot, send_type, type_id, message):
         if send_type == "guild":
             from ..database import DB as db
 
@@ -125,15 +210,15 @@
             result = await bot.send_guild_channel_msg(
                 guild_id=guild.guild_id,
                 channel_id=guild.channel_id,
                 message=message,
             )
         else:
             result = await bot.call_api(
-                "send_" + send_type + "_msg",
+                f"send_{send_type}_msg",
                 **{
                     "message": message,
                     "user_id" if send_type == "private" else "group_id": type_id,
                 },
             )
         return result
 
@@ -185,17 +270,15 @@
         else:
             logger.error(f"推送失败，未知错误，错误信息：{e.info}")
     except NetworkError as e:
         logger.error(f"推送失败，请检查网络连接，错误信息：{e.msg}")
 
 
 async def get_type_id(event: Union[MessageEvent, ChannelDestroyedNoticeEvent]):
-    if isinstance(event, GuildMessageEvent) or isinstance(
-        event, ChannelDestroyedNoticeEvent
-    ):
+    if isinstance(event, (GuildMessageEvent, ChannelDestroyedNoticeEvent)):
         from ..database import DB as db
 
         return await db.get_guild_type_id(event.guild_id, event.channel_id)
     return event.group_id if isinstance(event, GroupMessageEvent) else event.user_id
 
 
 def check_proxy():
```

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/utils/browser.py` & `haruka-bot-1.6.0.post3/haruka_bot/utils/browser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,166 +1,204 @@
 import asyncio
+import contextlib
 import os
 import re
 import sys
 from pathlib import Path
 from typing import Optional
 
 from nonebot.log import logger
 from playwright.__main__ import main
-from playwright.async_api import Browser, async_playwright
+from playwright.async_api import BrowserContext, async_playwright, Page
 
 from ..config import plugin_config
 from .fonts_provider import fill_font
 from .captcha import resolve_captcha
+from ..utils import get_path
 
-_browser: Optional[Browser] = None
+_browser: Optional[BrowserContext] = None
 mobile_js = Path(__file__).parent.joinpath("mobile.js")
 
 
-async def init_browser(proxy=plugin_config.haruka_proxy, **kwargs) -> Browser:
+async def init_browser(proxy=plugin_config.haruka_proxy, **kwargs) -> BrowserContext:
     if proxy:
         kwargs["proxy"] = {"server": proxy}
     global _browser
     p = await async_playwright().start()
-    _browser = await p.chromium.launch(**kwargs)
+    browser_data = Path(get_path("browser"))
+    browser_data.mkdir(parents=True, exist_ok=True)
+    browser_context = await p.chromium.launch_persistent_context(
+        browser_data,
+        user_agent=plugin_config.haruka_browser_ua
+        or (
+            (
+                "Mozilla/5.0 (Linux; Android 10; RMX1911) AppleWebKit/537.36 "
+                "(KHTML, like Gecko) Chrome/100.0.4896.127 Mobile Safari/537.36"
+            )
+            if plugin_config.haruka_screenshot_style.lower() == "mobile"
+            else None
+        ),
+        device_scale_factor=2,
+        **kwargs,
+    )
+    if plugin_config.haruka_screenshot_style.lower() != "mobile":
+        await browser_context.add_cookies(
+            [
+                {
+                    "name": "hit-dyn-v2",
+                    "value": "1",
+                    "domain": ".bilibili.com",
+                    "path": "/",
+                }
+            ]
+        )
+    _browser = browser_context
     return _browser
 
 
-async def get_browser() -> Browser:
+async def get_browser() -> BrowserContext:
     global _browser
-    if _browser is None or not _browser.is_connected():
+    if not _browser or _browser.browser is None or not _browser.browser.is_connected():
         _browser = await init_browser()
     return _browser
 
 
-async def get_dynamic_screenshot(
-    dynamic_id, style=plugin_config.haruka_screenshot_style
-):
+async def get_dynamic_screenshot(dynamic_id, style=plugin_config.haruka_screenshot_style):
     """获取动态截图"""
-    if style.lower() == "mobile":
-        return await get_dynamic_screenshot_mobile(dynamic_id)
-    else:
-        return await get_dynamic_screenshot_pc(dynamic_id)
+    image: Optional[bytes] = None
+    err = ""
+    for i in range(3):
+        browser = await get_browser()
+        page = await browser.new_page()
+        try:
+            # if style.lower() == "mobile":
+            #     page, clip = await get_dynamic_screenshot_mobile(dynamic_id, page)
+            # else:
+            #     page, clip = await get_dynamic_screenshot_pc(dynamic_id, page)
+            page, clip = await get_dynamic_screenshot_mobile(dynamic_id, page)
+            clip["height"] = min(clip["height"], 32766)
+            return (
+                await page.screenshot(clip=clip, full_page=True, type="jpeg", quality=98),
+                err,
+            )
+        except TimeoutError:
+            logger.warning(f"截图超时，重试 {i + 1}/3")
+            err = "截图超时"
+        except Notfound:
+            logger.error(f"动态 {dynamic_id} 不存在")
+            err = "动态不存在"
+        except AssertionError:
+            logger.error(f"动态 {dynamic_id} 截图失败")
+            err = "网页元素获取失败"
+            image = await page.screenshot(full_page=True, type="jpeg", quality=80)
+        except Exception as e:
+            if "bilibili.com/404" in page.url:
+                logger.error(f"动态 {dynamic_id} 不存在")
+                err = "动态不存在"
+                break
+            elif "waiting until" in str(e):
+                logger.error(f"动态 {dynamic_id} 截图超时")
+                err = "截图超时"
+            else:
+                logger.exception(f"动态 {dynamic_id} 截图失败")
+                err = "截图失败"
+                with contextlib.suppress(Exception):
+                    image = await page.screenshot(full_page=True, type="jpeg", quality=80)
+        finally:
+            with contextlib.suppress(Exception):
+                await page.close()
+    return image, err
 
 
-async def get_dynamic_screenshot_mobile(dynamic_id):
+async def get_dynamic_screenshot_mobile(dynamic_id, page: Page):
     """移动端动态截图"""
     url = f"https://m.bilibili.com/dynamic/{dynamic_id}"
-    browser = await get_browser()
-    page = await browser.new_page(
-        device_scale_factor=2,
-        user_agent=(
-            "Mozilla/5.0 (Linux; Android 10; RMX1911) AppleWebKit/537.36 "
-            "(KHTML, like Gecko) Chrome/100.0.4896.127 Mobile Safari/537.36"
-        ),
-        viewport={"width": 460, "height": 780},
-    )
-    try:
-        await page.route(re.compile("^https://static.graiax/fonts/(.+)$"), fill_font)
-        if plugin_config.haruka_captcha_address:
-            page = await resolve_captcha(url, page)
-        else:
-            await page.goto(
-                url,
-                wait_until="networkidle",
-                timeout=plugin_config.haruka_dynamic_timeout * 1000,
-            )
-        # 动态被删除或者进审核了
-        if page.url == "https://m.bilibili.com/404":
-            return None
-        # await page.add_script_tag(
-        #     content=
-        #     # 去除打开app按钮
-        #     "document.getElementsByClassName('m-dynamic-float-openapp').forEach(v=>v.remove());"
-        #     # 去除关注按钮
-        #     "document.getElementsByClassName('dyn-header__following').forEach(v=>v.remove());"
-        #     # 修复字体与换行问题
-        #     "const dyn=document.getElementsByClassName('dyn-card')[0];"
-        #     "dyn.style.fontFamily='Noto Sans CJK SC, sans-serif';"
-        #     "dyn.style.overflowWrap='break-word'"
-        # )
-        await page.add_script_tag(path=mobile_js)
-
-        await page.evaluate(
-            f'setFont("{plugin_config.haruka_dynamic_font}", '
-            f'"{plugin_config.haruka_dynamic_font_source}")'
-            if plugin_config.haruka_dynamic_font
-            else "setFont()"
+    await page.set_viewport_size({"width": 460, "height": 780})
+    await page.route(re.compile("^https://static.graiax/fonts/(.+)$"), fill_font)
+    if plugin_config.haruka_captcha_address:
+        page = await resolve_captcha(url, page)
+    else:
+        await page.goto(
+            url,
+            wait_until="networkidle",
+            timeout=plugin_config.haruka_dynamic_timeout * 1000,
         )
-        await page.wait_for_function("getMobileStyle()")
+    # 动态被删除或者进审核了
+    if page.url == "https://m.bilibili.com/404":
+        raise Notfound
+    # await page.add_script_tag(
+    #     content=
+    #     # 去除打开app按钮
+    #     "document.getElementsByClassName('m-dynamic-float-openapp').forEach(v=>v.remove());"
+    #     # 去除关注按钮
+    #     "document.getElementsByClassName('dyn-header__following').forEach(v=>v.remove());"
+    #     # 修复字体与换行问题
+    #     "const dyn=document.getElementsByClassName('dyn-card')[0];"
+    #     "dyn.style.fontFamily='Noto Sans CJK SC, sans-serif';"
+    #     "dyn.style.overflowWrap='break-word'"
+    # )
+
+    await page.wait_for_load_state(state="domcontentloaded", timeout=20000)
+    if "opus" in page.url:
+        await page.wait_for_selector(".opus-module-author", state="visible")
+    else:
+        await page.wait_for_selector(".dyn-header__author__face", state="visible")
 
-        await page.wait_for_load_state("networkidle")
-        await page.wait_for_load_state("domcontentloaded")
+    await page.add_script_tag(path=mobile_js)
 
-        await page.wait_for_timeout(
-            200 if plugin_config.haruka_dynamic_font_source == "remote" else 50
-        )
+    await page.evaluate(
+        f'setFont("{plugin_config.haruka_dynamic_font}", '
+        f'"{plugin_config.haruka_dynamic_font_source}")'
+        if plugin_config.haruka_dynamic_font
+        else "setFont()"
+    )
+    await page.wait_for_function(
+        f"getMobileStyle({'true' if plugin_config.haruka_dynamic_big_image else 'false'})"
+    )
 
-        # 判断字体是否加载完成
-        need_wait = ["imageComplete", "fontsLoaded"]
-        await asyncio.gather(*[page.wait_for_function(f"{i}()") for i in need_wait])
+    await page.wait_for_load_state("networkidle")
+    await page.wait_for_load_state("domcontentloaded")
 
-        card = await page.query_selector(
-            ".opus-modules" if "opus" in page.url else ".dyn-card"
-        )
-        assert card
-        clip = await card.bounding_box()
-        assert clip
-        return await page.screenshot(clip=clip, full_page=True)
-    except Exception:
-        logger.exception(f"截取动态时发生错误：{url}")
-        return await page.screenshot(full_page=True)
-    finally:
-        await page.close()
+    await page.wait_for_timeout(
+        200 if plugin_config.haruka_dynamic_font_source == "remote" else 50
+    )
+
+    # 判断字体是否加载完成
+    need_wait = ["imageComplete", "fontsLoaded"]
+    await asyncio.gather(*[page.wait_for_function(f"{i}()") for i in need_wait])
+
+    card = await page.query_selector(".opus-modules" if "opus" in page.url else ".dyn-card")
+    assert card
+    clip = await card.bounding_box()
+    assert clip
+    return page, clip
 
 
-async def get_dynamic_screenshot_pc(dynamic_id):
+async def get_dynamic_screenshot_pc(dynamic_id, page: Page):
     """电脑端动态截图"""
     url = f"https://t.bilibili.com/{dynamic_id}"
-    browser = await get_browser()
-    context = await browser.new_context(
-        viewport={"width": 2560, "height": 1080},
-        device_scale_factor=2,
-    )
-    await context.add_cookies(
-        [
-            {
-                "name": "hit-dyn-v2",
-                "value": "1",
-                "domain": ".bilibili.com",
-                "path": "/",
-            }
-        ]
+    await page.set_viewport_size({"width": 2560, "height": 1080})
+    await page.goto(
+        url,
+        wait_until="networkidle",
+        timeout=plugin_config.haruka_dynamic_timeout * 1000,
     )
-    page = await context.new_page()
-    try:
-        await page.goto(
-            url,
-            wait_until="networkidle",
-            timeout=plugin_config.haruka_dynamic_timeout * 1000,
-        )
-        # 动态被删除或者进审核了
-        if page.url == "https://www.bilibili.com/404":
-            return None
-        card = await page.query_selector(".card")
-        assert card
-        clip = await card.bounding_box()
-        assert clip
-        bar = await page.query_selector(".bili-dyn-action__icon")
-        assert bar
-        bar_bound = await bar.bounding_box()
-        assert bar_bound
-        clip["height"] = bar_bound["y"] - clip["y"]
-        return await page.screenshot(clip=clip, full_page=True)
-    except Exception:
-        logger.exception(f"截取动态时发生错误：{url}")
-        return await page.screenshot(full_page=True)
-    finally:
-        await context.close()
+    # 动态被删除或者进审核了
+    if page.url == "https://www.bilibili.com/404":
+        raise Notfound
+    card = await page.query_selector(".card")
+    assert card
+    clip = await card.bounding_box()
+    assert clip
+    bar = await page.query_selector(".bili-dyn-action__icon")
+    assert bar
+    bar_bound = await bar.bounding_box()
+    assert bar_bound
+    clip["height"] = bar_bound["y"] - clip["y"]
+    return page, clip
 
 
 def install():
     """自动安装、更新 Chromium"""
 
     def restore_env():
         del os.environ["PLAYWRIGHT_DOWNLOAD_HOST"]
@@ -197,10 +235,13 @@
     """检查 Playwright 依赖"""
     logger.info("检查 Playwright 依赖")
     try:
         async with async_playwright() as p:
             await p.chromium.launch()
     except Exception:
         raise ImportError(
-            "加载失败，Playwright 依赖不全，"
-            "解决方法：https://haruka-bot.sk415.icu/faq.html#playwright-依赖不全"
+            "加载失败，Playwright 依赖不全，" "解决方法：https://haruka-bot.sk415.icu/faq.html#playwright-依赖不全"
         )
+
+
+class Notfound(Exception):
+    pass
```

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/utils/captcha.py` & `haruka-bot-1.6.0.post3/haruka_bot/utils/captcha.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import contextlib
-from typing import Optional
+from typing import Optional, List
 
 import httpx
 from nonebot.log import logger
 from playwright._impl._api_structures import Position
 from playwright.async_api import Page, Response
 from pydantic import BaseModel
 from yarl import URL
 
 from ..config import plugin_config
 
 
 class CaptchaData(BaseModel):
     captcha_id: str
-    points: list[list[int]]
-    rectangles: list[list[int]]
-    yolo_data: list[list[int]]
+    points: List[List[int]]
+    rectangles: List[List[int]]
+    yolo_data: List[List[int]]
     time: int
 
 
 class CaptchaResponse(BaseModel):
     code: int
     message: str
     data: Optional[CaptchaData]
@@ -93,34 +93,33 @@
                 files={"img_file": captcha_image_body},
             )
             captcha_req = CaptchaResponse(**captcha_req.json())
             logger.debug(f"[Captcha] Get Resolve Result: {captcha_req}")
             assert captcha_req.data
             last_captcha_id = captcha_req.data.captcha_id
         if captcha_req.data:
-            click_points: list[list[int]] = captcha_req.data.points
+            click_points: List[List[int]] = captcha_req.data.points
             logger.warning(f"[Captcha] 识别到 {len(click_points)} 个坐标，正在点击")
             # 根据原图大小和截图大小计算缩放比例，然后计算出正确的需要点击的位置
             for point in click_points:
                 real_click_points = {
                     "x": point[0] * captcha_size["width"] / origin_image_size[0],
                     "y": point[1] * captcha_size["height"] / origin_image_size[1],
                 }
                 await captcha_image.click(position=Position(**real_click_points))
                 await page.wait_for_timeout(800)
-            captcha_image_body = ""
             await page.click("text=确认")
             geetest_up = await page.wait_for_selector(".geetest_up", state="visible")
             if not geetest_up:
                 logger.warning("[Captcha] 未检测到验证码验证结果，正在重试")
                 continue
             geetest_result = await geetest_up.text_content()
             assert geetest_result
             logger.debug(f"[Captcha] Geetest result: {geetest_result}")
             if "验证成功" in geetest_result:
                 logger.success("[Captcha] 极验网页 Tip 验证成功")
-                await page.wait_for_timeout(1000)
-                await page.wait_for_load_state("domcontentloaded")
+                captcha_image_body = ""
+                await page.wait_for_timeout(2000)
             else:
                 logger.warning("[Captcha] 极验验证失败，正在重试")
 
     return page
```

### Comparing `haruka-bot-1.6.0.post2/haruka_bot/utils/fonts_provider.py` & `haruka-bot-1.6.0.post3/haruka_bot/utils/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post2/pyproject.toml` & `haruka-bot-1.6.0.post3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 keywords = [
     "nonebot",
     "nonebot2",
     "qqbot",
     "bilibili",
     "bot",
 ]
-version = "1.6.0.post2"
+version = "1.6.0.post3"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.urls]
 homepage = "https://github.com/SK-415/HarukaBot"
 repository = "https://github.com/SK-415/HarukaBot/tree/master/src/plugins/haruka_bot"
@@ -54,14 +54,15 @@
 [tool.nonebot]
 adapters = [
     { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" },
 ]
 plugins = [
     "haruka_bot",
     "nonebot_plugin_gocqhttp",
+    "nonebot_plugin_guild_patch",
 ]
 plugin_dirs = []
 builtin_plugins = []
 
 [build-system]
 requires = [
     "pdm-pep517>=1.0.0",
```

### Comparing `haruka-bot-1.6.0.post2/PKG-INFO` & `haruka-bot-1.6.0.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka-bot
-Version: 1.6.0.post2
+Version: 1.6.0.post3
 Summary: Push dynamics and live informations from bilibili to QQ. Based on nonebot2.
 License: AGPL-3.0-or-later
 Keywords: nonebot,nonebot2,qqbot,bilibili,bot
 Author-email: SK-415 <2967923486@qq.com>
 Requires-Python: >=3.8,<4.0
 Project-URL: documentation, https://github.com/SK-415/HarukaBot#readme
 Project-URL: homepage, https://github.com/SK-415/HarukaBot
```

