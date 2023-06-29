# Comparing `tmp/prog_models-1.5.0rc1.tar.gz` & `tmp/prog_models-1.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prog_models-1.5.0rc1.tar", last modified: Wed Jun 28 22:38:12 2023, max compression
+gzip compressed data, was "prog_models-1.5.0rc2.tar", last modified: Wed Jun 28 22:53:02 2023, max compression
```

## Comparing `prog_models-1.5.0rc1.tar` & `prog_models-1.5.0rc2.tar`

### file list

```diff
@@ -1,170 +1,179 @@
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.120525 prog_models-1.5.0rc1/
--rw-r--r--   0 cteubert   (507) staff       (20)     1295 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/.gitignore
--rw-r--r--   0 cteubert   (507) staff       (20)     7016 2023-06-28 22:38:12.120254 prog_models-1.5.0rc1/PKG-INFO
--rw-r--r--   0 cteubert   (507) staff       (20)     5153 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/README.md
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.096255 prog_models-1.5.0rc1/docs/
--rw-r--r--   0 cteubert   (507) staff       (20)      230 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/.buildinfo
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.098152 prog_models-1.5.0rc1/docs/.doctrees/
--rw-r--r--   0 cteubert   (507) staff       (20)    96339 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/.doctrees/deriv_prog_model.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     2831 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/.doctrees/dev_guide.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)    18573 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/.doctrees/environment.pickle
--rw-r--r--   0 cteubert   (507) staff       (20)    12051 2023-06-20 18:40:01.000000 prog_models-1.5.0rc1/docs/.doctrees/exceptions.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     2775 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/.doctrees/getting_started.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     2837 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/.doctrees/index.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     2730 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/.doctrees/models.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     2785 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/.doctrees/prognostics_model.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)   102536 2023-06-20 18:40:01.000000 prog_models-1.5.0rc1/docs/.doctrees/visualize.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     5271 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/7150.md
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.099884 prog_models-1.5.0rc1/docs/_sources/
--rw-r--r--   0 cteubert   (507) staff       (20)      160 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_sources/deriv_prog_model.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)      119 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/_sources/dev_guide.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)      608 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_sources/exceptions.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)       86 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/_sources/getting_started.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)      150 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/_sources/index.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)      123 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/_sources/models.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)       96 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/_sources/prognostics_model.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)      179 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_sources/visualize.rst.txt
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.103907 prog_models-1.5.0rc1/docs/_static/
--rw-r--r--   0 cteubert   (507) staff       (20)    11185 2022-08-23 14:28:13.000000 prog_models-1.5.0rc1/docs/_static/alabaster.css
--rw-r--r--   0 cteubert   (507) staff       (20)    14692 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/_static/basic.css
--rw-r--r--   0 cteubert   (507) staff       (20)     4534 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_static/classic.css
--rw-r--r--   0 cteubert   (507) staff       (20)       42 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_static/custom.css
--rw-r--r--   0 cteubert   (507) staff       (20)    10766 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/_static/doctools.js
--rw-r--r--   0 cteubert   (507) staff       (20)      422 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/_static/documentation_options.js
--rw-r--r--   0 cteubert   (507) staff       (20)      286 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_static/file.png
--rw-r--r--   0 cteubert   (507) staff       (20)   287630 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_static/jquery-3.5.1.js
--rw-r--r--   0 cteubert   (507) staff       (20)    89476 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_static/jquery.js
--rw-r--r--   0 cteubert   (507) staff       (20)    10854 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/_static/language_data.js
--rw-r--r--   0 cteubert   (507) staff       (20)       90 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_static/minus.png
--rw-r--r--   0 cteubert   (507) staff       (20)       90 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_static/plus.png
--rw-r--r--   0 cteubert   (507) staff       (20)     5249 2022-08-23 14:28:13.000000 prog_models-1.5.0rc1/docs/_static/pygments.css
--rw-r--r--   0 cteubert   (507) staff       (20)    16634 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/_static/searchtools.js
--rw-r--r--   0 cteubert   (507) staff       (20)     4803 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_static/sidebar.js
--rw-r--r--   0 cteubert   (507) staff       (20)    67692 2021-05-10 16:37:43.000000 prog_models-1.5.0rc1/docs/_static/underscore-1.12.0.js
--rw-r--r--   0 cteubert   (507) staff       (20)    35168 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/_static/underscore-1.3.1.js
--rw-r--r--   0 cteubert   (507) staff       (20)    19530 2023-06-20 18:40:01.000000 prog_models-1.5.0rc1/docs/_static/underscore.js
--rw-r--r--   0 cteubert   (507) staff       (20)    27376 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/deriv_prog_model.html
--rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/dev_guide.html
--rw-r--r--   0 cteubert   (507) staff       (20)     7442 2023-06-20 18:44:15.000000 prog_models-1.5.0rc1/docs/exceptions.html
--rw-r--r--   0 cteubert   (507) staff       (20)     2295 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/genindex.html
--rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/getting_started.html
--rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/index.html
--rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/models.html
--rw-r--r--   0 cteubert   (507) staff       (20)      443 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/objects.inv
--rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/prognostics_model.html
--rw-r--r--   0 cteubert   (507) staff       (20)     8365 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/py-modindex.html
--rw-r--r--   0 cteubert   (507) staff       (20)     2608 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/search.html
--rw-r--r--   0 cteubert   (507) staff       (20)     1275 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/docs/searchindex.js
--rw-r--r--   0 cteubert   (507) staff       (20)      961 2021-03-10 17:51:45.000000 prog_models-1.5.0rc1/docs/softwareplan.md
--rw-r--r--   0 cteubert   (507) staff       (20)    31639 2023-06-20 18:42:18.000000 prog_models-1.5.0rc1/docs/visualize.html
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.104941 prog_models-1.5.0rc1/examples/
--rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/examples/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)      939 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/examples/benchmarking.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6312 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/examples/future_loading.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4767 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/examples/new_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4949 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/examples/noise.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2433 2023-06-20 18:45:28.000000 prog_models-1.5.0rc1/examples/sensitivity.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3608 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/examples/sim.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.105373 prog_models-1.5.0rc1/forms/
--rw-r--r--   0 cteubert   (507) staff       (20)   219343 2023-06-20 18:42:18.000000 prog_models-1.5.0rc1/forms/Corporate CLA.pdf
--rw-r--r--   0 cteubert   (507) staff       (20)   153485 2023-06-20 18:42:18.000000 prog_models-1.5.0rc1/forms/Individual CLA.pdf
--rw-r--r--   0 cteubert   (507) staff       (20)    94594 2021-05-10 16:37:43.000000 prog_models-1.5.0rc1/license.pdf
--rw-r--r--   0 cteubert   (507) staff       (20)    13424 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/prog_model_template.py
--rw-r--r--   0 cteubert   (507) staff       (20)       38 2023-06-28 22:38:12.120586 prog_models-1.5.0rc1/setup.cfg
--rw-r--r--   0 cteubert   (507) staff       (20)     2932 2023-06-28 22:37:55.000000 prog_models-1.5.0rc1/setup.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.091951 prog_models-1.5.0rc1/src/
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.106630 prog_models-1.5.0rc1/src/prog_models/
--rw-r--r--   0 cteubert   (507) staff       (20)      468 2023-06-28 22:37:45.000000 prog_models-1.5.0rc1/src/prog_models/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    12776 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/composite_model.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.108319 prog_models-1.5.0rc1/src/prog_models/data_models/
--rw-r--r--   0 cteubert   (507) staff       (20)      476 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/data_models/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8208 2023-06-28 14:47:51.000000 prog_models-1.5.0rc1/src/prog_models/data_models/data_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)    22276 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/data_models/dmd.py
--rw-r--r--   0 cteubert   (507) staff       (20)    35164 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/data_models/lstm_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8465 2023-06-28 21:50:30.000000 prog_models-1.5.0rc1/src/prog_models/data_models/pce.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.109509 prog_models-1.5.0rc1/src/prog_models/datasets/
--rw-r--r--   0 cteubert   (507) staff       (20)      157 2023-06-20 18:44:15.000000 prog_models-1.5.0rc1/src/prog_models/datasets/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6185 2023-06-22 23:28:06.000000 prog_models-1.5.0rc1/src/prog_models/datasets/nasa_battery.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6170 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/datasets/nasa_cmapss.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5558 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/ensemble_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)      543 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/exceptions.py
--rw-r--r--   0 cteubert   (507) staff       (20)     9133 2023-06-28 21:50:30.000000 prog_models-1.5.0rc1/src/prog_models/linear_model.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.110271 prog_models-1.5.0rc1/src/prog_models/loading/
--rw-r--r--   0 cteubert   (507) staff       (20)      347 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/loading/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    15484 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/loading/controllers.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1495 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/loading/gaussian_wrapper.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2102 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/loading/moving_average.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1772 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/loading/piecewise.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.111727 prog_models-1.5.0rc1/src/prog_models/models/
--rw-r--r--   0 cteubert   (507) staff       (20)      918 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/models/__init__.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.112110 prog_models-1.5.0rc1/src/prog_models/models/aircraft_model/
--rw-r--r--   0 cteubert   (507) staff       (20)      242 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/models/aircraft_model/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)      335 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/aircraft_model/aircraft.py
--rw-r--r--   0 cteubert   (507) staff       (20)    19213 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/aircraft_model/small_rotorcraft.py
--rw-r--r--   0 cteubert   (507) staff       (20)     7882 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/battery_circuit.py
--rw-r--r--   0 cteubert   (507) staff       (20)    32566 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/battery_electrochem.py
--rw-r--r--   0 cteubert   (507) staff       (20)    12741 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/centrifugal_pump.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6530 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/dcmotor.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5649 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/dcmotor_singlephase.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4653 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/esc.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.112384 prog_models-1.5.0rc1/src/prog_models/models/experimental/
--rw-r--r--   0 cteubert   (507) staff       (20)      158 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/models/experimental/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2949 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/experimental/paris_law.py
--rw-r--r--   0 cteubert   (507) staff       (20)    17214 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/pneumatic_valve.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6555 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/powertrain.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1428 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/propeller_load.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.112775 prog_models-1.5.0rc1/src/prog_models/models/test_models/
--rw-r--r--   0 cteubert   (507) staff       (20)      249 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/models/test_models/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4384 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/models/test_models/linear_models.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4050 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/test_models/linear_thrown_object.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5714 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/models/thrown_object.py
--rw-r--r--   0 cteubert   (507) staff       (20)    68508 2023-06-28 21:35:58.000000 prog_models-1.5.0rc1/src/prog_models/prognostics_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)    17091 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/sim_result.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.114441 prog_models-1.5.0rc1/src/prog_models/utils/
--rw-r--r--   0 cteubert   (507) staff       (20)      198 2023-06-20 18:44:15.000000 prog_models-1.5.0rc1/src/prog_models/utils/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    21583 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/utils/calc_error.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8984 2023-06-28 18:01:11.000000 prog_models-1.5.0rc1/src/prog_models/utils/containers.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1014 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/utils/input_validation.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4382 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/utils/next_state.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2242 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/utils/noise_functions.py
--rw-r--r--   0 cteubert   (507) staff       (20)    10374 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/utils/parameters.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1173 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/utils/progress_bar.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1859 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/utils/serialization.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2484 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/utils/size.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.114975 prog_models-1.5.0rc1/src/prog_models/utils/traj_gen/
--rw-r--r--   0 cteubert   (507) staff       (20)      221 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/src/prog_models/utils/traj_gen/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    24434 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/utils/traj_gen/geometry.py
--rw-r--r--   0 cteubert   (507) staff       (20)    16044 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/utils/traj_gen/nurbs.py
--rw-r--r--   0 cteubert   (507) staff       (20)    33968 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/src/prog_models/utils/traj_gen/trajectory.py
--rw-r--r--   0 cteubert   (507) staff       (20)    27416 2023-06-28 18:01:29.000000 prog_models-1.5.0rc1/src/prog_models/visualize.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.107276 prog_models-1.5.0rc1/src/prog_models.egg-info/
--rw-------   0 cteubert   (507) staff       (20)     7016 2023-06-28 22:38:12.000000 prog_models-1.5.0rc1/src/prog_models.egg-info/PKG-INFO
--rw-------   0 cteubert   (507) staff       (20)     4592 2023-06-28 22:38:12.000000 prog_models-1.5.0rc1/src/prog_models.egg-info/SOURCES.txt
--rw-------   0 cteubert   (507) staff       (20)        1 2023-06-28 22:38:12.000000 prog_models-1.5.0rc1/src/prog_models.egg-info/dependency_links.txt
--rw-------   0 cteubert   (507) staff       (20)      204 2023-06-28 22:38:12.000000 prog_models-1.5.0rc1/src/prog_models.egg-info/requires.txt
--rw-------   0 cteubert   (507) staff       (20)       12 2023-06-28 22:38:12.000000 prog_models-1.5.0rc1/src/prog_models.egg-info/top_level.txt
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:38:12.119752 prog_models-1.5.0rc1/tests/
--rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/tests/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3309 2023-06-20 20:08:13.000000 prog_models-1.5.0rc1/tests/__main__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    56896 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_base_models.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2652 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_battery.py
--rw-r--r--   0 cteubert   (507) staff       (20)    18087 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_calc_error.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8122 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_centrifugal_pump.py
--rw-r--r--   0 cteubert   (507) staff       (20)    14085 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_composite.py
--rw-r--r--   0 cteubert   (507) staff       (20)    13250 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_data_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1872 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_datasets.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4177 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_dict_like_matrix_wrapper.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4622 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_direct.py
--rw-r--r--   0 cteubert   (507) staff       (20)     7537 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_ensemble.py
--rw-r--r--   0 cteubert   (507) staff       (20)    55549 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_estimate_params.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1627 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_examples.py
--rw-r--r--   0 cteubert   (507) staff       (20)    18578 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_linear_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6686 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_manual.py
--rw-r--r--   0 cteubert   (507) staff       (20)    12907 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_pneumatic_valve.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2435 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_powertrain.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4267 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_serialization.py
--rw-r--r--   0 cteubert   (507) staff       (20)    35373 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_sim_result.py
--rw-r--r--   0 cteubert   (507) staff       (20)    32855 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_surrogates.py
--rw-r--r--   0 cteubert   (507) staff       (20)      918 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_tutorials.py
--rw-r--r--   0 cteubert   (507) staff       (20)    15470 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tests/test_uav_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)    47927 2023-06-28 14:48:00.000000 prog_models-1.5.0rc1/tutorial.ipynb
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.601831 prog_models-1.5.0rc2/
+-rw-r--r--   0 cteubert   (507) staff       (20)     1295 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/.gitignore
+-rw-r--r--   0 cteubert   (507) staff       (20)     7016 2023-06-28 22:53:02.601661 prog_models-1.5.0rc2/PKG-INFO
+-rw-r--r--   0 cteubert   (507) staff       (20)     5153 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/README.md
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.573172 prog_models-1.5.0rc2/docs/
+-rw-r--r--   0 cteubert   (507) staff       (20)      230 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.buildinfo
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.574539 prog_models-1.5.0rc2/docs/.doctrees/
+-rw-r--r--   0 cteubert   (507) staff       (20)    96339 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/.doctrees/deriv_prog_model.doctree
+-rw-r--r--   0 cteubert   (507) staff       (20)     2831 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/dev_guide.doctree
+-rw-r--r--   0 cteubert   (507) staff       (20)    18573 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/environment.pickle
+-rw-r--r--   0 cteubert   (507) staff       (20)    12051 2023-06-20 18:40:01.000000 prog_models-1.5.0rc2/docs/.doctrees/exceptions.doctree
+-rw-r--r--   0 cteubert   (507) staff       (20)     2775 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/getting_started.doctree
+-rw-r--r--   0 cteubert   (507) staff       (20)     2837 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/index.doctree
+-rw-r--r--   0 cteubert   (507) staff       (20)     2730 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/models.doctree
+-rw-r--r--   0 cteubert   (507) staff       (20)     2785 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/prognostics_model.doctree
+-rw-r--r--   0 cteubert   (507) staff       (20)   102536 2023-06-20 18:40:01.000000 prog_models-1.5.0rc2/docs/.doctrees/visualize.doctree
+-rw-r--r--   0 cteubert   (507) staff       (20)     5271 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/7150.md
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.575595 prog_models-1.5.0rc2/docs/_sources/
+-rw-r--r--   0 cteubert   (507) staff       (20)      160 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_sources/deriv_prog_model.rst.txt
+-rw-r--r--   0 cteubert   (507) staff       (20)      119 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_sources/dev_guide.rst.txt
+-rw-r--r--   0 cteubert   (507) staff       (20)      608 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_sources/exceptions.rst.txt
+-rw-r--r--   0 cteubert   (507) staff       (20)       86 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_sources/getting_started.rst.txt
+-rw-r--r--   0 cteubert   (507) staff       (20)      150 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_sources/index.rst.txt
+-rw-r--r--   0 cteubert   (507) staff       (20)      123 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_sources/models.rst.txt
+-rw-r--r--   0 cteubert   (507) staff       (20)       96 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_sources/prognostics_model.rst.txt
+-rw-r--r--   0 cteubert   (507) staff       (20)      179 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_sources/visualize.rst.txt
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.582662 prog_models-1.5.0rc2/docs/_static/
+-rw-r--r--   0 cteubert   (507) staff       (20)    11185 2022-08-23 14:28:13.000000 prog_models-1.5.0rc2/docs/_static/alabaster.css
+-rw-r--r--   0 cteubert   (507) staff       (20)    14692 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_static/basic.css
+-rw-r--r--   0 cteubert   (507) staff       (20)     4534 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/classic.css
+-rw-r--r--   0 cteubert   (507) staff       (20)       42 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/custom.css
+-rw-r--r--   0 cteubert   (507) staff       (20)    10766 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_static/doctools.js
+-rw-r--r--   0 cteubert   (507) staff       (20)      422 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_static/documentation_options.js
+-rw-r--r--   0 cteubert   (507) staff       (20)      286 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/file.png
+-rw-r--r--   0 cteubert   (507) staff       (20)   287630 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/jquery-3.5.1.js
+-rw-r--r--   0 cteubert   (507) staff       (20)    89476 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/jquery.js
+-rw-r--r--   0 cteubert   (507) staff       (20)    10854 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_static/language_data.js
+-rw-r--r--   0 cteubert   (507) staff       (20)       90 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/minus.png
+-rw-r--r--   0 cteubert   (507) staff       (20)       90 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/plus.png
+-rw-r--r--   0 cteubert   (507) staff       (20)     5249 2022-08-23 14:28:13.000000 prog_models-1.5.0rc2/docs/_static/pygments.css
+-rw-r--r--   0 cteubert   (507) staff       (20)    16634 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_static/searchtools.js
+-rw-r--r--   0 cteubert   (507) staff       (20)     4803 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/sidebar.js
+-rw-r--r--   0 cteubert   (507) staff       (20)    67692 2021-05-10 16:37:43.000000 prog_models-1.5.0rc2/docs/_static/underscore-1.12.0.js
+-rw-r--r--   0 cteubert   (507) staff       (20)    35168 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/underscore-1.3.1.js
+-rw-r--r--   0 cteubert   (507) staff       (20)    19530 2023-06-20 18:40:01.000000 prog_models-1.5.0rc2/docs/_static/underscore.js
+-rw-r--r--   0 cteubert   (507) staff       (20)    27376 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/deriv_prog_model.html
+-rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/dev_guide.html
+-rw-r--r--   0 cteubert   (507) staff       (20)     7442 2023-06-20 18:44:15.000000 prog_models-1.5.0rc2/docs/exceptions.html
+-rw-r--r--   0 cteubert   (507) staff       (20)     2295 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/genindex.html
+-rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/getting_started.html
+-rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/index.html
+-rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/models.html
+-rw-r--r--   0 cteubert   (507) staff       (20)      443 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/objects.inv
+-rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/prognostics_model.html
+-rw-r--r--   0 cteubert   (507) staff       (20)     8365 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/py-modindex.html
+-rw-r--r--   0 cteubert   (507) staff       (20)     2608 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/search.html
+-rw-r--r--   0 cteubert   (507) staff       (20)     1275 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/searchindex.js
+-rw-r--r--   0 cteubert   (507) staff       (20)      961 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/softwareplan.md
+-rw-r--r--   0 cteubert   (507) staff       (20)    31639 2023-06-20 18:42:18.000000 prog_models-1.5.0rc2/docs/visualize.html
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.583564 prog_models-1.5.0rc2/examples/
+-rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/examples/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)      939 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/examples/benchmarking.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6312 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/examples/future_loading.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4767 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/examples/new_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4949 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/examples/noise.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2433 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/examples/sensitivity.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     3608 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/examples/sim.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.583944 prog_models-1.5.0rc2/forms/
+-rw-r--r--   0 cteubert   (507) staff       (20)   219343 2023-06-20 18:42:18.000000 prog_models-1.5.0rc2/forms/Corporate CLA.pdf
+-rw-r--r--   0 cteubert   (507) staff       (20)   153485 2023-06-20 18:42:18.000000 prog_models-1.5.0rc2/forms/Individual CLA.pdf
+-rw-r--r--   0 cteubert   (507) staff       (20)    94594 2021-05-10 16:37:43.000000 prog_models-1.5.0rc2/license.pdf
+-rw-r--r--   0 cteubert   (507) staff       (20)    13424 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/prog_model_template.py
+-rw-r--r--   0 cteubert   (507) staff       (20)       38 2023-06-28 22:53:02.601868 prog_models-1.5.0rc2/setup.cfg
+-rw-r--r--   0 cteubert   (507) staff       (20)     2932 2023-06-28 22:52:14.000000 prog_models-1.5.0rc2/setup.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.567757 prog_models-1.5.0rc2/src/
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.585090 prog_models-1.5.0rc2/src/prog_models/
+-rw-r--r--   0 cteubert   (507) staff       (20)      468 2023-06-28 22:52:26.000000 prog_models-1.5.0rc2/src/prog_models/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    12776 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/composite_model.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.586479 prog_models-1.5.0rc2/src/prog_models/data_models/
+-rw-r--r--   0 cteubert   (507) staff       (20)      476 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/data_models/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     8208 2023-06-28 14:47:51.000000 prog_models-1.5.0rc2/src/prog_models/data_models/data_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    22276 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/data_models/dmd.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    35164 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/data_models/lstm_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     8465 2023-06-28 21:50:30.000000 prog_models-1.5.0rc2/src/prog_models/data_models/pce.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.587236 prog_models-1.5.0rc2/src/prog_models/datasets/
+-rw-r--r--   0 cteubert   (507) staff       (20)      157 2023-06-20 18:44:15.000000 prog_models-1.5.0rc2/src/prog_models/datasets/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6185 2023-06-22 23:28:06.000000 prog_models-1.5.0rc2/src/prog_models/datasets/nasa_battery.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6170 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/datasets/nasa_cmapss.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     5558 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/ensemble_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)      543 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/exceptions.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     9133 2023-06-28 21:50:30.000000 prog_models-1.5.0rc2/src/prog_models/linear_model.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.589213 prog_models-1.5.0rc2/src/prog_models/loading/
+-rw-r--r--   0 cteubert   (507) staff       (20)      347 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/loading/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    15484 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/loading/controllers.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1495 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/loading/gaussian_wrapper.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2102 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/loading/moving_average.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1772 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/loading/piecewise.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.591031 prog_models-1.5.0rc2/src/prog_models/models/
+-rw-r--r--   0 cteubert   (507) staff       (20)      918 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/models/__init__.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.591475 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/
+-rw-r--r--   0 cteubert   (507) staff       (20)      242 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)      335 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/aircraft.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    19213 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/small_rotorcraft.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.591737 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/
+-rw-r--r--   0 cteubert   (507) staff       (20)        0 2023-06-28 22:49:52.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/__init__.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.591987 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/aero/
+-rw-r--r--   0 cteubert   (507) staff       (20)        0 2023-06-28 22:50:32.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/aero/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1387 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/aero/aerodynamics.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.592987 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/control/
+-rw-r--r--   0 cteubert   (507) staff       (20)        0 2023-06-28 22:50:22.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/control/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2583 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/control/allocation_functions.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    12709 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/vehicles.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     7882 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/battery_circuit.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    32566 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/battery_electrochem.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    12741 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/centrifugal_pump.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6530 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/dcmotor.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     5649 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/dcmotor_singlephase.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4653 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/esc.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.593516 prog_models-1.5.0rc2/src/prog_models/models/experimental/
+-rw-r--r--   0 cteubert   (507) staff       (20)      158 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/models/experimental/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2949 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/experimental/paris_law.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    17214 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/pneumatic_valve.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6555 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/powertrain.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1428 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/propeller_load.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.594067 prog_models-1.5.0rc2/src/prog_models/models/test_models/
+-rw-r--r--   0 cteubert   (507) staff       (20)      249 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/models/test_models/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4384 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/models/test_models/linear_models.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4050 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/test_models/linear_thrown_object.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     5714 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/thrown_object.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    68508 2023-06-28 21:35:58.000000 prog_models-1.5.0rc2/src/prog_models/prognostics_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    17091 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/sim_result.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.596241 prog_models-1.5.0rc2/src/prog_models/utils/
+-rw-r--r--   0 cteubert   (507) staff       (20)      198 2023-06-20 18:44:15.000000 prog_models-1.5.0rc2/src/prog_models/utils/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    21583 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/calc_error.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     8984 2023-06-28 18:01:11.000000 prog_models-1.5.0rc2/src/prog_models/utils/containers.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1014 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/input_validation.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4382 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/next_state.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2242 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/noise_functions.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    10374 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/utils/parameters.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1173 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/utils/progress_bar.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1859 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/utils/serialization.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2484 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/utils/size.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.598136 prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/
+-rw-r--r--   0 cteubert   (507) staff       (20)      221 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    24434 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/geometry.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    16044 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/nurbs.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    33968 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/trajectory.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    27416 2023-06-28 18:01:29.000000 prog_models-1.5.0rc2/src/prog_models/visualize.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.585780 prog_models-1.5.0rc2/src/prog_models.egg-info/
+-rw-------   0 cteubert   (507) staff       (20)     7016 2023-06-28 22:53:02.000000 prog_models-1.5.0rc2/src/prog_models.egg-info/PKG-INFO
+-rw-------   0 cteubert   (507) staff       (20)     4988 2023-06-28 22:53:02.000000 prog_models-1.5.0rc2/src/prog_models.egg-info/SOURCES.txt
+-rw-------   0 cteubert   (507) staff       (20)        1 2023-06-28 22:53:02.000000 prog_models-1.5.0rc2/src/prog_models.egg-info/dependency_links.txt
+-rw-------   0 cteubert   (507) staff       (20)      204 2023-06-28 22:53:02.000000 prog_models-1.5.0rc2/src/prog_models.egg-info/requires.txt
+-rw-------   0 cteubert   (507) staff       (20)       12 2023-06-28 22:53:02.000000 prog_models-1.5.0rc2/src/prog_models.egg-info/top_level.txt
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.601462 prog_models-1.5.0rc2/tests/
+-rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/tests/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     3309 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/tests/__main__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    56896 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_base_models.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2652 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_battery.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    18087 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_calc_error.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     8122 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_centrifugal_pump.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    14085 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_composite.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    13250 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_data_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1872 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_datasets.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4177 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_dict_like_matrix_wrapper.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4622 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_direct.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     7537 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_ensemble.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    55549 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_estimate_params.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1627 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_examples.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    18578 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_linear_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6686 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_manual.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    12907 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_pneumatic_valve.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2435 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_powertrain.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4267 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_serialization.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    35373 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_sim_result.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    32855 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_surrogates.py
+-rw-r--r--   0 cteubert   (507) staff       (20)      918 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_tutorials.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    15470 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_uav_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    47927 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tutorial.ipynb
```

### Comparing `prog_models-1.5.0rc1/.gitignore` & `prog_models-1.5.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/PKG-INFO` & `prog_models-1.5.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog_models
-Version: 1.5.0rc1
+Version: 1.5.0rc2
 Summary: The NASA Prognostic Model Package is a python modeling framework focused on defining and building models for prognostics (computation of remaining useful life) of engineering systems, and provides a set of prognostics models for select components developed within this framework, suitable for use in prognostics applications for these components.
 Home-page: https://nasa.github.io/progpy/prog_models_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_models/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_models_guide.html
