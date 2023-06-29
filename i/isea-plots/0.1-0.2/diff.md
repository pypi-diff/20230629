# Comparing `tmp/isea_plots-0.1.tar.gz` & `tmp/isea_plots-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isea_plots-0.1.tar", last modified: Thu Jun 29 17:02:47 2023, max compression
+gzip compressed data, was "isea_plots-0.2.tar", last modified: Thu Jun 29 17:46:04 2023, max compression
```

## Comparing `isea_plots-0.1.tar` & `isea_plots-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 17:02:47.340192 isea_plots-0.1/
--rw-rw-rw-   0        0        0     1104 2023-06-29 16:22:50.000000 isea_plots-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      362 2023-06-29 17:02:47.341190 isea_plots-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-06-29 16:09:48.000000 isea_plots-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 17:02:47.313495 isea_plots-0.1/isea_plots/
--rw-rw-rw-   0        0        0       46 2023-06-29 16:29:06.000000 isea_plots-0.1/isea_plots/__init__.py
--rw-rw-rw-   0        0        0    10573 2023-06-29 14:59:19.000000 isea_plots-0.1/isea_plots/isea_plots.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:02:47.338184 isea_plots-0.1/isea_plots.egg-info/
--rw-rw-rw-   0        0        0      362 2023-06-29 17:02:46.000000 isea_plots-0.1/isea_plots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-06-29 17:02:46.000000 isea_plots-0.1/isea_plots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 17:02:46.000000 isea_plots-0.1/isea_plots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-29 17:02:46.000000 isea_plots-0.1/isea_plots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-29 17:02:46.000000 isea_plots-0.1/isea_plots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-06-29 17:02:47.347010 isea_plots-0.1/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-06-29 17:02:37.000000 isea_plots-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:46:04.986380 isea_plots-0.2/
+-rw-rw-rw-   0        0        0     1104 2023-06-29 16:22:50.000000 isea_plots-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      362 2023-06-29 17:46:04.986380 isea_plots-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2023-06-29 16:09:48.000000 isea_plots-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 17:46:04.959793 isea_plots-0.2/isea_plots/
+-rw-rw-rw-   0        0        0       46 2023-06-29 16:29:06.000000 isea_plots-0.2/isea_plots/__init__.py
+-rw-rw-rw-   0        0        0    10330 2023-06-29 17:37:47.000000 isea_plots-0.2/isea_plots/isea_plots.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:46:04.983379 isea_plots-0.2/isea_plots.egg-info/
+-rw-rw-rw-   0        0        0      362 2023-06-29 17:46:04.000000 isea_plots-0.2/isea_plots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-29 17:46:04.000000 isea_plots-0.2/isea_plots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 17:46:04.000000 isea_plots-0.2/isea_plots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-29 17:46:04.000000 isea_plots-0.2/isea_plots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-29 17:46:04.000000 isea_plots-0.2/isea_plots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-06-29 17:46:04.992056 isea_plots-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-06-29 17:44:16.000000 isea_plots-0.2/setup.py
```

### Comparing `isea_plots-0.1/LICENSE.txt` & `isea_plots-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `isea_plots-0.1/isea_plots/isea_plots.py` & `isea_plots-0.2/isea_plots/isea_plots.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,128 @@
 from matplotlib.patches import Rectangle
 from matplotlib.text import Text
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as numpy
 
+farben = {
+    'blau1': numpy.array([0, 84, 159]) / 255,
+    'blau2': numpy.array([64, 127, 183]) / 255,
+    'blau3': numpy.array([142, 186, 229]) / 255,
+    'blau4': numpy.array([199, 221, 242]) / 255,
+    'blau5': numpy.array([232, 241, 250]) / 255,
+    'petrol1': numpy.array([0, 97, 101]) / 255,
+    'petrol2': numpy.array([45, 127, 131]) / 255,
+    'petrol3': numpy.array([125, 164, 167]) / 255,
+    'petrol4': numpy.array([191, 209, 209]) / 255,
+    'petrol5': numpy.array([230, 236, 236]) / 255,
+    'tuerkis1': numpy.array([0, 152, 161]) / 255,
+    'tuerkis2': numpy.array([0, 177, 183]) / 255,
+    'tuerkis3': numpy.array([137, 204, 207]) / 255,
+    'tuerkis4': numpy.array([202, 231, 231]) / 255,
+    'tuerkis5': numpy.array([235, 246, 246]) / 255,
+    'maigruen1': numpy.array([189, 205, 0]) / 255,
+    'maigruen2': numpy.array([208, 217, 92]) / 255,
+    'maigruen3': numpy.array([224, 230, 154]) / 255,
+    'maigruen4': numpy.array([240, 243, 208]) / 255,
+    'maigruen5': numpy.array([249, 250, 237]) / 255,
+    'gruen1': numpy.array([87, 171, 39]) / 255,
+    'gruen2': numpy.array([141, 192, 96]) / 255,
+    'gruen3': numpy.array([184, 214, 152]) / 255,
+    'gruen4': numpy.array([221, 235, 206]) / 255,
+    'gruen5': numpy.array([242, 247, 236]) / 255,
+    'orange1': numpy.array([246, 168, 0]) / 255,
+    'orange2': numpy.array([250, 190, 80]) / 255,
+    'orange3': numpy.array([253, 212, 143]) / 255,
+    'orange4': numpy.array([254, 234, 201]) / 255,
+    'orange5': numpy.array([255, 247, 234]) / 255,
+    'bordeaux1': numpy.array([161, 16, 53]) / 255,
+    'bordeaux2': numpy.array([182, 82, 86]) / 255,
+    'bordeaux3': numpy.array([205, 139, 135]) / 255,
+    'bordeaux4': numpy.array([229, 197, 192]) / 255,
+    'bordeaux5': numpy.array([245, 232, 229]) / 255,
+    'violett1': numpy.array([97, 33, 88]) / 255,
+    'violett2': numpy.array([131, 78, 117]) / 255,
+    'violett3': numpy.array([168, 133, 158]) / 255,
+    'violett4': numpy.array([210, 192, 205]) / 255,
+    'violett5': numpy.array([237, 229, 234]) / 255,
+    'lila1': numpy.array([122, 11, 172]) / 255,
+    'lila2': numpy.array([155, 145, 193]) / 255,
+    'lila3': numpy.array([188, 181, 215]) / 255,
+    'lila4': numpy.array([222, 218, 235]) / 255,
+    'lila5': numpy.array([242, 240, 247]) / 255,
+    'magenta1': numpy.array([227, 0, 102]) / 255,
+    'magenta2': numpy.array([233, 96, 136]) / 255,
+    'magenta3': numpy.array([241, 158, 177]) / 255,
+    'magenta4': numpy.array([249, 210, 218]) / 255,
+    'magenta5': numpy.array([253, 238, 240]) / 255,
+    'gelb1': numpy.array([255, 237, 0]) / 255,
+    'gelb2': numpy.array([255, 240, 85]) / 255,
+    'gelb3': numpy.array([255, 245, 155]) / 255,
+    'gelb4': numpy.array([255, 250, 209]) / 255,
+    'gelb5': numpy.array([255, 253, 238]) / 255,
+    'grau1': numpy.array([88, 88, 88]) / 255,
+    'grau2': numpy.array([118, 118, 118]) / 255
+}
+
+
 class isea_plots():
-    def __init__(self):
-        self.farben = {
-            'blau1': numpy.array([0, 84, 159])/255,
-            'blau2': numpy.array([64, 127, 183])/255,
-            'blau3': numpy.array([142, 186, 229])/255,
-            'blau4': numpy.array([199, 221, 242])/255,
-            'blau5': numpy.array([232, 241, 250])/255,
-            'petrol1': numpy.array([0, 97, 101])/255,
-            'petrol2': numpy.array([45, 127, 131])/255,
-            'petrol3': numpy.array([125, 164, 167])/255,
-            'petrol4': numpy.array([191, 209, 209])/255,
-            'petrol5': numpy.array([230, 236, 236])/255,
-            'tuerkis1': numpy.array([0, 152, 161])/255,
-            'tuerkis2': numpy.array([0, 177, 183])/255,
-            'tuerkis3': numpy.array([137, 204, 207])/255,
-            'tuerkis4': numpy.array([202, 231, 231])/255,
-            'tuerkis5': numpy.array([235, 246, 246])/255,
-            'maigruen1': numpy.array([189, 205, 0])/255,
-            'maigruen2': numpy.array([208, 217, 92])/255,
-            'maigruen3': numpy.array([224, 230, 154])/255,
-            'maigruen4': numpy.array([240, 243, 208])/255,
-            'maigruen5': numpy.array([249, 250, 237])/255,
-            'gruen1': numpy.array([87, 171, 39])/255,
-            'gruen2': numpy.array([141, 192, 96])/255,
-            'gruen3': numpy.array([184, 214, 152])/255,
-            'gruen4': numpy.array([221, 235, 206])/255,
-            'gruen5': numpy.array([242, 247, 236])/255,
-            'orange1': numpy.array([246, 168, 0])/255,
-            'orange2': numpy.array([250, 190, 80])/255,
-            'orange3': numpy.array([253, 212, 143])/255,
-            'orange4': numpy.array([254, 234, 201])/255,
-            'orange5': numpy.array([255, 247, 234])/255,
-            'bordeaux1': numpy.array([161, 16, 53])/255,
-            'bordeaux2': numpy.array([182, 82, 86])/255,
-            'bordeaux3': numpy.array([205, 139, 135])/255,
-            'bordeaux4': numpy.array([229, 197, 192])/255,
-            'bordeaux5': numpy.array([245, 232, 229])/255,
-            'violett1': numpy.array([97, 33, 88])/255,
-            'violett2': numpy.array([131, 78, 117])/255,
-            'violett3': numpy.array([168, 133, 158])/255,
-            'violett4': numpy.array([210, 192, 205])/255,
-            'violett5': numpy.array([237, 229, 234])/255,
-            'lila1': numpy.array([122, 11, 172])/255,
-            'lila2': numpy.array([155, 145, 193])/255,
-            'lila3': numpy.array([188, 181, 215])/255,
-            'lila4': numpy.array([222, 218, 235])/255,
-            'lila5': numpy.array([242, 240, 247])/255,
-            'magenta1': numpy.array([227, 0, 102])/255,
-            'magenta2': numpy.array([233, 96, 136])/255,
-            'magenta3': numpy.array([241, 158, 177])/255,
-            'magenta4': numpy.array([249, 210, 218])/255,
-            'magenta5': numpy.array([253, 238, 240])/255,
-            'gelb1': numpy.array([255, 237, 0])/255,
-            'gelb2': numpy.array([255, 240, 85])/255,
-            'gelb3': numpy.array([255, 245, 155])/255,
-            'gelb4': numpy.array([255, 250, 209])/255,
-            'gelb5': numpy.array([255, 253, 238])/255,
-            'grau1': numpy.array([88, 88, 88])/255,
-            'grau2': numpy.array([118, 118, 118])/255}
 
-    def create_bar_chart(self,x, plot_name,x_label,y_label, result_path, color_grid,title, legend_titles, *args,  colors, figwhide=8, figheight=4):
+    def create_bar_chart(x, plot_name, x_label, y_label, result_path, color_grid, title, legend_titles, *args, colors,
+                         figwhide=8, figheight=4):
 
-        fig, axes = plt.subplots(figsize=(figwhide,figheight))
-        color_plot = [self.farben[color] for color in colors]
+        fig, axes = plt.subplots(figsize=(figwhide, figheight))
+        color_plot = [farben[color] for color in colors]
         plot_spacing = 1 / (len(x))
         xticks = numpy.arange(len(x))
         for i, arg in enumerate(args):
-            plt.bar(x, arg.values, color=color_plot[i], width=plot_spacing, label=legend_titles[i])
+            plt.bar(x, arg, color=color_plot[i], width=plot_spacing, label=legend_titles[i])
 
-            #plot_data = list(plotting_frame.loc[:, x[ctr_x]])
+            # plot_data = list(plotting_frame.loc[:, x[ctr_x]])
 
-            #ax[ctr_x, 0].bar(xticks, plot_data, , color=color_plot[i], label=legend_titles[i])
+            # ax[ctr_x, 0].bar(xticks, plot_data, , color=color_plot[i], label=legend_titles[i])
             x = [x + plot_spacing for x in xticks]
 
-        plt.grid(color =color_grid, linewidth=0.5, alpha=0.7, zorder=-3)
+        plt.grid(color=farben[color_grid], linewidth=0.5, alpha=0.7, zorder=-3)
         axes.set_axisbelow(True)
         plt.xlabel(xlabel=x_label)
         plt.ylabel(ylabel=y_label)
         plt.title(title)
-        axes.spines['top'].set_color(color_grid)
+        axes.spines['top'].set_color(farben[color_grid])
         axes.spines['top'].set_linewidth(0.5)
         axes.spines['top'].set_alpha(0.7)
-        axes.spines['right'].set_color(color_grid)
+        axes.spines['right'].set_color(farben[color_grid])
         axes.spines['right'].set_linewidth(0.5)
         axes.spines['right'].set_alpha(0.7)
         axes.tick_params(direction='in')
         axes.tick_params(axis='x', pad=10)
-        max_list =[]
+        max_list = []
         for arg in args:
             max_list.append(max(arg))
         max_all = max(max_list)
-        y_max =max_all * 1.1
-        axes.set_ylim([None,y_max])
-
-
+        y_max = max_all * 1.1
+        axes.set_ylim([None, y_max])
 
         # plot save integrieren, Fenstergröße einstellen
 
-        #rect = Rectangle((1 - 0.3, 1 - 0.1), 0.3, 0.08, facecolor='None', edgecolor='None', transform=axes.transAxes)
-        text = Text(1 - 0.16, 1 - 0.06, "\u00A9 ISEA RWTH Aachen", fontsize=10, ha='center', va='center', transform=axes.transAxes, color=self.farben['blau1'])
+        # rect = Rectangle((1 - 0.3, 1 - 0.1), 0.3, 0.08, facecolor='None', edgecolor='None', transform=axes.transAxes)
+        text = Text(1 - 0.16, 1 - 0.06, "\u00A9 ISEA RWTH Aachen", fontsize=10, ha='center', va='center',
+                    transform=axes.transAxes, color=farben['blau1'])
 
-        #axes.add_artist(rect)
+        # axes.add_artist(rect)
         axes.add_artist(text)
 
         plt.legend()
         plt.show()
         plt.savefig(result_path + '/' + plot_name + '.png')
 
-    def create_stacked_bar_chart(self,x, plot_name, result_path, color_grid, title, legend_titles, *args, colors, figwhide=8, figheight=4):
+    def create_stacked_bar_chart(x, plot_name, result_path, color_grid, title, legend_titles, *args, colors, figwhide=8,
+                                 figheight=4):
         fig, axes = plt.subplots(figsize=(figwhide, figheight))
-        color_plot = [self.farben[color] for color in colors]
+        color_plot = [farben[color] for color in colors]
 
         # Prepare the data
         data = []
         for arg in args:
             data.append(numpy.array(list(arg)))
 
         # Create the stacked bars
@@ -139,96 +142,94 @@
         axes.spines['right'].set_linewidth(0.5)
         axes.spines['right'].set_alpha(0.7)
         plt.grid(color=color_grid, linewidth=0.5, alpha=0.7, zorder=-3)
         axes.set_axisbelow(True)
 
         rect = Rectangle((1 - 0.3, 1 - 0.1), 0.3, 0.08, facecolor='None', edgecolor='None', transform=axes.transAxes)
         text = Text(1 - 0.16, 1 - 0.06, "\u00A9 ISEA RWTH Aachen", fontsize=10, ha='center', va='center',
-                    transform=axes.transAxes, color=self.farben['blau1'])
+                    transform=axes.transAxes, color=farben['blau1'])
 
         axes.add_artist(rect)
         axes.add_artist(text)
 
         # Add legend and save plot
         plt.legend()
         plt.show()
         plt.savefig(result_path + '/' + plot_name + '.png')
 
-    def create_line_chart(self,t, plot_name, result_path, color_grid,title, legend_titles, linestyle, *args,  colors,figwhide=8, figheight=4):
+    def create_line_chart(t, plot_name, result_path, color_grid, title, legend_titles, linestyle, *args, colors,
+                          figwhide=8, figheight=4):
 
-        fig, axes = plt.subplots(figsize=(figwhide,figheight))
-        color_plot = [self.farben[color] for color in colors]
+        fig, axes = plt.subplots(figsize=(figwhide, figheight))
+        color_plot = [farben[color] for color in colors]
 
         'abstände am anfang und ende gleich, stack bar plot integrieren in bar plot'
         for i, arg in enumerate(args):
             plt.plot(t, arg.values, color=color_plot[i], label=legend_titles[i], linestyle=linestyle)
 
-
-
-        plt.grid(color =color_grid, linewidth=0.5, alpha=0.7, zorder=-3)
+        plt.grid(color=color_grid, linewidth=0.5, alpha=0.7, zorder=-3)
         axes.set_axisbelow(True)
         plt.ylabel(ylabel='y')
         plt.ylabel(ylabel='y')
         plt.title(title)
         axes.spines['top'].set_color(color_grid)
         axes.spines['top'].set_linewidth(0.5)
         axes.spines['top'].set_alpha(0.7)
         axes.spines['right'].set_color(color_grid)
         axes.spines['right'].set_linewidth(0.5)
         axes.spines['right'].set_alpha(0.7)
         axes.tick_params(direction='in')
 
         # Berechnen des Abstands zwischen den x-Achsen-Ticks
-        x_tick_distance = (axes.get_xlim()[1] - axes.get_xlim()[0]) / (len(t) -1 )
+        x_tick_distance = (axes.get_xlim()[1] - axes.get_xlim()[0]) / (len(t) - 1)
         # Setzen des Abstands des ersten Datenpunktes zur y-Achse
-        axes.set_xlim(axes.get_xlim()[0] , axes.get_xlim()[1])
-
+        axes.set_xlim(axes.get_xlim()[0], axes.get_xlim()[1])
 
         axes.tick_params(axis='x', pad=10)
 
-
         rect = Rectangle((1 - 0.3, 1 - 0.1), 0.3, 0.08, facecolor='None', edgecolor='None', transform=axes.transAxes)
-        text = Text(1 - 0.16, 1 - 0.06, "\u00A9 ISEA RWTH Aachen", fontsize=10, ha='center', va='center', transform=axes.transAxes, color=self.farben['blau1'])
+        text = Text(1 - 0.16, 1 - 0.06, "\u00A9 ISEA RWTH Aachen", fontsize=10, ha='center', va='center',
+                    transform=axes.transAxes, color=farben['blau1'])
 
         axes.add_artist(rect)
         axes.add_artist(text)
 
         plt.legend()
         plt.show()
         plt.savefig(result_path + '/' + plot_name + '.png')
-    def create_scatter_chart(self,x, plot_name, result_path, color_grid,title, legend_titles, *args,  colors, figwidth=8, figheight=4 ):
+
+    def create_scatter_chart(x, plot_name, result_path, color_grid, title, legend_titles, *args, colors, figwidth=8,
+                             figheight=4):
 
         fig, axes = plt.subplots(figsize=(figwidth, figheight))
         plot_spacing = 1 / (len(x))
-        color_plot = [self.farben[color] for color in colors]
+        color_plot = [farben[color] for color in colors]
         for i, arg in enumerate(args):
             plt.plot(x, arg.values, 'o', color=color_plot[i], label=legend_titles[i])
 
-
-
-        plt.grid(color =color_grid, linewidth=0.5, alpha=0.7, zorder=-3)
+        plt.grid(color=color_grid, linewidth=0.5, alpha=0.7, zorder=-3)
         axes.set_axisbelow(True)
         plt.ylabel(ylabel='y')
         plt.ylabel(ylabel='y')
         plt.title(title)
         axes.spines['top'].set_color(color_grid)
         axes.spines['top'].set_linewidth(0.5)
         axes.spines['top'].set_alpha(0.7)
         axes.spines['right'].set_color(color_grid)
         axes.spines['right'].set_linewidth(0.5)
         axes.spines['right'].set_alpha(0.7)
         axes.tick_params(direction='in')
 
-
-
         axes.tick_params(axis='x', pad=10)
 
         rect = Rectangle((1 - 0.3, 1 - 0.1), 0.3, 0.08, facecolor='None', edgecolor='None', transform=axes.transAxes)
-        text = Text(1 - 0.16, 1 - 0.06, "\u00A9 ISEA RWTH Aachen", fontsize=10, ha='center', va='center', transform=axes.transAxes, color=self.farben['blau1'])
+        text = Text(1 - 0.16, 1 - 0.06, "\u00A9 ISEA RWTH Aachen", fontsize=10, ha='center', va='center',
+                    transform=axes.transAxes, color=farben['blau1'])
 
         axes.add_artist(rect)
         axes.add_artist(text)
         plt.legend()
         plt.show()
-if __name__ == "__main__":
 
-    test = pd.DataFrame({'X': ['Eigenheim', 'Gewerbe', 'Großspeicher', 'EV'], 'Y': [5, 6, 7, 8], 'Z': [2,3,4,5]})
+
+if __name__ == "__main__":
+    test = pd.DataFrame({'X': ['Eigenheim', 'Gewerbe', 'Großspeicher', 'EV'], 'Y': [5, 6, 7, 8], 'Z': [2, 3, 4, 5]})
```

