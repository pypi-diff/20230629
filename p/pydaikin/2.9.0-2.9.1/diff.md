# Comparing `tmp/pydaikin-2.9.0.tar.gz` & `tmp/pydaikin-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydaikin-2.9.0.tar", last modified: Sun Jan 29 10:26:47 2023, max compression
+gzip compressed data, was "pydaikin-2.9.1.tar", last modified: Fri May 26 20:03:44 2023, max compression
```

## Comparing `pydaikin-2.9.0.tar` & `pydaikin-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 fer        (501) staff       (20)        0 2023-01-29 10:26:47.550001 pydaikin-2.9.0/
--rw-r--r--   0 fer        (501) staff       (20)    35147 2018-11-06 08:11:08.000000 pydaikin-2.9.0/LICENSE
--rw-r--r--   0 fer        (501) staff       (20)     1594 2023-01-29 10:26:47.550083 pydaikin-2.9.0/PKG-INFO
--rw-r--r--   0 fer        (501) staff       (20)      828 2020-05-21 18:12:53.000000 pydaikin-2.9.0/README.md
-drwxr-xr-x   0 fer        (501) staff       (20)        0 2023-01-29 10:26:47.547877 pydaikin-2.9.0/bin/
--rwxr-xr-x   0 fer        (501) staff       (20)     4398 2022-10-23 15:16:02.000000 pydaikin-2.9.0/bin/pydaikin
-drwxr-xr-x   0 fer        (501) staff       (20)        0 2023-01-29 10:26:47.549164 pydaikin-2.9.0/pydaikin/
--rw-r--r--   0 fer        (501) staff       (20)       23 2021-02-01 08:49:43.000000 pydaikin-2.9.0/pydaikin/__init__.py
--rw-r--r--   0 fer        (501) staff       (20)     6244 2023-01-29 10:19:12.000000 pydaikin-2.9.0/pydaikin/daikin_airbase.py
--rw-r--r--   0 fer        (501) staff       (20)    15570 2022-10-23 14:36:03.000000 pydaikin-2.9.0/pydaikin/daikin_base.py
--rw-r--r--   0 fer        (501) staff       (20)     6730 2022-10-23 14:36:03.000000 pydaikin-2.9.0/pydaikin/daikin_brp069.py
--rw-r--r--   0 fer        (501) staff       (20)     1491 2023-01-29 10:13:21.000000 pydaikin-2.9.0/pydaikin/daikin_brp072c.py
--rw-r--r--   0 fer        (501) staff       (20)     5499 2022-10-23 14:36:03.000000 pydaikin-2.9.0/pydaikin/daikin_skyfi.py
--rw-r--r--   0 fer        (501) staff       (20)     3766 2022-10-23 14:36:03.000000 pydaikin-2.9.0/pydaikin/discovery.py
--rw-r--r--   0 fer        (501) staff       (20)      100 2022-10-13 14:09:56.000000 pydaikin-2.9.0/pydaikin/exceptions.py
--rw-r--r--   0 fer        (501) staff       (20)    10432 2022-10-13 14:09:56.000000 pydaikin-2.9.0/pydaikin/power.py
-drwxr-xr-x   0 fer        (501) staff       (20)        0 2023-01-29 10:26:47.549875 pydaikin-2.9.0/pydaikin.egg-info/
--rw-r--r--   0 fer        (501) staff       (20)     1594 2023-01-29 10:26:47.000000 pydaikin-2.9.0/pydaikin.egg-info/PKG-INFO
--rw-r--r--   0 fer        (501) staff       (20)      436 2023-01-29 10:26:47.000000 pydaikin-2.9.0/pydaikin.egg-info/SOURCES.txt
--rw-r--r--   0 fer        (501) staff       (20)        1 2023-01-29 10:26:47.000000 pydaikin-2.9.0/pydaikin.egg-info/dependency_links.txt
--rw-r--r--   0 fer        (501) staff       (20)       26 2023-01-29 10:26:47.000000 pydaikin-2.9.0/pydaikin.egg-info/requires.txt
--rw-r--r--   0 fer        (501) staff       (20)        9 2023-01-29 10:26:47.000000 pydaikin-2.9.0/pydaikin.egg-info/top_level.txt
--rw-r--r--   0 fer        (501) staff       (20)      235 2020-04-16 18:18:13.000000 pydaikin-2.9.0/pyproject.toml
--rw-r--r--   0 fer        (501) staff       (20)      539 2023-01-29 10:26:47.550482 pydaikin-2.9.0/setup.cfg
--rw-r--r--   0 fer        (501) staff       (20)     1206 2023-01-29 10:25:33.000000 pydaikin-2.9.0/setup.py
+drwxr-xr-x   0 fer        (501) staff       (20)        0 2023-05-26 20:03:44.614827 pydaikin-2.9.1/
+-rw-r--r--   0 fer        (501) staff       (20)    35147 2018-11-06 08:11:08.000000 pydaikin-2.9.1/LICENSE
+-rw-r--r--   0 fer        (501) staff       (20)     1594 2023-05-26 20:03:44.614898 pydaikin-2.9.1/PKG-INFO
+-rw-r--r--   0 fer        (501) staff       (20)      828 2020-05-21 18:12:53.000000 pydaikin-2.9.1/README.md
+drwxr-xr-x   0 fer        (501) staff       (20)        0 2023-05-26 20:03:44.611534 pydaikin-2.9.1/bin/
+-rwxr-xr-x   0 fer        (501) staff       (20)     4398 2022-10-23 15:16:02.000000 pydaikin-2.9.1/bin/pydaikin
+drwxr-xr-x   0 fer        (501) staff       (20)        0 2023-05-26 20:03:44.613963 pydaikin-2.9.1/pydaikin/
+-rw-r--r--   0 fer        (501) staff       (20)       23 2021-02-01 08:49:43.000000 pydaikin-2.9.1/pydaikin/__init__.py
+-rw-r--r--   0 fer        (501) staff       (20)     6804 2023-05-26 19:30:32.000000 pydaikin-2.9.1/pydaikin/daikin_airbase.py
+-rw-r--r--   0 fer        (501) staff       (20)    15610 2023-05-26 19:30:32.000000 pydaikin-2.9.1/pydaikin/daikin_base.py
+-rw-r--r--   0 fer        (501) staff       (20)     6753 2023-05-26 19:30:32.000000 pydaikin-2.9.1/pydaikin/daikin_brp069.py
+-rw-r--r--   0 fer        (501) staff       (20)     1491 2023-01-29 10:13:21.000000 pydaikin-2.9.1/pydaikin/daikin_brp072c.py
+-rw-r--r--   0 fer        (501) staff       (20)     5553 2023-05-26 19:30:32.000000 pydaikin-2.9.1/pydaikin/daikin_skyfi.py
+-rw-r--r--   0 fer        (501) staff       (20)     3766 2022-10-23 14:36:03.000000 pydaikin-2.9.1/pydaikin/discovery.py
+-rw-r--r--   0 fer        (501) staff       (20)      100 2022-10-13 14:09:56.000000 pydaikin-2.9.1/pydaikin/exceptions.py
+-rw-r--r--   0 fer        (501) staff       (20)    10432 2022-10-13 14:09:56.000000 pydaikin-2.9.1/pydaikin/power.py
+drwxr-xr-x   0 fer        (501) staff       (20)        0 2023-05-26 20:03:44.614703 pydaikin-2.9.1/pydaikin.egg-info/
+-rw-r--r--   0 fer        (501) staff       (20)     1594 2023-05-26 20:03:44.000000 pydaikin-2.9.1/pydaikin.egg-info/PKG-INFO
+-rw-r--r--   0 fer        (501) staff       (20)      436 2023-05-26 20:03:44.000000 pydaikin-2.9.1/pydaikin.egg-info/SOURCES.txt
+-rw-r--r--   0 fer        (501) staff       (20)        1 2023-05-26 20:03:44.000000 pydaikin-2.9.1/pydaikin.egg-info/dependency_links.txt
+-rw-r--r--   0 fer        (501) staff       (20)       26 2023-05-26 20:03:44.000000 pydaikin-2.9.1/pydaikin.egg-info/requires.txt
+-rw-r--r--   0 fer        (501) staff       (20)        9 2023-05-26 20:03:44.000000 pydaikin-2.9.1/pydaikin.egg-info/top_level.txt
+-rw-r--r--   0 fer        (501) staff       (20)      235 2020-04-16 18:18:13.000000 pydaikin-2.9.1/pyproject.toml
+-rw-r--r--   0 fer        (501) staff       (20)      539 2023-05-26 20:03:44.615257 pydaikin-2.9.1/setup.cfg
+-rw-r--r--   0 fer        (501) staff       (20)     1206 2023-05-26 19:54:22.000000 pydaikin-2.9.1/setup.py
```

### Comparing `pydaikin-2.9.0/LICENSE` & `pydaikin-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydaikin-2.9.0/PKG-INFO` & `pydaikin-2.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydaikin
-Version: 2.9.0
+Version: 2.9.1
 Summary: Python Daikin HVAC appliances interface
 Home-page: https://bitbucket.org/mustang51/pydaikin
 Author: Yari Adan
 Author-email: mustang@yadan.org
 Maintainer: Fredrik Erlandsson <fredrik.e+pydaikin@gmail.com>, Matthias Lemainque <matthias.lemainque+pydaikin@gmail.com>
 License: GPL
 Keywords: homeautomation,daikin
