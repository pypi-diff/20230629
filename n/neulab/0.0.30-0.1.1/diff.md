# Comparing `tmp/neulab-0.0.30-py3-none-any.whl.zip` & `tmp/neulab-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,21 @@
-Zip file size: 9526 bytes, number of entries: 11
+Zip file size: 19470 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 22-Apr-28 12:23 neulab/__init__.py
--rw-r--r--  2.0 unx    10293 b- defN 23-Feb-22 15:09 neulab/clusters.py
--rw-r--r--  2.0 unx     3712 b- defN 23-Feb-21 20:54 neulab/discover.py
--rw-r--r--  2.0 unx     1123 b- defN 23-Feb-21 23:24 neulab/normalization.py
--rw-r--r--  2.0 unx     5893 b- defN 23-Feb-22 01:09 neulab/outliers.py
--rw-r--r--  2.0 unx     8076 b- defN 23-Feb-21 21:05 neulab/recover.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Feb-22 18:00 neulab-0.0.30.dist-info/LICENSE
--rw-r--r--  2.0 unx      786 b- defN 23-Feb-22 18:00 neulab-0.0.30.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-22 18:00 neulab-0.0.30.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Feb-22 18:00 neulab-0.0.30.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      836 b- defN 23-Feb-22 18:00 neulab-0.0.30.dist-info/RECORD
-11 files, 31890 bytes uncompressed, 8126 bytes compressed:  74.5%
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 11:18 neulab/Dataframe/__init__.py
+-rw-r--r--  2.0 unx      348 b- defN 23-Jun-29 10:52 neulab/Dataframe/clusters.py
+-rw-r--r--  2.0 unx    15117 b- defN 23-Jun-29 10:52 neulab/Dataframe/discover.py
+-rw-r--r--  2.0 unx    10039 b- defN 23-Feb-26 16:50 neulab/Dataframe/importance.py
+-rw-r--r--  2.0 unx     3172 b- defN 23-Feb-26 16:49 neulab/Dataframe/normalization.py
+-rw-r--r--  2.0 unx     8272 b- defN 23-Jun-29 10:52 neulab/Dataframe/outliers.py
+-rw-r--r--  2.0 unx     5118 b- defN 23-Jun-29 10:52 neulab/Dataframe/recover.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 11:18 neulab/Vector/__init__.py
+-rw-r--r--  2.0 unx    10887 b- defN 23-Jun-29 00:35 neulab/Vector/clusters.py
+-rw-r--r--  2.0 unx     3712 b- defN 23-Feb-21 20:54 neulab/Vector/discover.py
+-rw-r--r--  2.0 unx     1123 b- defN 23-Feb-21 23:24 neulab/Vector/normalization.py
+-rw-r--r--  2.0 unx     6946 b- defN 23-Jun-29 10:52 neulab/Vector/outliers.py
+-rw-r--r--  2.0 unx     8676 b- defN 23-Jun-29 10:52 neulab/Vector/recover.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jun-29 11:06 neulab-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      877 b- defN 23-Jun-29 11:06 neulab-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 11:06 neulab-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-29 11:06 neulab-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1544 b- defN 23-Jun-29 11:06 neulab-0.1.1.dist-info/RECORD
+19 files, 77002 bytes uncompressed, 16948 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -1,34 +1,58 @@
 Filename: neulab/__init__.py
 Comment: 
 
-Filename: neulab/clusters.py
+Filename: neulab/Dataframe/__init__.py
 Comment: 
 
-Filename: neulab/discover.py
+Filename: neulab/Dataframe/clusters.py
 Comment: 
 
-Filename: neulab/normalization.py
+Filename: neulab/Dataframe/discover.py
 Comment: 
 
-Filename: neulab/outliers.py
+Filename: neulab/Dataframe/importance.py
 Comment: 
 
-Filename: neulab/recover.py
+Filename: neulab/Dataframe/normalization.py
 Comment: 
 
-Filename: neulab-0.0.30.dist-info/LICENSE
+Filename: neulab/Dataframe/outliers.py
 Comment: 
 
