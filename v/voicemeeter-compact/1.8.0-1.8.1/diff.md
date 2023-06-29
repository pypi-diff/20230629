# Comparing `tmp/voicemeeter-compact-1.8.0.tar.gz` & `tmp/voicemeeter-compact-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter-compact-1.8.0.tar", max compression
+gzip compressed data, was "voicemeeter-compact-1.8.1.tar", max compression
```

## Comparing `voicemeeter-compact-1.8.0.tar` & `voicemeeter-compact-1.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter-compact-1.8.0/LICENSE
--rw-r--r--   0        0        0      729 2023-06-29 17:10:11.382512 voicemeeter-compact-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter-compact-1.8.0/README.md
--rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter-compact-1.8.0/vmcompact/__init__.py
--rw-r--r--   0        0        0     4644 2023-06-29 17:12:44.240157 voicemeeter-compact-1.8.0/vmcompact/app.py
--rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter-compact-1.8.0/vmcompact/banner.py
--rw-r--r--   0        0        0    23309 2023-06-29 11:15:56.815136 voicemeeter-compact-1.8.0/vmcompact/builders.py
--rw-r--r--   0        0        0    10867 2023-06-29 10:15:56.869547 voicemeeter-compact-1.8.0/vmcompact/channels.py
--rw-r--r--   0        0        0     9634 2023-06-26 08:40:26.219945 voicemeeter-compact-1.8.0/vmcompact/config.py
--rw-r--r--   0        0        0     2497 2023-06-29 10:49:39.208371 voicemeeter-compact-1.8.0/vmcompact/configurations.py
--rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter-compact-1.8.0/vmcompact/data.py
--rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter-compact-1.8.0/vmcompact/errors.py
--rw-r--r--   0        0        0     8960 2023-06-29 10:16:01.341472 voicemeeter-compact-1.8.0/vmcompact/gainlayer.py
--rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter-compact-1.8.0/vmcompact/img/cat.ico
--rw-r--r--   0        0        0    17472 2023-06-29 11:09:26.649143 voicemeeter-compact-1.8.0/vmcompact/menu.py
--rw-r--r--   0        0        0     3785 2023-06-29 10:52:07.632943 voicemeeter-compact-1.8.0/vmcompact/navigation.py
--rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter-compact-1.8.0/vmcompact/subject.py
--rw-r--r--   0        0        0     7183 2023-06-29 17:25:10.583826 voicemeeter-compact-1.8.0/setup.py
--rw-r--r--   0        0        0     6857 2023-06-29 17:25:10.584801 voicemeeter-compact-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter-compact-1.8.1/LICENSE
+-rw-r--r--   0        0        0      730 2023-06-29 18:09:21.736138 voicemeeter-compact-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter-compact-1.8.1/README.md
+-rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter-compact-1.8.1/vmcompact/__init__.py
+-rw-r--r--   0        0        0     4644 2023-06-29 17:12:44.240157 voicemeeter-compact-1.8.1/vmcompact/app.py
+-rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter-compact-1.8.1/vmcompact/banner.py
+-rw-r--r--   0        0        0    23309 2023-06-29 11:15:56.815136 voicemeeter-compact-1.8.1/vmcompact/builders.py
+-rw-r--r--   0        0        0    10867 2023-06-29 10:15:56.869547 voicemeeter-compact-1.8.1/vmcompact/channels.py
+-rw-r--r--   0        0        0     9634 2023-06-26 08:40:26.219945 voicemeeter-compact-1.8.1/vmcompact/config.py
+-rw-r--r--   0        0        0     2661 2023-06-29 18:10:03.397989 voicemeeter-compact-1.8.1/vmcompact/configurations.py
+-rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter-compact-1.8.1/vmcompact/data.py
+-rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter-compact-1.8.1/vmcompact/errors.py
+-rw-r--r--   0        0        0     8960 2023-06-29 10:16:01.341472 voicemeeter-compact-1.8.1/vmcompact/gainlayer.py
+-rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter-compact-1.8.1/vmcompact/img/cat.ico
+-rw-r--r--   0        0        0    17472 2023-06-29 11:09:26.649143 voicemeeter-compact-1.8.1/vmcompact/menu.py
+-rw-r--r--   0        0        0     3785 2023-06-29 10:52:07.632943 voicemeeter-compact-1.8.1/vmcompact/navigation.py
+-rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter-compact-1.8.1/vmcompact/subject.py
+-rw-r--r--   0        0        0     7183 2023-06-29 18:13:16.117955 voicemeeter-compact-1.8.1/setup.py
+-rw-r--r--   0        0        0     6857 2023-06-29 18:13:16.118955 voicemeeter-compact-1.8.1/PKG-INFO
```

### Comparing `voicemeeter-compact-1.8.0/LICENSE` & `voicemeeter-compact-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/pyproject.toml` & `voicemeeter-compact-1.8.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-compact"
-version = "1.8.0"
+version = "1.8.1"
 description = "A Compact Voicemeeter Remote App"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-compact"
 
 packages = [{ include = "vmcompact" }]
