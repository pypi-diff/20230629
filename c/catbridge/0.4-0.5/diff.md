# Comparing `tmp/catbridge-0.4.tar.gz` & `tmp/catbridge-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catbridge-0.4.tar", last modified: Thu Jun 15 05:24:56 2023, max compression
+gzip compressed data, was "catbridge-0.5.tar", last modified: Thu Jun 29 08:06:26 2023, max compression
```

## Comparing `catbridge-0.4.tar` & `catbridge-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-15 05:24:56.138246 catbridge-0.4/
--rw-r--r--   0 bowen      (501) staff       (20)     1073 2023-06-13 01:32:07.000000 catbridge-0.4/LICENSE
--rw-r--r--   0 bowen      (501) staff       (20)     2004 2023-06-15 05:24:56.138038 catbridge-0.4/PKG-INFO
--rw-r--r--   0 bowen      (501) staff       (20)     1437 2023-06-15 05:21:37.000000 catbridge-0.4/README.md
-drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-15 05:24:56.136721 catbridge-0.4/catbridge/
--rw-r--r--   0 bowen      (501) staff       (20)       24 2023-06-13 07:10:57.000000 catbridge-0.4/catbridge/__init__.py
--rw-r--r--   0 bowen      (501) staff       (20)    38461 2023-06-14 09:29:36.000000 catbridge-0.4/catbridge/catbridge.py
-drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-15 05:24:56.137779 catbridge-0.4/catbridge.egg-info/
--rw-r--r--   0 bowen      (501) staff       (20)     2004 2023-06-15 05:24:44.000000 catbridge-0.4/catbridge.egg-info/PKG-INFO
--rw-r--r--   0 bowen      (501) staff       (20)      203 2023-06-15 05:24:56.000000 catbridge-0.4/catbridge.egg-info/SOURCES.txt
--rw-r--r--   0 bowen      (501) staff       (20)        1 2023-06-15 05:24:44.000000 catbridge-0.4/catbridge.egg-info/dependency_links.txt
--rw-r--r--   0 bowen      (501) staff       (20)       10 2023-06-15 05:24:44.000000 catbridge-0.4/catbridge.egg-info/top_level.txt
--rw-r--r--   0 bowen      (501) staff       (20)       38 2023-06-15 05:24:56.138304 catbridge-0.4/setup.cfg
--rw-r--r--   0 bowen      (501) staff       (20)      850 2023-06-15 05:23:33.000000 catbridge-0.4/setup.py
+drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-29 08:06:26.863741 catbridge-0.5/
+-rw-r--r--   0 bowen      (501) staff       (20)     1073 2023-06-13 01:32:07.000000 catbridge-0.5/LICENSE
+-rw-r--r--   0 bowen      (501) staff       (20)     2004 2023-06-29 08:06:26.863541 catbridge-0.5/PKG-INFO
+-rw-r--r--   0 bowen      (501) staff       (20)     1437 2023-06-15 05:21:37.000000 catbridge-0.5/README.md
+drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-29 08:06:26.862673 catbridge-0.5/catbridge/
+-rw-r--r--   0 bowen      (501) staff       (20)       24 2023-06-13 07:10:57.000000 catbridge-0.5/catbridge/__init__.py
+-rw-r--r--   0 bowen      (501) staff       (20)    58256 2023-06-29 07:52:55.000000 catbridge-0.5/catbridge/catbridge.py
+drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-29 08:06:26.863294 catbridge-0.5/catbridge.egg-info/
+-rw-r--r--   0 bowen      (501) staff       (20)     2004 2023-06-29 08:06:16.000000 catbridge-0.5/catbridge.egg-info/PKG-INFO
+-rw-r--r--   0 bowen      (501) staff       (20)      203 2023-06-29 08:06:26.000000 catbridge-0.5/catbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 bowen      (501) staff       (20)        1 2023-06-29 08:06:16.000000 catbridge-0.5/catbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 bowen      (501) staff       (20)       10 2023-06-29 08:06:16.000000 catbridge-0.5/catbridge.egg-info/top_level.txt
+-rw-r--r--   0 bowen      (501) staff       (20)       38 2023-06-29 08:06:26.863795 catbridge-0.5/setup.cfg
+-rw-r--r--   0 bowen      (501) staff       (20)      850 2023-06-29 08:04:12.000000 catbridge-0.5/setup.py
```

### Comparing `catbridge-0.4/LICENSE` & `catbridge-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `catbridge-0.4/PKG-INFO` & `catbridge-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catbridge
-Version: 0.4
+Version: 0.5
 Summary: CAT Bridge (Compounds And Transcripts Bridge) is a robust tool built with the goal of uncovering biosynthetic mechanisms in multi-omics data, such as identifying genes potentially involved in compound synthesis by incorporating metabolomics and transcriptomics data.
 Home-page: https://github.com/Bowen999/catbridge
 Author: Bowen Yang
 Author-email: by172@georgetown.edu
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `catbridge-0.4/README.md` & `catbridge-0.5/README.md`

 * *Files identical despite different names*

### Comparing `catbridge-0.4/catbridge/catbridge.py` & `catbridge-0.5/catbridge/catbridge.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,73 @@
 """
 Package Name: CAT Bridge (Compounds And Trancrips Bridge)
 Author: Bowen Yang
 email: by8@ualberta
-Version: 0.1.0
-Description: A detailed description of your package, what it does, and how to use it. 
+Homepage: 
+Version: 0.4.1
+Description: CAT Bridge (Compounds And Transcripts Bridge) is a robust tool built with the goal of uncovering biosynthetic mechanisms in multi-omics data, such as identifying genes potentially involved in compound synthesis by incorporating metabolomics and transcriptomics data. 
 
 For more detailed information on specific functions or classes, use the help() function on them. For example:
 help(your_package_name.your_function_name)
 
 
 #  ██████╗ █████╗ ████████╗    ██████╗ ██████╗ ██╗██████╗  ██████╗ ███████╗
 # ██╔════╝██╔══██╗╚══██╔══╝    ██╔══██╗██╔══██╗██║██╔══██╗██╔════╝ ██╔════╝
 # ██║     ███████║   ██║       ██████╔╝██████╔╝██║██║  ██║██║  ███╗█████╗  
 # ██║     ██╔══██║   ██║       ██╔══██╗██╔══██╗██║██║  ██║██║   ██║██╔══╝  
 # ╚██████╗██║  ██║   ██║       ██████╔╝██║  ██║██║██████╔╝╚██████╔╝███████╗
 #  ╚═════╝╚═╝  ╚═╝   ╚═╝       ╚═════╝ ╚═╝  ╚═╝╚═╝╚═════╝  ╚═════╝ ╚══════╝
 """
 
+# Data
 import pandas as pd
 import numpy as np
+from statsmodels.tsa.stattools import grangercausalitytests 
+import math
+
 from sklearn.preprocessing import MinMaxScaler
+from sklearn.preprocessing import StandardScaler
+from sklearn.decomposition import IncrementalPCA
+from sklearn.metrics.pairwise import cosine_similarity
+from sklearn.preprocessing import normalize
+from sklearn.decomposition import PCA
+from sklearn.cluster import KMeans
+from sklearn.preprocessing import normalize
 
+from scipy.stats import spearmanr
+from scipy.stats import pearsonr
+from scipy.stats import linregress #linear regression
+
+from tslearn.clustering import TimeSeriesKMeans
+from tslearn.preprocessing import TimeSeriesScalerMeanVariance
+
+
+
+
+# Plot
 import matplotlib.pyplot as plt
-import seaborn as sns
-import matplotlib.gridspec as gridspec
-from bioinfokit import analys, visuz
 import matplotlib.pyplot as plt
 from matplotlib.patches import Circle
-from PIL import Image
+import matplotlib.gridspec as gridspec
+import seaborn as sns
+from bioinfokit import analys, visuz
 import networkx as nx
-from sklearn.metrics.pairwise import cosine_similarity
+from PIL import Image
+from adjustText import adjust_text
+import textwrap
 
 
-from scipy.stats import spearmanr
-from scipy.stats import pearsonr
-import numpy as np
-from statsmodels.tsa.stattools import grangercausalitytests
-from sklearn.preprocessing import MinMaxScaler
-import subprocess
-import math
-from sklearn.decomposition import PCA
-from sklearn.cluster import KMeans
 
