# Comparing `tmp/google-maps-routing-0.5.1.tar.gz` & `tmp/google-maps-routing-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-routing-0.5.1.tar", last modified: Mon Jun  5 14:00:22 2023, max compression
+gzip compressed data, was "google-maps-routing-0.6.0.tar", last modified: Thu Jun 29 16:30:01 2023, max compression
```

## Comparing `google-maps-routing-0.5.1.tar` & `google-maps-routing-0.6.0.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.392258 google-maps-routing-0.5.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4657 2023-06-05 14:00:22.388258 google-maps-routing-0.5.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3751 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.380257 google-maps-routing-0.5.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.380257 google-maps-routing-0.5.1/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.380257 google-maps-routing-0.5.1/google/maps/routing/
--rw-rw-r--   0 root         (0)     1003     3465 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.384258 google-maps-routing-0.5.1/google/maps/routing_v2/
--rw-rw-r--   0 root         (0)     1003     2911 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     1387 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.384258 google-maps-routing-0.5.1/google/maps/routing_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.384258 google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/
--rw-rw-r--   0 root         (0)     1003      737 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/__init__.py
--rw-rw-r--   0 root         (0)     1003    18893 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/async_client.py
--rw-rw-r--   0 root         (0)     1003    27744 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.384258 google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/transports/
--rw-rw-r--   0 root         (0)     1003     1288 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6500 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17041 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17278 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17562 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.388258 google-maps-routing-0.5.1/google/maps/routing_v2/types/
--rw-rw-r--   0 root         (0)     1003     2300 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3426 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/fallback_info.py
--rw-rw-r--   0 root         (0)     1003     4200 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/geocoding_results.py
--rw-rw-r--   0 root         (0)     1003     2037 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/location.py
--rw-rw-r--   0 root         (0)     1003     2601 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/maneuver.py
--rw-rw-r--   0 root         (0)     1003     1685 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/navigation_instruction.py
--rw-rw-r--   0 root         (0)     1003     3876 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/polyline.py
--rw-rw-r--   0 root         (0)     1003    15904 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/route.py
--rw-rw-r--   0 root         (0)     1003     1856 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/route_label.py
--rw-rw-r--   0 root         (0)     1003     3646 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/route_modifiers.py
--rw-rw-r--   0 root         (0)     1003     1851 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/route_travel_mode.py
--rw-rw-r--   0 root         (0)     1003    21507 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/routes_service.py
--rw-rw-r--   0 root         (0)     1003     2609 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/routing_preference.py
--rw-rw-r--   0 root         (0)     1003     2809 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/speed_reading_interval.py
--rw-rw-r--   0 root         (0)     1003     1886 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/toll_info.py
--rw-rw-r--   0 root         (0)     1003    10744 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/toll_passes.py
--rw-rw-r--   0 root         (0)     1003     1337 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/units.py
--rw-rw-r--   0 root         (0)     1003     1609 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/vehicle_emission_type.py
--rw-rw-r--   0 root         (0)     1003     1455 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/vehicle_info.py
--rw-rw-r--   0 root         (0)     1003     4688 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/google/maps/routing_v2/types/waypoint.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.388258 google-maps-routing-0.5.1/google_maps_routing.egg-info/
--rw-r--r--   0 root         (0)     1003     4657 2023-06-05 14:00:22.000000 google-maps-routing-0.5.1/google_maps_routing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2161 2023-06-05 14:00:22.000000 google-maps-routing-0.5.1/google_maps_routing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 14:00:22.000000 google-maps-routing-0.5.1/google_maps_routing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       19 2023-06-05 14:00:22.000000 google-maps-routing-0.5.1/google_maps_routing.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 14:00:22.000000 google-maps-routing-0.5.1/google_maps_routing.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      348 2023-06-05 14:00:22.000000 google-maps-routing-0.5.1/google_maps_routing.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-05 14:00:22.000000 google-maps-routing-0.5.1/google_maps_routing.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-05 14:00:22.392258 google-maps-routing-0.5.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2965 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.388258 google-maps-routing-0.5.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.388258 google-maps-routing-0.5.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.388258 google-maps-routing-0.5.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:22.388258 google-maps-routing-0.5.1/tests/unit/gapic/routing_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/tests/unit/gapic/routing_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    73161 2023-06-05 13:56:51.000000 google-maps-routing-0.5.1/tests/unit/gapic/routing_v2/test_routes.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.050019 google-maps-routing-0.6.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4657 2023-06-29 16:30:01.050019 google-maps-routing-0.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3751 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.034021 google-maps-routing-0.6.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.038021 google-maps-routing-0.6.0/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.038021 google-maps-routing-0.6.0/google/maps/routing/
+-rw-rw-r--   0 root         (0)     1003     4023 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.038021 google-maps-routing-0.6.0/google/maps/routing_v2/
+-rw-rw-r--   0 root         (0)     1003     3360 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1387 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.038021 google-maps-routing-0.6.0/google/maps/routing_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.042020 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/
+-rw-rw-r--   0 root         (0)     1003      737 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18889 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27740 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.042020 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/
+-rw-rw-r--   0 root         (0)     1003     1288 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6500 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17041 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17278 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17558 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/google/maps/routing_v2/types/
+-rw-rw-r--   0 root         (0)     1003     2685 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3426 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/fallback_info.py
+-rw-rw-r--   0 root         (0)     1003     4200 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/geocoding_results.py
+-rw-rw-r--   0 root         (0)     1003     1659 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/localized_time.py
+-rw-rw-r--   0 root         (0)     1003     2027 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/location.py
+-rw-rw-r--   0 root         (0)     1003     2766 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/maneuver.py
+-rw-rw-r--   0 root         (0)     1003     1685 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/navigation_instruction.py
+-rw-rw-r--   0 root         (0)     1003     3876 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/polyline.py
+-rw-rw-r--   0 root         (0)     1003    31508 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/route.py
+-rw-rw-r--   0 root         (0)     1003     1856 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/route_label.py
+-rw-rw-r--   0 root         (0)     1003     3600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/route_modifiers.py
+-rw-rw-r--   0 root         (0)     1003     1962 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/route_travel_mode.py
+-rw-rw-r--   0 root         (0)     1003    29064 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/routes_service.py
+-rw-rw-r--   0 root         (0)     1003     2609 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/routing_preference.py
+-rw-rw-r--   0 root         (0)     1003     2809 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/speed_reading_interval.py
+-rw-rw-r--   0 root         (0)     1003     1886 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/toll_info.py
+-rw-rw-r--   0 root         (0)     1003    11021 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/toll_passes.py
+-rw-rw-r--   0 root         (0)     1003     2240 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/traffic_model.py
+-rw-rw-r--   0 root         (0)     1003     7327 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/transit.py
+-rw-rw-r--   0 root         (0)     1003     3209 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/transit_preferences.py
+-rw-rw-r--   0 root         (0)     1003     1337 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/units.py
+-rw-rw-r--   0 root         (0)     1003     1609 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/vehicle_emission_type.py
+-rw-rw-r--   0 root         (0)     1003     1502 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/vehicle_info.py
+-rw-rw-r--   0 root         (0)     1003     4688 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/waypoint.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/google_maps_routing.egg-info/
+-rw-r--r--   0 root         (0)     1003     4657 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2346 2023-06-29 16:30:01.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       19 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      348 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-06-29 16:30:01.050019 google-maps-routing-0.6.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2965 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/tests/unit/gapic/routing_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/tests/unit/gapic/routing_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    73205 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/tests/unit/gapic/routing_v2/test_routes.py
```

### Comparing `google-maps-routing-0.5.1/LICENSE` & `google-maps-routing-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/MANIFEST.in` & `google-maps-routing-0.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/PKG-INFO` & `google-maps-routing-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-routing
-Version: 0.5.1
+Version: 0.6.0
 Summary: Google Maps Routing API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-routing-0.5.1/README.rst` & `google-maps-routing-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing/__init__.py` & `google-maps-routing-0.6.0/google/maps/routing/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,26 +25,28 @@
     FallbackReason,
     FallbackRoutingMode,
 )
 from google.maps.routing_v2.types.geocoding_results import (
     GeocodedWaypoint,
     GeocodingResults,
 )