-Filename: neulab-0.0.30.dist-info/METADATA
+Filename: neulab/Dataframe/recover.py
 Comment: 
 
-Filename: neulab-0.0.30.dist-info/WHEEL
+Filename: neulab/Vector/__init__.py
 Comment: 
 
-Filename: neulab-0.0.30.dist-info/top_level.txt
+Filename: neulab/Vector/clusters.py
 Comment: 
 
-Filename: neulab-0.0.30.dist-info/RECORD
+Filename: neulab/Vector/discover.py
+Comment: 
+
+Filename: neulab/Vector/normalization.py
+Comment: 
+
+Filename: neulab/Vector/outliers.py
+Comment: 
+
+Filename: neulab/Vector/recover.py
+Comment: 
+
+Filename: neulab-0.1.1.dist-info/LICENSE
+Comment: 
+
+Filename: neulab-0.1.1.dist-info/METADATA
+Comment: 
+
+Filename: neulab-0.1.1.dist-info/WHEEL
+Comment: 
+
+Filename: neulab-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: neulab-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `neulab/clusters.py` & `neulab/Vector/clusters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-import networkx as nx
-import numpy as np
-import matplotlib.pyplot as plt
-import math
-import random
 
 def graph_clusterize(vectors, metric='euclidean', threshold=None, draw=False, figsize=(10, 10)):
     """
     Clusters input vectors using Graph algorithm in NetworkX.
     Parameters:
         - vectors: list of input vectors to be clustered
         - metric: distance metric to be used (default is Euclidean distance)
         - threshold: distance threshold for considering two vectors to be in the same cluster
         - draw: plot results if True
         - figsize: plot size
     Returns:
         - clusters: a list of clusters, where each cluster is a list of vector indices
     """
+
+    import numpy as np
+    import matplotlib.pyplot as plt
+    import networkx as nx
+
+    if not isinstance(vectors, np.ndarray):
+        vectors = np.array(vectors)
+
     # Compute pairwise distances between vectors
     dist_matrix = np.zeros((len(vectors), len(vectors)))
     for i in range(len(vectors)):
         for j in range(i+1, len(vectors)):
             if metric == 'euclidean':
                 dist = np.linalg.norm(vectors[i] - vectors[j])
             elif metric == 'cosine':
@@ -80,14 +83,23 @@
         - num_clusters: number of clusters to form
         - metric: distance metric to be used (default is Euclidean distance)
         - draw: plot results if True
         - figsize: plot size
     Returns:
         - clusters: a list of clusters, where each cluster is a list of vector indices
     """
+    import numpy as np
+
+    if not isinstance(vectors, np.ndarray):
+        vectors = np.array(vectors)
+
+    import numpy as np
+    import matplotlib.pyplot as plt
+    import networkx as nx
+
     # Compute pairwise distances between vectors
     dist_matrix = np.zeros((len(vectors), len(vectors)))
     for i in range(len(vectors)):
         for j in range(i+1, len(vectors)):
             if metric == 'euclidean':
                 dist = np.linalg.norm(vectors[i] - vectors[j])
             elif metric == 'cosine':
@@ -146,14 +158,22 @@
         - vectors: list of input vectors to be clustered
         - radius: distance of an existing centroid, the vector is assigned to the closest cluster.
         - draw: plot results if True
         - figsize: plot size
     Returns:
         - clusters: a list of clusters, where each cluster is a list of vector indices
     """
+
+    import math
+    import numpy as np
+    import matplotlib.pyplot as plt
+
+    if not isinstance(vectors, np.ndarray):
+        vectors = np.array(vectors)
+
     def distance(a, b):
         return math.sqrt(sum((a[i] - b[i])**2 for i in range(len(a))))
     
     def plot_clusters(vectors, centroids, clusters, radius):
         colors = ['r', 'g', 'b', 'c', 'm', 'y', 'k']
         fig, ax = plt.subplots(figsize=(8, 8))
         for i in range(len(clusters)):
@@ -198,14 +218,23 @@
         - num_clusters: number of clusters to create
         - max_iterations: maximum number of iterations for convergence
         - draw: plot results if True
         - figsize: plot size
     Returns:
         - clusters: a list of clusters, where each cluster is a list of vector indices
     """
+
+    import numpy as np
+    import random
+    import math
+    import matplotlib.pyplot as plt
+
+    if not isinstance(vectors, np.ndarray):
+        vectors = np.array(vectors)
+
     def distance(a, b):
         return math.sqrt(sum((a[i] - b[i])**2 for i in range(len(a))))
 
     def plot_clusters(vectors, centroids, clusters):
         fig, ax = plt.subplots(figsize=(8, 8))
         colors = ['r', 'g', 'b', 'c', 'm', 'y', 'k']
         for i, c in enumerate(clusters):
```

