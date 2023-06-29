# Comparing `tmp/fenics-smart-2.1.1.tar.gz` & `tmp/fenics-smart-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics-smart-2.1.1.tar", last modified: Fri Jun  9 15:15:17 2023, max compression
+gzip compressed data, was "fenics-smart-2.1.2.tar", last modified: Thu Jun 29 08:58:48 2023, max compression
```

## Comparing `fenics-smart-2.1.1.tar` & `fenics-smart-2.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:15:17.169085 fenics-smart-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15611 2023-06-09 15:15:17.169085 fenics-smart-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:15:17.165085 fenics-smart-2.1.1/fenics_smart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15611 2023-06-09 15:15:17.000000 fenics-smart-2.1.1/fenics_smart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 15:15:17.000000 fenics-smart-2.1.1/fenics_smart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:15:17.000000 fenics-smart-2.1.1/fenics_smart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-09 15:15:17.000000 fenics-smart-2.1.1/fenics_smart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 15:15:17.000000 fenics-smart-2.1.1/fenics_smart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:15:17.169085 fenics-smart-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:15:17.169085 fenics-smart-2.1.1/smart/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    27558 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/mesh_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    89606 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    63943 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/model_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    20870 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/smart/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:15:17.169085 fenics-smart-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/tests/test_compartment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-09 15:14:59.000000 fenics-smart-2.1.1/tests/test_species.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:48.386085 fenics-smart-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16773 2023-06-29 08:58:48.386085 fenics-smart-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:48.382085 fenics-smart-2.1.2/fenics_smart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16773 2023-06-29 08:58:48.000000 fenics-smart-2.1.2/fenics_smart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-29 08:58:48.000000 fenics-smart-2.1.2/fenics_smart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:58:48.000000 fenics-smart-2.1.2/fenics_smart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-29 08:58:48.000000 fenics-smart-2.1.2/fenics_smart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 08:58:48.000000 fenics-smart-2.1.2/fenics_smart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:58:48.386085 fenics-smart-2.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:48.382085 fenics-smart-2.1.2/smart/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27558 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/mesh_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89606 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63943 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/model_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20870 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:48.382085 fenics-smart-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/tests/test_compartment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/tests/test_species.py
```

### Comparing `fenics-smart-2.1.1/LICENSE` & `fenics-smart-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/PKG-INFO` & `fenics-smart-2.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-smart
-Version: 2.1.1
+Version: 2.1.2
 Summary: Spatial Modeling Algorithms for Reactions and Transport (SMART) is a high-performance finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes in biological cells.
 Author-email: Justin Laughlin <justinglaughlin@gmail.com>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         
