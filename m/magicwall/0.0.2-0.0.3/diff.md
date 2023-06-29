# Comparing `tmp/magicwall-0.0.2.tar.gz` & `tmp/magicwall-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicwall-0.0.2.tar", max compression
+gzip compressed data, was "magicwall-0.0.3.tar", max compression
```

## Comparing `magicwall-0.0.2.tar` & `magicwall-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     5121 2022-10-31 15:47:06.221205 magicwall-0.0.2/Readme.md
--rw-r--r--   0        0        0       45 2023-05-22 06:01:44.639872 magicwall-0.0.2/magicwall/__init__.py
--rw-r--r--   0        0        0      451 2023-06-18 12:57:55.403215 magicwall-0.0.2/magicwall/common.py
--rw-r--r--   0        0        0     1437 2023-06-18 12:57:55.403215 magicwall-0.0.2/magicwall/magicwall_api.py
--rwxr-xr-x   0        0        0    14248 2023-06-18 13:50:08.843120 magicwall-0.0.2/magicwall/server.py
--rw-r--r--   0        0        0    21604 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/static/DragDropTouch.js
--rw-r--r--   0        0        0     5119 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/static/hilite-solarized-light.css
--rw-r--r--   0        0        0     1785 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/static/magicwall.css
--rw-r--r--   0        0        0    16993 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/static/magicwall.js
--rw-r--r--   0        0        0     3600 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/static/unknown.png
--rw-r--r--   0        0        0     1095 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/templates/magicwall.html
--rw-r--r--   0        0        0     2132 2023-06-18 13:52:12.703419 magicwall-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5986 1970-01-01 00:00:00.000000 magicwall-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     5185 2023-06-29 18:49:22.931538 magicwall-0.0.3/Readme.md
+-rw-r--r--   0        0        0      131 2023-06-29 18:49:22.932538 magicwall-0.0.3/magicwall/Dockerfile
+-rw-r--r--   0        0        0       45 2023-06-29 18:49:22.932538 magicwall-0.0.3/magicwall/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-29 18:49:22.932538 magicwall-0.0.3/magicwall/common.py
+-rw-r--r--   0        0        0     1437 2023-06-29 18:49:22.932538 magicwall-0.0.3/magicwall/magicwall_api.py
+-rwxr-xr-x   0        0        0    16662 2023-06-29 18:49:22.932538 magicwall-0.0.3/magicwall/server.py
+-rw-r--r--   0        0        0    21604 2023-06-29 18:49:22.933538 magicwall-0.0.3/magicwall/static/DragDropTouch.js
+-rw-r--r--   0        0        0     5119 2023-06-29 18:49:22.933538 magicwall-0.0.3/magicwall/static/hilite-solarized-light.css
+-rw-r--r--   0        0        0     1785 2023-06-29 18:49:22.933538 magicwall-0.0.3/magicwall/static/magicwall.css
+-rw-r--r--   0        0        0    16993 2023-06-29 18:49:22.933538 magicwall-0.0.3/magicwall/static/magicwall.js
+-rw-r--r--   0        0        0     3600 2023-06-29 18:49:22.933538 magicwall-0.0.3/magicwall/static/unknown.png
+-rw-r--r--   0        0        0     1095 2023-06-29 18:49:22.933538 magicwall-0.0.3/magicwall/templates/magicwall.html
+-rw-r--r--   0        0        0     4457 2023-06-29 18:49:22.933538 magicwall-0.0.3/magicwall/utils.py
+-rw-r--r--   0        0        0     2133 2023-06-29 18:50:30.832800 magicwall-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6052 1970-01-01 00:00:00.000000 magicwall-0.0.3/PKG-INFO
```

### Comparing `magicwall-0.0.2/Readme.md` & `magicwall-0.0.3/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 * [ ] Resize elments
 * [ ] Caching mechanism
 * [ ] Square-select multiple items
 
 
 ## Future
 
+* Notification on change
 * Fullscreen / slideshow mode
 * Undo-stack
 * Config-YAML
 * Filter-Hub
 * Search
 * Offline use
 * Git support
@@ -92,16 +93,18 @@
 * Algorithm demonstration / education (-> Jupyter)
 * File exchange
 * Note taking
 
 
 ## Magic ideas
 
+* Document optimizer
 * Simple auto optimize images (contrast, etc)
 * Simple BW images
+* Polaroid images
 * Configurable Image with roation, cropping, color improvement, vignetting
 * Files to animation
 * SVG background
 * Auto align by date
 * fetch URL -> return generated HTML
