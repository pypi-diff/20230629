# Comparing `tmp/nonebot_plugin_genshin_cos-0.2.0.tar.gz` & `tmp/nonebot_plugin_genshin_cos-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshin_cos-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshin_cos-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_genshin_cos-0.2.0.tar` & `nonebot_plugin_genshin_cos-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1085 2023-03-28 09:06:05.557316 nonebot_plugin_genshin_cos-0.2.0/LICENSE
--rw-r--r--   0        0        0    14359 2023-06-28 07:36:48.597725 nonebot_plugin_genshin_cos-0.2.0/nonebot_plugin_genshin_cos/__init__.py
--rw-r--r--   0        0        0      230 2023-06-28 07:41:10.710745 nonebot_plugin_genshin_cos-0.2.0/nonebot_plugin_genshin_cos/config.py
--rw-r--r--   0        0        0   459180 2023-06-05 05:24:06.718316 nonebot_plugin_genshin_cos-0.2.0/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
--rw-r--r--   0        0        0    11088 2023-06-28 04:58:44.275589 nonebot_plugin_genshin_cos-0.2.0/nonebot_plugin_genshin_cos/hoyospider.py
--rw-r--r--   0        0        0     4019 2023-06-28 11:15:13.406876 nonebot_plugin_genshin_cos-0.2.0/nonebot_plugin_genshin_cos/utils.py
--rw-r--r--   0        0        0      636 2023-06-28 11:14:48.437590 nonebot_plugin_genshin_cos-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3882 2023-06-27 09:24:22.854792 nonebot_plugin_genshin_cos-0.2.0/README.md
--rw-r--r--   0        0        0     4635 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-29 07:37:38.097162 nonebot_plugin_genshin_cos-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3830 2023-06-29 07:37:38.097162 nonebot_plugin_genshin_cos-0.2.1/README.md
+-rw-r--r--   0        0        0    13815 2023-06-29 07:37:38.097162 nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/__init__.py
+-rw-r--r--   0        0        0      223 2023-06-29 07:37:38.097162 nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/config.py
+-rw-r--r--   0        0        0   459180 2023-06-29 07:37:38.101162 nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
+-rw-r--r--   0        0        0    12330 2023-06-29 07:37:38.101162 nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/hoyospider.py
+-rw-r--r--   0        0        0     3902 2023-06-29 07:37:38.101162 nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/utils.py
+-rw-r--r--   0        0        0      612 2023-06-29 07:37:38.101162 nonebot_plugin_genshin_cos-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4705 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_genshin_cos-0.2.0/LICENSE` & `nonebot_plugin_genshin_cos-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 divandia
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 divandia
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `nonebot_plugin_genshin_cos-0.2.0/nonebot_plugin_genshin_cos/__init__.py` & `nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,328 +1,327 @@
-from nonebot.adapters.onebot.v11 import (
-    Bot,
-    Message,
-    MessageEvent,
-    MessageSegment,
-    GroupMessageEvent
-)
-from nonebot.plugin import on_regex, on_command, require, PluginMetadata
-from nonebot.params import RegexGroup, ArgPlainText, CommandArg
-from nonebot.typing import T_State
-from nonebot.log import logger
-from nonebot import get_driver, get_bot
-from nonebot.matcher import Matcher
-from nonebot.exception import ActionFailed
-from typing import Tuple, Any
-from random import choice
-from datetime import datetime
-from .config import Config
-from .utils import *
-from .hoyospider import *
-try:
-    scheduler = require("nonebot_plugin_apscheduler").scheduler
-except:
-    scheduler = None
-try:
-    import ujson as json
-except ModuleNotFoundError:
-    import json
-import asyncio
-import re
-
-__plugin_meta__ = PluginMetadata(
-    name="米游社cos",
-    description="获取原神coser图片",
-    config=Config,
-    usage="原神cos,CosPlus,下载cos",
-    type="application",
-    homepage="https://github.com/Cvandia/nonebot_plugin_genshin_cos",
-    supported_adapters={"~onebot.v11"},
-    extra={
-        "unique_name": "genshin_cos",
-        "example": "保存cos:保存cos图片至本地文件",
-        "author": "divandia <106718176+Cvandia@users.noreply.github.com>",
-        "version": "0.2.0",
-    }
-)
-logo = """<g>
-  /$$$$$$                                /$$       /$$                  /$$$$$$                     
- /$$__  $$                              | $$      |__/                 /$$__  $$                    
-| $$  \__/  /$$$$$$  /$$$$$$$   /$$$$$$$| $$$$$$$  /$$ /$$$$$$$       | $$  \__/  /$$$$$$   /$$$$$$$
-| $$ /$$$$ /$$__  $$| $$__  $$ /$$_____/| $$__  $$| $$| $$__  $$      | $$       /$$__  $$ /$$_____/
-| $$|_  $$| $$$$$$$$| $$  \ $$|  $$$$$$ | $$  \ $$| $$| $$  \ $$      | $$      | $$  \ $$|  $$$$$$ 
-| $$  \ $$| $$_____/| $$  | $$ \____  $$| $$  | $$| $$| $$  | $$      | $$    $$| $$  | $$ \____  $$
-|  $$$$$$/|  $$$$$$$| $$  | $$ /$$$$$$$/| $$  | $$| $$| $$  | $$      |  $$$$$$/|  $$$$$$/ /$$$$$$$/
- \______/  \_______/|__/  |__/|_______/ |__/  |__/|__/|__/  |__/       \______/  \______/ |_______/ 
- </g>"""
-
-
-logger.opt(colors=True).info(logo)
-
-#用户cd数据
-user_data = {}
-CONFIG: Dict[str, Dict[str,str]] = {'原神':{},'崩坏3':{},'大别野':{},'星穹铁道':{}}
-DRIVER = get_driver()
-# 读取配置文件
-config_path = Path("config/genshincos.json")
-config_path.parent.mkdir(parents=True, exist_ok=True)
-if config_path.exists():
-    with open(config_path, "r", encoding="utf8") as f:
-        CONFIG = json.load(f)
-else:
-    with open(config_path, "w", encoding="utf8") as f:
-        json.dump(CONFIG, f, ensure_ascii=False, indent=4)
-
-#事件响应器
-download_cos = on_command('下载cos', aliases={'cos保存', '保存cos'}, block=False, priority=5, permission=SUPER_PERMISSION)
-hot_cos = on_command('热门cos', aliases={'热门coser', '热门cos图'}, block=False, priority=5)
-rank_cos = on_regex(r'^(日|月|周)榜cos[r]?[图]?(.+)?',priority=5, block=False, flags=re.I)
-latest_cos = on_command('最新cos', aliases={'最新coser', '最新cos图'}, block=False, priority=5)
-good_cos = on_command('精品cos', aliases={'精品coser', '精品cos图'}, block=False, priority=5)
-turn_aps = on_regex(r'^(开启|关闭)每日推送(原神|崩坏3|星穹铁道|大别野)(\s)?(.+)?', block=False, priority=5, flags=re.I, permission=SUPER_PERMISSION)
-show_aps = on_command('查看本群推送', aliases={'查看推送','查看订阅'}, block=False, priority=5)
-
-@show_aps.handle()
-async def _(bot: Bot, event: GroupMessageEvent):
-    send_msg = '本群订阅的推送有:\n'
-    for game_type, dict in CONFIG.items():
-        if game_type == "": continue
-        for goup_id, time in dict.items():
-            if str(event.group_id) == goup_id:
-                send_msg += f"{game_type}的每日{time}推送\n"
-    await show_aps.finish(send_msg)
-
-
-@turn_aps.handle()
-async def _(event: GroupMessageEvent, args: Tuple[Any, ...] = RegexGroup()):
-    # 检查是否安装了apscheduler插件，并且是否开启了定时推送
-    if scheduler == None:
-        await turn_aps.finish("未安装apscheduler插件,无法使用此功能")
-    mode = args[0] 
-    game_type = args[1]
-    time = args[3]
-    group_id = str(event.group_id)
-    MyConfig = CONFIG.copy()
-    if mode == "开启":
-        for name in MyConfig.keys():
-            if name == game_type:
-                if group_id in MyConfig[name].keys():
-                    await turn_aps.finish("该群已开启,无需重复开启")
-                elif not time:
-                    await turn_aps.finish("请指定推送时间")
-                else:
-                    CONFIG[name][group_id] = time
-                    try:
-                        scheduler.add_job(aps_send, trigger="cron", hour=time.split(":")[0], minute=time.split(":")[1], id=f"{game_type}{group_id}")
-                        logger.debug(f"已成功添加{group_id}的{game_type}定时推送")
-                        scheduler.start()
-                    except Exception as e:
-                        logger.error(e)
-    else:
-        for name in MyConfig.keys():
-            if name == game_type:
-                if group_id in MyConfig[name].keys():
-                    CONFIG[name].pop(group_id)
-                    try:
-                        scheduler.remove_job(f"{game_type}{group_id}")
-                    except Exception as e:
-                        logger.error(e)
-                        continue
-                else:
-                    await turn_aps.finish("该群已关闭,无需重复关闭")
-    with open(config_path, "w", encoding="utf8") as f:
-        f.write(json.dumps(CONFIG, ensure_ascii=False, indent=4))
-    await turn_aps.finish(f"已成功{mode}{group_id}的{game_type}定时推送")
-
-
-@hot_cos.handle()
-async def _(bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()):
-    if not arg:
-        await hot_cos.finish("请指定cos类型")
-    args = arg.extract_plain_text().split()
-    if args[0] in GENSHIN_NAME:
-        send_type = Hot(ForumType.GenshinCos)
-    elif args[0] in HONKAI3RD_NAME:
-        send_type = Hot(ForumType.Honkai3rdPic)
-    elif args[0] in DBY_NAME:
-        send_type = Hot(ForumType.DBYCOS)
-    elif args[0] in STAR_RAIL:
-        send_type = Hot(ForumType.StarRailCos)
-    else:
-        await hot_cos.finish("暂不支持该类型")
-    await send_images(bot,matcher,args,event,send_type)
-
-@rank_cos.handle()
-async def _(bot: Bot, matcher: Matcher, event: MessageEvent, group: Tuple[str, ...] = RegexGroup()):
-    if not group[1]:
-        await rank_cos.finish("请指定cos类型")
-    args = group[1].split()
-    if group[0] == "日":
-        rank_type = RankType.Daily
-    elif group[0] == "周":
-        rank_type = RankType.Weekly
-    elif group[0] == "月":
-        rank_type = RankType.Monthly
-
-    if args[0] in GENSHIN_NAME:
-        send_type = Rank(ForumType.GenshinCos, rank_type)
-    elif args[0] in HONKAI3RD_NAME:
-        send_type = Rank(ForumType.Honkai3rdPic, rank_type)
-    elif args[0] in DBY_NAME:
-        send_type = Rank(ForumType.DBYCOS, rank_type)
-    elif args[0] in STAR_RAIL:
-        send_type = Rank(ForumType.StarRailCos, rank_type)
-    else:
-        await rank_cos.finish("暂不支持该类型")
-    await send_images(bot,matcher,args,event,send_type)
-
-@latest_cos.handle()
-async def _(bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()):
-    if not arg:
-        await latest_cos.finish("请指定cos类型")
-    args = arg.extract_plain_text().split()
-    if args[0] in GENSHIN_NAME:
-        send_type = Latest(ForumType.GenshinCos, LatestType.LatestComment)
-    elif args[0] in HONKAI3RD_NAME:
-        send_type = Latest(ForumType.Honkai3rdPic, LatestType.LatestComment)
-    elif args[0] in DBY_NAME:
-        send_type = Latest(ForumType.DBYCOS, LatestType.LatestComment)
-    elif args[0] in STAR_RAIL:
-        send_type = Latest(ForumType.StarRailCos, LatestType.LatestComment)
-    else:
-        await latest_cos.finish("暂不支持该类型")
-    await send_images(bot,matcher,args,event,send_type)
-
-@good_cos.handle()
-async def _(bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()):
-    if not arg:
-        await good_cos.finish("请指定cos类型")
-    args = arg.extract_plain_text().split()
-    if args[0] in GENSHIN_NAME:
-        await good_cos.finish("原神暂不支持精品cos")
-    elif args[0] in HONKAI3RD_NAME:
-        send_type = Good(ForumType.Honkai3rdPic)
-    elif args[0] in DBY_NAME:
-        send_type = Good(ForumType.DBYCOS)
-    elif args[0] in STAR_RAIL:
-        await good_cos.finish("星穹铁道暂不支持精品cos")
-    else:
-        await good_cos.finish("暂不支持该类型")
-    await send_images(bot,matcher,args,event,send_type)
-
-
-@download_cos.got('game_type', prompt='你想下载哪种类型的,有原神和大别野,崩坏3')
-async def got_type(game_type: str = ArgPlainText()):
-    if game_type in GENSHIN_NAME:
-        hot = Hot(ForumType.GenshinCos)
-    elif game_type in DBY_NAME:
-        hot = Hot(ForumType.DBYCOS)
-    elif game_type in HONKAI3RD_NAME:
-        hot = Hot(ForumType.Honkai3rdPic)
-    elif game_type in STAR_RAIL:
-        hot = Hot(ForumType.StarRailCos)
-    image_urls = await hot.async_get_urls()
-    if not image_urls:
-        await download_cos.finish(f'没有找到{game_type}的cos图片')
-    else:
-        await download_cos.send(f'正在下载{game_type}的cos图片')
-        try:
-            await download_from_urls(image_urls, SAVE_PATH / f'{game_type}cos')
-            await download_cos.finish(f'已成功保存{len(image_urls)}张{game_type}的cos图片')
-        except WriteError as e:
-            await download_cos.finish(f'保存{game_type}的cos图片失败,原因:{e}')
-
-###########################################################################################
-
-#定时任务
-async def aps_send():
-    logger.debug("正在发送定时推送")
-    bot: Bot = get_bot()
-    for game_type, dict in CONFIG.items():
-        if game_type == "":
-            continue
-        for group_id, time in dict.items():
-            if not (datetime.now().hour == int(time.split(":")[0]) and datetime.now().minute == int(time.split(":")[1])):
-                continue
-            try:
-                group_id = int(group_id)
-                if game_type in GENSHIN_NAME:
-                    send_type = Rank(ForumType.GenshinCos, RankType.Daily)
-                elif game_type in DBY_NAME:
-                    send_type = Rank(ForumType.DBYCOS, RankType.Daily)
-                elif game_type in HONKAI3RD_NAME:
-                    send_type = Rank(ForumType.Honkai3rdPic, RankType.Daily)
-                elif game_type in STAR_RAIL:
-                    send_type = Rank(ForumType.StarRailCos, RankType.Daily)
-                else:
-                    continue
-                image_list = await send_type.async_get_urls(page_size=5)
-                name_list = await send_type.async_get_name(page_size=5)
-                rank_text = '\n'.join([f"{i+1}.{name_list[i]}" for i in range(len(name_list))])
-                msg_list = [f"✅米游社{game_type}cos每日榜单✅"]
-                msg_list.append(rank_text)
-                msg_list.append([MessageSegment.image(img) for img in image_list])
-                msg_list = msglist2forward('米游社cos', '2854196306', msg_list)
-                await bot.call_api("send_group_forward_msg", group_id=group_id, messages=msg_list)
-                await asyncio.sleep(1)
-            except Exception as e:
-                logger.error(e)
-
-
-async def send_images(bot:Bot, matcher: Matcher, args: list, event: MessageEvent, send_type: HoyoBasicSpider):
-    '''
-    发送图片
-
-    params:
-        bot: 当前bot
-        matcher: 事件响应器
-        args: 命令参数(0:类型 1:数量)
-        event: 消息事件类型
-        send_type: 爬虫类型
-    '''
-    global user_data
-    out_cd, deletime, user_data = check_cd(event.user_id, user_data)
-    if out_cd:
-        if len(args)<2:
-            await matcher.send("获取图片中…请稍等")
-            try:
-                image_list = await send_type.async_get_urls()
-                await matcher.send(MessageSegment.image(choice(image_list)))
-            except ActionFailed:
-                await matcher.finish("账户风控了,发送不了图片", at_sender=True)
-        else:
-            num = int(re.sub(r"[x|*|X]", "", args[1]))
-            num = num if num <= MAX else MAX
-            msg_list = [f'✅找到最新的一些{args[0]}图如下:✅']
-            image_list = await send_type.async_get_urls()
-            if num > len(image_list):
-                await matcher.finish(f"最多只能获取{len(image_list)}张图片", at_sender=True)
-            for i in range(num):
-                msg_list.append(MessageSegment.image(image_list[i]))
-            await send_forward_msg(bot, event, "米游社cos", bot.self_id, msg_list)
-    else:
-        await matcher.finish(f"cd冷却中,还剩{deletime}秒", at_sender=True)
-
-@DRIVER.on_startup
-@DRIVER.on_bot_connect
-async def start_aps():
-    try:
-        if scheduler == None:
-            logger.error("未安装apscheduler插件,无法使用此功能")
-        with open(config_path, "r", encoding="utf8") as f:
-            CONFIG = json.load(f)
-        for game_type, dict in CONFIG.items():
-            if game_type == "":
-                continue
-            for group_id, time in dict.items():
-                if time == "":
-                    continue
-                try:
-                    scheduler.add_job(aps_send, trigger="cron", hour=time.split(":")[0], minute=time.split(":")[1], id=f"{game_type}{group_id}")
-                    logger.debug(f"已成功添加{group_id}的{game_type}定时推送")
-                    scheduler.start()
-                except Exception as e:
-                    logger.error(e)
-                    continue
-    except Exception as e:
-        logger.error(e)
-        pass
+from nonebot.adapters.onebot.v11 import (
+    Bot,
+    Message,
+    MessageEvent,
+    MessageSegment,
+    GroupMessageEvent
+)
+from nonebot.plugin import on_regex, on_command, require, PluginMetadata
+from nonebot.params import RegexGroup, ArgPlainText, CommandArg
+from nonebot.log import logger
+from nonebot import get_driver, get_bot
+from nonebot.matcher import Matcher
+from nonebot.rule import to_me
+from nonebot.exception import ActionFailed
+from typing import Tuple, Any
+from random import choice
+from datetime import datetime
+from .config import Config
+from .utils import *
+from .hoyospider import *
+try:
+    scheduler = require("nonebot_plugin_apscheduler").scheduler
+except:
+    scheduler = None
+try:
+    import ujson as json
+except ModuleNotFoundError:
+    import json
+from nonebot_plugin_apscheduler import scheduler
+import asyncio
+import re
+
+__plugin_meta__ = PluginMetadata(
+    name="米游社cos",
+    description="获取原神coser图片",
+    config=Config,
+    usage="原神cos,CosPlus,下载cos",
+    type="application",
+    homepage="https://github.com/Cvandia/nonebot_plugin_genshin_cos",
+    supported_adapters={"~onebot.v11"},
+    extra={
+        "unique_name": "genshin_cos",
+        "example": "保存cos:保存cos图片至本地文件",
+        "author": "divandia <106718176+Cvandia@users.noreply.github.com>",
+        "version": "0.2.0",
+    }
+)
+logo = """<g>
+  /$$$$$$                                /$$       /$$                  /$$$$$$                     
+ /$$__  $$                              | $$      |__/                 /$$__  $$                    
+| $$  \__/  /$$$$$$  /$$$$$$$   /$$$$$$$| $$$$$$$  /$$ /$$$$$$$       | $$  \__/  /$$$$$$   /$$$$$$$
+| $$ /$$$$ /$$__  $$| $$__  $$ /$$_____/| $$__  $$| $$| $$__  $$      | $$       /$$__  $$ /$$_____/
+| $$|_  $$| $$$$$$$$| $$  \ $$|  $$$$$$ | $$  \ $$| $$| $$  \ $$      | $$      | $$  \ $$|  $$$$$$ 
+| $$  \ $$| $$_____/| $$  | $$ \____  $$| $$  | $$| $$| $$  | $$      | $$    $$| $$  | $$ \____  $$
+|  $$$$$$/|  $$$$$$$| $$  | $$ /$$$$$$$/| $$  | $$| $$| $$  | $$      |  $$$$$$/|  $$$$$$/ /$$$$$$$/
+ \______/  \_______/|__/  |__/|_______/ |__/  |__/|__/|__/  |__/       \______/  \______/ |_______/ 
+ </g>"""
+
+
+logger.opt(colors=True).info(logo)
+
+#用户cd数据
+user_data = {}
+CONFIG: Dict[str, Dict[str,str]] = {'原神':{},'崩坏3':{},'大别野':{},'星穹铁道':{}}
+DRIVER = get_driver()
+# 读取配置文件
+config_path = Path("config/genshincos.json")
+config_path.parent.mkdir(parents=True, exist_ok=True)
+if config_path.exists():
+    with open(config_path, "r", encoding="utf8") as f:
+        CONFIG = json.load(f)
+else:
+    with open(config_path, "w", encoding="utf8") as f:
+        json.dump(CONFIG, f, ensure_ascii=False, indent=4)
+
+#事件响应器
+download_cos = on_command('下载cos', aliases={'cos保存', '保存cos'}, block=False, priority=5, permission=SUPER_PERMISSION)
+hot_cos = on_command('热门cos', aliases={'热门coser', '热门cos图'}, block=False, priority=5)
+rank_cos = on_regex(r'^(日|月|周)榜cos[r]?[图]?(.+)?',priority=5, block=False, flags=re.I)
+latest_cos = on_command('最新cos', aliases={'最新coser', '最新cos图'}, block=False, priority=5)
+good_cos = on_command('精品cos', aliases={'精品coser', '精品cos图'}, block=False, priority=5)
+turn_aps = on_regex(r'^(开启|关闭)每日推送(原神|崩坏3|星穹铁道|大别野)(\s)?(.+)?', block=False, priority=5, flags=re.I, permission=SUPER_PERMISSION)
+show_aps = on_command('查看本群推送', aliases={'查看推送','查看订阅'}, block=False, priority=5, rule=to_me())
+
+@show_aps.handle()
+async def _(bot: Bot, event: GroupMessageEvent):
+    send_msg = '本群订阅的推送有:\n'
+    for game_type, dict in CONFIG.items():
+        if game_type == "": continue
+        for goup_id, time in dict.items():
+            if str(event.group_id) == goup_id:
+                send_msg += f"{game_type}的每日{time}推送\n"
+    await show_aps.finish(send_msg)
+
+
+@turn_aps.handle()
+async def _(event: GroupMessageEvent, args: Tuple[str, ...] = RegexGroup()):
+    # 检查是否安装了apscheduler插件，并且是否开启了定时推送
+    if scheduler == None:
+        await turn_aps.finish("未安装apscheduler插件,无法使用此功能")
+    mode = args[0] 
+    game_type = args[1]
+    time = args[3]
+    aps_group_id = str(event.group_id)
+    MyConfig = CONFIG.copy()
+    if mode == "开启":
+        for name in MyConfig.keys():
+            if name == game_type:
+                if aps_group_id in MyConfig[name].keys():
+                    await turn_aps.finish("该群已开启,无需重复开启")
+                elif not time:
+                    await turn_aps.finish("请指定推送时间")
+                else:
+                    CONFIG[name][aps_group_id] = time
+                    try:
+                        scheduler.add_job(aps_send, trigger="cron", hour=time.split(":")[0], minute=time.split(":")[1], id=f"{game_type}{aps_group_id}",args=(aps_group_id,)) 
+                        logger.debug(f"已成功添加{aps_group_id}的{game_type}定时推送")
+                    except Exception as e:
+                        logger.error(e)
+    else:
+        for name in MyConfig.keys():
+            if name == game_type:
+                if aps_group_id in MyConfig[name].keys():
+                    CONFIG[name].pop(aps_group_id)
+                    try:
+                        scheduler.remove_job(f"{game_type}{aps_group_id}")
+                    except Exception as e:
+                        logger.error(e)
+                        continue
+                else:
+                    await turn_aps.finish("该群已关闭,无需重复关闭")
+    with open(config_path, "w", encoding="utf8") as f:
+        f.write(json.dumps(CONFIG, ensure_ascii=False, indent=4))
+    await turn_aps.finish(f"已成功{mode}{aps_group_id}的{game_type}定时推送")
+
+
+@hot_cos.handle()
+async def _(bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()):
+    if not arg:
+        await hot_cos.finish("请指定cos类型")
+    args = arg.extract_plain_text().split()
+    if args[0] in GENSHIN_NAME:
+        send_type = genshin_hot
+    elif args[0] in HONKAI3RD_NAME:
+        send_type = honkai3rd_hot
+    elif args[0] in DBY_NAME:
+        send_type = dbycos_hot
+    elif args[0] in STAR_RAIL:
+        send_type = starrail_hot
+    else:
+        await hot_cos.finish("暂不支持该类型")
+    await send_images(bot,matcher,args,event,send_type)
+
+@rank_cos.handle()
+async def _(bot: Bot, matcher: Matcher, event: MessageEvent, group: Tuple[str, ...] = RegexGroup()):
+    if not group[1]:
+        await rank_cos.finish("请指定cos类型")
+    args = group[1].split()
+    if group[0] == "日":
+        rank_type = RankType.Daily
+    elif group[0] == "周":
+        rank_type = RankType.Weekly
+    elif group[0] == "月":
+        rank_type = RankType.Monthly
+
+    if args[0] in GENSHIN_NAME:
+        send_type = Rank(ForumType.GenshinCos, rank_type)
+    elif args[0] in HONKAI3RD_NAME:
+        send_type = Rank(ForumType.Honkai3rdPic, rank_type)
+    elif args[0] in DBY_NAME:
+        send_type = Rank(ForumType.DBYCOS, rank_type)
+    elif args[0] in STAR_RAIL:
+        send_type = Rank(ForumType.StarRailCos, rank_type)
+    else:
+        await rank_cos.finish("暂不支持该类型")
+    await send_images(bot,matcher,args,event,send_type)
+
+@latest_cos.handle()
+async def _(bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()):
+    if not arg:
+        await latest_cos.finish("请指定cos类型")
+    args = arg.extract_plain_text().split()
+    if args[0] in GENSHIN_NAME:
+        send_type = genshin_latest_comment
+    elif args[0] in HONKAI3RD_NAME:
+        send_type = honkai3rd_latest_comment
+    elif args[0] in DBY_NAME:
+        send_type = dbycos_latest_comment
+    elif args[0] in STAR_RAIL:
+        send_type = starrail_latest_comment
+    else:
+        await latest_cos.finish("暂不支持该类型")
+    await send_images(bot,matcher,args,event,send_type)
+
+@good_cos.handle()
+async def _(bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()):
+    if not arg:
+        await good_cos.finish("请指定cos类型")
+    args = arg.extract_plain_text().split()
+    if args[0] in GENSHIN_NAME:
+        await good_cos.finish("原神暂不支持精品cos")
+    elif args[0] in HONKAI3RD_NAME:
+        send_type = honkai3rd_good
+    elif args[0] in DBY_NAME:
+        send_type = dbycos_good
+    elif args[0] in STAR_RAIL:
+        await good_cos.finish("星穹铁道暂不支持精品cos")
+    else:
+        await good_cos.finish("暂不支持该类型")
+    await send_images(bot,matcher,args,event,send_type)
+
+
+@download_cos.got('game_type', prompt='你想下载哪种类型的,有原神和大别野,崩坏3')
+async def got_type(game_type: str = ArgPlainText()):
+    if game_type in GENSHIN_NAME:
+        hot = genshin_hot
+    elif game_type in DBY_NAME:
+        hot = dbycos_hot
+    elif game_type in HONKAI3RD_NAME:
+        hot = honkai3rd_hot
+    elif game_type in STAR_RAIL:
+        hot = starrail_hot
+    image_urls = await hot.async_get_urls()
+    if not image_urls:
+        await download_cos.finish(f'没有找到{game_type}的cos图片')
+    else:
+        await download_cos.send(f'正在下载{game_type}的cos图片')
+        try:
+            await download_from_urls(image_urls, SAVE_PATH / f'{game_type}cos')
+            await download_cos.finish(f'已成功保存{len(image_urls)}张{game_type}的cos图片')
+        except WriteError as e:
+            await download_cos.finish(f'保存{game_type}的cos图片失败,原因:{e}')
+
+###########################################################################################
+
+#定时任务
+async def aps_send(aps_goup_id: str):
+    logger.debug("正在发送定时推送")
+    bot: Bot = get_bot()
+    for game_type, dict in CONFIG.items():
+        if game_type == "":
+            continue
+        for saved_group_id, time in dict.items():
+            if not (datetime.now().hour == int(time.split(":")[0]) and datetime.now().minute == int(time.split(":")[1])):
+                continue
+            elif saved_group_id != aps_goup_id:
+                continue
+            try:
+                group_id = int(saved_group_id)
+                if game_type in GENSHIN_NAME:
+                    send_type = genshin_rank_daily
+                elif game_type in DBY_NAME:
+                    send_type = dby_rank_daily
+                elif game_type in HONKAI3RD_NAME:
+                    send_type = honkai3rd_rank_daily
+                elif game_type in STAR_RAIL:
+                    send_type = starrail_rank_daily
+                else:
+                    continue
+                image_list = await send_type.async_get_urls(page_size=5)
+                name_list = await send_type.async_get_name(page_size=5)
+                rank_text = '\n'.join([f"{i+1}.{name_list[i]}" for i in range(len(name_list))])
+                msg_list = [f"✅米游社{game_type}cos每日榜单✅"]
+                msg_list.append(rank_text)
+                msg_list.append([MessageSegment.image(img) for img in image_list])
+                msg_list = msglist2forward('米游社cos', '2854196306', msg_list)
+                await bot.call_api("send_group_forward_msg", group_id=group_id, messages=msg_list)
+                await asyncio.sleep(1)
+            except Exception as e:
+                logger.error(e)
+
+
+async def send_images(bot:Bot, matcher: Matcher, args: list, event: MessageEvent, send_type: HoyoBasicSpider):
+    '''
+    发送图片
+
+    params:
+        bot: 当前bot
+        matcher: 事件响应器
+        args: 命令参数(0:类型 1:数量)
+        event: 消息事件类型
+        send_type: 爬虫类型
+    '''
+    global user_data
+    out_cd, deletime, user_data = check_cd(event.user_id, user_data)
+    if out_cd:
+        if len(args)<2:
+            await matcher.send("获取图片中…请稍等")
+            try:
+                image_list = await send_type.async_get_urls()
+                await matcher.send(MessageSegment.image(choice(image_list)))
+            except ActionFailed:
+                await matcher.finish("账户风控了,发送不了图片", at_sender=True)
+        else:
+            num = int(re.sub(r"[x|*|X]", "", args[1]))
+            num = num if num <= MAX else MAX
+            msg_list = [f'✅找到最新的一些{args[0]}图如下:✅']
+            image_list = await send_type.async_get_urls()
+            if num > len(image_list):
+                await matcher.finish(f"最多只能获取{len(image_list)}张图片", at_sender=True)
+            for i in range(num):
+                msg_list.append(MessageSegment.image(image_list[i]))
+            await send_forward_msg(bot, event, "米游社cos", bot.self_id, msg_list)
+    else:
+        await matcher.finish(f"cd冷却中,还剩{deletime}秒", at_sender=True)
+
+@DRIVER.on_startup
+async def start_aps():
+    try:
+        if scheduler == None:
+            logger.error("未安装apscheduler插件,无法使用此功能")
+        with open(config_path, "r", encoding="utf8") as f:
+            CONFIG = json.load(f)
+        for game_type, dict in CONFIG.items():
+            if game_type == "":
+                continue
+            for aps_group_id, time in dict.items():
+                if time == "":
+                    continue
+                try:
+                    scheduler.add_job(aps_send, trigger="cron", hour=time.split(":")[0], minute=time.split(":")[1], id=f"{game_type}{aps_group_id}",args=(aps_group_id,))
+                    logger.debug(f"已成功添加{aps_group_id}的{game_type}定时推送")
+                except Exception as e:
+                    logger.error(e)
+                    continue
+    except Exception as e:
+        logger.error(e)
```

