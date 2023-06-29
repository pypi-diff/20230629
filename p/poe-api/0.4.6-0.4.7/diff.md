# Comparing `tmp/poe_api-0.4.6-py3-none-any.whl.zip` & `tmp/poe_api-0.4.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 40873 bytes, number of entries: 42
--rw-r--r--  2.0 unx    21094 b- defN 23-Jun-09 20:19 poe.py
+Zip file size: 40992 bytes, number of entries: 42
+-rw-r--r--  2.0 unx    21681 b- defN 23-Jun-29 06:05 poe.py
 -rw-r--r--  2.0 unx     1093 b- defN 23-May-27 23:16 poe_graphql/AddHumanMessageMutation.graphql
 -rw-r--r--  2.0 unx      504 b- defN 23-Jun-04 03:20 poe_graphql/AddMessageBreakMutation.graphql
 -rw-r--r--  2.0 unx      180 b- defN 23-May-27 23:16 poe_graphql/AutoSubscriptionMutation.graphql
 -rw-r--r--  2.0 unx       97 b- defN 23-May-27 23:16 poe_graphql/BioFragment.graphql
 -rw-r--r--  2.0 unx       73 b- defN 23-May-27 23:16 poe_graphql/ChatAddedSubscription.graphql
 -rw-r--r--  2.0 unx      100 b- defN 23-May-27 23:16 poe_graphql/ChatFragment.graphql
 -rw-r--r--  2.0 unx    11486 b- defN 23-Jun-04 03:16 poe_graphql/ChatListPaginationQuery.graphql
@@ -32,13 +32,13 @@
 -rw-r--r--  2.0 unx      147 b- defN 23-May-27 23:16 poe_graphql/SummarizeQuotePostQuery.graphql
 -rw-r--r--  2.0 unx      180 b- defN 23-May-27 23:16 poe_graphql/SummarizeSharePostQuery.graphql
 -rw-r--r--  2.0 unx      368 b- defN 23-May-27 23:16 poe_graphql/UserSnippetFragment.graphql
 -rw-r--r--  2.0 unx      400 b- defN 23-May-27 23:16 poe_graphql/ViewerInfoQuery.graphql
 -rw-r--r--  2.0 unx     1038 b- defN 23-May-27 23:16 poe_graphql/ViewerStateFragment.graphql
 -rw-r--r--  2.0 unx      657 b- defN 23-May-27 23:16 poe_graphql/ViewerStateUpdatedSubscription.graphql
 -rw-r--r--  2.0 unx        0 b- defN 23-May-27 23:16 poe_graphql/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jun-09 20:21 poe_api-0.4.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    18099 b- defN 23-Jun-09 20:21 poe_api-0.4.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 20:21 poe_api-0.4.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-09 20:21 poe_api-0.4.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3969 b- defN 23-Jun-09 20:21 poe_api-0.4.6.dist-info/RECORD
-42 files, 104697 bytes uncompressed, 34331 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-29 06:08 poe_api-0.4.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18103 b- defN 23-Jun-29 06:08 poe_api-0.4.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 06:08 poe_api-0.4.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 06:08 poe_api-0.4.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3969 b- defN 23-Jun-29 06:08 poe_api-0.4.7.dist-info/RECORD
+42 files, 105288 bytes uncompressed, 34450 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -105,23 +105,23 @@
 
 Filename: poe_graphql/ViewerStateUpdatedSubscription.graphql
 Comment: 
 
 Filename: poe_graphql/__init__.py
 Comment: 
 
-Filename: poe_api-0.4.6.dist-info/LICENSE
+Filename: poe_api-0.4.7.dist-info/LICENSE
 Comment: 
 
-Filename: poe_api-0.4.6.dist-info/METADATA
+Filename: poe_api-0.4.7.dist-info/METADATA
 Comment: 
 
-Filename: poe_api-0.4.6.dist-info/WHEEL
+Filename: poe_api-0.4.7.dist-info/WHEEL
 Comment: 
 
-Filename: poe_api-0.4.6.dist-info/top_level.txt
+Filename: poe_api-0.4.7.dist-info/top_level.txt
 Comment: 
 
-Filename: poe_api-0.4.6.dist-info/RECORD
+Filename: poe_api-0.4.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## poe.py

