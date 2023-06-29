# Comparing `tmp/joblib-1.3.0.tar.gz` & `tmp/joblib-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joblib-1.3.0.tar", last modified: Wed Jun 28 13:22:14 2023, max compression
+gzip compressed data, was "joblib-1.3.1.tar", last modified: Thu Jun 29 15:14:30 2023, max compression
```

## Comparing `joblib-1.3.0.tar` & `joblib-1.3.1.tar`

### file list

```diff
@@ -1,477 +1,477 @@
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.660021 joblib-1.3.0/
--rw-r--r--   0 tom       (1000) users      (984)       99 2023-06-28 08:33:35.000000 joblib-1.3.0/.readthedocs-requirements.txt
--rw-r--r--   0 tom       (1000) users      (984)     1527 2023-04-30 13:25:43.000000 joblib-1.3.0/LICENSE.txt
--rw-r--r--   0 tom       (1000) users      (984)      128 2023-03-26 21:55:29.000000 joblib-1.3.0/MANIFEST.in
--rw-r--r--   0 tom       (1000) users      (984)     5361 2023-06-28 13:22:14.660021 joblib-1.3.0/PKG-INFO
--rw-r--r--   0 tom       (1000) users      (984)     4210 2023-04-30 13:25:43.000000 joblib-1.3.0/README.rst
--rw-r--r--   0 tom       (1000) users      (984)     2885 2023-05-19 20:19:06.000000 joblib-1.3.0/conftest.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.640021 joblib-1.3.0/doc/
--rw-r--r--   0 tom       (1000) users      (984)    36681 2023-06-27 22:12:43.000000 joblib-1.3.0/doc/CHANGES.rst
--rw-r--r--   0 tom       (1000) users      (984)      535 2023-06-28 08:33:35.000000 joblib-1.3.0/doc/Makefile
--rw-r--r--   0 tom       (1000) users      (984)     4210 2023-06-27 22:12:43.000000 joblib-1.3.0/doc/README.rst
--rw-r--r--   0 tom       (1000) users      (984)       95 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/__init__.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.636687 joblib-1.3.0/doc/_build/
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.640021 joblib-1.3.0/doc/_build/html/
--rw-r--r--   0 tom       (1000) users      (984)      230 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/.buildinfo
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/.doctrees/
--rw-r--r--   0 tom       (1000) users      (984)   191208 2023-06-27 22:12:43.000000 joblib-1.3.0/doc/_build/html/.doctrees/CHANGES.doctree
--rw-r--r--   0 tom       (1000) users      (984)    21534 2023-06-27 22:12:43.000000 joblib-1.3.0/doc/_build/html/.doctrees/README.doctree
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/
--rw-r--r--   0 tom       (1000) users      (984)    40483 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/compressors_comparison.doctree
--rw-r--r--   0 tom       (1000) users      (984)    19900 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/index.doctree
--rw-r--r--   0 tom       (1000) users      (984)    26656 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/memory_basic_usage.doctree
--rw-r--r--   0 tom       (1000) users      (984)    26737 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/nested_parallel_memory.doctree
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel/
--rw-r--r--   0 tom       (1000) users      (984)    16962 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel/distributed_backend_simple.doctree
--rw-r--r--   0 tom       (1000) users      (984)     5867 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel/index.doctree
--rw-r--r--   0 tom       (1000) users      (984)     5298 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel/sg_execution_times.doctree
--rw-r--r--   0 tom       (1000) users      (984)    27872 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel_generator.doctree
--rw-r--r--   0 tom       (1000) users      (984)    35065 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel_memmap.doctree
--rw-r--r--   0 tom       (1000) users      (984)    27230 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel_random_state.doctree
--rw-r--r--   0 tom       (1000) users      (984)    32097 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/serialization_and_wrappers.doctree
--rw-r--r--   0 tom       (1000) users      (984)    12300 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/sg_execution_times.doctree
--rw-r--r--   0 tom       (1000) users      (984)   214237 2023-06-27 22:12:43.000000 joblib-1.3.0/doc/_build/html/.doctrees/developing.doctree
--rw-r--r--   0 tom       (1000) users      (984)  6257818 2023-06-27 22:12:43.000000 joblib-1.3.0/doc/_build/html/.doctrees/environment.pickle
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/.doctrees/generated/
--rw-r--r--   0 tom       (1000) users      (984)    50793 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.Memory.doctree
--rw-r--r--   0 tom       (1000) users      (984)    79449 2023-06-27 22:12:43.000000 joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.Parallel.doctree
--rw-r--r--   0 tom       (1000) users      (984)    21941 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.dump.doctree
--rw-r--r--   0 tom       (1000) users      (984)     7760 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.hash.doctree
--rw-r--r--   0 tom       (1000) users      (984)    17300 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.load.doctree
--rw-r--r--   0 tom       (1000) users      (984)    47094 2023-06-27 22:12:43.000000 joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.parallel_config.doctree
--rw-r--r--   0 tom       (1000) users      (984)     7466 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.register_compressor.doctree
--rw-r--r--   0 tom       (1000) users      (984)    32300 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/index.doctree
--rw-r--r--   0 tom       (1000) users      (984)     9749 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/installing.doctree
--rw-r--r--   0 tom       (1000) users      (984)   155458 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/memory.doctree
--rw-r--r--   0 tom       (1000) users      (984)   209728 2023-06-27 22:12:43.000000 joblib-1.3.0/doc/_build/html/.doctrees/parallel.doctree
--rw-r--r--   0 tom       (1000) users      (984)    24195 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/parallel_numpy.doctree
--rw-r--r--   0 tom       (1000) users      (984)    32670 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/persistence.doctree
--rw-r--r--   0 tom       (1000) users      (984)     9998 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/.doctrees/why.doctree
--rw-r--r--   0 tom       (1000) users      (984)    67500 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/CHANGES.html
--rw-r--r--   0 tom       (1000) users      (984)    12659 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/README.html
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.636687 joblib-1.3.0/doc/_build/html/_downloads/
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/
--rw-r--r--   0 tom       (1000) users      (984)    43714 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/
--rw-r--r--   0 tom       (1000) users      (984)     5685 2023-06-26 07:51:11.000000 joblib-1.3.0/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/serialization_and_wrappers.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/
--rw-r--r--   0 tom       (1000) users      (984)     6043 2023-06-26 07:51:15.000000 joblib-1.3.0/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/parallel_generator.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/
--rw-r--r--   0 tom       (1000) users      (984)     9044 2023-06-26 07:51:36.000000 joblib-1.3.0/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/compressors_comparison.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/
--rw-r--r--   0 tom       (1000) users      (984)     7302 2023-06-26 07:50:56.000000 joblib-1.3.0/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/nested_parallel_memory.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/
--rw-r--r--   0 tom       (1000) users      (984)    62629 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/
--rw-r--r--   0 tom       (1000) users      (984)     7872 2023-06-26 07:51:12.000000 joblib-1.3.0/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/serialization_and_wrappers.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/
--rw-r--r--   0 tom       (1000) users      (984)     7282 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/parallel_random_state.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/
--rw-r--r--   0 tom       (1000) users      (984)     6406 2023-06-26 07:51:11.000000 joblib-1.3.0/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/memory_basic_usage.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/
--rw-r--r--   0 tom       (1000) users      (984)     4695 2023-06-26 07:50:56.000000 joblib-1.3.0/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/memory_basic_usage.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/
--rw-r--r--   0 tom       (1000) users      (984)     1984 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/distributed_backend_simple.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/
--rw-r--r--   0 tom       (1000) users      (984)     8458 2023-06-26 07:51:15.000000 joblib-1.3.0/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/parallel_memmap.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/
--rw-r--r--   0 tom       (1000) users      (984)     5092 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/nested_parallel_memory.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/
--rw-r--r--   0 tom       (1000) users      (984)     7821 2023-06-26 07:51:36.000000 joblib-1.3.0/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/parallel_generator.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/
--rw-r--r--   0 tom       (1000) users      (984)     4551 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/parallel_random_state.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/
--rw-r--r--   0 tom       (1000) users      (984)    13465 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/compressors_comparison.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/
--rw-r--r--   0 tom       (1000) users      (984)     5588 2023-06-26 07:51:12.000000 joblib-1.3.0/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/parallel_memmap.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.643354 joblib-1.3.0/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/
--rw-r--r--   0 tom       (1000) users      (984)     2943 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/distributed_backend_simple.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.646687 joblib-1.3.0/doc/_build/html/_images/
--rw-r--r--   0 tom       (1000) users      (984)    14175 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/_images/sphx_glr_compressors_comparison_001.png
--rw-r--r--   0 tom       (1000) users      (984)     7869 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/_images/sphx_glr_compressors_comparison_002.png
--rw-r--r--   0 tom       (1000) users      (984)    13471 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/_build/html/_images/sphx_glr_compressors_comparison_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/_images/sphx_glr_distributed_backend_simple_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:11.000000 joblib-1.3.0/doc/_build/html/_images/sphx_glr_memory_basic_usage_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:50:56.000000 joblib-1.3.0/doc/_build/html/_images/sphx_glr_nested_parallel_memory_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    22465 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/_images/sphx_glr_parallel_generator_001.png
--rw-r--r--   0 tom       (1000) users      (984)    14949 2023-06-26 07:51:36.000000 joblib-1.3.0/doc/_build/html/_images/sphx_glr_parallel_generator_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:15.000000 joblib-1.3.0/doc/_build/html/_images/sphx_glr_parallel_memmap_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/_build/html/_images/sphx_glr_parallel_random_state_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:12.000000 joblib-1.3.0/doc/_build/html/_images/sphx_glr_serialization_and_wrappers_thumb.png
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.646687 joblib-1.3.0/doc/_build/html/_sources/
--rw-r--r--   0 tom       (1000) users      (984)    36681 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/_build/html/_sources/CHANGES.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     4210 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/_build/html/_sources/README.rst.txt
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.646687 joblib-1.3.0/doc/_build/html/_sources/auto_examples/
--rw-r--r--   0 tom       (1000) users      (984)    13174 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/compressors_comparison.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     4940 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/index.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     7558 2023-06-26 07:51:11.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/memory_basic_usage.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     7412 2023-06-26 07:50:56.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/nested_parallel_memory.rst.txt
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.646687 joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel/
--rw-r--r--   0 tom       (1000) users      (984)     4449 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel/distributed_backend_simple.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      789 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel/index.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      569 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel/sg_execution_times.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     8603 2023-06-26 07:51:36.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel_generator.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)    10854 2023-06-26 07:51:15.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel_memmap.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     8234 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel_random_state.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     9859 2023-06-26 07:51:12.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/serialization_and_wrappers.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     1976 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/_build/html/_sources/auto_examples/sg_execution_times.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)       97 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_build/html/_sources/developing.rst.txt
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.646687 joblib-1.3.0/doc/_build/html/_sources/generated/
--rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/_build/html/_sources/generated/joblib.Memory.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      197 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/_build/html/_sources/generated/joblib.Parallel.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/_build/html/_sources/generated/joblib.dump.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/_build/html/_sources/generated/joblib.hash.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/_build/html/_sources/generated/joblib.load.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      234 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/_build/html/_sources/generated/joblib.parallel_config.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      247 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/_build/html/_sources/generated/joblib.register_compressor.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     1060 2023-06-23 14:57:25.000000 joblib-1.3.0/doc/_build/html/_sources/index.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     1841 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_build/html/_sources/installing.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)    17016 2023-06-23 14:57:25.000000 joblib-1.3.0/doc/_build/html/_sources/memory.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)    18614 2023-06-27 22:12:21.000000 joblib-1.3.0/doc/_build/html/_sources/parallel.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     6336 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_build/html/_sources/parallel_numpy.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     7247 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_build/html/_sources/persistence.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     1680 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_build/html/_sources/why.rst.txt
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.646687 joblib-1.3.0/doc/_build/html/_static/
--rw-r--r--   0 tom       (1000) users      (984)    11230 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/_static/alabaster.css
--rw-r--r--   0 tom       (1000) users      (984)    14813 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/_static/basic.css
--rw-r--r--   0 tom       (1000) users      (984)     3380 2023-04-18 19:56:48.000000 joblib-1.3.0/doc/_build/html/_static/binder_badge_logo.svg
--rw-r--r--   0 tom       (1000) users      (984)    21404 2023-04-18 19:56:48.000000 joblib-1.3.0/doc/_build/html/_static/broken_example.png
--rw-r--r--   0 tom       (1000) users      (984)     1018 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_build/html/_static/custom.css
--rw-r--r--   0 tom       (1000) users      (984)     4472 2023-06-26 07:49:58.000000 joblib-1.3.0/doc/_build/html/_static/doctools.js
--rw-r--r--   0 tom       (1000) users      (984)      425 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/_static/documentation_options.js
--rw-r--r--   0 tom       (1000) users      (984)   268286 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_build/html/_static/favicon.ico
--rw-r--r--   0 tom       (1000) users      (984)      286 2023-06-26 07:49:58.000000 joblib-1.3.0/doc/_build/html/_static/file.png
--rw-r--r--   0 tom       (1000) users      (984)    15594 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_build/html/_static/joblib_logo.svg
--rw-r--r--   0 tom       (1000) users      (984)    27703 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_build/html/_static/joblib_logo_examples.png
--rw-r--r--   0 tom       (1000) users      (984)     6936 2023-04-18 19:56:48.000000 joblib-1.3.0/doc/_build/html/_static/jupyterlite_badge_logo.svg
--rw-r--r--   0 tom       (1000) users      (984)     4758 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/_static/language_data.js
--rw-r--r--   0 tom       (1000) users      (984)       90 2023-06-26 07:49:58.000000 joblib-1.3.0/doc/_build/html/_static/minus.png
--rw-r--r--   0 tom       (1000) users      (984)     4315 2023-04-18 19:56:48.000000 joblib-1.3.0/doc/_build/html/_static/no_image.png
--rw-r--r--   0 tom       (1000) users      (984)       90 2023-06-26 07:49:58.000000 joblib-1.3.0/doc/_build/html/_static/plus.png
--rw-r--r--   0 tom       (1000) users      (984)     4846 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/_static/pygments.css
--rw-r--r--   0 tom       (1000) users      (984)    18215 2023-06-26 07:49:58.000000 joblib-1.3.0/doc/_build/html/_static/searchtools.js
--rw-r--r--   0 tom       (1000) users      (984)      167 2023-04-18 19:56:48.000000 joblib-1.3.0/doc/_build/html/_static/sg_gallery-binder.css
--rw-r--r--   0 tom       (1000) users      (984)     1137 2023-04-18 19:56:48.000000 joblib-1.3.0/doc/_build/html/_static/sg_gallery-dataframe.css
--rw-r--r--   0 tom       (1000) users      (984)     4330 2023-04-18 19:56:48.000000 joblib-1.3.0/doc/_build/html/_static/sg_gallery-rendered-html.css
--rw-r--r--   0 tom       (1000) users      (984)     9530 2023-04-18 19:56:48.000000 joblib-1.3.0/doc/_build/html/_static/sg_gallery.css
--rw-r--r--   0 tom       (1000) users      (984)     4712 2023-06-26 07:49:58.000000 joblib-1.3.0/doc/_build/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.650021 joblib-1.3.0/doc/_build/html/auto_examples/
--rw-r--r--   0 tom       (1000) users      (984)    60961 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/compressors_comparison.html
--rw-r--r--   0 tom       (1000) users      (984)    10642 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/index.html
--rw-r--r--   0 tom       (1000) users      (984)    38082 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/memory_basic_usage.html
--rw-r--r--   0 tom       (1000) users      (984)    35272 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/nested_parallel_memory.html
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.650021 joblib-1.3.0/doc/_build/html/auto_examples/parallel/
--rw-r--r--   0 tom       (1000) users      (984)    14139 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/parallel/distributed_backend_simple.html
--rw-r--r--   0 tom       (1000) users      (984)     5718 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/parallel/index.html
--rw-r--r--   0 tom       (1000) users      (984)     5134 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/parallel/sg_execution_times.html
--rw-r--r--   0 tom       (1000) users      (984)    29778 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/parallel_generator.html
--rw-r--r--   0 tom       (1000) users      (984)    44012 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/parallel_memmap.html
--rw-r--r--   0 tom       (1000) users      (984)    36234 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/parallel_random_state.html
--rw-r--r--   0 tom       (1000) users      (984)    32607 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/serialization_and_wrappers.html
--rw-r--r--   0 tom       (1000) users      (984)     7236 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/auto_examples/sg_execution_times.html
--rw-r--r--   0 tom       (1000) users      (984)    77562 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/developing.html
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.650021 joblib-1.3.0/doc/_build/html/generated/
--rw-r--r--   0 tom       (1000) users      (984)    19179 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/generated/joblib.Memory.html
--rw-r--r--   0 tom       (1000) users      (984)    33735 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/generated/joblib.Parallel.html
--rw-r--r--   0 tom       (1000) users      (984)     9992 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/generated/joblib.dump.html
--rw-r--r--   0 tom       (1000) users      (984)     6212 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/generated/joblib.hash.html
--rw-r--r--   0 tom       (1000) users      (984)     8920 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/generated/joblib.load.html
--rw-r--r--   0 tom       (1000) users      (984)    19398 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/generated/joblib.parallel_config.html
--rw-r--r--   0 tom       (1000) users      (984)     6025 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/generated/joblib.register_compressor.html
--rw-r--r--   0 tom       (1000) users      (984)     9965 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/genindex.html
--rw-r--r--   0 tom       (1000) users      (984)    22003 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/index.html
--rw-r--r--   0 tom       (1000) users      (984)     8933 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/installing.html
--rw-r--r--   0 tom       (1000) users      (984)    75468 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/memory.html
--rw-r--r--   0 tom       (1000) users      (984)     1766 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/objects.inv
--rw-r--r--   0 tom       (1000) users      (984)   108722 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/parallel.html
--rw-r--r--   0 tom       (1000) users      (984)    21134 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/parallel_numpy.html
--rw-r--r--   0 tom       (1000) users      (984)    30312 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/persistence.html
--rw-r--r--   0 tom       (1000) users      (984)     4509 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/py-modindex.html
--rw-r--r--   0 tom       (1000) users      (984)     4748 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/search.html
--rw-r--r--   0 tom       (1000) users      (984)    76600 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/searchindex.js
--rw-r--r--   0 tom       (1000) users      (984)     7402 2023-06-27 22:12:44.000000 joblib-1.3.0/doc/_build/html/why.html
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.650021 joblib-1.3.0/doc/_static/
--rw-r--r--   0 tom       (1000) users      (984)     1018 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_static/custom.css
--rw-r--r--   0 tom       (1000) users      (984)   268286 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_static/favicon.ico
--rw-r--r--   0 tom       (1000) users      (984)    15594 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_static/joblib_logo.svg
--rw-r--r--   0 tom       (1000) users      (984)    27703 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_static/joblib_logo_examples.png
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.650021 joblib-1.3.0/doc/_templates/
--rw-r--r--   0 tom       (1000) users      (984)      208 2023-06-28 08:33:35.000000 joblib-1.3.0/doc/_templates/class.rst
--rw-r--r--   0 tom       (1000) users      (984)      226 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_templates/function.rst
--rw-r--r--   0 tom       (1000) users      (984)      479 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/_templates/layout.html
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.650021 joblib-1.3.0/doc/auto_examples/
--rw-r--r--   0 tom       (1000) users      (984)    62629 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/auto_examples/auto_examples_jupyter.zip
--rw-r--r--   0 tom       (1000) users      (984)    43714 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/auto_examples/auto_examples_python.zip
--rw-r--r--   0 tom       (1000) users      (984)    13465 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/auto_examples/compressors_comparison.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     9044 2023-06-26 07:51:36.000000 joblib-1.3.0/doc/auto_examples/compressors_comparison.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/auto_examples/compressors_comparison.py.md5
--rw-r--r--   0 tom       (1000) users      (984)    13174 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/auto_examples/compressors_comparison.rst
--rw-r--r--   0 tom       (1000) users      (984)     3437 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/auto_examples/compressors_comparison_codeobj.pickle
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.650021 joblib-1.3.0/doc/auto_examples/images/
--rw-r--r--   0 tom       (1000) users      (984)    14175 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/auto_examples/images/sphx_glr_compressors_comparison_001.png
--rw-r--r--   0 tom       (1000) users      (984)     7869 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/auto_examples/images/sphx_glr_compressors_comparison_002.png
--rw-r--r--   0 tom       (1000) users      (984)    22465 2023-06-26 07:51:36.000000 joblib-1.3.0/doc/auto_examples/images/sphx_glr_parallel_generator_001.png
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.650021 joblib-1.3.0/doc/auto_examples/images/thumb/
--rw-r--r--   0 tom       (1000) users      (984)    13471 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_compressors_comparison_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:11.000000 joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_memory_basic_usage_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:50:56.000000 joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_nested_parallel_memory_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    14949 2023-06-26 07:51:36.000000 joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_parallel_generator_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:15.000000 joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_parallel_memmap_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_parallel_random_state_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:12.000000 joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_serialization_and_wrappers_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)     4940 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/auto_examples/index.rst
--rw-r--r--   0 tom       (1000) users      (984)     6406 2023-06-26 07:51:11.000000 joblib-1.3.0/doc/auto_examples/memory_basic_usage.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     4695 2023-06-26 07:50:56.000000 joblib-1.3.0/doc/auto_examples/memory_basic_usage.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:11.000000 joblib-1.3.0/doc/auto_examples/memory_basic_usage.py.md5
--rw-r--r--   0 tom       (1000) users      (984)     7558 2023-06-26 07:51:11.000000 joblib-1.3.0/doc/auto_examples/memory_basic_usage.rst
--rw-r--r--   0 tom       (1000) users      (984)     2516 2023-06-26 07:51:11.000000 joblib-1.3.0/doc/auto_examples/memory_basic_usage_codeobj.pickle
--rw-r--r--   0 tom       (1000) users      (984)     7302 2023-06-26 07:50:56.000000 joblib-1.3.0/doc/auto_examples/nested_parallel_memory.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     5092 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/auto_examples/nested_parallel_memory.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:50:56.000000 joblib-1.3.0/doc/auto_examples/nested_parallel_memory.py.md5
--rw-r--r--   0 tom       (1000) users      (984)     7412 2023-06-26 07:50:56.000000 joblib-1.3.0/doc/auto_examples/nested_parallel_memory.rst
--rw-r--r--   0 tom       (1000) users      (984)     2729 2023-06-26 07:50:56.000000 joblib-1.3.0/doc/auto_examples/nested_parallel_memory_codeobj.pickle
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.653354 joblib-1.3.0/doc/auto_examples/parallel/
--rw-r--r--   0 tom       (1000) users      (984)     2943 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/auto_examples/parallel/distributed_backend_simple.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     1984 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/auto_examples/parallel/distributed_backend_simple.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/auto_examples/parallel/distributed_backend_simple.py.md5
--rw-r--r--   0 tom       (1000) users      (984)     4449 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/auto_examples/parallel/distributed_backend_simple.rst
--rw-r--r--   0 tom       (1000) users      (984)     2457 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/auto_examples/parallel/distributed_backend_simple_codeobj.pickle
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.636687 joblib-1.3.0/doc/auto_examples/parallel/images/
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.653354 joblib-1.3.0/doc/auto_examples/parallel/images/thumb/
--rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/auto_examples/parallel/images/thumb/sphx_glr_distributed_backend_simple_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)      789 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/auto_examples/parallel/index.rst
--rw-r--r--   0 tom       (1000) users      (984)      569 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/auto_examples/parallel/sg_execution_times.rst
--rw-r--r--   0 tom       (1000) users      (984)     7821 2023-06-26 07:51:36.000000 joblib-1.3.0/doc/auto_examples/parallel_generator.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     6043 2023-06-26 07:51:15.000000 joblib-1.3.0/doc/auto_examples/parallel_generator.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:36.000000 joblib-1.3.0/doc/auto_examples/parallel_generator.py.md5
--rw-r--r--   0 tom       (1000) users      (984)     8603 2023-06-26 07:51:36.000000 joblib-1.3.0/doc/auto_examples/parallel_generator.rst
--rw-r--r--   0 tom       (1000) users      (984)     2899 2023-06-26 07:51:36.000000 joblib-1.3.0/doc/auto_examples/parallel_generator_codeobj.pickle
--rw-r--r--   0 tom       (1000) users      (984)     8458 2023-06-26 07:51:15.000000 joblib-1.3.0/doc/auto_examples/parallel_memmap.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     5588 2023-06-26 07:51:12.000000 joblib-1.3.0/doc/auto_examples/parallel_memmap.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:15.000000 joblib-1.3.0/doc/auto_examples/parallel_memmap.py.md5
--rw-r--r--   0 tom       (1000) users      (984)    10854 2023-06-26 07:51:15.000000 joblib-1.3.0/doc/auto_examples/parallel_memmap.rst
--rw-r--r--   0 tom       (1000) users      (984)     2644 2023-06-26 07:51:15.000000 joblib-1.3.0/doc/auto_examples/parallel_memmap_codeobj.pickle
--rw-r--r--   0 tom       (1000) users      (984)     7282 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/auto_examples/parallel_random_state.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     4551 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/auto_examples/parallel_random_state.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/auto_examples/parallel_random_state.py.md5
--rw-r--r--   0 tom       (1000) users      (984)     8234 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/auto_examples/parallel_random_state.rst
--rw-r--r--   0 tom       (1000) users      (984)     1872 2023-06-26 07:50:44.000000 joblib-1.3.0/doc/auto_examples/parallel_random_state_codeobj.pickle
--rw-r--r--   0 tom       (1000) users      (984)      236 2023-06-26 07:51:47.000000 joblib-1.3.0/doc/auto_examples/searchindex.bak
--rw-r--r--   0 tom       (1000) users      (984)    99137 2023-06-26 07:51:47.000000 joblib-1.3.0/doc/auto_examples/searchindex.dat
--rw-r--r--   0 tom       (1000) users      (984)      236 2023-06-26 07:51:47.000000 joblib-1.3.0/doc/auto_examples/searchindex.dir
--rw-r--r--   0 tom       (1000) users      (984)     7872 2023-06-26 07:51:12.000000 joblib-1.3.0/doc/auto_examples/serialization_and_wrappers.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     5685 2023-06-26 07:51:11.000000 joblib-1.3.0/doc/auto_examples/serialization_and_wrappers.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:12.000000 joblib-1.3.0/doc/auto_examples/serialization_and_wrappers.py.md5
--rw-r--r--   0 tom       (1000) users      (984)     9859 2023-06-26 07:51:12.000000 joblib-1.3.0/doc/auto_examples/serialization_and_wrappers.rst
--rw-r--r--   0 tom       (1000) users      (984)     1572 2023-06-26 07:51:12.000000 joblib-1.3.0/doc/auto_examples/serialization_and_wrappers_codeobj.pickle
--rw-r--r--   0 tom       (1000) users      (984)     1976 2023-06-26 07:51:45.000000 joblib-1.3.0/doc/auto_examples/sg_execution_times.rst
--rw-r--r--   0 tom       (1000) users      (984)     7882 2023-06-28 08:33:35.000000 joblib-1.3.0/doc/conf.py
--rw-r--r--   0 tom       (1000) users      (984)      624 2023-05-19 20:19:06.000000 joblib-1.3.0/doc/conftest.py
--rw-r--r--   0 tom       (1000) users      (984)       97 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/developing.rst
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.653354 joblib-1.3.0/doc/generated/
--rw-r--r--   0 tom       (1000) users      (984)     1233 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Logger.cache.examples
--rw-r--r--   0 tom       (1000) users      (984)     1233 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Logger.clear.examples
--rw-r--r--   0 tom       (1000) users      (984)     3855 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Logger.examples
--rw-r--r--   0 tom       (1000) users      (984)     1235 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.MemorizedFunc.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Memory.__init__.examples
--rw-r--r--   0 tom       (1000) users      (984)     1233 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Memory.cache.examples
--rw-r--r--   0 tom       (1000) users      (984)     1233 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Memory.clear.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Memory.eval.examples
--rw-r--r--   0 tom       (1000) users      (984)     1221 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Memory.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Memory.format.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Memory.reduce_size.examples
--rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/generated/joblib.Memory.rst
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Parallel.dispatch_next.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Parallel.dispatch_one_batch.examples
--rw-r--r--   0 tom       (1000) users      (984)     3366 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Parallel.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Parallel.format.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.Parallel.print_progress.examples
--rw-r--r--   0 tom       (1000) users      (984)      197 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/generated/joblib.Parallel.rst
--rw-r--r--   0 tom       (1000) users      (984)     3364 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.delayed.examples
--rw-r--r--   0 tom       (1000) users      (984)     1210 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.dump.examples
--rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/generated/joblib.dump.rst
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.expires_after.examples
--rw-r--r--   0 tom       (1000) users      (984)      763 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.externals.loky.set_loky_pickler.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.hash.examples
--rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/generated/joblib.hash.rst
--rw-r--r--   0 tom       (1000) users      (984)     1210 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.load.examples
--rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/generated/joblib.load.rst
--rw-r--r--   0 tom       (1000) users      (984)     1247 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.logger.Logger.cache.examples
--rw-r--r--   0 tom       (1000) users      (984)     1247 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.logger.Logger.clear.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.memory.MemorizedFunc.__init__.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.memory.MemorizedFunc.call.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.memory.MemorizedFunc.check_call_in_cache.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.memory.MemorizedFunc.clear.examples
--rw-r--r--   0 tom       (1000) users      (984)     1249 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.memory.MemorizedFunc.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.parallel.AutoBatchingMixin.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.parallel.ParallelBackendBase.examples
--rw-r--r--   0 tom       (1000) users      (984)     1295 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.parallel_config.examples
--rw-r--r--   0 tom       (1000) users      (984)      234 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/generated/joblib.parallel_config.rst
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.register_compressor.examples
--rw-r--r--   0 tom       (1000) users      (984)      247 2023-06-26 07:50:43.000000 joblib-1.3.0/doc/generated/joblib.register_compressor.rst
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.register_parallel_backend.examples
--rw-r--r--   0 tom       (1000) users      (984)      753 2023-06-26 07:51:46.000000 joblib-1.3.0/doc/generated/joblib.wrap_non_picklable_objects.examples
--rw-r--r--   0 tom       (1000) users      (984)     1060 2023-06-28 08:33:35.000000 joblib-1.3.0/doc/index.rst
--rw-r--r--   0 tom       (1000) users      (984)     1841 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/installing.rst
--rw-r--r--   0 tom       (1000) users      (984)    17016 2023-06-28 08:33:35.000000 joblib-1.3.0/doc/memory.rst
--rw-r--r--   0 tom       (1000) users      (984)    19092 2023-06-28 08:33:35.000000 joblib-1.3.0/doc/parallel.rst
--rw-r--r--   0 tom       (1000) users      (984)     6328 2023-06-28 08:33:35.000000 joblib-1.3.0/doc/parallel_numpy.rst
--rw-r--r--   0 tom       (1000) users      (984)     7247 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/persistence.rst
--rw-r--r--   0 tom       (1000) users      (984)     1680 2023-03-26 21:55:29.000000 joblib-1.3.0/doc/why.rst
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.653354 joblib-1.3.0/joblib/
--rw-r--r--   0 tom       (1000) users      (984)     5132 2023-06-28 13:13:38.000000 joblib-1.3.0/joblib/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)      417 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/_cloudpickle_wrapper.py
--rw-r--r--   0 tom       (1000) users      (984)    13014 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/_dask.py
--rw-r--r--   0 tom       (1000) users      (984)    27908 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/_memmapping_reducer.py
--rw-r--r--   0 tom       (1000) users      (984)     1925 2023-04-30 13:25:43.000000 joblib-1.3.0/joblib/_multiprocessing_helpers.py
--rw-r--r--   0 tom       (1000) users      (984)    25923 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/_parallel_backends.py
--rw-r--r--   0 tom       (1000) users      (984)    16100 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/_store_backends.py
--rw-r--r--   0 tom       (1000) users      (984)     1357 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/_utils.py
--rw-r--r--   0 tom       (1000) users      (984)     5361 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/backports.py
--rw-r--r--   0 tom       (1000) users      (984)    19768 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/compressor.py
--rw-r--r--   0 tom       (1000) users      (984)     4389 2023-04-30 13:25:43.000000 joblib-1.3.0/joblib/disk.py
--rw-r--r--   0 tom       (1000) users      (984)     5136 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/executor.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.653354 joblib-1.3.0/joblib/externals/
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/externals/__init__.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.653354 joblib-1.3.0/joblib/externals/cloudpickle/
--rw-r--r--   0 tom       (1000) users      (984)      292 2023-04-30 13:25:43.000000 joblib-1.3.0/joblib/externals/cloudpickle/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)    35137 2023-04-30 13:25:43.000000 joblib-1.3.0/joblib/externals/cloudpickle/cloudpickle.py
--rw-r--r--   0 tom       (1000) users      (984)    34114 2023-04-30 13:25:43.000000 joblib-1.3.0/joblib/externals/cloudpickle/cloudpickle_fast.py
--rw-r--r--   0 tom       (1000) users      (984)      508 2023-04-30 13:25:43.000000 joblib-1.3.0/joblib/externals/cloudpickle/compat.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.653354 joblib-1.3.0/joblib/externals/loky/
--rw-r--r--   0 tom       (1000) users      (984)     1104 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)     1057 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/_base.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.656687 joblib-1.3.0/joblib/externals/loky/backend/
--rw-r--r--   0 tom       (1000) users      (984)      312 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)     1776 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/_posix_reduction.py
--rw-r--r--   0 tom       (1000) users      (984)      683 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/_win_reduction.py
--rw-r--r--   0 tom       (1000) users      (984)    13510 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/context.py
--rw-r--r--   0 tom       (1000) users      (984)     1186 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/fork_exec.py
--rw-r--r--   0 tom       (1000) users      (984)     5580 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/popen_loky_posix.py
--rw-r--r--   0 tom       (1000) users      (984)     5325 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/popen_loky_win32.py
--rw-r--r--   0 tom       (1000) users      (984)     2018 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/process.py
--rw-r--r--   0 tom       (1000) users      (984)     7322 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/queues.py
--rw-r--r--   0 tom       (1000) users      (984)     7063 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/reduction.py
--rw-r--r--   0 tom       (1000) users      (984)    14498 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/resource_tracker.py
--rw-r--r--   0 tom       (1000) users      (984)     8962 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/spawn.py
--rw-r--r--   0 tom       (1000) users      (984)    11768 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/synchronize.py
--rw-r--r--   0 tom       (1000) users      (984)     5757 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/backend/utils.py
--rw-r--r--   0 tom       (1000) users      (984)     3608 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/cloudpickle_wrapper.py
--rw-r--r--   0 tom       (1000) users      (984)     2567 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/initializers.py
--rw-r--r--   0 tom       (1000) users      (984)    51050 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/process_executor.py
--rw-r--r--   0 tom       (1000) users      (984)    10305 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/externals/loky/reusable_executor.py
--rw-r--r--   0 tom       (1000) users      (984)    14204 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/func_inspect.py
--rw-r--r--   0 tom       (1000) users      (984)    10535 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/hashing.py
--rw-r--r--   0 tom       (1000) users      (984)     5463 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/logger.py
--rw-r--r--   0 tom       (1000) users      (984)    47169 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/memory.py
--rw-r--r--   0 tom       (1000) users      (984)    26886 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/numpy_pickle.py
--rw-r--r--   0 tom       (1000) users      (984)     8547 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/numpy_pickle_compat.py
--rw-r--r--   0 tom       (1000) users      (984)     8705 2023-04-30 13:25:43.000000 joblib-1.3.0/joblib/numpy_pickle_utils.py
--rw-r--r--   0 tom       (1000) users      (984)    81153 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/parallel.py
--rw-r--r--   0 tom       (1000) users      (984)    14411 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/pool.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.656687 joblib-1.3.0/joblib/test/
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/test/__init__.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.656687 joblib-1.3.0/joblib/test/_openmp_test_helper/
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/_openmp_test_helper/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)      749 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/_openmp_test_helper/setup.py
--rw-r--r--   0 tom       (1000) users      (984)     2336 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/test/common.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.660021 joblib-1.3.0/joblib/test/data/
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)     3460 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/test/data/create_numpy_pickle.py
--rw-r--r--   0 tom       (1000) users      (984)      769 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np16.gz
--rw-r--r--   0 tom       (1000) users      (984)      757 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np17.gz
--rw-r--r--   0 tom       (1000) users      (984)      792 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py33_np18.gz
--rw-r--r--   0 tom       (1000) users      (984)      794 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py34_np19.gz
--rw-r--r--   0 tom       (1000) users      (984)      790 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py35_np19.gz
--rw-r--r--   0 tom       (1000) users      (984)      986 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl
--rw-r--r--   0 tom       (1000) users      (984)      997 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.bz2
--rw-r--r--   0 tom       (1000) users      (984)      798 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.gzip
--rw-r--r--   0 tom       (1000) users      (984)      660 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.lzma
--rw-r--r--   0 tom       (1000) users      (984)      712 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.xz
--rw-r--r--   0 tom       (1000) users      (984)     1068 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl
--rw-r--r--   0 tom       (1000) users      (984)     1000 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.bz2
--rw-r--r--   0 tom       (1000) users      (984)      831 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.gzip
--rw-r--r--   0 tom       (1000) users      (984)      694 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.lzma
--rw-r--r--   0 tom       (1000) users      (984)      752 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.xz
--rw-r--r--   0 tom       (1000) users      (984)     1068 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl
--rw-r--r--   0 tom       (1000) users      (984)     1021 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.bz2
--rw-r--r--   0 tom       (1000) users      (984)      831 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.gzip
--rw-r--r--   0 tom       (1000) users      (984)      697 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.lzma
--rw-r--r--   0 tom       (1000) users      (984)      752 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.xz
--rw-r--r--   0 tom       (1000) users      (984)     1068 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl
--rw-r--r--   0 tom       (1000) users      (984)     1005 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.bz2
--rw-r--r--   0 tom       (1000) users      (984)      833 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.gzip
--rw-r--r--   0 tom       (1000) users      (984)      701 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.lzma
--rw-r--r--   0 tom       (1000) users      (984)      752 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.xz
--rw-r--r--   0 tom       (1000) users      (984)      800 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.11.0_compressed_pickle_py36_np111.gz
--rw-r--r--   0 tom       (1000) users      (984)     1068 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl
--rw-r--r--   0 tom       (1000) users      (984)      991 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.bz2
--rw-r--r--   0 tom       (1000) users      (984)      800 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.gzip
--rw-r--r--   0 tom       (1000) users      (984)      715 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.lzma
--rw-r--r--   0 tom       (1000) users      (984)      752 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.xz
--rw-r--r--   0 tom       (1000) users      (984)      659 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.8.4_compressed_pickle_py27_np17.gz
--rw-r--r--   0 tom       (1000) users      (984)      658 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np16.gz
--rw-r--r--   0 tom       (1000) users      (984)      658 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np17.gz
--rw-r--r--   0 tom       (1000) users      (984)      673 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py34_np19.gz
--rw-r--r--   0 tom       (1000) users      (984)      673 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py35_np19.gz
--rw-r--r--   0 tom       (1000) users      (984)      670 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl
--rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_01.npy
--rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_02.npy
--rw-r--r--   0 tom       (1000) users      (984)      236 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_03.npy
--rw-r--r--   0 tom       (1000) users      (984)      104 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_04.npy
--rw-r--r--   0 tom       (1000) users      (984)      670 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl
--rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_01.npy
--rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_02.npy
--rw-r--r--   0 tom       (1000) users      (984)      236 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_03.npy
--rw-r--r--   0 tom       (1000) users      (984)      104 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_04.npy
--rw-r--r--   0 tom       (1000) users      (984)      691 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl
--rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_01.npy
--rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_02.npy
--rw-r--r--   0 tom       (1000) users      (984)      307 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_03.npy
--rw-r--r--   0 tom       (1000) users      (984)      104 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_04.npy
--rw-r--r--   0 tom       (1000) users      (984)      691 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl
--rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_01.npy
--rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_02.npy
--rw-r--r--   0 tom       (1000) users      (984)      307 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_03.npy
--rw-r--r--   0 tom       (1000) users      (984)      104 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_04.npy
--rw-r--r--   0 tom       (1000) users      (984)      691 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl
--rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_01.npy
--rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_02.npy
--rw-r--r--   0 tom       (1000) users      (984)      307 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_03.npy
--rw-r--r--   0 tom       (1000) users      (984)      104 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_04.npy
--rw-r--r--   0 tom       (1000) users      (984)      802 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz
--rw-r--r--   0 tom       (1000) users      (984)       43 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_01.npy.z
--rw-r--r--   0 tom       (1000) users      (984)       43 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_02.npy.z
--rw-r--r--   0 tom       (1000) users      (984)       37 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_03.npy.z
--rw-r--r--   0 tom       (1000) users      (984)     1175 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/test_backports.py
--rw-r--r--   0 tom       (1000) users      (984)      751 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/test/test_cloudpickle_wrapper.py
--rw-r--r--   0 tom       (1000) users      (984)     4303 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/test/test_config.py
--rw-r--r--   0 tom       (1000) users      (984)    18123 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/test/test_dask.py
--rw-r--r--   0 tom       (1000) users      (984)     2205 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/test_disk.py
--rw-r--r--   0 tom       (1000) users      (984)     9488 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/test/test_func_inspect.py
--rw-r--r--   0 tom       (1000) users      (984)      145 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/test/test_func_inspect_special_encoding.py
--rw-r--r--   0 tom       (1000) users      (984)    16054 2023-06-28 08:33:18.000000 joblib-1.3.0/joblib/test/test_hashing.py
--rw-r--r--   0 tom       (1000) users      (984)      422 2023-03-26 21:55:29.000000 joblib-1.3.0/joblib/test/test_init.py
--rw-r--r--   0 tom       (1000) users      (984)      984 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/test/test_logger.py
--rw-r--r--   0 tom       (1000) users      (984)    43298 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/test/test_memmapping.py
--rw-r--r--   0 tom       (1000) users      (984)    49277 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/test/test_memory.py
--rw-r--r--   0 tom       (1000) users      (984)     1123 2023-04-30 13:25:43.000000 joblib-1.3.0/joblib/test/test_missing_multiprocessing.py
--rw-r--r--   0 tom       (1000) users      (984)     1936 2023-04-30 13:25:43.000000 joblib-1.3.0/joblib/test/test_module.py
--rw-r--r--   0 tom       (1000) users      (984)    42485 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/test/test_numpy_pickle.py
--rw-r--r--   0 tom       (1000) users      (984)      609 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/test/test_numpy_pickle_compat.py
--rw-r--r--   0 tom       (1000) users      (984)      383 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/test/test_numpy_pickle_utils.py
--rw-r--r--   0 tom       (1000) users      (984)    68514 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/test/test_parallel.py
--rw-r--r--   0 tom       (1000) users      (984)     3121 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/test/test_store_backends.py
--rw-r--r--   0 tom       (1000) users      (984)     2570 2023-06-28 08:33:35.000000 joblib-1.3.0/joblib/test/test_testing.py
--rw-r--r--   0 tom       (1000) users      (984)      584 2023-04-30 13:25:43.000000 joblib-1.3.0/joblib/test/test_utils.py
--rw-r--r--   0 tom       (1000) users      (984)      251 2023-04-30 13:25:43.000000 joblib-1.3.0/joblib/test/testutils.py
--rw-r--r--   0 tom       (1000) users      (984)     3093 2023-05-19 20:19:06.000000 joblib-1.3.0/joblib/testing.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-28 13:22:14.653354 joblib-1.3.0/joblib.egg-info/
--rw-r--r--   0 tom       (1000) users      (984)     5361 2023-06-28 13:22:14.000000 joblib-1.3.0/joblib.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) users      (984)    19972 2023-06-28 13:22:14.000000 joblib-1.3.0/joblib.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) users      (984)        1 2023-06-28 13:22:14.000000 joblib-1.3.0/joblib.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) users      (984)        7 2023-06-28 13:22:14.000000 joblib-1.3.0/joblib.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) users      (984)     2352 2023-06-28 13:18:07.000000 joblib-1.3.0/pyproject.toml
--rw-r--r--   0 tom       (1000) users      (984)       38 2023-06-28 13:22:14.660021 joblib-1.3.0/setup.cfg
--rwxr-xr-x   0 tom       (1000) users      (984)       92 2023-05-19 20:19:06.000000 joblib-1.3.0/setup.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.810301 joblib-1.3.1/
+-rw-r--r--   0 tom       (1000) users      (984)       99 2023-06-28 08:33:35.000000 joblib-1.3.1/.readthedocs-requirements.txt
+-rw-r--r--   0 tom       (1000) users      (984)     1527 2023-04-30 13:25:43.000000 joblib-1.3.1/LICENSE.txt
+-rw-r--r--   0 tom       (1000) users      (984)      128 2023-03-26 21:55:29.000000 joblib-1.3.1/MANIFEST.in
+-rw-r--r--   0 tom       (1000) users      (984)     5361 2023-06-29 15:14:30.810301 joblib-1.3.1/PKG-INFO
+-rw-r--r--   0 tom       (1000) users      (984)     4210 2023-04-30 13:25:43.000000 joblib-1.3.1/README.rst
+-rw-r--r--   0 tom       (1000) users      (984)     2885 2023-05-19 20:19:06.000000 joblib-1.3.1/conftest.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.740301 joblib-1.3.1/doc/
+-rw-r--r--   0 tom       (1000) users      (984)    36681 2023-06-27 22:12:43.000000 joblib-1.3.1/doc/CHANGES.rst
+-rw-r--r--   0 tom       (1000) users      (984)      535 2023-06-28 08:33:35.000000 joblib-1.3.1/doc/Makefile
+-rw-r--r--   0 tom       (1000) users      (984)     4210 2023-06-27 22:12:43.000000 joblib-1.3.1/doc/README.rst
+-rw-r--r--   0 tom       (1000) users      (984)       95 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/__init__.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.733634 joblib-1.3.1/doc/_build/
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.743634 joblib-1.3.1/doc/_build/html/
+-rw-r--r--   0 tom       (1000) users      (984)      230 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/.buildinfo
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.756967 joblib-1.3.1/doc/_build/html/.doctrees/
+-rw-r--r--   0 tom       (1000) users      (984)   191208 2023-06-27 22:12:43.000000 joblib-1.3.1/doc/_build/html/.doctrees/CHANGES.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    21534 2023-06-27 22:12:43.000000 joblib-1.3.1/doc/_build/html/.doctrees/README.doctree
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.760300 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/
+-rw-r--r--   0 tom       (1000) users      (984)    40483 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/compressors_comparison.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    19900 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/index.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    26656 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/memory_basic_usage.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    26737 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/nested_parallel_memory.doctree
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.760300 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel/
+-rw-r--r--   0 tom       (1000) users      (984)    16962 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel/distributed_backend_simple.doctree
+-rw-r--r--   0 tom       (1000) users      (984)     5867 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel/index.doctree
+-rw-r--r--   0 tom       (1000) users      (984)     5298 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel/sg_execution_times.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    27872 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel_generator.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    35065 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel_memmap.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    27230 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel_random_state.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    32097 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/serialization_and_wrappers.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    12300 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/sg_execution_times.doctree
+-rw-r--r--   0 tom       (1000) users      (984)   214237 2023-06-27 22:12:43.000000 joblib-1.3.1/doc/_build/html/.doctrees/developing.doctree
+-rw-r--r--   0 tom       (1000) users      (984)  6257818 2023-06-27 22:12:43.000000 joblib-1.3.1/doc/_build/html/.doctrees/environment.pickle
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.760300 joblib-1.3.1/doc/_build/html/.doctrees/generated/
+-rw-r--r--   0 tom       (1000) users      (984)    50793 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.Memory.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    79449 2023-06-27 22:12:43.000000 joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.Parallel.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    21941 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.dump.doctree
+-rw-r--r--   0 tom       (1000) users      (984)     7760 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.hash.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    17300 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.load.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    47094 2023-06-27 22:12:43.000000 joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.parallel_config.doctree
+-rw-r--r--   0 tom       (1000) users      (984)     7466 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.register_compressor.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    32300 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/index.doctree
+-rw-r--r--   0 tom       (1000) users      (984)     9749 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/installing.doctree
+-rw-r--r--   0 tom       (1000) users      (984)   155458 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/memory.doctree
+-rw-r--r--   0 tom       (1000) users      (984)   209728 2023-06-27 22:12:43.000000 joblib-1.3.1/doc/_build/html/.doctrees/parallel.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    24195 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/parallel_numpy.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    32670 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/persistence.doctree
+-rw-r--r--   0 tom       (1000) users      (984)     9998 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/.doctrees/why.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    67500 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/CHANGES.html
+-rw-r--r--   0 tom       (1000) users      (984)    12659 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/README.html
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.733634 joblib-1.3.1/doc/_build/html/_downloads/
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/
+-rw-r--r--   0 tom       (1000) users      (984)    43714 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/
+-rw-r--r--   0 tom       (1000) users      (984)     5685 2023-06-26 07:51:11.000000 joblib-1.3.1/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/serialization_and_wrappers.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/
+-rw-r--r--   0 tom       (1000) users      (984)     6043 2023-06-26 07:51:15.000000 joblib-1.3.1/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/parallel_generator.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/
+-rw-r--r--   0 tom       (1000) users      (984)     9044 2023-06-26 07:51:36.000000 joblib-1.3.1/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/compressors_comparison.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/
+-rw-r--r--   0 tom       (1000) users      (984)     7302 2023-06-26 07:50:56.000000 joblib-1.3.1/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/nested_parallel_memory.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/
+-rw-r--r--   0 tom       (1000) users      (984)    62629 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/
+-rw-r--r--   0 tom       (1000) users      (984)     7872 2023-06-26 07:51:12.000000 joblib-1.3.1/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/serialization_and_wrappers.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/
+-rw-r--r--   0 tom       (1000) users      (984)     7282 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/parallel_random_state.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/
+-rw-r--r--   0 tom       (1000) users      (984)     6406 2023-06-26 07:51:11.000000 joblib-1.3.1/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/memory_basic_usage.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/
+-rw-r--r--   0 tom       (1000) users      (984)     4695 2023-06-26 07:50:56.000000 joblib-1.3.1/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/memory_basic_usage.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/
+-rw-r--r--   0 tom       (1000) users      (984)     1984 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/distributed_backend_simple.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/
+-rw-r--r--   0 tom       (1000) users      (984)     8458 2023-06-26 07:51:15.000000 joblib-1.3.1/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/parallel_memmap.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/
+-rw-r--r--   0 tom       (1000) users      (984)     5092 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/nested_parallel_memory.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/
+-rw-r--r--   0 tom       (1000) users      (984)     7821 2023-06-26 07:51:36.000000 joblib-1.3.1/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/parallel_generator.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/
+-rw-r--r--   0 tom       (1000) users      (984)     4551 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/parallel_random_state.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/
+-rw-r--r--   0 tom       (1000) users      (984)    13465 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/compressors_comparison.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/
+-rw-r--r--   0 tom       (1000) users      (984)     5588 2023-06-26 07:51:12.000000 joblib-1.3.1/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/parallel_memmap.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.763634 joblib-1.3.1/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/
+-rw-r--r--   0 tom       (1000) users      (984)     2943 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/distributed_backend_simple.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.766967 joblib-1.3.1/doc/_build/html/_images/
+-rw-r--r--   0 tom       (1000) users      (984)    14175 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/_images/sphx_glr_compressors_comparison_001.png
+-rw-r--r--   0 tom       (1000) users      (984)     7869 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/_images/sphx_glr_compressors_comparison_002.png
+-rw-r--r--   0 tom       (1000) users      (984)    13471 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/_build/html/_images/sphx_glr_compressors_comparison_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/_images/sphx_glr_distributed_backend_simple_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:11.000000 joblib-1.3.1/doc/_build/html/_images/sphx_glr_memory_basic_usage_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:50:56.000000 joblib-1.3.1/doc/_build/html/_images/sphx_glr_nested_parallel_memory_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    22465 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/_images/sphx_glr_parallel_generator_001.png
+-rw-r--r--   0 tom       (1000) users      (984)    14949 2023-06-26 07:51:36.000000 joblib-1.3.1/doc/_build/html/_images/sphx_glr_parallel_generator_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:15.000000 joblib-1.3.1/doc/_build/html/_images/sphx_glr_parallel_memmap_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/_build/html/_images/sphx_glr_parallel_random_state_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:12.000000 joblib-1.3.1/doc/_build/html/_images/sphx_glr_serialization_and_wrappers_thumb.png
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.766967 joblib-1.3.1/doc/_build/html/_sources/
+-rw-r--r--   0 tom       (1000) users      (984)    36681 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/_build/html/_sources/CHANGES.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     4210 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/_build/html/_sources/README.rst.txt
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.770301 joblib-1.3.1/doc/_build/html/_sources/auto_examples/
+-rw-r--r--   0 tom       (1000) users      (984)    13174 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/compressors_comparison.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     4940 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/index.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     7558 2023-06-26 07:51:11.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/memory_basic_usage.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     7412 2023-06-26 07:50:56.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/nested_parallel_memory.rst.txt
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.770301 joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel/
+-rw-r--r--   0 tom       (1000) users      (984)     4449 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel/distributed_backend_simple.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      789 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel/index.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      569 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel/sg_execution_times.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     8603 2023-06-26 07:51:36.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel_generator.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)    10854 2023-06-26 07:51:15.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel_memmap.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     8234 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel_random_state.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     9859 2023-06-26 07:51:12.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/serialization_and_wrappers.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     1976 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/_build/html/_sources/auto_examples/sg_execution_times.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)       97 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_build/html/_sources/developing.rst.txt
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.770301 joblib-1.3.1/doc/_build/html/_sources/generated/
+-rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/_build/html/_sources/generated/joblib.Memory.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      197 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/_build/html/_sources/generated/joblib.Parallel.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/_build/html/_sources/generated/joblib.dump.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/_build/html/_sources/generated/joblib.hash.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/_build/html/_sources/generated/joblib.load.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      234 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/_build/html/_sources/generated/joblib.parallel_config.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      247 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/_build/html/_sources/generated/joblib.register_compressor.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     1060 2023-06-23 14:57:25.000000 joblib-1.3.1/doc/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     1841 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_build/html/_sources/installing.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)    17016 2023-06-23 14:57:25.000000 joblib-1.3.1/doc/_build/html/_sources/memory.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)    18614 2023-06-27 22:12:21.000000 joblib-1.3.1/doc/_build/html/_sources/parallel.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     6336 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_build/html/_sources/parallel_numpy.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     7247 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_build/html/_sources/persistence.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     1680 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_build/html/_sources/why.rst.txt
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.773634 joblib-1.3.1/doc/_build/html/_static/
+-rw-r--r--   0 tom       (1000) users      (984)    11230 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/_static/alabaster.css
+-rw-r--r--   0 tom       (1000) users      (984)    14813 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/_static/basic.css
+-rw-r--r--   0 tom       (1000) users      (984)     3380 2023-04-18 19:56:48.000000 joblib-1.3.1/doc/_build/html/_static/binder_badge_logo.svg
+-rw-r--r--   0 tom       (1000) users      (984)    21404 2023-04-18 19:56:48.000000 joblib-1.3.1/doc/_build/html/_static/broken_example.png
+-rw-r--r--   0 tom       (1000) users      (984)     1018 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_build/html/_static/custom.css
+-rw-r--r--   0 tom       (1000) users      (984)     4472 2023-06-26 07:49:58.000000 joblib-1.3.1/doc/_build/html/_static/doctools.js
+-rw-r--r--   0 tom       (1000) users      (984)      425 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/_static/documentation_options.js
+-rw-r--r--   0 tom       (1000) users      (984)   268286 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_build/html/_static/favicon.ico
+-rw-r--r--   0 tom       (1000) users      (984)      286 2023-06-26 07:49:58.000000 joblib-1.3.1/doc/_build/html/_static/file.png
+-rw-r--r--   0 tom       (1000) users      (984)    15594 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_build/html/_static/joblib_logo.svg
+-rw-r--r--   0 tom       (1000) users      (984)    27703 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_build/html/_static/joblib_logo_examples.png
+-rw-r--r--   0 tom       (1000) users      (984)     6936 2023-04-18 19:56:48.000000 joblib-1.3.1/doc/_build/html/_static/jupyterlite_badge_logo.svg
+-rw-r--r--   0 tom       (1000) users      (984)     4758 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/_static/language_data.js
+-rw-r--r--   0 tom       (1000) users      (984)       90 2023-06-26 07:49:58.000000 joblib-1.3.1/doc/_build/html/_static/minus.png
+-rw-r--r--   0 tom       (1000) users      (984)     4315 2023-04-18 19:56:48.000000 joblib-1.3.1/doc/_build/html/_static/no_image.png
+-rw-r--r--   0 tom       (1000) users      (984)       90 2023-06-26 07:49:58.000000 joblib-1.3.1/doc/_build/html/_static/plus.png
+-rw-r--r--   0 tom       (1000) users      (984)     4846 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/_static/pygments.css
+-rw-r--r--   0 tom       (1000) users      (984)    18215 2023-06-26 07:49:58.000000 joblib-1.3.1/doc/_build/html/_static/searchtools.js
+-rw-r--r--   0 tom       (1000) users      (984)      167 2023-04-18 19:56:48.000000 joblib-1.3.1/doc/_build/html/_static/sg_gallery-binder.css
+-rw-r--r--   0 tom       (1000) users      (984)     1137 2023-04-18 19:56:48.000000 joblib-1.3.1/doc/_build/html/_static/sg_gallery-dataframe.css
+-rw-r--r--   0 tom       (1000) users      (984)     4330 2023-04-18 19:56:48.000000 joblib-1.3.1/doc/_build/html/_static/sg_gallery-rendered-html.css
+-rw-r--r--   0 tom       (1000) users      (984)     9530 2023-04-18 19:56:48.000000 joblib-1.3.1/doc/_build/html/_static/sg_gallery.css
+-rw-r--r--   0 tom       (1000) users      (984)     4712 2023-06-26 07:49:58.000000 joblib-1.3.1/doc/_build/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.776967 joblib-1.3.1/doc/_build/html/auto_examples/
+-rw-r--r--   0 tom       (1000) users      (984)    60961 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/compressors_comparison.html
+-rw-r--r--   0 tom       (1000) users      (984)    10642 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/index.html
+-rw-r--r--   0 tom       (1000) users      (984)    38082 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/memory_basic_usage.html
+-rw-r--r--   0 tom       (1000) users      (984)    35272 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/nested_parallel_memory.html
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.776967 joblib-1.3.1/doc/_build/html/auto_examples/parallel/
+-rw-r--r--   0 tom       (1000) users      (984)    14139 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/parallel/distributed_backend_simple.html
+-rw-r--r--   0 tom       (1000) users      (984)     5718 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/parallel/index.html
+-rw-r--r--   0 tom       (1000) users      (984)     5134 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/parallel/sg_execution_times.html
+-rw-r--r--   0 tom       (1000) users      (984)    29778 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/parallel_generator.html
+-rw-r--r--   0 tom       (1000) users      (984)    44012 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/parallel_memmap.html
+-rw-r--r--   0 tom       (1000) users      (984)    36234 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/parallel_random_state.html
+-rw-r--r--   0 tom       (1000) users      (984)    32607 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/serialization_and_wrappers.html
+-rw-r--r--   0 tom       (1000) users      (984)     7236 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/auto_examples/sg_execution_times.html
+-rw-r--r--   0 tom       (1000) users      (984)    77562 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/developing.html
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.780301 joblib-1.3.1/doc/_build/html/generated/
+-rw-r--r--   0 tom       (1000) users      (984)    19179 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/generated/joblib.Memory.html
+-rw-r--r--   0 tom       (1000) users      (984)    33735 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/generated/joblib.Parallel.html
+-rw-r--r--   0 tom       (1000) users      (984)     9992 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/generated/joblib.dump.html
+-rw-r--r--   0 tom       (1000) users      (984)     6212 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/generated/joblib.hash.html
+-rw-r--r--   0 tom       (1000) users      (984)     8920 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/generated/joblib.load.html
+-rw-r--r--   0 tom       (1000) users      (984)    19398 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/generated/joblib.parallel_config.html
+-rw-r--r--   0 tom       (1000) users      (984)     6025 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/generated/joblib.register_compressor.html
+-rw-r--r--   0 tom       (1000) users      (984)     9965 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/genindex.html
+-rw-r--r--   0 tom       (1000) users      (984)    22003 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/index.html
+-rw-r--r--   0 tom       (1000) users      (984)     8933 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/installing.html
+-rw-r--r--   0 tom       (1000) users      (984)    75468 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/memory.html
+-rw-r--r--   0 tom       (1000) users      (984)     1766 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/objects.inv
+-rw-r--r--   0 tom       (1000) users      (984)   108722 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/parallel.html
+-rw-r--r--   0 tom       (1000) users      (984)    21134 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/parallel_numpy.html
+-rw-r--r--   0 tom       (1000) users      (984)    30312 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/persistence.html
+-rw-r--r--   0 tom       (1000) users      (984)     4509 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/py-modindex.html
+-rw-r--r--   0 tom       (1000) users      (984)     4748 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/search.html
+-rw-r--r--   0 tom       (1000) users      (984)    76600 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/searchindex.js
+-rw-r--r--   0 tom       (1000) users      (984)     7402 2023-06-27 22:12:44.000000 joblib-1.3.1/doc/_build/html/why.html
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.780301 joblib-1.3.1/doc/_static/
+-rw-r--r--   0 tom       (1000) users      (984)     1018 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_static/custom.css
+-rw-r--r--   0 tom       (1000) users      (984)   268286 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_static/favicon.ico
+-rw-r--r--   0 tom       (1000) users      (984)    15594 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_static/joblib_logo.svg
+-rw-r--r--   0 tom       (1000) users      (984)    27703 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_static/joblib_logo_examples.png
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.780301 joblib-1.3.1/doc/_templates/
+-rw-r--r--   0 tom       (1000) users      (984)      208 2023-06-28 08:33:35.000000 joblib-1.3.1/doc/_templates/class.rst
+-rw-r--r--   0 tom       (1000) users      (984)      226 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_templates/function.rst
+-rw-r--r--   0 tom       (1000) users      (984)      479 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/_templates/layout.html
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.786967 joblib-1.3.1/doc/auto_examples/
+-rw-r--r--   0 tom       (1000) users      (984)    62629 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/auto_examples/auto_examples_jupyter.zip
+-rw-r--r--   0 tom       (1000) users      (984)    43714 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/auto_examples/auto_examples_python.zip
+-rw-r--r--   0 tom       (1000) users      (984)    13465 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/auto_examples/compressors_comparison.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     9044 2023-06-26 07:51:36.000000 joblib-1.3.1/doc/auto_examples/compressors_comparison.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/auto_examples/compressors_comparison.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)    13174 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/auto_examples/compressors_comparison.rst
+-rw-r--r--   0 tom       (1000) users      (984)     3437 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/auto_examples/compressors_comparison_codeobj.pickle
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.786967 joblib-1.3.1/doc/auto_examples/images/
+-rw-r--r--   0 tom       (1000) users      (984)    14175 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/auto_examples/images/sphx_glr_compressors_comparison_001.png
+-rw-r--r--   0 tom       (1000) users      (984)     7869 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/auto_examples/images/sphx_glr_compressors_comparison_002.png
+-rw-r--r--   0 tom       (1000) users      (984)    22465 2023-06-26 07:51:36.000000 joblib-1.3.1/doc/auto_examples/images/sphx_glr_parallel_generator_001.png
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.790301 joblib-1.3.1/doc/auto_examples/images/thumb/
+-rw-r--r--   0 tom       (1000) users      (984)    13471 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_compressors_comparison_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:11.000000 joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_memory_basic_usage_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:50:56.000000 joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_nested_parallel_memory_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    14949 2023-06-26 07:51:36.000000 joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_parallel_generator_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:15.000000 joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_parallel_memmap_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_parallel_random_state_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:12.000000 joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_serialization_and_wrappers_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)     4940 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/auto_examples/index.rst
+-rw-r--r--   0 tom       (1000) users      (984)     6406 2023-06-26 07:51:11.000000 joblib-1.3.1/doc/auto_examples/memory_basic_usage.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     4695 2023-06-26 07:50:56.000000 joblib-1.3.1/doc/auto_examples/memory_basic_usage.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:11.000000 joblib-1.3.1/doc/auto_examples/memory_basic_usage.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)     7558 2023-06-26 07:51:11.000000 joblib-1.3.1/doc/auto_examples/memory_basic_usage.rst
+-rw-r--r--   0 tom       (1000) users      (984)     2516 2023-06-26 07:51:11.000000 joblib-1.3.1/doc/auto_examples/memory_basic_usage_codeobj.pickle
+-rw-r--r--   0 tom       (1000) users      (984)     7302 2023-06-26 07:50:56.000000 joblib-1.3.1/doc/auto_examples/nested_parallel_memory.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     5092 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/auto_examples/nested_parallel_memory.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:50:56.000000 joblib-1.3.1/doc/auto_examples/nested_parallel_memory.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)     7412 2023-06-26 07:50:56.000000 joblib-1.3.1/doc/auto_examples/nested_parallel_memory.rst
+-rw-r--r--   0 tom       (1000) users      (984)     2729 2023-06-26 07:50:56.000000 joblib-1.3.1/doc/auto_examples/nested_parallel_memory_codeobj.pickle
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.790301 joblib-1.3.1/doc/auto_examples/parallel/
+-rw-r--r--   0 tom       (1000) users      (984)     2943 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/auto_examples/parallel/distributed_backend_simple.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     1984 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/auto_examples/parallel/distributed_backend_simple.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/auto_examples/parallel/distributed_backend_simple.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)     4449 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/auto_examples/parallel/distributed_backend_simple.rst
+-rw-r--r--   0 tom       (1000) users      (984)     2457 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/auto_examples/parallel/distributed_backend_simple_codeobj.pickle
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.736967 joblib-1.3.1/doc/auto_examples/parallel/images/
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.790301 joblib-1.3.1/doc/auto_examples/parallel/images/thumb/
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/auto_examples/parallel/images/thumb/sphx_glr_distributed_backend_simple_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)      789 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/auto_examples/parallel/index.rst
+-rw-r--r--   0 tom       (1000) users      (984)      569 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/auto_examples/parallel/sg_execution_times.rst
+-rw-r--r--   0 tom       (1000) users      (984)     7821 2023-06-26 07:51:36.000000 joblib-1.3.1/doc/auto_examples/parallel_generator.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     6043 2023-06-26 07:51:15.000000 joblib-1.3.1/doc/auto_examples/parallel_generator.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:36.000000 joblib-1.3.1/doc/auto_examples/parallel_generator.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)     8603 2023-06-26 07:51:36.000000 joblib-1.3.1/doc/auto_examples/parallel_generator.rst
+-rw-r--r--   0 tom       (1000) users      (984)     2899 2023-06-26 07:51:36.000000 joblib-1.3.1/doc/auto_examples/parallel_generator_codeobj.pickle
+-rw-r--r--   0 tom       (1000) users      (984)     8458 2023-06-26 07:51:15.000000 joblib-1.3.1/doc/auto_examples/parallel_memmap.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     5588 2023-06-26 07:51:12.000000 joblib-1.3.1/doc/auto_examples/parallel_memmap.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:15.000000 joblib-1.3.1/doc/auto_examples/parallel_memmap.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)    10854 2023-06-26 07:51:15.000000 joblib-1.3.1/doc/auto_examples/parallel_memmap.rst
+-rw-r--r--   0 tom       (1000) users      (984)     2644 2023-06-26 07:51:15.000000 joblib-1.3.1/doc/auto_examples/parallel_memmap_codeobj.pickle
+-rw-r--r--   0 tom       (1000) users      (984)     7282 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/auto_examples/parallel_random_state.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     4551 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/auto_examples/parallel_random_state.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/auto_examples/parallel_random_state.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)     8234 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/auto_examples/parallel_random_state.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1872 2023-06-26 07:50:44.000000 joblib-1.3.1/doc/auto_examples/parallel_random_state_codeobj.pickle
+-rw-r--r--   0 tom       (1000) users      (984)      236 2023-06-26 07:51:47.000000 joblib-1.3.1/doc/auto_examples/searchindex.bak
+-rw-r--r--   0 tom       (1000) users      (984)    99137 2023-06-26 07:51:47.000000 joblib-1.3.1/doc/auto_examples/searchindex.dat
+-rw-r--r--   0 tom       (1000) users      (984)      236 2023-06-26 07:51:47.000000 joblib-1.3.1/doc/auto_examples/searchindex.dir
+-rw-r--r--   0 tom       (1000) users      (984)     7872 2023-06-26 07:51:12.000000 joblib-1.3.1/doc/auto_examples/serialization_and_wrappers.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     5685 2023-06-26 07:51:11.000000 joblib-1.3.1/doc/auto_examples/serialization_and_wrappers.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2023-06-26 07:51:12.000000 joblib-1.3.1/doc/auto_examples/serialization_and_wrappers.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)     9859 2023-06-26 07:51:12.000000 joblib-1.3.1/doc/auto_examples/serialization_and_wrappers.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1572 2023-06-26 07:51:12.000000 joblib-1.3.1/doc/auto_examples/serialization_and_wrappers_codeobj.pickle
+-rw-r--r--   0 tom       (1000) users      (984)     1976 2023-06-26 07:51:45.000000 joblib-1.3.1/doc/auto_examples/sg_execution_times.rst
+-rw-r--r--   0 tom       (1000) users      (984)     7882 2023-06-28 08:33:35.000000 joblib-1.3.1/doc/conf.py
+-rw-r--r--   0 tom       (1000) users      (984)      624 2023-05-19 20:19:06.000000 joblib-1.3.1/doc/conftest.py
+-rw-r--r--   0 tom       (1000) users      (984)       97 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/developing.rst
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.793634 joblib-1.3.1/doc/generated/
+-rw-r--r--   0 tom       (1000) users      (984)     1233 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Logger.cache.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1233 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Logger.clear.examples
+-rw-r--r--   0 tom       (1000) users      (984)     3855 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Logger.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1235 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.MemorizedFunc.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Memory.__init__.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1233 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Memory.cache.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1233 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Memory.clear.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Memory.eval.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1221 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Memory.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Memory.format.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Memory.reduce_size.examples
+-rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/generated/joblib.Memory.rst
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Parallel.dispatch_next.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Parallel.dispatch_one_batch.examples
+-rw-r--r--   0 tom       (1000) users      (984)     3366 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Parallel.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Parallel.format.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.Parallel.print_progress.examples
+-rw-r--r--   0 tom       (1000) users      (984)      197 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/generated/joblib.Parallel.rst
+-rw-r--r--   0 tom       (1000) users      (984)     3364 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.delayed.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1210 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.dump.examples
+-rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/generated/joblib.dump.rst
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.expires_after.examples
+-rw-r--r--   0 tom       (1000) users      (984)      763 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.externals.loky.set_loky_pickler.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.hash.examples
+-rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/generated/joblib.hash.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1210 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.load.examples
+-rw-r--r--   0 tom       (1000) users      (984)      187 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/generated/joblib.load.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1247 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.logger.Logger.cache.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1247 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.logger.Logger.clear.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.memory.MemorizedFunc.__init__.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.memory.MemorizedFunc.call.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.memory.MemorizedFunc.check_call_in_cache.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.memory.MemorizedFunc.clear.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1249 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.memory.MemorizedFunc.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.parallel.AutoBatchingMixin.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.parallel.ParallelBackendBase.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1295 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.parallel_config.examples
+-rw-r--r--   0 tom       (1000) users      (984)      234 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/generated/joblib.parallel_config.rst
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.register_compressor.examples
+-rw-r--r--   0 tom       (1000) users      (984)      247 2023-06-26 07:50:43.000000 joblib-1.3.1/doc/generated/joblib.register_compressor.rst
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.register_parallel_backend.examples
+-rw-r--r--   0 tom       (1000) users      (984)      753 2023-06-26 07:51:46.000000 joblib-1.3.1/doc/generated/joblib.wrap_non_picklable_objects.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1060 2023-06-28 08:33:35.000000 joblib-1.3.1/doc/index.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1841 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/installing.rst
+-rw-r--r--   0 tom       (1000) users      (984)    17016 2023-06-28 08:33:35.000000 joblib-1.3.1/doc/memory.rst
+-rw-r--r--   0 tom       (1000) users      (984)    19092 2023-06-28 08:33:35.000000 joblib-1.3.1/doc/parallel.rst
+-rw-r--r--   0 tom       (1000) users      (984)     6328 2023-06-28 08:33:35.000000 joblib-1.3.1/doc/parallel_numpy.rst
+-rw-r--r--   0 tom       (1000) users      (984)     7247 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/persistence.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1680 2023-03-26 21:55:29.000000 joblib-1.3.1/doc/why.rst
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.796967 joblib-1.3.1/joblib/
+-rw-r--r--   0 tom       (1000) users      (984)     5132 2023-06-29 15:14:21.000000 joblib-1.3.1/joblib/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)      417 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/_cloudpickle_wrapper.py
+-rw-r--r--   0 tom       (1000) users      (984)    13014 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/_dask.py
+-rw-r--r--   0 tom       (1000) users      (984)    27908 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/_memmapping_reducer.py
+-rw-r--r--   0 tom       (1000) users      (984)     1925 2023-04-30 13:25:43.000000 joblib-1.3.1/joblib/_multiprocessing_helpers.py
+-rw-r--r--   0 tom       (1000) users      (984)    25923 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/_parallel_backends.py
+-rw-r--r--   0 tom       (1000) users      (984)    16100 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/_store_backends.py
+-rw-r--r--   0 tom       (1000) users      (984)     1357 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/_utils.py
+-rw-r--r--   0 tom       (1000) users      (984)     5361 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/backports.py
+-rw-r--r--   0 tom       (1000) users      (984)    19768 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/compressor.py
+-rw-r--r--   0 tom       (1000) users      (984)     4389 2023-04-30 13:25:43.000000 joblib-1.3.1/joblib/disk.py
+-rw-r--r--   0 tom       (1000) users      (984)     5136 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/executor.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.796967 joblib-1.3.1/joblib/externals/
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/externals/__init__.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.800301 joblib-1.3.1/joblib/externals/cloudpickle/
+-rw-r--r--   0 tom       (1000) users      (984)      292 2023-04-30 13:25:43.000000 joblib-1.3.1/joblib/externals/cloudpickle/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)    35137 2023-04-30 13:25:43.000000 joblib-1.3.1/joblib/externals/cloudpickle/cloudpickle.py
+-rw-r--r--   0 tom       (1000) users      (984)    34114 2023-04-30 13:25:43.000000 joblib-1.3.1/joblib/externals/cloudpickle/cloudpickle_fast.py
+-rw-r--r--   0 tom       (1000) users      (984)      508 2023-04-30 13:25:43.000000 joblib-1.3.1/joblib/externals/cloudpickle/compat.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.800301 joblib-1.3.1/joblib/externals/loky/
+-rw-r--r--   0 tom       (1000) users      (984)     1104 2023-06-29 15:14:21.000000 joblib-1.3.1/joblib/externals/loky/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)     1057 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/_base.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.800301 joblib-1.3.1/joblib/externals/loky/backend/
+-rw-r--r--   0 tom       (1000) users      (984)      312 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)     1776 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/_posix_reduction.py
+-rw-r--r--   0 tom       (1000) users      (984)      683 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/_win_reduction.py
+-rw-r--r--   0 tom       (1000) users      (984)    13654 2023-06-29 15:14:21.000000 joblib-1.3.1/joblib/externals/loky/backend/context.py
+-rw-r--r--   0 tom       (1000) users      (984)     1186 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/fork_exec.py
+-rw-r--r--   0 tom       (1000) users      (984)     5580 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/popen_loky_posix.py
+-rw-r--r--   0 tom       (1000) users      (984)     5325 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/popen_loky_win32.py
+-rw-r--r--   0 tom       (1000) users      (984)     2018 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/process.py
+-rw-r--r--   0 tom       (1000) users      (984)     7322 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/queues.py
+-rw-r--r--   0 tom       (1000) users      (984)     7063 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/reduction.py
+-rw-r--r--   0 tom       (1000) users      (984)    14498 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/resource_tracker.py
+-rw-r--r--   0 tom       (1000) users      (984)     8962 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/spawn.py
+-rw-r--r--   0 tom       (1000) users      (984)    11768 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/synchronize.py
+-rw-r--r--   0 tom       (1000) users      (984)     5757 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/backend/utils.py
+-rw-r--r--   0 tom       (1000) users      (984)     3608 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/cloudpickle_wrapper.py
+-rw-r--r--   0 tom       (1000) users      (984)     2567 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/initializers.py
+-rw-r--r--   0 tom       (1000) users      (984)    51050 2023-06-29 13:08:10.000000 joblib-1.3.1/joblib/externals/loky/process_executor.py
+-rw-r--r--   0 tom       (1000) users      (984)    10305 2023-06-29 13:10:50.000000 joblib-1.3.1/joblib/externals/loky/reusable_executor.py
+-rw-r--r--   0 tom       (1000) users      (984)    14204 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/func_inspect.py
+-rw-r--r--   0 tom       (1000) users      (984)    10535 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/hashing.py
+-rw-r--r--   0 tom       (1000) users      (984)     5463 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/logger.py
+-rw-r--r--   0 tom       (1000) users      (984)    47169 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/memory.py
+-rw-r--r--   0 tom       (1000) users      (984)    26886 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/numpy_pickle.py
+-rw-r--r--   0 tom       (1000) users      (984)     8547 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/numpy_pickle_compat.py
+-rw-r--r--   0 tom       (1000) users      (984)     8705 2023-04-30 13:25:43.000000 joblib-1.3.1/joblib/numpy_pickle_utils.py
+-rw-r--r--   0 tom       (1000) users      (984)    81153 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/parallel.py
+-rw-r--r--   0 tom       (1000) users      (984)    14411 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/pool.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.803634 joblib-1.3.1/joblib/test/
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/test/__init__.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.803634 joblib-1.3.1/joblib/test/_openmp_test_helper/
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/_openmp_test_helper/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)      749 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/_openmp_test_helper/setup.py
+-rw-r--r--   0 tom       (1000) users      (984)     2336 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/test/common.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.810301 joblib-1.3.1/joblib/test/data/
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)     3460 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/test/data/create_numpy_pickle.py
+-rw-r--r--   0 tom       (1000) users      (984)      769 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np16.gz
+-rw-r--r--   0 tom       (1000) users      (984)      757 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np17.gz
+-rw-r--r--   0 tom       (1000) users      (984)      792 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_compressed_pickle_py33_np18.gz
+-rw-r--r--   0 tom       (1000) users      (984)      794 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_compressed_pickle_py34_np19.gz
+-rw-r--r--   0 tom       (1000) users      (984)      790 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_compressed_pickle_py35_np19.gz
+-rw-r--r--   0 tom       (1000) users      (984)      986 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      997 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.bz2
+-rw-r--r--   0 tom       (1000) users      (984)      798 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.gzip
+-rw-r--r--   0 tom       (1000) users      (984)      660 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.lzma
+-rw-r--r--   0 tom       (1000) users      (984)      712 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.xz
+-rw-r--r--   0 tom       (1000) users      (984)     1068 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl
+-rw-r--r--   0 tom       (1000) users      (984)     1000 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.bz2
+-rw-r--r--   0 tom       (1000) users      (984)      831 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.gzip
+-rw-r--r--   0 tom       (1000) users      (984)      694 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.lzma
+-rw-r--r--   0 tom       (1000) users      (984)      752 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.xz
+-rw-r--r--   0 tom       (1000) users      (984)     1068 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl
+-rw-r--r--   0 tom       (1000) users      (984)     1021 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.bz2
+-rw-r--r--   0 tom       (1000) users      (984)      831 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.gzip
+-rw-r--r--   0 tom       (1000) users      (984)      697 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.lzma
+-rw-r--r--   0 tom       (1000) users      (984)      752 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.xz
+-rw-r--r--   0 tom       (1000) users      (984)     1068 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl
+-rw-r--r--   0 tom       (1000) users      (984)     1005 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.bz2
+-rw-r--r--   0 tom       (1000) users      (984)      833 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.gzip
+-rw-r--r--   0 tom       (1000) users      (984)      701 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.lzma
+-rw-r--r--   0 tom       (1000) users      (984)      752 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.xz
+-rw-r--r--   0 tom       (1000) users      (984)      800 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.11.0_compressed_pickle_py36_np111.gz
+-rw-r--r--   0 tom       (1000) users      (984)     1068 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      991 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.bz2
+-rw-r--r--   0 tom       (1000) users      (984)      800 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.gzip
+-rw-r--r--   0 tom       (1000) users      (984)      715 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.lzma
+-rw-r--r--   0 tom       (1000) users      (984)      752 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.xz
+-rw-r--r--   0 tom       (1000) users      (984)      659 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.8.4_compressed_pickle_py27_np17.gz
+-rw-r--r--   0 tom       (1000) users      (984)      658 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np16.gz
+-rw-r--r--   0 tom       (1000) users      (984)      658 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np17.gz
+-rw-r--r--   0 tom       (1000) users      (984)      673 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_compressed_pickle_py34_np19.gz
+-rw-r--r--   0 tom       (1000) users      (984)      673 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_compressed_pickle_py35_np19.gz
+-rw-r--r--   0 tom       (1000) users      (984)      670 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_01.npy
+-rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_02.npy
+-rw-r--r--   0 tom       (1000) users      (984)      236 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_03.npy
+-rw-r--r--   0 tom       (1000) users      (984)      104 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_04.npy
+-rw-r--r--   0 tom       (1000) users      (984)      670 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_01.npy
+-rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_02.npy
+-rw-r--r--   0 tom       (1000) users      (984)      236 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_03.npy
+-rw-r--r--   0 tom       (1000) users      (984)      104 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_04.npy
+-rw-r--r--   0 tom       (1000) users      (984)      691 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_01.npy
+-rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_02.npy
+-rw-r--r--   0 tom       (1000) users      (984)      307 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_03.npy
+-rw-r--r--   0 tom       (1000) users      (984)      104 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_04.npy
+-rw-r--r--   0 tom       (1000) users      (984)      691 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_01.npy
+-rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_02.npy
+-rw-r--r--   0 tom       (1000) users      (984)      307 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_03.npy
+-rw-r--r--   0 tom       (1000) users      (984)      104 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_04.npy
+-rw-r--r--   0 tom       (1000) users      (984)      691 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_01.npy
+-rw-r--r--   0 tom       (1000) users      (984)      120 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_02.npy
+-rw-r--r--   0 tom       (1000) users      (984)      307 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_03.npy
+-rw-r--r--   0 tom       (1000) users      (984)      104 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_04.npy
+-rw-r--r--   0 tom       (1000) users      (984)      802 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz
+-rw-r--r--   0 tom       (1000) users      (984)       43 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_01.npy.z
+-rw-r--r--   0 tom       (1000) users      (984)       43 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_02.npy.z
+-rw-r--r--   0 tom       (1000) users      (984)       37 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_03.npy.z
+-rw-r--r--   0 tom       (1000) users      (984)     1175 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/test_backports.py
+-rw-r--r--   0 tom       (1000) users      (984)      751 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/test/test_cloudpickle_wrapper.py
+-rw-r--r--   0 tom       (1000) users      (984)     4303 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/test/test_config.py
+-rw-r--r--   0 tom       (1000) users      (984)    18123 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/test/test_dask.py
+-rw-r--r--   0 tom       (1000) users      (984)     2205 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/test_disk.py
+-rw-r--r--   0 tom       (1000) users      (984)     9488 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/test/test_func_inspect.py
+-rw-r--r--   0 tom       (1000) users      (984)      145 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/test/test_func_inspect_special_encoding.py
+-rw-r--r--   0 tom       (1000) users      (984)    16054 2023-06-28 08:33:18.000000 joblib-1.3.1/joblib/test/test_hashing.py
+-rw-r--r--   0 tom       (1000) users      (984)      422 2023-03-26 21:55:29.000000 joblib-1.3.1/joblib/test/test_init.py
+-rw-r--r--   0 tom       (1000) users      (984)      984 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/test/test_logger.py
+-rw-r--r--   0 tom       (1000) users      (984)    43298 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/test/test_memmapping.py
+-rw-r--r--   0 tom       (1000) users      (984)    49277 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/test/test_memory.py
+-rw-r--r--   0 tom       (1000) users      (984)     1123 2023-04-30 13:25:43.000000 joblib-1.3.1/joblib/test/test_missing_multiprocessing.py
+-rw-r--r--   0 tom       (1000) users      (984)     1936 2023-04-30 13:25:43.000000 joblib-1.3.1/joblib/test/test_module.py
+-rw-r--r--   0 tom       (1000) users      (984)    42485 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/test/test_numpy_pickle.py
+-rw-r--r--   0 tom       (1000) users      (984)      609 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/test/test_numpy_pickle_compat.py
+-rw-r--r--   0 tom       (1000) users      (984)      383 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/test/test_numpy_pickle_utils.py
+-rw-r--r--   0 tom       (1000) users      (984)    68514 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/test/test_parallel.py
+-rw-r--r--   0 tom       (1000) users      (984)     3121 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/test/test_store_backends.py
+-rw-r--r--   0 tom       (1000) users      (984)     2570 2023-06-28 08:33:35.000000 joblib-1.3.1/joblib/test/test_testing.py
+-rw-r--r--   0 tom       (1000) users      (984)      584 2023-04-30 13:25:43.000000 joblib-1.3.1/joblib/test/test_utils.py
+-rw-r--r--   0 tom       (1000) users      (984)      251 2023-04-30 13:25:43.000000 joblib-1.3.1/joblib/test/testutils.py
+-rw-r--r--   0 tom       (1000) users      (984)     3093 2023-05-19 20:19:06.000000 joblib-1.3.1/joblib/testing.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 15:14:30.796967 joblib-1.3.1/joblib.egg-info/
+-rw-r--r--   0 tom       (1000) users      (984)     5361 2023-06-29 15:14:30.000000 joblib-1.3.1/joblib.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) users      (984)    19982 2023-06-29 15:14:30.000000 joblib-1.3.1/joblib.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) users      (984)        1 2023-06-29 15:14:30.000000 joblib-1.3.1/joblib.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) users      (984)        7 2023-06-29 15:14:30.000000 joblib-1.3.1/joblib.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) users      (984)     2341 2023-06-28 13:43:42.000000 joblib-1.3.1/pyproject.toml
+-rw-r--r--   0 tom       (1000) users      (984)      172 2023-06-29 15:14:30.813634 joblib-1.3.1/setup.cfg
+-rwxr-xr-x   0 tom       (1000) users      (984)       92 2023-05-19 20:19:06.000000 joblib-1.3.1/setup.py
```

### Comparing `joblib-1.3.0/LICENSE.txt` & `joblib-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/PKG-INFO` & `joblib-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joblib
-Version: 1.3.0
+Version: 1.3.1
 Summary: Lightweight pipelining with Python functions
 Author-email: Gael Varoquaux <gael.varoquaux@normalesup.org>
 License: BSD 3-Clause
 Project-URL: Homepage, https://joblib.readthedocs.io
 Project-URL: Source, https://github.com/joblib/joblib
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `joblib-1.3.0/README.rst` & `joblib-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/conftest.py` & `joblib-1.3.1/conftest.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/CHANGES.rst` & `joblib-1.3.1/doc/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/Makefile` & `joblib-1.3.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/README.rst` & `joblib-1.3.1/doc/README.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/CHANGES.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/CHANGES.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/README.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/compressors_comparison.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/compressors_comparison.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/index.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/index.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/memory_basic_usage.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/memory_basic_usage.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/nested_parallel_memory.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/nested_parallel_memory.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel/distributed_backend_simple.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel/distributed_backend_simple.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel/index.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel/index.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel/sg_execution_times.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel/sg_execution_times.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel_generator.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel_generator.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel_memmap.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel_memmap.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/parallel_random_state.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/parallel_random_state.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/serialization_and_wrappers.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/serialization_and_wrappers.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/auto_examples/sg_execution_times.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/auto_examples/sg_execution_times.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/developing.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/developing.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/environment.pickle` & `joblib-1.3.1/doc/_build/html/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.Memory.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.Memory.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.Parallel.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.Parallel.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.dump.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.dump.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.hash.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.hash.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.load.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.load.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.parallel_config.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.parallel_config.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/generated/joblib.register_compressor.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/generated/joblib.register_compressor.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/index.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/installing.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/installing.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/memory.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/memory.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/parallel.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/parallel.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/parallel_numpy.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/parallel_numpy.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/persistence.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/persistence.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/.doctrees/why.doctree` & `joblib-1.3.1/doc/_build/html/.doctrees/why.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/CHANGES.html` & `joblib-1.3.1/doc/_build/html/CHANGES.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/README.html` & `joblib-1.3.1/doc/_build/html/README.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip` & `joblib-1.3.1/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/serialization_and_wrappers.py` & `joblib-1.3.1/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/serialization_and_wrappers.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/parallel_generator.py` & `joblib-1.3.1/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/parallel_generator.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/compressors_comparison.py` & `joblib-1.3.1/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/compressors_comparison.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/nested_parallel_memory.ipynb` & `joblib-1.3.1/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/nested_parallel_memory.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip` & `joblib-1.3.1/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/serialization_and_wrappers.ipynb` & `joblib-1.3.1/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/serialization_and_wrappers.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/parallel_random_state.ipynb` & `joblib-1.3.1/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/parallel_random_state.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/memory_basic_usage.ipynb` & `joblib-1.3.1/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/memory_basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/memory_basic_usage.py` & `joblib-1.3.1/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/memory_basic_usage.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/distributed_backend_simple.py` & `joblib-1.3.1/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/distributed_backend_simple.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/parallel_memmap.ipynb` & `joblib-1.3.1/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/parallel_memmap.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/nested_parallel_memory.py` & `joblib-1.3.1/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/nested_parallel_memory.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/parallel_generator.ipynb` & `joblib-1.3.1/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/parallel_generator.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/parallel_random_state.py` & `joblib-1.3.1/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/parallel_random_state.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/compressors_comparison.ipynb` & `joblib-1.3.1/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/compressors_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/parallel_memmap.py` & `joblib-1.3.1/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/parallel_memmap.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/distributed_backend_simple.ipynb` & `joblib-1.3.1/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/distributed_backend_simple.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_images/sphx_glr_compressors_comparison_001.png` & `joblib-1.3.1/doc/_build/html/_images/sphx_glr_compressors_comparison_001.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_images/sphx_glr_compressors_comparison_002.png` & `joblib-1.3.1/doc/_build/html/_images/sphx_glr_compressors_comparison_002.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_images/sphx_glr_compressors_comparison_thumb.png` & `joblib-1.3.1/doc/_build/html/_images/sphx_glr_compressors_comparison_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_images/sphx_glr_distributed_backend_simple_thumb.png` & `joblib-1.3.1/doc/_build/html/_images/sphx_glr_distributed_backend_simple_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_images/sphx_glr_memory_basic_usage_thumb.png` & `joblib-1.3.1/doc/_build/html/_images/sphx_glr_memory_basic_usage_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_images/sphx_glr_nested_parallel_memory_thumb.png` & `joblib-1.3.1/doc/_build/html/_images/sphx_glr_nested_parallel_memory_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_images/sphx_glr_parallel_generator_001.png` & `joblib-1.3.1/doc/_build/html/_images/sphx_glr_parallel_generator_001.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_images/sphx_glr_parallel_generator_thumb.png` & `joblib-1.3.1/doc/_build/html/_images/sphx_glr_parallel_generator_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_images/sphx_glr_parallel_memmap_thumb.png` & `joblib-1.3.1/doc/_build/html/_images/sphx_glr_parallel_memmap_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_images/sphx_glr_parallel_random_state_thumb.png` & `joblib-1.3.1/doc/_build/html/_images/sphx_glr_parallel_random_state_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_images/sphx_glr_serialization_and_wrappers_thumb.png` & `joblib-1.3.1/doc/_build/html/_images/sphx_glr_serialization_and_wrappers_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/CHANGES.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/CHANGES.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/README.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/README.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/compressors_comparison.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/compressors_comparison.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/index.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/index.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/memory_basic_usage.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/memory_basic_usage.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/nested_parallel_memory.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/nested_parallel_memory.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel/distributed_backend_simple.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel/distributed_backend_simple.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel/index.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel/index.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel/sg_execution_times.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel/sg_execution_times.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel_generator.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel_generator.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel_memmap.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel_memmap.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/parallel_random_state.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/parallel_random_state.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/serialization_and_wrappers.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/serialization_and_wrappers.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/auto_examples/sg_execution_times.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/auto_examples/sg_execution_times.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/index.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/installing.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/installing.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/memory.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/memory.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/parallel.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/parallel.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/parallel_numpy.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/parallel_numpy.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/persistence.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/persistence.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_sources/why.rst.txt` & `joblib-1.3.1/doc/_build/html/_sources/why.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/alabaster.css` & `joblib-1.3.1/doc/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/basic.css` & `joblib-1.3.1/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/binder_badge_logo.svg` & `joblib-1.3.1/doc/_build/html/_static/binder_badge_logo.svg`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/broken_example.png` & `joblib-1.3.1/doc/_build/html/_static/broken_example.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/custom.css` & `joblib-1.3.1/doc/_build/html/_static/custom.css`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/doctools.js` & `joblib-1.3.1/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/favicon.ico` & `joblib-1.3.1/doc/_build/html/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/joblib_logo.svg` & `joblib-1.3.1/doc/_build/html/_static/joblib_logo.svg`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/joblib_logo_examples.png` & `joblib-1.3.1/doc/_build/html/_static/joblib_logo_examples.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/jupyterlite_badge_logo.svg` & `joblib-1.3.1/doc/_build/html/_static/jupyterlite_badge_logo.svg`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/language_data.js` & `joblib-1.3.1/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/no_image.png` & `joblib-1.3.1/doc/_build/html/_static/no_image.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/pygments.css` & `joblib-1.3.1/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/searchtools.js` & `joblib-1.3.1/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/sg_gallery-dataframe.css` & `joblib-1.3.1/doc/_build/html/_static/sg_gallery-dataframe.css`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/sg_gallery-rendered-html.css` & `joblib-1.3.1/doc/_build/html/_static/sg_gallery-rendered-html.css`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/sg_gallery.css` & `joblib-1.3.1/doc/_build/html/_static/sg_gallery.css`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/_static/sphinx_highlight.js` & `joblib-1.3.1/doc/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/compressors_comparison.html` & `joblib-1.3.1/doc/_build/html/auto_examples/compressors_comparison.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/index.html` & `joblib-1.3.1/doc/_build/html/auto_examples/index.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/memory_basic_usage.html` & `joblib-1.3.1/doc/_build/html/auto_examples/memory_basic_usage.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/nested_parallel_memory.html` & `joblib-1.3.1/doc/_build/html/auto_examples/nested_parallel_memory.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/parallel/distributed_backend_simple.html` & `joblib-1.3.1/doc/_build/html/auto_examples/parallel/distributed_backend_simple.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/parallel/index.html` & `joblib-1.3.1/doc/_build/html/auto_examples/parallel/index.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/parallel/sg_execution_times.html` & `joblib-1.3.1/doc/_build/html/auto_examples/parallel/sg_execution_times.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/parallel_generator.html` & `joblib-1.3.1/doc/_build/html/auto_examples/parallel_generator.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/parallel_memmap.html` & `joblib-1.3.1/doc/_build/html/auto_examples/parallel_memmap.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/parallel_random_state.html` & `joblib-1.3.1/doc/_build/html/auto_examples/parallel_random_state.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/serialization_and_wrappers.html` & `joblib-1.3.1/doc/_build/html/auto_examples/serialization_and_wrappers.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/auto_examples/sg_execution_times.html` & `joblib-1.3.1/doc/_build/html/auto_examples/sg_execution_times.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/developing.html` & `joblib-1.3.1/doc/_build/html/developing.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/generated/joblib.Memory.html` & `joblib-1.3.1/doc/_build/html/generated/joblib.Memory.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/generated/joblib.Parallel.html` & `joblib-1.3.1/doc/_build/html/generated/joblib.Parallel.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/generated/joblib.dump.html` & `joblib-1.3.1/doc/_build/html/generated/joblib.dump.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/generated/joblib.hash.html` & `joblib-1.3.1/doc/_build/html/generated/joblib.hash.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/generated/joblib.load.html` & `joblib-1.3.1/doc/_build/html/generated/joblib.load.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/generated/joblib.parallel_config.html` & `joblib-1.3.1/doc/_build/html/generated/joblib.parallel_config.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/generated/joblib.register_compressor.html` & `joblib-1.3.1/doc/_build/html/generated/joblib.register_compressor.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/genindex.html` & `joblib-1.3.1/doc/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/index.html` & `joblib-1.3.1/doc/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/installing.html` & `joblib-1.3.1/doc/_build/html/installing.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/memory.html` & `joblib-1.3.1/doc/_build/html/memory.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/objects.inv` & `joblib-1.3.1/doc/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/parallel.html` & `joblib-1.3.1/doc/_build/html/parallel.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/parallel_numpy.html` & `joblib-1.3.1/doc/_build/html/parallel_numpy.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/persistence.html` & `joblib-1.3.1/doc/_build/html/persistence.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/py-modindex.html` & `joblib-1.3.1/doc/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/search.html` & `joblib-1.3.1/doc/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/searchindex.js` & `joblib-1.3.1/doc/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_build/html/why.html` & `joblib-1.3.1/doc/_build/html/why.html`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_static/custom.css` & `joblib-1.3.1/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_static/favicon.ico` & `joblib-1.3.1/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_static/joblib_logo.svg` & `joblib-1.3.1/doc/_static/joblib_logo.svg`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/_static/joblib_logo_examples.png` & `joblib-1.3.1/doc/_static/joblib_logo_examples.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/auto_examples_jupyter.zip` & `joblib-1.3.1/doc/auto_examples/auto_examples_jupyter.zip`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/auto_examples_python.zip` & `joblib-1.3.1/doc/auto_examples/auto_examples_python.zip`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/compressors_comparison.ipynb` & `joblib-1.3.1/doc/auto_examples/compressors_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/compressors_comparison.py` & `joblib-1.3.1/doc/auto_examples/compressors_comparison.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/compressors_comparison.rst` & `joblib-1.3.1/doc/auto_examples/compressors_comparison.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/compressors_comparison_codeobj.pickle` & `joblib-1.3.1/doc/auto_examples/compressors_comparison_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/images/sphx_glr_compressors_comparison_001.png` & `joblib-1.3.1/doc/auto_examples/images/sphx_glr_compressors_comparison_001.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/images/sphx_glr_compressors_comparison_002.png` & `joblib-1.3.1/doc/auto_examples/images/sphx_glr_compressors_comparison_002.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/images/sphx_glr_parallel_generator_001.png` & `joblib-1.3.1/doc/auto_examples/images/sphx_glr_parallel_generator_001.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_compressors_comparison_thumb.png` & `joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_compressors_comparison_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_memory_basic_usage_thumb.png` & `joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_memory_basic_usage_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_nested_parallel_memory_thumb.png` & `joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_nested_parallel_memory_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_parallel_generator_thumb.png` & `joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_parallel_generator_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_parallel_memmap_thumb.png` & `joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_parallel_memmap_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_parallel_random_state_thumb.png` & `joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_parallel_random_state_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/images/thumb/sphx_glr_serialization_and_wrappers_thumb.png` & `joblib-1.3.1/doc/auto_examples/images/thumb/sphx_glr_serialization_and_wrappers_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/index.rst` & `joblib-1.3.1/doc/auto_examples/index.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/memory_basic_usage.ipynb` & `joblib-1.3.1/doc/auto_examples/memory_basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/memory_basic_usage.py` & `joblib-1.3.1/doc/auto_examples/memory_basic_usage.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/memory_basic_usage.rst` & `joblib-1.3.1/doc/auto_examples/memory_basic_usage.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/memory_basic_usage_codeobj.pickle` & `joblib-1.3.1/doc/auto_examples/memory_basic_usage_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/nested_parallel_memory.ipynb` & `joblib-1.3.1/doc/auto_examples/nested_parallel_memory.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/nested_parallel_memory.py` & `joblib-1.3.1/doc/auto_examples/nested_parallel_memory.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/nested_parallel_memory.rst` & `joblib-1.3.1/doc/auto_examples/nested_parallel_memory.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/nested_parallel_memory_codeobj.pickle` & `joblib-1.3.1/doc/auto_examples/nested_parallel_memory_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel/distributed_backend_simple.ipynb` & `joblib-1.3.1/doc/auto_examples/parallel/distributed_backend_simple.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel/distributed_backend_simple.py` & `joblib-1.3.1/doc/auto_examples/parallel/distributed_backend_simple.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel/distributed_backend_simple.rst` & `joblib-1.3.1/doc/auto_examples/parallel/distributed_backend_simple.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel/distributed_backend_simple_codeobj.pickle` & `joblib-1.3.1/doc/auto_examples/parallel/distributed_backend_simple_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel/images/thumb/sphx_glr_distributed_backend_simple_thumb.png` & `joblib-1.3.1/doc/auto_examples/parallel/images/thumb/sphx_glr_distributed_backend_simple_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel/index.rst` & `joblib-1.3.1/doc/auto_examples/parallel/index.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel/sg_execution_times.rst` & `joblib-1.3.1/doc/auto_examples/parallel/sg_execution_times.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_generator.ipynb` & `joblib-1.3.1/doc/auto_examples/parallel_generator.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_generator.py` & `joblib-1.3.1/doc/auto_examples/parallel_generator.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_generator.rst` & `joblib-1.3.1/doc/auto_examples/parallel_generator.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_generator_codeobj.pickle` & `joblib-1.3.1/doc/auto_examples/parallel_generator_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_memmap.ipynb` & `joblib-1.3.1/doc/auto_examples/parallel_memmap.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_memmap.py` & `joblib-1.3.1/doc/auto_examples/parallel_memmap.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_memmap.rst` & `joblib-1.3.1/doc/auto_examples/parallel_memmap.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_memmap_codeobj.pickle` & `joblib-1.3.1/doc/auto_examples/parallel_memmap_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_random_state.ipynb` & `joblib-1.3.1/doc/auto_examples/parallel_random_state.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_random_state.py` & `joblib-1.3.1/doc/auto_examples/parallel_random_state.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_random_state.rst` & `joblib-1.3.1/doc/auto_examples/parallel_random_state.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/parallel_random_state_codeobj.pickle` & `joblib-1.3.1/doc/auto_examples/parallel_random_state_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/searchindex.dat` & `joblib-1.3.1/doc/auto_examples/searchindex.dat`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/serialization_and_wrappers.ipynb` & `joblib-1.3.1/doc/auto_examples/serialization_and_wrappers.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/serialization_and_wrappers.py` & `joblib-1.3.1/doc/auto_examples/serialization_and_wrappers.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/serialization_and_wrappers.rst` & `joblib-1.3.1/doc/auto_examples/serialization_and_wrappers.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/serialization_and_wrappers_codeobj.pickle` & `joblib-1.3.1/doc/auto_examples/serialization_and_wrappers_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/auto_examples/sg_execution_times.rst` & `joblib-1.3.1/doc/auto_examples/sg_execution_times.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/conf.py` & `joblib-1.3.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/conftest.py` & `joblib-1.3.1/doc/conftest.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.Logger.cache.examples` & `joblib-1.3.1/doc/generated/joblib.Logger.cache.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.Logger.clear.examples` & `joblib-1.3.1/doc/generated/joblib.Logger.clear.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.Logger.examples` & `joblib-1.3.1/doc/generated/joblib.Logger.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.MemorizedFunc.examples` & `joblib-1.3.1/doc/generated/joblib.MemorizedFunc.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.Memory.cache.examples` & `joblib-1.3.1/doc/generated/joblib.Memory.cache.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.Memory.clear.examples` & `joblib-1.3.1/doc/generated/joblib.Memory.clear.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.Memory.examples` & `joblib-1.3.1/doc/generated/joblib.Memory.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.Parallel.examples` & `joblib-1.3.1/doc/generated/joblib.Parallel.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.delayed.examples` & `joblib-1.3.1/doc/generated/joblib.delayed.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.dump.examples` & `joblib-1.3.1/doc/generated/joblib.dump.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.externals.loky.set_loky_pickler.examples` & `joblib-1.3.1/doc/generated/joblib.externals.loky.set_loky_pickler.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.load.examples` & `joblib-1.3.1/doc/generated/joblib.load.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.logger.Logger.cache.examples` & `joblib-1.3.1/doc/generated/joblib.logger.Logger.cache.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.logger.Logger.clear.examples` & `joblib-1.3.1/doc/generated/joblib.logger.Logger.clear.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.memory.MemorizedFunc.examples` & `joblib-1.3.1/doc/generated/joblib.memory.MemorizedFunc.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.parallel_config.examples` & `joblib-1.3.1/doc/generated/joblib.parallel_config.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/generated/joblib.wrap_non_picklable_objects.examples` & `joblib-1.3.1/doc/generated/joblib.wrap_non_picklable_objects.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/index.rst` & `joblib-1.3.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/installing.rst` & `joblib-1.3.1/doc/installing.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/memory.rst` & `joblib-1.3.1/doc/memory.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/parallel.rst` & `joblib-1.3.1/doc/parallel.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/parallel_numpy.rst` & `joblib-1.3.1/doc/parallel_numpy.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/persistence.rst` & `joblib-1.3.1/doc/persistence.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/doc/why.rst` & `joblib-1.3.1/doc/why.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/__init__.py` & `joblib-1.3.1/joblib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 
 
 import os
 
 from .memory import Memory
 from .memory import MemorizedResult
 from .memory import register_store_backend
```