@@ -15,12 +15,12 @@
 sv-ttk = "^2.5.1"
 tomli = { version = "^2.0.1", python = "<3.11" }
 voicemeeter-api = "^2.0.2"
 vban-cmd = "^2.0.0"
 
 [tool.poetry.dev-dependencies]
 black = { version = "^22.6.0", allow-prereleases = true }
-isort = "^5.12.0"
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `voicemeeter-compact-1.8.0/README.md` & `voicemeeter-compact-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/vmcompact/app.py` & `voicemeeter-compact-1.8.1/vmcompact/app.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/vmcompact/banner.py` & `voicemeeter-compact-1.8.1/vmcompact/banner.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/vmcompact/builders.py` & `voicemeeter-compact-1.8.1/vmcompact/builders.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/vmcompact/channels.py` & `voicemeeter-compact-1.8.1/vmcompact/channels.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/vmcompact/config.py` & `voicemeeter-compact-1.8.1/vmcompact/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/vmcompact/configurations.py` & `voicemeeter-compact-1.8.1/vmcompact/configurations.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,16 +55,21 @@
     },
     "submixes": {
         "default": 0,
     },
     "navigation": {"show": True},
 }
 
+
 if "app" in configuration:
-    configuration["app"] = _defaults | configuration["app"]
+    for key in _defaults:
+        if key in configuration["app"]:
+            configuration["app"][key] = _defaults[key] | configuration["app"][key]
+        else:
+            configuration["app"][key] = _defaults[key]
 else:
     configuration["app"] = _defaults
 
 
 def get_configuration(key):
     if key in configuration:
         return configuration[key]
```