## Comparing `neulab/discover.py` & `neulab/Vector/discover.py`

 * *Files identical despite different names*

## Comparing `neulab/normalization.py` & `neulab/Vector/normalization.py`

 * *Files identical despite different names*

## Comparing `neulab/outliers.py` & `neulab/Vector/outliers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,53 @@
-from neulab.discover import std_deviation
-import numpy as np
-import warnings
-from scipy.special import erfc
 
-def zscore_outliers(*vectors):
+def zscore_outliers(*vectors, method='mean', threshold=3):
     """
     Z-score algorithm to remove outliers.
 
+    This function uses the Z-score algorithm to remove outliers from a variable-length list of vectors.
+
     Parameters:
-        *vectors: variable-length list of vectors, each represented as a list of numbers.
+        *vectors (list of lists): A variable-length list of vectors, each represented as a list of numbers.
+        method (str): Specifies the method used to calculate the Z-score. Acceptable values are 'mean' or 'median'.
+        threshold (int or float): The threshold for identifying outliers. Values greater than threshold times the standard deviation from the mean (or median) will be considered outliers.
 
     Returns:
         A tuple containing two lists:
             - A list of cleared vectors, where outliers have been removed.
             - A list of the dropped outliers.
     """
+
+    from neulab.Vector.discover import std_deviation
+    import numpy as np
+    import warnings
+
+    if method not in ['mean', 'median']:
+        raise ValueError('Invalid method specified.')
+
     cleared_vectors = []
     outliers = []
     for vector in vectors:
         # Convert the list to a numpy array
         vector = np.array(vector)
 
         if vector.shape[0] < 11:
-            warnings.warn(f'The z-score algorithm may not perform well on small vectors. Recommended minimum vector length is 11, recieved: {vector.shape[0]}')
+            warnings.warn(f'The z-score algorithm may not perform well on small vectors. Recommended minimum vector length is 11, received: {vector.shape[0]}')
 
-        # Calculate the mean and standard deviation of the vector
-        mean = np.mean(vector)
-        std = std_deviation(vector)
+        # Calculate the median and median absolute deviation of the vector
+        if method == 'median':
+            # Calculate z-score
+            z_score = np.abs((vector - np.median(vector)) / std_deviation(vector))
+            # Identify outliers using a threshold of standard deviations from the median
+            is_outlier = z_score > threshold
+        elif method == 'mean':
+            # Calculate z-score
+            z_score = np.abs((vector - np.mean(vector)) / std_deviation(vector))
+            # Identify outliers using a threshold times of standard deviations from the mean
+            is_outlier = z_score > threshold
 
-        # Find the outliers (values > 3 standard deviations from the mean)
-        is_outlier = np.abs(vector - mean) > 3 * std
         if np.any(is_outlier):
             # Add the outliers to the list
             outliers.extend(list(vector[is_outlier]))
 
             # Remove the outliers from the vector
             not_outlier_indices = np.where(~is_outlier)[0]
             vector = vector[not_outlier_indices]
