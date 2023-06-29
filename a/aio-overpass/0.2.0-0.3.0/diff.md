# Comparing `tmp/aio_overpass-0.2.0.tar.gz` & `tmp/aio_overpass-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_overpass-0.2.0.tar", max compression
+gzip compressed data, was "aio_overpass-0.3.0.tar", max compression
```

## Comparing `aio_overpass-0.2.0.tar` & `aio_overpass-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1536 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/LICENSE
--rw-r--r--   0        0        0     8085 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/README.md
--rwxr-xr-x   0        0        0      316 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/__init__.py
--rw-r--r--   0        0        0      977 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/_dist.py
--rwxr-xr-x   0        0        0      971 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/_ql.py
--rwxr-xr-x   0        0        0    12078 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/client.py
--rwxr-xr-x   0        0        0    28970 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/element.py
--rwxr-xr-x   0        0        0    14083 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/error.py
--rwxr-xr-x   0        0        0    25071 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/pt.py
--rwxr-xr-x   0        0        0    22491 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/pt_ordered.py
--rwxr-xr-x   0        0        0    14772 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/query.py
--rwxr-xr-x   0        0        0     2614 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9466 1970-01-01 00:00:00.000000 aio_overpass-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2105 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/LICENSE
+-rw-r--r--   0        0        0    10286 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/README.md
+-rwxr-xr-x   0        0        0      316 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/__init__.py
+-rw-r--r--   0        0        0      977 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/_dist.py
+-rwxr-xr-x   0        0        0      971 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/_ql.py
+-rwxr-xr-x   0        0        0    12078 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/client.py
+-rwxr-xr-x   0        0        0    28972 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/element.py
+-rwxr-xr-x   0        0        0    14070 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/error.py
+-rwxr-xr-x   0        0        0    25082 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/pt.py
+-rwxr-xr-x   0        0        0    22661 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/pt_ordered.py
+-rwxr-xr-x   0        0        0    14918 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/query.py
+-rwxr-xr-x   0        0        0     3398 2023-06-29 13:54:31.106119 aio_overpass-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11866 1970-01-01 00:00:00.000000 aio_overpass-0.3.0/PKG-INFO
```

### Comparing `aio_overpass-0.2.0/CHANGELOG.md` & `aio_overpass-0.3.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
+## [0.3.0] - 2023-06-29
+* Drop Python 3.8 support. The Python versions supported by this release are 3.9-3.11.
+* Relaxed `networkx` dependency to `>=2.7` according to [SPEC 0]
+* Increased `joblib` dependency to `~1.3`, which makes it ready for Python 3.12 among other things
+* Fixed doc: `maxsize` is not megabytes, but mebibytes
+* `Query`: affected properties ending in `_mb` now end in `_mib`
+* Add a section on coordinates to the `README`
+
 <br>
 
 ## [0.2.0] - 2023-06-14
 * `QueryError`: `messages` was renamed to `remarks`
 * Add `QueryResponseError`, which is raised for unexpected query responses
   instead of `QueryError`
 * `QueryError` is now similar to `ClientError` in that only objects of
@@ -32,7 +40,10 @@
 * Fix wrong coordinate order in elements' GeoJSON `bbox`
 * Fix wrong repository link in `pyproject.toml`
 
 [0.1.1]: https://github.com/timwie/aio-overpass/releases/tag/v0.1.1
 [0.1.2]: https://github.com/timwie/aio-overpass/releases/tag/v0.1.2
 [0.1.2.post1]: https://github.com/timwie/aio-overpass/releases/tag/v0.1.2.post1
 [0.2.0]: https://github.com/timwie/aio-overpass/releases/tag/v0.2.0
