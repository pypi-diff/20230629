# Comparing `tmp/ailingbot-0.0.4.tar.gz` & `tmp/ailingbot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailingbot-0.0.4.tar", max compression
+gzip compressed data, was "ailingbot-0.0.5.tar", max compression
```

## Comparing `ailingbot-0.0.4.tar` & `ailingbot-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.4/LICENSE
--rw-r--r--   0        0        0    19304 2023-06-27 07:53:22.469092 ailingbot-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.4/ailingbot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.4/ailingbot/channels/__init__.py
--rw-r--r--   0        0        0     2444 2023-06-27 07:20:37.148547 ailingbot-0.0.4/ailingbot/channels/channel.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.4/ailingbot/channels/dingtalk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.4/ailingbot/channels/feishu/__init__.py
--rw-r--r--   0        0        0     5760 2023-06-26 06:57:43.398602 ailingbot-0.0.4/ailingbot/channels/feishu/agent.py
--rw-r--r--   0        0        0     1398 2023-06-27 07:03:48.368295 ailingbot-0.0.4/ailingbot/channels/feishu/render.py
--rw-r--r--   0        0        0     7122 2023-06-27 07:22:31.063828 ailingbot-0.0.4/ailingbot/channels/feishu/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.4/ailingbot/channels/slack/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.4/ailingbot/channels/wechatwork/__init__.py
--rw-r--r--   0        0        0     4245 2023-06-26 06:57:43.400029 ailingbot-0.0.4/ailingbot/channels/wechatwork/agent.py
--rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.4/ailingbot/channels/wechatwork/encrypt.py
--rw-r--r--   0        0        0     2408 2023-06-19 04:30:43.452309 ailingbot-0.0.4/ailingbot/channels/wechatwork/render.py
--rw-r--r--   0        0        0     5942 2023-06-26 06:57:43.400763 ailingbot-0.0.4/ailingbot/channels/wechatwork/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.4/ailingbot/chat/__init__.py
--rw-r--r--   0        0        0     2076 2023-06-26 06:57:43.401435 ailingbot-0.0.4/ailingbot/chat/chatbot.py
--rw-r--r--   0        0        0     3487 2023-06-25 06:38:56.364334 ailingbot-0.0.4/ailingbot/chat/messages.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.4/ailingbot/chat/policies/__init__.py
--rw-r--r--   0        0        0     5850 2023-06-27 07:20:37.223615 ailingbot-0.0.4/ailingbot/chat/policies/langchain.py
--rw-r--r--   0        0        0     1678 2023-06-25 07:39:16.611374 ailingbot-0.0.4/ailingbot/chat/policy.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.4/ailingbot/cli/__init__.py
--rw-r--r--   0        0        0     9231 2023-06-27 07:20:37.309101 ailingbot-0.0.4/ailingbot/cli/cli.py
--rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.4/ailingbot/cli/options.py
--rw-r--r--   0        0        0     5347 2023-06-18 13:01:00.251299 ailingbot-0.0.4/ailingbot/cli/render.py
--rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.4/ailingbot/config.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.4/ailingbot/endpoint/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.4/ailingbot/shared/__init__.py
--rw-r--r--   0        0        0     3953 2023-06-27 05:30:31.536603 ailingbot-0.0.4/ailingbot/shared/abc.py
--rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.4/ailingbot/shared/errors.py
--rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.4/ailingbot/shared/misc.py
--rw-r--r--   0        0        0     1115 2023-06-27 08:59:52.998949 ailingbot-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    20872 1970-01-01 00:00:00.000000 ailingbot-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.5/LICENSE
+-rw-r--r--   0        0        0    22820 2023-06-29 08:11:26.468239 ailingbot-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.5/ailingbot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.5/ailingbot/channels/__init__.py
+-rw-r--r--   0        0        0     3128 2023-06-29 06:24:43.085356 ailingbot-0.0.5/ailingbot/channels/channel.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.5/ailingbot/channels/dingtalk/__init__.py
+-rw-r--r--   0        0        0     6335 2023-06-29 07:16:47.029744 ailingbot-0.0.5/ailingbot/channels/dingtalk/agent.py
+-rw-r--r--   0        0        0      799 2023-06-29 04:26:54.854394 ailingbot-0.0.5/ailingbot/channels/dingtalk/render.py
+-rw-r--r--   0        0        0     4273 2023-06-29 07:16:46.998937 ailingbot-0.0.5/ailingbot/channels/dingtalk/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.5/ailingbot/channels/feishu/__init__.py
+-rw-r--r--   0        0        0     5760 2023-06-29 04:10:57.580967 ailingbot-0.0.5/ailingbot/channels/feishu/agent.py
+-rw-r--r--   0        0        0     1398 2023-06-27 07:03:48.368295 ailingbot-0.0.5/ailingbot/channels/feishu/render.py
+-rw-r--r--   0        0        0     7052 2023-06-29 04:26:54.855074 ailingbot-0.0.5/ailingbot/channels/feishu/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.5/ailingbot/channels/slack/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.5/ailingbot/channels/wechatwork/__init__.py
+-rw-r--r--   0        0        0     4245 2023-06-26 06:57:43.400029 ailingbot-0.0.5/ailingbot/channels/wechatwork/agent.py
+-rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.5/ailingbot/channels/wechatwork/encrypt.py
+-rw-r--r--   0        0        0     2408 2023-06-19 04:30:43.452309 ailingbot-0.0.5/ailingbot/channels/wechatwork/render.py
+-rw-r--r--   0        0        0     5942 2023-06-26 06:57:43.400763 ailingbot-0.0.5/ailingbot/channels/wechatwork/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.5/ailingbot/chat/__init__.py
+-rw-r--r--   0        0        0     2067 2023-06-29 05:19:20.215510 ailingbot-0.0.5/ailingbot/chat/chatbot.py
+-rw-r--r--   0        0        0     3487 2023-06-25 06:38:56.364334 ailingbot-0.0.5/ailingbot/chat/messages.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.5/ailingbot/chat/policies/__init__.py
+-rw-r--r--   0        0        0     5436 2023-06-29 06:24:43.133890 ailingbot-0.0.5/ailingbot/chat/policies/langchain.py
+-rw-r--r--   0        0        0     1678 2023-06-25 07:39:16.611374 ailingbot-0.0.5/ailingbot/chat/policy.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.5/ailingbot/cli/__init__.py
+-rw-r--r--   0        0        0     9511 2023-06-29 08:06:11.693659 ailingbot-0.0.5/ailingbot/cli/cli.py
+-rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.5/ailingbot/cli/options.py
+-rw-r--r--   0        0        0     5347 2023-06-18 13:01:00.251299 ailingbot-0.0.5/ailingbot/cli/render.py
+-rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.5/ailingbot/config.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.5/ailingbot/endpoint/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.5/ailingbot/shared/__init__.py
+-rw-r--r--   0        0        0     3953 2023-06-27 05:30:31.536603 ailingbot-0.0.5/ailingbot/shared/abc.py
+-rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.5/ailingbot/shared/errors.py
+-rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.5/ailingbot/shared/misc.py
+-rw-r--r--   0        0        0     1115 2023-06-29 08:10:51.524952 ailingbot-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    24388 1970-01-01 00:00:00.000000 ailingbot-0.0.5/PKG-INFO
```

### Comparing `ailingbot-0.0.4/LICENSE` & `ailingbot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/README.md` & `ailingbot-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/logo.png" alt="AilingBot" width="300">
 </p>
 
 <p align="center"><b>AilingBot - 一站式解决方案，为你的IM机器人接入AI强大能力。</b></p>
 