```

### Comparing `prog_models-1.5.0rc1/README.md` & `prog_models-1.5.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/.doctrees/deriv_prog_model.doctree` & `prog_models-1.5.0rc2/docs/.doctrees/deriv_prog_model.doctree`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/.doctrees/dev_guide.doctree` & `prog_models-1.5.0rc2/docs/.doctrees/dev_guide.doctree`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/.doctrees/environment.pickle` & `prog_models-1.5.0rc2/docs/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/.doctrees/exceptions.doctree` & `prog_models-1.5.0rc2/docs/.doctrees/exceptions.doctree`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/.doctrees/getting_started.doctree` & `prog_models-1.5.0rc2/docs/.doctrees/getting_started.doctree`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/.doctrees/index.doctree` & `prog_models-1.5.0rc2/docs/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/.doctrees/models.doctree` & `prog_models-1.5.0rc2/docs/.doctrees/models.doctree`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/.doctrees/prognostics_model.doctree` & `prog_models-1.5.0rc2/docs/.doctrees/prognostics_model.doctree`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/.doctrees/visualize.doctree` & `prog_models-1.5.0rc2/docs/.doctrees/visualize.doctree`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/7150.md` & `prog_models-1.5.0rc2/docs/7150.md`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_sources/exceptions.rst.txt` & `prog_models-1.5.0rc2/docs/_sources/exceptions.rst.txt`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/alabaster.css` & `prog_models-1.5.0rc2/docs/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/basic.css` & `prog_models-1.5.0rc2/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/classic.css` & `prog_models-1.5.0rc2/docs/_static/classic.css`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/doctools.js` & `prog_models-1.5.0rc2/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/jquery-3.5.1.js` & `prog_models-1.5.0rc2/docs/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/jquery.js` & `prog_models-1.5.0rc2/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/language_data.js` & `prog_models-1.5.0rc2/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/pygments.css` & `prog_models-1.5.0rc2/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/searchtools.js` & `prog_models-1.5.0rc2/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/sidebar.js` & `prog_models-1.5.0rc2/docs/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/underscore-1.12.0.js` & `prog_models-1.5.0rc2/docs/_static/underscore-1.12.0.js`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/underscore-1.3.1.js` & `prog_models-1.5.0rc2/docs/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/_static/underscore.js` & `prog_models-1.5.0rc2/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/deriv_prog_model.html` & `prog_models-1.5.0rc2/docs/deriv_prog_model.html`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/exceptions.html` & `prog_models-1.5.0rc2/docs/exceptions.html`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/genindex.html` & `prog_models-1.5.0rc2/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/py-modindex.html` & `prog_models-1.5.0rc2/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/search.html` & `prog_models-1.5.0rc2/docs/search.html`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/searchindex.js` & `prog_models-1.5.0rc2/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/softwareplan.md` & `prog_models-1.5.0rc2/docs/softwareplan.md`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/docs/visualize.html` & `prog_models-1.5.0rc2/docs/visualize.html`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/examples/benchmarking.py` & `prog_models-1.5.0rc2/examples/benchmarking.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/examples/future_loading.py` & `prog_models-1.5.0rc2/examples/future_loading.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/examples/new_model.py` & `prog_models-1.5.0rc2/examples/new_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/examples/noise.py` & `prog_models-1.5.0rc2/examples/noise.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/examples/sensitivity.py` & `prog_models-1.5.0rc2/examples/sensitivity.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/examples/sim.py` & `prog_models-1.5.0rc2/examples/sim.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/forms/Corporate CLA.pdf` & `prog_models-1.5.0rc2/forms/Corporate CLA.pdf`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/forms/Individual CLA.pdf` & `prog_models-1.5.0rc2/forms/Individual CLA.pdf`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/license.pdf` & `prog_models-1.5.0rc2/license.pdf`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/prog_model_template.py` & `prog_models-1.5.0rc2/prog_model_template.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/setup.py` & `prog_models-1.5.0rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'fastdtw',  # For DTW error calculation
         "tensorflow; platform_system!='Darwin' or platform_machine!='arm64'",
         "tensorflow-macos; platform_system=='Darwin' and platform_machine=='arm64'",
     ]
 
 setup(
     name='prog_models',
-    version='1.5.0-rc1',
+    version='1.5.0-rc2',
     description='The NASA Prognostic Model Package is a python modeling framework focused on defining and building models for prognostics (computation of remaining useful life) of engineering systems, and provides a set of prognostics models for select components developed within this framework, suitable for use in prognostics applications for these components.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://nasa.github.io/progpy/prog_models_guide.html',
     author='Christopher Teubert',
     author_email='christopher.a.teubert@nasa.gov',
     classifiers=[
```