-import pandas as pd
-from tslearn.clustering import TimeSeriesKMeans
-from tslearn.preprocessing import TimeSeriesScalerMeanVariance
+# Others
+import shutil #move file
+import getpass 
+import os
+import subprocess #run command line
+import openai 
 
-import openai
-import getpass
 
 
 
 """
 ***********  1. Pre-Processing ***********
 #  ██████╗ █████╗ ████████╗    ██████╗ ██████╗ ██╗██████╗  ██████╗ ███████╗
 # ██╔════╝██╔══██╗╚══██╔══╝    ██╔══██╗██╔══██╗██║██╔══██╗██╔════╝ ██╔════╝
@@ -121,15 +137,30 @@
     if method == 'min-max':
         scaler = MinMaxScaler()
         df = scaler.fit_transform(df)
     elif method == 'pareto':
         df = (df - df.mean()) / np.sqrt(df.std())
 
 
-# ************* One Column Scaling ***************
+def scale_df(df):
+    """Apply a log10 transformation and scale all values in a dataframe to the range 0-1."""
+    
+    # Apply a log10 transformation, add a small constant to avoid log(0)
+    df = np.log10(df + 1e-10)
+    
+    # Check for NaNs and fill or remove them before scaling
+    if df.isnull().values.any():
+        df = df.fillna(method='ffill')  # you could also use 'bfill' or df.dropna()
+        
+    scaler = MinMaxScaler()
+    df_scaled = pd.DataFrame(scaler.fit_transform(df), columns=df.columns)
+    
+    return df_scaled
+
+
 def scale_column(df, column_name):
     """
     Scale the values of a column using the MinMaxScaler.
     """
     # Create a scaler object
     scaler = MinMaxScaler()
 
@@ -239,14 +270,102 @@
     for df in dataframes[1:]:
         merged_dataframe = merged_dataframe.merge(df, on='Name', how='outer')
 
     return merged_dataframe 
 
 
 
+# ************ Find the increasing trend ***************
+def calculate_trend_strength(df):
+    """
+    Function to calculate and sort the strength of the upward trend in each row of a DataFrame.
+
+    This function calculates the trend strength (r-value) for each row in the DataFrame 
+    using linear regression. It then adds a new column to the DataFrame with these r-values. 
+    Finally, it sorts the DataFrame by these r-values in descending order and returns the 
+    sorted DataFrame.
+
+    Parameters:
+    df (pandas.DataFrame): The DataFrame to be processed. 
+
+    Returns:
+    df_sorted_by_trend_strength (pandas.DataFrame): The input DataFrame, but with an added 
+    column for trend strength and sorted by this column in descending order.
+    """
+
+    # Function to calculate the trend strength (r-value)
+    def upward_trend_strength(row):
+        _, _, rvalue, _, _ = linregress(x=range(len(row)), y=row)
+        return rvalue
+
+    # Apply function to each row to get trend strengths
+    trend_strength = df.apply(upward_trend_strength, axis=1)
+
+    # Add a new column to df with trend strengths
+    df_with_trend_strength = df.assign(trend_strength=trend_strength)
+
+    # Sort df by trend strength (r-value) in descending order
+    df_sorted_by_trend_strength = df_with_trend_strength.sort_values(by='trend_strength', ascending=False)
+
+    # Return sorted dataframe
+    return df_sorted_by_trend_strength
+
+
+
+
+
+def merge_and_reduce(df1, df2, n_components):
+    """
+    This function takes two dataframes with the same columns (sample names), performs Incremental PCA to reduce 
+    the dimension of their index (IDs), and then merges them together. It ensures that both dataframes 
+    have the same contribution to the final result by normalizing and reducing the dimension of each dataframe 
+    separately before merging.
+
+    Parameters:
+    df1 (pandas.DataFrame): The first dataframe.
+    df2 (pandas.DataFrame): The second dataframe.
+    n_components (int): The number of dimensions for the output dataframe.
+
+    Returns:
+    pandas.DataFrame: The merged dataframe with reduced dimensions.
+    """
+    
+    # Normalize each dataframe by their L2 norm
+    scaler = StandardScaler()
+    df1_norm = pd.DataFrame(scaler.fit_transform(df1), columns=df1.columns, index=df1.index)
+    df2_norm = pd.DataFrame(scaler.fit_transform(df2), columns=df2.columns, index=df2.index)
+    
+    # Function to perform Incremental PCA and reduce dimensions
+    def ipca_reduce(df, n_components):
+        # Transpose the dataframe to reduce dimension of rows
+        df_t = df.T
+
+        # Apply Incremental PCA
+        ipca = IncrementalPCA(n_components=n_components, batch_size=10)
+        df_reduced = ipca.fit_transform(df_t)
+
+        # Create a dataframe with the reduced dimension data
+        df_reduced = pd.DataFrame(df_reduced, index=df_t.index, columns=[f'feature_{i}' for i in range(n_components)])
+
+        # Transpose back to original form
+        df_reduced_t = df_reduced.T
+
+        return df_reduced_t
+    
+    # Reduce dimensions of each dataframe
+    df1_reduced = ipca_reduce(df1_norm, n_components)
+    df2_reduced = ipca_reduce(df2_norm, n_components)
+
+    # Concatenate the two reduced dataframes
+    df_merged = pd.concat([df1_reduced, df2_reduced])
+
+    return df_merged
+
+
+
 
 
 
 
    
    
 """