@@ -51,14 +65,18 @@
 
     Returns:
         A tuple containing two lists:
             - A list of cleared vectors, where outliers have been removed.
             - A list of the dropped outliers.
     """
 
+    from neulab.Vector.discover import std_deviation
+    from scipy.special import erfc
+    import numpy as np
+
     cleared_vectors = []
     outliers = []
     for vector in vectors:
         # Convert the list to a numpy array
         vector = np.array(vector)
 
         mean = np.mean(vector)
@@ -97,14 +115,16 @@
 
     Returns:
         A tuple containing two lists:
             - A list of cleared vectors, where outliers have been removed.
             - A list of the dropped outliers.
     """
 
+    import numpy as np
+
     cleared_vectors = []
     outliers = []
     for vector in vectors:
         # Convert the list to a numpy array
         vector = np.array(vector).flatten()
 
         # Calculate the first and third quartiles of the data
```

## Comparing `neulab/recover.py` & `neulab/Vector/recover.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,217 +1,240 @@
 import numpy as np
-from neulab.discover import correlation_coefficient
-from neulab.discover import euclidean_distance
-from neulab.discover import manhattan_distance
-from neulab.discover import max_distance
 
 def replace_missing_with_mean(*vectors):
     """
     Replace missing value with mean. Returns the new vector and the mean value.
 
     Parameters:
-        vector (array-like): The input vector.
+        vectors (array-like): One or more input vectors.
 
     Returns:
-        tuple: A tuple containing the new vector with missing values replaced by the mean and the mean value.
+        tuple: A tuple containing the new vectors with missing values replaced by the mean and the mean value.
     """
 
-    # Combine the input vectors into a single 2D array
-    if len(vectors) > 1:
-        vector = np.vstack(vectors)
-    else:
-        vector = np.array(vectors)[0]
+    new_vectors = []
+    mean_values = []
 
-    missing_values = np.isnan(vector)
-    num_missing_values = np.count_nonzero(missing_values)
-    if num_missing_values == len(vector):
-        raise ValueError("All values in vector are missing.")
-    if num_missing_values == 0:
-        return vector, vector.mean()
-    mean_value = vector[~missing_values].mean()
-    new_vector = vector.copy()
-    new_vector[missing_values] = mean_value
-    return new_vector, mean_value
+    for vector in np.array(vectors):
+        missing_values = np.isnan(vector)
+        num_missing_values = np.count_nonzero(missing_values)
+        if num_missing_values == len(vector):
+            raise ValueError("All values in vector are missing.")
+        if num_missing_values == 0:
+            new_vectors.append(vector)
+            mean_values.append(vector.mean())
+            continue
+        
+        mean_value = np.mean(vector[~missing_values])
+        new_vector = vector.copy()
+        new_vector[missing_values] = mean_value
+        new_vectors.append(new_vector)
+        mean_values.append(mean_value)
+
+    if len(new_vectors) == 1:
+        return new_vectors[0], mean_values[0]
+    else:
+        return new_vectors, mean_values
 
 
 def replace_missing_with_median(*vectors):
     """
     Replace missing value with median. Returns the new vector and the median value.
 
     Parameters:
         vector (array-like): The input vector.
 
     Returns:
         tuple: A tuple containing the new vector with missing values replaced by the median and the median value.
     """
 
-    # Combine the input vectors into a single 2D array
-    if len(vectors) > 1:
-        vector = np.vstack(vectors)
-    else:
-        vector = np.array(vectors)[0]
+    new_vectors = []
+    median_values = []
 
