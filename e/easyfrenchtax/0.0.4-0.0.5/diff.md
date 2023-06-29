# Comparing `tmp/easyfrenchtax-0.0.4.tar.gz` & `tmp/easyfrenchtax-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfrenchtax-0.0.4.tar", last modified: Fri Jun  2 20:58:45 2023, max compression
+gzip compressed data, was "easyfrenchtax-0.0.5.tar", last modified: Thu Jun 29 16:04:20 2023, max compression
```

## Comparing `easyfrenchtax-0.0.4.tar` & `easyfrenchtax-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-02 20:58:45.124373 easyfrenchtax-0.0.4/
--rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.4/LICENSE
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-06-02 20:58:45.124444 easyfrenchtax-0.0.4/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.4/README.md
--rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.4/pyproject.toml
--rw-r--r--   0 hadrien    (501) staff       (20)      853 2023-06-02 20:58:45.124714 easyfrenchtax-0.0.4/setup.cfg
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-02 20:58:45.121005 easyfrenchtax-0.0.4/src/
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-02 20:58:45.122417 easyfrenchtax-0.0.4/src/easyfrenchtax/
--rw-r--r--   0 hadrien    (501) staff       (20)      100 2022-06-09 10:23:03.000000 easyfrenchtax-0.0.4/src/easyfrenchtax/__init__.py
--rw-r--r--   0 hadrien    (501) staff       (20)    21521 2023-06-02 20:57:43.000000 easyfrenchtax-0.0.4/src/easyfrenchtax/stock_helper.py
--rw-r--r--   0 hadrien    (501) staff       (20)    27735 2023-06-02 20:57:34.000000 easyfrenchtax-0.0.4/src/easyfrenchtax/tax_simulator.py
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-02 20:58:45.123052 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-06-02 20:58:45.000000 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)      480 2023-06-02 20:58:45.000000 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/SOURCES.txt
--rw-r--r--   0 hadrien    (501) staff       (20)        1 2023-06-02 20:58:45.000000 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/dependency_links.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       18 2023-06-02 20:58:45.000000 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/requires.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       14 2023-06-02 20:58:45.000000 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/top_level.txt
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-02 20:58:45.124248 easyfrenchtax-0.0.4/tests/
--rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.4/tests/test_capital_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.4/tests/test_fiscal_advantages.py
--rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.4/tests/test_income_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.4/tests/test_rental_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    11721 2023-06-02 20:57:43.000000 easyfrenchtax-0.0.4/tests/test_stock_helper.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-29 16:04:20.818938 easyfrenchtax-0.0.5/
+-rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.5/LICENSE
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-06-29 16:04:20.819012 easyfrenchtax-0.0.5/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.5/README.md
+-rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.5/pyproject.toml
+-rw-r--r--   0 hadrien    (501) staff       (20)      853 2023-06-29 16:04:20.819304 easyfrenchtax-0.0.5/setup.cfg
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-29 16:04:20.815135 easyfrenchtax-0.0.5/src/
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-29 16:04:20.816553 easyfrenchtax-0.0.5/src/easyfrenchtax/
+-rw-r--r--   0 hadrien    (501) staff       (20)      100 2022-06-09 10:23:03.000000 easyfrenchtax-0.0.5/src/easyfrenchtax/__init__.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    19882 2023-06-29 16:02:58.000000 easyfrenchtax-0.0.5/src/easyfrenchtax/stock_helper.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    27735 2023-06-02 20:57:34.000000 easyfrenchtax-0.0.5/src/easyfrenchtax/tax_simulator.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-29 16:04:20.817365 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-06-29 16:04:20.000000 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)      480 2023-06-29 16:04:20.000000 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/SOURCES.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)        1 2023-06-29 16:04:20.000000 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/dependency_links.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       18 2023-06-29 16:04:20.000000 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/requires.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       14 2023-06-29 16:04:20.000000 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/top_level.txt
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-29 16:04:20.818693 easyfrenchtax-0.0.5/tests/
+-rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.5/tests/test_capital_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.5/tests/test_fiscal_advantages.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.5/tests/test_income_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.5/tests/test_rental_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    12933 2023-06-29 16:00:34.000000 easyfrenchtax-0.0.5/tests/test_stock_helper.py
```

### Comparing `easyfrenchtax-0.0.4/LICENSE` & `easyfrenchtax-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.4/PKG-INFO` & `easyfrenchtax-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfrenchtax-0.0.4/README.md` & `easyfrenchtax-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.4/setup.cfg` & `easyfrenchtax-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easyfrenchtax
-version = 0.0.4
+version = 0.0.5
 author = Hadrien Hamel
 author_email = hadrien.hamel@gmail.com
 license = MIT
 description = A simulator of French taxes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/had/easyfrenchtax