@@ -256,15 +375,116 @@
 # ██║     ███████║   ██║       ██████╔╝██████╔╝██║██║  ██║██║  ███╗█████╗  
 # ██║     ██╔══██║   ██║       ██╔══██╗██╔══██╗██║██║  ██║██║   ██║██╔══╝  
 # ╚██████╗██║  ██║   ██║       ██████╔╝██║  ██║██║██████╔╝╚██████╔╝███████╗
 #  ╚═════╝╚═╝  ╚═╝   ╚═╝       ╚═════╝ ╚═╝  ╚═╝╚═╝╚═════╝  ╚═════╝ ╚══════╝
 """ 
 
 # ************* 2.1 Correlation Score ***************
+# ***************** Granger *********************
+def compute_granger(df, target, maxlag=1):
+    """
+    Compute the Granger causality score for each row in the dataframe.
+    The X is each row in the dataframe and the Y is the target list.
+    The returd value is the p-value of the F test for the maximum lag.
+    
+    Parameters:
+        df (pandas DataFrame): The DataFrame to be aggregated.
+        target (list): The target list.
+    
+    Returns:
+        index_list (list): The list of row indices.
+    
+    """
+    # Initialize lists to store results
+    index_list = []
+    p_value_list = []
+
+    # Loop through each row in the dataframe
+    for idx, row in df.iterrows():
+        # Skip if the row or the target list has constant values
+        if np.std(row.values) == 0 or np.std(target) == 0:
+            continue
+
+        # Combine the row and target into a DataFrame
+        data = pd.concat([pd.Series(target), pd.Series(row.values)], axis=1)
+
+        # Perform the Granger causality test
+        try:
+            result = grangercausalitytests(data, maxlag=maxlag, verbose=False)
+
+            # Extract the p-value of the F test for the maximum lag
+            p_value = result[maxlag][0]['ssr_ftest'][1]
+            p_value = 1-p_value
+
+            # Append results to the lists
+            index_list.append(idx)
+            p_value_list.append(p_value)
+        except Exception as e:
+            #add NA if there is an error
+            index_list.append(idx)
+            p_value_list.append(np.nan)
+            
+            # print(f"Error at index {idx}: {str(e)}")
+
+    # Create a new dataframe to store results
+    results_df = pd.DataFrame({
+        'Name': index_list,
+        'Granger': p_value_list
+    })
+
+    return results_df
+
+
+def compute_reverse_granger(df, target, maxlag=1):
+    """
+    X is target and Y is each row in the dataframe (df).
+    """
+    
+     # Initialize lists to store results
+    index_list = []
+    p_value_list = []
+
+    # Loop through each row in the dataframe
+    for idx, row in df.iterrows():
+        # Skip if the row or the target list has constant values
+        if np.std(row.values) == 0 or np.std(target) == 0:
+            continue
+
+        # Combine the row and target into a DataFrame
+        data = pd.concat([pd.Series(row.values), pd.Series(target)], axis=1)
+
+        # Perform the Granger causality test
+        try:
+            result = grangercausalitytests(data, maxlag=maxlag, verbose=False)
+
+            # Extract the p-value of the F test for the maximum lag
+            p_value = result[maxlag][0]['ssr_ftest'][1]
+            p_value = 1-p_value
+
+            # Append results to the lists
+            index_list.append(idx)
+            p_value_list.append(p_value)
+        except Exception as e:
+            #add NA if there is an error
+            index_list.append(idx)
+            p_value_list.append(np.nan)
+            
+            # print(f"Error at index {idx}: {str(e)}")
+
+    # Create a new dataframe to store results
+    results_df = pd.DataFrame({
+        'Name': index_list,
+        'Granger': p_value_list
+    })
 
+    return results_df
+
+    
+
+# ***************** Spearman *********************
 def compute_spearman(df, target):
     # Initialize lists to store results
     index_list = []
     corr_list = []
     p_value_list = []
 
     # Loop through each row in the dataframe
@@ -284,19 +504,15 @@
         #'P-value': p_value_list
     })
 
     return results_df
 
 
 
-"""
-Pearson 
-df is a dataframe, target is a list
-Pearson's correlation coefficient is the covariance of the two variables divided by the product of their standard deviations. The form of the definition involves a "product moment", that is, the mean (the first moment about the origin) of the product of the mean-adjusted random variables; hence the modifier product-moment in the name.
-"""
+# ***************** Pearson *********************
 def compute_pearson(df, target):
     # Initialize lists to store results
     index_list = []
     corr_list = []
     p_value_list = []
 
     # Loop through each row in the dataframe
@@ -318,95 +534,122 @@
 
     return results_df
 
 
 
 
 
-# ***************** Granger *********************
-def compute_granger(df, target, maxlag=1):
-    # Initialize lists to store results
-    index_list = []
-    p_value_list = []
 
-    # Loop through each row in the dataframe
-    for idx, row in df.iterrows():
-        # Skip if the row or the target list has constant values
-        if np.std(row.values) == 0 or np.std(target) == 0:
-            continue
 
-        # Combine the row and target into a DataFrame
-        data = pd.concat([pd.Series(target), pd.Series(row.values)], axis=1)
 
-        # Perform the Granger causality test
-        try:
-            result = grangercausalitytests(data, maxlag=maxlag, verbose=False)
+def granger_list(A, B, maxlag):
+    """
+    Compute granger test P value for listA (X), and listB (y) 
+    """
+    
+    # Combine the two lists into a 2D array
+    data = np.column_stack((A, B))
+    
+    # Perform the Granger causality test and return the result
+    result = grangercausalitytests(data, maxlag, verbose=False)
+    #result = grangercausalitytests(data, maxlag)
 
-            # Extract the p-value of the F test for the maximum lag
-            p_value = result[maxlag][0]['ssr_ftest'][1]
-            p_value = 1-p_value
+    # In this function, we'll return just the p-value for each lag.
+    # You may want to modify this to return other information.
+    p_values = {lag: result[lag][0]['ssr_ftest'][1] for lag in result.keys()}
+    
+    return p_values
 
-            # Append results to the lists
-            index_list.append(idx)
-            p_value_list.append(p_value)
-        except Exception as e:
-            #add NA if there is an error
-            index_list.append(idx)
-            p_value_list.append(np.nan)
-            
-            # print(f"Error at index {idx}: {str(e)}")
 
-    # Create a new dataframe to store results
-    results_df = pd.DataFrame({
-        'Name': index_list,
-        'Granger': p_value_list
-    })
+# *************** 2.2 FC Score ***************
+# ********* Noontide ************
+# def find_noontide(df, row_name):
+#     """
+#     Find the column with the highest value in the row, and return the column, and the column after it (name).
+#     If the column with the highest value is the last column, then return the column with the second highest value, and the column after it (name).
+    
+#     Parameters:
+#         df (pandas DataFrame): The DataFrame has been aggregated.
+#         row_name (str): The name of the row to be detected.
+        
+#     Returns:
+#         column_n (str): The name of the column with the highest value.
+#     """
+#     # Get the row with the specified name
+#     row = df.loc[row_name]
+
+#     # Identify the column with the highest value
+#     column_n = row.idxmax()
+#     col_idx = list(df.columns).index(column_n)
+
+#     # If column with max value is last column, then find the second highest column
+#     if col_idx == len(df.columns) - 1:
+#         row[column_n] = row.min() # set value in column_n to minimum value of row
+#         column_n = row.idxmax()   # get column with max value now
+
+#     # Find column after column_n
+#     col_idx = list(df.columns).index(column_n)
+#     if col_idx < len(df.columns) - 1: # Make sure it's not the last column
+#         column_n_plus_1 = df.columns[col_idx + 1]
+#     else:
+#         raise Exception("There is no column after the column with the maximum value.")
+
+#     # Keep only column n and column n+1
+#     df_filtered = df[[column_n, column_n_plus_1]]
+
+#     return df_filtered.columns
 
-    return results_df
 
 
-# *************** 2.2 FC Score ***************
 # ********* Noontide ************
 def find_noontide(df, row_name):
     """
     Find the column with the highest value in the row, and return the column, and the column after it (name).
     If the column with the highest value is the last column, then return the column with the second highest value, and the column after it (name).
     
     Parameters:
         df (pandas DataFrame): The DataFrame has been aggregated.
         row_name (str): The name of the row to be detected.
         
     Returns:
         column_n (str): The name of the column with the highest value.
     """
     # Get the row with the specified name
-    row = df.loc[row_name]
+    row = df.loc[row_name].copy()
+
+    # Convert to numeric and handle errors by replacing non-numeric values with NaN
+    row = pd.to_numeric(row, errors='coerce')
+
+    # Handle rows that are all NaN
+    if row.isna().all():
+        raise Exception(f"The row '{row_name}' contains only non-numeric or missing values.")
 
     # Identify the column with the highest value
     column_n = row.idxmax()
     col_idx = list(df.columns).index(column_n)
 
     # If column with max value is last column, then find the second highest column
     if col_idx == len(df.columns) - 1:
-        row[column_n] = row.min() # set value in column_n to minimum value of row
-        column_n = row.idxmax()   # get column with max value now
+        row[column_n] = np.nan # set value in column_n to NaN
+        column_n = row.idxmax() # get column with max value now
 
     # Find column after column_n
     col_idx = list(df.columns).index(column_n)
     if col_idx < len(df.columns) - 1: # Make sure it's not the last column
         column_n_plus_1 = df.columns[col_idx + 1]
     else:
         raise Exception("There is no column after the column with the maximum value.")
 
     # Keep only column n and column n+1
     df_filtered = df[[column_n, column_n_plus_1]]
 
     return df_filtered.columns
 
 
+
 # ********* df for fc ************
 def df_for_fc(df1, target, df2, design):
     """
     Gnerate the design matrix and matrix for computing the FC score.
     
     Parameters:
         df1 (pandas DataFrame): The DataFrame has been aggregated (processed_metabo).
@@ -420,28 +663,51 @@
 
     # Saving to CSV files instead of returning
     design_fc.to_csv('result/design_fc.csv')
     matrix_fc.to_csv('result/matrix_fc.csv')
     
     
 
+
 def no_repeat_fc(df, noontide):
+    
+    """
+    Compute the FC score for each metabolite. This function is used for Study Design that has no biological repeats.
+    
+    Parameters:
+        df (pandas DataFrame): The DataFrame for fc computing (gene).
+        noontide (list): The list of the column names of the noontide samples. (can be obtained from find_noontide function)
+    
+    Returns:
+        df (pandas DataFrame): The DataFrame with the FC score.
+    """
+    
     df['log2FoldChange'] = df[noontide[0]]/df[noontide[1]]
-    df['log2FoldChange'] = df['log2FoldChange'].apply(lambda x: math.log2(x))
+    df['log2FoldChange'] = df['log2FoldChange'].apply(lambda x: math.log2(x if x > 0 else np.finfo(float).eps))
+    
+    # Replace infinities with 0
+    df.replace([np.inf, -np.inf], 0, inplace=True)
+    
+    # Replace NaNs with 0
+    df['log2FoldChange'].fillna(0, inplace=True)
+    
     #make the range of log2FoldChange from 0-1
     scaler = MinMaxScaler()
     # Apply the scaler to the 'log2FoldChange' column
     df['log2FoldChange'] = scaler.fit_transform(df[['log2FoldChange']])
     df = df[['log2FoldChange']]
     return df
 
 
 
 # ********* FC Compute ********
 def fc_comp():
+    """
+    Compute the fold change using R script(FC.R)
+    """
     result = subprocess.run(['Rscript', 'FC.R'], stdout=subprocess.PIPE)
     fc = read_upload('result/fc.csv')
     fc.index.name = 'Name'
     #for value in fc['log2FoldChange'], do scaling to makeit range from 0-1
     scaler = MinMaxScaler()
     # Apply the scaler to the 'log2FoldChange' column 
     fc['log2FoldChange'] = -1 * fc['log2FoldChange']
@@ -465,14 +731,15 @@
     df_sorted = df.sort_values('Rank')
     # df_sorted.set_index('Rank', inplace=True)
     # df_sorted = df_sorted[['Name', 'Score', 'Rank']]
     
     return df_sorted
 
 
+# Annotation -> Score
 keywords_scores = {'ase': 0.2, 'enzyme': 0.2, 'synthase': 0.2}
 def annotation_score(df, keywords=keywords_scores):
     """
     This function replaces the value in the 'Description' column of the input dataframe with the highest score
     from the keywords dictionary if a word in the description ends with any of the keywords. If a description is NaN,
     it is replaced with 0.1. If no keyword is found in a description, the description is replaced with 0.
 