### Comparing `joblib-1.3.0/joblib/_dask.py` & `joblib-1.3.1/joblib/_dask.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/_memmapping_reducer.py` & `joblib-1.3.1/joblib/_memmapping_reducer.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/_multiprocessing_helpers.py` & `joblib-1.3.1/joblib/_multiprocessing_helpers.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/_parallel_backends.py` & `joblib-1.3.1/joblib/_parallel_backends.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/_store_backends.py` & `joblib-1.3.1/joblib/_store_backends.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/_utils.py` & `joblib-1.3.1/joblib/_utils.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/backports.py` & `joblib-1.3.1/joblib/backports.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/compressor.py` & `joblib-1.3.1/joblib/compressor.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/disk.py` & `joblib-1.3.1/joblib/disk.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/executor.py` & `joblib-1.3.1/joblib/executor.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/cloudpickle/cloudpickle.py` & `joblib-1.3.1/joblib/externals/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/cloudpickle/cloudpickle_fast.py` & `joblib-1.3.1/joblib/externals/cloudpickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/__init__.py` & `joblib-1.3.1/joblib/externals/loky/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,8 @@
     "FIRST_EXCEPTION",
     "ALL_COMPLETED",
     "wrap_non_picklable_objects",
     "set_loky_pickler",
 ]
 
 
