# Comparing `tmp/delve-fs-0.1.0.tar.gz` & `tmp/delve-fs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delve-fs-0.1.0.tar", last modified: Wed Jun 28 19:25:55 2023, max compression
+gzip compressed data, was "delve-fs-0.1.1.tar", last modified: Thu Jun 29 20:15:52 2023, max compression
```

## Comparing `delve-fs-0.1.0.tar` & `delve-fs-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jolene     (501) staff       (20)        0 2023-06-28 19:25:55.226177 delve-fs-0.1.0/
--rw-r--r--   0 jolene     (501) staff       (20)     1069 2023-05-13 23:13:36.000000 delve-fs-0.1.0/LICENSE
--rw-r--r--   0 jolene     (501) staff       (20)     4893 2023-06-28 19:25:55.226015 delve-fs-0.1.0/PKG-INFO
--rw-r--r--   0 jolene     (501) staff       (20)     4004 2023-06-28 19:14:36.000000 delve-fs-0.1.0/README.md
-drwxr-xr-x   0 jolene     (501) staff       (20)        0 2023-06-28 19:25:55.225136 delve-fs-0.1.0/delve/
--rw-r--r--   0 jolene     (501) staff       (20)       20 2023-06-28 18:44:57.000000 delve-fs-0.1.0/delve/__init__.py
--rw-r--r--   0 jolene     (501) staff       (20)    21100 2023-06-28 19:18:22.000000 delve-fs-0.1.0/delve/delve.py
-drwxr-xr-x   0 jolene     (501) staff       (20)        0 2023-06-28 19:25:55.225819 delve-fs-0.1.0/delve_fs.egg-info/
--rw-r--r--   0 jolene     (501) staff       (20)     4893 2023-06-28 19:25:55.000000 delve-fs-0.1.0/delve_fs.egg-info/PKG-INFO
--rw-r--r--   0 jolene     (501) staff       (20)      218 2023-06-28 19:25:55.000000 delve-fs-0.1.0/delve_fs.egg-info/SOURCES.txt
--rw-r--r--   0 jolene     (501) staff       (20)        1 2023-06-28 19:25:55.000000 delve-fs-0.1.0/delve_fs.egg-info/dependency_links.txt
--rw-r--r--   0 jolene     (501) staff       (20)      116 2023-06-28 19:25:55.000000 delve-fs-0.1.0/delve_fs.egg-info/requires.txt
--rw-r--r--   0 jolene     (501) staff       (20)        6 2023-06-28 19:25:55.000000 delve-fs-0.1.0/delve_fs.egg-info/top_level.txt
--rw-r--r--   0 jolene     (501) staff       (20)       38 2023-06-28 19:25:55.226250 delve-fs-0.1.0/setup.cfg
--rw-r--r--   0 jolene     (501) staff       (20)     1396 2023-06-28 19:22:58.000000 delve-fs-0.1.0/setup.py
+drwxr-xr-x   0 jolene     (501) staff       (20)        0 2023-06-29 20:15:52.568379 delve-fs-0.1.1/
+-rw-r--r--   0 jolene     (501) staff       (20)     1069 2023-05-13 23:13:36.000000 delve-fs-0.1.1/LICENSE
+-rw-r--r--   0 jolene     (501) staff       (20)     4798 2023-06-29 20:15:52.568244 delve-fs-0.1.1/PKG-INFO
+-rw-r--r--   0 jolene     (501) staff       (20)     3909 2023-06-29 20:00:24.000000 delve-fs-0.1.1/README.md
+drwxr-xr-x   0 jolene     (501) staff       (20)        0 2023-06-29 20:15:52.567153 delve-fs-0.1.1/delve/
+-rw-r--r--   0 jolene     (501) staff       (20)       20 2023-06-28 18:44:57.000000 delve-fs-0.1.1/delve/__init__.py
+-rw-r--r--   0 jolene     (501) staff       (20)    21098 2023-06-29 20:01:23.000000 delve-fs-0.1.1/delve/delve.py
+drwxr-xr-x   0 jolene     (501) staff       (20)        0 2023-06-29 20:15:52.568059 delve-fs-0.1.1/delve_fs.egg-info/
+-rw-r--r--   0 jolene     (501) staff       (20)     4798 2023-06-29 20:15:52.000000 delve-fs-0.1.1/delve_fs.egg-info/PKG-INFO
+-rw-r--r--   0 jolene     (501) staff       (20)      218 2023-06-29 20:15:52.000000 delve-fs-0.1.1/delve_fs.egg-info/SOURCES.txt
+-rw-r--r--   0 jolene     (501) staff       (20)        1 2023-06-29 20:15:52.000000 delve-fs-0.1.1/delve_fs.egg-info/dependency_links.txt
+-rw-r--r--   0 jolene     (501) staff       (20)      116 2023-06-29 20:15:52.000000 delve-fs-0.1.1/delve_fs.egg-info/requires.txt
+-rw-r--r--   0 jolene     (501) staff       (20)        6 2023-06-29 20:15:52.000000 delve-fs-0.1.1/delve_fs.egg-info/top_level.txt
+-rw-r--r--   0 jolene     (501) staff       (20)       38 2023-06-29 20:15:52.568432 delve-fs-0.1.1/setup.cfg
+-rw-r--r--   0 jolene     (501) staff       (20)     1396 2023-06-29 20:15:19.000000 delve-fs-0.1.1/setup.py
```

### Comparing `delve-fs-0.1.0/LICENSE` & `delve-fs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `delve-fs-0.1.0/PKG-INFO` & `delve-fs-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delve-fs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Feature selection for preserving biological trajectories from single-cell data
 Home-page: https://github.com/jranek/delve
 Author: Jolene Ranek
 Author-email: ranekjs@gmail.com
 License: MIT
 Keywords: trajectory inference,feature selection,single-cell bioinformatics,computational biology
 Classifier: Development Status :: 3 - Alpha
@@ -43,19 +43,14 @@
 ```
 
 Alternatively, you can clone the git repository and install the necessary dependencies using the provided yml file. First clone the repository by, 
 ```
 git clone https://github.com/jranek/delve.git
 ```
 