-    missing_values = np.isnan(vector)
-    num_missing_values = np.count_nonzero(missing_values)
-    if num_missing_values == len(vector):
-        raise ValueError("All values in vector are missing.")
-    if num_missing_values == 0:
-        return vector, np.median(vector)
-    median_value = np.median(vector[~missing_values])
-    vector[missing_values] = median_value
-    return vector, median_value
+    for vector in np.array(vectors):
+
+        missing_values = np.isnan(vector)
+        num_missing_values = np.count_nonzero(missing_values)
+        if num_missing_values == len(vector):
+            raise ValueError("All values in vector are missing.")
+        if num_missing_values == 0:
+            new_vectors.append(vector)
+            median_values.append(np.median(vector))
+            continue
+
+        median_value = np.median(vector[~missing_values])
+        new_vector = vector.copy()
+        new_vector[missing_values] = median_value
+        new_vectors.append(new_vector)
+        median_values.append(median_value)
+
+    if len(new_vectors) == 1:
+        return new_vectors[0], median_values[0]
+    else:
+        return new_vectors, median_values
 
 
 def replace_missing_with_mode(*vectors):
     """
     Replace missing value with mode. Returns the new vector and the mode value.
 
     Parameters:
-        vector (array-like): The input vector.
+        vectors (array-like): The input vectors.
 
     Returns:
-        tuple: A tuple containing the new vector with missing values replaced by the mode and the mode value.
+        tuple: A tuple containing the new vectors with missing values replaced by the mode and the mode values.
     """
 
-    # Combine the input vectors into a single 2D array
-    if len(vectors) > 1:
-        vector = np.vstack(vectors)
-    else:
-        vector = np.array(vectors)[0]
+    import numpy as np
 
-    missing_values = np.isnan(vector)
-    num_missing_values = np.count_nonzero(missing_values)
-    if num_missing_values == len(vector):
-        raise ValueError("All values in vector are missing.")
-    if num_missing_values == 0:
-        unique, counts = np.unique(vector, return_counts=True)
-        mode_index = np.argmax(counts)
-        mode_value = unique[mode_index]
-        return vector, mode_value
-    unique, counts = np.unique(vector[~missing_values], return_counts=True)
-    if len(unique) == 1:
-        mode_value = unique[0]
+    new_vectors = []
+    mode_values = []
+
+    for vector in np.array(vectors):
+
+        missing_values = np.isnan(vector)
+        num_missing_values = np.count_nonzero(missing_values)
+        if num_missing_values == len(vector):
+            raise ValueError("All values in vector are missing.")
+        if num_missing_values == 0:
+            unique, counts = np.unique(vector, return_counts=True)
+            mode_index = np.argmax(counts)
+            mode_value = unique[mode_index]
+        else:
+            unique, counts = np.unique(vector[~missing_values], return_counts=True)
+            if len(unique) == 1:
+                mode_value = unique[0]
+            else:
+                mode_index = np.argmax(counts)
+                mode_value = unique[mode_index]
+            vector[missing_values] = mode_value
+        new_vectors.append(vector)
+        mode_values.append(mode_value)
+
+    if len(new_vectors) == 1:
+        return new_vectors[0], mode_values[0]
     else:
-        mode_index = np.argmax(counts)
-        mode_value = unique[mode_index]
-    vector[missing_values] = mode_value
-    return vector, mode_value
+        return new_vectors, mode_values
 
 
 def replace_missing_with_corrcoef(*vectors):
     """
     Replace missing values using correlation coefficient. Returns the new vector and the correlation.
 
     Parameters:
         vector (array-like): The input vector.
 
     Returns:
         tuple: A tuple containing the new vector with missing values replaced by values calculated with correlation coefficient and the correlation coefficient value.
     """
 
-    # Combine the input vectors into a single 2D array
-    if len(vectors) > 1:
-        vector = np.vstack(vectors)
-    else:
-        vector = np.array(vectors)[0]
+    from neulab.Vector.discover import correlation_coefficient
+
+    recovered_vector = []
+    corr_coefs = []
 
-    missing_values = np.isnan(vector)
+    missing_values = np.isnan(vectors)
     num_missing_values = np.count_nonzero(missing_values)
-    if num_missing_values == len(vector):
-        raise ValueError("All values in vector are missing.")
-        
-    # Assuming that missing values are represented by NaNs
-    missing_mask = np.isnan(vector)
-    missing_indices = np.where(missing_mask)[0]
-    nonmissing_indices = np.where(~missing_mask)[0]
-    
-    if len(missing_indices) == 0:
+    if num_missing_values == 0:
         # If there are no non-missing values, return the input vector and NaN correlation
