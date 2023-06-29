# Comparing `tmp/aibench-0.0.4.tar.gz` & `tmp/aibench-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibench-0.0.4.tar", last modified: Sun Jun 25 15:37:56 2023, max compression
+gzip compressed data, was "aibench-0.0.5.tar", last modified: Thu Jun 29 19:22:09 2023, max compression
```

## Comparing `aibench-0.0.4.tar` & `aibench-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:56.751932 aibench-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-25 15:37:56.751932 aibench-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-25 15:37:44.000000 aibench-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-25 15:37:44.000000 aibench-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:56.751932 aibench-0.0.4/aibench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-25 15:37:56.000000 aibench-0.0.4/aibench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-25 15:37:56.000000 aibench-0.0.4/aibench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:37:56.000000 aibench-0.0.4/aibench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-25 15:37:56.000000 aibench-0.0.4/aibench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 15:37:56.000000 aibench-0.0.4/aibench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:56.751932 aibench-0.0.4/aibenchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:56.751932 aibench-0.0.4/aibenchmark/scrapers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/scrapers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-25 15:37:44.000000 aibench-0.0.4/aibenchmark/scrapers/papers_with_code_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-25 15:37:56.751932 aibench-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-25 15:37:44.000000 aibench-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:37:56.751932 aibench-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-25 15:37:44.000000 aibench-0.0.4/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-25 15:37:44.000000 aibench-0.0.4/tests/test_classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-25 15:37:44.000000 aibench-0.0.4/tests/test_nlp_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-25 15:37:44.000000 aibench-0.0.4/tests/test_regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:22:09.641405 aibench-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-29 19:22:09.641405 aibench-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-29 19:21:58.000000 aibench-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:22:09.637405 aibench-0.0.5/aibench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-29 19:22:09.000000 aibench-0.0.5/aibench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-29 19:22:09.000000 aibench-0.0.5/aibench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:22:09.000000 aibench-0.0.5/aibench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-29 19:22:09.000000 aibench-0.0.5/aibench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 19:22:09.000000 aibench-0.0.5/aibench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:22:09.641405 aibench-0.0.5/aibenchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-29 19:21:58.000000 aibench-0.0.5/aibenchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-29 19:21:58.000000 aibench-0.0.5/aibenchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-29 19:21:58.000000 aibench-0.0.5/aibenchmark/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-29 19:21:58.000000 aibench-0.0.5/aibenchmark/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-29 19:21:58.000000 aibench-0.0.5/aibenchmark/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-29 19:21:58.000000 aibench-0.0.5/aibenchmark/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:22:09.641405 aibench-0.0.5/aibenchmark/scrapers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:21:58.000000 aibench-0.0.5/aibenchmark/scrapers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-29 19:21:58.000000 aibench-0.0.5/aibenchmark/scrapers/papers_with_code_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 19:22:09.641405 aibench-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-29 19:21:58.000000 aibench-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:22:09.641405 aibench-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-29 19:21:58.000000 aibench-0.0.5/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-29 19:21:58.000000 aibench-0.0.5/tests/test_classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-29 19:21:58.000000 aibench-0.0.5/tests/test_nlp_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-29 19:21:58.000000 aibench-0.0.5/tests/test_regression_metrics.py
```

### Comparing `aibench-0.0.4/PKG-INFO` & `aibench-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: aibench
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/BasedLabs/aibenchmark/
 Author: Based Labs
 Author-email: 
 License: MIT
 Keywords: ai benchmark metrics
 Description-Content-Type: text/markdown
 
 <div align="center" id="top"> 
-  <img src="media/aibenchmark-logo.png" width="250px" alt="aibencharmk" />
+  <img src="https://github.com/BasedLabs/aibenchmark/raw/4f774ab8ad881724103b69ecd328a1eb80a94d3b/media/aibenchmark-logo.png" width="250px" alt="aibencharmk" />
 
   &#xa0;
 
   <!-- <a href="https://aibenchmark.netlify.app">Demo</a> -->
 </div>
 
 <h1 align="center">AIBenchmark</h1>
