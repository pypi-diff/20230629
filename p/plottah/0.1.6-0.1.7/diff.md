# Comparing `tmp/plottah-0.1.6.tar.gz` & `tmp/plottah-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plottah-0.1.6.tar", max compression
+gzip compressed data, was "plottah-0.1.7.tar", max compression
```

## Comparing `plottah-0.1.6.tar` & `plottah-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      835 2023-06-28 09:10:14.987435 plottah-0.1.6/README.md
--rw-r--r--   0        0        0       22 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/__init__.py
--rw-r--r--   0        0        0     1617 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/__main__.py
--rw-r--r--   0        0        0     1339 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/colors.py
--rw-r--r--   0        0        0     4266 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/config.py
--rw-r--r--   0        0        0       24 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/plot_builder/__init__.py
--rw-r--r--   0        0        0     2884 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/plot_builder/builders.py
--rw-r--r--   0        0        0     7487 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/plot_handler/PlotHandler.py
--rw-r--r--   0        0        0       37 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/plot_handler/__init__.py
--rw-r--r--   0        0        0     9975 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/plots/BinEventRatePlot.py
--rw-r--r--   0        0        0     3987 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/plots/DistPlot.py
--rw-r--r--   0        0        0     1927 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/plots/PlotProtocol.py
--rw-r--r--   0        0        0     3578 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/plots/RocCurvePlot.py
--rw-r--r--   0        0        0      117 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/plots/__init__.py
--rw-r--r--   0        0        0     4179 2023-06-28 09:10:16.003464 plottah-0.1.6/plottah/utils.py
--rw-r--r--   0        0        0      505 2023-06-28 09:10:44.675516 plottah-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 plottah-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-29 10:06:25.944332 plottah-0.1.7/README.md
+-rw-r--r--   0        0        0       22 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/__init__.py
+-rw-r--r--   0        0        0     2648 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/__main__.py
+-rw-r--r--   0        0        0     1339 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/colors.py
+-rw-r--r--   0        0        0     4841 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/config.py
+-rw-r--r--   0        0        0       24 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plot_builder/__init__.py
+-rw-r--r--   0        0        0     3821 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plot_builder/builders.py
+-rw-r--r--   0        0        0     7563 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plot_handler/PlotHandler.py
+-rw-r--r--   0        0        0       37 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plot_handler/__init__.py
+-rw-r--r--   0        0        0    10631 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plots/BinEventRatePlot.py
+-rw-r--r--   0        0        0     3987 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plots/DistPlot.py
+-rw-r--r--   0        0        0     3030 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plots/PlotProtocol.py
+-rw-r--r--   0        0        0     3578 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plots/RocCurvePlot.py
+-rw-r--r--   0        0        0      117 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plots/__init__.py
+-rw-r--r--   0        0        0     4179 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/utils.py
+-rw-r--r--   0        0        0      529 2023-06-29 10:06:56.908714 plottah-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2015 1970-01-01 00:00:00.000000 plottah-0.1.7/PKG-INFO
```

### Comparing `plottah-0.1.6/README.md` & `plottah-0.1.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 
 ### Requirements
 
 * Python (>=3.6)
 
 ### Development environment
 
+Clone the repo, give name plotting_analyis
+```shell
+git clone git@github.com:nielsota/plottah.git plotting_analysis
+```
+```shell
+cd plotting_analysis
+```
+
 Create a virtual environment by running:
 
 ```shell
 python -m venv .venv
 ```
 
 The virtual environment should be activated every time you start a new shell session before running subsequent commands:
@@ -21,14 +29,18 @@
 > ```shell
 > source .venv/bin/activate
 > ```
 > On Windows:
 > ```shell
 > .venv\Scripts\activate.bat
 > ```
+Make sure you have the latest pip version
+```shell
+python -m pip install --upgrade pip
+```
 
 Then install the packages listed in the requirements.txt
 ```shell
 pip install -r requirements.txt
 ```
 
 Then install the repository locally
```

### Comparing `plottah-0.1.6/plottah/colors.py` & `plottah-0.1.7/plottah/colors.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.6/plottah/config.py` & `plottah-0.1.7/plottah/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,37 +50,53 @@
             values["n_bins"] = len(bins)
             print(f'setting n_bins for {values["name"]} to {len(bins)} based on bins')
         return bins
 
 
 class Settings(BaseModel):
     file_path: Path
