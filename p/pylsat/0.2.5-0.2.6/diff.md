# Comparing `tmp/pylsat-0.2.5.tar.gz` & `tmp/pylsat-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylsat-0.2.5.tar", last modified: Thu Jun 29 17:16:31 2023, max compression
+gzip compressed data, was "pylsat-0.2.6.tar", last modified: Thu Jun 29 19:53:16 2023, max compression
```

## Comparing `pylsat-0.2.5.tar` & `pylsat-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 17:16:31.812717 pylsat-0.2.5/
--rw-rw-rw-   0        0        0     1089 2023-06-29 13:36:39.000000 pylsat-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      325 2023-06-29 17:16:31.811712 pylsat-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2179 2023-06-29 14:22:58.000000 pylsat-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 17:16:31.779677 pylsat-0.2.5/pylsat/
--rw-rw-rw-   0        0        0       75 2023-06-29 17:08:01.000000 pylsat-0.2.5/pylsat/__init__.py
--rw-rw-rw-   0        0        0     5279 2023-06-29 14:08:53.000000 pylsat-0.2.5/pylsat/pylsat.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:16:31.796365 pylsat-0.2.5/pylsat.egg-info/
--rw-rw-rw-   0        0        0      325 2023-06-29 17:16:31.000000 pylsat-0.2.5/pylsat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-06-29 17:16:31.000000 pylsat-0.2.5/pylsat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 17:16:31.000000 pylsat-0.2.5/pylsat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-29 17:16:31.000000 pylsat-0.2.5/pylsat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-29 17:16:31.000000 pylsat-0.2.5/pylsat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 17:16:31.813722 pylsat-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      504 2023-06-29 17:06:31.000000 pylsat-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:16:31.797369 pylsat-0.2.5/vendor/
--rw-rw-rw-   0        0        0        0 2023-06-29 16:21:16.000000 pylsat-0.2.5/vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:16:31.809609 pylsat-0.2.5/vendor/bolt11/
--rw-rw-rw-   0        0        0      155 2023-06-29 17:03:55.000000 pylsat-0.2.5/vendor/bolt11/__init__.py
--rw-rw-rw-   0        0        0      253 2023-06-29 14:05:03.000000 pylsat-0.2.5/vendor/bolt11/compat.py
--rw-rw-rw-   0        0        0     6626 2023-06-29 14:04:41.000000 pylsat-0.2.5/vendor/bolt11/core.py
--rw-rw-rw-   0        0        0     2743 2023-06-29 17:10:16.000000 pylsat-0.2.5/vendor/bolt11/types.py
--rw-rw-rw-   0        0        0     2149 2023-06-29 14:05:55.000000 pylsat-0.2.5/vendor/bolt11/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-29 19:53:16.687876 pylsat-0.2.6/
+-rw-rw-rw-   0        0        0     1089 2023-06-29 13:36:39.000000 pylsat-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      325 2023-06-29 19:53:16.686541 pylsat-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2752 2023-06-29 19:43:50.000000 pylsat-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 19:53:16.655064 pylsat-0.2.6/pylsat/
+-rw-rw-rw-   0        0        0       99 2023-06-29 18:08:51.000000 pylsat-0.2.6/pylsat/__init__.py
+-rw-rw-rw-   0        0        0     7087 2023-06-29 19:45:34.000000 pylsat-0.2.6/pylsat/pylsat.py
+drwxrwxrwx   0        0        0        0 2023-06-29 19:53:16.668777 pylsat-0.2.6/pylsat.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-06-29 19:53:16.000000 pylsat-0.2.6/pylsat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-06-29 19:53:16.000000 pylsat-0.2.6/pylsat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 19:53:16.000000 pylsat-0.2.6/pylsat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-29 19:53:16.000000 pylsat-0.2.6/pylsat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-29 19:53:16.000000 pylsat-0.2.6/pylsat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 19:53:16.687876 pylsat-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      504 2023-06-29 19:38:34.000000 pylsat-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 19:53:16.670777 pylsat-0.2.6/vendor/
+-rw-rw-rw-   0        0        0        0 2023-06-29 16:21:16.000000 pylsat-0.2.6/vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 19:53:16.684366 pylsat-0.2.6/vendor/bolt11/
+-rw-rw-rw-   0        0        0      155 2023-06-29 17:03:55.000000 pylsat-0.2.6/vendor/bolt11/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-06-29 14:05:03.000000 pylsat-0.2.6/vendor/bolt11/compat.py
+-rw-rw-rw-   0        0        0     6626 2023-06-29 14:04:41.000000 pylsat-0.2.6/vendor/bolt11/core.py
+-rw-rw-rw-   0        0        0     2743 2023-06-29 17:10:16.000000 pylsat-0.2.6/vendor/bolt11/types.py
+-rw-rw-rw-   0        0        0     2149 2023-06-29 14:05:55.000000 pylsat-0.2.6/vendor/bolt11/utils.py
```

### Comparing `pylsat-0.2.5/LICENSE` & `pylsat-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pylsat-0.2.5/pylsat/pylsat.py` & `pylsat-0.2.6/pylsat/pylsat.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,84 @@
 import asyncio
 from fastapi import HTTPException
 from starlette.requests import Request
 from pymacaroons import Macaroon, Verifier
 import datetime
 import hashlib
 import uuid
+import inspect
 from vendor.bolt11.core import decode
+from typing import Optional, Callable, Dict, Protocol
+from pydantic import BaseModel
 