-        return vector, np.nan
-    
-    # Calculate the correlation coefficient between non-missing values and missing indices
-    corr_coef = correlation_coefficient(nonmissing_indices, vector[nonmissing_indices])[0]
-    
-    if np.isnan(corr_coef):
-        # If the correlation coefficient is NaN, return the input vector and NaN correlation
-        return vector, np.nan
-    
-    # Calculate the new values for missing indices using the correlation coefficient
-    new_values = (missing_indices - nonmissing_indices.mean()) * corr_coef + vector[nonmissing_indices].mean()
-    
-    # Replace the missing values with the new values
-    new_vector = vector.copy()
-    new_vector[missing_mask] = new_values
+        return vectors, np.nan
+
+    for vector in np.array(vectors):
+
+        missing_values = np.isnan(vector)
+        num_missing_values = np.count_nonzero(missing_values)
+        if num_missing_values == len(vector):
+            raise ValueError("All values in vector are missing.")
+            
+        # Assuming that missing values are represented by NaNs
+        missing_mask = np.isnan(vector)
+        missing_indices = np.where(missing_mask)[0]
+        nonmissing_indices = np.where(~missing_mask)[0]
+        
+        # Calculate the correlation coefficient between non-missing values and missing indices
+        corr_coef = correlation_coefficient(nonmissing_indices, vector[nonmissing_indices])[0]
+        
+        if np.isnan(corr_coef):
+            # If the correlation coefficient is NaN, return the input vector and NaN correlation
+            return vector, np.nan
+        
+        # Calculate the new values for missing indices using the correlation coefficient
+        new_values = (missing_indices - nonmissing_indices.mean()) * corr_coef + vector[nonmissing_indices].mean()
+        
+        # Replace the missing values with the new values
+        new_vector = vector.copy()
+        new_vector[missing_mask] = new_values
+
+        recovered_vector.append(new_vector)
+        corr_coefs.append(round(corr_coef, 6))
     
-    return new_vector, round(corr_coef, 6)
+    return recovered_vector, corr_coefs
 
 
-def replace_missing_with_distance(*vectors, metric='euclidean', how='vertical'):
+def replace_missing_with_distance(*vectors, metric='euclidean'):
     """
     Replace missing values using a given distance metric. Returns the new vector and the distance.
-
     Parameters:
         *vectors (array-like): The input vectors.
         metric (str): The distance metric to use. Can be 'euclidean', 'manhattan', or 'max'.
-        how (str): The direction of deleting a missing value.
-            'vertical' - deletes missing values from different columns in each row.
-            'horizontal' - deletes missing values from different rows in each column.
-
     Returns:
         tuple: A tuple containing the new vectors with missing values replaced by values calculated with the given distance metric and the distance.
     """
-    # Combine the input vectors into a single 2D array
-    if len(vectors) > 1:
-        vector_array = np.vstack(vectors)
-    else:
-        vector_array = np.array(vectors)[0]
 
-    vec_arr_copy = vector_array.copy()
+    from neulab.Vector.discover import euclidean_distance
+    from neulab.Vector.discover import manhattan_distance
+    from neulab.Vector.discover import max_distance
+
+    if np.array(vectors).shape[1] == 1:
+        return vectors, np.nan
+    elif np.array(vectors).shape[1] > 1:
+        vectors = np.array(vectors).squeeze()
+
+    for vt in np.array(vectors):
+        # Find the missing values in the input vectors
+        missing_values = np.isnan(vt)
+        num_missing_values = np.count_nonzero(missing_values)
+        if num_missing_values == vt.size:
+            raise ValueError("All values in vectors are missing.")
     
-    # Find the missing values in the input vectors
-    missing_values = np.isnan(vector_array)
+    missing_values = np.isnan(vectors)
     num_missing_values = np.count_nonzero(missing_values)
-    if num_missing_values == vector_array.size:
-        raise ValueError("All values in vectors are missing.")
-    
     if num_missing_values == 0:
         # If there are no non-missing values, return the input vector and NaN correlation
-        return vector_array, np.nan
+        return vectors, np.nan
     