```

### Comparing `magicwall-0.0.2/magicwall/magicwall_api.py` & `magicwall-0.0.3/magicwall/magicwall_api.py`

 * *Files identical despite different names*

### Comparing `magicwall-0.0.2/magicwall/server.py` & `magicwall-0.0.3/magicwall/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  _ __ ___   __ _  __ _(_) _____      ____ _| | | (_) ___
 # | '_ ` _ \ / _` |/ _` | |/ __\ \ /\ / / _` | | | | |/ _ \
 # | | | | | | (_| | (_| | | (__ \ V  V / (_| | | |_| | (_) |
 # |_| |_| |_|\__,_|\__, |_|\___| \_/\_/ \__,_|_|_(_)_|\___/
 #                  |___/
 #
 # magicwall.io - a magic wall
-# Copyright (C) 2022 - Frans Fürst
+# Copyright (C) 2023 - Frans Fürst
 #
 # magicwall.io is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # magicwall.io is distributed in the hope that it will be useful, but WITHOUT
@@ -20,35 +20,43 @@
 # at <http://www.gnu.org/licenses/>.
 #
 
 """magicwall.io server implementation
 """
 
 import argparse
+import asyncio
 import json
+import logging
 import sys
 import tarfile
 import tempfile
 import threading
 import uuid
 from argparse import Namespace as Args
 from collections.abc import Mapping, MutableMapping, MutableSequence, Sequence
 from contextlib import suppress
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import cast
+from typing import Literal, cast
 
 import exifread
 import markdown
 import yaml
-from flask import Flask, Response, redirect, render_template, request, send_file
 from PIL import Image, UnidentifiedImageError
+from quart import Quart, Response, redirect, render_template, request, send_file
 from werkzeug.datastructures import FileStorage
 
 from magicwall.common import GenMap, GenMapArray, MutableGenMap, Tag
+from magicwall.utils import fs_changes, setup_logging, watchdog
+
+
+def log() -> logging.Logger:
+    """Logger for this module"""
+    return logging.getLogger("mw.server")
 
 
 @dataclass
 class File:
     """Models a file associated with an Item element"""
 
     name: str
@@ -62,14 +70,16 @@
         safe_name = store_file(name, wall, fileob)
         has_preview = Path(safe_name).suffix.lower() in {".png", ".jpg", ".gif", ".jpeg"}
         return File(name=name, safe_name=safe_name, preview_width="6cm" if has_preview else "1.5cm")
 
     @staticmethod
     def from_tree(tree: GenMap) -> "File":
         """Creates File element from untyped structure"""
+        if isinstance(tree, File):
+            return tree
         return File(
             name=str(tree["name"]),
             safe_name=str(tree["safe_name"]),
             hovertext=cast(str | None, tree.get("hovertext")),
             preview_width=cast(str | None, tree.get("preview_width")),
         )
 
@@ -77,22 +87,26 @@
 @dataclass
 class Item:
     """Models one visible element on a wall"""
 
     id: str  # pylint: disable=invalid-name
     pos: tuple[int, int]
     files: MutableSequence[File]
+    text_plain: str | None = None
+    text_html: str | None = None
 
     @staticmethod
     def from_tree(tree: GenMap) -> "Item":
         """Creates Item from untyped structure"""
         return Item(
             id=str(tree.get("id", uuid.uuid4())),
             pos=cast(tuple[int, int], tree.get("pos", [0, 0])),
             files=[File.from_tree(item) for item in cast(Sequence[GenMap], tree["files"])],
+            text_plain=cast(str | None, tree.get("text_plain") or tree.get("text/plain")),
+            text_html=cast(str | None, tree.get("text_html") or tree.get("text/html")),
         )
 
 
 @dataclass
 class Model:
     """Stores a magicwall model"""
 
@@ -114,22 +128,29 @@
     def from_tree(tree: GenMap) -> "Model":
         """Creates Model from untyped structure"""
         return Model(
             items=[Item.from_tree(cast(GenMap, item)) for item in cast(GenMapArray, tree["items"])]
         )
 
 
-def mw_representer(dumper: yaml.Dumper, data: object) -> yaml.nodes.Node:
+def to_external(data: GenMap) -> GenMap:
     """Makes some corrections to keys of dicts"""
-    return dumper.represent_dict(
+    return {
         {
-            {"preview_width": "preview-width"}.get(key, key): value
-            for key, value in data.__dict__.items()
-        }
-    )
+            "preview_width": "preview-width",
+            "text_plain": "text/plain",
+            "text_html": "text/html",
+        }.get(key, key): value
+        for key, value in data.items()
+    }
+
+
+def mw_representer(dumper: yaml.Dumper, data: object) -> yaml.nodes.Node:
+    """Makes some corrections to keys of dicts"""
+    return dumper.represent_dict(to_external(data.__dict__))
 
 
 def extract_tags(filename: str) -> Mapping[str, str]:
     """Reads interesting EXIF tags from given file"""
     # for PNG
     #  https://blender.stackexchange.com/questions/35504/read-image-metadata-from-python
     def extract_date(tags: Mapping[str, Tag]) -> str:
