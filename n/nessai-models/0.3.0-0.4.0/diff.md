# Comparing `tmp/nessai_models-0.3.0.tar.gz` & `tmp/nessai_models-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nessai_models-0.3.0.tar", last modified: Sun Feb 19 11:29:10 2023, max compression
+gzip compressed data, was "nessai_models-0.4.0.tar", last modified: Thu Jun 29 11:14:38 2023, max compression
```

## Comparing `nessai_models-0.3.0.tar` & `nessai_models-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 11:29:10.066899 nessai_models-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 11:29:10.062899 nessai_models-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 11:29:10.062899 nessai_models-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-19 11:29:00.000000 nessai_models-0.3.0/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-19 11:29:00.000000 nessai_models-0.3.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-02-19 11:29:00.000000 nessai_models-0.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-19 11:29:00.000000 nessai_models-0.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-02-19 11:29:00.000000 nessai_models-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-19 11:29:00.000000 nessai_models-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-02-19 11:29:00.000000 nessai_models-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-02-19 11:29:10.066899 nessai_models-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-02-19 11:29:00.000000 nessai_models-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 11:29:10.062899 nessai_models-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-02-19 11:29:00.000000 nessai_models-0.3.0/examples/basic_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 11:29:10.062899 nessai_models-0.3.0/nessai_models/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-19 11:29:00.000000 nessai_models-0.3.0/nessai_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-02-19 11:29:00.000000 nessai_models-0.3.0/nessai_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-02-19 11:29:00.000000 nessai_models-0.3.0/nessai_models/brewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-02-19 11:29:00.000000 nessai_models-0.3.0/nessai_models/eggbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-02-19 11:29:00.000000 nessai_models-0.3.0/nessai_models/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-02-19 11:29:00.000000 nessai_models-0.3.0/nessai_models/gaussianmixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-19 11:29:00.000000 nessai_models-0.3.0/nessai_models/halfgaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-19 11:29:00.000000 nessai_models-0.3.0/nessai_models/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-02-19 11:29:00.000000 nessai_models-0.3.0/nessai_models/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-02-19 11:29:00.000000 nessai_models-0.3.0/nessai_models/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 11:29:10.066899 nessai_models-0.3.0/nessai_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-02-19 11:29:10.000000 nessai_models-0.3.0/nessai_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-02-19 11:29:10.000000 nessai_models-0.3.0/nessai_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 11:29:10.000000 nessai_models-0.3.0/nessai_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-19 11:29:10.000000 nessai_models-0.3.0/nessai_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-19 11:29:10.000000 nessai_models-0.3.0/nessai_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-19 11:29:00.000000 nessai_models-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-19 11:29:10.066899 nessai_models-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-19 11:29:00.000000 nessai_models-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 11:29:10.066899 nessai_models-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-19 11:29:00.000000 nessai_models-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-02-19 11:29:00.000000 nessai_models-0.3.0/tests/test_base_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-02-19 11:29:00.000000 nessai_models-0.3.0/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-02-19 11:29:00.000000 nessai_models-0.3.0/tests/test_gaussianmixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-19 11:29:00.000000 nessai_models-0.3.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-02-19 11:29:00.000000 nessai_models-0.3.0/tests/test_nessai_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-19 11:29:00.000000 nessai_models-0.3.0/tests/test_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-02-19 11:29:00.000000 nessai_models-0.3.0/tests/test_rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-19 11:29:00.000000 nessai_models-0.3.0/tests/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.989502 nessai_models-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.977502 nessai_models-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.981502 nessai_models-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-29 11:14:23.000000 nessai_models-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-29 11:14:38.989502 nessai_models-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-29 11:14:23.000000 nessai_models-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.981502 nessai_models-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-29 11:14:23.000000 nessai_models-0.4.0/examples/basic_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.985502 nessai_models-0.4.0/nessai_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/brewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/eggbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/gaussianmixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/halfgaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.985502 nessai_models-0.4.0/nessai_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-29 11:14:38.000000 nessai_models-0.4.0/nessai_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-29 11:14:38.000000 nessai_models-0.4.0/nessai_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:14:38.000000 nessai_models-0.4.0/nessai_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-29 11:14:38.000000 nessai_models-0.4.0/nessai_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 11:14:38.000000 nessai_models-0.4.0/nessai_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-29 11:14:23.000000 nessai_models-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-29 11:14:38.989502 nessai_models-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-29 11:14:23.000000 nessai_models-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.989502 nessai_models-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_gaussianmixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_nessai_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_signals.py
```

### Comparing `nessai_models-0.3.0/.github/workflows/integration-tests.yml` & `nessai_models-0.4.0/.github/workflows/integration-tests.yml`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/.github/workflows/lint.yml` & `nessai_models-0.4.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/.github/workflows/publish-to-pypi.yml` & `nessai_models-0.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/.github/workflows/tests.yml` & `nessai_models-0.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/.gitignore` & `nessai_models-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/CHANGELOG.md` & `nessai_models-0.4.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.4.0] - 2023-06-29
+
+### Added
+
+- Add a Mixture of 1-dimensional distributions likelihood ([#31](https://github.com/mj-will/nessai-models/pull/31))
+
 
 ## [0.3.0] - 2023-02-19
 
 ### Added
 
 - Add Brewer likelihood described in [arXiv:0912.2380](https://arxiv.org/abs/0912.2380). ([#28](https://github.com/mj-will/nessai-models/pull/28))
 
@@ -30,11 +36,12 @@
 - Add n-dimensional HalfGaussian ([#8](https://github.com/mj-will/nessai-models/pull/8))
 - Add Gaussian Mixture Model based on a [`cpnest` example](https://github.com/johnveitch/cpnest/blob/master/examples/gaussianmixture.py) ([#5](https://github.com/mj-will/nessai-models/pull/5))
 - Add n-dimensional Egg Box based on the version from [Feroz et al. 2008](https://arxiv.org/abs/0809.3437) ([#11](https://github.com/mj-will/nessai-models/pull/11))
 - Add n-dimensional Pyramid-like model ([#15](https://github.com/mj-will/nessai-models/pull/15))
 - Add basic tests for all models
 - Add a basic example ([#21](https://github.com/mj-will/nessai-models/pull/21))
 
-[Unreleased]: https://github.com/mj-will/nessai-models/compare/v0.3.0...HEAD
+[Unreleased]: https://github.com/mj-will/nessai-models/compare/v0.4.0...HEAD
+[0.4.0]: https://github.com/mj-will/nessai-models/compare/v0.3.0...v0.4.0
 [0.3.0]: https://github.com/mj-will/nessai-models/compare/v0.2.0...v0.3.0
 [0.2.0]: https://github.com/mj-will/nessai-models/compare/v0.1.0...v0.2.0
 [0.1.0]: https://github.com/mj-will/nessai-models/releases/tag/v0.1.0
```

