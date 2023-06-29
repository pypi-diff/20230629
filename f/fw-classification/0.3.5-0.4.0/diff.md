# Comparing `tmp/fw_classification-0.3.5-py3-none-any.whl.zip` & `tmp/fw_classification-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 29982 bytes, number of entries: 24
+Zip file size: 30156 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      220 b- defN 80-Jan-01 00:00 fw_classification/__init__.py
 -rw-r--r--  2.0 unx      622 b- defN 80-Jan-01 00:00 fw_classification/adapters/__init__.py
 -rw-r--r--  2.0 unx     1329 b- defN 80-Jan-01 00:00 fw_classification/adapters/base.py
 -rw-r--r--  2.0 unx      981 b- defN 80-Jan-01 00:00 fw_classification/adapters/deps.py
 -rw-r--r--  2.0 unx     1498 b- defN 80-Jan-01 00:00 fw_classification/adapters/dicom.py
 -rw-r--r--  2.0 unx     4485 b- defN 80-Jan-01 00:00 fw_classification/adapters/fw.py
 -rw-r--r--  2.0 unx     5504 b- defN 80-Jan-01 00:00 fw_classification/adapters/nifti.py
 -rw-r--r--  2.0 unx      995 b- defN 80-Jan-01 00:00 fw_classification/adapters/utils.py
 -rw-r--r--  2.0 unx     1027 b- defN 80-Jan-01 00:00 fw_classification/classify/__init__.py
 -rw-r--r--  2.0 unx     8416 b- defN 80-Jan-01 00:00 fw_classification/classify/block.py
 -rw-r--r--  2.0 unx     1125 b- defN 80-Jan-01 00:00 fw_classification/classify/expressions/__init__.py
 -rw-r--r--  2.0 unx    12154 b- defN 80-Jan-01 00:00 fw_classification/classify/expressions/base.py
 -rw-r--r--  2.0 unx    13179 b- defN 80-Jan-01 00:00 fw_classification/classify/expressions/expression.py
 -rw-r--r--  2.0 unx     2919 b- defN 80-Jan-01 00:00 fw_classification/classify/includes.py
--rw-r--r--  2.0 unx     7762 b- defN 80-Jan-01 00:00 fw_classification/classify/profile.py
+-rw-r--r--  2.0 unx     8462 b- defN 80-Jan-01 00:00 fw_classification/classify/profile.py
 -rw-r--r--  2.0 unx    10859 b- defN 80-Jan-01 00:00 fw_classification/classify/rule.py
 -rw-r--r--  2.0 unx     2555 b- defN 80-Jan-01 00:00 fw_classification/classify/utils.py
 -rw-r--r--  2.0 unx     2945 b- defN 80-Jan-01 00:00 fw_classification/cli.py
 -rw-r--r--  2.0 unx      605 b- defN 80-Jan-01 00:00 fw_classification/utils.py
-?rw-r--r--  2.0 unx      108 b- defN 16-Jan-01 00:00 fw_classification-0.3.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     1077 b- defN 80-Jan-01 00:00 fw_classification-0.3.5.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 fw_classification-0.3.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx     3953 b- defN 16-Jan-01 00:00 fw_classification-0.3.5.dist-info/METADATA
-?rw-r--r--  2.0 unx     2208 b- defN 16-Jan-01 00:00 fw_classification-0.3.5.dist-info/RECORD
-24 files, 86609 bytes uncompressed, 26338 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx     1077 b- defN 80-Jan-01 00:00 fw_classification-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3907 b- defN 80-Jan-01 00:00 fw_classification-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_classification-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      108 b- defN 80-Jan-01 00:00 fw_classification-0.4.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2208 b- defN 16-Jan-01 00:00 fw_classification-0.4.0.dist-info/RECORD
+24 files, 87268 bytes uncompressed, 26512 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -51,23 +51,23 @@
 
 Filename: fw_classification/cli.py
 Comment: 
 
 Filename: fw_classification/utils.py
 Comment: 
 
-Filename: fw_classification-0.3.5.dist-info/entry_points.txt
+Filename: fw_classification-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: fw_classification-0.3.5.dist-info/LICENSE
+Filename: fw_classification-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: fw_classification-0.3.5.dist-info/WHEEL
+Filename: fw_classification-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: fw_classification-0.3.5.dist-info/METADATA
+Filename: fw_classification-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fw_classification-0.3.5.dist-info/RECORD
+Filename: fw_classification-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_classification/classify/profile.py