+[0.3.0]: https://github.com/timwie/aio-overpass/releases/tag/v0.3.0
+
+[SPEC 0]: https://scientific-python.org/specs/spec-0000/
```

### Comparing `aio_overpass-0.2.0/LICENSE` & `aio_overpass-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.2.0/README.md` & `aio_overpass-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">
 aio-overpass
 
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/timwie/aio-overpass/ci.yml)](https://github.com/timwie/aio-overpass/actions/workflows/ci.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/timwie/aio-overpass/test_and_publish.yml)](https://github.com/timwie/aio-overpass/actions/workflows/test_and_publish.yml)
 [![codecov](https://codecov.io/gh/timwie/aio-overpass/branch/main/graph/badge.svg?token=YX1218U740)](https://codecov.io/gh/timwie/aio-overpass)
 [![PyPI version](https://badge.fury.io/py/aio_overpass.svg)](https://badge.fury.io/py/aio_overpass)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aio-overpass)
 </h1>
 
 A client for the [Overpass API], a read-only API that serves up custom selected
 parts of [OpenStreetMap] data. It is optimized for data consumers that need a few
@@ -16,14 +16,15 @@
 
 #### Contents
 - [Features](#features)
 - [Getting Started](#getting-started)
   - [Choosing Extras](#choosing-extras)
 - [Basic Usage](#basic-usage)
   - [Example](#example)
+- [Coordinates](#coordinates)
 - [Motivation](#motivation)
 - [Related Projects](#related-projects)
 - [License](#license)
 
 #### See also
 - An overview of modules, classes and functions can be found in the [API reference](http://www.timwie.dev/aio-overpass/).
 - The version history is available in [CHANGELOG.md](https://github.com/timwie/aio-overpass/blob/main/CHANGELOG.md).
@@ -189,14 +190,45 @@
         53.5416212,
     ]
 }
 ```
 
 <br>
 
+## Coordinates
+* Geographic point locations are expressed by latitude (`lat`) and longitude (`lon`) coordinates.
+  * Latitude is given as an angle that ranges from –90° at the south pole to 90° at the north pole,
+    with 0° at the Equator.
+  * Longitude is given as an angle ranging from 0° at the Prime Meridian (the line that divides the
+    globe into Eastern and Western hemispheres), to +180° eastward and −180° westward.
+  * `lat/lon` values are `floats` that are exactly those degrees, just without the ° sign.
+* This might help you remember which coordinate is which:
+  * If you think of a world map, usually it’s a rectangle.
+  * The _long_ side (the largest side) is the longitude.
+  * Longitude is the x-axis, and latitude is the y-axis.
+* Be wary of coordinate order:
+  * The Overpass API explicitly names the coordinates: `{ "lat": 50.2726005, "lon": 10.9521885 }`
+  * Shapely geometries returned by this library use `lat/lon` order, which is the order
+    stated by [ISO 6709], and seems like the most common order.
+  * [GeoJSON], on the other hand, uses `lon/lat` order.
+* OpenStreetMap uses the [WGS84] spatial reference system
+  used by the Global Positioning System (GPS).
+* OpenStreetMap node coordinates have seven decimal places, which gives them centimetric precision.
+  However, the position accuracy of GPS data is only [about 10m](https://wiki.openstreetmap.org/wiki/Reliability_of_OSM_coordinates).
+  A reasonable display accuracy could be five places, which is precise to
+  [1.1 metres](https://wiki.openstreetmap.org/wiki/Precision_of_coordinates)
+  at the equator.
+* Spatial features that cross the 180th meridian are
+  [problematic](https://en.wikipedia.org/wiki/180th_meridian#Software_representation_problems),
+  since you go from longitude `180.0` to `-180.0`.
+  Such features usually have their geometries split up, like the
+  [area of Russia](https://www.openstreetmap.org/relation/60189).
+
+<br>
+
 ## Motivation
 
 ### Goals
 - A small and stable set of core functionality.
 - Good defaults for queries and retrying.
 - Room for extensions that simplify querying and/or processing of spatial data
   in specific problem domains.
@@ -207,15 +239,15 @@
 - Any sort of Python interface to replace writing Overpass QL code.
 - Integrating other OSM-related services (like the OSM API or Nominatim)
 - Command line interface
 
 <br>
 
 ## Related Projects
-- [Overpass API](https://github.com/drolbr/Overpass-API)
+- [Overpass API](https://github.com/drolbr/Overpass-API), and the [Overpass API Blog]
 - [Overpass Turbo], the best choice to prototype your queries in a browser
 - [Folium], which can be used to visualize GeoJSON on [Leaflet] maps
 - [OSMnx], which is specialized on street networks
 - [overpass-api-python-wrapper], another Python client for the Overpass API
 - [overpy], another Python client for the Overpass API
 - [OSMPythonTools], a Python client for OSM-related services 
 - [overpassify], a Python to Overpass QL transpiler
@@ -223,14 +255,15 @@
 <br>
 
 ## License
 Distributed under the MIT License. See `LICENSE` for more information.
 
 
 [Overpass API]: https://wiki.openstreetmap.org/wiki/Overpass_API
+[Overpass API Blog]: https://dev.overpass-api.de/blog/
 [Overpass QL]: https://wiki.openstreetmap.org/wiki/Overpass_API/Overpass_QL
 [OpenStreetMap]: https://www.openstreetmap.org
 
 [Overpass Turbo]: http://overpass-turbo.eu/
 [Folium]: https://python-visualization.github.io/folium/
 [Leaflet]: https://leafletjs.com/
 [overpass-api-python-wrapper]: https://github.com/mvexel/overpass-api-python-wrapper
@@ -243,7 +276,10 @@
 [Joblib]: https://joblib.readthedocs.io/en/latest/
 [NetworkX]: https://networkx.github.io/
 [PyGeodesy]: https://mrjean1.github.io/PyGeodesy/
 [Shapely]: https://shapely.readthedocs.io/en/latest/manual.html
 
 [GeoJSON]: https://en.wikipedia.org/wiki/GeoJSON
 [WKT]: https://en.wikipedia.org/wiki/Well-known_text_representation_of_geometry
+
+[WGS84]: https://en.wikipedia.org/wiki/World_Geodetic_System
+[ISO 6709]: https://en.wikipedia.org/wiki/ISO_6709
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aio_overpass-0.2.0/aio_overpass/_dist.py` & `aio_overpass-0.3.0/aio_overpass/_dist.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.2.0/aio_overpass/_ql.py` & `aio_overpass-0.3.0/aio_overpass/_ql.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.2.0/aio_overpass/client.py` & `aio_overpass-0.3.0/aio_overpass/client.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.2.0/aio_overpass/element.py` & `aio_overpass-0.3.0/aio_overpass/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Typed result set members."""
 
 from abc import ABC, abstractmethod
 from collections import defaultdict
+from collections.abc import Iterable, Iterator
 from dataclasses import dataclass
-from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Type, Union, cast
+from typing import Any, Optional, Union, cast
 
 from aio_overpass import Query
 
 import shapely.geometry
 import shapely.ops
 from shapely.geometry import (
     GeometryCollection,
@@ -33,25 +34,25 @@
     "AreaWay",
     "AreaRelation",
     "Relationship",
     "Metadata",
     "collect_elements",
 )
 
-GeoJsonDict = Dict[str, Any]
+GeoJsonDict = dict[str, Any]
 """
 A dictionary representing a GeoJSON object.
 """
 
-OverpassDict = Dict[str, Any]
+OverpassDict = dict[str, Any]
 """
 A dictionary representing a JSON object returned by the Overpass API.
 """
 
-Bbox = Tuple[float, float, float, float]
+Bbox = tuple[float, float, float, float]
 """
 The bounding box of a spatial object.
 
 This tuple can be understood as any of 
     - ``(s, w, n, e)``
     - ``(minlat, minlon, maxlat, maxlon)``
     - ``(minx, miny, maxx, maxy)``
@@ -166,15 +167,15 @@
     """
 
     id: int
     tags: Optional[OverpassDict]
     bounds: Optional[Bbox]
     center: Optional[Point]
     meta: Optional[Metadata]
-    relations: List["Relationship"]
+    relations: list["Relationship"]
 
     def tag(self, key: str, default: Any = None) -> Any:
         """
         Get the tag value for the given key.
 
         Returns ``default`` if there is no ``key`` tag.
 
@@ -342,15 +343,15 @@
                   a Polygon if the way is closed and its tags indicate that it represents an area,
                   or ``None`` if the geometry is not included in the query's result set.
 
     References:
         - https://wiki.openstreetmap.org/wiki/Way
     """
 
-    node_ids: Optional[List[int]]
+    node_ids: Optional[list[int]]
     geometry: Union[LineString, LinearRing, None]
 
 
 @dataclass(repr=False, eq=False)
 class Relation(Element):
     """
     A relation is a group of nodes and ways that have a logical or geographic relationship,
@@ -361,17 +362,17 @@
     Attributes:
         members: Ordered member elements of this relation, with an optional role
 
     References:
         - https://wiki.openstreetmap.org/wiki/Relation
     """
 
-    members: List["Relationship"]
+    members: list["Relationship"]
 
-    def __iter__(self) -> Iterator[Tuple[Optional[str], Element]]:
+    def __iter__(self) -> Iterator[tuple[Optional[str], Element]]:
         for relship in self.members:
             yield relship.role, relship.member
 
 
 @dataclass(repr=False, eq=False)
 class AreaWay(Way):
     """
@@ -470,30 +471,30 @@
         role = f" as '{self.role}'" if self.role else " "
         return f"{type(self).__name__}({self.member}{role} in {self.relation})"
 
 
 _KNOWN_ELEMENTS = {"node", "way", "relation", "area"}
 
 
-_ElementKey = Tuple[str, int]
+_ElementKey = tuple[str, int]
 """Elements are uniquely identified by the tuple (type, id)."""
 
-_MemberKey = Tuple[_ElementKey, str]
+_MemberKey = tuple[_ElementKey, str]
 """Relation members are identified by their element key and role."""
 
 
 class _ElementCollector:
     def __init__(self) -> None:
-        self.list: List[Element] = []
-        self.typed_dict: Dict[_ElementKey, Element] = {}
-        self.untyped_dict: Dict[_ElementKey, OverpassDict] = defaultdict(dict)
-        self.member_dict: Dict[int, List[_MemberKey]] = defaultdict(list)
+        self.list: list[Element] = []
+        self.typed_dict: dict[_ElementKey, Element] = {}
+        self.untyped_dict: dict[_ElementKey, OverpassDict] = defaultdict(dict)
+        self.member_dict: dict[int, list[_MemberKey]] = defaultdict(list)
 
 
-def collect_elements(query: Query) -> List[Element]:
+def collect_elements(query: Query) -> list[Element]:
     """
     Produce typed elements from the result set of a query.
 
     This function collects elements that are of type "node", "way", "relation", or "area".
     Derived elements with other types - f.e. produced by ``make`` and ``convert`` statements
     or when using ``out count`` - are ignored. An exception is made for areas, which are so
     closely derived from ways and relations that it makes sense to represent them as such.
@@ -570,15 +571,15 @@
                 user_id=elem_dict["uid"],
             )
             if "timestamp" in elem_dict
             else None,
             relations=[],  # add later
         )
 
-        cls: Type[Element]
+        cls: type[Element]
 
         if elem_type == "node":
             cls = Node
 
         elif elem_type == "way":
             cls = Way
             args["node_ids"] = elem_dict.get("nodes")
```

### Comparing `aio_overpass-0.2.0/aio_overpass/error.py` & `aio_overpass-0.3.0/aio_overpass/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import html
 import re
 from dataclasses import dataclass
 from enum import Enum, auto
 from json import JSONDecodeError
-from typing import List, Optional, Tuple, Union, no_type_check
+from typing import Optional, Union, no_type_check
 
 import aiohttp
 import aiohttp.typedefs
 
 
 __docformat__ = "google"
 __all__ = (
@@ -96,15 +96,15 @@
 
     This error is raised when a request fails, but we can't specifically say why.
     This may indicate a bug on our end, since the client is meant to process almost any
     response of an Overpass API instance.
     """
 
     request_info: aiohttp.RequestInfo
-    history: Tuple[aiohttp.ClientResponse, ...]
+    history: tuple[aiohttp.ClientResponse, ...]
     status: int
     message: str
     headers: Optional[aiohttp.typedefs.LooseHeaders]
 
     @property
     def response(self) -> aiohttp.ClientResponse:
         return self.history[-1]
@@ -146,15 +146,15 @@
 
     Attributes:
         kwargs: the query's ``kwargs``
         remarks: the error remarks provided by the API
     """
 
     kwargs: dict
-    remarks: List[str]
+    remarks: list[str]
 
     def __str__(self) -> str:
         if self.kwargs:
             query = f"query {self.kwargs}"
         else:
             query = "query <no kwargs>"
 
@@ -440,15 +440,15 @@
         message=str(response.reason) if response.reason else "",
         headers=response.headers,
     )
 
 
 def _query_response_error(
     kwargs: dict,
-    remarks: List[str],
+    remarks: list[str],
     response: aiohttp.ClientResponse,
 ) -> QueryResponseError:
     return QueryResponseError(
         kwargs=kwargs,
         remarks=remarks,
         request_info=response.request_info,
         history=response.history,
```

### Comparing `aio_overpass-0.2.0/aio_overpass/pt.py` & `aio_overpass-0.3.0/aio_overpass/pt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Classes and queries specialized on public transportation routes.
 """
 
 from collections import Counter
+from collections.abc import Generator
 from dataclasses import dataclass
 from enum import Enum, auto
-from typing import Any, Generator, List, Optional, Set, Union, cast
+from typing import Any, Optional, Union, cast
 
 from aio_overpass._dist import fast_distance
 from aio_overpass._ql import one_of_filter, poly_filter
 from aio_overpass.element import (
     Bbox,
     GeoJsonDict,
     Node,
@@ -118,15 +119,15 @@
                  of coordinates on the exterior will slow down the query.
         vehicles: A list of transportation modes to filter by, or an empty list to include
                   routes of any type. A non-empty list will filter routes by the ``route``
                   key.
     """
 
     def __init__(
-        self, polygon: Polygon, vehicles: Optional[List["Vehicle"]] = None, **kwargs
+        self, polygon: Polygon, vehicles: Optional[list["Vehicle"]] = None, **kwargs
     ) -> None:
         if not vehicles:
             vehicles = list(Vehicle)
 
         self.polygon = polygon
         self.vehicles = vehicles
 
@@ -232,15 +233,15 @@
             _connection(relship) for relship in (self.stop_position, self.platform) if relship
         ]
         return next(
             (opt for opt in options if opt != Connection.ENTRY_AND_EXIT), Connection.ENTRY_AND_EXIT
         )
 
     @property
-    def stop_areas(self) -> Set[Relation]:
+    def stop_areas(self) -> set[Relation]:
         """Any stop area related to this stop."""
         return {
             relship_to_stop_area.relation
             for relship_to_route in (self.platform, self.stop_position)
             if relship_to_route
             for relship_to_stop_area in relship_to_route.member.relations
             if relship_to_stop_area.relation.tag("public_transport") == "stop_area"
@@ -366,15 +367,15 @@
     References:
         - https://wiki.openstreetmap.org/wiki/Public_transport
         - https://wiki.openstreetmap.org/wiki/Relation:route#Public_transport_routes
     """
 
     relation: Relation
     scheme: RouteScheme
-    stops: List[Stop]
+    stops: list[Stop]
 
     @property
     def id(self) -> int:
         """Route relation ID."""
         return self.relation.id
 
     @property
@@ -389,15 +390,15 @@
 
         masters = self.masters
         master = masters[0] if len(masters) == 1 else None
 
         if master and master.tags is not None:
             from_master = {k: v for k, v in master.tags.items() if k in _TAGS_FROM_ROUTE_MASTER}
 
-        return {**from_master, **from_relation}
+        return from_master | from_relation
 
     def tag(self, key: str, default: Any = None) -> Any:
         """
         Get the tag value for the given key.
 
         Some tags can be inherited from a route master, if not set already.
         """
@@ -413,29 +414,29 @@
 
         if not master:
             return default
 
         return master.tag(key, default)
 
     @property
-    def ways(self) -> List[Way]:
+    def ways(self) -> list[Way]:
         """
         The ways making up the path of the route.
 
         Ways may be ordered, and appear multiple times if a way is travelled on more than once.
         All the ways may be contiguous, but gaps are not uncommon.
         """
         return [
             relship.member
             for relship in self.relation.members
             if isinstance(relship.member, Way) and _role(relship) == _RouteRole.NONE
         ]
 
     @property
-    def masters(self) -> List[Relation]:
+    def masters(self) -> list[Relation]:
         """
         Route master relations this route is a part of.
 
         By convention, this should be a single relation at most.
 
         References:
             - https://wiki.openstreetmap.org/wiki/Relation:route_master
@@ -550,15 +551,15 @@
 in order to avoid duplication.
 
 References:
     - https://wiki.openstreetmap.org/wiki/Relation:route_master 
 """
 
 
-def collect_routes(query: RouteQuery, perimeter: Optional[Polygon] = None) -> List[Route]:
+def collect_routes(query: RouteQuery, perimeter: Optional[Polygon] = None) -> list[Route]:
     # TODO the way 'perimeter' works might be confusing
     """
     Consumes the result set of a query and produces ``Route`` objects.
 
     The order of elements is *not* retained.
 
     The result set in the input query will be empty after calling this function.
```

### Comparing `aio_overpass-0.2.0/aio_overpass/pt_ordered.py` & `aio_overpass-0.3.0/aio_overpass/pt_ordered.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Collect the routes of a ``RouteQuery`` with optimized geometry.
 """
 
 import itertools
+from collections.abc import Generator
 from dataclasses import dataclass, replace
-from typing import Any, Callable, Generator, List, Optional, Tuple, Union, cast
+from typing import Any, Callable, Optional, Union, cast
 
 from aio_overpass._dist import fast_distance
 from aio_overpass.element import GeoJsonDict, Node, Relation, Relationship, Spatial, Way
 
 import networkx as nx
 import shapely.ops
 from networkx import MultiDiGraph
@@ -69,15 +70,15 @@
     Attributes:
         route: The viewed route.
         ordering: The visited nodes while trying to walk the shortest paths between pairs of stops,
                   ordered from start to finish. This is an empty list if this is an empty view.
     """
 
     route: Route
-    ordering: List[OrderedRouteViewNode]
+    ordering: list[OrderedRouteViewNode]
 
     @property
     def is_continuous(self) -> bool:
         """
         True if there's a path between all stops on the route.
 
         False for empty views.
@@ -90,15 +91,15 @@
         sequence_actual = [n for n, _grp in grouped]
         sequence_continuous = list(range(min(sequence_actual), max(sequence_actual) + 1))
 
         # True if 'path_idx' never skips any stop when iterating 'ordering'
         return sequence_actual == sequence_continuous
 
     @property
-    def stops(self) -> List[Stop]:
+    def stops(self) -> list[Stop]:
         """All stops of this view where a path either starts or ends."""
         if not self.ordering:
             return []
 
         has_path_to_idx = {node.n_seen_stops for node in self.ordering}
         has_path_from_idx = {node.n_seen_stops - 1 for node in self.ordering}
         indexes = has_path_to_idx | has_path_from_idx
@@ -107,34 +108,34 @@
 
     def _split(
         self, predicate: Callable[[OrderedRouteViewNode, OrderedRouteViewNode], bool]
     ) -> Generator["OrderedRouteView", None, None]:
         if len(self.ordering) < 2:
             return
 
-        ordering: List[OrderedRouteViewNode] = []
+        ordering: list[OrderedRouteViewNode] = []
 
         for a, b in zip(self.ordering, self.ordering[1:]):
             if predicate(a, b):
                 yield replace(self, ordering=ordering)
                 ordering = [a]
             else:
                 ordering.append(a)
 
         ordering.append(b)
         yield replace(self, ordering=ordering)
 
-    def _group_by(self, key: Callable[[OrderedRouteViewNode], Any]) -> List["OrderedRouteView"]:
+    def _group_by(self, key: Callable[[OrderedRouteViewNode], Any]) -> list["OrderedRouteView"]:
         return list(self._split(predicate=lambda a, b: key(a) != key(b)))
 
-    def gap_split(self) -> List["OrderedRouteView"]:
+    def gap_split(self) -> list["OrderedRouteView"]:
         """Split this view wherever there's a gap in between stops."""
         return list(self._split(predicate=lambda a, b: b.path_idx > a.path_idx + 1))
 
-    def stop_split(self) -> List["OrderedRouteView"]:
+    def stop_split(self) -> list["OrderedRouteView"]:
         """Split this view at every stop, returning views between every pair of stops."""
         return self._group_by(key=lambda node: node.path_idx)
 
     def take(self, first_n: int) -> "OrderedRouteView":
         """
         Returns the continuous view that connects a maximum number of stops at the beginning.
         """
@@ -157,41 +158,41 @@
         """
         pre_gap, *_ = self.gap_split()
 
         distance_start = pre_gap.ordering[0].distance
 
         by_stop = itertools.groupby(pre_gap.ordering, key=lambda node: node.path_idx)
 
-        ordering: List[OrderedRouteViewNode] = []
+        ordering: list[OrderedRouteViewNode] = []
 
         for _, nodes_iter in by_stop:
             nodes = list(nodes_iter)
             distance_end = nodes[-1].distance
 
             if (distance_end - distance_start) > distance:
                 break
 
             ordering.extend(nodes)
 
         return replace(self, ordering=ordering)
 
     @property
-    def paths(self) -> List[Optional[LineString]]:
+    def paths(self) -> list[Optional[LineString]]:
         """
         The simple paths between every pair of stops.
 
         These linestrings are the shortest paths, merged from contiguous ways in the route relation.
         Whenever there is no path between two stops, a `None` element will be inserted into the
         result list.
         """
         max_nb_paths = len(self.stops) - 1
 
         grouped = itertools.groupby(iterable=self.ordering, key=lambda node: node.path_idx)
 
-        lines: List[Optional[LineString]] = [None for _ in range(max_nb_paths)]
+        lines: list[Optional[LineString]] = [None for _ in range(max_nb_paths)]
 
         for n, nodes_iter in grouped:
             nodes = [(node.lat, node.lon) for node in nodes_iter]
             if len(nodes) < 2:
                 continue
             line = LineString(nodes)
             lines[n] = line
@@ -218,15 +219,15 @@
 
         # select all sets of consecutive lines to merge them
         stretches = (line_strings for has_track, line_strings in stretches_grouped if has_track)
 
         merged_lines = []
 
         for line_strings in stretches:
-            coords: List[List[float]] = []
+            coords: list[list[float]] = []
 
             for line in line_strings:
                 if not coords:
                     coords.extend(line.coords)
                 else:
                     coords.extend(
                         line.coords[1:]
@@ -244,15 +245,15 @@
     def geojson(self) -> GeoJsonDict:
         # TODO OrderedRouteView geojson
         raise NotImplementedError
 
 
 def collect_ordered_routes(
     query: RouteQuery, perimeter: Optional[Polygon] = None, n_jobs: int = 1
-) -> List[OrderedRouteView]:
+) -> list[OrderedRouteView]:
     """
     Produce ``OrderedRouteViews`` objects from a result set.
 
     Compare to ``collect_routes()``, this function tries to build the geometry representing the
     path travelled on every route from the first to last stop. If there are no holes in a route's
     relation, this can typically generate a single line string to represent the entire path of
     a route. Note that routes tagged with the PTv1 scheme will be ignored (in an effort to keep
@@ -331,14 +332,16 @@
         # Note: keep in mind that these objects have to be serialized to use in a seperate process,
         # which could take a while for large objects.
         parallel_args = [
             (graph, [stop._stop_point for stop in route.stops])
             for route, graph in zip(views, graphs)
         ]
 
+        # TODO think about using joblib.Parallel's "return_as"
+        #   => can produce a generator that yields the results as soon as they are available
         with joblib.parallel_backend(backend="loky", n_jobs=n_jobs):
             paths = joblib.Parallel()(joblib.delayed(_paths)(*args) for args in parallel_args)
 
         for seg, path in zip(views, paths):
             seg.ordering = path
 
     return [*views, *views_empty]
@@ -469,15 +472,15 @@
     # This node is *probably* representative of the actual stop position for this stop.
     # It is possible though, that the node is actually close to more than one way
     # on the route's track, and that we choose a node that could be far from the
     # actual stop position.
     return a
 
 
-def _paths(route_graph: MultiDiGraph, targets: List[Optional[Point]]) -> List[OrderedRouteViewNode]:
+def _paths(route_graph: MultiDiGraph, targets: list[Optional[Point]]) -> list[OrderedRouteViewNode]:
     """
     Find shortest paths in the directed route graph between every target stop.
 
     Edge weights are set to the metric distance between two nodes.
 
     Not every two stops can be connected, f.e. when they have no representative
     position on the route's track, or when that track has gaps.
@@ -512,22 +515,22 @@
     )
 
     traversal = _traverse_graph(graph=route_graph, progress=traversal)
 
     return traversal.ordering
 
 
-_GraphNode = Tuple[float, float]
+_GraphNode = tuple[float, float]
 
 
 @dataclass
 class _Traversal:
-    ordering: List[OrderedRouteViewNode]
-    targets_visited: List[Optional[Point]]
-    targets_left: List[Optional[Point]]
+    ordering: list[OrderedRouteViewNode]
+    targets_visited: list[Optional[Point]]
+    targets_left: list[Optional[Point]]
     distance: float
     path_idx: int
 
 
 def _traverse_graph(graph: MultiDiGraph, progress: _Traversal) -> _Traversal:
     """Find shortest paths between targets, while discouraging edges to be traversed twice."""
     if len(progress.targets_left) == 0:
@@ -564,15 +567,15 @@
         distance=progress.distance,
         path_idx=progress.path_idx + 1,
     )
     return _traverse_graph(graph, next_progress)
 
 
 def _traverse_path(
-    graph: MultiDiGraph, progress: _Traversal, path_nodes: List[_GraphNode]
+    graph: MultiDiGraph, progress: _Traversal, path_nodes: list[_GraphNode]
 ) -> _Traversal:
     """
     Walk the path to visit the next stop, and collect path nodes along the way.
 
     Repeated traversal of the edge (u, v) is discouraged by setting a large, arbitrary weight.
     Implicitly, this discourages repeated traversal of ways in a route relation. Since the path
     members are supposed to be ordered, ways that are repeatedly traversed should appear more than
```

### Comparing `aio_overpass-0.2.0/aio_overpass/query.py` & `aio_overpass-0.3.0/aio_overpass/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "DefaultQueryRunner",
     "DEFAULT_MAXSIZE",
     "DEFAULT_TIMEOUT",
 )
 
 
 DEFAULT_MAXSIZE = 512
-"""Default ``maxsize`` setting in megabytes"""
+"""Default ``maxsize`` setting in mebibytes"""
 
 DEFAULT_TIMEOUT = 180
 """Default ``timeout`` setting in seconds"""
 
 _COPYRIGHT = "The data included in this document is from www.openstreetmap.org. The data is made available under ODbL."  # noqa: E501
 """This is the same copyright notice included in result sets"""
 
@@ -132,32 +132,32 @@
         References:
             - https://www.openstreetmap.org/copyright
             - https://opendatacommons.org/licenses/odbl/1-0/
         """
         return self._result_set
 
     @property
-    def result_size_mb(self) -> float:
-        """The size of the result set in megabytes."""
+    def result_size_mib(self) -> float:
+        """The size of the result set in mebibytes."""
         return self._result_set_bytes / 1024.0 / 1024.0
 
     @property
-    def maxsize_mb(self) -> int:
+    def maxsize_mib(self) -> int:
         """
-        The current value of the [maxsize:*] setting in megabytes.
+        The current value of the [maxsize:*] setting in mebibytes.
 
         This size indicates the maximum allowed memory for the query in bytes RAM on the server,
         as expected by the user. If the query needs more RAM than this value, the server may abort
         the query with a memory exhaustion. The higher this size, the more probably the server
         rejects the query before executing it.
         """
         return int(self._settings["maxsize"]) // 1024 // 1024
 
-    @maxsize_mb.setter
-    def maxsize_mb(self, value: int) -> None:
+    @maxsize_mib.setter
+    def maxsize_mib(self, value: int) -> None:
         self._settings["maxsize"] = value * 1024 * 1024
 
     @property
     def timeout_secs(self) -> int:
         """
         The current value of the [timeout:*] setting in seconds.
 
@@ -257,14 +257,17 @@
         return self.result_set["generator"]
 
     @property
     def timestamp_osm(self) -> Optional[str]:
         """
         All OSM edits that have been uploaded before this date are included.
 
+        It can take a couple of minutes for changes to the database to show up in the
+        Overpass API query results.
+
         The format is ``YYYY-MM-DDThh:mm:ssZ``.
         """
         if not self.result_set:
             return None
 
         return self.result_set["osm3s"]["timestamp_osm_base"]
 
@@ -291,15 +294,15 @@
 
     def __str__(self) -> str:
         if self.kwargs:
             query = f"query {self.kwargs}"
         else:
             query = "query <no kwargs>"
 
-        size = self.result_size_mb
+        size = self.result_size_mib
         time_query = self.query_duration_secs
         time_total = self.run_duration_secs
 
         if self.nb_tries == 0:
             details = "pending"
         elif self.done:
             if self.nb_tries == 1:
@@ -322,21 +325,21 @@
         if self.nb_tries == 0 or self.error:
             details["tries"] = self.nb_tries
 
         if self.error:
             details["error"] = type(self.error).__name__
 
         if self.done:
-            details["result_size"] = f"{self.result_size_mb}mb"
+            details["result_size"] = f"{self.result_size_mib:.02f}mb"
 
             if self.nb_tries != 1:
-                details["query_duration"] = f"{self.query_duration_secs}s"
+                details["query_duration"] = f"{self.query_duration_secs:.02f}s"
 
         if self.nb_tries > 0:
-            details["run_duration"] = f"{self.run_duration_secs}s"
+            details["run_duration"] = f"{self.run_duration_secs:.02f}s"
 
         details_str = ", ".join((f"{k}={v!r}" for k, v in details.items()))
 
         return f"{cls_name}({details_str})"
 
 
 class QueryRunner(Protocol):
@@ -436,15 +439,15 @@
 
             # Double timeout if exceeded.
             elif err.cause == QueryRejectCause.EXCEEDED_TIMEOUT:
                 query.timeout_secs = max(query.timeout_secs * 2, DEFAULT_TIMEOUT)
 
             # Double maxsize if exceeded.
             elif err.cause == QueryRejectCause.EXCEEDED_MAXSIZE:
-                query.maxsize_mb = max(query.maxsize_mb * 2, DEFAULT_MAXSIZE)
+                query.maxsize_mib = max(query.maxsize_mib * 2, DEFAULT_MAXSIZE)
 
 
 def _backoff_secs(tries: int) -> float:
     """Fibonacci sequence: 1, 2, 3, 5, 8, etc."""
     a, b = 1.0, 2.0
 
     for _ in range(tries):
```

### Comparing `aio_overpass-0.2.0/pyproject.toml` & `aio_overpass-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,103 @@
 [tool.poetry]
 name = "aio-overpass"
-version = "0.2.0"
+version = "0.3.0"
 description = "Async client for the Overpass API"
 authors = ["Tim Wiechers <mail@timwie.dev>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/timwie/aio-overpass"
 documentation = "https://www.timwie.dev/aio-overpass/"
 packages = [{ include = "aio_overpass" }]
 include = ["CHANGELOG.md"]
-exclude = ["test/", "tasks.py"]
+exclude = ["examples/", "test/", "tasks.py"]
 keywords = [
     "geojson",
     "geospatial",
     "gis",
-    "open-street-map",
+    "openstreetmap",
     "osm",
     "overpass-api",
     "public-transport",
+    "spatial-analysis",
+    "spatial-data",
+    "shapely",
 ]
 classifiers = [
+    # TODO "Development Status :: 4 - Beta"
+    #   - complete test suites
+    #   - usability testing
+    #   - check for performance issues
+
+    # TODO "Development Status :: 5 - Production/Stable"
+    #   - release 1.0
+    #   - field-tested
+    #   - no major bugs
+
+    "Development Status :: 3 - Alpha",
     "Framework :: aiohttp",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering :: GIS",
-    "Topic :: Software Development :: Libraries",
+    "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3 :: Only",
 ]
 
+[tool.poetry.urls]
+"Coverage" = "https://codecov.io/gh/timwie/aio-overpass"
+
 [tool.poetry.dependencies]
-aiohttp = "~3.8.4"
-joblib = { version = "~1.2.0", optional = true }
-networkx = { version = "~3.1", optional = true }
-python = "^3.8"
-shapely = { version = "~2.0.1", optional = true }
+aiohttp = "~3.8"
+joblib = { version = "~1.3", optional = true }
+networkx = { version = ">=2.7", optional = true }
+python = "^3.9"
+shapely = { version = "~2.0", optional = true }
 
 [tool.poetry.extras]
 joblib = ["joblib"]
 networkx = ["networkx"]
 shapely = ["shapely"]
 
 [tool.poetry.group.dev.dependencies]
 aioresponses = "^0.7.4"
 black = "^23.3.0"
 codecov = "^2.1.13"
-invoke = "^2.1.2"
+invoke = "^2.1.3"
 isort = "^5.12.0"
-mypy = "^1.3.0"
-pdoc = "^13.1.1"
-pytest = "^7.3.2"
+mypy = "^1.4.1"
+pdoc = "^14.0.0"
+pytest = "^7.4.0"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.1.0"
-ruff = "^0.0.272"
+ruff = "^0.0.275"
 
 [tool.poetry.group.notebooks]
 optional = true
 
 [tool.poetry.group.notebooks.dependencies]
 folium = "^0.14.0"
-jupyterlab = "^4.0.0"
+jupyterlab = "^4.0.2"
+papermill = "^2.4.0"
 randomcolor = "^0.4.4.6"
+selenium = "^4.10.0"
 tabulate = "^0.9.0"
 
 [tool.ruff]
 # https://github.com/charliermarsh/ruff#configuration
 # https://beta.ruff.rs/docs/rules/
 line-length = 100
-target-version = "py38"
+target-version = "py39"
 select = ["E", "F", "N",  "UP", "ANN", "S", "B", "C4", "PL"]
 ignore = ["ANN003", "ANN101", "ANN401", "C408", "PLR2004", "PLW2901"]
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".git",
     ".ipynb_checkpoints",
```

### Comparing `aio_overpass-0.2.0/PKG-INFO` & `aio_overpass-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 Metadata-Version: 2.1
 Name: aio-overpass
-Version: 0.2.0
+Version: 0.3.0
 Summary: Async client for the Overpass API
 Home-page: https://github.com/timwie/aio-overpass
 License: MIT
-Keywords: geojson,geospatial,gis,open-street-map,osm,overpass-api,public-transport
+Keywords: geojson,geospatial,gis,openstreetmap,osm,overpass-api,public-transport,spatial-analysis,spatial-data,shapely
 Author: Tim Wiechers
 Author-email: mail@timwie.dev
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: aiohttp
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: GIS
-Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: joblib
 Provides-Extra: networkx
 Provides-Extra: shapely
-Requires-Dist: aiohttp (>=3.8.4,<3.9.0)
-Requires-Dist: joblib (>=1.2.0,<1.3.0) ; extra == "joblib"
-Requires-Dist: networkx (>=3.1,<3.2) ; extra == "networkx"
-Requires-Dist: shapely (>=2.0.1,<2.1.0) ; extra == "shapely"
+Requires-Dist: aiohttp (>=3.8,<3.9)
+Requires-Dist: joblib (>=1.3,<1.4) ; extra == "joblib"
+Requires-Dist: networkx (>=2.7) ; extra == "networkx"
+Requires-Dist: shapely (>=2.0,<2.1) ; extra == "shapely"
+Project-URL: Coverage, https://codecov.io/gh/timwie/aio-overpass
 Project-URL: Documentation, https://www.timwie.dev/aio-overpass/
 Project-URL: Repository, https://github.com/timwie/aio-overpass
 Description-Content-Type: text/markdown
 
 <h1 align="center">
 aio-overpass
 
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/timwie/aio-overpass/ci.yml)](https://github.com/timwie/aio-overpass/actions/workflows/ci.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/timwie/aio-overpass/test_and_publish.yml)](https://github.com/timwie/aio-overpass/actions/workflows/test_and_publish.yml)
 [![codecov](https://codecov.io/gh/timwie/aio-overpass/branch/main/graph/badge.svg?token=YX1218U740)](https://codecov.io/gh/timwie/aio-overpass)
 [![PyPI version](https://badge.fury.io/py/aio_overpass.svg)](https://badge.fury.io/py/aio_overpass)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aio-overpass)
 </h1>
 
 A client for the [Overpass API], a read-only API that serves up custom selected
 parts of [OpenStreetMap] data. It is optimized for data consumers that need a few
@@ -50,14 +53,15 @@
 
 #### Contents
 - [Features](#features)
 - [Getting Started](#getting-started)
   - [Choosing Extras](#choosing-extras)
 - [Basic Usage](#basic-usage)
   - [Example](#example)
+- [Coordinates](#coordinates)
 - [Motivation](#motivation)
 - [Related Projects](#related-projects)
 - [License](#license)
 
 #### See also
 - An overview of modules, classes and functions can be found in the [API reference](http://www.timwie.dev/aio-overpass/).
 - The version history is available in [CHANGELOG.md](https://github.com/timwie/aio-overpass/blob/main/CHANGELOG.md).
@@ -223,14 +227,45 @@
         53.5416212,
     ]
 }
 ```
 
 <br>
 
+## Coordinates
+* Geographic point locations are expressed by latitude (`lat`) and longitude (`lon`) coordinates.
+  * Latitude is given as an angle that ranges from –90° at the south pole to 90° at the north pole,
+    with 0° at the Equator.
+  * Longitude is given as an angle ranging from 0° at the Prime Meridian (the line that divides the
+    globe into Eastern and Western hemispheres), to +180° eastward and −180° westward.
+  * `lat/lon` values are `floats` that are exactly those degrees, just without the ° sign.
+* This might help you remember which coordinate is which:
+  * If you think of a world map, usually it’s a rectangle.
+  * The _long_ side (the largest side) is the longitude.
+  * Longitude is the x-axis, and latitude is the y-axis.
+* Be wary of coordinate order:
+  * The Overpass API explicitly names the coordinates: `{ "lat": 50.2726005, "lon": 10.9521885 }`
+  * Shapely geometries returned by this library use `lat/lon` order, which is the order
+    stated by [ISO 6709], and seems like the most common order.
+  * [GeoJSON], on the other hand, uses `lon/lat` order.
+* OpenStreetMap uses the [WGS84] spatial reference system
+  used by the Global Positioning System (GPS).
+* OpenStreetMap node coordinates have seven decimal places, which gives them centimetric precision.
+  However, the position accuracy of GPS data is only [about 10m](https://wiki.openstreetmap.org/wiki/Reliability_of_OSM_coordinates).
+  A reasonable display accuracy could be five places, which is precise to
+  [1.1 metres](https://wiki.openstreetmap.org/wiki/Precision_of_coordinates)
+  at the equator.
+* Spatial features that cross the 180th meridian are
+  [problematic](https://en.wikipedia.org/wiki/180th_meridian#Software_representation_problems),
+  since you go from longitude `180.0` to `-180.0`.
+  Such features usually have their geometries split up, like the
+  [area of Russia](https://www.openstreetmap.org/relation/60189).
+
+<br>
+
 ## Motivation
 
 ### Goals
 - A small and stable set of core functionality.
 - Good defaults for queries and retrying.
 - Room for extensions that simplify querying and/or processing of spatial data
   in specific problem domains.
@@ -241,15 +276,15 @@
 - Any sort of Python interface to replace writing Overpass QL code.
 - Integrating other OSM-related services (like the OSM API or Nominatim)
 - Command line interface
 
 <br>
 
 ## Related Projects
-- [Overpass API](https://github.com/drolbr/Overpass-API)
+- [Overpass API](https://github.com/drolbr/Overpass-API), and the [Overpass API Blog]
 - [Overpass Turbo], the best choice to prototype your queries in a browser
 - [Folium], which can be used to visualize GeoJSON on [Leaflet] maps
 - [OSMnx], which is specialized on street networks
 - [overpass-api-python-wrapper], another Python client for the Overpass API
 - [overpy], another Python client for the Overpass API
 - [OSMPythonTools], a Python client for OSM-related services 
 - [overpassify], a Python to Overpass QL transpiler
@@ -257,14 +292,15 @@
 <br>
 
 ## License
 Distributed under the MIT License. See `LICENSE` for more information.
 
 
 [Overpass API]: https://wiki.openstreetmap.org/wiki/Overpass_API
+[Overpass API Blog]: https://dev.overpass-api.de/blog/
 [Overpass QL]: https://wiki.openstreetmap.org/wiki/Overpass_API/Overpass_QL
 [OpenStreetMap]: https://www.openstreetmap.org
 
 [Overpass Turbo]: http://overpass-turbo.eu/
 [Folium]: https://python-visualization.github.io/folium/
 [Leaflet]: https://leafletjs.com/
 [overpass-api-python-wrapper]: https://github.com/mvexel/overpass-api-python-wrapper
@@ -278,7 +314,10 @@
 [NetworkX]: https://networkx.github.io/
 [PyGeodesy]: https://mrjean1.github.io/PyGeodesy/
 [Shapely]: https://shapely.readthedocs.io/en/latest/manual.html
 
 [GeoJSON]: https://en.wikipedia.org/wiki/GeoJSON
 [WKT]: https://en.wikipedia.org/wiki/Well-known_text_representation_of_geometry
 
+[WGS84]: https://en.wikipedia.org/wiki/World_Geodetic_System
+[ISO 6709]: https://en.wikipedia.org/wiki/ISO_6709
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