@@ -146,15 +167,18 @@
     """Interfaces one specific magicwall."""
 
     def __init__(self, wall_name: str) -> None:
         self._folder = app.config["UPLOAD_FOLDER"] / wall_name
         self._folder.mkdir(parents=True, exist_ok=True)
         self._model: Model = Model()
         self._lock = threading.Lock()
+        self.load()
 
+    def load(self) -> None:
+        """Read a wall from disk"""
         with self._lock:
             with suppress(FileNotFoundError):
                 try:
                     self._model = Model.from_yaml(self._folder / "model.yaml")
                 except FileNotFoundError:
                     self._model = Model.from_json(self._folder / "model.json")
                 for i in self._model.items:
@@ -173,40 +197,52 @@
     def model(self) -> Model:
         """RW access to the model structure"""
         return self._model
 
     def save(self) -> None:
         """Store to disk"""
         with self._lock:
+            path = self._folder / "_model.yaml"
+            log().debug("write wall model file %s", path)
             # make sure we don't delete data by stumbling over a failing save
-            with open(self._folder / "_model.yaml", "w", encoding="utf-8") as model_file:
+            with open(path, "w", encoding="utf-8") as model_file:
                 yaml.dump(self._model, model_file)
             (self._folder / "_model.yaml").rename(self._folder / "model.yaml")
 
     def add_item(self, item: Item) -> str:
         """Adds a visible item to the wall and saves the wall"""
         self._model.items.append(item)
         self.save()
         return item.id
 
+    def dirty(self) -> None:
+        """Does whatever is needed after a file inside a wall directory has been touched"""
+        self.load()
+
 
 class WallStore:
     """Singleton Wall container"""
 
     _walls: MutableMapping[str, Wall] = {}
     _instance = None
 
     def __new__(cls) -> "WallStore":
         if cls._instance is None:
             cls._instance = super(WallStore, cls).__new__(cls)
         return cls._instance
 
     def get(self, name: str) -> Wall:
         """Returns a Wall element identified by its @name. Creates it if it doesn't exist yet."""
-        return self._walls.setdefault(name, Wall(name))
+        if name not in self._walls:
+            self._walls[name] = Wall(name)
+        return self._walls[name]
+
+    def loaded(self, name: str) -> bool:
+        """Returns True if a wall is already loaded to memory and thus might have to be reloaded"""
+        return name in self._walls
 
 
 def wall_from_name(name: str) -> Wall:
     """Convenience function to avoid manual access to the WallStore singleton"""
     return WallStore().get(name)
 
 
@@ -267,79 +303,93 @@
 
         # file_object = io.BytesIO()
         # img.resize((basewidth, hsize), Image.ANTIALIAS).save(file_object, 'JPEG')
         # file_object.seek(0)
     return None
 
 
