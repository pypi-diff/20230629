# Comparing `tmp/py-np4vtt-1.0.5.tar.gz` & `tmp/py-np4vtt-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-np4vtt-1.0.5.tar", max compression
+gzip compressed data, was "py-np4vtt-1.0.6.tar", max compression
```

## Comparing `py-np4vtt-1.0.5.tar` & `py-np4vtt-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3162 2023-05-15 18:15:40.174563 py-np4vtt-1.0.5/README.md
--rw-r--r--   0        0        0      705 2023-05-17 06:21:35.582999 py-np4vtt-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1168 2023-05-15 18:15:40.190980 py-np4vtt-1.0.5/src/py_np4vtt/__init__.py
--rw-r--r--   0        0        0     3579 2023-05-15 18:28:22.310516 py-np4vtt-1.0.5/src/py_np4vtt/data_format.py
--rw-r--r--   0        0        0     7968 2023-05-15 18:28:22.311128 py-np4vtt-1.0.5/src/py_np4vtt/data_import.py
--rw-r--r--   0        0        0    10354 2023-05-15 18:15:40.191804 py-np4vtt-1.0.5/src/py_np4vtt/model_ann.py
--rw-r--r--   0        0        0     6590 2023-05-15 18:15:40.192356 py-np4vtt-1.0.5/src/py_np4vtt/model_lconstant.py
--rw-r--r--   0        0        0     6952 2023-05-15 18:15:40.192592 py-np4vtt-1.0.5/src/py_np4vtt/model_loclogit.py
--rw-r--r--   0        0        0     6819 2023-05-15 18:15:40.192800 py-np4vtt-1.0.5/src/py_np4vtt/model_logistic.py
--rw-r--r--   0        0        0     9175 2023-05-15 18:15:40.192984 py-np4vtt-1.0.5/src/py_np4vtt/model_rouwendal.py
--rw-r--r--   0        0        0     5385 2023-05-15 18:15:40.193225 py-np4vtt-1.0.5/src/py_np4vtt/model_rv.py
--rw-r--r--   0        0        0     4909 2023-05-15 18:15:40.193377 py-np4vtt-1.0.5/src/py_np4vtt/plots.py
--rw-r--r--   0        0        0     8211 2023-05-15 18:15:40.193577 py-np4vtt-1.0.5/src/py_np4vtt/utils.py
--rw-r--r--   0        0        0     4103 2023-05-17 06:21:50.096403 py-np4vtt-1.0.5/setup.py
--rw-r--r--   0        0        0     3981 2023-05-17 06:21:50.096883 py-np4vtt-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3118 2023-05-31 08:48:35.140975 py-np4vtt-1.0.6/README.md
+-rw-r--r--   0        0        0      704 2023-06-29 09:55:49.938857 py-np4vtt-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1168 2023-05-15 18:15:40.190980 py-np4vtt-1.0.6/src/py_np4vtt/__init__.py
+-rw-r--r--   0        0        0     3579 2023-05-15 18:28:22.310516 py-np4vtt-1.0.6/src/py_np4vtt/data_format.py
+-rw-r--r--   0        0        0     7968 2023-05-15 18:28:22.311128 py-np4vtt-1.0.6/src/py_np4vtt/data_import.py
+-rw-r--r--   0        0        0    10354 2023-05-22 23:30:16.755935 py-np4vtt-1.0.6/src/py_np4vtt/model_ann.py
+-rw-r--r--   0        0        0     6590 2023-05-15 18:15:40.192356 py-np4vtt-1.0.6/src/py_np4vtt/model_lconstant.py
+-rw-r--r--   0        0        0     6952 2023-05-15 18:15:40.192592 py-np4vtt-1.0.6/src/py_np4vtt/model_loclogit.py
+-rw-r--r--   0        0        0     6819 2023-05-15 18:15:40.192800 py-np4vtt-1.0.6/src/py_np4vtt/model_logistic.py
+-rw-r--r--   0        0        0     9183 2023-05-31 08:30:28.806935 py-np4vtt-1.0.6/src/py_np4vtt/model_rouwendal.py
+-rw-r--r--   0        0        0     5399 2023-05-23 11:00:07.003580 py-np4vtt-1.0.6/src/py_np4vtt/model_rv.py
+-rw-r--r--   0        0        0     4909 2023-05-15 18:15:40.193377 py-np4vtt-1.0.6/src/py_np4vtt/plots.py
+-rw-r--r--   0        0        0     8211 2023-05-15 18:15:40.193577 py-np4vtt-1.0.6/src/py_np4vtt/utils.py
+-rw-r--r--   0        0        0     4059 2023-06-29 09:56:10.352601 py-np4vtt-1.0.6/setup.py
+-rw-r--r--   0        0        0     3937 2023-06-29 09:56:10.352934 py-np4vtt-1.0.6/PKG-INFO
```

### Comparing `py-np4vtt-1.0.5/README.md` & `py-np4vtt-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
    * ANN-based VTT model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/ann.ipynb)
    * Logistic Regression-based VTT model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/logistic.ipynb)
 
 These examples guide the user through the process of loading a dataset, estimating a nonparametric model, and visualising the VTT distribution using scatter and histogram plots. We use the Norwegian 2009 VTT data to illustrate each example.
 
 **Take, for example, the VTT distribution from the Rouwendal model using NP4VTT:**
 
