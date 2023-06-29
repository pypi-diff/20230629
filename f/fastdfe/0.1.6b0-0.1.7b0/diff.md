# Comparing `tmp/fastdfe-0.1.6b0.tar.gz` & `tmp/fastdfe-0.1.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdfe-0.1.6b0.tar", max compression
+gzip compressed data, was "fastdfe-0.1.7b0.tar", max compression
```

## Comparing `fastdfe-0.1.6b0.tar` & `fastdfe-0.1.7b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      881 2023-05-25 06:14:31.511946 fastdfe-0.1.6b0/README.md
--rw-r--r--   0        0        0     4933 2023-05-25 06:14:31.675947 fastdfe-0.1.6b0/fastdfe/__init__.py
--rw-r--r--   0        0        0    20069 2023-05-25 06:14:31.675947 fastdfe-0.1.6b0/fastdfe/abstract_inference.py
--rw-r--r--   0        0        0    31181 2023-05-25 06:14:31.675947 fastdfe-0.1.6b0/fastdfe/annotation.py
--rw-r--r--   0        0        0    48780 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/base_inference.py
--rw-r--r--   0        0        0     4869 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/bootstrap.py
--rw-r--r--   0        0        0    10468 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/config.py
--rw-r--r--   0        0        0    15069 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/discretization.py
--rw-r--r--   0        0        0     9215 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/filtration.py
--rw-r--r--   0        0        0    44110 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/joint_inference.py
--rw-r--r--   0        0        0     3902 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/json_handlers.py
--rw-r--r--   0        0        0     2484 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/mle.py
--rw-r--r--   0        0        0    37834 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/optimization.py
--rw-r--r--   0        0        0    21679 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/parametrization.py
--rw-r--r--   0        0        0    27820 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/parser.py
--rw-r--r--   0        0        0    12485 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/polydfe.py
--rw-r--r--   0        0        0     5254 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/polydfe_utils.py
--rw-r--r--   0        0        0    22109 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/spectrum.py
--rw-r--r--   0        0        0     8492 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/vcf.py
--rw-r--r--   0        0        0    28670 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/visualization.py
--rw-r--r--   0        0        0     1084 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/pyproject.toml
--rw-r--r--   0        0        0     2027 1970-01-01 00:00:00.000000 fastdfe-0.1.6b0/PKG-INFO
+-rw-r--r--   0        0        0      859 2023-06-29 11:11:32.811581 fastdfe-0.1.7b0/README.md
+-rw-r--r--   0        0        0     5295 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/__init__.py
+-rw-r--r--   0        0        0    22526 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/abstract_inference.py
+-rw-r--r--   0        0        0    33177 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/annotation.py
+-rw-r--r--   0        0        0    50946 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/base_inference.py
+-rw-r--r--   0        0        0    15952 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/bio_handlers.py
+-rw-r--r--   0        0        0     4891 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/bootstrap.py
+-rw-r--r--   0        0        0    11097 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/config.py
+-rw-r--r--   0        0        0    15236 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/discretization.py
+-rw-r--r--   0        0        0    14334 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/filtration.py
+-rw-r--r--   0        0        0    46481 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/joint_inference.py
+-rw-r--r--   0        0        0     3902 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/json_handlers.py
+-rw-r--r--   0        0        0     2556 2023-06-29 11:11:33.003583 fastdfe-0.1.7b0/fastdfe/likelihood.py
+-rw-r--r--   0        0        0    38134 2023-06-29 11:11:33.007583 fastdfe-0.1.7b0/fastdfe/optimization.py
+-rw-r--r--   0        0        0    28107 2023-06-29 11:11:33.007583 fastdfe-0.1.7b0/fastdfe/parametrization.py
+-rw-r--r--   0        0        0    30031 2023-06-29 11:11:33.007583 fastdfe-0.1.7b0/fastdfe/parser.py
+-rw-r--r--   0        0        0    12947 2023-06-29 11:11:33.007583 fastdfe-0.1.7b0/fastdfe/polydfe.py
+-rw-r--r--   0        0        0     5254 2023-06-29 11:11:33.007583 fastdfe-0.1.7b0/fastdfe/polydfe_utils.py
+-rw-r--r--   0        0        0    23180 2023-06-29 11:11:33.007583 fastdfe-0.1.7b0/fastdfe/spectrum.py
+-rw-r--r--   0        0        0    31581 2023-06-29 11:11:33.007583 fastdfe-0.1.7b0/fastdfe/visualization.py
+-rw-r--r--   0        0        0      925 2023-06-29 11:11:33.007583 fastdfe-0.1.7b0/pyproject.toml
+-rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 fastdfe-0.1.7b0/PKG-INFO
```

### Comparing `fastdfe-0.1.6b0/README.md` & `fastdfe-0.1.7b0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 [![tests](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml)
 [![codecov](https://codecov.io/gh/Sendrowski/fastDFE/branch/master/graph/badge.svg?token=0LUE8SZYBJ)](https://codecov.io/gh/Sendrowski/fastDFE)
 [![Documentation Status](https://readthedocs.org/projects/fastdfe/badge/?version=latest)](https://fastdfe.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/fastdfe.svg)](https://badge.fury.io/py/fastdfe)
 
-fastDFE is a new package designed for inferring the distribution of fitness effects (DFE) from site-frequency spectra (SFS). As it is currently in its beta phase, we are continuously working to improve and refine its features.
+fastDFE is a package for fast, flexible, and hierarchical inference of the distribution of fitness effects (DFE) from site frequency spectra (SFS). Please note that fastDFE is currently in its beta phase.
 
 Please see the [documentation](https://fastdfe.readthedocs.io/en/latest/) for all the details.
```

### Comparing `fastdfe-0.1.6b0/fastdfe/__init__.py` & `fastdfe-0.1.7b0/fastdfe/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 fastDFE package.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-03-10"
 
-__version__ = '0.1.6-beta'
+__version__ = '0.1.7-beta'
 
 import logging
 import sys
 import warnings
 
 import jsonpickle
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import requests_cache
 from tqdm import tqdm
 
 from .json_handlers import DataframeHandler, SpectrumHandler, SpectraHandler, NumpyArrayHandler
 from .spectrum import Spectrum, Spectra
 
+# set the default figure size
+plt.rcParams['figure.figsize'] = np.array([6.4, 4.8]) * 0.8
+
 # register custom handles
 jsonpickle.handlers.registry.register(pd.DataFrame, DataframeHandler)
 jsonpickle.handlers.registry.register(Spectrum, SpectrumHandler)
 jsonpickle.handlers.registry.register(Spectra, SpectraHandler)
 jsonpickle.handlers.registry.register(np.ndarray, NumpyArrayHandler)
 
 
@@ -40,15 +43,15 @@
     def emit(self, record):
         """
         Emit a record.
         """
         try:
             msg = self.format(record)
 
-            # we write to stderr to avoid as the progress bar
+            # we write to stderr as the progress bar
             # to make the two work together
             tqdm.write(msg, file=sys.stderr)
             self.flush()
         except Exception:
             self.handleError(record)
 
 
@@ -87,25 +90,22 @@
 # set to INFO by default
 logger.setLevel(logging.INFO)
 
 # let TQDM handle the logging
 handler = TqdmLoggingHandler()
 
 # define a Formatter with colors
-formatter = ColoredFormatter('%(levelname)s:%(name)s:%(message)s')
+formatter = ColoredFormatter('%(levelname)s:%(name)s: %(message)s')
 
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
 # whether to disable the progress bar
 disable_pbar = False
 
-# install cache
-requests_cache.install_cache('fastdfe_requests_cache', expire_after=3600 * 24)
-
 
 def raise_on_warning(message, category, filename, lineno, file=None, line=None):
     """
     Raise exception on warning.
     """
     raise Exception(warnings.formatwarning(message, category, filename, lineno, line))
 
@@ -114,36 +114,37 @@
 
 # configure default colormap
 # plt.rcParams['image.cmap'] = 'Dark2'
 # plt.rcParams['axes.prop_cycle'] = cycler('color', plt.get_cmap('Dark2').colors)
 
 # load class from modules
 from .parametrization import Parametrization, GammaExpParametrization, DiscreteParametrization, \
-    GammaDiscreteParametrization, DisplacedGammaParametrization
+    GammaDiscreteParametrization, DisplacedGammaParametrization, DiscreteFractionalParametrization
 from .config import Config
 from .abstract_inference import Inference
 from .base_inference import BaseInference, InferenceResults
 from .joint_inference import JointInference, SharedParams
 from .optimization import Covariate
 from .visualization import Visualization
 from .spectrum import Spectrum, Spectra
 from .parser import Parser, Stratification, BaseTransitionStratification, BaseContextStratification, \
     DegeneracyStratification, TransitionTransversionStratification, AncestralBaseStratification, \
-    SynonymyStratification, VEPStratification, SnpEffStratification
+    SynonymyStratification, VEPStratification, SnpEffStratification, ContigStratification, ChunkedStratification
+from .bio_handlers import VCFHandler
 from .annotation import Annotator, Annotation, MaximumParsimonyAnnotation, DegeneracyAnnotation, SynonymyAnnotation
 from .filtration import Filterer, Filtration, SNPFiltration, PolyAllelicFiltration, CodingSequenceFiltration, \
-    SNVFiltration
-from .vcf import VCFHandler
+    SNVFiltration, DeviantOutgroupFiltration, AllFiltration, NoFiltration, BiasedGCConversionFiltration
 
 __all__ = [
     'Parametrization',
     'GammaExpParametrization',
     'DiscreteParametrization',
     'GammaDiscreteParametrization',
     'DisplacedGammaParametrization',
+    'DiscreteFractionalParametrization',
     'Config',
     'Inference',
     'BaseInference',
     'JointInference',
     'SharedParams',
     'Covariate',
     'Visualization',
@@ -154,21 +155,26 @@
     'BaseContextStratification',
     'DegeneracyStratification',
     'TransitionTransversionStratification',
     'AncestralBaseStratification',
     'SynonymyStratification',
     'VEPStratification',
     'SnpEffStratification',
+    'ContigStratification',
+    'ChunkedStratification',
     'Annotator',
     'Annotation',
     'MaximumParsimonyAnnotation',
     'DegeneracyAnnotation',
     'SynonymyAnnotation',
     'Filtration',
     'CodingSequenceFiltration',
+    'DeviantOutgroupFiltration',
+    'AllFiltration',
+    'NoFiltration',
     'Filterer',
     'SNPFiltration',
     'SNVFiltration',
     'PolyAllelicFiltration',
+    'BiasedGCConversionFiltration',
     'Filterer',
-    'VCFHandler',
 ]
```

### Comparing `fastdfe-0.1.6b0/fastdfe/abstract_inference.py` & `fastdfe-0.1.7b0/fastdfe/abstract_inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 Abstract inference class and static utilities.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-03-12"
 
+import logging
 from abc import ABC, abstractmethod
 from typing import List, Optional, Literal, Tuple, Dict
-from typing_extensions import Self
 
 import jsonpickle
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
+from typing_extensions import Self
 
 from .bootstrap import Bootstrap
-from .parametrization import Parametrization, from_string
+from .parametrization import Parametrization, _from_string
 from .visualization import Visualization
 
+logger = logging.getLogger("fastdfe")
+
 
 class Inference:
     """
     Static utility methods for inference objects.
     """
 
     @staticmethod
@@ -33,14 +36,15 @@
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'discretized DFEs',
             labels: list | np.ndarray = None,
             ax: plt.Axes = None,
+            kwargs_legend: dict = dict(prop=dict(size=8)),
             **kwargs
 
     ) -> plt.Axes:
         """
         Visualize several discretized DFEs given by the list of inference objects.
 
         :param inferences: List of inference objects.
@@ -50,14 +54,15 @@
         :param bootstrap_type: Type of bootstrap to use for confidence intervals.
         :param file: Path to file to save the plot to.
         :param show: Whether to show the plot.
         :param title: Title of the plot.
         :param labels: Labels for the DFEs.
         :param kwargs: Additional arguments for the plot.
         :param ax: Axes of the plot.
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes of the plot.
         """
         # get data from inference objects
         values = []
         errors = []
         for i, inference in enumerate(inferences):
             val, errs = inference.get_discretized(
@@ -75,15 +80,16 @@
             values=values,
             errors=errors,
             labels=labels,
             file=file,
             show=show,
             intervals=intervals,
             title=title,
-            ax=ax
+            ax=ax,
+            kwargs_legend=kwargs_legend
         )
 
     @staticmethod
     def plot_continuous(
             inferences: List['AbstractInference'],
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
@@ -92,14 +98,15 @@
             file: str = None,
             show: bool = True,
             title: str = 'continuous DFEs',
             labels: list | np.ndarray = None,
             scale: Literal['lin', 'log', 'symlog'] = 'lin',
             scale_density: bool = False,
             ax: plt.Axes = None,
+            kwargs_legend: dict = dict(prop=dict(size=8)),
             **kwargs
 
     ) -> plt.Axes:
         """
         Visualize several DFEs given by the list of inference objects.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
         the x-axis, we may get a wrong intuition on how the mass is distributed,
@@ -116,14 +123,15 @@
         :param file: Path to file to save the plot to.
         :param show: Whether to show the plot.
         :param title: Title of the plot.
         :param labels: Labels for the DFEs.
         :param scale: y-scale of the plot.
         :param scale_density: Whether to scale the density by the x-axis interval size.
         :param ax: Axes of the plot.
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :param kwargs: Additional arguments for the plot.
         :return: Axes of the plot.
         """
         # get data from inference objects
         values = []
         errors = []
         for i, inf in enumerate(inferences):
@@ -152,14 +160,15 @@
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             scale: Literal['lin', 'log', 'symlog'] = 'log',
             legend: bool = True,
             ax: plt.Axes = None,
+            kwargs_legend: dict = dict(prop=dict(size=8), loc='upper right'),
             **kwargs
 
     ) -> plt.Axes:
         """
         Visualize several discretized DFEs given by the list of inference objects.
         Note that the DFE parametrization needs to be the same for all inference objects.
 
@@ -172,14 +181,15 @@
         :param bootstrap_type: Type of bootstrap to use for confidence intervals.
         :param file: Path to file to save the plot to.
         :param show: Whether to show the plot.
         :param title: Title of the plot.
         :param ax: Axes of the plot.
         :param kwargs: Additional arguments for the plot.
         :return: Axes of the plot.
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :raises ValueError: If no inference objects are given.
         """
         if len(inferences) == 0:
             raise ValueError('No inference objects given.')
 
         # get sorted list of parameter names
         param_names = sorted(list(inferences[0].get_bootstrap_param_names()))
@@ -200,15 +210,59 @@
             param_names=param_names,
             file=file,
             show=show,
             title=title,
             labels=labels,
             scale=scale,
             legend=len(labels) > 1,
-            ax=ax
+            kwargs_legend=kwargs_legend,
+            ax=ax,
+        )
+
+    @staticmethod
+    def plot_inferred_parameters_boxplot(
+            inferences: List['AbstractInference'],
+            labels: list | np.ndarray,
+            file: str = None,
+            show: bool = True,
+            title: str = 'parameter estimates',
+            **kwargs
+
+    ) -> plt.Axes:
+        """
+        Visualize several discretized DFEs given by the list of inference objects.
+        Note that the DFE parametrization needs to be the same for all inference objects.
+
+        :param inferences: List of inference objects.
+        :param labels: Unique labels for the DFEs.
+        :param file: Path to file to save the plot to.
+        :param show: Whether to show the plot.
+        :param title: Title of the plot.
+        :param kwargs: Additional arguments for the plot.
+        :return: Axes of the plot.
+        :raises ValueError: If no inference objects are given or no bootstraps are found.
+        """
+        if len(inferences) == 0:
+            raise ValueError('No inference objects given.')
+
+        # get sorted list of parameter names
+        param_names = sorted(list(inferences[0].get_bootstrap_param_names()))
+
+        if inferences[0].bootstraps is None:
+            raise ValueError('No bootstraps found.')
+
+        # create dict of dataframes
+        values = dict((k, inf.bootstraps) for k, inf in zip(labels, inferences))
+
+        return Visualization.plot_inferred_parameters_boxplot(
+            values=values,
+            param_names=param_names,
+            file=file,
+            show=show,
+            title=title,
         )
 
     @staticmethod
     def get_cis_params_mle(
             bootstrap_type: Literal['percentile', 'bca'],
             ci_level: float,
             inferences: List['AbstractInference'],
@@ -249,15 +303,15 @@
     def get_errors_params_mle(
             bootstrap_type: Literal['percentile', 'bca'],
             ci_level: float,
             confidence_intervals: bool,
             inferences: List['AbstractInference'],
             labels: list | np.ndarray,
             param_names: list | np.ndarray
-    ):
+    ) -> (Dict[str, Tuple[np.ndarray, np.ndarray] | None], Dict[str, np.ndarray]):
         """
         Get errors and values for MLE params of inferences.
 
         :param bootstrap_type: Type of bootstrap to use.
         :param ci_level: Confidence level for confidence intervals.
         :param confidence_intervals: Whether to compute confidence intervals.
         :param inferences: List of inference objects.
@@ -397,15 +451,15 @@
 
         :param model: DFE parametrization
         :param params: Parameters of the model
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
         :return: Discretized DFE
         """
         # discrete DFE
-        y = from_string(model)._discretize(params, intervals)
+        y = _from_string(model)._discretize(params, intervals)
 
         # return normalized histogram
         return y / y.sum()
 
 
 class AbstractInference(ABC):
     """
@@ -414,14 +468,16 @@
 
     def __init__(self, **kwargs):
         """
         Initialize the inference.
 
         :param kwargs: Keyword arguments
         """
+        self.logger = logger.getChild(self.__class__.__name__)
+
         self.bootstraps: Optional[pd.DataFrame] = None
         self.params_mle: Optional[dict] = None
         self.model: Optional[Parametrization] = None
 
     @abstractmethod
     def get_bootstrap_params(self) -> Dict[str, float]:
         """
@@ -463,38 +519,41 @@
             file: str = None,
             show: bool = True,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             title: str = 'discretized DFE',
-            ax: plt.Axes = None
+            ax: plt.Axes = None,
+            kwargs_legend: dict = dict(prop=dict(size=8)),
     ) -> plt.Axes:
         """
         Plot discretized DFE.
 
         :param title: Title of the plot
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence interval level
         :param confidence_intervals: Whether to plot confidence intervals
         :param file: File to save the plot to
         :param show: Whether to show the plot
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bars.
         :param ax: Axes to plot to
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes
         """
         return Inference.plot_discretized(
             inferences=[self],
             file=file,
             show=show,
             intervals=intervals,
             confidence_intervals=confidence_intervals,
             ci_level=ci_level,
             bootstrap_type=bootstrap_type,
             title=title,
+            kwargs_legend=kwargs_legend,
             ax=ax
         )
 
     def get_cis_params_mle(
             self,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             ci_level: float = 0.05,
```

### Comparing `fastdfe-0.1.6b0/fastdfe/annotation.py` & `fastdfe-0.1.7b0/fastdfe/annotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """
-VCF annotators.
+VCF annotations and an annotator to apply them.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-05-09"
 
 import logging
 import re
 from abc import ABC
-from collections import Counter
-from functools import cached_property
 from itertools import product
 from typing import List, Optional, Dict
 
 import Bio.Data.CodonTable
 import numpy as np
 import pandas as pd
 from Bio.Seq import Seq
+from Bio.SeqRecord import SeqRecord
 from cyvcf2 import Variant, Writer, VCF
-from pyfaidx import Fasta, FastaRecord
 
-from .vcf import VCFHandler, get_called_bases
+from .bio_handlers import get_major_base, FASTAHandler, GFFHandler, VCFHandler
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 bases = np.array(['G', 'A', 'T', 'C'])
 codon_table = Bio.Data.CodonTable.standard_dna_table.forward_table
 stop_codons = Bio.Data.CodonTable.standard_dna_table.stop_codons
@@ -45,239 +43,218 @@
 
 class Annotation:
 
     def __init__(self):
         """
         Create a new annotation instance.
         """
+        #: The logger.
+        self.logger = logger.getChild(self.__class__.__name__)
+
         #: The annotator.
         self.annotator: Annotator | None = None
 
         #: The number of annotated sites.
         self.n_annotated: int = 0
 
-    def _setup(self, annotator: 'Annotator'):
+    def _setup(self, annotator: 'Annotator', reader: VCF):
         """
         Provide context by passing the annotator. This should be called before the annotation starts.
 
         :param annotator: The annotator.
+        :param reader: The VCF reader.
         """
         self.annotator = annotator
 
-    def _add_info(self, reader: VCF):
-        """
-        Add info fields to the header.
-
-        :param reader: The reader.
-        """
-        pass
-
     def _teardown(self):
         """
         Finalize the annotation. Called after all sites have been annotated.
         """
-        logger.info(type(self).__name__ + f': Annotated {self.n_annotated} sites.')
+        self.logger.info(f'Annotated {self.n_annotated} sites.')
 
     def annotate_site(self, variant: Variant):
         """
         Annotate a single site.
 
         :param variant: The variant to annotate.
         :return: The annotated variant.
         """
         pass
 
     @staticmethod
-    def _load_cds(file: str) -> pd.DataFrame:
+    def count_target_sites(file: str) -> Dict[str, int]:
         """
-        Load coding sequences from a GFF file.
+        Count the number of target sites in a GFF file.
 
         :param file: The path to The GFF file path, possibly gzipped or a URL
-        :return: The DataFrame.
+        :return: The number of target sites per chromosome/contig.
         """
-        # download and unzip if necessary
-        local_file = VCFHandler.unzip_if_zipped(VCFHandler.download_if_url(file))
-
-        # column labels for GFF file
-        col_labels = ['seqid', 'source', 'type', 'start', 'end', 'score', 'strand', 'phase', 'attributes']
-
-        dtypes = dict(
-            seqid='category',
-            type='category',
-            start=int,
-            end=int,
-            strand='category',
-            phase='category'
-        )
-
-        logger.info(f'Loading GFF file.')
-
-        # load GFF file
-        df = pd.read_csv(
-            local_file,
-            sep='\t',
-            comment='#',
-            names=col_labels,
-            dtype=dtypes,
-            usecols=['seqid', 'type', 'start', 'end', 'strand', 'phase']
-        )
-
-        # filter for coding sequences
-        df = df[df['type'] == 'CDS']
-
-        # drop type column
-        df.drop(columns=['type'], inplace=True)
-
-        # sort by seqid and start
-        df.sort_values(by=['seqid', 'start'], inplace=True)
-
-        return df
+        return GFFHandler(file)._count_target_sites()
 
 
 class AncestralAlleleAnnotation(Annotation, ABC):
     """
     Base class for ancestral allele annotation.
     """
 
-    def _add_info(self, reader: VCF):
+    def _setup(self, annotator: 'Annotator', reader: VCF):
         """
         Add info fields to the header.
 
+        :param annotator: The annotator.
         :param reader: The reader.
         """
+        super()._setup(annotator, reader)
+
         reader.add_info_to_header({
             'ID': self.annotator.info_ancestral,
             'Number': '.',
             'Type': 'Character',
             'Description': 'Ancestral Allele'
         })
 
 
 class MaximumParsimonyAnnotation(AncestralAlleleAnnotation):
     """
     Annotation of ancestral alleles using maximum parsimony. The info field ``AA`` is added to the VCF file,
     which holds the ancestral allele. To be used with :class:`~fastdfe.parser.AncestralBaseStratification`.
+
+    Note that maximum parsimony is not a reliable way to determine ancestral alleles, so it is recommended
+    to use this annotation together with the ancestral misidentification parameter ``eps`` or to fold
+    spectra altogether. Alternatively, you can use :class:`~fastdfe.filtration.DeviantOutgroupFiltration` to
+    filter out sites where the major allele among outgroups does not coincide with the major allele among ingroups.
     """
 
+    def __init__(self, samples: List[str] = None):
+        """
+        Create a new ancestral allele annotation instance.
+
+        :param samples: The samples to consider when determining the ancestral allele. If ``None``, all samples are
+
+        """
+        super().__init__()
+
+        #: The samples to consider when determining the ancestral allele.
+        self.samples: List[str] | None = samples
+
+        self.samples_mask: np.ndarray | None = None
+
+    def _setup(self, annotator: 'Annotator', reader: VCF):
+        """
+        Add info fields to the header.
+
+        :param annotator: The annotator.
+        :param reader: The reader.
+        """
+        super()._setup(annotator, reader)
+
+        # create mask for ingroups
+        if self.samples is None:
+            self.samples_mask = np.ones(len(reader.samples)).astype(bool)
+        else:
+            self.samples_mask = np.isin(reader.samples, self.samples)
+
     def annotate_site(self, variant: Variant):
         """
         Annotate a single site.
 
         :param variant: The variant to annotate.
         :return: The annotated variant.
         """
-        # get the called bases
-        b = get_called_bases(variant)
+        # get the major base
+        base = get_major_base(variant.gt_bases[self.samples_mask])
 
-        if len(b) != 0:
-            # get the major allele
-            major_allele = Counter(b).most_common(1)[0][0]
-        else:
-            major_allele = '.'
+        # take base if defined
+        major_allele = base if base is not None else '.'
 
         # set the ancestral allele
         variant.INFO[self.annotator.info_ancestral] = major_allele
 
         # increase the number of annotated sites
         self.n_annotated += 1
 
 
-class DegeneracyAnnotation(Annotation):
+class DegeneracyAnnotation(Annotation, GFFHandler, FASTAHandler):
     """
     Degeneracy annotation. We annotate the degeneracy by looking at each codon for coding variants.
     This also annotates mono-allelic sites.
 
     This annotation adds the info fields ``Degeneracy`` and ``Degeneracy_Info``, which hold the degeneracy
     of a site (0, 2, 4) and extra information about the degeneracy, respectively. To be used with
     :class:`~fastdfe.parser.DegeneracyStratification`.
     """
 
     #: The genomic positions for coding sequences that are mocked.
     _pos_mock: int = 1e100
 
-    def __init__(self, gff_file: str, fasta_file: str, aliases: Dict[str, List[str]] = {}):
+    def __init__(
+            self,
+            gff_file: str,
+            fasta_file: str,
+            aliases: Dict[str, List[str]] = {},
+            cache: bool = True
+    ):
         """
         Create a new annotation instance.
 
         :param gff_file: The GFF file path, possibly gzipped or a URL
         :param fasta_file: The FASTA file path, possibly gzipped or a URL
         :param aliases: Dictionary of aliases for the contigs in the VCF file, e.g. ``{'chr1': ['1']}``.
             This is used to match the contig names in the VCF file with the contig names in the FASTA file and GFF file.
+        :param cache: Whether to cache files that are downloaded from URLs
         """
-        super().__init__()
+        Annotation.__init__(self)
 
-        #: The GFF file.
-        self.gff_file: str = gff_file
+        GFFHandler.__init__(self, gff_file, cache=cache)
 
-        #: The FASTA file.
-        self.fasta_file: str = fasta_file
+        FASTAHandler.__init__(self, fasta_file, cache=cache)
 
         #: Dictionary of aliases for the contigs in the VCF file
         self.aliases: Dict[str, List[str]] = aliases
 
         #: The current coding sequence or the closest coding sequence downstream.
         self.cd: Optional[pd.Series] = None
 
         #: The coding sequence following the current coding sequence.
         self.cd_next: Optional[pd.Series] = None
 
         #: The coding sequence preceding the current coding sequence.
         self.cd_prev: Optional[pd.Series] = None
 
         #: The current contig.
-        self.contig: Optional[FastaRecord] = None
+        self.contig: Optional[SeqRecord] = None
 
         #: The variants that could not be annotated correctly.
         self.mismatches: List[Variant] = []
 
         #: The variant that were skipped because they were not in coding regions.
         self.n_skipped = 0
 
         #: The variants for which the codon could not be determined.
         self.errors: List[Variant] = []
 
-    @cached_property
-    def _ref(self) -> Fasta:
-        """
-        Get the reference reader.
-
-        :return: The reference reader.
-        """
-        return VCFHandler.load_fasta(self.fasta_file)
+        #: The number of sites in coding sequences determined on runtime by looking at the GFF file.
+        self.n_target_sites: int = 0
 
-    @cached_property
-    def _cds(self) -> pd.DataFrame:
-        """
-        The coding sequences.
-
-        :return: The coding sequences.
-        """
-        return Annotation._load_cds(self.gff_file)
-
-    def _setup(self, annotator: 'Annotator'):
+    def _setup(self, annotator: 'Annotator', reader: VCF):
         """
         Provide context to the annotator.
 
         :param annotator: The annotator.
+        :param reader: The reader.
         """
-        super()._setup(annotator)
+        super()._setup(annotator, reader)
 
         # touch the cached properties to make for a nicer logging experience
         # noinspection PyStatementEffect
         self._cds
 
         # noinspection PyStatementEffect
         self._ref
 
-    def _add_info(self, reader: VCF):
-        """
-        Add info fields to the header.
-
-        :param reader: The reader.
-        """
         reader.add_info_to_header({
             'ID': 'Degeneracy',
             'Number': '.',
             'Type': 'Integer',
             'Description': 'n-fold degeneracy'
         })
 
@@ -307,34 +284,33 @@
         # the codon positions
         codon_pos = [codon_start, codon_start + 1, codon_start + 2]
 
         if self.cd_prev is None and codon_pos[0] < self.cd.start:
             raise IndexError(f'Codon at site {variant.CHROM}:{variant.POS} overlaps with '
                              f'start position of current CDS and no previous CDS was given.')
 
-        # We assume here that cd_prev and cd_next have the same orientation
         # Use final positions from previous coding sequence if current codon
         # starts before start position of current coding sequence
         if codon_pos[1] == self.cd.start:
-            codon_pos[0] = self.cd_prev.end
+            codon_pos[0] = self.cd_prev.end if self.cd_prev.strand == '+' else self.cd_prev.start
         elif codon_pos[2] == self.cd.start:
-            codon_pos[1] = self.cd_prev.end
-            codon_pos[0] = self.cd_prev.end - 1
+            codon_pos[1] = self.cd_prev.end if self.cd_prev.strand == '+' else self.cd_prev.start
+            codon_pos[0] = self.cd_prev.end - 1 if self.cd_prev.strand == '+' else self.cd_prev.start + 1
 
         if self.cd_next is None and codon_pos[2] > self.cd.end:
             raise IndexError(f'Codon at site {variant.CHROM}:{variant.POS} overlaps with '
                              f'end position of current CDS and no subsequent CDS was given.')
 
         # use initial positions from subsequent coding sequence if current codon
         # ends before end position of current coding sequence
         if codon_pos[2] == self.cd.end + 1:
-            codon_pos[2] = self.cd_next.start
+            codon_pos[2] = self.cd_next.start if self.cd_next.strand == '+' else self.cd_next.end
         elif codon_pos[1] == self.cd.end + 1:
-            codon_pos[1] = self.cd_next.start
-            codon_pos[2] = self.cd_next.start + 1
+            codon_pos[1] = self.cd_next.start if self.cd_next.strand == '+' else self.cd_next.end
+            codon_pos[2] = self.cd_next.start + 1 if self.cd_next.strand == '+' else self.cd_next.end - 1
 
         # seq uses 0-based positions
         codon = ''.join([str(self.contig[int(pos - 1)]) for pos in codon_pos]).upper()
 
         return codon, codon_pos, codon_start, pos_codon, pos_rel
 
     def _parse_codon_backward(self, variant: Variant):
@@ -356,34 +332,33 @@
         # the codon positions
         codon_pos = [codon_start, codon_start - 1, codon_start - 2]
 
         if self.cd_prev is None and codon_pos[2] < self.cd.start:
             raise IndexError(f'Codon at site {variant.CHROM}:{variant.POS} overlaps with '
                              f'start position of current CDS and no previous CDS was given.')
 
-        # We assume here that cd_prev and cd_next have the same orientation.
         # Use final positions from previous coding sequence if current codon
         # ends before start position of current coding sequence.
         if codon_pos[1] == self.cd.start:
-            codon_pos[2] = self.cd_prev.end
+            codon_pos[2] = self.cd_prev.end if self.cd_prev.strand == '-' else self.cd_prev.start
         elif codon_pos[0] == self.cd.start:
-            codon_pos[1] = self.cd_prev.end
-            codon_pos[2] = self.cd_prev.end - 1
+            codon_pos[1] = self.cd_prev.end if self.cd_prev.strand == '-' else self.cd_prev.start
+            codon_pos[2] = self.cd_prev.end - 1 if self.cd_prev.strand == '-' else self.cd_prev.start + 1
 
         if self.cd_next is None and codon_pos[0] > self.cd.end:
             raise IndexError(f'Codon at site {variant.CHROM}:{variant.POS} overlaps with '
                              f'end position of current CDS and no subsequent CDS was given.')
 
         # use initial positions from subsequent coding sequence if current codon
         # starts before end position of current coding sequence
         if codon_pos[0] == self.cd.end + 1:
-            codon_pos[0] = self.cd_next.start
+            codon_pos[0] = self.cd_next.start if self.cd_next.strand == '-' else self.cd_next.end
         elif codon_pos[1] == self.cd.end + 1:
-            codon_pos[0] = self.cd_next.start + 1
-            codon_pos[1] = self.cd_next.start
+            codon_pos[1] = self.cd_next.start if self.cd_next.strand == '-' else self.cd_next.end
+            codon_pos[0] = self.cd_next.start + 1 if self.cd_next.strand == '-' else self.cd_next.end - 1
 
         # we use 0-based positions here
         codon = ''.join(str(self.contig[int(pos - 1)]) for pos in codon_pos)
 
         # take complement and convert to uppercase ('n' might be lowercase)
         codon = str(Seq(codon).complement()).upper()
 
@@ -444,15 +419,15 @@
         """
         Fetch the coding sequence for the given variant.
 
         :param v: The variant to fetch the coding sequence for.
         :raises LookupError: If no coding sequence was found.
         """
         # get the aliases for the current chromosome
-        aliases = VCFHandler.get_aliases(v.CHROM, self.aliases)
+        aliases = self.get_aliases(v.CHROM, self.aliases)
 
         # only fetch coding sequence if we are on a new chromosome or the
         # variant is not within the current coding sequence
         if self.cd is None or self.cd.seqid not in aliases or v.POS > self.cd.end:
 
             # reset coding sequences to mocking positions
             self.cd_prev = None
@@ -465,18 +440,18 @@
             # filter for positions ending after the variant
             cds = on_contig[(on_contig.end >= v.POS)]
 
             if not cds.empty:
                 # take the first coding sequence
                 self.cd = cds.iloc[0]
 
-                logger.debug(f'Found coding sequence: {self.cd.seqid}:{self.cd.start}-{self.cd.end}, '
-                             f'reminder: {(self.cd.end - self.cd.start + 1) % 3}, '
-                             f'phase: {int(self.cd.phase)}, orientation: {self.cd.strand}, '
-                             f'current position: {v.CHROM}:{v.POS}')
+                self.logger.debug(f'Found coding sequence: {self.cd.seqid}:{self.cd.start}-{self.cd.end}, '
+                                  f'reminder: {(self.cd.end - self.cd.start + 1) % 3}, '
+                                  f'phase: {int(self.cd.phase)}, orientation: {self.cd.strand}, '
+                                  f'current position: {v.CHROM}:{v.POS}')
 
                 # filter for positions ending after the current coding sequence
                 cds = on_contig[(on_contig.start > self.cd.end)]
 
                 if not cds.empty:
                     # take the first coding sequence
                     self.cd_next = cds.iloc[0]
@@ -485,36 +460,40 @@
                 cds = on_contig[(on_contig.end < self.cd.start)]
 
                 if not cds.empty:
                     # take the last coding sequence
                     self.cd_prev = cds.iloc[-1]
 
             if self.cd.start == self._pos_mock and self.n_annotated == 0:
-                logger.warning(f"No coding sequence found on all of contig '{v.CHROM}' and no previous "
-                               f'sites were annotated. Are you sure that this is the correct GFF file '
-                               f'and that the contig names match the chromosome names in the VCF file? '
-                               f'Note that you can also specify aliases for contig names in the VCF file.')
+                self.logger.warning(f"No coding sequence found on all of contig '{v.CHROM}' and no previous "
+                                    f'sites were annotated. Are you sure that this is the correct GFF file '
+                                    f'and that the contig names match the chromosome names in the VCF file? '
+                                    f'Note that you can also specify aliases for contig names in the VCF file.')
 
         # check if variant is located within coding sequence
         if self.cd is None or not (self.cd.start <= v.POS <= self.cd.end):
             raise LookupError(f"No coding sequence found, skipping record {v.CHROM}:{v.POS}")
 
     def _fetch_contig(self, v: Variant):
         """
         Fetch the contig for the given variant.
 
         :param v: The variant to fetch the contig for.
         """
-        aliases = VCFHandler.get_aliases(v.CHROM, self.aliases)
+        aliases = self.get_aliases(v.CHROM, self.aliases)
+
+        # check if contig is up-to-date
+        if self.contig is None or self.contig.id not in aliases:
+            self.logger.debug(f"Fetching contig '{v.CHROM}'.")
 
-        # fetch contig if not up to date
-        if self.contig is None or self.contig.name not in aliases:
-            self.contig = VCFHandler.get_contig(self._ref, aliases)
+            # fetch contig
+            self.contig = self.get_contig(aliases)
 
-            logger.debug(f"Fetching contig '{self.contig.name}'.")
+            # add to number of target sites
+            self.n_target_sites += self._compute_lengths(self._cds[(self._cds.seqid.isin(aliases))])['length'].sum()
 
     def _fetch(self, variant: Variant):
         """
         Fetch all required data for the given variant.
 
         :param variant:
         :raises LookupError: if some data could not be found.
@@ -538,58 +517,62 @@
 
         # skip locus if not a single site
         if len(v.REF) != 1:
             self.n_skipped += 1
             return
 
         # annotate if record is in coding sequence
-        if self.cd.seqid in VCFHandler.get_aliases(v.CHROM, self.aliases) and self.cd.start <= v.POS <= self.cd.end:
+        if self.cd.seqid in self.get_aliases(v.CHROM, self.aliases) and self.cd.start <= v.POS <= self.cd.end:
 
             try:
                 # parse codon
                 codon, codon_pos, codon_start, pos_codon, pos_rel = self._parse_codon(v)
 
             except IndexError as e:
 
                 # skip site on IndexError
-                logger.warning(e)
+                self.logger.warning(e)
                 self.errors.append(v)
                 return
 
             # make sure the reference allele matches with the position on the reference genome
             if str(self.contig[v.POS - 1]).upper() != v.REF.upper():
-                logger.warning(f"Reference allele does not match with reference genome at {v.CHROM}:{v.POS}.")
+                self.logger.warning(f"Reference allele does not match with reference genome at {v.CHROM}:{v.POS}.")
                 self.mismatches.append(v)
                 return
 
             degeneracy = '.'
             if 'N' not in codon:
                 degeneracy = self._get_degeneracy(codon, pos_codon)
 
                 # increment counter of annotated sites
                 self.n_annotated += 1
 
             v.INFO['Degeneracy'] = degeneracy
             v.INFO['Degeneracy_Info'] = f"{pos_codon},{self.cd.strand},{codon}"
 
-            logger.debug(f'pos codon: {pos_codon}, pos abs: {v.POS}, '
-                         f'codon start: {codon_start}, codon: {codon}, '
-                         f'strand: {self.cd.strand}, ref allele: {self.contig[v.POS - 1]}, '
-                         f'degeneracy: {degeneracy}, codon pos: {str(codon_pos)}, '
-                         f'ref allele: {v.REF}')
+            self.logger.debug(f'pos codon: {pos_codon}, pos abs: {v.POS}, '
+                              f'codon start: {codon_start}, codon: {codon}, '
+                              f'strand: {self.cd.strand}, ref allele: {self.contig[v.POS - 1]}, '
+                              f'degeneracy: {degeneracy}, codon pos: {str(codon_pos)}, '
+                              f'ref allele: {v.REF}')
 
 
 class SynonymyAnnotation(DegeneracyAnnotation):
     """
     Synonymy annotation. This class annotates a variant with the synonymous/non-synonymous status.
     Use this when mono-allelic sites are not present in the VCF file.
 
     This annotation adds the info fields ``Synonymous`` and ``Synonymous_Info``, which hold
     the synonymous status (Synonymous (0) or non-synonymous (1)) and the codon information, respectively.
     To be used with :class:`~fastdfe.parser.SynonymyStratification`.
+
+    Note that since we cannot determine the synonymy for monomorphic sites, we determine the number of
+    target sites dynamically by adding up the number of  coding sequences per contig contained in the vcf
+    file. This value is broadcast to :class:`~fastdfe.parser.Parser` if ``n_target_sites`` is not set.
     """
 
     def __init__(self, gff_file: str, fasta_file: str, aliases: Dict[str, List[str]] = {}):
         """
         Create a new annotation instance.
 
         :param gff_file: The GFF file path, possibly gzipped or a URL
@@ -614,20 +597,30 @@
 
         #: The number of sites that were concordant with SnpEff.
         self.n_snpeff_comparisons: int = 0
 
         #: The aliases for the contigs in the VCF file.
         self.aliases: Dict[str, List[str]] = aliases
 
-    def _add_info(self, reader: VCF):
+    def _setup(self, annotator: 'Annotator', reader: VCF):
         """
-        Add the INFO field to the VCF header.
+        Provide context to the annotator.
 
-        :param reader: The VCF reader.
+        :param annotator: The annotator.
+        :param reader: The reader.
         """
+        Annotation._setup(self, annotator, reader)
+
+        # touch the cached properties to make for a nicer logging experience
+        # noinspection PyStatementEffect
+        self._cds
+
+        # noinspection PyStatementEffect
+        self._ref
+
         reader.add_info_to_header({
             'ID': 'Synonymy',
             'Number': '.',
             'Type': 'Integer',
             'Description': 'Synonymous (0) or non-synonymous (1)'
         })
 
@@ -679,56 +672,61 @@
 
         # handle case where there are stop codons
         if codon1 in stop_codons or codon2 in stop_codons:
             return codon1 in stop_codons and codon2 in stop_codons
 
         return codon_table[codon1] == codon_table[codon2]
 
-    @staticmethod
-    def _parse_codons_vep(variant: Variant) -> List[str]:
+    def _parse_codons_vep(self, variant: Variant) -> List[str]:
         """
         Parse the codons from the VEP annotation if present.
 
         :param variant: The variant.
         :return: The codons.
         """
         # match codons
         match = re.search("([actgACTG]{3})/([actgACTG]{3})", variant.INFO.get('CSQ'))
 
         if match is not None:
             if len(match.groups()) != 2:
-                logger.info(f'VEP annotation has more than two codons: {variant.INFO.get("CSQ")}')
+                self.logger.info(f'VEP annotation has more than two codons: {variant.INFO.get("CSQ")}')
 
             return [m.upper() for m in [match[1], match[2]]]
 
         return []
 
     @staticmethod
     def _parse_synonymy_snpeff(variant: Variant) -> int | None:
         """
         Parse the synonymy from the annotation provided by SnpEff
 
         :param variant: The variant.
         :return: The codons.
         """
-        if 'synonymous_variant' in variant.INFO.get('ANN'):
+        ann = variant.INFO.get('ANN')
+
+        if 'synonymous_variant' in ann:
             return 1
 
-        if 'missense_variant' in variant.INFO.get('ANN'):
+        if 'missense_variant' in ann:
             return 0
 
         return None
 
     def _teardown(self):
         """
         Finalize the annotation.
         """
         super()._teardown()
 
-        logger.info(f'Number of mismatches with VEP: {len(self.vep_mismatches)}')
+        if self.n_vep_comparisons != 0:
+            self.logger.info(f'Number of mismatches with VEP: {len(self.vep_mismatches)}')
+
+        if self.n_snpeff_comparisons != 0:
+            self.logger.info(f'Number of mismatches with SnpEff: {len(self.snpeff_mismatches)}')
 
     def annotate_site(self, v: Variant):
         """
         Annotate a single site.
 
         :param v: The variant to annotate.
         :return: The annotated variant.
@@ -748,21 +746,21 @@
                 try:
                     # parse codon
                     codon, codon_pos, codon_start, pos_codon, pos_rel = self._parse_codon(v)
 
                 except IndexError as e:
 
                     # skip site on IndexError
-                    logger.warning(e)
+                    self.logger.warning(e)
                     self.errors.append(v)
                     return
 
                 # make sure the reference allele matches with the position in the reference genome
                 if str(self.contig[v.POS - 1]).upper() != v.REF.upper():
-                    logger.warning(f"Reference allele does not match with reference genome at {v.CHROM}:{v.POS}.")
+                    self.logger.warning(f"Reference allele does not match with reference genome at {v.CHROM}:{v.POS}.")
                     self.mismatches.append(v)
                     return
 
                 # fetch the alternative allele if present
                 alt = self._get_alt_allele(v)
 
                 info = ''
@@ -793,90 +791,92 @@
 
                         if len(codons_vep) > 0:
                             # increase number of comparisons
                             self.n_vep_comparisons += 1
 
                             # make sure the codons determined by VEP are the same as our codons.
                             if set(codons_vep) != {codon, alt_codon}:
-                                logger.warning(f'VEP codons do not match with codons determined by '
-                                               f'codon table for {v.CHROM}:{v.POS}')
+                                self.logger.warning(f'VEP codons do not match with codons determined by '
+                                                    f'codon table for {v.CHROM}:{v.POS}')
 
                                 self.vep_mismatches.append(v)
                                 return
 
                 if v.INFO.get('ANN') is not None:
                     synonymy_snpeff = self._parse_synonymy_snpeff(v)
 
                     self.n_snpeff_comparisons += 1
 
                     if synonymy_snpeff is not None:
                         if synonymy_snpeff != synonymy:
-                            logger.warning(f'SnpEff annotation does not match with custom '
-                                           f'annotation for {v.CHROM}:{v.POS}')
+                            self.logger.warning(f'SnpEff annotation does not match with custom '
+                                                f'annotation for {v.CHROM}:{v.POS}')
 
                             self.snpeff_mismatches.append(v)
                             return
 
                 # increase number of annotated sites
                 self.n_annotated += 1
 
                 # add to info field
                 v.INFO['Synonymy'] = synonymy
                 v.INFO['Synonymy_Info'] = info
 
 
 class Annotator(VCFHandler):
     """
-    Annotator base class.
+    Annotate a VCF file with the given annotations.
     """
 
     def __init__(
             self,
             vcf: str,
             output: str,
             annotations: List[Annotation],
             info_ancestral: str = 'AA',
             max_sites: int = np.inf,
-            seed: int | None = 0
+            seed: int | None = 0,
+            cache: bool = True
     ):
         """
         Create a new annotator instance.
 
         :param vcf: The path to the VCF file, can be gzipped, urls are also supported
         :param output: The path to the output file
         :param annotations: The annotations to apply.
         :param info_ancestral: The tag in the INFO field that contains the ancestral allele
         :param max_sites: Maximum number of sites to consider
-        :param seed: Seed for the random number generator
+        :param seed: Seed for the random number generator. Use ``None`` for no seed.
+        :param cache: Whether to cache files downloaded from urls
         """
         super().__init__(
             vcf=vcf,
             info_ancestral=info_ancestral,
             max_sites=max_sites,
-            seed=seed
+            seed=seed,
+            cache=cache
         )
 
         self.output: str = output
 
         self.annotations: List[Annotation] = annotations
 
     def annotate(self):
         """
         Annotate the VCF file.
         """
         # count the number of sites
         self.n_sites = self.count_sites()
 
         # create the reader
-        reader = VCF(self.vcf)
+        reader = VCF(self.download_if_url(self.vcf))
 
         # provide annotator to annotations and add info fields
         for annotation in self.annotations:
-            annotation._setup(self)
-            annotation._add_info(reader)
+            annotation._setup(self, reader)
 
         # create the writer
         writer = Writer(self.output, reader)
 
         # get progress bar
         with self.get_pbar() as pbar:
```

### Comparing `fastdfe-0.1.6b0/fastdfe/base_inference.py` & `fastdfe-0.1.7b0/fastdfe/base_inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 import pandas as pd
 from matplotlib import pyplot as plt
 from numpy.linalg import norm
 from scipy.optimize._optimize import OptimizeResult
 from scipy.stats import chi2
 from typing_extensions import Self
 
-from . import parametrization, optimization
+from . import optimization
+from . import parametrization
 from .abstract_inference import AbstractInference, Inference
 from .config import Config
 from .discretization import Discretization
 from .json_handlers import CustomEncoder
 from .optimization import Optimization, flatten_dict, pack_params, expand_fixed, unpack_shared
-from .parametrization import Parametrization, from_string
+from .parametrization import Parametrization, _from_string
 from .spectrum import Spectrum, Spectra
 from .spectrum import standard_kingman
 from .visualization import Visualization
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
@@ -131,15 +132,15 @@
             used.
         :param intervals_del: ``(start, stop, n_interval)`` for deleterious population-scaled
             selection coefficients. The intervals will be log10-spaced.
         :param integration_mode: Integration mode for the DFE, ``quad`` not recommended
         :param linearized: Whether to use the linearized DFE, ``False`` not recommended
         :param intervals_ben: Same as for intervals_del but for beneficial selection coefficients.
         :param model: Instance of DFEParametrization which parametrized the DFE
-        :param seed: Seed for the random number generator.
+        :param seed: Seed for the random number generator. Use ``None`` for no seed.
         :param x0: Dictionary of initial values in the form ``{'all': {param: value}}``
         :param bounds: Bounds for the optimization in the form ``{param: (lower, upper)}``
         :param scales: Scales for the optimization in the form ``{param: scale}`
         :param loss_type: Type of loss function to use for optimization.
         :param opts_mle: Options for the optimization.
         :param n_runs: Number of independent optimization runs out of which the best one is chosen. The first run
             will use the initial values if specified. Consider increasing this number if the optimization does not
@@ -175,15 +176,15 @@
 
         # check that we have monomorphic counts
         if self.sfs_neut.to_list()[0] == 0 or self.sfs_sel.to_list()[0] == 0:
             raise ValueError('Some of the provided SFS have zero ancestral monomorphic counts. '
                              'Note that we require monomorphic counts in order to infer the mutation rate.')
 
         #: The DFE parametrization
-        self.model: Parametrization = parametrization.from_string(model)
+        self.model: Parametrization = parametrization._from_string(model)
 
         if folded is None:
             #: Whether the SFS are folded
             self.folded: bool = self.sfs_sel.is_folded() and self.sfs_neut.is_folded()
         else:
             self.folded = folded
 
@@ -206,15 +207,15 @@
             self.discretization: Discretization = discretization
 
         #: Estimate of theta from neutral SFS
         self.theta: float = self.sfs_neut.theta
 
         # raise warning if theta is unusually large
         if self.theta > 0.05 or self.sfs_sel.theta > 0.05:
-            logger.warning("Mutation rate is unusually highly. This is a reminder to provide monomorphic counts.")
+            self.logger.warning("Mutation rate is unusually highly. This is a reminder to provide monomorphic counts.")
 
         #: MLE estimates of the initial optimization
         self.params_mle: Optional[Dict[str, float]] = None
 
         #: Modelled MLE SFS
         self.sfs_mle: Optional[Spectrum] = None
 
@@ -274,17 +275,17 @@
 
         # warn if folded is true, and we estimate the full DFE
         if self.folded:
             fixed_dele = set(self.model.submodels['dele'].keys()) if 'dele' in self.model.submodels else set()
             fixed = set(self.fixed_params['all'].keys()) if 'all' in self.fixed_params else set()
 
             if not fixed_dele.issubset(fixed):
-                logger.warning("You are estimating the full DFE, but the SFS are folded. "
-                               "This is not recommend as the folded SFS contains little information "
-                               "on beneficial mutations.")
+                self.logger.warning("You are estimating the full DFE, but the SFS are folded. "
+                                    "This is not recommend as the folded SFS contains little information "
+                                    "on beneficial mutations.")
 
         #: Initial values
         self.x0 = dict(all=self.model.x0 | self.default_x0 | (x0['all'] if 'all' in x0 else {}))
 
         #: Bootstrapped MLE parameter estimates
         self.bootstraps: Optional[pd.DataFrame] = None
 
@@ -344,19 +345,19 @@
         Run if not run yet.
 
         :param args: Arguments.
         :param kwargs: Keyword arguments.
         :return: DFE parametrization and modelled SFS.
         """
         if self.execution_time == 0:
-            logger.debug('Inference needs to be run first, triggering run.')
+            self.logger.debug('Inference needs to be run first, triggering run.')
 
             return self.run(*args, **kwargs)
 
-        logger.debug('Inference already run, not running again.')
+        self.logger.debug('Inference already run, not running again.')
 
     @staticmethod
     def run_if_required_wrapper(func):
         """
         Decorator to run inference if required.
 
         :param func: Function to decorate.
@@ -402,32 +403,33 @@
 
         # update properties
         self.update_properties(
             do_bootstrap=do_bootstrap
         )
 
         # perform MLE
-        logger.info(f'Starting numerical optimization of {self.n_runs} '
-                    'independently initialized samples which are run ' +
-                    ('in parallel.' if self.parallelize else 'sequentially.'))
+        self.logger.debug(f'Starting numerical optimization of {self.n_runs} '
+                         'independently initialized samples which are run ' +
+                         ('in parallel.' if self.parallelize else 'sequentially.'))
 
         # Access cached property to trigger potential pre-computation
         # of linearization. This is necessary if the optimization is
         # parallelized so that the pre-computation does not have to be
         # performed in each thread.
         _ = self.discretization.dfe_to_sfs
 
         # perform numerical minimization
         result, params_mle = self.optimization.run(
             x0=self.x0,
             scales=self.scales,
             bounds=self.bounds,
             get_counts=self.get_counts(),
             n_runs=self.n_runs,
-            pbar=pbar
+            pbar=pbar,
+            desc='Performing inference'
         )
 
         # assign likelihoods
         self.likelihoods = self.optimization.likelihoods
 
         # unpack shared parameters
         params_mle = unpack_shared(params_mle)
@@ -501,34 +503,33 @@
 
         # create spectrum object from polymorphic counts
         self.sfs_mle = Spectrum.from_polymorphic(counts_mle)
 
         # L2 norm of fit minus observed SFS
         self.L2_residual = norm(self.sfs_mle.polymorphic - self.sfs_sel.polymorphic, 2)
 
-    @staticmethod
-    def report_result(result: OptimizeResult, params: dict):
+    def report_result(self, result: OptimizeResult, params: dict):
         """
         Inform on optimization result.
 
         :param params: MLE parameters.
         :param result: Optimization result.
         """
         # report on optimization result
         if result.success:
-            logger.info(f"Successfully finished optimization after {result.nit} iterations "
-                        f"and {result.nfev} function evaluations, obtaining a log-likelihood "
-                        f"of -{result.fun}.")
+            self.logger.info(f"Successfully finished optimization after {result.nit} iterations "
+                             f"and {result.nfev} function evaluations, obtaining a log-likelihood "
+                             f"of -{result.fun}.")
         else:
-            logger.warning("Numerical optimization did not terminate normally, so "
-                           "the result might be compromised. Consider adjusting "
-                           "the optimization parameters (increasing `gtol` or `n_runs`) "
-                           "or decrease the number of optimized parameters.")
+            self.logger.warning("Numerical optimization did not terminate normally, so "
+                                "the result might be compromised. Consider adjusting "
+                                "the optimization parameters (increasing `gtol` or `n_runs`) "
+                                "or decrease the number of optimized parameters.")
 
-        logger.info(f"Inferred parameters: {flatten_dict(params)}.")
+        self.logger.info(f"Inferred parameters: {flatten_dict(params)}.")
 
     def update_properties(self, **kwargs) -> Self:
         """
         Update the properties of this class with the given dictionary
         given that its entries are not None.
 
         :param kwargs: Dictionary of properties to update.
@@ -537,24 +538,27 @@
         for key, value in kwargs.items():
             if value is not None:
                 setattr(self, key, value)
 
         return self
 
     def bootstrap(
-            self, n_samples: int = None,
+            self,
+            n_samples: int = None,
             parallelize: bool = None,
-            update_likelihood: bool = True
+            update_likelihood: bool = True,
+            pbar: bool = True
     ) -> pd.DataFrame:
         """
         Perform the parametric bootstrap.
 
         :param n_samples: Number of bootstrap samples.
         :param parallelize: Whether to parallelize the bootstrap.
         :param update_likelihood: Whether to update the likelihood to be the mean of the bootstrap samples.
+        :param pbar: Whether to show a progress bar.
         :return: Dataframe with bootstrap results.
         """
         # check if locked
         self.raise_if_locked()
 
         # perform inference first if not done yet
         self.run_if_required()
@@ -566,44 +570,45 @@
         )
 
         start_time = time.time()
 
         # parallelize computations if desired
         if self.parallelize:
 
-            logger.info(f"Running {self.n_bootstraps} bootstrap samples "
-                        f"in parallel on {mp.cpu_count()} cores.")
+            self.logger.debug(f"Running {self.n_bootstraps} bootstrap samples "
+                              f"in parallel on {min(mp.cpu_count(), self.n_bootstraps)} cores.")
 
             # We need to assign new random states to the subprocesses.
             # Otherwise, they would all produce the same result.
             seeds = self.rng.integers(0, high=2 ** 32, size=self.n_bootstraps)
 
         else:
-            logger.info(f"Running {self.n_bootstraps} bootstrap samples sequentially.")
+            self.logger.debug(f"Running {self.n_bootstraps} bootstrap samples sequentially.")
 
             seeds = [None] * self.n_bootstraps
 
         # run bootstraps
         result = optimization.parallelize(
             func=self.run_bootstrap_sample,
             data=seeds,
             parallelize=self.parallelize,
-            pbar=True
+            pbar=pbar,
+            desc='Bootstrapping'
         )
 
         # number of successful runs
         n_success = np.sum([res.success for res in result[:, 0]])
 
         # issue warning if some runs did not finish successfully
         if n_success < self.n_bootstraps:
-            logger.warning(f"{self.n_bootstraps - n_success} out of {self.n_bootstraps} bootstrap samples "
-                           "did not terminate normally during numerical optimization. "
-                           "The confidence intervals might thus be unreliable. Consider adjusting "
-                           "the optimization parameters (increasing `gtol` or `n_runs`) "
-                           "or decrease the number of optimized parameters.")
+            self.logger.warning(f"{self.n_bootstraps - n_success} out of {self.n_bootstraps} bootstrap samples "
+                                "did not terminate normally during numerical optimization. "
+                                "The confidence intervals might thus be unreliable. Consider adjusting "
+                                "the optimization parameters (increasing `gtol` or `n_runs`) "
+                                "or decrease the number of optimized parameters.")
 
             # dataframe of MLE estimates
         self.bootstraps = pd.DataFrame([r['all'] for r in result[:, 1]])
 
         # assign bootstrap results
         self.bootstrap_results = list(result[:, 0])
 
@@ -619,15 +624,15 @@
 
         return self.bootstraps
 
     def add_alpha_to_bootstraps(self):
         """
         Add estimates for alpha to the bootstraps.
         """
-        logger.debug('Computing estimates for alpha.')
+        self.logger.debug('Computing estimates for alpha.')
 
         # add alpha estimates
         self.bootstraps['alpha'] = self.bootstraps.apply(lambda r: self.get_alpha(dict(r)), axis=1)
 
     def resample_sfs(self, sfs: Spectrum, seed: int = None) -> Spectrum:
         """
         Resample SFS assuming independent Poisson counts.
@@ -670,15 +675,16 @@
             n_runs=1,
             debug_iterations=False,
             print_info=False,
             get_counts=dict(all=lambda params: self.model_sfs(
                 params,
                 sfs_neut=sfs_neut,
                 sfs_sel=sfs_sel
-            ))
+            )),
+            desc='Bootstrapping'
         )
 
         # unpack shared parameters
         params_mle = unpack_shared(params_mle)
 
         # normalize MLE estimates
         params_mle['all'] = self.model._normalize(params_mle['all'])
@@ -784,14 +790,15 @@
             intervals: np.ndarray = None,
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             scale_density: bool = False,
             scale: Literal['lin', 'log', 'symlog'] = 'lin',
             title: str = 'DFE',
+            kwargs_legend: dict = dict(prop=dict(size=8)),
             ax: plt.Axes = None
 
     ) -> plt.Axes:
         """
         Plot continuous DFE.
         The special constants np.inf and -np.inf are also valid interval bounds.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
@@ -806,14 +813,15 @@
         :param ci_level: Confidence level for confidence intervals.
         :param confidence_intervals: Whether to plot confidence intervals.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param scale: y-scale
         :param scale_density: Whether to scale the density by the x-axis interval size
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :param ax: Axes object to plot on.
         :return: Axes object
         """
         if intervals is None:
             intervals = self.discretization.bins
 
         return Inference.plot_continuous(
@@ -823,14 +831,15 @@
             intervals=intervals,
             confidence_intervals=confidence_intervals,
             ci_level=ci_level,
             bootstrap_type=bootstrap_type,
             title=title,
             scale=scale,
             scale_density=scale_density,
+            kwargs_legend=kwargs_legend,
             ax=ax
         )
 
     @run_if_required_wrapper
     def plot_bucket_sizes(
             self,
             file: str = None,
@@ -884,56 +893,68 @@
         :param interval_labels: Labels for the intervals.
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
         :param ax: Axes object to plot on.
         :return: Axes object
         """
         # issue warning
         if not self.discretization.linearized:
-            logger.warning('Note that the interval density is not important if the DFE was not linearized.')
+            self.logger.warning('Note that the interval density is not important if the DFE was not linearized.')
 
         return Visualization.plot_interval_density(
             density=self.discretization.get_interval_density(intervals),
             **locals()
         )
 
     def plot_sfs_comparison(
             self,
-            types: List[Literal['modelled', 'observed', 'modelled', 'neutral']] = ['modelled', 'observed'],
+            sfs_types: List[Literal['modelled', 'observed', 'modelled', 'neutral']] = ['modelled', 'observed'],
             labels: List[str] = None,
             file: str = None,
             show: bool = True,
-            ax: plt.Axes = None
+            ax: plt.Axes = None,
+            title: str = 'SFS comparison',
+            use_subplots: bool = False,
+            show_monomorphic: bool = False,
+            kwargs_legend: dict = dict(prop=dict(size=8)),
 
     ) -> plt.Axes:
         """
         Plot SFS comparison.
 
         :param file: File to save plot to.
         :param labels: Labels for the SFS.
-        :param types: Types of SFS to plot.
+        :param sfs_types: Types of SFS to plot.
         :param show: Whether to show plot.
         :param ax: Axes object to plot on.
+        :param title: Plot title
+        :param use_subplots: Whether to use subplots
+        :param show_monomorphic: Whether to show monomorphic counts
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes object
         """
-        if 'modelled' in types:
+        if 'modelled' in sfs_types:
             self.run_if_required()
 
         mapping = dict(
             observed=self.sfs_sel,
             selected=self.sfs_sel,
             modelled=self.sfs_mle,
             neutral=self.sfs_neut
         )
 
         return Visualization.plot_sfs_comparison(
-            spectra=[mapping[t] for t in types],
-            labels=types if labels is None else labels,
+            spectra=[mapping[t] for t in sfs_types],
+            labels=sfs_types if labels is None else labels,
             file=file,
             show=show,
-            ax=ax
+            ax=ax,
+            title=title,
+            use_subplots=use_subplots,
+            show_monomorphic=show_monomorphic,
+            kwargs_legend=kwargs_legend
         )
 
     def plot_observed_sfs(
             self,
             labels: List[str] = None,
             file: str = None,
             show: bool = True,
@@ -946,25 +967,25 @@
         :param file: File to save plot to.
         :param labels: Labels for the SFS.
         :param show: Whether to show plot.
         :param ax: Axes object to plot on.
         :return: Axes object
         """
         return self.plot_sfs_comparison(
-            types=['neutral', 'selected'],
+            sfs_types=['neutral', 'selected'],
             labels=labels,
             file=file,
             show=show,
             ax=ax
         )
 
     @run_if_required_wrapper
     def plot_all(self, show: bool = True):
         """
-        Plot everything.
+        Plot a bunch of plots.
 
         :param show: Whether to show plot.
         """
         self.plot_inferred_parameters(show=show)
         self.plot_discretized(show=show)
         self.plot_sfs_comparison(show=show)
         self.plot_continuous(show=show)
@@ -1002,55 +1023,83 @@
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             scale: Literal['lin', 'log', 'symlog'] = 'log',
             legend: bool = True,
             ax: plt.Axes = None,
+            kwargs_legend: dict = dict(prop=dict(size=8), loc='upper right'),
             **kwargs
     ) -> plt.Axes:
         """
         Visualize the inferred parameters and their confidence intervals.
 
         :param scale: y-scale of the plot.
         :param title: Plot title.
         :param legend: Whether to show the legend.
         :param confidence_intervals: Whether to show confidence intervals.
         :param bootstrap_type: Type of bootstrap to use.
         :param ci_level: Confidence level for the confidence intervals.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param ax: Axes object to plot on.
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes object
         """
         return Inference.plot_inferred_parameters(
             inferences=[self],
             labels=['all'],
             file=file,
             show=show,
             title=title,
             ci_level=ci_level,
             confidence_intervals=confidence_intervals,
             bootstrap_type=bootstrap_type,
             scale=scale,
-            ax=ax
+            ax=ax,
+            kwargs_legend=kwargs_legend,
+        )
+
+    @run_if_required_wrapper
+    def plot_inferred_parameters_boxplot(
+            self,
+            file: str = None,
+            show: bool = True,
+            title: str = 'parameter estimates',
+            **kwargs
+    ) -> plt.Axes:
+        """
+        Visualize the inferred parameters and their confidence intervals.
+
+        :param title: Plot title.
+        :param file: File to save plot to.
+        :param show: Whether to show plot.
+        :return: Axes object
+        :raises ValueError: If no inference objects are given or no bootstraps are found.
+        """
+        return Inference.plot_inferred_parameters_boxplot(
+            inferences=[self],
+            labels=['all'],
+            file=file,
+            show=show,
+            title=title
         )
 
     @run_if_required_wrapper
     def plot_likelihoods(
             self,
             file: str = None,
             show: bool = True,
             title: str = 'likelihoods',
-            scale: Literal['lin', 'log', 'symlog'] = 'lin',
+            scale: Literal['lin', 'log'] = 'lin',
             ax: plt.Axes = None,
             **kwargs
     ) -> plt.Axes:
         """
-        Visualize the likelihoods of the optimization runs.
+        Visualize the likelihoods of the optimization runs using a scatter plot.
 
         :param scale: y-scale of the plot.
         :param title: Plot title.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param ax: Axes object to plot on.
         :return: Axes object
@@ -1060,30 +1109,29 @@
             file=file,
             show=show,
             title=title,
             scale=scale,
             ax=ax
         )
 
-    @staticmethod
-    def lrt(ll_simple: float, ll_complex: float, df: int = 1) -> float:
+    def lrt(self, ll_simple: float, ll_complex: float, df: int = 1) -> float:
         """
         Perform the likelihood ratio test (LRT).
 
         :param ll_simple: Log-likelihood of the simple model.
         :param ll_complex: Log-likelihood of the complex model.
         :param df: Degrees of freedom.
         :return: p-value
         """
         lr = -2 * (ll_simple - ll_complex)
 
         # issue info message
-        logger.info(f"Simple model likelihood: {ll_simple}, "
-                    f"complex model likelihood: {ll_complex}, "
-                    f"degrees of freedom: {df}.")
+        self.logger.info(f"Simple model likelihood: {ll_simple}, "
+                         f"complex model likelihood: {ll_complex}, "
+                         f"degrees of freedom: {df}.")
 
         return chi2.sf(lr, df)
 
     def compare_nested_likelihoods(self, complex: 'BaseInference') -> float | None:
         """
         Perform likelihood ratio test with given more complex model.
         The given model's fixed parameters need to be a proper
@@ -1113,15 +1161,15 @@
         model using likelihood ratio tests.
 
         :param do_bootstrap: Whether to perform bootstrapping. This is recommended to get more accurate p-values.
         :return: Matrix of p-values, dict of base inference objects
         """
 
         # get sub-model specifications
-        submodels_dfe = from_string(self.model).submodels
+        submodels_dfe = _from_string(self.model).submodels
         submodels_outer = dict(
             no_anc=dict(eps=0),
             anc={}
         )
 
         # take outer product to get fixed parameters for each model
         inferences: Dict[str, BaseInference] = {}
@@ -1135,15 +1183,15 @@
             # dict of params to be fixed
             params = dict(all=submodels_dfe[p[0]] | submodels_outer[p[1]])
 
             # assign fixed parameters
             inference._set_fixed_params(params)
 
             # inform about fixed parameters
-            logger.info(f'Holding parameters fixed to {params}.')
+            self.logger.info(f'Holding parameters fixed to {params}.')
 
             # run inference
             inference.run()
 
             # define name
             name = '.'.join(p).rstrip('_')
```

### Comparing `fastdfe-0.1.6b0/fastdfe/bootstrap.py` & `fastdfe-0.1.7b0/fastdfe/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import logging
 from typing import Literal
 
 import numpy as np
 from scipy.stats import norm as normal
 
 # get logger
-logger = logging.getLogger('fastdfe')
+logger = logging.getLogger('fastdfe').getChild('Bootstrap')
 
 
 class Bootstrap:
     """
     Bootstrap utilities.
     """
```

### Comparing `fastdfe-0.1.6b0/fastdfe/config.py` & `fastdfe-0.1.7b0/fastdfe/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 from typing import List, Literal, Dict, Tuple
 
 import yaml
 
 from .json_handlers import CustomEncoder
 from .optimization import Covariate
 from .optimization import SharedParams, merge_dicts
-from .parametrization import Parametrization, from_string, to_string
+from .parametrization import Parametrization, _from_string, _to_string
 from .polydfe_utils import create_sfs_config, parse_init_file, create_init_file, models
-from .spectrum import Spectra, parse_polydfe_sfs_config
+from .spectrum import Spectra, parse_polydfe_sfs_config, Spectrum
 
-logger = logging.getLogger('fastdfe')
+logger = logging.getLogger('fastdfe').getChild('Config')
 
 
 class Config:
     """
     Configuration class to be used for :class:`~fastdfe.base_inference.BaseInference` and
     :class:`fastdfe.joint_inference.JointInference`.
     """
 
     def __init__(
             self,
             polydfe_spectra_config: str = None,
             polydfe_init_file: str = None,
             polydfe_init_file_id: int = 1,
-            sfs_neut: Spectra = None,
-            sfs_sel: Spectra = None,
+            sfs_neut: Spectra | Spectrum = None,
+            sfs_sel: Spectra | Spectrum = None,
             intervals_del: (float, float, int) = (-1.0e+8, -1.0e-5, 1000),
             intervals_ben: (float, float, int) = (1.0e-5, 1.0e4, 1000),
             integration_mode: Literal['midpoint', 'quad'] = 'midpoint',
             linearized: bool = True,
             model: Parametrization | str = 'GammaExpParametrization',
             seed: int = 0,
             x0: Dict[str, Dict[str, float]] = {},
@@ -66,15 +66,15 @@
         :param sfs_sel: Selected SFS. Note that we require monomorphic counts to be specified in order to infer
             the mutation rate.
         :param intervals_del: Integration intervals for deleterious mutations in log space.
         :param intervals_ben: Integration intervals for beneficial mutations in log space.
         :param integration_mode: Integration mode, ``quad`` not recommended
         :param linearized: Whether to use the linearized version of the DFE, ``False`` not recommended.
         :param model: Parametrization of the DFE.
-        :param seed: Seed for the random number generator.
+        :param seed: Seed for the random number generator. Use ``None`` for no seed.
         :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
         :param bounds: Bounds for the optimization in the form {param: (lower, upper)}
         :param scales: Scales for the optimization in the form {param: scale}
         :param loss_type: Loss function to use.
         :param opts_mle: Options for the optimization.
         :param n_runs: Number of independent optimization runs out of which the best one is chosen. The first run
             will use the initial values if specified. Consider increasing this number if the optimization does not
@@ -100,16 +100,16 @@
             n_runs=n_runs,
             x0=x0,
             bounds=bounds,
             scales=scales,
             fixed_params=fixed_params,
             shared_params=shared_params,
             covariates=covariates,
-            sfs_neut=sfs_neut,
-            sfs_sel=sfs_sel,
+            sfs_neut=Spectra.from_spectrum(sfs_neut) if isinstance(sfs_neut, Spectrum) else sfs_neut,
+            sfs_sel=Spectra.from_spectrum(sfs_sel) if isinstance(sfs_sel, Spectrum) else sfs_sel,
             do_bootstrap=do_bootstrap,
             n_bootstraps=n_bootstraps,
             parallelize=parallelize,
             loss_type=loss_type
         )
 
         # parse spectra file if specified
@@ -123,29 +123,34 @@
     def update(self, **kwargs) -> 'Config':
         """
         Update config with given data.
 
         :param kwargs: Data to update.
         :return: Updated config.
         """
+        # convert spectrum to spectra objects
+        for key in ['sfs_neut', 'sfs_sel']:
+            if key in kwargs and isinstance(kwargs[key], Spectrum):
+                kwargs[key] = Spectra.from_spectrum(kwargs[key])
+
         self.data |= kwargs
 
         return self
 
     def parse_polydfe_init_file(self, file: str, id: int = 1, type='all'):
         """
         Parse polyDFE init file.
         This will define the initial parameters and
         which ones will be held fixed during the optimization.
 
         :param type: Type of parameters to parse for.
         :param id: ID of the init file.
         :param file: Path to the init file.
         """
-        fixed_params, x0 = parse_init_file(from_string(self.data['model']).param_names, file, id)
+        fixed_params, x0 = parse_init_file(_from_string(self.data['model']).param_names, file, id)
 
         # merge with existing config
         self.data['fixed_params'] = merge_dicts(self.data['fixed_params'], dict(all=fixed_params))
         self.data['x0'] |= {type: x0}
 
     def create_polydfe_init_file(self, file: str, n: int, type: str = 'all'):
         """
@@ -153,17 +158,17 @@
 
         :param type: Type to use for the init file.
         :param n: SFS samples size.
         :param file: Path to the init file to be created.
         """
         create_init_file(
             file=file,
-            fixed_params=list(self.data['fixed_params'][type].keys()),
+            fixed_params=list(self.data['fixed_params'][type].keys()) if type in self.data['fixed_params'] else [],
             x0=self.data['x0'][type] if type in self.data['x0'] else {},
-            dfe_params=from_string(self.data['model']).param_names,
+            dfe_params=_from_string(self.data['model']).param_names,
             n=n
         )
 
     def parse_polydfe_sfs_config(self, file: str):
         """
         Parse frequency spectra and mutational target site from
         polyDFE configuration file.
@@ -182,16 +187,16 @@
         """
         Create a sfs config file for polyDFE.
 
         :param file: Path to the sfs config file to be created.
         """
         create_sfs_config(
             file=file,
-            sfs_neut=self.data['sfs_neut']['all'],
-            sfs_sel=self.data['sfs_sel']['all']
+            sfs_neut=self.data['sfs_neut'].all if isinstance(self.data['sfs_neut'], Spectra) else self.data['sfs_neut'],
+            sfs_sel=self.data['sfs_sel'].all if isinstance(self.data['sfs_sel'], Spectra) else self.data['sfs_sel']
         )
 
     def to_dict(self) -> dict:
         """
         Represent config as dictionary.
 
         :return: Dictionary representation of config.
@@ -286,15 +291,15 @@
         """
         Get the model name in polyDFE that corresponds
         to the configured DFE parametrization.
 
         :return: polyDFE model name.
         """
         # get name of configured model
-        name = to_string(self.data['model'])
+        name = _to_string(self.data['model'])
 
         # return polyDFE model name if it exists
         if name in models:
             return models[name]
 
         # raise error otherwise
         raise NotImplementedError(f'There is no polyDFE equivalent of {name}')
```

### Comparing `fastdfe-0.1.6b0/fastdfe/discretization.py` & `fastdfe-0.1.7b0/fastdfe/discretization.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import mpmath as mp
 import numpy as np
 from scipy.integrate import quad
 
 from fastdfe import Parametrization
 
 # configure logger
-logger = logging.getLogger('fastdfe')
+logger = logging.getLogger('fastdfe').getChild('Discretization')
 
 
 def get_midpoints_and_spacing(bins: np.ndarray) -> (np.ndarray, np.ndarray):
     """
     Obtain midpoints and spacing for the given bins.
 
     :param bins: Array of bins
@@ -100,15 +100,15 @@
     :return: Sojourn time as x -> 1
     """
     return S / (1 - np.exp(-S))
 
 
 def H_fixed_regularized(S: float | int | np.ndarray) -> float | int | np.ndarray:
     """
-    As H_fixed but replacing with the limits close to the limit points.
+    As :func:`H_fixed` but replacing with the limits close to the limit points.
 
     :param S: Selection coefficient
     :return: Sojourn time as x -> 1
     """
     # make it accept scalars
     if isinstance(S, (float, int)):
         return H_fixed(np.array([S]))[0]
@@ -314,25 +314,25 @@
             return self.get_dfe_to_sfs_quad()
 
         raise NotImplementedError(f'Integration mode {self.integration_mode} not supported.')
 
     @to_float
     def get_allele_count_large_negative_S(self, S: float | np.ndarray, k: float | np.ndarray) -> np.ndarray | float:
         """
-        Same as get_allele_count but performing the division on the log scale.
+        Limit of get_allele_count for large negative S.
 
         :param S: Population-scaled selection coefficient
         :param k: Allele count
         :return: Number of counts in frequency class P(k)
         """
         return self.n / (k * (self.n - k)) * hyp1f1(k, self.n, S)
 
     def get_allele_count_large_positive_S(self, S: float | np.ndarray, k: float | np.ndarray) -> np.ndarray | float:
         """
-        Limit of get_allele_count for S >> 0.
+        Limit of get_allele_count for large positive S.
 
         :param S: Population-scaled selection coefficient
         :param k: Allele count
         :return: Number of counts in frequency class P(k)
         """
         return self.n / (k * (self.n - k))
 
@@ -348,34 +348,35 @@
         :param k: Allele count
         :return: Number of counts in frequency class P(k)
         """
         return (self.n / (k * (self.n - k))) * ((1 - exp(-S) * hyp1f1(k, self.n, S)) / (1 - exp(-S)))
 
     def get_allele_count_regularized(self, S: float | np.ndarray, k: float | np.ndarray) -> float | np.ndarray:
         """
-        As get_allele_count(S, k) but using the respective limits
-        for S close to zero and S very negative.
-        Note that S and k need to have the same shape due to
-        the conditioning.
+        As :meth:`get_allele_count` but using the respective limits
+        for ``S`` close to zero and ``S`` very negative.
+        Note that ``S`` and ``k`` need to have the same shape.
 
         :param S: Population-scaled selection coefficient
         :param k: Allele count
-        :return: Number of counts in frequency class P(k)
+        :return: Number of counts in frequency class ``P(k)`
         """
         # make it accept scalars for S
         if isinstance(S, (float, int)):
             return self.get_allele_count_regularized(np.array([S]), np.array([k]))[0]
 
         # else S is an array
         y = np.zeros_like(S, dtype=float)
 
         # S close to zero
         close_to_zero = np.abs(S) < 1e-8
 
         # simply take limit value as S -> 0
+        # see https://www.wolframalpha.com/input?i=limit+of+%5Cfrac%7B1-e%5E%7B-S%281-x%29%7D%7D%7Bx%281-
+        # x%29%281-e%5E%7B-S%7D%29%7D+as+S+-%3E+0
         if close_to_zero.any():
             y[close_to_zero] = np.ones_like(S[close_to_zero]) / k[close_to_zero]
 
         # large negative S
         very_negative = S < -1e4
 
         # Evaluate using limit.
```

### Comparing `fastdfe-0.1.6b0/fastdfe/filtration.py` & `fastdfe-0.1.7b0/fastdfe/filtration.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """
-VCF filters.
+VCF filtrations and a filterer to apply them.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-05-11"
 
+import functools
 import logging
-from functools import cached_property
 from typing import Iterable, List, Optional, Callable, Dict
 
 import numpy as np
 import pandas as pd
 from cyvcf2 import Variant, Writer, VCF
 
-from .annotation import Annotation, DegeneracyAnnotation
-from .vcf import VCFHandler
+from .annotation import DegeneracyAnnotation
+from .bio_handlers import get_major_base, GFFHandler, VCFHandler
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
-def count_filtered(func: Callable) -> Callable:
+def _count_filtered(func: Callable) -> Callable:
     """
     Decorator that increases ``self.n_filtered`` by 1 if the decorated function returns False.
     """
 
+    @functools.wraps(func)
     def wrapper(self, variant):
         result = func(self, variant)
         if not result:
             self.n_filtered += 1
         return result
 
     return wrapper
@@ -39,139 +40,177 @@
     """
     Base class for filtering sites based on certain criteria.
     """
 
     #: The number of sites that didn't pass the filter.
     n_filtered: int = 0
 
-    @count_filtered
+    def __init__(self):
+        """
+        Initialize filtration.
+        """
+        self.logger = logger.getChild(self.__class__.__name__)
+
+    @_count_filtered
     def filter_site(self, variant: Variant) -> bool:
         """
         Filter site.
 
         :param variant: The variant to filter.
         :return: ``True`` if the variant should be kept, ``False`` otherwise.
         """
         pass
 
-    def _setup(self):
+    def _setup(self, reader: VCF):
         """
         Perform any necessary pre-processing. This method is called before the actual filtration.
+
+        :param reader: The VCF reader.
         """
         pass
 
     def _teardown(self):
         """
         Perform any necessary post-processing. This method is called after the actual filtration.
         """
-        logger.info(type(self).__name__ + f": Filtered out {self.n_filtered} sites.")
+        self.logger.info(f"Filtered out {self.n_filtered} sites.")
 
 
 class SNPFiltration(Filtration):
     """
-    Only keep SNPs (discard monomorphic sites).
+    Only keep SNPs. Note that this includes discarding mono-morphic sites.
     """
 
-    @count_filtered
+    @_count_filtered
     def filter_site(self, variant: Variant) -> bool:
         """
         Filter site.
 
         :param variant: The variant to filter.
         :return: ``True`` if the variant is an SNP, ``False`` otherwise.
         """
         return variant.is_snp
 
 
 class SNVFiltration(Filtration):
     """
-    Only keep single site variants (discardi indels and MNPs but keep monomorphic sites).
+    Only keep single site variants (discard indels and MNPs but keep monomorphic sites).
     """
 
-    @count_filtered
+    @_count_filtered
     def filter_site(self, variant: Variant) -> bool:
         """
         Filter site.
 
         :param variant: The variant to filter.
         :return: ``True`` if the variant is kept, ``False`` otherwise.
         """
-        return len(variant.REF) == 1
+        return np.all([alt in ['A', 'C', 'G', 'T'] for alt in [variant.REF] + variant.ALT])
 
 
 class PolyAllelicFiltration(Filtration):
     """
     Filter out poly-allelic sites.
     """
 
-    @count_filtered
+    @_count_filtered
     def filter_site(self, variant: Variant) -> bool:
         """
         Filter site. Note that we don't check explicitly all alleles, but rather
         rely on ``ALT`` field.
 
         :param variant: The variant to filter.
         :return: ``True`` if the variant is not poly-allelic, ``False`` otherwise.
         """
         return len(variant.ALT) < 2
 
 
-class CodingSequenceFiltration(Filtration):
+class AllFiltration(Filtration):
+    """
+    Filter out all sites. This is useful for testing purposes.
+    """
+
+    @_count_filtered
+    def filter_site(self, variant: Variant) -> bool:
+        """
+        Filter site.
+
+        :param variant: The variant to filter.
+        :return: ``False``.
+        """
+        return False
+
+
+class NoFiltration(Filtration):
+    """
+    Do not filter out any sites. This is useful for testing purposes.
+    """
+
+    @_count_filtered
+    def filter_site(self, variant: Variant) -> bool:
+        """
+        Filter site.
+
+        :param variant: The variant to filter.
+        :return: ``True``.
+        """
+        return True
+
+
+class CodingSequenceFiltration(Filtration, GFFHandler):
     """
     Filter out sites that are not in coding sequences. This filter should find frequent use when parsing
     spectra for DFE inference as we only consider sites in coding sequences for this purpose.
     By using it, the annotation and parsing of unnecessary sites can be avoided which increases the speed.
     Note that we assume here that within contigs, sites in the GFF file are sorted by position in ascending order.
     """
 
-    def __init__(self, gff_file: str, aliases: Dict[str, List[str]] = {}):
+    def __init__(self, gff_file: str, aliases: Dict[str, List[str]] = {}, cache: bool = True):
         """
         Create a new filtration instance.
 
         :param gff_file: The GFF file.
         :param aliases: Dictionary of aliases for the contigs in the VCF file, e.g. ``{'chr1': ['1']}``.
             This is used to match the contig names in the VCF file with the contig names in the FASTA file.
+        :param cache: Whether to cache files that are downloaded from URLs
         """
-        #: The GFF file.
-        self.gff_file: str = gff_file
+        Filtration.__init__(self)
+
+        GFFHandler.__init__(self, gff_file, cache=cache)
 
         #: The coding sequence enclosing the current variant or the closest one downstream.
         self.cd: Optional[pd.Series] = None
 
         #: The number of processed sites.
         self.n_processed: int = 0
 
         #: The contig aliases.
         self.aliases: Dict[str, List[str]] = aliases
 
-    def _setup(self):
+    def _setup(self, reader: VCF):
         """
         Touch the GFF file to load it.
-        """
-        # noinspection PyStatementEffect
-        self._cds
 
-    @cached_property
-    def _cds(self) -> pd.DataFrame:
+        :param reader: The VCF reader.
         """
-        The coding sequences.
+        super()._setup(reader)
 
-        :return: Dataframe with coding sequences.
-        """
-        return Annotation._load_cds(self.gff_file)
+        # load coding sequences
+        # noinspection PyStatementEffect
+        self._cds
 
-    @count_filtered
+    @_count_filtered
     def filter_site(self, v: Variant) -> bool:
         """
         Filter site by whether it is in a coding sequence.
 
         :param v: The variant to filter.
         :return: ``True`` if the variant is in a coding sequence, ``False`` otherwise.
         """
-        aliases = VCFHandler.get_aliases(v.CHROM, self.aliases)
+        aliases = self.get_aliases(v.CHROM, self.aliases)
 
         # if self.cd is None or not on the same chromosome or ends before the variant
         if self.cd is None or self.cd.seqid not in aliases or v.POS > self.cd.end:
 
             # initialize mock coding sequence
             self.cd = pd.Series({
                 'seqid': v.CHROM,
@@ -179,65 +218,182 @@
                 'end': DegeneracyAnnotation._pos_mock
             })
 
             # find coding sequences downstream
             cds = self._cds[self._cds['seqid'].isin(aliases) & (self._cds['end'] >= v.POS)]
 
             if not cds.empty:
-                # take the last coding sequence
+                # take the first coding sequence
                 self.cd = cds.iloc[0]
 
                 if self.cd.start == v.POS:
-                    logger.debug(f'Found coding sequence for {v.CHROM}:{v.POS}.')
+                    self.logger.debug(f'Found coding sequence for {v.CHROM}:{v.POS}.')
                 else:
-                    logger.debug(f'Found coding sequence downstream of {v.CHROM}:{v.POS}.')
+                    self.logger.debug(f'Found coding sequence downstream of {v.CHROM}:{v.POS}.')
 
             if self.n_processed == 0 and self.cd.start == DegeneracyAnnotation._pos_mock:
-                logger.warning(f'No subsequent coding sequence found on the same contig as the first variant. '
-                               f'Please make sure this is the correct GFF file with contig names matching '
-                               f'the VCF file. You can use the aliases parameter to match contig names.')
+                self.logger.warning(f'No subsequent coding sequence found on the same contig as the first variant. '
+                                    f'Please make sure this is the correct GFF file with contig names matching '
+                                    f'the VCF file. You can use the aliases parameter to match contig names.')
 
         self.n_processed += 1
 
         # check whether the variant is in the current CDS
         if self.cd is not None and self.cd.seqid in aliases and self.cd.start <= v.POS <= self.cd.end:
             return True
 
         return False
 
 
+class DeviantOutgroupFiltration(Filtration):
+    """
+    Filter out sites where the major allele of the specified outgroup samples differs from the major
+    allele of the ingroup samples.
+    """
+
+    def __init__(self, outgroups: List[str], ingroups: List[str] = None, strict_mode: bool = True):
+        """
+        Construct DeviantOutgroupFiltration.
+
+        :param outgroups: The name of the outgroup samples to consider.
+        :param ingroups: The name of the ingroup samples to consider, defaults to all samples but the outgroups.
+        :param strict_mode: Whether to filter out sites where no outgroup sample is present, defaults to ``True``
+        which is recommended.
+        """
+        super().__init__()
+
+        #: The ingroup samples.
+        self.ingroups: List[str] | None = ingroups
+
+        #: The outgroup samples.
+        self.outgroups: List[str] = outgroups
+
+        #: Whether to filter out sites where no outgroup sample is present.
+        self.strict_mode: bool = strict_mode
+
+        #: The samples found in the VCF file.
+        self.samples: Optional[np.ndarray] = None
+
+        #: The ingroup mask.
+        self.ingroup_mask: Optional[np.ndarray] = None
+
+        #: The outgroup mask.
+        self.outgroup_mask: Optional[np.ndarray] = None
+
+    def _setup(self, reader: VCF):
+        """
+        Touch the reader to load the samples.
+
+        :param reader: The VCF reader.
+        """
+        super()._setup(reader)
+
+        # create samples array
+        self.samples: np.ndarray = np.array(reader.samples)
+
+        # create ingroup and outgroup masks
+        self.create_masks()
+
+    def create_masks(self):
+        """
+        Create ingroup and outgroup masks based on the samples.
+        """
+
+        # create outgroup masks
+        self.outgroup_mask: np.ndarray = np.isin(self.samples, self.outgroups)
+
+        # create ingroup mask
+        if self.ingroups is None:
+            self.ingroup_mask = ~self.outgroup_mask
+        else:
+            self.ingroup_mask = np.isin(self.samples, self.ingroups)
+
+    @_count_filtered
+    def filter_site(self, variant: Variant) -> bool:
+        """
+        Filter site.
+
+        :param variant: The variant to filter.
+        :return: ``True`` if the variant should be kept, ``False`` otherwise.
+        """
+        if variant.is_snp:
+            # get major base among ingroup samples
+            ingroup_base = get_major_base(variant.gt_bases[self.ingroup_mask])
+
+            # get major base among outgroup samples
+            outgroup_base = get_major_base(variant.gt_bases[self.outgroup_mask])
+
+            # filter out if no outgroup base is present and strict mode is enabled
+            if outgroup_base is None:
+                return not self.strict_mode
+
+            # filter out if outgroup base is different from ingroup base
+            return ingroup_base == outgroup_base
+
+        return True
+
+
+class BiasedGCConversionFiltration(Filtration):
+    """
+    Only retain A<->T and G<->C substitutions (which are unaffected
+    by biased gene conversion, see [CITGB]_).
+
+    Mono-allelic sites are always retained, and we assume sites are at most bi-allelic.
+
+    .. [CITGB] See Pouyet et al., 'Background selection and biased
+        gene conversion affect more than 95% of the human genome and bias demographic inferences.',
+        Elife, 7:e36317, 2018
+    """
+
+    @_count_filtered
+    def filter_site(self, variant: Variant) -> bool:
+        """
+        Remove bi-allelic sites that are not A<->T or G<->C substitutions.
+
+        :param variant: The variant to filter.
+        :return: ``True`` if the variant should be kept, ``False`` otherwise.
+        """
+        if variant.is_snp and len(variant.ALT) > 0:
+            return variant.REF in 'AT' and variant.ALT[0] in 'AT' or variant.REF in 'GC' and variant.ALT[0] in 'GC'
+
+        return True
+
+
 class Filterer(VCFHandler):
     """
-    Base class for filters.
+    Filter a VCF file using a list of filtrations.
     """
 
     def __init__(
             self,
             vcf: str | Iterable[Variant],
             output: str,
             filtrations: List[Filtration] = [],
             info_ancestral: str = 'AA',
             max_sites: int = np.inf,
-            seed: int | None = 0
+            seed: int | None = 0,
+            cache: bool = True
     ):
         """
         Create a new filter instance.
 
         :param vcf: The VCF file.
         :param output: The output file.
         :param filtrations: The filtrations.
         :param info_ancestral: The info field for the ancestral allele.
         :param max_sites: The maximum number of sites to process.
-        :param seed: The seed for the random number generator.
+        :param seed: The seed for the random number generator. Use ``None`` for no seed.
+        :param cache: Whether to cache files downloaded from urls.
         """
         super().__init__(
             vcf=vcf,
             info_ancestral=info_ancestral,
             max_sites=max_sites,
-            seed=seed
+            seed=seed,
+            cache=cache
         )
 
         #: The filtrations.
         self.filtrations: List[Filtration] = filtrations
 
         #: The output file.
         self.output: str = output
@@ -260,28 +416,28 @@
 
         return True
 
     def filter(self):
         """
         Filter the VCF.
         """
-        logger.info('Start filtering')
+        self.logger.info('Start filtering')
 
         # count the number of sites
         self.n_sites = self.count_sites()
 
         # create the reader
-        reader = VCF(self.vcf)
+        reader = VCF(self.download_if_url(self.vcf))
 
         # create the writer
         writer = Writer(self.output, reader)
 
         # setup filtrations
         for f in self.filtrations:
-            f._setup()
+            f._setup(reader)
 
         # get progress bar
         with self.get_pbar() as pbar:
 
             # iterate over the sites
             for i, variant in enumerate(reader):
 
@@ -300,8 +456,8 @@
         for f in self.filtrations:
             f._teardown()
 
         # close the writer and reader
         writer.close()
         reader.close()
 
-        logger.info(f'Filtered out {self.n_filtered} out of {self.n_filtered} sites.')
+        self.logger.info(f'Filtered out {self.n_filtered} out of {self.n_filtered} sites.')
```

### Comparing `fastdfe-0.1.6b0/fastdfe/joint_inference.py` & `fastdfe-0.1.7b0/fastdfe/joint_inference.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 from typing import List, Dict, Tuple, Literal, Optional, cast
 
 import jsonpickle
 import multiprocess as mp
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
-from scipy.optimize import OptimizeResult
 from numpy.linalg import norm
+from scipy.optimize import OptimizeResult
+from tqdm import tqdm
 
-from . import Config
 from .abstract_inference import Inference
 from .base_inference import BaseInference
+from .config import Config
 from .optimization import Optimization, SharedParams, pack_shared, expand_shared, \
     Covariate, flatten_dict, merge_dicts, correct_values, parallelize as parallelize_func, expand_fixed, \
     collapse_fixed, unpack_shared
 from .parametrization import Parametrization
 from .spectrum import Spectrum, Spectra
 
 # get logger
@@ -101,18 +102,18 @@
             the mutation rate.
         :param sfs_sel: Selected SFS. Note that we require monomorphic counts to be specified in order to infer
             the mutation rate.
         :param include_divergence: Whether to include divergence in the likelihood
         :param intervals_del: ``(start, stop, n_interval)`` for deleterious population-scaled
             selection coefficients. The intervals will be log10-spaced.
         :param intervals_ben: Same as intervals_del but for beneficial selection coefficients
-        :param integration_mode: Integration mode, ``quad`` not recommmended
+        :param integration_mode: Integration mode, ``quad`` not recommended
         :param linearized: Whether to use the linearized model, ``False`` not recommended
         :param model: DFE parametrization
-        :param seed: Random seed
+        :param seed: Random seed. Use ``None`` for no seed.
         :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
         :param bounds: Bounds for the optimization in the form {param: (lower, upper)}
         :param scales: Scales for the optimization in the form {param: scale}
         :param loss_type: Loss type
         :param opts_mle: Options for the optimization
         :param n_runs: Number of independent optimization runs out of which the best one is chosen. The first run
             will use the initial values if specified. Consider increasing this number if the optimization does not
@@ -152,29 +153,29 @@
         self.add_covariates_as_shared(covariates)
 
         # check if the shared parameters were specified correctly
         self.check_shared_params()
 
         # throw error if joint inference does not make sense
         if not self.joint_inference_makes_sense():
-            logger.warning('Joint inference does not make sense as there are no parameters to be shared '
-                           'across more than one types. If this is not intended consider running '
-                           'several marginal inferences instead, which is more efficient.')
+            self.logger.warning('Joint inference does not make sense as there are no parameters to be shared '
+                                'across more than one types. If this is not intended consider running '
+                                'several marginal inferences instead, which is more efficient.')
 
         # issue notice
-        logger.info(f'Using shared parameters {self.shared_params}.')
+        self.logger.info(f'Using shared parameters {self.shared_params}.')
 
         #: Covariates indexed by parameter name
         self.covariates: Dict[str, Covariate] = {f"c{i}": cov for i, cov in enumerate(covariates)}
 
         # only show param and values
         cov_repr = dict((k, dict(param=v.param, values=v.values)) for k, v in self.covariates.items())
 
         # issue notice
-        logger.info(f'Including covariates: {cov_repr}.')
+        self.logger.info(f'Including covariates: {cov_repr}.')
 
         # parameter names for covariates
         args_cov = list(self.covariates.keys())
 
         # bounds for covariates
         bounds_cov = dict((k, cov.bounds) for k, cov in self.covariates.items())
 
@@ -266,38 +267,37 @@
                 folded=self.folded,
                 n_runs=n_runs
             )
 
         #: Joint inference object indexed by type
         self.joint_inferences: Dict[str, BaseInference] = {}
 
-        # only add if more than one type and at least one shared parameter is given
-        if len(self.types) > 1 and len(self.shared_params) > 0:
-            for t in sfs_neut.types:
-                self.joint_inferences[t] = BaseInference(
-                    # pass subtypes
-                    sfs_neut=sfs_neut[[t]],
-                    sfs_sel=sfs_sel[[t]],
-                    discretization=self.discretization,
-                    include_divergence=include_divergence,
-                    model=model,
-                    seed=seed,
-                    x0=x0,
-                    bounds=bounds,
-                    scales=scales,
-                    loss_type=loss_type,
-                    opts_mle=opts_mle,
-                    fixed_params=dict(all=self.fixed_params[t]) if t in self.fixed_params else {},
-                    do_bootstrap=do_bootstrap,
-                    n_bootstraps=n_bootstraps,
-                    parallelize=parallelize,
-                    folded=self.folded,
-                    n_runs=n_runs,
-                    locked=True
-                )
+        # add base inference object for each type
+        for t in sfs_neut.types:
+            self.joint_inferences[t] = BaseInference(
+                # pass subtypes
+                sfs_neut=sfs_neut[[t]],
+                sfs_sel=sfs_sel[[t]],
+                discretization=self.discretization,
+                include_divergence=include_divergence,
+                model=model,
+                seed=seed,
+                x0=x0,
+                bounds=bounds,
+                scales=scales,
+                loss_type=loss_type,
+                opts_mle=opts_mle,
+                fixed_params=dict(all=self.fixed_params[t]) if t in self.fixed_params else {},
+                do_bootstrap=do_bootstrap,
+                n_bootstraps=n_bootstraps,
+                parallelize=parallelize,
+                folded=self.folded,
+                n_runs=n_runs,
+                locked=True
+            )
 
     def check_shared_params(self):
         """
         Check if the shared parameters were specified correctly.
         """
         for shared in self.shared_params:
             # check parameters
@@ -346,17 +346,17 @@
 
         :param covariates: List of covariates.
         """
         cov_but_not_shared = self.determine_unshared_covariates(covariates)
 
         # add parameters with covariates to shared parameters
         if len(cov_but_not_shared) > 0:
-            logger.info(f'Parameters {cov_but_not_shared} have '
-                        f'covariates and thus need to be shared. '
-                        f'Adding them to shared parameters.')
+            self.logger.info(f'Parameters {cov_but_not_shared} have '
+                             f'covariates and thus need to be shared. '
+                             f'Adding them to shared parameters.')
 
             # add to shared parameters
             self.shared_params.append(SharedParams(params=cov_but_not_shared, types=self.types))
 
     def determine_unshared_covariates(self, covariates):
         """
         Determine which covariates are not shared.
@@ -373,24 +373,20 @@
         params_with_covariates = [cov.param for cov in covariates]
 
         # determine parameters with covariates that are not shared
         return list(set(params_with_covariates) - set(completely_shared))
 
     def run(
             self,
-            do_bootstrap: bool = None,
-            pbar: bool = True,
             **kwargs
     ) -> Spectrum:
         """
         Run inference.
 
-        :param do_bootstrap: Whether to perform bootstrapping.
-        :param pbar: Whether to show progress bar.
-        :param kwargs: Additional keyword arguments passed to
+        :param kwargs: Additional keyword arguments
         :return: Modelled SFS.
         """
 
         # run marginal optimization
         self.run_marginal()
 
         # run joint optimization
@@ -407,38 +403,38 @@
             """
             Run marginal inference. Start with initial values
             obtained from 'all' type.
 
             :param data: Tuple of type and inference object.
             :return: Tuple of type and inference object.
             """
+            # issue notice
+            self.logger.info(f"Running marginal inference for type '{data[0]}'.")
+
             data[1].run_if_required(
                 do_bootstrap=False,
                 pbar=False
             )
 
             return data
 
-        # issue notice
-        logger.info(f"Running marginal inferences for type 'all'.")
-
         # run for 'all' type
         run_marginal(('all', self.marginal_inferences['all']))
 
         # update initial values of marginal inferences
         # with MLE estimate of 'all' type
         for inf in self.marginal_inferences.values():
             inf.x0 = dict(all=self.marginal_inferences['all'].params_mle)
 
         # skip marginal inference if only one type was specified
         if len(self.types) == 1:
-            logger.info('Skipping marginal inference as only one type was specified.')
+            self.logger.info('Skipping marginal inference as only one type was specified.')
         else:
             # issue notice
-            logger.info(f'Running marginal inferences for types {self.types}.')
+            self.logger.info(f'Running marginal inferences for types {self.types}.')
 
         # optionally parallelize marginal inferences
         run_inferences = dict(parallelize_func(
             func=run_marginal,
             data=list(self.marginals_without_all().items()),
             parallelize=False,
             pbar=False
@@ -453,38 +449,39 @@
         """
         Get marginal inference without 'all' type.
 
         :return: Dict of marginal inferences indexed by type.
         """
         return dict((t, inf) for t, inf in self.marginal_inferences.items() if t != 'all')
 
-    def run_joint(self):
+    def run_joint(self) -> Spectrum:
         """
         Run joint optimization.
 
         :return: Modelled SFS.
         """
         # issue notice
-        logger.info(f'Running joint inference.')
+        self.logger.debug(f'Running joint inference.')
 
         # issue notice
-        logger.info(f'Starting numerical optimization of {self.n_runs} '
-                    'independently initialized samples which are run ' +
-                    ('in parallel.' if self.parallelize else 'sequentially.'))
+        self.logger.debug(f'Starting numerical optimization of {self.n_runs} '
+                          'independently initialized samples which are run ' +
+                          ('in parallel.' if self.parallelize else 'sequentially.'))
 
         # starting time of joint inference
         start_time = time.time()
 
         # Perform joint optimization.
         self.result, params_mle = self.optimization.run(
             x0=self.get_x0(),
             scales=self.scales,
             bounds=self.bounds,
             n_runs=self.n_runs,
-            get_counts=self.get_counts()
+            get_counts=self.get_counts(),
+            desc='Performing joint inference'
         )
 
         # assign likelihoods
         self.likelihoods = self.optimization.likelihoods
 
         # store packed MLE params for later usage
         self.params_mle_raw = copy.deepcopy(params_mle)
@@ -570,15 +567,15 @@
             do_bootstrap=do_bootstrap
         )
 
         # create copy
         other = JointInference.from_config(config)
 
         # issue notice
-        logger.info('Running joint inference without covariates.')
+        self.logger.info('Running joint inference without covariates.')
 
         # run inference
         other.run()
 
         return other
 
     def create_config(self) -> 'Config':
@@ -613,14 +610,17 @@
     @BaseInference.run_if_required_wrapper
     def perform_lrt_covariates(self, do_bootstrap: bool = True) -> float:
         """
         Perform likelihood ratio test against joint inference without covariates.
         In the simple model we share parameters across types. Low p-values indicate that
         the covariates provide a significant improvement in the fit.
 
+        To access the JointInference object without covariates, you can call :meth:`run_joint_without_covariates`,
+        which is cached.
+
         :param do_bootstrap: Whether to bootstrap. This improves the accuracy of the p-value. Note
             that if bootstrapping was performed previously without updating the likelihood, this won't have any effect.
         :return: Likelihood ratio test statistic.
         """
         if len(self.covariates) == 0:
             raise ValueError('No covariates were specified.')
 
@@ -650,15 +650,16 @@
 
         return params
 
     def bootstrap(
             self,
             n_samples: int = None,
             parallelize: bool = None,
-            update_likelihood: bool = True
+            update_likelihood: bool = True,
+            **kwargs
     ) -> Optional[pd.DataFrame]:
         """
         Perform the parametric bootstrap both for the marginal and joint inferences.
 
         :param n_samples: Number of bootstrap samples
         :param parallelize: Whether to parallelize computations
         :param update_likelihood: Whether to update the likelihood
@@ -669,71 +670,83 @@
 
         # update properties
         self.update_properties(
             n_bootstraps=n_samples,
             parallelize=parallelize
         )
 
-        logger.info("Bootstrapping marginal inferences.")
+        from . import disable_pbar
 
-        # bootstrap marginal inferences
-        for inf in self.marginal_inferences.values():
-            inf.bootstrap(
-                n_samples=n_samples,
-                parallelize=self.parallelize,
-                update_likelihood=update_likelihood
-            )
+        with tqdm(
+                total=len(self.marginal_inferences) * self.n_bootstraps,
+                disable=disable_pbar,
+                desc="Bootstrapping marginal inferences"
+        ) as pbar:
+
+            # bootstrap marginal inferences
+            for t, inf in self.marginal_inferences.items():
+                self.logger.info(f"Bootstrapping type '{t}'.")
+
+                inf.bootstrap(
+                    n_samples=self.n_bootstraps,
+                    parallelize=self.parallelize,
+                    update_likelihood=update_likelihood,
+                    pbar=False
+                )
 
-        start_time = time.time()
+                pbar.update(self.n_bootstraps)
 
-        logger.info("Bootstrapping joint inference.")
+        start_time = time.time()
 
         # parallelize computations if desired
         if self.parallelize:
 
-            logger.info(f"Running {self.n_bootstraps} joint bootstrap samples "
-                        f"in parallel on {mp.cpu_count()} cores.")
+            self.logger.debug(f"Running {self.n_bootstraps} joint bootstrap samples "
+                              f"in parallel on {min(mp.cpu_count(), self.n_bootstraps)} cores.")
 
             # We need to assign new random states to the subprocesses.
             # Otherwise, they would all produce the same result.
             seeds = self.rng.integers(0, high=2 ** 32, size=self.n_bootstraps)
 
         else:
-            logger.info(f"Running {self.n_bootstraps} joint bootstrap samples sequentially.")
+            self.logger.debug(f"Running {self.n_bootstraps} joint bootstrap samples sequentially.")
 
             seeds = [None] * self.n_bootstraps
 
         # run bootstraps
         result = parallelize_func(
             func=self.run_joint_bootstrap_sample,
             data=seeds,
             parallelize=self.parallelize,
-            pbar=True
+            pbar=True,
+            desc="Bootstrapping joint inference"
         )
 
         # number of successful runs
         n_success = np.sum([res.success for res in result[:, 0]])
 
         # issue warning if some runs did not finish successfully
         if n_success < self.n_bootstraps:
-            logger.warning(f"{self.n_bootstraps - n_success} out of {self.n_bootstraps} bootstrap samples "
-                           "did not terminate normally during numerical optimization. "
-                           "The confidence intervals might thus be unreliable. Consider adjusting "
-                           "the optimization parameters (increasing `gtol` or `n_runs`) "
-                           "or decrease the number of optimized parameters.")
+            self.logger.warning(f"{self.n_bootstraps - n_success} out of {self.n_bootstraps} bootstrap samples "
+                                "did not terminate normally during numerical optimization. "
+                                "The confidence intervals might thus be unreliable. Consider adjusting "
+                                "the optimization parameters (increasing `gtol` or `n_runs`) "
+                                "or decrease the number of optimized parameters.")
 
         # dataframe of MLE estimates in flattened format
         self.bootstraps = pd.DataFrame([flatten_dict(r) for r in result[:, 1]])
 
         # assign bootstrap results
         self.bootstrap_results = list(result[:, 0])
 
-        # assign bootstrap parameters to joint inferences
+        # assign bootstrap parameters to joint inference objects
         for t, inf in self.joint_inferences.items():
-            inf.bootstraps = self.bootstraps.filter(regex=f'{t}.*').rename(columns=lambda x: x.split('.')[-1])
+
+            # filter for columns belonging to the current type
+            inf.bootstraps = self.bootstraps.filter(regex=f'{t}\\..*').rename(columns=lambda x: x.split('.')[-1])
 
             # add estimates for alpha to the bootstraps
             inf.add_alpha_to_bootstraps()
 
         # add execution time
         self.execution_time += time.time() - start_time
 
@@ -763,14 +776,15 @@
         result, params_mle = self.optimization.run(
             x0=self.params_mle_raw,
             scales=self.get_scales_linear(),
             bounds=self.get_bounds_linear(),
             n_runs=1,
             debug_iterations=False,
             print_info=False,
+            desc="Bootstrapping joint inference",
             get_counts=dict((t, lambda params, t=t: inf.model_sfs(
                 correct_values(self.add_covariates(params, t), self.bounds, self.scales),
                 sfs_neut=self.resample_sfs(self.marginal_inferences[t].sfs_neut, seed=seed),
                 sfs_sel=self.resample_sfs(self.marginal_inferences[t].sfs_sel, seed=seed)
             )) for t, inf in self.marginals_without_all().items())
         )
 
@@ -826,16 +840,16 @@
     @BaseInference.run_if_required_wrapper
     def perform_lrt_shared(self, do_bootstrap: bool = True) -> float:
         """
         Compare likelihood of joint inference with product of marginal likelihoods.
         This provides information about the goodness of fit achieved by the parameter sharing.
         Low p-values indicate that parameter sharing is not justified, i.e., that the marginal
         inferences provide a better fit to the data. Note that it is more difficult to properly
-        optimize the joint likelihood, which makes this test conservative, i.e., the p-value
-        might be larger than it should be.
+        optimize the joint likelihood, which makes this test conservative, i.e., the reported p-value
+        might be larger than what it really is.
 
         :param do_bootstrap: Whether to perform bootstrapping. This improves the accuracy of the p-value. Note
             that if bootstrapping was performed previously without updating the likelihood, this won't have any effect.
         :return: p-value
         """
         if do_bootstrap:
             self.bootstrap_if_required()
@@ -889,14 +903,15 @@
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             intervals_del: (float, float, int) = (-1.0e+8, -1.0e-5, 1000),
             intervals_ben: (float, float, int) = (1.0e-5, 1.0e4, 1000),
             title: str = 'discretized DFE comparison',
             labels: List[str] = None,
+            kwargs_legend: dict = dict(prop=dict(size=8)),
             ax: plt.Axes = None
     ) -> plt.Axes:
         """
         Plot discretized DFE comparing the different types.
 
         :param labels: Labels for types
         :param title: Title of plot
@@ -905,39 +920,48 @@
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence level
         :param confidence_intervals: Whether to plot confidence intervals
         :param file: File to save plot to
         :param show: Whether to show plot
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bars.
         :param ax: Axes object
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes object
         """
         labels, inferences = zip(*self.get_inferences(labels=labels).items())
 
         return Inference.plot_discretized(**locals())
 
     def plot_sfs_comparison(
             self,
-            sfs_types: List[Literal['modelled', 'observed', 'modelled', 'neutral']] = ['modelled', 'observed'],
+            sfs_types: List[Literal['modelled', 'observed', 'selected', 'neutral']] = ['modelled', 'observed'],
             types: List[str] = None,
             labels: List[str] = None,
             file: str = None,
             show: bool = True,
-            ax: plt.Axes = None
+            ax: plt.Axes = None,
+            title: str = 'SFS comparison',
+            use_subplots: bool = False,
+            show_monomorphic: bool = False,
+            kwargs_legend: dict = dict(prop=dict(size=8)),
 
     ) -> plt.Axes:
         """
         Plot SFS comparison.
 
         :param types: Types to plot
         :param file: File to save plot to
         :param labels: Labels for types
         :param sfs_types: Types of SFS to plot
         :param show: Whether to show plot
         :param ax: Axes object
+        :param title: Plot title
+        :param use_subplots: Whether to use subplots
+        :param show_monomorphic: Whether to show monomorphic counts
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes object
         """
         from fastdfe import Visualization
 
         if 'modelled' in sfs_types:
             self.run_if_required()
 
@@ -967,15 +991,19 @@
         spectra = {get_label(t, sfs): getattr(inf, mapping[sfs]) for t, inf in inferences for sfs in sfs_types}
 
         return Visualization.plot_sfs_comparison(
             spectra=list(spectra.values()),
             labels=list(spectra.keys()) if labels is None else labels,
             file=file,
             show=show,
-            ax=ax
+            ax=ax,
+            title=title,
+            use_subplots=use_subplots,
+            show_monomorphic=show_monomorphic,
+            kwargs_legend=kwargs_legend
         )
 
     @BaseInference.run_if_required_wrapper
     def plot_continuous(
             self,
             file: str = None,
             show: bool = True,
@@ -983,14 +1011,15 @@
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             title: str = 'DFE comparison',
             labels: List[str] = None,
             scale_density: bool = False,
             scale: Literal['lin', 'log', 'symlog'] = 'lin',
+            kwargs_legend: dict = dict(prop=dict(size=8)),
             ax: plt.Axes = None
     ) -> plt.Axes:
         """
         Plot discretized DFE. The special constants ``np.inf`` and ``-np.inf`` are also valid interval bounds.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
         the x-axis, we may get a wrong intuition on how the mass is distributed,
         however. To get a better intuition, we can optionally scale the density
@@ -1004,14 +1033,15 @@
         :param title: Title of plot
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence level
         :param confidence_intervals: Whether to plot confidence intervals
         :param file: File to save plot to
         :param show: Whether to show plot
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :param ax: Axes object
         :return: Axes object
         """
         if intervals is None:
             intervals = self.discretization.bins
 
         labels, inferences = zip(*self.get_inferences(labels=labels).items())
@@ -1026,34 +1056,59 @@
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             ci_level: float = 0.05,
             show: bool = True,
             title: str = 'inferred parameters',
             labels: List[str] = None,
             legend: bool = True,
             ax: plt.Axes = None,
+            kwargs_legend: dict = dict(prop=dict(size=8), loc='upper right'),
             **kwargs: List[str]
     ) -> plt.Axes:
         """
         Plot discretized DFE comparing the different types.
 
         :param legend: Whether to show legend
         :param labels: Labels for types
         :param title: Title of plot
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence level
         :param confidence_intervals: Whether to plot confidence intervals
         :param file: File to save plot to
         :param show: Whether to show plot
         :param ax: Axes object
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes object
         """
         labels, inferences = zip(*self.get_inferences(labels=labels).items())
 
         return Inference.plot_inferred_parameters(**locals())
 
+    @BaseInference.run_if_required_wrapper
+    def plot_inferred_parameters_boxplot(
+            self,
+            file: str = None,
+            show: bool = True,
+            title: str = 'inferred parameters',
+            labels: List[str] = None,
+            **kwargs: List[str]
+    ) -> plt.Axes:
+        """
+        Plot discretized DFE comparing the different types.
+
+        :param labels: Labels for types
+        :param title: Title of plot
+        :param file: File to save plot to
+        :param show: Whether to show plot
+        :return: Axes object
+        :raises ValueError: If no inference objects are given or no bootstraps are found.
+        """
+        labels, inferences = zip(*self.get_inferences(labels=labels).items())
+
+        return Inference.plot_inferred_parameters_boxplot(**locals())
+
     def get_cis_params_mle(
             self,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             ci_level: float = 0.05,
             param_names: Optional[list[str]] = None
     ):
         """
```

### Comparing `fastdfe-0.1.6b0/fastdfe/json_handlers.py` & `fastdfe-0.1.7b0/fastdfe/json_handlers.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.6b0/fastdfe/mle.py` & `fastdfe-0.1.7b0/fastdfe/likelihood.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 __date__ = "2023-02-26"
 
 import numpy as np
 from scipy.special import factorial
 from scipy.stats import poisson
 
 
-class MLE:
+class Likelihood:
     """
-    MLE utilities.
+    Utilities for computing Poisson likelihoods.
     """
 
     #: Epsilon for numerical stability
     eps = 1e-50
 
     @staticmethod
     def add_epsilon(x: np.ndarray) -> np.ndarray:
@@ -27,45 +27,45 @@
         :param x: Array to add epsilon to
         :return: Array with epsilon added to zero counts
         """
         # convert to float
         x = x.astype(float)
 
         # replace 0s with epsilon to avoid log(0)
-        x[x == 0] = MLE.eps
+        x[x == 0] = Likelihood.eps
 
         return x
 
     @staticmethod
     def poisson(mu: np.ndarray, k: np.ndarray) -> np.ndarray:
         """
         Compute Poisson(mu, k).
 
         :param mu: Mean of Poisson distribution
         :param k: Number of events
         :return: Poisson(mu, k)
         """
         # add epsilon to zero counts
-        mu = MLE.add_epsilon(mu)
+        mu = Likelihood.add_epsilon(mu)
 
         return poisson.pmf(k, mu)
 
     @staticmethod
     def log_poisson(mu: np.ndarray, k: np.ndarray) -> np.ndarray:
         """
         Compute log(Poisson(mu, k)).
 
         :param mu: Mean of Poisson distribution
         :param k: Number of events
         :return: log(Poisson(mu, k))
         """
         # add epsilon to zero counts
-        mu = MLE.add_epsilon(mu)
+        mu = Likelihood.add_epsilon(mu)
 
-        return k * np.log(mu) - mu - MLE.log_factorial(k)
+        return k * np.log(mu) - mu - Likelihood.log_factorial(k)
 
     @staticmethod
     def log_factorial_stirling(n: np.ndarray | float) -> np.ndarray | float:
         """
         Use Stirling's approximation for values larger than n_threshold.
         https://en.wikipedia.org/wiki/Stirling%27s_approximation
 
@@ -88,10 +88,10 @@
 
         low = n <= n_threshold
 
         # compute for low values of n
         x[low] = np.log(factorial(n[low]))
 
         # use Stirling's approximation for large value of n
-        x[~low] = MLE.log_factorial_stirling(n[~low])
+        x[~low] = Likelihood.log_factorial_stirling(n[~low])
 
         return x
```

### Comparing `fastdfe-0.1.6b0/fastdfe/optimization.py` & `fastdfe-0.1.7b0/fastdfe/optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,34 +15,36 @@
 import numpy as np
 from numpy.linalg import norm
 from numpy.random import Generator
 from scipy.optimize import minimize, OptimizeResult
 from scipy.stats import loguniform, uniform
 from tqdm import tqdm
 
-from .mle import MLE
+from .likelihood import Likelihood
 
 # get logger
-logger = logging.getLogger('fastdfe')
+logger = logging.getLogger('fastdfe').getChild('Optimization')
 
 
 def parallelize(
         func: Callable,
         data: list | np.ndarray,
         parallelize: bool = True,
-        pbar: bool = None
+        pbar: bool = None,
+        desc: str = None
 ) -> np.ndarray:
     """
     Convenience function that parallelizes the given function
     if specified or executes them sequentially otherwise.
 
-    :param pbar: Whether to show a progress bar
     :param parallelize: Whether to parallelize
     :param data: Data to iterate over
     :param func: Function to apply to each element of data
+    :param pbar: Whether to show a progress bar
+    :param desc: Description for progress bar
     :return: List of results
     """
     from . import disable_pbar
 
     n = len(data)
 
     if parallelize and n > 1:
@@ -50,15 +52,15 @@
         iterator = mp.Pool().imap(func, data)
     else:
         # sequentialize
         iterator = map(func, data)
 
     # whether to show a progress bar
     if pbar is True or (pbar is None and not parallelize and n > 1) or pbar is None and n > mp.cpu_count():
-        iterator = tqdm(iterator, total=n, disable=disable_pbar)
+        iterator = tqdm(iterator, total=n, disable=disable_pbar, desc=desc)
 
     return np.array(list(iterator), dtype=object)
 
 
 def flatten_dict(d: dict, separator='.', prefix=''):
     """
     Flatten dictionary.
@@ -369,15 +371,16 @@
     return corrected
 
 
 def get_real_bounds(bounds: Tuple[float, float], scale: Literal['lin', 'log', 'symlog']) -> Tuple[float, float]:
     """
     Get real bounds from the given bounds.
 
-    :param bounds:
+    :param bounds: Bounds of the parameter
+    :param scale: Scale of the parameter
     :return:
     """
     if scale == 'symlog':
         return -bounds[1], bounds[1]
 
     return bounds
 
@@ -692,15 +695,15 @@
 
     #: The bounds of the covariate parameter to be estimated
     bounds: tuple = (1e-4, 1e4)
 
     #: The initial value of the covariate
     x0: float = 0
 
-    #: The scale of the bounds. See :func:`scale_value` for details.
+    #: The scale of the bounds. See :func:`scale_value` for details
     bounds_scale: Literal['lin', 'log', 'symlog'] = 'symlog'
 
     def __post_init__(self):
         """
         Cast bounds to tuple and check if an inverse_callback is provided
         when a custom callback is specified.
         """
@@ -811,15 +814,16 @@
             x0: Dict[str, Dict[str, float]] = {},
             scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
             bounds: Dict[str, Tuple[float, float]] = {},
             n_runs: int = 1,
             debug_iterations: bool = True,
             print_info: bool = True,
             opts_mle: dict = None,
-            pbar: bool = None
+            pbar: bool = None,
+            desc: str = 'Inferring DFE',
     ) -> (OptimizeResult, dict):
         """
         Perform the optimization procedure.
 
         :param scales: Scales of the parameters
         :param bounds: Bounds of the parameters
         :param n_runs: Number of independent optimization runs out of which the best one is chosen. The first run
@@ -827,14 +831,15 @@
             produce good results.
         :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
         :param get_counts: Dictionary of functions to evaluate counts for each type
         :param debug_iterations: Whether to print debug messages for each iteration
         :param opts_mle: Dictionary of options for the optimizer
         :param print_info: Whether to print information about the bounds
         :param pbar: Whether to show a progress bar
+        :param desc: Description for the progress bar
         :return: The optimization result and the likelihoods
         """
         # number of optimization runs
         self.n_runs = n_runs
 
         # store the scales of the parameters
         if scales:
@@ -894,15 +899,15 @@
                 options=self.opts_mle
             )
 
         # initial parameters for the samples
         initial_params = [self.x0] + [self.sample_x0(self.x0) for _ in range(self.n_runs - 1)]
 
         # parallelize MLE for different initializations
-        results = parallelize(optimize, initial_params, self.parallelize, pbar=pbar)
+        results = parallelize(optimize, initial_params, self.parallelize, pbar=pbar, desc=desc)
 
         # list of the best likelihood for each run
         self.likelihoods = -np.array([res.fun for res in results])
 
         # get result with the lowest likelihood
         result = results[np.argmax(self.likelihoods)]
 
@@ -964,15 +969,15 @@
             # flatten and convert to array
             counts = np.array(list(counts_dict.values()))
 
             # reshape and merge
             counts_modelled, counts_observed = np.stack(counts, axis=1).reshape(2, -1)
 
             # use independent Poisson likelihoods
-            LL = MLE.log_poisson(mu=counts_modelled, k=counts_observed)
+            LL = Likelihood.log_poisson(mu=counts_modelled, k=counts_observed)
 
             # combine likelihoods and take additive inverse
             ll = np.sum(LL)
 
             # compute L2 norm
             L2 = norm(counts_modelled - counts_observed, 2)
```

### Comparing `fastdfe-0.1.6b0/fastdfe/parametrization.py` & `fastdfe-0.1.7b0/fastdfe/parametrization.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import logging
 from abc import abstractmethod
 from functools import wraps
-from typing import Callable, List, Union
+from typing import Callable, List, Union, Dict
 
 import numpy as np
-from matplotlib import pyplot as plt
 from scipy.stats import gamma, expon
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
-def from_string(model: Union['Parametrization', str]) -> 'Parametrization':
+def _from_string(model: Union['Parametrization', str]) -> 'Parametrization':
     """
     Return Parametrization from class name string.
 
     :param model: Class name string or parametrization object
     :return: Parametrization object
     """
     if isinstance(model, Parametrization):
@@ -31,15 +30,15 @@
 
     if isinstance(model, str):
         return globals()[model]()
 
     raise ValueError(f'Unknown parametrization: {model}')
 
 
-def to_string(model: Union['Parametrization', str]) -> str:
+def _to_string(model: Union['Parametrization', str]) -> str:
     """
     Return class name string from Parametrization.
 
     :param model: Class name string or Parametrization object
     :return: Class name string
     """
     if isinstance(model, Parametrization):
@@ -70,14 +69,16 @@
     #: Scales over which to optimize the parameters, either 'log' or 'lin'
     scales = {}
 
     def __init__(self):
         """
         Initialize parametrization.
         """
+        self.logger = logger.getChild(self.__class__.__name__)
+
         #: argument names
         self.param_names: List = list(self.x0.keys())
 
     @staticmethod
     def _accepts_scalars(func: Callable) -> Callable[[np.ndarray | float], np.ndarray | float]:
         """
         Make func accept scalar values.
@@ -128,17 +129,17 @@
         :param bins: Bins to use for discretization
         :return: Histogram
         """
         x = self.get_cdf(**params)(bins)
 
         # issue warning if values at bounds are outside [0, 1]
         if not -1e-5 < x[0] < 1e-5 or not 1 - 1e-5 < x[-1] < 1 + 1e-5:
-            logger.warning(f'CDF evaluates to {(x[0], x[-1])} at the lower and upper '
-                           f'bounds, which is a bit off from the expected (0, 1). '
-                           f'Used parameters: {params}.')
+            self.logger.warning(f'CDF evaluates to {(x[0], x[-1])} at the lower and upper '
+                                f'bounds, which is a bit off from the expected (0, 1). '
+                                f'Used parameters: {params}.')
 
         # compute histogram
         hist = x[1:] - x[:-1]
 
         return hist
 
     def _normalize(self, params: dict) -> dict:
@@ -557,28 +558,28 @@
 
         #: Intervals
         self.intervals = np.concatenate(([-np.inf], intervals, [np.inf]))
 
         #: Interval sizes
         self.interval_sizes = self.intervals[1:] - self.intervals[:-1]
 
-        #: Number of intervals
+        #: Number of intervals, including the two infinite ones
         self.k = self.intervals.shape[0] - 1
 
-        #: All parameter names
+        #: All parameter names, including the fixed ones
         self.params = np.array([f"S{i}" for i in range(self.k)])
 
-        #: Parameter names without bounds
+        #: Parameter names that are not fixed
         self.param_names = self.params[1:-1].tolist()
 
         #: Fixed parameters
         self.fixed_params = {self.params[0]: 0, self.params[-1]: 0}
 
         #: Default initial parameters
-        self.x0 = dict((p, 1 / self.k) for p in self.param_names)
+        self.x0 = dict((p, 1 / (self.k - 2)) for p in self.param_names)
 
         #: Default parameter bounds
         self.bounds = dict((p, (0, 1)) for p in self.param_names)
 
         #: Scales
         self.scales = dict((p, 'lin') for p in self.param_names)
 
@@ -647,14 +648,201 @@
 
         # convert to numpy arrays
         intervals = np.array(self.intervals)
         interval_sizes = np.array(self.interval_sizes)
 
         # convert to ordered array values
         vals = np.array([values[self.params[i]] for i in range(self.k)])
+
+        @Parametrization._accepts_scalars
+        def cdf(S: np.ndarray) -> np.ndarray:
+            """
+            The CDF.
+
+            :param S: Selection coefficients
+            :return: Cumulative probability
+            """
+            # iterate over parameters and assign values
+            cum = np.cumsum([values[self.params[i]] for i in range(self.k)])
+
+            # obtain bin indices
+            i = np.sum(self.intervals[:, None] <= S[None, :], axis=0) - 1
+
+            # make sure we don't go out of bounds which can happen if S is np.inf
+            i[i >= self.k] = self.k - 1
+
+            # cumulative probability up into previous bin
+            cum_prev = cum[np.maximum(i - 1, np.zeros_like(S, dtype=int))]
+
+            # probability in current bin
+            cum_within = np.abs(intervals[i] - S) / interval_sizes[i] * vals[i]
+            cum_within[np.isnan(cum_within)] = 0
+
+            # return cumulative probability
+            return cum_prev + cum_within
+
+        return cdf
+
+
+class DiscreteFractionalParametrization(Parametrization):
+    r"""
+    Same model as :class:`DiscreteParametrization`, but re-parametrized by
+    :math:`\hat{S}_1, \hat{S}_2, \dots, \hat{S}_{k-1}`, so that the mass in the ith interval :math:`S_i`
+    is determined by the sum of masses to the left, i.e.
+
+    :math:`S_i = \hat{S}_i \sum_{j<i} S_j, i = 1, \dots, k - 1`,
+
+    :math:`S_k = 1 - \sum_{j=1}^{k-1} S_j`.
+
+    This parametrization has the advantage of not imposing a shape on the DFE. For a reasonably fine parametrization,
+    the number of parameters is larger than those of the other models, however. It is preferable over
+    :class:`DiscreteParametrization` as it has one parameter less and does not impose a constraint on the parameters.
+    """
+
+    def __init__(
+            self,
+            intervals: np.ndarray = np.array([-100000, -100, -10, -1, 0, 1, 1000])
+    ):
+        """
+        Constructor.
+
+        :param intervals: The intervals of the discrete distribution.
+        """
+        super().__init__()
+
+        #: Intervals
+        self.intervals = np.concatenate(([-np.inf], intervals, [np.inf]))
+
+        #: Interval sizes
+        self.interval_sizes = self.intervals[1:] - self.intervals[:-1]
+
+        #: Number of intervals, including the two infinite ones
+        self.k = self.intervals.shape[0] - 1
+
+        #: All parameter names, including fixed parameters
+        self.params = np.array([f"S{i}" for i in range(self.k)])
+
+        #: Parameter names that are not fixed
+        self.param_names = self.params[1:-2].tolist()
+
+        #: Fixed parameters
+        self.fixed_params = {self.params[0]: 0, self.params[-2]: 1, self.params[-1]: 0}
+
+        #: Default initial parameters
+        self.x0 = self.to_fractional(dict((p, 1 / (self.k - 2)) for p in self.param_names))
+
+        #: Default parameter bounds
+        self.bounds = dict((p, (0, 1)) for p in self.param_names)
+
+        #: Scales
+        self.scales = dict((p, 'lin') for p in self.param_names)
+
+        #: Submodels
+        self.submodels = dict(
+            full=dict(),
+            dele=dict((p, 0) for p in self.params[1:-1][self.intervals[1:-2] < 0])
+        )
+
+    def to_nominal(self, params: Dict[str, float]) -> Dict[str, float]:
+        """
+        Convert representation of fraction of total mass to the left
+        to representation of fractions which sum to 1.
+
+        :param params: Parameter values S0, S2, ..., Sk
+        :return: Converted parameters
+        """
+        # converted parameters
+        converted = params.copy()
+
+        # cumulative sum up to the previous parameter
+        mass = 0
+
+        # take mass of current bin to be fraction of mass assigned to the previous bins
+        for p in self.params[1:-2]:
+            converted[p] = params[p] * (1 - mass)
+            mass += converted[p]
+
+        # assign remaining mass to last bin
+        converted[self.params[-2]] = 1 - mass
+
+        return converted
+
+    def to_fractional(self, params: Dict[str, float]) -> Dict[str, float]:
+        """
+        Invert the to_nominal operation: Convert representation of fractions which sum to 1
+        back to representation of fraction of total mass to the left.
+
+        :param params: Converted parameters (nominal space)
+        :return: Original parameters (parameter space)
+        """
+        # converted parameters
+        converted = params.copy()
+
+        # cumulative sum up to the previous parameter
+        mass = 0
+
+        # Iterate over parameters
+        for p in self.params[1:-2]:
+            # Calculate original parameter value
+            converted[p] = params[p] / (1 - mass)
+
+            # update cumulative sum
+            mass += params[p]
+
+        # last parameter is simply what's left
+        converted[self.params[-2]] = 1 - mass
+
+        return converted
+
+    def get_pdf(self, **kwargs) -> Callable[[np.ndarray], np.ndarray]:
+        """
+        Get PDF.
+
+        :param kwargs: Parameter values S1, S2, ..., Sk-1
+        :return: Function that computes the PDF for given S values
+        """
+
+        # normalize and add boundary parameters
+        values = self.to_nominal(kwargs | self.fixed_params)
+
+        @Parametrization._accepts_scalars
+        def pdf(S: np.ndarray) -> np.ndarray:
+            """
+            The PDF.
+
+            :param S: Selection coefficients
+            :return: Probability density
+            """
+            x = np.zeros_like(S, dtype=float)
+
+            # iterate over parameters and assign values
+            for i, p in enumerate(self.params):
+                x[(self.intervals[i] < S) & (S <= self.intervals[i + 1])] = values[p] / self.interval_sizes[i]
+
+            return x
+
+        return pdf
+
+    def get_cdf(self, **kwargs) -> Callable[[np.ndarray], np.ndarray]:
+        """
+        Get CDF.
+
+        :param kwargs: Parameter values S1, S2, ..., Sk-1
+        :return: Function that computes the CDF for given S values
+        """
+
+        # normalize and add boundary parameters
+        values = self.to_nominal(kwargs | self.fixed_params)
+
+        # convert to numpy arrays
+        intervals = np.array(self.intervals)
+        interval_sizes = np.array(self.interval_sizes)
+
+        # convert to ordered array values
+        vals = np.array([values[self.params[i]] for i in range(self.k)])
 
         @Parametrization._accepts_scalars
         def cdf(S: np.ndarray) -> np.ndarray:
             """
             The CDF.
 
             :param S: Selection coefficients
```

### Comparing `fastdfe-0.1.6b0/fastdfe/parser.py` & `fastdfe-0.1.7b0/fastdfe/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,52 @@
 """
-Parser module.
+A VCF parser that can be used to extract the site frequency spectrum (SFS) from a VCF file.
+Stratifying the SFS is supported by providing a list of :class:`Stratification` instances.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-03-26"
 
 import itertools
 import logging
 from abc import ABC, abstractmethod
-from functools import cached_property
-from typing import List, Callable, Literal, Optional, Iterable, Dict
+from collections import Counter
+from typing import List, Callable, Literal, Optional, Iterable, Dict, cast
 
 import numpy as np
+from Bio.SeqRecord import SeqRecord
 from cyvcf2 import Variant, VCF
-from pyfaidx import Fasta
 
-from .annotation import Annotation, Annotator
+from .annotation import Annotation, Annotator, SynonymyAnnotation
+from .bio_handlers import bases, get_called_bases, count_no_type, FASTAHandler, VCFHandler, NoTypeException
 from .filtration import Filtration, PolyAllelicFiltration
 from .spectrum import Spectra
-from .vcf import VCFHandler
 
-#: Logger
+# logger
 logger = logging.getLogger('fastdfe')
 
-#: The DNA bases
-bases = ["A", "C", "G", "T"]
-
-
-def count_no_type(func: Callable) -> Callable:
-    """
-    Decorator that increases ``self.n_no_type`` by 1 if the decorated function raises a ``NoTypeException``.
-    """
-
-    def wrapper(self, variant):
-        try:
-            return func(self, variant)
-        except NoTypeException as e:
-            self.n_no_type += 1
-            raise e
-
-    return wrapper
-
-
-class NoTypeException(BaseException):
-    """
-    Exception thrown when no type can be determined.
-    """
-    pass
-
 
 class Stratification(ABC):
     """
-    Abstract class for Stratifying the SFS by determining
-    a site's type based on its properties.
+    Abstract class for Stratifying the SFS by determining a site's type based on its properties.
     """
 
     #: Parser instance
     parser: Optional['Parser'] = None
 
     #: The number of sites that didn't have a type.
     n_no_type: int = 0
 
+    def __init__(self):
+        """
+        Create instance.
+        """
+        self.logger = logger.getChild(self.__class__.__name__)
+
     def _setup(self, parser: 'Parser'):
         """
         Provide the stratification with some context by specifying the parser.
         This should be done before calling :meth:`get_type`.
 
         :param parser: The parser
         """
@@ -74,39 +55,15 @@
     def _teardown(self):
         """
         Perform any necessary post-processing. This method is called after the actual stratification.
         """
         n_total = self.parser.n_sites - self.parser.n_skipped + self.n_no_type
         n_valid = n_total - self.n_no_type
 
-        logger.info(f":{type(self).__name__} Number of sites with valid type: {n_valid} / {n_total}")
-
-    def _get_ancestral(self, variant: Variant) -> str:
-        """
-        Determine the ancestral allele.
-
-        :param variant: The vcf site
-        :return: Ancestral allele
-        :raises ValueError: If the ancestral allele could not be determined
-        """
-        if variant.is_snp:
-            # obtain ancestral allele
-            aa = variant.INFO.get(self.parser.info_ancestral)
-
-            # return the ancestral allele if it is a valid base
-            if aa in bases:
-                return aa
-
-            # if we don't skip non-polarized sites, we raise an error
-            if self.parser.ignore_not_polarized:
-                raise ValueError("No valid AA tag found.")
-
-        # if we don't skip non-polarized sites, or if the site is not an SNP
-        # we return the reference allele
-        return variant.REF
+        self.logger.info(f"Number of sites with valid type: {n_valid} / {n_total}")
 
     @abstractmethod
     def get_type(self, variant: Variant) -> Optional[str]:
         """
         Get type of given Variant. Only the types
         given by :meth:`get_types()` are valid, or ``None`` if
         no type could be determined.
@@ -122,265 +79,188 @@
         Get all possible types.
 
         :return: List of types
         """
         pass
 
 
-class BaseContextStratification(Stratification):
+class BaseContextStratification(Stratification, FASTAHandler):
     """
     Stratify the SFS by the base context of the mutation. The number of flanking bases
     can be configured. Note that we attempt to take the ancestral allele as the
-    middle base. If ``ignore_not_polarized`` is set to ``True``, we skip sites
+    middle base. If ``skip_non_polarized`` is set to ``True``, we skip sites
     that are not polarized, otherwise we use the reference allele as the middle base.
     """
 
-    def __init__(self, fasta_file: str, n_flanking: int = 1, aliases: Dict[str, List[str]] = {}):
+    def __init__(
+            self,
+            fasta_file: str,
+            n_flanking: int = 1,
+            aliases: Dict[str, List[str]] = {},
+            cache: bool = True
+    ):
         """
         Create instance. Note that we require a fasta file to be specified
         for base context to be able to be inferred
 
         :param fasta_file: The fasta file path, possibly gzipped or a URL
         :param n_flanking: The number of flanking bases
         :param aliases: Dictionary of aliases for the contigs in the VCF file, e.g. ``{'chr1': ['1']}``.
             This is used to match the contig names in the VCF file with the contig names in the FASTA file and GFF file.
+        :param cache: Whether to cache files that are downloaded from URLs
         """
-        #: The fasta file
-        self.fasta_file: str = fasta_file
+        Stratification.__init__(self)
+
+        FASTAHandler.__init__(self, fasta_file, cache=cache)
 
         #: The number of flanking bases
         self.n_flanking: int = n_flanking
 
         #: Aliases for the contigs in the VCF file
         self.aliases: Dict[str, List[str]] = aliases
 
-    @cached_property
-    def _ref(self) -> Fasta:
-        """
-        Get the reference reader.
-
-        :return: The reference reader.
-        """
-        return VCFHandler.load_fasta(self.fasta_file)
+        #: The current contig
+        self.contig: Optional[SeqRecord] = None
 
     @count_no_type
     def get_type(self, variant: Variant) -> str:
         """
         Get the base context for a given mutation
 
         :param variant: The vcf site
         :return: Base context of the mutation
         """
         pos = variant.POS - 1
 
-        try:
-            ref = self._get_ancestral(variant)
-        except ValueError:
-            raise NoTypeException("Invalid ancestral allele: Ancestral allele must be a valid base.")
+        # get the ancestral allele
+        aa = self.parser._get_ancestral(variant)
 
-        # retrieve the sequence of the chromosome from the reference genome
-        sequence = VCFHandler.get_contig(self._ref, VCFHandler.get_aliases(variant.CHROM, self.aliases))
+        # get aliases
+        aliases = self.get_aliases(variant.CHROM, self.aliases)
 
-        if pos < 0 or pos >= len(sequence):
+        # check if contig is up-to-date
+        if self.contig is None or self.contig.id not in aliases:
+            self.logger.debug(f"Fetching contig '{variant.CHROM}'.")
+
+            # fetch contig
+            self.contig = self.get_contig(aliases)
+
+        # check if position is valid
+        if pos < 0 or pos >= len(self.contig):
             raise NoTypeException("Invalid position: Position must be within the bounds of the sequence.")
 
+        # get upstream bases
         upstream_start = max(0, pos - self.n_flanking)
-        upstream_bases = sequence[upstream_start:pos]
+        upstream_bases = str(self.contig.seq[upstream_start:pos])
 
-        downstream_end = min(len(sequence), pos + self.n_flanking + 1)
-        downstream_bases = sequence[pos + 1:downstream_end]
+        # get downstream bases
+        downstream_end = min(len(self.contig), pos + self.n_flanking + 1)
+        downstream_bases = str(self.contig.seq[pos + 1:downstream_end])
 
-        return f"{upstream_bases}{ref}{downstream_bases}"
+        return f"{upstream_bases}{aa}{downstream_bases}"
 
     def get_types(self) -> List[str]:
         """
         Create all possible base contexts.
 
         :return: List of contexts
         """
         return [''.join(c) for c in itertools.product(bases, repeat=2 * self.n_flanking + 1)]
 
 
 class BaseTransitionStratification(Stratification):
     """
     Stratify the SFS by the base transition of the mutation, i.e., ``A>T``.
-    We parse the VCF file twice, once to determine the base transition probabilities
-    used for the monomorphic counts, and once to determine the base transitions.
-    Note that we assume sites here to be at most bi-allelic.
+    Should be used with ``n_target_sites`` since we can't infer the type of monomorphic sites.
     """
 
-    #: Base-transition probabilities
-    probabilities = dict()
-
-    def _setup(self, parser: 'Parser'):
-        """
-        Determine base transition probabilities for polymorphic sites.
-        We do this to calibrate the number of monomorphic sites.
-
-        :param parser: The parser
-        """
-        self.parser = parser
-
-        logger.info(f'Determining base transition probabilities.')
-
-        # initialize counts
-        counts = {base_transition: 0 for base_transition in self.get_types()}
-
-        with parser.get_pbar() as pbar:
-
-            # count base transitions
-            for i, variant in enumerate(VCF(parser.vcf)):
-                if variant.is_snp:
-                    try:
-                        counts[self.get_type(variant)] += 1
-                    except NoTypeException:
-                        pass
-
-                pbar.update()
-
-        # normalize counts to probabilities
-        self.probabilities = {k: v / sum(counts.values()) for k, v in counts.items()}
-
     @count_no_type
     def get_type(self, variant: Variant) -> str:
         """
         Get the base transition for the given variant.
 
         :param variant: The vcf site
         :return: Base transition
         :raises NoTypeException: if not type could be determined
         """
         if variant.is_snp:
-            ref = variant.REF
-
-            # assume there is at most one alternate allele
-            alt = variant.ALT[0]
-
-            # obtain ancestral allele
-            aa = variant.INFO.get(self.parser.info_ancestral)
-
-            # swap reference and alternative allele
-            # note that here we assume again the site is bi-allelic
-            if aa in bases and aa != ref:
-                ref, alt = alt, ref
-
-            # report type if aa tag is valid or if we don't skip non-polarized sites
-            if aa in bases or not self.parser.ignore_not_polarized:
+            ancestral = self.parser._get_ancestral(variant)
 
-                if ref == alt:
-                    raise NoTypeException("Site marked as polymorphic, but reference "
-                                          "and alternative allele are the same.")
+            derived = variant.REF if variant.REF != ancestral else variant.ALT[0]
 
-                return f"{ref}>{alt}"
+            if ancestral in bases and derived in bases and ancestral != derived:
+                return f"{ancestral}>{derived}"
 
-            raise NoTypeException("No valid AA tag found.")
+            raise NoTypeException("Not a valid base transition.")
 
-        # for mono-allelic sites, we sample from the base-transition probabilities
-        return self.parser.rng.choice(list(self.probabilities.keys()), p=list(self.probabilities.values()))
+        raise NoTypeException("Site is not a SNP.")
 
     def get_types(self) -> List[str]:
         """
         Get all possible base transitions.
 
         :return: List of contexts
         """
         return ['>'.join([a, b]) for a in bases for b in bases if a != b]
 
 
 class AncestralBaseStratification(Stratification):
     """
     Stratify the SFS by the base context of the mutation: the reference base.
-    If ``ignore_not_polarized`` is set to ``True``, we skip sites
+    If ``skip_non_polarized`` is set to ``True``, we skip sites
     that are not polarized, otherwise we use the reference allele as ancestral base.
     By default, we use the ``AA`` tag to determine the ancestral allele.
 
     Any subclass of :class:`~fastdfe.parser.AncestralAnnotation` can be used to annotate the ancestral allele.
     """
 
     @count_no_type
     def get_type(self, variant: Variant) -> str:
         """
         Get the type which is the reference allele.
 
         :param variant: The vcf site
         :return: reference allele
         """
-        try:
-            return self._get_ancestral(variant)
-        except ValueError:
-            raise NoTypeException("Invalid ancestral allele: Ancestral allele must be a valid base.")
+        return self.parser._get_ancestral(variant)
 
     def get_types(self) -> List[str]:
         """
         The possible base types.
 
         :return: List of contexts
         """
         return bases
 
 
 class TransitionTransversionStratification(BaseTransitionStratification):
     """
     Stratify the SFS by whether we have a transition or transversion.
-    We parse the VCF file twice here, once to determine the transition-transversion
-    probabilities used for the monomorphic counts, and once to stratify the SFS.
-    Note that we assume sites here to be at most bi-allelic.
+    Should be used with ``n_target_sites`` since we can't infer the type of monomorphic sites.
     """
 
-    #: Transition-transversion probabilities
-    probabilities = dict(
-        transition=0.5,
-        transversion=0.5
-    )
-
-    def _setup(self, parser: 'Parser'):
-        """
-        Determine transition-transversion probabilities for polymorphic sites.
-        We do this to calibrate the number of monomorphic sites.
-
-        :param parser: The parser
-        """
-        self.parser = parser
-
-        logger.info(f'Determining transition-transversion probabilities.')
-
-        # initialize counts
-        counts = dict(
-            transition=0,
-            transversion=0
-        )
-
-        with parser.get_pbar() as pbar:
-
-            # count transitions and transversions
-            for i, variant in enumerate(VCF(parser.vcf)):
-                if variant.is_snp:
-                    counts[self.get_type(variant)] += 1
-
-                pbar.update()
-
-        # normalize counts to probabilities
-        self.probabilities = {k: v / sum(counts.values()) for k, v in counts.items()}
-
     @count_no_type
     def get_type(self, variant: Variant) -> str:
         """
         Get the mutation type (transition or transversion) for a given mutation.
 
         :param variant: The vcf site
         :return: Mutation type
         """
         if variant.is_snp:
+
+            if variant.ALT[0] not in bases:
+                raise NoTypeException("Invalid alternate allele: Alternate allele must be a valid base.")
+
             if (variant.REF, variant.ALT[0]) in [('A', 'G'), ('G', 'A'), ('C', 'T'), ('T', 'C')]:
                 return "transition"
             else:
                 return "transversion"
 
-        # for mono-allelic sites, we sample from the transition-transversion probabilities
-        return self.parser.rng.choice(list(self.probabilities.keys()), p=list(self.probabilities.values()))
+        raise NoTypeException("Site is not a SNP.")
 
     def get_types(self) -> List[str]:
         """
         All possible mutation types (transition and transversion).
 
         :return: List of mutation types
         """
@@ -400,14 +280,16 @@
             custom_callback: Callable[[Variant], str] = None,
     ):
         """
         Initialize the stratification.
 
         :param custom_callback: Custom callback to determine the type of mutation
         """
+        super().__init__()
+
         #: Custom callback to determine the degeneracy of mutation
         self.get_degeneracy = custom_callback if custom_callback is not None else self._get_degeneracy_default
 
     @staticmethod
     def _get_degeneracy_default(variant: Variant) -> Optional[Literal['neutral', 'selected']]:
         """
         Get degeneracy based on 'Degeneracy' tag.
@@ -446,16 +328,15 @@
         :return: List of contexts
         """
         return ['neutral', 'selected']
 
 
 class SynonymyStratification(Stratification):
     """
-    Stratify SFS by synonymy (neutral or selected). Note that we extrapolate the number of monomorphic sites
-    for each type from the relative number of types for polymorphic sites.
+    Stratify SFS by synonymy (neutral or selected).
 
     :class:`~fastdfe.annotation.SynonymyAnnotation` can be used to annotate the synonymy of a site.
     """
 
     def get_types(self) -> List[str]:
         """
         Get all possible synonymy types (``neutral`` and ``selected``).
@@ -485,16 +366,21 @@
 
             raise NoTypeException(f"Synonymy tag has invalid value: '{synonymy}' at {variant.CHROM}:{variant.POS}")
 
 
 class VEPStratification(SynonymyStratification):
     """
     Stratify SFS by synonymy (neutral or selected) based on annotation provided by VEP.
+    Note that since we cannot determine the synonymy for monomorphic sites, this should be used together
+    with ``n_target_sites``.
     """
 
+    #: The tag used by VEP to annotate the synonymy
+    info_tag = 'CSQ'
+
     def get_types(self) -> List[str]:
         """
         Get all possible synonymy types (``neutral`` and ``selected``).
 
         :return: List of contexts
         """
         return ['neutral', 'selected']
@@ -503,55 +389,124 @@
     def get_type(self, variant: Variant) -> Literal['neutral', 'selected']:
         """
         Get the synonymy of a site.
 
         :param variant: The vcf site
         :return: Type of the mutation, either ``neutral`` or ``selected``
         """
-        synonymy = variant.INFO.get('CSQ')
+        synonymy = variant.INFO.get(self.info_tag, '')
 
         if 'synonymous_variant' in synonymy:
             return 'neutral'
 
         if 'missense_variant' in synonymy:
             return 'selected'
 
         raise NoTypeException(f"Synonymy tag has invalid value: '{synonymy}' at {variant.CHROM}:{variant.POS}")
 
 
-class SnpEffStratification(SynonymyStratification):
+class SnpEffStratification(VEPStratification):
     """
     Stratify SFS by synonymy (neutral or selected) based on annotation provided by SnpEff.
+    Note that since we cannot determine the synonymy for monomorphic sites, this should be used together
+    with ``n_target_sites``.
     """
 
+    #: The tag used by SnpEff to annotate the synonymy
+    info_tag = 'ANN'
+
+
+class GenomePositionDependentStratification(Stratification, ABC):
+    pass
+
+
+class ContigStratification(GenomePositionDependentStratification):
+    """
+    Stratify SFS by contig.
+    """
+
+    def get_type(self, variant: Variant) -> str:
+        """
+        Get the contig.
+
+        :param variant: The vcf site
+        :return: The contig name
+        """
+        return variant.CHROM
+
     def get_types(self) -> List[str]:
         """
-        Get all possible synonymy types (``neutral`` and ``selected``).
+        Get all possible contig type.
 
         :return: List of contexts
         """
-        return ['neutral', 'selected']
+        return list(self.parser.reader.seqnames)
 
-    @count_no_type
-    def get_type(self, variant: Variant) -> Literal['neutral', 'selected']:
+
+class ChunkedStratification(GenomePositionDependentStratification):
+    """
+    Stratify SFS by creating ``n`` chunks of roughly equal size.
+    """
+
+    def __init__(self, n_chunks: int):
         """
-        Get the synonymy of a site.
+        Initialize the stratification.
+
+        :param n_chunks: Number of sites per window
+        """
+        super().__init__()
+
+        #: Number of chunks
+        self.n_chunks: int = n_chunks
+
+        #: List of chunk sizes
+        self.chunk_sizes: Optional[List[int]] = None
+
+        #: Number of sites seen so far
+        self.counter: int = 0
+
+    def _setup(self, parser: 'Parser'):
+        """
+        Set up the stratification.
+
+        :param parser: The parser
+        """
+        super()._setup(parser)
+
+        # compute base chunk size and remainder
+        base_chunk_size, remainder = divmod(parser.n_sites, self.n_chunks)
+
+        # create list of chunk sizes
+        self.chunk_sizes = [base_chunk_size + (i < remainder) for i in range(self.n_chunks)]
+
+    def get_types(self) -> List[str]:
+        """
+        Get all possible window types.
+
+        :return: List of contexts
+        """
+        return [f'chunk{i}' for i in range(self.n_chunks)]
+
+    def get_type(self, variant: Variant) -> str:
+        """
+        Get the type.
 
         :param variant: The vcf site
-        :return: Type of the mutation, either ``neutral`` or ``selected``
+        :return: The type
         """
-        synonymy = variant.INFO.get('CSQ')
+        # find the index of the chunk to which the current site belongs
+        chunk_index = next(i for i, size in enumerate(self.chunk_sizes) if self.counter < sum(self.chunk_sizes[:i + 1]))
 
-        if 'synonymous_variant' in synonymy:
-            return 'neutral'
+        # get the type
+        t = f'chunk{chunk_index}'
 
-        if 'missense_variant' in synonymy:
-            return 'selected'
+        # update the counter
+        self.counter += 1
 
-        raise NoTypeException(f"Synonymy tag has invalid value: '{synonymy}' at {variant.CHROM}:{variant.POS}")
+        return t
 
 
 class Parser(VCFHandler):
     """
     Parse site-frequency spectra from VCF files.
 
     By default, the parser looks at the ``AA`` tag in the VCF file's info field to retrieve
@@ -563,169 +518,242 @@
     sites and their ancestral alleles. This is done by providing a list of annotations to
     the parser. The annotations are applied in the order they are provided.
 
     The parser also allows to filter sites based on their annotations. This is done by
     providing a list of filtrations to the parser. By default, we filter out poly-allelic
     sites which is highly recommended as some stratifications assume sites to be at most bi-allelic.
 
-    :warning: Not tested for polyploids.
+    Example usage:
+
+    ::
+
+        from fastdfe import Parser, DegeneracyAnnotation, DegeneracyStratification, \\
+            MaximumParsimonyAnnotation, CodingSequenceFiltration
+
+        # parse selected and neutral SFS from human chromosome 21
+        p = Parser(
+            vcf="http://ftp.1000genomes.ebi.ac.uk/vol1/ftp/data_collections/"
+                "1000_genomes_project/release/20181203_biallelic_SNV/"
+                "ALL.chr21.shapeit2_integrated_v1a.GRCh38.20181129.phased.vcf.gz",
+            n=10,
+            annotations=[
+                DegeneracyAnnotation(
+                    fasta_file="http://ftp.ensembl.org/pub/release-109/fasta/homo_sapiens/"
+                               "dna/Homo_sapiens.GRCh38.dna.chromosome.21.fa.gz",
+                    gff_file="http://ftp.ensembl.org/pub/release-109/gff3/homo_sapiens/"
+                             "Homo_sapiens.GRCh38.109.chromosome.21.gff3.gz",
+                    aliases=dict(chr21=['21'])
+                ),
+                MaximumParsimonyAnnotation()
+            ],
+            filtrations=[
+                CodingSequenceFiltration(
+                    gff_file="http://ftp.ensembl.org/pub/release-109/gff3/homo_sapiens/"
+                             "Homo_sapiens.GRCh38.109.chromosome.21.gff3.gz",
+                    aliases=dict(chr21=['21'])
+                )
+            ],
+            stratifications=[DegeneracyStratification()],
+        )
+
+        sfs = p.parse()
+
+        sfs.plot()
+
     """
 
     def __init__(
             self,
             vcf: str | Iterable[Variant],
             n: int,
             info_ancestral: str = 'AA',
-            ignore_not_polarized: bool = False,
-            stratifications: List[Stratification] = [
-                DegeneracyStratification()
-            ],
+            skip_non_polarized: bool = False,
+            stratifications: List[Stratification] = [],
             annotations: List[Annotation] = [],
             filtrations: List[Filtration] = [PolyAllelicFiltration()],
+            samples: List[str] = None,
             max_sites: int = np.inf,
             n_target_sites: int = None,
-            seed: int | None = 0
+            seed: int | None = 0,
+            cache: bool = True
     ):
         """
         Initialize the parser.
 
         :param vcf: The path to the VCF file or an iterable of variants, can be gzipped, urls are also supported
         :param n: The number of individuals in the sample. We down-sample to this number by drawing without replacement.
             Sites with fewer than ``n`` individuals are skipped.
         :param info_ancestral: The tag in the INFO field that contains the ancestral allele
-        :param ignore_not_polarized: Whether to ignore sites that are not polarized, i.e., without a valid info tag
+        :param skip_non_polarized: Whether to skip sites that are not polarized, i.e., without a valid info tag
             providing the ancestral allele
         :param stratifications: List of stratifications to use
         :param annotations: List of annotations to use
         :param filtrations: List of filtrations to use.
+        :param samples: List of samples to use. If ``None``, all samples are used.
         :param max_sites: Maximum number of sites to parse
         :param n_target_sites: The number of mutational target sites.
             Allows to adjust the number of monomorphic site count. Ideally, we obtain the SFS by
             parsing VCF files that contain both mono- and polymorphic sites. This is because for DFE inference, we
             require the number of monomorphic sites to calibrate the mutation rate. However, often, only polymorphic
             sites are available. In this case, we can use ``n_target_sites`` to extrapolate the number of monomorphic
-            sites by looking at the relative number of polymorphic sites for each type. Note that the total number of
+            sites by looking at the relative number of polymorphic sites for each type. Note that the *total* number of
             mono- and polymorphic sites should be specified here. This often corresponds to the number of sites in
-            coding regions over the sequence considered.
-        :param seed: Seed for the random number generator
+            coding regions over the sequence considered. If ``None``, and
+            :class:`~fastdfe.annotation.SynonymyAnnotation` is used, the number
+            of monomorphic sites is inferred dynamically from the length of the coding sequences considered.
+            Alternatively, you can use :meth:`~fastdfe.annotation.Annotation.count_target_sites` to count the number of
+            coding sites.
+        :param seed: Seed for the random number generator. Use ``None`` for no seed.
+        :param cache: Whether to cache files downloaded from urls
         """
         super().__init__(
             vcf=vcf,
+            info_ancestral=info_ancestral,
             max_sites=max_sites,
             seed=seed,
-            info_ancestral=info_ancestral
+            cache=cache
         )
 
         #: The number of individuals in the sample
-        self.n = n
+        self.n: int = n
 
         #: The number of mutational target sites
         self.n_target_sites: int | None = n_target_sites
 
-        #: Whether to ignore sites that are not polarized, i.e., without a valid info tag providing the ancestral allele
-        self.ignore_not_polarized: bool = ignore_not_polarized
+        #: The list of samples to use
+        self.samples: List[str] | None = samples
+
+        #: The mask of samples to use
+        self.samples_mask: np.ndarray | None = None
+
+        #: Whether to skip sites that are not polarized, i.e., without a valid info tag providing the ancestral allele
+        self.skip_non_polarized: bool = skip_non_polarized
 
         #: List of stratifications to use
         self.stratifications: List[Stratification] = stratifications
 
         #: List of annotations to use
         self.annotations: List[Annotation] = annotations
 
         #: List of filtrations to use
         self.filtrations: List[Filtration] = filtrations
 
         #: The number of sites that were skipped for various reasons
         self.n_skipped: int = 0
 
-        #: Dictionary of SFS indexed by type
+        #: Dictionary of SFS indexed by joint type
         self.sfs: Dict[str, np.ndarray] = {}
 
         #: The VCF reader
         self.reader: Optional[VCF] = None
 
-    def _create_sfs_dictionary(self):
+    def _get_ancestral(self, variant: Variant) -> str:
+        """
+        Determine the ancestral allele.
+
+        :param variant: The vcf site
+        :return: Ancestral allele
+        :raises NoTypeException: If the site is not polarized and ``skip_non_polarized`` is ``True``
+        """
+        if variant.is_snp:
+            # obtain ancestral allele
+            aa = variant.INFO.get(self.info_ancestral)
+
+            # return the ancestral allele if it is a valid base
+            if aa in bases:
+                return aa
+
+            # if we skip non-polarized sites, we raise an error here
+            if self.skip_non_polarized:
+                raise NoTypeException("No valid AA tag found so we skip the site")
+
+        # if we don't skip non-polarized sites, or if the site is not an SNP
+        # we return the reference allele if valid
+        if variant.REF in bases:
+            return variant.REF
+
+        # if the reference allele is not a valid base, we raise an error
+        raise NoTypeException("Reference allele is not a valid base")
+
+    def _create_sfs_dictionary(self) -> Dict[str, np.ndarray]:
         """
         Create an SFS dictionary initialized with all possible base contexts.
 
         :return: SFS dictionary
         """
         types = [s.get_types() for s in self.stratifications]
+
         # define the DNA bases
         contexts = ['.'.join(t) for t in itertools.product(*types)]
 
         # create dict
         sfs = {}
         for context in contexts:
             sfs[context] = np.zeros(self.n + 1)
 
-        self.sfs = sfs
+        return sfs
 
     def _parse_site(self, variant: Variant):
         """
         Parse a single site.
 
         :param variant: The variant
         """
+        if variant.is_snp:
 
-        # number of samples
-        n_samples = variant.ploidy * variant.num_called
-
-        # skip if not enough samples
-        if n_samples < self.n:
-            logger.debug(f'Skipping site due to too few samples at {variant.CHROM}:{variant.POS}.')
-            self.n_skipped += 1
-            return
-
-        # determine reference allele count
-        # this doesn't work for polyploids
-        n_ref = variant.ploidy * variant.num_hom_ref + variant.num_het
-
-        # swap reference and alternative allele if the AA info field
-        # is defined and indicates so
-        aa = variant.INFO.get(self.info_ancestral)
+            # obtain called bases
+            genotypes = get_called_bases(variant.gt_bases[self.samples_mask])
 
-        if aa not in bases:
+            # number of samples
+            n_samples = len(genotypes)
 
-            # log a warning
-            logger.debug(f'No valid ancestral allele defined at {variant.CHROM}:{variant.POS}.')
+            # skip if not enough samples
+            if n_samples < self.n:
+                self.logger.debug(f'Skipping site due to too few samples at {variant.CHROM}:{variant.POS}.')
+                self.n_skipped += 1
+                return
 
-            if self.ignore_not_polarized:
+            try:
+                # determine ancestral allele
+                aa = self._get_ancestral(variant)
+            except NoTypeException:
                 self.n_skipped += 1
                 return
-        else:
-            # adjust orientation if the ancestral allele is not the reference
-            if aa != variant.REF:
 
-                # change alternative allele if defined
-                if len(variant.ALT) != 0:
-                    # we only consider the first alternative allele
-                    variant.ALT[0] = variant.REF
+            # count called bases
+            counter = Counter(genotypes)
 
-                # change reference allele
-                variant.REF = aa
+            # determine ancestral allele count
+            n_aa = counter[aa]
 
-                # change reference count
-                n_ref = n_samples - n_ref
+            # determine down-projected allele count
+            k = self.rng.hypergeometric(ngood=n_samples - n_aa, nbad=n_aa, nsample=self.n)
 
-        # determine down-projected allele count
-        k = self.rng.hypergeometric(ngood=n_samples - n_ref, nbad=n_ref, nsample=self.n)
+        else:
+            # if we don't have an SNP, we assume the reference allele to be the ancestral allele,
+            # so the derived allele count is 0
+            k = 0
 
         # try to obtain type
         try:
-            t = '.'.join([s.get_type(variant) for s in self.stratifications])
+            # create joint type
+            t = '.'.join([s.get_type(variant) for s in self.stratifications]) or 'all'
 
-            # add count by 1 if context is defined
-            if t in self.sfs:
-                self.sfs[t][k] += 1
+            # if the type is not in the dictionary, we add it
+            if t not in self.sfs:
+                self.sfs[t] = np.zeros(self.n + 1)
+
+            # add count by 1
+            self.sfs[t][k] += 1
 
         except NoTypeException as e:
             self.n_skipped += 1
-            logger.debug(e)
+            self.logger.debug(e)
 
-    def _handle_site(self, variant: Variant):
+    def _process_site(self, variant: Variant):
         """
         Handle a single site.
 
         :param variant: The variant
         """
         # filter the variant
         for filtration in self.filtrations:
@@ -760,80 +788,106 @@
         # total number of polymorphic sites across all types
         n_polymorphic = np.sum([np.sum(c[1:-1]) for c in self.sfs.values()])
 
         for t, counts in self.sfs.items():
             self.sfs[t][0] = np.sum(counts[1:-1]) / n_polymorphic * (self.n_target_sites - n_polymorphic)
             self.sfs[t][-1] = 0
 
+    def _update_target_sites(self):
+        """
+        Update the number of target sites based on the SynonymyAnnotation if present.
+        """
+
+        if self.n_target_sites is None:
+
+            # find index of SynonymyAnnotation in list
+            index = next((i for i, a in enumerate(self.annotations) if isinstance(a, SynonymyAnnotation)), -1)
+
+            if index != -1:
+                self.logger.info(f'Updating target sites based on SynonymyAnnotation.')
+
+                self.n_target_sites = cast(SynonymyAnnotation, self.annotations[index]).n_target_sites
+
     def parse(self) -> Spectra:
         """
         Parse the VCF file.
 
         :return: The spectra for the different stratifications
         """
-        self._create_sfs_dictionary()
-
-        # create a string representation of the stratifications
-        representation = '.'.join(['[' + ', '.join(s.get_types()) + ']' for s in self.stratifications])
-
-        # log the stratifications
-        logger.info(f'Using stratification: {representation}.')
+        # create reader
+        self.reader = VCF(self.download_if_url(self.vcf))
 
         # count the number of sites
         self.n_sites = self.count_sites()
 
         # make parser available to stratifications
         for s in self.stratifications:
             s._setup(self)
 
-        # touch all filtrations
-        for f in self.filtrations:
-            f._setup()
+        # create a string representation of the stratifications
+        representation = '.'.join(['[' + ', '.join(s.get_types()) + ']' for s in self.stratifications]) or "[all]"
+
+        # log the stratifications
+        self.logger.info(f'Using stratification: {representation}.')
 
         # instantiate annotator to provide context to annotations
         ann = Annotator(
             vcf=self.vcf,
             max_sites=self.max_sites,
             seed=self.seed,
             info_ancestral=self.info_ancestral,
             annotations=[],
             output=''
         )
 
-        # create reader
-        reader = VCF(self.download_if_url(self.vcf))
+        # create samples mask
+        if self.samples is None:
+            self.samples_mask = np.ones(len(self.reader.samples)).astype(bool)
+        else:
+            self.samples_mask = np.isin(self.reader.samples, self.samples)
 
         # provide annotator to annotations and add info fields
         for annotation in self.annotations:
-            annotation._setup(ann)
-            annotation._add_info(reader)
+            annotation._setup(ann, self.reader)
+
+        # touch all filtrations
+        for f in self.filtrations:
+            f._setup(self.reader)
 
-        logger.info(f'Starting to parse.')
+        self.logger.info(f'Starting to parse.')
 
         # create progress bar
         with self.get_pbar() as pbar:
 
-            for i, variant in enumerate(reader):
+            for i, variant in enumerate(self.reader):
 
                 # handle site
-                self._handle_site(variant)
+                self._process_site(variant)
 
                 pbar.update()
 
                 # explicitly stopping after ``n``sites fixes a bug with cyvcf2:
                 # 'error parsing variant with `htslib::bcf_read` error-code: 0 and ret: -2'
                 if i + 1 == self.n_sites or i + 1 == self.max_sites:
                     break
 
         # tear down all objects
         self._teardown()
 
         # close reader
-        reader.close()
+        self.reader.close()
+
+        # update target sites
+        self._update_target_sites()
 
         # correct monomorphic counts if number of target sites is defined
         if self.n_target_sites is not None:
             self._infer_monomorphic_counts()
 
-        logger.info(f'Parsed {self.n_sites - self.n_skipped} out of {self.n_sites} sites in total.')
+        if len(self.sfs) == 0:
+            self.logger.warning(f"No sites were included in the spectra. If this is not expected, "
+                                "please check that all components work as expected. You can do this by "
+                                "setting the log level to DEBUG.")
+        else:
+            self.logger.info(f'Included {self.n_sites - self.n_skipped} out of {self.n_sites} sites in total.')
 
-        return Spectra(self.sfs)
+        return Spectra(self.sfs).sort_types()
```

### Comparing `fastdfe-0.1.6b0/fastdfe/polydfe.py` & `fastdfe-0.1.7b0/fastdfe/polydfe.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 from matplotlib import pyplot as plt
 from rpy2.robjects.packages import importr
 from rpy2.robjects.vectors import ListVector
 from typing_extensions import Self
 
 from .abstract_inference import AbstractInference, Inference
 from .config import Config
-from .parametrization import from_string, Parametrization, DiscreteParametrization
+from .parametrization import _from_string, Parametrization, DiscreteParametrization
 from .polydfe_utils import create_sfs_config, models
 
 # get logger
-logger = logging.getLogger('fastdfe')
+logger = logging.getLogger('fastdfe').getChild('PolydfeWrapper')
 
 
 class PolyDFEResult:
     """
     Class for parsing polyDFE output.
     """
     # default postprocessing source
@@ -230,34 +230,34 @@
             return subprocess.run(command, check=True, cwd=wd, shell=True)
 
         # define default function for executing command
         if execute is None:
             execute = shell
 
         # save the spectra and init file, so they can be reviewed if necessary
-        # use tempfile to generate the file name.
+        # use temp file to generate the file name.
         with open(tempfile.NamedTemporaryFile().name, 'w') as spectra_file:
             with open(tempfile.NamedTemporaryFile().name, 'w') as init_file:
                 # save files
                 self.config.create_polydfe_sfs_config(spectra_file.name)
                 self.config.create_polydfe_init_file(init_file.name, n=self.config.data['sfs_neut'].n)
 
                 # add number of fragment if model is DiscreteParametrization
-                model = from_string(self.config.data['model'])
+                model = _from_string(self.config.data['model'])
                 k = str(model.k - 1) + ' ' if isinstance(model, DiscreteParametrization) else ''
 
                 # construct command string
                 command = (f"{bin} "
                            f"-d {spectra_file.name} "
                            f"-m {self.config.get_polydfe_model()} {k}"
                            f"-i {init_file.name} 1 "
                            f"-v 1 > {output_file}")
 
                 # log command signature
-                logger.info(f"Running: {command}")
+                self.logger.info(f"Running: '{command}'")
 
                 # execute command
                 execute(command)
 
         # add execution time
         self.execution_time += time.time() - start_time
 
@@ -316,15 +316,17 @@
         self.bootstraps.drop(columns=['r', 'eps_cont'], inplace=True)
 
         # update execution time
         self.summary.data['execution_time'] += np.sum([bs.summary.data['execution_time'] for bs in bootstraps])
 
     def plot_all(self, show: bool = True):
         """
-        Plot everything.
+        Plot a bunch of plots.
+
+        :param show: Whether to show the plot
         """
         self.plot_inferred_parameters(show=show)
         self.plot_discretized(show=show)
 
     def plot_inferred_parameters(
             self,
             confidence_intervals: bool = True,
@@ -332,49 +334,55 @@
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             scale: Literal['lin', 'log', 'symlog'] = 'log',
             legend: bool = True,
             ax: plt.Axes = None,
+            kwargs_legend: dict = dict(prop=dict(size=8), loc='upper right'),
     ) -> plt.Axes:
         """
         Visualize the inferred parameters and their confidence intervals.
 
         :param scale: Scale of the y-axis
+        :param confidence_intervals: Whether to show confidence intervals
+        :param ci_level: Confidence interval level
+        :param bootstrap_type: Type of bootstrap
         :param legend: Show legend
         :param ax: Axes object
         :param title: Title of the plot
         :param show: Show the plot
         :param file: File to save the plot to
         :param show: Show the plot
         :param ax: Axes object
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes object
         """
         return Inference.plot_inferred_parameters(
             inferences=[self],
             labels=['all'],
             confidence_intervals=confidence_intervals,
             ci_level=ci_level,
             bootstrap_type=bootstrap_type,
             file=file,
             show=show,
             title=title,
             legend=legend,
             scale=scale,
-            ax=ax
+            ax=ax,
+            kwargs_legend=kwargs_legend
         )
 
     def get_bootstrap_param_names(self) -> List[str]:
         """
         Parameter names for parameters included in bootstraps.
 
         :return: List of parameter names
         """
-        return from_string(self.config.data['model']).param_names + ['eps', 'alpha']
+        return _from_string(self.config.data['model']).param_names + ['eps', 'alpha']
 
     def get_bootstrap_params(self) -> Dict[str, float]:
         """
         Get the parameters to be included in the bootstraps.
 
         :return: Dict of parameters
         """
@@ -405,15 +413,15 @@
     def model(self) -> Parametrization:
         """
         Get the DFE parametrization.
 
         :return: Parametrization
         """
 
-        return from_string(self.config.data['model'])
+        return _from_string(self.config.data['model'])
 
     @model.setter
     def model(self, value):
         """
         Set the DFE parametrization.
 
         :param value: Parametrization
```

### Comparing `fastdfe-0.1.6b0/fastdfe/polydfe_utils.py` & `fastdfe-0.1.7b0/fastdfe/polydfe_utils.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.6b0/fastdfe/spectrum.py` & `fastdfe-0.1.7b0/fastdfe/spectrum.py`

 * *Files 5% similar despite different names*

```diff
@@ -254,36 +254,39 @@
 
     def plot(
             self,
             show: bool = True,
             file: str = None,
             title: str = None,
             show_monomorphic: bool = False,
+            kwargs_legend: dict = dict(prop=dict(size=8)),
             ax: plt.Axes = None
     ) -> plt.Axes:
         """
         Plot spectrum.
 
         :param show: Whether to show plot
         :param file: File to save plot to
         :param title: Title of plot
         :param show_monomorphic: Whether to show monomorphic counts
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :param ax: Axes to plot on
         :return: Axes
         """
         # import locally to avoid circular dependencies
         from fastdfe import Visualization
 
         return Visualization.plot_sfs_comparison(
             spectra=[self],
             file=file,
             show=show,
             title=title,
             show_monomorphic=show_monomorphic,
-            ax=ax
+            ax=ax,
+            kwargs_legend=kwargs_legend
         )
 
     @staticmethod
     def standard_kingman(n: int) -> 'Spectrum':
         """
         Get standard Kingman SFS.
 
@@ -494,30 +497,30 @@
         return self.k
 
     def __add__(self, other: 'Spectra') -> 'Spectra':
         """
         Merge types of two spectra objects by adding up their counts entry-wise.
 
         :param other: Spectra object
-        :return: Spectra object
+        :return: Spectra with merged types
         """
         return Spectra.from_dataframe(self.data.add(other.data, fill_value=0))
 
-    def __getitem__(self, keys) -> Union['Spectrum', 'Spectra']:
+    def __getitem__(self, keys: str | List[str] | np.ndarray | tuple) -> Union['Spectrum', 'Spectra']:
         """
         Get item.
 
-        :param keys: string or list of strings
-        :return: Spectrum or Spectra
+        :param keys: string or list of strings, possibly regex to match type names
+        :return: Spectrum or Spectra depending on the number of matches
         """
         # whether the input in an array
         is_array = isinstance(keys, (np.ndarray, list, tuple))
 
-        # use regex to select columns
-        subset = self.data.filter(regex=('|'.join(keys) if is_array else keys))
+        # use regex to subset dataframe using column names
+        subset = self.data.loc[:, self.data.columns.str.fullmatch('|'.join(keys) if is_array else keys)]
 
         # return spectrum object if only one column is left
         # and if not multiple keys were supplied
         if subset.shape[1] == 1 and not is_array:
             return Spectrum.from_list(list(subset.iloc[:, 0]))
 
         # wrap subset dataframe in spectra object
@@ -629,15 +632,15 @@
         :return: Merged Spectra object
         """
         return Spectra(self.to_dict() | s.to_dict())
 
     @staticmethod
     def from_dict(data: dict) -> 'Spectra':
         """
-        Load from dictionary.
+        Load from nested dictionary first indexed by types and then by samples.
 
         :param data: Dictionary of lists indexed by types
         :return: Spectra object
         """
         lists = [list(v.values() if isinstance(v, dict) else v) for v in data.values()]
 
         return Spectra.from_list(lists, types=list(data.keys()))
@@ -661,17 +664,17 @@
         :return: Spectra object
         """
         return Spectra.from_dataframe(pd.read_csv(file))
 
     @staticmethod
     def from_spectra(spectra: Dict[str, Spectrum]) -> 'Spectra':
         """
-        Create from dict of spectrum objects indexed by types.
+        Create from dict of spectrum objects indexed by type.
 
-        :param spectra: Dictionary of spectrum objects indexed by types
+        :param spectra: Dictionary of spectrum objects indexed by type
         :return: Spectra object
         """
         return Spectra.from_list([sfs.to_list() for sfs in spectra.values()], types=list(spectra.keys()))
 
     @staticmethod
     def from_spectrum(sfs: Spectrum) -> 'Spectra':
         """
@@ -685,58 +688,69 @@
     def plot(
             self,
             show: bool = True,
             file: str = None,
             title: str = None,
             use_subplots: bool = False,
             show_monomorphic: bool = False,
+            kwargs_legend: dict = dict(prop=dict(size=8)),
             ax: plt.Axes = None
     ) -> plt.Axes:
         """
         Visualize spectra.
 
         :param show: Whether to show the plot
         :param file: File name to save the plot to
         :param title: Plot title
         :param use_subplots: Whether to use subplots
         :param show_monomorphic: Whether to show monomorphic sites
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :param ax: Axes to plot on
         :return: Axes
         """
         # import locally to avoid circular dependencies
         from fastdfe import Visualization
 
         return Visualization.plot_sfs_comparison(
             spectra=list(self.to_spectra().values()),
             labels=self.types,
             file=file,
             show=show,
             title=title,
             use_subplots=use_subplots,
             show_monomorphic=show_monomorphic,
+            kwargs_legend=kwargs_legend,
             ax=ax
         )
 
-    def remove_empty(self) -> 'Spectra':
+    def drop_empty(self) -> 'Spectra':
         """
         Remove types whose spectra have no counts.
 
         :return: Spectra with non-empty types
         """
         return Spectra.from_dataframe(self.data.loc[:, self.data.any()])
 
-    def remove_zero_entries(self) -> 'Spectra':
+    def drop_zero_entries(self) -> 'Spectra':
         """
         Remove types whose spectra have some zero entries.
         Note that we ignore zero counts in the last entry i.e. fixed derived alleles.
 
         :return: Spectra with non-zero entries
         """
         return Spectra.from_dataframe(self.data.loc[:, self.data[:-1].all()])
 
+    def drop_sparse(self, n_polymorphic: int) -> 'Spectra':
+        """
+        Remove types whose spectra have fewer than equal ``n_polymorphic`` polymorphic sites.
+
+        :return: Spectra
+        """
+        return Spectra.from_dataframe(self.data.loc[:, self.data[1:-1].sum() > n_polymorphic])
+
     def rename(self, names: List[str]) -> 'Spectra':
         """
         Rename types.
 
         :param names: New names
         :return: Spectra with renamed types
         """
@@ -777,14 +791,22 @@
         """
         Check whether spectra are folded.
 
         :return: Dictionary of types and whether they are folded
         """
         return {t: s.is_folded() for t, s in self.to_spectra().items()}
 
+    def sort_types(self) -> 'Spectra':
+        """
+        Sort types alphabetically.
+
+        :return: Sorted spectra object
+        """
+        return Spectra.from_dataframe(self.data.sort_index(axis=1))
+
 
 def parse_polydfe_sfs_config(file: str) -> Spectra:
     """
     Parse frequency spectra and mutational target site from
     polyDFE configuration file.
 
     :param file: File name
```

### Comparing `fastdfe-0.1.6b0/fastdfe/visualization.py` & `fastdfe-0.1.7b0/fastdfe/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 import functools
 import logging
 from typing import Callable, List, Literal, Dict
 
 import matplotlib.colors as mcolors
 import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
 import seaborn as sns
 from matplotlib import colors
 from matplotlib.colors import LogNorm
 from matplotlib.container import BarContainer
 from matplotlib.ticker import MaxNLocator
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
-from . import Parametrization
+from .parametrization import Parametrization
 from .spectrum import Spectrum
 
 # get logger
-logger = logging.getLogger('fastdfe')
+logger = logging.getLogger('fastdfe').getChild('Visualization')
 
 
 class Visualization:
     """
     Visualization class.
     """
 
@@ -143,28 +144,30 @@
             errors: list | np.ndarray = None,
             labels: list | np.ndarray = None,
             file: str = None,
             show: bool = True,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             title: str = 'discretized DFE',
             interval_labels: List[str] = None,
+            kwargs_legend: dict = dict(prop=dict(size=8)),
 
     ) -> plt.Axes:
         """
         Plot discretized DFEs using a bar plot.
 
-        :param interval_labels: Labels for the intervals
-        :param labels: Labels for the DFEs
+        :param interval_labels: Labels for the intervals (which are the same for all types)
+        :param labels: Labels for the different types of DFEs
         :param title: Title of the plot
-        :param values: Array of values of size ``intervals.shape[0] - 1``
-        :param errors: Array of errors of size ``intervals.shape[0] - 1``
+        :param values: Array of values of size ``intervals.shape[0] - 1``, containing the discretized DFE for each type
+        :param errors: Array of errors of size ``intervals.shape[0] - 1``, containing the discretized DFE for each type
         :param file: File path to save plot to
         :param show: Whether to show plot
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bars.
         :param ax: Axes to plot on
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes
         """
         # number of intervals
         n_intervals = len(intervals) - 1
         n_dfes = len(values)
 
         width_total = 0.9
@@ -174,15 +177,15 @@
             x = np.arange(n_intervals) + i * width
 
             # plot discretized DFE
             bars = ax.bar(
                 x=x,
                 height=values[i],
                 width=width,
-                yerr=errors[i],
+                yerr=errors[i] if errors is not None else None,
                 error_kw=dict(
                     capsize=width * 7
                 ),
                 label=labels[i] if labels is not None else None,
                 linewidth=0,
                 hatch=Visualization.get_hatch(i, labels),
                 color=Visualization.get_color(labels[i], labels) if labels is not None else None
@@ -205,15 +208,15 @@
         ax.set_xticklabels(xlabels)
 
         # set title
         ax.set_title(title)
 
         # show legend if labels were given
         if labels is not None:
-            plt.legend(prop=dict(size=8))
+            plt.legend(**kwargs_legend)
 
         # remove x-margins
         ax.autoscale(tight=True, axis='x')
 
         return ax
 
     @staticmethod
@@ -226,14 +229,15 @@
             labels: list | np.ndarray = None,
             file: str = None,
             show: bool = True,
             title: str = 'continuous DFE',
             scale: Literal['log', 'linear'] = 'lin',
             ylim: float = 1e-2,
             scale_density: bool = False,
+            kwargs_legend: dict = dict(prop=dict(size=8)),
             **kwargs
     ) -> plt.Axes:
         """
         Plot DFEs using a line plot.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
         the x-axis, we may get a wrong intuition on how the mass is distributed,
         however. To get a better intuition, we can optionally scale the density
@@ -248,14 +252,15 @@
         :param labels: Labels for the DFEs
         :param errors: Array of errors
         :param values: Array of values
         :param file: File path to save plot to
         :param show: Whether to show plot
         :param scale_density: Whether to scale the density by the bin size
         :param ax: Axes to plot on
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes
         """
         from fastdfe.discretization import get_midpoints_and_spacing
 
         n_bins = len(bins) - 1
         n_dfes = len(values)
 
@@ -285,15 +290,15 @@
         # use log scale if specified
         if scale == 'log':
             ax.set_yscale('log')
             ax.set_ylim(bottom=ylim)
 
         # show legend if labels were given
         if labels is not None:
-            plt.legend(prop=dict(size=8))
+            plt.legend(**kwargs_legend)
 
         # remove x-margins
         ax.set_xmargin(0)
 
         ax.set_title(title)
 
         return ax
@@ -321,70 +326,103 @@
             spectra: List[Spectrum] | np.ndarray,
             labels: List[str] = [],
             file: str = None,
             show: bool = True,
             title: str = 'SFS comparison',
             use_subplots: bool = False,
             show_monomorphic: bool = False,
+            kwargs_legend: dict = dict(prop=dict(size=8)),
     ) -> plt.Axes:
         """
         Plot SFS comparison.
 
         :param use_subplots: Whether to use subplots
         :param show_monomorphic: Whether to show monomorphic counts
         :param title: Title of the plot
         :param labels: Labels for the SFSs
         :param spectra: List of spectrum objects in the same order as the labels or a 2D array
         :param file: File path to save plot to
         :param show: Whether to show plot
         :param ax: Axes to plot on
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes
         """
         # plot modelled vs observed non-neutral SFS
         ax = Visualization.plot_spectra(
             ax=ax,
             spectra=spectra,
             labels=labels,
             use_subplots=use_subplots,
             show_monomorphic=show_monomorphic,
             title=title,
             file=file,
-            show=show
+            show=show,
+            kwargs_legend=kwargs_legend
         )
 
         return ax
 
     @staticmethod
+    def name_to_label(key: str, param_names: list | np.ndarray, vals: list | np.ndarray) -> str:
+        """
+        Map parameter name to label.
+
+        :param key: Parameter name
+        :param param_names: Parameter names
+        :param vals: Parameter values
+        :return: Label
+        """
+        # define new names for some parameters
+        label_mapping = dict(
+            alpha='α',
+            eps='ε'
+        )
+
+        # map to new name
+        label = label_mapping[key] if key in label_mapping else key
+
+        # get index of parameter
+        k = np.where(np.array(param_names) == key)[0][0]
+
+        # check parameter value and add minus sign if negative
+        if vals[k] >= 0:
+            return '$' + label + '$'
+
+        return '$-' + key + '$'
+
+    @staticmethod
     @clear_show_save
     def plot_inferred_parameters(
             ax: plt.Axes,
             values: Dict[str, np.ndarray],
             labels: list | np.ndarray,
             param_names: list | np.ndarray,
             errors: Dict[str, np.ndarray | None],
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             legend: bool = True,
-            scale: Literal['lin', 'log', 'symlog'] = 'log'
+            scale: Literal['lin', 'log', 'symlog'] = 'log',
+            kwargs_legend: dict = dict(prop=dict(size=8), loc='upper right')
     ) -> plt.Axes:
         """
         Visualize the inferred parameters and their confidence intervals.
-        using a bar plot. Note that there problems with parameters that span 0.
+        using a bar plot. Note that there problems with parameters that span 0 (which is usually note the case).
 
         :param labels: Unique labels for the DFEs
         :param param_names: Labels for the parameters
         :param scale: Whether to use a linear or log scale
         :param title: Title of the plot
         :param legend: Whether to show the legend
         :param errors: Dictionary of errors with the parameter in the same order as ``labels``
         :param values: Dictionary of parameter values with the parameter in the same order as ``labels``
         :param file: File path to save plot to
         :param show: Whether to show plot
         :param ax: Axes to plot on
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes
         """
         n_types = len(values)
 
         width_total = 0.9
         width = width_total / n_types
 
@@ -392,41 +430,16 @@
         n_params = len(param_names)
 
         # iterate over types
         for i, vals, errs in zip(range(n_types), values.values(), errors.values()):
 
             x = np.arange(n_params) + i * width
 
-            def name_to_label(key: str) -> str:
-                """
-                Add parameter name to label.
-
-                :param key: Parameter name
-                :return: Label
-                """
-                # define new names for some parameters
-                label_mapping = dict(
-                    alpha='α',
-                    eps='ε'
-                )
-
-                # map to new name
-                label = label_mapping[key] if key in label_mapping else key
-
-                # get index of parameter
-                k = np.where(np.array(param_names) == key)[0][0]
-
-                # check parameter value and add minus sign if negative
-                if vals[k] >= 0:
-                    return '$' + label + '$'
-
-                return '$-' + key + '$'
-
-            # append a minus sign to negative parameters values
-            xlabels = np.array([name_to_label(key) for key in param_names])
+            # get labels for parameters
+            xlabels = np.array([Visualization.name_to_label(key, param_names, vals) for key in param_names])
 
             # flip errors for negative parameters
             if errs is not None:
                 errs = np.array([err if vals[i] >= 0 else err[::-1] for i, err in enumerate(errs.T)]).T
 
             # Plot bars.
             # Note that we plot the absolute value of the parameter
@@ -449,29 +462,88 @@
             # customize x-ticks
             x = np.arange(n_params)
             ax.set_xticks([i + (width_total - width) / 2 for i in x], x)
             ax.set_xticklabels(xlabels)
 
         # show legend if specified
         if legend:
-            plt.legend(prop=dict(size=8), loc='upper right')
+            plt.legend(**kwargs_legend)
 
         # set title
         ax.set_title(title)
 
         # change to log-scale if specified
         if scale == 'log':
             ax.set_yscale('symlog', linthresh=1e-3)
 
         # remove x-margins
         ax.autoscale(tight=True, axis='x')
 
         return ax
 
     @staticmethod
+    def plot_inferred_parameters_boxplot(
+            values: Dict[str, pd.DataFrame],
+            param_names: list | np.ndarray,
+            file: str = None,
+            show: bool = True,
+            title: str = 'parameter estimates'
+    ) -> plt.Axes:
+        """
+        Visualize the inferred parameters using a boxplot.
+
+        :param values: Type-indexed dictionary of dataframes with parameters as columns and values as rows
+        :param param_names: Parameters to plot
+        :param scale: Whether to use a linear or log scale
+        :param title: Title of the plot
+        :param legend: Whether to show the legend
+        :param file: File path to save plot to
+        :param show: Whether to show plot
+        :return: Axes
+        """
+        # create a subplot with number of parameters axes
+        fig, axs = plt.subplots(len(param_names), 1, figsize=(6, 1.4 * len(param_names)))
+
+        axs[0].set_title(title)
+
+        for i, param_name in enumerate(param_names):
+            ax = axs[i]
+
+            # Prepare a dataframe for seaborn
+            df_list = []
+            for t, df in values.items():
+                subset = df[[param_name]].copy()
+                subset['Type'] = t
+                df_list.append(subset)
+
+            df_plot = pd.concat(df_list)
+
+            # plot
+            sns.boxplot(x='Type', y=param_name, data=df_plot, ax=ax)
+
+            ax.set_ylabel(
+                Visualization.name_to_label(param_name, param_names, df_plot[param_name].abs().values),
+                rotation=0,
+                labelpad=20
+            )
+
+            ax.set_xlabel(None)
+
+            if i < len(param_names) - 1:
+                ax.set(xticklabels=[])
+                ax.tick_params(bottom=False)
+            else:
+                [l.set_rotation(90) for l in ax.get_xticklabels()]
+
+        plt.tight_layout(pad=.3)
+
+        # show and save plot
+        return Visualization.show_and_save(file, show)
+
+    @staticmethod
     def get_color(
             label: str,
             labels: List[str],
             get_group: Callable = lambda x: x.split('.')[-1]
     ) -> str:
         """
         Get color for specified label.
@@ -523,31 +595,37 @@
             labels: List[str] = [],
             log_scale: bool = False,
             use_subplots: bool = False,
             show_monomorphic: bool = False,
             title: str = None,
             n_ticks=10,
             file: str = None,
-            show: bool = True
+            show: bool = True,
+            kwargs_legend: dict = dict(prop=dict(size=8))
     ) -> plt.Axes:
         """
         Plot the given 1D spectra.
 
         :param show_monomorphic: Whether to show monomorphic site counts
         :param n_ticks: Number of x-ticks to use
         :param ax: Axes to plot on, only if ``use_subplots`` is ``False``
         :param use_subplots: Whether to use subplots
         :param title: Title of plot
         :param spectra: List of spectra to plot
         :param labels: List of labels for each spectrum
         :param log_scale: Whether to use logarithmic y-scale
         :param file: File to save plot to
         :param show: Whether to show the plot
+        :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`
         :return: Axes
         """
+        if len(spectra) == 0:
+            logger.warning('No spectra to plot.')
+            return ax
+
         if use_subplots:
             n_plots = len(spectra)
             n_rows = int(np.ceil(np.sqrt(n_plots)))
             n_cols = int(np.ceil(np.sqrt(n_plots)))
             fig = plt.figure(figsize=(6.4 * n_cols ** (1 / 3), 4.8 * n_rows ** (1 / 3)))
             axes = fig.subplots(ncols=n_cols, nrows=n_rows, squeeze=False).flatten()
 
@@ -566,17 +644,15 @@
                 # set title
                 axes[i].set_title(labels[i] if len(labels) <= i else '')
 
             # make empty plots invisible
             [ax.set_visible(False) for ax in axes[n_plots:]]
 
             # show and save plot
-            Visualization.show_and_save(file, show)
-
-            return plt.gca()
+            return Visualization.show_and_save(file, show)
 
         if ax is None:
             plt.clf()
             _, ax = plt.subplots()
 
         # determine sample size and width
         n = spectra[0].n
@@ -607,35 +683,33 @@
 
         # filter ticks
         if n > n_ticks:
             indices_ticks = indices_ticks[indices_ticks % max(int(np.ceil(n / n_ticks)), 1) == 1]
 
         ax.set_xticks([i + (width_total - width) / 2 for i in indices_ticks], indices_ticks)
 
-        ax.set_xlabel('allele count')
+        ax.set_xlabel('frequency')
 
         # remove x-margins
         ax.autoscale(tight=True, axis='x')
 
         if log_scale:
             ax.set_yscale('log')
 
         if len(labels) == 1:
             ax.set_title(labels[0])
         elif len(labels) > 1:
 
             # set title
             ax.set_title(title)
 
-            ax.legend(prop=dict(size=8))
+            ax.legend(**kwargs_legend)
 
         # show and save plot
-        Visualization.show_and_save(file, show)
-
-        return ax
+        return Visualization.show_and_save(file, show)
 
     @staticmethod
     def darken_edge_colors(bars: BarContainer):
         """
         Darken the edge color of the given bars.
 
         :param bars: Bars to darken
@@ -721,42 +795,37 @@
         return ax
 
     @staticmethod
     @clear_show_save
     def plot_likelihoods(
             likelihoods: list | np.ndarray,
             file: str, show: bool,
-            title: str,
             ax: plt.Axes,
+            title: str = 'likelihoods',
             scale: Literal['lin', 'log', 'symlog'] = 'lin'
     ) -> plt.Axes:
         """
         A scatter plot of the likelihoods specified.
 
         :param scale: Scale of y-axis
         :param likelihoods: Likelihoods to plot
         :param file: File to save plot to
         :param show: Whether to show plot
         :param title: Title of plot
         :param ax: Axes to plot on
         :return: Axes
         """
         # plot
-        ax.scatter(np.arange(len(likelihoods)), likelihoods)
+        sns.scatterplot(x=range(len(likelihoods)), y=likelihoods, ax=ax)
+
+        ax.set(ylabel='lnl')
 
         # set title
         ax.set_title(title)
 
-        # use integer ticks
-        ax.xaxis.set_major_locator(MaxNLocator(integer=True))
-
-        # set labels
-        ax.set_xlabel('iteration')
-        ax.set_ylabel('lnl')
-
         if scale == 'log':
             ax.set_yscale('symlog')
 
         return ax
 
     @staticmethod
     @clear_show_save
```

### Comparing `fastdfe-0.1.6b0/pyproject.toml` & `fastdfe-0.1.7b0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastdfe"
-version = "0.1.6-beta"
+version = "0.1.7-beta"
 description = "Fast, flexible, and hierarchical inference of the distribution of fitness effects"
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
@@ -13,32 +13,25 @@
 seaborn = "^0.12.0"
 numpy = "^1.24.0"
 pandas = "^2.0.0"
 jsonpickle = "^3.0.0"
 multiprocess = "^0.70.12"
 pyyaml = "^6.0"
 cyvcf2 = "^0.30.9"
-pyfaidx = "^0.7.1"
 tqdm = "^4.60.0"
 mpmath = "^1.3.0"
 biopython = ">=1.80,<1.82"
 requests = ">=2.28"
-requests-cache = "^1.0.0"
 scipy = "^1.10.1"
 
 [tool.poetry.group.dev.dependencies]
 urllib3 = "^1.26.0" # problems with poetry and urllib3 version 2
 sphinx-rtd-theme = "^1.2.0"
 sphinx-autodoc-typehints = "^1.23.0"
 sphinx-copybutton = "^0.5.2"
 myst-nb = "^0.17.2"
 sphinx = "5.3.0"
 pygments = "^2.15.1"
-pytest = "^7.3.1"
-pytest-xdist = "^3.3.1"
-pytest-cov = "^4.0.0"
-pytest-sugar = "^0.9.7"
-pytest-pycharm = "^0.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fastdfe-0.1.6b0/PKG-INFO` & `fastdfe-0.1.7b0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdfe
-Version: 0.1.6b0
+Version: 0.1.7b0
 Summary: Fast, flexible, and hierarchical inference of the distribution of fitness effects
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,26 +14,24 @@
 Requires-Dist: cyvcf2 (>=0.30.9,<0.31.0)
 Requires-Dist: jsonpickle (>=3.0.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: mpmath (>=1.3.0,<2.0.0)
 Requires-Dist: multiprocess (>=0.70.12,<0.71.0)
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: pyfaidx (>=0.7.1,<0.8.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28)
-Requires-Dist: requests-cache (>=1.0.0,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.0,<0.13.0)
 Requires-Dist: tqdm (>=4.60.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 [![tests](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml)
 [![codecov](https://codecov.io/gh/Sendrowski/fastDFE/branch/master/graph/badge.svg?token=0LUE8SZYBJ)](https://codecov.io/gh/Sendrowski/fastDFE)
 [![Documentation Status](https://readthedocs.org/projects/fastdfe/badge/?version=latest)](https://fastdfe.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/fastdfe.svg)](https://badge.fury.io/py/fastdfe)
 
-fastDFE is a new package designed for inferring the distribution of fitness effects (DFE) from site-frequency spectra (SFS). As it is currently in its beta phase, we are continuously working to improve and refine its features.
+fastDFE is a package for fast, flexible, and hierarchical inference of the distribution of fitness effects (DFE) from site frequency spectra (SFS). Please note that fastDFE is currently in its beta phase.
 
 Please see the [documentation](https://fastdfe.readthedocs.io/en/latest/) for all the details.
```