```

### Comparing `pydaikin-2.9.0/README.md` & `pydaikin-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pydaikin-2.9.0/bin/pydaikin` & `pydaikin-2.9.1/bin/pydaikin`

 * *Files identical despite different names*

### Comparing `pydaikin-2.9.0/pydaikin/daikin_airbase.py` & `pydaikin-2.9.1/pydaikin/daikin_airbase.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,67 +10,67 @@
 
 class DaikinAirBase(DaikinBRP069):
     """Daikin class for AirBase (BRP15B61) units."""
 
     TRANSLATIONS = dict(
         DaikinBRP069.TRANSLATIONS,
         **{
-            'mode': {
-                '0': 'fan',
-                '1': 'hot',
-                '2': 'cool',
-                '3': 'auto',
-                '7': 'dry',
+            "mode": {
+                "0": "fan",
+                "1": "hot",
+                "2": "cool",
+                "3": "auto",
+                "7": "dry",
             },
-            'f_rate': {
-                '0': 'auto',
-                '1': 'low',
-                '3': 'mid',
-                '5': 'high',
-                '1a': 'low/auto',
-                '3a': 'mid/auto',
-                '5a': 'high/auto',
+            "f_rate": {
+                "0": "auto",
+                "1": "low",
+                "3": "mid",
+                "5": "high",
+                "1a": "low/auto",
+                "3a": "mid/auto",
+                "5a": "high/auto",
             },
         },
     )
 
     HTTP_RESOURCES = [
-        'common/basic_info',
-        'aircon/get_control_info',
-        'aircon/get_model_info',
-        'aircon/get_sensor_info',
-        'aircon/get_zone_setting',
+        "common/basic_info",
+        "aircon/get_control_info",
+        "aircon/get_model_info",
+        "aircon/get_sensor_info",
+        "aircon/get_zone_setting",
     ]
 
-    INFO_RESOURCES = DaikinBRP069.INFO_RESOURCES + ['aircon/get_zone_setting']
+    INFO_RESOURCES = DaikinBRP069.INFO_RESOURCES + ["aircon/get_zone_setting"]
 
     @staticmethod
     def parse_response(response_body):
         """Parse response from Daikin, add support for f_rate-auto."""
         _LOGGER.debug("Parsing %s", response_body)
         response = super(DaikinAirBase, DaikinAirBase).parse_response(response_body)
-        if response.get('f_auto') == '1':
-            response['f_rate'] = f'{response["f_rate"]}a'
+        if response.get("f_auto") == "1":
+            response["f_rate"] = f'{response["f_rate"]}a'
         return response
 
     def __init__(self, device_id, session=None):
         """Init the pydaikin appliance, representing one Daikin AirBase
         (BRP15B61) device."""
         super().__init__(device_id, session)
-        self.values.update({'htemp': '-', 'otemp': '-', 'shum': '--'})
+        self.values.update({"htemp": "-", "otemp": "-", "shum": "--"})
 
     async def init(self):
         """Init status and set defaults."""
         await super().init()
         if not self.values:
             raise Exception("Empty values.")
 
     async def _run_get_resource(self, resource):
         """Make the http request."""
-        resource = 'skyfi/%s' % resource
+        resource = "skyfi/%s" % resource
         return await super()._run_get_resource(resource)
 
     @property
     def support_away_mode(self):
         """Return True if the device support away_mode."""
         return False
 
@@ -81,22 +81,27 @@
 
     @property
     def support_outside_temperature(self):
         """AirBase unit returns otemp if master controller starts before it."""
         return True
 
     @property
+    def support_zone_temperature(self):
+        """Return True if the device support setting zone_temperature."""
+        return "lztemp_h" in self.values
+
+    @property
     def fan_rate(self):
         """Return list of supported fan rates."""
-        fan_rates = list(map(str.title, self.TRANSLATIONS.get('f_rate', {}).values()))
-        if self.values.get('frate_steps') == '2':
-            if self.values.get('en_frate_auto') == '0':
+        fan_rates = list(map(str.title, self.TRANSLATIONS.get("f_rate", {}).values()))
+        if self.values.get("frate_steps") == "2":
+            if self.values.get("en_frate_auto") == "0":
                 return fan_rates[1:4:2]
             return fan_rates[:3:2] + fan_rates[3::2]
-        if self.values.get('en_frate_auto') == '0':
+        if self.values.get("en_frate_auto") == "0":
             return fan_rates[1:4]
         return fan_rates
 
     async def _update_settings(self, settings):
         """Update settings to set on Daikin device."""
 
         # Call the base BRP069 method to update the settings; it will
@@ -104,75 +109,84 @@
         # so we can further process them
         current_val = await super()._update_settings(settings)
 
         # f_auto requires some special handling, as it is managed as an
         # attribute of f_rate and we don't directly set it - so when f_rate
         # is being changed, ensure we update f_auto accordingly if it is
         # defined in the current device's returned settings
-        if 'f_auto' in current_val:
+        if "f_auto" in current_val:
             # The system supports f_auto; if we are setting the fan speed
             # then ensure we update the f_auto setting as well
-            if 'f_rate' in settings:
-                self.values['f_auto'] = '1' if 'a' in self.values['f_rate'] else '0'
+            if "f_rate" in settings:
+                self.values["f_auto"] = "1" if "a" in self.values["f_rate"] else "0"
             else:
-                key = 'auto' + self.values['mode']
+                key = "auto" + self.values["mode"]
                 if key in current_val:
-                    self.values['f_auto'] = current_val[key]
+                    self.values["f_auto"] = current_val[key]
 
                     # The f_rate value would have been retrieved from the unit's current
                     # operating mode fan rate setting, and needs the 'a' suffix reinstated
                     # if we are running in an automatic fan speed mode
-                    if self.values['f_auto'] == '1':
-                        self.values['f_rate'] = f'{self.values["f_rate"]}a'
+                    if self.values["f_auto"] == "1":
+                        self.values["f_rate"] = f'{self.values["f_rate"]}a'
 
         return current_val
 
     async def set(self, settings):
         """Set settings on Daikin device."""
         await self._update_settings(settings)
 
-        self.values.setdefault('f_airside', 0)
+        self.values.setdefault("f_airside", 0)
         query_c = (
-            'aircon/set_control_info'
-            '?pow={pow}&mode={mode}&stemp={stemp}&shum={shum}'
-            '&f_rate={f_rate[0]}&f_auto={f_auto}&f_dir={f_dir}'
-            '&lpw=&f_airside={f_airside}'
+            "aircon/set_control_info"
+            "?pow={pow}&mode={mode}&stemp={stemp}&shum={shum}"
+            "&f_rate={f_rate[0]}&f_auto={f_auto}&f_dir={f_dir}"
+            "&lpw=&f_airside={f_airside}"
         ).format(**self.values)
 
         _LOGGER.debug("Sending query_c: %s", query_c)
         await self._get_resource(query_c)
 
     def represent(self, key):
         """Return translated value from key."""
         k, val = super().represent(key)
 
-        if key in ['zone_name', 'zone_onoff']:
-            val = unquote(self.values[key]).split(';')
+        if key in ["zone_name", "zone_onoff", "lztemp_h"]:
+            val = unquote(self.values[key]).split(";")
 
         return (k, val)
 
     @property
     def zones(self):
         """Return list of zones."""
-        if not self.values.get('zone_name'):
+        if not self.values.get("zone_name"):
             return None
-        zone_onoff = self.represent('zone_onoff')[1]
+        zone_onoff = self.represent("zone_onoff")[1]
+        if self.support_zone_temperature:
+            zone_temp = self.represent("lztemp_h")[1]
+            return [
+                (name.strip(" +,"), zone_onoff[i], float(zone_temp[i]))
+                for i, name in enumerate(self.represent("zone_name")[1])
+            ]
         return [
-            (name.strip(' +,'), zone_onoff[i])
-            for i, name in enumerate(self.represent('zone_name')[1])
+            (name.strip(" +,"), zone_onoff[i], 0)
+            for i, name in enumerate(self.represent("zone_name")[1])
         ]
 
-    async def set_zone(self, zone_id, status):
+    async def set_zone(self, zone_id, key, value):
         """Set zone status."""
-        current_state = await self._get_resource('aircon/get_zone_setting')
+        current_state = await self._get_resource("aircon/get_zone_setting")
         self.values.update(current_state)
-        zone_onoff = self.represent('zone_onoff')[1]
-        zone_onoff[zone_id] = status
-        self.values['zone_onoff'] = quote(';'.join(zone_onoff)).lower()
-
-        query = 'aircon/set_zone_setting?zone_name={}&zone_onoff={}'.format(
-            current_state['zone_name'],
-            self.values['zone_onoff'],
+        current_group = self.represent(key)[1]
+        current_group[zone_id] = value
+        self.values[key] = quote(";".join(current_group)).lower()
+
+        query = "aircon/set_zone_setting?zone_name={}&zone_onoff={}".format(
+            current_state["zone_name"],
+            self.values["zone_onoff"],
         )
 
+        if self.support_zone_temperature:
+            query += "&lztemp_h=%s" % self.values["lztemp_h"]
+
         _LOGGER.debug("Set zone:: %s", query)
         await self._get_resource(query)
```

### Comparing `pydaikin-2.9.0/pydaikin/daikin_base.py` & `pydaikin-2.9.1/pydaikin/daikin_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,15 +407,17 @@
             mode=ATTR_TOTAL,
             time=TIME_TODAY,
         )
 
     @property
     def today_energy_consumption(self):
         """Return today's energy consumption in kWh."""
-        return self.today_cool_energy_consumption + self.today_heat_energy_consumption
+        return (self.today_cool_energy_consumption or 0) + (
+            self.today_heat_energy_consumption or 0
+        )
 
     @property
     def fan_rate(self):
         """Return list of supported fan rates."""
         return list(map(str.title, self.TRANSLATIONS.get('f_rate', {}).values()))
 
     @property
@@ -440,10 +442,10 @@
         raise NotImplementedError
 
     @property
     def zones(self):
         """Return list of zones."""
         return
 
-    async def set_zone(self, zone_id, status):
+    async def set_zone(self, zone_id, key, value):
         """Set zone status."""
         raise NotImplementedError
```

### Comparing `pydaikin-2.9.0/pydaikin/daikin_brp069.py` & `pydaikin-2.9.1/pydaikin/daikin_brp069.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,17 +116,17 @@
         'adv': 'advanced mode',
     }
 
     async def init(self):
         """Init status."""
         await self.auto_set_clock()
         if self.values:
-            await self.update_status(self.HTTP_RESOURCES[1:])
-        else:
             await self.update_status(self.HTTP_RESOURCES)
+        else:
+            await self.update_status(self.HTTP_RESOURCES[1:])
 
         if self.support_energy_consumption:
             self.INFO_RESOURCES += [  # pylint: disable=invalid-name
                 'aircon/get_day_power_ex',
                 'aircon/get_week_power',
             ]
 
@@ -140,15 +140,15 @@
         self.values.update({k: self.human_to_daikin(k, v) for k, v in settings.items()})
 
         # we are using an extra mode "off" to power off the unit
         if settings.get('mode', '') == 'off':
             self.values['pow'] = '0'
             # some units are picky with the off mode
             self.values['mode'] = current_val['mode']
-        else:
+        elif 'mode' in settings:
             self.values['pow'] = '1'
 
         # Use settings for respecitve mode (dh and dt)
         for k, val in {'stemp': 'dt', 'shum': 'dh', 'f_rate': 'dfr'}.items():
             if k not in settings:
                 key = val + self.values['mode']
                 if key in current_val:
@@ -203,15 +203,15 @@
         value = self.human_to_daikin('en_streamer', mode)
         if value in ('0', '1'):
             query_h = 'aircon/set_special_mode?en_streamer=%s' % value
             _LOGGER.debug("Sending query: %s", query_h)
             # Update the adv value from the response
             self.values.update(await self._get_resource(query_h))
 
-    async def set_zone(self, zone_id, status):
+    async def set_zone(self, zone_id, key, value):
         """Set zone status."""
 
     async def auto_set_clock(self):
         """Tells the AC to auto-set its internal clock."""
         try:
             await self._get_resource('common/get_datetime?cur=')
         except Exception as exc:  # pylint: disable=broad-except
```

### Comparing `pydaikin-2.9.0/pydaikin/daikin_brp072c.py` & `pydaikin-2.9.1/pydaikin/daikin_brp072c.py`

 * *Files identical despite different names*

### Comparing `pydaikin-2.9.0/pydaikin/daikin_skyfi.py` & `pydaikin-2.9.1/pydaikin/daikin_skyfi.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,14 +165,16 @@
                     (self.represent(f'zone{i+1}')[1].strip(' +,'), onoff)
                     for i, onoff in enumerate(self.represent('zone')[1])
                 ]
             )
             if v != f'Zone {i+1}'
         ]
 