```

### Comparing `easyfrenchtax-0.0.4/src/easyfrenchtax/stock_helper.py` & `easyfrenchtax-0.0.5/src/easyfrenchtax/stock_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from dataclasses import dataclass
 from datetime import date, datetime
+from typing import Optional
+
 from dateutil.relativedelta import relativedelta
 from currency_converter import CurrencyConverter
 from collections import defaultdict
 import csv
 import glob
 
 
@@ -28,19 +30,22 @@
 
 
 @dataclass
 class SaleEvent:
     symbol: str
     stock_type: str  # TODO change to enum
     nb_stocks_sold: int
-    unit_acquisition_price: float
+    unit_acquisition_price: float # in Euros
     sell_date: date
     sell_price_eur: float
-    sell_details: list[dict[str, any]]  # TODO typing of details
     selling_fees: float
+    owner: Optional[int] = None
+    plan_name: Optional[str] = None
+    acq_date: Optional[date] = None
+
 
 
 # currency converter (USD/EUR in particular)
 cc = CurrencyConverter(fallback_on_wrong_date=True, fallback_on_missing_rate=True)
 
 
 class StockHelper:
@@ -92,17 +97,17 @@
     # ----- RSU related load functions ------
     @staticmethod
     def _determine_rsu_plans_type(approval_date: date) -> str:
         if approval_date <= date(2012, 9, 27):
             return "2007"  # TODO replace with an enum
         elif approval_date <= date(2015, 8, 8):
             return "2012"
-        elif approval_date <= date(2017, 1, 1):
+        elif approval_date <= date(2016, 12, 30):
             return "2015"
-        elif approval_date <= date(2018, 1, 1):
+        elif approval_date <= date(2017, 12, 31):
             return "2017"
         else:
             return "2018"
 
     ## IMPORTANT! approval_date here is used to determine the taxation scheme
     # (Macron I, Macron II, etc.) so it needs to be the date where the plan was
     # approved by the shareholders, NOT the grant date.
@@ -193,55 +198,46 @@
 
     ####### stock selling related load functions #######
 
     def sell_stockoptions(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
                           currency: str = "EUR"):
         if nb_stocks == 0:
             return
-        sell_details = []
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
         stocks_before_sell_date = [r for r in self.stock_options[symbol] if r.acq_date < sell_date]
         for i, acq in enumerate(stocks_before_sell_date):
             if acq.available == 0:
                 continue
             sell_from_acq = min(to_sell, acq.available)
             strike_price_eur = acq.acq_price_eur if acq.acq_price_eur else cc.convert(acq.acq_price, currency, "EUR",
                                                                                       date=sell_date)
-            sell_details.append({
-                "owner": acq.owner,
-                "plan_name": acq.plan_name,
-                "count": sell_from_acq,
-                "strike_price_eur": strike_price_eur,
-                "acq_date": acq.acq_date
-            })
-            # update the rsu data with new availability (tuples are immutable, so replace with new one)
+            self.stock_sales[sell_date.year].append(SaleEvent(
+                symbol=symbol,
+                stock_type="stockoption",
+                nb_stocks_sold=sell_from_acq,
+                unit_acquisition_price=strike_price_eur,  # re-using this field to store the strike price
+                sell_date=sell_date,
+                sell_price_eur=sell_price_eur,
+                selling_fees=round(cc.convert(fees, currency, "EUR", date=sell_date), 2),
+                owner=acq.owner
+            ))
+            # update the stock options data with new availability
             self.stock_options[symbol][i].available = acq.available - sell_from_acq
             to_sell -= sell_from_acq
             if to_sell == 0:
                 break
         if to_sell > 0:
             print(f"WARNING: You are trying to sell more stocks ({nb_stocks}) than you have ({to_sell})")