@@ -63,14 +63,15 @@
 Project-URL: homepage, https://rangamanilabucsd.github.io/smart
 Project-URL: repository, https://github.com/RangamaniLabUCSD/smart
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: examples
+Provides-Extra: pyvista
 Provides-Extra: all
 License-File: LICENSE
 
 [![Test fenics_smart](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml)
 [![PyPI](https://img.shields.io/pypi/v/fenics-smart)](https://pypi.org/project/fenics-smart/)
 [![Deploy static content to Pages](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml)
 [![pre-commit](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml)
@@ -101,14 +102,31 @@
 will use version 2.0.1.
 
 In order to start a container you can use the [`docker run`](https://docs.docker.com/engine/reference/commandline/run/) command. For example the command
 ```
 docker run --rm -v $(pwd):/home/shared -w /home/shared -ti ghcr.io/rangamanilabucsd/smart:latest
 ```
 will run the latest version and share your current working directory with the container.
+The source code of smart is located at `/repo` in the docker container.
+
+#### Running the example notebooks
+To run the example notebooks, one can use `ghcr.io/rangamanilabucsd/smart-lab`
+```bash
+docker run -ti -p 8888:8888 --rm ghcr.io/rangamanilabucsd/smart-lab
+```
+to run interactively with Jupyter lab in browser
+
+#### Converting notebooks to Python files
+In the `smart` and `smart-lab` images, these files exist under `/repo/examples/**/example*.py`.
+
+If you clone the git repository or make changes to the notebooks that should be reflected in the python files, you can run
+```bash
+python3 examples/convert_notebooks_to_python.py
+```
+to convert all notebooks to python files. **NOTE** this command overwrites existing files.
 
 ### Using pip
 `fenics-smart` is also available on [pypi](https://pypi.org/project/fenics-smart/) and can be installed with
 ```
 python3 -m pip install fenics-smart
 ```
 However this requires FEniCS version 2019.2.0 or later to already be installed. Currently, FEniCS version 2019.2.0 needs to be built [from source](https://bitbucket.org/fenics-project/dolfin/src/master/) or use some of the [pre-built docker images](https://github.com/orgs/scientificcomputing/packages?repo_name=packages)
@@ -132,16 +150,20 @@
 
 The general form of the mixed-dimensional partial differential equations (PDEs) solved by SMART, along with mathematical details of the numerical implementation, are documented [here](https://rangamanilabucsd.github.io/smart/docs/math.html).
 
 Our API documentation can be accessed [here](https://rangamanilabucsd.github.io/smart/docs/api.html).
 
 ## Automated tests
 Upon pushing new code to the SMART repository, a number of tests run:
-* pre-commit tests
-* unit tests (can be found in `tests` folder): test initialization of compartment, species, and parameter objects
+* pre-commit tests.
+    - Install `pre-commit`: `python3 -m pip install pre-commit`
+    - Run pre-commit hooks: `pre-commit run --all`
+* unit tests (can be found in `tests` folder): test initialization of compartment, species, and parameter objects.
+    - Install test dependencies: `python3 -m pip install fenics-smart[test]`. Alternatively, if you have already installed SMART, you can install `pytest` and `pytest-cov` using `python3 -m pip install pytest pytest-cov`.
+    - Run tests from the root of the repository: `python3 -m pytest`
 * Examples 1-6: All 6 examples are run when building the docs. These serve as Contiuous Integration (CI) tests; within each run, there is a regression test comparing the output values from the simulation with values obtained from a previous build of SMART. Outputs from examples 2 and 3 are also compared to analytical solutions to demonstrate the accuracy of SMART simulations.
 * Example 3 with MPI: Example 3 is run using MPI to run differently sized meshes in parallel (each process is assigned a single mesh).
 
 ## Contributing guidelines
 
 Detailed contributing guidelines are given [here](https://rangamanilabucsd.github.io/smart/CONTRIBUTING.html).
```

### Comparing `fenics-smart-2.1.1/README.md` & `fenics-smart-2.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -29,14 +29,31 @@
 will use version 2.0.1.
 
 In order to start a container you can use the [`docker run`](https://docs.docker.com/engine/reference/commandline/run/) command. For example the command
 ```
 docker run --rm -v $(pwd):/home/shared -w /home/shared -ti ghcr.io/rangamanilabucsd/smart:latest
 ```
 will run the latest version and share your current working directory with the container.
+The source code of smart is located at `/repo` in the docker container.
+
+#### Running the example notebooks
+To run the example notebooks, one can use `ghcr.io/rangamanilabucsd/smart-lab`
+```bash
+docker run -ti -p 8888:8888 --rm ghcr.io/rangamanilabucsd/smart-lab
+```
+to run interactively with Jupyter lab in browser
+
+#### Converting notebooks to Python files
+In the `smart` and `smart-lab` images, these files exist under `/repo/examples/**/example*.py`.
+
+If you clone the git repository or make changes to the notebooks that should be reflected in the python files, you can run
+```bash
+python3 examples/convert_notebooks_to_python.py
+```
+to convert all notebooks to python files. **NOTE** this command overwrites existing files.
 
 ### Using pip
 `fenics-smart` is also available on [pypi](https://pypi.org/project/fenics-smart/) and can be installed with
 ```
 python3 -m pip install fenics-smart
 ```
 However this requires FEniCS version 2019.2.0 or later to already be installed. Currently, FEniCS version 2019.2.0 needs to be built [from source](https://bitbucket.org/fenics-project/dolfin/src/master/) or use some of the [pre-built docker images](https://github.com/orgs/scientificcomputing/packages?repo_name=packages)
@@ -60,16 +77,20 @@
 
 The general form of the mixed-dimensional partial differential equations (PDEs) solved by SMART, along with mathematical details of the numerical implementation, are documented [here](https://rangamanilabucsd.github.io/smart/docs/math.html).
 
 Our API documentation can be accessed [here](https://rangamanilabucsd.github.io/smart/docs/api.html).
 
 ## Automated tests
 Upon pushing new code to the SMART repository, a number of tests run:
-* pre-commit tests
-* unit tests (can be found in `tests` folder): test initialization of compartment, species, and parameter objects
+* pre-commit tests.
+    - Install `pre-commit`: `python3 -m pip install pre-commit`
+    - Run pre-commit hooks: `pre-commit run --all`
+* unit tests (can be found in `tests` folder): test initialization of compartment, species, and parameter objects.
+    - Install test dependencies: `python3 -m pip install fenics-smart[test]`. Alternatively, if you have already installed SMART, you can install `pytest` and `pytest-cov` using `python3 -m pip install pytest pytest-cov`.
+    - Run tests from the root of the repository: `python3 -m pytest`
 * Examples 1-6: All 6 examples are run when building the docs. These serve as Contiuous Integration (CI) tests; within each run, there is a regression test comparing the output values from the simulation with values obtained from a previous build of SMART. Outputs from examples 2 and 3 are also compared to analytical solutions to demonstrate the accuracy of SMART simulations.
 * Example 3 with MPI: Example 3 is run using MPI to run differently sized meshes in parallel (each process is assigned a single mesh).
 
 ## Contributing guidelines
 
 Detailed contributing guidelines are given [here](https://rangamanilabucsd.github.io/smart/CONTRIBUTING.html).
```

### Comparing `fenics-smart-2.1.1/fenics_smart.egg-info/PKG-INFO` & `fenics-smart-2.1.2/fenics_smart.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-smart
-Version: 2.1.1
+Version: 2.1.2
 Summary: Spatial Modeling Algorithms for Reactions and Transport (SMART) is a high-performance finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes in biological cells.
 Author-email: Justin Laughlin <justinglaughlin@gmail.com>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         
@@ -63,14 +63,15 @@
 Project-URL: homepage, https://rangamanilabucsd.github.io/smart
 Project-URL: repository, https://github.com/RangamaniLabUCSD/smart
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: examples
+Provides-Extra: pyvista
 Provides-Extra: all
 License-File: LICENSE
 
 [![Test fenics_smart](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml)
 [![PyPI](https://img.shields.io/pypi/v/fenics-smart)](https://pypi.org/project/fenics-smart/)
 [![Deploy static content to Pages](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml)
 [![pre-commit](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml)
@@ -101,14 +102,31 @@
 will use version 2.0.1.
 
 In order to start a container you can use the [`docker run`](https://docs.docker.com/engine/reference/commandline/run/) command. For example the command
 ```
 docker run --rm -v $(pwd):/home/shared -w /home/shared -ti ghcr.io/rangamanilabucsd/smart:latest
 ```
 will run the latest version and share your current working directory with the container.
+The source code of smart is located at `/repo` in the docker container.
+
+#### Running the example notebooks
+To run the example notebooks, one can use `ghcr.io/rangamanilabucsd/smart-lab`
+```bash
+docker run -ti -p 8888:8888 --rm ghcr.io/rangamanilabucsd/smart-lab
+```
+to run interactively with Jupyter lab in browser
+
+#### Converting notebooks to Python files
+In the `smart` and `smart-lab` images, these files exist under `/repo/examples/**/example*.py`.
+
+If you clone the git repository or make changes to the notebooks that should be reflected in the python files, you can run
+```bash
+python3 examples/convert_notebooks_to_python.py
+```
+to convert all notebooks to python files. **NOTE** this command overwrites existing files.
 
 ### Using pip
 `fenics-smart` is also available on [pypi](https://pypi.org/project/fenics-smart/) and can be installed with
 ```
 python3 -m pip install fenics-smart
 ```
 However this requires FEniCS version 2019.2.0 or later to already be installed. Currently, FEniCS version 2019.2.0 needs to be built [from source](https://bitbucket.org/fenics-project/dolfin/src/master/) or use some of the [pre-built docker images](https://github.com/orgs/scientificcomputing/packages?repo_name=packages)
@@ -132,16 +150,20 @@
 
 The general form of the mixed-dimensional partial differential equations (PDEs) solved by SMART, along with mathematical details of the numerical implementation, are documented [here](https://rangamanilabucsd.github.io/smart/docs/math.html).
 
 Our API documentation can be accessed [here](https://rangamanilabucsd.github.io/smart/docs/api.html).
 
 ## Automated tests
 Upon pushing new code to the SMART repository, a number of tests run:
-* pre-commit tests
-* unit tests (can be found in `tests` folder): test initialization of compartment, species, and parameter objects
+* pre-commit tests.
+    - Install `pre-commit`: `python3 -m pip install pre-commit`
+    - Run pre-commit hooks: `pre-commit run --all`
+* unit tests (can be found in `tests` folder): test initialization of compartment, species, and parameter objects.
+    - Install test dependencies: `python3 -m pip install fenics-smart[test]`. Alternatively, if you have already installed SMART, you can install `pytest` and `pytest-cov` using `python3 -m pip install pytest pytest-cov`.
+    - Run tests from the root of the repository: `python3 -m pytest`
 * Examples 1-6: All 6 examples are run when building the docs. These serve as Contiuous Integration (CI) tests; within each run, there is a regression test comparing the output values from the simulation with values obtained from a previous build of SMART. Outputs from examples 2 and 3 are also compared to analytical solutions to demonstrate the accuracy of SMART simulations.
 * Example 3 with MPI: Example 3 is run using MPI to run differently sized meshes in parallel (each process is assigned a single mesh).
 
 ## Contributing guidelines
 
 Detailed contributing guidelines are given [here](https://rangamanilabucsd.github.io/smart/CONTRIBUTING.html).
```

### Comparing `fenics-smart-2.1.1/pyproject.toml` & `fenics-smart-2.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "fenics-smart"
-version = "2.1.1"
+version = "2.1.2"
 description = "Spatial Modeling Algorithms for Reactions and Transport (SMART) is a high-performance finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes in biological cells."
 authors = [{name = "Justin Laughlin", email = "justinglaughlin@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "numpy>=1.16.0",
@@ -39,23 +39,29 @@
 docs = [
    "jupyter-book",
    "sphinx-autoapi"
 ]
 examples = [
     "meshio",
     "gmsh",
+    "matplotlib",
+    "jupyter",
+    "jupyterlab"
+]
+pyvista = [
     "pyvista==0.38.4",
-    "panel",
-    "matplotlib"
+    "panel"
 ]
+
 all = [
    "smart[examples]",
    "smart[test]",
    "smart[docs]",
-   "smart[dev]"
+   "smart[dev]",
+   "smart[pyvista]"
 ]
 
 
 [tool.pytest.ini_options]
 addopts = [
    "--cov=smart",
    "--cov-report=html",
```

### Comparing `fenics-smart-2.1.1/smart/common.py` & `fenics-smart-2.1.2/smart/common.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/smart/config.py` & `fenics-smart-2.1.2/smart/config.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/smart/deprecation.py` & `fenics-smart-2.1.2/smart/deprecation.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/smart/mesh.py` & `fenics-smart-2.1.2/smart/mesh.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/smart/mesh_tools.py` & `fenics-smart-2.1.2/smart/mesh_tools.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/smart/model.py` & `fenics-smart-2.1.2/smart/model.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/smart/model_assembly.py` & `fenics-smart-2.1.2/smart/model_assembly.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/smart/solvers.py` & `fenics-smart-2.1.2/smart/solvers.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/smart/units.py` & `fenics-smart-2.1.2/smart/units.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/smart/utils.py` & `fenics-smart-2.1.2/smart/utils.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/smart/visualization.py` & `fenics-smart-2.1.2/smart/visualization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 Utility functions for visualizing SMART meshes using pyvista.
 """
 import dolfin
-import pyvista
 from ufl import vertex
 from typing import Tuple
 import numpy.typing as npt
 import numpy as np
+import functools
 import pathlib
 from typing import Optional
-
-# pyvista.global_theme.trame.server_proxy_enabled = True
+import warnings
 
 __all__ = ["create_vtk_structures", "plot"]
 
 _vtk_perm = {
     dolfin.interval: {i: np.arange(i) for i in range(2, 10)},
     vertex: {1: 1},
     dolfin.triangle: {
@@ -27,14 +26,27 @@
         1: [0, 1, 2, 3],
         2: [0, 1, 2, 3, 9, 6, 8, 7, 5, 4],
         3: [0, 1, 2, 3, 14, 15, 8, 9, 13, 12, 10, 11, 6, 7, 4, 5, 18, 16, 17, 19],
     },
 }
 
 
+def require_pyvista(func):
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        try:
+            import pyvista as _  # noqa: F401
+
+            return func(*args, **kwargs)
+        except ImportError:
+            warnings.warn("Pyvista is not installed, skipping function", ImportWarning)
+
+    return wrapper
+
+
 def create_vtk_structures(
     Vh: dolfin.FunctionSpace,
 ) -> Tuple[npt.NDArray[np.int32], npt.NDArray[np.int32], npt.NDArray[np.float64]]:
     """Given a (discontinuous) Lagrange space, create pyvista compatible structures based on the
     dof coordinates
 
     Args:
@@ -90,14 +102,15 @@
         perm = _vtk_perm[d_cell][degree]
     except KeyError:
         raise RuntimeError(f"Unsupported plotting of space {family} of {degree=} on {d_cell}")
     topology[:, 1:] = topology[:, 1:][:, perm]
     return topology, cell_types, x
 
 
+@require_pyvista
 def plot(
     uh: dolfin.Function,
     filename: Optional[pathlib.Path] = None,
     show_edges: bool = True,
     glyph_factor: float = 1,
     off_screen: bool = True,
     view_xy: bool = False,
@@ -123,14 +136,15 @@
     u_vec = uh.vector().get_local(np.arange(num_vertices_local))
     if bs > 1:
         u_out = np.zeros((len(u_vec) // bs, 3), dtype=np.float64)
         u_out[:, :bs] = u_vec.reshape(len(u_vec) // bs, bs)
     else:
         u_out = u_vec
     topology, cell_types, x = create_vtk_structures(Vh)
+    import pyvista
 
     grid = pyvista.UnstructuredGrid(topology, cell_types, x)
     grid[uh.name()] = u_out
 
     if bs > 1:
         grid.set_active_scalars(None)
 
@@ -167,14 +181,15 @@
     print(filename)
     if filename is None:
         plotter.show()
     else:
         plotter.screenshot(filename)
 
 
+@require_pyvista
 def plot_dolfin_mesh(
     msh: dolfin.mesh,
     mf_cell: dolfin.MeshFunction,
     mf_facet: dolfin.MeshFunction = None,
     outer_marker: int = 10,
     filename: Optional[pathlib.Path] = None,
     show_edges: bool = True,
@@ -198,14 +213,17 @@
         show_edges: Show mesh edges if ``True``
         off_screen: If ``True`` generate plots with virtual frame buffer using ``xvfb``.
         view_xy: If ``True``, view xy plane
     """
     Vh = dolfin.FunctionSpace(msh, "P", 1)
     u_out = mf_cell.array()
     topology, cell_types, x = create_vtk_structures(Vh)
+
+    import pyvista
+
     grid = pyvista.UnstructuredGrid(topology, cell_types, x)
     grid["mf"] = u_out
 
     facets_loaded = False
     if mf_facet is not None:
         msh_facet = dolfin.BoundaryMesh(msh, "exterior")
         Vh_facet = dolfin.FunctionSpace(msh_facet, "P", 1)
@@ -245,12 +263,11 @@
             plotter.add_mesh(grid, show_edges=show_edges)
             if facets_loaded:
                 plotter.add_mesh(grid_facet, show_edges=show_edges)
 
     if msh.geometric_dimension() == 2 or view_xy:
         plotter.view_xy()
 
-    print(filename)
     if filename is None:
         plotter.show()
     else:
         plotter.screenshot(filename)
```

### Comparing `fenics-smart-2.1.1/tests/test_compartment.py` & `fenics-smart-2.1.2/tests/test_compartment.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/tests/test_parameter.py` & `fenics-smart-2.1.2/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.1/tests/test_species.py` & `fenics-smart-2.1.2/tests/test_species.py`

 * *Files identical despite different names*