-![VTT distribution from the Rouwendal model using NP4VTT](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/raw/master/examples/outcomes/rouwendal.png)
+![VTT distribution from the Rouwendal model using NP4VTT](examples/norway_data/outcomes/rouwendal.png)
 
 ## References
 
    * Fosgerau, M. (2006). Investigating the distribution of the value of travel time savings. Transportation Research Part B: Methodological, 40(8), 688–707. https://doi.org/10.1016/j.trb.2005.09.007
    * Fosgerau, M. (2007). Using nonparametrics to specify a model to measure the value of travel time. Transportation Research Part A: Policy and Practice, 41(9), 842–856. https://doi.org/10.1016/j.tra.2006.10.004
    * Rouwendal, J., de Blaeij, A., Rietveld, P., & Verhoef, E. (2010). The information content of a stated choice experiment: A new method and its application to the value of a statistical life. Transportation Research Part B: Methodological, 44(1), 136–151. https://doi.org/10.1016/j.trb.2009.04.006
    * Ojeda-Cabral, M., Batley, R., & Hess, S. (2016). The value of travel time: Random utility versus random valuation. Transportmetrica A: Transport Science, 12(3), 230–248. https://doi.org/10.1080/23249935.2015.1125398
```

### Comparing `py-np4vtt-1.0.5/pyproject.toml` & `py-np4vtt-1.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-np4vtt"
-version = "1.0.5"
+version = "1.0.6"
 description = "Python library providing NonParametric models for Value of Travel Time analysis"
 authors = ["José Ignacio Hernández <J.I.Hernandez@tudelft.nl>", "João Paulo Pizani Flor <paulopizani@posteo.net>"]
 
 homepage = "https://gitlab.tudelft.nl/np4vtt/py-np4vtt"
 repository = "https://gitlab.tudelft.nl/np4vtt/py-np4vtt"
 readme = "README.md"
 
@@ -17,8 +17,8 @@
 numdifftools = "^0.9.40"
 
 [tool.poetry.dev-dependencies]
 ipykernel = "^6.15.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `py-np4vtt-1.0.5/src/py_np4vtt/__init__.py` & `py-np4vtt-1.0.6/src/py_np4vtt/__init__.py`

 * *Files identical despite different names*

### Comparing `py-np4vtt-1.0.5/src/py_np4vtt/data_format.py` & `py-np4vtt-1.0.6/src/py_np4vtt/data_format.py`

 * *Files identical despite different names*

### Comparing `py-np4vtt-1.0.5/src/py_np4vtt/data_import.py` & `py-np4vtt-1.0.6/src/py_np4vtt/data_import.py`

 * *Files identical despite different names*

### Comparing `py-np4vtt-1.0.5/src/py_np4vtt/model_ann.py` & `py-np4vtt-1.0.6/src/py_np4vtt/model_ann.py`

 * *Files identical despite different names*