+from google.maps.routing_v2.types.localized_time import LocalizedTime
 from google.maps.routing_v2.types.location import Location
 from google.maps.routing_v2.types.maneuver import Maneuver
 from google.maps.routing_v2.types.navigation_instruction import NavigationInstruction
 from google.maps.routing_v2.types.polyline import (
     Polyline,
     PolylineEncoding,
     PolylineQuality,
 )
 from google.maps.routing_v2.types.route import (
     Route,
     RouteLeg,
     RouteLegStep,
+    RouteLegStepTransitDetails,
     RouteLegStepTravelAdvisory,
     RouteLegTravelAdvisory,
     RouteTravelAdvisory,
 )
 from google.maps.routing_v2.types.route_label import RouteLabel
 from google.maps.routing_v2.types.route_modifiers import RouteModifiers
 from google.maps.routing_v2.types.route_travel_mode import RouteTravelMode
@@ -57,36 +59,46 @@
     RouteMatrixElementCondition,
     RouteMatrixOrigin,
 )
 from google.maps.routing_v2.types.routing_preference import RoutingPreference
 from google.maps.routing_v2.types.speed_reading_interval import SpeedReadingInterval
 from google.maps.routing_v2.types.toll_info import TollInfo
 from google.maps.routing_v2.types.toll_passes import TollPass
+from google.maps.routing_v2.types.traffic_model import TrafficModel
+from google.maps.routing_v2.types.transit import (
+    TransitAgency,
+    TransitLine,
+    TransitStop,
+    TransitVehicle,
+)
+from google.maps.routing_v2.types.transit_preferences import TransitPreferences
 from google.maps.routing_v2.types.units import Units
 from google.maps.routing_v2.types.vehicle_emission_type import VehicleEmissionType
 from google.maps.routing_v2.types.vehicle_info import VehicleInfo
 from google.maps.routing_v2.types.waypoint import Waypoint
 
 __all__ = (
     "RoutesClient",
     "RoutesAsyncClient",
     "FallbackInfo",
     "FallbackReason",
     "FallbackRoutingMode",
     "GeocodedWaypoint",
     "GeocodingResults",
+    "LocalizedTime",
     "Location",
     "Maneuver",
     "NavigationInstruction",
     "Polyline",
     "PolylineEncoding",
     "PolylineQuality",
     "Route",
     "RouteLeg",
     "RouteLegStep",
+    "RouteLegStepTransitDetails",
     "RouteLegStepTravelAdvisory",
     "RouteLegTravelAdvisory",
     "RouteTravelAdvisory",
     "RouteLabel",
     "RouteModifiers",
     "RouteTravelMode",
     "ComputeRouteMatrixRequest",
@@ -96,12 +108,18 @@
     "RouteMatrixElement",
     "RouteMatrixOrigin",
     "RouteMatrixElementCondition",
     "RoutingPreference",
     "SpeedReadingInterval",
     "TollInfo",
     "TollPass",
+    "TrafficModel",
+    "TransitAgency",
+    "TransitLine",
+    "TransitStop",
+    "TransitVehicle",
+    "TransitPreferences",
     "Units",
     "VehicleEmissionType",
     "VehicleInfo",
     "Waypoint",
 )
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing/gapic_version.py` & `google-maps-routing-0.6.0/google/maps/routing/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.5.1"  # {x-release-please-version}
+__version__ = "0.6.0"  # {x-release-please-version}
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/__init__.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,22 +17,24 @@
 
 __version__ = package_version.__version__
 
 
 from .services.routes import RoutesAsyncClient, RoutesClient
 from .types.fallback_info import FallbackInfo, FallbackReason, FallbackRoutingMode
 from .types.geocoding_results import GeocodedWaypoint, GeocodingResults