-class L402Validator:
+class Pricing:
     """
-    Middleware for validating L402 (Lightning Service Authentication Tokens) in a FastAPI application.
+    Pricing class for encapsulating price information.
     
     Attributes:
-        root_key: The root key for generating and verifying macaroons.
-        price_sats: The price (in satoshis) for accessing the API endpoint.
-        expiry_sec: The expiration time (in seconds) for the macaroon.
-        generate_invoice: A function for generating Lightning Network invoices.
-        verified_macaroons: A dictionary for caching verified macaroons to ensure they are used only once.
-        cleanup_interval: The interval (in seconds) at which expired macaroons are cleaned up from the cache.
+        price_sats: The price in satoshis. None if pricing is in fiat.
+        price_fiat: The price in fiat. None if pricing is in sats.
+        conversion_func: A function that converts fiat to satoshis.
     """
-    def __init__(self, root_key: str, price_sats: int, expiry_sec: int, generate_invoice_func):
+    def __init__(self, price_sats: Optional[int] = None, price_fiat: Optional[float] = None, 
+                 conversion_func: Optional[Callable[[float], int]] = None):
+
+        if price_sats is not None and price_fiat is not None:
+            raise ValueError("Must specify either price_sats or price_fiat, but not both.")
+        elif price_sats is None and price_fiat is None:
+            raise ValueError("Must specify either price_sats or price_fiat.")
+
+        if price_fiat is not None and conversion_func is None:
+            raise ValueError("Must provide a conversion function when pricing in fiat.")
+
+        self.price_sats = price_sats
+        self.price_fiat = price_fiat
+        self.conversion_func = conversion_func
+
+    async def get_price_sats(self) -> int:
+        if self.price_sats is not None:
+            return self.price_sats
+        else:
+            if inspect.iscoroutinefunction(self.conversion_func):
+                return await self.conversion_func(self.price_fiat)
+            else:
+                return self.conversion_func(self.price_fiat)
+
+
+
+class InvoiceDict(BaseModel):
+    bolt11: str
+
+    class Config:
+        extra = "allow"
+
+class InvoiceFunction(Protocol):
+    def __call__(self, price_sats: int, label: str, description: str) -> InvoiceDict: ...
+
+
+class L402Validator:
+    def __init__(self, root_key: str, expiry_sec: int, generate_invoice_func : InvoiceFunction, invoice_description: str, pricing: Pricing ):
         """
-        Initializes the L402Validator with the root key, price, expiry time, and invoice generation function.
-        Starts the cleanup task for expired macaroons.
+        Initializes the L402Validator.
+
+        Args:
+            root_key (str): The root key for generating and verifying macaroons.
+            expiry_sec (int): The expiration time (in seconds) for the macaroon.
+            generate_invoice_func (InvoiceFunction): A function for generating Lightning Network invoices.
+            invoice_description (str): A description to be included in the generated invoices.
+            pricing (Pricing): A Pricing object that encapsulates the pricing information. The object contains either the price in satoshis or the price in fiat, along with a conversion function for converting fiat to satoshis if the price is provided in fiat.
+
+        The function also starts a cleanup task for expired macaroons.
         """
         
         self.root_key = root_key
-        self.price_sats = price_sats
+        self.pricing = pricing
         self.expiry_sec = expiry_sec
         self.generate_invoice = generate_invoice_func
+        self.invoice_description = invoice_description
         self.verified_macaroons = {}  # Cache to store verified macaroons
         self.cleanup_interval = 60 * 10  # Cleanup interval in seconds (10 minutes)
         asyncio.create_task(self.cleanup_expired_macaroons())  # Start the cleanup task
 
     async def cleanup_expired_macaroons(self):
         """
         Periodically cleanup expired macaroons from the cache.
@@ -48,15 +94,15 @@
     
     async def __call__(self, request: Request):
         l402_key = request.headers.get('Authorization')
         if l402_key is None or not l402_key.startswith('LSAT '):
 
             try:
                 label = str(uuid.uuid4()) 
-                invoice = await self.generate_invoice(self.price_sats, f'LSAT_{label}', f'payment for endpoint')  # function to generate invoice
+                invoice = await self.generate_invoice(await self.pricing.get_price_sats(), f'LSAT_{label}', self.invoice_description )  # function to generate invoice
             except Exception as e:
                 raise HTTPException(status_code=500, detail=f"Couldn't generate invoice. Reason: {str(e)}")
 
             encoded_invoice = invoice['bolt11']    
             decoded_invoice = decode(encoded_invoice)
             payment_hash = decoded_invoice.tags['p']
             print(payment_hash)
@@ -100,7 +146,8 @@
 
         # If verification is successful, add macaroon to cache with its expiry time
         for caveat in macaroon.caveats:
             if caveat.caveat_id.split(' = ')[0] == 'expires':
                 self.verified_macaroons[macaroon.identifier] = caveat.caveat_id.split(' = ')[1]
 
         return request  # Add this line
+
```

### Comparing `pylsat-0.2.5/vendor/bolt11/core.py` & `pylsat-0.2.6/vendor/bolt11/core.py`

 * *Files identical despite different names*

### Comparing `pylsat-0.2.5/vendor/bolt11/types.py` & `pylsat-0.2.6/vendor/bolt11/types.py`

 * *Files identical despite different names*

### Comparing `pylsat-0.2.5/vendor/bolt11/utils.py` & `pylsat-0.2.6/vendor/bolt11/utils.py`

 * *Files identical despite different names*

