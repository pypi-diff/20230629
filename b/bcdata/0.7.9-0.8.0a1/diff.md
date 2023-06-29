# Comparing `tmp/bcdata-0.7.9.tar.gz` & `tmp/bcdata-0.8.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcdata-0.7.9.tar", last modified: Tue Jun 13 20:15:14 2023, max compression
+gzip compressed data, was "bcdata-0.8.0a1.tar", last modified: Thu Jun 29 21:34:51 2023, max compression
```

## Comparing `bcdata-0.7.9.tar` & `bcdata-0.8.0a1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-13 20:15:14.292203 bcdata-0.7.9/
--rw-r--r--   0 snorris    (501) staff       (20)     6511 2023-06-13 20:13:50.000000 bcdata-0.7.9/CHANGES.txt
--rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.7.9/LICENSE.txt
--rw-r--r--   0 snorris    (501) staff       (20)    16453 2023-06-13 20:15:14.292054 bcdata-0.7.9/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)    15633 2023-06-02 00:00:04.000000 bcdata-0.7.9/README.md
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-13 20:15:14.290510 bcdata-0.7.9/bcdata/
--rw-r--r--   0 snorris    (501) staff       (20)      349 2023-06-13 20:13:50.000000 bcdata-0.7.9/bcdata/__init__.py
--rw-r--r--   0 snorris    (501) staff       (20)     5267 2022-09-26 21:48:59.000000 bcdata-0.7.9/bcdata/bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     3876 2022-11-18 22:34:58.000000 bcdata-0.7.9/bcdata/bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     9795 2023-04-13 19:53:56.000000 bcdata-0.7.9/bcdata/cli.py
--rw-r--r--   0 snorris    (501) staff       (20)     6342 2022-09-29 00:22:24.000000 bcdata-0.7.9/bcdata/database.py
--rw-r--r--   0 snorris    (501) staff       (20)     3034 2022-11-18 22:34:58.000000 bcdata-0.7.9/bcdata/wcs.py
--rw-r--r--   0 snorris    (501) staff       (20)    11297 2023-06-13 20:13:50.000000 bcdata-0.7.9/bcdata/wfs.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-13 20:15:14.291456 bcdata-0.7.9/bcdata.egg-info/
--rw-r--r--   0 snorris    (501) staff       (20)    16453 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)      474 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/SOURCES.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/dependency_links.txt
--rw-r--r--   0 snorris    (501) staff       (20)       42 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/entry_points.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.7.9/bcdata.egg-info/not-zip-safe
--rw-r--r--   0 snorris    (501) staff       (20)      124 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/requires.txt
--rw-r--r--   0 snorris    (501) staff       (20)        7 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/top_level.txt
--rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.7.9/pyproject.toml
--rw-r--r--   0 snorris    (501) staff       (20)      105 2023-06-13 20:13:50.000000 bcdata-0.7.9/requirements.txt
--rw-r--r--   0 snorris    (501) staff       (20)       38 2023-06-13 20:15:14.292240 bcdata-0.7.9/setup.cfg
--rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.7.9/setup.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-13 20:15:14.291879 bcdata-0.7.9/tests/
--rw-r--r--   0 snorris    (501) staff       (20)     3851 2022-11-18 21:53:34.000000 bcdata-0.7.9/tests/test_bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     6049 2023-04-13 19:53:56.000000 bcdata-0.7.9/tests/test_bcdata.py
--rw-r--r--   0 snorris    (501) staff       (20)    11548 2022-07-20 16:54:44.000000 bcdata-0.7.9/tests/test_bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.7.9/tests/test_cli.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-29 21:34:51.740166 bcdata-0.8.0a1/
+-rw-r--r--   0 snorris    (501) staff       (20)     7126 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/CHANGES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.8.0a1/LICENSE.txt
+-rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-06-29 21:34:51.740002 bcdata-0.8.0a1/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)    15657 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/README.md
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-29 21:34:51.738242 bcdata-0.8.0a1/bcdata/
+-rw-r--r--   0 snorris    (501) staff       (20)      351 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/__init__.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6196 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3876 2022-11-18 22:34:58.000000 bcdata-0.8.0a1/bcdata/bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     9774 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/cli.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6337 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/database.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3654 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/wcs.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11261 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/wfs.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-29 21:34:51.739309 bcdata-0.8.0a1/bcdata.egg-info/
+-rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)      474 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/SOURCES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/dependency_links.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       42 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/entry_points.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.8.0a1/bcdata.egg-info/not-zip-safe
+-rw-r--r--   0 snorris    (501) staff       (20)      134 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/requires.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        7 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/top_level.txt
+-rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.8.0a1/pyproject.toml
+-rw-r--r--   0 snorris    (501) staff       (20)      115 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/requirements.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       38 2023-06-29 21:34:51.740211 bcdata-0.8.0a1/setup.cfg
+-rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.8.0a1/setup.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-29 21:34:51.739818 bcdata-0.8.0a1/tests/
+-rw-r--r--   0 snorris    (501) staff       (20)     5033 2023-06-28 23:17:04.000000 bcdata-0.8.0a1/tests/test_bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6088 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/tests/test_bcdata.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11548 2022-07-20 16:54:44.000000 bcdata-0.8.0a1/tests/test_bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.8.0a1/tests/test_cli.py
```

### Comparing `bcdata-0.7.9/CHANGES.txt` & `bcdata-0.8.0a1/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,31 @@
 Changes
 =======
 