+from .types.localized_time import LocalizedTime
 from .types.location import Location
 from .types.maneuver import Maneuver
 from .types.navigation_instruction import NavigationInstruction
 from .types.polyline import Polyline, PolylineEncoding, PolylineQuality
 from .types.route import (
     Route,
     RouteLeg,
     RouteLegStep,
+    RouteLegStepTransitDetails,
     RouteLegStepTravelAdvisory,
     RouteLegTravelAdvisory,
     RouteTravelAdvisory,
 )
 from .types.route_label import RouteLabel
 from .types.route_modifiers import RouteModifiers
 from .types.route_travel_mode import RouteTravelMode
@@ -45,14 +47,17 @@
     RouteMatrixElementCondition,
     RouteMatrixOrigin,
 )
 from .types.routing_preference import RoutingPreference
 from .types.speed_reading_interval import SpeedReadingInterval
 from .types.toll_info import TollInfo
 from .types.toll_passes import TollPass
+from .types.traffic_model import TrafficModel
+from .types.transit import TransitAgency, TransitLine, TransitStop, TransitVehicle
+from .types.transit_preferences import TransitPreferences
 from .types.units import Units
 from .types.vehicle_emission_type import VehicleEmissionType
 from .types.vehicle_info import VehicleInfo
 from .types.waypoint import Waypoint
 
 __all__ = (
     "RoutesAsyncClient",
@@ -60,36 +65,44 @@
     "ComputeRoutesRequest",
     "ComputeRoutesResponse",
     "FallbackInfo",
     "FallbackReason",
     "FallbackRoutingMode",
     "GeocodedWaypoint",
     "GeocodingResults",
+    "LocalizedTime",
     "Location",
     "Maneuver",
     "NavigationInstruction",
     "Polyline",
     "PolylineEncoding",
     "PolylineQuality",
     "Route",
     "RouteLabel",
     "RouteLeg",
     "RouteLegStep",
+    "RouteLegStepTransitDetails",
     "RouteLegStepTravelAdvisory",
     "RouteLegTravelAdvisory",
     "RouteMatrixDestination",
     "RouteMatrixElement",
     "RouteMatrixElementCondition",
     "RouteMatrixOrigin",
     "RouteModifiers",
     "RouteTravelAdvisory",
     "RouteTravelMode",
     "RoutesClient",
     "RoutingPreference",
     "SpeedReadingInterval",
     "TollInfo",
     "TollPass",
+    "TrafficModel",
+    "TransitAgency",
+    "TransitLine",
+    "TransitPreferences",
+    "TransitStop",
+    "TransitVehicle",
     "Units",
     "VehicleEmissionType",
     "VehicleInfo",
     "Waypoint",
 )
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/gapic_metadata.json` & `google-maps-routing-0.6.0/google/maps/routing_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/gapic_version.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.5.1"  # {x-release-please-version}
+__version__ = "0.6.0"  # {x-release-please-version}
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/services/__init__.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/__init__.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/async_client.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,18 +397,18 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             AsyncIterable[google.maps.routing_v2.types.RouteMatrixElement]:
-                Encapsulates route information
-                computed for an origin/destination pair
-                in the ComputeRouteMatrix API. This
-                proto can be streamed to the client.
+                Contains route information computed
+                for an origin/destination pair in the
+                ComputeRouteMatrix API. This proto can
+                be streamed to the client.
 
         """
         # Create or coerce a protobuf request object.
         request = routes_service.ComputeRouteMatrixRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/client.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -614,18 +614,18 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             Iterable[google.maps.routing_v2.types.RouteMatrixElement]:
-                Encapsulates route information
-                computed for an origin/destination pair
-                in the ComputeRouteMatrix API. This
-                proto can be streamed to the client.
+                Contains route information computed
+                for an origin/destination pair in the
+                ComputeRouteMatrix API. This proto can
+                be streamed to the client.
 
         """
         # Create or coerce a protobuf request object.
         # Minor optimization to avoid making a copy if the user passes
         # in a routes_service.ComputeRouteMatrixRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/transports/__init__.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/transports/base.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/transports/grpc.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/services/routes/transports/rest.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,18 +259,18 @@
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.routes_service.RouteMatrixElement:
-                    Encapsulates route information
-                computed for an origin/destination pair
-                in the ComputeRouteMatrix API. This
-                proto can be streamed to the client.
+                    Contains route information computed
+                for an origin/destination pair in the
+                ComputeRouteMatrix API. This proto can
+                be streamed to the client.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
                     "uri": "/distanceMatrix/v2:computeRouteMatrix",
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/__init__.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from .fallback_info import FallbackInfo, FallbackReason, FallbackRoutingMode
 from .geocoding_results import GeocodedWaypoint, GeocodingResults
+from .localized_time import LocalizedTime
 from .location import Location
 from .navigation_instruction import NavigationInstruction
 from .polyline import Polyline, PolylineEncoding, PolylineQuality
 from .route import (
     Route,
     RouteLeg,
     RouteLegStep,
+    RouteLegStepTransitDetails,
     RouteLegStepTravelAdvisory,
     RouteLegTravelAdvisory,
     RouteTravelAdvisory,
 )
 from .route_modifiers import RouteModifiers
 from .routes_service import (
     ComputeRouteMatrixRequest,
@@ -34,32 +36,36 @@
     RouteMatrixDestination,
     RouteMatrixElement,
     RouteMatrixElementCondition,
     RouteMatrixOrigin,
 )
 from .speed_reading_interval import SpeedReadingInterval
 from .toll_info import TollInfo