-        self.stock_sales[sell_date.year].append(SaleEvent(
-            symbol=symbol,
-            stock_type="stockoption",
-            nb_stocks_sold=nb_stocks - to_sell,
-            unit_acquisition_price=None,  # not applicable for stock options when doing "exercise and sell"
-            sell_date=sell_date,
-            sell_price_eur=sell_price_eur,
-            sell_details=sell_details,
-            selling_fees=round(cc.convert(fees, currency, "EUR", date=sell_date), 2)
-        ))
-        return ((nb_stocks - to_sell), None, sell_details)
+        return nb_stocks - to_sell
 
     def sell_espp(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
                   currency: str = "EUR"):
         if nb_stocks == 0:
             return
-        sell_details = []
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
         stocks_before_sell_date = [r for r in self.espp_stocks[symbol] if r.acq_date < sell_date]
         for i, acq in enumerate(stocks_before_sell_date):
             if acq.available == 0:
                 continue
             sell_from_acq = min(to_sell, acq.available)
@@ -250,34 +246,27 @@
             self.stock_sales[sell_date.year].append(SaleEvent(
                 symbol=symbol,
                 stock_type="espp",
                 nb_stocks_sold=sell_from_acq,
                 unit_acquisition_price=round(acq.acq_price_eur, 2),
                 sell_date=sell_date,
                 sell_price_eur=sell_price_eur,
-                sell_details=[{
-                    "plan_name": acq.plan_name,
-                    "count": sell_from_acq,
-                    "acq_price": acq.acq_price,  # keep price in original currency here
-                    "acq_date": acq.acq_date
-                }],
                 selling_fees=0  # not sure how to handle this
             ))
             if to_sell == 0:
                 break
         if to_sell > 0:
             print(f"WARNING: You are trying to sell more stocks ({nb_stocks}) than you have")
             return (0, 0, [])
         return (nb_stocks - to_sell)
 
     def sell_rsus(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
                   currency: str = "EUR") -> int:
         if nb_stocks == 0:
             return 0
-        sell_details = []
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
 
         # Acquisitions are sorted by date, this is the rule set by the tax office (FIFO, or PEPS="premier entré premier
         # sorti"); we only keep stocks acquired *before* the sell date, in case we input a sell event in the middle of
         # acquisitions.
         rsu_before_sell_date = [r for r in self.rsus[symbol] if r.acq_date < sell_date]
@@ -291,40 +280,26 @@
             self.stock_sales[sell_date.year].append(SaleEvent(
                 symbol=symbol,
                 stock_type="rsu",
                 nb_stocks_sold=sell_from_acq,
                 unit_acquisition_price=round(acq.acq_price_eur, 2),
                 sell_date=sell_date,
                 sell_price_eur=sell_price_eur,
-                sell_details=[{
-                    "plan_name": acq.plan_name,
-                    "count": sell_from_acq,
-                    "acq_price": acq.acq_price,  # keep price in original currency here
-                    "acq_price_currency": "TODO",  # TODO
-                    "acq_date": acq.acq_date
-                }],
-                selling_fees=0  # not sure how to handle this
+                selling_fees=0,  # not sure how to handle this
+                owner=None,
+                plan_name=acq.plan_name,
+                acq_date=acq.acq_date
             ))
             # update the rsu data with new availability (tuples are immutable, so replace with new one)
             self.rsus[symbol][i].available = acq.available - sell_from_acq
             to_sell -= sell_from_acq
             if to_sell == 0:
                 break
         if to_sell > 0:
             print(f"WARNING: You are trying to sell more stocks ({nb_stocks}) than you have ({to_sell})")