### Comparing `nonebot_plugin_genshin_cos-0.2.0/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF` & `nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.2.0/nonebot_plugin_genshin_cos/utils.py` & `nonebot_plugin_genshin_cos-0.2.1/nonebot_plugin_genshin_cos/utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-from pathlib import Path
-from nonebot import get_driver
-from .config import Config
-from typing import Dict, List, Tuple
-from datetime import datetime, timedelta
-from httpx import TimeoutException
-import httpx
-from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent, Message, GROUP_ADMIN, GROUP_OWNER
-from nonebot.permission import SUPERUSER
-#######################################################
-
-# 拓展的异常类和函数
-SUPER_PERMISSION = GROUP_ADMIN | GROUP_OWNER | SUPERUSER
-GENSHIN_NAME = ["原神",'OP','op','欧泡','⭕','🅾️','🅾️P','🅾️p','原','圆']
-HONKAI3RD_NAME = ['崩坏3', '崩崩崩', '蹦蹦蹦','崩坏三','崩三','崩崩崩三','崩坏3rd','崩坏3Rd','崩坏3RD','崩坏3rd','崩坏3RD','崩坏3Rd']
-DBY_NAME = ['大别野','DBY','dby']
-STAR_RAIL = ['星穹铁道','星穹','崩铁','铁道','星铁','穹p','穹铁']
-
-class WriteError(Exception):
-    """写入错误"""
-    def __init__(self):
-        super().__init__('写入错误')
-
-
-# 加载配置
-
-MAX = Config.parse_obj(get_driver().config.dict()).cos_max
-SAVE_PATH = Path(Config.parse_obj(get_driver().config.dict()).cos_path)
-CD = Config.parse_obj(get_driver().config.dict()).cos_cd
-
-
-def check_cd(user_id: int, user_data: Dict[str, datetime]) -> Tuple[bool, int, dict]:
-    """检查用户触发事件的cd
-
-    Args:
-        user_id (int): 用户的id
-        user_data (dict): 用户数据
-
-    Returns:
-        Tuple[bool,int,dict]: 返回一个元组，第一个元素为True表示可以触发，为False表示不可以触发，第二个元素为剩余时间，第三个元素为用户数据
-    """
-    data = user_data
-    if str(user_id) not in data:
-        data[str(user_id)] = datetime.now()
-    if datetime.now() < data[f'{user_id}']:
-        delta = (data[str(user_id)] - datetime.now()).seconds
-        return False, delta, data
-    else:
-        data[str(user_id)] = datetime.now() + timedelta(seconds=CD)
-        return True, 0, data
-
-
-async def download_from_urls(urls: List[str], path: Path):
-    '''
-    下载图片
-    :param urls: 图片链接
-    :param path: 保存路径
-    :return: None
-    '''
-    if not path.parent.exists():
-        path.parent.mkdir(parents=True)
-    async with httpx.AsyncClient() as client:
-        for url in urls:
-            try:
-                filename = url.split('/')[-1]
-                new_path = path / filename
-                rsp = await client.get(url)
-                content = rsp.content
-                with open(new_path, 'wb') as f:
-                    f.write(content)
-            except (IndexError, IOError, httpx.ConnectError, httpx.RequestError, httpx.ReadTimeout, TimeoutException):
-                raise WriteError('下载失败')
-
-
-async def send_forward_msg(
-    bot: Bot,
-    event: MessageEvent,
-    name: str,
-    uin: str,
-    msgs: list,
-) -> dict:
-    """调用合并转发API
-
-    params:
-        bot: Bot,
-        event: 消息事件类型,
-        name: 发送者昵称,
-        uin: 发送者账号,
-        msgs: 消息列表,
-    """
-    def to_json(msg: Message):
-        return {"type": "node", "data": {"name": name, "uin": uin, "content": msg}}
-
-    messages = [to_json(msg) for msg in msgs]
-
-    if isinstance(event, GroupMessageEvent):
-        return await bot.call_api(
-            "send_group_forward_msg", group_id=event.group_id, messages=messages
-        )
-    else:
-        return await bot.call_api(
-            "send_private_forward_msg", user_id=event.user_id, messages=messages
-        )
-
-
-def msglist2forward(name: str, uin: str, msgs: list) -> list:
-    """调用合并转发群API
-
-    params:
-        bot: Bot
-        name: 发送者昵称
-        uin: 发送者账号
-        msgs: 消息列表
-    """
-    def to_json(msg: Message):
-        return {"type": "node", "data": {"name": name, "uin": uin, "content": msg}}
-
+from pathlib import Path
+from nonebot import get_driver
+from .config import Config
+from typing import Dict, List, Tuple
+from datetime import datetime, timedelta
+from httpx import TimeoutException
+import httpx
+from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent, Message, GROUP_ADMIN, GROUP_OWNER
+from nonebot.permission import SUPERUSER
+#######################################################
+
+# 拓展的异常类和函数
+SUPER_PERMISSION = GROUP_ADMIN | GROUP_OWNER | SUPERUSER
+GENSHIN_NAME = ["原神",'OP','op','欧泡','⭕','🅾️','🅾️P','🅾️p','原','圆']
+HONKAI3RD_NAME = ['崩坏3', '崩崩崩', '蹦蹦蹦','崩坏三','崩三','崩崩崩三','崩坏3rd','崩坏3Rd','崩坏3RD','崩坏3rd','崩坏3RD','崩坏3Rd']
+DBY_NAME = ['大别野','DBY','dby']
+STAR_RAIL = ['星穹铁道','星穹','崩铁','铁道','星铁','穹p','穹铁']
+
+class WriteError(Exception):
+    """写入错误"""
+    def __init__(self):
+        super().__init__('写入错误')
+
+
+# 加载配置
+
+MAX = Config.parse_obj(get_driver().config.dict()).cos_max
+SAVE_PATH = Path(Config.parse_obj(get_driver().config.dict()).cos_path)
+CD = Config.parse_obj(get_driver().config.dict()).cos_cd
+
+
+def check_cd(user_id: int, user_data: Dict[str, datetime]) -> Tuple[bool, int, dict]:
+    """检查用户触发事件的cd
+
+    Args:
+        user_id (int): 用户的id
+        user_data (dict): 用户数据
+
+    Returns:
+        Tuple[bool,int,dict]: 返回一个元组，第一个元素为True表示可以触发，为False表示不可以触发，第二个元素为剩余时间，第三个元素为用户数据
+    """
+    data = user_data
+    if str(user_id) not in data:
+        data[str(user_id)] = datetime.now()
+    if datetime.now() < data[f'{user_id}']:
+        delta = (data[str(user_id)] - datetime.now()).seconds
+        return False, delta, data
+    else:
+        data[str(user_id)] = datetime.now() + timedelta(seconds=CD)
+        return True, 0, data
+
+
+async def download_from_urls(urls: List[str], path: Path):
+    '''
+    下载图片
+    :param urls: 图片链接
+    :param path: 保存路径
+    :return: None
+    '''
+    if not path.parent.exists():
+        path.parent.mkdir(parents=True)
+    async with httpx.AsyncClient() as client:
+        for url in urls:
+            try:
+                filename = url.split('/')[-1]
+                new_path = path / filename
+                rsp = await client.get(url)
+                content = rsp.content
+                with open(new_path, 'wb') as f:
+                    f.write(content)
+            except (IndexError, IOError, httpx.ConnectError, httpx.RequestError, httpx.ReadTimeout, TimeoutException):
+                raise WriteError('下载失败')
+
+
+async def send_forward_msg(
+    bot: Bot,
+    event: MessageEvent,
+    name: str,
+    uin: str,
+    msgs: list,
+) -> dict:
+    """调用合并转发API
+
+    params:
+        bot: Bot,
+        event: 消息事件类型,
+        name: 发送者昵称,
+        uin: 发送者账号,
+        msgs: 消息列表,
+    """
+    def to_json(msg: Message):
+        return {"type": "node", "data": {"name": name, "uin": uin, "content": msg}}
+
+    messages = [to_json(msg) for msg in msgs]
+
+    if isinstance(event, GroupMessageEvent):
+        return await bot.call_api(
+            "send_group_forward_msg", group_id=event.group_id, messages=messages
+        )
+    else:
+        return await bot.call_api(
+            "send_private_forward_msg", user_id=event.user_id, messages=messages
+        )
+
+
+def msglist2forward(name: str, uin: str, msgs: list) -> list:
+    """调用合并转发群API
+
+    params:
+        bot: Bot
+        name: 发送者昵称
+        uin: 发送者账号
+        msgs: 消息列表
+    """
+    def to_json(msg: Message):
+        return {"type": "node", "data": {"name": name, "uin": uin, "content": msg}}
+
     return [to_json(msg) for msg in msgs]
