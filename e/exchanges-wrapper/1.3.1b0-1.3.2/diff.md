# Comparing `tmp/exchanges_wrapper-1.3.1b0.tar.gz` & `tmp/exchanges_wrapper-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges_wrapper-1.3.1b0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "exchanges_wrapper-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `exchanges_wrapper-1.3.1b0.tar` & `exchanges_wrapper-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1114 2023-06-21 11:42:27.744918 exchanges_wrapper-1.3.1b0/LICENSE.md
--rw-r--r--   0        0        0     6941 2023-06-21 11:42:27.744918 exchanges_wrapper-1.3.1b0/README.md
--rw-r--r--   0        0        0     1319 2023-06-21 11:42:27.744918 exchanges_wrapper-1.3.1b0/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    45215 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/api_pb2.py
--rw-r--r--   0        0        0    44445 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/api_pb2_grpc.py
--rw-r--r--   0        0        0    19618 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0     6048 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/c_structures.py
--rw-r--r--   0        0        0    61936 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2601 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12494 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    43819 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     4189 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    10270 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    15723 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/huobi_parser.py
--rw-r--r--   0        0        0    16098 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    12097 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/proto/exchanges_wrapper/api.proto
--rw-r--r--   0        0        0    22384 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0     1121 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/pyproject.toml
--rw-r--r--   0        0        0     7822 1970-01-01 00:00:00.000000 exchanges_wrapper-1.3.1b0/PKG-INFO
+-rw-r--r--   0        0        0     1114 2023-06-29 17:23:13.074875 exchanges_wrapper-1.3.2/LICENSE.md
+-rw-r--r--   0        0        0     7142 2023-06-29 17:23:13.074875 exchanges_wrapper-1.3.2/README.md
+-rw-r--r--   0        0        0     1317 2023-06-29 17:23:13.074875 exchanges_wrapper-1.3.2/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    45215 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/api_pb2.py
+-rw-r--r--   0        0        0    44445 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/api_pb2_grpc.py
+-rw-r--r--   0        0        0    19618 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/bitfinex_parser.py
+-rw-r--r--   0        0        0     6184 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/c_structures.py
+-rw-r--r--   0        0        0    62117 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2768 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12494 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    48580 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     4429 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    10270 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/http_client.py
+-rw-r--r--   0        0        0    15723 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/huobi_parser.py
+-rw-r--r--   0        0        0    16098 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/okx_parser.py
+-rw-r--r--   0        0        0    12097 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/proto/exchanges_wrapper/api.proto
+-rw-r--r--   0        0        0    22397 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0      612 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/ws_api/__init__.py
+-rw-r--r--   0        0        0     8315 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/ws_api/ws_session.py
+-rw-r--r--   0        0        0     1147 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8054 1970-01-01 00:00:00.000000 exchanges_wrapper-1.3.2/PKG-INFO
```

### Comparing `exchanges_wrapper-1.3.1b0/LICENSE.md` & `exchanges_wrapper-1.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.1b0/README.md` & `exchanges_wrapper-1.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 <a href="https://badge.fury.io/py/exchanges-wrapper"><img src="https://badge.fury.io/py/exchanges-wrapper.svg" alt="PyPI version"></a>
 <a href="https://codeclimate.com/github/DogsTailFarmer/exchanges-wrapper/maintainability"><img src="https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/maintainability" /></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=resolved+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=active+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_exchanges-wrapper" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_exchanges-wrapper&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/exchanges-wrapper" target="_blank"><img alt="Downloads" title="Downloads" src="https://pepy.tech/badge/exchanges-wrapper/month"/></a>
 ***