-app = Flask(
+@watchdog
+async def watch_fs_changes() -> None:
+    """Observe changes to filesystem and mark walls dirty"""
+    wall_dir = app.config["UPLOAD_FOLDER"]
+    async for changed_path in fs_changes(wall_dir, timeout=1, postpone=True):
+        log().info("file %s changed", changed_path)
+        if not changed_path.is_relative_to(wall_dir):
+            continue
+        if len(changed_path.parts) <= len(wall_dir.parts):
+            continue
+        if not WallStore().loaded(wall_name := changed_path.parts[len(wall_dir.parts)]):
+            continue
+        WallStore().get(wall_name).dirty()
+
+
+app = Quart(
     __name__,
     # static_url_path="/"
 )
 
 
 @app.route("/")
 def root() -> Response:
     """Landing page, creates a dummy site 'first'"""
     # here we might copy some default wall and give it a random name
     return cast(Response, redirect("first"))
 
 
 @app.route("/<wall_name>/")
-def index(wall_name: str) -> str:  # pylint: disable=unused-argument
+async def index(wall_name: str) -> str:  # pylint: disable=unused-argument
     """Returns the (static) magicwalll HTML site"""
     # TODO: use Blueprints:
     # https://stackoverflow.com/questions/15231359/split-python-flask-app-into-multiple-files
     # return open(app.config["BASE_FOLDER"] / "magicwall.html").read()
-    return render_template("magicwall.html")
+    return await render_template("magicwall.html")
 
 
 @app.route("/<wall_name>/model", methods=["GET"])
 def model(wall_name: str) -> str:
     """Retrieves the whole model of a wall"""
-    res = json.dumps(wall_from_name(wall_name).model(), default=lambda __o: __o.__dict__)
-    return res
+    model_ = wall_from_name(wall_name).model()
+    return json.dumps(model_, default=lambda __o: to_external(__o.__dict__))
 
 
 @app.route("/<wall_name>/file/<name>", methods=["GET"])
-def get_file(wall_name: str, name: str) -> Response:
+async def get_file(wall_name: str, name: str) -> Response:
     """Retrieves a file specified by @name"""
-    return send_file(app.config["UPLOAD_FOLDER"] / wall_name / name)
+    return await send_file(app.config["UPLOAD_FOLDER"] / wall_name / name)
 
 
 @app.route("/<wall_name>/preview/<name>", methods=["GET"])
-def get_file_preview(wall_name: str, name: str) -> Response:
+async def get_file_preview(wall_name: str, name: str) -> Response:
     """GETs a thumbnail for file indicated by @name"""
     if Path(name).suffix.lower() in {".gif"}:
         preview_filename = app.config["UPLOAD_FOLDER"] / wall_name / name
     elif Path(name).suffix.lower() in {".jpeg", ".jpg", ".png"}:
         preview_filename = app.config["UPLOAD_FOLDER"] / wall_name / f"{name}.preview.jpeg"
         if not preview_filename.exists():
             create_preview(
                 app.config["UPLOAD_FOLDER"] / wall_name / name,
                 preview_filename,
             )
     else:
-        return send_file("static/unknown.png")
-    return send_file(preview_filename)
+        return await send_file("static/unknown.png")
+    return await send_file(preview_filename)
 
 
 @app.route("/<wall_name>/add_elements", methods=["POST"])
-def add_elements(wall_name: str) -> str:
+async def add_elements(wall_name: str) -> str:
     """This function takes quite informal input from raw drop/paste data and
     turns it into something structured.
     """
     request_data: MutableGenMap = {
-        name: parse_json_value(name, itemobj) for name, itemobj in request.form.items()
+        name: parse_json_value(name, itemobj) for name, itemobj in (await request.form).items()
     }
     request_data["files"] = [
-        json.dumps(
-            File.from_file_storage(wall_name, name, fileob)
-            for name, fileob in request.files.items()
-        )
+        # this is formally incorrect but works for now
+        cast(GenMap, File.from_file_storage(wall_name, name, fileob))
+        for name, fileob in (await request.files).items()
     ]
     if "text/plain" in request_data:
         request_data["text/html"] = markdown.markdown(
             str(request_data["text/plain"]),
             extensions=[
                 "extra",
                 "codehilite",
@@ -349,62 +399,79 @@
 
     print(f"add on {wall_name}: {request_data}")
 
     return wall_from_name(wall_name).add_item(Item.from_tree(request_data))
 
 
 @app.route("/<wall_name>/update_position", methods=["POST"])
-def update_position(wall_name: str) -> str:
+async def update_position(wall_name: str) -> Literal["OK", "NOK"]:
     """Moves item indicated by `id` to another position"""
-    item_id = request.form["id"]
-    new_pos = json.loads(request.form["pos"])
+    form = await request.form
+    item_id = form["id"]
+    new_pos = json.loads(form["pos"])
     wall = wall_from_name(wall_name)
     print(item_id, new_pos)
     for item in wall.model().items:
         if item.id == item_id:
             item.pos = new_pos
             wall.save()
             return "OK"
     return "NOK"
 
 
 @app.route("/<wall_name>/remove_item", methods=["POST"])
-def remove_item(wall_name: str) -> str:
+async def remove_item(wall_name: str) -> Literal["OK", "NOK"]:
     """Removes item indicated by `id`"""
-    item_id = request.form["id"]
+    form = await request.form
+    item_id = form["id"]
     wall = wall_from_name(wall_name)
 
     for item in (items := wall.model().items):
         if item.id == item_id:
             items.remove(item)
             wall.save()
             return "OK"
     return "NOK"
 
 
 @app.route("/<wall_name>/download", methods=["GET"])
-def download_archive(wall_name: str) -> Response:
+async def download_archive(wall_name: str) -> Response:
     """Creates a tar archive from wall indicated by @wall_name"""
     tar_file_name = app.config["UPLOAD_FOLDER"] / f"{wall_name}.tar.gz"
     with tarfile.open(tar_file_name, "w:gz") as tar:
         tar.add(app.config["UPLOAD_FOLDER"] / wall_name, arcname=wall_name)
 
-    return send_file(tar_file_name)
+    return await send_file(tar_file_name)
+
+
+@app.before_serving
+async def start_tasks() -> None:
+    """Starts asynchronous background tasks after webserver has been started"""
+    asyncio.ensure_future(watch_fs_changes())
 
 
 def main() -> int:
     """Run Flask"""
+    setup_logging(level="DEBUG")
+
     args = parse_args(sys.argv[1:])
 
     yaml.add_representer(File, mw_representer)
     yaml.add_representer(Item, mw_representer)
     yaml.add_representer(Model, mw_representer)
 
     app.config["BASE_FOLDER"] = Path(__file__).parent
     app.config["UPLOAD_FOLDER"] = Path(".").absolute() / "walls"
+    app.config["TEMPLATES_AUTO_RELOAD"] = True
 
-    app.run(host="0.0.0.0", port=args.port, debug=args.debug)
+    app.run(
+        host="0.0.0.0",
+        port=args.port,
+        debug=args.debug,
+        use_reloader=False,
+        # loop=asyncio.get_event_loop(),
+    )
     return 0
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `magicwall-0.0.2/magicwall/static/DragDropTouch.js` & `magicwall-0.0.3/magicwall/static/DragDropTouch.js`

 * *Files identical despite different names*

### Comparing `magicwall-0.0.2/magicwall/static/hilite-solarized-light.css` & `magicwall-0.0.3/magicwall/static/hilite-solarized-light.css`

 * *Files identical despite different names*

### Comparing `magicwall-0.0.2/magicwall/static/magicwall.css` & `magicwall-0.0.3/magicwall/static/magicwall.css`

 * *Files identical despite different names*

### Comparing `magicwall-0.0.2/magicwall/static/magicwall.js` & `magicwall-0.0.3/magicwall/static/magicwall.js`

 * *Files identical despite different names*

### Comparing `magicwall-0.0.2/magicwall/static/unknown.png` & `magicwall-0.0.3/magicwall/static/unknown.png`

 * *Files identical despite different names*

### Comparing `magicwall-0.0.2/magicwall/templates/magicwall.html` & `magicwall-0.0.3/magicwall/templates/magicwall.html`

 * *Files identical despite different names*

### Comparing `magicwall-0.0.2/pyproject.toml` & `magicwall-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magicwall"
-version = "0.0.2"
+version = "0.0.3"
 description = "This is the magic wall (magicwall.io)"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/magicwall.io"
 readme = "Readme.md"
 packages = [
   {include = "magicwall"}
 ]
@@ -15,17 +15,17 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 asyncinotify = "^4.0.1"
 exifread = "^3.0.0"
 markdown = "^3.4.3"
 pyyaml = "^6.0"
-flask = "^2.3.2"
 pillow = "^9.5.0"
-checkmk-dev-tools = "^0.1.12"
+markdown-checklist = "^0.4.4"
+quart = "^0.18.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
```

### Comparing `magicwall-0.0.2/PKG-INFO` & `magicwall-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: magicwall
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is the magic wall (magicwall.io)
 Home-page: https://projects.om-office.de/frans/magicwall.io
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncinotify (>=4.0.1,<5.0.0)
-Requires-Dist: checkmk-dev-tools (>=0.1.12,<0.2.0)
 Requires-Dist: exifread (>=3.0.0,<4.0.0)
-Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: markdown (>=3.4.3,<4.0.0)
+Requires-Dist: markdown-checklist (>=0.4.4,<0.5.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: quart (>=0.18.4,<0.19.0)
 Project-URL: Repository, https://projects.om-office.de/frans/magicwall.io
 Description-Content-Type: text/markdown
 
 # magicwall.io
 
 View, share, compose, edit visual, textual and acustical content and apply
 arbitraty effects on it.
@@ -85,14 +85,15 @@
 * [ ] Resize elments
 * [ ] Caching mechanism
 * [ ] Square-select multiple items
 
 
 ## Future
 
+* Notification on change
 * Fullscreen / slideshow mode
 * Undo-stack
 * Config-YAML
 * Filter-Hub
 * Search
 * Offline use
 * Git support
@@ -114,16 +115,18 @@
 * Algorithm demonstration / education (-> Jupyter)
 * File exchange
 * Note taking
 
 
 ## Magic ideas
 
+* Document optimizer
 * Simple auto optimize images (contrast, etc)
 * Simple BW images
+* Polaroid images
 * Configurable Image with roation, cropping, color improvement, vignetting
 * Files to animation
 * SVG background
 * Auto align by date
 * fetch URL -> return generated HTML
```

