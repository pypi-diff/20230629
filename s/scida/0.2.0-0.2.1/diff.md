# Comparing `tmp/scida-0.2.0.tar.gz` & `tmp/scida-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scida-0.2.0.tar", max compression
+gzip compressed data, was "scida-0.2.1.tar", max compression
```

## Comparing `scida-0.2.0.tar` & `scida-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-06-20 17:16:51.245941 scida-0.2.0/LICENSE
--rw-r--r--   0        0        0     1665 2023-06-20 17:16:51.245941 scida-0.2.0/README.md
--rw-r--r--   0        0        0     1546 2023-06-20 17:16:51.257941 scida-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      391 2023-06-20 17:16:51.257941 scida-0.2.0/src/scida/__init__.py
--rw-r--r--   0        0        0     5752 2023-06-20 17:16:51.257941 scida-0.2.0/src/scida/config.py
--rw-r--r--   0        0        0        0 2023-06-20 17:16:51.257941 scida-0.2.0/src/scida/configfiles/__init__.py
--rw-r--r--   0        0        0      953 2023-06-20 17:16:51.257941 scida-0.2.0/src/scida/configfiles/config.yaml
--rw-r--r--   0        0        0     3198 2023-06-20 17:16:51.257941 scida-0.2.0/src/scida/configfiles/simulations.yaml
--rw-r--r--   0        0        0        0 2023-06-20 17:16:51.257941 scida-0.2.0/src/scida/configfiles/units/__init__.py
--rw-r--r--   0        0        0     3144 2023-06-20 17:16:51.257941 scida-0.2.0/src/scida/configfiles/units/eagle.yaml
--rw-r--r--   0        0        0      662 2023-06-20 17:16:51.257941 scida-0.2.0/src/scida/configfiles/units/gaia.yaml
--rw-r--r--   0        0        0       30 2023-06-20 17:16:51.257941 scida-0.2.0/src/scida/configfiles/units/general.yaml
--rw-r--r--   0        0        0     1319 2023-06-20 17:16:51.257941 scida-0.2.0/src/scida/configfiles/units/gizmo.yaml
--rw-r--r--   0        0        0     6118 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/configfiles/units/illustris.yaml
--rw-r--r--   0        0        0    11409 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/convenience.py
--rw-r--r--   0        0        0        0 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/customs/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/customs/arepo/__init__.py
--rw-r--r--   0        0        0    35045 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/customs/arepo/dataset.py
--rw-r--r--   0        0        0     2204 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/customs/arepo/series.py
--rw-r--r--   0        0        0      480 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/customs/gizmo/series.py
--rw-r--r--   0        0        0     1366 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/customs/rockstar/dataset.py
--rw-r--r--   0        0        0     3628 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/discovertypes.py
--rw-r--r--   0        0        0    11915 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/fields.py
--rw-r--r--   0        0        0     9055 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/helpers_hdf5.py
--rw-r--r--   0        0        0     2356 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/helpers_misc.py
--rw-r--r--   0        0        0    12540 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/interface.py
--rw-r--r--   0        0        0     5803 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/interfaces/gadgetstyle.py
--rw-r--r--   0        0        0      307 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/interfaces/mixins/__init__.py
--rw-r--r--   0        0        0       22 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/interfaces/mixins/base.py
--rw-r--r--   0        0        0     2434 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/interfaces/mixins/cosmology.py
--rw-r--r--   0        0        0     2360 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/interfaces/mixins/spatial.py
--rw-r--r--   0        0        0    14876 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/interfaces/mixins/units.py
--rw-r--r--   0        0        0    13398 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/io.py
--rw-r--r--   0        0        0     6142 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/misc.py
--rw-r--r--   0        0        0      221 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/registries.py
--rw-r--r--   0        0        0     9578 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/series.py
--rw-r--r--   0        0        0      314 2023-06-20 17:16:51.261941 scida-0.2.0/src/scida/utilities.py
--rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 scida-0.2.0/setup.py
--rw-r--r--   0        0        0     2565 1970-01-01 00:00:00.000000 scida-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-29 21:39:54.909294 scida-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1473 2023-06-29 21:39:54.909294 scida-0.2.1/README.md
+-rw-r--r--   0        0        0     1546 2023-06-29 21:39:54.917294 scida-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      391 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/__init__.py
+-rw-r--r--   0        0        0     5752 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/config.py
+-rw-r--r--   0        0        0        0 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/__init__.py
+-rw-r--r--   0        0        0      953 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/config.yaml
+-rw-r--r--   0        0        0     3198 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/simulations.yaml
+-rw-r--r--   0        0        0        0 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/__init__.py
+-rw-r--r--   0        0        0     3144 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/eagle.yaml
+-rw-r--r--   0        0        0      662 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/gaia.yaml
+-rw-r--r--   0        0        0       30 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/general.yaml
+-rw-r--r--   0        0        0     1319 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/gizmo.yaml
+-rw-r--r--   0        0        0     6118 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/illustris.yaml
+-rw-r--r--   0        0        0    11409 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/convenience.py
+-rw-r--r--   0        0        0        0 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/arepo/__init__.py
+-rw-r--r--   0        0        0    35081 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/arepo/dataset.py
+-rw-r--r--   0        0        0     2204 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/arepo/series.py
+-rw-r--r--   0        0        0      480 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/gizmo/series.py
+-rw-r--r--   0        0        0     1366 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/rockstar/dataset.py
+-rw-r--r--   0        0        0     3628 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/discovertypes.py
+-rw-r--r--   0        0        0    12114 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/fields.py
+-rw-r--r--   0        0        0     9055 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/helpers_hdf5.py
+-rw-r--r--   0        0        0     2356 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/helpers_misc.py
+-rw-r--r--   0        0        0    12540 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interface.py
+-rw-r--r--   0        0        0     5803 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/gadgetstyle.py
+-rw-r--r--   0        0        0      307 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/mixins/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/mixins/base.py
+-rw-r--r--   0        0        0     2419 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/mixins/cosmology.py
+-rw-r--r--   0        0        0     2360 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/mixins/spatial.py
+-rw-r--r--   0        0        0    15238 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/mixins/units.py
+-rw-r--r--   0        0        0    13618 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/io.py
+-rw-r--r--   0        0        0     6144 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/misc.py
+-rw-r--r--   0        0        0      221 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/registries.py
+-rw-r--r--   0        0        0     9772 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/series.py
+-rw-r--r--   0        0        0      314 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/utilities.py
+-rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 scida-0.2.1/setup.py
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 scida-0.2.1/PKG-INFO
```

### Comparing `scida-0.2.0/LICENSE` & `scida-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/pyproject.toml` & `scida-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "scida"
-version = "0.2.0"
+version = "0.2.1"
 description = "Convenience wrapper around large scientific datasets to process with dask."
 authors = ["Chris Byrohl"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-numpy = "^1.18"
+numpy = "^1.21"
 dask = {extras = ["array", "dataframe", "distributed"], version = "^2023"}
 distributed = "^2023"
 h5py = "^3.7.0"
 zarr = "^v2.10.0"
 astropy = "^5.0"
 numba = "^0.56"
 pyyaml = ">=5.3.1"
```

### Comparing `scida-0.2.0/src/scida/config.py` & `scida-0.2.1/src/scida/config.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/configfiles/config.yaml` & `scida-0.2.1/src/scida/configfiles/config.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/configfiles/simulations.yaml` & `scida-0.2.1/src/scida/configfiles/simulations.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/configfiles/units/eagle.yaml` & `scida-0.2.1/src/scida/configfiles/units/eagle.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/configfiles/units/gaia.yaml` & `scida-0.2.1/src/scida/configfiles/units/gaia.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/configfiles/units/gizmo.yaml` & `scida-0.2.1/src/scida/configfiles/units/gizmo.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/configfiles/units/illustris.yaml` & `scida-0.2.1/src/scida/configfiles/units/illustris.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/convenience.py` & `scida-0.2.1/src/scida/convenience.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/customs/arepo/dataset.py` & `scida-0.2.1/src/scida/customs/arepo/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import warnings
 from typing import Dict, List, Optional, Union
 
 import dask
 import numpy as np
 from dask import array as da
 from dask import delayed
-from numba import jit, njit
-from numpy._typing import NDArray
+from numba import jit
+from numpy.typing import NDArray
 
 from scida.discovertypes import _determine_mixins
 from scida.fields import FieldContainer
 from scida.helpers_misc import computedecorator, get_args, get_kwargs, parse_humansize
 from scida.interface import Selector, create_MixinDataset
 from scida.interfaces.gadgetstyle import GadgetStyleSnapshot
 from scida.interfaces.mixins import SpatialCartesian3DMixin, UnitMixin
@@ -564,15 +564,15 @@
                 res[-1] = res[-1].item()
             continue
         arrchunks = [arr[o : offsets[i + 1]] for arr in arrs]
         res.append(func(*arrchunks))
     return np.array(res)
 
 
-@njit
+@jit(nopython=True)
 def get_hidx(gidx_start, gidx_count, celloffsets):
     """Get halo index of a given cell
 
     Parameters
     ----------
     gidx_start: integer
         The first unique integer ID for the first particle
@@ -635,15 +635,15 @@
         gidx,
         halocelloffsets,
         hvals,
         meta=np.array((), dtype=hvals.dtype),
     )
 
 
-@jit
+@jit(nopython=True)
 def get_shidx(
     gidx_start: int,
     gidx_count: int,
     celloffsets: NDArray[np.int64],
     shnumber,
     shcounts,
     shcellcounts,
@@ -735,15 +735,15 @@
         shnumber,
         shcounts,
         shcellcounts,
         meta=np.array((), dtype=np.int64),
     )
 
 
-@njit
+@jit(nopython=True)
 def get_shcounts_shcells(SubhaloGrNr, hlength):
     """Returns the number offset and count of subhalos per halo."""
     shcounts = np.zeros(hlength, dtype=np.int32)
     shnumber = np.zeros(hlength, dtype=np.int32)
     i = 0
     hid = 0
     hid_old = 0
```

### Comparing `scida-0.2.0/src/scida/customs/arepo/series.py` & `scida-0.2.1/src/scida/customs/arepo/series.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/customs/rockstar/dataset.py` & `scida-0.2.1/src/scida/customs/rockstar/dataset.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/discovertypes.py` & `scida-0.2.1/src/scida/discovertypes.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/fields.py` & `scida-0.2.1/src/scida/fields.py`

 * *Files 21% similar despite different names*

```diff
@@ -58,147 +58,150 @@
     ):
         if aliases is None:
             aliases = {}
         if fieldrecipes_kwargs is None:
             fieldrecipes_kwargs = {}
         self.aliases = aliases
         self.name = kwargs.pop("name", None)
-        self.fields: Dict[str, da.Array] = {}
-        self.fields.update(*args, **kwargs)
-        self.fieldrecipes = {}
+        self._fields: Dict[str, da.Array] = {}
+        self._fields.update(*args, **kwargs)
+        self._recipes = "bla"
+        self._fieldrecipes = {}
         self.fieldrecipes_kwargs = fieldrecipes_kwargs
         self.withunits = withunits
-        self.containers: Dict[
+        self._containers: Dict[
             str, FieldContainer
         ] = dict()  # other containers as subgroups
         if containers is not None:
             for k in containers:
                 self.add_container(k)
         self.internals = ["uid"]  # names of internal fields/groups
         self.parent = parent
 
     def info(self, level=0, name: Optional[str] = None) -> str:
         rep = ""
         length = self.fieldlength
         count = self.fieldcount
         if name is None:
             name = self.name
-        ncontainers = len(self.containers)
+        ncontainers = len(self._containers)
         statstrs = []
         if length is not None and length > 0:
             statstrs.append("fields: %i" % count)
             statstrs.append("entries: %i" % length)
         if ncontainers > 0:
             statstrs.append("containers: %i" % ncontainers)
         if len(statstrs) > 0:
             statstr = ", ".join(statstrs)
             rep += sprint((level + 1) * "+", name, "(%s)" % statstr)
-        for k in sorted(self.containers.keys()):
-            v = self.containers[k]
+        for k in sorted(self._containers.keys()):
+            v = self._containers[k]
             rep += v.info(level=level + 1)
         return rep
 
     def merge(self, collection, overwrite=True):
         if not isinstance(collection, FieldContainer):
             raise TypeError("Can only merge FieldContainers.")
         # TODO: support nested containers
-        for k in collection.containers:
-            if k not in self.containers:
-                self.containers[k] = FieldContainer(
+        for k in collection._containers:
+            if k not in self._containers:
+                self._containers[k] = FieldContainer(
                     fieldrecipes_kwargs=self.fieldrecipes_kwargs
                 )
             if overwrite:
-                c1 = self.containers[k]
-                c2 = collection.containers[k]
+                c1 = self._containers[k]
+                c2 = collection._containers[k]
             else:
-                c1 = collection.containers[k]
-                c2 = self.containers[k]
-            c1.fields.update(**c2.fields)
-            c1.fieldrecipes.update(**c2.fieldrecipes)
+                c1 = collection._containers[k]
+                c2 = self._containers[k]
+            c1._fields.update(**c2._fields)
+            c1._fieldrecipes.update(**c2._fieldrecipes)
 
     @property
     def fieldcount(self):
-        nrecipes = len(self.fieldrecipes)
-        nfields = len(self.fields)
-        ntot = nrecipes + nfields
+        rcps = set(self._fieldrecipes)
+        flds = set([k for k in self._fields if k not in self.internals])
+        ntot = len(rcps | flds)
         return ntot
 
     @property
     def fieldlength(self):
-        itr = iter(self.fields.values())
-        if len(self.fields) == 0:
+        itr = iter(self._fields.values())
+        if len(self._fields) == 0:
             return None
         first = next(itr)
-        if all(first.shape[0] == v.shape[0] for v in self.fields.values()):
+        if all(first.shape[0] == v.shape[0] for v in self._fields.values()):
             return first.shape[0]
         else:
             return None
 
-    # def keys(self) -> set:
-    #    # TODO: hacky; also know that we have not / can not write .items() right now
-    #    # which will lead to unintended behaviour down the line
-    #    return set(self.fields.keys()) | set(self.derivedfields.keys())
     def keys(
         self, withgroups=True, withrecipes=True, withinternal=False, withfields=True
     ):
         fieldkeys = []
         if withfields:
-            fieldkeys = list(self.fields.keys())
+            fieldkeys = list(self._fields.keys())
             if not withinternal:
                 for ikey in self.internals:
                     if ikey in fieldkeys:
                         fieldkeys.remove(ikey)
             if withrecipes:
-                recipekeys = self.fieldrecipes.keys()
+                recipekeys = self._fieldrecipes.keys()
                 fieldkeys = list(set(fieldkeys) | set(recipekeys))
         if withgroups:
-            groupkeys = self.containers.keys()
-            return list(set(fieldkeys) | set(groupkeys))
-        return fieldkeys
+            groupkeys = self._containers.keys()
+            fieldkeys = list(set(fieldkeys) | set(groupkeys))
+        return sorted(fieldkeys)
+
+    def items(self):
+        return ((k, self._getitem(k, evaluate_recipe=False)) for k in self.keys())
+
+    def values(self):
+        return (self._getitem(k, evaluate_recipe=False) for k in self.keys())
 
     def register_field(
         self,
         containernames=None,
         name: Optional[str] = None,
         description="",
         units=None,
     ):
         # we only construct field upon first call to it (default)
         # if to_containers, we register to the respective children containers
         containers = []
         if isinstance(containernames, list):
-            containers = [self.containers[c] for c in containernames]
+            containers = [self._containers[c] for c in containernames]
         elif containernames == "all":
-            containers = self.containers.values()
+            containers = self._containers.values()
         elif containernames is None:
             containers = [self]
         elif isinstance(containernames, str):  # just a single container as a string?
-            containers.append(self.containers[containernames])
+            containers.append(self._containers[containernames])
         else:
             raise ValueError("Unknown type.")
 
         def decorator(func, name=name, description=description, units=units):
             if name is None:
                 name = func.__name__
             for container in containers:
-                drvfields = container.fieldrecipes
+                drvfields = container._fieldrecipes
                 drvfields[name] = DerivedFieldRecipe(
                     name, func, description=description, units=units
                 )
             return func
 
         return decorator
 
     def __setitem__(self, key, value):
         if key in self.aliases:
             key = self.aliases[key]
         if isinstance(value, FieldContainer):
-            self.containers[key] = value
+            self._containers[key] = value
         else:
-            self.fields[key] = value
+            self._fields[key] = value
 
     def __getitem__(self, key):
         return self._getitem(key)
 
     def __iter__(self):
         return iter(self.keys())
 
@@ -207,16 +210,16 @@
         Return a string representation of the object.
         Returns
         -------
         str
         """
         txt = ""
         txt += "FieldContainer[containers=%s, fields=%s]" % (
-            len(self.containers),
-            len(self.fields),
+            len(self._containers),
+            self.fieldcount,
         )
         return txt
 
     @property
     def dataframe(self):
         return self.get_dataframe()
 
@@ -256,32 +259,36 @@
         ddf = dd.concat(dfs, axis=1)
         return ddf
 
     def add_alias(self, alias, name):
         self.aliases[alias] = name
 
     def add_container(self, key, **kwargs):
-        self.containers[key] = FieldContainer(
+        self._containers[key] = FieldContainer(
             fieldrecipes_kwargs=self.fieldrecipes_kwargs,
             withunits=self.withunits,
             parent=self,
             **kwargs,
         )
 
-    def _getitem(self, key, force_derived=False, update_dict=True):
+    def _getitem(
+        self, key, force_derived=False, update_dict=True, evaluate_recipe=True
+    ):
         if key in self.aliases:
             key = self.aliases[key]
-        if key in self.containers:
-            return self.containers[key]
-        if key in self.fields and not force_derived:
-            return self.fields[key]
+        if key in self._containers:
+            return self._containers[key]
+        if key in self._fields and not force_derived:
+            return self._fields[key]
         else:
-            if key in self.fieldrecipes:
-                func = self.fieldrecipes[key].func
-                units = self.fieldrecipes[key].units
+            if key in self._fieldrecipes:
+                if not evaluate_recipe:
+                    return self._fieldrecipes[key]
+                func = self._fieldrecipes[key].func
+                units = self._fieldrecipes[key].units
                 accept_kwargs = inspect.getfullargspec(func).varkw is not None
                 func_kwargs = get_kwargs(func)
                 dkwargs = self.fieldrecipes_kwargs
                 # first, we overwrite all optional arguments with class instance defaults where func kwarg is None
                 kwargs = {
                     k: dkwargs[k]
                     for k in (
@@ -299,29 +306,29 @@
                         }
                     )
                 # finally, instantiate field
                 field = func(self, **kwargs)
                 if self.withunits and units is not None:
                     field = field * units
                 if update_dict:
-                    self.fields[key] = field
+                    self._fields[key] = field
                 return field
             else:
                 raise KeyError("Unknown field '%s'" % key)
 
     def __delitem__(self, key):
-        if key in self.fieldrecipes:
-            del self.fieldrecipes[key]
-        del self.fields[key]
+        if key in self._fieldrecipes:
+            del self._fieldrecipes[key]
+        del self._fields[key]
 
     def __len__(self):
         return len(self.keys())
 
     def get(self, key, value=None, allow_derived=True, force_derived=False):
-        if key in self.fieldrecipes and not allow_derived:
+        if key in self._fieldrecipes and not allow_derived:
             raise KeyError("Field '%s' is derived (allow_derived=False)" % key)
         else:
             try:
                 return self._getitem(
                     key, force_derived=force_derived, update_dict=False
                 )
             except KeyError:
```

### Comparing `scida-0.2.0/src/scida/helpers_hdf5.py` & `scida-0.2.1/src/scida/helpers_hdf5.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/helpers_misc.py` & `scida-0.2.1/src/scida/helpers_misc.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/interface.py` & `scida-0.2.1/src/scida/interface.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/interfaces/gadgetstyle.py` & `scida-0.2.1/src/scida/interfaces/gadgetstyle.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/interfaces/mixins/cosmology.py` & `scida-0.2.1/src/scida/interfaces/mixins/cosmology.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
 import numpy as np
 
 from scida.helpers_misc import sprint
 from scida.interfaces.mixins.base import Mixin
+from scida.interfaces.mixins.units import ignore_warn_redef
 
 log = logging.getLogger(__name__)
 
 
 class CosmologyMixin(Mixin):
     def __init__(self, *args, **kwargs):
         self.metadata = {}
@@ -16,22 +17,20 @@
         c = get_cosmology_from_rawmetadata(metadata_raw)
         self.cosmology = c
         z = get_redshift_from_rawmetadata(metadata_raw)
         self.redshift = z
         self.metadata["redshift"] = self.redshift
         if hasattr(self, "ureg"):
             ureg = self.ureg
-            backupval = ureg._on_redefinition
-            ureg._on_redefinition = "ignore"
-            if c is not None:
-                ureg.define("h = %s" % str(c.h))
-            if z is not None:
-                a = 1.0 / (1.0 + z)
-                ureg.define("a = %s" % str(float(a)))
-            ureg._on_redefinition = backupval
+            with ignore_warn_redef(ureg):
+                if c is not None:
+                    ureg.define("h = %s" % str(c.h))
+                if z is not None:
+                    a = 1.0 / (1.0 + z)
+                    ureg.define("a = %s" % str(float(a)))
 
     def _info_custom(self):
         rep = sprint("=== Cosmological Simulation ===")
         if self.redshift is not None:
             rep += sprint("z = %.2f" % self.redshift)
         if self.cosmology is not None:
             rep += sprint("cosmology =", str(self.cosmology))
```

### Comparing `scida-0.2.0/src/scida/interfaces/mixins/spatial.py` & `scida-0.2.1/src/scida/interfaces/mixins/spatial.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.0/src/scida/interfaces/mixins/units.py` & `scida-0.2.1/src/scida/interfaces/mixins/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import logging
 from typing import Optional
 
 import numpy as np
 import pint
 from pint import UnitRegistry
 
@@ -157,19 +158,23 @@
         if require:
             raise ValueError("Could not find explicit units nor cgs-factor.")
     if require:
         raise ValueError("Could not find units.")
     return str_to_unit("", ureg)
 
 
-def update_unitregistry_fromdict(udict: dict, ureg: UnitRegistry):
+def update_unitregistry_fromdict(udict: dict, ureg: UnitRegistry, warn_redef=False):
     ulist = []
     for k, v in udict.items():
         ulist.append("%s = %s" % (k, v))
-    ureg.load_definitions(ulist)
+    if warn_redef:
+        ureg.load_definitions(ulist)
+    else:
+        with ignore_warn_redef(ureg):
+            ureg.load_definitions(ulist)
 
 
 def update_unitregistry(filepath: str, ureg: UnitRegistry):
     conf = get_config_fromfile(filepath).get("units", {})
     update_unitregistry_fromdict(conf, ureg)
 
 
@@ -323,16 +328,16 @@
                         udict[p] = {}
                     udict = udict[p]
                 udict[k] = unit
                 # redefine dask arrays with units
                 # we treat recipes separately so that they stay recipes
                 # this is important due to the following memory issue for now:
                 # as we run into a memory issue (https://github.com/h5py/h5py/issues/2220)
-                if k not in container.fields and k in container.fieldrecipes:
-                    container.fieldrecipes[k].units = unit
+                if k not in container._fields and k in container._fieldrecipes:
+                    container._fieldrecipes[k].units = unit
                     # TODO: Add cgs conversion for recipes, see else-statement.
                 else:
                     container[k] = unit * container[k]
                     if units == "cgs" and isinstance(container[k], pint.Quantity):
                         container[k] = container[k].to_base_units()
 
         # fwu = unithints.get("fields", {})
@@ -365,7 +370,17 @@
     #        def handler_field(entry, newpath, parent=None):
     #            key = pathlib.Path(newpath).name
     #            cntr = get_container_from_path(newpath, newcontainer, create_missing=True)
     #            cntr[key] = parent[key].magnitude
     #            print(entry, newpath, parent)
     #        walk_container(self.data, handler_field=handler_field)
     #    super().save(*args, fields=newcontainer, **kwargs)
+
+
+@contextlib.contextmanager
+def ignore_warn_redef(ureg):
+    backupval = ureg._on_redefinition
+    ureg._on_redefinition = "ignore"
+    try:
+        yield
+    finally:
+        ureg._on_redefinition = backupval
```

### Comparing `scida-0.2.0/src/scida/io.py` & `scida-0.2.1/src/scida/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Optional
 
 import dask.array as da
 import h5py
 import numpy as np
 import zarr
 
+from scida.config import get_config
 from scida.fields import FieldContainer, walk_container
 from scida.helpers_hdf5 import create_mergedhdf5file, walk_hdf5file, walk_zarrfile
 from scida.misc import get_container_from_path, return_hdf5cachepath
 
 log = logging.getLogger(__name__)
 
 
@@ -202,14 +203,18 @@
             raise ValueError(msg)
         nmbrs = [int(f.split(".")[-2]) for f in files]
         sortidx = np.argsort(nmbrs)
         files = files[sortidx]
         return files
 
     def create_cachefile(self, fileprefix="", virtualcache=False):
+        config = get_config()
+        print_msg = config.get("print_cachefile_creation", True)
+        if print_msg:
+            print("Creating cache file, this may take a while...")
         cachefp = return_hdf5cachepath(self.path)
         files = self.get_chunkedfiles(fileprefix)
 
         self.location = cachefp
         if cachefp is None:
             # no filepath available
             self.tempfile = tempfile.NamedTemporaryFile("wb", suffix=".hdf5")
```

### Comparing `scida-0.2.0/src/scida/misc.py` & `scida-0.2.1/src/scida/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     element: str, container: FieldContainer = None, create_missing: bool = False
 ) -> FieldContainer:
     keys = element.split("/")
     rv = container
     for key in keys:
         if key == "":
             continue
-        if key not in rv.containers:
+        if key not in rv._containers:
             if not create_missing:
                 raise ValueError("Container '%s' not found in '%s'" % (key, rv))
             rv.add_container(key, name=key)
-        rv = rv.containers[key]
+        rv = rv._containers[key]
     return rv
 
 
 def return_hdf5cachepath(path_original) -> str:
     fp = return_cachefile_path(os.path.join(hash_path(path_original), "data.hdf5"))
     return fp
```

### Comparing `scida-0.2.0/src/scida/series.py` & `scida-0.2.1/src/scida/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,25 @@
         def __init__(self, *args, **kwargs):
             self._args = args
             self._kwargs = kwargs
 
         def __getattribute__(self, name):
             """Replace the class with the actual class and initialize it if needed."""
             # a few special calls do not trigger initialization:
-            if name in [
+            specialattrs = [
                 "__repr__",
                 "__str__",
                 "__dir__",
                 "__class__",
                 "_args",
                 "_kwargs",
-            ]:
+                # https://github.com/jupyter/notebook/issues/2014
+                "_ipython_canary_method_should_not_exist_",
+            ]
+            if name in specialattrs or name.startswith("_repr"):
                 return object.__getattribute__(self, name)
             elif hasattr(cls, name) and inspect.ismethod(getattr(cls, name)):
                 # do not need to initialize for class methods
                 return getattr(cls, name)
             arg = self._args
             kwarg = self._kwargs
             self.__class__ = cls
```

### Comparing `scida-0.2.0/setup.py` & `scida-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 install_requires = \
 ['astropy>=5.0,<6.0',
  'dask[array,dataframe,distributed]>=2023,<2024',
  'distributed>=2023,<2024',
  'h5py>=3.7.0,<4.0.0',
  'jupyter>=1.0.0,<2.0.0',
  'numba>=0.56,<0.57',
- 'numpy>=1.18,<2.0',
+ 'numpy>=1.21,<2.0',
  'pint>=0.22,<0.23',
  'pyyaml>=5.3.1',
  'requests>=2.31.0,<3.0.0',
  'tqdm>=4.64.1,<5.0.0',
  'zarr>=v2.10.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'scida',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Convenience wrapper around large scientific datasets to process with dask.',
-    'long_description': "# scida\n\n![test status](https://github.com/cbyrohl/scida/actions/workflows/tests.yml/badge.svg)\n\nscida is an out-of-the-box analysis tool for large scientific datasets. It primarily supports the astrophysics community, focusing on cosmological and galaxy formation simulations using particles or unstructured meshes, as well as large observational datasets.\nThis tool uses dask, allowing analysis to scale up from your personal computer to HPC resources and the cloud.\n\n## Features\n\n- Unified, high-level interface to load and analyze large datasets from a variety of sources.\n- Parallel, task-based data processing with dask arrays.\n- Physical unit support via pint.\n- Easily extensible architecture.\n\n## Requirements\n\n- Python >= 3.9\n\n\n## Documentation\nThe documentation can be found [here](https://cbyrohl.github.io/scida/)\n\n## Install\nFor now, do a  git clone of this repository:\n\n```\ngit clone https://github.com/cbyrohl/scida\ncd scida\npip install .\n```\n\n\n## First Steps\nStart up a Jupyter notebook server and begin with the 'Getting Started' section of the documentation. You can also find the underlying notebook [here](docs/notebooks/gettingstarted.ipynb).\n\n## License\n\nDistributed under the terms of the [MIT license](LICENSE),\n_scida_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue](https://github.com/cbyrohl/scida/issues/new) along with a detailed description.\n\n## Acknowledgements\n\nThe project structure was adapted from [Wolt](https://github.com/woltapp/wolt-python-package-cookiecutter) and [Hypermodern Python](https://github.com/cjolowicz/cookiecutter-hypermodern-python) cookiecutter templates.\n",
+    'long_description': '# scida\n\n![test status](https://github.com/cbyrohl/scida/actions/workflows/tests.yml/badge.svg)\n\nscida is an out-of-the-box analysis tool for large scientific datasets. It primarily supports the astrophysics community, focusing on cosmological and galaxy formation simulations using particles or unstructured meshes, as well as large observational datasets.\nThis tool uses dask, allowing analysis to scale up from your personal computer to HPC resources and the cloud.\n\n## Features\n\n- Unified, high-level interface to load and analyze large datasets from a variety of sources.\n- Parallel, task-based data processing with dask arrays.\n- Physical unit support via pint.\n- Easily extensible architecture.\n\n## Requirements\n\n- Python >= 3.9\n\n\n## Documentation\nThe documentation can be found [here](https://cbyrohl.github.io/scida/).\n\n## Install\n\n```\npip install scida\n```\n\n## First Steps\nAfter installing scida, follow the [tutorial](https://cbyrohl.github.io/scida/tutorial/).\n\n## License\n\nDistributed under the terms of the [MIT license](LICENSE),\n_scida_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue](https://github.com/cbyrohl/scida/issues/new) along with a detailed description.\n\n## Acknowledgements\n\nThe project structure was adapted from [Wolt](https://github.com/woltapp/wolt-python-package-cookiecutter) and [Hypermodern Python](https://github.com/cjolowicz/cookiecutter-hypermodern-python) cookiecutter templates.\n',
     'author': 'Chris Byrohl',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `scida-0.2.0/PKG-INFO` & `scida-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: scida
-Version: 0.2.0
+Version: 0.2.1
 Summary: Convenience wrapper around large scientific datasets to process with dask.
 Author: Chris Byrohl
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astropy (>=5.0,<6.0)
 Requires-Dist: dask[array,dataframe,distributed] (>=2023,<2024)
 Requires-Dist: distributed (>=2023,<2024)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: numba (>=0.56,<0.57)
-Requires-Dist: numpy (>=1.18,<2.0)
+Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: pint (>=0.22,<0.23)
 Requires-Dist: pyyaml (>=5.3.1)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: zarr (>=v2.10.0,<3.0.0)
 Description-Content-Type: text/markdown
 
@@ -38,28 +38,24 @@
 
 ## Requirements
 
 - Python >= 3.9
 
 
 ## Documentation
-The documentation can be found [here](https://cbyrohl.github.io/scida/)
+The documentation can be found [here](https://cbyrohl.github.io/scida/).
 
 ## Install
-For now, do a  git clone of this repository:
 
 ```
-git clone https://github.com/cbyrohl/scida
-cd scida
-pip install .
+pip install scida
 ```
 
-
 ## First Steps
-Start up a Jupyter notebook server and begin with the 'Getting Started' section of the documentation. You can also find the underlying notebook [here](docs/notebooks/gettingstarted.ipynb).
+After installing scida, follow the [tutorial](https://cbyrohl.github.io/scida/tutorial/).
 
 ## License
 
 Distributed under the terms of the [MIT license](LICENSE),
 _scida_ is free and open source software.
 
 ## Issues
```