+from .transit import TransitAgency, TransitLine, TransitStop, TransitVehicle
+from .transit_preferences import TransitPreferences
 from .vehicle_info import VehicleInfo
 from .waypoint import Waypoint
 
 __all__ = (
     "FallbackInfo",
     "FallbackReason",
     "FallbackRoutingMode",
     "GeocodedWaypoint",
     "GeocodingResults",
+    "LocalizedTime",
     "Location",
     "Maneuver",
     "NavigationInstruction",
     "Polyline",
     "PolylineEncoding",
     "PolylineQuality",
     "Route",
     "RouteLeg",
     "RouteLegStep",
+    "RouteLegStepTransitDetails",
     "RouteLegStepTravelAdvisory",
     "RouteLegTravelAdvisory",
     "RouteTravelAdvisory",
     "RouteLabel",
     "RouteModifiers",
     "RouteTravelMode",
     "ComputeRouteMatrixRequest",
@@ -69,12 +75,18 @@
     "RouteMatrixElement",
     "RouteMatrixOrigin",
     "RouteMatrixElementCondition",
     "RoutingPreference",
     "SpeedReadingInterval",
     "TollInfo",
     "TollPass",
+    "TrafficModel",
+    "TransitAgency",
+    "TransitLine",
+    "TransitStop",
+    "TransitVehicle",
+    "TransitPreferences",
     "Units",
     "VehicleEmissionType",
     "VehicleInfo",
     "Waypoint",
 )
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/fallback_info.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/fallback_info.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/geocoding_results.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/geocoding_results.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/location.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/location.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,19 +34,19 @@
     heading).
 
     Attributes:
         lat_lng (google.type.latlng_pb2.LatLng):
             The waypoint's geographic coordinates.
         heading (google.protobuf.wrappers_pb2.Int32Value):
             The compass heading associated with the direction of the
