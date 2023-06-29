# Comparing `tmp/pecs_framework-1.2.0.tar.gz` & `tmp/pecs_framework-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pecs_framework-1.2.0.tar", max compression
+gzip compressed data, was "pecs_framework-1.2.1.tar", max compression
```

## Comparing `pecs_framework-1.2.0.tar` & `pecs_framework-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1085 2022-06-10 19:53:43.228064 pecs_framework-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0      277 2022-12-12 01:12:02.677008 pecs_framework-1.2.0/pecs_framework/__init__.py
--rw-r--r--   0        0        0      460 2022-11-29 04:09:33.534556 pecs_framework-1.2.0/pecs_framework/_types.py
--rw-r--r--   0        0        0     1938 2022-12-11 23:43:58.407261 pecs_framework-1.2.0/pecs_framework/base_system.py
--rw-r--r--   0        0        0     1389 2022-12-11 23:43:58.407760 pecs_framework-1.2.0/pecs_framework/component.py
--rw-r--r--   0        0        0     5500 2022-12-11 23:43:58.408261 pecs_framework-1.2.0/pecs_framework/domain.py
--rw-r--r--   0        0        0     5232 2022-12-11 23:43:58.408762 pecs_framework-1.2.0/pecs_framework/engine.py
--rw-r--r--   0        0        0      215 2022-12-11 23:43:58.408762 pecs_framework-1.2.0/pecs_framework/entities/__init__.py
--rw-r--r--   0        0        0     2254 2022-12-11 23:43:58.409260 pecs_framework-1.2.0/pecs_framework/entities/entity.py
--rw-r--r--   0        0        0     2895 2022-12-11 23:43:58.409260 pecs_framework-1.2.0/pecs_framework/entities/utils.py
--rw-r--r--   0        0        0     1652 2022-12-11 23:43:58.409763 pecs_framework-1.2.0/pecs_framework/events.py
--rw-r--r--   0        0        0      988 2022-11-29 04:09:33.574678 pecs_framework-1.2.0/pecs_framework/loader.py
--rw-r--r--   0        0        0     5306 2022-12-11 23:43:58.410261 pecs_framework-1.2.0/pecs_framework/prefab.py
--rw-r--r--   0        0        0     2160 2022-12-11 23:43:58.410261 pecs_framework-1.2.0/pecs_framework/query.py
--rw-r--r--   0        0        0     1241 2022-12-11 23:43:58.410761 pecs_framework-1.2.0/pecs_framework/utils.py
--rw-r--r--   0        0        0     1051 2022-12-12 02:00:51.573881 pecs_framework-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     8502 2022-12-12 01:50:29.967382 pecs_framework-1.2.0/README.md
--rw-r--r--   0        0        0     9449 1970-01-01 00:00:00.000000 pecs_framework-1.2.0/setup.py
--rw-r--r--   0        0        0     9470 1970-01-01 00:00:00.000000 pecs_framework-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-06-10 19:53:43.228064 pecs_framework-1.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      333 2023-06-29 19:29:04.228017 pecs_framework-1.2.1/pecs_framework/__init__.py
+-rw-r--r--   0        0        0      460 2023-01-22 04:46:10.712761 pecs_framework-1.2.1/pecs_framework/_types.py
+-rw-r--r--   0        0        0     1929 2023-01-22 04:43:10.236797 pecs_framework-1.2.1/pecs_framework/base_system.py
+-rw-r--r--   0        0        0     1370 2023-01-22 04:43:14.833033 pecs_framework-1.2.1/pecs_framework/component.py
+-rw-r--r--   0        0        0     5460 2023-01-22 04:43:18.383783 pecs_framework-1.2.1/pecs_framework/domain.py
+-rw-r--r--   0        0        0     5198 2023-01-22 04:43:22.749476 pecs_framework-1.2.1/pecs_framework/engine.py
+-rw-r--r--   0        0        0      215 2022-12-11 23:43:58.408762 pecs_framework-1.2.1/pecs_framework/entities/__init__.py
+-rw-r--r--   0        0        0     2216 2023-01-22 04:46:02.897766 pecs_framework-1.2.1/pecs_framework/entities/entity.py
+-rw-r--r--   0        0        0     2894 2023-01-22 04:46:05.879759 pecs_framework-1.2.1/pecs_framework/entities/utils.py
+-rw-r--r--   0        0        0     1652 2023-01-22 04:46:12.115199 pecs_framework-1.2.1/pecs_framework/events.py
+-rw-r--r--   0        0        0      980 2023-01-22 04:43:30.036921 pecs_framework-1.2.1/pecs_framework/loader.py
+-rw-r--r--   0        0        0     5238 2023-01-22 04:45:43.942386 pecs_framework-1.2.1/pecs_framework/prefab.py
+-rw-r--r--   0        0        0     2160 2022-12-11 23:43:58.410261 pecs_framework-1.2.1/pecs_framework/query.py
+-rw-r--r--   0        0        0     1242 2023-01-22 04:45:52.911469 pecs_framework-1.2.1/pecs_framework/utils.py
+-rw-r--r--   0        0        0     1051 2023-06-29 19:32:07.152260 pecs_framework-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8502 2022-12-12 01:50:29.967382 pecs_framework-1.2.1/README.md
+-rw-r--r--   0        0        0     9319 1970-01-01 00:00:00.000000 pecs_framework-1.2.1/PKG-INFO
```

### Comparing `pecs_framework-1.2.0/LICENSE.txt` & `pecs_framework-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pecs_framework-1.2.0/pecs_framework/base_system.py` & `pecs_framework-1.2.1/pecs_framework/base_system.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def teardown(self) -> None:
         raise NotImplementedError("Method has no implementation")
 
     @abstractmethod
     def pre_update(self) -> None:
         raise NotImplementedError("Method has no implementation")
 