-        # self.stock_sales[sell_date.year].append(SaleEvent(
-        #     symbol=symbol,
-        #     stock_type="rsu",
-        #     nb_stocks_sold=nb_stocks - to_sell,
-        #     unit_acquisition_price=-1,
-        #     sell_date=sell_date,
-        #     sell_price_eur=sell_price_eur,
-        #     sell_details=sell_details,
-        #     selling_fees=round(cc.convert(fees, currency, "EUR", date=sell_date), 2)
-        # ))
         return (nb_stocks - to_sell)
 
     ####### tax computation functions #######
 
     # the bible of acquisition and capital gain tax (version 2021):
     # https://www.impots.gouv.fr/portail/www2/fichiers/documentation/brochure/ir_2021/pdf_som/09-plus_values_141a158.pdf
     def compute_acquisition_gain_tax(self, year: int):
@@ -335,53 +310,50 @@
         other_taxable_gain_1 = 0  # this would contribute to box 1TT
         other_taxable_gain_2 = 0  # this would contribute to box 1UT
 
         for sale in sell_events:
             if sale.stock_type == "stockoption":
                 # exercise gain only applies to Stock Options
                 # /!\ only stock options attributed after 28/09/2012 are supported
-                for sale_detail in sale.sell_details:
-                    exercise_gain_eur = sale_detail["count"] * (sale.sell_price_eur - sale_detail["strike_price_eur"])
-                    if sale_detail["owner"] == 1:
-                        other_taxable_gain_1 += exercise_gain_eur
-                    elif sale_detail["owner"] == 2:
-                        other_taxable_gain_2 += exercise_gain_eur
-                    else:
-                        raise Exception(
-                            f"Owner must be 1 or 2, not {sale_detail['owner']} (type={type(sale_detail['owner'])}")
+
+                # Note: strike price is stored in unit_acquisition_price
+                exercise_gain_eur = sale.nb_stocks_sold * (sale.sell_price_eur - sale.unit_acquisition_price)
+                if sale.owner == 1:
+                    other_taxable_gain_1 += exercise_gain_eur
+                elif sale.owner == 2:
+                    other_taxable_gain_2 += exercise_gain_eur
+                else:
+                    raise Exception(
+                        f"Owner must be 1 or 2, not {sale.owner} (type={type(sale.owner)}")
             elif sale.stock_type == "rsu":
                 # acquisition gain only applies to RSU
                 sell_date = sale.sell_date
                 sell_date_minus_2y = sell_date + relativedelta(years=-2)
                 sell_date_minus_8y = sell_date + relativedelta(years=-8)
-                for sale_detail in sale.sell_details:
-                    rsu_plan = self.rsu_plans[sale_detail["plan_name"]]
-                    taxation_scheme = rsu_plan.taxation_scheme
-                    plan_currency = rsu_plan.currency
-                    acq_date = sale_detail["acq_date"]
-                    usd_eur = cc.convert(1, plan_currency, "EUR",
-                                         date=acq_date)
-                    gain_eur = sale_detail["count"] * sale_detail["acq_price"] * usd_eur
-                    # gain tax
-                    if taxation_scheme == "2015" or taxation_scheme == "2017":
-                        # 50% rebates btw 2 and 8y retention, 65% above 8y
-                        if acq_date <= sell_date_minus_8y:
-                            taxable_gain += gain_eur * 0.35
-                            rebates += gain_eur * 0.65
-                        elif acq_date <= sell_date_minus_2y:
-                            taxable_gain += gain_eur * 0.5
-                            rebates += gain_eur * 0.5
-                        else:
-                            taxable_gain += gain_eur  # too recent to have a rebate
-                    elif taxation_scheme == "2018":
-                        # 50% rebate
+                rsu_plan = self.rsu_plans[sale.plan_name]
+                taxation_scheme = rsu_plan.taxation_scheme
+                acq_date = sale.acq_date
+                gain_eur = sale.nb_stocks_sold * sale.unit_acquisition_price
+                # gain tax
+                if taxation_scheme == "2015" or taxation_scheme == "2017":
+                    # 50% rebates btw 2 and 8y retention, 65% above 8y
+                    if acq_date <= sell_date_minus_8y:
+                        taxable_gain += gain_eur * 0.35
+                        rebates += gain_eur * 0.65
+                    elif acq_date <= sell_date_minus_2y:
                         taxable_gain += gain_eur * 0.5