-            flow of traffic. This value is used to specify the side of
-            the road to use for pickup and drop-off. Heading values can
-            be from 0 to 360, where 0 specifies a heading of due North,
-            90 specifies a heading of due East, etc. You can use this
-            field only for ``DRIVE`` and ``TWO_WHEELER``
+            flow of traffic. This value specifies the side of the road
+            for pickup and drop-off. Heading values can be from 0 to
+            360, where 0 specifies a heading of due North, 90 specifies
+            a heading of due East, and so on. You can use this field
+            only for ``DRIVE`` and ``TWO_WHEELER``
             [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
     """
 
     lat_lng: latlng_pb2.LatLng = proto.Field(
         proto.MESSAGE,
         number=1,
         message=latlng_pb2.LatLng,
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/maneuver.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/maneuver.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,18 @@
             Take the ferry.
         FERRY_TRAIN (16):
             Take the train leading onto the ferry.
         ROUNDABOUT_LEFT (17):
             Turn left at the roundabout.
         ROUNDABOUT_RIGHT (18):
             Turn right at the roundabout.
+        DEPART (19):
+            Initial maneuver.
+        NAME_CHANGE (20):
+            Used to indicate a street name change.
     """
     MANEUVER_UNSPECIFIED = 0
     TURN_SLIGHT_LEFT = 1
     TURN_SHARP_LEFT = 2
     UTURN_LEFT = 3
     TURN_LEFT = 4
     TURN_SLIGHT_RIGHT = 5
@@ -86,10 +90,12 @@
     MERGE = 12
     FORK_LEFT = 13
     FORK_RIGHT = 14
     FERRY = 15
     FERRY_TRAIN = 16
     ROUNDABOUT_LEFT = 17
     ROUNDABOUT_RIGHT = 18
+    DEPART = 19
+    NAME_CHANGE = 20
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/navigation_instruction.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/navigation_instruction.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/polyline.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/polyline.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/route_label.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/route_label.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/route_modifiers.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/route_modifiers.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,32 +32,32 @@
 
 class RouteModifiers(proto.Message):
     r"""Encapsulates a set of optional conditions to satisfy when
     calculating the routes.
 
     Attributes:
         avoid_tolls (bool):
-            Specifies whether to avoid toll roads where reasonable.
-            Preference will be given to routes not containing toll
-            roads. Applies only to the ``DRIVE`` and ``TWO_WHEELER``
+            When set to true, avoids toll roads where reasonable, giving
+            preference to routes not containing toll roads. Applies only
+            to the ``DRIVE`` and ``TWO_WHEELER``
             [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
         avoid_highways (bool):
-            Specifies whether to avoid highways where reasonable.
-            Preference will be given to routes not containing highways.
-            Applies only to the ``DRIVE`` and ``TWO_WHEELER``
+            When set to true, avoids highways where reasonable, giving
+            preference to routes not containing highways. Applies only
+            to the ``DRIVE`` and ``TWO_WHEELER``
             [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
         avoid_ferries (bool):
-            Specifies whether to avoid ferries where reasonable.
-            Preference will be given to routes not containing travel by
-            ferries. Applies only to the ``DRIVE`` and\ ``TWO_WHEELER``
+            When set to true, avoids ferries where reasonable, giving
+            preference to routes not containing ferries. Applies only to
+            the ``DRIVE`` and\ ``TWO_WHEELER``
             [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
         avoid_indoor (bool):
-            Specifies whether to avoid navigating indoors where
-            reasonable. Preference will be given to routes not
-            containing indoor navigation. Applies only to the ``WALK``
+            When set to true, avoids navigating indoors where
+            reasonable, giving preference to routes not containing
+            indoor navigation. Applies only to the ``WALK``
             [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
         vehicle_info (google.maps.routing_v2.types.VehicleInfo):
             Specifies the vehicle information.
         toll_passes (MutableSequence[google.maps.routing_v2.types.TollPass]):
             Encapsulates information about toll passes. If toll passes
             are provided, the API tries to return the pass price. If
             toll passes are not provided, the API treats the toll pass
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/route_travel_mode.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/route_travel_mode.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,16 +43,20 @@
             Travel by bicycle.
         WALK (3):
             Travel by walking.
         TWO_WHEELER (4):
             Two-wheeled, motorized vehicle. For example, motorcycle.
             Note that this differs from the ``BICYCLE`` travel mode
             which covers human-powered mode.
+        TRANSIT (7):
+            Travel by public transit routes, where
+            available.
     """
     TRAVEL_MODE_UNSPECIFIED = 0
     DRIVE = 1
     BICYCLE = 2
     WALK = 3
     TWO_WHEELER = 4
+    TRANSIT = 7
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/routes_service.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/routes_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,22 +16,25 @@
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
+from google.type import localized_text_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.maps.routing_v2.types import geocoding_results as gmr_geocoding_results
 from google.maps.routing_v2.types import routing_preference as gmr_routing_preference
+from google.maps.routing_v2.types import transit_preferences as gmr_transit_preferences
 from google.maps.routing_v2.types import fallback_info as gmr_fallback_info
 from google.maps.routing_v2.types import polyline, route
 from google.maps.routing_v2.types import route_modifiers as gmr_route_modifiers
 from google.maps.routing_v2.types import route_travel_mode
+from google.maps.routing_v2.types import traffic_model as gmr_traffic_model
 from google.maps.routing_v2.types import units as gmr_units
 from google.maps.routing_v2.types import waypoint as gmr_waypoint
 
 __protobuf__ = proto.module(
     package="google.maps.routing.v2",
     manifest={
         "RouteMatrixElementCondition",
@@ -90,19 +93,25 @@
         polyline_quality (google.maps.routing_v2.types.PolylineQuality):
             Optional. Specifies your preference for the
             quality of the polyline.
         polyline_encoding (google.maps.routing_v2.types.PolylineEncoding):
             Optional. Specifies the preferred encoding
             for the polyline.
         departure_time (google.protobuf.timestamp_pb2.Timestamp):
-            Optional. The departure time. If you don't
-            set this value, then this value defaults to the
-            time that you made the request. If you set this
-            value to a time that has already occurred, then
-            the request fails.
+            Optional. The departure time. If you don't set this value,
+            then this value defaults to the time that you made the
+            request. NOTE: You can only specify a ``departure_time`` in
+            the past when
+            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] is
+            set to ``TRANSIT``.
+        arrival_time (google.protobuf.timestamp_pb2.Timestamp):
+            Optional. The arrival time. NOTE: Can only be set when
+            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] is
+            set to ``TRANSIT``. You can specify either departure_time or
+            arrival_time, but not both.
         compute_alternative_routes (bool):
             Optional. Specifies whether to calculate
             alternate routes in addition to the route. No
             alternative routes are returned for requests
             that have intermediate waypoints.
         route_modifiers (google.maps.routing_v2.types.RouteModifiers):
             Optional. A set of conditions to satisfy that
@@ -118,20 +127,33 @@
             location of the route request.
         region_code (str):
             Optional. The region code, specified as a ccTLD ("top-level
             domain") two-character value. For more information see
             https://en.wikipedia.org/wiki/List_of_Internet_top-level_domains#Country_code_top-level_domains
         units (google.maps.routing_v2.types.Units):
             Optional. Specifies the units of measure for the display
-            fields. This includes the ``instruction`` field in
+            fields. These fields include the ``instruction`` field in
             [NavigationInstruction][google.maps.routing.v2.NavigationInstruction].
             The units of measure used for the route, leg, step distance,
             and duration are not affected by this value. If you don't
             provide this value, then the display units are inferred from
-            the location of the request.
+            the location of the first origin.
+        optimize_waypoint_order (bool):
+            Optional. If set to true, the service attempts to minimize
+            the overall cost of the route by re-ordering the specified
+            intermediate waypoints. The request fails if any of the
+            intermediate waypoints is a ``via`` waypoint. Use
+            ``ComputeRoutesResponse.Routes.optimized_intermediate_waypoint_index``
+            to find the new ordering. If
+            ``ComputeRoutesResponseroutes.optimized_intermediate_waypoint_index``
+            is not requested in the ``X-Goog-FieldMask`` header, the
+            request fails. If ``optimize_waypoint_order`` is set to
+            false,
+            ``ComputeRoutesResponse.optimized_intermediate_waypoint_index``
+            will be empty.
         requested_reference_routes (MutableSequence[google.maps.routing_v2.types.ComputeRoutesRequest.ReferenceRoute]):
             Optional. Specifies what reference routes to calculate as
             part of the request in addition to the default route. A
             reference route is a route with a different route
             calculation objective than the default route. For example a
             ``FUEL_EFFICIENT`` reference route calculation takes into
             account various parameters that would generate an optimal
@@ -139,14 +161,34 @@
         extra_computations (MutableSequence[google.maps.routing_v2.types.ComputeRoutesRequest.ExtraComputation]):
             Optional. A list of extra computations which
             may be used to complete the request. Note: These
             extra computations may return extra fields on
             the response. These extra fields must also be
             specified in the field mask to be returned in
             the response.
+        traffic_model (google.maps.routing_v2.types.TrafficModel):
+            Optional. Specifies the assumptions to use when calculating
+            time in traffic. This setting affects the value returned in
+            the duration field in the
+            [Route][google.maps.routing.v2.Route] and
+            [RouteLeg][google.maps.routing.v2.RouteLeg] which contains
+            the predicted time in traffic based on historical averages.
+            ``TrafficModel`` is only available for requests that have
+            set
+            [RoutingPreference][google.maps.routing.v2.RoutingPreference]
+            to ``TRAFFIC_AWARE_OPTIMAL`` and
+            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] to
+            ``DRIVE``. Defaults to ``BEST_GUESS`` if traffic is
+            requested and ``TrafficModel`` is not specified.
+        transit_preferences (google.maps.routing_v2.types.TransitPreferences):
+            Optional. Specifies preferences that influence the route
+            returned for ``TRANSIT`` routes. NOTE: You can only specify
+            a ``transit_preferences`` when
+            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] is
+            set to ``TRANSIT``.
     """
 
     class ReferenceRoute(proto.Enum):
         r"""A supported reference route on the ComputeRoutesRequest.
 
         Values:
             REFERENCE_ROUTE_UNSPECIFIED (0):