-    async def set_zone(self, zone_id, status):
+    async def set_zone(self, zone_id, key, value):
         """Set zone status."""
+        if key != 'zone_onoff':
+            return
         zone_id += 1
-        query = f'setzone.cgi?pass={{}}&z={zone_id}&s={status}'
+        query = f'setzone.cgi?pass={{}}&z={zone_id}&s={value}'
         _LOGGER.debug("Set zone: %s", query)
         current_state = await self._get_resource(query)
         self.values.update(current_state)
```

### Comparing `pydaikin-2.9.0/pydaikin/discovery.py` & `pydaikin-2.9.1/pydaikin/discovery.py`

 * *Files identical despite different names*

### Comparing `pydaikin-2.9.0/pydaikin/power.py` & `pydaikin-2.9.1/pydaikin/power.py`

 * *Files identical despite different names*

### Comparing `pydaikin-2.9.0/pydaikin.egg-info/PKG-INFO` & `pydaikin-2.9.1/pydaikin.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydaikin
-Version: 2.9.0
+Version: 2.9.1
 Summary: Python Daikin HVAC appliances interface
 Home-page: https://bitbucket.org/mustang51/pydaikin
 Author: Yari Adan
 Author-email: mustang@yadan.org
 Maintainer: Fredrik Erlandsson <fredrik.e+pydaikin@gmail.com>, Matthias Lemainque <matthias.lemainque+pydaikin@gmail.com>
 License: GPL
 Keywords: homeautomation,daikin
```

### Comparing `pydaikin-2.9.0/setup.cfg` & `pydaikin-2.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pydaikin-2.9.0/setup.py` & `pydaikin-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pydaikin',
-    version='2.9.0',
+    version='2.9.1',
     description='Python Daikin HVAC appliances interface',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Yari Adan',
     author_email='mustang@yadan.org',
     maintainer=', '.join(
         (
```