### Comparing `py-np4vtt-1.0.5/src/py_np4vtt/model_lconstant.py` & `py-np4vtt-1.0.6/src/py_np4vtt/model_lconstant.py`

 * *Files identical despite different names*

### Comparing `py-np4vtt-1.0.5/src/py_np4vtt/model_loclogit.py` & `py-np4vtt-1.0.6/src/py_np4vtt/model_loclogit.py`

 * *Files identical despite different names*

### Comparing `py-np4vtt-1.0.5/src/py_np4vtt/model_logistic.py` & `py-np4vtt-1.0.6/src/py_np4vtt/model_logistic.py`

 * *Files identical despite different names*

### Comparing `py-np4vtt-1.0.5/src/py_np4vtt/model_rouwendal.py` & `py-np4vtt-1.0.6/src/py_np4vtt/model_rouwendal.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,25 +171,25 @@
         # Starting values
         argTuple = (self.arrays.NP, self.arrays.T, BVTT_array, Choice_array, self.vtt_grid)
 
         # Start optimization
         t0 = time.time()
         results = _bfgsmin(ModelRouwendal.objectiveFunction, x0, args=argTuple,tol=1e-6,verbose=True)
 
-        # Compute elapsed time
-        t1 = time.time()
-        est_time = t1 - t0
-
         # Collect results
         x = results['x']
         hess = Hessian(ModelRouwendal.objectiveFunction,method='forward')(x,self.arrays.NP, self.arrays.T, BVTT_array, Choice_array, self.vtt_grid)
         se = np.sqrt(np.diag(np.linalg.inv(hess)))
         ll = -results['fun']
         exitflag = results['convergence']
 
+        # Compute elapsed time
+        t1 = time.time()
+        est_time = t1 - t0
+        
         # Get estimated probability of consistent choice
         q_prob = np.exp(x[0])/(1+np.exp(x[0]))
         q_est = x[0]
         q_se = np.sqrt((np.exp(q_est)/(1+np.exp(q_est)))**2)**2 * se[0]**2
 
         # Get estimated FVTT and xameters
         x = x[1:]
```

### Comparing `py-np4vtt-1.0.5/src/py_np4vtt/model_rv.py` & `py-np4vtt-1.0.6/src/py_np4vtt/model_rv.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,16 @@
         scale, VTT = x
 
         # Create value functions
         V1 = scale * BVTT
         V2 = scale * VTT
 
         dV = V2 - V1
-        dV[dV>700] = 700
+        # dV[dV>700] = 700
 
         # Create choice probability and Log-likelihood
         p = 1 / (1 + np.exp(-dV))
-        ll = - np.sum(np.log(p * (y_regress == 1) + (1 - p) * (y_regress == 0)))
+        ll_n = (1-y_regress) * np.log(1-p) + y_regress*np.log(p)
+        ll = - np.sum(ll_n)
 
         # Return choice probability
         return ll
```

### Comparing `py-np4vtt-1.0.5/src/py_np4vtt/plots.py` & `py-np4vtt-1.0.6/src/py_np4vtt/plots.py`

 * *Files identical despite different names*

### Comparing `py-np4vtt-1.0.5/src/py_np4vtt/utils.py` & `py-np4vtt-1.0.6/src/py_np4vtt/utils.py`

 * *Files identical despite different names*

### Comparing `py-np4vtt-1.0.5/setup.py` & `py-np4vtt-1.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'numdifftools>=0.9.40,<0.10.0',
  'pandas>=1.3.1,<2.0.0',
  'scikit-learn>=1.0.2,<2.0.0',
  'scipy>=1.7.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'py-np4vtt',
-    'version': '1.0.5',
+    'version': '1.0.6',
     'description': 'Python library providing NonParametric models for Value of Travel Time analysis',