@@ -169,19 +211,26 @@
                 fail.
             TOLLS (1):
                 Toll information for the route(s).
             FUEL_CONSUMPTION (2):
                 Estimated fuel consumption for the route(s).
             TRAFFIC_ON_POLYLINE (3):
                 Traffic aware polylines for the route(s).
+            HTML_FORMATTED_NAVIGATION_INSTRUCTIONS (4):
+                [Navigation
+                Instructions][google.maps.routing.v2.NavigationInstructions.instructions]
+                presented as a formatted HTML text string. This content is
+                meant to be read as-is. This content is for display only. Do
+                not programmatically parse it.
         """
         EXTRA_COMPUTATION_UNSPECIFIED = 0
         TOLLS = 1
         FUEL_CONSUMPTION = 2
         TRAFFIC_ON_POLYLINE = 3
+        HTML_FORMATTED_NAVIGATION_INSTRUCTIONS = 4
 
     origin: gmr_waypoint.Waypoint = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gmr_waypoint.Waypoint,
     )
     destination: gmr_waypoint.Waypoint = proto.Field(
@@ -215,14 +264,19 @@
         enum=polyline.PolylineEncoding,
     )
     departure_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=7,
         message=timestamp_pb2.Timestamp,
     )
+    arrival_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=19,
+        message=timestamp_pb2.Timestamp,
+    )
     compute_alternative_routes: bool = proto.Field(
         proto.BOOL,
         number=8,
     )
     route_modifiers: gmr_route_modifiers.RouteModifiers = proto.Field(
         proto.MESSAGE,
         number=9,
@@ -237,24 +291,38 @@
         number=16,
     )
     units: gmr_units.Units = proto.Field(
         proto.ENUM,
         number=11,
         enum=gmr_units.Units,
     )
+    optimize_waypoint_order: bool = proto.Field(
+        proto.BOOL,
+        number=13,
+    )
     requested_reference_routes: MutableSequence[ReferenceRoute] = proto.RepeatedField(
         proto.ENUM,
         number=14,
         enum=ReferenceRoute,
     )
     extra_computations: MutableSequence[ExtraComputation] = proto.RepeatedField(
         proto.ENUM,
         number=15,
         enum=ExtraComputation,
     )
+    traffic_model: gmr_traffic_model.TrafficModel = proto.Field(
+        proto.ENUM,
+        number=18,
+        enum=gmr_traffic_model.TrafficModel,
+    )
+    transit_preferences: gmr_transit_preferences.TransitPreferences = proto.Field(
+        proto.MESSAGE,
+        number=20,
+        message=gmr_transit_preferences.TransitPreferences,
+    )
 
 
 class ComputeRoutesResponse(proto.Message):
     r"""ComputeRoutes the response message.
 
     Attributes:
         routes (MutableSequence[google.maps.routing_v2.types.Route]):
@@ -319,19 +387,25 @@
             Optional. Specifies how to compute the route. The server
             attempts to use the selected routing preference to compute
             the route. If the routing preference results in an error or
             an extra long latency, an error is returned. You can specify
             this option only when the ``travel_mode`` is ``DRIVE`` or
             ``TWO_WHEELER``, otherwise the request fails.
         departure_time (google.protobuf.timestamp_pb2.Timestamp):
-            Optional. The departure time. If you don't
-            set this value, this defaults to the time that
-            you made the request. If you set this value to a
-            time that has already occurred, the request
-            fails.
+            Optional. The departure time. If you don't set this value,
+            then this value defaults to the time that you made the
+            request. NOTE: You can only specify a ``departure_time`` in
+            the past when
+            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] is
+            set to ``TRANSIT``.
+        arrival_time (google.protobuf.timestamp_pb2.Timestamp):
+            Optional. The arrival time. NOTE: Can only be set when
+            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] is
+            set to ``TRANSIT``. You can specify either departure_time or
+            arrival_time, but not both.
         language_code (str):
             Optional. The BCP-47 language code, such as "en-US" or
             "sr-Latn". For more information, see
             http://www.unicode.org/reports/tr35/#Unicode_locale_identifier.
             See `Language
             Support <https://developers.google.com/maps/faq#languagesupport>`__
             for the list of supported languages. When you don't provide
@@ -344,14 +418,32 @@
         extra_computations (MutableSequence[google.maps.routing_v2.types.ComputeRouteMatrixRequest.ExtraComputation]):
             Optional. A list of extra computations which
             may be used to complete the request. Note: These
             extra computations may return extra fields on
             the response. These extra fields must also be
             specified in the field mask to be returned in
             the response.
+        traffic_model (google.maps.routing_v2.types.TrafficModel):
+            Optional. Specifies the assumptions to use when calculating
+            time in traffic. This setting affects the value returned in
+            the duration field in the
+            [RouteMatrixElement][google.maps.routing.v2.RouteMatrixElement]
+            which contains the predicted time in traffic based on
+            historical averages.
+            [RoutingPreference][google.maps.routing.v2.RoutingPreference]
+            to ``TRAFFIC_AWARE_OPTIMAL`` and
+            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] to
+            ``DRIVE``. Defaults to ``BEST_GUESS`` if traffic is
+            requested and ``TrafficModel`` is not specified.
+        transit_preferences (google.maps.routing_v2.types.TransitPreferences):
+            Optional. Specifies preferences that influence the route
+            returned for ``TRANSIT`` routes. NOTE: You can only specify
+            a ``transit_preferences`` when
+            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] is
+            set to ``TRANSIT``.
     """
 
     class ExtraComputation(proto.Enum):
         r"""Extra computations to perform while completing the request.
 
         Values:
             EXTRA_COMPUTATION_UNSPECIFIED (0):
@@ -384,27 +476,42 @@
         enum=gmr_routing_preference.RoutingPreference,
     )
     departure_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
