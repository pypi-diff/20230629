# Comparing `tmp/tea-web-0.5.9.tar.gz` & `tmp/tea-web-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tea-web-0.5.9.tar", last modified: Sun Mar 12 12:52:10 2023, max compression
+gzip compressed data, was "tea-web-0.6.0.tar", last modified: Thu Jun 29 20:41:48 2023, max compression
```

## Comparing `tea-web-0.5.9.tar` & `tea-web-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 12:52:10.409131 tea-web-0.5.9/
--rw-rw-rw-   0        0        0     2343 2023-03-12 12:52:10.408131 tea-web-0.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     1706 2023-03-05 18:58:14.000000 tea-web-0.5.9/README.md
--rw-rw-rw-   0        0        0       42 2023-03-12 12:52:10.409131 tea-web-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0      594 2023-03-12 12:52:09.000000 tea-web-0.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-12 12:52:10.360131 tea-web-0.5.9/src/
-drwxrwxrwx   0        0        0        0 2023-03-12 12:52:10.387131 tea-web-0.5.9/src/tea/
--rw-rw-rw-   0        0        0      299 2023-03-12 12:52:09.000000 tea-web-0.5.9/src/tea/__init__.py
--rw-rw-rw-   0        0        0    13195 2023-03-12 12:52:00.000000 tea-web-0.5.9/src/tea/main.py
--rw-rw-rw-   0        0        0     2580 2023-03-08 19:00:08.000000 tea-web-0.5.9/src/tea/request.py
--rw-rw-rw-   0        0        0     9619 2023-02-26 19:40:09.000000 tea-web-0.5.9/src/tea/response.py
--rw-rw-rw-   0        0        0      712 2023-03-05 18:42:29.000000 tea-web-0.5.9/src/tea/url.py
--rw-rw-rw-   0        0        0     2850 2023-03-09 20:54:38.000000 tea-web-0.5.9/src/tea/websocket_client.py
--rw-rw-rw-   0        0        0      925 2023-03-06 17:28:12.000000 tea-web-0.5.9/src/tea/websocket_server.py
-drwxrwxrwx   0        0        0        0 2023-03-12 12:52:10.405134 tea-web-0.5.9/src/tea_web.egg-info/
--rw-rw-rw-   0        0        0     2343 2023-03-12 12:52:10.000000 tea-web-0.5.9/src/tea_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-03-12 12:52:10.000000 tea-web-0.5.9/src/tea_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 12:52:10.000000 tea-web-0.5.9/src/tea_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-03-12 12:52:10.000000 tea-web-0.5.9/src/tea_web.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 20:41:48.180608 tea-web-0.6.0/
+-rw-rw-rw-   0        0        0     2254 2023-06-29 20:41:48.179600 tea-web-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-06-28 20:28:36.000000 tea-web-0.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 20:41:48.181606 tea-web-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      594 2023-06-29 20:41:47.000000 tea-web-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:41:48.118985 tea-web-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 20:41:48.141526 tea-web-0.6.0/src/tea/
+-rw-rw-rw-   0        0        0      138 2023-06-29 20:41:47.000000 tea-web-0.6.0/src/tea/__init__.py
+-rw-rw-rw-   0        0        0     2850 2023-03-09 20:54:38.000000 tea-web-0.6.0/src/tea/ignore-websocket_client.py
+-rw-rw-rw-   0        0        0      925 2023-03-06 17:28:12.000000 tea-web-0.6.0/src/tea/ignore-websocket_server.py
+-rw-rw-rw-   0        0        0    11761 2023-06-29 20:31:47.000000 tea-web-0.6.0/src/tea/main.py
+-rw-rw-rw-   0        0        0     3597 2023-06-29 20:38:32.000000 tea-web-0.6.0/src/tea/request.py
+-rw-rw-rw-   0        0        0    10570 2023-06-29 17:43:53.000000 tea-web-0.6.0/src/tea/response.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:41:48.176608 tea-web-0.6.0/src/tea_web.egg-info/
+-rw-rw-rw-   0        0        0     2254 2023-06-29 20:41:47.000000 tea-web-0.6.0/src/tea_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-29 20:41:47.000000 tea-web-0.6.0/src/tea_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 20:41:47.000000 tea-web-0.6.0/src/tea_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-29 20:41:47.000000 tea-web-0.6.0/src/tea_web.egg-info/top_level.txt
```

### Comparing `tea-web-0.5.9/PKG-INFO` & `tea-web-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 Metadata-Version: 2.1
 Name: tea-web