-__version__ = "3.4.0"
+__version__ = "3.4.1"
```

### Comparing `joblib-1.3.0/joblib/externals/loky/_base.py` & `joblib-1.3.1/joblib/externals/loky/_base.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/_posix_reduction.py` & `joblib-1.3.1/joblib/externals/loky/backend/_posix_reduction.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/_win_reduction.py` & `joblib-1.3.1/joblib/externals/loky/backend/_win_reduction.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/context.py` & `joblib-1.3.1/joblib/externals/loky/backend/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,28 @@
 import math
 import subprocess
 import traceback
 import warnings
 import multiprocessing as mp
 from multiprocessing import get_context as mp_get_context
 from multiprocessing.context import BaseContext
-from concurrent.futures.process import _MAX_WINDOWS_WORKERS
+
 
 from .process import LokyProcess, LokyInitMainProcess
 
 # Apparently, on older Python versions, loky cannot work 61 workers on Windows
 # but instead 60: ¯\_(ツ)_/¯
-if sys.version_info < (3, 10):
-    _MAX_WINDOWS_WORKERS = _MAX_WINDOWS_WORKERS - 1
+if sys.version_info >= (3, 8):
+    from concurrent.futures.process import _MAX_WINDOWS_WORKERS
+
+    if sys.version_info < (3, 10):
+        _MAX_WINDOWS_WORKERS = _MAX_WINDOWS_WORKERS - 1
+else:
+    # compat for versions before 3.8 which do not define this.
+    _MAX_WINDOWS_WORKERS = 60
 
 START_METHODS = ["loky", "loky_init_main", "spawn"]
 if sys.platform != "win32":
     START_METHODS += ["fork", "forkserver"]
 
 _DEFAULT_START_METHOD = None