@@ -534,14 +801,98 @@
     df['Cluster'] = labels
     df = df['Cluster']
 
     return df
 
 
 
+# ************* Upward trend strength *************
+def trend_strength(df):
+    """
+    Function to calculate and sort the strength of the upward trend in each row of a DataFrame.
+
+    This function calculates the trend strength (r-value) for each row in the DataFrame 
+    using linear regression. It then adds a new column to the DataFrame with these r-values. 
+    Finally, it sorts the DataFrame by these r-values in descending order and returns the 
+    sorted DataFrame.
+
+    Parameters:
+    df (pandas.DataFrame): The DataFrame to be processed. 
+
+    Returns:
+    df_sorted_by_trend_strength (pandas.DataFrame): The input DataFrame, but with an added 
+    column for trend strength and sorted by this column in descending order.
+    """
+
+    # Function to calculate the trend strength (r-value)
+    def upward_trend_strength(row):
+        _, _, rvalue, _, _ = linregress(x=range(len(row)), y=row)
+        return rvalue
+
+    # Apply function to each row to get trend strengths
+    trend_strength = df.apply(upward_trend_strength, axis=1)
+
+    # Add a new column to df with trend strengths
+    df_with_trend_strength = df.assign(trend_strength=trend_strength)
+
+    # Sort df by trend strength (r-value) in descending order
+    df_sorted_by_trend_strength = df_with_trend_strength.sort_values(by='trend_strength', ascending=False)
+
+    # Return sorted dataframe
+    return df_sorted_by_trend_strength
+
+
+
+# ****************** Importance *******************
+def top_important_features(df, n_top):
+    """
+    This function calculates the importance of features based on a PCA model. The importance is calculated 
+    as the sum of the squares of the PCA loadings for each feature. The function then returns the top n 
+    features based on their importance.
+    
+    Parameters:
+    df (pd.DataFrame): The input DataFrame where each row corresponds to a sample and each column corresponds 
+                       to a feature (e.g., gene expression values for different genes). The index of the DataFrame
+                       is assumed to represent sample identifiers and the columns of the DataFrame are assumed to 
+                       represent feature names.
+    n_top (int): The number of top features to return based on their calculated importance.
+
+    Returns:
+    pd.DataFrame: A DataFrame containing the top n features and their corresponding importances, sorted by importance.
+    """
+
+    try:
+        # Transpose your data so that rows are time points and columns are genes
+        df_transposed = df.transpose()
+
+        # Initialize PCA object
+        pca = PCA()
+
+        # Fit the model
+        pca.fit(df_transposed)
+
+        # Get the loadings for each gene
+        loadings = pca.components_
+
+        # Calculate the importance of each gene as the sum of squares of its loadings
+        importance = np.sum(loadings**2, axis=0)
+
+        # Create a DataFrame of importances and gene names
+        importance_df = pd.DataFrame({'Gene': df_transposed.columns, 'Importance': importance})
+
+        # Sort by importance
+        importance_df = importance_df.sort_values('Importance', ascending=False)
+
+        # Return the top n genes
+        return importance_df.head(n_top)
+
+    except Exception as e:
+        print("An error occurred while computing the top important features.")
+        print(str(e))
+        return None
 
 
 
 
 
 
 
@@ -549,217 +900,275 @@
 
 
 
 
 
 
 
+"""
 #********* 3 PLOT FUNCTION ********   
 #  ██████╗ █████╗ ████████╗    ██████╗ ██████╗ ██╗██████╗  ██████╗ ███████╗
 # ██╔════╝██╔══██╗╚══██╔══╝    ██╔══██╗██╔══██╗██║██╔══██╗██╔════╝ ██╔════╝
 # ██║     ███████║   ██║       ██████╔╝██████╔╝██║██║  ██║██║  ███╗█████╗  
 # ██║     ██╔══██║   ██║       ██╔══██╗██╔══██╗██║██║  ██║██║   ██║██╔══╝  
 # ╚██████╗██║  ██║   ██║       ██████╔╝██║  ██║██║██████╔╝╚██████╔╝███████╗
 #  ╚═════╝╚═╝  ╚═╝   ╚═╝       ╚═════╝ ╚═╝  ╚═╝╚═╝╚═════╝  ╚═════╝ ╚══════╝
-    
-    
-    
-# Line
-def plot_line(target, title):
-    plt.figure(figsize=(10, 3))
-    plt.plot(target)
-    plt.title(title)
-    plt.show()
-    return
-
-# Heatmap
-def plot_heatmap(dataframe, palette='viridis', figsize=(10, 8), row_threshold=50, save_path=None):
-    #remov the rows that have all 0 values
-    dataframe = dataframe.loc[~(dataframe==0).all(axis=1)]
-    if dataframe.shape[0] > row_threshold:
-        row_labels = False
-    else:
-        row_labels = True
-    
-    sns.clustermap(dataframe, cmap=palette, yticklabels=row_labels, xticklabels=True, figsize=figsize)
-    #set x axis label
-    plt.xlabel(dataframe.columns.name)
-    
-    if save_path:
-        plt.savefig(save_path)
-    
-    plt.show()
-    return 
-
-
-# Hexbin
-def plot_hexbin(data, x_axis, y_axis, gridsize=20):
-    sns.jointplot(x=x_axis, y=y_axis, data=data, kind='hex', gridsize=20)
-    plt.xlabel(x_axis)
-    plt.ylabel(y_axis)
-    plt.show()
-
+"""
 
-# Line Heatmap
-def plot_line_heatmap(df, name_value, cmap='vlag'):
-    """
-    Plot a line plot and a heatmap of the specified row in the input dataframe.
     
-    Parameters:
-        df (pandas.DataFrame): The input dataframe.
-        name_value (str): The value in the 'Name' column of the row to plot.
-        cmap (str): The name of the colormap to use for the heatmap. Defaults to 'vlag'.
+# Line Plot
+def plot_line(df, target, save_path=None):
     """
