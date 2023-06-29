# Comparing `tmp/ackl-1.0.2.tar.gz` & `tmp/ackl-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ackl-1.0.2.tar", last modified: Wed Jan 18 12:10:12 2023, max compression
+gzip compressed data, was "ackl-1.0.6.tar", last modified: Thu Jun 29 08:04:07 2023, max compression
```

## Comparing `ackl-1.0.2.tar` & `ackl-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-18 12:10:12.264634 ackl-1.0.2/
--rw-rw-rw-   0        0        0     1087 2022-09-05 02:47:29.000000 ackl-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      640 2023-01-18 12:10:12.264634 ackl-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       49 2022-10-12 07:48:45.000000 ackl-1.0.2/README.md
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 ackl-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      863 2023-01-18 12:10:12.264634 ackl-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-18 12:10:12.233370 ackl-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-01-18 12:10:12.249003 ackl-1.0.2/src/ackl/
--rw-rw-rw-   0        0        0       75 2022-09-28 13:06:58.000000 ackl-1.0.2/src/ackl/__init__.py
--rw-rw-rw-   0        0        0    38827 2023-01-18 12:08:47.000000 ackl-1.0.2/src/ackl/kernels.py
--rw-rw-rw-   0        0        0    21391 2023-01-06 04:49:35.000000 ackl-1.0.2/src/ackl/metrics.py
-drwxrwxrwx   0        0        0        0 2023-01-18 12:10:12.249003 ackl-1.0.2/src/ackl.egg-info/
--rw-rw-rw-   0        0        0      640 2023-01-18 12:10:12.000000 ackl-1.0.2/src/ackl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-01-18 12:10:12.000000 ackl-1.0.2/src/ackl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-18 12:10:12.000000 ackl-1.0.2/src/ackl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-01-18 12:10:12.000000 ackl-1.0.2/src/ackl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-01-18 12:10:12.000000 ackl-1.0.2/src/ackl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 08:04:07.627028 ackl-1.0.6/
+-rw-rw-rw-   0        0        0     1087 2022-09-05 02:47:29.000000 ackl-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1679 2023-06-29 08:04:07.627028 ackl-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1088 2023-06-23 01:41:47.000000 ackl-1.0.6/README.md
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 ackl-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      900 2023-06-29 08:04:07.627028 ackl-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 08:04:07.330206 ackl-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 08:04:07.595767 ackl-1.0.6/src/ackl/
+-rw-rw-rw-   0        0        0       75 2022-09-28 13:06:58.000000 ackl-1.0.6/src/ackl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:04:07.627028 ackl-1.0.6/src/ackl/gui/
+-rw-rw-rw-   0        0        0        0 2023-01-31 05:39:02.000000 ackl-1.0.6/src/ackl/gui/__init__.py
+-rw-rw-rw-   0        0        0     2564 2023-03-31 07:47:59.000000 ackl-1.0.6/src/ackl/gui/run.py
+-rw-rw-rw-   0        0        0    38910 2023-06-29 04:12:06.000000 ackl-1.0.6/src/ackl/kernels.py
+-rw-rw-rw-   0        0        0    24988 2023-06-29 05:36:46.000000 ackl-1.0.6/src/ackl/metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:04:07.627028 ackl-1.0.6/src/ackl.egg-info/
+-rw-rw-rw-   0        0        0     1679 2023-06-29 08:04:07.000000 ackl-1.0.6/src/ackl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-06-29 08:04:07.000000 ackl-1.0.6/src/ackl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:04:07.000000 ackl-1.0.6/src/ackl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-06-29 08:04:07.000000 ackl-1.0.6/src/ackl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-29 08:04:07.000000 ackl-1.0.6/src/ackl.egg-info/top_level.txt
```

### Comparing `ackl-1.0.2/LICENSE` & `ackl-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ackl-1.0.2/setup.cfg` & `ackl-1.0.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 636b 6c0d 0a76 6572 7369 6f6e   = ackl..version
-00000020: 203d 2031 2e30 2e32 0d0a 6175 7468 6f72   = 1.0.2..author
+00000020: 203d 2031 2e30 2e36 0d0a 6175 7468 6f72   = 1.0.6..author
 00000030: 203d 2059 696e 7368 656e 6720 5a68 616e   = Yinsheng Zhan
 00000040: 6720 2850 682e 442e 290d 0a61 7574 686f  g (Ph.D.)..autho
 00000050: 725f 656d 6169 6c20 3d20 6f6f 407a 6a75  r_email = oo@zju
 00000060: 2e65 6475 2e63 6e0d 0a64 6573 6372 6970  .edu.cn..descrip
 00000070: 7469 6f6e 203d 2041 2050 7974 686f 6e20  tion = A Python 
 00000080: 6c69 6272 6172 7920 666f 7220 6b65 726e  library for kern
 00000090: 656c 7320 7573 6564 2069 6e20 616e 616c  els used in anal