-                        rebates_50p += gain_eur * 0.5
+                        rebates += gain_eur * 0.5
                     else:
-                        raise Exception(f"Unsupported tax scheme: {taxation_scheme}")
+                        taxable_gain += gain_eur  # too recent to have a rebate
+                elif taxation_scheme == "2018":
+                    # 50% rebate
+                    taxable_gain += gain_eur * 0.5
+                    rebates_50p += gain_eur * 0.5
+                else:
+                    raise Exception(f"Unsupported tax scheme: {taxation_scheme}")
 
         return {
             "taxable_acquisition_gain_1TZ": round(taxable_gain),
             "acquisition_gain_rebates_1UZ": round(rebates),
             "acquisition_gain_50p_rebates_1WZ": round(rebates_50p),
             "exercise_gain_1_1TT": round(other_taxable_gain_1),
             "exercise_gain_2_1UT": round(other_taxable_gain_2)
```

### Comparing `easyfrenchtax-0.0.4/src/easyfrenchtax/tax_simulator.py` & `easyfrenchtax-0.0.5/src/easyfrenchtax/tax_simulator.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/PKG-INFO` & `easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfrenchtax-0.0.4/tests/test_capital_tax.py` & `easyfrenchtax-0.0.5/tests/test_capital_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.4/tests/test_fiscal_advantages.py` & `easyfrenchtax-0.0.5/tests/test_fiscal_advantages.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.4/tests/test_income_tax.py` & `easyfrenchtax-0.0.5/tests/test_income_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.4/tests/test_rental_tax.py` & `easyfrenchtax-0.0.5/tests/test_rental_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.4/tests/test_stock_helper.py` & `easyfrenchtax-0.0.5/tests/test_stock_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 8, 28), 19)
     stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 9, 28), 14)
     stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 10, 29), 15)
     stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 11, 28), 14)
     stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 12, 28), 19)
     stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2019, 1, 28), 23)
     stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2019, 2, 28), 24)
+    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 100, date(2020, 2, 28), 24)
     stock_helper.rsu_plan("Pineapple", date(2016, 6, 29), "PZZA", "USD")
     stock_helper.rsu_vesting(1, "PZZA", "Pineapple", 313, date(2020, 12, 28), 20.84)
     stock_helper.rsu_vesting(1, "PZZA", "Pineapple", 312, date(2021, 3, 28), 27.44)
     stock_helper.rsu_vesting(1, "PZZA", "Pineapple", 313, date(2021, 6, 28), 37.25)
     stock_helper.rsu_plan("Pepperoni", date(2017, 7, 28), "PZZA", "USD")
     stock_helper.rsu_vesting(1, "PZZA", "Pepperoni", 398, date(2020, 12, 16), 18.75)
     stock_helper.rsu_vesting(1, "PZZA", "Pepperoni", 133, date(2021, 1, 26), 19.13)
@@ -38,38 +39,62 @@
     return cc.convert
 
 
 def test_summary(stock_helper_with_plan):
     summary = stock_helper_with_plan.summary()
     assert set(summary.keys()) == {"CAKE", "BUD", "PZZA"}
     assert set(summary["CAKE"].keys()) == {"RSU"}
-    assert summary["CAKE"]["RSU"] == 320
+    assert summary["CAKE"]["RSU"] == 420
     assert set(summary["BUD"].keys()) == {"ESPP"}
     assert summary["BUD"]["ESPP"] == 500
     assert set(summary["PZZA"].keys()) == {"StockOption", "RSU"}
     assert summary["PZZA"]["StockOption"] == 150
 
 
 def test_rsu_sale(stock_helper_with_plan):