-    # Find the row where 'Name' is equal to name_value
-    row = df.loc[df['Name'] == name_value]
-
-    # Extract the desired columns and convert them to a list
-    desired_columns = ['Granger', 'log2FoldChange', 'Pearson', 'Spearman']
-    list1 = row[desired_columns].values.tolist()[0]
+    Plots a line graph of the target row from the dataframe.
+    Args:
+    df (pd.DataFrame): DataFrame to plot.
+    target (str): Target row to plot.
+    """
+    try:
+        # Access the target row
+        target_row = df.loc[target]
+
+        # Create the line plot
+        plt.figure(figsize=(12,3))
+        plt.plot(target_row.index, target_row.values)
+        
+        # Add labels and title
+        plt.title(f'{target}')
+        
+        if save_path:
+            plt.savefig(save_path)
+        else:
+            plt.show()
 
-    # Get the other columns by dropping the ones already in list1
-    remaining_columns = df.drop(columns=['Name'] + desired_columns)
-    list2 = remaining_columns.loc[remaining_columns.index == row.index[0]].values.tolist()[0]
+    except Exception as e:
+        print(f"An error occurred: {e}")
 
-    # Reshape list1 into a 2D array for the heatmap
-    list1_2d = np.array(list1).reshape(-1, 1)
 
-    # Create subplots with adjusted sizes
-    fig = plt.figure(figsize=(10, 2))
-    grid = plt.GridSpec(1, 10, hspace=0.2, wspace=0.2)  # We'll use 8 columns in total
+# Heatmap
+def plot_heatmap(dataframe, palette='vlag', figsize=(6, 8), row_threshold=50, save_path=None):
+    """
+    Plot the heatmap of the dataframe. If the number of rows is greater than row_threshold, row labels are not shown.
+    Args:
+    dataframe (pd.DataFrame): DataFrame to plot.
+    palette (str, optional): Palette to use for the plot. Defaults to 'vlag'.
+    figsize (tuple, optional): Size of the plot. Defaults to (10, 8).
+    row_threshold (int, optional): Threshold for number of rows to determine whether to show row labels. Defaults to 50.
+    save_path (str, optional): If provided, save the plot to this path. Otherwise, the plot is shown using plt.show(). Defaults to None.
+    """
+    try:
+        # Remove the rows that have all 0 values
+        dataframe = dataframe.loc[~(dataframe==0).all(axis=1)]
+
+        if dataframe.shape[0] > row_threshold:
+            row_labels = False
+            g = sns.clustermap(dataframe, cmap=palette, yticklabels=row_labels, xticklabels=True, figsize=figsize, col_cluster=False)
+        else:
+            row_labels = True
+            plt.figure(figsize=figsize)
+            sns.heatmap(dataframe, cmap=palette, yticklabels=row_labels, xticklabels=True)
+
+        # Set x axis label
+        plt.xlabel(dataframe.columns.name)
+
+        # If row_labels is False, add a y-axis label 'features'
+        if not row_labels:
+            g.ax_heatmap.set_ylabel(' ')
+        
+        if save_path:
+            plt.savefig(save_path)
+        else:
+            plt.show()
 
-    # Plot the line graph on the left (using 7 out of 8 columns)
-    ax1 = plt.subplot(grid[:9])  # equivalent to grid[0, :7]
-    ax1.plot(list2, color='navy')
-    ax1.set_title(name_value)
-    ax1.set_xticks(range(len(remaining_columns.columns)))
-    ax1.set_xticklabels(remaining_columns.columns, rotation=90)
+    except Exception as e:
+        print(f"An error occurred: {e}")
 
-    # Plot the heatmap on the right (using 1 out of 8 columns) without color bar
-    ax2 = plt.subplot(grid[9:])  # equivalent to grid[0, 7:]
-    sns.heatmap(list1_2d, ax=ax2, cmap=cmap, cbar=False, yticklabels=desired_columns)
-    ax2.yaxis.tick_right()
-    ax2.xaxis.set_visible(False)  # hide the x-axis
-    ax2.set_yticklabels(ax2.get_yticklabels(), rotation=0)  # set rotation to 0
 
-    # Show the plotc
-    plt.tight_layout()
-    plt.show()
 
 
-# Line Heatmap for all data
-def plot_data(df, name_value, ax1, ax2, cmap='vlag'):
+# ********************* PCA ****************************
+def plot_pca(gene, design, n_clusters, save_path=None):
     """
-    plot the line graph and heatmap for the given gene name
+    Perform PCA on the gene expression data, and plot the result.
     
-    df: dataframe
-    name_value: the name of the gene
-    ax1: the axis for the line graph, ax1 = plt.subplot(grid[:9])
-    ax2: the axis for the heatmap, ax2 = plt.subplot(grid[9:])
-    cmap: the color map for the heatmap
-    """
-    # Find the row where 'Name' is equal to name_value
-    row = df.loc[df['Name'] == name_value]
-
-    # Extract the desired columns and convert them to a list
-    desired_columns = ['Granger', 'log2FoldChange', 'Pearson', 'Spearman']
-    list1 = row[desired_columns].values.tolist()[0]
-
-    # Get the other columns by dropping the ones already in list1
-    remaining_columns = df.drop(columns=['Name'] + desired_columns)
-    list2 = remaining_columns.loc[remaining_columns.index == row.index[0]].values.tolist()[0]
+    Parameters:
+        gene: the gene expression dataframe
+        design: the design dataframe
+        n_clusters: the number of clusters to use in K-means clustering
+    """
+    try:
+        # Transpose your DataFrame, as PCA works on the features (columns), not on the samples (rows)
+        gene_transposed = gene.T
+
+        # Perform PCA on your data
+        pca = PCA(n_components=2)  # here we ask for the first two principal components
+        pca_result = pca.fit_transform(gene_transposed)
+
+        # Convert the PCA result to a DataFrame
+        pca_df = pd.DataFrame(data=pca_result, columns=['PC1', 'PC2'])
+
+        # Add a 'sample' column
+        pca_df['sample'] = gene_transposed.index
+
+        # Get group information from the design dataframe
+        pca_df = pca_df.merge(design[['group']], left_on='sample', right_index=True)
+
+        fig, ax = plt.subplots(figsize=(6, 8))
+
+        if n_clusters > 0:
+            # Perform K-means clustering
+            kmeans = KMeans(n_clusters=n_clusters, random_state=0).fit(pca_df[['PC1', 'PC2']])
+            pca_df['Cluster'] = kmeans.labels_
+
+            # Plot the points on the scatterplot
+            scatter = sns.scatterplot(x="PC1", y="PC2", hue="group", data=pca_df, palette="Paired", s=100, alpha=0.7, ax=ax)
+
+            # For each cluster, add a circle at the mean coordinates with radius proportional to the standard deviation
+            for cluster in set(kmeans.labels_):
+                cluster_points = pca_df[pca_df['Cluster'] == cluster][['PC1', 'PC2']]
+                # Calculate mean and standard deviation for the cluster
+                cluster_mean = cluster_points.mean().values
+                cluster_std = cluster_points.std().values
+                # Add a circle at the mean coordinates with radius=stddev
+                circle = Circle(cluster_mean, np.linalg.norm(cluster_std), alpha=0.1)
+                ax.add_artist(circle)
+        else:
+            # Plot the points on the scatterplot without clustering
+            scatter = sns.scatterplot(x="PC1", y="PC2", hue="group", data=pca_df, palette="Paired", s=100, alpha=0.7, ax=ax)
 
-    # Reshape list1 into a 2D array for the heatmap
-    list1_2d = np.array(list1).reshape(-1, 1)
+        # Check if the legend exists before trying to remove it
+        legend = ax.get_legend()
+        if legend is not None:
+            legend.remove()
+
+        # Annotate points on the graph with the sample names
+        texts = []
+        for i, sample in enumerate(pca_df['sample']):
+            texts.append(plt.text(pca_df.iloc[i].PC1, pca_df.iloc[i].PC2, sample, color='gray'))
+            
+        # Adjust the labels to avoid overlap
+        adjust_text(texts)
 
-    # Plot the line graph on the left 
-    ax1.plot(list2, color='navy')
-    ax1.set_title(name_value)
-    ax1.set_xticks(range(len(remaining_columns.columns)))
-    ax1.set_xticklabels(remaining_columns.columns, rotation=90)
+        plt.xlabel('PC1')
+        plt.ylabel('PC2')
+        # plt.title('PCA', fontweight='bold')
+
+        # Hide X and Y values
+        plt.xticks([])
+        plt.yticks([])
+        
+        if save_path:
+            plt.savefig(save_path)
+        else:
+            plt.show()
+    except Exception as e:
+        print(f"An error occurred: {e}")
 
-    # Plot the heatmap on the right without color bar
-    sns.heatmap(list1_2d, ax=ax2, cmap=cmap, cbar=False, yticklabels=desired_columns)
-    ax2.yaxis.tick_right()
-    ax2.xaxis.set_visible(False)  # hide the x-axis
-    ax2.set_yticklabels(ax2.get_yticklabels(), rotation=0)  # set rotation to 0
 
 
-def plot_all_data(df):
+# ****************** Top Important Features ******************
+def plot_top_features(df, color='crest', save_path=None):
     """
-    plot the line graph and heatmap for the top 10 genes in the dataframe
+    This function creates a scatter plot of the importances of the top n features, as returned by the 
+    top_important_features function. The color palette is applied based on bins of 'Importance'.
+    
+    Parameters:
+    df (pd.DataFrame): The input DataFrame as returned by the top_important_features function.
+    color (str): The color map to use for the scatter plot.
+
+    Returns:
+    None
     """
