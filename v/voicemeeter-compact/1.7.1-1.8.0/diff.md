# Comparing `tmp/voicemeeter-compact-1.7.1.tar.gz` & `tmp/voicemeeter-compact-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter-compact-1.7.1.tar", max compression
+gzip compressed data, was "voicemeeter-compact-1.8.0.tar", max compression
```

## Comparing `voicemeeter-compact-1.7.1.tar` & `voicemeeter-compact-1.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter-compact-1.7.1/LICENSE
--rw-r--r--   0        0        0      729 2023-06-26 15:07:46.680784 voicemeeter-compact-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter-compact-1.7.1/README.md
--rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter-compact-1.7.1/vmcompact/__init__.py
--rw-r--r--   0        0        0     4248 2023-06-26 14:34:16.801058 voicemeeter-compact-1.7.1/vmcompact/app.py
--rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter-compact-1.7.1/vmcompact/banner.py
--rw-r--r--   0        0        0    23293 2023-06-25 22:00:45.712304 voicemeeter-compact-1.7.1/vmcompact/builders.py
--rw-r--r--   0        0        0    10827 2023-06-24 21:16:46.007160 voicemeeter-compact-1.7.1/vmcompact/channels.py
--rw-r--r--   0        0        0     9634 2023-06-26 08:40:26.219945 voicemeeter-compact-1.7.1/vmcompact/config.py
--rw-r--r--   0        0        0     2438 2023-06-26 15:00:20.558979 voicemeeter-compact-1.7.1/vmcompact/configurations.py
--rw-r--r--   0        0        0     1882 2022-09-15 22:41:23.144367 voicemeeter-compact-1.7.1/vmcompact/data.py
--rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter-compact-1.7.1/vmcompact/errors.py
--rw-r--r--   0        0        0     8878 2023-06-24 22:19:08.257020 voicemeeter-compact-1.7.1/vmcompact/gainlayer.py
--rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter-compact-1.7.1/vmcompact/img/cat.ico
--rw-r--r--   0        0        0    16124 2023-06-26 14:51:26.442226 voicemeeter-compact-1.7.1/vmcompact/menu.py
--rw-r--r--   0        0        0     3705 2023-06-26 08:38:15.234618 voicemeeter-compact-1.7.1/vmcompact/navigation.py
--rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter-compact-1.7.1/vmcompact/subject.py
--rw-r--r--   0        0        0     7183 2023-06-26 15:09:12.001068 voicemeeter-compact-1.7.1/setup.py
--rw-r--r--   0        0        0     6857 2023-06-26 15:09:12.001068 voicemeeter-compact-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter-compact-1.8.0/LICENSE
+-rw-r--r--   0        0        0      729 2023-06-29 17:10:11.382512 voicemeeter-compact-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter-compact-1.8.0/README.md
+-rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter-compact-1.8.0/vmcompact/__init__.py
+-rw-r--r--   0        0        0     4644 2023-06-29 17:12:44.240157 voicemeeter-compact-1.8.0/vmcompact/app.py
+-rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter-compact-1.8.0/vmcompact/banner.py
+-rw-r--r--   0        0        0    23309 2023-06-29 11:15:56.815136 voicemeeter-compact-1.8.0/vmcompact/builders.py
+-rw-r--r--   0        0        0    10867 2023-06-29 10:15:56.869547 voicemeeter-compact-1.8.0/vmcompact/channels.py
+-rw-r--r--   0        0        0     9634 2023-06-26 08:40:26.219945 voicemeeter-compact-1.8.0/vmcompact/config.py
+-rw-r--r--   0        0        0     2497 2023-06-29 10:49:39.208371 voicemeeter-compact-1.8.0/vmcompact/configurations.py
+-rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter-compact-1.8.0/vmcompact/data.py
+-rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter-compact-1.8.0/vmcompact/errors.py
+-rw-r--r--   0        0        0     8960 2023-06-29 10:16:01.341472 voicemeeter-compact-1.8.0/vmcompact/gainlayer.py
+-rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter-compact-1.8.0/vmcompact/img/cat.ico
+-rw-r--r--   0        0        0    17472 2023-06-29 11:09:26.649143 voicemeeter-compact-1.8.0/vmcompact/menu.py
+-rw-r--r--   0        0        0     3785 2023-06-29 10:52:07.632943 voicemeeter-compact-1.8.0/vmcompact/navigation.py
+-rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter-compact-1.8.0/vmcompact/subject.py
+-rw-r--r--   0        0        0     7183 2023-06-29 17:25:10.583826 voicemeeter-compact-1.8.0/setup.py
+-rw-r--r--   0        0        0     6857 2023-06-29 17:25:10.584801 voicemeeter-compact-1.8.0/PKG-INFO
```

### Comparing `voicemeeter-compact-1.7.1/LICENSE` & `voicemeeter-compact-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.1/pyproject.toml` & `voicemeeter-compact-1.8.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "voicemeeter-compact"
-version = "1.7.1"
+version = "1.8.0"
 description = "A Compact Voicemeeter Remote App"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-compact"
 
 packages = [{ include = "vmcompact" }]
 include = ["vmcompact/img/cat.ico"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-sv-ttk = "^2.4.5"
+sv-ttk = "^2.5.1"
 tomli = { version = "^2.0.1", python = "<3.11" }
-voicemeeter-api = "^2.0.1"
+voicemeeter-api = "^2.0.2"
 vban-cmd = "^2.0.0"
 
 [tool.poetry.dev-dependencies]
 black = { version = "^22.6.0", allow-prereleases = true }
 isort = "^5.12.0"
 
 [build-system]
```

### Comparing `voicemeeter-compact-1.7.1/README.md` & `voicemeeter-compact-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.1/vmcompact/app.py` & `voicemeeter-compact-1.8.0/vmcompact/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+import logging
 import tkinter as tk
 from functools import cached_property
 from pathlib import Path
 from tkinter import ttk
 from typing import NamedTuple
 
 from .builders import MainFrameBuilder
 from .configurations import loader
 from .data import _base_values, _configuration, _kinds_all
 from .errors import VMCompactError
 from .menu import Menus
 from .subject import Subject
 
+logger = logging.getLogger(__name__)
+
 
 class App(tk.Tk):
     """App mainframe"""
 
     @classmethod
     def make(cls, kind: NamedTuple):
         """
@@ -30,17 +33,18 @@
                 "kind": kind,
             },
         )
         return APP_cls
 
     def __init__(self, vmr):
         super().__init__()
-
+        self.logger = logger.getChild(self.__class__.__name__)
         self._vmr = vmr
         self._vmr.event.add(["pdirty", "ldirty"])
+        self.after(12000 if self._vmr.gui.launched_by_api else 1, self.start_updates)
         self._vmr.init_thread()
         icon_path = Path(__file__).parent.resolve() / "img" / "cat.ico"
         if icon_path.is_file():
             self.iconbitmap(str(icon_path))
         self.minsize(275, False)
         self.subject = Subject()
         self._configs = None
@@ -50,14 +54,20 @@
             vmr.apply_config(_configuration.config)
 
         self.build_app()
 
         self.drag_id = ""
         self.bind("<Configure>", self.dragging)
 
+    def start_updates(self):
+        self.logger.debug("updates started")
+        _base_values.run_update = True
+        if self._vmr.gui.launched_by_api:
+            self.on_pdirty()
+
     def __str__(self):
         return f"{type(self).__name__}App"
 
     @property
     def target(self):
         """returns the current interface"""
```

### Comparing `voicemeeter-compact-1.7.1/vmcompact/banner.py` & `voicemeeter-compact-1.8.0/vmcompact/banner.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.1/vmcompact/builders.py` & `voicemeeter-compact-1.8.0/vmcompact/builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,17 +191,17 @@
     def grid_configure(self):
         [
             child.grid_configure(padx=1, pady=1, sticky=(tk.N, tk.S, tk.W, tk.E))
             for child in self.navframe.winfo_children()
             if isinstance(child, ttk.Checkbutton)
         ]
         if _configuration.themes_enabled:
-            self.navframe.rowconfigure(1, minsize=_configuration.level_height)
+            self.navframe.rowconfigure(1, minsize=_configuration.channel_height)
         else:
-            self.navframe.rowconfigure(1, minsize=_configuration.level_height + 10)
+            self.navframe.rowconfigure(1, minsize=_configuration.channel_height + 10)
 
     def teardown(self):
         pass
 
 
 class ChannelLabelFrameBuilder(AbstractBuilder):
     """Responsible for building channel labelframe widgets"""
@@ -239,15 +239,15 @@
         self.scale = ttk.Scale(
             self.labelframe,
             from_=12.0,
             to=-60.0,
             orient="vertical",
             variable=self.labelframe.gain,
             command=self.labelframe.scale_callback,
-            length=_configuration.level_height,
+            length=_configuration.channel_height,
         )
         self.scale.grid(column=1, row=0)
         self.scale.bind("<Double-Button-1>", self.labelframe.reset_gain)
         self.scale.bind("<Button-1>", self.labelframe.scale_press)
         self.scale.bind("<ButtonRelease-1>", self.labelframe.scale_release)
         self.scale.bind("<MouseWheel>", self.labelframe._on_mousewheel)
 
@@ -320,15 +320,15 @@
         [
             child.grid_configure(padx=1, pady=1, sticky=(tk.W, tk.E))
             for child in self.configframe.winfo_children()
             if isinstance(child, ttk.Checkbutton)
         ]
         self.configframe.grid(sticky=(tk.W))
         [
-            self.configframe.columnconfigure(i, minsize=_configuration.level_width)
+            self.configframe.columnconfigure(i, minsize=_configuration.channel_width)
             for i in range(self.configframe.phys_out + self.configframe.virt_out)
         ]
 
 
 class StripConfigFrameBuilder(ChannelConfigFrameBuilder):
     """Responsible for building channel configframe widgets"""
 
@@ -388,15 +388,15 @@
     def create_comp_slider(self):
         comp_label = ttk.Label(self.configframe, text="Comp")
         comp_scale = ttk.Scale(
             self.configframe,
             from_=0.0,
             to=10.0,
             orient="horizontal",
-            length=_configuration.level_width,
+            length=_configuration.channel_width,
             variable=self.configframe.slider_vars[
                 self.configframe.slider_params.index("comp.knob")
             ],
             command=partial(self.configframe.scale_callback, "comp.knob"),
         )
         comp_scale.bind(
             "<Double-Button-1>", partial(self.configframe.reset_scale, "comp.knob", 0)
@@ -412,15 +412,15 @@
     def create_gate_slider(self):
         gate_label = ttk.Label(self.configframe, text="Gate")
         gate_scale = ttk.Scale(
             self.configframe,
             from_=0.0,
             to=10.0,
             orient="horizontal",
-            length=_configuration.level_width,
+            length=_configuration.channel_width,
             variable=self.configframe.slider_vars[
                 self.configframe.slider_params.index("gate.knob")
             ],
             command=partial(self.configframe.scale_callback, "gate.knob"),
         )
         gate_scale.bind(
             "<Double-Button-1>", partial(self.configframe.reset_scale, "gate.knob", 0)
@@ -436,15 +436,15 @@
     def create_limit_slider(self):
         limit_label = ttk.Label(self.configframe, text="Limit")
         limit_scale = ttk.Scale(
             self.configframe,
             from_=-40,
             to=12,
             orient="horizontal",
-            length=_configuration.level_width,
+            length=_configuration.channel_width,
             variable=self.configframe.slider_vars[
                 self.configframe.slider_params.index("limit")
             ],
             command=partial(self.configframe.scale_callback, "limit"),
         )
         limit_scale.bind(
             "<Double-Button-1>", partial(self.configframe.reset_scale, "limit", 12)
@@ -460,15 +460,15 @@
     def create_audibility_slider(self):
         aud_label = ttk.Label(self.configframe, text="Audibility")
         aud_scale = ttk.Scale(
             self.configframe,
             from_=0.0,
             to=10.0,
             orient="horizontal",
-            length=_configuration.level_width,
+            length=_configuration.channel_width,
             variable=self.configframe.slider_vars[
                 self.configframe.slider_params.index("audibility")
             ],
             command=partial(self.configframe.scale_callback, "audibility"),
         )
         aud_scale.bind(
             "<Double-Button-1>", partial(self.configframe.reset_scale, "audibility", 0)
```

### Comparing `voicemeeter-compact-1.7.1/vmcompact/channels.py` & `voicemeeter-compact-1.8.0/vmcompact/channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             self.grid_remove()
         else:
             self.parent.parent.subject.add(self)
             self.grid()
         self.configure(text=retval)
 
     def grid_configure(self):
-        self.grid(sticky=(tk.N, tk.S))
+        self.grid(padx=_configuration.channel_xpadding, sticky=(tk.N, tk.S))
         [
             child.grid_configure(padx=1, pady=1, sticky=(tk.W, tk.E))
             for child in self.winfo_children()
             if isinstance(child, ttk.Checkbutton)
         ]
         [
             child.grid_configure(padx=1, pady=1, sticky=(tk.N, tk.S))
@@ -254,15 +254,15 @@
             num = getattr(self.parent.kind, f"num_{self.id}")
             if self.label_cache[self.id] != [target[i].label for i in range(num)]:
                 for labelframe in self.labelframes:
                     labelframe.on_update("labelframe")
 
     def grid_configure(self):
         [
-            self.columnconfigure(i, minsize=_configuration.level_width)
+            self.columnconfigure(i, minsize=_configuration.channel_width)
             for i, _ in enumerate(self.labelframes)
         ]
         [self.rowconfigure(0, minsize=100) for i, _ in enumerate(self.labelframes)]
 
     def teardown(self):
         [self.parent.subject.remove(frame) for frame in self.labelframes]
         self.parent.subject.remove(self)
```

### Comparing `voicemeeter-compact-1.7.1/vmcompact/config.py` & `voicemeeter-compact-1.8.0/vmcompact/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.1/vmcompact/configurations.py` & `voicemeeter-compact-1.8.0/vmcompact/configurations.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,21 +44,23 @@
     "extends": {
         "extended": True,
         "extends_horizontal": True,
     },
     "channel": {
         "width": 80,
         "height": 130,
+        "xpadding": 3,
     },
     "mwscroll_step": {
         "size": 3,
     },
     "submixes": {
         "default": 0,
     },
+    "navigation": {"show": True},
 }
 
 if "app" in configuration:
     configuration["app"] = _defaults | configuration["app"]
 else:
     configuration["app"] = _defaults
```

### Comparing `voicemeeter-compact-1.7.1/vmcompact/data.py` & `voicemeeter-compact-1.8.0/vmcompact/data.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,29 +28,34 @@
     # light or dark
     theme_mode: str = configuration["theme"]["mode"]
     # size of mousewheel scroll step
     mwscroll_step: int = configuration["mwscroll_step"]["size"]
     # bus assigned as current submix
     submixes: int = configuration["submixes"]["default"]
 
-    # width of a single labelframe
-    level_width: int = configuration["channel"]["width"]
-    # height of a single labelframe
-    level_height: int = configuration["channel"]["height"]
+    # width of a single channel labelframe
+    channel_width: int = configuration["channel"]["width"]
+    # height of a single channel labelframe
+    channel_height: int = configuration["channel"]["height"]
+    # xpadding for a single channel labelframe
+    channel_xpadding: int = configuration["channel"]["xpadding"]
+
+    # do we grid the navigation frame?
+    navigation_show: bool = configuration["navigation"]["show"]
 
     @property
     def config(self):
         if "configs" in configuration:
             return configuration["configs"]["config"]
 
 
 @dataclass
 class BaseValues(metaclass=SingletonMeta):
     # pause updates after releasing scale
-    run_update: bool = True
+    run_update: bool = False
     # are we dragging main window with mouse 1
     dragging: bool = False
     # a vban connection established
     vban_connected: bool = False
 
 
 _base_values = BaseValues()
```

### Comparing `voicemeeter-compact-1.7.1/vmcompact/gainlayer.py` & `voicemeeter-compact-1.8.0/vmcompact/gainlayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
                     if self.parent.parent.strip_frame.strips[self.index].mute.get()
                     or not self.on.get()
                     else 72 + val - 12 + self.gain.get()
                 )
             )
 
     def grid_configure(self):
+        self.grid(padx=_configuration.channel_xpadding, sticky=(tk.N, tk.S))
         [
             child.grid_configure(padx=1, pady=1, sticky=(tk.N, tk.S, tk.W, tk.E))
             for child in self.winfo_children()
             if isinstance(child, ttk.Checkbutton)
         ]
         [
             child.grid_configure(padx=1, pady=1, sticky=(tk.N, tk.S))
@@ -249,19 +250,19 @@
     def on_update(self, subject):
         if subject == "pdirty":
             for labelframe in self.labelframes:
                 labelframe.on_update("labelframe")
 
     def grid_configure(self):
         [
-            self.columnconfigure(i, minsize=_configuration.level_width)
+            self.columnconfigure(i, minsize=_configuration.channel_width)
             for i, _ in enumerate(self.labelframes)
         ]
         [
-            self.rowconfigure(0, minsize=_configuration.level_height)
+            self.rowconfigure(0, minsize=_configuration.channel_height)
             for i, _ in enumerate(self.labelframes)
         ]
 
     def teardown(self):
         # deregisters submixframe as pdirty observer
         [self.parent.subject.remove(frame) for frame in self.gainlayers]
         self.parent.subject.remove(self)
```

### Comparing `voicemeeter-compact-1.7.1/vmcompact/img/cat.ico` & `voicemeeter-compact-1.8.0/vmcompact/img/cat.ico`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.1/vmcompact/menu.py` & `voicemeeter-compact-1.8.0/vmcompact/menu.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         self.vmr = vmr
         self.logger = logger.getChild(self.__class__.__name__)
         self.vban_config = get_configuration("vban")
         self.app_config = get_configuration("app")
         self._is_topmost = tk.BooleanVar()
         self._lock = tk.BooleanVar()
         self._unlock = tk.BooleanVar()
+        self._navigation_show = tk.BooleanVar(value=_configuration.navigation_show)
+        self._navigation_hide = tk.BooleanVar(value=not _configuration.navigation_show)
         self._selected_bus = list(tk.BooleanVar() for _ in range(8))
 
         # voicemeeter menu
         self.menu_voicemeeter = tk.Menu(self, tearoff=0)
         self.add_cascade(menu=self.menu_voicemeeter, label="Voicemeeter")
         self.menu_voicemeeter.add_checkbutton(
             label="Always On Top",
@@ -158,14 +160,31 @@
         )
         self.menu_themes.entryconfig(
             0 if self.app_config["theme"]["mode"] == "light" else 1,
             state="disabled",
         )
         if not _configuration.themes_enabled:
             self.menu_layout.entryconfig(2, state="disabled")
+        # layout/navigation
+        self.menu_navigation = tk.Menu(self.menu_layout, tearoff=0)
+        self.menu_layout.add_cascade(menu=self.menu_navigation, label="Navigation")
+        self.menu_navigation.add_checkbutton(
+            label="show",
+            onvalue=1,
+            offvalue=0,
+            variable=self._navigation_show,
+            command=partial(self.toggle_navigation, "show"),
+        )
+        self.menu_navigation.add_checkbutton(
+            label="hide",
+            onvalue=1,
+            offvalue=0,
+            variable=self._navigation_hide,
+            command=partial(self.toggle_navigation, "hide"),
+        )
 
         # vban connect menu
         self.menu_vban = tk.Menu(self, tearoff=0)
         self.add_cascade(menu=self.menu_vban, label="VBAN")
         if self.vban_config:
             for i, _ in enumerate(self.vban_config):
                 setattr(self, f"menu_vban_{i+1}", tk.Menu(self.menu_vban, tearoff=0))
@@ -331,14 +350,26 @@
                 )
                 for name, data in self.parent.userconfigs.items()
                 if name not in self.config_defaults
             ]
         else:
             self.menu_configs.entryconfig(0, state="disabled")
 
+    def toggle_navigation(self, cmd=None):
+        if cmd == "show":
+            self.logger.debug("show navframe")
+            self.parent.nav_frame.grid()
+            self._navigation_show.set(True)
+            self._navigation_hide.set(not self._navigation_show.get())
+        else:
+            self.logger.debug("hide navframe")
+            self.parent.nav_frame.grid_remove()
+            self._navigation_hide.set(True)
+            self._navigation_show.set(not self._navigation_hide.get())
+
     def vban_connect(self, i):
         opts = {}
         opts |= self.vban_config[f"connection-{i+1}"]
         kind_id = opts.pop("kind")
         self.vban = vban_cmd.api(kind_id, **opts)
         # login to vban interface
         try:
```

### Comparing `voicemeeter-compact-1.7.1/vmcompact/navigation.py` & `voicemeeter-compact-1.8.0/vmcompact/navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 class Navigation(ttk.Frame):
     def __init__(self, parent):
         super().__init__(parent)
         self.parent = parent
         self.logger = logger.getChild(self.__class__.__name__)
         self.grid(row=0, column=3, padx=(0, 2), pady=(5, 5), sticky=(tk.W, tk.E))
+        if not _configuration.navigation_show:
+            self.grid_remove()
         self.styletable = self.parent.styletable
 
         self.builder = builders.NavigationFrameBuilder(self)
         self.builder.setup()
         self.builder.create_submix_button()
         self.builder.create_channel_button()
         self.builder.create_extend_button()
```

### Comparing `voicemeeter-compact-1.7.1/vmcompact/subject.py` & `voicemeeter-compact-1.8.0/vmcompact/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.1/setup.py` & `voicemeeter-compact-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 packages = \
 ['vmcompact']
 
 package_data = \
 {'': ['*'], 'vmcompact': ['img/*']}
 
 install_requires = \
-['sv-ttk>=2.4.5,<3.0.0',
+['sv-ttk>=2.5.1,<3.0.0',
  'vban-cmd>=2.0.0,<3.0.0',
- 'voicemeeter-api>=2.0.1,<3.0.0']
+ 'voicemeeter-api>=2.0.2,<3.0.0']
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'voicemeeter-compact',
-    'version': '1.7.1',
+    'version': '1.8.0',
     'description': 'A Compact Voicemeeter Remote App',
     'long_description': '[![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![OS: Windows](https://img.shields.io/badge/os-windows-red)\n\n![Image of app/potato size comparison](./doc_imgs/potatocomparisonsmaller.png)\n\n# Voicemeeter Compact\n\nA compact Voicemeeter remote app, works locally and over LAN.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Prerequisites\n\n-   [Voicemeeter](https://voicemeeter.com/) (Basic v1.0.8.4), (Banana v2.0.6.4) or (Potato v3.0.2.4)\n-   Python 3.10 or greater\n\n## Installation\n\nFor a step-by-step guide [click here](INSTALLATION.md)\n\n```\npip install voicemeeter-compact\n```\n\n## Usage\n\nExample `__main__.py` file:\n\n```python\nimport voicemeeterlib\nimport vmcompact\n\n\ndef main():\n    # pass the kind_id and the vm object to the app\n    with voicemeeterlib.api(kind_id) as vm:\n        app = vmcompact.connect(kind_id, vm)\n        app.mainloop()\n\n\nif __name__ == "__main__":\n    # choose the kind of Voicemeeter (Local connection)\n    kind_id = "banana"\n\n    main()\n```\n\nIt\'s important to know that only labelled strips and buses will appear in the Channel frames. Removing a Channels label will cause the GUI to grow/shrink in real time.\n\n![Image of unlabelled app](./doc_imgs/nolabels.png)\n\nIf the GUI looks like the above when you first load it, then no channels are labelled. From the menu, `Configs->Load config` you may load an example config. Save your current Voicemeeter settings first :).\n\n### kind_id\n\nSet the kind of Voicemeeter, kind_id may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## TOML Files\n\nThis is how your files should be organised. Wherever your `__main__.py` file is located (after install this can be any location), `configs` should be in the same location.\nDirectly inside of configs directory you may place an app.toml, vban.toml and a directory for each kind.\nInside each kind directory you may place as many custom toml configurations as you wish.\n\n.\n\n├── `__main__.py`\n\n├── configs\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── app.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── vban.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── basic\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other_config.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── streaming_config.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── banana\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── potato\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...\n\n## Configs\n\n### app.toml\n\nConfigure certain startup states for the app.\n\n-   `configs`\n    Configure a user config to load on app startup. Don\'t include the .toml extension in the config name.\n\n-   `theme`\n    By default the app loads up the [Sun Valley light or dark theme](https://github.com/rdbende/Sun-Valley-ttk-theme) by @rdbende. You have the option to load up the app without any theme loaded. Simply set `enabled` to false and `mode` will take no effect.\n\n-   `extends`\n    Extending the app will show both strips and buses. In reduced mode only one or the other. This app will extend both horizontally and vertically, simply set `extends_horizontal` true or false accordingly.\n\n-   `channel`\n    For each channel labelframe the width and height may be adjusted which effects the spacing between widgets and the length of the scales and progressbars respectively.\n\n-   `mwscroll_step`\n    Sets the amount (in db) the gain slider moves with a single mousewheel step. Default 3.\n\n-   `submixes`\n    Select the default submix bus when Submix frame is shown. For example, a dedicated bus for OBS.\n\n### vban.toml\n\nConfigure as many vban connections as you wish. This allows the app to work over a LAN connection as well as with a local Voicemeeter installation.\n\nFor vban connections to work correctly VBAN TEXT incoming stream MUST be configured correctly on the remote machine. Both pcs ought to be connected to a local private network and should be able to ping one another.\n\nA valid `vban.toml` might look like this:\n\n```toml\n[connection-1]\nkind = \'banana\'\nip = \'192.168.1.2\'\nstreamname = \'worklaptop\'\nport = 6980\n\n[connection-2]\nkind = \'potato\'\nip = \'192.168.1.3\'\nstreamname = \'streampc\'\nport = 6990\n```\n\n### basic/ banana/ potato/\n\nThree example user configs are included with the package, one for each kind of Voicemeeter. Use these to configure parameter startup states. Any parameter supported by the underlying interfaces may be used. Check the \'multiple-parameters\' section for more info:\n\n[Python Interface for Voicemeeter API](https://github.com/onyx-and-iris/voicemeeter-api-python#multiple-parameters)\n\n[Python Interface for VBAN CMD](https://github.com/onyx-and-iris/vban-cmd-python#multiple-parameters)\n\nUser configs may be loaded at any time via the menu.\n\n## Special Thanks\n\n[Vincent Burel](https://github.com/vburel2018) for creating Voicemeeter, its SDK, the C Remote API, the RT Packet service and Streamer View app!\n\n[Rdbende](https://github.com/rdbende) for creating the beautiful Sun Valley Tkinter theme and adding it to Pypi!\n',
     'author': 'onyx-and-iris',
     'author_email': 'code@onyxandiris.online',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/onyx-and-iris/voicemeeter-compact',
```

### Comparing `voicemeeter-compact-1.7.1/PKG-INFO` & `voicemeeter-compact-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: voicemeeter-compact
-Version: 1.7.1
+Version: 1.8.0
 Summary: A Compact Voicemeeter Remote App
 Home-page: https://github.com/onyx-and-iris/voicemeeter-compact
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: sv-ttk (>=2.4.5,<3.0.0)
+Requires-Dist: sv-ttk (>=2.5.1,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0); python_version < "3.11"
 Requires-Dist: vban-cmd (>=2.0.0,<3.0.0)
-Requires-Dist: voicemeeter-api (>=2.0.1,<3.0.0)
+Requires-Dist: voicemeeter-api (>=2.0.2,<3.0.0)
 Project-URL: Repository, https://github.com/onyx-and-iris/voicemeeter-compact
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![OS: Windows](https://img.shields.io/badge/os-windows-red)
```