### Comparing `nessai_models-0.3.0/PKG-INFO` & `nessai_models-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessai_models
-Version: 0.3.0
+Version: 0.4.0
 Summary: Models for nessai
 Home-page: https://github.com/mj-will/nessai-models
 Author: Michael J. Williams
 Author-email: m.williams.4@research.gla.ac.uk
 License: MIT
 Keywords: nested sampling,normalising flows,machine learning,nessai
 Classifier: Programming Language :: Python :: 3.7
@@ -30,17 +30,18 @@
 * n-dimensional unit Gaussian
 * n-dimensional HalfGaussian
 * n-dimensional Rosenbrock
 * n-dimensional mixture of Gaussians
 * Gaussian mixture using data to based on [this example](https://github.com/johnveitch/cpnest/blob/master/examples/gaussianmixture.py) from `cpnest`
 * n-dimensional Egg Box based on the version in [Feroz et al. 2008](https://arxiv.org/abs/0809.3437)
 * n-dimensional Pyramid-like model
-* n-dimensional Brewer likelihod (Skilling's "Staistical Model") from [Brewer et al.](https://arxiv.org/abs/0912.2380)
+* n-dimensional Brewer likelihood (Skilling's "Staistical Model") from [Brewer et al.](https://arxiv.org/abs/0912.2380)
 * Linear signal plus Gaussian noise model (`LinearSignal`)
 * Sinusoidal signal plus Gaussian noise model (`SinusoidalSignal`)
+* Mixture of 1-dimensional distributions (`MixtureOfDistributions`)
 
 ## Requirements
 
 `nessai_models` requires:
 
 * `numpy`
 * `scipy`
```

### Comparing `nessai_models-0.3.0/README.md` & `nessai_models-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 * n-dimensional unit Gaussian
 * n-dimensional HalfGaussian
 * n-dimensional Rosenbrock
 * n-dimensional mixture of Gaussians
 * Gaussian mixture using data to based on [this example](https://github.com/johnveitch/cpnest/blob/master/examples/gaussianmixture.py) from `cpnest`
 * n-dimensional Egg Box based on the version in [Feroz et al. 2008](https://arxiv.org/abs/0809.3437)
 * n-dimensional Pyramid-like model
-* n-dimensional Brewer likelihod (Skilling's "Staistical Model") from [Brewer et al.](https://arxiv.org/abs/0912.2380)
+* n-dimensional Brewer likelihood (Skilling's "Staistical Model") from [Brewer et al.](https://arxiv.org/abs/0912.2380)
 * Linear signal plus Gaussian noise model (`LinearSignal`)
 * Sinusoidal signal plus Gaussian noise model (`SinusoidalSignal`)
+* Mixture of 1-dimensional distributions (`MixtureOfDistributions`)
 
 ## Requirements
 
 `nessai_models` requires:
 
 * `numpy`
 * `scipy`
```

### Comparing `nessai_models-0.3.0/examples/basic_example.py` & `nessai_models-0.4.0/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/nessai_models/__init__.py` & `nessai_models-0.4.0/nessai_models/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,23 +14,25 @@
     pass
 
 from .brewer import Brewer
 from .eggbox import EggBox
 from .gaussian import Gaussian
 from .gaussianmixture import GaussianMixture, GaussianMixtureWithData
 from .halfgaussian import HalfGaussian
+from .mixture import MixtureOfDistributions
 from .pyramid import Pyramid
 from .rosenbrock import Rosenbrock
 from .signals import LinearSignal, SinusoidalSignal
 
 __all__ = [
     "Brewer",
     "EggBox",
     "Gaussian",
     "GaussianMixture",
     "GaussianMixtureWithData",
     "HalfGaussian",
     "LinearSignal",
+    "MixtureOfDistributions",
     "Pyramid",
     "Rosenbrock",
     "SinusoidalSignal",
 ]
```

### Comparing `nessai_models-0.3.0/nessai_models/base.py` & `nessai_models-0.4.0/nessai_models/base.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/nessai_models/brewer.py` & `nessai_models-0.4.0/nessai_models/brewer.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/nessai_models/eggbox.py` & `nessai_models-0.4.0/nessai_models/eggbox.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/nessai_models/gaussian.py` & `nessai_models-0.4.0/nessai_models/gaussian.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/nessai_models/gaussianmixture.py` & `nessai_models-0.4.0/nessai_models/gaussianmixture.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/nessai_models/halfgaussian.py` & `nessai_models-0.4.0/nessai_models/halfgaussian.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/nessai_models/pyramid.py` & `nessai_models-0.4.0/nessai_models/pyramid.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/nessai_models/rosenbrock.py` & `nessai_models-0.4.0/nessai_models/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/nessai_models/signals.py` & `nessai_models-0.4.0/nessai_models/signals.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/nessai_models.egg-info/PKG-INFO` & `nessai_models-0.4.0/nessai_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessai-models
-Version: 0.3.0
+Version: 0.4.0
 Summary: Models for nessai
 Home-page: https://github.com/mj-will/nessai-models
 Author: Michael J. Williams
 Author-email: m.williams.4@research.gla.ac.uk
 License: MIT
 Keywords: nested sampling,normalising flows,machine learning,nessai
 Classifier: Programming Language :: Python :: 3.7
@@ -30,17 +30,18 @@
 * n-dimensional unit Gaussian
 * n-dimensional HalfGaussian
 * n-dimensional Rosenbrock
 * n-dimensional mixture of Gaussians
 * Gaussian mixture using data to based on [this example](https://github.com/johnveitch/cpnest/blob/master/examples/gaussianmixture.py) from `cpnest`
 * n-dimensional Egg Box based on the version in [Feroz et al. 2008](https://arxiv.org/abs/0809.3437)
 * n-dimensional Pyramid-like model
-* n-dimensional Brewer likelihod (Skilling's "Staistical Model") from [Brewer et al.](https://arxiv.org/abs/0912.2380)
+* n-dimensional Brewer likelihood (Skilling's "Staistical Model") from [Brewer et al.](https://arxiv.org/abs/0912.2380)
 * Linear signal plus Gaussian noise model (`LinearSignal`)
 * Sinusoidal signal plus Gaussian noise model (`SinusoidalSignal`)
+* Mixture of 1-dimensional distributions (`MixtureOfDistributions`)
 
 ## Requirements
 
 `nessai_models` requires:
 
 * `numpy`
 * `scipy`
```

### Comparing `nessai_models-0.3.0/nessai_models.egg-info/SOURCES.txt` & `nessai_models-0.4.0/nessai_models.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 nessai_models/__init__.py
 nessai_models/base.py
 nessai_models/brewer.py
 nessai_models/eggbox.py
 nessai_models/gaussian.py
 nessai_models/gaussianmixture.py
 nessai_models/halfgaussian.py
+nessai_models/mixture.py
 nessai_models/pyramid.py
 nessai_models/rosenbrock.py
 nessai_models/signals.py
 nessai_models.egg-info/PKG-INFO
 nessai_models.egg-info/SOURCES.txt
 nessai_models.egg-info/dependency_links.txt
 nessai_models.egg-info/requires.txt
 nessai_models.egg-info/top_level.txt
 tests/conftest.py
 tests/test_base_models.py
 tests/test_gaussian.py
 tests/test_gaussianmixture.py
+tests/test_mixture.py
 tests/test_models.py
 tests/test_nessai_integration.py
 tests/test_pyramid.py
 tests/test_rosenbrock.py
 tests/test_signals.py
```

### Comparing `nessai_models-0.3.0/setup.cfg` & `nessai_models-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/tests/conftest.py` & `nessai_models-0.4.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     Brewer,
     EggBox,
     Gaussian,
     GaussianMixture,
     GaussianMixtureWithData,
     HalfGaussian,
     LinearSignal,
+    MixtureOfDistributions,
     Pyramid,
     Rosenbrock,
     SinusoidalSignal,
 )
 import pytest
 
 
@@ -18,14 +19,15 @@
     Brewer,
     EggBox,
     Gaussian,
     GaussianMixture,
     GaussianMixtureWithData,
     HalfGaussian,
     LinearSignal,
+    MixtureOfDistributions,
     Pyramid,
     Rosenbrock,
     SinusoidalSignal,
 ]
 
 
 @pytest.fixture(params=all_models)
```

### Comparing `nessai_models-0.3.0/tests/test_base_models.py` & `nessai_models-0.4.0/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/tests/test_gaussian.py` & `nessai_models-0.4.0/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/tests/test_gaussianmixture.py` & `nessai_models-0.4.0/tests/test_gaussianmixture.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/tests/test_nessai_integration.py` & `nessai_models-0.4.0/tests/test_nessai_integration.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/tests/test_rosenbrock.py` & `nessai_models-0.4.0/tests/test_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.3.0/tests/test_signals.py` & `nessai_models-0.4.0/tests/test_signals.py`

 * *Files identical despite different names*

