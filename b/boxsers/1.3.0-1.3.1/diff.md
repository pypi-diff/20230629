# Comparing `tmp/boxsers-1.3.0.tar.gz` & `tmp/boxsers-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxsers-1.3.0.tar", last modified: Fri Jun  2 18:23:38 2023, max compression
+gzip compressed data, was "boxsers-1.3.1.tar", last modified: Thu Jun 29 17:32:15 2023, max compression
```

## Comparing `boxsers-1.3.0.tar` & `boxsers-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 18:23:38.809660 boxsers-1.3.0/
--rw-rw-rw-   0        0        0     1093 2021-08-13 16:59:11.000000 boxsers-1.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     8765 2023-06-02 18:23:38.808670 boxsers-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    11114 2023-04-06 13:13:22.000000 boxsers-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 18:23:38.746309 boxsers-1.3.0/boxsers/
--rw-rw-rw-   0        0        0      673 2022-09-26 19:10:22.000000 boxsers-1.3.0/boxsers/__init__.py
--rw-rw-rw-   0        0        0      987 2022-07-15 15:44:15.000000 boxsers-1.3.0/boxsers/_boxsers_utils.py
--rw-rw-rw-   0        0        0    27447 2023-05-31 17:04:22.000000 boxsers-1.3.0/boxsers/data_augmentation.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:23:38.807652 boxsers-1.3.0/boxsers/machine_learning/
--rw-rw-rw-   0        0        0      380 2022-07-20 13:18:32.000000 boxsers-1.3.0/boxsers/machine_learning/__init__.py
--rw-rw-rw-   0        0        0    12773 2022-09-26 19:07:40.000000 boxsers-1.3.0/boxsers/machine_learning/classification.py
--rw-rw-rw-   0        0        0     7295 2022-07-13 19:35:31.000000 boxsers-1.3.0/boxsers/machine_learning/clustering.py
--rw-rw-rw-   0        0        0    24197 2023-04-06 13:16:16.000000 boxsers-1.3.0/boxsers/machine_learning/dimension_reduction.py
--rw-rw-rw-   0        0        0    35367 2023-04-04 19:42:12.000000 boxsers-1.3.0/boxsers/machine_learning/neural_networks.py
--rw-rw-rw-   0        0        0     7667 2022-07-20 19:26:31.000000 boxsers-1.3.0/boxsers/machine_learning/validation_metrics.py
--rw-rw-rw-   0        0        0     7755 2023-05-31 17:28:13.000000 boxsers-1.3.0/boxsers/misc_tools.py
--rw-rw-rw-   0        0        0    13083 2023-06-02 18:14:58.000000 boxsers-1.3.0/boxsers/preprocessing.py
--rw-rw-rw-   0        0        0    18237 2022-11-17 19:02:06.000000 boxsers-1.3.0/boxsers/visual_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:23:38.762330 boxsers-1.3.0/boxsers.egg-info/
--rw-rw-rw-   0        0        0     8765 2023-06-02 18:23:38.000000 boxsers-1.3.0/boxsers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-06-02 18:23:38.000000 boxsers-1.3.0/boxsers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 18:23:38.000000 boxsers-1.3.0/boxsers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-06-02 18:23:38.000000 boxsers-1.3.0/boxsers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 18:23:38.000000 boxsers-1.3.0/boxsers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 18:23:38.809660 boxsers-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-05-31 17:28:54.000000 boxsers-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:32:15.966259 boxsers-1.3.1/
+-rw-rw-rw-   0        0        0     1093 2021-08-13 16:59:11.000000 boxsers-1.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     8765 2023-06-29 17:32:15.965254 boxsers-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11132 2023-06-21 18:24:44.000000 boxsers-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 17:32:15.894865 boxsers-1.3.1/boxsers/
+-rw-rw-rw-   0        0        0      673 2022-09-26 19:10:22.000000 boxsers-1.3.1/boxsers/__init__.py
+-rw-rw-rw-   0        0        0      987 2022-07-15 15:44:15.000000 boxsers-1.3.1/boxsers/_boxsers_utils.py
+-rw-rw-rw-   0        0        0    27499 2023-06-29 17:16:00.000000 boxsers-1.3.1/boxsers/data_augmentation.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:32:15.964347 boxsers-1.3.1/boxsers/machine_learning/
+-rw-rw-rw-   0        0        0      380 2022-07-20 13:18:32.000000 boxsers-1.3.1/boxsers/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0    12773 2022-09-26 19:07:40.000000 boxsers-1.3.1/boxsers/machine_learning/classification.py
+-rw-rw-rw-   0        0        0     7295 2022-07-13 19:35:31.000000 boxsers-1.3.1/boxsers/machine_learning/clustering.py
+-rw-rw-rw-   0        0        0    24197 2023-04-06 13:16:16.000000 boxsers-1.3.1/boxsers/machine_learning/dimension_reduction.py
+-rw-rw-rw-   0        0        0    35367 2023-04-04 19:42:12.000000 boxsers-1.3.1/boxsers/machine_learning/neural_networks.py
+-rw-rw-rw-   0        0        0     7667 2022-07-20 19:26:31.000000 boxsers-1.3.1/boxsers/machine_learning/validation_metrics.py
+-rw-rw-rw-   0        0        0     7755 2023-05-31 17:28:13.000000 boxsers-1.3.1/boxsers/misc_tools.py
+-rw-rw-rw-   0        0        0    13083 2023-06-02 18:14:58.000000 boxsers-1.3.1/boxsers/preprocessing.py
+-rw-rw-rw-   0        0        0    18846 2023-06-29 17:19:18.000000 boxsers-1.3.1/boxsers/visual_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:32:15.917346 boxsers-1.3.1/boxsers.egg-info/
+-rw-rw-rw-   0        0        0     8765 2023-06-29 17:32:15.000000 boxsers-1.3.1/boxsers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2023-06-29 17:32:15.000000 boxsers-1.3.1/boxsers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 17:32:15.000000 boxsers-1.3.1/boxsers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-29 17:32:15.000000 boxsers-1.3.1/boxsers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-29 17:32:15.000000 boxsers-1.3.1/boxsers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 17:32:15.966259 boxsers-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-06-29 17:31:48.000000 boxsers-1.3.1/setup.py
```

### Comparing `boxsers-1.3.0/LICENSE.txt` & `boxsers-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `boxsers-1.3.0/PKG-INFO` & `boxsers-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsers
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python package that provides a full range of functionality to process and analyze vibrational spectra (Raman, SERS, FTIR, etc.).
 Home-page: https://github.com/ALebrun-108/BoxSERS
 Author: Alexis Lebrun
 Author-email: alexis.lebrun.1@ulaval.ca
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boxsers-1.3.0/README.md` & `boxsers-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 This module provides functions to preprocess vibrational spectra. These features
 improve spectrum quality and can improve performance for machine learning applications.
 
 * **als_baseline_cor** : Subtracts the baseline signal from the spectrum(s) using an
   Asymmetric Least Squares estimation.
 
 
-* **intensity_normalization** : Normalizes the spectrum(s) using one of the available norms in this function.
+* **spectral_normalization** : Normalizes the spectrum(s) using one of the available norms in this function.
 
 
 * **savgol_smoothing** : Smoothes the spectrum(s) using a Savitzky-Golay polynomial filter.
 
 
 * **cosmic_filter** : Applies a median filter to the spectrum(s) to remove cosmic rays.
 
@@ -186,29 +186,29 @@
 
 * **spline_interpolation** : Performs a one-dimensional interpolation spline on the spectra to reproduce
   them with a new x-axis.
 
 ```python
 # Code example:
 import numpy as np
