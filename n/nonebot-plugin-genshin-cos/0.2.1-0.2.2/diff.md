# Comparing `tmp/nonebot_plugin_genshin_cos-0.2.1.tar.gz` & `tmp/nonebot_plugin_genshin_cos-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshin_cos-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshin_cos-0.2.2.tar", max compression
```

## Comparing `nonebot_plugin_genshin_cos-0.2.1.tar` & `nonebot_plugin_genshin_cos-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-06-29 07:37:38.097162 nonebot_plugin_genshin_cos-0.2.1/LICENSE
--rw-r--r--   0        0        0     3830 2023-06-29 07:37:38.097162 nonebot_plugin_genshin_cos-0.2.1/README.md
--rw-r--r--   0        0        0    13815 2023-06-29 07:37:38.097162 nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/__init__.py
--rw-r--r--   0        0        0      223 2023-06-29 07:37:38.097162 nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/config.py
--rw-r--r--   0        0        0   459180 2023-06-29 07:37:38.101162 nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
--rw-r--r--   0        0        0    12330 2023-06-29 07:37:38.101162 nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/hoyospider.py
--rw-r--r--   0        0        0     3902 2023-06-29 07:37:38.101162 nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/utils.py
--rw-r--r--   0        0        0      612 2023-06-29 07:37:38.101162 nonebot_plugin_genshin_cos-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4705 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-29 11:26:08.100934 nonebot_plugin_genshin_cos-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3973 2023-06-29 11:26:08.100934 nonebot_plugin_genshin_cos-0.2.2/README.md
+-rw-r--r--   0        0        0    13942 2023-06-29 11:26:08.100934 nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-29 11:26:08.100934 nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/config.py
+-rw-r--r--   0        0        0   459180 2023-06-29 11:26:08.104934 nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
+-rw-r--r--   0        0        0    12330 2023-06-29 11:26:08.104934 nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/hoyospider.py
+-rw-r--r--   0        0        0     4931 2023-06-29 11:26:08.104934 nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/utils.py
+-rw-r--r--   0        0        0      612 2023-06-29 11:26:08.104934 nonebot_plugin_genshin_cos-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4848 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_genshin_cos-0.2.1/LICENSE` & `nonebot_plugin_genshin_cos-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.2.1/README.md` & `nonebot_plugin_genshin_cos-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -74,14 +74,16 @@
 ### 在env.中添加以下配置
 
 | 配置 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:---:|
 |cos_max|int|5|最大返回cos图片数量|
 |cos_path|str|无|不配置则默认下载到bot根目录的`"data/genshin_cos"`,支持绝对路劲如`"C:/Users/image"`和相对bot根目录路劲如`"coser/image"`
 |cos_cd|int|30|用户触发cd|
+|cos_forward_msg|bool|True|默认是否合并转发|
+|cos_delay|float|0.5|当上面的配置项为`False`时，发送图片的每张延迟s|
 
 > 注意：绝对路劲中用`/`，用`\`可能会被转义
 
 ## ⭐ 使用
 
 ### 指令：
 | 指令 | 需要@ | 范围 | 说明 |权限|
@@ -100,16 +102,18 @@
 
 ## 🌙 未来
  - [x] 缓慢更新，最近学业繁忙哦~
  - [x] 随机发送cos图片
  - [x] 保存cos图
  - [x] 内置cd和用户触发上限
  - [x] 合并转发发送多张cos图
+
 ~~playwright获取cos图~~
 ~~选择发送图库方式：离线 (迅速) or 在线（缓慢、目前是的）~~
+
  - [x] 支持米游社其他社区cos获取
  - [x] 支持每日推送热榜的cos图
 
 --- 喜欢记得点个star⭐---
 
 ## ❗免责声明
```

#### html2text {}

