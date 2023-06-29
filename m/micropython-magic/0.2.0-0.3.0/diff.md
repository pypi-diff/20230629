# Comparing `tmp/micropython_magic-0.2.0.tar.gz` & `tmp/micropython_magic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_magic-0.2.0.tar", max compression
+gzip compressed data, was "micropython_magic-0.3.0.tar", max compression
```

## Comparing `micropython_magic-0.2.0.tar` & `micropython_magic-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1090 2023-04-13 20:20:40.063549 micropython_magic-0.2.0/LICENSE
--rw-r--r--   0        0        0     1424 2023-06-07 13:42:12.573794 micropython_magic-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6195 2023-06-07 13:04:28.271109 micropython_magic-0.2.0/readme.md
--rw-r--r--   0        0        0      871 2023-06-07 09:44:57.685197 micropython_magic-0.2.0/src/micropython_magic/__init__.py
--rw-r--r--   0        0        0      742 2023-06-07 09:44:35.633369 micropython_magic-0.2.0/src/micropython_magic/magic_transformer.py
--rw-r--r--   0        0        0     4358 2023-06-07 09:44:35.635378 micropython_magic-0.2.0/src/micropython_magic/mpr.py
--rw-r--r--   0        0        0    12010 2023-06-07 13:46:25.009898 micropython_magic-0.2.0/src/micropython_magic/octarine.py
--rw-r--r--   0        0        0      488 2023-06-07 09:44:35.636682 micropython_magic-0.2.0/src/micropython_magic/param_fixup.py
--rw-r--r--   0        0        0     2514 2023-06-07 09:44:57.688172 micropython_magic-0.2.0/src/micropython_magic/test_magics.py
--rw-r--r--   0        0        0     6942 1970-01-01 00:00:00.000000 micropython_magic-0.2.0/setup.py
--rw-r--r--   0        0        0     6736 1970-01-01 00:00:00.000000 micropython_magic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-13 20:20:40.063549 micropython_magic-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1424 2023-06-29 18:43:16.469527 micropython_magic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6364 2023-06-29 18:39:42.591892 micropython_magic-0.3.0/readme.md
+-rw-r--r--   0        0        0      875 2023-06-29 18:39:42.635353 micropython_magic-0.3.0/src/micropython_magic/__init__.py
+-rw-r--r--   0        0        0     3611 2023-06-29 18:39:42.637353 micropython_magic-0.3.0/src/micropython_magic/interactive.py
+-rw-r--r--   0        0        0      773 2023-06-29 18:39:42.638770 micropython_magic-0.3.0/src/micropython_magic/magic_transformer.py
+-rw-r--r--   0        0        0    26108 2023-06-29 18:39:42.639775 micropython_magic-0.3.0/src/micropython_magic/memoryinfo.py
+-rw-r--r--   0        0        0     4816 2023-06-29 18:39:42.640926 micropython_magic-0.3.0/src/micropython_magic/mpr.py
+-rw-r--r--   0        0        0    11949 2023-06-29 18:39:42.643280 micropython_magic-0.3.0/src/micropython_magic/octarine.py
+-rw-r--r--   0        0        0      488 2023-06-07 09:44:35.636682 micropython_magic-0.3.0/src/micropython_magic/param_fixup.py
+-rw-r--r--   0        0        0     2928 2023-06-29 18:39:42.645270 micropython_magic-0.3.0/src/micropython_magic/test_magics.py
+-rw-r--r--   0        0        0     7111 1970-01-01 00:00:00.000000 micropython_magic-0.3.0/setup.py
+-rw-r--r--   0        0        0     6890 1970-01-01 00:00:00.000000 micropython_magic-0.3.0/PKG-INFO
```

### Comparing `micropython_magic-0.2.0/LICENSE` & `micropython_magic-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.2.0/pyproject.toml` & `micropython_magic-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-magic"
-version = "0.2.0"
+version = "0.3.0"
 description = "MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs"
 keywords = [
     "MicroPython",
     "stubs",
     "Jupyter",
     "notebooks",
     "Jupyter Labs",
```

### Comparing `micropython_magic-0.2.0/readme.md` & `micropython_magic-0.3.0/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,34 +13,49 @@
  * Capturing the results and outputs in a consistent way
  * Mixing documentation with code  
 
 
 ## Samples 
 
 <table>
+
 <tr>
 <td>
-<img src="docs/cpu_plot.gif" width="400" />
+Plot cpu temperature  
+
+<img src="docs/cpu_plot.gif" width="300" />
 </td>
 <td>
-<img src="docs/memory_map.gif" width="400" />
+Visualize the memory map of the MCU
+
+<img src="docs/memory_map.gif" width="300" />
+</td>
+</tr>
+
+<tr>
+<td>
+</td>
+<td>
+Memory allocation of the MCU over time
+
+<img src="docs/memory_map_sequence.gif" width="300" />
 </td>
 </tr>
 </table>
 
 For the source please refer to the samples folder
 ## Installation
 - create and activate a venv `python3 -m venv .venv`
- - [ ] `pip install -U "git+https://github.com/josverl/micropython-magic"`
+ - [ ] `pip install -U "micropython-magic"`
 
 - or install directly into your notbook environment/kernel using the '%pip' magic by running
-  - [ ] `%pip install -U "git+https://github.com/josverl/micropython-magic"`
+  - [ ] `%pip install -U "micropython-magic"`
 
 Recommended : install stubs for your MCU of choice
-- [ ] Install stubs for MicroPython syntax checking `pip install micropython-rp2-stubs`
+- [ ] Install stubs for MicroPython syntax checking `pip install micropython-rp2-stubs` (or your port of choise)
 
 ## Usage
 
 **1) Create a notebook**
 - install your desired notebook environment:
   - [VScode and the **Juypyter extension**](https://code.visualstudio.com/docs/languages/python#_jupyter-notebooks) ,
   - [Jupyter Notebook](https://jupyter.org/install#jupyter-notebook)
```

### Comparing `micropython_magic-0.2.0/src/micropython_magic/__init__.py` & `micropython_magic-0.3.0/src/micropython_magic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 
 from .magic_transformer import comment_magic_transformer
 from .octarine import MpyMagics
 from .test_magics import TestMagics
 
 
 def load_ipython_extension(ipython: InteractiveShell):
-    # register the input transformer to allow magis in comments
+    # register the input transformer to allow %%cell_magics in comments
     ipython.input_transformers_cleanup.append(comment_magic_transformer)
     # register the magics
-
     ipython.register_magics(MpyMagics)
-    # ipython.register_magics(TestMagics)
+    ipython.register_magics(TestMagics)
 
 
 def unload_ipython_extension(ipython: InteractiveShell):
     # unregister the magics, allows to unload / reload the extension
     # ipython.magics_manager.magics["cell"].pop("mpy", None)
     # TODO
     pass
```

### Comparing `micropython_magic-0.2.0/src/micropython_magic/magic_transformer.py` & `micropython_magic-0.3.0/src/micropython_magic/magic_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
 Transforms a cell with a commented cell magic into a cell without the comment, but with the %%celmagic.
 
 `# %%micropython --> %%micropython`
 This allows Pylance to only see python code and not the magic, 
-which would otherwise confuse it, and cause it to be disabled.
+which would otherwise confuse it, and cause it to be     disabled.
 """
 import re
 
-re_comment_magic = r"#\s(%%(micropython|python|mypy|script))"
-"""Regex to match a comment magic, e.g. `# %%micropython`"""
-subst = "\\g<1>"
+re_comment_magic = r"#[ |\t|!]*%%((micropython|python|mypy|script))"  # matches `# %%micropython` or `#!%%micropython` with optional spaces in between
+subst = r"%%\g<1>"
 
 
 def comment_magic_transformer(lines: list[str]):
     """
     Transforms a cell with a commented cell magic into a cell without the comment, but with the %%celmagic.
     """
     if "%%" not in lines[0]:
         return lines
-
     return [re.sub(re_comment_magic, subst, lines[0])] + lines[1:]
```

### Comparing `micropython_magic-0.2.0/src/micropython_magic/mpr.py` & `micropython_magic-0.3.0/src/micropython_magic/mpr.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,45 +9,52 @@
 
 import IPython
 from colorama import Style
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.utils.text import LSString, SList
 from loguru import logger as log
 
+from .interactive import ipython_run
 
 JSON_START = "<json~"
 JSON_END = "~json>"
 DONT_KNOW = "<~?~>"
 
+from .interactive import TIMEOUT
+
+
 class MPRemote2:
     def __init__(self, shell: InteractiveShell, port: str = "auto", resume: bool = True):
         self.shell: InteractiveShell = shell
         self.port: str = "auto"  # by default connect to the first device
-        self.resume = True  # by default resume the device to maintain state
+        self.resume = resume  # by default resume the device to maintain state
+        self.timeout = TIMEOUT
 
     @property
     def cmd_prefix(self):
         """mpremote command prefix including port and resume according to options"""
         return f"mpremote {self.connect_to}{'resume' if self.resume else ''} "
 
     @property
     def connect_to(self):
         "Creates mpremote 'connect to string' if port is specified."
         return f"connect {self.port} " if self.port else ""
 
-    def run_cmd(self, cmd: str, auto_connect: bool = True):
+    def run_cmd(self, cmd: str, *, auto_connect: bool = True, stream_out: bool = True, shell=True, timeout=0):
         """run a command on the device and return the output"""
         if auto_connect:
             cmd = f"""{self.cmd_prefix} {cmd}"""
         log.debug(cmd)
-        output = self.shell.getoutput(cmd, split=True)
-        assert isinstance(output, SList)
-        if len(output) > 0 and output[0].strip() == "no device found":
-            raise ConnectionError("no device found")
-        return output
+        return ipython_run(cmd, stream_out=stream_out, shell=shell, timeout=timeout or self.timeout)
+
+        # output = self.shell.getoutput(cmd, split=True)
+        # assert isinstance(output, SList)
+        # if len(output) > 0 and output[0].strip() == "no device found":
+        #     raise ConnectionError("no device found")
+        # return output
 
     def select_device(self, line: Optional[str]):
         """try to select the device to connect to by specifying the serial port name."""
         _port = line.strip() if line else "auto"
         cmd = f"""eval \"'Checking connection to MCU on port {_port}.'\""""
         try:
             output = self.run_cmd(cmd)
@@ -59,39 +66,40 @@
     def run_cell(self, cell: str):
         """run a codeblock on the device and return the output"""
         #     # TODO: if the cell is small enough, concat the cell with \n an use exec instead of copy
         #     # - may need escaping quotes and newlines
         # copy the cell to a file on the device
         self.cell_to_mcu_file(cell, "__magic.py")
         # run the transferred cell/file
-        return self.run_mcu_file("__magic.py")
+        result = self.run_mcu_file("__magic.py", stream_out=True)
+        return
 
-    def run_mcu_file(self, filename):
+    def run_mcu_file(self, filename: str, stream_out: bool = True, timeout: int = 0):
         exec_cmd = f"exec \"exec( open('{filename}').read() , globals() )\""
-        return self.run_cmd(exec_cmd)
+        return self.run_cmd(exec_cmd, stream_out=stream_out, timeout=timeout)
 
     def cell_to_mcu_file(self, cell, filename):
         with tempfile.NamedTemporaryFile(mode="w", suffix=".py", delete=False) as f:
             f.write("# Jupyter cell\n")  # add a line to replace the cell magic to keep the line numbers aligned
             f.write(cell)
             f.close()
             # copy the file to the device
             copy_cmd = f"cp {f.name} :{filename}"
             # TODO: detect / retry / report errors copying the file
-            _ = self.run_cmd(copy_cmd)
+            _ = self.run_cmd(copy_cmd, stream_out=False, timeout=60)
             # log.info(_)
             # log.info(f.name, "copied to device")
             Path(f.name).unlink()
 
     def cell_from_mcu_file(self, filename):
         """read a file from the device and return the contents"""
         with tempfile.NamedTemporaryFile(mode="w", suffix=".py", delete=False) as f:
             copy_cmd = f"cp :{filename} {f.name}"
             # TODO: detect / retry / report errors copying the file
-            _ = self.run_cmd(copy_cmd)
+            _ = self.run_cmd(copy_cmd, stream_out=False, timeout=60)
 
             return Path(f.name).read_text()
 
     @staticmethod
     def load_json_from_MCU(line: str):
         """try to load the output from the MCU transferred as json"""
         result = DONT_KNOW
```

### Comparing `micropython_magic-0.2.0/src/micropython_magic/octarine.py` & `micropython_magic-0.3.0/src/micropython_magic/octarine.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 from .mpr import DONT_KNOW, JSON_END, JSON_START, MPRemote2
 
 # https://ipython.readthedocs.io/en/stable/config/custommagics.html
 # https://ipython.readthedocs.io/en/stable/api/generated/IPython.core.magic.html#IPython.core.magic.Magics
 # https://nbviewer.org/github/rossant/ipython-minibook/blob/master/chapter6/602-cpp.ipynb
 
 
+class MCUException(Exception):
+    """Exception raised for errors on the MCU."""
+
+    pass
+
+
 def set_log_level(llevel: str):
     # format_str = "<level>{level: <8}</level> | <cyan>{module: <18}</cyan> - <level>{message}</level>"
     # format_str = "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <8}</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>"
     format_str = "<level>{level: <8}</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>"
     log.remove(0)
     log.add(sys.stdout, format=format_str, level=llevel, colorize=True)
 
@@ -158,15 +164,15 @@
             else:
                 self.shell.set_next_input(code, replace=True)
             return
 
         if not cell:
             raise UsageError("Please specify some MicroPython code to execute")
         output = self.MCU.run_cell(cell)
-        return PrettyOutput(output)
+        # return PrettyOutput(output)
 
     # -------------------------------------------------------------------------
     # line magics
     # -------------------------------------------------------------------------
 
     @line_magic("micropython")
     @line_magic("mpy")
@@ -222,35 +228,30 @@
             return self.eval(args.eval)
 
         elif args.statement:
             # Assemble the command to run
             statement = "\n".join(args.statement)
             cmd = f'exec "{statement}"'
             log.debug(f"{cmd=}")
-            output = self.MCU.run_cmd(cmd)
-            return PrettyOutput(output)
+
+            output = self.MCU.run_cmd(cmd, stream_out=False)
+            return output
 
     # -------------------------------------------------------------------------
     # worker mothods - these are called by the magics
     # -------------------------------------------------------------------------
 
     def list_devices(self) -> list:
         """
         Return a SList or list of the Micropython devices connected to the computer through serial ports or USB.
         """
         cmd = "mpremote connect list"
         # output = self.shell.getoutput(cmd)
-        output = self.MCU.run_cmd(cmd, auto_connect=False)
-        if isinstance(output, SList):
-            return output.list
-        elif isinstance(output, list):
-            return output
-        else:
-            return [output]
-        # TODO: handle other output types #
+        output = self.MCU.run_cmd(cmd, auto_connect=False, stream_out=False)
+        return output
 
     def select(self, line: Optional[str]):
         """
         Select the device to connect to by specifying the serial port name.
         """
         device = line.strip() if line else "auto"
         output = self.MCU.select_device(device)
@@ -266,21 +267,21 @@
         Runs the statement on the MCU and tries to convert the output to a python object.
         If that fails it returns the raw output as a string.
         """
         # Assemble the command to run
         statement = line.strip()
         cmd = f'''exec "import json; print('{JSON_START}',json.dumps({statement}),'{JSON_END}')"'''
         # print(cmd)
-        output = self.MCU.run_cmd(cmd)
+        output = self.MCU.run_cmd(cmd, stream_out=False)
         matchers = [r"^.*Error:", r"^.*Exception:"]
 
         for ln in output.l:
             # check for errors and raise them
             if any(re.match(m, ln) for m in matchers):
-                raise RuntimeError(ln) from eval(ln.split(":")[0])
+                raise MCUException(ln) from eval(ln.split(":")[0])
             # check for json output and try to convert it
             if ln.startswith(JSON_START) and ln.endswith(JSON_END):
                 result = self.MCU.load_json_from_MCU(ln)
                 if result != DONT_KNOW:
                     return result
         return output
```

### Comparing `micropython_magic-0.2.0/setup.py` & `micropython_magic-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['mpremote==1.20.0']
 
 setup_kwargs = {
     'name': 'micropython-magic',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs',
-    'long_description': '# micropython-magic\n\nThese magic methods allow MicroPython to be used from within any Jupyter Notebook or JupyterLab (formerly IPython Notebook)\nThe magics make use of the [mpremote tool](https://github.com/micropython/micropython/blob/master/tools/mpremote/README.md) to enable communication with the MCUs \n\n\nIt allows \n * Mixing of Host and MCU Code ( and languages if you wish)\n * Creating graphs of the data captured by MCU sensors \n * create re-uasable sequences ( download/compile firmware - flash firmware - uploade code - run expiriment - same outcome) \n * create and execute tests that require orchestration across multiple MCUs and hosts \n * Rapid Prototyping \n * Capturing the results and outputs in a consistent way\n * Mixing documentation with code  \n\n\n## Samples \n\n<table>\n<tr>\n<td>\n<img src="docs/cpu_plot.gif" width="400" />\n</td>\n<td>\n<img src="docs/memory_map.gif" width="400" />\n</td>\n</tr>\n</table>\n\nFor the source please refer to the samples folder\n## Installation\n- create and activate a venv `python3 -m venv .venv`\n - [ ] `pip install -U "git+https://github.com/josverl/micropython-magic"`\n\n- or install directly into your notbook environment/kernel using the \'%pip\' magic by running\n  - [ ] `%pip install -U "git+https://github.com/josverl/micropython-magic"`\n\nRecommended : install stubs for your MCU of choice\n- [ ] Install stubs for MicroPython syntax checking `pip install micropython-rp2-stubs`\n\n## Usage\n\n**1) Create a notebook**\n- install your desired notebook environment:\n  - [VScode and the **Juypyter extension**](https://code.visualstudio.com/docs/languages/python#_jupyter-notebooks) ,\n  - [Jupyter Notebook](https://jupyter.org/install#jupyter-notebook) \n  - [JupyterLab ](https://jupyter.org/install)\n\n- create a new notebook \n\n**2) Load the magic**\n```python\n%load_ext micropython_magic\n```\nThis can also be configured once to always load automatically ( see below)\n\n\n**3) add a cell with some code to run on the MCU**\n```python\n# %%micropython  \nfrom machine import Pin\nled = Pin(25, Pin.OUT)\nled.value(1)\n```\nThe `%%micropython` cell magic will instruct Jupyter to run the code on the connected MCU\n\n**4) enable code highlighting for MicroPython**\n```python\n%pip install micropython-esp32-stubs==1.20.0.*\n# installs the stubs for MicroPython syntax checking (one time install per environment) \n```\n\n```python\n# %%micropython  \nfrom machine import Pin\nled = Pin(25, Pin.OUT)\nled.value(1)\n```\nThis allows for syntax highlighting and code completion of MicroPython code.\nTested in VSCode with\n- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) extension\n- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension\n\n\n## Advanced \nList the connected devices \n```python\n%mpy --list\n```\n\n## Automatically load the magic on startup\n\nIn order to automatically load the magic on startup, you can add the following to your `ipython_config.py` file:\n\n- create a ipython profile \n  - `ipython profile create`\n  - add the following to the configuration file (`.../.ipython/profile_default/ipython_config.py`)\n\n    ```python\n    c = get_config()  #noqa\n\n    c.InteractiveShellApp.extensions = [\n        \'micropython_magic\'\n    ]\n    ```\n\n# initial \n\n - [x] run a code cell on a MCU \n - [ ] mpremote primitives\n   - [x] list connected boards and loop through them \n   - [x] switch the active MCU\n   - [x] avoid resetting MCU between cells ( use `resume`)\n   - [x] soft-reset a MCU\n   - [/] hard-reset a MCU\n       - only works on non-rp2040 devices \n       - report / fix hardware reset  issue on rp2040 `machine.reset()` ?\n   - all mpremote commands are possible using `!mpremote`\n   - [ ] mip install \n   - [ ] direct - copy file / files to / from \n   - [ ] mount folder \n   - [ ] ls and other file operations \n   - [ ] recursive delete wipe files from MCU - as a built-in magic ? / wait for / create PR for mpremote update ?\n   - [ ] cellmagic to copy cell content to specific files on the MCS \n       - [ ] %%micropython --writefile main.py\n       - [ ] %%micropython --readfile boot.py\n- [ ] Notebook essentials\n   - [x] load magics from `%pip install micropython-magic`\n   - [x] get the output from the MCU into a python variable `local = %eval remote`\n         - eval is not quite the same as mpremote\n         - retain type through json ?\n         - [?] can this be done with repr(insted) of json ?\n   - [x] plot data from a MCU\n            - [x] using bqplot ( > pyplot > vscode-Jupyter) \n            - [/] add documentation / sample\n-   \n   - [ ] copy/echo MCU global vars to local vars ( sync_from / sync_to)?\n   - [ ] get a data series onto the notebook and plot the outcome \n       - [x] loop one by one and update plot\n       - [ ] get larger series \n   - [ ] loop and update plot \n         https://ipywidgets.readthedocs.io/en/7.x/examples/Widget%20Asynchronous.html#Updating-a-widget-in-the-background\n   - [ ] long running via mqtt / async / folder mount ?\n - [ ] is there a way to avoid needing to set %%micropython on all cells ?\n       this could be done via an input_transformer - but keeping the state between cells may be quuite hard / confusing\n - [ ] %timeit / %%timeit for micropython code to avoid measuring the mpremote startup overhead \n\nSamples\n   - [x] Install\n   - [x] basic board control\n   - [x] blink\n   - [x] list connected boards and loop through them \n   - [~] read sensor and build series ( file / list / plot)\n   - [ ] flash a mcu with new firmware ( sample per port )\n   - [ ] mip install \n   - [ ] upload a repo / folder to a MCU\n\n## development\n## Testing \n\n- using Pytest\n- using testbook for testing notebooks\n  - located in the `./tests/` folder\n  - tests are paired with notebooks that contain the cells and magic commands to be tested\n  - tests have not been mocked - and therefore require a connected MCU to run ( rp2040 )\n\n- TODO: add tests for (remote) kernels \n  - [x] Local (on windows)\n  - [ ] on windows \n  - [ ] on linux\n  - [ ] jupyter notebook\n  - [ ] jupyter labs \n\n',
+    'long_description': '# micropython-magic\n\nThese magic methods allow MicroPython to be used from within any Jupyter Notebook or JupyterLab (formerly IPython Notebook)\nThe magics make use of the [mpremote tool](https://github.com/micropython/micropython/blob/master/tools/mpremote/README.md) to enable communication with the MCUs \n\n\nIt allows \n * Mixing of Host and MCU Code ( and languages if you wish)\n * Creating graphs of the data captured by MCU sensors \n * create re-uasable sequences ( download/compile firmware - flash firmware - uploade code - run expiriment - same outcome) \n * create and execute tests that require orchestration across multiple MCUs and hosts \n * Rapid Prototyping \n * Capturing the results and outputs in a consistent way\n * Mixing documentation with code  \n\n\n## Samples \n\n<table>\n\n<tr>\n<td>\nPlot cpu temperature  \n\n<img src="docs/cpu_plot.gif" width="300" />\n</td>\n<td>\nVisualize the memory map of the MCU\n\n<img src="docs/memory_map.gif" width="300" />\n</td>\n</tr>\n\n<tr>\n<td>\n</td>\n<td>\nMemory allocation of the MCU over time\n\n<img src="docs/memory_map_sequence.gif" width="300" />\n</td>\n</tr>\n</table>\n\nFor the source please refer to the samples folder\n## Installation\n- create and activate a venv `python3 -m venv .venv`\n - [ ] `pip install -U "micropython-magic"`\n\n- or install directly into your notbook environment/kernel using the \'%pip\' magic by running\n  - [ ] `%pip install -U "micropython-magic"`\n\nRecommended : install stubs for your MCU of choice\n- [ ] Install stubs for MicroPython syntax checking `pip install micropython-rp2-stubs` (or your port of choise)\n\n## Usage\n\n**1) Create a notebook**\n- install your desired notebook environment:\n  - [VScode and the **Juypyter extension**](https://code.visualstudio.com/docs/languages/python#_jupyter-notebooks) ,\n  - [Jupyter Notebook](https://jupyter.org/install#jupyter-notebook) \n  - [JupyterLab ](https://jupyter.org/install)\n\n- create a new notebook \n\n**2) Load the magic**\n```python\n%load_ext micropython_magic\n```\nThis can also be configured once to always load automatically ( see below)\n\n\n**3) add a cell with some code to run on the MCU**\n```python\n# %%micropython  \nfrom machine import Pin\nled = Pin(25, Pin.OUT)\nled.value(1)\n```\nThe `%%micropython` cell magic will instruct Jupyter to run the code on the connected MCU\n\n**4) enable code highlighting for MicroPython**\n```python\n%pip install micropython-esp32-stubs==1.20.0.*\n# installs the stubs for MicroPython syntax checking (one time install per environment) \n```\n\n```python\n# %%micropython  \nfrom machine import Pin\nled = Pin(25, Pin.OUT)\nled.value(1)\n```\nThis allows for syntax highlighting and code completion of MicroPython code.\nTested in VSCode with\n- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) extension\n- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension\n\n\n## Advanced \nList the connected devices \n```python\n%mpy --list\n```\n\n## Automatically load the magic on startup\n\nIn order to automatically load the magic on startup, you can add the following to your `ipython_config.py` file:\n\n- create a ipython profile \n  - `ipython profile create`\n  - add the following to the configuration file (`.../.ipython/profile_default/ipython_config.py`)\n\n    ```python\n    c = get_config()  #noqa\n\n    c.InteractiveShellApp.extensions = [\n        \'micropython_magic\'\n    ]\n    ```\n\n# initial \n\n - [x] run a code cell on a MCU \n - [ ] mpremote primitives\n   - [x] list connected boards and loop through them \n   - [x] switch the active MCU\n   - [x] avoid resetting MCU between cells ( use `resume`)\n   - [x] soft-reset a MCU\n   - [/] hard-reset a MCU\n       - only works on non-rp2040 devices \n       - report / fix hardware reset  issue on rp2040 `machine.reset()` ?\n   - all mpremote commands are possible using `!mpremote`\n   - [ ] mip install \n   - [ ] direct - copy file / files to / from \n   - [ ] mount folder \n   - [ ] ls and other file operations \n   - [ ] recursive delete wipe files from MCU - as a built-in magic ? / wait for / create PR for mpremote update ?\n   - [ ] cellmagic to copy cell content to specific files on the MCS \n       - [ ] %%micropython --writefile main.py\n       - [ ] %%micropython --readfile boot.py\n- [ ] Notebook essentials\n   - [x] load magics from `%pip install micropython-magic`\n   - [x] get the output from the MCU into a python variable `local = %eval remote`\n         - eval is not quite the same as mpremote\n         - retain type through json ?\n         - [?] can this be done with repr(insted) of json ?\n   - [x] plot data from a MCU\n            - [x] using bqplot ( > pyplot > vscode-Jupyter) \n            - [/] add documentation / sample\n-   \n   - [ ] copy/echo MCU global vars to local vars ( sync_from / sync_to)?\n   - [ ] get a data series onto the notebook and plot the outcome \n       - [x] loop one by one and update plot\n       - [ ] get larger series \n   - [ ] loop and update plot \n         https://ipywidgets.readthedocs.io/en/7.x/examples/Widget%20Asynchronous.html#Updating-a-widget-in-the-background\n   - [ ] long running via mqtt / async / folder mount ?\n - [ ] is there a way to avoid needing to set %%micropython on all cells ?\n       this could be done via an input_transformer - but keeping the state between cells may be quuite hard / confusing\n - [ ] %timeit / %%timeit for micropython code to avoid measuring the mpremote startup overhead \n\nSamples\n   - [x] Install\n   - [x] basic board control\n   - [x] blink\n   - [x] list connected boards and loop through them \n   - [~] read sensor and build series ( file / list / plot)\n   - [ ] flash a mcu with new firmware ( sample per port )\n   - [ ] mip install \n   - [ ] upload a repo / folder to a MCU\n\n## development\n## Testing \n\n- using Pytest\n- using testbook for testing notebooks\n  - located in the `./tests/` folder\n  - tests are paired with notebooks that contain the cells and magic commands to be tested\n  - tests have not been mocked - and therefore require a connected MCU to run ( rp2040 )\n\n- TODO: add tests for (remote) kernels \n  - [x] Local (on windows)\n  - [ ] on windows \n  - [ ] on linux\n  - [ ] jupyter notebook\n  - [ ] jupyter labs \n\n',
     'author': 'Jos Verlinde',
     'author_email': 'jos_verlinde@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `micropython_magic-0.2.0/PKG-INFO` & `micropython_magic-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-magic
-Version: 0.2.0
+Version: 0.3.0
 Summary: MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs
 License: MIT
 Keywords: MicroPython,stubs,Jupyter,notebooks,Jupyter Labs,vscode
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -32,34 +32,49 @@
  * Capturing the results and outputs in a consistent way
  * Mixing documentation with code  
 
 
 ## Samples 
 
 <table>
+
 <tr>
 <td>
-<img src="docs/cpu_plot.gif" width="400" />
+Plot cpu temperature  
+
+<img src="docs/cpu_plot.gif" width="300" />
 </td>
 <td>
-<img src="docs/memory_map.gif" width="400" />
+Visualize the memory map of the MCU
+
+<img src="docs/memory_map.gif" width="300" />
+</td>
+</tr>
+
+<tr>
+<td>
+</td>
+<td>
+Memory allocation of the MCU over time
+
+<img src="docs/memory_map_sequence.gif" width="300" />
 </td>
 </tr>
 </table>
 
 For the source please refer to the samples folder
 ## Installation
 - create and activate a venv `python3 -m venv .venv`
- - [ ] `pip install -U "git+https://github.com/josverl/micropython-magic"`
+ - [ ] `pip install -U "micropython-magic"`
 
 - or install directly into your notbook environment/kernel using the '%pip' magic by running
-  - [ ] `%pip install -U "git+https://github.com/josverl/micropython-magic"`
+  - [ ] `%pip install -U "micropython-magic"`
 
 Recommended : install stubs for your MCU of choice
-- [ ] Install stubs for MicroPython syntax checking `pip install micropython-rp2-stubs`
+- [ ] Install stubs for MicroPython syntax checking `pip install micropython-rp2-stubs` (or your port of choise)
 
 ## Usage
 
 **1) Create a notebook**
 - install your desired notebook environment:
   - [VScode and the **Juypyter extension**](https://code.visualstudio.com/docs/languages/python#_jupyter-notebooks) ,
   - [Jupyter Notebook](https://jupyter.org/install#jupyter-notebook)
```

