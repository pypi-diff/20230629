# Comparing `tmp/configzen-0.4.5.tar.gz` & `tmp/configzen-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.4.5.tar", max compression
+gzip compressed data, was "configzen-0.4.6.tar", max compression
```

## Comparing `configzen-0.4.5.tar` & `configzen-0.4.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      513 2023-06-29 09:13:33.339374 configzen-0.4.5/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4.5/configzen/__main__.py
--rw-r--r--   0        0        0     1437 2023-06-29 09:14:40.075983 configzen-0.4.5/configzen/_isolation.py
--rw-r--r--   0        0        0     2916 2023-06-29 09:09:47.165217 configzen-0.4.5/configzen/_setup.py
--rw-r--r--   0        0        0    76173 2023-06-29 09:14:43.431854 configzen-0.4.5/configzen/config.py
--rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4.5/configzen/decorators.py
--rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4.5/configzen/errors.py
--rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4.5/configzen/field.py
--rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4.5/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4.5/configzen/py.typed
--rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4.5/configzen/route.py
--rw-r--r--   0        0        0     1168 2023-06-29 08:15:33.949387 configzen-0.4.5/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4.5/LICENSE
--rw-r--r--   0        0        0     1473 2023-06-29 09:14:10.332011 configzen-0.4.5/pyproject.toml
--rw-r--r--   0        0        0    12655 2023-06-29 08:54:11.087815 configzen-0.4.5/README.md
--rw-r--r--   0        0        0    13246 1970-01-01 00:00:00.000000 configzen-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-29 09:13:33.339374 configzen-0.4.6/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4.6/configzen/__main__.py
+-rw-r--r--   0        0        0     1437 2023-06-29 09:14:40.075983 configzen-0.4.6/configzen/_isolation.py
+-rw-r--r--   0        0        0     2916 2023-06-29 09:09:47.165217 configzen-0.4.6/configzen/_setup.py
+-rw-r--r--   0        0        0    74687 2023-06-29 09:23:25.826027 configzen-0.4.6/configzen/config.py
+-rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4.6/configzen/decorators.py
+-rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4.6/configzen/errors.py
+-rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4.6/configzen/field.py
+-rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4.6/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4.6/configzen/py.typed
+-rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4.6/configzen/route.py
+-rw-r--r--   0        0        0     1168 2023-06-29 08:15:33.949387 configzen-0.4.6/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4.6/LICENSE
+-rw-r--r--   0        0        0     1473 2023-06-29 09:24:58.049052 configzen-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0    12655 2023-06-29 08:54:11.087815 configzen-0.4.6/README.md
+-rw-r--r--   0        0        0    13246 1970-01-01 00:00:00.000000 configzen-0.4.6/PKG-INFO
```

### Comparing `configzen-0.4.5/configzen/__init__.py` & `configzen-0.4.6/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/configzen/__main__.py` & `configzen-0.4.6/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/configzen/_isolation.py` & `configzen-0.4.6/configzen/_isolation.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/configzen/_setup.py` & `configzen-0.4.6/configzen/_setup.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/configzen/config.py` & `configzen-0.4.6/configzen/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,18 +121,14 @@
     aiofiles = None  # type: ignore[assignment]
     AIOFILES_AVAILABLE = False
 
 __all__ = (
     "ConfigAgent",
     "ConfigModel",
     "ConfigMeta",
-    "save",
-    "save_async",
-    "reload",
-    "reload_async",
     "export_hook",
     "field_hook",
     "export_model",
     "export_model_async",
 )
 
 _URL_SCHEMES: set[str] = set(
@@ -1286,83 +1282,67 @@
         **kwargs
             Keyword arguments to pass to the saving function.
 
         Returns
         -------
         The number of bytes written.
         """
-        return await save_async(self, **kwargs)
+        return await _save_async(self, **kwargs)
 
     def save(self, **kwargs: Any) -> int:
         """
         Save the configuration.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the saving function.
 
         Returns
         -------
         The number of bytes written.
         """
-        return save(self, **kwargs)
+        return _save(self, **kwargs)
 
     async def reload_async(self, **kwargs: Any) -> Any:
         """
         Reload the configuration asynchronously.
 
         Parameters
         ----------
         kwargs
             Keyword arguments to pass to the reloading function.
 
         Returns
         -------
         The reloaded configuration or its belonging item.
         """
-        return await reload_async(self, **kwargs)
+        return await _reload_async(self, **kwargs)
 
     def reload(self, **kwargs: Any) -> Any:
         """
         Reload the configuration.
 
         Parameters
         ----------
         kwargs
             Keyword arguments to pass to the reloading function.
 
         Returns
         -------
         The reloaded configuration or its belonging item.
         """
-        return reload(self, **kwargs)
+        return _reload(self, **kwargs)
 
 
-def save(
+def _save(
     section: ConfigModelT | ConfigAt[ConfigModelT],
     write_kwargs: dict[str, Any] | None = None,
     **kwargs: Any,
 ) -> int:
-    """
-    Save the configuration.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    write_kwargs
-        Keyword arguments to pass to the writing function.
-    **kwargs
-        Keyword arguments to pass to the dumping function.
-
-    Returns
-    -------
-    The number of bytes written.
-    """
     if isinstance(section, ConfigModel):
         config = section
         return config.save(write_kwargs=write_kwargs, **kwargs)
 
     if write_kwargs is None:
         write_kwargs = {}
 
@@ -1373,35 +1353,19 @@
     context = get_context(config)
     blob = context.agent.dump_config(config.copy(update=data), **kwargs)
     result = config.write(blob, **write_kwargs)
     context.initial_state = data
     return result
 
 
-async def save_async(
+async def _save_async(
     section: ConfigModelT | ConfigAt[ConfigModelT],
     write_kwargs: dict[str, Any] | None = None,
     **kwargs: Any,
 ) -> int:
-    """
-    Save the configuration asynchronously.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    write_kwargs
-        Keyword arguments to pass to the writing function.
-    **kwargs
-        Keyword arguments to pass to the dumping function.
-
-    Returns
-    -------
-    The number of bytes written.
-    """
     if isinstance(section, ConfigModel):
         config = section
         return await config.save_async(write_kwargs=write_kwargs, **kwargs)
 
     if write_kwargs is None:
         write_kwargs = {}
 
@@ -1412,59 +1376,31 @@
     context = get_context(config)
     blob = context.agent.dump_config(config.copy(update=data), **kwargs)
     result = await config.write_async(blob, **write_kwargs)
     context.initial_state = data
     return result
 
 
-def reload(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> Any:
-    """
-    Reload the configuration.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    **kwargs
-        Keyword arguments to pass to the reloading function.
-
-    Returns
-    -------
-    The reloaded configuration or its belonging item.
-    """
+def _reload(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> Any:
     if isinstance(section, ConfigModel):
         config = section
         return config.reload()
 
     config = section.owner
     context = get_context(config)
     state = config.__dict__
     newest = context.agent.read(config_class=type(config), **kwargs)
     section_data = ConfigAt(newest, newest.__dict__, section.route).get()
     ConfigAt(config, state, section.route).update(section_data)
     return section_data
 
 
-async def reload_async(
+async def _reload_async(
     section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any
 ) -> Any:
-    """
-    Reload the configuration asynchronously.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    kwargs
-        Keyword arguments to pass to the reloading function.
-
-    Returns
-    -------
-    The reloaded configuration or its belonging item.
-    """
     if isinstance(section, ConfigModel):
         config = section
         return await config.reload_async()
 
     config = section.owner
     context = get_context(config)
     state = config.__dict__
@@ -2200,15 +2136,15 @@
         self
         """
         context = get_context(self)
         current_context.set(get_context(context.owner))
         if context.owner is self:
             changed = context.agent.read(config_class=type(self), **kwargs)
         else:
-            changed = reload(cast(ConfigModelT, context.at), **kwargs)
+            changed = _reload(cast(ConfigModelT, context.at), **kwargs)
         state = changed.__dict__
         context.initial_state = state
         self.update(state)
         return self
 
     def save(
         self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
@@ -2231,15 +2167,15 @@
         if context.owner is self:
             if write_kwargs is None:
                 write_kwargs = {}
             blob = context.agent.dump_config(self, **kwargs)
             result = self.write(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
-        return save(
+        return _save(
             cast(ConfigAt[ConfigModelT], context.at),
             write_kwargs=write_kwargs,
             **kwargs,
         )
 
     def write(self, blob: str | bytes, **kwargs: Any) -> int:
         """
@@ -2324,15 +2260,15 @@
         self
         """
         context = get_context(self)
         current_context.set(get_context(context.owner))
         if context.owner is self:
             changed = await context.agent.read_async(config_class=type(self), **kwargs)
         else:
-            changed = await reload_async(
+            changed = await _reload_async(
                 cast(ConfigAt[ConfigModelT], context.at), **kwargs
             )
         state = changed.__dict__
         context.initial_state = state
         self.update(state)
         return self
 
@@ -2358,15 +2294,15 @@
             if write_kwargs is None:
                 write_kwargs = {}
             _exporting.set(True)  # noqa: FBT003
             blob = await context.agent.dump_config_async(self, **kwargs)
             result = await self.write_async(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
-        return await save_async(
+        return await _save_async(
             cast(ConfigAt[ConfigModelT], context.at),
             write_kwargs=write_kwargs,
             **kwargs,
         )
 
     async def write_async(self, blob: str | bytes, **kwargs: Any) -> int:
         """
```

### Comparing `configzen-0.4.5/configzen/decorators.py` & `configzen-0.4.6/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/configzen/errors.py` & `configzen-0.4.6/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/configzen/field.py` & `configzen-0.4.6/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/configzen/processor.py` & `configzen-0.4.6/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/configzen/route.py` & `configzen-0.4.6/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/configzen/typedefs.py` & `configzen-0.4.6/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/LICENSE` & `configzen-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/pyproject.toml` & `configzen-0.4.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.4.5"
+version = "0.4.6"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.4.5/README.md` & `configzen-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.4.5/PKG-INFO` & `configzen-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.4.5
+Version: 0.4.6
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

