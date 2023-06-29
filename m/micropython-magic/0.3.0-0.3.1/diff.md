# Comparing `tmp/micropython_magic-0.3.0.tar.gz` & `tmp/micropython_magic-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_magic-0.3.0.tar", max compression
+gzip compressed data, was "micropython_magic-0.3.1.tar", max compression
```

## Comparing `micropython_magic-0.3.0.tar` & `micropython_magic-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1090 2023-04-13 20:20:40.063549 micropython_magic-0.3.0/LICENSE
--rw-r--r--   0        0        0     1424 2023-06-29 18:43:16.469527 micropython_magic-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6364 2023-06-29 18:39:42.591892 micropython_magic-0.3.0/readme.md
--rw-r--r--   0        0        0      875 2023-06-29 18:39:42.635353 micropython_magic-0.3.0/src/micropython_magic/__init__.py
--rw-r--r--   0        0        0     3611 2023-06-29 18:39:42.637353 micropython_magic-0.3.0/src/micropython_magic/interactive.py
--rw-r--r--   0        0        0      773 2023-06-29 18:39:42.638770 micropython_magic-0.3.0/src/micropython_magic/magic_transformer.py
--rw-r--r--   0        0        0    26108 2023-06-29 18:39:42.639775 micropython_magic-0.3.0/src/micropython_magic/memoryinfo.py
--rw-r--r--   0        0        0     4816 2023-06-29 18:39:42.640926 micropython_magic-0.3.0/src/micropython_magic/mpr.py
--rw-r--r--   0        0        0    11949 2023-06-29 18:39:42.643280 micropython_magic-0.3.0/src/micropython_magic/octarine.py
--rw-r--r--   0        0        0      488 2023-06-07 09:44:35.636682 micropython_magic-0.3.0/src/micropython_magic/param_fixup.py
--rw-r--r--   0        0        0     2928 2023-06-29 18:39:42.645270 micropython_magic-0.3.0/src/micropython_magic/test_magics.py
--rw-r--r--   0        0        0     7111 1970-01-01 00:00:00.000000 micropython_magic-0.3.0/setup.py
--rw-r--r--   0        0        0     6890 1970-01-01 00:00:00.000000 micropython_magic-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-13 20:20:40.063549 micropython_magic-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1424 2023-06-29 18:52:04.239019 micropython_magic-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6364 2023-06-29 18:39:42.591892 micropython_magic-0.3.1/readme.md
+-rw-r--r--   0        0        0      875 2023-06-29 18:39:42.635353 micropython_magic-0.3.1/src/micropython_magic/__init__.py
+-rw-r--r--   0        0        0     3611 2023-06-29 18:39:42.637353 micropython_magic-0.3.1/src/micropython_magic/interactive.py
+-rw-r--r--   0        0        0      773 2023-06-29 18:39:42.638770 micropython_magic-0.3.1/src/micropython_magic/magic_transformer.py
+-rw-r--r--   0        0        0    26107 2023-06-29 18:51:41.327067 micropython_magic-0.3.1/src/micropython_magic/memoryinfo.py
+-rw-r--r--   0        0        0     4816 2023-06-29 18:39:42.640926 micropython_magic-0.3.1/src/micropython_magic/mpr.py
+-rw-r--r--   0        0        0    11949 2023-06-29 18:39:42.643280 micropython_magic-0.3.1/src/micropython_magic/octarine.py
+-rw-r--r--   0        0        0      488 2023-06-07 09:44:35.636682 micropython_magic-0.3.1/src/micropython_magic/param_fixup.py
+-rw-r--r--   0        0        0     2928 2023-06-29 18:39:42.645270 micropython_magic-0.3.1/src/micropython_magic/test_magics.py
+-rw-r--r--   0        0        0     7111 1970-01-01 00:00:00.000000 micropython_magic-0.3.1/setup.py
+-rw-r--r--   0        0        0     6890 1970-01-01 00:00:00.000000 micropython_magic-0.3.1/PKG-INFO
```

### Comparing `micropython_magic-0.3.0/LICENSE` & `micropython_magic-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.0/pyproject.toml` & `micropython_magic-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-magic"
-version = "0.3.0"
+version = "0.3.1"
 description = "MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs"
 keywords = [
     "MicroPython",
     "stubs",
     "Jupyter",
     "notebooks",
     "Jupyter Labs",
```

### Comparing `micropython_magic-0.3.0/readme.md` & `micropython_magic-0.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.0/src/micropython_magic/__init__.py` & `micropython_magic-0.3.1/src/micropython_magic/__init__.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.0/src/micropython_magic/interactive.py` & `micropython_magic-0.3.1/src/micropython_magic/interactive.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.0/src/micropython_magic/magic_transformer.py` & `micropython_magic-0.3.1/src/micropython_magic/magic_transformer.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.0/src/micropython_magic/memoryinfo.py` & `micropython_magic-0.3.1/src/micropython_magic/memoryinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,15 +600,15 @@
         ax2.minorticks_on()
         ##################################################################################
         # adjust display of the x-axis labels
         for label in ax1.get_xticklabels():
             label.set_horizontalalignment("left")
             label.set_rotation(-10)
             label.set_fontsize("x-small")
-            label.set_fontweight("ligsht")
+            label.set_fontweight("light")
             label.set_y(label.get_position()[1] + 0.01)
         # make more room for the labels below  the figure
         fig.subplots_adjust(bottom=0.1)
 
         ##################################################################################
         # Add stackplot of free, used and stack memory if requested
         labels = ["heap used"]
```

### Comparing `micropython_magic-0.3.0/src/micropython_magic/mpr.py` & `micropython_magic-0.3.1/src/micropython_magic/mpr.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.0/src/micropython_magic/octarine.py` & `micropython_magic-0.3.1/src/micropython_magic/octarine.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.0/src/micropython_magic/test_magics.py` & `micropython_magic-0.3.1/src/micropython_magic/test_magics.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.0/setup.py` & `micropython_magic-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['mpremote==1.20.0']
 
 setup_kwargs = {
     'name': 'micropython-magic',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs',
     'long_description': '# micropython-magic\n\nThese magic methods allow MicroPython to be used from within any Jupyter Notebook or JupyterLab (formerly IPython Notebook)\nThe magics make use of the [mpremote tool](https://github.com/micropython/micropython/blob/master/tools/mpremote/README.md) to enable communication with the MCUs \n\n\nIt allows \n * Mixing of Host and MCU Code ( and languages if you wish)\n * Creating graphs of the data captured by MCU sensors \n * create re-uasable sequences ( download/compile firmware - flash firmware - uploade code - run expiriment - same outcome) \n * create and execute tests that require orchestration across multiple MCUs and hosts \n * Rapid Prototyping \n * Capturing the results and outputs in a consistent way\n * Mixing documentation with code  \n\n\n## Samples \n\n<table>\n\n<tr>\n<td>\nPlot cpu temperature  \n\n<img src="docs/cpu_plot.gif" width="300" />\n</td>\n<td>\nVisualize the memory map of the MCU\n\n<img src="docs/memory_map.gif" width="300" />\n</td>\n</tr>\n\n<tr>\n<td>\n</td>\n<td>\nMemory allocation of the MCU over time\n\n<img src="docs/memory_map_sequence.gif" width="300" />\n</td>\n</tr>\n</table>\n\nFor the source please refer to the samples folder\n## Installation\n- create and activate a venv `python3 -m venv .venv`\n - [ ] `pip install -U "micropython-magic"`\n\n- or install directly into your notbook environment/kernel using the \'%pip\' magic by running\n  - [ ] `%pip install -U "micropython-magic"`\n\nRecommended : install stubs for your MCU of choice\n- [ ] Install stubs for MicroPython syntax checking `pip install micropython-rp2-stubs` (or your port of choise)\n\n## Usage\n\n**1) Create a notebook**\n- install your desired notebook environment:\n  - [VScode and the **Juypyter extension**](https://code.visualstudio.com/docs/languages/python#_jupyter-notebooks) ,\n  - [Jupyter Notebook](https://jupyter.org/install#jupyter-notebook) \n  - [JupyterLab ](https://jupyter.org/install)\n\n- create a new notebook \n\n**2) Load the magic**\n```python\n%load_ext micropython_magic\n```\nThis can also be configured once to always load automatically ( see below)\n\n\n**3) add a cell with some code to run on the MCU**\n```python\n# %%micropython  \nfrom machine import Pin\nled = Pin(25, Pin.OUT)\nled.value(1)\n```\nThe `%%micropython` cell magic will instruct Jupyter to run the code on the connected MCU\n\n**4) enable code highlighting for MicroPython**\n```python\n%pip install micropython-esp32-stubs==1.20.0.*\n# installs the stubs for MicroPython syntax checking (one time install per environment) \n```\n\n```python\n# %%micropython  \nfrom machine import Pin\nled = Pin(25, Pin.OUT)\nled.value(1)\n```\nThis allows for syntax highlighting and code completion of MicroPython code.\nTested in VSCode with\n- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) extension\n- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension\n\n\n## Advanced \nList the connected devices \n```python\n%mpy --list\n```\n\n## Automatically load the magic on startup\n\nIn order to automatically load the magic on startup, you can add the following to your `ipython_config.py` file:\n\n- create a ipython profile \n  - `ipython profile create`\n  - add the following to the configuration file (`.../.ipython/profile_default/ipython_config.py`)\n\n    ```python\n    c = get_config()  #noqa\n\n    c.InteractiveShellApp.extensions = [\n        \'micropython_magic\'\n    ]\n    ```\n\n# initial \n\n - [x] run a code cell on a MCU \n - [ ] mpremote primitives\n   - [x] list connected boards and loop through them \n   - [x] switch the active MCU\n   - [x] avoid resetting MCU between cells ( use `resume`)\n   - [x] soft-reset a MCU\n   - [/] hard-reset a MCU\n       - only works on non-rp2040 devices \n       - report / fix hardware reset  issue on rp2040 `machine.reset()` ?\n   - all mpremote commands are possible using `!mpremote`\n   - [ ] mip install \n   - [ ] direct - copy file / files to / from \n   - [ ] mount folder \n   - [ ] ls and other file operations \n   - [ ] recursive delete wipe files from MCU - as a built-in magic ? / wait for / create PR for mpremote update ?\n   - [ ] cellmagic to copy cell content to specific files on the MCS \n       - [ ] %%micropython --writefile main.py\n       - [ ] %%micropython --readfile boot.py\n- [ ] Notebook essentials\n   - [x] load magics from `%pip install micropython-magic`\n   - [x] get the output from the MCU into a python variable `local = %eval remote`\n         - eval is not quite the same as mpremote\n         - retain type through json ?\n         - [?] can this be done with repr(insted) of json ?\n   - [x] plot data from a MCU\n            - [x] using bqplot ( > pyplot > vscode-Jupyter) \n            - [/] add documentation / sample\n-   \n   - [ ] copy/echo MCU global vars to local vars ( sync_from / sync_to)?\n   - [ ] get a data series onto the notebook and plot the outcome \n       - [x] loop one by one and update plot\n       - [ ] get larger series \n   - [ ] loop and update plot \n         https://ipywidgets.readthedocs.io/en/7.x/examples/Widget%20Asynchronous.html#Updating-a-widget-in-the-background\n   - [ ] long running via mqtt / async / folder mount ?\n - [ ] is there a way to avoid needing to set %%micropython on all cells ?\n       this could be done via an input_transformer - but keeping the state between cells may be quuite hard / confusing\n - [ ] %timeit / %%timeit for micropython code to avoid measuring the mpremote startup overhead \n\nSamples\n   - [x] Install\n   - [x] basic board control\n   - [x] blink\n   - [x] list connected boards and loop through them \n   - [~] read sensor and build series ( file / list / plot)\n   - [ ] flash a mcu with new firmware ( sample per port )\n   - [ ] mip install \n   - [ ] upload a repo / folder to a MCU\n\n## development\n## Testing \n\n- using Pytest\n- using testbook for testing notebooks\n  - located in the `./tests/` folder\n  - tests are paired with notebooks that contain the cells and magic commands to be tested\n  - tests have not been mocked - and therefore require a connected MCU to run ( rp2040 )\n\n- TODO: add tests for (remote) kernels \n  - [x] Local (on windows)\n  - [ ] on windows \n  - [ ] on linux\n  - [ ] jupyter notebook\n  - [ ] jupyter labs \n\n',
     'author': 'Jos Verlinde',
     'author_email': 'jos_verlinde@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `micropython_magic-0.3.0/PKG-INFO` & `micropython_magic-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-magic
-Version: 0.3.0
+Version: 0.3.1
 Summary: MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs
 License: MIT
 Keywords: MicroPython,stubs,Jupyter,notebooks,Jupyter Labs,vscode
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