### Comparing `prog_models-1.5.0rc1/src/prog_models/composite_model.py` & `prog_models-1.5.0rc2/src/prog_models/composite_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/data_models/data_model.py` & `prog_models-1.5.0rc2/src/prog_models/data_models/data_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/data_models/dmd.py` & `prog_models-1.5.0rc2/src/prog_models/data_models/dmd.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/data_models/lstm_model.py` & `prog_models-1.5.0rc2/src/prog_models/data_models/lstm_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/data_models/pce.py` & `prog_models-1.5.0rc2/src/prog_models/data_models/pce.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/datasets/nasa_battery.py` & `prog_models-1.5.0rc2/src/prog_models/datasets/nasa_battery.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/datasets/nasa_cmapss.py` & `prog_models-1.5.0rc2/src/prog_models/datasets/nasa_cmapss.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/ensemble_model.py` & `prog_models-1.5.0rc2/src/prog_models/ensemble_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/exceptions.py` & `prog_models-1.5.0rc2/src/prog_models/exceptions.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/linear_model.py` & `prog_models-1.5.0rc2/src/prog_models/linear_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/loading/controllers.py` & `prog_models-1.5.0rc2/src/prog_models/loading/controllers.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/loading/gaussian_wrapper.py` & `prog_models-1.5.0rc2/src/prog_models/loading/gaussian_wrapper.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/loading/moving_average.py` & `prog_models-1.5.0rc2/src/prog_models/loading/moving_average.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/loading/piecewise.py` & `prog_models-1.5.0rc2/src/prog_models/loading/piecewise.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/__init__.py` & `prog_models-1.5.0rc2/src/prog_models/models/__init__.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/aircraft_model/small_rotorcraft.py` & `prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/small_rotorcraft.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/battery_circuit.py` & `prog_models-1.5.0rc2/src/prog_models/models/battery_circuit.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/battery_electrochem.py` & `prog_models-1.5.0rc2/src/prog_models/models/battery_electrochem.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/centrifugal_pump.py` & `prog_models-1.5.0rc2/src/prog_models/models/centrifugal_pump.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/dcmotor.py` & `prog_models-1.5.0rc2/src/prog_models/models/dcmotor.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/dcmotor_singlephase.py` & `prog_models-1.5.0rc2/src/prog_models/models/dcmotor_singlephase.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/esc.py` & `prog_models-1.5.0rc2/src/prog_models/models/esc.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/experimental/paris_law.py` & `prog_models-1.5.0rc2/src/prog_models/models/experimental/paris_law.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/pneumatic_valve.py` & `prog_models-1.5.0rc2/src/prog_models/models/pneumatic_valve.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/powertrain.py` & `prog_models-1.5.0rc2/src/prog_models/models/powertrain.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/propeller_load.py` & `prog_models-1.5.0rc2/src/prog_models/models/propeller_load.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/test_models/linear_models.py` & `prog_models-1.5.0rc2/src/prog_models/models/test_models/linear_models.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/test_models/linear_thrown_object.py` & `prog_models-1.5.0rc2/src/prog_models/models/test_models/linear_thrown_object.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/models/thrown_object.py` & `prog_models-1.5.0rc2/src/prog_models/models/thrown_object.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/prognostics_model.py` & `prog_models-1.5.0rc2/src/prog_models/prognostics_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/sim_result.py` & `prog_models-1.5.0rc2/src/prog_models/sim_result.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/calc_error.py` & `prog_models-1.5.0rc2/src/prog_models/utils/calc_error.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/containers.py` & `prog_models-1.5.0rc2/src/prog_models/utils/containers.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/input_validation.py` & `prog_models-1.5.0rc2/src/prog_models/utils/input_validation.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/next_state.py` & `prog_models-1.5.0rc2/src/prog_models/utils/next_state.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/noise_functions.py` & `prog_models-1.5.0rc2/src/prog_models/utils/noise_functions.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/parameters.py` & `prog_models-1.5.0rc2/src/prog_models/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/progress_bar.py` & `prog_models-1.5.0rc2/src/prog_models/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/serialization.py` & `prog_models-1.5.0rc2/src/prog_models/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/size.py` & `prog_models-1.5.0rc2/src/prog_models/utils/size.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/traj_gen/geometry.py` & `prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/geometry.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/traj_gen/nurbs.py` & `prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/nurbs.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/utils/traj_gen/trajectory.py` & `prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/trajectory.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models/visualize.py` & `prog_models-1.5.0rc2/src/prog_models/visualize.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/src/prog_models.egg-info/PKG-INFO` & `prog_models-1.5.0rc2/src/prog_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog-models
-Version: 1.5.0rc1
+Version: 1.5.0rc2
 Summary: The NASA Prognostic Model Package is a python modeling framework focused on defining and building models for prognostics (computation of remaining useful life) of engineering systems, and provides a set of prognostics models for select components developed within this framework, suitable for use in prognostics applications for these components.
 Home-page: https://nasa.github.io/progpy/prog_models_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_models/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_models_guide.html
