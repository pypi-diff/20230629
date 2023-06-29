# Comparing `tmp/strawberry_django_pubsub-0.0.6a0.tar.gz` & `tmp/strawberry_django_pubsub-0.0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_pubsub-0.0.6a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "strawberry_django_pubsub-0.0.7a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `strawberry_django_pubsub-0.0.6a0.tar` & `strawberry_django_pubsub-0.0.7a0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090251 strawberry_django_pubsub-0.0.6a0/.flake8
--rw-r--r--   0        0        0     3187 2023-05-22 12:10:46.979031 strawberry_django_pubsub-0.0.6a0/.gitignore
--rw-r--r--   0        0        0      264 2023-05-25 12:49:21.090454 strawberry_django_pubsub-0.0.6a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1058 2023-05-26 06:42:27.160926 strawberry_django_pubsub-0.0.6a0/LICENSE
--rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090542 strawberry_django_pubsub-0.0.6a0/Makefile
--rw-r--r--   0        0        0       29 2023-04-26 10:05:26.787023 strawberry_django_pubsub-0.0.6a0/README.md
--rw-r--r--   0        0        0     1690 2023-05-25 12:50:39.844857 strawberry_django_pubsub-0.0.6a0/pyproject.toml
--rw-r--r--   0        0        0     1959 2023-05-25 12:49:21.090815 strawberry_django_pubsub-0.0.6a0/requirements/compile.py
--rw-r--r--   0        0        0     3938 2023-05-25 12:49:21.090957 strawberry_django_pubsub-0.0.6a0/requirements/py310-django41.txt
--rw-r--r--   0        0        0     3936 2023-05-25 12:49:21.091083 strawberry_django_pubsub-0.0.6a0/requirements/py310-django42.txt
--rw-r--r--   0        0        0     3529 2023-05-25 12:49:21.091198 strawberry_django_pubsub-0.0.6a0/requirements/py311-django41.txt
--rw-r--r--   0        0        0     3527 2023-05-25 12:49:21.091307 strawberry_django_pubsub-0.0.6a0/requirements/py311-django42.txt
--rw-r--r--   0        0        0     3937 2023-05-25 12:49:21.091429 strawberry_django_pubsub-0.0.6a0/requirements/py39-django41.txt
--rw-r--r--   0        0        0     3935 2023-05-25 12:49:21.091548 strawberry_django_pubsub-0.0.6a0/requirements/py39-django42.txt
--rw-r--r--   0        0        0       68 2023-05-25 12:49:21.091644 strawberry_django_pubsub-0.0.6a0/requirements/requirements.in
--rw-r--r--   0        0        0       61 2023-06-28 21:08:42.883890 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/__init__.py
--rw-r--r--   0        0        0     6498 2023-06-28 20:06:16.062690 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/asgi.py
--rw-r--r--   0        0        0      521 2023-06-28 20:06:16.062832 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/context.py
--rw-r--r--   0        0        0     1435 2023-05-25 12:49:21.092317 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/debug.py
--rw-r--r--   0        0        0     6616 2023-05-30 19:26:00.787412 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/django/auth.py
--rw-r--r--   0        0        0      562 2023-05-30 19:26:00.787702 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/django/db.py
--rw-r--r--   0        0        0      756 2023-05-30 19:26:00.788092 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/django/middleware.py
--rw-r--r--   0        0        0     4524 2023-05-30 19:26:00.788355 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/django/router.py
--rw-r--r--   0        0        0    10093 2023-05-30 19:26:00.788614 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/django/sessions.py
--rw-r--r--   0        0        0      484 2023-05-25 12:49:21.092418 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/event.py
--rw-r--r--   0        0        0      841 2023-05-30 10:26:07.846938 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/exceptions.py
--rw-r--r--   0        0        0     1990 2023-06-28 20:34:06.719562 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py
--rw-r--r--   0        0        0     4157 2023-06-28 20:09:56.704728 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/queue.py
--rw-r--r--   0        0        0      264 2023-05-25 12:49:21.092910 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/types.py
--rw-r--r--   0        0        0      507 2023-05-25 12:49:21.093182 strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/utils.py
--rw-r--r--   0        0        0      324 2023-05-25 12:49:21.093287 strawberry_django_pubsub-0.0.6a0/tox.ini
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 strawberry_django_pubsub-0.0.6a0/PKG-INFO
+-rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090251 strawberry_django_pubsub-0.0.7a0/.flake8
+-rw-r--r--   0        0        0     3187 2023-05-22 12:10:46.979031 strawberry_django_pubsub-0.0.7a0/.gitignore
+-rw-r--r--   0        0        0      264 2023-05-25 12:49:21.090454 strawberry_django_pubsub-0.0.7a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1058 2023-05-26 06:42:27.160926 strawberry_django_pubsub-0.0.7a0/LICENSE
+-rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090542 strawberry_django_pubsub-0.0.7a0/Makefile
+-rw-r--r--   0        0        0       29 2023-04-26 10:05:26.787023 strawberry_django_pubsub-0.0.7a0/README.md
+-rw-r--r--   0        0        0     1690 2023-05-25 12:50:39.844857 strawberry_django_pubsub-0.0.7a0/pyproject.toml
+-rw-r--r--   0        0        0     1959 2023-05-25 12:49:21.090815 strawberry_django_pubsub-0.0.7a0/requirements/compile.py
+-rw-r--r--   0        0        0     3938 2023-05-25 12:49:21.090957 strawberry_django_pubsub-0.0.7a0/requirements/py310-django41.txt
+-rw-r--r--   0        0        0     3936 2023-05-25 12:49:21.091083 strawberry_django_pubsub-0.0.7a0/requirements/py310-django42.txt
+-rw-r--r--   0        0        0     3529 2023-05-25 12:49:21.091198 strawberry_django_pubsub-0.0.7a0/requirements/py311-django41.txt
+-rw-r--r--   0        0        0     3527 2023-05-25 12:49:21.091307 strawberry_django_pubsub-0.0.7a0/requirements/py311-django42.txt
+-rw-r--r--   0        0        0     3937 2023-05-25 12:49:21.091429 strawberry_django_pubsub-0.0.7a0/requirements/py39-django41.txt
+-rw-r--r--   0        0        0     3935 2023-05-25 12:49:21.091548 strawberry_django_pubsub-0.0.7a0/requirements/py39-django42.txt
+-rw-r--r--   0        0        0       68 2023-05-25 12:49:21.091644 strawberry_django_pubsub-0.0.7a0/requirements/requirements.in
+-rw-r--r--   0        0        0       61 2023-06-29 11:59:58.254909 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/__init__.py
+-rw-r--r--   0        0        0     6550 2023-06-29 09:18:36.409856 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/asgi.py
+-rw-r--r--   0        0        0      521 2023-06-28 20:06:16.062832 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/context.py
+-rw-r--r--   0        0        0     1435 2023-05-25 12:49:21.092317 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/debug.py
+-rw-r--r--   0        0        0     6616 2023-05-30 19:26:00.787412 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/auth.py
+-rw-r--r--   0        0        0      562 2023-05-30 19:26:00.787702 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/db.py
+-rw-r--r--   0        0        0      756 2023-05-30 19:26:00.788092 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/middleware.py
+-rw-r--r--   0        0        0     5177 2023-06-29 11:59:33.542786 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/router.py
+-rw-r--r--   0        0        0    10093 2023-05-30 19:26:00.788614 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/sessions.py
+-rw-r--r--   0        0        0      484 2023-05-25 12:49:21.092418 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/event.py
+-rw-r--r--   0        0        0      841 2023-05-30 10:26:07.846938 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/exceptions.py
+-rw-r--r--   0        0        0     1990 2023-06-28 20:34:06.719562 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py
+-rw-r--r--   0        0        0     4119 2023-06-29 11:46:03.627036 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/queue.py
+-rw-r--r--   0        0        0      264 2023-05-25 12:49:21.092910 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/types.py
+-rw-r--r--   0        0        0      798 2023-06-29 11:46:18.556383 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/utils.py
+-rw-r--r--   0        0        0      324 2023-05-25 12:49:21.093287 strawberry_django_pubsub-0.0.7a0/tox.ini
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 strawberry_django_pubsub-0.0.7a0/PKG-INFO
```

### Comparing `strawberry_django_pubsub-0.0.6a0/.gitignore` & `strawberry_django_pubsub-0.0.7a0/.gitignore`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/LICENSE` & `strawberry_django_pubsub-0.0.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/pyproject.toml` & `strawberry_django_pubsub-0.0.7a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/requirements/compile.py` & `strawberry_django_pubsub-0.0.7a0/requirements/compile.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/requirements/py310-django41.txt` & `strawberry_django_pubsub-0.0.7a0/requirements/py310-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/requirements/py310-django42.txt` & `strawberry_django_pubsub-0.0.7a0/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/requirements/py311-django41.txt` & `strawberry_django_pubsub-0.0.7a0/requirements/py311-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/requirements/py311-django42.txt` & `strawberry_django_pubsub-0.0.7a0/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/requirements/py39-django41.txt` & `strawberry_django_pubsub-0.0.7a0/requirements/py39-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/requirements/py39-django42.txt` & `strawberry_django_pubsub-0.0.7a0/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/asgi.py` & `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,28 +29,33 @@
 __all__ = ["DjangoWsGraphQL"]
 
 
 WEBSOCKET_TYPE = "websocket"
 
 
 class DjangoWsGraphQL:
-    def __init__(self, schema: BaseSchema, debug: bool = False, *args, **kwargs):
+    def __init__(
+        self,
+        schema: BaseSchema,
+        debug: bool = False,
+        *args,
+        **kwargs,
+    ):
         self.schema = schema
         self.debug = debug
 
     async def __call__(
         self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable
     ) -> None:
         """
         Handles ASGI Websocket protocol for Django, without channels dependency.
         """
 
         self.scope = scope
         self._send = send
-
         self.user = self.scope['user']
 
         self.client_state = WebSocketState.CONNECTING
         self.application_state = WebSocketState.CONNECTING
 
         # ensure where mounted on a websocket
         if not self.scope["type"] == WEBSOCKET_TYPE:
@@ -122,15 +127,15 @@
         """
 
         await self.send({"type": "websocket.accept", "subprotocol": subprotocol})
 
     async def connect(self) -> None:
         self._handler = GraphQLTransportWSHandler(
             schema=self.schema,
-            debug=True,
+            debug=self.debug,
             connection_init_wait_timeout=datetime.timedelta(minutes=1),
             get_context=self.get_context,
             get_root_value=self.get_root_value,
             ws=self,
         )
 
         await self._handler.handle()
```