+# AilingBot是什么
+
+AilingBot是一个开源的工程开发框架，同时也是IM机器人接入AI模型的一站式解决方案。通过AilingBot你可以：
+
+- ☕**零代码使用**：快速将现有AI大模型能力接入主流IM机器人（如企业微信、飞书、钉钉等），实现通过IM机器人与AI大模型交互以完成业务需求。目前内置了多轮对话和文档知识问答两种能力，未来将内置更多能力
+- 🛠️**二次开发**：AilingBot提供了一套清晰的工程架构、接口定义和必需基础组件，无需从头开始重复开发大模型服务的工程框架，只需实现自己Chat
+  Policy，并通过一些简单的配置，就能完成端到端的AI模型对IM机器人的赋能。同时也支持通过开发自己的Channel扩展到你自己的端（如自己的IM、Web应用或移动端应用）
+
 # 特点
 
 - 💯**开源&免费**：完全开源且免费
 - 📦**开箱即用**：无需开发，预置接入现有主流IM及AI模型的能力
 - 🔗**LangChain友好**：方便集成LangChain
 - 🧩**模块化**：项目采用模块化组织，模块之间通过抽象协议依赖，同类模块实现协议即可即插即用
 - 💻**可扩展**：可以扩展AilingBot的使用场景和能力。例如接入到新的IM，新的AI模型，或者定制自己的对话策略
@@ -233,14 +241,77 @@
 
 完成以上配置后，就可以在飞书中找到机器人，进行对话了：
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/feishu-screenshot.png" alt="企业微信机器人" width="1000"/>
 </p>
 