+0.8.0a1 (2023-06-29)
+------------------
+- cache WFS GetCapabilities response for faster requests and fewer http errors
+- retry bc2pg requests on failure
+- move bc2pg download logging to bcdata.log
+- fix dem command default output CRS (#125)
+- upgrade to sqlalchemy v2 (#124)
+
+0.7.12 (2023-06-28)
+------------------
+- fix bc2pg cli error
+
+0.7.11 (2023-06-28)
+------------------
+- fix conflicting bc2pg short option definitions (#134)
+
+0.7.10 (2023-06-28)
+------------------
+- add bc2pg option --geometry_type to avoid issues when type sniffing (#132)
+- fix appending to table with name different from source (#133)
+
 0.7.9 (2023-06-13)
 ------------------
 - fix geometry type checking (#131)
 - update geopandas requirement (#129)
 
 0.7.8 (2023-06-01)
 ------------------
```

### Comparing `bcdata-0.7.9/LICENSE.txt` & `bcdata-0.8.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.9/PKG-INFO` & `bcdata-0.8.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.7.9
+Version: 0.8.0a1
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
@@ -135,19 +135,21 @@
    $ bcdata bc2pg bc-airports --db_url postgresql://postgres:postgres@localhost:5432/postgis
 
 Options:
   -db, --db_url TEXT      Target database url, defaults to $DATABASE_URL
                           environment variable if set
   --table TEXT            Destination table name
   --schema TEXT           Destination schema name
+  --geometry_type TEXT    Spatial type of geometry column
   --query TEXT            A valid CQL or ECQL query
   -c, --count INTEGER     Total number of features to load
   -p, --pagesize INTEGER  Maximum request size
   -k, --primary_key TEXT  Primary key of dataset
-  -s, --schema_only       Dump only the object definitions (schema), not data
+  -s, --sortby TEXT       Name of sort field
+  -e, --schema_only       Create empty table from catalogue schema
   -a, --append            Append to existing table
   -t, --no_timestamp      Do not add download timestamp to bcdata meta table
   -v, --verbose           Increase verbosity.
   -q, --quiet             Decrease verbosity.
   --help                  Show this message and exit.
 ```
 
@@ -168,15 +170,14 @@
   --indent INTEGER                Indentation level for JSON output
   --compact / --not-compact       Use compact separators (',', ':').
   --dst-crs, --dst_crs TEXT       Destination CRS
   -p, --pagesize INTEGER          Maximum request size
   -s, --sortby TEXT               Name of sort field
   --bounds-crs, --bounds_crs TEXT
                                   CRS of provided bounds
-  -w, --max_workers INTEGER       Max number of concurrent requests
   -l, --lowercase                 Write column/properties names as lowercase
   -v, --verbose                   Increase verbosity.
   -q, --quiet                     Decrease verbosity.
   --help                          Show this message and exit.
 ```
 
 #### dem
```

### Comparing `bcdata-0.7.9/README.md` & `bcdata-0.8.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,19 +113,21 @@
    $ bcdata bc2pg bc-airports --db_url postgresql://postgres:postgres@localhost:5432/postgis
 
 Options:
   -db, --db_url TEXT      Target database url, defaults to $DATABASE_URL
                           environment variable if set
   --table TEXT            Destination table name
   --schema TEXT           Destination schema name
+  --geometry_type TEXT    Spatial type of geometry column
   --query TEXT            A valid CQL or ECQL query
   -c, --count INTEGER     Total number of features to load
   -p, --pagesize INTEGER  Maximum request size
   -k, --primary_key TEXT  Primary key of dataset
-  -s, --schema_only       Dump only the object definitions (schema), not data
+  -s, --sortby TEXT       Name of sort field
+  -e, --schema_only       Create empty table from catalogue schema
   -a, --append            Append to existing table
   -t, --no_timestamp      Do not add download timestamp to bcdata meta table
   -v, --verbose           Increase verbosity.
   -q, --quiet             Decrease verbosity.
   --help                  Show this message and exit.
 ```
 
@@ -146,15 +148,14 @@
   --indent INTEGER                Indentation level for JSON output
   --compact / --not-compact       Use compact separators (',', ':').
   --dst-crs, --dst_crs TEXT       Destination CRS
   -p, --pagesize INTEGER          Maximum request size
   -s, --sortby TEXT               Name of sort field
   --bounds-crs, --bounds_crs TEXT
                                   CRS of provided bounds
-  -w, --max_workers INTEGER       Max number of concurrent requests
   -l, --lowercase                 Write column/properties names as lowercase
   -v, --verbose                   Increase verbosity.
   -q, --quiet                     Decrease verbosity.
   --help                          Show this message and exit.
 ```
 
 #### dem
```

### Comparing `bcdata-0.7.9/bcdata/bc2pg.py` & `bcdata-0.8.0a1/bcdata/bc2pg.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,26 +5,48 @@
 import geopandas as gpd
 from shapely.geometry.point import Point
 from shapely.geometry.multipoint import MultiPoint
 from shapely.geometry.linestring import LineString
 from shapely.geometry.multilinestring import MultiLineString
 from shapely.geometry.polygon import Polygon
 from shapely.geometry.multipolygon import MultiPolygon
+from tenacity import retry
+from tenacity.stop import stop_after_delay
+from tenacity.wait import wait_random_exponential
 
 import bcdata
 from bcdata.database import Database
 
 log = logging.getLogger(__name__)
 
+SUPPORTED_TYPES = [
+    "POINT",
+    "POINTZ",
+    "MULTIPOINT",
+    "MULTIPOINTZ",
+    "LINESTRING",
+    "MULTILINESTRING",
+    "MULTILINESTRINGZ",
+    "POLYGON",
+    "MULTIPOLYGON",
+]
+
+
+@retry(stop=stop_after_delay(10), wait=wait_random_exponential(multiplier=1, max=60))
+def _download(url):
+    """offload download requests to geopandas, using tenacity to handle unsuccessful requests"""
+    return gpd.read_file(url)
+
 
 def bc2pg(
     dataset,
     db_url,
     table=None,
     schema=None,
+    geometry_type=None,
     query=None,
     count=None,
     sortby=None,
     primary_key=None,
     pagesize=10000,
     timestamp=True,
     schema_only=False,
@@ -40,32 +62,42 @@
 
     # connect to target db
     db = Database(db_url)
 
     # if appending, get column names from db
     if append:
         # make sure table actually exists
-        if dataset.lower() not in db.tables:
-            raise ValueError(f"{dataset} does not exist, nothing to append to")
+        if schema_name + "." + table_name not in db.tables:
+            raise ValueError(
+                f"{schema_name}.{table_name} does not exist, nothing to append to"
+            )
         column_names = db.get_columns(schema_name, table_name)
 
     # if not appending, define and create table
     else:
         # get info about the table from catalouge
         table_comments, table_details = bcdata.get_table_definition(dataset)
-        # find geometry type(s) in first 10 records and take the first one
-        geom_type = bcdata.get_types(dataset, 10)[0]
+
+        # clean provided geometry type and ensure it is valid
+        if geometry_type:
+            geometry_type = geometry_type.upper()
+            if geometry_type not in SUPPORTED_TYPES:
+                raise ValueError("Geometry type {geometry_type} is not supported")
+
+        # if geometry type is not provided, infer from first 10 records in dataset
+        if not geometry_type:
+            geometry_type = bcdata.get_types(dataset, 10)[0]
 
         # build the table definition and create table
         table = db.define_table(
             schema_name,
             table_name,
             table_details,
             table_comments,
-            geom_type,
+            geometry_type,
             primary_key,
             append,
         )
         column_names = [c.name for c in table.columns]
 
     # check if column provided in sortby option is present in dataset
     if sortby and sortby.lower() not in column_names:
@@ -82,18 +114,16 @@
             count=count,
             sortby=sortby,
             pagesize=pagesize,
             crs="epsg:3005",
         )
         # loop through the requests
         for n, url in enumerate(urls):
-            # download with geopandas, let geopandas handle errors
             log.info(url)
-            df = gpd.read_file(url)
-
+            df = _download(url)
             # tidy the resulting dataframe
             df = df.rename_geometry("geom")
             # lowercasify
             df.columns = df.columns.str.lower()
             # retain only columns matched in table definition
             df = df[column_names]
             # extract features with no geometry
@@ -129,24 +159,25 @@
                 if_exists="append",
                 schema=schema_name,
                 index=False,
             )
 
         # once load complete, note date/time of load completion in public.bcdata
         if timestamp:
-            log.info("Logging download date to public.bcdata")
+            log.info("Logging download date to bcdata.log")
             db.execute(
-                """CREATE TABLE IF NOT EXISTS public.bcdata (
+                """CREATE SCHEMA IF NOT EXISTS bcdata;
+                   CREATE TABLE IF NOT EXISTS bcdata.log (
                      table_name text PRIMARY KEY,
-                     date_downloaded timestamp WITH TIME ZONE
-                   )
+                     latest_download timestamp WITH TIME ZONE
+                   );
                 """
             )
             db.execute(
-                """INSERT INTO public.bcdata (table_name, date_downloaded)
-                   SELECT %s as table_name, NOW() as date_downloaded
-                   ON CONFLICT (table_name) DO UPDATE SET date_downloaded = NOW();
+                """INSERT INTO bcdata.log (table_name, latest_download)
+                   SELECT %s as table_name, NOW() as latest_download
+                   ON CONFLICT (table_name) DO UPDATE SET latest_download = NOW();
                 """,
                 (schema_name + "." + table_name,),
             )
 
     return schema_name + "." + table_name
```

### Comparing `bcdata-0.7.9/bcdata/bcdc.py` & `bcdata-0.8.0a1/bcdata/bcdc.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.9/bcdata/cli.py` & `bcdata-0.8.0a1/bcdata/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,18 +129,21 @@
     else:
         click.echo(json.dumps(info, indent=indent))
 
 
 @cli.command()
 @click.option("--out_file", "-o", help="Output file", default="dem25.tif")
 @bounds_opt_dem
-@dst_crs_opt
+@click.option(
+    "--dst-crs",
+    help="CRS of output file",
+    default="EPSG:3005",
+)
 @click.option(
     "--bounds-crs",
-    "--bounds_crs",
     help="CRS of provided bounds",
     default="EPSG:3005",
 )
 @click.option("--resolution", "-r", type=int, default=25)
 @click.option(
     "--align",
     "-a",
@@ -164,16 +167,14 @@
     interpolation,
     verbose,
     quiet,
 ):
     """Dump BC DEM to TIFF"""
     verbosity = verbose - quiet
     configure_logging(verbosity)
-    if not dst_crs:
-        dst_crs = "EPSG:3005"
     bcdata.get_dem(
         bounds,
         out_file=out_file,
         align=align,
         src_crs=bounds_crs,
         dst_crs=dst_crs,
         resolution=resolution,
@@ -239,31 +240,27 @@
 @click.option("--sortby", "-s", help="Name of sort field")
 @click.option(
     "--bounds-crs",
     "--bounds_crs",
     help="CRS of provided bounds",
     default="EPSG:3005",
 )
-@click.option(
-    "--max_workers", "-w", default=2, help="Max number of concurrent requests"
-)
 @lowercase_opt
 @verbose_opt
 @quiet_opt
 def cat(
     dataset,
     query,
     bounds,
     bounds_crs,
     indent,
     compact,
     dst_crs,
     pagesize,
     sortby,
-    max_workers,
     lowercase,
     verbose,
     quiet,
 ):
     """Write DataBC features to stdout as GeoJSON feature objects."""
     # Note that cat does not concatenate!
     verbosity = verbose - quiet
@@ -280,15 +277,14 @@
         table,
         query=query,
         bounds=bounds,
         bounds_crs=bounds_crs,
         sortby=sortby,
         crs=dst_crs,
         pagesize=pagesize,
-        max_workers=max_workers,
         lowercase=lowercase,
     ):
         click.echo(json.dumps(feat, **dump_kwds))
 
 
 @cli.command()
 @click.argument("dataset", type=click.STRING)
@@ -296,14 +292,15 @@
     "--db_url",
     "-db",
     help="Target database url, defaults to $DATABASE_URL environment variable if set",
     default=os.environ.get("DATABASE_URL"),
 )
 @click.option("--table", help="Destination table name")
 @click.option("--schema", help="Destination schema name")
+@click.option("--geometry_type", help="Spatial type of geometry column")
 @click.option(
     "--query",
     help="A valid CQL or ECQL query",
 )
 @click.option(
     "--count",
     "-c",
@@ -311,18 +308,18 @@
     type=int,
     help="Total number of features to load",
 )
 @click.option("--pagesize", "-p", default=10000, help="Maximum request size")
 @click.option("--primary_key", "-k", default=None, help="Primary key of dataset")
 @click.option("--sortby", "-s", help="Name of sort field")
 @click.option(
+    "-e",
     "--schema_only",
-    "-s",
     is_flag=True,
-    help="Dump only the object definitions (schema), not data",
+    help="Create empty table from catalogue schema",
 )
 @click.option(
     "--append",
     "-a",
     is_flag=True,
     help="Append to existing table",
 )
@@ -335,14 +332,15 @@
 @verbose_opt
 @quiet_opt
 def bc2pg(
     dataset,
     db_url,
     table,
     schema,
+    geometry_type,
     query,
     count,
     pagesize,
     primary_key,
     sortby,
     no_timestamp,
     schema_only,
@@ -366,14 +364,15 @@
         timestamp = True
     out_table = bcdata.bc2pg(
         dataset,
         db_url,
         table=table,
         schema=schema,
         query=query,
+        geometry_type=geometry_type,
         count=count,
         pagesize=pagesize,
         primary_key=primary_key,
         sortby=sortby,
         timestamp=timestamp,
         schema_only=schema_only,
         append=append,
```

### Comparing `bcdata-0.7.9/bcdata/database.py` & `bcdata-0.8.0a1/bcdata/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,18 +146,18 @@
                 )
 
         # make everything multipart
         # (some datasets have mixed singlepart/multipart geometries)
         if geom_type[:5] != "MULTI":
             geom_type = "MULTI" + geom_type
         columns.append(Column("geom", Geometry(geom_type, srid=3005)))
-        meta = MetaData(bind=self.engine)
+        metadata_obj = MetaData()
         table = Table(
             table_name,
-            meta,
+            metadata_obj,
             *columns,
             comment=table_comments,
             schema=schema_name,
         )
 
         if schema_name not in self.schemas:
             self.create_schema(schema_name)
@@ -166,16 +166,15 @@
         if schema_name + "." + table_name in self.tables and not append:
             log.info(f"Table {schema_name}.{table_name} exists, overwriting")
             self.drop_table(schema_name, table_name)
 
         # create the table
         if schema_name + "." + table_name not in self.tables:
             log.info(f"Creating table {schema_name}.{table_name}")
-            table.create()
+            table.create(self.engine)
 
         return table
 
     def get_columns(self, schema, table):
-        metadata = MetaData(schema=schema)
-        metadata.bind = self.engine
-        table = Table(table, metadata, schema=schema, autoload=True)
+        metadata_obj = MetaData(schema=schema)
+        table = Table(table, metadata_obj, schema=schema, autoload_with=self.engine)
         return list(table.columns.keys())
```

### Comparing `bcdata-0.7.9/bcdata/wcs.py` & `bcdata-0.8.0a1/bcdata/wcs.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,18 +30,20 @@
     align=False,
     interpolation=None,
     as_rasterio=False,
 ):
     """Get TRIM DEM for provided bounds, write to GeoTIFF."""
     # align bounds if specified (and bounds are BC Albers CRS)
     if align:
-        if src_crs == "EPSG:3005" and dst_crs == "EPSG:3005":
+        if src_crs.upper() == "EPSG:3005" and dst_crs.upper() == "EPSG:3005":
             bounds = align_bounds(bounds)
         else:
-            raise ValueError("Align is only valid for BC Albers based requests")
+            raise ValueError(
+                f"Target CRS is {dst_crs}, align is only valid for BC Albers based bounds and outputs"
+            )
 
     bbox = ",".join([str(b) for b in bounds])
 
     # do not upsample
     if resolution < 25:
         raise ValueError("Resolution requested must be 25m or greater")
 
@@ -83,19 +85,31 @@
 
     if interpolation:
         payload["INTERPOLATION"] = interpolation
 
     # request data from WCS
     log.debug(payload)
     r = requests.get(WCS_URL, params=payload)
-
-    # save to tiff
+    log.debug(r.headers)
     if r.status_code == 200:
-        with open(out_file, "wb") as file:
-            file.write(r.content)
+        if r.headers["Content-Type"] == "image/tiff":
+            with open(out_file, "wb") as file:
+                file.write(r.content)
+        elif r.headers["Content-Type"] == "application/vnd.ogc.se_xml;charset=UTF-8":
+            raise RuntimeError(
+                "WCS request {} failed with error {}".format(
+                    r.url, str(r.content.decode("utf-8"))
+                )
+            )
+        else:
+            raise RuntimeError(
+                "WCS request {} failed, content type {}".format(
+                    r.url, str(r.headers["Content-Type"])
+                )
+            )
     else:
         raise RuntimeError(
             "WCS request {} failed with status code {}".format(
                 r.url, str(r.status_code)
             )
         )
```

### Comparing `bcdata-0.7.9/bcdata/wfs.py` & `bcdata-0.8.0a1/bcdata/wfs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,130 +9,128 @@
 import sys
 import warnings
 import xml.etree.ElementTree as ET
 from concurrent.futures import ThreadPoolExecutor
 
 from owslib.wfs import WebFeatureService
 import requests
+from tenacity import retry
+from tenacity.stop import stop_after_delay
+from tenacity.wait import wait_random_exponential
+from tenacity.retry import retry_if_exception_type
 import geopandas as gpd
 
-
 import bcdata
 
 if not sys.warnoptions:
     warnings.simplefilter("ignore")
 
 log = logging.getLogger(__name__)
 
 WFS_URL = "https://openmaps.gov.bc.ca/geo/pub/wfs"
 OWS_URL = "http://openmaps.gov.bc.ca/geo/ows"
 
 
-def get_sortkey(table, wfs_schema):
+def check_cache(path):
+    """Return true if the getcapabilities cache does not exist or is more than a day old"""
+    if not os.path.exists(path):
+        return True
+    else:
+        # check the age
+        mod_date = datetime.fromtimestamp(os.path.getmtime(path))
+        if mod_date < (datetime.now() - timedelta(days=1)):
+            return True
+        else:
+            return False
+
+
+def get_capabilities(refresh=False, cache_file=None):
+    """
+    Request server capabilities (layer definitions).
+    Cache response as file daily, caching to location specified by:
+      - cache_file parameter
+      - $BCDATA_CACHE environment variable
+      - default (~/.bcdata)
+    """
+    if not cache_file:
+        if "BCDATA_CACHE" in os.environ:
+            cache_file = os.environ["BCDATA_CACHE"]
+        else:
+            cache_file = os.path.join(str(Path.home()), ".bcdata")
+
+    # download capabilites xml if file is > 1 day old or refresh is specified
+    if check_cache(cache_file) or refresh:
+        with open(cache_file, "w") as f:
+            f.write(
+                ET.tostring(
+                    WebFeatureService(OWS_URL, version="2.0.0")._capabilities,
+                    encoding="unicode",
+                )
+            )
+
+    # load cached xml to WFS object
+    with open(cache_file, "r") as f:
+        return WebFeatureService(OWS_URL, version="2.0.0", xml=f.read())
+
+
+def get_sortkey(table, schema):
     """Check data for unique columns available for sorting paged requests"""
-    columns = list(wfs_schema["properties"].keys())
+    columns = list(schema["properties"].keys())
     # use OBJECTID as default sort key, if present
     if "OBJECTID" in columns:
         return "OBJECTID"
     # if OBJECTID is not present (several GSR tables), use SEQUENCE_ID
     elif "SEQUENCE_ID" in columns:
         return "SEQUENCE_ID"
     # otherwise, it should be safe to presume first column is the primary key
     # (WHSE_FOREST_VEGETATION.VEG_COMP_LYR_R1_POLY's FEATURE_ID appears to be
     # the only public case, and very large veg downloads are likely better
     # accessed via some other channel)
     else:
         return columns[0]
 
 
-def check_cache(path):
-    """Return true if the cache file holding list of all datasets
-    does not exist or is more than a day old
-    (this is not very long, but checking daily seems to be a good strategy)
-    """
-    if not os.path.exists(path):
-        return True
-    else:
-        # check the age
-        mod_date = datetime.fromtimestamp(os.path.getmtime(path))
-        if mod_date < (datetime.now() - timedelta(days=1)):
-            return True
-        else:
-            return False
-
-
 def validate_name(dataset):
     """Check wfs/cache and the bcdc api to see if dataset name is valid"""
     if dataset.upper() in list_tables():
         return dataset.upper()
     else:
         return bcdata.get_table_name(dataset.upper())
 
 
-def list_tables(refresh=False, cache_file=None):
-    """Return a list of all datasets available via WFS"""
-    # default cache listing all objects available is
-    # ~/.bcdata
-    if not cache_file:
-        if "BCDATA_CACHE" in os.environ:
-            cache_file = os.environ["BCDATA_CACHE"]
-        else:
-            cache_file = os.path.join(str(Path.home()), ".bcdata")
-
-    # regenerate the cache if:
-    # - the cache file doesn't exist
-    # - we force a refresh
-    # - the cache is older than 1 day
-    if refresh or check_cache(cache_file):
-        WFS = WebFeatureService(OWS_URL, version="2.0.0")
-        bcdata_objects = [i.strip("pub:") for i in list(WFS.contents)]
-        with open(cache_file, "w") as outfile:
-            json.dump(sorted(bcdata_objects), outfile)
-    else:
-        with open(cache_file, "r") as infile:
-            bcdata_objects = json.load(infile)
-
-    return bcdata_objects
+def list_tables(cache_file=None):
+    """Return a list of all tables available via WFS"""
+    capabilites = get_capabilities(cache_file)
+    return [i.strip("pub:") for i in list(capabilites.contents)]
 
 
+@retry(
+    retry=retry_if_exception_type(requests.exceptions.HTTPError),
+    stop=stop_after_delay(10),
+    wait=wait_random_exponential(multiplier=1, max=60),
+)
 def get_count(dataset, query=None):
     """Ask DataBC WFS how many features there are in a table/query"""
     # https://gis.stackexchange.com/questions/45101/only-return-the-numberoffeatures-in-a-wfs-query
     table = validate_name(dataset)
     payload = {
         "service": "WFS",
         "version": "2.0.0",
         "request": "GetFeature",
         "typeName": table,
         "resultType": "hits",
         "outputFormat": "json",
     }
     if query:
         payload["CQL_FILTER"] = query
-    try:
-        r = requests.get(WFS_URL, params=payload)
-        log.debug(r.url)
-        r.raise_for_status()  # check status code is 200
-    except requests.exceptions.HTTPError as err:  # fail if not 200
-        raise SystemExit(err)
-    return int(ET.fromstring(r.text).attrib["numberMatched"])
-
-
-def make_request(url):
-    """Submit a getfeature request to DataBC WFS and return features"""
-    try:
-        r = requests.get(url)
-        log.info(r.url)
-        log.debug(r.headers)
-        r.raise_for_status()  # check status code is 200
-    except requests.exceptions.HTTPError as err:  # fail if not 200
-        print(log.debug(r.headers))
-        raise SystemExit(err)
 
-    return r.json()["features"]  # return features if status code is 200
+    r = requests.get(WFS_URL, params=payload)
+    log.debug(r.url)
+    r.raise_for_status()  # check status code is 200
+    return int(ET.fromstring(r.text).attrib["numberMatched"])
 
 
 def define_requests(
     dataset,
     query=None,
     crs="epsg:4326",
     bounds=None,
@@ -153,28 +151,24 @@
     table = validate_name(dataset)
     n = bcdata.get_count(table, query=query)
     # if count not provided or if it is greater than n of total features,
     # set count to number of features
     if not count or count > n:
         count = n
     log.info(f"Total features requested: {count}")
-    WFS = WebFeatureService(OWS_URL, version="2.0.0")
-    wfs_schema = WFS.get_schema("pub:" + table)
-    geom_column = wfs_schema["geometry_column"]
-    # DataBC WFS getcapabilities says that it supports paging,
-    # and the spec says that responses should include 'next URI'
-    # (section 7.7.4.4.1)....
-    # But I do not see any next uri in the responses. Instead of following
-    # the paged urls, for datasets with >10k records, just generate urls
-    # based on number of features in the dataset.
+    wfs = get_capabilities()
+    schema = wfs.get_schema("pub:" + table)
+    geom_column = schema["geometry_column"]
+
+    # for datasets with >10k records, generate a list of urls based on number of features in the dataset.
     chunks = math.ceil(count / pagesize)
 
     # if making several requests, we need to sort by something
     if chunks > 1 and not sortby:
-        sortby = get_sortkey(table, wfs_schema)
+        sortby = get_sortkey(table, schema)
 
     # build the request parameters for each chunk
     urls = []
     for i in range(chunks):
         request = {
             "service": "WFS",
             "version": "2.0.0",
@@ -204,40 +198,55 @@
                 request["count"] = count - request["startIndex"]
             else:
                 request["count"] = pagesize
         urls.append(WFS_URL + "?" + urlencode(request, doseq=True))
     return urls
 
 
+@retry(
+    retry=retry_if_exception_type(requests.exceptions.HTTPError),
+    stop=stop_after_delay(10),
+    wait=wait_random_exponential(multiplier=1, max=60),
+)
+def make_request(url):
+    """Submit a getfeature request to DataBC WFS and return features"""
+    r = requests.get(url)
+    log.info(r.url)
+    log.debug(r.headers)
+    r.raise_for_status()  # check status code is 200, otherwise HTTPError is raised
+    return r.json()["features"]
+
+
 def get_data(
     dataset,
     query=None,
     crs="epsg:4326",
     bounds=None,
     bounds_crs="epsg:3005",
     count=None,
     sortby=None,
     pagesize=10000,
-    max_workers=2,
     as_gdf=False,
     lowercase=False,
 ):
-    """Get GeoJSON featurecollection (or geodataframe) from DataBC WFS"""
+    """Request features from DataBC WFS and return GeoJSON featurecollection or geodataframe"""
     urls = define_requests(
         dataset,
         query=query,
         crs=crs,
         bounds=bounds,
         bounds_crs=bounds_crs,
         count=count,
         sortby=sortby,
         pagesize=pagesize,
     )
-    with ThreadPoolExecutor(max_workers=max_workers) as executor:
-        results = executor.map(make_request, urls)
+    # loop through requests
+    results = []
+    for url in urls:
+        results.append(make_request(url))
 
     outjson = dict(type="FeatureCollection", features=[])
     for result in results:
         outjson["features"] += result
     # if specified, lowercasify all properties
     if lowercase:
         for feature in outjson["features"]:
@@ -267,36 +276,34 @@
     query=None,
     crs="epsg:4326",
     bounds=None,
     bounds_crs="epsg:3005",
     count=None,
     sortby=None,
     pagesize=10000,
-    max_workers=2,
     lowercase=False,
 ):
     """Yield features from DataBC WFS"""
     urls = define_requests(
         dataset,
         query=query,
         crs=crs,
         bounds=bounds,
         bounds_crs=bounds_crs,
         count=count,
         sortby=sortby,
         pagesize=pagesize,
     )
-    with ThreadPoolExecutor(max_workers=max_workers) as executor:
-        for result in executor.map(make_request, urls):
-            for feature in result:
-                if lowercase:
-                    feature["properties"] = {
-                        k.lower(): v for k, v in feature["properties"].items()
-                    }
-                yield feature
+    for url in urls:
+        for feature in make_request(url):
+            if lowercase:
+                feature["properties"] = {
+                    k.lower(): v for k, v in feature["properties"].items()
+                }
+            yield feature
 
 
 def get_types(dataset, count=10):
     """Return distinct types within the first n features"""
     # validate the table name
     table = validate_name(dataset)
     log.info("Getting feature geometry type")
```

### Comparing `bcdata-0.7.9/bcdata.egg-info/PKG-INFO` & `bcdata-0.8.0a1/bcdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.7.9
+Version: 0.8.0a1
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
@@ -135,19 +135,21 @@
    $ bcdata bc2pg bc-airports --db_url postgresql://postgres:postgres@localhost:5432/postgis
 
 Options:
   -db, --db_url TEXT      Target database url, defaults to $DATABASE_URL
                           environment variable if set
   --table TEXT            Destination table name
   --schema TEXT           Destination schema name
+  --geometry_type TEXT    Spatial type of geometry column
   --query TEXT            A valid CQL or ECQL query
   -c, --count INTEGER     Total number of features to load
   -p, --pagesize INTEGER  Maximum request size
   -k, --primary_key TEXT  Primary key of dataset
-  -s, --schema_only       Dump only the object definitions (schema), not data
+  -s, --sortby TEXT       Name of sort field
+  -e, --schema_only       Create empty table from catalogue schema
   -a, --append            Append to existing table
   -t, --no_timestamp      Do not add download timestamp to bcdata meta table
   -v, --verbose           Increase verbosity.
   -q, --quiet             Decrease verbosity.
   --help                  Show this message and exit.
 ```
 
@@ -168,15 +170,14 @@
   --indent INTEGER                Indentation level for JSON output
   --compact / --not-compact       Use compact separators (',', ':').
   --dst-crs, --dst_crs TEXT       Destination CRS
   -p, --pagesize INTEGER          Maximum request size
   -s, --sortby TEXT               Name of sort field
   --bounds-crs, --bounds_crs TEXT
                                   CRS of provided bounds
-  -w, --max_workers INTEGER       Max number of concurrent requests
   -l, --lowercase                 Write column/properties names as lowercase
   -v, --verbose                   Increase verbosity.
   -q, --quiet                     Decrease verbosity.
   --help                          Show this message and exit.
 ```
 
 #### dem
```

### Comparing `bcdata-0.7.9/setup.py` & `bcdata-0.8.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.9/tests/test_bc2pg.py` & `bcdata-0.8.0a1/tests/test_bc2pg.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 import bcdata
 from bcdata.database import Database
 
 
 DB_URL = "postgresql://postgres@localhost:5432/bcdata_test"
 DB_CONNECTION = Database(url=DB_URL)
 AIRPORTS_PACKAGE = "bc-airports"
@@ -37,14 +39,30 @@
 
 def test_bc2pg_schema():
     bcdata.bc2pg(AIRPORTS_TABLE, DB_URL, schema="testschema")
     assert "testschema.gsr_airports_svw" in DB_CONNECTION.tables
     DB_CONNECTION.execute("drop schema testschema cascade")
 
 
+def test_bc2pg_geometry_type():
+    bcdata.bc2pg(AIRPORTS_TABLE, DB_URL, count=10, geometry_type="POINT")
+    assert AIRPORTS_TABLE in DB_CONNECTION.tables
+    DB_CONNECTION.execute("drop table " + AIRPORTS_TABLE)
+
+
+def test_bc2pg_geometry_type_mismatch():
+    with pytest.raises(Exception):
+        bcdata.bc2pg(AIRPORTS_TABLE, DB_URL, count=10, geometry_type="LINESTRING")
+
+
+def test_bc2pg_geometry_type_invalid():
+    with pytest.raises(Exception):
+        bcdata.bc2pg(AIRPORTS_TABLE, DB_URL, count=10, geometry_type="MULTIPOLYGONZ")
+
+
 def test_bc2pg_z():
     bcdata.bc2pg(STREAMS_TABLE, DB_URL, query="WATERSHED_GROUP_CODE='VICT'")
     assert STREAMS_TABLE in DB_CONNECTION.tables
     r = DB_CONNECTION.query(
         """
         SELECT ST_NDims(geom) from whse_basemapping.fwa_stream_networks_sp limit 1
         """
@@ -107,7 +125,28 @@
         DB_URL,
         query="AIRPORT_NAME='Victoria International Airport'",
         append=True,
     )
     r = DB_CONNECTION.query("select * from whse_imagery_and_base_maps.gsr_airports_svw")
     assert len(r) == 2
     DB_CONNECTION.execute("drop table " + AIRPORTS_TABLE)
+
+
+def test_bc2pg_append_to_other():
+    bcdata.bc2pg(AIRPORTS_TABLE, DB_URL, schema_only=True, table="arpt")
+    bcdata.bc2pg(
+        AIRPORTS_TABLE,
+        DB_URL,
+        table="arpt",
+        query="AIRPORT_NAME='Terrace (Northwest Regional) Airport'",
+        append=True,
+    )
+    bcdata.bc2pg(
+        AIRPORTS_TABLE,
+        DB_URL,
+        table="arpt",
+        query="AIRPORT_NAME='Victoria International Airport'",
+        append=True,
+    )
+    r = DB_CONNECTION.query("select * from whse_imagery_and_base_maps.arpt")
+    assert len(r) == 2
+    DB_CONNECTION.execute("drop table whse_imagery_and_base_maps.arpt")
```

### Comparing `bcdata-0.7.9/tests/test_bcdata.py` & `bcdata-0.8.0a1/tests/test_bcdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 
 import rasterio
 import pytest
 from rasterio.coords import BoundingBox
 
 import bcdata
+from bcdata.wfs import get_capabilities
+
 from geopandas.geodataframe import GeoDataFrame
 
 AIRPORTS_PACKAGE = "bc-airports"
 AIRPORTS_TABLE = "WHSE_IMAGERY_AND_BASE_MAPS.GSR_AIRPORTS_SVW"
 UTMZONES_KEY = "utm-zones-of-british-columbia"
 BEC_KEY = "biogeoclimatic-ecosystem-classification-bec-map"
 ASSESSMENTS_TABLE = "whse_fish.pscis_assessment_svw"
@@ -18,15 +20,15 @@
 
 def test_validate_table_lowercase():
     table = bcdata.validate_name(AIRPORTS_TABLE.lower())
     assert table == AIRPORTS_TABLE
 
 
 def test_cache_file(tmp_path):
-    bcdata.list_tables(refresh=True, cache_file=tmp_path / ".bcdata_test")
+    get_capabilities(refresh=True, cache_file=tmp_path / ".bcdata_test")
     assert os.path.exists(tmp_path / ".bcdata_test")
 
 
 def test_get_table_name_urlparse():
     # bcdc api query result["object_name"] is not correct WFS layer name,
     # use WFS resource url
     table = bcdata.get_table_name("natural-resource-nr-district")
```

### Comparing `bcdata-0.7.9/tests/test_bcdc.py` & `bcdata-0.8.0a1/tests/test_bcdc.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.9/tests/test_cli.py` & `bcdata-0.8.0a1/tests/test_cli.py`

 * *Files identical despite different names*