```diff
@@ -18,17 +18,20 @@
 æ¨èéåç«ä¸è½½ æ¸åæº```https://pypi.tuna.tsinghua.edu.cn/simple```
 é¿éæº```https://mirrors.aliyun.com/pypi/simple/```  ## âï¸ éç½® ###
 å¨env.ä¸­æ·»å ä»¥ä¸éç½® | éç½® | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:
 |:----:|:----:|:---:| |cos_max|int|5|æå¤§è¿åcoså¾çæ°é|
 |cos_path|str|æ |ä¸éç½®åé»è®¤ä¸è½½å°botæ ¹ç®å½ç`"data/
 genshin_cos"`,æ¯æç»å¯¹è·¯å²å¦`"C:/Users/
 image"`åç¸å¯¹botæ ¹ç®å½è·¯å²å¦`"coser/image"`
-|cos_cd|int|30|ç¨æ·è§¦åcd| > æ³¨æï¼ç»å¯¹è·¯å²ä¸­ç¨`/
-`ï¼ç¨`\`å¯è½ä¼è¢«è½¬ä¹ ## â­ ä½¿ç¨ ### æä»¤ï¼ | æä»¤ | éè¦@ |
-èå´ | è¯´æ |æé| |:-----:|:----:|:----:|:----:|:----:
+|cos_cd|int|30|ç¨æ·è§¦åcd|
+|cos_forward_msg|bool|True|é»è®¤æ¯å¦åå¹¶è½¬å|
+|cos_delay|float|0.5|å½ä¸é¢çéç½®é¡¹ä¸º`False`æ¶ï¼åéå¾ççæ¯å¼ å»¶è¿s|
+> æ³¨æï¼ç»å¯¹è·¯å²ä¸­ç¨`/`ï¼ç¨`\`å¯è½ä¼è¢«è½¬ä¹ ## â­ ä½¿ç¨ ###
+æä»¤ï¼ | æä»¤ | éè¦@ | èå´ | è¯´æ |æé| |:-----:|:----:|:----:
+|:----:|:----:
 |
 |ä¸è½½cos|å¦|ç¾¤èãç§è|ä¸è½½ç­é¨coså¾|è¶ç®¡ãç¾¤ä¸»ãç®¡çå|
 |ç­é¨cos|å¦|åä¸|è·åæå®æ¸¸æç­é¨coså¾ï¼å¦`ç­é¨cos åç¥
 x3`|å¨é¨|
 |æ¥ãå¨ãææ¦cos|å¦|åä¸|è·åæè¡æ¦coså¾ãå¦`æ¥æ¦cos åç¥
 x3`|å¨é¨|
 |ææ°cos|å¦|åä¸|åä¸é¢å·®ä¸å¤ï¼ä¸åäºï¼å¼å¼|å¨é¨|
```

### Comparing `nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/__init__.py` & `nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
 logger.opt(colors=True).info(logo)
 
 #用户cd数据
 user_data = {}
 CONFIG: Dict[str, Dict[str,str]] = {'原神':{},'崩坏3':{},'大别野':{},'星穹铁道':{}}
 DRIVER = get_driver()
+
 # 读取配置文件
 config_path = Path("config/genshincos.json")
 config_path.parent.mkdir(parents=True, exist_ok=True)
 if config_path.exists():
     with open(config_path, "r", encoding="utf8") as f:
         CONFIG = json.load(f)
 else:
@@ -206,15 +207,15 @@
     elif args[0] in STAR_RAIL:
         await good_cos.finish("星穹铁道暂不支持精品cos")
     else:
         await good_cos.finish("暂不支持该类型")
     await send_images(bot,matcher,args,event,send_type)
 
 
-@download_cos.got('game_type', prompt='你想下载哪种类型的,有原神和大别野,崩坏3')
+@download_cos.got('game_type', prompt='你想下载哪种类型的,有原神和大别野,崩坏3,星穹铁道')
 async def got_type(game_type: str = ArgPlainText()):
     if game_type in GENSHIN_NAME:
         hot = genshin_hot
     elif game_type in DBY_NAME:
         hot = dbycos_hot
     elif game_type in HONKAI3RD_NAME:
         hot = honkai3rd_hot
@@ -225,15 +226,15 @@
         await download_cos.finish(f'没有找到{game_type}的cos图片')
     else:
         await download_cos.send(f'正在下载{game_type}的cos图片')
         try:
             await download_from_urls(image_urls, SAVE_PATH / f'{game_type}cos')
             await download_cos.finish(f'已成功保存{len(image_urls)}张{game_type}的cos图片')
         except WriteError as e:
-            await download_cos.finish(f'保存{game_type}的cos图片失败,原因:{e}')
+            await download_cos.finish(f'保存部分{game_type}的cos图片失败,原因:{e}')
 
 ###########################################################################################
 
 #定时任务
 async def aps_send(aps_goup_id: str):
     logger.debug("正在发送定时推送")
     bot: Bot = get_bot()
@@ -296,15 +297,18 @@
             num = num if num <= MAX else MAX
             msg_list = [f'✅找到最新的一些{args[0]}图如下:✅']
             image_list = await send_type.async_get_urls()
             if num > len(image_list):
                 await matcher.finish(f"最多只能获取{len(image_list)}张图片", at_sender=True)
             for i in range(num):
                 msg_list.append(MessageSegment.image(image_list[i]))
-            await send_forward_msg(bot, event, "米游社cos", bot.self_id, msg_list)
+            if IS_FORWARD:
+                await send_forward_msg(bot, event, "米游社cos", bot.self_id, msg_list)
+            else:
+                await send_regular_msg(matcher, msg_list)
     else:
         await matcher.finish(f"cd冷却中,还剩{deletime}秒", at_sender=True)
 
 @DRIVER.on_startup
 async def start_aps():
     try:
         if scheduler == None:
```

### Comparing `nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF` & `nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/hoyospider.py` & `nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/hoyospider.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,18 +369,18 @@
 honkai3rd_latest_comment = Latest(ForumType.Honkai3rdPic, LatestType.LatestComment)
 
 dby_rank_daily = Rank(ForumType.DBYPIC, RankType.Daily)
 dby_hot = Hot(ForumType.DBYPIC)
 dby_good = Good(ForumType.DBYPIC)
 dby_latest_comment = Latest(ForumType.DBYPIC, LatestType.LatestComment)
 
-starrail_rank_daily = Rank(ForumType.StarRailPic, RankType.Daily)
-starrail_hot = Hot(ForumType.StarRailPic)
-starrail_good = Good(ForumType.StarRailPic)
-starrail_latest_comment = Latest(ForumType.StarRailPic, LatestType.LatestComment)
+starrail_rank_daily = Rank(ForumType.StarRailCos, RankType.Daily)
+starrail_hot = Hot(ForumType.StarRailCos)
+starrail_good = Good(ForumType.StarRailCos)
+starrail_latest_comment = Latest(ForumType.StarRailCos, LatestType.LatestComment)
 
 honkai2_rank_daily = Rank(ForumType.Honkai2Pic, RankType.Daily)
 honkai2_hot = Hot(ForumType.Honkai2Pic)
 honkai2_good = Good(ForumType.Honkai2Pic)
 honkai2_latest_comment = Latest(ForumType.Honkai2Pic, LatestType.LatestComment)
 
 dbycos_rank_daily = Rank(ForumType.DBYCOS, RankType.Daily)
```

### Comparing `nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/utils.py` & `nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,34 +3,39 @@
 from .config import Config
 from typing import Dict, List, Tuple
 from datetime import datetime, timedelta
 from httpx import TimeoutException
 import httpx
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent, Message, GROUP_ADMIN, GROUP_OWNER
 from nonebot.permission import SUPERUSER
+from nonebot.matcher import Matcher
+from nonebot.log import logger
+from nonebot.exception import ActionFailed
+from asyncio import sleep
 #######################################################
 
 # 拓展的异常类和函数
 SUPER_PERMISSION = GROUP_ADMIN | GROUP_OWNER | SUPERUSER
 GENSHIN_NAME = ["原神",'OP','op','欧泡','⭕','🅾️','🅾️P','🅾️p','原','圆']
 HONKAI3RD_NAME = ['崩坏3', '崩崩崩', '蹦蹦蹦','崩坏三','崩三','崩崩崩三','崩坏3rd','崩坏3Rd','崩坏3RD','崩坏3rd','崩坏3RD','崩坏3Rd']
 DBY_NAME = ['大别野','DBY','dby']
 STAR_RAIL = ['星穹铁道','星穹','崩铁','铁道','星铁','穹p','穹铁']
 
 class WriteError(Exception):
     """写入错误"""