+## 接入钉钉
+
+下面演示如何快速将上面的机器人接入钉钉。
+
+### 通过Docker
+
+```shell
+git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
+cd ailingbot
+docker build -t ailingbot .
+docker run -d \
+  -e AILINGBOT_POLICY__NAME=lc_conversation \
+  -e AILINGBOT_POLICY__HISTORY_SIZE=5 \
+  -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
+  -e AILINGBOT_CHANNEL__NAME=dingtalk \
+  -e AILINGBOT_CHANNEL__APP_KEY={你的钉钉机器人app key} \
+  -e AILINGBOT_CHANNEL__APP_SECRET={你的钉钉机器人app secret} \
+  -e AILINGBOT_CHANNEL__ROBOT_CODE={你的钉钉机器人robot code} \
+  -p 8080:8080
+  ailingbot poetry run ailingbot serve
+```
+
+### 通过PIP
+
+#### 安装
+
+```shell
+pip install ailingbot
+```
+
+#### 生成配置文件
+
+```shell
+ailingbot init --silence --overwrite
+```
+
+#### 修改配置文件
+
+打开`settings.toml`，将其中的channel部分改为如下，并填入你的飞书真实信息：
+
+```toml
+[channel]
+name = "dingtalk"
+app_key = "" # 填写真实信息
+app_secret = "" # 填写真实信息
+robot_code = "" # 填写真实信息
+```
+
+#### 启动服务
+
+```shell
+ailingbot serve
+```
+
+最后我们需要去钉钉的管理后台，将webhook地址配置好。
+钉钉Webhook的URL为：`http(s)://你的公网IP:8080/webhook/dingtalk/event/`
+
+完成以上配置后，就可以在钉钉中找到机器人，进行对话了：
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/dingtalk-screenshot.png" alt="企业微信机器人" />
+</p>
+
 # 📖使用指南
 
 ## 主要流程
 
 AilingBot的主要处理流程如下图：
 
 <p align="center">
@@ -293,23 +364,23 @@
 - `some_conf.conf_1`的对应环境变量为`AILINGBOT_SOME_CONF__CONF_1`
 - `some_conf.conf_1.subconf`的对应环境变量为`AILINGBOT_SOME_CONF__CONF_1__SUBCONF`
 
 ### 配置项
 
 #### 通用
 