+    arrival_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=11,
+        message=timestamp_pb2.Timestamp,
+    )
     language_code: str = proto.Field(
         proto.STRING,
         number=6,
     )
     region_code: str = proto.Field(
         proto.STRING,
         number=9,
     )
     extra_computations: MutableSequence[ExtraComputation] = proto.RepeatedField(
         proto.ENUM,
         number=8,
         enum=ExtraComputation,
     )
+    traffic_model: gmr_traffic_model.TrafficModel = proto.Field(
+        proto.ENUM,
+        number=10,
+        enum=gmr_traffic_model.TrafficModel,
+    )
+    transit_preferences: gmr_transit_preferences.TransitPreferences = proto.Field(
+        proto.MESSAGE,
+        number=12,
+        message=gmr_transit_preferences.TransitPreferences,
+    )
 
 
 class RouteMatrixOrigin(proto.Message):
     r"""A single origin for ComputeRouteMatrixRequest
 
     Attributes:
         waypoint (google.maps.routing_v2.types.Waypoint):
@@ -438,17 +545,17 @@
         proto.MESSAGE,
         number=1,
         message=gmr_waypoint.Waypoint,
     )
 
 
 class RouteMatrixElement(proto.Message):
-    r"""Encapsulates route information computed for an
-    origin/destination pair in the ComputeRouteMatrix API. This
-    proto can be streamed to the client.
+    r"""Contains route information computed for an origin/destination
+    pair in the ComputeRouteMatrix API. This proto can be streamed
+    to the client.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         origin_index (int):
             Zero-based index of the origin in the
@@ -489,16 +596,57 @@
             compute the route with the given preferences for
             this particular origin/destination pair, it may
             fall back to using a different mode of
             computation. When fallback mode is used, this
             field contains detailed information about the
             fallback response. Otherwise this field is
             unset.
+        localized_values (google.maps.routing_v2.types.RouteMatrixElement.LocalizedValues):
+            Text representations of properties of the
+            ``RouteMatrixElement``.
     """
 
+    class LocalizedValues(proto.Message):
+        r"""Text representations of certain properties.
+
+        Attributes:
+            distance (google.type.localized_text_pb2.LocalizedText):
+                Travel distance represented in text form.
+            duration (google.type.localized_text_pb2.LocalizedText):
+                Duration represented in text form taking traffic conditions
+                into consideration. Note: If traffic information was not
+                requested, this value is the same value as static_duration.
+            static_duration (google.type.localized_text_pb2.LocalizedText):
+                Duration represented in text form without
+                taking traffic conditions into consideration.
+            transit_fare (google.type.localized_text_pb2.LocalizedText):
+                Transit fare represented in text form.
+        """
+
+        distance: localized_text_pb2.LocalizedText = proto.Field(
+            proto.MESSAGE,
+            number=1,
+            message=localized_text_pb2.LocalizedText,
+        )
+        duration: localized_text_pb2.LocalizedText = proto.Field(
+            proto.MESSAGE,
+            number=2,
+            message=localized_text_pb2.LocalizedText,
+        )
+        static_duration: localized_text_pb2.LocalizedText = proto.Field(
+            proto.MESSAGE,
+            number=3,
+            message=localized_text_pb2.LocalizedText,
+        )
+        transit_fare: localized_text_pb2.LocalizedText = proto.Field(
+            proto.MESSAGE,
+            number=4,
+            message=localized_text_pb2.LocalizedText,
+        )
+
     origin_index: int = proto.Field(
         proto.INT32,
         number=1,
         optional=True,
     )
     destination_index: int = proto.Field(
         proto.INT32,
@@ -535,10 +683,15 @@
         message=route.RouteTravelAdvisory,
     )
     fallback_info: gmr_fallback_info.FallbackInfo = proto.Field(
         proto.MESSAGE,
         number=8,
         message=gmr_fallback_info.FallbackInfo,
     )
+    localized_values: LocalizedValues = proto.Field(
+        proto.MESSAGE,
+        number=10,
+        message=LocalizedValues,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/routing_preference.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/routing_preference.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/speed_reading_interval.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/speed_reading_interval.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/toll_info.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/toll_info.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/toll_passes.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/toll_passes.py`

 * *Files 6% similar despite different names*

```diff
@@ -179,14 +179,17 @@
             MI, USA.
         US_MI_BCPASS (94):
             MI, USA.
         US_MI_GROSSE_ILE_TOLL_BRIDGE_PASS_TAG (37):
             MI, USA.
         US_MI_IQ_PROX_CARD (38):
             MI, USA.
+            Deprecated as this pass type no longer exists.
+        US_MI_IQ_TAG (95):
+            MI, USA.
         US_MI_MACKINAC_BRIDGE_MAC_PASS (39):
             MI, USA.
         US_MI_NEXPRESS_TOLL (40):
             MI, USA.
         US_MN_EZPASSMN (41):
             MN, USA.
         US_NC_EZPASSNC (42):
@@ -209,28 +212,32 @@
             OH, USA.
         US_PA_EZPASSPA (45):
             PA, USA.
         US_RI_EZPASSRI (46):
             RI, USA.
         US_SC_PALPASS (47):
             SC, USA.
+        US_TX_AVI_TAG (97):
+            TX, USA.
         US_TX_BANCPASS (48):
             TX, USA.
         US_TX_DEL_RIO_PASS (49):
             TX, USA.
         US_TX_EFAST_PASS (50):
             TX, USA.
         US_TX_EAGLE_PASS_EXPRESS_CARD (51):
             TX, USA.
         US_TX_EPTOLL (52):
             TX, USA.
         US_TX_EZ_CROSS (53):
             TX, USA.
         US_TX_EZTAG (54):
             TX, USA.
+        US_TX_FUEGO_TAG (96):
+            TX, USA.
         US_TX_LAREDO_TRADE_TAG (55):
             TX, USA.
         US_TX_PLUSPASS (56):
             TX, USA.
         US_TX_TOLLTAG (57):
             TX, USA.
         US_TX_TXTAG (58):
@@ -307,14 +314,15 @@
     US_MA_EZPASSMA = 6
     US_MD_EZPASSMD = 34
     US_ME_EZPASSME = 35
     US_MI_AMBASSADOR_BRIDGE_PREMIER_COMMUTER_CARD = 36
     US_MI_BCPASS = 94
     US_MI_GROSSE_ILE_TOLL_BRIDGE_PASS_TAG = 37
     US_MI_IQ_PROX_CARD = 38
+    US_MI_IQ_TAG = 95
     US_MI_MACKINAC_BRIDGE_MAC_PASS = 39
     US_MI_NEXPRESS_TOLL = 40
     US_MN_EZPASSMN = 41
     US_NC_EZPASSNC = 42
     US_NC_PEACH_PASS = 87
     US_NC_QUICK_PASS = 43
     US_NH_EZPASSNH = 80
@@ -322,21 +330,23 @@
     US_NJ_EZPASSNJ = 74
     US_NY_EXPRESSPASS = 76
     US_NY_EZPASSNY = 77
     US_OH_EZPASSOH = 44
     US_PA_EZPASSPA = 45
     US_RI_EZPASSRI = 46
     US_SC_PALPASS = 47
+    US_TX_AVI_TAG = 97
     US_TX_BANCPASS = 48
     US_TX_DEL_RIO_PASS = 49
     US_TX_EFAST_PASS = 50
     US_TX_EAGLE_PASS_EXPRESS_CARD = 51
     US_TX_EPTOLL = 52
     US_TX_EZ_CROSS = 53
     US_TX_EZTAG = 54
+    US_TX_FUEGO_TAG = 96
     US_TX_LAREDO_TRADE_TAG = 55
     US_TX_PLUSPASS = 56
     US_TX_TOLLTAG = 57
     US_TX_TXTAG = 58
     US_TX_XPRESS_CARD = 59
     US_UT_ADAMS_AVE_PARKWAY_EXPRESSCARD = 60
     US_VA_EZPASSVA = 61
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/units.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/units.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/vehicle_emission_type.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/vehicle_emission_type.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/vehicle_info.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/vehicle_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,21 +26,22 @@
     manifest={
         "VehicleInfo",
     },
 )
 
 
 class VehicleInfo(proto.Message):
