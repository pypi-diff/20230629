# Comparing `tmp/martin_binance-1.3.1b5.tar.gz` & `tmp/martin_binance-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin_binance-1.3.1b5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "martin_binance-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `martin_binance-1.3.1b5.tar` & `martin_binance-1.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1079 2023-06-21 14:52:44.450621 martin_binance-1.3.1b5/LICENSE
--rwxr-xr-x   0        0        0     3944 2023-06-21 14:52:44.450621 martin_binance-1.3.1b5/README.md
--rw-r--r--   0        0        0     2013 2023-06-21 14:52:44.494621 martin_binance-1.3.1b5/martin_binance/__init__.py
--rw-r--r--   0        0        0     4186 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2946 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    14050 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6721 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6716 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6722 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4707 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/client.py
--rw-r--r--   0        0        0   185525 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    85764 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16369 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1282 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1354 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/pyproject.toml
--rw-r--r--   0        0        0     5145 1970-01-01 00:00:00.000000 martin_binance-1.3.1b5/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-29 19:06:04.244467 martin_binance-1.3.2/LICENSE
+-rwxr-xr-x   0        0        0     4025 2023-06-29 19:06:04.244467 martin_binance-1.3.2/README.md
+-rw-r--r--   0        0        0     2013 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/__init__.py
+-rw-r--r--   0        0        0     4642 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2946 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    14575 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6721 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6716 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6722 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4707 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/client.py
+-rw-r--r--   0        0        0   186112 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    82924 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16282 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1282 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1427 2023-06-29 19:06:04.292467 martin_binance-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 martin_binance-1.3.2/PKG-INFO
```

### Comparing `martin_binance-1.3.1b5/LICENSE` & `martin_binance-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.1b5/README.md` & `martin_binance-1.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 > 
 >Incorrectly: (BTC/USDT), (ETH/USDT), (BTC/ETH)
 > 
 >As a result of the mutual impact on the operating balance sheet, the liquidity control system will block the work.
 
 ## References
 * Detailed information about use this strategy placed to [wiki](https://github.com/DogsTailFarmer/martin-binance/wiki)
+* [Trade idea](https://github.com/DogsTailFarmer/martin-binance/wiki/Trade-idea)
 * [Quick start](https://github.com/DogsTailFarmer/martin-binance/wiki/Quick-start)
 * [Back testing and parameters optimization](https://github.com/DogsTailFarmer/martin-binance/wiki/Back-testing-and-parameters-optimization)
 
 ## Referral link
 <p id="referral-link"></p>
 
 Create account on [Binance](https://accounts.binance.com/en/register?ref=QCS4OGWR) and get 10% discount on all trading
```

#### html2text {}

```diff
@@ -19,16 +19,17 @@
 updated ```cli_X_AAABBB.py```, use ```martin_binance/
 cli_0_BTCUSDT.py.template``` for compare and update * You cannot run multiple
 pairs with overlapping currencies on the same account! >Valid: (BTC/USDT),
 (ETH/BUSD), (SOL/LTC) > >Incorrectly: (BTC/USDT), (ETH/USDT), (BTC/ETH) > >As a
 result of the mutual impact on the operating balance sheet, the liquidity
 control system will block the work. ## References * Detailed information about
 use this strategy placed to [wiki](https://github.com/DogsTailFarmer/martin-
-binance/wiki) * [Quick start](https://github.com/DogsTailFarmer/martin-binance/
-wiki/Quick-start) * [Back testing and parameters optimization](https://
+binance/wiki) * [Trade idea](https://github.com/DogsTailFarmer/martin-binance/
+wiki/Trade-idea) * [Quick start](https://github.com/DogsTailFarmer/martin-
+binance/wiki/Quick-start) * [Back testing and parameters optimization](https://
 github.com/DogsTailFarmer/martin-binance/wiki/Back-testing-and-parameters-
 optimization) ## Referral link
 Create account on [Binance](https://accounts.binance.com/en/
 register?ref=QCS4OGWR) and get 10% discount on all trading fee Create account
 on [HUOBI](https://www.huobi.com/en-us/topic/double-reward/
 ?invite_code=9uaw3223) and will get 50 % off trading fees Create account on
 [Bitfinex](https://www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6%
```

### Comparing `martin_binance-1.3.1b5/martin_binance/__init__.py` & `martin_binance-1.3.2/martin_binance/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.1b5"
+__version__ = "1.3.2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 
 STANDALONE = True
@@ -26,14 +26,15 @@
     LAST_STATE_PATH = Path(WORK_PATH, "last_state")
     BACKTEST_PATH = Path(WORK_PATH, "back_test")
 else:
     LOG_PATH = None
     LAST_STATE_PATH = None
     BACKTEST_PATH = None
 
+
 def init():
     if CONFIG_FILE.exists():
         print(f"Client config found at {CONFIG_FILE}")
     else:
         print("Can't find client config file! Creating it...")
         CONFIG_PATH.mkdir(parents=True, exist_ok=True)
         if STANDALONE:
@@ -48,8 +49,8 @@
         print(f"Before the first run, set the parameters in {CONFIG_FILE}")
         if STANDALONE:
             raise SystemExit(1)
         raise UserWarning()
 
 
 if __name__ == '__main__':
-    init()
+    init()
```

### Comparing `martin_binance-1.3.1b5/martin_binance/backtest/OoTSP.py` & `martin_binance-1.3.2/martin_binance/backtest/OoTSP.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,29 +2,34 @@
 # -*- coding: utf-8 -*-
 """
 Optimization of Trading Strategy Parameters
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.1b5"
+__version__ = "1.3.1-2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
+
 from pathlib import Path
 import importlib.util
 from decimal import Decimal
 import optuna
 import inquirer
 from inquirer.themes import GreenPassion
 from martin_binance import BACKTEST_PATH
 
 
+vis = optuna.visualization
+ii_params = []
+
 PARAMS_FLOAT = ['PRICE_SHIFT', 'KBB']
 
+
 def try_trade(mbs, **kwargs):
     for key, value in kwargs.items():
         print(key, value)
         setattr(mbs.ex, key, value if isinstance(value, int) or key in PARAMS_FLOAT else Decimal(f"{value}"))
     mbs.ex.MODE = 'S'
     mbs.ex.SAVE_DS = False
     mbs.trade()
@@ -60,15 +65,15 @@
             choices=["New", "Plot from saved"],
         ),
         inquirer.Text(
             "n_trials",
             message="Enter number of cycles, from 50 to 500",
             ignore=lambda x: x["mode"] == "Plot from saved",
             default='150',
-            validate=lambda _, c: 2 <= int(c) < 500,
+            validate=lambda _, c: 10 <= int(c) <= 500,
         ),
     ]
 
     answers = inquirer.prompt(questions, theme=GreenPassion())
 
     study_name = answers.get('path')  # Unique identifier of the study
     storage_name = f"sqlite:///{Path(BACKTEST_PATH, study_name, f'{study_name}.db')}"
@@ -80,25 +85,42 @@
         except StopIteration:
             raise UserWarning(f"Can't find cli_*.py in {Path(BACKTEST_PATH, answers.get('path'))}")
         spec = importlib.util.spec_from_file_location("strategy", strategy)
         mbs = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(mbs)
         study = optuna.create_study(study_name=study_name, storage=storage_name, direction="maximize")
         study.optimize(objective, n_trials=int(answers.get('n_trials', '0')))
-        print(f"Optimal parameters: {study.best_params} for get {study.best_value}")
-        importance_params = optuna.importance.get_param_importances(study)
-        print("Evaluate parameter importance based on completed trials in the given study:")
-        for p in importance_params.items():
-            print(p)
+        print_study_result(study)
         print(f"Study instance saved to {storage_name} for later use")
     else:
         study = optuna.load_study(study_name=study_name, storage=storage_name)
     #
+    i_params = print_study_result(study)
+    for index, p in enumerate(i_params.items()):
+        ii_params.append(p[0])
+        if index == 2:
+            break
+    #
     try:
-        fig = optuna.visualization.plot_optimization_history(study)
+        fig = vis.plot_optimization_history(study)
         fig.show()
+
+        contour_plot = vis.plot_contour(study, params=ii_params)
+        contour_plot.show()
+
+        slice_plot = vis.plot_slice(study, params=ii_params)
+        slice_plot.show()
     except ImportError:
         print("Can't find GUI, you can copy study instance to another environment for analyze it")
 
 
+def print_study_result(study):
+    print(f"Optimal parameters: {study.best_params} for get {study.best_value}")
+    importance_params = optuna.importance.get_param_importances(study)
+    print("Evaluate parameter importance based on completed trials in the given study:")
+    for p in importance_params.items():
+        print(p)
+    return importance_params
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `martin_binance-1.3.1b5/martin_binance/backtest/VCoSEL.py` & `martin_binance-1.3.2/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.1b5/martin_binance/backtest/exchange_simulator.py` & `martin_binance-1.3.2/martin_binance/backtest/exchange_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 # -*- coding: utf-8 -*-
 """
 Simple exchange simulator for backtest purpose
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0-2"
+__version__ = "1.3.1-1"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from decimal import Decimal
 import pandas as pd
 
 
+def any2str(_x) -> str:
+    return f"{_x:.8f}".rstrip('0').rstrip('.')
+
+
 class Funds:
     __slots__ = ("base", "quote")
 
     def __init__(self):
         # {'asset': 'BTC', 'free': '0.0', 'locked': '0.0'}
         self.base = {}
         self.quote = {}
@@ -136,15 +140,15 @@
     )
 
     def __init__(self, save_ds: bool):
         self.save_ds = save_ds
         self.funds = Funds()
         self.fee_maker = Decimal('0')
         self.fee_taker = Decimal('0')
-        self.orders = []
+        self.orders = {}
         self.orders_buy = pd.Series()
         self.orders_sell = pd.Series()
         self.trade_id = 0
         self.ticker = {}
         self.grid_buy = {}
         self.grid_sell = {}
         self.ticker_last = Decimal('0')
@@ -155,15 +159,15 @@
             client_order_id: str,
             buy: bool,
             amount: str,
             price: str,
             lt: int,
             order_id=None) -> {}:
 
-        order_id = order_id or len(self.orders)
+        order_id = order_id or ((max(self.orders.keys()) + 1) if self.orders else 1)
         order = Order(symbol=symbol,
                       order_id=order_id,
                       client_order_id=client_order_id,
                       buy=buy,
                       amount=amount,
                       price=price,
                       lt=lt)
@@ -194,15 +198,15 @@
             else:
                 self.orders_sell.at[order_id] = Decimal(price)
                 if self.save_ds:
                     self.grid_sell[lt] = self.orders_sell
             #
             self.funds.on_order_created(buy=buy, amount=amount, price=price)
 
-        self.orders.append(order)
+        self.orders[order_id] = order
 
         # print(f"create_order.order: {vars(order)}")
         return {'symbol': order.symbol,
                 'orderId': order.order_id,
                 'orderListId': order.order_list_id,
                 'clientOrderId': order.client_order_id,
                 'transactTime': order.transact_time,
@@ -214,35 +218,31 @@
                 'timeInForce': order.time_in_force,
                 'type': order.type,
                 'side': order.side,
                 'workingTime': order.working_time,
                 'selfTradePreventionMode': order.self_trade_prevention_mode}
 
     def cancel_order(self, order_id: int, ts: int):
-        try:
-            order = next(x for x in self.orders if x.order_id == order_id)
-        except StopIteration:
+        order = self.orders.get(order_id)
+        if order is None:
             raise UserWarning(f"Error on Cancel order, can't find {order_id} anymore")
-        _order_id = self.orders.index(order)
         order.status = 'CANCELED'
         try:
             if order.side == 'BUY':
                 self.orders_buy = self.orders_buy.drop(order_id)
                 if self.save_ds and self.orders_buy.values.size:
                     self.grid_buy[ts] = self.orders_buy
             else:
                 self.orders_sell = self.orders_sell.drop(order_id)
                 if self.save_ds and self.orders_sell.values.size:
                     self.grid_sell[ts] = self.orders_sell
         except Exception as ex:
             raise UserWarning(f"Order {order_id} not active: {ex}")
         else:
-
-            self.orders[_order_id] = order
-
+            self.orders[order_id] = order
             self.funds.on_order_canceled(order.side, order.orig_qty, order.price)
             return {'symbol': order.symbol,
                     'origClientOrderId': order.client_order_id,
                     'orderId': order.order_id,
                     'orderListId': order.order_list_id,
                     'clientOrderId': 'qwert',
                     'price': order.price,
@@ -284,16 +284,16 @@
             if self.orders_sell.values.size:
                 self.grid_sell[ts] = self.orders_sell
             if self.orders_buy.values.size:
                 self.grid_buy[ts] = self.orders_buy
         #
         orders_filled = []
         for order_id in orders_id:
-            order = self.orders[order_id]
-            if order.status == 'NEW':
+            order = self.orders.get(order_id)
+            if order and order.status == 'NEW':
                 order.transact_time = int(ticker['closeTime'])
                 order.executed_qty = order.orig_qty
                 order.cummulative_quote_qty = str(Decimal(order.orig_qty) * Decimal(order.price))
                 order.status = 'FILLED'
                 order.event_time = order.transact_time
                 order.last_executed_quantity = order.orig_qty
                 order.cumulative_filled_quantity = order.orig_qty
@@ -338,18 +338,27 @@
                        'quote_order_quantity': order.quote_order_quantity}
                 #
                 orders_filled.append(res)
                 self.funds.on_order_filled(order.side, order.orig_qty, order.last_executed_price, self.fee_maker)
             #
         return orders_filled
 
-    def restore_state(self, symbol: str, lt: int, orders: []):
+    def restore_state(self, symbol: str, lt: int, orders: [], tp=()):
         for order in orders:
             self.create_order(
                 symbol=symbol,
                 client_order_id='',
                 buy=order['buy'],
-                amount=order['amount'],
-                price=order['price'],
+                amount=any2str(order['amount']),
+                price=any2str(order['price']),
                 lt=lt,
                 order_id=order['id']
             )
+
+            if tp:
+                funds = self.funds
+                if order['buy']:
+                    funds.base['free'] = str(Decimal(funds.base.get('free', 0)) - tp[0])
+                    funds.quote['free'] = str(Decimal(funds.quote.get('free', 0)) + tp[1])
+                else:
+                    funds.base['free'] = str(Decimal(funds.base.get('free', 0)) + tp[0])
+                    funds.quote['free'] = str(Decimal(funds.quote.get('free', 0)) - tp[1])
```

### Comparing `martin_binance-1.3.1b5/martin_binance/cli_0_BTCUSDT.py.template` & `martin_binance-1.3.2/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.1b5/martin_binance/cli_1_BTCUSDT.py.template` & `martin_binance-1.3.2/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.1b5/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin_binance-1.3.2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.1b5/martin_binance/client.py` & `martin_binance-1.3.2/martin_binance/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import asyncio
 # noinspection PyPackageRequirements
 import grpc
 import random
 import logging
-import uuid
+import shortuuid
 
 from exchanges_wrapper import api_pb2, api_pb2_grpc
 
 logger = logging.getLogger('logger.client')
 stream_handler = logging.StreamHandler()
 stream_handler.setFormatter(logging.Formatter(fmt="[%(asctime)s: %(levelname)s] %(message)s"))
-# stream_handler.setLevel(logging.INFO)
-stream_handler.setLevel(logging.DEBUG)
+stream_handler.setLevel(logging.INFO)
+# stream_handler.setLevel(logging.DEBUG)
 logger.addHandler(stream_handler)
 
 
 class Trade:
     def __init__(self, channel_options, account_name, rate_limiter):
         self.channel = grpc.aio.insecure_channel(target='localhost:50051', options=channel_options)
         self.stub = api_pb2_grpc.MartinStub(self.channel)
         self.account_name = account_name
         self.rate_limiter = rate_limiter
         self.client: api_pb2.OpenClientConnectionId = None
         self.wait_connection = False
-        self.trade_id = str(uuid.uuid4().hex)
+        self.trade_id = shortuuid.uuid()
 
     async def get_client(self):
         if not self.wait_connection:
             self.wait_connection = True
             client = None
             while client is None:
                 try:
@@ -86,15 +86,15 @@
                     (status_code == grpc.StatusCode.UNKNOWN
                      and "'NoneType' object has no attribute 'client'" in ex.details())
                 ):
                     self.client = None
                     raise UserWarning("Connection to gRPC server failed, wait connection...")
                 if status_code == grpc.StatusCode.RESOURCE_EXHAUSTED:
                     raise
-                logger.error(f"Exception on send request {_request}: {status_code.name}, {ex.details()}")
+                logger.debug(f"Exception on send request {_request}: {status_code.name}, {ex.details()}")
                 raise
             else:
                 # logger.info(f"send_request.res: {res}")
                 return res
         else:
             raise UserWarning("Send gRPC request failed, not active client session")
```

### Comparing `martin_binance-1.3.1b5/martin_binance/executor.py` & `martin_binance-1.3.2/martin_binance/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0-4"
+__version__ = "1.3.1-3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 from decimal import Decimal, ROUND_FLOOR, ROUND_CEILING
@@ -469,15 +469,15 @@
     connection_analytic.commit()
 
 
 def f2d(_f: float) -> Decimal:
     return Decimal(str(_f))
 
 
-def solve(fn, value: Decimal, x: Decimal, max_err: Decimal, max_tries=50, **kwargs) -> Decimal:
+def solve(fn, value: Decimal, x: Decimal, max_err: Decimal, max_tries=50, **kwargs) -> ():
     """
     Numerical solution of the equation, value = fn(x)
     :param fn: Function
     :param value: Specified value
     :param x: Predict of the search value
     :param max_err:
     :param max_tries:
@@ -494,39 +494,35 @@
         return (_fn(_x + _delta, **_kwargs) - _fn(_x, **_kwargs)) / _delta
 
     while 1:
         tries += 1
         err = fn(x, **kwargs) - value
         # print(f"tries: {tries}, x: {x}, fn: {fn(x, **kwargs)}, err: {err}")
         if err >= 0 and abs(err) <= max_err:
-            print(f"In {tries} attempts the best solution was found!", )
-            return x
+            return x, f"In {tries} attempts the best solution was found!"
         correction = (delta * tries) if err < 0 and _err.count(err) else 0
         if err >= 0:
             solves.append((err, x))
         slope = dx(fn, x, delta, **kwargs)
         if slope != 0.0:
             x -= err/slope
             x = max(_x + delta * tries, x + correction)
         else:
             delta *= 10
             if delta > 1:
                 break
         # print(f"tries: {tries}, delta: {delta}, correction: {correction}, slope: {slope}")
         if (_err.count(err) or tries > max_tries) and len(solves) > 5:
             solves.sort(key=lambda a: (a[0], a[1]), reverse=False)
-            print('Solve return the best of the right value ;-)')
             # print("\n".join(f"delta: {k}\t result: {v}" for k, v in solves))
-            return solves[0][1]
+            return solves[0][1], 'Solve return the best of the right value ;-)'
         if tries > max_tries * 2:
             break
         _err.append(err)
-    print('Oops. No solution found')
-    print("\n".join(f"delta: {k}\tresult: {v}" for k, v in solves))
-    return f2d(0)
+    return f2d(0), "\n".join(f"delta: {k}\tresult: {v}" for k, v in solves)
 
 
 class Orders:
     __slots__ = ("orders_list",)
 
     def __init__(self):
         self.orders_list = []
@@ -886,15 +882,14 @@
             self.message_log("Can't get actual price, initialization checks stopped", log_level=LogLevel.CRITICAL)
             if STANDALONE:
                 raise SystemExit(1)
         # self.message_log('End Init section')
 
     @staticmethod
     def get_strategy_config() -> StrategyConfig:
-        print('Get config')
         s = StrategyConfig()
         s.required_data_updates = {StrategyConfig.ORDER_BOOK,
                                    StrategyConfig.FUNDS,
                                    StrategyConfig.TICKER}
         s.normalize_exchange_buy_amounts = True
         return s
 
@@ -1206,18 +1201,22 @@
             self.tp_part_amount_first = f2d(json.loads(strategy_state.get('tp_part_amount_first')))
             self.tp_part_amount_second = f2d(json.loads(strategy_state.get('tp_part_amount_second')))
             self.tp_target = f2d(json.loads(strategy_state.get('tp_target')))
             self.tp_order = eval(json.loads(strategy_state.get('tp_order')))
             self.tp_wait_id = json.loads(strategy_state.get('tp_wait_id'))
             self.first_run = False
             self.start_after_shift = False if GRID_ONLY and USE_ALL_FUND else self.start_after_shift
-        # Variants are processed when the actual order is equal to or less than it should be
-        # Exotic when drop during placed grid or unconfirmed TP left for later
+        #
         self.start_process()
-        open_orders = self.get_buffered_open_orders(True)  # lgtm [py/call/wrong-arguments]
+        if self.command == 'stopped':
+            self.message_log("Restore, strategy stopped. Need manual action", tlg=True)
+            return
+        self.avg_rate = f2d(self.get_buffered_ticker().last_price)
+        #
+        open_orders = self.get_buffered_open_orders()
         tp_order = None
         # Separate TP order
         if self.tp_order_id:
             for i, o in enumerate(open_orders):
                 if o.id == self.tp_order_id:
                     tp_order = open_orders[i]
                     del open_orders[i]  # skipcq: PYL-E1138
@@ -1238,201 +1237,199 @@
         part_amount_first = Decimal('0')
         part_amount_second = Decimal('0')
         if grid_filled:
             for v in self.part_amount.values():
                 part_amount_first += v[0]
                 part_amount_second += v[1]
         #
-        self.avg_rate = f2d(self.get_buffered_ticker().last_price)
-        #
-        if self.command == 'stopped':
-            self.message_log("Restore, strategy stopped. Need manual action", tlg=True)
-        elif grid_no_change and tp_no_change:
+        if grid_no_change and tp_no_change:
             if grid_hold:
                 self.message_log("Restore, no grid orders, place from hold now", tlg=True)
                 self.place_grid_part()
             elif no_orders:
                 self.restart = True
                 self.message_log("Restore, no orders, restart", tlg=True)
                 self.start()
             elif not GRID_ONLY and not self.tp_order_id and self.check_min_amount():
                 self.message_log("Restore, replace TP", tlg=True)
                 self.place_profit_order()
             else:
                 self.message_log("Restore, No difference, go work", tlg=True)
-
-        elif grid_filled and tp_filled:
-            self.message_log("Restore, all grid orders and TP was filled", tlg=True)
-            # Get actual parameter of filled tp order
-            market_order = self.get_buffered_completed_trades(True)
-            amount_first = Decimal('0')
-            amount_second = Decimal('0')
-            for o in market_order:
-                if o.order_id == self.tp_order_id:
-                    amount_first += f2d(o.amount)
-                    amount_second += f2d(o.amount) * f2d(o.price)
-            if amount_first == 0:
-                # If execution event was missed
-                _buy, _amount, _price = self.tp_order
-                amount_first = self.round_truncate(_amount, base=True)
-                amount_second = self.round_truncate(_amount * _price, base=False)
-            self.tp_was_filled = (amount_first, amount_second, True)
-            self.tp_order_id = None
-            self.tp_order = ()
-            self.message_log(f"restore_strategy_state.was_filled_tp: {self.tp_was_filled}", log_level=LogLevel.DEBUG)
-            # Calculate sum trade amount for both currency
-            amount_first = Decimal('0')
-            amount_second = Decimal('0')
-            for i in self.orders_grid:
-                amount_first += i['amount']
-                amount_second += i['amount'] * i['price']
-                print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
-            amount_first += part_amount_first
-            amount_second += part_amount_second
-            self.part_amount.clear()
-            print(f"Total grid amount first: {amount_first}, second: {amount_second}")
-            # Clear list of grid order
-            self.orders_grid.orders_list.clear()
-            self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
-
-        elif grid_filled and tp_no_change:
-            self.message_log('Restore, No grid orders -> Reverse', tlg=True)
-            self.shift_grid_threshold = None
-            # Admit that missing orders were executed on conditions no worse than those saved
-            # Calculate sum trade amount for both currency
-            amount_first = Decimal('0')
-            amount_second = Decimal('0')
-            for i in self.orders_grid:
-                amount_first += i['amount']
-                amount_second += i['amount'] * i['price']
-                print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
-            amount_first += part_amount_first
-            amount_second += part_amount_second
-            self.part_amount.clear()
-            print(f"Total amount first: {amount_first}, second: {amount_second}")
-            # Clear list of grid order
-            self.orders_grid.orders_list.clear()
-            self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
-
-        elif grid_less and tp_filled:
-            self.message_log("Restore, some grid orders and TP was filled", tlg=True)
-            # Get actual parameter of filled tp order
-            market_order = self.get_buffered_completed_trades(True)
-            amount_first = Decimal('0')
-            amount_second = Decimal('0')
-            for o in market_order:
-                if o.order_id == self.tp_order_id:
-                    amount_first += f2d(o.amount)
-                    amount_second += f2d(o.amount) * f2d(o.price)
-                    print(f"order_id={o.order_id}, first: {o.amount}, price: {o.price}")
-            if amount_first == 0:
-                # If execution event was missed
-                _buy, _amount, _price = self.tp_order
-                amount_first = self.round_truncate(f2d(_amount), base=True)
-                amount_second = self.round_truncate(f2d(_amount * _price), base=False)
-            self.tp_was_filled = (amount_first, amount_second, True)
-            self.tp_order_id = None
-            self.tp_order = ()
-            self.message_log(f"restore_strategy_state.was_filled_tp: {self.tp_was_filled}", log_level=LogLevel.DEBUG)
-            # Calculate sum trade amount for both currency
-            exch_orders_id = []
-            save_orders_id = []
-            for i in open_orders:
-                exch_orders_id.append(i.id)
-            for i in self.orders_grid:
-                save_orders_id.append(i.get('id'))
-            print(f"restore_strategy_state.exch_orders_id: {exch_orders_id}")
-            print(f"restore_strategy_state.save_orders_id: {save_orders_id}")
-            diff_id = list(set(save_orders_id).difference(exch_orders_id))
-            print(f"Executed order id is: {diff_id}")
-            # Calculate sum trade amount for both currency
-            amount_first = Decimal('0')
-            amount_second = Decimal('0')
-            for i in self.orders_grid:
-                if i['id'] in diff_id:
+        elif not STANDALONE:
+            # For MARGINE mode compatibility
+            # Variants are processed when the actual order is equal to or less than it should be
+            # Exotic when dropped during grid placement or unconfirmed TP, left for later
+            if grid_filled and tp_filled:
+                self.message_log("Restore, all grid orders and TP was filled", tlg=True)
+                # Get actual parameter of filled tp order
+                market_order = self.get_buffered_completed_trades(True)
+                amount_first = Decimal('0')
+                amount_second = Decimal('0')
+                for o in market_order:
+                    if o.order_id == self.tp_order_id:
+                        amount_first += f2d(o.amount)
+                        amount_second += f2d(o.amount) * f2d(o.price)
+                if amount_first == 0:
+                    # If execution event was missed
+                    _buy, _amount, _price = self.tp_order
+                    amount_first = self.round_truncate(_amount, base=True)
+                    amount_second = self.round_truncate(_amount * _price, base=False)
+                self.tp_was_filled = (amount_first, amount_second, True)
+                self.tp_order_id = None
+                self.tp_order = ()
+                self.message_log(f"restore_strategy_state.was_filled_tp: {self.tp_was_filled}", log_level=LogLevel.DEBUG)
+                # Calculate sum trade amount for both currency
+                amount_first = Decimal('0')
+                amount_second = Decimal('0')
+                for i in self.orders_grid:
                     amount_first += i['amount']
                     amount_second += i['amount'] * i['price']
                     print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
-                    part_amount_first, part_amount_second = self.part_amount.pop(i['id'], (Decimal('0'), Decimal('0')))
-            amount_first += part_amount_first
-            amount_second += part_amount_second
-            self.message_log(f"Total amount first: {amount_first:f}, second: {amount_second:f}", color=Style.B_WHITE)
-            # Remove from list of grid order
-            for i in diff_id:
-                self.orders_grid.remove(i)
-            # Calculate trade amount with Fee
-            amount_first_fee, amount_second_fee = self.fee_for_grid(amount_first, amount_second)
-            # Calculate cycle sum trading for both currency
-            self.sum_amount_first += amount_first_fee
-            self.sum_amount_second += amount_second_fee
-            if open_orders_len == 0 and self.orders_hold:
-                self.place_grid_part()
-            self.after_filled_tp(one_else_grid=True)
+                amount_first += part_amount_first
+                amount_second += part_amount_second
+                self.part_amount.clear()
+                print(f"Total grid amount first: {amount_first}, second: {amount_second}")
+                # Clear list of grid order
+                self.orders_grid.orders_list.clear()
+                self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
 
-        elif grid_less:
-            self.message_log("Restore, Less grid orders -> replace tp order", tlg=True)
-            self.shift_grid_threshold = None
-            exch_orders_id = []
-            save_orders_id = []
-            for i in open_orders:
-                exch_orders_id.append(i.id)
-            for i in self.orders_grid:
-                save_orders_id.append(i.get('id'))
-            print(f"restore_strategy_state.exch_orders_id: {exch_orders_id}")
-            print(f"restore_strategy_state.save_orders_id: {save_orders_id}")
-            diff_id = list(set(save_orders_id).difference(exch_orders_id))
-            print(f"Executed order id is: {diff_id}")
-            # Calculate sum trade amount for both currency
-            amount_first = Decimal('0')
-            amount_second = Decimal('0')
-            for i in self.orders_grid:
-                if i['id'] in diff_id:
+            elif grid_filled and tp_no_change:
+                self.message_log('Restore, No grid orders -> Reverse', tlg=True)
+                self.shift_grid_threshold = None
+                # Admit that missing orders were executed on conditions no worse than those saved
+                # Calculate sum trade amount for both currency
+                amount_first = Decimal('0')
+                amount_second = Decimal('0')
+                for i in self.orders_grid:
                     amount_first += i['amount']
                     amount_second += i['amount'] * i['price']
                     print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
-                    part_amount_first, part_amount_second = self.part_amount.pop(i['id'], (Decimal('0'), Decimal('0')))
-            amount_first += part_amount_first
-            amount_second += part_amount_second
-            self.message_log(f"Total amount first: {amount_first:f}, second: {amount_second:f}", color=Style.B_WHITE)
-            # Remove from list of grid order
-            for i in diff_id:
-                self.orders_grid.remove(i)
-            self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
-
-        elif tp_filled:
-            self.message_log('Restore, TP order was filled -> Restart', tlg=True)
-            # Get actual parameter of filled tp order
-            market_order = self.get_buffered_completed_trades(True)
-            amount_first = Decimal('0')
-            amount_second = Decimal('0')
-            for o in market_order:
-                if o.order_id == self.tp_order_id:
-                    amount_first += f2d(o.amount)
-                    amount_second += f2d(o.amount) * f2d(o.price)
-                    print(f"order_id={o.order_id}, first: {o.amount}, price: {o.price}")
-            if amount_first == 0:
-                # If execution event was missed
-                _buy, _amount, _price = self.tp_order
-                amount_first = self.round_truncate(f2d(_amount), base=True)
-                amount_second = self.round_truncate(f2d(_amount * _price), base=False)
-            self.tp_was_filled = (amount_first, amount_second, True)
-            self.tp_order_id = None
-            self.tp_order = ()
-            self.grid_remove = True
-            self.cancel_grid(cancel_all=True)
+                amount_first += part_amount_first
+                amount_second += part_amount_second
+                self.part_amount.clear()
+                print(f"Total amount first: {amount_first}, second: {amount_second}")
+                # Clear list of grid order
+                self.orders_grid.orders_list.clear()
+                self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
 
-        elif grid_more and self.orders_init:
-            self.message_log('Restored, some grid order(s) was placed', tlg=True)
+            elif grid_less and tp_filled:
+                self.message_log("Restore, some grid orders and TP was filled", tlg=True)
+                # Get actual parameter of filled tp order
+                market_order = self.get_buffered_completed_trades(True)
+                amount_first = Decimal('0')
+                amount_second = Decimal('0')
+                for o in market_order:
+                    if o.order_id == self.tp_order_id:
+                        amount_first += f2d(o.amount)
+                        amount_second += f2d(o.amount) * f2d(o.price)
+                        print(f"order_id={o.order_id}, first: {o.amount}, price: {o.price}")
+                if amount_first == 0:
+                    # If execution event was missed
+                    _buy, _amount, _price = self.tp_order
+                    amount_first = self.round_truncate(f2d(_amount), base=True)
+                    amount_second = self.round_truncate(f2d(_amount * _price), base=False)
+                self.tp_was_filled = (amount_first, amount_second, True)
+                self.tp_order_id = None
+                self.tp_order = ()
+                self.message_log(f"restore_strategy_state.was_filled_tp: {self.tp_was_filled}", log_level=LogLevel.DEBUG)
+                # Calculate sum trade amount for both currency
+                exch_orders_id = []
+                save_orders_id = []
+                for i in open_orders:
+                    exch_orders_id.append(i.id)
+                for i in self.orders_grid:
+                    save_orders_id.append(i.get('id'))
+                print(f"restore_strategy_state.exch_orders_id: {exch_orders_id}")
+                print(f"restore_strategy_state.save_orders_id: {save_orders_id}")
+                diff_id = list(set(save_orders_id).difference(exch_orders_id))
+                print(f"Executed order id is: {diff_id}")
+                # Calculate sum trade amount for both currency
+                amount_first = Decimal('0')
+                amount_second = Decimal('0')
+                for i in self.orders_grid:
+                    if i['id'] in diff_id:
+                        amount_first += i['amount']
+                        amount_second += i['amount'] * i['price']
+                        print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
+                        part_amount_first, part_amount_second = self.part_amount.pop(i['id'], (Decimal('0'), Decimal('0')))
+                amount_first += part_amount_first
+                amount_second += part_amount_second
+                self.message_log(f"Total amount first: {amount_first:f}, second: {amount_second:f}", color=Style.B_WHITE)
+                # Remove from list of grid order
+                for i in diff_id:
+                    self.orders_grid.remove(i)
+                # Calculate trade amount with Fee
+                amount_first_fee, amount_second_fee = self.fee_for_grid(amount_first, amount_second)
+                # Calculate cycle sum trading for both currency
+                self.sum_amount_first += amount_first_fee
+                self.sum_amount_second += amount_second_fee
+                if open_orders_len == 0 and self.orders_hold:
+                    self.place_grid_part()
+                self.after_filled_tp(one_else_grid=True)
 
-        elif tp_placed:
-            self.message_log('Restored, take profit order(s) was placed', tlg=True)
+            elif grid_less:
+                self.message_log("Restore, Less grid orders -> replace tp order", tlg=True)
+                self.shift_grid_threshold = None
+                exch_orders_id = []
+                save_orders_id = []
+                for i in open_orders:
+                    exch_orders_id.append(i.id)
+                for i in self.orders_grid:
+                    save_orders_id.append(i.get('id'))
+                print(f"restore_strategy_state.exch_orders_id: {exch_orders_id}")
+                print(f"restore_strategy_state.save_orders_id: {save_orders_id}")
+                diff_id = list(set(save_orders_id).difference(exch_orders_id))
+                print(f"Executed order id is: {diff_id}")
+                # Calculate sum trade amount for both currency
+                amount_first = Decimal('0')
+                amount_second = Decimal('0')
+                for i in self.orders_grid:
+                    if i['id'] in diff_id:
+                        amount_first += i['amount']
+                        amount_second += i['amount'] * i['price']
+                        print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
+                        part_amount_first, part_amount_second = self.part_amount.pop(i['id'], (Decimal('0'), Decimal('0')))
+                amount_first += part_amount_first
+                amount_second += part_amount_second
+                self.message_log(f"Total amount first: {amount_first:f}, second: {amount_second:f}", color=Style.B_WHITE)
+                # Remove from list of grid order
+                for i in diff_id:
+                    self.orders_grid.remove(i)
+                self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
 
-        else:
-            self.message_log('Restored, unknown state. Investigation needed', tlg=True)
-        # self.unsuspend()
+            elif tp_filled:
+                self.message_log('Restore, TP order was filled -> Restart', tlg=True)
+                # Get actual parameter of filled tp order
+                market_order = self.get_buffered_completed_trades(True)
+                amount_first = Decimal('0')
+                amount_second = Decimal('0')
+                for o in market_order:
+                    if o.order_id == self.tp_order_id:
+                        amount_first += f2d(o.amount)
+                        amount_second += f2d(o.amount) * f2d(o.price)
+                        print(f"order_id={o.order_id}, first: {o.amount}, price: {o.price}")
+                if amount_first == 0:
+                    # If execution event was missed
+                    _buy, _amount, _price = self.tp_order
+                    amount_first = self.round_truncate(f2d(_amount), base=True)
+                    amount_second = self.round_truncate(f2d(_amount * _price), base=False)
+                self.tp_was_filled = (amount_first, amount_second, True)
+                self.tp_order_id = None
+                self.tp_order = ()
+                self.grid_remove = True
+                self.cancel_grid(cancel_all=True)
+
+            elif grid_more and self.orders_init:
+                self.message_log('Restored, some grid order(s) was placed', tlg=True)
+
+            elif tp_placed:
+                self.message_log('Restored, take profit order(s) was placed', tlg=True)
+
+            else:
+                self.message_log('Restored, unknown state. Investigation needed', tlg=True)
 
     def start(self, profit_f: Decimal = f2d(0), profit_s: Decimal = f2d(0)) -> None:
         self.message_log('Start')
         if self.command == 'stopped':
             self.message_log('Strategy stopped, waiting manual action')
             return
         # Cancel take profit order in all state
@@ -1548,16 +1545,15 @@
             self.command = 'stop'
         if self.command == 'end' or (self.command == 'stop' and
                                      (not self.reverse or (self.reverse and REVERSE_STOP))):
             self.command = 'stopped'
             self.start_collect = 1
             self.message_log('Stop, waiting manual action', tlg=True)
         else:
-            n = gc.collect(generation=2)
-            print('Number of unreachable objects collected by GC:', n)
+            self.message_log(f"Number of unreachable objects collected by GC: {gc.collect(generation=2)}")
             self.message_log(f"Initial first: {ff}, second: {fs}", color=Style.B_WHITE)
             self.restart = None
             # Init variable
             self.profit_first = Decimal('0')
             self.profit_second = Decimal('0')
             self.over_price = OVER_PRICE
             self.order_q = ORDER_Q
@@ -1596,28 +1592,28 @@
                                                   AND f_currency=:f_currency\
                                                   AND s_currency=:s_currency",
                                                  {'id_exchange': ID_EXCHANGE,
                                                   'f_currency': self.f_currency,
                                                   's_currency': self.s_currency})
                 self.connection_analytic.commit()
             except sqlite3.Error as err:
-                print(f"DELETE from t_order: {err}")
+                self.message_log(f"DELETE from t_order: {err}")
             self.connection_analytic.close()
         self.connection_analytic = None
 
     def suspend(self) -> None:
-        print('Suspend')
+        self.message_log('Suspend')
         self.queue_to_db.put({'stop_signal': True})
         self.queue_to_tlg.put(STOP_TLG)
         self.connection_analytic.commit()
         self.connection_analytic.close()
         self.connection_analytic = None
 
     def unsuspend(self) -> None:
-        print('Unsuspend')
+        self.message_log('Unsuspend')
         self.start_process()
 
     def init_warning(self, _amount_first_grid: Decimal):
         if self.cycle_buy:
             depo = self.deposit_second
         else:
             depo = self.deposit_first
@@ -1671,33 +1667,33 @@
         if fs >= f2d(tcm.min_notional):
             self.message_log(f"Sending {fs} {self.s_currency} to main account", color=Style.UNDERLINE, tlg=True)
             self.transfer_to_master(self.s_currency, any2str(fs))
         else:
             fs = f2d(0)
         return ff, fs
 
-    def message_log(self, msg: str, log_level=LogLevel.INFO, tlg: bool = False, color=Style.WHITE) -> None:
+    def message_log(self, msg: str, log_level=LogLevel.INFO, tlg=False, color=Style.WHITE) -> None:
         if tlg and color == Style.WHITE:
             color = Style.B_WHITE
         if log_level in (LogLevel.ERROR, LogLevel.CRITICAL):
             tlg = True
             color = Style.B_RED
         color = color if STANDALONE else 0
         color_msg = color+msg+Style.RESET if color else msg
         if log_level not in LOG_LEVEL_NO_PRINT:
             if MODE in ('T', 'TC'):
-                local_time = datetime.now().strftime('%d/%m %H:%M:%S')
+                print(f"{datetime.now().strftime('%d/%m %H:%M:%S')} {color_msg}")
             else:
-                local_time = datetime.fromtimestamp(self.local_time()).strftime('%H:%M:%S.%f')
-            print(f"{local_time} {color_msg}")
-        write_log(log_level, msg)
-        if MODE in ('T', 'TC') and tlg and self.queue_to_tlg:
-            msg = self.tlg_header + msg
-            self.status_time = self.local_time()
-            self.queue_to_tlg.put(msg)
+                tqdm.write(f"{datetime.fromtimestamp(self.local_time()).strftime('%H:%M:%S.%f')} {color_msg}")
+        if MODE in ('T', 'TC'):
+            write_log(log_level, msg)
+            if tlg and self.queue_to_tlg:
+                msg = self.tlg_header + msg
+                self.status_time = self.local_time()
+                self.queue_to_tlg.put(msg)
 
     ##############################################################
     # Technical analysis
     ##############################################################
 
     def atr(self, interval: int = 14):
         """
@@ -2440,15 +2436,16 @@
             # Fine calculate over_price for target return amount
             params = {'buy_side': buy_side,
                       'depo': depo,
                       'base_price': base_price,
                       'amount_first_grid': amount_first_grid,
                       'min_delta': min_delta,
                       'amount_min': amount_min}
-            over_price = solve(self.calc_grid, reverse_target_amount, over_price_coarse, max_err, **params)
+            over_price, msg = solve(self.calc_grid, reverse_target_amount, over_price_coarse, max_err, **params)
+            self.message_log(msg)
             if over_price == 0:
                 self.message_log("Can't calculate over price for reverse cycle,"
                                  " use previous or over_price_coarse * 3", log_level=LogLevel.ERROR)
                 over_price = over_price_previous or 3 * over_price_coarse
         else:
             over_price = over_price_coarse
         return over_price
@@ -2458,21 +2455,21 @@
         self.connection_analytic = self.connection_analytic or sqlite3.connect(DB_FILE,
                                                                                check_same_thread=False,
                                                                                timeout=10)
         # Create processes for save to .db and send Telegram message
         self.pr_db = Thread(target=save_to_db, args=(self.queue_to_db,))
         self.pr_tlg = Thread(target=telegram, args=(self.queue_to_tlg, self.tlg_header.split('.')[0],))
         if not self.pr_db.is_alive():
-            print('Start process for .db save')
+            self.message_log('Start process for .db save')
             try:
                 self.pr_db.start()
             except AssertionError as error:
                 self.message_log(str(error), log_level=LogLevel.ERROR, color=Style.B_RED)
         if not self.pr_tlg.is_alive():
-            print('Start process for Telegram')
+            self.message_log('Start process for Telegram')
             try:
                 self.pr_tlg.start()
             except AssertionError as error:
                 self.message_log(str(error), log_level=LogLevel.ERROR, color=Style.B_RED)
 
     def fee_for_grid(self,
                      amount_first: Decimal,
@@ -3421,15 +3418,15 @@
                         self.place_grid_part()
             else:
                 self.message_log(F"Did not have waiting order id for {place_order_id}", LogLevel.ERROR)
 
     def on_place_order_error_string(self, place_order_id: int, error: str) -> None:
         # Check all orders on exchange if exists required
         self.message_log(f"On place order {place_order_id} error: {error}", LogLevel.ERROR, tlg=True)
-        open_orders = self.get_buffered_open_orders(True)  # lgtm [py/call/wrong-arguments]
+        open_orders = self.get_buffered_open_orders()
         order = None
         if self.orders_init.exist(place_order_id):
             order = self.orders_init.find_order(open_orders, place_order_id)
         elif place_order_id == self.tp_wait_id:
             for k, o in enumerate(open_orders):
                 if o.buy == self.tp_order[0] and o.amount == float(self.tp_order[1]) and o.price == float(self.tp_order[2]):
                     order = open_orders[k]
@@ -3506,15 +3503,15 @@
             if self.tp_cancel:
                 # Restart
                 self.tp_cancel = False
                 self.start()
 
     def on_cancel_order_error_string(self, order_id: int, error: str) -> None:
         # Check all orders on exchange if not exists required
-        open_orders = self.get_buffered_open_orders(True)  # lgtm [py/call/wrong-arguments]
+        open_orders = self.get_buffered_open_orders()
         if any(i.id == order_id for i in open_orders):
             self.message_log(f"On cancel order {order_id} {error}, retry", LogLevel.ERROR)
             self.cancel_order(order_id)
         elif not STANDALONE:
             self.message_log(f"On cancel order {order_id} {error}", LogLevel.ERROR)
             if self.orders_grid.exist(order_id):
                 self.message_log("It's was grid order, probably filled", LogLevel.WARNING)
```

### Comparing `martin_binance-1.3.1b5/martin_binance/funds_rate.db.template` & `martin_binance-1.3.2/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.1b5/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin_binance-1.3.2/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.1b5/martin_binance/margin_wrapper.py` & `martin_binance-1.3.2/martin_binance/margin_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 margin.de <-> Python strategy <-> <margin_wrapper> <-> exchanges-wrapper <-> Exchanges API/WSS
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0-3"
+__version__ = "1.3.2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import ast
 import asyncio
 import simplejson as json
 import logging
@@ -22,14 +22,15 @@
 import shutil
 import psutil
 
 from colorama import init as color_init
 from decimal import Decimal
 from pathlib import Path
 from datetime import datetime, timedelta
+from tqdm import tqdm
 
 # noinspection PyPackageRequirements
 import grpc
 import jsonpickle
 # noinspection PyPackageRequirements
 from google.protobuf import json_format
 from margin_strategy_sdk import LogLevel, OrderUpdate, RoundingType, Dict, List
@@ -39,26 +40,27 @@
 from exchanges_wrapper.definitions import Interval
 from exchanges_wrapper import api_pb2, api_pb2_grpc
 
 from martin_binance import executor as ms, BACKTEST_PATH, copy
 from martin_binance.client import Trade
 from martin_binance.backtest.exchange_simulator import Account as backTestAccount
 
+ORDER_BOOK_PKL = "order_book.pkl"
+TICKER_PKL = "ticker.pkl"
 
 # For more channel options, please see https://grpc.io/grpc/core/group__grpc__arg__keys.html
 CHANNEL_OPTIONS = [('grpc.lb_policy_name', 'pick_first'),
                    ('grpc.enable_retries', 0),
                    ('grpc.keepalive_timeout_ms', 10000)]
 
 loop = asyncio.get_event_loop()
 KLINES_INIT = [Interval.ONE_MINUTE, Interval.FIFTY_MINUTES, Interval.ONE_HOUR]
 KLINES_LIM = 50  # Number of candles must be <= 1000
 CANCEL_ALL_ORDERS = True  # Ask about cancel all active orders before start strategy and ms.LOAD_LAST_STATE = 0
-ALL_TRADES_LIST_LIMIT = 100
-TRADES_LIST_LIMIT = 50
+TRADES_LIST_LIMIT = 100
 HEARTBEAT = 2  # Sec
 RATE_LIMITER = HEARTBEAT * 5
 ORDER_TIMEOUT = HEARTBEAT * 15  # Sec
 # Set logger
 logger = logging.getLogger('logger')
 color_init()
 ms_order_id = 'ms.order_id'
@@ -417,17 +419,15 @@
     quote_asset = str()
     ticker = {}
     funds = {}
     order_book = {}
     order_id = int(datetime.now().strftime("%S%M")) * 1000
     wait_order_id = []  # List of placed orders for time-out detect
     canceled_order_id = []  # List canceled orders  for time-out detect
-    all_trades = []  # List of all (limit = ALL_TRADES_LIST_LIMIT) trades for a specific account and symbol
     trades = []  # List of trades associated with strategy (limit = TRADES_LIST_LIMIT)
-    all_orders = []  # List of all open orders for symbol
     orders = []  # List orders associated with strategy
     tcm = None  # TradingCapabilityManager
     last_state = None
     rate_limiter = RATE_LIMITER
     start_time_ms = int(time.time() * 1000)
     send_request = None
     for_request = None
@@ -509,17 +509,14 @@
 
     def message_log(self, *args, **kwargs):
         pass  # meant to be overridden in a subclass
 
     def order_exist(self, _id) -> bool:
         return any(i.id == _id for i in self.orders)
 
-    def all_order_exist(self, _id) -> bool:
-        return any(i.id == _id for i in self.all_orders)
-
     def get_trading_capability_manager(self) -> TradingCapabilityManager:
         return self.tcm
 
     def get_first_currency(self) -> str:
         return self.info_symbol.get('baseAsset')
 
     def get_second_currency(self) -> str:
@@ -551,22 +548,18 @@
         loop.create_task(create_limit_order(cls.order_id, buy, any2str(amount), any2str(price)))
         if cls.exchange == 'huobi':
             time.sleep(0.02)
         elif cls.exchange == 'okx':
             time.sleep(0.035)
         return cls.order_id
 
-    def get_buffered_completed_trades(self, get_all_trades: bool = False) -> List[PrivateTrade]:
-        if get_all_trades:
-            return self.all_trades
+    def get_buffered_completed_trades(self, _get_all_trades: bool = False) -> List[PrivateTrade]:
         return self.trades
 
-    def get_buffered_open_orders(self, get_all_orders: bool = False) -> List[Order]:
-        if get_all_orders:
-            return self.all_orders
+    def get_buffered_open_orders(self) -> List[Order]:
         return self.orders
 
     def get_time(self) -> float:
         """
         For backtesting purpose. Calculating monotonic local time based on self.time_operational['new'] value.
         It can be set from external source as int(time.time()) getting from historical data. If can't setting
         return system int(time.time()) Unix time.
@@ -619,15 +612,16 @@
     @staticmethod
     def cancel_all_order(order_id: int) -> None:
         loop.create_task(cancel_order_timeout(order_id))
         loop.create_task(cancel_all_order_call(order_id))
 
     @staticmethod
     def transfer_to_master(symbol: str, amount: str):
-        loop.create_task(transfer2master(symbol, amount))
+        if ms.MODE in ('T', 'TC'):
+            loop.create_task(transfer2master(symbol, amount))
 
 
 async def heartbeat(_session):
     cls = StrategyBase
     # print(f"tik-tak:' {int(time.time() * 1000)}")
     last_exec_time = time.time()
     while cls.strategy:
@@ -833,20 +827,21 @@
     :return:
     """
     session_root = Path(BACKTEST_PATH, f"{cls.exchange}_{cls.symbol}")
     raw_path = Path(session_root, "raw")
     raw_path.mkdir(parents=True, exist_ok=True)
     # Save ticker
     ds = pd.Series(cls.s_ticker)
-    ds.to_pickle(Path(raw_path, "ticker.pkl"))
+    ds.to_pickle(Path(raw_path, TICKER_PKL))
     # Save order_book
     ds = pd.Series(cls.s_order_book)
-    ds.to_pickle(Path(raw_path, "order_book.pkl"))
+    ds.to_pickle(Path(raw_path, ORDER_BOOK_PKL))
     # Save klines snapshot
-    json.dump(cls.klines, open(Path(raw_path, "klines.json"), 'w'))
+    with open(Path(raw_path, "klines.json"), 'w') as f:
+        json.dump(cls.klines, f)
     # Save candles
     for k, v in cls.candles.items():
         ds = pd.Series(v)
         ds.to_pickle(Path(raw_path, f"candles_{k}.pkl"))
     # Save session detail for analytics
     session_data = Path(session_root, "snapshot")
     session_data.mkdir(parents=True, exist_ok=True)
@@ -858,15 +853,15 @@
     ds_ticker.index = pd.to_datetime(ds_ticker.index, unit='ms')
     #
     df_grid_sell = pd.DataFrame().from_dict(cls.grid_sell, orient='index')
     df_grid_sell.index = pd.to_datetime(df_grid_sell.index, unit='ms')
     df_grid_buy = pd.DataFrame().from_dict(cls.grid_buy, orient='index')
     df_grid_buy.index = pd.to_datetime(df_grid_buy.index, unit='ms')
     #
-    ds_ticker.to_pickle(Path(session_data, "ticker.pkl"))
+    ds_ticker.to_pickle(Path(session_data, TICKER_PKL))
     df_grid_sell.to_pickle(Path(session_data, "sell.pkl"))
     df_grid_buy.to_pickle(Path(session_data, "buy.pkl"))
     #
     copy(ms.PARAMS, Path(session_root, Path(ms.PARAMS).name))
 
     shutil.make_archive(str(Path(BACKTEST_PATH, f"{session_root}_{datetime.now().strftime('%m%d-%H:%M')}")),
                         'zip',
@@ -952,15 +947,15 @@
             ds = pd.read_pickle(Path(BACKTEST_PATH, f"{cls.exchange}_{cls.symbol}/raw/candles_{i}.pkl"))
             loop.create_task(aiter_candles(ds, _klines, i))
 
 
 async def aiter_candles(ds: pd.Series, _klines: {str: StrategyBase.Klines}, _i: str):
     async for row in loop_ds(ds):
         _klines.get(_i).refresh(json.loads(row))
-    print(f"Backtest candles *** {_i} *** timeSeries ended")
+    StrategyBase.strategy.message_log(f"Backtest candles *** {_i} *** timeSeries ended")
 
 
 async def buffered_funds(print_info: bool = True):
     cls = StrategyBase
     try:
         if ms.MODE in ('T', 'TC'):
             res = await cls.send_request(cls.stub.FetchAccountInformation, api_pb2.OpenClientConnectionId)
@@ -995,15 +990,14 @@
             funds = {cls.base_asset: FundsEntry(cls.funds[cls.base_asset]),
                      cls.quote_asset: FundsEntry(cls.funds[cls.quote_asset])}
             cls.strategy.on_new_funds(funds)
 
 
 async def buffered_orders():
     cls = StrategyBase
-    all_orders = []
     exch_orders_id = []
     save_orders_id = []
     restore = False
     run = False
     while not run:
         try:
             res = await cls.send_request(cls.stub.CheckStream, api_pb2.MarketRequest, symbol=cls.symbol)
@@ -1015,127 +1009,92 @@
         await asyncio.sleep(HEARTBEAT)
     while run:
         try:
             res = await cls.send_request(cls.stub.CheckStream, api_pb2.MarketRequest, symbol=cls.symbol)
             if res is None or not res.success:
                 cls.wss_fire_up = True
                 raise UserWarning(f"Not active WSS for {cls.symbol} on {cls.exchange}, restart request sent")
+
+            if cls.last_state:
+                cls.strategy.message_log("Trying restore saved state after restart", color=ms.Style.GREEN)
+                # Restore StrategyBase class var
+                cls.order_id = json.loads(cls.last_state.pop(ms_order_id,
+                                                             str(int(datetime.now().strftime("%S%M")) * 1000)))
+                cls.start_time_ms = json.loads(cls.last_state.pop('ms_start_time_ms', str(int(time.time() * 1000))))
+                cls.trades = jsonpickle.decode(cls.last_state.pop('ms_trades', '[]'))
+                cls.orders = jsonpickle.decode(cls.last_state.pop(ms_orders, '[]'))
+                #
+                cls.strategy.restore_strategy_state(cls.last_state)
+
+            if restore:
+                cls.strategy.message_log("Trying restore saved state after lost connection to host",
+                                         color=ms.Style.GREEN)
+
             _orders = await cls.send_request(cls.stub.FetchOpenOrders, api_pb2.MarketRequest, symbol=cls.symbol)
             if _orders is None:
                 raise UserWarning("Can't fetch open orders")
             StrategyBase.rate_limiter = max(StrategyBase.rate_limiter, _orders.rate_limiter)
             orders = json_format.MessageToDict(_orders).get('items', [])
             # print(f"buffered_orders.orders: {orders}")
             part_id = []
             for order in orders:
                 _id = int(order['orderId'])
-                all_orders.append(Order(order))
                 exch_orders_id.append(_id)
                 if (order.get('status', None) == 'PARTIALLY_FILLED'
                         and order_trades_sum(_id) < Decimal(order['executedQty'])):
                     part_id.append(_id)
-            for i in cls.all_orders:
+            for i in cls.orders:
                 save_orders_id.append(i.id)
             # Missed fill event list
             diff_id = list(set(save_orders_id).difference(exch_orders_id))
             # print(f"buffered_orders.diff_id: {diff_id}")
             # Erroneously not deleted order
             diff_excess_id = list(set(exch_orders_id).
                                   difference(save_orders_id).
                                   intersection(cls.canceled_order_id))
             # print(f"buffered_orders.diff_excess_id: {diff_excess_id}")
             exch_orders_id.clear()
             save_orders_id.clear()
-            if not (restore or cls.last_state) and (diff_id or part_id):
+            if diff_id or part_id:
                 cls.strategy.message_log(f"Perhaps was missed event for order(s): {diff_id + part_id},"
                                          f" checking it", log_level=LogLevel.WARNING, tlg=False)
                 for _id in list(set(diff_id + part_id)):
                     await fetch_order(_id, _filled_update_call=True)
                 part_id.clear()
-            if not (restore or cls.last_state) and diff_excess_id:
+            if diff_excess_id:
                 cls.strategy.message_log(f"Find excess order(s): {diff_excess_id}, checking it",
                                          log_level=LogLevel.WARNING, tlg=False)
                 for _id in diff_excess_id:
                     check_status = await fetch_order(_id, _filled_update_call=False)
                     if check_status and check_status.get('status') not in ('FILLED', 'CANCELED'):
                         cls.strategy.message_log(f"buffered_orders.create_task: cancel_order: {_id}",
                                                  log_level=LogLevel.INFO)
                         loop.create_task(cancel_order_timeout(_id))
                         loop.create_task(cancel_order_call(_id))
-            cls.all_orders = all_orders.copy()
-            all_orders.clear()
-            if restore or cls.last_state:
-                if restore:
-                    cls.strategy.message_log("Trying restore saved state after lost connection to host",
-                                             color=ms.Style.GREEN)
-                else:
-                    cls.strategy.message_log("Trying restore saved state after restart", color=ms.Style.GREEN)
-                try:
-                    last_state = {}
-                    if cls.last_state:
-                        last_state.update(cls.last_state)
-                        cls.last_state = None
-                        # Restore StrategyBase class var
-                        cls.order_id = json.loads(last_state.pop(ms_order_id,
-                                                                 str(int(datetime.now().strftime("%S%M")) * 1000)))
-                        cls.start_time_ms = json.loads(last_state.pop('ms_start_time_ms', str(int(time.time() * 1000))))
-                        cls.trades = jsonpickle.decode(last_state.pop('ms_trades', '[]'))
-                        cls.orders = jsonpickle.decode(last_state.pop(ms_orders, '[]'))
-                    else:
-                        last_state.pop(ms_order_id, None)
-                        # last_state.pop('ms.trades', None)
-                        last_state.pop(ms_orders, None)
-                    # Get trades for strategy
-                    _trades = await cls.send_request(cls.stub.FetchAccountTradeList, api_pb2.AccountTradeListRequest,
-                                                     symbol=cls.symbol,
-                                                     limit=ALL_TRADES_LIST_LIMIT,
-                                                     start_time=cls.start_time_ms)
-                    trades = json_format.MessageToDict(_trades).get('items', [])
-                    # print(f"main.trades: {trades}")
-                    for trade in trades:
-                        cls.all_trades.append(PrivateTrade(trade))
-                    # Update StrategyBase class var
-                    exch_orders_id = []
-                    ms_orders_id = []
-                    for i in cls.all_orders:
-                        exch_orders_id.append(i.id)
-                    # print(f"buffered_orders.exch_orders_id: {exch_orders_id}")
-                    for i in cls.orders:
-                        ms_orders_id.append(i.id)
-                    # print(f"buffered_orders.ms_orders_id: {ms_orders_id}")
-                    diff_id = list(set(ms_orders_id).difference(exch_orders_id))
-                    if diff_id:
-                        cls.strategy.message_log(f"Executed order(s) is: {diff_id}", log_level=LogLevel.INFO)
-                        for _id in diff_id:
-                            await fetch_order(_id, _filled_update_call=True)
-                    if not restore:
-                        cls.strategy.restore_strategy_state(last_state)
-                        if ms.MODE == 'TC':
-                            last_state = cls.strategy.save_strategy_state(return_only=True)
-                            last_state_update(cls, last_state)
-                            with cls.state_file.open(mode='w') as outfile:
-                                json.dump(last_state, outfile, sort_keys=True, indent=4, ensure_ascii=False)
-                            cls.strategy.start_collect = True
-                except Exception as _ex:
-                    cls.last_state = None
-                    cls.strategy.message_log(f"Exception restore_strategy_state: {_ex}\n{traceback.format_exc()}",
-                                             log_level=LogLevel.WARNING)
-                else:
-                    restore = False
-                    cls.strategy.message_log("Restored successfully", color=ms.Style.GREEN)
+
+            if ms.MODE == 'TC' and cls.last_state:
+                last_state = cls.strategy.save_strategy_state(return_only=True)
+                last_state_update(cls, last_state)
+                with cls.state_file.open(mode='w') as outfile:
+                    json.dump(last_state, outfile, sort_keys=True, indent=4, ensure_ascii=False)
+                cls.strategy.start_collect = True
+
+            cls.last_state = None
+            restore = False
+
         except asyncio.CancelledError:
             # print("buffered_orders.Cancelled")
             run = False
         except UserWarning as ex:
             cls.strategy.message_log(f"Exception buffered_orders: {ex}", log_level=LogLevel.WARNING)
             restore = True
         except grpc.RpcError as ex:
             status_code = ex.code()
             cls.strategy.message_log(f"Exception buffered_orders: {status_code.name}, {ex.details()}",
-                                     log_level=LogLevel.WARNING, tlg=True)
+                                     log_level=LogLevel.WARNING, color=ms.Style.B_RED, tlg=True)
             if status_code == grpc.StatusCode.RESOURCE_EXHAUSTED:
                 # Decrease requests frequency
                 StrategyBase.rate_limiter += HEARTBEAT
                 cls.strategy.message_log(f"RATE_LIMITER set to {StrategyBase.rate_limiter}s",
                                          log_level=LogLevel.WARNING)
                 await asyncio.sleep(ORDER_TIMEOUT)
                 await cls.send_request(cls.stub.ResetRateLimit, api_pb2.OpenClientConnectionId,
@@ -1216,17 +1175,14 @@
                      "orderId": ed['order_id'],
                      "price": ed['last_executed_price'],
                      "time": ed['transaction_time']}
             #  Append to all_trades and trades list
             if len(cls.trades) > TRADES_LIST_LIMIT:
                 del cls.trades[0]
             cls.trades.append(PrivateTrade(trade))
-            if len(cls.all_trades) > ALL_TRADES_LIST_LIMIT:
-                del cls.all_trades[0]
-                cls.all_trades.append(PrivateTrade(trade))
             cumulative_quantity = Decimal(ed['cumulative_filled_quantity'])
             saved_filled_quantity = order_trades_sum(ed['order_id'])
             if ed['order_status'] == 'FILLED' and saved_filled_quantity != cumulative_quantity:
                 cls.strategy.message_log(f"Order: {ed['order_id']} was missed partially filling event",
                                          log_level=LogLevel.INFO)
                 # Remove trades associated with order from list
                 remove_from_trades_lists(ed['order_id'])
@@ -1295,20 +1251,16 @@
                          "orderId": order.id,
                          "price": price,
                          "time": order.timestamp}
                 # cls.strategy.message_log(f"place_limit_order_callback.trade: {trade}", color=ms.Style.YELLOW)
                 if len(cls.trades) > TRADES_LIST_LIMIT:
                     del cls.trades[0]
                 cls.trades.append(PrivateTrade(trade))
-                if len(cls.all_trades) > ALL_TRADES_LIST_LIMIT:
-                    del cls.all_trades[0]
-                cls.all_trades.append(PrivateTrade(trade))
             if executed_qty < orig_qty:
                 cls.orders.append(order)
-                cls.all_orders.append(order)
             if ms.MODE == 'TC' and cls.strategy.start_collect:
                 cls.strategy.open_orders_snapshot()
             elif ms.MODE == 'S':
                 await on_funds_update()
             cls.strategy.on_place_order_success(_id, order)
 
 
@@ -1405,17 +1357,17 @@
         cls.strategy.message_log(f"Exception in fetch_order: {_ex}", log_level=LogLevel.ERROR)
         return {}
     else:
         cls.strategy.message_log(f"For order {_id} fetched status is {result.get('status')}",
                                  log_level=LogLevel.INFO)
         if _filled_update_call and result and result.get('status') == 'CANCELED':
             remove_from_orders_lists([_id])
-            cls.strategy.message_log(f"Cancel order {_id} OK", color=ms.Style.GREEN)
-            cls.strategy.on_cancel_order_success(_id, Order(result))
             cls.canceled_order_id.append(_id)
+            cls.strategy.message_log(f"Order {_id} has already been deleted", color=ms.Style.GREEN)
+            cls.strategy.on_cancel_order_success(_id, Order(result))
         return result
 
 
 async def transfer2master(symbol: str, amount: str):
     cls = StrategyBase
     try:
         res = await cls.send_request(cls.stub.TransferToMaster,
@@ -1437,22 +1389,20 @@
                                      log_level=LogLevel.ERROR)
 
 
 def remove_from_orders_lists(_order_id_list: []) -> None:
     cls = StrategyBase
     # print(f"remove_from_orders_lists._order_id: {_order_id}")
     cls.orders[:] = [i for i in cls.orders if i.id not in _order_id_list]
-    cls.all_orders[:] = [i for i in cls.all_orders if i.id not in _order_id_list]
 
 
 def remove_from_trades_lists(_order_id) -> None:
     cls = StrategyBase
     # print(f"remove_from_trades_lists._order_id: {_order_id}")
     cls.trades[:] = [i for i in cls.trades if i.order_id != _order_id]
-    cls.all_trades[:] = [i for i in cls.all_trades if i.order_id != _order_id]
 
 
 async def loop_ds(ds, tik=False):
     """
     Pandas time Series asynchronous generator with delay (real time/XTIME) multiplier
     :param tik: True - update local time
     :param ds: pandas time Series object
@@ -1492,22 +1442,25 @@
                     ticker_24h['delay'] = cls.delay_ordering_s
                     cls.strategy.s_ticker.update({int(time.time() * 1000): ticker_24h})
                     cls.strategy.open_orders_snapshot()
         except Exception as ex:
             logger.warning(f"Exception on WSS, on_ticker_update loop closed: {ex}")
             cls.wss_fire_up = True
     else:
+        pbar = tqdm(total=cls.backtest['ticker'].count())
         async for row in loop_ds(cls.backtest['ticker'], tik=True):
             cls.delay_ordering_s = row.pop('delay', 0)
             cls.ticker = row
             cls.strategy.on_new_ticker(Ticker(row))
             res = cls.strategy.account.on_ticker_update(row, int(cls.strategy.local_time() * 1000))
             for _res in res:
                 on_order_update_handler(cls, _res)
                 await on_funds_update()
+            pbar.update()
+        pbar.close()
         cls.strategy.message_log("Backtest *** ticker *** timeSeries ended")
         back_test_handler(cls)
 
 
 def back_test_handler(cls):
     # Test result handler
     test_time = datetime.utcnow() - cls.strategy.cycle_time
@@ -1522,15 +1475,15 @@
         ds_ticker = pd.Series(cls.strategy.account.ticker).astype(float)
         ds_ticker.index = pd.to_datetime(ds_ticker.index, unit='ms')
         df_grid_sell = pd.DataFrame().from_dict(cls.strategy.account.grid_sell, orient='index').astype(float)
         df_grid_sell.index = pd.to_datetime(df_grid_sell.index, unit='ms')
         df_grid_buy = pd.DataFrame().from_dict(cls.strategy.account.grid_buy, orient='index').astype(float)
         df_grid_buy.index = pd.to_datetime(df_grid_buy.index, unit='ms')
         #
-        ds_ticker.to_pickle(Path(session_path, "ticker.pkl"))
+        ds_ticker.to_pickle(Path(session_path, TICKER_PKL))
         df_grid_sell.to_pickle(Path(session_path, "sell.pkl"))
         df_grid_buy.to_pickle(Path(session_path, "buy.pkl"))
         copy(ms.PARAMS, Path(session_path, Path(ms.PARAMS).name))
         print(f"Session data saved to: {session_path}")
         #
     s_profit = session_result['profit'] = f"{cls.strategy.get_sum_profit()}"
     s_free = session_result['free'] = f"{cls.strategy.get_free_assets(mode='free', backtest=True)[2]}"
@@ -1568,15 +1521,15 @@
         except Exception as ex:
             logger.warning(f"Exception on WSS, on_order_book_update loop closed: {ex}")
             cls.wss_fire_up = True
     else:
         async for row in loop_ds(cls.backtest['order_book']):
             cls.order_book = row
             cls.strategy.on_new_order_book(OrderBook(cls.order_book))
-        print("Backtest *** order_book *** timeSeries ended")
+        cls.strategy.message_log("Backtest *** order_book *** timeSeries ended")
 
 
 def load_file(name: Path) -> {}:
     _res = {}
     if name.exists():
         try:
             with name.open() as state_file:
@@ -1697,14 +1650,27 @@
     cls.strategy.tp_init = eval(json.loads(saved_state.get('tp_init')))
     cls.strategy.tp_order_id = json.loads(saved_state.get('tp_order_id'))
     cls.strategy.tp_part_amount_first = ms.f2d(json.loads(saved_state.get('tp_part_amount_first')))
     cls.strategy.tp_part_amount_second = ms.f2d(json.loads(saved_state.get('tp_part_amount_second')))
     cls.strategy.tp_target = ms.f2d(json.loads(saved_state.get('tp_target')))
     cls.strategy.tp_order = eval(json.loads(saved_state.get('tp_order')))
     cls.strategy.tp_wait_id = json.loads(saved_state.get('tp_wait_id'))
+    # Restore TP order
+    tp_order = [
+        {"id": cls.strategy.tp_order_id,
+         "buy": cls.strategy.tp_order[0],
+         "amount": cls.strategy.tp_order[1],
+         "price": cls.strategy.tp_order[2]}
+    ]
+    cls.strategy.account.restore_state(
+        cls.symbol,
+        cls.start_time_ms,
+        tp_order,
+        tp=(cls.strategy.sum_amount_first, cls.strategy.sum_amount_second)
+    )
     cls.strategy.start_collect = True
 
 
 async def main(_symbol):
     cls = StrategyBase
     cls.strategy = ms.Strategy()
     restore_state = None
@@ -1818,17 +1784,17 @@
             cls.strategy.account.funds.quote = {'asset': cls.quote_asset,
                                                 'free': f"{ms.AMOUNT_SECOND}",
                                                 'locked': '0.0'}
             cls.strategy.account.fee_maker = ms.FEE_MAKER
             cls.strategy.account.fee_taker = ms.FEE_TAKER
             #
             cls.backtest['ticker'] = pd.read_pickle(Path(BACKTEST_PATH,
-                                                         f"{cls.exchange}_{cls.symbol}/raw/ticker.pkl"))
+                                                         f"{cls.exchange}_{cls.symbol}/raw/{TICKER_PKL}"))
             cls.backtest['order_book'] = pd.read_pickle(Path(BACKTEST_PATH,
-                                                             f"{cls.exchange}_{cls.symbol}/raw/order_book.pkl"))
+                                                             f"{cls.exchange}_{cls.symbol}/raw/{ORDER_BOOK_PKL}"))
             cls.ticker = cls.backtest['ticker'].iat[0]
             cls.order_book = cls.backtest['order_book'].iat[0]
         #
         await buffered_funds()
         answer = str()
         restored = True
         if restore_state:
```

### Comparing `martin_binance-1.3.1b5/martin_binance/ms_cfg.toml.template` & `martin_binance-1.3.2/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.1b5/martin_binance/service/funds_rate_exporter.py` & `martin_binance-1.3.2/martin_binance/service/funds_rate_exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Config for prometheus_client
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0-2"
+__version__ = "1.3.1-2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 
 import os
 import time
 import sqlite3
 import psutil
@@ -168,28 +168,28 @@
     for row in records:
         _currency_rate.setdefault(str(row[2]))
         _currency_rate.setdefault(str(row[3]))
     # Get currency rate for all currency from CoinMarketCap in relation to USD
     time_for_refresh = time.time() - currency_rate_last_time > 86400
     if None in _currency_rate.values() or time_for_refresh:
         get_rate(_currency_rate)
-        if time_for_refresh:
-            F_BALANCE.clear()
-            S_BALANCE.clear()
-            TOTAL_BALANCE.clear()
-            BALANCE_USD.clear()
-            CYCLE_BUY.clear()
-            F_DEPO.clear()
-            S_DEPO.clear()
-            OVER_PRICE.clear()
         currency_rate_last_time = int(time.time())
         REQUEST_DELAY_G.labels(VPS_NAME).set(request_delay)
         if request_delay > 60:
             request_delay = 60 / config.get('rate_limit')
     #
+    F_BALANCE.clear()
+    S_BALANCE.clear()
+    TOTAL_BALANCE.clear()
+    BALANCE_USD.clear()
+    CYCLE_BUY.clear()
+    F_DEPO.clear()
+    S_DEPO.clear()
+    OVER_PRICE.clear()
+    #
     for row in records:
         # print(f"row: {row}")
         exchange = str(row[0])
         name = names.get(exchange)
         id_exchange = int(row[1])
         f_currency = str(row[2])
         s_currency = str(row[3])
```

### Comparing `martin_binance-1.3.1b5/martin_binance/service/grafana.json` & `martin_binance-1.3.2/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.1b5/martin_binance/service/relaunch.py` & `martin_binance-1.3.2/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.1b5/pyproject.toml` & `martin_binance-1.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
-    "exchanges-wrapper==1.3.1",
+    "exchanges-wrapper==1.3.2",
     "margin-strategy-sdk==0.0.11",
     "aiohttp==3.8.4",
     "grpcio==1.48.1",
     "grpcio-tools==1.48.1",
     "jsonpickle==3.0.1",
     "psutil==5.9.5",
     "requests==2.31.0",
@@ -31,15 +31,18 @@
     "colorama==0.4.6",
     "prometheus-client==0.17.0",
     "optuna==3.2.0",
     "plotly==5.15.0",
     "pandas==2.0.2",
     "dash==2.10.2",
     "future==0.18.3",
-    "inquirer==3.1.3"
+    "inquirer==3.1.3",
+    "scikit-learn==1.2.2",
+    "tqdm==4.65.0",
+    "shortuuid==1.0.11",
 ]
 
 [tool.flit.module]
 name = "martin_binance"
 
 [project.urls]
 Source = "https://github.com/DogsTailFarmer/martin-binance"
```

### Comparing `martin_binance-1.3.1b5/PKG-INFO` & `martin_binance-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.3.1b5
+Version: 1.3.2
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper==1.3.1
+Requires-Dist: exchanges-wrapper==1.3.2
 Requires-Dist: margin-strategy-sdk==0.0.11
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: grpcio==1.48.1
 Requires-Dist: grpcio-tools==1.48.1
 Requires-Dist: jsonpickle==3.0.1
 Requires-Dist: psutil==5.9.5
 Requires-Dist: requests==2.31.0
@@ -26,14 +26,17 @@
 Requires-Dist: prometheus-client==0.17.0
 Requires-Dist: optuna==3.2.0
 Requires-Dist: plotly==5.15.0
 Requires-Dist: pandas==2.0.2
 Requires-Dist: dash==2.10.2
 Requires-Dist: future==0.18.3
 Requires-Dist: inquirer==3.1.3
+Requires-Dist: scikit-learn==1.2.2
+Requires-Dist: tqdm==4.65.0
+Requires-Dist: shortuuid==1.0.11
 Project-URL: Source, https://github.com/DogsTailFarmer/martin-binance
 
 <p align="center"><img src="https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/Modified%20martingale.svg" width="250"></p>
 <h3 align="center">Profitable, fault-tolerant, adaptable to the market</h3>
 
 ***
 <h1 align="center">Modified Martingale</h1>
@@ -69,14 +72,15 @@
 > 
 >Incorrectly: (BTC/USDT), (ETH/USDT), (BTC/ETH)
 > 
 >As a result of the mutual impact on the operating balance sheet, the liquidity control system will block the work.
 
 ## References
 * Detailed information about use this strategy placed to [wiki](https://github.com/DogsTailFarmer/martin-binance/wiki)
+* [Trade idea](https://github.com/DogsTailFarmer/martin-binance/wiki/Trade-idea)
 * [Quick start](https://github.com/DogsTailFarmer/martin-binance/wiki/Quick-start)
 * [Back testing and parameters optimization](https://github.com/DogsTailFarmer/martin-binance/wiki/Back-testing-and-parameters-optimization)
 
 ## Referral link
 <p id="referral-link"></p>
 
 Create account on [Binance](https://accounts.binance.com/en/register?ref=QCS4OGWR) and get 10% discount on all trading
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 1.3.1b5 Summary: Free
-trading system for Binance SPOT API Author-email: Jerry Fedorenko
+Metadata-Version: 2.1 Name: martin-binance Version: 1.3.2 Summary: Free trading
+system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: exchanges-wrapper==1.3.1 Requires-Dist: margin-strategy-sdk==0.0.11
+Dist: exchanges-wrapper==1.3.2 Requires-Dist: margin-strategy-sdk==0.0.11
 Requires-Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.48.1 Requires-Dist:
 grpcio-tools==1.48.1 Requires-Dist: jsonpickle==3.0.1 Requires-Dist:
 psutil==5.9.5 Requires-Dist: requests==2.31.0 Requires-Dist: simplejson==3.19.1
 Requires-Dist: toml==0.10.2 Requires-Dist: libtmux==0.22.1 Requires-Dist:
 colorama==0.4.6 Requires-Dist: prometheus-client==0.17.0 Requires-Dist:
 optuna==3.2.0 Requires-Dist: plotly==5.15.0 Requires-Dist: pandas==2.0.2
 Requires-Dist: dash==2.10.2 Requires-Dist: future==0.18.3 Requires-Dist:
-inquirer==3.1.3 Project-URL: Source, https://github.com/DogsTailFarmer/martin-
-binance
+inquirer==3.1.3 Requires-Dist: scikit-learn==1.2.2 Requires-Dist: tqdm==4.65.0
+Requires-Dist: shortuuid==1.0.11 Project-URL: Source, https://github.com/
+DogsTailFarmer/martin-binance
        [https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/
                           Modified%20martingale.svg]
          **** Profitable, fault-tolerant, adaptable to the market ****
 ***
                        ****** Modified Martingale ******
                ***** Cyclic grid strategy for SPOT market *****
 **** Free trading system for crypto exchanges (Binance, Bitfinex, Huobi, OKX,)
@@ -36,16 +37,17 @@
 updated ```cli_X_AAABBB.py```, use ```martin_binance/
 cli_0_BTCUSDT.py.template``` for compare and update * You cannot run multiple
 pairs with overlapping currencies on the same account! >Valid: (BTC/USDT),
 (ETH/BUSD), (SOL/LTC) > >Incorrectly: (BTC/USDT), (ETH/USDT), (BTC/ETH) > >As a
 result of the mutual impact on the operating balance sheet, the liquidity
 control system will block the work. ## References * Detailed information about
 use this strategy placed to [wiki](https://github.com/DogsTailFarmer/martin-
-binance/wiki) * [Quick start](https://github.com/DogsTailFarmer/martin-binance/
-wiki/Quick-start) * [Back testing and parameters optimization](https://
+binance/wiki) * [Trade idea](https://github.com/DogsTailFarmer/martin-binance/
+wiki/Trade-idea) * [Quick start](https://github.com/DogsTailFarmer/martin-
+binance/wiki/Quick-start) * [Back testing and parameters optimization](https://
 github.com/DogsTailFarmer/martin-binance/wiki/Back-testing-and-parameters-
 optimization) ## Referral link
 Create account on [Binance](https://accounts.binance.com/en/
 register?ref=QCS4OGWR) and get 10% discount on all trading fee Create account
 on [HUOBI](https://www.huobi.com/en-us/topic/double-reward/
 ?invite_code=9uaw3223) and will get 50 % off trading fees Create account on
 [Bitfinex](https://www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6%
```