-    def __init__(self):
-        super().__init__('写入错误')
+    pass
 
 
 # 加载配置
 
 MAX = Config.parse_obj(get_driver().config.dict()).cos_max
 SAVE_PATH = Path(Config.parse_obj(get_driver().config.dict()).cos_path)
 CD = Config.parse_obj(get_driver().config.dict()).cos_cd
+DELAY = Config.parse_obj(get_driver().config.dict()).cos_delay
+IS_FORWARD = Config.parse_obj(get_driver().config.dict()).cos_forward_msg
 
 
 def check_cd(user_id: int, user_data: Dict[str, datetime]) -> Tuple[bool, int, dict]:
     """检查用户触发事件的cd
 
     Args:
         user_id (int): 用户的id
@@ -53,27 +58,38 @@
 async def download_from_urls(urls: List[str], path: Path):
     '''
     下载图片
     :param urls: 图片链接
     :param path: 保存路径
     :return: None
     '''
-    if not path.parent.exists():
-        path.parent.mkdir(parents=True)
+    is_download_error = False
+    error_cnt = 0
+    success_cnt = 0
+    if not path.exists():
+        path.mkdir(parents=True)
+    if not path.is_dir():
+        raise WriteError('路径不是文件夹')
     async with httpx.AsyncClient() as client:
         for url in urls:
             try:
                 filename = url.split('/')[-1]
                 new_path = path / filename
                 rsp = await client.get(url)
                 content = rsp.content
                 with open(new_path, 'wb') as f:
                     f.write(content)
-            except (IndexError, IOError, httpx.ConnectError, httpx.RequestError, httpx.ReadTimeout, TimeoutException):
-                raise WriteError('下载失败')
+            except (httpx.ConnectError, httpx.RequestError, httpx.ReadTimeout, TimeoutException):
+                is_download_error = True
+                error_cnt += 1
+                continue
+            if is_download_error:
+                raise WriteError(f'有{error_cnt}张图片由于超时下载失败了')
+            success_cnt += 1
+            logger.success(f'下载{success_cnt}张成功')
 
 
 async def send_forward_msg(
     bot: Bot,
     event: MessageEvent,
     name: str,
     uin: str,
@@ -111,8 +127,24 @@
         name: 发送者昵称
         uin: 发送者账号
         msgs: 消息列表
     """
     def to_json(msg: Message):
         return {"type": "node", "data": {"name": name, "uin": uin, "content": msg}}
 