-from boxsers.preprocessing import savgol_smoothing, als_baseline_cor, intensity_normalization
+from boxsers.preprocessing import savgol_smoothing, als_baseline_cor, spectral_normalization
 from boxsers.visual_tools import spectro_plot
 
 # Two spectrum are selected randomly 
 random_index = np.random.randint(0, sp.shape[0]-1, 2)
 sp_sample = sp[random_index]  # selected spectra
 label_a = label[random_index[0]]  # class corresponding to the first spectrum
 label_b = label[random_index[1]]  # class corresponding to the second spectrum
 
 # 1) Subtracts the baseline signal from the spectra
 sp_bc = als_baseline_cor(sp_sample, lam=1e4, p=0.001, niter=10, return_baseline=False)
 # 2) Smoothes the spectra
 sp_bc_svg = savgol_smoothing(sp_bc, window_length=15, p=3, degree=0)
 # 3) Normalizes the spectra 
-sp_bc_svg_norm = intensity_normalization(sp_bc_svg, norm='maxmin')
+sp_bc_svg_norm = spectral_normalization(sp_bc_svg, norm='minmax')
 
 # Graphs visualization : 
 legend=(label_a, label_b)
 spectro_plot(wn, sp_sample, title='Raw spectra', legend=legend')
 spectro_plot(wn, sp_bc_svg_norm[0], sp_bc_svg_norm[1], y_space=1, title='Preprocessed spectra', legend=legend)
 ```
 ![test image size](fig/preprocessing_plots.png)
@@ -251,15 +251,16 @@
 * **SpectroPCA** : Principal Component Analysis (PCA) model object.
 
 ```python
 pca_model = SpectroPCA(n_comp=10)
 pca_model.fit_model(sp)
 pca_model.scatter_plot(sp, label, component_x=1, component_y=2, fontsize=13, class_names=['Mol. A', 'Mol. B', 'Mol. C']) 
 ```
-![test image size](fig/PCA_scatterplot.png)
+<img src="fig/PCA_scatterplot.png" alt="drawing" width="500"/>
+
 ### Module ``clustering``
 This module provides unsupervised learning models for vibrational spectra cluster analysis.
 
 * **SpectroKmeans** : K-Means clustering model.
 
 
 * **SpectroGmixture** : Gaussian mixture probability distribution model.
```

### Comparing `boxsers-1.3.0/boxsers/__init__.py` & `boxsers-1.3.1/boxsers/__init__.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.3.0/boxsers/_boxsers_utils.py` & `boxsers-1.3.1/boxsers/_boxsers_utils.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.3.0/boxsers/data_augmentation.py` & `boxsers-1.3.1/boxsers/data_augmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     if return_infos:
         # returns the indexes for the spectra mixed together
         return sp_aug, lab_aug, random_indexes, lambda_values
 
     return sp_aug, lab_aug
 
 
-def aug_newband(sp, lab, inv_p=None, inv_p_degree=4, intensity_range=(0.05, 0.95), width_range=(2, 5),
+def aug_newband(sp, lab, inv_p=None, inv_p_degree=1, intensity_range=(0.05, 0.95), width_range=(2, 5),
                 quantity=1, shuffle_enabled=True, return_band=False):
     """
     Randomly generates new spectra with additionnal Gaussian peak added.
 
     Parameters:
         sp : array
             Input Spectrum(s), array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
@@ -182,18 +182,18 @@
         inv_p_degree : float, default=1
             Determines where additional Raman bands will be more likely positioned on the spectrum according
             to inv_p.
                 - > 0 : positioned at different locations than input spectrum bands.
                 - = 0 : randomly postioned.
                 - < 0 : positioned close to input spectrum bands.
 
-        intensity_range : float or integer, list or tuple, default = (0.02, 0.98)
+        intensity_range : float or integer, list or tuple, default = (0.05, 0.95)
             Values delimiting the range of possible values for the Raman band intensity..
 
-        width_range : list or tuple, default = (1, 5)
+        width_range : list or tuple, default = (2, 5)
             Values delimiting the range of possible values for the Raman band width (in pixels).
 
         quantity : integer, default=1
             Quantity of new spectra generated for one spectrum. If less than or equal to zero, no new
             spectrum is generated.
 
         shuffle_enabled : boolean, default=True
@@ -220,15 +220,15 @@
     sp_aug = np.empty((quantity * n_spectra, sp_len))
     added_bands = np.empty((quantity * n_spectra, sp_len))
     # as no changes are made to the labels, they are repeated to match the new spectra generated.
     lab_aug = np.repeat(lab, quantity, axis=0)
 
     if inv_p is None:
         # spectra values are used as the input for the inverse probability density
-        inv_p = sp
+        inv_p = np.abs(sp)  # np.abs() used to remove negatives values
     else:
         # inverse probability density function is given
         inv_p = np.array(inv_p, ndmin=2)
 
     # inverse density probabilities calculation
     inv_density = 1.0 / (inv_p ** inv_p_degree)
     # normalizing the probabilities to sum up to 1 for each row
```

### Comparing `boxsers-1.3.0/boxsers/machine_learning/classification.py` & `boxsers-1.3.1/boxsers/machine_learning/classification.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.3.0/boxsers/machine_learning/clustering.py` & `boxsers-1.3.1/boxsers/machine_learning/clustering.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.3.0/boxsers/machine_learning/dimension_reduction.py` & `boxsers-1.3.1/boxsers/machine_learning/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.3.0/boxsers/machine_learning/neural_networks.py` & `boxsers-1.3.1/boxsers/machine_learning/neural_networks.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.3.0/boxsers/machine_learning/validation_metrics.py` & `boxsers-1.3.1/boxsers/machine_learning/validation_metrics.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.3.0/boxsers/misc_tools.py` & `boxsers-1.3.1/boxsers/misc_tools.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.3.0/boxsers/preprocessing.py` & `boxsers-1.3.1/boxsers/preprocessing.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.3.0/boxsers/visual_tools.py` & `boxsers-1.3.1/boxsers/visual_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 This module provides different tools to visualize vibrational spectra quickly.
 """
 import matplotlib.pyplot as plt
 import numpy as np
 from boxsers._boxsers_utils import _lightdark_switch
 
 
-def random_plot(wn, sp, random_spectra, y_space=0, title=None, xlabel='Raman Shift (cm$^{-1}$)',
-                ylabel='Intensity (a.u.)', line_width=1.5, line_style='solid', darktheme=False,
-                grid=True, fontsize=10, fig_width=6.08, fig_height=3.8, save_path=None):
+def random_plot(wn, sp, random_spectra, y_space=0, xlim=None, ylim=None, title=None,
+                xlabel='Raman Shift (cm$^{-1}$)', ylabel='Intensity (a.u.)', line_width=1.5,
+                line_style='solid', darktheme=False, grid=True, fontsize=10, fig_width=6.08,
+                fig_height=3.8, save_path=None):
     """
     Plot a number of randomly selected spectra from a set of spectra.
 
     Parameters:
         wn : array
             X-axis(wavenumber, wavelenght, Raman shift, etc.), array shape = (n_pixels, ).
 
@@ -25,14 +26,20 @@
 
         random_spectra : integer
             Number of spectrum that are randomly selected from "sp" to be plotted.
 
         y_space : int or float, default=0
             Extra space on the y-axis between the spectra to allow a better visualization of the spectra.
 
+        xlim : list or tupple of float/int values, default=None
+            X-axis view limits.
+
+        ylim : list or tupple of float/int values, default=None
+            Y-axis view limits.
+
         title : string, default=None
             Font size(pts) used for the different elements of the graph. The title's font
             is two points larger than "fonctsize".
 
         xlabel : string, default='Raman Shift (cm$^{-1}$)'
             X-axis title. If None, there is no title displayed.
 
@@ -85,14 +92,18 @@
     y_space_sum = 0  # the y_space starts at zero
     for s in sp:
         # plots random spectra
         ax.plot(wn, s + y_space_sum, lw=line_width, ls=line_style)
         y_space_sum += y_space  # adds an offset for the next spectrum
     ax = plt.gca()  # get the current Axes instance
 
+    # axis view settings
+    ax.set_xlim(xlim)
+    ax.set_ylim(ylim)
+
     # titles settings
     ax.set_title(title, fontsize=fontsize+1.2, color=frame_color)  # sets the plot title, 1.2 points larger font size
     ax.set_xlabel(xlabel, fontsize=fontsize, color=frame_color)  # sets the X-axis label
     ax.set_ylabel(ylabel, fontsize=fontsize, color=frame_color)  # sets the Y-axis label
 
     # tick settings
     ax.minorticks_on()
@@ -116,31 +127,37 @@
     fig.tight_layout()
     # save figure
     if save_path is not None:
         plt.savefig(save_path, dpi=300, bbox_inches='tight')
     plt.show()
 
 
-def spectro_plot(wn, *sp, y_space=0, title=None, xlabel='Raman Shift (cm$^{-1}$)', ylabel='Intensity (a.u.)',
-                 legend=None, line_width=1.5, line_style='solid', color=None, darktheme=False, grid=True,
-                 fontsize=10, fig_width=6.08, fig_height=3.8, save_path=None):
+def spectro_plot(wn, *sp, y_space=0, xlim=None, ylim=None, title=None, xlabel='Raman Shift (cm$^{-1}$)',
+                 ylabel='Intensity (a.u.)', legend=None, line_width=1.5, line_style='solid', color=None,
+                 darktheme=False, grid=True, fontsize=10, fig_width=6.08, fig_height=3.8, save_path=None):
     """
     Returns a plot with the selected spectrum(s)
 
     Parameters:
         wn : array or list
             X-axis(wavenumber, wavelenght, Raman shift, etc.), array shape = (n_pixels, ).
 
         *sp : array
             Input Spectrum(s), array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
             for a single spectrum.
 
         y_space : int or float, default=0
             Extra space on the y-axis between the spectra to allow a better visualization of the spectra.
 
+        xlim : list or tupple of float/int values, default=None
+            X-axis view limits.
+
+        ylim : list or tupple of float/int values, default=None
+            Y-axis view limits.
+
         title : string, default=None
             Font size(pts) used for the different elements of the graph. The title's font
              is two points larger than "fonctsize".
 
         xlabel : string, default='Raman Shift (cm$^{-1}$)'
             X-axis title. If None, there is no title displayed.
 
@@ -190,14 +207,18 @@
         ax.set_prop_cycle(color=color)
     for s in sp:
         # plots all the input spectra
         ax.plot(wn, s.T + y_space_sum, lw=line_width, ls=line_style, label='a')
         y_space_sum += y_space  # adds an offset for the next spectrum
     ax = plt.gca()  # get the current Axes instance
 
+    # axis view settings
+    ax.set_xlim(xlim)
+    ax.set_ylim(ylim)
+
     # titles settings
     ax.set_title(title, fontsize=fontsize + 1.2, color=frame_color)  # sets the plot title, 1.2 points larger font size
     ax.set_xlabel(xlabel, fontsize=fontsize, color=frame_color)  # sets the X-axis label
     ax.set_ylabel(ylabel, fontsize=fontsize, color=frame_color)  # sets the Y-axis label
 
     # tick settings
     ax.minorticks_on()
```

### Comparing `boxsers-1.3.0/boxsers.egg-info/PKG-INFO` & `boxsers-1.3.1/boxsers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsers
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python package that provides a full range of functionality to process and analyze vibrational spectra (Raman, SERS, FTIR, etc.).
 Home-page: https://github.com/ALebrun-108/BoxSERS
 Author: Alexis Lebrun
 Author-email: alexis.lebrun.1@ulaval.ca
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boxsers-1.3.0/boxsers.egg-info/SOURCES.txt` & `boxsers-1.3.1/boxsers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boxsers-1.3.0/setup.py` & `boxsers-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     author='Alexis Lebrun',
     author_email='alexis.lebrun.1@ulaval.ca',
     # dependencies
     install_requires=['numpy', 'pandas', 'matplotlib', 'seaborn', 'scipy', 'scikit-learn', 'tensorflow',
                       'tables'],
     python_requires='>=3.6',
     # *strongly* suggested for sharing
-    version='1.3.0',
+    version='1.3.1',
     # The license can be anything you like
     license='MIT',
     description='Python package that provides a full range of functionality to process and analyze vibrational'
                 ' spectra (Raman, SERS, FTIR, etc.).',
     # We will also need a readme eventually (there will be a warning)
     long_description=open('README_pypi.md').read(),
     long_description_content_type="text/markdown",
```