```

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/fork_exec.py` & `joblib-1.3.1/joblib/externals/loky/backend/fork_exec.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/popen_loky_posix.py` & `joblib-1.3.1/joblib/externals/loky/backend/popen_loky_posix.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/popen_loky_win32.py` & `joblib-1.3.1/joblib/externals/loky/backend/popen_loky_win32.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/process.py` & `joblib-1.3.1/joblib/externals/loky/backend/process.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/queues.py` & `joblib-1.3.1/joblib/externals/loky/backend/queues.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/reduction.py` & `joblib-1.3.1/joblib/externals/loky/backend/reduction.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/resource_tracker.py` & `joblib-1.3.1/joblib/externals/loky/backend/resource_tracker.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/spawn.py` & `joblib-1.3.1/joblib/externals/loky/backend/spawn.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/synchronize.py` & `joblib-1.3.1/joblib/externals/loky/backend/synchronize.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/backend/utils.py` & `joblib-1.3.1/joblib/externals/loky/backend/utils.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/cloudpickle_wrapper.py` & `joblib-1.3.1/joblib/externals/loky/cloudpickle_wrapper.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/initializers.py` & `joblib-1.3.1/joblib/externals/loky/initializers.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/process_executor.py` & `joblib-1.3.1/joblib/externals/loky/process_executor.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/externals/loky/reusable_executor.py` & `joblib-1.3.1/joblib/externals/loky/reusable_executor.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/func_inspect.py` & `joblib-1.3.1/joblib/func_inspect.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/hashing.py` & `joblib-1.3.1/joblib/hashing.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/logger.py` & `joblib-1.3.1/joblib/logger.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/memory.py` & `joblib-1.3.1/joblib/memory.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/numpy_pickle.py` & `joblib-1.3.1/joblib/numpy_pickle.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/numpy_pickle_compat.py` & `joblib-1.3.1/joblib/numpy_pickle_compat.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/numpy_pickle_utils.py` & `joblib-1.3.1/joblib/numpy_pickle_utils.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/parallel.py` & `joblib-1.3.1/joblib/parallel.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/pool.py` & `joblib-1.3.1/joblib/pool.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/_openmp_test_helper/setup.py` & `joblib-1.3.1/joblib/test/_openmp_test_helper/setup.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/common.py` & `joblib-1.3.1/joblib/test/common.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/create_numpy_pickle.py` & `joblib-1.3.1/joblib/test/data/create_numpy_pickle.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np16.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np16.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np17.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np17.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py33_np18.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_compressed_pickle_py33_np18.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py34_np19.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_compressed_pickle_py34_np19.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py35_np19.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_compressed_pickle_py35_np19.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.bz2` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.bz2`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.gzip` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.gzip`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.lzma` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.lzma`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.xz` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.xz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.bz2` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.bz2`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.gzip` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.gzip`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.lzma` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.lzma`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.xz` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.xz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.bz2` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.bz2`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.gzip` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.gzip`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.lzma` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.lzma`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.xz` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.xz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.bz2` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.bz2`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.gzip` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.gzip`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.lzma` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.lzma`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.xz` & `joblib-1.3.1/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.xz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.11.0_compressed_pickle_py36_np111.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.11.0_compressed_pickle_py36_np111.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl` & `joblib-1.3.1/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.bz2` & `joblib-1.3.1/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.bz2`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.gzip` & `joblib-1.3.1/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.gzip`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.lzma` & `joblib-1.3.1/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.lzma`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.xz` & `joblib-1.3.1/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.xz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.8.4_compressed_pickle_py27_np17.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.8.4_compressed_pickle_py27_np17.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np16.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np16.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np17.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np17.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py34_np19.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.9.2_compressed_pickle_py34_np19.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py35_np19.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.9.2_compressed_pickle_py35_np19.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl` & `joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl` & `joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl` & `joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl` & `joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl` & `joblib-1.3.1/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz` & `joblib-1.3.1/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_backports.py` & `joblib-1.3.1/joblib/test/test_backports.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_cloudpickle_wrapper.py` & `joblib-1.3.1/joblib/test/test_cloudpickle_wrapper.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_config.py` & `joblib-1.3.1/joblib/test/test_config.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_dask.py` & `joblib-1.3.1/joblib/test/test_dask.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_disk.py` & `joblib-1.3.1/joblib/test/test_disk.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_func_inspect.py` & `joblib-1.3.1/joblib/test/test_func_inspect.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_hashing.py` & `joblib-1.3.1/joblib/test/test_hashing.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_logger.py` & `joblib-1.3.1/joblib/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_memmapping.py` & `joblib-1.3.1/joblib/test/test_memmapping.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_memory.py` & `joblib-1.3.1/joblib/test/test_memory.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_missing_multiprocessing.py` & `joblib-1.3.1/joblib/test/test_missing_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_module.py` & `joblib-1.3.1/joblib/test/test_module.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_numpy_pickle.py` & `joblib-1.3.1/joblib/test/test_numpy_pickle.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_numpy_pickle_compat.py` & `joblib-1.3.1/joblib/test/test_numpy_pickle_compat.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_parallel.py` & `joblib-1.3.1/joblib/test/test_parallel.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_store_backends.py` & `joblib-1.3.1/joblib/test/test_store_backends.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_testing.py` & `joblib-1.3.1/joblib/test/test_testing.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/test/test_utils.py` & `joblib-1.3.1/joblib/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib/testing.py` & `joblib-1.3.1/joblib/testing.py`

 * *Files identical despite different names*

### Comparing `joblib-1.3.0/joblib.egg-info/PKG-INFO` & `joblib-1.3.1/joblib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joblib
-Version: 1.3.0
+Version: 1.3.1
 Summary: Lightweight pipelining with Python functions
 Author-email: Gael Varoquaux <gael.varoquaux@normalesup.org>
 License: BSD 3-Clause
 Project-URL: Homepage, https://joblib.readthedocs.io
 Project-URL: Source, https://github.com/joblib/joblib
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `joblib-1.3.0/joblib.egg-info/SOURCES.txt` & `joblib-1.3.1/joblib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .readthedocs-requirements.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
 conftest.py
 pyproject.toml
+setup.cfg
 setup.py
 doc/CHANGES.rst
 doc/Makefile
 doc/README.rst
 doc/__init__.py
 doc/conf.py
 doc/conftest.py
```

### Comparing `joblib-1.3.0/pyproject.toml` & `joblib-1.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = ["setuptools>=61.2"]
-build-backend = "setuptools.build_meta:__legacy__"
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "joblib"
 authors = [{name = "Gael Varoquaux", email = "gael.varoquaux@normalesup.org"}]
 license = {text = "BSD 3-Clause"}
 description = "Lightweight pipelining with Python functions"
 classifiers = [
```