-Version: 0.5.9
+Version: 0.6.0
 Summary: Micro HTTP library with WebSocket support for Python.
 Home-page: UNKNOWN
 Author: orhanemree (Orhan Emre Dikicigil)
 Author-email: orhanemre.dev@gmail.com
 License: MIT
 Description: # 🍵 Tea
-        Micro HTTP library with WebSocket support for Python.
+        Micro HTTP library for Python.
         
-        Tea has [Express.js](https://github.com/expressjs/express)-like syntax (which is web framework for JavaScript) with it's callback function syntax, Request, Response and URL objects. Got a lot of reference from popular web frameweorks like [Flask](https://github.com/pallets/flask), [FastAPI](https://github.com/tiangolo/fastapi) and Express.js. Tea is like lightweight mix of their best features. Of course pretty good with WebSocket support.
+        Tea has [Express.js](https://github.com/expressjs/express)-like syntax (which is web framework for JavaScript) with it's callback function syntax, Request, Response and URL objects. Got a lot of reference from popular web frameweorks like [Flask](https://github.com/pallets/flask), [FastAPI](https://github.com/tiangolo/fastapi) and Express.js. Tea is like lightweight mix of their best features.
         
         Finally, the `418 I am a teapot` code comes true. Enjoy!
         
         ## Quick Start
         ```console
         $ pip install tea-web
         ```
         
         ## `Hello, World!`
         Simple `Hello, World!` example in Tea. See [`/examples`](https://github.com/orhanemree/tea/tree/master/examples) for more example.
         
         ```python
         # app.py
         from tea import Tea
+        
         app = Tea()
+        
         def handle_index(req, res):
             res.send("Hello, World!")
+        
         app.get("/", handle_index)
-        app.listen(port=8080)
+        
+        app.listen() # listening port 8080
         ```
         
-        ## Advantages of Tea
+        ## Pros
         * Lightweight. No external requirement and the package cost is only ~10 KB.
-        * More control over the Request, Response and URL objects. This objects can be used outside the library structure.
+        * More control over the Request and Response objects. This objects can be used outside the library structure.
         * Easy to use and helpful on handling simple HTTP requests.
-        * Built-in WebSocket support.
         
-        ## Disadvantages of Tea
+        ## Cons
         * Limited features and methods.
         * No template engine.
         * Callback function syntax is not really Pythonic without decorators. (Done on purpose but true.)
         * Not sure if it's ready for production.
         
         ## Documentation
         * See [DOCUMENTATION.md](https://github.com/orhanemree/tea/blob/master/DOCUMENTATION.md).
```

### Comparing `tea-web-0.5.9/README.md` & `tea-web-0.6.0/src/tea_web.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,55 @@
-# 🍵 Tea
-Micro HTTP library with WebSocket support for Python.
-
-Tea has [Express.js](https://github.com/expressjs/express)-like syntax (which is web framework for JavaScript) with it's callback function syntax, Request, Response and URL objects. Got a lot of reference from popular web frameweorks like [Flask](https://github.com/pallets/flask), [FastAPI](https://github.com/tiangolo/fastapi) and Express.js. Tea is like lightweight mix of their best features. Of course pretty good with WebSocket support.
-
-Finally, the `418 I am a teapot` code comes true. Enjoy!
-
-## Quick Start
-```console
-$ pip install tea-web
-```
-
-## `Hello, World!`
-Simple `Hello, World!` example in Tea. See [`/examples`](https://github.com/orhanemree/tea/tree/master/examples) for more example.
-
-```python
-# app.py
-from tea import Tea
-app = Tea()
-def handle_index(req, res):
-    res.send("Hello, World!")
-app.get("/", handle_index)
-app.listen(port=8080)
-```
-
-## Advantages of Tea
-* Lightweight. No external requirement and the package cost is only ~10 KB.
-* More control over the Request, Response and URL objects. This objects can be used outside the library structure.
-* Easy to use and helpful on handling simple HTTP requests.
-* Built-in WebSocket support.
-
-## Disadvantages of Tea
-* Limited features and methods.
-* No template engine.
-* Callback function syntax is not really Pythonic without decorators. (Done on purpose but true.)
-* Not sure if it's ready for production.
-
-## Documentation
-* See [DOCUMENTATION.md](https://github.com/orhanemree/tea/blob/master/DOCUMENTATION.md).
-
-## License
-* Licensed under the [MIT License](https://github.com/orhanemree/tea/blob/master/LICENSE).
+Metadata-Version: 2.1
+Name: tea-web
+Version: 0.6.0
+Summary: Micro HTTP library with WebSocket support for Python.
+Home-page: UNKNOWN
+Author: orhanemree (Orhan Emre Dikicigil)
+Author-email: orhanemre.dev@gmail.com
+License: MIT
+Description: # 🍵 Tea
+        Micro HTTP library for Python.
+        
+        Tea has [Express.js](https://github.com/expressjs/express)-like syntax (which is web framework for JavaScript) with it's callback function syntax, Request, Response and URL objects. Got a lot of reference from popular web frameweorks like [Flask](https://github.com/pallets/flask), [FastAPI](https://github.com/tiangolo/fastapi) and Express.js. Tea is like lightweight mix of their best features.
+        
+        Finally, the `418 I am a teapot` code comes true. Enjoy!
+        
+        ## Quick Start
+        ```console
+        $ pip install tea-web
+        ```
+        
+        ## `Hello, World!`
+        Simple `Hello, World!` example in Tea. See [`/examples`](https://github.com/orhanemree/tea/tree/master/examples) for more example.
+        
+        ```python
+        # app.py
+        from tea import Tea
+        
+        app = Tea()
+        
+        def handle_index(req, res):
+            res.send("Hello, World!")
+        
+        app.get("/", handle_index)
+        
+        app.listen() # listening port 8080
+        ```
+        
+        ## Pros
+        * Lightweight. No external requirement and the package cost is only ~10 KB.
+        * More control over the Request and Response objects. This objects can be used outside the library structure.
+        * Easy to use and helpful on handling simple HTTP requests.
+        
+        ## Cons
+        * Limited features and methods.
+        * No template engine.
+        * Callback function syntax is not really Pythonic without decorators. (Done on purpose but true.)
+        * Not sure if it's ready for production.
+        
+        ## Documentation
+        * See [DOCUMENTATION.md](https://github.com/orhanemree/tea/blob/master/DOCUMENTATION.md).
+        
+        ## License
+        * Licensed under the [MIT License](https://github.com/orhanemree/tea/blob/master/LICENSE).
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `tea-web-0.5.9/setup.py` & `tea-web-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 def readme():
     with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
         return f.read()
 
 setup(
     name="tea-web",
-    version="0.5.9",
+    version="0.6.0",
     description="Micro HTTP library with WebSocket support for Python.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     author="orhanemree (Orhan Emre Dikicigil)",
     author_email="orhanemre.dev@gmail.com",
     license="MIT",
     packages=["tea"],
```

### Comparing `tea-web-0.5.9/src/tea/response.py` & `tea-web-0.6.0/src/tea/response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Union
-from datetime import datetime
-from pathlib import Path
+from time import strftime
+from os import path
+
 
 status_list = {
     "202": "ACCEPTED",
     "208": "ALREADY REPORTED",
     "502": "BAD GATEWAY",
     "400": "BAD REQUEST",
     "409": "CONFLICT",
@@ -196,85 +196,144 @@
     "mov": "video/quicktime",
     "qt": "video/quicktime",
     "webm": "video/webm",
     "avi": "video/x-msvideo",
     "movie": "video/x-sgi-movie"
 }
 
+
 class Response:
     
-    def __init__(self, body: str="",
-                headers: Union[dict[str, str], None]=None,
-                status_code: int=200,
-                content_type: str="text/plain"):
+    
+    def __init__(self, body: str="", headers={}, status_code: int=200, content_type: str="text/plain"):
+        
         self.status_code    = status_code
-        self.status_message = status_list[str(self.status_code)]
-        self.content_type   = content_type if "/" in content_type else mimetype_list.get(content_type, "text/plain")
-        self.headers        = {}
-        self.set_headers({ "Content-Type": f"{self.content_type}; charset=utf-8", "Server": "Python/Tea" })
-        if headers:
-            self.set_headers(headers)
+        self.status_message = status_list[str(self.status_code)].title()
+        self.content_type   = content_type if "/" in content_type else mimetype_list.get(content_type, content_type)
+        
+        # set body
         self.body = body
         
+        # set headers
+        self.headers = headers
+        self._set_default_headers()
+        
     
-    def __get_headers_as_string(self) -> str:
-        return "\r\n".join([f"{key.replace('-', ' ').title().replace(' ', '-')}: {self.headers[key]}" for key in list(self.headers.keys())])
+    def _get_headers_as_string(self) -> str:
+        
+        """
+        Get response headers as raw string.
+        """
+        
+        return "\r\n".join([f"{key}: {self.headers[key]}" for key in self.headers.keys()])
         
     
+    def _set_default_headers(self):
+        
+        if not self.has_header("Content-Type"):
+            self.set_header("Content-Type", f"{self.content_type}; charset=utf-8")
+        
+        if not self.has_header("Server"):
+            self.set_header("Server", "Python/Tea")
+            
+        self.set_header("Content-Length", len(self.body))
+        
+        self.set_header("Date", strftime("%Y-%m-%d %H:%M:%S"))
+    
+    
     def get_res_as_text(self) -> str:
+        
+        """
+        Get response text as raw string.
+        """
+        
+        self._set_default_headers()
+
+        status_line = f"HTTP/1.1 {self.status_code} {self.status_message}"
+
+        return f"{status_line}\r\n{self._get_headers_as_string()}\r\n\r\n{self.body}"
+
+
+    def has_header(self, key: str) -> bool:
+        
+        """
+        Check if header exists. (Not case sensitive)
+        """
+        
+        return (key.replace("-", " ").title().replace(" ", "-") in self.headers)
+    
+
+    def get_header(self, key: str):
+        
         """
-        Get raw response text as string.
+        Get value of specific header. Return None if not exists. (Not case sensitive)
         """
-        self.set_headers({ "Content-Length": len(self.body), "Date": datetime.now() })
-        return f"HTTP/1.1 {self.status_code} {status_list[str(self.status_code)]}\r\n{self.__get_headers_as_string()}\r\n\r\n{self.body}"
+        
+        return self.headers.get(key.replace("-", " ").title().replace(" ", "-"))
     
     
-    def set_header(self, key: str, value: str) -> None:
+    def set_header(self, key: str, value: str):
+        
         """
         Add new header to response.
         """
+        
         self.headers[key.replace("-", " ").title().replace(" ", "-")] = value
                 
     
-    def set_headers(self, headers: dict[str, str]) -> None:
+    def set_headers(self, headers: dict[str, str]):
+        
         """
         Add multiple headers as dict to response.
         """
+        
         for key in headers:
             self.headers[key.replace("-", " ").title().replace(" ", "-")] = headers[key]
                 
     
-    def send(self, body: str="",
-            headers: Union[dict[str, str], None]=None,
-            status_code: int=200,
-            content_type: str="text/plain") -> None:
+    def send(self, body: str="", headers=None, status_code: int=200, content_type: str="text/plain"):
+        
         """
         Send response inside the callback function.
         """
+        
         self.status_code    = status_code
-        self.status_message = status_list[str(self.status_code)]
-        self.content_type   = content_type if "/" in content_type else mimetype_list.get(content_type, "text/plain")
-        self.set_header("Content-Type", f"{self.content_type}; charset=utf-8")
-        if headers:
-            self.set_headers(headers)
+        self.status_message = status_list[str(self.status_code)].title()
+        self.content_type   = content_type if "/" in content_type else mimetype_list.get(content_type, content_type)
+        
+        # set body
         self.body = body
         
+        # set headers
+        if headers:
+            self.set_headers(headers)
+        self._set_default_headers()
+
     
-    def send_file(self, filename: str,
-                headers: dict[str, str]=None,
-                status_code: int=200) -> None:
+    def send_file(self, filename: str, headers=None, status_code: int=200, content_type: str="text/plain"):
+        
         """
         Send file as response inside the callback function with auto content type.
         """
+        
         self.status_code    = status_code
         self.status_message = status_list[str(self.status_code)]
-        self.content_type   = mimetype_list.get(filename.split(".")[-1], "text/plain")
-        self.set_header("Content-Type", f"{self.content_type}; charset=utf-8")
-        if headers:
-            self.set_headers(headers)
+        self.content_type   = mimetype_list.get(filename.split(".")[-1], content_type)
         
-        absolute_path = Path(filename).resolve()
+        absolute_path = path.abspath(filename)
+        
+        # read file and update body with file content
         try:
             with open(absolute_path, "r", encoding="utf-8") as f:
+                
+                # set body
                 self.body = f.read()
+                
         except Exception as e:
             raise
+        
+        # set headers
+        if headers:
+            self.set_headers(headers)
+        self._set_default_headers()
+        
+        print(self.headers)
```

### Comparing `tea-web-0.5.9/src/tea/websocket_client.py` & `tea-web-0.6.0/src/tea/ignore-websocket_client.py`

 * *Files identical despite different names*

### Comparing `tea-web-0.5.9/src/tea/websocket_server.py` & `tea-web-0.6.0/src/tea/ignore-websocket_server.py`

 * *Files identical despite different names*