-From 1.2.10 update exch_srv_cfg.toml (see CHANGELOG for details)
+From 1.3.2 update exch_srv_cfg.toml (see [CHANGELOG](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/master/CHANGELOG.md#added-for-new-features) for details)
 ***
 
 ## exchanges-wrapper vs binance.py
 The main difference is the development of the project for trading with many exchanges.
 
 Next is adding a new module ```exchanges_wrapper/exch_srv.py``` as a multiplexer layer, providing simultaneous async interaction for many accounts
 and many trading pairs through one connection. It's powered by [gRPC](https://grpc.io/about/)
@@ -41,14 +41,15 @@
 
 ### Added Features
 - Multi exchanges support
 - Adaptive algorithm to ensure maximum performance and avoid exceeding the rates limits
 - Passthrough logging
 - WSS keepalive
 - Reuse session for new client sessions
+- Utilizing Websocket API (bidirectional) for the most commonly used methods (Binance ws-api/v3, )
 
 ## Extra exchanges implementation features
 - Binance REST API and WSS are accepted as basic, connection of other exchanges wrapped their API to Binance compatible
 - For other, some data cannot be obtained by directly calling one method, it is generated by a synthetic or calculation
 method
 - Some exchanges have not any testing or "paper trading" features, therefore, application development and testing is possible only
 at real bidding. First, run applications on the [Binance Spot Test Network](https://testnet.binance.vision/) or (Bitfinex, OKX) test account.
```

#### html2text {}

```diff
@@ -3,31 +3,34 @@
                                 Logo%202v3.svg]
 ***
     ****** Crypto exchanges API/WSS wrapper with grpc powered server ******
                   ***** Binance, Bitfinex, Huobi, OKX, *****
                           **** For SPOT markets ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/
 maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** From
-1.2.10 update exch_srv_cfg.toml (see CHANGELOG for details) *** ## exchanges-
-wrapper vs binance.py The main difference is the development of the project for
-trading with many exchanges. Next is adding a new module ```exchanges_wrapper/
-exch_srv.py``` as a multiplexer layer, providing simultaneous async interaction
-for many accounts and many trading pairs through one connection. It's powered
-by [gRPC](https://grpc.io/about/) Remote Procedure Call framework. Warning.
-Coverage of overridden binance.py packages is significant but not complete.
-Served methods describes into ```example/exch_client.py``` ### Initial
-capabilities (inherited from binance.py) - Covers general endpoints (test
-connectivity and get exchange information's) - Covers market data endpoints -
-Covers Account endpoints (create and manage orders) - Covers user data stream
-(receive real time user updates) - Covers web socket streams (receive real time
-market updates) - Async support - Auto reconnect after exchanges API or network
-failure - Completely free and without limitations ### Added Features - Multi
-exchanges support - Adaptive algorithm to ensure maximum performance and avoid
-exceeding the rates limits - Passthrough logging - WSS keepalive - Reuse
-session for new client sessions ## Extra exchanges implementation features -
+1.3.2 update exch_srv_cfg.toml (see [CHANGELOG](https://github.com/
+DogsTailFarmer/exchanges-wrapper/blob/master/CHANGELOG.md#added-for-new-
+features) for details) *** ## exchanges-wrapper vs binance.py The main
+difference is the development of the project for trading with many exchanges.
+Next is adding a new module ```exchanges_wrapper/exch_srv.py``` as a
+multiplexer layer, providing simultaneous async interaction for many accounts
+and many trading pairs through one connection. It's powered by [gRPC](https://
+grpc.io/about/) Remote Procedure Call framework. Warning. Coverage of
+overridden binance.py packages is significant but not complete. Served methods
+describes into ```example/exch_client.py``` ### Initial capabilities (inherited
+from binance.py) - Covers general endpoints (test connectivity and get exchange
+information's) - Covers market data endpoints - Covers Account endpoints
+(create and manage orders) - Covers user data stream (receive real time user
+updates) - Covers web socket streams (receive real time market updates) - Async
+support - Auto reconnect after exchanges API or network failure - Completely
+free and without limitations ### Added Features - Multi exchanges support -
+Adaptive algorithm to ensure maximum performance and avoid exceeding the rates
+limits - Passthrough logging - WSS keepalive - Reuse session for new client
+sessions - Utilizing Websocket API (bidirectional) for the most commonly used
+methods (Binance ws-api/v3, ) ## Extra exchanges implementation features -
 Binance REST API and WSS are accepted as basic, connection of other exchanges
 wrapped their API to Binance compatible - For other, some data cannot be
 obtained by directly calling one method, it is generated by a synthetic or
 calculation method - Some exchanges have not any testing or "paper trading"
 features, therefore, application development and testing is possible only at
 real bidding. First, run applications on the [Binance Spot Test Network](https:
 //testnet.binance.vision/) or (Bitfinex, OKX) test account. ## Get started ###
```

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/__init__.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.3.1b0"
+__version__ = "1.3.2"
 
 from pathlib import Path
 import shutil
 
 WORK_PATH = Path(Path.home(), ".MartinBinance")
 CONFIG_PATH = Path(WORK_PATH, "config")
 CONFIG_FILE = Path(CONFIG_PATH, "exch_srv_cfg.toml")
```

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/api_pb2.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/api_pb2.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/api_pb2_grpc.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/bitfinex_parser.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/bitfinex_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/c_structures.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/c_structures.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 
 def generate_signature(exchange, api_secret, data):
     if exchange == 'bitfinex':
         sig = hmac.new(api_secret.encode("utf-8"), data.encode("utf-8"), hashlib.sha384).hexdigest()
     elif exchange in ('huobi', 'okx'):
         sig = hmac.new(api_secret.encode("utf-8"), data.encode("utf-8"), hashlib.sha256).digest()
         sig = base64.b64encode(sig).decode()
+    elif exchange == 'binance_ws':
+        sig = hmac.new(api_secret.encode("ascii"), data.encode("ascii"), hashlib.sha256).hexdigest()
     else:
         sig = hmac.new(api_secret.encode("utf-8"), data.encode("utf-8"), hashlib.sha256).hexdigest()
     return sig
 
 
 def order(res: {}, response_type=None) -> {}:
     if response_type:
```

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/client.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,82 +14,75 @@
 from exchanges_wrapper.web_sockets import UserEventsDataStream,\
                                             MarketEventsDataStream,\
                                             BfxPrivateEventsDataStream,\
                                             HbpPrivateEventsDataStream,\
                                             OkxPrivateEventsDataStream
 from exchanges_wrapper.definitions import OrderType
 from exchanges_wrapper.events import Events
+from exchanges_wrapper.ws_api.ws_session import UserWSSession
 import exchanges_wrapper.bitfinex_parser as bfx
 import exchanges_wrapper.huobi_parser as hbp
 import exchanges_wrapper.okx_parser as okx
 
 logger = logging.getLogger('exch_srv_logger')
 
 STATUS_TIMEOUT = 5  # sec
 
 
 def truncate(f, n):
     return math.floor(f * 10 ** n) / 10 ** n
 
 
 class Client:
-    def __init__(
-        self,
-        exchange,
-        sub_account,
-        test_net,
-        api_key,
-        api_secret,
-        endpoint_api_public,
-        endpoint_ws_public,
-        endpoint_api_auth,
-        endpoint_ws_auth,
-        ws_public_mbr,
-        passphrase,
-        master_email,
-        master_name,
-        two_fa
-    ):
-        self.exchange = exchange
-        self.sub_account = sub_account
-        self.test_net = test_net
-        self.api_key = api_key
-        self.api_secret = api_secret
-        self.passphrase = passphrase
-        self.endpoint_api_public = endpoint_api_public
-        self.endpoint_ws_public = endpoint_ws_public
-        self.endpoint_api_auth = endpoint_api_auth
-        self.endpoint_ws_auth = endpoint_ws_auth
-        self.ws_public_mbr = ws_public_mbr
-        self.master_email = master_email
-        self.master_name = master_name
-        self.two_fa = two_fa
+    def __init__(self, *acc):
+        self.exchange = acc[0]
+        self.sub_account = acc[1]
+        self.test_net = acc[2]
+        self.api_key = acc[3]
+        self.api_secret = acc[4]
+        self.passphrase = acc[10]
+        self.endpoint_api_public = acc[5]
+        self.endpoint_ws_public = acc[6]
+        self.endpoint_api_auth = acc[7]
+        self.endpoint_ws_auth = acc[8]
+        self.endpoint_ws_api = acc[14]
+        self.ws_public_mbr = acc[9]
+        self.master_email = acc[11]
+        self.master_name = acc[12]
+        self.two_fa = acc[13]
         #
         self.session = aiohttp.ClientSession()
         client_init_params = {
-            'api_key': api_key,
-            'api_secret': api_secret,
-            'passphrase': passphrase,
-            'endpoint': endpoint_api_auth,
+            'api_key': self.api_key,
+            'api_secret': self.api_secret,
+            'passphrase': self.passphrase,
+            'endpoint': self.endpoint_api_auth,
             'session': self.session,
-            'exchange': exchange,
-            'sub_account': sub_account,
-            'test_net': test_net
+            'exchange': self.exchange,
+            'sub_account': self.sub_account,
+            'test_net': self.test_net
         }
 
-        if exchange == 'binance':
+        self.user_wss_session = None
+        if self.exchange == 'binance':
             self.http = ClientBinance(**client_init_params)
-        elif exchange == 'bitfinex':
+            self.user_wss_session = UserWSSession(
+                self.api_key,
+                self.api_secret,
+                self.session,
+                self.endpoint_ws_api
+            )
+        elif self.exchange == 'bitfinex':
             self.http = ClientBFX(**client_init_params)
-        elif exchange == 'huobi':
+        elif self.exchange == 'huobi':
             self.http = ClientHBP(**client_init_params)
-        elif exchange == 'okx':
+        elif self.exchange == 'okx':
             self.http = ClientOKX(**client_init_params)
         else:
-            raise UserWarning(f"Exchange {exchange} not yet connected")
+            raise UserWarning(f"Exchange {self.exchange} not yet connected")
         #
         self.loaded = False
         self.symbols = {}
         self.highest_precision = None
         self.rate_limits = None
         self.data_streams = defaultdict(set)
         self.active_orders = {}
@@ -136,14 +129,16 @@
             self._events = Events()  # skipcq: PYL-W0201
         return self._events
 
     async def start_user_events_listener(self, _trade_id, symbol):
         logger.info(f"Start '{self.exchange}' user events listener for {_trade_id}")
         user_data_stream = None
         if self.exchange == 'binance':
+            if self.user_wss_session:
+                await self.user_wss_session.start(_trade_id)
             user_data_stream = UserEventsDataStream(self, self.endpoint_ws_auth, self.exchange, _trade_id)
         elif self.exchange == 'bitfinex':
             user_data_stream = BfxPrivateEventsDataStream(self, self.endpoint_ws_auth, self.exchange, _trade_id)
         elif self.exchange == 'huobi':
             user_data_stream = HbpPrivateEventsDataStream(self, self.endpoint_ws_auth, self.exchange, _trade_id, symbol)
         elif self.exchange == 'okx':
             user_data_stream = OkxPrivateEventsDataStream(self,
@@ -173,14 +168,16 @@
         await asyncio.gather(*start_list, return_exceptions=True)
 
     async def stop_events_listener(self, _trade_id):
         logger.info(f"Stop events listener data streams for {_trade_id}")
         stopped_data_stream = self.data_streams.pop(_trade_id, set())
         for data_stream in stopped_data_stream:
             await data_stream.stop()
+        if self.user_wss_session:
+            await self.user_wss_session.stop()
 
     def assert_symbol_exists(self, symbol):
         if self.loaded and symbol not in self.symbols:
             raise ExchangePyError(f"Symbol {symbol} is not valid according to the loaded exchange infos")
 
     def symbol_to_bfx(self, symbol) -> str:
         symbol_info = self.symbols.get(symbol)
```

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/definitions.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # Enum definitions of the exchanges_wrapper REST API
 # see: https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md#enum-definitions
 
 from enum import Enum
 
 
+# https://binance-docs.github.io/apidocs/websocket_api/en/#rate-limits
+class RateLimitInterval(Enum):
+    SECOND = 1
+    MINUTE = 60
+    HOUR = 3600
+    DAY = 86400
+
+
 # Symbol status (status)
 class SymbolStatus(Enum):
     PRE_TRADING = "PRE_TRADING"
     TRADING = "TRADING"
     POST_TRADING = "POST_TRADING"
     END_OF_DAY = "END_OF_DAY"
     HALT = "HALT"
```

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/errors.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/events.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/exch_srv.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/exch_srv.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,15 @@
             endpoint = config['endpoint'][exchange]
             #
             api_public = endpoint['api_public']
             ws_public = endpoint['ws_public']
             api_auth = endpoint['api_test'] if test_net else endpoint['api_auth']
             ws_auth = endpoint['ws_test'] if test_net else endpoint['ws_auth']
             ws_public_mbr = endpoint.get('ws_public_mbr')
+            ws_api = endpoint.get('ws_api_test') if test_net else endpoint.get('ws_api')
             #
             exchange = 'binance' if exchange == 'binance_us' else exchange
             #
             res = (exchange,        # 0
                    sub_account,     # 1
                    test_net,        # 2
                    api_key,         # 3
@@ -65,14 +66,15 @@
                    api_auth,        # 7
                    ws_auth,         # 8
                    ws_public_mbr,   # 9
                    passphrase,      # 10
                    master_email,    # 11
                    master_name,     # 12
                    two_fa,          # 13
+                   ws_api,          # 14
                    )
             break
     return res
 
 
 class OpenClient:
     open_clients = []
@@ -196,15 +198,30 @@
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         # message list
         response = api_pb2.FetchOpenOrdersResponse()
         # Nested dict
         response_order = api_pb2.FetchOpenOrdersResponse.Order()
         try:
-            res = await client.fetch_open_orders(symbol=request.symbol, receive_window=None)
+            res = []
+            ws_status = bool(client.exchange == 'binance'
+                             and client.user_wss_session
+                             and client.user_wss_session.operational_status)
+            if ws_status:
+                params = {
+                    "symbol": request.symbol,
+                }
+                res = await client.user_wss_session.handle_request(
+                    "openOrders.status",
+                    params,
+                    api_key=True,
+                    signed=True
+                )
+            if not ws_status or res is None:
+                res = await client.fetch_open_orders(symbol=request.symbol, receive_window=None)
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except (errors.RateLimitReached, errors.QueryCanceled) as ex:
             Martin.rate_limit_reached_time = time.time()
             logger.warning(f"FetchOpenOrders for {open_client.name}:{request.symbol} exception: {ex}")
             _context.set_details(f"{ex}")
             _context.set_code(grpc.StatusCode.RESOURCE_EXHAUSTED)
@@ -244,18 +261,34 @@
     async def FetchOrder(self, request: api_pb2.FetchOrderRequest,
                          _context: grpc.aio.ServicerContext) -> api_pb2.FetchOrderResponse:
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         _queue = client.on_order_update_queues.get(request.trade_id)
         response = api_pb2.FetchOrderResponse()
         try:
-            res = await client.fetch_order(symbol=request.symbol,
-                                           order_id=request.order_id,
-                                           origin_client_order_id=None,
-                                           receive_window=None)
+            res = {}
+            ws_status = bool(client.exchange == 'binance'
+                             and client.user_wss_session
+                             and client.user_wss_session.operational_status)
+            if ws_status:
+                params = {
+                    "symbol": request.symbol,
+                    "orderId": request.order_id,
+                }
+                res = await client.user_wss_session.handle_request(
+                    "order.status",
+                    params,
+                    api_key=True,
+                    signed=True
+                )
+            if not ws_status or res is None:
+                res = await client.fetch_order(symbol=request.symbol,
+                                               order_id=request.order_id,
+                                               origin_client_order_id=None,
+                                               receive_window=None)
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except Exception as _ex:
             logger.error(f"FetchOrders for {open_client.name}: {request.symbol} exception: {_ex}")
         else:
             if _queue and request.filled_update_call:
                 if res.get('status') == 'FILLED':
@@ -282,15 +315,30 @@
 
     async def CancelAllOrders(self, request: api_pb2.MarketRequest,
                               _context: grpc.aio.ServicerContext) -> api_pb2.SimpleResponse():
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         response = api_pb2.SimpleResponse()
         try:
-            res = await client.cancel_all_orders(symbol=request.symbol, receive_window=None)
+            res = []
+            ws_status = bool(client.exchange == 'binance'
+                             and client.user_wss_session
+                             and client.user_wss_session.operational_status)
+            if ws_status:
+                params = {
+                    "symbol": request.symbol,
+                }
+                res = await client.user_wss_session.handle_request(
+                    "openOrders.cancelAll",
+                    params,
+                    api_key=True,
+                    signed=True
+                )
+            if not ws_status or res is None:
+                res = await client.cancel_all_orders(symbol=request.symbol, receive_window=None)
             # logger.info(f"CancelAllOrders: {res}")
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except Exception as ex:
             logger.error(f"CancelAllOrder for {open_client.name}:{request.symbol} exception: {ex}")
             _context.set_details(f"{ex}")
             _context.set_code(grpc.StatusCode.UNKNOWN)
@@ -359,15 +407,26 @@
     async def FetchAccountInformation(self, request: api_pb2.OpenClientConnectionId,
                                       _context: grpc.aio.ServicerContext
                                       ) -> api_pb2.FetchAccountBalanceResponse:
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         response = api_pb2.FetchAccountBalanceResponse()
         response_balance = api_pb2.FetchAccountBalanceResponse.Balances()
-        account_information = await client.fetch_account_information(receive_window=None)
+        account_information = {}
+        ws_status = bool(client.exchange == 'binance'
+                         and client.user_wss_session
+                         and client.user_wss_session.operational_status)
+        if ws_status:
+            account_information = await client.user_wss_session.handle_request(
+                "account.status",
+                api_key=True,
+                signed=True
+            )
+        if not ws_status or account_information is None:
+            account_information = await client.fetch_account_information(receive_window=None)
         # Send only balances
         res = account_information.get('balances', [])
         # Create consolidated list of asset balances from SPOT and Funding wallets
         balances = []
         for i in res:
             _free = float(i.get('free'))
             _locked = float(i.get('locked'))
@@ -501,21 +560,37 @@
                 yield response
 
     async def FetchAccountTradeList(self, request: api_pb2.AccountTradeListRequest,
                                     _context: grpc.aio.ServicerContext) -> api_pb2.AccountTradeListResponse:
         client = OpenClient.get_client(request.client_id).client
         response = api_pb2.AccountTradeListResponse()
         response_trade = api_pb2.AccountTradeListResponse.Trade()
-        res = await client.fetch_account_trade_list(
-            symbol=request.symbol,
-            start_time=request.start_time,
-            end_time=None,
-            from_id=None,
-            limit=request.limit,
-            receive_window=None)
+        res = []
+        ws_status = bool(client.user_wss_session and client.user_wss_session.operational_status)
+        if ws_status:
+            params = {
+                "symbol": request.symbol,
+                "startTime": request.start_time,
+                "limit": request.limit,
+                "apiKey": 1,
+                "signature": 1,
+                "timestamp": 1
+            }
+            try:
+                res = await client.user_wss_session.handle_request("myTrades", params)
+            except TimeoutError:
+                ws_status = False
+        if not ws_status:
+            res = await client.fetch_account_trade_list(
+                symbol=request.symbol,
+                start_time=request.start_time,
+                end_time=None,
+                from_id=None,
+                limit=request.limit,
+                receive_window=None)
         # logger.info(f"FetchAccountTradeList: {res}")
         for trade in res:
             trade_order = json_format.ParseDict(trade, response_trade)
             response.items.append(trade_order)
         return response
 
     async def OnTickerUpdate(self, request: api_pb2.MarketRequest,
@@ -669,28 +744,50 @@
     async def CreateLimitOrder(self, request: api_pb2.CreateLimitOrderRequest,
                                _context: grpc.aio.ServicerContext) -> api_pb2.CreateLimitOrderResponse:
         response = api_pb2.CreateLimitOrderResponse()
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         # logger.info(f"CreateLimitOrder: quantity: {request.quantity}, price: {request.price}")
         try:
-            res = await client.create_order(
-                request.symbol,
-                Side.BUY if request.buy_side else Side.SELL,
-                order_type=OrderType.LIMIT,
-                time_in_force=TimeInForce.GTC,
-                quantity=request.quantity,
-                quote_order_quantity=None,
-                price=request.price,
-                new_client_order_id=request.new_client_order_id,
-                stop_price=None,
-                iceberg_quantity=None,
-                response_type=ResponseType.RESULT.value,
-                receive_window=None,
-                test=False)
+            res = {}
+            ws_status = bool(client.exchange == 'binance'
+                             and client.user_wss_session
+                             and client.user_wss_session.operational_status)
+            if ws_status:
+                params = {
+                    "symbol": request.symbol,
+                    "side": 'BUY' if request.buy_side else 'SELL',
+                    "type": 'LIMIT',
+                    "timeInForce": 'GTC',
+                    "price": request.price,
+                    "quantity": request.quantity,
+                    "newClientOrderId": request.new_client_order_id,
+                    "newOrderRespType": 'RESULT',
+                }
+                res = await client.user_wss_session.handle_request(
+                    "order.place",
+                    params,
+                    api_key=True,
+                    signed=True
+                )
+            if not ws_status or res is None:
+                res = await client.create_order(
+                    request.symbol,
+                    Side.BUY if request.buy_side else Side.SELL,
+                    order_type=OrderType.LIMIT,
+                    time_in_force=TimeInForce.GTC,
+                    quantity=request.quantity,
+                    quote_order_quantity=None,
+                    price=request.price,
+                    new_client_order_id=request.new_client_order_id,
+                    stop_price=None,
+                    iceberg_quantity=None,
+                    response_type=ResponseType.RESULT.value,
+                    receive_window=None,
+                    test=False)
         except errors.HTTPError as ex:
             logger.error(f"CreateLimitOrder for {open_client.name}:{request.symbol}:{request.new_client_order_id}"
                          f" exception: {ex}")
             _context.set_details(f"{ex}")
             _context.set_code(grpc.StatusCode.FAILED_PRECONDITION)
         except Exception as ex:
             logger.error(f"CreateLimitOrder for {open_client.name}:{request.symbol} exception: {ex}")
@@ -710,20 +807,36 @@
 
     async def CancelOrder(self, request: api_pb2.CancelOrderRequest,
                           _context: grpc.aio.ServicerContext) -> api_pb2.CancelOrderResponse:
         response = api_pb2.CancelOrderResponse()
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         try:
-            res = await client.cancel_order(
-                request.symbol,
-                order_id=request.order_id,
-                origin_client_order_id=None,
-                new_client_order_id=None,
-                receive_window=None)
+            res = {}
+            ws_status = bool(client.exchange == 'binance'
+                             and client.user_wss_session
+                             and client.user_wss_session.operational_status)
+            if ws_status:
+                params = {
+                    "symbol": request.symbol,
+                    "orderId": request.order_id,
+                }
+                res = await client.user_wss_session.handle_request(
+                    "order.cancel",
+                    params,
+                    api_key=True,
+                    signed=True
+                )
+            if not ws_status or res is None:
+                res = await client.cancel_order(
+                    request.symbol,
+                    order_id=request.order_id,
+                    origin_client_order_id=None,
+                    new_client_order_id=None,
+                    receive_window=None)
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except errors.RateLimitReached as ex:
             Martin.rate_limit_reached_time = time.time()
             logger.warning(f"CancelOrder for {open_client.name}:{request.symbol} exception: {ex}")
             _context.set_details(f"{ex}")
             _context.set_code(grpc.StatusCode.RESOURCE_EXHAUSTED)
```

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges_wrapper-1.3.2/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # Parameters for exchanges-wrapper REST API Server exch_srv.py
 # Copyright © 2021 Jerry Fedorenko aka VM
-# __version__ = "1.2.10"
+# __version__ = "1.3.2"
 
 # region endpoint
 [endpoint]
     [endpoint.binance]
         api_public = 'https://api.binance.com'
         api_auth = 'https://api.binance.com'
         ws_public = 'wss://stream.binance.com:9443'
         ws_auth = 'wss://stream.binance.com:9443'
         api_test = 'https://testnet.binance.vision'
         ws_test = 'wss://testnet.binance.vision/ws'
+        ws_api = 'wss://ws-api.binance.com:443/ws-api/v3'
+        ws_api_test = 'wss://testnet.binance.vision/ws-api/v3'
 
     [endpoint.binance_us]
         api_public = 'https://api.binance.us'
         api_auth = 'https://api.binance.us'
         ws_public = 'wss://stream.binance.us:9443'
         ws_auth = 'wss://stream.binance.us:9443'
         api_test = 'https://testnet.binance.vision'
         ws_test = 'wss://testnet.binance.vision/ws'
+        ws_api = 'wss://ws-api.binance.us:443/ws-api/v3'
+        ws_api_test = 'wss://testnet.binance.vision/ws-api/v3'
 
     [endpoint.ftx]
         api_public = 'https://ftx.com/api'
         ws_public = 'wss://ftx.com/ws/'
         api_auth = 'https://ftx.com/api'
         ws_auth = 'wss://ftx.com/ws/'
```

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/http_client.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/http_client.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/huobi_parser.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/huobi_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/okx_parser.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/okx_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/proto/exchanges_wrapper/api.proto` & `exchanges_wrapper-1.3.2/exchanges_wrapper/proto/exchanges_wrapper/api.proto`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.1b0/exchanges_wrapper/web_sockets.py` & `exchanges_wrapper-1.3.2/exchanges_wrapper/web_sockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                             raise aiohttp.ClientOSError('WSS reconnection request received from exchange')
                         elif code == 20060:
                             logger.info('WSS entering in maintenance mode, trying reconnect after 120s')
                             await asyncio.sleep(120)
                             raise aiohttp.ClientOSError
                 # data handling
                 elif isinstance(msg_data, list) and len(msg_data) == 2 and msg_data[1] == 'hb':
-                    pass
+                    pass  # heartbeat message
                 elif isinstance(msg_data, list):
                     if ch_type == 'book' and isinstance(msg_data[1][-1], list):
                         order_book = bfx.OrderBook(msg_data[1], symbol)
                     else:
                         await self._handle_event(msg_data, symbol, ch_type, order_book)
                 else:
                     logger.debug(f"Bitfinex undefined WSS: symbol: {symbol}, ch_type: {ch_type}, msg_data: {msg_data}")
@@ -175,15 +175,15 @@
         self.candles_max_time = None
 
     async def start_wss(self):
         logger.info(f"Start market WSS {self.channel if self.channel else ''} for {self.exchange}")
         registered_streams = self.client.events.registered_streams.get(self.exchange, {}).get(self.trade_id, set())
         if self.exchange == 'binance':
             combined_streams = "/".join(registered_streams)
-            self.web_socket = await self.session.ws_connect(url=f"{self.endpoint}/stream?streams={combined_streams}",
+            self.web_socket = await self.session.ws_connect(f"{self.endpoint}/stream?streams={combined_streams}",
                                                             receive_timeout=100)
             logger.info(f"Combined events stream started: {combined_streams}")
             await self._handle_messages(self.web_socket)
         else:
             symbol = self.channel.split('@')[0]
             ch_type = self.channel.split('@')[1]
             request = {}
@@ -439,15 +439,15 @@
         # https://github.com/binance-exchange/binance-official-api-docs/blob/master/user-data-stream.md#pingkeep-alive-a-listenkey
         while True:
             await asyncio.sleep(interval)
             await self.client.keep_alive_listen_key(listen_key)
 
     async def start_wss(self):
         listen_key = (await self.client.create_listen_key())["listenKey"]
-        self.web_socket = await self.session.ws_connect(url=f"{self.endpoint}/ws/{listen_key}", heartbeat=500)
+        self.web_socket = await self.session.ws_connect(f"{self.endpoint}/ws/{listen_key}", heartbeat=500)
         _task = asyncio.ensure_future(self._heartbeat(listen_key))
         try:
             await self._handle_messages(self.web_socket)
         finally:
             _task.cancel()
 
     async def _handle_event(self, content):
```

### Comparing `exchanges_wrapper-1.3.1b0/pyproject.toml` & `exchanges_wrapper-1.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 dependencies = [
     "aiohttp==3.8.4",
     "grpcio==1.48.1",
     "grpcio-tools==1.48.1",
     "toml==0.10.2",
     "idna==3.4",
     "pyotp~=2.8.0",
-    "simplejson==3.19.1"
+    "simplejson==3.19.1",
+    "shortuuid~=1.0.11",
 ]
 
 [tool.flit.module]
 name = "exchanges_wrapper"
 
 [project.urls]
 Source = "https://github.com/DogsTailFarmer/exchanges-wrapper"
```

### Comparing `exchanges_wrapper-1.3.1b0/PKG-INFO` & `exchanges_wrapper-1.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 1.3.1b0
+Version: 1.3.2
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: grpcio==1.48.1
 Requires-Dist: grpcio-tools==1.48.1
 Requires-Dist: toml==0.10.2
 Requires-Dist: idna==3.4
 Requires-Dist: pyotp~=2.8.0
 Requires-Dist: simplejson==3.19.1
+Requires-Dist: shortuuid~=1.0.11
 Project-URL: Source, https://github.com/DogsTailFarmer/exchanges-wrapper
 
 
 <p align="center"><img src="https://raw.githubusercontent.com/gist/DogsTailFarmer/167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/Logo%202v3.svg" width="300"></p>
 
 ***
 <h1 align="center">Crypto exchanges API/WSS wrapper with grpc powered server</h1>
@@ -34,15 +35,15 @@
 <a href="https://badge.fury.io/py/exchanges-wrapper"><img src="https://badge.fury.io/py/exchanges-wrapper.svg" alt="PyPI version"></a>
 <a href="https://codeclimate.com/github/DogsTailFarmer/exchanges-wrapper/maintainability"><img src="https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/maintainability" /></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=resolved+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=active+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_exchanges-wrapper" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_exchanges-wrapper&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/exchanges-wrapper" target="_blank"><img alt="Downloads" title="Downloads" src="https://pepy.tech/badge/exchanges-wrapper/month"/></a>
 ***
-From 1.2.10 update exch_srv_cfg.toml (see CHANGELOG for details)
+From 1.3.2 update exch_srv_cfg.toml (see [CHANGELOG](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/master/CHANGELOG.md#added-for-new-features) for details)
 ***
 
 ## exchanges-wrapper vs binance.py
 The main difference is the development of the project for trading with many exchanges.
 
 Next is adding a new module ```exchanges_wrapper/exch_srv.py``` as a multiplexer layer, providing simultaneous async interaction for many accounts
 and many trading pairs through one connection. It's powered by [gRPC](https://grpc.io/about/)
@@ -63,14 +64,15 @@
 
 ### Added Features
 - Multi exchanges support
 - Adaptive algorithm to ensure maximum performance and avoid exceeding the rates limits
 - Passthrough logging
 - WSS keepalive
 - Reuse session for new client sessions
+- Utilizing Websocket API (bidirectional) for the most commonly used methods (Binance ws-api/v3, )
 
 ## Extra exchanges implementation features
 - Binance REST API and WSS are accepted as basic, connection of other exchanges wrapped their API to Binance compatible
 - For other, some data cannot be obtained by directly calling one method, it is generated by a synthetic or calculation
 method
 - Some exchanges have not any testing or "paper trading" features, therefore, application development and testing is possible only
 at real bidding. First, run applications on the [Binance Spot Test Network](https://testnet.binance.vision/) or (Bitfinex, OKX) test account.
```

#### html2text {}

```diff
@@ -1,46 +1,50 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.1b0 Summary: REST
-API and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.2 Summary: REST API
+and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
 email: Thomas Marchand
 marchand@tuta.io>, Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
 Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.48.1 Requires-Dist: grpcio-
 tools==1.48.1 Requires-Dist: toml==0.10.2 Requires-Dist: idna==3.4 Requires-
-Dist: pyotp~=2.8.0 Requires-Dist: simplejson==3.19.1 Project-URL: Source,
-https://github.com/DogsTailFarmer/exchanges-wrapper
+Dist: pyotp~=2.8.0 Requires-Dist: simplejson==3.19.1 Requires-Dist:
+shortuuid~=1.0.11 Project-URL: Source, https://github.com/DogsTailFarmer/
+exchanges-wrapper
             [https://raw.githubusercontent.com/gist/DogsTailFarmer/
 167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/
                                 Logo%202v3.svg]
 ***
     ****** Crypto exchanges API/WSS wrapper with grpc powered server ******
                   ***** Binance, Bitfinex, Huobi, OKX, *****
                           **** For SPOT markets ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/
 maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** From
-1.2.10 update exch_srv_cfg.toml (see CHANGELOG for details) *** ## exchanges-
-wrapper vs binance.py The main difference is the development of the project for
-trading with many exchanges. Next is adding a new module ```exchanges_wrapper/
-exch_srv.py``` as a multiplexer layer, providing simultaneous async interaction
-for many accounts and many trading pairs through one connection. It's powered
-by [gRPC](https://grpc.io/about/) Remote Procedure Call framework. Warning.
-Coverage of overridden binance.py packages is significant but not complete.
-Served methods describes into ```example/exch_client.py``` ### Initial
-capabilities (inherited from binance.py) - Covers general endpoints (test
-connectivity and get exchange information's) - Covers market data endpoints -
-Covers Account endpoints (create and manage orders) - Covers user data stream
-(receive real time user updates) - Covers web socket streams (receive real time
-market updates) - Async support - Auto reconnect after exchanges API or network
-failure - Completely free and without limitations ### Added Features - Multi
-exchanges support - Adaptive algorithm to ensure maximum performance and avoid
-exceeding the rates limits - Passthrough logging - WSS keepalive - Reuse
-session for new client sessions ## Extra exchanges implementation features -
+1.3.2 update exch_srv_cfg.toml (see [CHANGELOG](https://github.com/
+DogsTailFarmer/exchanges-wrapper/blob/master/CHANGELOG.md#added-for-new-
+features) for details) *** ## exchanges-wrapper vs binance.py The main
+difference is the development of the project for trading with many exchanges.
+Next is adding a new module ```exchanges_wrapper/exch_srv.py``` as a
+multiplexer layer, providing simultaneous async interaction for many accounts
+and many trading pairs through one connection. It's powered by [gRPC](https://
+grpc.io/about/) Remote Procedure Call framework. Warning. Coverage of
+overridden binance.py packages is significant but not complete. Served methods
+describes into ```example/exch_client.py``` ### Initial capabilities (inherited
+from binance.py) - Covers general endpoints (test connectivity and get exchange
+information's) - Covers market data endpoints - Covers Account endpoints
+(create and manage orders) - Covers user data stream (receive real time user
+updates) - Covers web socket streams (receive real time market updates) - Async
+support - Auto reconnect after exchanges API or network failure - Completely
+free and without limitations ### Added Features - Multi exchanges support -
+Adaptive algorithm to ensure maximum performance and avoid exceeding the rates
+limits - Passthrough logging - WSS keepalive - Reuse session for new client
+sessions - Utilizing Websocket API (bidirectional) for the most commonly used
+methods (Binance ws-api/v3, ) ## Extra exchanges implementation features -
 Binance REST API and WSS are accepted as basic, connection of other exchanges
 wrapped their API to Binance compatible - For other, some data cannot be
 obtained by directly calling one method, it is generated by a synthetic or
 calculation method - Some exchanges have not any testing or "paper trading"
 features, therefore, application development and testing is possible only at
 real bidding. First, run applications on the [Binance Spot Test Network](https:
 //testnet.binance.vision/) or (Bitfinex, OKX) test account. ## Get started ###
```