@@ -39,16 +39,19 @@
 00000260: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
 00000270: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
 00000280: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
 00000290: 203e 3d33 2e36 0d0a 696e 7374 616c 6c5f   >=3.6..install_
 000002a0: 7265 7175 6972 6573 203d 200d 0a09 7363  requires = ...sc
 000002b0: 696b 6974 2d6c 6561 726e 0d0a 0973 6369  ikit-learn...sci
 000002c0: 7079 0d0a 096d 6174 706c 6f74 6c69 620d  py...matplotlib.
-000002d0: 0a09 6e75 6d70 790d 0a09 636c 610d 0a0d  ..numpy...cla...
-000002e0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000002f0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-00000300: 3d20 7372 630d 0a0d 0a5b 6f70 7469 6f6e  = src....[option
-00000310: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
-00000320: 0a2a 203d 202a 2e74 7874 2c20 2a2e 6373  .* = *.txt, *.cs
-00000330: 760d 0a0d 0a5b 6567 675f 696e 666f 5d0d  v....[egg_info].
-00000340: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000350: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+000002d0: 0a09 6e75 6d70 790d 0a09 636c 610d 0a09  ..numpy...cla...
+000002e0: 6f70 656e 6376 2d70 7974 686f 6e0d 0a09  opencv-python...
+000002f0: 7270 7932 0d0a 0966 6c61 736b 7765 6267  rpy2...flaskwebg
+00000300: 7569 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  ui....[options.p
+00000310: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+00000320: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
+00000330: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
+00000340: 6174 615d 0d0a 2a20 3d20 2a2e 7478 742c  ata]..* = *.txt,
+00000350: 202a 2e63 7376 0d0a 0d0a 5b65 6767 5f69   *.csv....[egg_i
+00000360: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000370: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000380: 0d0a 0d0a                                ....
```

### Comparing `ackl-1.0.2/src/ackl/kernels.py` & `ackl-1.0.6/src/ackl/kernels.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,25 +378,25 @@
     "linear": r"$k(x,y) = <x,y> $",
     "poly": r"$k(x,y)=(\alpha <x,y> + c)^d$",
     "gaussian": r"$k(x, y) = exp(-||x-y||^2/ (2 \sigma^2) )$",
     "sigmoid": r"$k(x, y) = tanh(\alpha <x, y> + c)$",
     "exp": r"$k(x, y)=exp(-||x - y||/(2 \sigma^2))$",
     "laplace": r"$k(x, y) = exp(-||x - y||/ \sigma)$",
     "cosine": r"$k(x, y) = <x,y>/(||x|| ||y||)$",
-    "wave": r"$k(x, y) = \frac{\sigma}{\lVert x-y \rVert } \sin \frac{\lVert x-y \rVert }{\sigma}$",
+    "wave": r"$k(x, y) = \frac{\sigma}{|x-y|} \sin \frac{|x-y|}{\sigma}$",
     "matern": r"$k(x, y) = (||x-y||^v \sqrt{2v} / s) * Bessel(||x-y||^v \sqrt{2v} / s) /(\Gamma(v) 2^{v-1} ) $",
     "rq": r"$k(x, y) = \left(1 + \frac{ {||x - y||} ^2 }{ 2\alpha  l^2}\right)^{-\alpha} $",
     "imq": r"$k(x, y) = 1 / \sqrt{||x-y||^2 + c^2}$",
     "cauchy": r"$k(x, y) = 1 / (1 + ||x - y||^2 / \sigma)$",
     "ts": r"$k(x, y) = 1 / (1 + ||x - y||^d)$",
     "anova": r"$k(x, y) = \sum_i exp( - \sigma * (x_i - y_i)^2 )^d$",
     "wavelet": r"$k(x, y) = \prod_i { h( (x_i-y_i)/a )}$",
     "fourier": r"$k(x, y) = \prod_i { (1-q^2)/(2(1-2q cos(||x - y||)+q^2)) }$",
-    "circular": r"$k(x, y) = \frac{2}{\pi} \arccos ( \frac{ \lVert x-y \rVert}{\sigma}) - \frac{2}{\pi} \frac{ \lVert x-y \rVert}{\sigma} \sqrt{1 - {\left( \frac{ \lVert x-y \rVert}{\sigma} \right)}^2 } , if \lVert x-y \rVert < \sigma$ , 0 otherwise.",
-    "spherical": r"$k(x, y) = 1 - \frac{3}{2} \frac{\lVert x-y \rVert}{\sigma} + \frac{1}{2} \left( \frac{ \lVert x-y \rVert}{\sigma} \right)^3$",
+    "circular": r"$k(x, y) = \frac{2}{\pi} \arccos ( \frac{ | x-y | }{\sigma}) - \frac{2}{\pi} \frac{ | x-y | }{\sigma} \sqrt{1 - {\left( \frac{ | x-y |}{\sigma} \right)}^2 } , if | x-y | < \sigma$ , 0 otherwise.",
+    "spherical": r"$k(x, y) = 1 - \frac{3}{2} \frac{| x-y |}{\sigma} + \frac{1}{2} \left( \frac{ | x-y |}{\sigma} \right)^3$",
     "tanimoto": r"$k(x, y) = <x, y> / (||x||^2 + ||y||^2 - <x, y>)$",
     "sorensen": r"$k(x, y) = 2 <x, y> / (||x||^2 + ||y||^2)$",
     "achi2": r"$k(x, y) = \sum_i { 2 x_i y_i / (x_i + y_i) }$",
     "chi2": r"$k(x, y) = \sum_i { (x_i - y_i)^2 / (x_i + y_i) } $",
     "min": r"$k(x, y) = \sum_i min(x_i, y_i)$",
     "ghi": r"$k(x, y) = \sum_i min(|x_i|^\alpha, |y_i|^\alpha)$",
     "minmax": r"$k(x, y) = \sum_i min(x_i, y_i) / \sum_i max(x_i, y_i)$",
@@ -411,31 +411,31 @@
 
 
 # Stores the hyper parameter search range for each kernel.
 # Some hparams are dynamic (based on data dim).
 # Not all kernels have tunable hyper-parameters.
 kernel_hparams = {
     "poly": [1, 2, 3, 4],  # when d = 1, becomes a linear kernel
-    "gaussian": [1, 3.33, 10, 60, 100, 300, 400],
-    "sigmoid": [0.1, 1, 10],
-    "laplace": [0.01, 0.1, 1, 10, 30, 50],
+    "gaussian": [0.1, 1, 3.33, 10, 60, 100, 300, 400],
+    "sigmoid": [0.01, 0.1, 1, 10],
+    "laplace": [0.001, 0.01, 0.1, 1, 10, 30, 50],
     # "exp": alias of laplace
-    "chi2":  [0.0001, 0.001, 0.01, 0.1, 1.0, 10, 100],
-    "anova": [0.00001, 0.001, 0.1, 1, 10, 1000, 100000],
-    "cauchy": [1, 10, 100, 1000, 10000],
-    "power": [.0001, .001, .01, .1, 0.25, .5, 1],
-    "matern": [0.1, 0.5, 1, 10],
-    "ess": [0.01, 0.1, 0.5, 1, 2, 10],
+    "chi2":  [0.00001, 0.0001, 0.001, 0.01, 0.1, 1.0, 10, 100],
+    "anova": [0.000001, 0.00001, 0.001, 0.1, 1, 10, 1000, 100000],
+    "cauchy": [0.01, 0.1, 1, 10, 100, 1000, 10000],
+    "power": [.00001, .0001, .001, .01, .1, 1],
+    "matern": [0.01, 0.1, 0.5, 1, 10],
+    "ess": [0.001, 0.01, 0.1, 0.5, 1, 2, 10],
     "fejer": [2, 3, 4, 5],
-    "circular": [0.01, 0.1, 1, 10, 1000, 10000],
-    "spherical": [.001, 0.1, 10, 1000, 10000],
-    "wave": [1, 2, 10, 100, 1000, 10000],
-    "fourier": [0.05, 0.1, 0.2, 0.4, 0.8, 2],
-    "rq": [0.5, 1, 2, 4, 16],
-    "imq": [0.5, 1, 2],
+    "circular": [0.001, 0.01, 0.1, 1, 10, 1000, 10000],
+    "spherical": [.0001, .001, 0.1, 10, 1000, 10000],
+    "wave": [0.1, 1, 2, 10, 100, 1000, 10000],
+    "fourier": [0.001, 0.01, 0.05, 0.1, 0.2, 0.4, 0.8, 2],
+    "rq": [0.1, 0.5, 1, 2, 4, 16],
+    "imq": [0.1, 0.5, 1, 2],
 }
 
 kernel_hparas_divide_n = ['gaussian', 'sigmoid', 'laplace']
 # these kernels' hparam should be divided by n
 
 kernel_names = list(kernel_dict.keys())
 
@@ -794,15 +794,18 @@
         return kernel
 
     def dim(self):
         return None
 
 
 def default_wavelet(x):
-    return np.cos(1.75*x)*np.exp(-x**2/2)
+    '''
+    Default wavelet is the morlet wavelet.
+    '''
+    return np.cos(5*x)*np.exp(-x**2/2) # 1.75
 
 
 class Wavelet(Kernel):
     """
     Wavelet kernel,
 
         k(x, y) = PROD_i h( (x_i-c)/a ) h( (y_i-c)/a )
```

### Comparing `ackl-1.0.2/src/ackl/metrics.py` & `ackl-1.0.6/src/ackl/metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,38 @@
+import os
+import sys
 import math
 import timeit
 import numpy as np
 import matplotlib.pyplot as plt
-# import full name to avoid conflict with those display params
-import IPython.core.display
+import IPython.display
 
-from sklearn.linear_model import LogisticRegressionCV
-from sklearn.preprocessing import MinMaxScaler
 from sklearn.decomposition import PCA
 from sklearn.cross_decomposition import PLSRegression
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
-from cla.metrics import get_metrics, metric_polarity_dict, es_max
-from .kernels import kernel_names, kernel_hparams, kernel_formulas, \
+from sklearn.linear_model import LogisticRegressionCV
+from sklearn.metrics import classification_report, confusion_matrix
+from sklearn.preprocessing import MinMaxScaler
+from sklearn.decomposition import PCA
+from cla.metrics import get_metrics, metric_polarity_dict, es_max, run_multiclass_clfs
+from cla.vis.plt2base64 import plt2html
+
+if __package__:
+    from .kernels import kernel_names, kernel_hparams, kernel_formulas, \
+    kernel_fullnames, kernel_dict, kernel_hparas_divide_n, \
+    cosine_kernel
+else:
+    ROOT_DIR = os.path.dirname(__file__)
+    if ROOT_DIR not in sys.path:
+        sys.path.append(ROOT_DIR)
+    from kernels import kernel_names, kernel_hparams, kernel_formulas, \
     kernel_fullnames, kernel_dict, kernel_hparas_divide_n, \
     cosine_kernel
 
-
-def acc(X, y, f):
+def acc(X, y, f, verbose = True):
     '''
     Use classification accuracy as a metric for kernel performance
 
     Parameters
     ----------
     X : expect an already-scaled data matrix
     y : target labels. support bianary classification.
@@ -28,22 +40,22 @@
         lambda x, y: laplacian_kernel(x, y, 2.0/N)
         lambda x, y: laplacian_kernel(x, y, 4.0/N)
     '''
     XK = f(X, X)  # convert mxn matrix to mxm matrix in the kernel space
     XK = np.nan_to_num(XK, copy=False, nan=0)  # replace NaN with 0
 
     try:
-        clf = LogisticRegressionCV().fit(XK, y)
+        clf = LogisticRegressionCV(max_iter=1000, multi_class='multinomial').fit(XK, y)
         return clf.score(XK, y)
     except Exception as e:
-        print(e)
+        if verbose:
+            print(e)
         return np.NaN
 
-
-def kes(X, y, f):
+def kes(X, y, f, verbose = True):
     '''
     kernel effect size
 
     Parameter
     ---------
     f - a kernel function. Can use lambda to pass concrete kernel-specific parameters, e.g., 
         lambda x, y: laplacian_kernel(x, y, 2.0/N)
@@ -55,30 +67,33 @@
     '''
     XK = f(X, X)  # kernel transform
     XK = np.nan_to_num(XK)
 
     try:
         lda = LinearDiscriminantAnalysis()
         X_dr = lda.fit_transform(XK, y)
-    except:    
-        print('Exception in LDA. Try PLS.')
+    except:
+        if verbose:
+            print('Exception in LDA. Try PLS.')
         try:
             pls = PLSRegression(n_components=len(XK), scale=False)
             X_dr = pls.fit(XK, y).transform(XK)
         except:
-            print('Exception in PLS. Use PCA instead.')
+            if verbose:
+                print('Exception in PLS. Use PCA instead.')
             try:
                 X_dr = PCA().fit_transform(XK)
             except:
                 X_dr = XK  # do without DR
 
     X_dr = np.nan_to_num(X_dr)
-    return es_max(X_dr, y)
+    return es_max(X_dr, y, verbose=verbose)
 
-def nmd(X, y, f, display=False):
+
+def nmd(X, y, f, display=False, verbose = True):
     '''
     Computes the normalized mean difference between the between-class and within-class matrices.
 
     Parameter
     ---------
     f - a kernel function. Can use lambda to pass concrete kernel-specific parameters, e.g., 
         lambda x, y: laplacian_kernel(x, y, 2.0/N)
@@ -86,15 +101,19 @@
 
     Return
     ------
     ratio
     '''
 
     labels = list(set(y))
-    assert len(labels) == 2
+    if len(labels) != 2:
+        if verbose:
+            print('NMD only supports binary classification. Return 0 by default.')
+        return 0
+    
     X1 = X[y == labels[0]]
     X2 = X[y == labels[1]]
 
     LT = np.nan_to_num(f(X1, X1))  # left-top
     RB = np.nan_to_num(f(X2, X2))  # right-bottom
     RT = np.nan_to_num(f(X1, X2))  # right-top
     LB = np.nan_to_num(f(X2, X1))  # left-bottom
@@ -174,20 +193,24 @@
     y = [0]*round(n/2) + [1]*(n-round(n/2))
 
     if dim == 2:
         zeros = np.array([0] * n).reshape(-1, 1)
         X = np.vstack((np.hstack((X, zeros)), np.hstack((zeros, X))))
         y = [0] * n + [1] * n
 
-    _ = preview_kernels(X, np.array(y), cmap, None,
-                        True, False, False, False, False)
+    _ = preview_kernels(X, np.array(y), cmap, hyper_param_optimizer = None,
+                        scale = True, calc_metrics = False,
+                        scatterplot = False, embed_title = False, verbose = False)
 
 
 def preview_kernels(X, y, cmap=None, hyper_param_optimizer=kes,
-                    scale=False, metrics=True, logplot=False, scatterplot=True, embed_title=True):
+                    scale=False, calc_metrics=True, logplot=False, 
+                    scatterplot=True, embed_title=True,
+                    output_html=False,
+                    selected_kernel_names=None, verbose = True):
     '''
     Try various kernel types to evaluate the pattern after kernel-ops.  
     Each kernel uses their own default/empirical paramters.    
     In binary classification, because the first and last half samples belong to two classes respectively. 
     We want to get a contrasive pattern, i.e., (LT、RB) and （LB、RT）have blocks of different colors. 
 
     Parameters
@@ -196,109 +219,140 @@
         Should be already rescaled to non-negative ranges (required by chi2 family) 
         and re-ordered by y. 
     y : class labels
     cmap : color map scheme to use. set None to use default, or set another scheme, e.g., 'gray', 'viridis', 'jet', 'rainbow', etc.
         For small dataset, we recommend 'gray'. For complex dataset, we recommend 'viridis'.
     hyper_param_optimizer : which optimizer to optimize the hyper parameters for each kernel. 
         For real-world dataset, use kes by default. For toy dataset, set None to disable optimizer.
+        For multi-class dataset (y has more than 5 classes), use acc.
     scale : whether do feature scaling
-    metrics : whether calculate clam metrics.
+    calc_metrics : whether calculate classifiability metrics.
     logplot : whether to output the log-scale plot in parallel.
-    scatterplot : whether to ouptut the scatter plots after PCA / PLS, to check classifiability.
+    scatterplot : whether to ouptut the kernel heatmaps and the scatter plots after PCA / PLS, to check classifiability.
         The PLS tries to maximize the covariance between X and Y.
     embed_title : whether embed the title in the plots. If not, will generate the title in HTML.
+    selected_kernel_names : a list of kernel names to be process. 
+        If None or 'all', will use all kernels.
     '''
 
     all_dic_metrics = {}
+    html_str = ''
 
     if scale:
         X = MinMaxScaler().fit_transform(X)
 
+    if calc_metrics:
+        result_html = '<h3>0. no kernel</h3><p>Classification on original dataset</p>'
+        result_html += run_multiclass_clfs(X, y, show = False)
+        if output_html:
+            html_str += result_html
+        else:
+            IPython.display.display(IPython.display.HTML(result_html))
+
     # to be safe, perform a re-order
     if (y is not None and len(set(y)) == 2):
         labels = list(set(y))  # re-order X by y
         X = np.vstack((X[y == labels[0]], X[y == labels[1]]))
         y = [labels[0]] * np.sum(y == labels[0]) + \
             [labels[1]] * np.sum(y == labels[1])
 
-    for i, key in enumerate(kernel_names):
+    if selected_kernel_names is None or selected_kernel_names == 'all':
+        selected_kernel_names = kernel_names
+
+    for i, key in enumerate(selected_kernel_names):
         best_hparam = None
         best_metric = -np.inf
         title = str(i+1) + '. ' + \
             (kernel_fullnames[key] if key in kernel_fullnames else key)
 
         if hyper_param_optimizer is not None and key in kernel_hparams:
             for param in kernel_hparams[key]:
                 if key in kernel_hparas_divide_n:
                     param = param/X.shape[1]  # divide hparam by data dim
                 new_metric = hyper_param_optimizer(
-                    X, y, lambda x, y: kernel_dict[key](x, y, param))
+                    X, y, lambda x, y: kernel_dict[key](x, y, param), verbose = verbose)
                 if (new_metric > best_metric):
                     best_metric = new_metric
                     best_hparam = param
             title = str(i+1) + '. ' + (kernel_fullnames[key] if key in kernel_fullnames else key) \
                 + ('(' + format(best_hparam, '.2g') +
                    ')') if best_hparam is not None else ''
 
         if hyper_param_optimizer is None or key not in kernel_hparams:
             kns = kernel_dict[key](X, X)
-            metric_nmd = nmd(X, y, lambda x, y: kernel_dict[key](x, y))
+            # metric_nmd = nmd(X, y, lambda x, y: kernel_dict[key](x, y), verbose = verbose)
         else:
             kns = kernel_dict[key](X, X, best_hparam)
-            metric_nmd = nmd(X, y, lambda x, y: kernel_dict[key](x, y, param))
-
-        ######## plot after kernel transforms ########
-        _, ax = plt.subplots(1, 2, figsize=(12, 6))
-        ax[0].imshow(kns, cmap=cmap)
-        ax[0].set_axis_off()
-        if logplot:
-            ax[1].imshow(1+np.log(kns), cmap=cmap)
-            ax[1].set_axis_off()
+            # metric_nmd = nmd(X, y, lambda x, y: kernel_dict[key](x, y, param), verbose = verbose)
 
-        plt.axis('off')
-        if embed_title:
-            plt.title(title + '\n' +
-                      kernel_formulas[key] + '\n' + "NMD = %.3g" % metric_nmd)
-        else:
-            # print(title)
-            IPython.display.display(IPython.display.HTML('<h3>' + title + '</h3>' + '<p>' + kernel_formulas[key].replace('<', '&lt;')
-                                                         .replace('>', '&gt;') + '</p><p>' + "NMD = %.3g" % metric_nmd + '</p>'))
-        plt.show()
+        kns = np.nan_to_num(kns)
 
-        if scatterplot:
+        ######## plot after kernel transforms ########
+        
+        if scatterplot or output_html:
+            _, ax = plt.subplots(1, 2, figsize=(round(len(set(y))/2.0) + 6, round(len(set(y))/4.0) + 3)) # figsize = (round(len(labels)/4.0) + 4, round(len(labels)/4.0) + 3)
+            ax[0].imshow(kns, cmap=cmap)
+            ax[0].set_axis_off()
+            if logplot:
+                ax[1].imshow(1+np.log(kns), cmap=cmap)
+                ax[1].set_axis_off()
+
+            plt.axis('off')
+            if embed_title:
+                plt.title(title + '\n' + kernel_formulas[key] + '\n') # + "NMD = %.3g" % metric_nmd)
+            else:
+                # print(title)
+                IPython.display.display(IPython.display.HTML('<h3>' + title + '</h3>' + '<p>' + kernel_formulas[key].replace('<', '&lt;')
+                                                            .replace('>', '&gt;') + '</p>')) # <p>' + "NMD = %.3g" % metric_nmd + '</p>'
+            if output_html:
+                html_str += plt2html(plt)
+                plt.close()
+            else:
+                plt.show()
 
-            ######## scatter plot after PCA ########
-            kns = np.nan_to_num(kns)
+            ######## scatter plot after PCA ########            
             pca = PCA(n_components=2)  # keep the first 2 components
             X_pca = pca.fit_transform(kns)
             X_pca = np.nan_to_num(X_pca)
             plot_components_2d(X_pca, y)
             plt.title('PCA')
-            plt.show()
+
+            if output_html:
+                html_str += plt2html(plt)
+                plt.close()
+            else:
+                plt.show()
 
             ######## scatter plot after LDA ########
 
             try:
-                kns = np.nan_to_num(kns)
                 lda = LinearDiscriminantAnalysis()
                 X_lda = lda.fit(kns, y).transform(kns)
                 X_lda = np.nan_to_num(X_lda)
 
                 lda.score(kns, y)
                 if (X_lda.shape[1] == 1):
                     X_lda = np.hstack((X_lda, np.zeros((X_lda.shape[0], 1))))
                 plot_components_2d(X_lda, y)
                 # the coefficient of determination or R squared method is the proportion of the variance in the dependent variable that is predicted from the independent variable.
                 plt.title(
                     'LDA (ACC = ' + str(np.round(lda.score(kns, y), 3)) + ')')
-                plt.show()
+                
+                if output_html:
+                    html_str += plt2html(plt)
+                    plt.close()
+                else:
+                    plt.show()
+
             except Exception as e:
-                print('Exception : ', e)
+                if verbose:
+                    print('Exception : ', e)
                 # print('X_pls = ', X_pls)
                 # plt.title('PLS')
+                html_str += '<p>' + str(e) + '</p>'
 
             ######## scatter plot after PLS ########
 
             try:
                 ''' # using CV
                 kns = np.nan_to_num(kns)
                 pls = PLSRegression(n_components=2, scale=False)
@@ -323,54 +377,69 @@
                 X_pls = np.nan_to_num(X_pls)
 
                 pls.score(kns, y)
                 plot_components_2d(X_pls, y)
                 # the coefficient of determination or R squared method is the proportion of the variance in the dependent variable that is predicted from the independent variable.
                 plt.title(
                     'PLS (R2 = ' + str(np.round(pls.score(kns, y), 3)) + ')')
-                plt.show()
+                if output_html:
+                    html_str += plt2html(plt)
+                    plt.close()
+                else:
+                    plt.show()
             except Exception as e:
-                print('Exception : ', e)
+                if verbose:
+                    print('Exception : ', e)
                 # print('X_pls = ', X_pls)
                 # plt.title('PLS')
+                html_str += '<p>' + str(e) + '</p>'
+
+        ###### Classifiction after kernel transformation #######
+        if calc_metrics:
+            # result_html = '<h3>classification</h3>'
+            result_html = run_multiclass_clfs(kns, y, show = False)
+            if output_html:
+                html_str += result_html
+            else:
+                IPython.display.display(IPython.display.HTML(result_html))
 
-        ###### metrics ######
-        if metrics:
+        ###### cla metrics ######
+        if calc_metrics:
             kns = np.nan_to_num(np.hstack((kns, np.array(y).reshape(-1, 1))),   # do nan filtering simultaneously for X and y
                                 nan=0, posinf=kns.max(), neginf=kns.min())
-            _, dic_metrics = get_metrics(kns[:, :-1], kns[:, -1].flatten())
-            dic_metrics['NMD'] = metric_nmd
+            _, dic_metrics = get_metrics(kns[:, :-1], kns[:, -1].flatten(), verbose = False)
+            # dic_metrics['NMD'] = metric_nmd
             all_dic_metrics[key] = dic_metrics
 
-    return all_dic_metrics
+    return all_dic_metrics, html_str
 
 
 def visualize_metric_dicts(dics, plot=True):
     '''
     Example
     -------
     dics = preview_kernels(X, y)
     html_str = generate_html_from_dicts(dics)
     display(HTML(html_str)) # use in jupyter notebook
     '''
 
     row_names = []
     column_names = []
 
-    html_str = '<table><tr><th></th>'
+    html_str = '<table><tr><th>metric</th>'
 
     # use the 1st loop to get row and col names
     for kernel in dics:
         column_names.append(kernel)
-        html_str += '<th>' + kernel + '</th>'
+        html_str += '<th>' + str(kernel) + '</th>'
         for key in dics[kernel]:
             if key not in row_names:
                 row_names.append(key)
 
-    html_str += '<th>best kernel(s)</th>'
+    html_str += '<th>best</th><th>chart</th>'
     html_str += '</tr>'
 
     # use the 2nd loop to fill in data
     for row in row_names:
         if row not in metric_polarity_dict:
             continue
 
@@ -397,29 +466,35 @@
             best_metric_idxs = np.where(metrics == best_metric_value)
         except Exception as e:
             print(e)  # All-NaN slice encountered
             best_metric_idxs = []
 
         best_kernel_names = str(np.array(column_names)[best_metric_idxs])
         html_str += '<td>' + best_kernel_names + '</td>'
-        html_str += '</tr>'
+        
+        if len(column_names) > 1: # only need to draw bar chart when more than two kernels are compared
 
-        if plot:
-            plt.figure(figsize=(20, 3))            
+            plt.figure(figsize=(20, 3))
             plt.bar(column_names, metrics, alpha=0.7,
-                    width=0.6, edgecolor='black', color='white', label = row)
+                    width=0.6, edgecolor='black', color='white', label=row)
             plt.bar(np.array(column_names)[best_metric_idxs], metrics[best_metric_idxs], alpha=0.7,
                     width=0.6, edgecolor='black', color='gold',
-                    label = "best kernels: " + best_kernel_names)
+                    label="best kernels: " + best_kernel_names)
             plt.xticks(rotation=40)
+            plt.title(row + "\nbest kernels: " + best_kernel_names +
+                    "\nbest value: " + str(best_metric_value))
             plt.legend()
-            plt.show()
 
-            print(row + "\nbest kernels: " + best_kernel_names +
-            "\nbest value: " + str(best_metric_value))
+            if plot:
+                plt.show()
+            else:
+                html_str += '<td style="min-width:400px">' + plt2html(plt) + '</td>'
+                plt.close()
+
+        html_str += '</tr>'
 
     html_str += '</table>'
     # display(HTML( html_str ))
 
     return html_str
 
 
@@ -513,42 +588,49 @@
         plt.legend()
         # plt.bar(x, y)
         plt.xticks(rotation=45)
         plt.ylabel('second')
         plt.show()
 
     dct_mu = {}
-    for k,v in zip(x, y.mean(axis = 1)):
+    for k, v in zip(x, y.mean(axis=1)):
         dct_mu[k] = v
 
     return dct_mu
 
-def plot_components_2d(X, y, labels=None, use_markers=False, ax=None, legends=None, tags=None):
+
+def plot_components_2d(X, y, labels=None, use_markers=False, legends=None, tags=None):
     '''
     Copied from qsi.vis.plot_components_2d, to avoid package dependency.
     '''
     if X.shape[1] < 2:
         print(
             'ERROR: X MUST HAVE AT LEAST 2 FEATURES/COLUMNS! SKIPPING plot_components_2d().')
         return
 
-    # Gray shades can be given as a string encoding a float in the 0-1 range
-    colors = ['0.9', '0.1', 'red', 'blue', 'black',
-              'orange', 'green', 'cyan', 'purple', 'gray']
-    markers = ['o', 's', '^', 'D', 'H', 'o', 's', '^', 'D',
-               'H', 'o', 's', '^', 'D', 'H', 'o', 's', '^', 'D', 'H']
-
-    if ax is None:
-        _, ax = plt.subplots()
-
     if y is None or len(y) == 0:
         labels = [0]  # only one class
     if labels is None:
         labels = set(y)
 
+    _, ax = plt.subplots(figsize = (round(len(labels)/4.0) + 4, round(len(labels)/4.0) + 3))
+
+    # Gray shades can be given as a string encoding a float in the 0-1 range
+    colors = ['0.9', '0.1', 'red', 'blue', 'green',
+              'orange', 'cyan', 'purple', 'gray']
+    if len(labels) > len(colors):
+        for i in range(len(labels) - len(colors) + 5):
+            colors.append('C' + str(i))
+
+    markers = ['o', 's', '^', 'D', 'H', 'o', 's', '^', 'D',
+               'H', 'o', 's', '^', 'D', 'H', 'o', 's', '^', 'D', 'H']
+    if len(labels) > len(markers):
+        for i in range(len(labels) - len(markers) + 5):
+            markers.append(np.random.choice(markers))
+
     i = 0
 
     for label in labels:
         if y is None or len(y) == 0:
             cluster = X
         else:
             cluster = X[np.where(y == label)]
```