-    @abstractmethod    
+    @abstractmethod
     def update(self) -> None:
         raise NotImplementedError("Method has no implementation")
 
     @abstractmethod
     def post_update(self) -> None:
         raise NotImplementedError("Method has no implementation")
 
@@ -41,26 +41,26 @@
 
     def __init__(self, loop: Loop) -> None:
         self.loop = loop
         self._queries: dict[str, Query] = {}
         self.initialize()
 
     def query(
-        self, 
-        key: str, 
+        self,
+        key: str,
         all_of: ComponentQuery | None = None,
-        any_of: ComponentQuery | None = None, 
+        any_of: ComponentQuery | None = None,
         none_of: ComponentQuery | None = None,
     ) -> None:
         all_of = all_of if all_of else []
         any_of = any_of if any_of else []
         none_of = none_of if none_of else []
         self._queries[key] = self.loop.domain.create_query(
-            all_of, 
-            any_of, 
+            all_of,
+            any_of,
             none_of,
         )
 
     def initialize(self):
         raise NotImplementedError("Method has no implementation")
 
     def update(self):
```

### Comparing `pecs_framework-1.2.0/pecs_framework/component.py` & `pecs_framework-1.2.1/pecs_framework/component.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 
 class ComponentMeta(type):
     """Base Component Metaclass"""
     comp_id: str
     cbit: int
     _entity_id: str
-    
+
     def __new__(
-        cls: type[ComponentMeta], 
-        clsname: str, 
-        bases: Bases, 
+        cls: type[ComponentMeta],
+        clsname: str,
+        bases: Bases,
         namespace: Namespace,
     ) -> ComponentMeta:
         clsobj = super().__new__(cls, clsname, bases, namespace)
         clsobj.comp_id = clsname.upper()
         clsobj.cbit = 0
         return clsobj
-    
-    
+
+
 class Component(metaclass=ComponentMeta):
     """Root Component class that all components extend."""
     _entity_id: str
 
     @property
     def entity_id(self) -> str:
         return self._entity_id
@@ -45,11 +45,11 @@
             return None
         except Exception:
             traceback.print_exc(file=sys.stderr)
             raise
 
     def on_event(self, evt: EntityEvent) -> EntityEvent | None:
         pass
-    
+
 
 # Type variable ranging over Component instances
 CT = TypeVar("CT", bound=Component)
```

### Comparing `pecs_framework-1.2.0/pecs_framework/domain.py` & `pecs_framework-1.2.1/pecs_framework/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self._map[key] = entity
 
     def keys(self):
         return self._map.keys()
 
     def values(self):
         return self._map.values()
-    
+
     def get_entity_id(self, entity_or_alias: Entity | str) -> str:
         """
         Get an Entity's identifier either by passing the entity itself or its
         alias.
 
         Parameters
         ----------
@@ -52,15 +52,15 @@
             The Entity's unique identifier
         """
         if isinstance(entity_or_alias, str):
             id_: str = self.aliases.get(entity_or_alias, '')
         else:
             id_: str = entity_or_alias.eid
         return id_
-    
+
     def create(self, alias: str | None = None) -> Entity:
         """
         Create a new Entity in the engine's Entity registry.
 
         Parameters
         ----------
         alias, optional
@@ -68,15 +68,15 @@
 
         Returns
         -------
             The newly created Entity instance
         """
         entity = Entity(self.domain, self.domain.create_uid())
         self._map[entity.eid] = entity
-        
+
         if alias:
             if alias in self.aliases.keys():
                 raise KeyError(f"Entity already exists with alias {alias}")
             self.aliases[alias] = entity.eid
 
         return entity
 
@@ -104,15 +104,15 @@
                 if name in keys:
                     comp_props[name].update(prop_block)
 
         # Finally, attach concrete components to the entity, using the resolved
         # props from the process above.
         for name, props in comp_props.items():
             self.domain.engine.components.attach(entity, name, props)