### Comparing `voicemeeter-compact-1.8.0/vmcompact/data.py` & `voicemeeter-compact-1.8.1/vmcompact/data.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/vmcompact/gainlayer.py` & `voicemeeter-compact-1.8.1/vmcompact/gainlayer.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/vmcompact/img/cat.ico` & `voicemeeter-compact-1.8.1/vmcompact/img/cat.ico`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/vmcompact/menu.py` & `voicemeeter-compact-1.8.1/vmcompact/menu.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/vmcompact/navigation.py` & `voicemeeter-compact-1.8.1/vmcompact/navigation.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/vmcompact/subject.py` & `voicemeeter-compact-1.8.1/vmcompact/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.0/setup.py` & `voicemeeter-compact-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'voicemeeter-api>=2.0.2,<3.0.0']
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'voicemeeter-compact',
-    'version': '1.8.0',
+    'version': '1.8.1',
     'description': 'A Compact Voicemeeter Remote App',
     'long_description': '[![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![OS: Windows](https://img.shields.io/badge/os-windows-red)\n\n![Image of app/potato size comparison](./doc_imgs/potatocomparisonsmaller.png)\n\n# Voicemeeter Compact\n\nA compact Voicemeeter remote app, works locally and over LAN.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Prerequisites\n\n-   [Voicemeeter](https://voicemeeter.com/) (Basic v1.0.8.4), (Banana v2.0.6.4) or (Potato v3.0.2.4)\n-   Python 3.10 or greater\n\n## Installation\n\nFor a step-by-step guide [click here](INSTALLATION.md)\n\n```\npip install voicemeeter-compact\n```\n\n## Usage\n\nExample `__main__.py` file:\n\n```python\nimport voicemeeterlib\nimport vmcompact\n\n\ndef main():\n    # pass the kind_id and the vm object to the app\n    with voicemeeterlib.api(kind_id) as vm:\n        app = vmcompact.connect(kind_id, vm)\n        app.mainloop()\n\n\nif __name__ == "__main__":\n    # choose the kind of Voicemeeter (Local connection)\n    kind_id = "banana"\n\n    main()\n```\n\nIt\'s important to know that only labelled strips and buses will appear in the Channel frames. Removing a Channels label will cause the GUI to grow/shrink in real time.\n\n![Image of unlabelled app](./doc_imgs/nolabels.png)\n\nIf the GUI looks like the above when you first load it, then no channels are labelled. From the menu, `Configs->Load config` you may load an example config. Save your current Voicemeeter settings first :).\n\n### kind_id\n\nSet the kind of Voicemeeter, kind_id may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## TOML Files\n\nThis is how your files should be organised. Wherever your `__main__.py` file is located (after install this can be any location), `configs` should be in the same location.\nDirectly inside of configs directory you may place an app.toml, vban.toml and a directory for each kind.\nInside each kind directory you may place as many custom toml configurations as you wish.\n\n.\n\n├── `__main__.py`\n\n├── configs\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── app.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── vban.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── basic\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other_config.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── streaming_config.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── banana\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── potato\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...\n\n## Configs\n\n### app.toml\n\nConfigure certain startup states for the app.\n\n-   `configs`\n    Configure a user config to load on app startup. Don\'t include the .toml extension in the config name.\n\n-   `theme`\n    By default the app loads up the [Sun Valley light or dark theme](https://github.com/rdbende/Sun-Valley-ttk-theme) by @rdbende. You have the option to load up the app without any theme loaded. Simply set `enabled` to false and `mode` will take no effect.\n\n-   `extends`\n    Extending the app will show both strips and buses. In reduced mode only one or the other. This app will extend both horizontally and vertically, simply set `extends_horizontal` true or false accordingly.\n\n-   `channel`\n    For each channel labelframe the width and height may be adjusted which effects the spacing between widgets and the length of the scales and progressbars respectively.\n\n-   `mwscroll_step`\n    Sets the amount (in db) the gain slider moves with a single mousewheel step. Default 3.\n\n-   `submixes`\n    Select the default submix bus when Submix frame is shown. For example, a dedicated bus for OBS.\n\n### vban.toml\n\nConfigure as many vban connections as you wish. This allows the app to work over a LAN connection as well as with a local Voicemeeter installation.\n\nFor vban connections to work correctly VBAN TEXT incoming stream MUST be configured correctly on the remote machine. Both pcs ought to be connected to a local private network and should be able to ping one another.\n\nA valid `vban.toml` might look like this:\n\n```toml\n[connection-1]\nkind = \'banana\'\nip = \'192.168.1.2\'\nstreamname = \'worklaptop\'\nport = 6980\n\n[connection-2]\nkind = \'potato\'\nip = \'192.168.1.3\'\nstreamname = \'streampc\'\nport = 6990\n```\n\n### basic/ banana/ potato/\n\nThree example user configs are included with the package, one for each kind of Voicemeeter. Use these to configure parameter startup states. Any parameter supported by the underlying interfaces may be used. Check the \'multiple-parameters\' section for more info:\n\n[Python Interface for Voicemeeter API](https://github.com/onyx-and-iris/voicemeeter-api-python#multiple-parameters)\n\n[Python Interface for VBAN CMD](https://github.com/onyx-and-iris/vban-cmd-python#multiple-parameters)\n\nUser configs may be loaded at any time via the menu.\n\n## Special Thanks\n\n[Vincent Burel](https://github.com/vburel2018) for creating Voicemeeter, its SDK, the C Remote API, the RT Packet service and Streamer View app!\n\n[Rdbende](https://github.com/rdbende) for creating the beautiful Sun Valley Tkinter theme and adding it to Pypi!\n',
     'author': 'onyx-and-iris',
     'author_email': 'code@onyxandiris.online',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/onyx-and-iris/voicemeeter-compact',
```

### Comparing `voicemeeter-compact-1.8.0/PKG-INFO` & `voicemeeter-compact-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-compact
-Version: 1.8.0
+Version: 1.8.1
 Summary: A Compact Voicemeeter Remote App
 Home-page: https://github.com/onyx-and-iris/voicemeeter-compact
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