@@ -50,14 +50,21 @@
   <a href="#checkered_flag-starting">Starting</a> &#xa0; | &#xa0;
   <a href="#memo-license">License</a> &#xa0; | &#xa0;
   <a href="https://github.com/BasedLabs" target="_blank">Author</a>
 </p>
 
 <br>
 
+## Installation ##
+
+Run this script in your terminal:
+```bash
+$ pip install aibench
+```
+
 ## About ##
 
 AIBenchmark is a package which lets you quickly get the benchmark of your model based on the popular datasets and compare with existing leaderboard. It also has a nice collection of metrics which you could easily import.
 
 We currently support 14 text-based and 2 image-based datasets for AutoBenchmarking aiming for regression/classification tasks. Available datasets could be found in aibenchmark/dataset.py file. 
 
 Or run the following code:
@@ -97,21 +104,14 @@
 
 ## Features ##
 
 1) Fast comparison of metrics of your model and other SOTA models for particular dataset
 2) Supporting 16+ most populat datasets, the list is always updating. Soon we willl support more than 1000 datasets
 3) All metrics in one place and we are adding new ones in a standardised way
 
-## Starting ##
-
-```bash
-# Clone this project
-$ pip install git+https://github.com/BasedLabs/aibenchmark
-```
-
 ## Technologies ##
 
 The following tools were used in this project:
 
 - [Pytorch](https://pytorch.org/)
 - [Transformers](https://huggingface.co/transformers)
 - [Scikit-learn](https://scikit-learn.org/stable/)
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: aibench Version: 0.0.4 Home-page: https://
+Metadata-Version: 2.1 Name: aibench Version: 0.0.5 Home-page: https://
 github.com/BasedLabs/aibenchmark/ Author: Based Labs Author-email: License: MIT
 Keywords: ai benchmark metrics Description-Content-Type: text/markdown
                              [aibencharmk] &#xa0;
                            ****** AIBenchmark ******
              ***** Benchmark your model against other models *****
  [Github top language] [Github language count] [Repository size] [License]
 
   About &#xa0; | &#xa0; Features &#xa0; | &#xa0; Technologies &#xa0; | &#xa0;
             Starting &#xa0; | &#xa0; License &#xa0; | &#xa0; Author
 
-## About ## AIBenchmark is a package which lets you quickly get the benchmark
-of your model based on the popular datasets and compare with existing
+## Installation ## Run this script in your terminal: ```bash $ pip install
+aibench ``` ## About ## AIBenchmark is a package which lets you quickly get the
+benchmark of your model based on the popular datasets and compare with existing
 leaderboard. It also has a nice collection of metrics which you could easily
 import. We currently support 14 text-based and 2 image-based datasets for
 AutoBenchmarking aiming for regression/classification tasks. Available datasets
 could be found in aibenchmark/dataset.py file. Or run the following code:
 ```python from aibenchmark.dataset import DatasetsList print(list
 (DatasetsList.get_available_datasets())) ``` Code example for benchmarking:
 ```python from aibenchmark.benchmark import Benchmark from aibenchmark.dataset
@@ -26,14 +27,13 @@
 predictions benchmark_results = benchmark.run(predictions=outputs, metrics=
 ['accuracy', 'precision', 'recall', 'f1_score']) # Metrics print
 (benchmark_results) # Existing leaderboard for this dataset print
 (benchmark.get_existing_benchmarks()) ``` ## Features ## 1) Fast comparison of
 metrics of your model and other SOTA models for particular dataset 2)
 Supporting 16+ most populat datasets, the list is always updating. Soon we
 willl support more than 1000 datasets 3) All metrics in one place and we are
-adding new ones in a standardised way ## Starting ## ```bash # Clone this
-project $ pip install git+https://github.com/BasedLabs/aibenchmark ``` ##
-Technologies ## The following tools were used in this project: - [Pytorch]
-(https://pytorch.org/) - [Transformers](https://huggingface.co/transformers) -
-[Scikit-learn](https://scikit-learn.org/stable/) ## :memo: License ## This
-project is under license from MIT. For more details, see the [LICENSE]
-(LICENSE.md) file. Made by Igor and Tim &#xa0; Back_to_top
+adding new ones in a standardised way ## Technologies ## The following tools
+were used in this project: - [Pytorch](https://pytorch.org/) - [Transformers]
+(https://huggingface.co/transformers) - [Scikit-learn](https://scikit-
+learn.org/stable/) ## :memo: License ## This project is under license from MIT.
+For more details, see the [LICENSE](LICENSE.md) file. Made by Igor and Tim
+&#xa0; Back_to_top
```

### Comparing `aibench-0.0.4/README.md` & `aibench-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center" id="top"> 
-  <img src="media/aibenchmark-logo.png" width="250px" alt="aibencharmk" />
+  <img src="https://github.com/BasedLabs/aibenchmark/raw/4f774ab8ad881724103b69ecd328a1eb80a94d3b/media/aibenchmark-logo.png" width="250px" alt="aibencharmk" />
 
   &#xa0;
 
   <!-- <a href="https://aibenchmark.netlify.app">Demo</a> -->
 </div>
 
 <h1 align="center">AIBenchmark</h1>
@@ -40,14 +40,21 @@
   <a href="#checkered_flag-starting">Starting</a> &#xa0; | &#xa0;
   <a href="#memo-license">License</a> &#xa0; | &#xa0;
   <a href="https://github.com/BasedLabs" target="_blank">Author</a>
 </p>
 
 <br>
 
+## Installation ##
+
+Run this script in your terminal:
+```bash
+$ pip install aibench
+```
+
 ## About ##
 
 AIBenchmark is a package which lets you quickly get the benchmark of your model based on the popular datasets and compare with existing leaderboard. It also has a nice collection of metrics which you could easily import.
 
 We currently support 14 text-based and 2 image-based datasets for AutoBenchmarking aiming for regression/classification tasks. Available datasets could be found in aibenchmark/dataset.py file. 
 
 Or run the following code:
@@ -87,21 +94,14 @@
 
 ## Features ##
 
 1) Fast comparison of metrics of your model and other SOTA models for particular dataset
 2) Supporting 16+ most populat datasets, the list is always updating. Soon we willl support more than 1000 datasets
 3) All metrics in one place and we are adding new ones in a standardised way
 
-## Starting ##
-
-```bash
-# Clone this project
-$ pip install git+https://github.com/BasedLabs/aibenchmark
-```
-
 ## Technologies ##
 
 The following tools were used in this project:
 
 - [Pytorch](https://pytorch.org/)
 - [Transformers](https://huggingface.co/transformers)
 - [Scikit-learn](https://scikit-learn.org/stable/)
```

#### html2text {}

```diff
@@ -2,16 +2,17 @@
                            ****** AIBenchmark ******
              ***** Benchmark your model against other models *****
  [Github top language] [Github language count] [Repository size] [License]
 
   About &#xa0; | &#xa0; Features &#xa0; | &#xa0; Technologies &#xa0; | &#xa0;
             Starting &#xa0; | &#xa0; License &#xa0; | &#xa0; Author
 
-## About ## AIBenchmark is a package which lets you quickly get the benchmark
-of your model based on the popular datasets and compare with existing
+## Installation ## Run this script in your terminal: ```bash $ pip install
+aibench ``` ## About ## AIBenchmark is a package which lets you quickly get the
+benchmark of your model based on the popular datasets and compare with existing
 leaderboard. It also has a nice collection of metrics which you could easily
 import. We currently support 14 text-based and 2 image-based datasets for
 AutoBenchmarking aiming for regression/classification tasks. Available datasets
 could be found in aibenchmark/dataset.py file. Or run the following code:
 ```python from aibenchmark.dataset import DatasetsList print(list
 (DatasetsList.get_available_datasets())) ``` Code example for benchmarking:
 ```python from aibenchmark.benchmark import Benchmark from aibenchmark.dataset
@@ -23,14 +24,13 @@
 predictions benchmark_results = benchmark.run(predictions=outputs, metrics=
 ['accuracy', 'precision', 'recall', 'f1_score']) # Metrics print
 (benchmark_results) # Existing leaderboard for this dataset print
 (benchmark.get_existing_benchmarks()) ``` ## Features ## 1) Fast comparison of
 metrics of your model and other SOTA models for particular dataset 2)
 Supporting 16+ most populat datasets, the list is always updating. Soon we
 willl support more than 1000 datasets 3) All metrics in one place and we are
-adding new ones in a standardised way ## Starting ## ```bash # Clone this
-project $ pip install git+https://github.com/BasedLabs/aibenchmark ``` ##
-Technologies ## The following tools were used in this project: - [Pytorch]
-(https://pytorch.org/) - [Transformers](https://huggingface.co/transformers) -
-[Scikit-learn](https://scikit-learn.org/stable/) ## :memo: License ## This
-project is under license from MIT. For more details, see the [LICENSE]
-(LICENSE.md) file. Made by Igor and Tim &#xa0; Back_to_top
+adding new ones in a standardised way ## Technologies ## The following tools
+were used in this project: - [Pytorch](https://pytorch.org/) - [Transformers]
+(https://huggingface.co/transformers) - [Scikit-learn](https://scikit-
+learn.org/stable/) ## :memo: License ## This project is under license from MIT.
+For more details, see the [LICENSE](LICENSE.md) file. Made by Igor and Tim
+&#xa0; Back_to_top
```

### Comparing `aibench-0.0.4/aibench.egg-info/PKG-INFO` & `aibench-0.0.5/aibench.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: aibench
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/BasedLabs/aibenchmark/
 Author: Based Labs
 Author-email: 
 License: MIT
 Keywords: ai benchmark metrics
 Description-Content-Type: text/markdown
 
 <div align="center" id="top"> 
-  <img src="media/aibenchmark-logo.png" width="250px" alt="aibencharmk" />
+  <img src="https://github.com/BasedLabs/aibenchmark/raw/4f774ab8ad881724103b69ecd328a1eb80a94d3b/media/aibenchmark-logo.png" width="250px" alt="aibencharmk" />
 
   &#xa0;
 
   <!-- <a href="https://aibenchmark.netlify.app">Demo</a> -->
 </div>
 
 <h1 align="center">AIBenchmark</h1>
@@ -50,14 +50,21 @@
   <a href="#checkered_flag-starting">Starting</a> &#xa0; | &#xa0;
   <a href="#memo-license">License</a> &#xa0; | &#xa0;
   <a href="https://github.com/BasedLabs" target="_blank">Author</a>
 </p>
 
 <br>
 
+## Installation ##
+
+Run this script in your terminal:
+```bash
+$ pip install aibench
+```
+
 ## About ##
 
 AIBenchmark is a package which lets you quickly get the benchmark of your model based on the popular datasets and compare with existing leaderboard. It also has a nice collection of metrics which you could easily import.
 
 We currently support 14 text-based and 2 image-based datasets for AutoBenchmarking aiming for regression/classification tasks. Available datasets could be found in aibenchmark/dataset.py file. 
 
 Or run the following code:
@@ -97,21 +104,14 @@
 
 ## Features ##
 
 1) Fast comparison of metrics of your model and other SOTA models for particular dataset
 2) Supporting 16+ most populat datasets, the list is always updating. Soon we willl support more than 1000 datasets
 3) All metrics in one place and we are adding new ones in a standardised way
 
-## Starting ##
-
-```bash
-# Clone this project
-$ pip install git+https://github.com/BasedLabs/aibenchmark
-```
-
 ## Technologies ##
 
 The following tools were used in this project:
 
 - [Pytorch](https://pytorch.org/)
 - [Transformers](https://huggingface.co/transformers)
 - [Scikit-learn](https://scikit-learn.org/stable/)
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: aibench Version: 0.0.4 Home-page: https://
+Metadata-Version: 2.1 Name: aibench Version: 0.0.5 Home-page: https://
 github.com/BasedLabs/aibenchmark/ Author: Based Labs Author-email: License: MIT
 Keywords: ai benchmark metrics Description-Content-Type: text/markdown
                              [aibencharmk] &#xa0;
                            ****** AIBenchmark ******
              ***** Benchmark your model against other models *****
  [Github top language] [Github language count] [Repository size] [License]
 
   About &#xa0; | &#xa0; Features &#xa0; | &#xa0; Technologies &#xa0; | &#xa0;
             Starting &#xa0; | &#xa0; License &#xa0; | &#xa0; Author
 
-## About ## AIBenchmark is a package which lets you quickly get the benchmark
-of your model based on the popular datasets and compare with existing
+## Installation ## Run this script in your terminal: ```bash $ pip install
+aibench ``` ## About ## AIBenchmark is a package which lets you quickly get the
+benchmark of your model based on the popular datasets and compare with existing
 leaderboard. It also has a nice collection of metrics which you could easily
 import. We currently support 14 text-based and 2 image-based datasets for
 AutoBenchmarking aiming for regression/classification tasks. Available datasets
 could be found in aibenchmark/dataset.py file. Or run the following code:
 ```python from aibenchmark.dataset import DatasetsList print(list
 (DatasetsList.get_available_datasets())) ``` Code example for benchmarking:
 ```python from aibenchmark.benchmark import Benchmark from aibenchmark.dataset
@@ -26,14 +27,13 @@
 predictions benchmark_results = benchmark.run(predictions=outputs, metrics=
 ['accuracy', 'precision', 'recall', 'f1_score']) # Metrics print
 (benchmark_results) # Existing leaderboard for this dataset print
 (benchmark.get_existing_benchmarks()) ``` ## Features ## 1) Fast comparison of
 metrics of your model and other SOTA models for particular dataset 2)
 Supporting 16+ most populat datasets, the list is always updating. Soon we
 willl support more than 1000 datasets 3) All metrics in one place and we are
-adding new ones in a standardised way ## Starting ## ```bash # Clone this
-project $ pip install git+https://github.com/BasedLabs/aibenchmark ``` ##
-Technologies ## The following tools were used in this project: - [Pytorch]
-(https://pytorch.org/) - [Transformers](https://huggingface.co/transformers) -
-[Scikit-learn](https://scikit-learn.org/stable/) ## :memo: License ## This
-project is under license from MIT. For more details, see the [LICENSE]
-(LICENSE.md) file. Made by Igor and Tim &#xa0; Back_to_top
+adding new ones in a standardised way ## Technologies ## The following tools
+were used in this project: - [Pytorch](https://pytorch.org/) - [Transformers]
+(https://huggingface.co/transformers) - [Scikit-learn](https://scikit-
+learn.org/stable/) ## :memo: License ## This project is under license from MIT.
+For more details, see the [LICENSE](LICENSE.md) file. Made by Igor and Tim
+&#xa0; Back_to_top
```

### Comparing `aibench-0.0.4/aibench.egg-info/SOURCES.txt` & `aibench-0.0.5/aibench.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 README.md
-README.rst
 setup.cfg
 setup.py
 aibench.egg-info/PKG-INFO
 aibench.egg-info/SOURCES.txt
 aibench.egg-info/dependency_links.txt
 aibench.egg-info/requires.txt
 aibench.egg-info/top_level.txt
```

### Comparing `aibench-0.0.4/aibenchmark/benchmark.py` & `aibench-0.0.5/aibenchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.4/aibenchmark/dataset.py` & `aibench-0.0.5/aibenchmark/dataset.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.4/aibenchmark/metrics.py` & `aibench-0.0.5/aibenchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.4/aibenchmark/scrapers/papers_with_code_scraper.py` & `aibench-0.0.5/aibenchmark/scrapers/papers_with_code_scraper.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.4/setup.py` & `aibench-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aibench',
-    version='0.0.4',
+    version='0.0.5',
     license='MIT',
     author="Based Labs",
     author_email='',
     packages=find_packages(exclude=["tests"]),
     url='https://github.com/BasedLabs/aibenchmark/',
     keywords='ai benchmark metrics',
     install_requires=[
```

### Comparing `aibench-0.0.4/tests/test_benchmark.py` & `aibench-0.0.5/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.4/tests/test_classification_metrics.py` & `aibench-0.0.5/tests/test_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `aibench-0.0.4/tests/test_regression_metrics.py` & `aibench-0.0.5/tests/test_regression_metrics.py`

 * *Files identical despite different names*