-        
+
         return entity
 
     def get_by_alias(self, alias: str) -> Entity:
         """
         Get a specific Entity instance via its alias, if it has one.
 
         Parameters
@@ -140,19 +140,19 @@
 
     def remove_entity_by_alias(self, alias: str) -> None:
         entity_id = self.get_entity_id(alias)
         self.remove_entity_by_id(entity_id)
 
 
 class Domain:
-    
+
     @staticmethod
     def create_uid() -> str:
         return str(uuid1())
-    
+
     def __init__(self, engine: Engine) -> None:
         self.engine = engine
         self.entities = EntityRegistry(self)
         self.queries: List[Query] = []
 
     def destroy_entity(self, entity: Entity | str) -> None:
         if isinstance(entity, str):
@@ -164,15 +164,15 @@
             self.entities.remove_entity_by_id(entity.eid)
 
     def create_query(
         self,
         all_of: ComponentQuery | None = None,
         any_of: ComponentQuery | None = None,
         none_of: ComponentQuery | None = None,
-    ) -> Query:        
+    ) -> Query:
         query = Query(self, all_of, any_of, none_of)
         self.queries.append(query)
         return query
 
     def candidate(self, entity: Entity) -> None:
         for query in self.queries:
             query.candidate(entity)
```

### Comparing `pecs_framework-1.2.0/pecs_framework/engine.py` & `pecs_framework-1.2.1/pecs_framework/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     from pecs_framework.loader import Loader
 
 from pecs_framework.utils import *
 from pecs_framework.component import ComponentMeta, Component
 from pecs_framework.domain import Domain, EntityRegistry
 from pecs_framework.entities import Entity
 from pecs_framework.entities import (
-    has_component, 
+    has_component,
     add_component,
     add_component_type,
     remove_component,
 )
 from pecs_framework.prefab import PrefabBuilder
 
 
 class ComponentRegistry:
-    
+
     def __init__(self, engine: Engine) -> None:
         self._engine = engine
         self._cbits = 0
         self._map: OrderedDict[CompId, ComponentMeta] = OrderedDict()
 
     def load(self, pathspec: str) -> None:
         if self._engine._loader:
@@ -49,16 +49,16 @@
             _key: CompId = key.upper()
         else:
             _key = key.comp_id
         return cast(type[Component], self._map[_key])
 
     @beartype
     def attach(
-        self, 
-        entity: Entity, 
+        self,
+        entity: Entity,
         component: ComponentMeta | str | Component,
         properties: dict[str, Any] | None = None,
     ) -> None:
         """
         Attach a Component to an Entity.
 
         A Component in this context can be a ComponentType (an uninstantiated
@@ -79,47 +79,47 @@
         component
             A ComponentType, Component instance, or a Component name
         properties, optional
             A dict of arguments to pass to a Component class, by default None
         """
         if isinstance(component, str):
             component = self._map[component.upper()]
-            
+
         if isinstance(component, ComponentMeta):
             properties_ = properties if properties else {}
             add_component_type(entity, component, properties_)
         else:
             add_component(entity, component)
 
     @beartype
     def remove(
-        self, 
-        entity: Entity, 
+        self,
+        entity: Entity,
         component: ComponentMeta | str | Component
     ) -> None:
         if not isinstance(component, ComponentMeta):
             if isinstance(component, str):
                 component = self._map[component.upper()]
             else:
                 component = component.__class__
-        
+
         remove_component(entity, component)
 
     @beartype
     def has(self, entity: Entity, component_type: ComponentMeta) -> bool:
         if not entity:
             return False
         return has_component(entity, component_type)
 
 
 class Engine:
-    
+
     def __init__(self, loader: Loader | None = None) -> None:
         """
-        The core ECS engine, providing access to the Domain and 
+        The core ECS engine, providing access to the Domain and
         ComponentRegistry objects.
         """
         self._domain: Domain
         self._components: ComponentRegistry
         self._prefabs: PrefabBuilder
         self._domains = {}
         self._registries = {}
```

### Comparing `pecs_framework-1.2.0/pecs_framework/entities/entity.py` & `pecs_framework-1.2.1/pecs_framework/entities/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,41 +25,41 @@
         if isinstance(component, str):
             _component = self.domain.engine.components.get_type(component)
         else:
             _component = component
         return cast(CT, get_component(self, _component))
 
     def fire_event(
-            self, 
-            event: str, 
-            data: dict[str, Any] | EventData | None = None
-        ) -> EntityEvent:
+        self,
+        event: str,
+        data: dict[str, Any] | EventData | None = None
+    ) -> EntityEvent:
         if data and isinstance(data, EventData):
             data = data.record
         elif data and isinstance(data, dict):
             data = EventData(**data).record
         else:
             data = {}
         evt = EntityEvent(event, data)
 
         for component in self.components.values():
             component.handle_event(evt)
             if evt.prevented:
                 return evt
         return evt
-    
+
     def on_component_added(self):
         pass
 
     def on_component_removed(self):
         pass
 
     def on_entity_destroyed(self):
         pass
-    
+
     def _on_component_added(self):
         candidacy(self.domain, self)
         self.on_component_added()
 
     def _on_component_removed(self):
         candidacy(self.domain, self)
         self.on_component_removed()
@@ -68,9 +68,9 @@
         to_delete = []
         for component in self.components.values():
             to_delete.append(component)
 
         for component in to_delete:
             self.components[component.comp_id]._entity_id = ''
             del self.components[component.comp_id]
-            
+
         self.on_entity_destroyed()
```

### Comparing `pecs_framework-1.2.0/pecs_framework/entities/utils.py` & `pecs_framework-1.2.1/pecs_framework/entities/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from .entity import Entity
 
 from pecs_framework.utils import has_bit, subtract_bit, add_bit
 from pecs_framework.component import Component, ComponentMeta, CT
 
 
 def add_component_type(
-    entity: Entity, 
+    entity: Entity,
     component: ComponentMeta,
     properties: dict[str, Any] | None = None,
 ) -> None:
     """
     Add a Component class and instantiate it on the Entity.
 
     If the Component class requires parameters, these can be passed as a
```

### Comparing `pecs_framework-1.2.0/pecs_framework/events.py` & `pecs_framework-1.2.1/pecs_framework/events.py`

 * *Files identical despite different names*

### Comparing `pecs_framework-1.2.0/pecs_framework/loader.py` & `pecs_framework-1.2.1/pecs_framework/loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Loader:
 
     def __init__(self, file: str) -> None:
         here = os.path.dirname(os.path.abspath(file))
         self.tree = os.listdir(here)
         self.tree.remove("__init__.py")
         self.tree.remove("__pycache__")
-        
+
         self._components = []
 
     @property
     def components(self) -> list[type[Component]]:
         return self._components
 
     def load(self, pathspec: str) -> None:
```

### Comparing `pecs_framework-1.2.0/pecs_framework/prefab.py` & `pecs_framework-1.2.1/pecs_framework/prefab.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,55 +49,55 @@
         self._depth = 0
 
     @property
     def templates(self) -> dict[str, EntityTemplate]:
         return self._templates
 
     def deserialize(self, definition: str) -> EntityTemplate:
-        data = dict(json.loads(definition))
+        data: dict[str, Any] = dict(json.loads(definition))
         components: list[ComponentTemplate] = []
 
         if 'components' in data.keys():
-            for comp_def in data['components']:                
+            for comp_def in data['components']:
                 component_template = ComponentTemplate(
-                    component_type = comp_def['type'],
-                    properties = comp_def.get('properties', {}),
+                    component_type=comp_def['type'],
+                    properties=comp_def.get('properties', {}),
                 )
 
                 components.append(component_template)
 
         entity_template = EntityTemplate(
-            name = data['name'],
-            inherit = data.get('inherit', []),
-            components = components,
+            name=data['name'],
+            inherit=data.get('inherit', []),
+            components=components,
         )
 
         return entity_template
-        
+
     def register(self, path: str, file: str) -> None:
         full_path = os.path.join(str(Path(path) / file))
         if full_path[-5:] != '.json':
-             full_path += '.json'
-        
+            full_path += '.json'
+
         with open(full_path, 'r') as prefab_file:
             data = prefab_file.read()
-            
+
         prefab = self.deserialize(data)
         self._templates[prefab.name] = prefab
 
     def build_prefab(self, template_name: str) -> EntityTemplate:
         copied_prefab = deepcopy(self._templates[template_name])
 
         # Traverse up the inheritance tree, writing all found entity templates
         # to the temp array to cache them.
         prefab = self.recurse_template(copied_prefab)
 
         # Once we've returned to this method, extend our original prefab's
         # components with the components of each found parent template.
-        
+
         # prefab_components = deque(prefab.components)
         for template in self._temp:
             # for component in template.components:
             #     prefab_components.append(component)
             prefab.components.extend(template.components)
 
         # Clear the temp array so we don't pollute other templates.
@@ -107,21 +107,21 @@
     def recurse_template(self, template: EntityTemplate) -> EntityTemplate:
         inherited = deque(template.inherit)
         while len(inherited) > 0:
             parent = inherited.popleft()
             self._temp.appendleft(self.recurse_template(self.templates[parent]))
         else:
             return template
-                    
+
         # for parent in template.inherit:
         #     self._temp.append(self.recurse_template(self.templates[parent]))
         # return template
 
     def resolve_overrides(
-        self, 
+        self,
         components: list[ComponentTemplate]
     ) -> dict[str, dict[str, Any]]:
         """
         From a list of potentially non-unique ComponentTemplate objects, resolve
         all property blocks down to unary blocks, where blocks from descendant
         components override those of their ancestor components in the
         inheritance tree.
```

### Comparing `pecs_framework-1.2.0/pecs_framework/query.py` & `pecs_framework-1.2.1/pecs_framework/query.py`

 * *Files identical despite different names*

### Comparing `pecs_framework-1.2.0/pecs_framework/utils.py` & `pecs_framework-1.2.1/pecs_framework/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 def all_equal(arr: Iterable) -> bool:
     g = groupby(arr)
     return next(g, True) and not next(g, False)
 
 
 def iter_index(
-    arr: Sequence[ComponentTemplate], 
+    arr: Sequence[ComponentTemplate],
     value: ComponentTemplate,
     start: int = 0,
 ) -> Generator[int, None, None]:
     try:
         # Check if the iterable supports indexing.
         seq_index = arr.index
     except AttributeError:
@@ -41,10 +41,10 @@
         for i, element in enumerate(it, start):
             if element is value or element == value:
                 yield i
     else:
         i = start - 1
         try:
             while True:
-                yield (i := seq_index(value, i+1))
+                yield (i := seq_index(value, i + 1))
         except ValueError:
             pass
```

### Comparing `pecs_framework-1.2.0/pyproject.toml` & `pecs_framework-1.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pecs-framework"
-version = "1.2.0"
+version = "1.2.1"
 description = "The ✨Respectably Muscled✨ Python Entity Component System"
 authors = ["Jonathan Crum <crumja4@gmail.com>"]
 readme = 'README.md'
 repository = 'https://github.com/krummja/PECS'
 classifiers = [
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
```

### Comparing `pecs_framework-1.2.0/README.md` & `pecs_framework-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pecs_framework-1.2.0/setup.py` & `pecs_framework-1.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,295 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pecs-framework
+Version: 1.2.1
+Summary: The ✨Respectably Muscled✨ Python Entity Component System
+Home-page: https://github.com/krummja/PECS
+Author: Jonathan Crum
+Author-email: crumja4@gmail.com
+Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Dist: beartype (>=0.11.0,<0.12.0)
+Requires-Dist: deepmerge (==1.0.1)
+Requires-Dist: numpy (>=1.23.4,<2.0.0)
+Requires-Dist: pytest (>=7.2.0,<8.0.0)
+Requires-Dist: rich (>=12.6.0,<13.0.0)
+Project-URL: Repository, https://github.com/krummja/PECS
+Description-Content-Type: text/markdown
 
-packages = \
-['pecs_framework', 'pecs_framework.entities']
+# PECS
+[![Tests](https://github.com/krummja/PECS/actions/workflows/main.yml/badge.svg)](https://github.com/krummja/PECS/actions/workflows/main.yml) [![Coverage Status](https://coveralls.io/repos/github/krummja/PECS/badge.svg?branch=master)](https://coveralls.io/github/krummja/PECS?branch=master)
 
-package_data = \
-{'': ['*']}
+![Armstrong](/static/lm_pecs_armstrong.png)
 
-install_requires = \
-['beartype>=0.11.0,<0.12.0',
- 'deepmerge==1.0.1',
- 'numpy>=1.23.4,<2.0.0',
- 'pytest>=7.2.0,<8.0.0',
- 'rich>=12.6.0,<13.0.0']
-
-setup_kwargs = {
-    'name': 'pecs-framework',
-    'version': '1.2.0',
-    'description': 'The ✨Respectably Muscled✨ Python Entity Component System',
-    'long_description': '# PECS\n[![Tests](https://github.com/krummja/PECS/actions/workflows/main.yml/badge.svg)](https://github.com/krummja/PECS/actions/workflows/main.yml) [![Coverage Status](https://coveralls.io/repos/github/krummja/PECS/badge.svg?branch=master)](https://coveralls.io/github/krummja/PECS?branch=master)\n\n![Armstrong](/static/lm_pecs_armstrong.png)\n\nPECS is the ✨Respectably Muscled✨ Python ECS library that aims to provide a powerful, user-friendly, and fast-as-hell framework for game development.\n\nThis library is the spiritual successor to my prior ECS library, [ECStremity](https://github.com/krummja/ECStremity). Both this and its predecessor were inspired by the JavaScript ECS library [geotic](https://github.com/ddmills/geotic), created and maintained by [@ddmills](https://github.com/ddmills). I highly recommend checking out that project as well as the excellent resources cited in its README.\n\nWhat is ECS, you ask? [Check it out](https://medium.com/ingeniouslysimple/entities-components-and-systems-89c31464240d)!\n\n## Installation\n\nInstall the package from PyPI using pip:\n\n```\npip install pecs-framework\n```\n\nOr grab it directly from this repository:\n\n```\npip install git+https://github.com/krummja/PECS\n```\n\n## Usage and Examples\n\nTo start flexing your PECS, import the library and set up some components. Components can be built as standard Python classes:\n\n```python\nimport pecs_framework as pecs\n\n\nclass Position(pecs.Component):\n    """Representation of an Entity\'s position in 2D space."""\n\n    def __init__(self, x: int = 0, y: int = 0) -> None:\n        self.x = x\n        self.y = y\n\n    @property\n    def xy(self) -> tuple[int, int]:\n        return self.x, self.y\n```\n\nAs extensions of existing components:\n\n```py\nimport pecs_framework as pecs\n\n\nclass Velocity(Position):\n    """Representation of an Entity\'s velocity in 2D space."""\n\n```\n\nOr as dataclasses:\n\n```py\nimport pecs_framework as pecs\nfrom dataclasses import dataclass, field\n\n\n@dataclass\nclass Health(pecs.Component):\n    """Representation of an Entity\'s health."""\n    maximum: int = 100\n    current: int = field(init=False)\n\n    def __post_init__(self) -> None:\n        self.current = self.maximum\n```\n\nComponents can have as much or as little behavior as needed, although it is generally better to keep to a strict single-repsonsibility principle. We can even have components that have no behavior at all, representing boolean flags for queries:\n\n```py\nimport pecs_framework as pecs\n\n\nclass IsFrozen(pecs.Component):\n    """Flag component denoting a frozen entity."""\n```\n\n\n### Queries\n\nThe easiest way to build out systems is through world queries. To make a system that tracks and updates the components relevant to movement, we might query for `Position` and `Velocity` components. Because we want our entities to move, we want to exclude those marked with the `IsFrozen` flag. Perhaps we also want to grab only those entities that can fly through `Wings` or swim through `Fins`: \n\n```python\nimport pecs_framework as pecs\n\n\necs = pecs.Engine()\ndomain = ecs.create_domain("World")\n\nkinematics = domain.create_query(\n    all_of = [\n        Position, \n        Velocity\n    ],\n    any_of = [\n        Wings, \n        Fins\n    ],\n    none_of = [\n        IsFrozen\n    ],\n)\n```\n\nQueries can specify `all_of`, `any_of`, or `none_of` quantifiers. The query in the example above asks for entities that must have **both** `Position` **and** `Velocity`, may have (inclusive) `Wings` **or** `Fins`, and **must not** have `IsFrozen`.\n\nWe can access the result set of the query and do some operation on them every loop cycle:\n\n```py\ndef process(dt):\n    for entity in targets.result:\n        entity[Position].x += entity[Velocity].x * dt\n        entity[Position].y += entity[Velocity].y * dt\n```\n\nFor convenience, the library provides barebones system class that you can extend for your own purposes:\n\n```py\nimport pecs_framework as pecs\n\n\nclass MovementSystem(pecs.BaseSystem):\n\n    def initialize(self) -> None:\n        self.query(\n            \'movable\',\n            all_of = [Position, Velocity],\n            none_of = [IsFrozen],\n        )\n\n    def update(self) -> None:\n        movables = self._queries\n        for entity in movables:\n            entity[Position].x += entity[Velocity].x\n            entity[Position].y += entity[Velocity].y\n```\n\n> ---\n> \n> **Warning:** \n> \n> Do not override the `__init__` method of `BaseSystem` -- use the provided `initialize` method instead.\n> \n> --- \n\n\n### Broadcasting Events to Components\n\nComplex interactions within and among entities can be achieved by firing events on an entity. This creates an `EntityEvent` that looks for methods on all of the entity\'s methods prefixed with `on_`.\n\n```python\nzombie.fire_event(\'attack\', {\n    \'target\': survivor,\n    \'multiplier\': 1.5,\n})\n```\n\nOn the `zombie` entity, we might have attached an `Attacker` component with the following logic:\n\n```python\nclass Attacker(pecs.Component):\n\n    def __init__(self, strength: int) -> None:\n        self.strength = strength\n\n    def on_attack(self, evt: pecs.EntityEvent) -> pecs.EntityEvent:\n        target: Entity = evt.data.target\n        target.fire_event(\'damage_taken\', {\n            \'amount\': self.strength * evt.data.pultiplier,\n        })\n        evt.handle()\n        return evt\n```\n\nWhen we execute `fire_event` with the event name `attack`, the event system will find all `on_attack` methods on that entity\'s components. If we want the event propagation to stop at a particular component, we can call `evt.handle()` which will immediately break broadcasting down the component list. This means that we can potentially have any number of components respond to a specific event, although it may generally be safer to fire a secondary event to prevent ordering issues.\n\nInternally, the `EntityEvent` class puts together an instance of the class `EventData`, which provides access to the properties defined in the `fire_event` call.\n\n```python\nzombie.fire_event(\'attack\', {\n    \'target\': survivor,                 # <-- We defined \'target\' here\n    \'multiplier\': 1.5                   # <-- and \'multiplier\' here\n})\n\ndef on_attack(self, evt: pecs.EntityEvent) -> pecs.EntityEvent:\n    target = evt.data.target            # --> survivor\n    multiplier = evt.data.multiplier    # --> 1.5\n```\n\nActions can also be defined as a tuple and passed into the `fire_event` method. This allows for easy abstraction over variables used in the event:\n\n```python\nattack_against = (lambda target : (\'attack\', {\n    \'target\': target,\n    \'multiplier\': 1.5\n}))\n\nzombie.fire_event(attack_against(survivor))\n```\n\n### Creating Entities from Prefabs\n\nPECS supports defining prefab entities with preconfigured component properties. Define prefabs as `.json` files and register them with the engine:\n\n```json\n{\n  "name": "GameObject",\n  "inherit": [],\n  "components": [\n    {\n      "type": "Position"\n    },\n    {\n      "type": "Renderable",\n      "properties": {\n        "ch": "?",\n        "bg": [0, 0, 0],\n      }\n    },\n    {\n      "type": "Noun"\n    }\n  ]\n}\n```\n\n```py\nimport pecs_framework as pecs\nimport os\n\n\nROOTDIR = os.path.dirname(__file__)\nPREFABS = os.path.join(ROOTDIR, \'prefabs\')\n\n\necs = pecs.Engine()\necs.prefabs.register(PREFABS, \'game_object\')\n```\n\nNow PECS will look for a file named `game_object.json` in the specified prefabs path and automatically load it for you. We can build an entity using this prefab very easily:\n\n```py\ngame_object = ecs.domain.entities.create_from_prefab(\n    template = \'GameObject\',\n    properties = {\n        \'Position\': {\n            \'x\': 15,\n            \'y\': 10,\n        },\n        \'Renderable\': {\n            \'fg\': [255, 0, 255],\n        },\n        \'Noun\': {\n            \'text\': \'Test Object\'\n        }\n    },\n    alias = \'test_object_01\',\n)\n```\n\nPrefabs can specify other prefabs to inherit from as well. Prefabs can be defined as hierarchies of any depth and breadth. Note that properties will always be resolved from the most deeply embedded prefab to the least, overwriting with the most recent specification. If no properties are passed in the prefab or when creating from prefab, defaults from the component itself will be used.\n\nFor examples, check out the `tests` folder in this repository.\n',
-    'author': 'Jonathan Crum',
-    'author_email': 'crumja4@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/krummja/PECS',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*',
+PECS is the ✨Respectably Muscled✨ Python ECS library that aims to provide a powerful, user-friendly, and fast-as-hell framework for game development.
+
+This library is the spiritual successor to my prior ECS library, [ECStremity](https://github.com/krummja/ECStremity). Both this and its predecessor were inspired by the JavaScript ECS library [geotic](https://github.com/ddmills/geotic), created and maintained by [@ddmills](https://github.com/ddmills). I highly recommend checking out that project as well as the excellent resources cited in its README.
+
+What is ECS, you ask? [Check it out](https://medium.com/ingeniouslysimple/entities-components-and-systems-89c31464240d)!
+
+## Installation
+
+Install the package from PyPI using pip:
+
+```
+pip install pecs-framework
+```
+
+Or grab it directly from this repository:
+
+```
+pip install git+https://github.com/krummja/PECS
+```
+
+## Usage and Examples
+
+To start flexing your PECS, import the library and set up some components. Components can be built as standard Python classes:
+
+```python
+import pecs_framework as pecs
+
+
+class Position(pecs.Component):
+    """Representation of an Entity's position in 2D space."""
+
+    def __init__(self, x: int = 0, y: int = 0) -> None:
+        self.x = x
+        self.y = y
+
+    @property
+    def xy(self) -> tuple[int, int]:
+        return self.x, self.y
+```
+
+As extensions of existing components:
+
+```py
+import pecs_framework as pecs
+
+
+class Velocity(Position):
+    """Representation of an Entity's velocity in 2D space."""
+
+```
+
+Or as dataclasses:
+
+```py
+import pecs_framework as pecs
+from dataclasses import dataclass, field
+
+
+@dataclass
+class Health(pecs.Component):
+    """Representation of an Entity's health."""
+    maximum: int = 100
+    current: int = field(init=False)
+
+    def __post_init__(self) -> None:
+        self.current = self.maximum
+```
+
+Components can have as much or as little behavior as needed, although it is generally better to keep to a strict single-repsonsibility principle. We can even have components that have no behavior at all, representing boolean flags for queries:
+
+```py
+import pecs_framework as pecs
+
+
+class IsFrozen(pecs.Component):
+    """Flag component denoting a frozen entity."""
+```
+
+
+### Queries
+
+The easiest way to build out systems is through world queries. To make a system that tracks and updates the components relevant to movement, we might query for `Position` and `Velocity` components. Because we want our entities to move, we want to exclude those marked with the `IsFrozen` flag. Perhaps we also want to grab only those entities that can fly through `Wings` or swim through `Fins`: 
+
+```python
+import pecs_framework as pecs
+
+
+ecs = pecs.Engine()
+domain = ecs.create_domain("World")
+
+kinematics = domain.create_query(
+    all_of = [
+        Position, 
+        Velocity
+    ],
+    any_of = [
+        Wings, 
+        Fins
+    ],
+    none_of = [
+        IsFrozen
+    ],
+)
+```
+
+Queries can specify `all_of`, `any_of`, or `none_of` quantifiers. The query in the example above asks for entities that must have **both** `Position` **and** `Velocity`, may have (inclusive) `Wings` **or** `Fins`, and **must not** have `IsFrozen`.
+
+We can access the result set of the query and do some operation on them every loop cycle:
+
+```py
+def process(dt):
+    for entity in targets.result:
+        entity[Position].x += entity[Velocity].x * dt
+        entity[Position].y += entity[Velocity].y * dt
+```
+
+For convenience, the library provides barebones system class that you can extend for your own purposes:
+
+```py
+import pecs_framework as pecs
+
+
+class MovementSystem(pecs.BaseSystem):
+
+    def initialize(self) -> None:
+        self.query(
+            'movable',
+            all_of = [Position, Velocity],
+            none_of = [IsFrozen],
+        )
+
+    def update(self) -> None:
+        movables = self._queries
+        for entity in movables:
+            entity[Position].x += entity[Velocity].x
+            entity[Position].y += entity[Velocity].y
+```
+
+> ---
+> 
+> **Warning:** 
+> 
+> Do not override the `__init__` method of `BaseSystem` -- use the provided `initialize` method instead.
+> 
+> --- 
+
+
+### Broadcasting Events to Components
+
+Complex interactions within and among entities can be achieved by firing events on an entity. This creates an `EntityEvent` that looks for methods on all of the entity's methods prefixed with `on_`.
+
+```python
+zombie.fire_event('attack', {
+    'target': survivor,
+    'multiplier': 1.5,
+})
+```
+
+On the `zombie` entity, we might have attached an `Attacker` component with the following logic:
+
+```python
+class Attacker(pecs.Component):
+
+    def __init__(self, strength: int) -> None:
+        self.strength = strength
+
+    def on_attack(self, evt: pecs.EntityEvent) -> pecs.EntityEvent:
+        target: Entity = evt.data.target
+        target.fire_event('damage_taken', {
+            'amount': self.strength * evt.data.pultiplier,
+        })
+        evt.handle()
+        return evt
+```
+
+When we execute `fire_event` with the event name `attack`, the event system will find all `on_attack` methods on that entity's components. If we want the event propagation to stop at a particular component, we can call `evt.handle()` which will immediately break broadcasting down the component list. This means that we can potentially have any number of components respond to a specific event, although it may generally be safer to fire a secondary event to prevent ordering issues.
+
+Internally, the `EntityEvent` class puts together an instance of the class `EventData`, which provides access to the properties defined in the `fire_event` call.
+
+```python
+zombie.fire_event('attack', {
+    'target': survivor,                 # <-- We defined 'target' here
+    'multiplier': 1.5                   # <-- and 'multiplier' here
+})
+
+def on_attack(self, evt: pecs.EntityEvent) -> pecs.EntityEvent:
+    target = evt.data.target            # --> survivor
+    multiplier = evt.data.multiplier    # --> 1.5
+```
+
+Actions can also be defined as a tuple and passed into the `fire_event` method. This allows for easy abstraction over variables used in the event:
+
+```python
+attack_against = (lambda target : ('attack', {
+    'target': target,
+    'multiplier': 1.5
+}))
+
+zombie.fire_event(attack_against(survivor))
+```
+
+### Creating Entities from Prefabs
+
+PECS supports defining prefab entities with preconfigured component properties. Define prefabs as `.json` files and register them with the engine:
+
+```json
+{
+  "name": "GameObject",
+  "inherit": [],
+  "components": [
+    {
+      "type": "Position"
+    },
+    {
+      "type": "Renderable",
+      "properties": {
+        "ch": "?",
+        "bg": [0, 0, 0],
+      }
+    },
+    {
+      "type": "Noun"
+    }
+  ]
 }
+```
+
+```py
+import pecs_framework as pecs
+import os
+
+
+ROOTDIR = os.path.dirname(__file__)
+PREFABS = os.path.join(ROOTDIR, 'prefabs')
+
+
+ecs = pecs.Engine()
+ecs.prefabs.register(PREFABS, 'game_object')
+```
+
+Now PECS will look for a file named `game_object.json` in the specified prefabs path and automatically load it for you. We can build an entity using this prefab very easily:
+
+```py
+game_object = ecs.domain.entities.create_from_prefab(
+    template = 'GameObject',
+    properties = {
+        'Position': {
+            'x': 15,
+            'y': 10,
+        },
+        'Renderable': {
+            'fg': [255, 0, 255],
+        },
+        'Noun': {
+            'text': 'Test Object'
+        }
+    },
+    alias = 'test_object_01',
+)
+```
+
+Prefabs can specify other prefabs to inherit from as well. Prefabs can be defined as hierarchies of any depth and breadth. Note that properties will always be resolved from the most deeply embedded prefab to the least, overwriting with the most recent specification. If no properties are passed in the prefab or when creating from prefab, defaults from the component itself will be used.
 
+For examples, check out the `tests` folder in this repository.
 
-setup(**setup_kwargs)
```