-    return [to_json(msg) for msg in msgs]        
+    return [to_json(msg) for msg in msgs]   
+
+async def send_regular_msg(matcher: Matcher,messages:list):
+    '''
+    发送常规消息
+    :param matcher: Matcher
+    :param messages: 消息列表
+    '''
+    cnt = 1
+    for msg in messages:
+        try:
+            cnt += 1
+            await matcher.send(msg)
+            await sleep(DELAY)
+        except ActionFailed:
+            if cnt <= 2:
+                await matcher.send('消息可能风控,请尝试更改为合并转发模式')
```

### Comparing `nonebot_plugin_genshin_cos-0.2.1/pyproject.toml` & `nonebot_plugin_genshin_cos-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-genshin-cos"
-version = "0.2.1"
+version = "0.2.2"
 description = "米游社原神cos图获取"
 authors = ["Cvandia <106718176+Cvandia@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_genshin_cos"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_genshin_cos-0.2.1/PKG-INFO` & `nonebot_plugin_genshin_cos-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshin-cos
-Version: 0.2.1
+Version: 0.2.2
 Summary: 米游社原神cos图获取
 License: MIT
 Author: Cvandia
 Author-email: 106718176+Cvandia@users.noreply.github.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -98,14 +98,16 @@
 ### 在env.中添加以下配置
 
 | 配置 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:---:|
 |cos_max|int|5|最大返回cos图片数量|
 |cos_path|str|无|不配置则默认下载到bot根目录的`"data/genshin_cos"`,支持绝对路劲如`"C:/Users/image"`和相对bot根目录路劲如`"coser/image"`
 |cos_cd|int|30|用户触发cd|
+|cos_forward_msg|bool|True|默认是否合并转发|
+|cos_delay|float|0.5|当上面的配置项为`False`时，发送图片的每张延迟s|
 
 > 注意：绝对路劲中用`/`，用`\`可能会被转义
 
 ## ⭐ 使用
 
 ### 指令：
 | 指令 | 需要@ | 范围 | 说明 |权限|
@@ -124,16 +126,18 @@
 
 ## 🌙 未来
  - [x] 缓慢更新，最近学业繁忙哦~
  - [x] 随机发送cos图片
  - [x] 保存cos图
  - [x] 内置cd和用户触发上限
  - [x] 合并转发发送多张cos图
+
 ~~playwright获取cos图~~
 ~~选择发送图库方式：离线 (迅速) or 在线（缓慢、目前是的）~~
+
  - [x] 支持米游社其他社区cos获取
  - [x] 支持每日推送热榜的cos图
 
 --- 喜欢记得点个star⭐---
 
 ## ❗免责声明
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.2.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.2.2 Summary:
 ç±³æ¸¸ç¤¾åç¥coså¾è·å License: MIT Author: Cvandia Author-email:
 106718176+Cvandia@users.noreply.github.com Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.7.0) Requires-Dist: httpx (>=0.19.0) Requires-
@@ -30,17 +30,20 @@
 æ¨èéåç«ä¸è½½ æ¸åæº```https://pypi.tuna.tsinghua.edu.cn/simple```
 é¿éæº```https://mirrors.aliyun.com/pypi/simple/```  ## âï¸ éç½® ###
 å¨env.ä¸­æ·»å ä»¥ä¸éç½® | éç½® | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:
 |:----:|:----:|:---:| |cos_max|int|5|æå¤§è¿åcoså¾çæ°é|
 |cos_path|str|æ |ä¸éç½®åé»è®¤ä¸è½½å°botæ ¹ç®å½ç`"data/
 genshin_cos"`,æ¯æç»å¯¹è·¯å²å¦`"C:/Users/
 image"`åç¸å¯¹botæ ¹ç®å½è·¯å²å¦`"coser/image"`
-|cos_cd|int|30|ç¨æ·è§¦åcd| > æ³¨æï¼ç»å¯¹è·¯å²ä¸­ç¨`/
-`ï¼ç¨`\`å¯è½ä¼è¢«è½¬ä¹ ## â­ ä½¿ç¨ ### æä»¤ï¼ | æä»¤ | éè¦@ |
-èå´ | è¯´æ |æé| |:-----:|:----:|:----:|:----:|:----:
+|cos_cd|int|30|ç¨æ·è§¦åcd|
+|cos_forward_msg|bool|True|é»è®¤æ¯å¦åå¹¶è½¬å|
+|cos_delay|float|0.5|å½ä¸é¢çéç½®é¡¹ä¸º`False`æ¶ï¼åéå¾ççæ¯å¼ å»¶è¿s|
+> æ³¨æï¼ç»å¯¹è·¯å²ä¸­ç¨`/`ï¼ç¨`\`å¯è½ä¼è¢«è½¬ä¹ ## â­ ä½¿ç¨ ###
+æä»¤ï¼ | æä»¤ | éè¦@ | èå´ | è¯´æ |æé| |:-----:|:----:|:----:
+|:----:|:----:
 |
 |ä¸è½½cos|å¦|ç¾¤èãç§è|ä¸è½½ç­é¨coså¾|è¶ç®¡ãç¾¤ä¸»ãç®¡çå|
 |ç­é¨cos|å¦|åä¸|è·åæå®æ¸¸æç­é¨coså¾ï¼å¦`ç­é¨cos åç¥
 x3`|å¨é¨|
 |æ¥ãå¨ãææ¦cos|å¦|åä¸|è·åæè¡æ¦coså¾ãå¦`æ¥æ¦cos åç¥
 x3`|å¨é¨|
 |ææ°cos|å¦|åä¸|åä¸é¢å·®ä¸å¤ï¼ä¸åäºï¼å¼å¼|å¨é¨|
```

