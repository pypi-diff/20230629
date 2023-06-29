# Comparing `tmp/tomato-engine-1.8.5.tar.gz` & `tmp/tomato-engine-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomato-engine-1.8.5.tar", last modified: Fri Jun  2 03:34:01 2023, max compression
+gzip compressed data, was "tomato-engine-2.0.0.tar", last modified: Thu Jun 29 18:09:03 2023, max compression
```

## Comparing `tomato-engine-1.8.5.tar` & `tomato-engine-2.0.0.tar`

### file list

```diff
@@ -1,37 +1,45 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    35149 2022-05-23 23:00:31.000000 tomato-engine-1.8.5/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2417 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/README.md
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       61 2022-05-23 23:00:31.000000 tomato-engine-1.8.5/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      836 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/setup.cfg
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1009 2023-06-02 03:29:46.000000 tomato-engine-1.8.5/setup.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:00.999160 tomato-engine-1.8.5/src/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:00.999160 tomato-engine-1.8.5/src/tomato/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      116 2023-05-08 19:51:10.000000 tomato-engine-1.8.5/src/tomato/__init__.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/src/tomato/classes/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       93 2023-05-08 19:52:06.000000 tomato-engine-1.8.5/src/tomato/classes/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    10952 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/classes/board.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    13921 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/classes/cell.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5109 2023-06-02 03:25:30.000000 tomato-engine-1.8.5/src/tomato/classes/cellmatrix.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3621 2023-05-08 19:51:41.000000 tomato-engine-1.8.5/src/tomato/classes/window.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/src/tomato/functions/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.5/src/tomato/functions/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      842 2022-06-20 19:13:20.000000 tomato-engine-1.8.5/src/tomato/functions/display.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4192 2022-07-06 18:41:02.000000 tomato-engine-1.8.5/src/tomato/functions/file_io.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4163 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/functions/utils.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/src/tomato/rules/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.5/src/tomato/rules/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      660 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/rules/colorful.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      273 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/rules/colorful_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      912 2023-05-13 01:05:56.000000 tomato-engine-1.8.5/src/tomato/rules/cyclic.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      316 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/rules/cyclic_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      872 2023-05-04 22:48:21.000000 tomato-engine-1.8.5/src/tomato/rules/game_of_life.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      274 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/rules/game_of_life_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      759 2023-05-13 01:06:01.000000 tomato-engine-1.8.5/src/tomato/rules/toothpick_fractal.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      297 2023-04-27 23:43:06.000000 tomato-engine-1.8.5/src/tomato/rules/toothpick_fractal_demo.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/src/tomato_engine.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-06-02 03:34:00.000000 tomato-engine-1.8.5/src/tomato_engine.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      856 2023-06-02 03:34:00.000000 tomato-engine-1.8.5/src/tomato_engine.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-06-02 03:34:00.000000 tomato-engine-1.8.5/src/tomato_engine.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       53 2023-06-02 03:34:00.000000 tomato-engine-1.8.5/src/tomato_engine.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        7 2023-06-02 03:34:00.000000 tomato-engine-1.8.5/src/tomato_engine.egg-info/top_level.txt
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-29 18:09:03.411544 tomato-engine-2.0.0/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    35149 2022-05-23 23:00:31.000000 tomato-engine-2.0.0/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-06-29 18:09:03.411544 tomato-engine-2.0.0/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2417 2022-10-20 06:23:30.000000 tomato-engine-2.0.0/README.md
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       61 2022-05-23 23:00:31.000000 tomato-engine-2.0.0/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      836 2023-06-29 18:09:03.411544 tomato-engine-2.0.0/setup.cfg
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1009 2023-06-29 18:08:14.000000 tomato-engine-2.0.0/setup.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-29 18:09:03.407544 tomato-engine-2.0.0/src/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-29 18:09:03.407544 tomato-engine-2.0.0/src/tomato/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      117 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/__init__.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-29 18:09:03.407544 tomato-engine-2.0.0/src/tomato/classes/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       94 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/classes/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4055 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/classes/agent.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    17429 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/classes/board.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4763 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/classes/cell.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    12272 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/classes/element.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3623 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/classes/window.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-29 18:09:03.407544 tomato-engine-2.0.0/src/tomato/functions/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-2.0.0/src/tomato/functions/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      856 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/functions/display.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4197 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/functions/file_io.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1511 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/functions/handling_rules.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4163 2022-10-20 06:23:30.000000 tomato-engine-2.0.0/src/tomato/functions/utils.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-29 18:09:03.411544 tomato-engine-2.0.0/src/tomato/rules/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-2.0.0/src/tomato/rules/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2194 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/automata1D.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      839 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/automata1D_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1338 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/cyclic.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      444 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/cyclic_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      872 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/game_of_life.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      274 2022-10-20 06:23:30.000000 tomato-engine-2.0.0/src/tomato/rules/game_of_life_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1068 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/langtons_ant.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      375 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/langtons_ant_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      971 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/random_walkers.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      447 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/random_walkers_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3275 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/tomato_life.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      314 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/tomato_life_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      780 2023-06-29 18:07:20.000000 tomato-engine-2.0.0/src/tomato/rules/toothpick_fractal.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      297 2023-06-29 15:43:01.000000 tomato-engine-2.0.0/src/tomato/rules/toothpick_fractal_demo.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-29 18:09:03.411544 tomato-engine-2.0.0/src/tomato_engine.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-06-29 18:09:03.000000 tomato-engine-2.0.0/src/tomato_engine.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1139 2023-06-29 18:09:03.000000 tomato-engine-2.0.0/src/tomato_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-06-29 18:09:03.000000 tomato-engine-2.0.0/src/tomato_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       53 2023-06-29 18:09:03.000000 tomato-engine-2.0.0/src/tomato_engine.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        7 2023-06-29 18:09:03.000000 tomato-engine-2.0.0/src/tomato_engine.egg-info/top_level.txt
```

### Comparing `tomato-engine-1.8.5/LICENSE` & `tomato-engine-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.5/PKG-INFO` & `tomato-engine-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-engine
-Version: 1.8.5
+Version: 2.0.0
 Summary: Engine for prototyping and playing with cellular automata
 Home-page: https://codeberg.org/eduardotogpi/tomato-engine
 Author: Eduardo Lopes Dias, Murilo Melhem
 Author-email: eduardosprp@usp.br
 Project-URL: Bug Tracker, https://codeberg.org/eduardotogpi/tomato-engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tomato-engine-1.8.5/README.md` & `tomato-engine-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.5/setup.cfg` & `tomato-engine-2.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tomato-engine