### Comparing `strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/context.py` & `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/context.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/debug.py` & `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/debug.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/django/auth.py` & `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/auth.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/django/db.py` & `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/db.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/django/middleware.py` & `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/middleware.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/django/router.py` & `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/router.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import importlib
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.urls.exceptions import Resolver404
 from django.urls.resolvers import URLResolver
 
+from strawberry_django_pubsub.queue import queue
+
 """
 All Routing instances inside this file are also valid ASGI applications - with
 new Channels routing, whatever you end up with as the top level object is just
 served up as the "ASGI application".
 """
 
 
@@ -29,31 +31,46 @@
     except AttributeError:
         raise ImproperlyConfigured(
             "Cannot find %r in ASGI_APPLICATION module %s" % (name, path)
         )
     return value
 
 
-class ProtocolTypeRouter:
+class QueueProtocolTypeRouter:
     """
     Takes a mapping of protocol type names to other Application instances,
     and dispatches to the right one based on protocol name (or raises an error)
     """
 
-    def __init__(self, application_mapping):
+    def __init__(
+        self,
+        application_mapping,
+    ):
         self.application_mapping = application_mapping
 
     async def __call__(self, scope, receive, send):
-        if scope["type"] in self.application_mapping:
-            application = self.application_mapping[scope["type"]]
-            return await application(scope, receive, send)
+        # Need to move this into QueueLifeSpanRouter
+        if scope['type'] == 'lifespan':
+            while True:
+                message = await receive()
+                if message['type'] == 'lifespan.startup':
+                    await queue.connect()
+                    await send({'type': 'lifespan.startup.complete'})
+                elif message['type'] == 'lifespan.shutdown':
+                    await queue.disconnect()
+                    await send({'type': 'lifespan.shutdown.complete'})
+                    return
         else:
-            raise ValueError(
-                "No application configured for scope type %r" % scope["type"]
-            )
+            if scope["type"] in self.application_mapping:
+                application = self.application_mapping[scope["type"]]
+                return await application(scope, receive, send)
+            else:
+                raise ValueError(
+                    "No application configured for scope type %r" % scope["type"]
+                )
 
 
 class URLRouter:
     """
     Routes to different applications/consumers based on the URL path.
 
     Works with anything that has a ``path`` key, but intended for WebSocket
```

### Comparing `strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/django/sessions.py` & `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/sessions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/exceptions.py` & `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/exceptions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py` & `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.6a0/strawberry_django_pubsub/queue.py` & `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,22 +64,22 @@
         return self
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
         await self.disconnect()
 
     async def connect(self) -> None:
         """
-        connect method: setup queue and run a seperate listener task
+        setup queue and run a seperate listener task
         """
         await self._queue.connect()
         self._current_task = asyncio.create_task(self._listener())
 
     async def disconnect(self) -> None:
         """
-        disconnect method: we cleanup all running tasks.
+        cleanup all running tasks.
         rather then calling this method directly it should
         be mounted on a shutdown of lifespan queue.
         """
 
         if self._current_task.done():
             self._current_task.result()
         else:
```

### Comparing `strawberry_django_pubsub-0.0.6a0/PKG-INFO` & `strawberry_django_pubsub-0.0.7a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-pubsub
-Version: 0.0.6a0
+Version: 0.0.7a0
 Summary: Strawberry Django PubSub 
 Author-email: DK <dk@terminalkitten.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