-    df = df.head(10)
-    num_rows = df.shape[0]
-    fig = plt.figure(figsize=(10, num_rows * 2))  # adjust the figure height based on the number of rows
-    grid = plt.GridSpec(num_rows, 10, hspace=0.5, wspace=0.2)
-
-    for i, row in df.iterrows():
-        ax1 = plt.subplot(grid[i, :9])  # line graph
-        ax2 = plt.subplot(grid[i, 9:])  # heatmap
-        plot_data(df, row['Name'], ax1, ax2)
+
+    try:
+        # Bin the 'Importance' into categories
+        df['Importance_Category'] = pd.qcut(df['Importance'], q=4)
+
+        # Create the scatter plot
+        fig, ax = plt.subplots(figsize=(6, 6))
+        scatter = sns.scatterplot(data=df, y='Gene', x='Importance', hue='Importance_Category', size='Importance', palette=color, sizes=(50, 200), ax=ax)
         
-        # Hide the x labels except for the last line plot
-        if i < num_rows - 1:
-            ax1.set_xticklabels([]) 
+        # Set title and labels
+        ax.set_xlabel('Importance')
+        ax.set_ylabel(' ')
+
+        # Split long y labels into two lines
+        y_labels = [textwrap.fill(label.get_text(), width=20) for label in scatter.get_yticklabels()]
+        ax.set_yticklabels(y_labels)
+
+        # Remove legend
+        scatter.legend_.remove()
+
+        # Adjust the space for y label
+        plt.subplots_adjust(left=0.3)
+          
+        if save_path:
+            plt.savefig(save_path)
         else:
-            ax1.set_xticklabels(ax1.get_xticklabels(), rotation=90)
+            plt.show()
+        return plt
 
-    plt.tight_layout()
-    plt.show()
+    except Exception as e:
+        print("An error occurred while creating the scatter plot.")
+        print(str(e))
 
 
 
 
 # Volcano Plot
 def plot_volcano(path, lfc_threshold, padj_threshold):
+    """
+    path: the path to the csv file
+    lfc_threshold: the log2 fold change threshold
+    padj_threshold: the adjusted p-value threshold
+    """
     # Import and preprocess data
     fc_for_volcano = pd.read_csv(path)
     fc_for_volcano.reset_index(inplace=True)
     fc_for_volcano.rename(columns={'index':'Name'}, inplace=True)
     gene_exp = fc_for_volcano
     gene_exp = gene_exp.dropna(subset=['padj'])
 
     # Check if at least 10 gene names exist
     genenames = gene_exp['Name'].head(10) if len(gene_exp['Name']) >= 10 else None
 
     # Create plot
+    plt.rcParams['figure.figsize'] = [6, 6]
     visuz.GeneExpression.volcano(df=gene_exp, 
                                 lfc='log2FoldChange', pv='padj', sign_line=True,
                                 lfc_thr=(lfc_threshold, lfc_threshold), pv_thr=(padj_threshold, padj_threshold),
                                 plotlegend=True, legendpos='upper right', legendanchor=(1.46,1),
                                 color=('maroon','gainsboro','steelblue'), theme='whitesmoke',
                                 valpha=1, dotsize=5,
-                                geneid = 'Name',
-                                genenames = tuple(genenames) if genenames is not None else None,
+                                geneid = 'Name'
+                                # genenames = tuple(genenames) if genenames is not None else None,
                                 )
 
-    # Save and display image
     # plt.savefig('result/volcano_plot.png')
-    img = Image.open('volcano.png')
-    
     img = Image.open('volcano.png')  # replace with your image file path if not in the same directory
-
-    # Create a figure and a set of subplots
+    
+    shutil.move("volcano.png", "result/plot/volcano.png")
+    if os.path.exists("volcano.png"):
+        os.remove("volcano.png")
+    
+    # Create a figure and a set of subplots with specified size
     fig, ax = plt.subplots()
-
     # Display the image
     ax.imshow(img)
-
     # Remove the axis
     ax.axis('off')
-
     # Show the figure
     plt.show()
 
-    # return gene_exp
 
 
 
-def plot_ts_clusters(result, processed_gene, palette_name='Paired'):
+
+# ********************** Time Series Clusters **********************
+# Plot each line, and put them in the same figure (for each Cluster)
+def plot_ts_clusters(result, processed_gene, palette_name='crest', save_fig=False):
     result = result[['Name', 'Cluster']]
     data = merge_dataframes([result, processed_gene])
 
     # Drop the 'Name' column
     data = data.drop(columns=['Name'])
 
     # Reset index, group by 'Cluster', and set the index back
@@ -770,90 +1179,89 @@
     palette = sns.color_palette(palette_name, 12)  # The palette_name palette has maximum 12 distinct colors
 
     # Iterate over groups (clusters) and plot each one
     for name, group in grouped:
         group = group.set_index('index')  # set the index back to 'index'
         group = group.drop(columns='Cluster')  # drop the 'Cluster' column
 
-        plt.figure(figsize=(10, 6))
+        plt.figure(figsize=(10, 3))
         for i, feature in enumerate(group.index):
             plt.plot(group.columns, group.loc[feature], color=palette[i % len(palette)])
 
         plt.xlabel('Time')
         plt.ylabel('Value')
         plt.title(f'Cluster: {name}', weight='bold')
-        plt.show()
+        # plt.savefig('result/plot/ts_cluster.png')
+        # plt.show()
+
+        if save_fig:
+            # Save the figure with a unique filename for each cluster
+            plt.savefig(f"result/plot/ts_cluster_{name}.png")
+        else:
+            plt.show()
 
 
+def plot_ts_clusters_average(result, processed_gene, palette_name='Paired', save_fig=None):
+    """
+    Plot each line, and put them in the same figure (for each Cluster)
+    
+    Parameters:
+        result: the result dataframe including the 'Name' and 'Cluster' columns
+        processed_gene: the dataframe (with the 'Name' column) to plot
+    
+    result: the result dataframe from the clustering algorithm
+    """
+    data = merge_dataframes([result, processed_gene])
+
+    # Drop the 'Name' column
+    data = data.drop(columns=['Name'])
 
-# PCA
-def plot_pca(gene, design, n_clusters):
-    # transpose your DataFrame, as PCA works on the features (columns), not on the samples (rows)
-    gene_transposed = gene.T
-
-    # Perform PCA on your data
-    pca = PCA(n_components=2)  # here we ask for the first two principal components
-    pca_result = pca.fit_transform(gene_transposed)
-
-    # convert the PCA result to a DataFrame
-    pca_df = pd.DataFrame(data=pca_result, columns=['PC1', 'PC2'])
-
-    # add a 'sample' column
-    pca_df['sample'] = gene_transposed.index
-
-    # get group information from the design dataframe
-    pca_df = pca_df.merge(design[['group']], left_on='sample', right_index=True)
-
-    if n_clusters:
-        # Perform K-means clustering
-        kmeans = KMeans(n_clusters=n_clusters, random_state=0).fit(pca_df[['PC1', 'PC2']])
-        pca_df['Cluster'] = kmeans.labels_
-
-        # create the figure and axis objects
-        fig, ax = plt.subplots(figsize=(8, 6))
-
-        # plot the points on the scatterplot
-        scatter = sns.scatterplot(x="PC1", y="PC2", hue="group", data=pca_df, palette="Paired", s=100, alpha=0.7, ax=ax)
-
-        # for each cluster, add a circle at the mean coordinates with radius proportional to the standard deviation
-        for cluster in set(kmeans.labels_):
-            cluster_points = pca_df[pca_df['Cluster'] == cluster][['PC1', 'PC2']]
-            # calculate mean and standard deviation for the cluster
-            cluster_mean = cluster_points.mean().values
-            cluster_std = cluster_points.std().values
-            # add a circle at the mean coordinates with radius=stddev
-            circle = Circle(cluster_mean, np.linalg.norm(cluster_std), alpha=0.1)
-            ax.add_artist(circle)
+    # Reset index, group by 'Cluster', and set the index back
+    data = data.reset_index()
+    grouped = data.groupby('Cluster')
 
-        # hide the legend
-        ax.get_legend().remove()
-    else:
-        # create the figure and axis objects
-        fig, ax = plt.subplots(figsize=(8, 6))
+    # Set color palette
+    palette = sns.color_palette(palette_name, 12)  # The palette_name palette has maximum 12 distinct colors
 
-        # plot the points on the scatterplot without clustering
-        scatter = sns.scatterplot(x="PC1", y="PC2", hue="group", data=pca_df, palette="Paired", s=100, alpha=0.7, ax=ax)
+    # Iterate over groups (clusters) and plot each one
+    for name, group in grouped:
+        group = group.set_index('index')  # set the index back to 'index'
+        group = group.drop(columns='Cluster')  # drop the 'Cluster' column
 
