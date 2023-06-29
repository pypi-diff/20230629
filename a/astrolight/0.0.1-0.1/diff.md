# Comparing `tmp/astrolight-0.0.1-py3-none-any.whl.zip` & `tmp/astrolight-0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,18 @@
-Zip file size: 2104 bytes, number of entries: 8
+Zip file size: 7447 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 astrolight/__init__.py
--rw-r--r--  2.0 unx      276 b- defN 80-Jan-01 00:00 astrolight/__main__.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 astrolight/py.typed
--rw-r--r--  2.0 unx     1383 b- defN 80-Jan-01 00:00 astrolight-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 astrolight-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 80-Jan-01 00:00 astrolight-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 80-Jan-01 00:00 astrolight-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      635 b- defN 80-Jan-01 00:00 astrolight-0.0.1.dist-info/RECORD
-8 files, 2453 bytes uncompressed, 982 bytes compressed:  60.0%
+-rw-r--r--  2.0 unx     1191 b- defN 80-Jan-01 00:00 astrolight/__main__.py
+-rw-r--r--  2.0 unx      381 b- defN 80-Jan-01 00:00 astrolight/account_connector.py
+-rw-r--r--  2.0 unx     2549 b- defN 80-Jan-01 00:00 astrolight/app.py
+-rw-r--r--  2.0 unx      301 b- defN 80-Jan-01 00:00 astrolight/config.py
+-rw-r--r--  2.0 unx      934 b- defN 80-Jan-01 00:00 astrolight/ewelink_connector.py
+-rw-r--r--  2.0 unx      904 b- defN 80-Jan-01 00:00 astrolight/timer.py
+-rw-r--r--  2.0 unx      336 b- defN 80-Jan-01 00:00 astrolight/times/__init__.py
+-rw-r--r--  2.0 unx     1024 b- defN 80-Jan-01 00:00 astrolight/times/dynamic_time.py
+-rw-r--r--  2.0 unx     2447 b- defN 80-Jan-01 00:00 astrolight/times/expression.py
+-rw-r--r--  2.0 unx      811 b- defN 80-Jan-01 00:00 astrolight/times/sun_time.py
+-rw-r--r--  2.0 unx     1459 b- defN 80-Jan-01 00:00 astrolight-0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 astrolight-0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 80-Jan-01 00:00 astrolight-0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 80-Jan-01 00:00 astrolight-0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1296 b- defN 80-Jan-01 00:00 astrolight-0.1.dist-info/RECORD
+16 files, 13792 bytes uncompressed, 5303 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -1,25 +1,49 @@
 Filename: astrolight/__init__.py
 Comment: 
 
 Filename: astrolight/__main__.py
 Comment: 
 
-Filename: astrolight/py.typed
+Filename: astrolight/account_connector.py
 Comment: 
 
-Filename: astrolight-0.0.1.dist-info/METADATA
+Filename: astrolight/app.py
 Comment: 
 
-Filename: astrolight-0.0.1.dist-info/WHEEL
+Filename: astrolight/config.py
 Comment: 
 
-Filename: astrolight-0.0.1.dist-info/entry_points.txt
+Filename: astrolight/ewelink_connector.py
 Comment: 
 
-Filename: astrolight-0.0.1.dist-info/top_level.txt
+Filename: astrolight/timer.py
 Comment: 
 
-Filename: astrolight-0.0.1.dist-info/RECORD
+Filename: astrolight/times/__init__.py
+Comment: 
+
+Filename: astrolight/times/dynamic_time.py
+Comment: 
+
+Filename: astrolight/times/expression.py
+Comment: 
+
+Filename: astrolight/times/sun_time.py
+Comment: 
+
+Filename: astrolight-0.1.dist-info/METADATA
+Comment: 
+
+Filename: astrolight-0.1.dist-info/WHEEL
+Comment: 
+
+Filename: astrolight-0.1.dist-info/entry_points.txt
+Comment: 
+
+Filename: astrolight-0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: astrolight-0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## astrolight/__main__.py

```diff
@@ -1,18 +1,48 @@
 import asyncio
 import logging
+import yaml
+from argparse import ArgumentParser, Namespace
+from datetime import datetime
+from pathlib import Path
+
+from .app import App
+from .config import Config
 
 
 def configure_logging() -> None:
     logging.basicConfig(level="INFO")
 
 
+def parse_args() -> Namespace:
+    parser = ArgumentParser()
+    parser.add_argument("--config", type=Path, default=Path("config.yml"))
+    parser.add_argument("--interval", type=float, default=300)
+    parser.add_argument("--time-multiplier", type=float, default=1)
+    return parser.parse_args()
+
+
 async def amain() -> None:
     configure_logging()
-    logging.info("Hello World!")
+    args = parse_args()
+
+    config_file: Path = args.config
+    with config_file.open() as f:
+        config = Config.parse_obj(yaml.load(f, Loader=yaml.BaseLoader))
+
+    time_multiplier: float = args.time_multiplier
+    start_time = datetime.now()
+
+    def get_time_func() -> datetime:
+        return start_time + time_multiplier * (datetime.now() - start_time)
+
+    interval: float = args.interval / time_multiplier
+
+    app = App(config, get_time_func)
+    await app.run(interval)
 
 
 def main() -> None:
     asyncio.run(amain())
 
 
 if __name__ == "__main__":
```

## Comparing `astrolight-0.0.1.dist-info/METADATA` & `astrolight-0.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: astrolight
-Version: 0.0.1
+Version: 0.1
 Requires-Python: >=3.9
 Requires-Dist: PyYAML
+Requires-Dist: pydantic
+Requires-Dist: suntime
+Requires-Dist: ewelink (~=0.2)
 Provides-Extra: black
 Requires-Dist: black (==22.8.0) ; extra == 'black'
 Provides-Extra: dev
 Requires-Dist: tox ; extra == 'dev'
 Requires-Dist: pytest (>=7) ; extra == 'dev'
 Requires-Dist: pytest-asyncio ; extra == 'dev'
 Requires-Dist: pytest-cov ; extra == 'dev'
```