```diff
@@ -41,17 +41,17 @@
         self.errors: t.List[ProfileError] = []
         self.path = Path(path).resolve()
         # Local yaml loader/dumper
         self.yaml = YAML(typ="safe")
         # Raw profile as dict
         self.profile_raw: t.Dict[str, t.Any] = {}
         # Dictionary of <block_name> and their execution results
-        self.block_results: t.Dict[str, bool] = {}
+        self.block_results: t.Dict[t.Union[str, Path], bool] = {}
         # Dictionary of blocks and which profile they came from
-        self.block_map: t.Dict[str, str] = {}
+        self.block_map: t.Dict[t.Union[str, Path], str] = {}
         # Deque of block objects
         self.blocks: OrderedDict = OrderedDict()
         # Map of include path to Profile object
         self.include_map: t.Dict[str, "Profile"] = {}
         try:
             with open(self.path, "r", encoding="utf-8") as fp:
                 self.profile_raw = self.yaml.load(fp)
@@ -77,15 +77,15 @@
             block, errs = Block.from_dict(block_raw)
             # `block` will be None, skip it.
             if errs:
                 self.errors.extend(
                     [e.add_component(f"profile ({self.name})") for e in errs]
                 )
                 continue
-            self.handle_block(block, "local")  # type: ignore
+            self.handle_block(block, "local", self.path)  # type: ignore
         if exit_on_error:
             self.report_errs_and_exit()
 
     def report_errs_and_exit(self) -> None:
         """Print errors and exit."""
         if self.errors:
             msg = (
@@ -93,38 +93,41 @@
                 f"{self.path}:\n"
             )
             for err in self.errors:
                 msg += textwrap.indent(f"- {err}\n\n", "  ")
             log.error(msg)
             sys.exit(1)
 
-    def handle_block(self, block: Block, prof_name: str) -> None:
+    def handle_block(self, block: Block, prof_name: str, prof_path: Path) -> None:
         """Handle a given block.
 
         * Add block to self.blocks, overriding the same name with newer (local)
             block
         * Add block to self.block_map with given profile name.
         * Add block to self.block_results with default result of False.
 
         Args:
             block (Block): block to handle.
             prof_name (str): Name of profile block came from.
+            prof_path (Path): Path of profile block came from.
         """
-        if block.name in self.block_map:
-            defined_profile = self.block_map[block.name]
+        # Dynamically add prof_path to block.name and depends
+        block_name = prof_path.with_suffix("") / block.name
+        if block_name in self.block_map:
+            defined_profile = self.block_map[block_name]
             log.info(
-                f"Found duplicate block {block.name} defined in  {prof_name} "
+                f"Found duplicate block {block_name} defined in  {prof_name} "
                 f"replacing existing block defined in {defined_profile}"
             )
 
-        self.block_map[block.name] = prof_name
+        self.block_map[block_name] = prof_name
         # Set all initial result to false
-        self.block_results[block.name] = False
+        self.block_results[block_name] = False
         # Populate block
-        self.blocks[block.name] = block
+        self.blocks[block_name] = block
 
     def resolve_include(
         self, search_dirs: t.List[Path], include: str
     ) -> t.List[ProfileError]:
         """Add included rules.
 
         Args:
@@ -135,25 +138,26 @@
         profile_path = includes.get_profile(search_dirs, include)
         profile = self.__class__(profile_path, exit_on_error=False)
         if profile.errors:
             errors.extend(
                 [e.add_component(f"profile ({self.name}") for e in profile.errors]
             )
         prof_name = profile.name
+        prof_path = profile.path
         if prof_name in self.include_map:
             errors.append(
                 ProfileError(
                     prof_name,
                     "Profile is already included.  Profile names must be unique.",
                 )
             )
             return errors
         self.include_map[prof_name] = profile
         for _, block in profile.blocks.items():
-            self.handle_block(block, prof_name)
+            self.handle_block(block, prof_name, prof_path)
         return errors
 
     def evaluate(self, i_dict: t.Dict) -> t.Tuple[bool, Dotty]:
         """Evaluate the profile.
 
         Args:
             i_dict (t.Dict): Input dictionary
@@ -168,14 +172,23 @@
         """
         dotty_mods: Dotty = dotty(i_dict)
 
         for name, block in self.blocks.items():
             # Decide whether or not block should execute
             should_execute = True
             for depends in block.depends_on:
+                # depends_on should be in the format of profle_name/block or just block.
+                try:
+                    depends_profile = self.include_map[depends.split("/")[0]]
+                    depends = (
+                        depends_profile.path.with_suffix("") / depends.split("/")[1]
+                    )
+                except KeyError:
+                    depends = name.parent / depends
+
                 try:
                     if not self.block_results[depends]:
                         should_execute = False
                         break
                 except KeyError as e:
                     raise ValueError(
                         f"Block {name} depends on an unknown block {depends}"
```

## Comparing `fw_classification-0.3.5.dist-info/LICENSE` & `fw_classification-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_classification-0.3.5.dist-info/METADATA` & `fw_classification-0.4.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: fw-classification
-Version: 0.3.5
+Version: 0.4.0
 Summary: Flywheel classification toolkit.
 Home-page: https://gitlab.com/flywheel-io/public/classification-toolkit
 License: MIT
 Author: Flywheel
 Author-email: support@flywheel.io
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: fw
 Provides-Extra: geartk
 Requires-Dist: backoff (>=1.11.1,<2.0.0)
 Requires-Dist: dotty-dict (>=1.3.0,<2.0.0)