```

### Comparing `nonebot_plugin_genshin_cos-0.2.0/pyproject.toml` & `nonebot_plugin_genshin_cos-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[tool.poetry]
-name = "nonebot-plugin-genshin-cos"
-version = "0.2.0"
-description = "米游社原神cos图获取"
-authors = ["Cvandia <106718176+Cvandia@users.noreply.github.com>"]
-license = "MIT"
-readme = "README.md"
-packages = [{include = "nonebot_plugin_genshin_cos"}]
-
-[tool.poetry.dependencies]
-python = ">=3.8,<4"
-nonebot2 = ">=2.0.0-beta.1"
-nonebot-adapter-onebot = ">=2.0.0-beta.1"
-httpx = ">=0.19.0"
-nonebot-plugin-apscheduler= ">=0.1.3"
-aiofiles = ">=0.7.0"
-pydantic = ">=1.10.2"
-pathlib = ">=1.0.1"
-ujson = ">=5.5.0"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "nonebot-plugin-genshin-cos"
+version = "0.2.1"
+description = "米游社原神cos图获取"
+authors = ["Cvandia <106718176+Cvandia@users.noreply.github.com>"]
+license = "MIT"
+readme = "README.md"
+packages = [{include = "nonebot_plugin_genshin_cos"}]
+
+[tool.poetry.dependencies]
+python = ">=3.8,<4"
+nonebot2 = ">=2.0.0-beta.1"
+nonebot-adapter-onebot = ">=2.0.0-beta.1"
+httpx = ">=0.19.0"
+nonebot-plugin-apscheduler= ">=0.1.3"
+aiofiles = ">=0.7.0"
+pydantic = ">=1.10.2"
+pathlib = ">=1.0.1"
+ujson = ">=5.5.0"
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_genshin_cos-0.2.0/README.md` & `nonebot_plugin_genshin_cos-0.2.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,124 @@
-
-<div align="center">
-
-<a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/Cvandia/nonebot_plugin_genshin_cos/blob/main/res/ico.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-
-</div>
-
-<div align="center">
-
-# nonebot-plugin-genshin-cos
-
-_⭐基于Nonebot2的一款获取米游社cos的插件⭐_
-
-
-</div>
-
-<div align="center">
-<a href="https://www.python.org/downloads/release/python-390/"><img src="https://img.shields.io/badge/python-3.8+-blue"></a>  <a href=""><img src="https://img.shields.io/badge/QQ-1141538825-yellow"></a> <a href="https://github.com/Cvandia/nonebot_plugin_genshin_cos/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue"></a> <a href="https://v2.nonebot.dev/"><img src="https://img.shields.io/badge/Nonebot2-rc1+-red"></a>
-</div>
-
-
-## ⭐ 介绍
-
-受到[教程](https://juejin.cn/post/6990320268010848286)的启发，所以写了这个插件，更多功能后续更新~~我很懒，学业重~~
-
-
-<div align="center">
-
-### 或者你有啥关于该插件的新想法的，可以提issue或者pr (>A<)
-
-</div>
-
-## 💿 安装
-
-<details>
-<summary>安装</summary>
-
-pip 安装
-
-```
-pip install nonebot-plugin-genshin-cos
-```
-- 在nonebot的pyproject.toml中的plugins = ["xxx"]添加此插件
-
-nb-cli安装
-
-```
-nb plugin install nonebot-plugin-genshin-cos --upgrade
-```
-
-git clone安装(不推荐)
-
-- 运行
-```git clone https://github.com/Cvandia/nonebot_plugin_genshin_cos```
-- 在运行处
-把文件夹`nonebot-plugin-genshen-cos`复制到bot根目录下的`src/plugins`(或者你创建bot时的其他名称`xxx/plugins`)
-
- 
- </details>
- 
- <details>
- <summary>注意</summary>
- 
- 推荐镜像站下载
-  
- 清华源```https://pypi.tuna.tsinghua.edu.cn/simple```
- 
- 阿里源```https://mirrors.aliyun.com/pypi/simple/```
-
-</details>
-
-
-## ⚙️ 配置
-### 在env.中添加以下配置
-
-| 配置 | 类型 | 默认值 | 说明 |
-|:-----:|:----:|:----:|:---:|
-|cos_max|int|5|最大返回cos图片数量|
-|cos_path|str|无|不配置则默认下载到bot根目录的`"data/genshin_cos"`,支持绝对路劲如`"C:/Users/image"`和相对bot根目录路劲如`"coser/image"`
-|cos_cd|int|30|用户触发cd|
-
-> 注意：绝对路劲中用`/`，用`\`可能会被转义
-
-## ⭐ 使用
-
-### 指令：
-| 指令 | 需要@ | 范围 | 说明 |权限|
-|:-----:|:----:|:----:|:----:|:----:|
-|下载cos|否|群聊、私聊|下载热门cos图|超管、群主、管理员|
-|热门cos|否|同上|获取指定游戏热门cos图，如`热门cos 原神 x3`|全部|
-|日、周、月榜cos|否|同上|获取排行榜cos图。如`日榜cos 原神 x3`|全部|
-|最新cos|否|同上|和上面差不多，不写了，哼哼|全部|
-|精品cos|否|同上|上上面一样的道理！|全部|
-|开启每日推送xx (时间)|否|仅群聊|如`开启每日推送原神 8:30`,注意时间的格式|超管、群主、管理员|
-
-**注意**
-
-指令触发方式是正则匹配的，不需要加指令前缀
-
-## 🌙 未来
- - [x] 缓慢更新，最近学业繁忙哦~
- - [x] 随机发送cos图片
- - [x] 保存cos图
- - [x] 内置cd和用户触发上限
- - [x] 合并转发发送多张cos图
-~~playwright获取cos图~~
-~~选择发送图库方式：离线 (迅速) or 在线（缓慢、目前是的）~~
- - [x] 支持米游社其他社区cos获取
- - [x] 支持每日推送热榜的cos图
-
---- 喜欢记得点个star⭐---
-
-## ❗免责声明
-
-图片版权归米游社原神cos社区所属，请尊重
-coser的创作权
-
-
-
-## 💝 特别鸣谢
-
-- [x] [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
+
+<div align="center">
+
+<a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/Cvandia/nonebot_plugin_genshin_cos/blob/main/res/ico.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+
+</div>
+
+<div align="center">
+
+# nonebot-plugin-genshin-cos
+
+_⭐基于Nonebot2的一款获取米游社cos的插件⭐_
+
+
+</div>
+
+<div align="center">
+<a href="https://www.python.org/downloads/release/python-390/"><img src="https://img.shields.io/badge/python-3.8+-blue"></a>  <a href=""><img src="https://img.shields.io/badge/QQ-1141538825-yellow"></a> <a href="https://github.com/Cvandia/nonebot_plugin_genshin_cos/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue"></a> <a href="https://v2.nonebot.dev/"><img src="https://img.shields.io/badge/Nonebot2-rc1+-red"></a>
+</div>
+
+
+## ⭐ 介绍
+
+受到[教程](https://juejin.cn/post/6990320268010848286)的启发，所以写了这个插件，更多功能后续更新~~我很懒，学业重~~
+
+
+<div align="center">
+
+### 或者你有啥关于该插件的新想法的，可以提issue或者pr (>A<)
+
+</div>
+
+## 💿 安装
+
+<details>
+<summary>安装</summary>
+
+pip 安装
+
+```
+pip install nonebot-plugin-genshin-cos
+```
+- 在nonebot的pyproject.toml中的plugins = ["xxx"]添加此插件
+
+nb-cli安装
+
+```
+nb plugin install nonebot-plugin-genshin-cos --upgrade
+```
+
+git clone安装(不推荐)
+
+- 运行
+```git clone https://github.com/Cvandia/nonebot_plugin_genshin_cos```
+- 在运行处
+把文件夹`nonebot-plugin-genshen-cos`复制到bot根目录下的`src/plugins`(或者你创建bot时的其他名称`xxx/plugins`)
+
+ 
+ </details>
+ 
+ <details>
+ <summary>注意</summary>
+ 
+ 推荐镜像站下载
+  
+ 清华源```https://pypi.tuna.tsinghua.edu.cn/simple```
+ 
+ 阿里源```https://mirrors.aliyun.com/pypi/simple/```
+
+</details>
+
+
+## ⚙️ 配置
+### 在env.中添加以下配置
+
+| 配置 | 类型 | 默认值 | 说明 |
+|:-----:|:----:|:----:|:---:|
+|cos_max|int|5|最大返回cos图片数量|
+|cos_path|str|无|不配置则默认下载到bot根目录的`"data/genshin_cos"`,支持绝对路劲如`"C:/Users/image"`和相对bot根目录路劲如`"coser/image"`
+|cos_cd|int|30|用户触发cd|
+
+> 注意：绝对路劲中用`/`，用`\`可能会被转义
+
+## ⭐ 使用
+
+### 指令：
+| 指令 | 需要@ | 范围 | 说明 |权限|
+|:-----:|:----:|:----:|:----:|:----:|
+|下载cos|否|群聊、私聊|下载热门cos图|超管、群主、管理员|
+|热门cos|否|同上|获取指定游戏热门cos图，如`热门cos 原神 x3`|全部|
+|日、周、月榜cos|否|同上|获取排行榜cos图。如`日榜cos 原神 x3`|全部|
+|最新cos|否|同上|和上面差不多，不写了，哼哼|全部|
+|精品cos|否|同上|上上面一样的道理！|全部|
+|开启每日推送xx (时间)|否|仅群聊|如`开启每日推送原神 8:30`,注意时间的格式|超管、群主、管理员|
+|查看本群推送|是|群聊|查看本群的订阅cos目录|全部|
+
+**注意**
+
+指令触发方式是正则匹配的，不需要加指令前缀
+
+## 🌙 未来
+ - [x] 缓慢更新，最近学业繁忙哦~
+ - [x] 随机发送cos图片
+ - [x] 保存cos图
+ - [x] 内置cd和用户触发上限
+ - [x] 合并转发发送多张cos图
+~~playwright获取cos图~~
+~~选择发送图库方式：离线 (迅速) or 在线（缓慢、目前是的）~~
+ - [x] 支持米游社其他社区cos获取
+ - [x] 支持每日推送热榜的cos图
+
+--- 喜欢记得点个star⭐---
+
+## ❗免责声明
+
+图片版权归米游社原神cos社区所属，请尊重
+coser的创作权
+
+
+
+## 💝 特别鸣谢
+
+- [x] [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
 - [x] [@qxdn](https://github.com/qxdn):感谢qxdn的[博客文章](https://qianxu.run/2021/11/12/mihoyo-bbs-crawler/),有兴趣大家也去看看咯
```

#### html2text {}

```diff
@@ -30,19 +30,20 @@
 |ç­é¨cos|å¦|åä¸|è·åæå®æ¸¸æç­é¨coså¾ï¼å¦`ç­é¨cos åç¥
 x3`|å¨é¨|
 |æ¥ãå¨ãææ¦cos|å¦|åä¸|è·åæè¡æ¦coså¾ãå¦`æ¥æ¦cos åç¥
 x3`|å¨é¨|
 |ææ°cos|å¦|åä¸|åä¸é¢å·®ä¸å¤ï¼ä¸åäºï¼å¼å¼|å¨é¨|
 |ç²¾åcos|å¦|åä¸|ä¸ä¸é¢ä¸æ ·çéçï¼|å¨é¨| |å¼å¯æ¯æ¥æ¨éxx
 (æ¶é´)|å¦|ä»ç¾¤è|å¦`å¼å¯æ¯æ¥æ¨éåç¥ 8:
-30`,æ³¨ææ¶é´çæ ¼å¼|è¶ç®¡ãç¾¤ä¸»ãç®¡çå| **æ³¨æ**
-æä»¤è§¦åæ¹å¼æ¯æ­£åå¹éçï¼ä¸éè¦å æä»¤åç¼ ## ð æªæ¥
-- [x] ç¼æ¢æ´æ°ï¼æè¿å­¦ä¸ç¹å¿å¦~ - [x] éæºåécoså¾ç - [x]
-ä¿å­coså¾ - [x] åç½®cdåç¨æ·è§¦åä¸é - [x]
-åå¹¶è½¬ååéå¤å¼ coså¾ ~~playwrightè·åcoså¾~~
+30`,æ³¨ææ¶é´çæ ¼å¼|è¶ç®¡ãç¾¤ä¸»ãç®¡çå|
+|æ¥çæ¬ç¾¤æ¨é|æ¯|ç¾¤è|æ¥çæ¬ç¾¤çè®¢écosç®å½|å¨é¨|
+**æ³¨æ** æä»¤è§¦åæ¹å¼æ¯æ­£åå¹éçï¼ä¸éè¦å æä»¤åç¼ ##
+ð æªæ¥ - [x] ç¼æ¢æ´æ°ï¼æè¿å­¦ä¸ç¹å¿å¦~ - [x]
+éæºåécoså¾ç - [x] ä¿å­coså¾ - [x] åç½®cdåç¨æ·è§¦åä¸é -
+[x] åå¹¶è½¬ååéå¤å¼ coså¾ ~~playwrightè·åcoså¾~~
 ~~éæ©åéå¾åºæ¹å¼ï¼ç¦»çº¿ (è¿é) or
 å¨çº¿ï¼ç¼æ¢ãç®åæ¯çï¼~~ - [x] æ¯æç±³æ¸¸ç¤¾å¶ä»ç¤¾åºcosè·å
 - [x] æ¯ææ¯æ¥æ¨éç­æ¦çcoså¾ --- åæ¬¢è®°å¾ç¹ä¸ªstarâ­--- ##
 âåè´£å£°æ å¾ççæå½ç±³æ¸¸ç¤¾åç¥cosç¤¾åºæå±ï¼è¯·å°é
 coserçåä½æ ## ð ç¹å«é¸£è°¢ - [x] [Nonebot](https://github.com/
 nonebot/nonebot2): æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã
 - [x] [@qxdn](https://github.com/qxdn):æè°¢qxdnç[åå®¢æç« ](https://
```

### Comparing `nonebot_plugin_genshin_cos-0.2.0/PKG-INFO` & `nonebot_plugin_genshin_cos-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshin-cos
-Version: 0.2.0
+Version: 0.2.1
 Summary: 米游社原神cos图获取
 License: MIT
 Author: Cvandia
 Author-email: 106718176+Cvandia@users.noreply.github.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -112,14 +112,15 @@
 |:-----:|:----:|:----:|:----:|:----:|
 |下载cos|否|群聊、私聊|下载热门cos图|超管、群主、管理员|
 |热门cos|否|同上|获取指定游戏热门cos图，如`热门cos 原神 x3`|全部|
 |日、周、月榜cos|否|同上|获取排行榜cos图。如`日榜cos 原神 x3`|全部|
 |最新cos|否|同上|和上面差不多，不写了，哼哼|全部|
 |精品cos|否|同上|上上面一样的道理！|全部|
 |开启每日推送xx (时间)|否|仅群聊|如`开启每日推送原神 8:30`,注意时间的格式|超管、群主、管理员|
+|查看本群推送|是|群聊|查看本群的订阅cos目录|全部|
 
 **注意**
 
 指令触发方式是正则匹配的，不需要加指令前缀
 
 ## 🌙 未来
  - [x] 缓慢更新，最近学业繁忙哦~
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.2.1 Summary:
 ç±³æ¸¸ç¤¾åç¥coså¾è·å License: MIT Author: Cvandia Author-email:
 106718176+Cvandia@users.noreply.github.com Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.7.0) Requires-Dist: httpx (>=0.19.0) Requires-