-    output_path: Path
+    images_output_path: Path
+    powerpoint_output_path: Path
     features: list[FeatureSchema]
     target: str
     primary_color: str
     secondary_color: str
     tertiary_color: str
     grey_tint_color: str
 
-    @validator("file_path", "output_path", pre=True)
+    @validator("file_path", "images_output_path", pre=True)
     def path_must_exist(cls, v):
         """
         validates path specified in config. the path/file must exist before the code can execute the ensure valid reading and writing locations exist
         """
 
         if not isinstance(v, Path):
             v = Path(v)
 
         if not v.exists():
             raise ValueError(
                 f"Directory: {v} does not exist \n Please ensure the config.yaml contains a valid directory"
             )
         return v
 
+    @validator("powerpoint_output_path")
+    def parent_dir_must_exist(cls, v):
+        """
+        validates path specified in config. the path/file must exist before the code can execute the ensure valid reading and writing locations exist
+        """
+
+        if not isinstance(v, Path):
+            v = Path(v)
+
+        if not v.parent.exists():
+            raise ValueError(
+                f"Directory: {v.parent} does not exist \n Please ensure the config.yaml contains a valid directory"
+            )
+        return v
+
     @validator(
         "primary_color",
         "secondary_color",
         "tertiary_color",
         "grey_tint_color",
         pre=True,
     )
```

### Comparing `plottah-0.1.6/plottah/plot_builder/builders.py` & `plottah-0.1.7/plottah/plot_builder/builders.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from plottah.plot_handler import PlotHandler
 from plottah.colors import PlotColors
 from typing import Dict
 
 import pathlib
 import pandas as pd