-Once you've cloned the repository, please change your working directory as, 
-```
-cd delve
-```
-
 You can then create the conda environment using the provided yml file. 
 
 ```
 conda env create -f venv_delve.yml
 ```
 
 Once the environment is created, you can activate it by,
```

### Comparing `delve-fs-0.1.0/README.md` & `delve-fs-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 ```
 
 Alternatively, you can clone the git repository and install the necessary dependencies using the provided yml file. First clone the repository by, 
 ```
 git clone https://github.com/jranek/delve.git
 ```
 
-Once you've cloned the repository, please change your working directory as, 
-```
-cd delve
-```
-
 You can then create the conda environment using the provided yml file. 
 
 ```
 conda env create -f venv_delve.yml
 ```
 
 Once the environment is created, you can activate it by,
```

### Comparing `delve-fs-0.1.0/delve/delve.py` & `delve-fs-0.1.1/delve/delve.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     delta_mean: np.ndarray
         array containing average pairwise change in expression of all features across subsampled neighborhoods (dimensions = num_subsamples x features)
     state: int
         random seed parameter
     ----------
     """     
     #perform clustering     
-    clusters = KMeans(n_clusters = n_clusters, random_state = state, init = 'k-means++', n_init='auto').fit_predict(delta_mean.transpose())
+    clusters = KMeans(n_clusters = n_clusters, random_state = state, init = 'k-means++', n_init = 10).fit_predict(delta_mean.transpose())
     feats = {i:feature_names[np.where(clusters == i)[0]] for i in np.unique(clusters)}
 
     #record feature-cluster assignment to find intersection across runs
     mapping = np.full((len(feature_names), 1), 'NaN')
     for id, feature in feats.items():
         mapping[np.isin(feature_names, feature)] = str(id)  
     mapping_df = pd.DataFrame(mapping, index = feature_names, columns = [state])
```

### Comparing `delve-fs-0.1.0/delve_fs.egg-info/PKG-INFO` & `delve-fs-0.1.1/delve_fs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delve-fs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Feature selection for preserving biological trajectories from single-cell data
 Home-page: https://github.com/jranek/delve
 Author: Jolene Ranek
 Author-email: ranekjs@gmail.com
 License: MIT
 Keywords: trajectory inference,feature selection,single-cell bioinformatics,computational biology
 Classifier: Development Status :: 3 - Alpha
@@ -43,19 +43,14 @@
 ```
 
 Alternatively, you can clone the git repository and install the necessary dependencies using the provided yml file. First clone the repository by, 
 ```
 git clone https://github.com/jranek/delve.git
 ```
 
-Once you've cloned the repository, please change your working directory as, 
-```
-cd delve
-```
-
 You can then create the conda environment using the provided yml file. 
 
 ```
 conda env create -f venv_delve.yml
 ```
 
 Once the environment is created, you can activate it by,
```

### Comparing `delve-fs-0.1.0/setup.py` & `delve-fs-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='delve-fs',
     packages=['delve'],
-    version='0.1.0',
+    version='0.1.1',
     description='Feature selection for preserving biological trajectories from single-cell data',
     author='Jolene Ranek',
     author_email='ranekjs@gmail.com',
     url='https://github.com/jranek/delve',
     license='MIT',
     python_requires='>=3.6',
     long_description=long_description,
```