-version = 1.8.5
+version = 2.0.0
 author = Eduardo Lopes Dias, Murilo Melhem
 author_email = eduardotogpi@usp.br
 description = Engine for prototyping and playing with cellular automata.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://codeberg.org/eduardotogpi/tomato-engine
 project_urls =
```

### Comparing `tomato-engine-1.8.5/setup.py` & `tomato-engine-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tomato-engine",
-    version="1.8.5",
+    version="2.0.0",
     author="Eduardo Lopes Dias, Murilo Melhem",
     author_email="eduardosprp@usp.br",
     description="Engine for prototyping and playing with cellular automata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://codeberg.org/eduardotogpi/tomato-engine",
     project_urls={
```

### Comparing `tomato-engine-1.8.5/src/tomato/classes/board.py` & `tomato-engine-2.0.0/src/tomato/classes/board.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,201 +1,210 @@
 import os
 from time import time
+from types import ModuleType
 
 import numpy as np
 from IPython import display
 
 from ..functions import file_io
-from .cellmatrix import CellMatrixThreaded, CellMatrixUnthreaded
+from ..functions.handling_rules import agent_from_rule, cell_from_rule
+from .agent import AgentList
+from .cell import CellMatrix
 from .window import Window
 
 
 class Board:
-
+    # {{{
     """
-    O nome dessa classe é vago, mas ela é importante. Esta é a
-    interface do usuário, e também coordena a CellMatrix e a
-    Window.
+    O nome dessa classe é vago, mas ela é importante. Esta é a interface do
+    usuário, e também coordena a CellMatrix e a Window.
     """
 
-    def __init__(self, rule, **kwargs):
-        # {{{
-        """
-        Recebe a regra a ser adotada, assim como algumas
-        configurações. A simulação em si começa com a função
-        start.
+    # The default configs for Board
+    config_dict = {
+        "show_window": True,
+        "paused": False,
+        "generations": None,
+        "inline": False,
+        "generate_figures": False,
+        "generate_figures_dir": f"AutomataSimulation{os.path.sep}",
+        "generate_gif": False,
+        "step": None,
+        "debug": False,
+        "title": "Simulation",
+        "max_fps": 60,
+        "cell_size": 4,
+    }
+
+    def __init__(self, rule, rule_agents=None, **kwargs):
+        # {{{
+        """
+        Recebe a regra a ser adotada, assim como algumas configurações. A
+        simulação em si começa com a função start.
+
+        A rule é o módulo importado contendo a regra, no formato
+        especificado pelo exemplo game_of_life.py.
+
+        Se só o argumento `rule` for passado, entende-se que isso é ou um
+        módulo contendo a classe Cell e a Agent, ou é a própria classe
+        Cell, ou um módulo só com a Cell.
+        """
+
+        if isinstance(rule, ModuleType):
+            try:  # checks if Agents class is present
+                agent_class = agent_from_rule(rule)
+                cell_class = cell_from_rule(rule)
+                self.backend = BoardBackendAgents(
+                    cell_class, agent_class, **kwargs
+                )
+            except TypeError:  # then assumes the module contains only Cell
+                cell_class = cell_from_rule(rule)
+                self.backend = BoardBackendCells(cell_class, **kwargs)
+        else:  # then it must be a Cell class
+            cell_class = cell_from_rule(rule)
+            if rule_agents is not None:
+                agent_class = agent_from_rule(rule_agents)
+                self.backend = BoardBackendAgents(
+                    cell_class, agent_class, **kwargs
+                )
+            else:
+                self.backend = BoardBackendCells(cell_class, **kwargs)
 
-        A rule é o módulo importado contendo a regra, no
-        formato especificado pelo exemplo game_of_life.py.
-        """
+        # Then set all frontend methods to be the BoardBackend equivalents
+        self.load_state = self.backend.load_state
 
-        self.rule = rule
 
         # Configurações opcionais são passadas por kwargs.
-        self.debug = kwargs.get("debug", False)
-        self.title = kwargs.get("title", "Simulação")
-        self.max_fps = kwargs.get("max_fps", 60)
-        self.cell_size = kwargs.get("cell_size", 4)
-
-        self.generation = 0
+        self.config_dict = Board.config_dict.copy()
+        self.update_config(kwargs)
 
         if self.debug:
             # Lista com o tempo transcorrido para cada geração
             self.gen_time = []
 
     # }}}
 
-    def start(self, state_matrix, **kwargs):
+    def update(self):
+        # {{{
+        if self.generate_figures:
+            if self.step is None:
+                self.save_png()
+            else:
+                if self.backend.generation % self.step == 0:
+                    self.save_png()
+        if self.inline:
+            display.clear_output(wait=True)
+            display.display(file_io.img(self.display_matrix, self.cell_size))
+
+        if not self.debug:
+            self.backend.update()
+        else:
+            initial_time = time()
+            self.backend.update()
+            self.gen_time.append(1000.0 * (time() - initial_time))
+
+    # }}}
+
+    def start(self, *args, **kwargs):
         # {{{
         """
-        Inicia a simulação, o estado inicial sendo dado pela
-        state_matrix. state_matrix pode ser o caminho para uma
-        imagem ou uma matriz de numpy com os valores desejados.
+        Inicia a simulação, o estado inicial das células sendo dado pelo
+        primeiro argumento. state_matrix pode ser o caminho para uma imagem
+        ou uma matriz de numpy com os valores desejados.
         """
 
-        cell_args = kwargs.get("cell_args", None)
-        show_window = kwargs.get("show_window", True)
-        multithreaded = kwargs.get("multithreaded", False)
-        self.paused = kwargs.get("paused", False)
-        self.generations = kwargs.get("generations", None)
-        self.inline = kwargs.get("inline", False)
-        self.generate_figures = kwargs.get("generate_figures", False)
-        self.generate_figures_dir = kwargs.get(
-            "generate_figures_dir", f"{self.title}{os.path.sep}"
-        )
-        self.generate_gif = kwargs.get("generate_gif", False)
-        self.step = kwargs.get("step", None)
-
-        if self.inline:
-            show_window = False
+        self.update_config(kwargs)
 
         if self.generate_gif:
             self.generate_figures = True
             if self.generations is None:
                 raise TypeError(
-                    "You must specify the number of generations for the gif to "
-                    "be created."
+                    "You must specify the number of generations for "
+                    "the gif to be created."
                 )
 
         if self.generate_figures:
             self.check_dir(self.generate_figures_dir)
 
-        self.load_state(state_matrix, cell_args, multithreaded)
-        self.cellMatrix.simulation_start(state_matrix, cell_args)
+        # We expect state_matrix to be the first and only argument if the
+        # backend is BoardBackendCells
+        # And if it is BoardBackendAgents, state_matrix is the first argument
+        # and state_list to be the second
+        # cell_args is amongst the kwargs here
+        self.backend.start(*args, **kwargs)
 
-        if show_window:
-            self.show_window()
-        else:
+        if self.inline or not self.show_window:
             self.mainloop()
+        else:
+            self.start_window()
 
     # }}}
 
     def resume(self, **kwargs):
         # {{{
         """
         Continua a simulação de onde ela parou.
         """
 
-        show_window = kwargs.get("show_window", True)
-        self.paused = kwargs.get("paused", False)
-        self.generations = kwargs.get("generations", None)
-        self.inline = kwargs.get("inline", False)
-        self.generate_figures = kwargs.get("generate_figures", False)
-        self.generate_figures_dir = kwargs.get(
-            "generate_figures_dir", f"{self.title}{os.path.sep}"
-        )
-        self.generate_gif = kwargs.get("generate_gif", False)
-        self.step = kwargs.get("step", None)
-
-        if self.inline is True:
-            show_window = False
+        self.update_config(kwargs)
 
         if self.generate_gif:
             self.generate_figures = True
             if self.generations is None:
                 raise TypeError(
-                    "You must specify the number of generations for the gif to "
-                    "be created."
+                    "You must specify the number of generations for "
+                    "the gif to be created."
                 )
 
         if self.generate_figures:
             self.check_dir(self.generate_figures_dir)
 
-        if show_window:
-            self.show_window()
-        else:
+        if self.inline or not self.show_window:
             self.mainloop()
-
-    # }}}
-
-    def update(self, *args, **kwargs):
-        # {{{
-        """
-        Atualiza o estado da simulação, ou seja, realiza uma nova
-        iteração.
-        """
-        try:
-            if self.generate_figures:
-                if self.step is None:
-                    self.save_png()
-                else:
-                    if self.generation % self.step == 0:
-                        self.save_png()
-            if self.inline:
-                display.clear_output(wait=True)
-                display.display(file_io.img(self.display_matrix, self.cell_size))
-        except AttributeError:
-            pass
-        if not self.debug:
-            self.cellMatrix.update(*args, **kwargs)
         else:
-            initial_time = time()
-            self.cellMatrix.update()
-            self.gen_time.append(1000.0 * (time() - initial_time))
-
-        self.generation += 1
+            self.start_window()
 
     # }}}
 
-    def show_window(self, paused=None):
+    def start_window(self, paused=None):
         # {{{
         """
         Começa a simulação, mostrando a janelinha.
         """
 
         if paused is None:
             try:
                 paused = self.paused
             except AttributeError:
                 paused = False
 
         window = Window(
-            self.cellMatrix.display(),
+            self.display_matrix,
             debug=self.debug,
             title=self.title,
             paused=paused,
             max_fps=self.max_fps,
             cell_size=self.cell_size,
         )
 
         while window.running:
             window.query_inputs()
 
             if window.paused is False:
                 self.update()
-                window.update(self.cellMatrix.display())
+                window.update(self.display_matrix)
 
                 if self.debug:
                     self.print_debug()
 
                 try:
                     if self.generations is not None:
-                        if self.generation >= self.generations:
+                        if self.backend.generation >= self.generations:
                             window.running = False
-                        if self.generation == self.generations:
+                        if self.backend.generation == self.generations:
                             if self.generate_gif:
                                 self.save_gif()
                 except AttributeError:
                     pass
 
         if self.debug:
             self.print_avg_update_time()
@@ -207,68 +216,41 @@
         window.quit()
 
     # }}}
 
     def mainloop(self):
         # {{{
         """
-        Começa a simulação, sem mostrar a janelinha.
+        Começa a simulação, sem mostrar a janelinha. Note aqui que
+        self.backend.generations eh o numero de geracoes da simulacao e
+        self.generations eh o numero maximo de geracoes
         """
 
         running = True
         while running:
             try:
                 self.update()
             except KeyboardInterrupt:
                 break
 
             if self.debug:
                 self.print_debug()
 
             if self.generations is not None:
-                if self.generation >= self.generations:
+                if self.backend.generation >= self.generations:
                     running = False
-                if self.generation == self.generations:
+                if self.backend.generation == self.generations:
                     if self.generate_gif:
                         self.save_gif()
 
         if self.debug:
             self.print_avg_update_time()
 
     # }}}
 
-    def load_state(self, state_matrix, cell_args=None, multithreaded=False):
-        # {{{
-        """
-        Carrega uma matriz de estados a partir de uma imagem, uma
-        matriz numpy ou uma lista de listas.
-        """
-
-        if multithreaded:
-            CellMatrix = CellMatrixThreaded
-        else:
-            CellMatrix = CellMatrixUnthreaded
-
-        self.generation = 0
-
-        if isinstance(state_matrix, str):
-            png_matrix = file_io.load_png(state_matrix, size=self.cell_size)
-            self.cellMatrix = CellMatrix.from_display(png_matrix, self.rule, cell_args)
-        elif isinstance(state_matrix, np.ndarray):
-            self.cellMatrix = CellMatrix(state_matrix, self.rule, cell_args)
-        elif isinstance(state_matrix, list):
-            state_matrix = np.array(state_matrix)
-            self.cellMatrix = CellMatrix(state_matrix, self.rule, cell_args)
-        else:
-            raise TypeError(
-                f"{type(state_matrix)} is not a valid type for a state matrix."
-            )
-
-    # }}}
-
     def print_debug(self):
         # {{{
         """
         Auto-explicativo. Printa as informações de depuração.
         """
 
         print(
@@ -309,15 +291,17 @@
             path = f"{self.generate_figures_dir}{self.generation}.png"
         elif isinstance(path, str):
             if path.endswith(f"{os.path.sep}"):
                 path = f"{path}{self.generation}.png"
             elif not path.endswith(".png"):
                 path = f"{path}{os.path.sep}{self.generation}.png"
 
-        file_io.save_png(path, self.display_matrix, self.cell_size, print_output=False)
+        file_io.save_png(
+            path, self.display_matrix, self.cell_size, print_output=False
+        )
 
     # }}}
 
     def save_gif(self, path=None, max_fps=60):
         # {{{
         """
         Salva o estado da cellMatrix em uma png, para
@@ -340,15 +324,17 @@
         dir = self.generate_figures_dir
         if dir is None:
             dir = f"{self.title}{os.path.sep}"
         if not dir.endswith(f"{os.path.sep}"):
             dir = f"{dir}{os.path.sep}"
         while os.path.isdir(dir):
             num = "%03d" % i
-            dir = f"{dir.split(os.path.sep)[0].split('_')[0]}_{num}{os.path.sep}"
+            dir = (
+                f"{dir.split(os.path.sep)[0].split('_')[0]}_{num}{os.path.sep}"
+            )
             i += 1
         os.mkdir(dir)
         self.generate_figures_dir = dir
 
     # }}}
 
     def current_time_millis(self):
@@ -364,22 +350,270 @@
     @property
     def state_matrix(self):
         # {{{
         """
         Propriedade de conveniência para acessar a matriz de estados.
         """
 
+        return self.backend.state_matrix
+
+    # }}}
+
+    @property
+    def display_matrix(self):
+        # {{{
+        """
+        Propriedade de conveniência para acessar a matriz display.
+        """
+
+        return self.backend.display_matrix
+
+    # }}}
+
+    @property
+    def generation(self):
+        return self.backend.generation
+
+    def update_config(self, config_dict):
+        # {{{
+        """
+        Since I never seem to know whether to pass a kwarg on start or init,
+        why not make it so they can be passed on either?
+        """
+
+        self.config_dict.update(config_dict)
+
+        for key, val in self.config_dict.items():
+            setattr(self, key, val)
+
+
+# }}}
+
+
+# }}}
+
+
+class BoardBackendCells:
+    # {{{
+    def __init__(self, cell_class, **kwargs):
+        # {{{
+        # And the prize for the stupidest hack of the year goes to...
+        self.img_cell_size = kwargs.get(
+            "img_cell_size", kwargs.get("cell_size", 1)
+        )
+
+        self.cell_class = cell_class
+
+    # }}}
+
+    def start(self, state_matrix, **kwargs):
+        # {{{
+        """
+        Inicia a simulação, o estado inicial sendo dado pela
+        state_matrix. state_matrix pode ser o caminho para uma
+        imagem ou uma matriz de numpy com os valores desejados.
+
+        O abuso de *args e **kwargs aqui e insano
+        """
+
+        cell_args = kwargs.get("cell_args", None)
+        self.load_state(
+            state_matrix, cell_args=cell_args, img_cell_size=self.img_cell_size
+        )
+        self.cellMatrix.simulation_start(state_matrix)
+
+    # }}}
+
+    def update(self):
+        # {{{
+        """
+        Atualiza o estado da simulação, ou seja, realiza uma nova iteração.
+        """
+        self.cellMatrix.update()
+        self.generation += 1
+
+    # }}}
+
+    def load_state(self, state_matrix, cell_args=None, img_cell_size=1):
+        # {{{
+        """
+        Carrega uma matriz de estados a partir de uma imagem, uma
+        matriz numpy ou uma lista de listas.
+        """
+
+        self.generation = 0
+
+        if isinstance(state_matrix, str):
+            png_matrix = file_io.load_png(state_matrix, size=img_cell_size)
+            self.cellMatrix = CellMatrix.from_display(
+                png_matrix, self.cell_class, cell_args=cell_args
+            )
+        elif isinstance(state_matrix, np.ndarray):
+            self.cellMatrix = CellMatrix(
+                state_matrix, self.cell_class, cell_args=cell_args
+            )
+        elif isinstance(state_matrix, list):
+            state_matrix = np.array(state_matrix)
+            self.cellMatrix = CellMatrix(
+                state_matrix, self.cell_class, cell_args=cell_args
+            )
+        else:
+            raise TypeError(
+                f"{type(state_matrix)} is not a valid type for a state "
+                "matrix."
+            )
+
+    # }}}
+
+    @property
+    def state_matrix(self):
+        # {{{
+        """
+        Propriedade de conveniência para acessar a matriz de estados.
+        """
+
         return self.cellMatrix.state_matrix
 
     # }}}
 
     @property
     def display_matrix(self):
         # {{{
         """
         Propriedade de conveniência para acessar a matriz display.
         """
 
         return self.cellMatrix.display()
 
+    # }}}
+
+
+# }}}
+
+
+class BoardBackendAgents:
+    # {{{
+    def __init__(self, cell_class, agent_class, **kwargs):
+        # {{{
+        # And the prize for the stupidest hack of the year goes to...
+        self.img_cell_size = kwargs.get(
+            "img_cell_size", kwargs.get("cell_size", 1)
+        )
+
+        self.cell_class = cell_class
+        self.agent_class = agent_class
+
+    # }}}
+
+    def start(self, state_matrix, state_list, *args, **kwargs):
+        # {{{
+        """
+        Inicia a simulação, o estado inicial sendo dado pela
+        state_matrix. state_matrix pode ser o caminho para uma
+        imagem ou uma matriz de numpy com os valores desejados.
+
+        O abuso de *args e **kwargs aqui e insano
+        """
+
+        cell_args = kwargs.get("cell_args", None)
+        self.load_state(
+            state_matrix,
+            state_list,
+            cell_args=cell_args,
+            img_cell_size=self.img_cell_size,
+        )
+        self.cellMatrix.simulation_start(state_matrix, state_list)
+        self.agentList.simulation_start(state_matrix, state_list)
+
+        # this is stupid, is used just to keep track of the agents spawn queue
+        self.cell_instance = self.cellMatrix[0, 0]
+
+    # }}}
+
+    def update(self):
+        # {{{
+        """
+        Atualiza o estado da simulação, ou seja, realiza uma nova iteração.
+        """
+        old_state_list = self.agentList.state_list.copy()
+
+        for i in range(len(self.cell_instance._agent_spawn_queue)):
+            self.agentList.spawn_agent(
+                self.cell_instance._agent_spawn_queue[i]
+            )
+            self.cell_instance._agent_spawn_queue.pop(i)
+
+        self.agentList.update(self.cellMatrix.state_matrix)
+        self.cellMatrix.update(old_state_list)
+
+        # self.cell_instance._agent_spawn_queue = []
+
+        self.generation += 1
+
+    # }}}
+
+    def load_state(
+        self, state_matrix, state_list=None, cell_args=None, img_cell_size=1
+    ):
+        # {{{
+        """
+        Carrega uma matriz de estados a partir de uma imagem, uma
+        matriz numpy ou uma lista de listas.
+        """
+
+        self.generation = 0
+
+        if isinstance(state_matrix, str):
+            png_matrix = file_io.load_png(state_matrix, size=img_cell_size)
+            self.cellMatrix = CellMatrix.from_display(
+                png_matrix, self.cell_class, cell_args=cell_args
+            )
+            self.agentList = AgentList.from_display(
+                png_matrix, self.agent_class, cell_args=cell_args
+            )
+        elif isinstance(state_matrix, (np.ndarray, list)):
+            if isinstance(state_matrix, list):
+                state_matrix = np.array(state_matrix)
+            self.cellMatrix = CellMatrix(
+                state_matrix, self.cell_class, cell_args=cell_args
+            )
+            if state_list is None:
+                raise TypeError(
+                    "Agent's list of initial states (state_list) not "
+                    "provided to BoardBackendAgents.load_state."
+                )
+            elif isinstance(state_list, list):
+                self.agentList = AgentList(
+                    state_list, self.agent_class, cell_args=cell_args
+                )
+            else:
+                raise TypeError(
+                    f"{type(state_matrix)} is not a valid type for a state "
+                    "matrix."
+                )
+
+    # }}}
+
+    @property
+    def state_matrix(self):
+        return self.cellMatrix.state_matrix
+
+    @property
+    def state_list(self):
+        return self.agentList.state_list
+
+    @property
+    def display_matrix(self):
+        # {{{
+
+        display_matrix = self.cellMatrix.display()
+        agent_display_list = self.agentList.display()
+
+        for agent in agent_display_list:
+            display_matrix[agent.pos] = agent.rgb_tuple
+
+        return display_matrix
+
+    # }}}
+
 
 # }}}
```

### Comparing `tomato-engine-1.8.5/src/tomato/classes/cell.py` & `tomato-engine-2.0.0/src/tomato/classes/element.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,74 @@
-class CellTemplate:
+"""
+The abstraction that exists above Cell and Agent, and exists to store things in
+common between the two
+"""
+
+
+class ElementTemplate:
     # {{{
     """
-    Um template para a implementação de regras. Também define uma série de funções úteis
-    que serão herdadas. Tem um monte de pylint: disable aí porque isso deve servir
-    somente como uma classe template, ela não deve ser diretamente instanciada.
+    Class that exists just to contain both AgentTemplate and CellTemplate, so
+    agents and cells can share variables.
     """
-    # pylint: disable=no-self-use, unused-argument
 
-    def __init__(self, val, pos, cell_args=None):
+    _agent_spawn_queue = []
+
+    def spawn_agent(self, agent_tuple):
         # {{{
-        """
-        Durante a inicialização, cada célula precisa saber a sua
-        posição na matriz (para saber quais são seus vizinhos) e
-        seu valor inicial. Esse __init__ é o absoluto mínimo, mas
-        é claro que é possível sobrescrever esse init para
-        implementar mais coisa.
-        """
+        ElementTemplate._agent_spawn_queue.append(agent_tuple)
 
+    # }}}
+
+    def __init__(self, val, pos, cell_args=None):
+        # {{{
         self.lin, self.col = pos
         self.value = val
 
     # }}}
 
-    def update(self, state_matrix, cell_args=None):
+    def update(self, state_matrix, state_list=None):
         # {{{
-        """
-        É aqui que a célula recebe o estado do tabuleiro. e
-        atualiza seu próprio estado. Este é o método que é
-        executado em cada célula a cada iteração.
-        """
         ...
 
     # }}}
 
     @classmethod
-    def simulation_start(cls, state_matrix, cell_args=None):
+    def simulation_start(cls, state_matrix, state_list=None, cell_args=None):
         # {{{
-        """
-        Método executado somente uma vez no começo da simulação, antes da primeira
-        geração. Por padrão não faz nada.
-        """
         ...
 
     # }}}
 
     @classmethod
-    def generation_start(cls, state_matrix, cell_args=None):
+    def generation_start(cls, state_matrix, state_list=None):
         # {{{
         """
         Método executado somente uma vez no começo de cada geração. Por padrão não faz
         nada.
         """
         ...
 
     # }}}
 
     @classmethod
-    def generation_end(cls, state_matrix, cell_args=None):
+    def generation_end(cls, state_matrix, state_list=None):
         # {{{
-        """
-        Método executado somente uma vez por geração, depois do update. Por padrão não
-        faz nada.
-        """
         ...
 
     # }}}
 
     @property
     def pos(self):
         return (self.lin, self.col)
 
     @property
     def neighbors(self):
         # {{{
-        """
-        Aqui se implementa uma vizinhança arbitrária para o tipo
-        de célula. Também se pode usar uma das vizinhanças
-        padrão. Confira o exemplo rules/game_of_life.py.
-        """
-
-        raise NotImplementedError("Implementado na classe derivada")
+        raise NotImplementedError("Implemented in derived class")
 
     # }}}
 
     @property
     def moore_neighborhood(self):
         # {{{
         """
@@ -373,76 +358,48 @@
                 state_matrix[lin, prev_col],
             ]
 
         return neighbors
 
     # }}}
 
-    @staticmethod
-    def display(value):
+    @property
+    def agents_neighbors(self):
         # {{{
-        """
-        Retorna um array numpy com os valores RGB, ou um intenro
-        entre 0 e 255 para representar o autômato em função do
-        value.
-
-        O default é o caso binário, o mais simples.
-        """
-        return CellTemplate.display_binary(value)
+        raise NotImplementedError("Implemented in derived class")
 
     # }}}
 
-    @staticmethod
-    def from_display(rgb):
+    @property
+    def agents_moore_neighborhood(self):
         # {{{
-        """
-        Retorna o valor da célula a partir do array RGB que o
-        representa. É a operação inversa da função display.
+        lin, col = self.pos
+        neighbors = []
+        for agent in self.state_list:
+            if lin - 2 < agent.lin < lin + 2 and col - 2 < agent.col < col + 2:
+                neighbors.append(agent)
 
-        Novamente, o default é o caso binário.
-        """
-
-        return CellTemplate.from_binary(rgb)
+        return neighbors
 
     # }}}
 
     @staticmethod
-    def display_binary(value):
-        # {{{
-        """
-        Branco se o valor da célula for maior que zero, preto
-        caso contrário.
-        """
-
-        return 255 if value > 0 else 0
-
-    # }}}
+    def display(value):
+        ...
 
     @staticmethod
-    def from_binary(rgb):
-        # {{{
-        """
-        1 caso o valor seja maior que 0, 0 caso contrário.
-        """
-
-        return 1 if (rgb > 123).all() else 0
-
-    # }}}
+    def from_display(rgb):
+        ...
 
     @classmethod
     def init_from_display(cls, rgb, *args, **kwargs):
         # {{{
-        """
-        Inicializa a célula a partir de um array RGB. Este é o
-        método que de fato é chamado quando se carrega o estado
-        do tabuleiro a partir de uma imagem.
-        """
 
         return cls(cls.from_display(rgb), *args, **kwargs)
 
     # }}}
 
     def __repr__(self):
-        return f"Cell({self.value}, ({self.lin}, {self.col}))"
+        return f"Element({self.value}, ({self.lin}, {self.col}))"
 
 
 # }}}
```

### Comparing `tomato-engine-1.8.5/src/tomato/classes/cellmatrix.py` & `tomato-engine-2.0.0/src/tomato/classes/cell.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,89 @@
-from functools import partial
-from multiprocessing import Pool
-from types import ModuleType
-
 import numpy as np
 
-from .cell import CellTemplate
+from .element import ElementTemplate
 
 """
-Estrutura de dados para a matriz que contém todos os autômatos.
+Este módulo contém as classes que serão usadas para implementação de regras que
+não envolvem agentes
 """
 
 
-def cell_from_rule(rule):
+class CellMatrix:
     # {{{
-    """
-    A regra pode ser um módulo de Python contendo uma classe que herda de CellTemplate,
-    ou a própria classe. Esta função existe para que as demais funções deste módulo se
-    adequem a estes requisitos.
-    """
+    def __init__(self, state_matrix, cell_class, cell_args=None):
+        # {{{
+        """
+        Cria a matriz de autômatos a partir de uma regra e a
+        matriz de estado inicial.
+        """
 
-    if rule in CellTemplate.__subclasses__():
-        return rule
-    elif isinstance(rule, ModuleType):
-        for name in dir(rule):
-            try:
-                attribute = rule.__dict__[name]
-                return cell_from_rule(attribute)
-            except TypeError:
-                pass
-
-        raise TypeError(
-            f"Tipo {type(rule)} inválido para o parâmetro rule. "
-            "Tipos válidos são 'CellTemplate' e 'module'"
-        )
+        self.state_matrix = state_matrix.copy()
 
-    else:
-        raise TypeError(
-            f"Tipo {type(rule)} inválido para o parâmetro rule. "
-            "Tipos válidos são 'CellTemplate' e 'module'"
-        )
+        self.cell_args = cell_args
+        if cell_args is None:
+            self.cell_init = self.cell_init_nocellargs
+        else:
+            self.cell_init = self.cell_init_cellargs
 
+        self.Cell = cell_class
 
-# }}}
+        self.cell_matrix = np.array(
+            [
+                self.cell_init(value, (lin_num, col_num))
+                for lin_num, lin in enumerate(self.state_matrix)
+                for col_num, value in enumerate(lin)
+            ]
+        )
 
+        self.display_func = np.vectorize(self.Cell.display)
 
-class CellMatrix:
-    # {{{
-    def __init__(self, state_matrix, rule, cell_args=None):
+    # }}}
+
+    def update(self, *args):
         # {{{
         """
-        Cria a matriz de autômatos a partir de uma regra e a
-        matriz de estado inicial.
+        Atualiza o estado de todas as células. Detalhe que é
+        necessário copiar a matriz de estados porque matrizes do
+        numpy são passadas por referência. A state_matrix é
+        modificada in-place.
         """
 
-        self.Cell = cell_from_rule(rule)
+        old_state_matrix = self.state_matrix.copy()
+        self.Cell.generation_start(self.state_matrix, *args)
 
-        self.state_matrix = state_matrix.copy()
+        for cell in self.cell_matrix:
+            cell.update(old_state_matrix, *args)
+            self.state_matrix[cell.pos] = cell.value
 
-        if cell_args is not None:
-            self.cell_matrix = np.array(
-                [
-                    self.Cell(value, (lin_num, col_num), cell_args)
-                    for lin_num, lin in enumerate(self.state_matrix)
-                    for col_num, value in enumerate(lin)
-                ]
-            )
-        else:
-            self.cell_matrix = np.array(
-                [
-                    self.Cell(value, (lin_num, col_num))
-                    for lin_num, lin in enumerate(self.state_matrix)
-                    for col_num, value in enumerate(lin)
-                ]
-            )
+        self.Cell.generation_end(self.state_matrix, *args)
 
-        self.display_func = np.vectorize(self.Cell.display)
+        return self.state_matrix
 
     # }}}
 
     @classmethod
-    def from_display(cls, display_matrix, rule, cell_args=None):
+    def from_display(cls, display_matrix, cell_class, cell_args=None):
         # {{{
         """
         Inicializa a partir da matriz de valores RGB ou valor de
         escala monocromática extraídos de uma imagem. Essa
         provavelmente é a maneira mais lenta possível de se fazer
         isso.
         """
-    
-        cell = cell_from_rule(rule)
 
-        cell_from_display = cell.from_display
-        pixels_gen = (cell_from_display(col) for lin in display_matrix for col in lin)
+        cell_from_display = cell_class.from_display
+        pixels_gen = (
+            cell_from_display(col) for lin in display_matrix for col in lin
+        )
 
         state_matrix = np.array(list(pixels_gen))
         state_matrix = state_matrix.reshape(display_matrix.shape[:2])
 
-        return cls(state_matrix, rule, cell_args)
+        return cls(state_matrix, cell_class, cell_args)
 
     # }}}
 
     def display(self):
         # {{{
         """
         Retorna a matriz para representação visual do conjunto de
@@ -115,76 +98,97 @@
             rgb_tuple = (rgb_tuple, rgb_tuple, rgb_tuple)
 
         rgb_matrix = np.dstack(rgb_tuple).astype(np.uint8)
         return rgb_matrix
 
     # }}}
 
-    def simulation_start(self, state_matrix, cell_args):
-        self.Cell.simulation_start(state_matrix, cell_args)
+    def cell_init_nocellargs(self, value, pos):
+        # {{{
+        return self.Cell(value, pos)
+
+    # }}}
+
+    def cell_init_cellargs(self, value, pos):
+        # {{{
+        return self.Cell(value, pos, self.cell_args)
+
+    # }}}
+
+    def simulation_start(self, state_matrix, *args):
+# {{{
+        if self.cell_args is None:
+            self.Cell.simulation_start(state_matrix, *args)
+        else:
+            self.Cell.simulation_start(
+                state_matrix, *args, cell_args=self.cell_args
+            )
+# }}}
 
     @property
     def shape(self):
         return self.state_matrix.shape
 
+    def __getitem__(self, key):
+        return self.cell_matrix.reshape(self.state_matrix.shape)[key]
+
 
 # }}}
 
 
-class CellMatrixThreaded(CellMatrix):
+class CellTemplate(ElementTemplate):
     # {{{
-    def update(self, *args, **kwargs):
-        # {{{
-
-        old_state_matrix = self.state_matrix
+    """
+    Um template para a implementação de células. Também define uma série de
+    funções úteis que serão herdadas. Tem um monte de pylint: disable aí porque
+    isso deve servir somente como uma classe template, ela não deve ser
+    diretamente instanciada.
+    """
+    # pylint: disable=no-self-use, unused-argument
 
-        update_cell = partial(
-            self.update_cell, old_state_matrix=old_state_matrix, *args, **kwargs
-        )
+    def __repr__(self):
+        return f"Cell({self.value}, ({self.lin}, {self.col}))"
 
-        with Pool() as p:
-            new_state_matrix = p.map(update_cell, self.cell_matrix)
+    @staticmethod
+    def display(value):
+        # {{{
+        return CellTemplate.display_binary(value)
 
-        for cell, new_value in zip(self.cell_matrix, new_state_matrix):
-            cell.value = new_value
+    # }}}
 
-        self.state_matrix = np.array(new_state_matrix).reshape(old_state_matrix.shape)
+    @staticmethod
+    def from_display(rgb):
+        # {{{
 
-        return self.state_matrix
+        return CellTemplate.from_binary(rgb)
 
     # }}}
 
     @staticmethod
-    def update_cell(cell, old_state_matrix, *args, **kwargs):
-        cell.update(old_state_matrix, *args, **kwargs)
-        return cell.value
-
+    def display_binary(value):
+        # {{{
 
-# }}}
+        return 255 if value > 0 else 0
 
+    # }}}
 
-class CellMatrixUnthreaded(CellMatrix):
-    # {{{
-    def update(self, *args, **kwargs):
+    @staticmethod
+    def from_binary(rgb):
         # {{{
-        """
-        Atualiza o estado de todas as células. Detalhe que é
-        necessário copiar a matriz de estados porque matrizes do
-        numpy são passadas por referência. A state_matrix é
-        modificada in-place.
-        """
 
-        old_state_matrix = self.state_matrix.copy()
-        self.Cell.generation_start(self.state_matrix, *args, **kwargs)
+        return 1 if (rgb > 123).all() else 0
 
-        for cell in self.cell_matrix:
-            cell.update(old_state_matrix, *args, **kwargs)
-            self.state_matrix[cell.pos] = cell.value
+    # }}}
 
-        self.Cell.generation_end(self.state_matrix, *args, **kwargs)
+    @property
+    def agent_above(self):
+        # {{{
+        for agent_tuple in self.agent_list:
+            if self.pos == agent_tuple.pos:
+                return agent_tuple
+        return False
 
-        return self.state_matrix
 
-    # }}}
+# }}}
 
 
 # }}}
```

### Comparing `tomato-engine-1.8.5/src/tomato/classes/window.py` & `tomato-engine-2.0.0/src/tomato/classes/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from ..functions import display
 from time import time
 from numpy import mean, std
 
 from os import environ
-environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
+
+environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
 import pygame
 
+
 class Window:
 
     """
     Uma classe para ser a representação da janelinha da simulação
     no projeto. Sim, porque não temos overhead suficiente.
 
     Nota-se que a Window não tem acesso direto à CellMatrix. Tudo
```

### Comparing `tomato-engine-1.8.5/src/tomato/functions/display.py` & `tomato-engine-2.0.0/src/tomato/functions/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 """
 
 
 def create_screen(cells, cell_size, title):
     # {{{
     cells_y, cells_x = cells
 
-    screen = pygame.display.set_mode((cells_x * cell_size, cells_y * cell_size))
+    screen = pygame.display.set_mode(
+        (cells_x * cell_size, cells_y * cell_size)
+    )
     pygame.display.set_caption(title)
 
     return screen
 
 
 # }}}
```

### Comparing `tomato-engine-1.8.5/src/tomato/functions/file_io.py` & `tomato-engine-2.0.0/src/tomato/functions/file_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,17 @@
     line = separator.join(str(x) for x in values) + "\n"
     file_obj.write(line)
 
 
 # }}}
 
 
-def read_from_record(file_path, value_types=None, num_values=None, separator="\t"):
+def read_from_record(
+    file_path, value_types=None, num_values=None, separator="\t"
+):
     # {{{
     """
     Lê os valores de cada linha de file_obj.
 
     file_types é uma tupla de tipos (como int, float, np.uint8, etc.), e tem
     que ter o mesmo comprimento do número de valores em cada linha a ser lida
     do arquivo. Essa função vai converter os valores que lê do arquivo aos
@@ -121,15 +123,14 @@
     elif value_types is not None:
         num_values = len(value_types)
 
     # Tupla com uma lista para cada coluna no arquivo
     cols = tuple([] for x in range(num_values))
 
     with open(file_path, "r") as record:
-
         # Poderia colocar esses elifs dentro do for line in record, mas aí
         # seria mais lento, apesar de mais sucinto
         if value_types is None:
             for line in record:
                 separated_line = line.split(separator)
 
                 for index, col in enumerate(cols):
```

### Comparing `tomato-engine-1.8.5/src/tomato/functions/utils.py` & `tomato-engine-2.0.0/src/tomato/functions/utils.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.5/src/tomato/rules/game_of_life.py` & `tomato-engine-2.0.0/src/tomato/rules/game_of_life.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from tomato.classes import cell
 
 """
 Author: Eduardo Lopes Dias (codeberg.org/eduardotogpi)
 
-An implementation of Conways' classic Game of Life. Besides being cool to look at, it
-serves as a simple example as to how new rulesets can be implemented.
+An implementation of Conways' classic Game of Life. Besides being cool to look
+at, it serves as a simple example as to how new rulesets can be implemented.
 """
 
 
 class Cell(cell.CellTemplate):
     # {{{
     def update(self, state_matrix):
         self.state_matrix = state_matrix
```

### Comparing `tomato-engine-1.8.5/src/tomato/rules/toothpick_fractal.py` & `tomato-engine-2.0.0/src/tomato/rules/toothpick_fractal.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 The 'toothpick fractal' featured on episode 'Terrific Toothpick Patterns' of
 Numberphile. The Von Neumann neighborhood version of this rule is known as the
 Ulam-Warbuton Cellular Automaton. Included this mainly because it's a notable and fun
 rule.
 """
 
 
-class Cell(cell.CellTemplate):
+class ToothpickCell(cell.CellTemplate):
     # {{{
     @classmethod
-    def simulation_start(cls, state_matrix, neighborhood):
-        neighborhood = getattr(Cell, f"{neighborhood}_neighborhood")
-        setattr(Cell, "neighbors", neighborhood)
+    def simulation_start(cls, state_matrix, cell_args):
+        neighborhood = getattr(ToothpickCell, f"{cell_args}_neighborhood")
+        setattr(ToothpickCell, "neighbors", neighborhood)
 
     def update(self, state_matrix):
         self.state_matrix = state_matrix
 
         if sum(self.neighbors) == 1:  # only one live neighbor
             self.value = 1
```

### Comparing `tomato-engine-1.8.5/src/tomato_engine.egg-info/PKG-INFO` & `tomato-engine-2.0.0/src/tomato_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-engine
-Version: 1.8.5
+Version: 2.0.0
 Summary: Engine for prototyping and playing with cellular automata
 Home-page: https://codeberg.org/eduardotogpi/tomato-engine
 Author: Eduardo Lopes Dias, Murilo Melhem
 Author-email: eduardosprp@usp.br
 Project-URL: Bug Tracker, https://codeberg.org/eduardotogpi/tomato-engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tomato-engine-1.8.5/src/tomato_engine.egg-info/SOURCES.txt` & `tomato-engine-2.0.0/src/tomato_engine.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/tomato/__init__.py
 src/tomato/classes/__init__.py
+src/tomato/classes/agent.py
 src/tomato/classes/board.py
 src/tomato/classes/cell.py
-src/tomato/classes/cellmatrix.py
+src/tomato/classes/element.py
 src/tomato/classes/window.py
 src/tomato/functions/__init__.py
 src/tomato/functions/display.py
 src/tomato/functions/file_io.py
+src/tomato/functions/handling_rules.py
 src/tomato/functions/utils.py
 src/tomato/rules/__init__.py
-src/tomato/rules/colorful.py
-src/tomato/rules/colorful_demo.py
+src/tomato/rules/automata1D.py
+src/tomato/rules/automata1D_demo.py
 src/tomato/rules/cyclic.py
 src/tomato/rules/cyclic_demo.py
 src/tomato/rules/game_of_life.py
 src/tomato/rules/game_of_life_demo.py
+src/tomato/rules/langtons_ant.py
+src/tomato/rules/langtons_ant_demo.py
+src/tomato/rules/random_walkers.py
+src/tomato/rules/random_walkers_demo.py
+src/tomato/rules/tomato_life.py
+src/tomato/rules/tomato_life_demo.py
 src/tomato/rules/toothpick_fractal.py
 src/tomato/rules/toothpick_fractal_demo.py
 src/tomato_engine.egg-info/PKG-INFO
 src/tomato_engine.egg-info/SOURCES.txt
 src/tomato_engine.egg-info/dependency_links.txt
 src/tomato_engine.egg-info/requires.txt
 src/tomato_engine.egg-info/top_level.txt
```