```diff
@@ -191,26 +191,31 @@
     r = request_with_retries(self.session.get, self.home_url)
     json_regex = r'<script id="__NEXT_DATA__" type="application\/json">(.+?)</script>'
     json_text = re.search(json_regex, r.text).group(1)
     next_data = json.loads(json_text)
 
     if overwrite_vars:
       self.formkey = self.extract_formkey(r.text)
-      self.viewer = next_data["props"]["pageProps"]["payload"]["viewer"]
+      if "payload" in next_data["props"]["pageProps"]:
+        self.viewer = next_data["props"]["pageProps"]["payload"]["viewer"]
+      else:
+        self.viewer = next_data["props"]["pageProps"]["data"]["viewer"]
       self.user_id = self.viewer["poeUser"]["id"]
       self.next_data = next_data
 
     return next_data
   
   def get_bot(self, display_name):
     url = f'https://poe.com/_next/data/{self.next_data["buildId"]}/{display_name}.json'
     
-    r = request_with_retries(self.session.get, url)
-
-    chat_data = r.json()["pageProps"]["payload"]["chatOfBotDisplayName"]
+    data = request_with_retries(self.session.get, url).json()
+    if "payload" in data["pageProps"]:
+      chat_data = data["pageProps"]["payload"]["chatOfBotDisplayName"]
+    else:
+      chat_data = data["pageProps"]["data"]["chatOfBotDisplayName"]
     return chat_data
     
   def get_bots(self, download_next_data=True):
     logger.info("Downloading all bots...")
     if download_next_data:
       next_data = self.get_next_data(overwrite_vars=True)
     else:
@@ -254,21 +259,26 @@
       bot_obj = self.bots[bot_nickname]["defaultBotObject"]
       bot_names[bot_nickname] = bot_obj["displayName"]
     return bot_names
   
   def explore_bots(self, end_cursor=None, count=25):
     if not end_cursor:
       url = f'https://poe.com/_next/data/{self.next_data["buildId"]}/explore_bots.json'
-      r = request_with_retries(self.session.get, url)
-      nodes = r.json()["pageProps"]["payload"]["exploreBotsConnection"]["edges"]
+      r = request_with_retries(self.session.get, url).json()
+      if "payload" in r["pageProps"]:
+        key = "payload"
+        nodes = r["pageProps"]["payload"]["exploreBotsConnection"]["edges"]
+      else:
+        key = "data"
+        nodes = r["pageProps"]["data"]["exploreBotsConnection"]["edges"]
       bots = [node["node"] for node in nodes]
       bots = bots[:count]
       return {
         "bots": bots,
-        "end_cursor": r.json()["pageProps"]["payload"]["exploreBotsConnection"]["pageInfo" ]["endCursor"],
+        "end_cursor": r["pageProps"][key]["exploreBotsConnection"]["pageInfo" ]["endCursor"],
       }
 
     else:
       # Use graphql to get the next page
       result = self.send_query("ExploreBotsListPaginationQuery", {
         "count": count, 
         "cursor": end_cursor
@@ -344,14 +354,18 @@
       proxy_parsed = urlparse(self.proxy)
       kwargs = {
         "proxy_type": proxy_parsed.scheme,
         "http_proxy_host": proxy_parsed.hostname,
         "http_proxy_port": proxy_parsed.port
       }
 
+      # auth if exists
+      if proxy_parsed.username and proxy_parsed.password:
+        kwargs["http_proxy_auth"] = (proxy_parsed.username, proxy_parsed.password)
+
     self.ws.run_forever(**kwargs)
 
   def connect_ws(self, timeout=5):
     if self.ws_connected:
       return
 
     if self.ws_connecting:
```

## Comparing `poe_api-0.4.6.dist-info/LICENSE` & `poe_api-0.4.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `poe_api-0.4.6.dist-info/METADATA` & `poe_api-0.4.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: poe-api
-Version: 0.4.6
+Version: 0.4.7
 Summary: A reverse engineered API wrapper for Quora's Poe
 Home-page: https://github.com/ading2210/poe-api
 Author: ading2210
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: python-socks
+License-File: LICENSE
+Requires-Dist: websocket-client
 Requires-Dist: requests[socks]
+Requires-Dist: python-socks
 Requires-Dist: tls-client
