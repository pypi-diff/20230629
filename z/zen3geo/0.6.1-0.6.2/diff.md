# Comparing `tmp/zen3geo-0.6.1.tar.gz` & `tmp/zen3geo-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen3geo-0.6.1.tar", max compression
+gzip compressed data, was "zen3geo-0.6.2.tar", max compression
```

## Comparing `zen3geo-0.6.1.tar` & `zen3geo-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     7652 2023-05-31 05:14:08.491117 zen3geo-0.6.1/LICENSE.md
--rw-r--r--   0        0        0      826 2023-05-31 05:14:08.491117 zen3geo-0.6.1/README.md
--rw-r--r--   0        0        0     2912 2023-05-31 05:14:29.288022 zen3geo-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      207 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/__init__.py
--rw-r--r--   0        0        0     1050 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/__init__.py
--rw-r--r--   0        0        0    15274 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/datashader.py
--rw-r--r--   0        0        0     7162 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/geopandas.py
--rw-r--r--   0        0        0     3350 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/pyogrio.py
--rw-r--r--   0        0        0     3395 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/pystac.py
--rw-r--r--   0        0        0     5153 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/pystac_client.py
--rw-r--r--   0        0        0     2723 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/rioxarray.py
--rw-r--r--   0        0        0     7123 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/stackstac.py
--rw-r--r--   0        0        0     3899 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/xbatcher.py
--rw-r--r--   0        0        0     5323 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/xpystac.py
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 zen3geo-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-29 08:04:47.187026 zen3geo-0.6.2/LICENSE.md
+-rw-r--r--   0        0        0      826 2023-06-29 08:04:47.187026 zen3geo-0.6.2/README.md
+-rw-r--r--   0        0        0     2912 2023-06-29 08:05:06.939225 zen3geo-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-06-29 08:04:47.191027 zen3geo-0.6.2/zen3geo/__init__.py
+-rw-r--r--   0        0        0     1110 2023-06-29 08:04:47.191027 zen3geo-0.6.2/zen3geo/datapipes/__init__.py
+-rw-r--r--   0        0        0    15274 2023-06-29 08:04:47.191027 zen3geo-0.6.2/zen3geo/datapipes/datashader.py
+-rw-r--r--   0        0        0     7162 2023-06-29 08:04:47.195026 zen3geo-0.6.2/zen3geo/datapipes/geopandas.py
+-rw-r--r--   0        0        0     3350 2023-06-29 08:04:47.195026 zen3geo-0.6.2/zen3geo/datapipes/pyogrio.py
+-rw-r--r--   0        0        0     3421 2023-06-29 08:04:47.195026 zen3geo-0.6.2/zen3geo/datapipes/pystac.py
+-rw-r--r--   0        0        0     8925 2023-06-29 08:04:47.195026 zen3geo-0.6.2/zen3geo/datapipes/pystac_client.py
+-rw-r--r--   0        0        0     2723 2023-06-29 08:04:47.195026 zen3geo-0.6.2/zen3geo/datapipes/rioxarray.py
+-rw-r--r--   0        0        0     7123 2023-06-29 08:04:47.195026 zen3geo-0.6.2/zen3geo/datapipes/stackstac.py
+-rw-r--r--   0        0        0     3899 2023-06-29 08:04:47.195026 zen3geo-0.6.2/zen3geo/datapipes/xbatcher.py
+-rw-r--r--   0        0        0     5323 2023-06-29 08:04:47.195026 zen3geo-0.6.2/zen3geo/datapipes/xpystac.py
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 zen3geo-0.6.2/PKG-INFO
```

### Comparing `zen3geo-0.6.1/LICENSE.md` & `zen3geo-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.1/README.md` & `zen3geo-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.1/pyproject.toml` & `zen3geo-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zen3geo"
-version = "0.6.1"
+version = "0.6.2"
 description = "The 🌏 data science library you've been waiting for~"
 authors = ["Wei Ji <23487320+weiji14@users.noreply.github.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
@@ -95,9 +95,9 @@
 [tool.poetry-dynamic-versioning]
 bump = true
 enable = true
 metadata = false
 style = "pep440"
 
 [build-system]
-requires = ["poetry-core>=1.5.0", "poetry-dynamic-versioning"]
+requires = ["poetry-core>=1.6.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `zen3geo-0.6.1/zen3geo/datapipes/__init__.py` & `zen3geo-0.6.2/zen3geo/datapipes/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 )
 from zen3geo.datapipes.geopandas import (
     GeoPandasRectangleClipperIterDataPipe as GeoPandasRectangleClipper,
 )
 from zen3geo.datapipes.pyogrio import PyogrioReaderIterDataPipe as PyogrioReader
 from zen3geo.datapipes.pystac import PySTACItemReaderIterDataPipe as PySTACItemReader
 from zen3geo.datapipes.pystac_client import (
+    PySTACAPIItemListerIterDataPipe as PySTACAPIItemLister,
     PySTACAPISearcherIterDataPipe as PySTACAPISearcher,
 )
 from zen3geo.datapipes.rioxarray import RioXarrayReaderIterDataPipe as RioXarrayReader
 from zen3geo.datapipes.stackstac import (
     StackSTACMosaickerIterDataPipe as StackSTACMosaicker,
     StackSTACStackerIterDataPipe as StackSTACStacker,
 )
```

### Comparing `zen3geo-0.6.1/zen3geo/datapipes/datashader.py` & `zen3geo-0.6.2/zen3geo/datapipes/datashader.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.1/zen3geo/datapipes/geopandas.py` & `zen3geo-0.6.2/zen3geo/datapipes/geopandas.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.1/zen3geo/datapipes/pyogrio.py` & `zen3geo-0.6.2/zen3geo/datapipes/pyogrio.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.1/zen3geo/datapipes/pystac.py` & `zen3geo-0.6.2/zen3geo/datapipes/pystac.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 
     kwargs : Optional
         Extra keyword arguments to pass to :py:meth:`pystac.Item.from_file`.
 
     Yields
     ------
     stac_item : pystac.Item
-        An :py:class:`pystac.Item` object containing the specific STACObject
-        implementation class represented in a JSON format.
+        A :py:class:`pystac.Item` object containing the specific
+        :py:class:`pystac.STACObject` implementation class represented in a
+        JSON format.
 
     Raises
     ------
     ModuleNotFoundError
         If ``pystac`` is not installed. See
         :doc:`install instructions for pystac <pystac:installation>`, (e.g. via
         ``pip install pystac``) before using this class.
```

### Comparing `zen3geo-0.6.1/zen3geo/datapipes/pystac_client.py` & `zen3geo-0.6.2/zen3geo/datapipes/pystac_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     >>> pystac_client = pytest.importorskip("pystac_client")
     ...
     >>> from torchdata.datapipes.iter import IterableWrapper
     >>> from zen3geo.datapipes import PySTACAPISearcher
     ...
     >>> # Peform STAC API query using DataPipe
     >>> query = dict(
-    ...     bbox=[174.5, -41.37, 174.9, -41.19],
+    ...     bbox=[174.5, -41.37, 174.9, -41.19],  # xmin, ymin, xmax, ymax
     ...     datetime=["2012-02-20T00:00:00Z", "2022-12-22T00:00:00Z"],
     ...     collections=["cop-dem-glo-30"],
     ... )
     >>> dp = IterableWrapper(iterable=[query])
     >>> dp_pystac_client = dp.search_for_pystac_item(
     ...     catalog_url="https://planetarycomputer.microsoft.com/api/stac/v1",
     ...     # modifier=planetary_computer.sign_inplace,
@@ -129,7 +129,105 @@
 
         for query in self.source_datapipe:
             search = catalog.search(**query)
             yield search
 
     def __len__(self) -> int:
         return len(self.source_datapipe)
+
+
+@functional_datapipe("list_pystac_items_by_search")
+class PySTACAPIItemListerIterDataPipe(IterDataPipe):
+    """
+    Lists the :py:class:`pystac.Item` objects that match the provided STAC API
+    search parameters (functional name: ``list_pystac_items_by_search``).
+
+    Parameters
+    ----------
+    source_datapipe : IterDataPipe[pystac_client.ItemSearch]
+        A DataPipe that contains :py:class:`pystac_client.ItemSearch` object
+        instances that represents
+        a deferred query to a STAC search endpoint as described in the
+        `STAC API - Item Search spec <https://github.com/radiantearth/stac-api-spec/tree/main/item-search>`_.
+
+    Yields
+    ------
+    stac_item : pystac.Item
+        A :py:class:`pystac.Item` object containing the specific
+        :py:class:`pystac.STACObject` implementation class represented in a
+        JSON format.
+
+    Raises
+    ------
+    ModuleNotFoundError
+        If ``pystac_client`` is not installed. See
+        :doc:`install instructions for pystac-client <pystac_client:index>`,
+        (e.g. via ``pip install pystac-client``) before using this class.
+
+    Example
+    -------
+    >>> import pytest
+    >>> pystac_client = pytest.importorskip("pystac_client")
+    ...
+    >>> from torchdata.datapipes.iter import IterableWrapper
+    >>> from zen3geo.datapipes import PySTACAPIItemLister
+    ...
+    >>> # List STAC Items from a STAC API query
+    >>> catalog = pystac_client.Client.open(
+    ...     url="https://explorer.digitalearth.africa/stac/"
+    ... )
+    >>> search = catalog.search(
+    ...     bbox=[57.2, -20.6, 57.9, -19.9],  # xmin, ymin, xmax, ymax
+    ...     datetime=["2023-01-01T00:00:00Z", "2023-01-31T00:00:00Z"],
+    ...     collections=["s2_l2a"],
+    ... )
+    >>> dp = IterableWrapper(iterable=[search])
+    >>> dp_pystac_item_list = dp.list_pystac_items_by_search()
+    ...
+    >>> # Loop or iterate over the DataPipe stream
+    >>> it = iter(dp_pystac_item_list)
+    >>> stac_item = next(it)
+    >>> stac_item
+    <Item id=ec16dbf6-9729-5a8f-9d72-5e83a8b9f30d>
+    >>> stac_item.properties  # doctest: +NORMALIZE_WHITESPACE
+    {'title': 'S2B_MSIL2A_20230103T062449_N0509_R091_T40KED_20230103T075000',
+     'gsd': 10,
+     'proj:epsg': 32740,
+     'platform': 'sentinel-2b',
+     'view:off_nadir': 0,
+     'instruments': ['msi'],
+     'eo:cloud_cover': 0.02,
+     'odc:file_format': 'GeoTIFF',
+     'odc:region_code': '40KED',
+     'constellation': 'sentinel-2',
+     'sentinel:sequence': '0',
+     'sentinel:utm_zone': 40,
+     'sentinel:product_id': 'S2B_MSIL2A_20230103T062449_N0509_R091_T40KED_20230103T075000',
+     'sentinel:grid_square': 'ED',
+     'sentinel:data_coverage': 28.61,
+     'sentinel:latitude_band': 'K',
+     'created': '2023-01-03T06:24:53Z',
+     'sentinel:valid_cloud_cover': True,
+     'sentinel:boa_offset_applied': True,
+     'sentinel:processing_baseline': '05.09',
+     'proj:shape': [10980, 10980],
+     'proj:transform': [10.0, 0.0, 499980.0, 0.0, -10.0, 7900000.0, 0.0, 0.0, 1.0],
+     'datetime': '2023-01-03T06:24:53Z',
+     'cubedash:region_code': '40KED'}
+    """
+
+    def __init__(self, source_datapipe):
+        if pystac_client is None:
+            raise ModuleNotFoundError(
+                "Package `pystac_client` is required to be installed to use this datapipe. "
+                "Please use `pip install pystac-client` or "
+                "`conda install -c conda-forge pystac-client` "
+                "to install the package"
+            )
+        self.source_datapipe = source_datapipe
+
+    def __iter__(self):
+        for item_search in self.source_datapipe:
+            yield from item_search.items()
+
+    def __len__(self):
+        return sum(item_search.matched() for item_search in self.source_datapipe)
```

### Comparing `zen3geo-0.6.1/zen3geo/datapipes/rioxarray.py` & `zen3geo-0.6.2/zen3geo/datapipes/rioxarray.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.1/zen3geo/datapipes/stackstac.py` & `zen3geo-0.6.2/zen3geo/datapipes/stackstac.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.1/zen3geo/datapipes/xbatcher.py` & `zen3geo-0.6.2/zen3geo/datapipes/xbatcher.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.1/zen3geo/datapipes/xpystac.py` & `zen3geo-0.6.2/zen3geo/datapipes/xpystac.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.1/PKG-INFO` & `zen3geo-0.6.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: zen3geo
-Version: 0.6.1
+Version: 0.6.2
 Summary: The 🌏 data science library you've been waiting for~
 License: LGPL-3.0-or-later
 Author: Wei Ji
 Author-email: 23487320+weiji14@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Provides-Extra: raster
 Provides-Extra: spatial
```