-    assert sum([r.available for r in stock_helper_with_plan.rsus["CAKE"]]) == 320
     final_count_1 = stock_helper_with_plan.sell_rsus("CAKE", 200, date(2019, 6, 3), sell_price=22, fees=0,
                                                      currency="USD")
     assert final_count_1 == 200
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 40
-    assert all([r.available == 10 for r in stock_helper_with_plan.rsus["CAKE"][1:]])
+    assert all([r.available == 10 or r.acq_date > date(2019, 6, 3) for r in stock_helper_with_plan.rsus["CAKE"][1:]])
     final_count_2 = stock_helper_with_plan.sell_rsus("CAKE", 200, date(2019, 6, 3), sell_price=22, fees=0,
                                                      currency="USD")
     assert final_count_2 == 120, "Cannot sell more than we have"
 
+def test_rsu_sell_available(stock_helper_with_plan):
+    # check that we only consider RSUs available at the sale date, not afterwards
+    # on 1-4-2021, only 313+312+398+133 are available
+    available_before = 313+312+398+133
+    available_after = 313
+
+    amount_sold = stock_helper_with_plan.sell_rsus("PZZA", available_before + available_after, date(2021, 4, 1), sell_price=22, fees=0)
+    assert amount_sold == available_before
+    amount_sold_2 = stock_helper_with_plan.sell_rsus("PZZA", available_after, date(2021, 12, 1), sell_price=22, fees=0)
+    assert amount_sold_2 == available_after
+
+def test_rsu_fifo(stock_helper_with_plan):
+    stock_helper_with_plan.sell_rsus("PZZA", 800, date(2022,1,1), sell_price=22, fees=0)
+    vestings = sorted(stock_helper_with_plan.rsus["PZZA"],key=lambda sg: sg.acq_date)
+    assert vestings[0].available == 0
+    assert vestings[0].count == 398
+    assert vestings[1].available == 0
+    assert vestings[1].count == 313
+    assert vestings[2].available == 44
+    assert vestings[2].count == 133
+    assert vestings[3].available == 312
+    assert vestings[3].count == 312
+    assert vestings[4].available == 313
+    assert vestings[4].count == 313
+
 
 def test_rsu_acquisition_gain_tax(stock_helper_with_plan):
     stock_helper_with_plan.sell_rsus("CAKE", 200, date(2019, 1, 16),
                                      sell_price=22, fees=0, currency="USD")
     taxes = stock_helper_with_plan.compute_acquisition_gain_tax(2019)
-    assert taxes["taxable_acquisition_gain_1TZ"] == 3431
+    assert taxes["taxable_acquisition_gain_1TZ"] == 3432
     assert taxes["acquisition_gain_50p_rebates_1WZ"] == 0
     assert taxes["acquisition_gain_rebates_1UZ"] == 0
     assert taxes["exercise_gain_1_1TT"] == 0
     assert taxes["exercise_gain_2_1UT"] == 0
 
 
 def test_rsu_acquisition_gain_tax_rebates(stock_helper_with_plan):
@@ -142,15 +167,15 @@
     )
     assert report_2042C["capital_gain_3VG"] == expected_capital_gain, \
         "Capital gain tax should be compliant"
 
 
 def test_stockoptions_sale(stock_helper_with_plan, convert_fn):
     sell_price = 40
-    final_count, _, sell = stock_helper_with_plan.sell_stockoptions("PZZA", 50, date(2021, 8, 2), sell_price=sell_price,
+    final_count = stock_helper_with_plan.sell_stockoptions("PZZA", 50, date(2021, 8, 2), sell_price=sell_price,
                                                                     fees=0, currency="USD")
     agt = stock_helper_with_plan.compute_acquisition_gain_tax(2021)
     cgt = stock_helper_with_plan.compute_capital_gain_tax(2021)
 
     strike_price = stock_helper_with_plan.stock_options["PZZA"][0].acq_price
     assert final_count == 50
     ex_gain_usd = 50 * (sell_price - strike_price)
```