-Requires-Dist: flywheel-gear-toolkit (>=0.6.4,<0.7.0); extra == "all" or extra == "geartk"
-Requires-Dist: fw-core-client (>=1.0.0,<2.0.0); extra == "all" or extra == "fw"
+Requires-Dist: flywheel-gear-toolkit (>=0.6.4,<0.7.0) ; extra == "all" or extra == "geartk"
+Requires-Dist: fw-core-client (>=1.0.0,<2.0.0) ; extra == "all" or extra == "fw"
 Requires-Dist: fw-file (>=1.1.0,<2.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.4,<0.18.0)
 Requires-Dist: typer (>=0.4.1,<0.5.0)
 Project-URL: Repository, https://gitlab.com/flywheel-io/public/classification-toolkit
 Description-Content-Type: text/markdown
 
 # Classification Toolkit
```

## Comparing `fw_classification-0.3.5.dist-info/RECORD` & `fw_classification-0.4.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 fw_classification/adapters/utils.py,sha256=0mWQJbcRPjGV_jAoB69ysJhECo1sAl3oWojQmaHbMwY,995
 fw_classification/classify/__init__.py,sha256=3rxsLgmwxl4m_pMBHZwEwBmioMEI7By8C2LPRr7TWZs,1027
 fw_classification/classify/block.py,sha256=mYZXAwqtUsjAOpH3EBdBPOjTtwyBxLGrQVMH4qziyEM,8416
 fw_classification/classify/expressions/__init__.py,sha256=eyOhQSKwd1IhmY3aP-CFiGrdihgQc-6chhOj5EtwBEA,1125
 fw_classification/classify/expressions/base.py,sha256=Mu-H-bS9kHYJMtrKbA6hrrQzVq3OOcibF0OcbcmIgbQ,12154
 fw_classification/classify/expressions/expression.py,sha256=xDxLlenh5WVAukzYRUnPbY46UawwhhSVZx4Exg83PF4,13179
 fw_classification/classify/includes.py,sha256=6RKiFpl0Mr0hvTXgNfQWXSp_-SobxQDZ2zVP62KtqLk,2919
-fw_classification/classify/profile.py,sha256=UvPaPpfr9zE_XwLNhVFTPy6dJnt5S0wQyKIcUEd10nE,7762
+fw_classification/classify/profile.py,sha256=C9wvEQVRyKlXay7o37bcGYvHcTN0I89NFSQrZEwdOdU,8462
 fw_classification/classify/rule.py,sha256=Ly6NVQk-4OnWvIOgl2hKMYJqFyf5U4__pM5Z0Dfbdm8,10859
 fw_classification/classify/utils.py,sha256=WE2EUM4aHJts7xuDT_-6Gd1XDYhN_XFxnNsx7XMoZZc,2555
 fw_classification/cli.py,sha256=0ImcEIb3vBnMIiUUYkFlba3ECP2C0z3oJ793-4EhgCk,2945
 fw_classification/utils.py,sha256=CCu7yx7i1WA6EfCswQB886tiCbMdc5zF7LJJFbpDGRE,605
-fw_classification-0.3.5.dist-info/entry_points.txt,sha256=RyLEV0GDVT8CzEXFkhUktLw24ywdokP6zjVuDUxYTOI,108
-fw_classification-0.3.5.dist-info/LICENSE,sha256=EmDQE8zHgRCuAaYxpDVanIo1Nmn7VUdxGHD17LXcjYY,1077
-fw_classification-0.3.5.dist-info/WHEEL,sha256=y3eDiaFVSNTPbgzfNn0nYn5tEn1cX6WrdetDlQM4xWw,83
-fw_classification-0.3.5.dist-info/METADATA,sha256=NwcKCgf2R_NsGxAnCBj4fWv4BFGZJ7U-d3cwdYqG34s,3953
-fw_classification-0.3.5.dist-info/RECORD,,
+fw_classification-0.4.0.dist-info/LICENSE,sha256=EmDQE8zHgRCuAaYxpDVanIo1Nmn7VUdxGHD17LXcjYY,1077
+fw_classification-0.4.0.dist-info/METADATA,sha256=azZFFc8rQB0qhM9JWqc_uR95uTnZG1Qq-xo-Bb4km-w,3907
+fw_classification-0.4.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fw_classification-0.4.0.dist-info/entry_points.txt,sha256=RyLEV0GDVT8CzEXFkhUktLw24ywdokP6zjVuDUxYTOI,108
+fw_classification-0.4.0.dist-info/RECORD,,
```