-        # hide the legend
-        ax.get_legend().remove()
+        # Convert the group dataframe to long form
+        long_form = pd.melt(group.reset_index(), id_vars='index')
 
-    # annotate points on the graph with the sample names
-    for i, sample in enumerate(pca_df['sample']):
-        plt.annotate(sample, (pca_df.iloc[i].PC1, pca_df.iloc[i].PC2), color='gray')
-
-    plt.xlabel('PC1')
-    plt.ylabel('PC2')
-    plt.title('PCA with K-means clustering', fontweight='bold')
+        plt.figure(figsize=(20, 8))
+        
+        # Use seaborn lineplot to plot each line (gene) and the average line with 95% CI
+        sns.lineplot(x='variable', y='value', data=long_form, color=palette[int(name) % len(palette)], ci=95)
 
-    plt.show()
+        plt.xlabel('Time')
+        plt.ylabel('Value')
+        plt.title(f'Cluster: {name}', weight='bold')
+        
+        if save_fig:
+            # Save the figure with a unique filename for each cluster
+            plt.savefig(f"result/plot/ts_cluster_{name}.png")
+        else:
+            plt.show()
 
 
 
 
-def plot_network(data, target_index, num_nodes):
+# ******************* Network ***********************
+def plot_network(data, target_index, num_nodes=20, save_path=None):
+    """
+    Plot the network graph of the top num_nodes similar nodes for the target.
+    
+    Parameters:
+        data: the dataframe containing the similarity data
+        target_index: the index of the target node
+        num_nodes: the number of nodes to plot
+    """
     # Compute the similarity
     similarity = cosine_similarity(data)
     similarity_df = pd.DataFrame(similarity, index=data.index, columns=data.index)
     
     # Get the top num_nodes similar nodes for the target
     target_similarities = similarity_df.loc[target_index].sort_values(ascending=False)[1:num_nodes+1].to_dict()
 
@@ -861,40 +1269,204 @@
     G = nx.Graph()
 
     # Add nodes and edges
     for node, similarity in target_similarities.items():
         G.add_edge(target_index, node, weight=similarity)
     
     # Draw the network
-    plt.figure(figsize=(8,8))
+    plt.figure(figsize=(10,8))
     pos = nx.spring_layout(G)
     colors = ['red' if node == target_index else 'moccasin' for node in G.nodes()]
     
     nx.draw_networkx_nodes(G, pos, node_color=colors)
     nx.draw_networkx_labels(G, pos, font_size=8)
     nx.draw_networkx_edges(G, pos, edge_color='gray', width=[G[u][v]['weight'] for u,v in G.edges()], alpha=0.7)
 
-    plt.title(f'Top {num_nodes} similar nodes to the target', fontsize=10)
+    # plt.title(f'Top {num_nodes} similar features to the target', fontsize=10)
     plt.axis('off')  # to turn off the frame
+    
+    if save_path:
+        plt.savefig(save_path)
+        
+    else:
+        plt.show()
+        
+    plt.show()
+
+
+
+
+# Hexbin
+def plot_hexbin(data, x_axis, y_axis, gridsize=20, save_path=None):
+    """
+    Plot a hexbin plot of the specified columns in the input dataframe.
+    
+    Parameters:
+        data (pandas.DataFrame): The input dataframe.
+        x_axis (str): The name of the column to plot on the x-axis.
+        y_axis (str): The name of the column to plot on the y-axis.
+    """
+    sns.jointplot(x=x_axis, y=y_axis, data=data, kind='hex', gridsize=20)
+    plt.xlabel(x_axis)
+    plt.ylabel(y_axis)
+    plt.show()
+    
+    if save_path:
+        plt.savefig(save_path)
+    else:
+        plt.show()
+    return plt
+
+
+
+# Line Heatmap
+def plot_line_heatmap(df, name_value, cmap='vlag'):  
+    """
+    Plot a line plot and a heatmap of the specified row in the input dataframe.
+    Heatmap includes all columns except 'Name'.
+    
+    Parameters:
+        df (pandas.DataFrame): The input dataframe.
+        name_value (str): The value in the 'Name' column of the row to plot.
+        cmap (str): The name of the colormap to use for the heatmap. Defaults to 'vlag'.
+    """
+    # Find the row where 'Name' is equal to name_value
+    row = df.loc[df['Name'] == name_value]
+
+    # Extract the desired columns and convert them to a list
+    desired_columns = ['Granger', 'log2FoldChange', 'Pearson', 'Spearman']
+    list1 = row[desired_columns].values.tolist()[0]
+
+    # Get the other columns by dropping the ones already in list1
+    remaining_columns = df.drop(columns=['Name'] + desired_columns)
+    list2 = remaining_columns.loc[remaining_columns.index == row.index[0]].values.tolist()[0]
+
+    # Reshape list1 into a 2D array for the heatmap
+    list1_2d = np.array(list1).reshape(-1, 1)
+
+    # Create subplots with adjusted sizes
+    fig = plt.figure(figsize=(10, 2))
+    grid = plt.GridSpec(1, 10, hspace=0.2, wspace=0.2)  # We'll use 8 columns in total
+
+    # Plot the line graph on the left (using 7 out of 8 columns)
+    ax1 = plt.subplot(grid[:9])  # equivalent to grid[0, :7]
+    ax1.plot(list2, color='navy')
+    ax1.set_title(name_value)
+    ax1.set_xticks(range(len(remaining_columns.columns)))
+    ax1.set_xticklabels(remaining_columns.columns, rotation=90)
+
+    # Plot the heatmap on the right (using 1 out of 8 columns) without color bar
+    ax2 = plt.subplot(grid[9:])  # equivalent to grid[0, 7:]
+    sns.heatmap(list1_2d, ax=ax2, cmap=cmap, cbar=False, yticklabels=desired_columns)
+    ax2.yaxis.tick_right()
+    ax2.xaxis.set_visible(False)  # hide the x-axis
+    ax2.set_yticklabels(ax2.get_yticklabels(), rotation=0)  # set rotation to 0
+
+    # Show the plotc
+    plt.tight_layout()
     plt.show()
 
 
+# ***************************  Temporarily Unavailable  *******************************
+# # Line Heatmap for all data
+# def plot_data(df, name_value, ax1, ax2, cmap='vlag'):
+#     """
+#     plot the line graph and heatmap for the given gene name
+    
+#     df: dataframe
+#     name_value: the name of the gene
+#     ax1: the axis for the line graph, ax1 = plt.subplot(grid[:9])
+#     ax2: the axis for the heatmap, ax2 = plt.subplot(grid[9:])
+#     cmap: the color map for the heatmap
+#     """
+#     # Find the row where 'Name' is equal to name_value
+#     row = df.loc[df['Name'] == name_value]
+
+#     # Extract the desired columns and convert them to a list
+#     desired_columns = ['Granger', 'log2FoldChange', 'Pearson', 'Spearman']
+#     list1 = row[desired_columns].values.tolist()[0]
+
+#     # Get the other columns by dropping the ones already in list1
+#     remaining_columns = df.drop(columns=['Name'] + desired_columns)
+#     list2 = remaining_columns.loc[remaining_columns.index == row.index[0]].values.tolist()[0]
+
+#     # Reshape list1 into a 2D array for the heatmap
+#     list1_2d = np.array(list1).reshape(-1, 1)
+
+#     # Plot the line graph on the left 
+#     ax1.plot(list2, color='navy')
+#     ax1.set_title(name_value)
+#     ax1.set_xticks(range(len(remaining_columns.columns)))
+#     ax1.set_xticklabels(remaining_columns.columns, rotation=90)
+
+#     # Plot the heatmap on the right without color bar
+#     sns.heatmap(list1_2d, ax=ax2, cmap=cmap, cbar=False, yticklabels=desired_columns)
+#     ax2.yaxis.tick_right()
+#     ax2.xaxis.set_visible(False)  # hide the x-axis
+#     ax2.set_yticklabels(ax2.get_yticklabels(), rotation=0)  # set rotation to 0
+
+
+# def plot_all_data(df):
+#     """
+#     plot the line graph and heatmap for the top 10 genes in the dataframe
+#     """
+#     df = df.head(10)
+#     num_rows = df.shape[0]
+#     fig = plt.figure(figsize=(10, num_rows * 2))  # adjust the figure height based on the number of rows
+#     grid = plt.GridSpec(num_rows, 10, hspace=0.5, wspace=0.2)
+
+#     for i, row in df.iterrows():
+#         ax1 = plt.subplot(grid[i, :9])  # line graph
+#         ax2 = plt.subplot(grid[i, 9:])  # heatmap
+#         plot_data(df, row['Name'], ax1, ax2)
+        
+#         # Hide the x labels except for the last line plot
+#         if i < num_rows - 1:
+#             ax1.set_xticklabels([]) 
+#         else:
+#             ax1.set_xticklabels(ax1.get_xticklabels(), rotation=90)
+
+#     plt.tight_layout()
+#     plt.show()
+# ***************************  Temporarily Unavailable  *******************************
+
+
+
+
+
+
+
+
 
 
 
 
 
 
 # AI
 def Yuanfang(df, target):