-    'long_description': '# NP4VTT\n\nNP4VTT is a Python package that enables researchers to estimate and compare nonparametric models in a fast and convenient way. It comprises five nonparametric models for estimating the VTT distribution from data coming from two-attribute-two-alternative stated choice experiments:\n\n   * Local constant model  (Fosgerau, 2006, 2007)\n   * Local logit (Fosgerau, 2007)\n   * Rouwendal model (Rouwendal et al., 2010)\n   * Artificial Neural Network (ANN) based VTT model (van Cranenburgh & Kouwenhoven, 2021)\n   * Logistic Regression based VTT model (van Cranenburgh & Kouwenhoven, 2021)\n\nAdditionally, a Random Valuation model (Ojeda-Cabral, 2006) is included for benchmarking purposes\n\n## Installation steps\n\n* Use `pip` to install the `py-np4vtt` library normally:\n    - `python3 -m pip install py-np4vtt`\n\n\n## Examples\n\nWe provide Jupyter Notebooks that show how to configure and estimate each model included in NP4VTT:\n\n   * Local constant model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/lconstant.ipynb)\n   * Local logit: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/loclogit.ipynb)\n   * Rouwendal model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/rouwendal.ipynb)\n   * ANN-based VTT model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/ann.ipynb)\n   * Logistic Regression-based VTT model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/logistic.ipynb)\n\nThese examples guide the user through the process of loading a dataset, estimating a nonparametric model, and visualising the VTT distribution using scatter and histogram plots. We use the Norwegian 2009 VTT data to illustrate each example.\n\n**Take, for example, the VTT distribution from the Rouwendal model using NP4VTT:**\n\n![VTT distribution from the Rouwendal model using NP4VTT](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/raw/master/examples/outcomes/rouwendal.png)\n\n## References\n\n   * Fosgerau, M. (2006). Investigating the distribution of the value of travel time savings. Transportation Research Part B: Methodological, 40(8), 688–707. https://doi.org/10.1016/j.trb.2005.09.007\n   * Fosgerau, M. (2007). Using nonparametrics to specify a model to measure the value of travel time. Transportation Research Part A: Policy and Practice, 41(9), 842–856. https://doi.org/10.1016/j.tra.2006.10.004\n   * Rouwendal, J., de Blaeij, A., Rietveld, P., & Verhoef, E. (2010). The information content of a stated choice experiment: A new method and its application to the value of a statistical life. Transportation Research Part B: Methodological, 44(1), 136–151. https://doi.org/10.1016/j.trb.2009.04.006\n   * Ojeda-Cabral, M., Batley, R., & Hess, S. (2016). The value of travel time: Random utility versus random valuation. Transportmetrica A: Transport Science, 12(3), 230–248. https://doi.org/10.1080/23249935.2015.1125398\n   * van Cranenburgh, S., & Kouwenhoven, M. (2021). An artificial neural network based method to uncover the value-of-travel-time distribution. Transportation, 48(5), 2545–2583. https://doi.org/10.1007/s11116-020-10139-3',
+    'long_description': '# NP4VTT\n\nNP4VTT is a Python package that enables researchers to estimate and compare nonparametric models in a fast and convenient way. It comprises five nonparametric models for estimating the VTT distribution from data coming from two-attribute-two-alternative stated choice experiments:\n\n   * Local constant model  (Fosgerau, 2006, 2007)\n   * Local logit (Fosgerau, 2007)\n   * Rouwendal model (Rouwendal et al., 2010)\n   * Artificial Neural Network (ANN) based VTT model (van Cranenburgh & Kouwenhoven, 2021)\n   * Logistic Regression based VTT model (van Cranenburgh & Kouwenhoven, 2021)\n\nAdditionally, a Random Valuation model (Ojeda-Cabral, 2006) is included for benchmarking purposes\n\n## Installation steps\n\n* Use `pip` to install the `py-np4vtt` library normally:\n    - `python3 -m pip install py-np4vtt`\n\n\n## Examples\n\nWe provide Jupyter Notebooks that show how to configure and estimate each model included in NP4VTT:\n\n   * Local constant model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/lconstant.ipynb)\n   * Local logit: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/loclogit.ipynb)\n   * Rouwendal model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/rouwendal.ipynb)\n   * ANN-based VTT model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/ann.ipynb)\n   * Logistic Regression-based VTT model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/logistic.ipynb)\n\nThese examples guide the user through the process of loading a dataset, estimating a nonparametric model, and visualising the VTT distribution using scatter and histogram plots. We use the Norwegian 2009 VTT data to illustrate each example.\n\n**Take, for example, the VTT distribution from the Rouwendal model using NP4VTT:**\n\n![VTT distribution from the Rouwendal model using NP4VTT](examples/norway_data/outcomes/rouwendal.png)\n\n## References\n\n   * Fosgerau, M. (2006). Investigating the distribution of the value of travel time savings. Transportation Research Part B: Methodological, 40(8), 688–707. https://doi.org/10.1016/j.trb.2005.09.007\n   * Fosgerau, M. (2007). Using nonparametrics to specify a model to measure the value of travel time. Transportation Research Part A: Policy and Practice, 41(9), 842–856. https://doi.org/10.1016/j.tra.2006.10.004\n   * Rouwendal, J., de Blaeij, A., Rietveld, P., & Verhoef, E. (2010). The information content of a stated choice experiment: A new method and its application to the value of a statistical life. Transportation Research Part B: Methodological, 44(1), 136–151. https://doi.org/10.1016/j.trb.2009.04.006\n   * Ojeda-Cabral, M., Batley, R., & Hess, S. (2016). The value of travel time: Random utility versus random valuation. Transportmetrica A: Transport Science, 12(3), 230–248. https://doi.org/10.1080/23249935.2015.1125398\n   * van Cranenburgh, S., & Kouwenhoven, M. (2021). An artificial neural network based method to uncover the value-of-travel-time distribution. Transportation, 48(5), 2545–2583. https://doi.org/10.1007/s11116-020-10139-3',
     'author': 'José Ignacio Hernández',
     'author_email': 'J.I.Hernandez@tudelft.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.tudelft.nl/np4vtt/py-np4vtt',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `py-np4vtt-1.0.5/PKG-INFO` & `py-np4vtt-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-np4vtt
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python library providing NonParametric models for Value of Travel Time analysis
 Home-page: https://gitlab.tudelft.nl/np4vtt/py-np4vtt
 Author: José Ignacio Hernández
 Author-email: J.I.Hernandez@tudelft.nl
 Requires-Python: >=3.8,<=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -46,15 +46,15 @@
    * ANN-based VTT model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/ann.ipynb)
    * Logistic Regression-based VTT model: [link](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/blob/master/examples/logistic.ipynb)
 
 These examples guide the user through the process of loading a dataset, estimating a nonparametric model, and visualising the VTT distribution using scatter and histogram plots. We use the Norwegian 2009 VTT data to illustrate each example.
 
 **Take, for example, the VTT distribution from the Rouwendal model using NP4VTT:**
 
-![VTT distribution from the Rouwendal model using NP4VTT](https://gitlab.tudelft.nl/np4vtt/py-np4vtt/-/raw/master/examples/outcomes/rouwendal.png)
+![VTT distribution from the Rouwendal model using NP4VTT](examples/norway_data/outcomes/rouwendal.png)
 
 ## References
 
    * Fosgerau, M. (2006). Investigating the distribution of the value of travel time savings. Transportation Research Part B: Methodological, 40(8), 688–707. https://doi.org/10.1016/j.trb.2005.09.007
    * Fosgerau, M. (2007). Using nonparametrics to specify a model to measure the value of travel time. Transportation Research Part A: Policy and Practice, 41(9), 842–856. https://doi.org/10.1016/j.tra.2006.10.004
    * Rouwendal, J., de Blaeij, A., Rietveld, P., & Verhoef, E. (2010). The information content of a stated choice experiment: A new method and its application to the value of a statistical life. Transportation Research Part B: Methodological, 44(1), 136–151. https://doi.org/10.1016/j.trb.2009.04.006
    * Ojeda-Cabral, M., Batley, R., & Hess, S. (2016). The value of travel time: Random utility versus random valuation. Transportmetrica A: Transport Science, 12(3), 230–248. https://doi.org/10.1080/23249935.2015.1125398
```