-    if how == 'vertical':
-        vector_array = vector_array.transpose()
-        # Find the rows containing missing values
-        missing_rows = np.any(missing_values, axis=1)
-        # Delete the rows containing missing values
-        vector_array = np.delete(vector_array, np.where(missing_rows), axis=1)
-    elif how == 'horizontal':
-        # Find the columns containing missing values
-        missing_cols = np.any(missing_values, axis=0)
-        # Delete the columns containing missing values
-        vector_array = np.delete(vector_array, np.where(missing_cols), axis=1)
+    vectors = np.array(vectors)
 
     indices = np.where(missing_values)
-        
+
     distances = []
-    for i in range(vector_array.shape[0]-1):
-        if  i != indices:
-            if metric == 'euclidean':
-                distances.append(euclidean_distance(vector_array[i], vector_array[-1])[0])
-            if metric == 'manhattan':
-                distances.append(manhattan_distance(vector_array[i], vector_array[-1])[0])
-            if metric == 'max':
-                distances.append(max_distance(vector_array[i], vector_array[-1])[0])
-
-    # Get row with nan
-    val_list = vec_arr_copy[indices[0][0]]
-    val_list = val_list[~np.isnan(val_list)]
-    
-    DISTANCE = round(1/(sum([1/i for i in distances])) * sum([v/d for v, d in zip(val_list, distances)]), 2)
+    dst = []
+    for i in range(len(vectors)):
+        indices = np.where(np.isnan(vectors[i]))
+        num_missing_values = np.count_nonzero(np.isnan(vectors[i]))
+        if num_missing_values == 0:
+            continue
+        distances = []
+        for j in range(len(vectors)):
+            non_missing_values_i = np.delete(vectors[i], np.where(np.isnan(vectors[i])))
+            non_missing_values_j = np.delete(vectors[j], np.where(np.isnan(vectors[j])))
+            if i != j:
+                v1 = np.where(np.isnan(vectors[i]), np.mean(non_missing_values_i), vectors[i])
+                v2 = np.where(np.isnan(vectors[j]), np.mean(non_missing_values_j), vectors[j])
+                if metric == 'euclidean':
+                    distances.append(euclidean_distance(v1, v2)[0])
+                if metric == 'manhattan':
+                    distances.append(manhattan_distance(v1, v2)[0])
+                if metric == 'max':
+                    distances.append(max_distance(v1, v2)[0])
+
+        val_list = np.delete(vectors[i], np.where(np.isnan(vectors[i])))
+        DISTANCE = round(1 / (sum([1/i for i in distances])) * sum([v/d for v, d in zip(val_list, distances)]), 2)
+        dst.append(DISTANCE)
 
-    # Replace missing values with DISTANCE
-    vec_arr_copy[indices] = DISTANCE
+        for z in indices[0]:
+            vectors[i][z] = DISTANCE
 
     # Transpose the vector array back to its original shape if necessary
-    if how == 'vertical':
-        vector_array = vec_arr_copy.transpose()
+    replaced = np.array(vectors)
     
-    return vec_arr_copy, DISTANCE
+    return replaced, dst
```

## Comparing `neulab-0.0.30.dist-info/LICENSE` & `neulab-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `neulab-0.0.30.dist-info/METADATA` & `neulab-0.1.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: neulab
-Version: 0.0.30
+Version: 0.1.1
 Summary: Tool for data preprocess in ML.
 Home-page: https://github.com/kndahl/neulab
 Author: Roman Fitzjalen
 Author-email: romaactor@gmail.com
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: networkx
 Requires-Dist: matplotlib
+Requires-Dist: jinja2
+Requires-Dist: seaborn
+Requires-Dist: scikit-learn
 
 # neulab
 Tool for data preprocess in ML.
 
 [![Downloads](https://pepy.tech/badge/neulab)](https://pepy.tech/project/neulab)
 # Installation
 ```
 pip install neulab
 ```
 # Description
 The library contains several blocks: data analysis, data recovery methods, data normalization, outlier detection, clustering. A detailed description and instructions can be found on Github: https://github.com/kndahl/neulab
+
```