+from pptx import Presentation
+from pptx.util import Inches, Pt
+
 
 from plottah.plots import DistPlot, RocCurvePlot, BinEventRatePlot
 
 
 def build_univariate_plot(
     df,
     feature_col: str,
@@ -81,14 +84,15 @@
 
     # create mapping from bins to none if not passed as argument
     if bins is None:
         bins = {feature: None for feature in features}
 
     # Run loop
     figs = {}
+    save_locs = []
     for i, feature in enumerate(features):
         print(f"[{i+1}/{len(features)}] Starting univariate analysis for: {feature}")
         if feature not in df.columns:
             raise ValueError(f"{feature} not in columns of dataframe")
 
         fig = build_univariate_plot(
             df=df,
@@ -99,13 +103,43 @@
             show_plot=show_plot,
             hoverinfo=hoverinfo,
             n_bins=n_bins[feature],
             bins=bins[feature],
         )
 
         if save_directory is not None:
-            fig.save_fig(save_directory)
+            save_loc = fig.save_fig(save_directory)
             print(f"[{i+1}/{len(features)}] Saving univariate anaylsis for {feature}")
+            save_locs.append(save_loc)
 
         figs[feature] = fig
 
-    return figs
+    return figs, save_locs
+
+
+def build_powerpoint(
+    fig_locs: list,
+    feature_names: list,
+    save_path: pathlib.Path(),
+):
+    pres = Presentation()
+
+    print(len(pres.slide_layouts))
+    for i, fig_loc in enumerate(fig_locs):
+        s_register = pres.slide_layouts[7]
+        s = pres.slides.add_slide(s_register)
+
+        pic = s.shapes.add_picture(
+            str(pathlib.Path(fig_loc).resolve()),
+            Inches(0.5),
+            Inches(1.75),
+            width=Inches(7),
+            height=Inches(5),
+        )
+        pic.left = int((pres.slide_width - pic.width) / 2)
+
+        title = s.shapes.title
+        title.text = f"{i} Univariate analysis for {(feature_names)[i]}"
+        title_para = s.shapes.title.text_frame.paragraphs[0]
+        title_para.font.size = Pt(24)
+
+    pres.save(save_path)
```

### Comparing `plottah-0.1.6/plottah/plot_handler/PlotHandler.py` & `plottah-0.1.7/plottah/plot_handler/PlotHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,12 +218,14 @@
         # make directory if not exists
         if not directory.exists():
             raise ValueError(f"directory: {directory} does not exist")
 
         # save the image in the directory
         self.fig.write_image(directory / f"univariate_plot_{self.feature_col}.jpeg")
 
+        return str(directory / f"univariate_plot_{self.feature_col}.jpeg")
+
     def get_fig(self):
         """
         Return figure object
         """
         return self.fig
```

### Comparing `plottah-0.1.6/plottah/plots/BinEventRatePlot.py` & `plottah-0.1.7/plottah/plots/BinEventRatePlot.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 import logging
 
 MIN_N_UNIQUE = 25
 
 
 @dataclass
 class CategoricalBinner:
+    """
+    seperated out binning to increase cohesion -> only responsible for
+        1. Adding bins to dataframe given as input
+        2. Returning labels based on bins
+
+    """
+
     _labels: list = field(default_factory=lambda: None)
 
     def get_labels(self):
         return self._labels.copy()
 
     def add_bins(self, df: pd.DataFrame, feature_col: str) -> pd.DataFrame:
         # Extract unique values
@@ -43,14 +50,21 @@
         self._labels[-1] = "NA"
 
         return df, self._labels
 
 
 @dataclass
 class StandardBinner:
+    """
+    seperated out binning to increase cohesion -> only responsible for
+        1. Adding bins to dataframe given as input
+        2. Returning labels based on bins
+
+    """
+
     _labels: list = field(default_factory=lambda: None)
 
     def get_labels(self):
         return self._labels.copy()
 
     def add_bins(
         self,
@@ -177,26 +191,31 @@
 
         # Calculate global event rate
         self.event_rate = np.mean(self.df[target_col])
 
         # Adjust n_bins if less unique values exist
         self.n_bins = self.n_bins if self.bins is None else len(self.bins)
         n_unique_feat_vals = df[feature_col].nunique()
+        if n_unique_feat_vals < self.n_bins:
+            logging.warning(
+                f"{self.feature_col} only has {n_unique_feat_vals} distinct values, decreasing n_bins from {self.n_bins} to {n_unique_feat_vals} "
+            )
         self.n_bins = np.minimum(n_unique_feat_vals, self.n_bins)
 
         # add bins column using strategy depending on feature type
         if self.feature_type == "categorical":
-            print("using categorical binner")
+            logging.info("using categorical binner")
             if self.df[self.feature_col].nunique() > self.n_bins:
                 raise ValueError(
                     f"Too many unique values for feature: {self.feature_col} ({self.df[self.feature_col].nunique()}) to only use {self.n_bins} bins. Increase n_bins to at least {self.df[self.feature_col].nunique()}!"
                 )
             binner = CategoricalBinner()
             self.df, self.labels = binner.add_bins(self.df, self.feature_col)
         else:
+            logging.info("using standard binner")
             if self.df[self.feature_col].nunique() < MIN_N_UNIQUE:
                 logging.warning(
                     f"{self.feature_col} only has {self.df[self.feature_col].nunique()} distinct values, consider switching feature type for {self.feature_col} to categorical (currenly {self.feature_type})"
                 )
             binner = StandardBinner()
             self.df, self.labels = binner.add_bins(
                 self.df, self.feature_col, self.n_bins, self.bins, method=method
```

### Comparing `plottah-0.1.6/plottah/plots/DistPlot.py` & `plottah-0.1.7/plottah/plots/DistPlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.6/plottah/plots/RocCurvePlot.py` & `plottah-0.1.7/plottah/plots/RocCurvePlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.6/plottah/utils.py` & `plottah-0.1.7/plottah/utils.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.6/PKG-INFO` & `plottah-0.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plottah
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Niels Ota
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,14 +13,15 @@
 Requires-Dist: numpy (>=1.20.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: plotly (>=5.15.0,<6.0.0)
 Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.9,<2.0.0)
 Requires-Dist: pylint (>=2.17.4,<3.0.0)
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
+Requires-Dist: python-pptx (>=0.6.21,<0.7.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 *Copyright © 2023 by Boston Consulting Group. All rights reserved*
@@ -30,14 +31,22 @@
 
 ### Requirements
 
 * Python (>=3.6)
 
 ### Development environment
 
+Clone the repo, give name plotting_analyis
+```shell
+git clone git@github.com:nielsota/plottah.git plotting_analysis
+```
+```shell
+cd plotting_analysis
+```
+
 Create a virtual environment by running:
 
 ```shell
 python -m venv .venv
 ```
 
 The virtual environment should be activated every time you start a new shell session before running subsequent commands:
@@ -46,14 +55,18 @@
 > ```shell
 > source .venv/bin/activate
 > ```
 > On Windows:
 > ```shell
 > .venv\Scripts\activate.bat
 > ```
+Make sure you have the latest pip version
+```shell
+python -m pip install --upgrade pip
+```
 
 Then install the packages listed in the requirements.txt
 ```shell
 pip install -r requirements.txt
 ```
 
 Then install the repository locally
```