-| 配置项       | 说明                                                                  | TOML                 | 环境变量                            |
-|-----------|---------------------------------------------------------------------|----------------------|---------------------------------|
-| 语言        | 语言码（参考：http://www.lingoes.net/en/translator/langcode.htm）           | lang                 | AILINGBOT_LANG                  |
-| 时区        | 时区码（参考：https://en.wikipedia.org/wiki/List_of_tz_database_time_zones | tz                   | AILINGBOT_TZ                    |
-| 会话策略名称    | 预置会话策略名称或完整会话策略class路径                                              | policy.name          | AILINGBOT_POLICY__NAME          |
-| Channel名称 | 预置Channel名称                                                         | channel.name         | AILINGBOT_CHANNEL__NAME         |
-| Webhook路径 | 非预置Channel webhook的完整class路径                                        | channel.webhook_name | AILINGBOT_CHANNEL__WEBHOOK_NAME |
-| Agent路径   | 非预置Channel agent的完整class路径                                          | channel.agent_name   | AILINGBOT_CHANNEL__AGENT_NAME   |
-| Uvicorn配置 | 所有uvicorn配置（参考：https://www.uvicorn.org/settings/)，这部分配置会透传给uvicorn  | uvicorn.*            | AILINGBOT_CHANNEL__UVICORN__*   |
+| 配置项       | 说明                                                                                     | TOML                 | 环境变量                            |
+|-----------|----------------------------------------------------------------------------------------|----------------------|---------------------------------|
+| 语言        | 语言码（参考：http://www.lingoes.net/en/translator/langcode.htm）                              | lang                 | AILINGBOT_LANG                  |
+| 时区        | 时区码（参考：https://en.wikipedia.org/wiki/List_of_tz_database_time_zones                    | tz                   | AILINGBOT_TZ                    |
+| 会话策略名称    | 预置会话策略名称或完整会话策略class路径                                                                 | policy.name          | AILINGBOT_POLICY__NAME          |
+| Channel名称 | 预置Channel名称                                                                            | channel.name         | AILINGBOT_CHANNEL__NAME         |
+| Webhook路径 | 非预置Channel webhook的完整class路径                                                           | channel.webhook_name | AILINGBOT_CHANNEL__WEBHOOK_NAME |
+| Agent路径   | 非预置Channel agent的完整class路径                                                             | channel.agent_name   | AILINGBOT_CHANNEL__AGENT_NAME   |
+| Uvicorn配置 | 所有uvicorn配置（参考：[uvicorn settings](https://www.uvicorn.org/settings/)），这部分配置会透传给uvicorn | uvicorn.*            | AILINGBOT_CHANNEL__UVICORN__*   |
 
 配置示例：
 
 ```toml
 lang = "zh_CN"
 tz = "Asia/Shanghai"
 
@@ -420,14 +491,32 @@
 [channel]
 name = "feishu"
 app_id = "cli_a**********9d00e"
 app_secret = "y********************cyk8AxmYVDD"
 verification_token = "yIJ********************7bfNHUcYH"
 ```
 
+##### 钉钉
+
+| 配置项        | 说明                | TOML               | 环境变量                          |
+|------------|-------------------|--------------------|-------------------------------|
+| App Key    | 钉钉自建应用的app key    | channel.app_key    | AILINGBOT_CHANNEL__APP_KEY    |
+| App Secret | 钉钉自建应用的app secret | channel.app_secret | AILINGBOT_CHANNEL__APP_SECRET |
+| Robot Code | 钉钉自建应用的robot code | channel.robot_code | AILINGBOT_CHANNEL__ROBOT_CODE |
+
+配置示例：
+
+```toml
+[channel]
+name = "dingtalk"
+app_key = "dingi**********wymdr"
+app_secret = "ombrcUp****************************************GL2AwObLjILUY1MzD"
+robot_code = "ding**********owymdr"
+```
+
 ## 命令行工具
 
 ### 初始化配置文件（init）
 
 #### 使用方法
 
 `init`命令将在当前目录生成配置文件settings.toml。默认情况下，将以交互方式询问用户，
@@ -539,15 +628,27 @@
 ## 开发Channel
 
 TBD
 
 # 发展计划
 
 - [ ] 提供完善的使用文档和开发者文档
-- [ ] 支持更多的IM端，如钉钉、Slack等
+- [ ] 支持更多的Channel
+    - [x] 企业微信
+    - [x] 飞书
+    - [x] 钉钉
+    - [ ] Slack
 - [ ] 开发更多的开箱即用的对话策略
-- [ ] 对向量数据库等常用基础组件做更完善的支持，并支持Grounding能力
+    - [x] 多轮会话策略
+    - [ ] 文档问答策略
+    - [ ] 数据库问答策略
+    - [ ] 在线搜索问答策略
+- [ ] 基础组件抽象
+    - [ ] 大语言模型
+    - [ ] 知识库
+- [ ] 支持本地模型部署
+    - [ ] ChatGLM-6B
 - [ ] 支持通过API调用
 - [ ] Web管理后台及可视化配置管理
-- [ ] 提供基于Docker容器的一键部署能力
+- [x] 提供基于Docker容器的部署能力
 - [ ] 增强系统的可观测性和可治理性
 - [ ] 完善的测试用例
```

### Comparing `ailingbot-0.0.4/ailingbot/channels/channel.py` & `ailingbot-0.0.5/ailingbot/channels/channel.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,32 +12,40 @@
 class ChannelAgent(AbstractAsyncComponent, abc.ABC):
     """Base class of channel agents."""
 
     def __init__(self):
         super(ChannelAgent, self).__init__()
 
     @staticmethod
-    def get_agent(name: str) -> ChannelAgent:
+    def get_agent(
+        name: str, full_class_path: typing.Optional[str] = None
+    ) -> ChannelAgent:
         """Gets channel agent instance.
 
         :param name: Built-in channel name or full path of agent class.
         :type name: str
+        :param full_class_path:
+        :type full_class_path:
         :return: Agent instance.
         :rtype: ChannelAgent
         """
         if name.lower() == 'wechatwork':
             from ailingbot.channels.wechatwork.agent import WechatworkAgent
 
             instance = WechatworkAgent()
         elif name.lower() == 'feishu':
             from ailingbot.channels.feishu.agent import FeishuAgent
 
             instance = FeishuAgent()
+        elif name.lower() == 'dingtalk':
+            from ailingbot.channels.dingtalk.agent import DingtalkAgent
+
+            instance = DingtalkAgent()
         else:
-            instance = get_class_dynamically(name)()
+            instance = get_class_dynamically(full_class_path)()
 
         return instance
 
 
 class ChannelWebhookFactory(abc.ABC):
     """Base class of channel webhook factories."""
 
@@ -50,20 +58,26 @@
         :return: ASGI application.
         :rtype: typing.Union[ASGIApplication, typing.Callable]
         """
         raise NotImplementedError
 
     @staticmethod
     async def get_webhook(
-        name: str, debug: bool = False
+        name: str,
+        full_class_path: typing.Optional[str] = None,
+        debug: bool = False,
     ) -> ASGIApplication | typing.Callable:
         """Gets channel webhook ASGI application instance.
 
         :param name: Built-in channel name or full path of webhook factory class.
         :type name: str
+        :param full_class_path:
+        :type full_class_path:
+        :param debug:
+        :type debug:
         :return: Webhook ASGI application.
         :rtype: typing.Union[ASGIApplication, typing.Callable]
         """
         if name.lower() == 'wechatwork':
             from ailingbot.channels.wechatwork.webhook import (
                 WechatworkWebhookFactory,
             )
@@ -71,11 +85,18 @@
             factory = WechatworkWebhookFactory(debug=debug)
         elif name.lower() == 'feishu':
             from ailingbot.channels.feishu.webhook import (
                 FeishuWebhookFactory,
             )
 
             factory = FeishuWebhookFactory(debug=debug)
+
+        elif name.lower() == 'dingtalk':
+            from ailingbot.channels.dingtalk.webhook import (
+                DingtalkWebhookFactory,
+            )
+
+            factory = DingtalkWebhookFactory(debug=debug)
         else:
-            factory = get_class_dynamically(name)()
+            factory = get_class_dynamically(full_class_path)()
 
         return await factory.create_webhook_app()
```

### Comparing `ailingbot-0.0.4/ailingbot/channels/feishu/agent.py` & `ailingbot-0.0.5/ailingbot/channels/feishu/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/channels/feishu/render.py` & `ailingbot-0.0.5/ailingbot/channels/feishu/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/channels/feishu/webhook.py` & `ailingbot-0.0.5/ailingbot/channels/feishu/webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 
             req_msg.uuid = event.event.message.message_id
             req_msg.sender_id = event.event.sender.sender_id.get('open_id', '')
             if event.event.message.chat_type == 'p2p':
                 req_msg.scope = MessageScope.USER
             elif event.event.message.chat_type == 'group':
                 req_msg.scope = MessageScope.GROUP
-                req_msg.meta['chat_id'] = event.event.message.chat_id
 
             response = await self.bot.chat(
                 conversation_id=conversation_id, message=req_msg
             )
             await self.agent.send_message(response)
 
         @self.app.on_event('startup')
```

### Comparing `ailingbot-0.0.4/ailingbot/channels/wechatwork/agent.py` & `ailingbot-0.0.5/ailingbot/channels/wechatwork/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/channels/wechatwork/encrypt.py` & `ailingbot-0.0.5/ailingbot/channels/wechatwork/encrypt.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/channels/wechatwork/render.py` & `ailingbot-0.0.5/ailingbot/channels/wechatwork/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/channels/wechatwork/webhook.py` & `ailingbot-0.0.5/ailingbot/channels/wechatwork/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/chat/chatbot.py` & `ailingbot-0.0.5/ailingbot/chat/chatbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,27 +43,29 @@
         """
         if conversation_id not in self.locks:
             self.locks[conversation_id] = asyncio.Lock()
         lock = self.locks[conversation_id]
 
         async with lock:
             try:
-                return await self.policy.respond(
+                r = await self.policy.respond(
                     conversation_id=conversation_id, message=message
                 )
             except Exception as e:
                 logger.error(e)
-                return FallbackResponseMessage(
-                    uuid=str(uuid.uuid4()),
-                    ack_uuid=message.uuid,
-                    receiver_id=message.sender_id,
-                    scope=message.scope,
-                    echo=message.echo,
+                r = FallbackResponseMessage(
                     reason=str(e),
                 )
+            r.uuid = str(uuid.uuid4())
+            r.ack_uuid = message.uuid
+            r.receiver_id = message.sender_id
+            r.scope = message.scope
+            r.echo = message.echo
+
+            return r
 
     async def _initialize(self) -> None:
         self.policy = ChatPolicy.get_policy(
             name=settings.policy.name,
             debug=self.debug,
         )
         await self.policy.initialize()
```

### Comparing `ailingbot-0.0.4/ailingbot/chat/messages.py` & `ailingbot-0.0.5/ailingbot/chat/messages.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/chat/policies/langchain.py` & `ailingbot-0.0.5/ailingbot/chat/policies/langchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import copy
 import tempfile
-import uuid
 
 from langchain import ConversationChain
 from langchain.chains import RetrievalQA
 from langchain.chains.base import Chain
 from langchain.document_loaders import PyPDFLoader
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.llms.loading import load_llm_from_config
@@ -39,15 +38,15 @@
         super(LCConversationChatPolicy, self).__init__(
             debug=debug,
         )
 
         llm_config = copy.deepcopy(settings.policy.llm)
         llm = load_llm_from_config(llm_config)
         self.chain = ConversationChain(llm=llm, verbose=debug)
-        self.history_size = settings.policy.history_size or 5
+        self.history_size = settings.policy.get('history_size', 5)
         self.memories: dict[str, BaseChatMemory] = {}
 
     async def _load_memory(self, *, conversation_id: str) -> BaseChatMemory:
         """Load memory for conversation. Create a new memory if not exists.
 
         :param conversation_id: Conversation ID.
         :type conversation_id: str
@@ -69,19 +68,14 @@
         else:
             if conversation_id not in self.chain:
                 self.chain.memory = await self._load_memory(
                     conversation_id=conversation_id
                 )
             response = TextResponseMessage()
             response.text = await self.chain.arun(message.text)
-        response.uuid = str(uuid.uuid4())
-        response.ack_uuid = message.uuid
-        response.receiver_id = message.sender_id
-        response.scope = message.scope
-        response.echo = message.echo
 
         return response
 
 
 class LCDocumentQAPolicy(ChatPolicy):
     """Question-Answering based on documents."""
 
@@ -93,16 +87,16 @@
         super(LCDocumentQAPolicy, self).__init__(
             debug=debug,
         )
 
         llm_config = copy.deepcopy(settings.policy.llm)
         self.llm = load_llm_from_config(llm_config)
         self.chains: dict[str, Chain] = {}
-        self.chunk_size = settings.policy.chunk_size or 1000
-        self.chunk_overlap = settings.policy.chunk_overlap or 0
+        self.chunk_size = settings.policy.get('chunk_size', 1000)
+        self.chunk_overlap = settings.policy.get('chunk_overlap', 0)
 
     def _build_documents_index(
         self, *, content: bytes, file_type: str
     ) -> VectorStoreRetriever:
         """Load document and build index."""
         if file_type.lower() != 'pdf':
             raise ailingbot.shared.errors.ChatPolicyError(
@@ -152,14 +146,8 @@
             )
             response = TextResponseMessage()
             response.text = f'我已完成学习，现在可以针对 {message.file_name} 进行提问了'
         else:
             response = FallbackResponseMessage()
             response.reason = '不支持的消息类型'
 
-        response.uuid = str(uuid.uuid4())
-        response.ack_uuid = message.uuid
-        response.receiver_id = message.sender_id
-        response.scope = message.scope
-        response.echo = message.echo
-
         return response
```

### Comparing `ailingbot-0.0.4/ailingbot/chat/policy.py` & `ailingbot-0.0.5/ailingbot/chat/policy.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/cli/cli.py` & `ailingbot-0.0.5/ailingbot/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,17 @@
     log_level: str,
     log_file: str,
     debug: bool,
 ):
     _set_logger(sink=log_file, level=log_level)
 
     webhook = await ChannelWebhookFactory.get_webhook(
-        settings.channel.name, debug=debug
+        settings.channel.name,
+        settings.channel.get('webhook_name', None),
+        debug=debug,
     )
 
     config = uvicorn.Config(app=webhook, **settings.uvicorn)
     server = uvicorn.Server(config)
     await server.serve()
 
 
@@ -316,14 +318,21 @@
         elif channel == 'feishu':
             config['channel'] = {
                 'name': 'feishu',
                 'app_id': '',
                 'app_secret': '',
                 'verification_token': 0,
             }
+        elif channel == 'dingtalk':
+            config['channel'] = {
+                'name': 'dingtalk',
+                'app_key': '',
+                'app_secret': '',
+                'robot_code': '',
+            }
 
     with open(file_path, 'w') as f:
         f.write(tomlkit.dumps(config))
     click.echo(
         click.style(
             text=f'Configuration file {file_path} has been created.',
             fg='green',
```

### Comparing `ailingbot-0.0.4/ailingbot/cli/options.py` & `ailingbot-0.0.5/ailingbot/cli/options.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/cli/render.py` & `ailingbot-0.0.5/ailingbot/cli/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/config.py` & `ailingbot-0.0.5/ailingbot/config.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/shared/abc.py` & `ailingbot-0.0.5/ailingbot/shared/abc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/shared/errors.py` & `ailingbot-0.0.5/ailingbot/shared/errors.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/ailingbot/shared/misc.py` & `ailingbot-0.0.5/ailingbot/shared/misc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.4/pyproject.toml` & `ailingbot-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ailingbot"
-version = "0.0.4"
+version = "0.0.5"
 description = "An all-in-one solution to empower your IM bot with AI."
 authors = ["ericzhang-cn <ericzhang.buaa@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `ailingbot-0.0.4/PKG-INFO` & `ailingbot-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ailingbot
-Version: 0.0.4
+Version: 0.0.5
 Summary: An all-in-one solution to empower your IM bot with AI.
 License: MIT
 Author: ericzhang-cn
 Author-email: ericzhang.buaa@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -44,14 +44,22 @@
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/logo.png" alt="AilingBot" width="300">
 </p>
 
 <p align="center"><b>AilingBot - 一站式解决方案，为你的IM机器人接入AI强大能力。</b></p>
 
+# AilingBot是什么
+
+AilingBot是一个开源的工程开发框架，同时也是IM机器人接入AI模型的一站式解决方案。通过AilingBot你可以：
+
+- ☕**零代码使用**：快速将现有AI大模型能力接入主流IM机器人（如企业微信、飞书、钉钉等），实现通过IM机器人与AI大模型交互以完成业务需求。目前内置了多轮对话和文档知识问答两种能力，未来将内置更多能力
+- 🛠️**二次开发**：AilingBot提供了一套清晰的工程架构、接口定义和必需基础组件，无需从头开始重复开发大模型服务的工程框架，只需实现自己Chat
+  Policy，并通过一些简单的配置，就能完成端到端的AI模型对IM机器人的赋能。同时也支持通过开发自己的Channel扩展到你自己的端（如自己的IM、Web应用或移动端应用）
+
 # 特点
 
 - 💯**开源&免费**：完全开源且免费
 - 📦**开箱即用**：无需开发，预置接入现有主流IM及AI模型的能力
 - 🔗**LangChain友好**：方便集成LangChain
 - 🧩**模块化**：项目采用模块化组织，模块之间通过抽象协议依赖，同类模块实现协议即可即插即用
 - 💻**可扩展**：可以扩展AilingBot的使用场景和能力。例如接入到新的IM，新的AI模型，或者定制自己的对话策略
@@ -273,14 +281,77 @@
 
 完成以上配置后，就可以在飞书中找到机器人，进行对话了：
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/feishu-screenshot.png" alt="企业微信机器人" width="1000"/>
 </p>
 
+## 接入钉钉
+
+下面演示如何快速将上面的机器人接入钉钉。
+
+### 通过Docker
+
+```shell
+git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
+cd ailingbot
+docker build -t ailingbot .
+docker run -d \
+  -e AILINGBOT_POLICY__NAME=lc_conversation \
+  -e AILINGBOT_POLICY__HISTORY_SIZE=5 \
+  -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
+  -e AILINGBOT_CHANNEL__NAME=dingtalk \
+  -e AILINGBOT_CHANNEL__APP_KEY={你的钉钉机器人app key} \
+  -e AILINGBOT_CHANNEL__APP_SECRET={你的钉钉机器人app secret} \
+  -e AILINGBOT_CHANNEL__ROBOT_CODE={你的钉钉机器人robot code} \
+  -p 8080:8080
+  ailingbot poetry run ailingbot serve
+```
+
+### 通过PIP
+
+#### 安装
+
+```shell
+pip install ailingbot
+```
+
+#### 生成配置文件
+
+```shell
+ailingbot init --silence --overwrite
+```
+
+#### 修改配置文件
+
+打开`settings.toml`，将其中的channel部分改为如下，并填入你的飞书真实信息：
+
+```toml
+[channel]
+name = "dingtalk"
+app_key = "" # 填写真实信息
+app_secret = "" # 填写真实信息
+robot_code = "" # 填写真实信息
+```
+
+#### 启动服务
+
+```shell
+ailingbot serve
+```
+
+最后我们需要去钉钉的管理后台，将webhook地址配置好。
+钉钉Webhook的URL为：`http(s)://你的公网IP:8080/webhook/dingtalk/event/`
+
+完成以上配置后，就可以在钉钉中找到机器人，进行对话了：
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/dingtalk-screenshot.png" alt="企业微信机器人" />
+</p>
+
 # 📖使用指南
 
 ## 主要流程
 
 AilingBot的主要处理流程如下图：
 
 <p align="center">
@@ -333,23 +404,23 @@
 - `some_conf.conf_1`的对应环境变量为`AILINGBOT_SOME_CONF__CONF_1`
 - `some_conf.conf_1.subconf`的对应环境变量为`AILINGBOT_SOME_CONF__CONF_1__SUBCONF`
 
 ### 配置项
 
 #### 通用
 
-| 配置项       | 说明                                                                  | TOML                 | 环境变量                            |
-|-----------|---------------------------------------------------------------------|----------------------|---------------------------------|
-| 语言        | 语言码（参考：http://www.lingoes.net/en/translator/langcode.htm）           | lang                 | AILINGBOT_LANG                  |
-| 时区        | 时区码（参考：https://en.wikipedia.org/wiki/List_of_tz_database_time_zones | tz                   | AILINGBOT_TZ                    |
-| 会话策略名称    | 预置会话策略名称或完整会话策略class路径                                              | policy.name          | AILINGBOT_POLICY__NAME          |
-| Channel名称 | 预置Channel名称                                                         | channel.name         | AILINGBOT_CHANNEL__NAME         |
-| Webhook路径 | 非预置Channel webhook的完整class路径                                        | channel.webhook_name | AILINGBOT_CHANNEL__WEBHOOK_NAME |
-| Agent路径   | 非预置Channel agent的完整class路径                                          | channel.agent_name   | AILINGBOT_CHANNEL__AGENT_NAME   |
-| Uvicorn配置 | 所有uvicorn配置（参考：https://www.uvicorn.org/settings/)，这部分配置会透传给uvicorn  | uvicorn.*            | AILINGBOT_CHANNEL__UVICORN__*   |
+| 配置项       | 说明                                                                                     | TOML                 | 环境变量                            |
+|-----------|----------------------------------------------------------------------------------------|----------------------|---------------------------------|
+| 语言        | 语言码（参考：http://www.lingoes.net/en/translator/langcode.htm）                              | lang                 | AILINGBOT_LANG                  |
+| 时区        | 时区码（参考：https://en.wikipedia.org/wiki/List_of_tz_database_time_zones                    | tz                   | AILINGBOT_TZ                    |
+| 会话策略名称    | 预置会话策略名称或完整会话策略class路径                                                                 | policy.name          | AILINGBOT_POLICY__NAME          |
+| Channel名称 | 预置Channel名称                                                                            | channel.name         | AILINGBOT_CHANNEL__NAME         |
+| Webhook路径 | 非预置Channel webhook的完整class路径                                                           | channel.webhook_name | AILINGBOT_CHANNEL__WEBHOOK_NAME |
+| Agent路径   | 非预置Channel agent的完整class路径                                                             | channel.agent_name   | AILINGBOT_CHANNEL__AGENT_NAME   |
+| Uvicorn配置 | 所有uvicorn配置（参考：[uvicorn settings](https://www.uvicorn.org/settings/)），这部分配置会透传给uvicorn | uvicorn.*            | AILINGBOT_CHANNEL__UVICORN__*   |
 
 配置示例：
 
 ```toml
 lang = "zh_CN"
 tz = "Asia/Shanghai"
 
@@ -460,14 +531,32 @@
 [channel]
 name = "feishu"
 app_id = "cli_a**********9d00e"
 app_secret = "y********************cyk8AxmYVDD"
 verification_token = "yIJ********************7bfNHUcYH"
 ```
 
+##### 钉钉
+
+| 配置项        | 说明                | TOML               | 环境变量                          |
+|------------|-------------------|--------------------|-------------------------------|
+| App Key    | 钉钉自建应用的app key    | channel.app_key    | AILINGBOT_CHANNEL__APP_KEY    |
+| App Secret | 钉钉自建应用的app secret | channel.app_secret | AILINGBOT_CHANNEL__APP_SECRET |
+| Robot Code | 钉钉自建应用的robot code | channel.robot_code | AILINGBOT_CHANNEL__ROBOT_CODE |
+
+配置示例：
+
+```toml
+[channel]
+name = "dingtalk"
+app_key = "dingi**********wymdr"
+app_secret = "ombrcUp****************************************GL2AwObLjILUY1MzD"
+robot_code = "ding**********owymdr"
+```
+
 ## 命令行工具
 
 ### 初始化配置文件（init）
 
 #### 使用方法
 
 `init`命令将在当前目录生成配置文件settings.toml。默认情况下，将以交互方式询问用户，
@@ -579,16 +668,28 @@
 ## 开发Channel
 
 TBD
 
 # 发展计划
 
 - [ ] 提供完善的使用文档和开发者文档
-- [ ] 支持更多的IM端，如钉钉、Slack等
+- [ ] 支持更多的Channel
+    - [x] 企业微信
+    - [x] 飞书
+    - [x] 钉钉
+    - [ ] Slack
 - [ ] 开发更多的开箱即用的对话策略
-- [ ] 对向量数据库等常用基础组件做更完善的支持，并支持Grounding能力
+    - [x] 多轮会话策略
+    - [ ] 文档问答策略
+    - [ ] 数据库问答策略
+    - [ ] 在线搜索问答策略
+- [ ] 基础组件抽象
+    - [ ] 大语言模型
+    - [ ] 知识库
+- [ ] 支持本地模型部署
+    - [ ] ChatGLM-6B
 - [ ] 支持通过API调用
 - [ ] Web管理后台及可视化配置管理
-- [ ] 提供基于Docker容器的一键部署能力
+- [x] 提供基于Docker容器的部署能力
 - [ ] 增强系统的可观测性和可治理性
 - [ ] 完善的测试用例
```