```

### Comparing `prog_models-1.5.0rc1/src/prog_models.egg-info/SOURCES.txt` & `prog_models-1.5.0rc2/src/prog_models.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,20 @@
 src/prog_models/models/pneumatic_valve.py
 src/prog_models/models/powertrain.py
 src/prog_models/models/propeller_load.py
 src/prog_models/models/thrown_object.py
 src/prog_models/models/aircraft_model/__init__.py
 src/prog_models/models/aircraft_model/aircraft.py
 src/prog_models/models/aircraft_model/small_rotorcraft.py
+src/prog_models/models/aircraft_model/vehicles/__init__.py
+src/prog_models/models/aircraft_model/vehicles/vehicles.py
+src/prog_models/models/aircraft_model/vehicles/aero/__init__.py
+src/prog_models/models/aircraft_model/vehicles/aero/aerodynamics.py
+src/prog_models/models/aircraft_model/vehicles/control/__init__.py
+src/prog_models/models/aircraft_model/vehicles/control/allocation_functions.py
 src/prog_models/models/experimental/__init__.py
 src/prog_models/models/experimental/paris_law.py
 src/prog_models/models/test_models/__init__.py
 src/prog_models/models/test_models/linear_models.py
 src/prog_models/models/test_models/linear_thrown_object.py
 src/prog_models/utils/__init__.py
 src/prog_models/utils/calc_error.py