-Requires-Dist: websocket-client
 
 # Python Poe API
 
 [![PyPi Version](https://img.shields.io/pypi/v/poe-api.svg)](https://pypi.org/project/poe-api/)
 
 This is a reverse engineered API wrapper for Quora's Poe, which allows you free access to OpenAI's ChatGPT and GPT-4, as well as Anthropic's Claude.
 
@@ -243,15 +243,15 @@
 The function returns the message which represents the chat break.
 
 #### Downloading Conversation History:
 To download past messages in a conversation, use the `client.get_message_history` function, which accepts the following arguments:
  - `chatbot` - The codename of the chatbot.
  - `count = 25` - The number of messages to download.
  - `cursor = None` - The message ID to start at instead of the latest one.
-
+ 
 Note that if you don't specify a cursor, the client will have to perform an extra request to determine what the latest cursor is.
 
 The returned messages are ordered from oldest to newest. 
 
 ```python
 message_history = client.get_message_history("capybara", count=10)
 print(json.dumps(message_history, indent=2))
@@ -411,8 +411,7 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ```
-
```

## Comparing `poe_api-0.4.6.dist-info/RECORD` & `poe_api-0.4.7.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-poe.py,sha256=CQ4qwqH49eDzNumBwiKITQzgLivG6DiX0Ja4etOhZNI,21094
+poe.py,sha256=vty7y4zUbHJ4cvVotLagR5FbVyu40KWMKp9MNEDwZeY,21681
 poe_graphql/AddHumanMessageMutation.graphql,sha256=Va4SoysKE2qPlJfbwoKp6mNv0vs5hnVR20g8hPvAxdY,1093
 poe_graphql/AddMessageBreakMutation.graphql,sha256=lFDgYYX0ZTHso-ZQwm-oUk-HaSTRqOmj-zIjBQRL2sM,504
 poe_graphql/AutoSubscriptionMutation.graphql,sha256=3i8EnqwUrjOcJ2Hxly-lKhwPBJdbpO99POiM_K6jVD4,180
 poe_graphql/BioFragment.graphql,sha256=3ZdXaPtuHK38bG10WFH6bvpebcyrTLu5fs-ddtfLjf0,97
 poe_graphql/ChatAddedSubscription.graphql,sha256=NFLZJAwi0V2WQea1oelyRUrtNrwOE58NOeX8ChzVE10,73
 poe_graphql/ChatFragment.graphql,sha256=NFVSvT3NdYlEquue3yTHPu9ezCIgx6k1OXJZo2ytIzU,100
 poe_graphql/ChatListPaginationQuery.graphql,sha256=WameJV_yyS6Ey_VKn7okXAzR45AE9wOB2U6QlRgp-M4,11486
@@ -31,12 +31,12 @@
 poe_graphql/SummarizeQuotePostQuery.graphql,sha256=V4PQ1XkEDCsVR3z7h4SLsonZsWG7RptFd6JPwlGwOvE,147
 poe_graphql/SummarizeSharePostQuery.graphql,sha256=iCN8oiUUp2jfsiBxmsTA7k3_60E0MNwA5gnNrhnYpJc,180
 poe_graphql/UserSnippetFragment.graphql,sha256=Eg8rK7XM6-HqVJkpEBY0bJaYqF-FdDdWdg-Jj3VTnF0,368
 poe_graphql/ViewerInfoQuery.graphql,sha256=Xtn-VGGiknKgrW81s7YfIJwhmilobrSqiCObpoJdYfw,400
 poe_graphql/ViewerStateFragment.graphql,sha256=aicUJncsRpPBh_L2xqDv0aHcUIPIsDrDFPfDs3jcFoU,1038
 poe_graphql/ViewerStateUpdatedSubscription.graphql,sha256=1dPs0WuOLl4ybZXm4bUF60eVc94O10EkKOtqnQYODic,657
 poe_graphql/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-poe_api-0.4.6.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-poe_api-0.4.6.dist-info/METADATA,sha256=4CQN1BC_CGbWIubizQw7-fRDpIilWRGDqHEyndyY_gw,18099
-poe_api-0.4.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-poe_api-0.4.6.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
-poe_api-0.4.6.dist-info/RECORD,,
+poe_api-0.4.7.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+poe_api-0.4.7.dist-info/METADATA,sha256=b5Yir6Qz7hZX2UGEqerz70NeQVnQeFq4QML2n-3PA6U,18103
+poe_api-0.4.7.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+poe_api-0.4.7.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
+poe_api-0.4.7.dist-info/RECORD,,
```