-    r"""Encapsulates the vehicle information, such as the license
-    plate last character.
+    r"""Contains the vehicle information, such as the vehicle
+    emission type.
 
     Attributes:
         emission_type (google.maps.routing_v2.types.VehicleEmissionType):
             Describes the vehicle's emission type. Applies only to the
-            ``DRIVE`` travel mode.
+            ``DRIVE``
+            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
     """
 
     emission_type: vehicle_emission_type.VehicleEmissionType = proto.Field(
         proto.ENUM,
         number=2,
         enum=vehicle_emission_type.VehicleEmissionType,
     )
```

### Comparing `google-maps-routing-0.5.1/google/maps/routing_v2/types/waypoint.py` & `google-maps-routing-0.6.0/google/maps/routing_v2/types/waypoint.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/google_maps_routing.egg-info/PKG-INFO` & `google-maps-routing-0.6.0/google_maps_routing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-routing
-Version: 0.5.1
+Version: 0.6.0
 Summary: Google Maps Routing API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-routing-0.5.1/google_maps_routing.egg-info/SOURCES.txt` & `google-maps-routing-0.6.0/google_maps_routing.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,31 @@
 google/maps/routing_v2/services/routes/transports/base.py
 google/maps/routing_v2/services/routes/transports/grpc.py
 google/maps/routing_v2/services/routes/transports/grpc_asyncio.py
 google/maps/routing_v2/services/routes/transports/rest.py
 google/maps/routing_v2/types/__init__.py
 google/maps/routing_v2/types/fallback_info.py
 google/maps/routing_v2/types/geocoding_results.py
+google/maps/routing_v2/types/localized_time.py
 google/maps/routing_v2/types/location.py
 google/maps/routing_v2/types/maneuver.py
 google/maps/routing_v2/types/navigation_instruction.py
 google/maps/routing_v2/types/polyline.py
 google/maps/routing_v2/types/route.py
 google/maps/routing_v2/types/route_label.py
 google/maps/routing_v2/types/route_modifiers.py
 google/maps/routing_v2/types/route_travel_mode.py
 google/maps/routing_v2/types/routes_service.py
 google/maps/routing_v2/types/routing_preference.py
 google/maps/routing_v2/types/speed_reading_interval.py
 google/maps/routing_v2/types/toll_info.py
 google/maps/routing_v2/types/toll_passes.py
+google/maps/routing_v2/types/traffic_model.py
+google/maps/routing_v2/types/transit.py
+google/maps/routing_v2/types/transit_preferences.py
 google/maps/routing_v2/types/units.py
 google/maps/routing_v2/types/vehicle_emission_type.py
 google/maps/routing_v2/types/vehicle_info.py
 google/maps/routing_v2/types/waypoint.py
 google_maps_routing.egg-info/PKG-INFO
 google_maps_routing.egg-info/SOURCES.txt
 google_maps_routing.egg-info/dependency_links.txt
```

### Comparing `google-maps-routing-0.5.1/setup.py` & `google-maps-routing-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/tests/__init__.py` & `google-maps-routing-0.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/tests/unit/__init__.py` & `google-maps-routing-0.6.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/tests/unit/gapic/__init__.py` & `google-maps-routing-0.6.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/tests/unit/gapic/routing_v2/__init__.py` & `google-maps-routing-0.6.0/tests/unit/gapic/routing_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.5.1/tests/unit/gapic/routing_v2/test_routes.py` & `google-maps-routing-0.6.0/tests/unit/gapic/routing_v2/test_routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     polyline,
     route,
     route_modifiers,
     route_travel_mode,
     routes_service,
     routing_preference,
     toll_passes,
+    traffic_model,
+    transit_preferences,
     units,
     vehicle_emission_type,
     vehicle_info,
     waypoint,
 )
```