+    """
+    Use OpenAI's API to generate a question for the user to answer.
+    Question: Which one may be involved in the synthesis of target?
+    
+    Parameters:
+        df: the dataframe containing the similarity data
+        target: the target node
+    """
     # annotation = read_upload(annotation_file)
     # df = merge_dataframes([df, annotation])
     df = df.head(20)
     
-    hits = df['Description'].to_list()
+    #if 'Description' in df.columns, is 'Descripton is not in df.columns, then use 'Name'
+    if 'Description' in df.columns:
+        hits = df['Description'].to_list()
+    else:
+        hits = df['Name'].to_list()
+    # hits = df['Description'].to_list()
+    
     hits = [str(item) for item in hits]
     hits = ', '.join(hits)
     
     q = hits + '\n\n\nWhich one may be involved in the synthesis of ' + target + '?'
     
     openai_api_key = getpass.getpass("Please enter your OpenAI API Key: ")
     openai.api_key = openai_api_key
@@ -911,36 +1483,53 @@
         messages = messages
     )
     
     print(' ')
     print(completion.choices[0].message.content)
     print(' ')
     print(' ')
-    print('NOTICE: The output is generated by GPT 3.5 turbo, which is a large language model, so the statement can only be treated as a inspiration.')
+    print('NOTICE: The output was produced by the large language model GPT 3.5 turbo, so it should only be regarded as a source of inspiration.')
+
+
+
+
+
 
 
 
 
 
 
 
 
 
-# ************* Pipeline *************
-def pipeline(gene_file, metabo_file, design_file, annotation_file, target, cluster_count, aggregation_func=None):
+"""
+#  ██████╗ █████╗ ████████╗    ██████╗ ██████╗ ██╗██████╗  ██████╗ ███████╗
+# ██╔════╝██╔══██╗╚══██╔══╝    ██╔══██╗██╔══██╗██║██╔══██╗██╔════╝ ██╔════╝
+# ██║     ███████║   ██║       ██████╔╝██████╔╝██║██║  ██║██║  ███╗█████╗  
+# ██║     ██╔══██║   ██║       ██╔══██╗██╔══██╗██║██║  ██║██║   ██║██╔══╝  
+# ╚██████╗██║  ██║   ██║       ██████╔╝██║  ██║██║██████╔╝╚██████╔╝███████╗
+#  ╚═════╝╚═╝  ╚═╝   ╚═╝       ╚═════╝ ╚═╝  ╚═╝╚═╝╚═════╝  ╚═════╝ ╚══════╝
+"""
+
+
+
+# ******************* Pipeline ***********************
+def pipeline(gene_file, metabo_file, design_file, annotation_file, target, cluster_count, max_lag=1, aggregation_func=None):
     """
     This function processes gene expression data, performs computations, and returns results.
 
     Parameters:
     - gene_file (str): The filename of the gene count data.
     - metabo_file (str): The filename of the metabolome data.
     - design_file (str): The filename of the experimental design data (can be None).
     - annotation_file (str): The filename of the gene annotation data (can be None).
     - target (str): The target metabolite for the analysis.
     - cluster_count (int): The number of clusters for time series clustering.
+    - max_lag (int): The maximum number of lags for Granger causality test (default is 1).
     - aggregation_func (function): The function to be used for data aggregation.
 
     Returns:
     - result (pd.DataFrame): A pandas DataFrame containing the processed results, with annotations and clustering information if provided.
     """
     # Read data
     gene = read_upload(gene_file)
@@ -954,30 +1543,30 @@
         processed_gene = aggregation_func(gene, design)
         processed_metabo = aggregation_func(metabo, design)
 
         # Get target data
         t = get_target(target, processed_metabo)
 
         # Compute Granger causality
-        granger = compute_granger(processed_gene, t, 1)
+        granger = compute_granger(processed_gene, t, max_lag)
 
         # Prepare dataframe for fold change calculation
         df_for_fc(processed_metabo, target, gene, design)
 
         # Compute fold change
         fc = fc_comp()
 
         # Merge data
         data = merge_dataframes([granger, fc])
 
     else:
         # If there is no design file
         t = get_target(target, metabo)
         noontide = find_noontide(metabo, target)
-        granger = compute_granger(gene, t)
+        granger = compute_granger(gene, t, max_lag)
 
         # Compute fold change
         fc = no_repeat_fc(gene, noontide)
         data = merge_dataframes([granger, fc])
         
     # Compute score
     result = score(data)
@@ -997,26 +1586,14 @@
     result.set_index('Rank', inplace=True)
 
     return result
 
 
 
 
-
-# print('''
-      
-      
-#  ██████╗ █████╗ ████████╗    ██████╗ ██████╗ ██╗██████╗  ██████╗ ███████╗
-# ██╔════╝██╔══██╗╚══██╔══╝    ██╔══██╗██╔══██╗██║██╔══██╗██╔════╝ ██╔════╝
-# ██║     ███████║   ██║       ██████╔╝██████╔╝██║██║  ██║██║  ███╗█████╗  
-# ██║     ██╔══██║   ██║       ██╔══██╗██╔══██╗██║██║  ██║██║   ██║██╔══╝  
-# ╚██████╗██║  ██║   ██║       ██████╔╝██║  ██║██║██████╔╝╚██████╔╝███████╗
-#  ╚═════╝╚═╝  ╚═╝   ╚═╝       ╚═════╝ ╚═╝  ╚═╝╚═╝╚═════╝  ╚═════╝ ╚══════╝
-# ''')
-# print(r'''
 #                                    ___
 #                       |\---/|  / )|Guo|
 #           ------------;     |-/ / |Lab|
 #                       )     (' /  `---'
 #           ===========(       ,'==========
 #           ||  _      |      |      
 #           || ( (    /       ;
@@ -1024,17 +1601,7 @@
 #           ||   `._        /|
 #           ||      |\    _/||
 #         __||_____.' )  |__||____________
 #          ________\  |  |_________________
 #                   \ \  `-.
 #                    `-`---'  
                    
-
-
-
-# CAT Bridge is a Python-based, cross-platform tool designed for integrated analysis of transcriptomes and metabolites. It is adept at processing time series data, aiding in the discovery of genes contributing to specific metabolite synthesis. 
-
-# For more information on our other research outputs, welcome to visit the Guo Lab's website at: http://www.guo-lab.site.
-
-# For any queries about this software, feel free to contact us at by8@ualberta.ca.
-
-# ''')
```

### Comparing `catbridge-0.4/catbridge.egg-info/PKG-INFO` & `catbridge-0.5/catbridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catbridge
-Version: 0.4
+Version: 0.5
 Summary: CAT Bridge (Compounds And Transcripts Bridge) is a robust tool built with the goal of uncovering biosynthetic mechanisms in multi-omics data, such as identifying genes potentially involved in compound synthesis by incorporating metabolomics and transcriptomics data.
 Home-page: https://github.com/Bowen999/catbridge
 Author: Bowen Yang
 Author-email: by172@georgetown.edu
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `catbridge-0.4/setup.py` & `catbridge-0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="catbridge",
-    version="0.4",
+    version="0.5",
     packages=find_packages(),
 
     # Metadata
     author="Bowen Yang",
     author_email="by172@georgetown.edu",
     description="CAT Bridge (Compounds And Transcripts Bridge) is a robust tool built with the goal of uncovering biosynthetic mechanisms in multi-omics data, such as identifying genes potentially involved in compound synthesis by incorporating metabolomics and transcriptomics data.",
     long_description=open('README.md').read(),
```