@@ -42,19 +42,20 @@
 |ç­é¨cos|å¦|åä¸|è·åæå®æ¸¸æç­é¨coså¾ï¼å¦`ç­é¨cos åç¥
 x3`|å¨é¨|
 |æ¥ãå¨ãææ¦cos|å¦|åä¸|è·åæè¡æ¦coså¾ãå¦`æ¥æ¦cos åç¥
 x3`|å¨é¨|
 |ææ°cos|å¦|åä¸|åä¸é¢å·®ä¸å¤ï¼ä¸åäºï¼å¼å¼|å¨é¨|
 |ç²¾åcos|å¦|åä¸|ä¸ä¸é¢ä¸æ ·çéçï¼|å¨é¨| |å¼å¯æ¯æ¥æ¨éxx
 (æ¶é´)|å¦|ä»ç¾¤è|å¦`å¼å¯æ¯æ¥æ¨éåç¥ 8:
-30`,æ³¨ææ¶é´çæ ¼å¼|è¶ç®¡ãç¾¤ä¸»ãç®¡çå| **æ³¨æ**
-æä»¤è§¦åæ¹å¼æ¯æ­£åå¹éçï¼ä¸éè¦å æä»¤åç¼ ## ð æªæ¥
-- [x] ç¼æ¢æ´æ°ï¼æè¿å­¦ä¸ç¹å¿å¦~ - [x] éæºåécoså¾ç - [x]
-ä¿å­coså¾ - [x] åç½®cdåç¨æ·è§¦åä¸é - [x]
-åå¹¶è½¬ååéå¤å¼ coså¾ ~~playwrightè·åcoså¾~~
+30`,æ³¨ææ¶é´çæ ¼å¼|è¶ç®¡ãç¾¤ä¸»ãç®¡çå|
+|æ¥çæ¬ç¾¤æ¨é|æ¯|ç¾¤è|æ¥çæ¬ç¾¤çè®¢écosç®å½|å¨é¨|
+**æ³¨æ** æä»¤è§¦åæ¹å¼æ¯æ­£åå¹éçï¼ä¸éè¦å æä»¤åç¼ ##
+ð æªæ¥ - [x] ç¼æ¢æ´æ°ï¼æè¿å­¦ä¸ç¹å¿å¦~ - [x]
+éæºåécoså¾ç - [x] ä¿å­coså¾ - [x] åç½®cdåç¨æ·è§¦åä¸é -
+[x] åå¹¶è½¬ååéå¤å¼ coså¾ ~~playwrightè·åcoså¾~~
 ~~éæ©åéå¾åºæ¹å¼ï¼ç¦»çº¿ (è¿é) or
 å¨çº¿ï¼ç¼æ¢ãç®åæ¯çï¼~~ - [x] æ¯æç±³æ¸¸ç¤¾å¶ä»ç¤¾åºcosè·å
 - [x] æ¯ææ¯æ¥æ¨éç­æ¦çcoså¾ --- åæ¬¢è®°å¾ç¹ä¸ªstarâ­--- ##
 âåè´£å£°æ å¾ççæå½ç±³æ¸¸ç¤¾åç¥cosç¤¾åºæå±ï¼è¯·å°é
 coserçåä½æ ## ð ç¹å«é¸£è°¢ - [x] [Nonebot](https://github.com/
 nonebot/nonebot2): æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã
 - [x] [@qxdn](https://github.com/qxdn):æè°¢qxdnç[åå®¢æç« ](https://
```