```

### Comparing `prog_models-1.5.0rc1/tests/__main__.py` & `prog_models-1.5.0rc2/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_base_models.py` & `prog_models-1.5.0rc2/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_battery.py` & `prog_models-1.5.0rc2/tests/test_battery.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_calc_error.py` & `prog_models-1.5.0rc2/tests/test_calc_error.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_centrifugal_pump.py` & `prog_models-1.5.0rc2/tests/test_centrifugal_pump.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_composite.py` & `prog_models-1.5.0rc2/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_data_model.py` & `prog_models-1.5.0rc2/tests/test_data_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_datasets.py` & `prog_models-1.5.0rc2/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_dict_like_matrix_wrapper.py` & `prog_models-1.5.0rc2/tests/test_dict_like_matrix_wrapper.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_direct.py` & `prog_models-1.5.0rc2/tests/test_direct.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_ensemble.py` & `prog_models-1.5.0rc2/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_estimate_params.py` & `prog_models-1.5.0rc2/tests/test_estimate_params.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_examples.py` & `prog_models-1.5.0rc2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_linear_model.py` & `prog_models-1.5.0rc2/tests/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_manual.py` & `prog_models-1.5.0rc2/tests/test_manual.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_pneumatic_valve.py` & `prog_models-1.5.0rc2/tests/test_pneumatic_valve.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_powertrain.py` & `prog_models-1.5.0rc2/tests/test_powertrain.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_serialization.py` & `prog_models-1.5.0rc2/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_sim_result.py` & `prog_models-1.5.0rc2/tests/test_sim_result.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_surrogates.py` & `prog_models-1.5.0rc2/tests/test_surrogates.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_tutorials.py` & `prog_models-1.5.0rc2/tests/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tests/test_uav_model.py` & `prog_models-1.5.0rc2/tests/test_uav_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc1/tutorial.ipynb` & `prog_models-1.5.0rc2/tutorial.ipynb`

 * *Files identical despite different names*

