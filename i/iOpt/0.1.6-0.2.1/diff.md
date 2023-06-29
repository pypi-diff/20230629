# Comparing `tmp/iOpt-0.1.6.tar.gz` & `tmp/iOpt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iOpt-0.1.6.tar", last modified: Sun Mar 12 10:40:22 2023, max compression
+gzip compressed data, was "iOpt-0.2.1.tar", last modified: Thu Jun 29 07:15:58 2023, max compression
```

## Comparing `iOpt-0.1.6.tar` & `iOpt-0.2.1.tar`

### file list

```diff
@@ -1,141 +1,181 @@
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.265358 iOpt-0.1.6/
--rw-r--r--   0 anton      (501) staff       (20)     1543 2023-03-12 09:50:57.000000 iOpt-0.1.6/LICENSE
--rw-r--r--   0 anton      (501) staff       (20)     6421 2023-03-12 10:40:22.264904 iOpt-0.1.6/PKG-INFO
--rw-r--r--   0 anton      (501) staff       (20)     5883 2023-03-12 09:50:57.000000 iOpt-0.1.6/README.md
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.228092 iOpt-0.1.6/examples/
--rw-r--r--   0 anton      (501) staff       (20)     1191 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/GKLS_example.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.228306 iOpt-0.1.6/examples/Genetic_algorithm/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.228506 iOpt-0.1.6/examples/Genetic_algorithm/TSP/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.229097 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_1D/
--rw-r--r--   0 anton      (501) staff       (20)     1552 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_1D/Example_GA_TSP_Vary_Mutation.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.229712 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_1D/Problems/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_1D/Problems/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     3553 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_1D/Problems/ga_tsp_vary_mutation.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_1D/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.230546 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_2D/
--rw-r--r--   0 anton      (501) staff       (20)     1712 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_2D/Example_GA_TSP_Vary_Mutation_Population_Size.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.231097 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_2D/Problems/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_2D/Problems/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     4586 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_2D/Problems/ga_tsp_2d.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Genetic_algorithm/TSP/_2D/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Genetic_algorithm/TSP/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Genetic_algorithm/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     1190 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Grishagin_example.py
--rw-r--r--   0 anton      (501) staff       (20)     1113 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Hill_example.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.231663 iOpt-0.1.6/examples/Machine_learning/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.231926 iOpt-0.1.6/examples/Machine_learning/SVC/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.233409 iOpt-0.1.6/examples/Machine_learning/SVC/_1D/
--rw-r--r--   0 anton      (501) staff       (20)     1423 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_kernel_coefficient.py
--rw-r--r--   0 anton      (501) staff       (20)     1463 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_regularization.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.234542 iOpt-0.1.6/examples/Machine_learning/SVC/_1D/Problems/
--rw-r--r--   0 anton      (501) staff       (20)     3086 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Kernel.py
--rw-r--r--   0 anton      (501) staff       (20)     3162 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Regularization.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/_1D/Problems/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/_1D/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.235590 iOpt-0.1.6/examples/Machine_learning/SVC/_2D/
--rw-r--r--   0 anton      (501) staff       (20)     1346 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/_2D/Example_2D_SVC.py
--rw-r--r--   0 anton      (501) staff       (20)     1449 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/_2D/Example_2D_SVC_Industrial.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.236539 iOpt-0.1.6/examples/Machine_learning/SVC/_2D/Problems/
--rw-r--r--   0 anton      (501) staff       (20)     3181 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/_2D/Problems/SVC_2d.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/_2D/Problems/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/_2D/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/SVC/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Machine_learning/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     1190 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Rastrigin_example.py
--rw-r--r--   0 anton      (501) staff       (20)      857 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Shekel4_example.py
--rw-r--r--   0 anton      (501) staff       (20)     1094 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/Shekel_example.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.237940 iOpt-0.1.6/examples/console_output/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/console_output/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      594 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/console_output/example_custom_output.py
--rw-r--r--   0 anton      (501) staff       (20)      582 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/console_output/example_full_output.py
--rw-r--r--   0 anton      (501) staff       (20)      583 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/console_output/example_only_result_output.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.238458 iOpt-0.1.6/examples/dynamic_painters/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.238864 iOpt-0.1.6/examples/dynamic_painters/1D_examples/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/dynamic_painters/1D_examples/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      600 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/dynamic_painters/1D_examples/example_1D_with_objective_function.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.239402 iOpt-0.1.6/examples/dynamic_painters/2D_examples/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/dynamic_painters/2D_examples/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      600 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/dynamic_painters/2D_examples/example_2D_with_level_lines.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/dynamic_painters/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.239795 iOpt-0.1.6/examples/static_painters/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.243308 iOpt-0.1.6/examples/static_painters/1D_examples/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/1D_examples/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      616 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/1D_examples/example_1D_with_approximation.py
--rw-r--r--   0 anton      (501) staff       (20)      675 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/1D_examples/example_1D_with_interpolation.py
--rw-r--r--   0 anton      (501) staff       (20)      613 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/1D_examples/example_1D_with_objective_function_pointsInBottom_mode.py
--rw-r--r--   0 anton      (501) staff       (20)      614 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/1D_examples/example_1D_with_only_points.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.245458 iOpt-0.1.6/examples/static_painters/2D_examples/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/2D_examples/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      749 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/2D_examples/example_2D_with_1-dimension_section.py
--rw-r--r--   0 anton      (501) staff       (20)      643 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/2D_examples/example_2D_with_approximation.py
--rw-r--r--   0 anton      (501) staff       (20)      643 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/2D_examples/example_2D_with_interpolation.py
--rw-r--r--   0 anton      (501) staff       (20)      615 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/2D_examples/example_2D_with_level_lines.py
--rw-r--r--   0 anton      (501) staff       (20)      647 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/2D_examples/example_2D_with_level_lines_by_interpolation.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/examples/static_painters/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.247269 iOpt-0.1.6/iOpt/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.249884 iOpt-0.1.6/iOpt/evolvent/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/evolvent/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)    11327 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/evolvent/evolvent.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.252633 iOpt-0.1.6/iOpt/method/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/method/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)    14706 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/method/listener.py
--rw-r--r--   0 anton      (501) staff       (20)    13819 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/method/method.py
--rw-r--r--   0 anton      (501) staff       (20)     1359 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/method/optim_task.py
--rw-r--r--   0 anton      (501) staff       (20)     6689 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/method/process.py
--rw-r--r--   0 anton      (501) staff       (20)    19001 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/method/search_data.py
--rw-r--r--   0 anton      (501) staff       (20)      368 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/method/sol_value.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.252961 iOpt-0.1.6/iOpt/output_system/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/output_system/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.253363 iOpt-0.1.6/iOpt/output_system/console/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/output_system/console/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     6291 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/output_system/console/console_output.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.254625 iOpt-0.1.6/iOpt/output_system/painters/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/output_system/painters/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     7688 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/output_system/painters/dynamic_painter.py
--rw-r--r--   0 anton      (501) staff       (20)    20712 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/output_system/painters/static_painter.py
--rw-r--r--   0 anton      (501) staff       (20)     1402 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problem.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.257816 iOpt-0.1.6/iOpt/problems/
--rw-r--r--   0 anton      (501) staff       (20)     3276 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/GKLS.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.258928 iOpt-0.1.6/iOpt/problems/GKLS_function/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/GKLS_function/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)    34146 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/GKLS_function/gkls_function.py
--rw-r--r--   0 anton      (501) staff       (20)     5230 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/GKLS_function/gkls_random.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.259456 iOpt-0.1.6/iOpt/problems/Hill/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/Hill/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)   418174 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/Hill/hill_generation.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.261000 iOpt-0.1.6/iOpt/problems/Shekel/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/Shekel/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)   355176 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/Shekel/shekel_generation.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.262306 iOpt-0.1.6/iOpt/problems/Shekel4/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/Shekel4/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      407 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/Shekel4/shekel4_generation.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     3067 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/grishagin.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.263404 iOpt-0.1.6/iOpt/problems/grishagin_function/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/grishagin_function/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     4226 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/grishagin_function/grishagin_function.py
--rw-r--r--   0 anton      (501) staff       (20)     6176 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/grishagin_function/grishagin_generation.py
--rw-r--r--   0 anton      (501) staff       (20)     3170 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/hill.py
--rw-r--r--   0 anton      (501) staff       (20)     2674 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/rastrigin.py
--rw-r--r--   0 anton      (501) staff       (20)     3204 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/shekel.py
--rw-r--r--   0 anton      (501) staff       (20)     3177 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/shekel4.py
--rw-r--r--   0 anton      (501) staff       (20)     3270 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/stronginC3.py
--rw-r--r--   0 anton      (501) staff       (20)     2211 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/problems/xsquared.py
--rw-r--r--   0 anton      (501) staff       (20)     1424 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/solution.py
--rw-r--r--   0 anton      (501) staff       (20)     4382 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/solver.py
--rw-r--r--   0 anton      (501) staff       (20)     2443 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/solver_parametrs.py
--rw-r--r--   0 anton      (501) staff       (20)      902 2023-03-12 09:50:57.000000 iOpt-0.1.6/iOpt/trial.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.249316 iOpt-0.1.6/iOpt.egg-info/
--rw-r--r--   0 anton      (501) staff       (20)     6421 2023-03-12 10:40:22.000000 iOpt-0.1.6/iOpt.egg-info/PKG-INFO
--rw-r--r--   0 anton      (501) staff       (20)     4308 2023-03-12 10:40:22.000000 iOpt-0.1.6/iOpt.egg-info/SOURCES.txt
--rw-r--r--   0 anton      (501) staff       (20)        1 2023-03-12 10:40:22.000000 iOpt-0.1.6/iOpt.egg-info/dependency_links.txt
--rw-r--r--   0 anton      (501) staff       (20)      153 2023-03-12 10:40:22.000000 iOpt-0.1.6/iOpt.egg-info/requires.txt
--rw-r--r--   0 anton      (501) staff       (20)       14 2023-03-12 10:40:22.000000 iOpt-0.1.6/iOpt.egg-info/top_level.txt
--rw-r--r--   0 anton      (501) staff       (20)       38 2023-03-12 10:40:22.265429 iOpt-0.1.6/setup.cfg
--rw-r--r--   0 anton      (501) staff       (20)     1359 2023-03-12 10:38:36.000000 iOpt-0.1.6/setup.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-03-12 10:40:22.264437 iOpt-0.1.6/test/
--rw-r--r--   0 anton      (501) staff       (20)     3818 2023-03-12 09:50:57.000000 iOpt-0.1.6/test/test_evolvent.py
--rw-r--r--   0 anton      (501) staff       (20)     1870 2023-03-12 09:50:57.000000 iOpt-0.1.6/test/test_optim_task.py
--rw-r--r--   0 anton      (501) staff       (20)     9988 2023-03-12 09:50:57.000000 iOpt-0.1.6/test/test_solving_test_problems.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.250923 iOpt-0.2.1/
+-rw-r--r--   0 anton      (501) staff       (20)     1543 2023-04-21 14:01:15.000000 iOpt-0.2.1/LICENSE
+-rw-r--r--   0 anton      (501) staff       (20)     7406 2023-06-29 07:15:58.250511 iOpt-0.2.1/PKG-INFO
+-rw-r--r--   0 anton      (501) staff       (20)     6867 2023-04-25 16:30:22.000000 iOpt-0.2.1/README.md
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.177737 iOpt-0.2.1/examples/
+-rw-r--r--   0 anton      (501) staff       (20)     1380 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/GKLS_example.py
+-rw-r--r--   0 anton      (501) staff       (20)     1002 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/GKLS_timeout_example.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.178161 iOpt-0.2.1/examples/Genetic_algorithm/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.178451 iOpt-0.2.1/examples/Genetic_algorithm/TSP/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.179031 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/
+-rw-r--r--   0 anton      (501) staff       (20)     1687 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Example_GA_TSP_Vary_Mutation.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.179476 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Problems/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Problems/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     3554 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Problems/ga_tsp_vary_mutation.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.180591 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/
+-rw-r--r--   0 anton      (501) staff       (20)     1798 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Example_GA_TSP_Vary_Mutation_Population_Size.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.181042 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Problems/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Problems/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     4587 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Problems/ga_tsp_2d.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     1288 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Grishagin_example.py
+-rw-r--r--   0 anton      (501) staff       (20)     1210 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Hill_example.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.181369 iOpt-0.2.1/examples/Machine_learning/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.181673 iOpt-0.2.1/examples/Machine_learning/SVC/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.182616 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/
+-rw-r--r--   0 anton      (501) staff       (20)     1509 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_kernel_coefficient.py
+-rw-r--r--   0 anton      (501) staff       (20)     1548 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_regularization.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.183660 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/
+-rw-r--r--   0 anton      (501) staff       (20)     3032 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Kernel.py
+-rw-r--r--   0 anton      (501) staff       (20)     3108 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Regularization.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.186064 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/
+-rw-r--r--   0 anton      (501) staff       (20)     1482 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Example_2D_SVC.py
+-rw-r--r--   0 anton      (501) staff       (20)     1563 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Example_2D_SVC_Industrial.py
+-rw-r--r--   0 anton      (501) staff       (20)     1240 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Example_SVC_Float_Discrete.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.187239 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Problems/
+-rw-r--r--   0 anton      (501) staff       (20)     3031 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Problems/SVC_2D_Float_Discrete.py
+-rw-r--r--   0 anton      (501) staff       (20)     3065 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Problems/SVC_2d.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Problems/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.195050 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/
+-rw-r--r--   0 anton      (501) staff       (20)     1379 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/Example_SVC_Discrete_Param.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.195561 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/Problem/
+-rw-r--r--   0 anton      (501) staff       (20)     3366 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/Problem/SVC_3D.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/Problem/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     1238 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/RastriginInt_example.py
+-rw-r--r--   0 anton      (501) staff       (20)     1462 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Rastrigin_example.py
+-rw-r--r--   0 anton      (501) staff       (20)      894 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Shekel4_example.py
+-rw-r--r--   0 anton      (501) staff       (20)     1245 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Shekel_example.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.197132 iOpt-0.2.1/examples/console_output/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/console_output/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      607 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/console_output/example_custom_output.py
+-rw-r--r--   0 anton      (501) staff       (20)      595 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/console_output/example_full_output.py
+-rw-r--r--   0 anton      (501) staff       (20)      596 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/console_output/example_only_result_output.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.197442 iOpt-0.2.1/examples/dynamic_painters/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.197910 iOpt-0.2.1/examples/dynamic_painters/1D_examples/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/dynamic_painters/1D_examples/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      620 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/dynamic_painters/1D_examples/example_1D_with_objective_function.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.198452 iOpt-0.2.1/examples/dynamic_painters/2D_examples/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/dynamic_painters/2D_examples/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      778 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/dynamic_painters/2D_examples/example_2D_with_level_lines.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/dynamic_painters/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.199010 iOpt-0.2.1/examples/static_painters/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.200788 iOpt-0.2.1/examples/static_painters/1D_examples/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/1D_examples/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      639 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_approximation.py
+-rw-r--r--   0 anton      (501) staff       (20)      639 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_interpolation.py
+-rw-r--r--   0 anton      (501) staff       (20)      636 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_objective_function_pointsInBottom_mode.py
+-rw-r--r--   0 anton      (501) staff       (20)      637 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_only_points.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.202890 iOpt-0.2.1/examples/static_painters/2D_examples/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      774 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_1-dimension_section.py
+-rw-r--r--   0 anton      (501) staff       (20)      666 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_approximation.py
+-rw-r--r--   0 anton      (501) staff       (20)      666 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_interpolation.py
+-rw-r--r--   0 anton      (501) staff       (20)      638 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_level_lines.py
+-rw-r--r--   0 anton      (501) staff       (20)      670 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_level_lines_by_interpolation.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.212153 iOpt-0.2.1/iOpt/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.214550 iOpt-0.2.1/iOpt/evolvent/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/evolvent/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)    11432 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/evolvent/evolvent.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.219657 iOpt-0.2.1/iOpt/method/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/method/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     3291 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/calculator.py
+-rw-r--r--   0 anton      (501) staff       (20)      359 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/icriterion_evaluate_method.py
+-rw-r--r--   0 anton      (501) staff       (20)     7340 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/index_method.py
+-rw-r--r--   0 anton      (501) staff       (20)     2194 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/index_method_calculator.py
+-rw-r--r--   0 anton      (501) staff       (20)      577 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/method/listener.py
+-rw-r--r--   0 anton      (501) staff       (20)    17783 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/method.py
+-rw-r--r--   0 anton      (501) staff       (20)    12978 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/mixed_integer_method.py
+-rw-r--r--   0 anton      (501) staff       (20)     1493 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/optim_task.py
+-rw-r--r--   0 anton      (501) staff       (20)     3614 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/parallel_process.py
+-rw-r--r--   0 anton      (501) staff       (20)     9748 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/process.py
+-rw-r--r--   0 anton      (501) staff       (20)    24759 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/search_data.py
+-rw-r--r--   0 anton      (501) staff       (20)      368 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/method/sol_value.py
+-rw-r--r--   0 anton      (501) staff       (20)     3676 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/solverFactory.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.220071 iOpt-0.2.1/iOpt/output_system/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.221534 iOpt-0.2.1/iOpt/output_system/listeners/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/listeners/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     4695 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/listeners/animate_painters.py
+-rw-r--r--   0 anton      (501) staff       (20)     2351 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/listeners/console_outputers.py
+-rw-r--r--   0 anton      (501) staff       (20)    10166 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/listeners/static_painters.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.222069 iOpt-0.2.1/iOpt/output_system/outputers/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/outputers/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     8761 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/outputers/console_outputer.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.230116 iOpt-0.2.1/iOpt/output_system/painters/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/painters/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     5164 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/painters/animate_painters.py
+-rw-r--r--   0 anton      (501) staff       (20)      389 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/painters/painter.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.230721 iOpt-0.2.1/iOpt/output_system/painters/plotters/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/painters/plotters/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)    19460 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/painters/plotters/plotters.py
+-rw-r--r--   0 anton      (501) staff       (20)    12090 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/painters/static_painters.py
+-rw-r--r--   0 anton      (501) staff       (20)     1661 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/problem.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.231305 iOpt-0.2.1/iOpt/routine/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/routine/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      843 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/routine/timeout.py
+-rw-r--r--   0 anton      (501) staff       (20)     1424 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/solution.py
+-rw-r--r--   0 anton      (501) staff       (20)     9049 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/solver.py
+-rw-r--r--   0 anton      (501) staff       (20)     3159 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/solver_parametrs.py
+-rw-r--r--   0 anton      (501) staff       (20)      906 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/trial.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.214026 iOpt-0.2.1/iOpt.egg-info/
+-rw-r--r--   0 anton      (501) staff       (20)     7406 2023-06-29 07:15:58.000000 iOpt-0.2.1/iOpt.egg-info/PKG-INFO
+-rw-r--r--   0 anton      (501) staff       (20)     5506 2023-06-29 07:15:58.000000 iOpt-0.2.1/iOpt.egg-info/SOURCES.txt
+-rw-r--r--   0 anton      (501) staff       (20)        1 2023-06-29 07:15:58.000000 iOpt-0.2.1/iOpt.egg-info/dependency_links.txt
+-rw-r--r--   0 anton      (501) staff       (20)      153 2023-06-29 07:15:58.000000 iOpt-0.2.1/iOpt.egg-info/requires.txt
+-rw-r--r--   0 anton      (501) staff       (20)       23 2023-06-29 07:15:58.000000 iOpt-0.2.1/iOpt.egg-info/top_level.txt
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.242588 iOpt-0.2.1/problems/
+-rw-r--r--   0 anton      (501) staff       (20)     3299 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/GKLS.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.243858 iOpt-0.2.1/problems/GKLS_function/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/GKLS_function/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)    34141 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/GKLS_function/gkls_function.py
+-rw-r--r--   0 anton      (501) staff       (20)     5230 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/GKLS_function/gkls_random.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.244702 iOpt-0.2.1/problems/Hill/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Hill/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)   418174 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Hill/hill_generation.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.245906 iOpt-0.2.1/problems/Shekel/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Shekel/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)   355176 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Shekel/shekel_generation.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.248030 iOpt-0.2.1/problems/Shekel4/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Shekel4/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      407 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Shekel4/shekel4_generation.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     2631 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/g2c.py
+-rw-r--r--   0 anton      (501) staff       (20)     2564 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/g8c.py
+-rw-r--r--   0 anton      (501) staff       (20)     3053 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/grishagin.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.248934 iOpt-0.2.1/problems/grishagin_function/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/grishagin_function/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     3968 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/grishagin_function/grishagin_function.py
+-rw-r--r--   0 anton      (501) staff       (20)     6176 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/grishagin_function/grishagin_generation.py
+-rw-r--r--   0 anton      (501) staff       (20)     3168 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/hill.py
+-rw-r--r--   0 anton      (501) staff       (20)     2677 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/rastrigin.py
+-rw-r--r--   0 anton      (501) staff       (20)     5378 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/rastriginInt.py
+-rw-r--r--   0 anton      (501) staff       (20)     3034 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/rastrigin_hidden_constraint.py
+-rw-r--r--   0 anton      (501) staff       (20)     5684 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/rastrigin_int_hidden_constraint.py
+-rw-r--r--   0 anton      (501) staff       (20)     2391 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/romeijn1c.py
+-rw-r--r--   0 anton      (501) staff       (20)     2913 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/romeijn2c.py
+-rw-r--r--   0 anton      (501) staff       (20)     2949 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/romeijn3c.py
+-rw-r--r--   0 anton      (501) staff       (20)     2637 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/romeijn5c.py
+-rw-r--r--   0 anton      (501) staff       (20)     3200 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/shekel.py
+-rw-r--r--   0 anton      (501) staff       (20)     3173 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/shekel4.py
+-rw-r--r--   0 anton      (501) staff       (20)     2938 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/stronginc2.py
+-rw-r--r--   0 anton      (501) staff       (20)     3150 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/stronginc3.py
+-rw-r--r--   0 anton      (501) staff       (20)     3407 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/stronginc5.py
+-rw-r--r--   0 anton      (501) staff       (20)     2212 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/xsquared.py
+-rw-r--r--   0 anton      (501) staff       (20)       38 2023-06-29 07:15:58.251011 iOpt-0.2.1/setup.cfg
+-rw-r--r--   0 anton      (501) staff       (20)     1359 2023-06-29 07:15:09.000000 iOpt-0.2.1/setup.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.250050 iOpt-0.2.1/test/
+-rw-r--r--   0 anton      (501) staff       (20)     3795 2023-06-29 05:54:18.000000 iOpt-0.2.1/test/test_evolvent.py
+-rw-r--r--   0 anton      (501) staff       (20)     1865 2023-04-21 14:01:16.000000 iOpt-0.2.1/test/test_optim_task.py
+-rw-r--r--   0 anton      (501) staff       (20)     6617 2023-06-29 05:54:18.000000 iOpt-0.2.1/test/test_solving_test_problems.py
```

### Comparing `iOpt-0.1.6/LICENSE` & `iOpt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iOpt-0.1.6/PKG-INFO` & `iOpt-0.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-Metadata-Version: 2.1
-Name: iOpt
-Version: 0.1.6
-Summary: Фреймворк для автоматического выбора значений параметров для математических моделей, ИИ и МО.
-Home-page: https://github.com/aimclub/iOpt
-Author: UNN Team
-Author-email: 
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <img src="/docs/iOpt_logo.png" width="200" height="150"/>
 </p>
 
+[![SAI](https://github.com/ITMO-NSS-team/open-source-ops/blob/master/badges/SAI_badge_flat.svg)](https://sai.itmo.ru/)
+[![ITMO](https://github.com/ITMO-NSS-team/open-source-ops/blob/master/badges/ITMO_badge_flat.svg)](https://en.itmo.ru/en/)
+
 [![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-green)](LICENSE)
 [![python: 3.9](https://img.shields.io/badge/python-3.9-44cc12?style=flat-square&logo=python)](https://www.python.org/downloads/release/python-390/)
 [![python: 3.8](https://img.shields.io/badge/python-3.8-44cc12?style=flat-square&logo=python)](https://www.python.org/downloads/release/python-380/)
 [![docs: ](https://readthedocs.org/projects/ebonite/badge/?style=flat-square)](https://iopt.readthedocs.io/ru/latest/)
 [![build:](https://github.com/UNN-ITMM-Software/iOpt/actions/workflows/python-app.yml/badge.svg)](https://github.com/UNN-ITMM-Software/iOpt/actions)
 [![rus:](https://img.shields.io/badge/lang-ru-yellow.svg)](README_ru.md)
 
@@ -34,64 +23,90 @@
 - Integration with external artificial intelligence and machine learning libraries or frameworks as well as applied models.
 - Automation of the preliminary analysis of the models under study, e.g., by identifying different types of model dependencies on different groups of parameters.
 - Visualization of the process of choosing optimal parameters.
 
 
 # **Installation**
 
-## On Unix-like systems:
+
+
+## Automatic installation
+
+The simplest way to install **iOpt** is using *pip*:
 
 ```
-git clone https://github.com/UNN-ITMM-Software/iOpt
+pip install iOpt
+``` 
+
+## Manual installation
+
+### On Unix-like systems:
+
+```
+git clone https://github.com/aimclub/iOpt
 cd iOpt
 pip install virtualenv
 virtualenv ioptenv
 source ioptenv/bin/activate
 python setup.py install
 ```
 
-## On Windows:
+### On Windows:
 
 ```
-git clone https://github.com/UNN-ITMM-Software/iOpt
+git clone https://github.com/aimclub/iOpt
 cd iOpt
 pip install virtualenv
 virtualenv ioptenv
 ioptenv\Scripts\activate.bat
 python setup.py install
 ```
+## Docker
+
+Download the image:
+
+```
+docker pull aimclub/iopt:latest
+```
+
+Using the iOpt image:
+
+```
+docker run -it aimclub/iopt:latest
+```
 
 
 # **How to Use**
 
 Using the iOpt framework to minimize the Rastrigin test function.
 
 ```python
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticNDPaintListener, ConsoleFullOutputListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 from subprocess import Popen, PIPE, STDOUT
 
 if __name__ == "__main__":
     """
     Minimization of the Rastrigin test function with visualization
     """
     #Create a test task
     problem = Rastrigin(2)
     #Setup a solver options
     params = SolverParameters(r=2.5, eps=0.01, itersLimit=300, refineSolution=True)
     #Create the solver
     solver = Solver(problem, parameters=params)
     #Print results to console while solving
-    cfol = ConsoleFullOutputListener(mode='full')
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
     #3D visualization at the end of the solution
-    spl = StaticNDPaintListener("rastrigin.png", "output", varsIndxs=[0,1], mode="surface", calc="interpolation")
+    spl = StaticPainterNDListener("rastrigin.png", "output", varsIndxs=[0,1], mode="surface", calc="interpolation")
     solver.AddListener(spl)
     #Run problem solution
     sol = solver.Solve()
 ```
 
 # **Examples**
 
@@ -99,15 +114,17 @@
 
 
 ```python
 import numpy as np
 from sklearn.utils import shuffle
 from sklearn.datasets import load_breast_cancer
 
-from iOpt.method.listener import StaticNDPaintListener, AnimationNDPaintListener, ConsoleFullOutputListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
+from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
 from examples.Machine_learning.SVC._2D.Problems import SVC_2d
 
 
 def load_breast_cancer_data():
     dataset = load_breast_cancer()
@@ -122,21 +139,21 @@
     kernel_coefficient_bound = {'low': -7, 'up': -3}
 
     problem = SVC_2d.SVC_2D(x, y, regularization_value_bound, kernel_coefficient_bound)
 
     method_params = SolverParameters(r=np.double(3.0), itersLimit=100)
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimationNDPaintListener("svc2d_anim.png", "output", varsIndxs=[0, 1], toPaintObjFunc=False)
+    apl = AnimatePainterNDListener("svc2d_anim.png", "output", varsIndxs=[0, 1], toPaintObjFunc=False)
     solver.AddListener(apl)
 
-    spl = StaticNDPaintListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
+    spl = StaticPainterNDListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
     solver.AddListener(spl)
     
-    cfol = ConsoleFullOutputListener(mode='full')
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
 
     solver_info = solver.Solve()
 
 ```
 
 # **Project Structure**
@@ -146,7 +163,12 @@
 - The [examples](https://github.com/UNN-ITMM-Software/iOpt/tree/main/examples) directory contains examples of using the framework for both test and applied problems.
 - Unit tests are located in the [test](https://github.com/UNN-ITMM-Software/iOpt/tree/main/test) directory.
 - Documentation source files are located in the [docs](https://github.com/UNN-ITMM-Software/iOpt/tree/main/docs) directory.
 
 # **Documentation**
 
 A detailed description of the iOpt framework API is available at [Read the Docs](https://iopt.readthedocs.io/ru/latest/).
+
+# **Supported by**
+
+The study is supported by the [Research Center Strong Artificial Intelligence in Industry](https://sai.itmo.ru/) 
+of [ITMO University](https://en.itmo.ru/) as part of the plan of the center's program: Framework of intelligent heuristic optimization methods.
```

### Comparing `iOpt-0.1.6/examples/GKLS_example.py` & `iOpt-0.2.1/examples/GKLS_timeout_example.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-from iOpt.problems.GKLS import GKLS
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticNDPaintListener, ConsoleFullOutputListener
+from problems.GKLS import GKLS
 
 
 def SolveSingleGKLS():
     """
     Минимизация тестовой функции из GKLS генератора с номером 39
     """
 
     # создание объекта задачи
-    problem = GKLS(2, 39)
+    problem = GKLS(dimension=6, functionNumber=39)
 
     # Формируем параметры решателя
-    params = SolverParameters(r=3.5, eps=0.01, itersLimit=300, refineSolution=True)
+    params = SolverParameters(r=7, eps=0.01, itersLimit=3000000,
+                              numberOfParallelPoints=4, timeout=1)
 
     # Создаем решатель
-    solver = Solver(problem, parameters=params)
+    solver = Solver(problem=problem, parameters=params)
 
     # Добавляем вывод резултатов в консоль
-    cfol = ConsoleFullOutputListener(mode='full')
+    cfol = ConsoleOutputListener(mode='result')
     solver.AddListener(cfol)
 
-    # Добавляем построение 3D визуализации после решения задачи
-    spl = StaticNDPaintListener("GKLS.png", "output", varsIndxs=[0, 1], mode="lines layers", calc="objective function")
-    solver.AddListener(spl)
-
     # Решение задачи
     sol = solver.Solve()
 
 
 if __name__ == "__main__":
     SolveSingleGKLS()
```

### Comparing `iOpt-0.1.6/examples/Genetic_algorithm/TSP/_1D/Example_GA_TSP_Vary_Mutation.py` & `iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Example_GA_TSP_Vary_Mutation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from iOpt.method.listener import StaticPaintListener, AnimationPaintListener, ConsoleFullOutputListener
+from iOpt.output_system.listeners.static_painters import StaticPainterListener
+from iOpt.output_system.listeners.animate_painters import AnimatePainterListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
+
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
 from examples.Genetic_algorithm.TSP._1D.Problems import ga_tsp_vary_mutation
 import numpy as np
 import xml.etree.ElementTree as ET
 
-
 def load_TSPs_matrix(filename):
     root = ET.parse(filename).getroot()
     columns = root.findall('graph/vertex')
     num_cols = len(columns)
     trans_matrix = np.zeros((num_cols, num_cols))
     for i, v in enumerate(columns):
         for e in v:
@@ -25,17 +27,17 @@
     mutation_probability_bound = {'low': 0.0, 'up': 1.0}
     problem = ga_tsp_vary_mutation.GA_TSP_Vary_Mutation(tsp_matrix, num_iteration,
                                                         population_size, mutation_probability_bound)
 
     method_params = SolverParameters(r=np.double(3.0), itersLimit=40)
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimationPaintListener("gatsp_1d_anim_vary_mutation.png", "output", toPaintObjFunc=False)
+    apl = AnimatePainterListener("gatsp_1d_anim_vary_mutation.png", "output", toPaintObjFunc=False)
     solver.AddListener(apl)
 
-    spl = StaticPaintListener("gatsp_1d_stat_vary_mutation.png", "output", mode="interpolation")
+    spl = StaticPainterListener("gatsp_1d_stat_vary_mutation.png", "output", mode="interpolation")
     solver.AddListener(spl)
 
-    cfol = ConsoleFullOutputListener(mode='full')
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
 
     solver_info = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/Genetic_algorithm/TSP/_1D/Problems/ga_tsp_vary_mutation.py` & `iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Problems/ga_tsp_vary_mutation.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         :param num_iteration: Максимальное число итераций генетического алгоритма
         :param population_size: Размер популяции
         :param mutation_probability_bound: Границы изменения вероятности мутации (low - нижняя граница, up - верхняя)
         """
         super(GA_TSP_Vary_Mutation, self).__init__()
         self.dimension = 1
         self.numberOfFloatVariables = 1
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
         self.costMatrix = cost_matrix
         if num_iteration <= 0:
             raise ValueError('The number of iterations cannot be zero or negative.')
         if population_size <= 0:
             raise ValueError('Population size cannot be negative or zero')
```

### Comparing `iOpt-0.1.6/examples/Genetic_algorithm/TSP/_2D/Example_GA_TSP_Vary_Mutation_Population_Size.py` & `iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Example_GA_TSP_Vary_Mutation_Population_Size.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from iOpt.method.listener import StaticNDPaintListener, AnimationNDPaintListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
+from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
+
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
 from examples.Genetic_algorithm.TSP._2D.Problems import ga_tsp_2d
 import numpy as np
 import xml.etree.ElementTree as ET
 
 
@@ -25,18 +27,18 @@
     population_size_bound = {'low': 10.0, 'up': 100.0}
     problem = ga_tsp_2d.GA_TSP_2D(tsp_matrix, num_iteration,
                                   mutation_probability_bound, population_size_bound)
 
     method_params = SolverParameters(r=np.double(2.0), itersLimit=300)
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimationNDPaintListener("gatsp_2d_anim_vary_mutation.png", "output",  varsIndxs=[0, 1], toPaintObjFunc=True)
+    apl = AnimatePainterNDListener("gatsp_2d_anim_vary_mutation.png", "output",  varsIndxs=[0, 1], toPaintObjFunc=True)
     solver.AddListener(apl)
 
-    spl = StaticNDPaintListener("gatsp_2d_stat_vary_mutation.png", "output", varsIndxs=[0, 1], mode="interpolation")
+    spl = StaticPainterNDListener("gatsp_2d_stat_vary_mutation.png", "output", varsIndxs=[0, 1], mode="interpolation")
     solver.AddListener(spl)
 
     solver_info = solver.Solve()
     print(solver_info.numberOfGlobalTrials)
     print(solver_info.numberOfLocalTrials)
     print(solver_info.solvingTime)
```

### Comparing `iOpt-0.1.6/examples/Genetic_algorithm/TSP/_2D/Problems/ga_tsp_2d.py` & `iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Problems/ga_tsp_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         :param num_iteration: Максимальное число итераций генетического алгоритма
         :param population_size_bound: Границы изменения размера популяции (low - нижняя граница, up - верхняя)
         :param mutation_probability_bound: Границы изменения вероятности мутации (low - нижняя граница, up - верхняя)
         """
         super(GA_TSP_2D, self).__init__()
         self.dimension = 2
         self.numberOfFloatVariables = 2
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
         self.costMatrix = cost_matrix
         # Проверка корректности числа итераций метода
         if num_iteration <= 0:
             raise ValueError('The number of iterations cannot be zero or negative.')
         # Проверка валидности интервала вероятностей мутации
```

### Comparing `iOpt-0.1.6/examples/Grishagin_example.py` & `iOpt-0.2.1/examples/Rastrigin_example.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from iOpt.problems.grishagin import Grishagin
+from iOpt.trial import Point
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticNDPaintListener, ConsoleFullOutputListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 if __name__ == "__main__":
     """
-    Минимизация тестовой функции Гришагина с визуализацией
+    Минимизация тестовой функции Растригина с визуализацией
     """
 
-    # создание объекта задачи
-    problem = Grishagin(1)
-
-    # Формируем параметры решателя
-    params = SolverParameters(r=2.5, eps=0.01, itersLimit=300, refineSolution=True)
-
-    # Создаем решатель
-    solver = Solver(problem, parameters=params)
-
-    # Добавляем вывод результатов в консоль
-    cfol = ConsoleFullOutputListener(mode='full')
+    # Создание тестовой задачи
+    problem = Rastrigin(dimension=2)
+    # Начальная точка
+    startPoint: Point = Point(floatVariables=[0.5, 0.5], discreteVariables=None)
+    # Параметры решателя
+    params = SolverParameters(r=2.5, eps=0.01, itersLimit=300, refineSolution=True, startPoint=startPoint)
+    # Создание решателя
+    solver = Solver(problem=problem, parameters=params)
+    # Вывод результатов в консоль в процессе решения задачи
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
-
-    # Добавляем построение 3D визуализации после решения задачи
-    spl = StaticNDPaintListener("grishagin.png", "output", varsIndxs=[0, 1], mode="lines layers",
-                                calc="objective function")
+    # 3D визуализация по окончании решения задачи
+    spl = StaticPainterNDListener(fileName="rastrigin.png", pathForSaves="output", varsIndxs=[0, 1], mode="surface",
+                                  calc="interpolation")
     solver.AddListener(spl)
-
-    # Решение задачи
+    # Запуск решения задачи
     sol = solver.Solve()
+
```

### Comparing `iOpt-0.1.6/examples/Hill_example.py` & `iOpt-0.2.1/examples/Hill_example.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from iOpt.problems.hill import Hill
+from problems.hill import Hill
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticPaintListener, ConsoleFullOutputListener
+from iOpt.output_system.listeners.static_painters import StaticPainterListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 if __name__ == "__main__":
     """
     Минимизация тестовой функции Хилла c визуализацией
     """
 
     # создание объекта задачи
-    problem = Hill(0)
+    problem = Hill(function_number=5)
 
     # Формируем параметры решателя
     params = SolverParameters(r=3, eps=0.01, itersLimit=300, refineSolution=True)
 
     # Создаем решатель
-    solver = Solver(problem, parameters=params)
+    solver = Solver(problem=problem, parameters=params)
 
     # Добавляем вывод результатов в консоль
-    cfol = ConsoleFullOutputListener(mode='full')
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
 
     # Добавляем построение визуализации после решения задачи
-    spl = StaticPaintListener("hill.png", "output", indx=0, isPointsAtBottom=False, mode="objective function")
+    spl = StaticPainterListener("hill.png", "output", indx=0, isPointsAtBottom=False, mode="objective function")
     solver.AddListener(spl)
 
     # Решение задачи
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_kernel_coefficient.py` & `iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_kernel_coefficient.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from iOpt.method.listener import StaticPaintListener, AnimationPaintListener
+from iOpt.output_system.listeners.static_painters import StaticPainterListener
+from iOpt.output_system.listeners.animate_painters import AnimatePainterListener
+
 from sklearn.datasets import load_breast_cancer
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
 from examples.Machine_learning.SVC._1D.Problems import SVC_Fixed_Kernel
 from sklearn.utils import shuffle
 import numpy as np
 
@@ -19,18 +21,18 @@
     kernel_coefficient = -5
     regularization_value_bound = {'low': 1, 'up': 6}
     problem = SVC_Fixed_Kernel.SVC_Fixed_Kernel(x, y, kernel_coefficient, regularization_value_bound)
 
     method_params = SolverParameters(r=np.double(3.0), eps=np.double(0.05))
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimationPaintListener("svc1d_anim.png", "output", toPaintObjFunc=True)
+    apl = AnimatePainterListener("svc1d_anim.png", "output", toPaintObjFunc=True)
     solver.AddListener(apl)
 
-    spl = StaticPaintListener("svc1d_stat.png", "output", mode="interpolation")
+    spl = StaticPainterListener("svc1d_stat.png", "output", mode="interpolation")
     solver.AddListener(spl)
 
     solver_info = solver.Solve()
     print(solver_info.numberOfGlobalTrials)
     print(solver_info.numberOfLocalTrials)
     print(solver_info.solvingTime)
```

### Comparing `iOpt-0.1.6/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_regularization.py` & `iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_regularization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from iOpt.method.listener import StaticPaintListener, AnimationPaintListener
+from iOpt.output_system.listeners.static_painters import StaticPainterListener
+from iOpt.output_system.listeners.animate_painters import AnimatePainterListener
 from sklearn.datasets import load_breast_cancer
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
 from examples.Machine_learning.SVC._1D.Problems import SVC_Fixed_Regularization
 from sklearn.utils import shuffle
 import numpy as np
 
@@ -19,18 +20,18 @@
     regularization_value = 6
     kernel_coefficient_bound = {'low': -7, 'up': -3}
     problem = SVC_Fixed_Regularization.SVC_Fixed_Regularization(x, y, regularization_value, kernel_coefficient_bound)
 
     method_params = SolverParameters(r=np.double(3.0), itersLimit=10, eps=np.double(0.05))
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimationPaintListener("svc1d_anim.png", "output", toPaintObjFunc=True)
+    apl = AnimatePainterListener("svc1d_anim.png", "output", toPaintObjFunc=True)
     solver.AddListener(apl)
 
-    spl = StaticPaintListener("svc1d_stat.png", "output", mode="interpolation")
+    spl = StaticPainterListener("svc1d_stat.png", "output", mode="interpolation")
     solver.AddListener(spl)
 
     solver_info = solver.Solve()
     print(solver_info.numberOfGlobalTrials)
     print(solver_info.numberOfLocalTrials)
     print(solver_info.solvingTime)
```

### Comparing `iOpt-0.1.6/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Kernel.py` & `iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
-from iOpt.trial import Trial
 from iOpt.problem import Problem
-from sko.GA import GA_TSP
 from sklearn.metrics import f1_score
 from sklearn.svm import SVC
 from sklearn.model_selection import cross_val_score
 from typing import Dict
 
 
 class SVC_Fixed_Kernel(Problem):
@@ -27,15 +25,15 @@
         :param y_dataset: выходные данные обучающе выборки метода SVC
         :param kernel_coefficient_value: Значение коэфицента ядра
         :param regularization_bound: Границы изменения параметра регуляризации (low - нижняя граница, up - верхняя)
         """
         super(SVC_Fixed_Kernel, self).__init__()
         self.dimension = 1
         self.numberOfFloatVariables = 1
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
         if x_dataset.shape[0] != y_dataset.shape[0]:
             raise ValueError('The input and output sample sizes do not match.')
         self.x = x_dataset
         self.y = y_dataset
         self.kernelCoefficient = kernel_coefficient_value
```

### Comparing `iOpt-0.1.6/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Regularization.py` & `iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Regularization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
-from iOpt.trial import Trial
 from iOpt.problem import Problem
-from sko.GA import GA_TSP
 from sklearn.metrics import f1_score
 from sklearn.svm import SVC
 from sklearn.model_selection import cross_val_score
 from typing import Dict
 
 
 class SVC_Fixed_Regularization(Problem):
@@ -27,15 +25,15 @@
         :param y_dataset: выходные данные обучающе выборки метода SVC
         :param regularization_value: Значение параметра регуляризации
         :param kernel_coefficient_bound: Границы изменения значений коэфицента ядра (low - нижняя граница, up - верхняя)
         """
         super(SVC_Fixed_Regularization, self).__init__()
         self.dimension = 1
         self.numberOfFloatVariables = 1
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
         if x_dataset.shape[0] != y_dataset.shape[0]:
             raise ValueError('The input and output sample sizes do not match.')
         self.x = x_dataset
         self.y = y_dataset
         self.regularizationValue = regularization_value
```

### Comparing `iOpt-0.1.6/examples/Machine_learning/SVC/_2D/Example_2D_SVC.py` & `iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Example_2D_SVC.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from iOpt.method.listener import StaticNDPaintListener, AnimationNDPaintListener, ConsoleFullOutputListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
+from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
+
 from sklearn.datasets import load_breast_cancer
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
 from examples.Machine_learning.SVC._2D.Problems import SVC_2d
 from sklearn.utils import shuffle
 import numpy as np
 
@@ -20,17 +23,17 @@
     kernel_coefficient_bound = {'low': -7, 'up': -3}
 
     problem = SVC_2d.SVC_2D(x, y, regularization_value_bound, kernel_coefficient_bound)
 
     method_params = SolverParameters(r=np.double(3.0), itersLimit=100)
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimationNDPaintListener("svc2d_anim.png", "output", varsIndxs=[0, 1], toPaintObjFunc=False)
+    apl = AnimatePainterNDListener("svc2d_anim.png", "output", varsIndxs=[0, 1], toPaintObjFunc=False)
     solver.AddListener(apl)
 
-    spl = StaticNDPaintListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
+    spl = StaticPainterNDListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
     solver.AddListener(spl)
 
-    cfol = ConsoleFullOutputListener(mode='full')
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
 
     solver_info = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/Machine_learning/SVC/_2D/Example_2D_SVC_Industrial.py` & `iOpt-0.2.1/examples/Machine_learning/SVC/_3D/Example_SVC_Discrete_Param.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-from iOpt.method.listener import StaticNDPaintListener, AnimationNDPaintListener, ConsoleFullOutputListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
+from iOpt.output_system.listeners.static_painters import StaticDiscreteListener
+from sklearn.datasets import load_breast_cancer
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from examples.Machine_learning.SVC._2D.Problems import SVC_2d
+from examples.Machine_learning.SVC._3D.Problem import SVC_3D
 from sklearn.utils import shuffle
-import numpy as np
-import pandas as pd
 
-def get_SCANIA_dataset():
-    xls = pd.read_excel(r"../Datasets/aps_failure_training_set1.xls", header=None)
-    data = xls.values[1:]
-    row, col = data.shape
-    _x = data[:, 1:col]
-    _y = data[:, 0]
-    y = np.array(_y, dtype=np.double)
-    x = np.array(_x, dtype=np.double)
-    return shuffle(x, y, random_state=42)
+def load_breast_cancer_data():
+    dataset = load_breast_cancer()
+    x_raw, y_raw = dataset['data'], dataset['target']
+    inputs, outputs = shuffle(x_raw, y_raw ^ 1, random_state=42)
+    return inputs, outputs
+
 if __name__ == "__main__":
-    X, Y = get_SCANIA_dataset()
-    x = X[:2000]
-    y = Y[:2000]
+    x, y = load_breast_cancer_data()
     regularization_value_bound = {'low': 1, 'up': 10}
-    kernel_coefficient_bound = {'low': -8, 'up': -1}
-    problem = SVC_2d.SVC_2D(x, y, regularization_value_bound, kernel_coefficient_bound)
-    method_params = SolverParameters(r=np.double(2.0), itersLimit=200)
+    kernel_coefficient_bound = {'low': -9, 'up': -6.7}
+    kernel_type = {'kernel': ['rbf', 'sigmoid', 'poly']}
+    problem = SVC_3D.SVC_3D(x, y, regularization_value_bound, kernel_coefficient_bound, kernel_type)
+    method_params = SolverParameters(itersLimit=400)
     solver = Solver(problem, parameters=method_params)
-    apl = AnimationNDPaintListener("svc2d_anim.png", "output", varsIndxs=[0, 1], toPaintObjFunc=False)
+    apl = StaticDiscreteListener("experiment1.png", mode='analysis')
+    solver.AddListener(apl)
+    apl = StaticDiscreteListener("experiment2.png", mode='bestcombination', calc='interpolation', mrkrs=4)
     solver.AddListener(apl)
-    spl = StaticNDPaintListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
-    solver.AddListener(spl)
-    cfol = ConsoleFullOutputListener(mode='full')
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
-    solver_info = solver.Solve()
+    solver_info = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/Machine_learning/SVC/_2D/Problems/SVC_2d.py` & `iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Problems/SVC_2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
-from iOpt.trial import Trial
 from iOpt.problem import Problem
-from sklearn.metrics import f1_score
 from sklearn.svm import SVC
 from sklearn.model_selection import cross_val_score
 from typing import Dict
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import StandardScaler
 
 class SVC_2D(Problem):
@@ -28,31 +26,33 @@
         :param y_dataset: выходные данные обучающе выборки метода SVC
         :param kernel_coefficient_bound: Значение параметра регуляризации
         :param regularization_bound: Границы изменения значений коэфицента ядра (low - нижняя граница, up - верхняя)
         """
         super(SVC_2D, self).__init__()
         self.dimension = 2
         self.numberOfFloatVariables = 2
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
         if x_dataset.shape[0] != y_dataset.shape[0]:
             raise ValueError('The input and output sample sizes do not match.')
         self.x = x_dataset
         self.y = y_dataset
         self.floatVariableNames = np.array(["Regularization parameter", "Kernel coefficient"], dtype=str)
         self.lowerBoundOfFloatVariables = np.array([regularization_bound['low'], kernel_coefficient_bound['low']],
                                                    dtype=np.double)
         self.upperBoundOfFloatVariables = np.array([regularization_bound['up'], kernel_coefficient_bound['up']],
                                                    dtype=np.double)
 
+
+
     def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
         """
         Метод расчёта значения целевой функции в точке
 
         :param point: Точка испытания
         :param functionValue: объект хранения значения целевой функции в точке
         """
         cs, gammas = point.floatVariables[0], point.floatVariables[1]
-        clf = Pipeline([('scaler', StandardScaler()), ('model', SVC(C=10 ** cs, gamma=10 ** gammas))])
+        clf = SVC(C=10 ** cs, gamma=10 ** gammas)
         functionValue.value = -cross_val_score(clf, self.x, self.y, scoring='f1').mean()
         return functionValue
```

### Comparing `iOpt-0.1.6/examples/Rastrigin_example.py` & `iOpt-0.2.1/examples/RastriginInt_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from iOpt.problems.rastrigin import Rastrigin
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticNDPaintListener, ConsoleFullOutputListener
-
-from subprocess import Popen, PIPE, STDOUT
+from iOpt.trial import Point
+from problems.rastriginInt import RastriginInt
 
 if __name__ == "__main__":
     """
     Минимизация тестовой функции Растригина с визуализацией
     """
 
     # Создание тестовой задачи
-    problem = Rastrigin(2)
+    problem = RastriginInt(dimension=5, numberOfDiscreteVariables=3)
+    # Начальная точка
+    startPoint: Point = Point(floatVariables=[0.5, 0.5], discreteVariables=['A', 'B', 'A'])
     # Параметры решателя
-    params = SolverParameters(r=2.5, eps=0.01, itersLimit=300, refineSolution=True)
+    params = SolverParameters(r=2.5, eps=0.01, itersLimit=10000, startPoint=startPoint, numberOfParallelPoints=16)
     # Создание решателя
-    solver = Solver(problem, parameters=params)
+    solver = Solver(problem=problem, parameters=params)
     # Вывод результатов в консоль в процессе решения задачи
-    cfol = ConsoleFullOutputListener(mode='full')
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
     # 3D визуализация по окончании решения задачи
-    spl = StaticNDPaintListener("rastrigin.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
-    solver.AddListener(spl)
+
     # Запуск решения задачи
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/Shekel4_example.py` & `iOpt-0.2.1/examples/Shekel4_example.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from iOpt.problems.shekel4 import Shekel4
+from problems.shekel4 import Shekel4
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import ConsoleFullOutputListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 if __name__ == "__main__":
     """
     Минимизация тестовой функции Шекеля (размерность = 4)
     """
 
     # создание объекта задачи
-    problem = Shekel4(1)
+    problem = Shekel4(function_number=1)
 
     # Формируем параметры решателя
     params = SolverParameters(r=2.5, eps=0.01, itersLimit=10000, refineSolution=True)
 
     # Создаем решатель
-    solver = Solver(problem, parameters=params)
+    solver = Solver(problem=problem, parameters=params)
 
     # Добавляем вывод результатов в консоль
-    cfol = ConsoleFullOutputListener(mode='full')
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
 
     # Решение задачи
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/Shekel_example.py` & `iOpt-0.2.1/examples/GKLS_example.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-from iOpt.problems.shekel import Shekel
+from problems.GKLS import GKLS
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticPaintListener, ConsoleFullOutputListener
 
-if __name__ == "__main__":
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
+
+
+def SolveSingleGKLS():
     """
-    Минимизация тестовой функции Шекеля
+    Минимизация тестовой функции из GKLS генератора с номером 39
     """
 
     # создание объекта задачи
-    problem = Shekel(0)
+    problem = GKLS(dimension=2, functionNumber=39)
 
     # Формируем параметры решателя
-    params = SolverParameters(r=3, eps=0.01, itersLimit=300, refineSolution=True)
+    params = SolverParameters(r=3.5, eps=0.01, itersLimit=300, refineSolution=True, numberOfParallelPoints=4)
 
     # Создаем решатель
-    solver = Solver(problem, parameters=params)
+    solver = Solver(problem=problem, parameters=params)
 
-    # Добавляем вывод результатов в консоль
-    cfol = ConsoleFullOutputListener(mode='full')
+    # Добавляем вывод резултатов в консоль
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
 
-    # Добавляем построение визуализации после решения задачи
-    spl = StaticPaintListener("shekel.png", "output", indx=0, isPointsAtBottom=False, mode="objective function")
+    # Добавляем построение 3D визуализации после решения задачи
+    spl = StaticPainterNDListener(fileName="GKLS.png", pathForSaves="output", varsIndxs=[0, 1], mode="lines layers",
+                                  calc="objective function")
     solver.AddListener(spl)
 
     # Решение задачи
     sol = solver.Solve()
+
+
+if __name__ == "__main__":
+    SolveSingleGKLS()
```

### Comparing `iOpt-0.1.6/examples/console_output/example_custom_output.py` & `iOpt-0.2.1/examples/console_output/example_custom_output.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import ConsoleFullOutputListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 if __name__ == "__main__":
     # create the problem
     problem = Rastrigin(2)
 
     # add solver parameters
     params = SolverParameters(r=3.5, eps=0.001)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    cfol = ConsoleFullOutputListener(mode="custom", iters=400)
+    cfol = ConsoleOutputListener(mode="custom", iters=400)
     solver.AddListener(cfol)
 
     # solve the problem
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/console_output/example_full_output.py` & `iOpt-0.2.1/examples/console_output/example_only_result_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import ConsoleFullOutputListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 if __name__ == "__main__":
     # create the problem
-    problem = Rastrigin(1)
+    problem = Rastrigin(2)
 
     # add solver parameters
     params = SolverParameters(r=3.5, eps=0.001)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    cfol = ConsoleFullOutputListener(mode="full")
+    cfol = ConsoleOutputListener(mode="result")
     solver.AddListener(cfol)
 
     # solve the problem
     sol = solver.Solve()
-
```

### Comparing `iOpt-0.1.6/examples/console_output/example_only_result_output.py` & `iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_only_points.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import ConsoleFullOutputListener
+from iOpt.output_system.listeners.static_painters import StaticPainterListener
 
 if __name__ == "__main__":
-    # create the problem
-    problem = Rastrigin(2)
+    # create the problem 1D dimension
+    problem = Rastrigin(1)
 
     # add solver parameters
-    params = SolverParameters(r=3.5, eps=0.001)
+    params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    cfol = ConsoleFullOutputListener(mode="result")
-    solver.AddListener(cfol)
+    apl = StaticPainterListener("rastrigin_1_2.5_0.01.png", mode="only points")
+    solver.AddListener(apl)
 
     # solve the problem
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/dynamic_painters/1D_examples/example_1D_with_objective_function.py` & `iOpt-0.2.1/examples/dynamic_painters/1D_examples/example_1D_with_objective_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import AnimationPaintListener
+from iOpt.output_system.listeners.animate_painters import AnimatePainterListener
 
 if __name__ == "__main__":
     # create the problem 1D dimension
     problem = Rastrigin(1)
 
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = AnimationPaintListener("rastrigin_1_2.5_0.01.png")
+    apl = AnimatePainterListener("rastrigin_1_2.5_0.01.png")
     solver.AddListener(apl)
 
     # solve the problem
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/dynamic_painters/2D_examples/example_2D_with_level_lines.py` & `iOpt-0.2.1/examples/console_output/example_full_output.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from iOpt.problems.xsquared import XSquared
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import AnimationNDPaintListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 if __name__ == "__main__":
-    # create the problem 2D dimension
-    problem = XSquared(2)
+    # create the problem
+    problem = Rastrigin(1)
 
     # add solver parameters
-    params = SolverParameters(r=2.5, eps=0.01)
+    params = SolverParameters(r=3.5, eps=0.001)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = AnimationNDPaintListener("xsquared_1_2.5_0.01.png")
-    solver.AddListener(apl)
+    cfol = ConsoleOutputListener(mode="full")
+    solver.AddListener(cfol)
 
     # solve the problem
     sol = solver.Solve()
+
```

### Comparing `iOpt-0.1.6/examples/static_painters/1D_examples/example_1D_with_approximation.py` & `iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_approximation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticPaintListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 
 if __name__ == "__main__":
-    # create the problem 1D dimension
-    problem = Rastrigin(1)
+    # create the problem 2D dimension
+    problem = Rastrigin(2)
 
     # add solver parameters
-    params = SolverParameters(r=3, eps=0.01)
+    params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticPaintListener("rastrigin_1_3_0.01.png", mode="approximation")
+    apl = StaticPainterNDListener("rastrigin_2_2.5_0.01_approx.png", mode='surface', calc='approximation')
     solver.AddListener(apl)
 
     # solve the problem
     sol = solver.Solve()
-
```

### Comparing `iOpt-0.1.6/examples/static_painters/1D_examples/example_1D_with_interpolation.py` & `iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_interpolation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticPaintListener
-from iOpt.method.listener import ConsoleFullOutputListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 
 if __name__ == "__main__":
     # create the problem 2D dimension
-    problem = Rastrigin(1)
+    problem = Rastrigin(2)
 
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticPaintListener("rastrigin_1_2.5_0.01.png", mode="interpolation")
+    apl = StaticPainterNDListener("rastrigin_2_2.5_0.01_interp.png", mode='surface', calc='interpolation')
     solver.AddListener(apl)
 
     # solve the problem
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/static_painters/1D_examples/example_1D_with_objective_function_pointsInBottom_mode.py` & `iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_objective_function_pointsInBottom_mode.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from iOpt.problems.xsquared import XSquared
+from problems.xsquared import XSquared
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticPaintListener
+from iOpt.output_system.listeners.static_painters import StaticPainterListener
 
 if __name__ == "__main__":
     # create the problem 1D dimension
     problem = XSquared(1)
 
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticPaintListener("xsquared_1_2.5_0.01.png", isPointsAtBottom=True)
+    apl = StaticPainterListener("xsquared_1_2.5_0.01.png", isPointsAtBottom=True)
     solver.AddListener(apl)
 
     # solve the problem
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/static_painters/1D_examples/example_1D_with_only_points.py` & `iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_interpolation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticPaintListener
+from iOpt.output_system.listeners.static_painters import StaticPainterListener
 
 if __name__ == "__main__":
-    # create the problem 1D dimension
+    # create the problem 2D dimension
     problem = Rastrigin(1)
 
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticPaintListener("rastrigin_1_2.5_0.01.png", mode="only points")
+    apl = StaticPainterListener("rastrigin_1_2.5_0.01.png", mode="interpolation")
     solver.AddListener(apl)
 
     # solve the problem
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/static_painters/2D_examples/example_2D_with_1-dimension_section.py` & `iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_1-dimension_section.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticPaintListener
+from iOpt.output_system.listeners.static_painters import StaticPainterListener
 
 if __name__ == "__main__":
     # create the problem 2D dimension
     problem = Rastrigin(2)
 
     # add solver parameters
     params = SolverParameters(r=3.5, eps=0.001)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl_0 = StaticPaintListener("rastrigin_2_3.5_0.001_static1D_0.png", "output", indx=0)
-    apl_1 = StaticPaintListener("rastrigin_2_3.5_0.001_static1D_1.png", "output", indx=1)
+    apl_0 = StaticPainterListener("rastrigin_2_3.5_0.001_static1D_0.png", "output", indx=0)
+    apl_1 = StaticPainterListener("rastrigin_2_3.5_0.001_static1D_1.png", "output", indx=1)
     solver.AddListener(apl_0)
     solver.AddListener(apl_1)
 
     # solve the problem
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/static_painters/2D_examples/example_2D_with_approximation.py` & `iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_level_lines.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from iOpt.problems.rastrigin import Rastrigin
+from problems.xsquared import XSquared
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticNDPaintListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 
 if __name__ == "__main__":
     # create the problem 2D dimension
-    problem = Rastrigin(2)
+    problem = XSquared(2)
 
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticNDPaintListener("rastrigin_2_2.5_0.01_approx.png", mode='surface', calc='approximation')
+    apl = StaticPainterNDListener("xsquared_2_2.5_0.01.png", mode='lines layers')
     solver.AddListener(apl)
 
     # solve the problem
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/static_painters/2D_examples/example_2D_with_interpolation.py` & `iOpt-0.2.1/examples/dynamic_painters/2D_examples/example_2D_with_level_lines.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-from iOpt.problems.rastrigin import Rastrigin
+from problems.xsquared import XSquared
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticNDPaintListener
+
+from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 if __name__ == "__main__":
     # create the problem 2D dimension
-    problem = Rastrigin(2)
+    problem = XSquared(2)
 
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
+    cfol = ConsoleOutputListener(mode="full")
+    solver.AddListener(cfol)
+
     # add needed listeners for solver
-    apl = StaticNDPaintListener("rastrigin_2_2.5_0.01_interp.png", mode='surface', calc='interpolation')
+    apl = AnimatePainterNDListener("xsquared_1_2.5_0.01.png")
     solver.AddListener(apl)
 
     # solve the problem
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/examples/static_painters/2D_examples/example_2D_with_level_lines.py` & `iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_approximation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from iOpt.problems.xsquared import XSquared
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticNDPaintListener
+from iOpt.output_system.listeners.static_painters import StaticPainterListener
 
 if __name__ == "__main__":
-    # create the problem 2D dimension
-    problem = XSquared(2)
+    # create the problem 1D dimension
+    problem = Rastrigin(1)
 
     # add solver parameters
-    params = SolverParameters(r=2.5, eps=0.01)
+    params = SolverParameters(r=3, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticNDPaintListener("xsquared_2_2.5_0.01.png", mode='lines layers')
+    apl = StaticPainterListener("rastrigin_1_3_0.01.png", mode="approximation")
     solver.AddListener(apl)
 
     # solve the problem
     sol = solver.Solve()
+
```

### Comparing `iOpt-0.1.6/examples/static_painters/2D_examples/example_2D_with_level_lines_by_interpolation.py` & `iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_level_lines_by_interpolation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticNDPaintListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 
 if __name__ == "__main__":
     # create the problem 2D dimension
     problem = Rastrigin(2)
 
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticNDPaintListener("xsquared_2_2.5_0.01_interp.png", mode='lines layers', calc='interpolation')
+    apl = StaticPainterNDListener("xsquared_2_2.5_0.01_interp.png", mode='lines layers', calc='interpolation')
     solver.AddListener(apl)
 
     # solve the problem
     sol = solver.Solve()
```

### Comparing `iOpt-0.1.6/iOpt/evolvent/evolvent.py` & `iOpt-0.2.1/iOpt/evolvent/evolvent.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     def __GetYonX(self, _x: np.double) -> np.ndarray(shape=(1), dtype=np.double):
         if self.numberOfFloatVariables == 1:
             self.yValues[0] = _x - 0.5
             return self.yValues
 
         iu: np.narray(shape=(1), dtype=np.int32)
         iv: np.narray(shape=(1), dtype=np.int32)
-        l: np.int32
+        node: np.int32
         d: np.double = 0.0
         # mn: np.int32
         r: np.double
         iw: np.narray(shape=(1), dtype=np.int32)
         it: np.int32
         i: np.int32
         j: np.int32
@@ -154,32 +154,32 @@
                 d = 0.0
             else:
                 d *= self.nexpExtended
                 iis = int(d)
                 d -= iis
 
                 # print(iis, self.numberOfFloatVariables)
-            l = self.__CalculateNode(iis, self.numberOfFloatVariables, iu, iv)
-            # print(j, l)
+            node = self.__CalculateNode(iis, self.numberOfFloatVariables, iu, iv)
+            # print(j, node)
 
             # заменить на () = () !
             i = iu[0]
             iu[0] = iu[it]
             iu[it] = i
             i = iv[0]
             iv[0] = iv[it]
             iv[it] = i
 
-            if l == 0:
-                l = it
-            elif l == it:
-                l = 0
+            if node == 0:
+                node = it
+            elif node == it:
+                node = 0
 
             r *= 0.5
-            it = l
+            it = node
             for i in range(0, self.numberOfFloatVariables):
                 iu[i] *= iw[i]
                 iw[i] *= -iv[i]
                 self.yValues[i] += r * iu[i]
 
         return np.copy(self.yValues)
 
@@ -193,15 +193,15 @@
         u: np.narray(shape=(1), dtype=np.int32)
         v: np.narray(shape=(1), dtype=np.int32)
         w: np.narray(shape=(1), dtype=np.int32)
         r: np.double = 0.0
         i: np.int32
         j: np.int32
         it: np.int32
-        l: np.int32
+        node: np.int32
         r1: np.double
         iis: np.double
         w = np.ones(self.numberOfFloatVariables, dtype=np.int32)
         u = np.zeros(self.numberOfFloatVariables, dtype=np.int32)
         v = np.zeros(self.numberOfFloatVariables, dtype=np.int32)
         r = 0.5
         r1 = 1.0
@@ -219,121 +219,121 @@
                 self.yValues[i] -= r * u[i]
                 u[i] *= w[i]
 
             i = u[0]
             u[0] = u[it]
             u[it] = i
 
-            iis, l, v = self.__CalculateNumbr(u, v)
+            iis, node, v = self.__CalculateNumbr(u, v)
             # print(u)
             # print(v)
-            # print(iis, l)
+            # print(iis, node)
 
             i = v[0]
             v[0] = v[it]
             v[it] = i
 
             for i in range(0, self.numberOfFloatVariables):
                 w[i] *= -v[i]
 
-            if l == 0:
-                l = it
-            elif l == it:
-                l = 0
+            if node == 0:
+                node = it
+            elif node == it:
+                node = 0
 
-            it = l
+            it = node
             r1 = r1 / self.nexpExtended
             x += r1 * iis
 
         return x
 
     # -----------------------------------------------------------------------------------------
     def __CalculateNumbr(self,
                          u: np.ndarray(shape=(1), dtype=np.int32),
                          v: np.ndarray(shape=(1), dtype=np.int32)
                          ):
         i = 0
         k1 = -1
         k2 = 0
         l1 = 0
-        l = 0
+        node = 0
         iis: np.double
         iff: np.double
 
         iff = self.nexpExtended
         iis = 0.0
 
         for i in range(0, self.numberOfFloatVariables):
             iff /= 2
             k2 = -k1 * u[i]
             v[i] = u[i]
             k1 = k2
             if k2 < 0:
-                l1 = i
+                node1 = i
             else:
                 iis += iff
-                l = i
+                node = i
 
         if math.isclose(iis, 0.0):
-            l = self.numberOfFloatVariables - 1
+            node = self.numberOfFloatVariables - 1
         else:
             v[self.numberOfFloatVariables - 1] = -v[self.numberOfFloatVariables - 1]
             if math.isclose(iis, self.nexpExtended - 1.0):
-                l = self.numberOfFloatVariables - 1
+                node = self.numberOfFloatVariables - 1
             else:
-                if l1 == self.numberOfFloatVariables - 1:
-                    v[l] = -v[l]
+                if node1 == self.numberOfFloatVariables - 1:
+                    v[node] = -v[node]
                 else:
-                    l = l1
+                    node = node1
         s = iis
 
-        return s, l, v
+        return s, node, v
 
     # -----------------------------------------------------------------------------------------
     def __CalculateNode(self,
                         iis: np.double,
                         n: int,
                         u: np.ndarray(shape=(1), dtype=np.int32),
                         v: np.ndarray(shape=(1), dtype=np.int32),
                         ):
 
         iq = 1
         n1 = n - 1
-        l = 0
+        node = 0
         if math.isclose(iis, 0.0):
-            l = n1
+            node = n1
             for i in range(0, n):
                 u[i] = -1
                 v[i] = -1
         elif math.isclose(iis, self.nexpExtended - 1.0):
-            l = n1
+            node = n1
             u[0] = 1
             v[0] = 1
             for i in range(1, n):
                 u[i] = -1
                 v[i] = -1
             v[n1] = 1
         else:
             iff = self.nexpExtended
             k1 = -1
             for i in range(0, n):
                 iff /= 2
                 if iis >= iff:  # исправить сравнение!
                     if math.isclose(iis, iff) and not math.isclose(iis, 1.0):
-                        l = i
+                        node = i
                         iq = -1
                     iis -= iff
                     k2 = 1
                 else:
                     k2 = -1
                     if math.isclose(iis, (iff - 1.0)) and not math.isclose(iis, 0.0):
-                        l = i
+                        node = i
                         iq = 1
                 j = -k1 * k2
                 v[i] = j
                 u[i] = j
                 k1 = k2
-            v[l] = v[l] * iq
+            v[node] = v[node] * iq
             v[n1] = -v[n1]
-        return l
+        return node
 
 # -----------------------------------------------------------------------------------------
```

### Comparing `iOpt-0.1.6/iOpt/method/method.py` & `iOpt-0.2.1/iOpt/method/method.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 import copy
+import math
+import sys
 from typing import Tuple
 
 import numpy as np
 
 from iOpt.evolvent.evolvent import Evolvent
+from iOpt.method.calculator import Calculator
 from iOpt.method.optim_task import OptimizationTask
 from iOpt.method.search_data import SearchData
 from iOpt.method.search_data import SearchDataItem
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.trial import Point
+from iOpt.trial import Point, FunctionValue
 
 
 class Method:
     """
     Класс Method содержит реализацию Алгоритма Глобального Поиска
     """
 
@@ -29,106 +32,191 @@
 
         :param parameters: параметры решения задачи оптимизации.
         :param task: обёртка решаемой задачи.
         :param evolvent: развертка Пеано-Гильберта, отображающая отрезок [0,1] на многомерную область D.
         :param searchData: структура данных для хранения накопленной поисковой информации.
         """
         self.stop: bool = False
-        self.recalc: bool = True
+        self.recalcR: bool = True
+        self.recalcM: bool = True
         self.iterationsCount: int = 0
         self.best: SearchDataItem = None
 
         self.parameters = parameters
         self.task = task
         self.evolvent = evolvent
         self.searchData = searchData
         # change to np.array, but indexing np is slower
         self.M = [1.0 for _ in range(task.problem.numberOfObjectives + task.problem.numberOfConstraints)]
         self.Z = [np.infty for _ in range(task.problem.numberOfObjectives + task.problem.numberOfConstraints)]
         self.dimension = task.problem.numberOfFloatVariables  # А ДЛЯ ДИСКРЕТНЫХ?
         self.searchData.solution.solutionAccuracy = np.infty
+        self.numberOfAllFunctions = task.problem.numberOfObjectives + task.problem.numberOfConstraints
 
     @property
     def min_delta(self):
         return self.searchData.solution.solutionAccuracy
 
     @min_delta.setter
     def min_delta(self, val):
         self.searchData.solution.solutionAccuracy = val
 
-    @staticmethod
-    def CalculateDelta(lx: float, rx: float, dimension: int) -> float:
+    # @staticmethod
+    # def CalculateDelta(lx: float, rx: float, dimension: int) -> float:
+    #     """
+    #     Вычисляет гельдерово расстояние в метрике Гельдера между двумя точками на отрезке [0,1],
+    #       полученными при редукции размерности.
+    #
+    #     :param lx: левая точка
+    #     :param rx: правая точка
+    #     :param dimension: размерность исходного пространства
+    #
+    #     :return: гельдерово расстояние между lx и rx.
+    #     """
+    #     return pow(rx - lx, 1.0 / dimension)
+
+    def CalculateDelta(self, lPoint: SearchDataItem, rPoint: SearchDataItem, dimension: int) -> float:
         """
         Вычисляет гельдерово расстояние в метрике Гельдера между двумя точками на отрезке [0,1],
           полученными при редукции размерности.
 
-        :param lx: левая точка
-        :param rx: правая точка
+        :param lPoint: левая точка
+        :param rPoint: правая точка
         :param dimension: размерность исходного пространства
 
         :return: гельдерово расстояние между lx и rx.
         """
-        return pow(rx - lx, 1.0 / dimension)
+        return pow(rPoint.GetX() - lPoint.GetX(), 1.0 / dimension)
 
-    def FirstIteration(self) -> None:
+    def FirstIteration(self, calculator: Calculator = None) -> list[SearchDataItem]:
         r"""
         Метод выполняет первую итерацию Алгоритма Глобального Поиска.
         """
-        self.iterationsCount = 1
+
         # Генерация 3х точек 0, 0.5, 1. Значение функции будет вычисляться только в точке 0.5.
         # Интервал задаётся правой точкой, т.е. будут интервалы только для 0.5 и 1
-        x: float = 0.5
-        y = Point(self.evolvent.GetImage(x), None)
-        middle = SearchDataItem(y, x)
-        left = SearchDataItem(Point(self.evolvent.GetImage(0.0), None), 0.0)
-        right = SearchDataItem(Point(self.evolvent.GetImage(1.0), None), 1.0)
+        left = SearchDataItem(Point(self.evolvent.GetImage(0.0), None), 0.,
+                              functionValues=[FunctionValue()] * self.numberOfAllFunctions)
+        right = SearchDataItem(Point(self.evolvent.GetImage(1.0), None), 1.0,
+                               functionValues=[FunctionValue()] * self.numberOfAllFunctions)
+
+        items: list[SearchDataItem] = []
+
+        if self.parameters.startPoint:
+            numberOfPoint: int = self.parameters.numberOfParallelPoints - 1
+            h: float = 1.0 / (numberOfPoint + 1)
+
+            yStartPoint = Point(copy.copy(self.parameters.startPoint.floatVariables), None)
+            xStartPoint = self.evolvent.GetInverseImage(self.parameters.startPoint.floatVariables)
+
+            itemStartPoint = SearchDataItem(yStartPoint, xStartPoint,
+                                  functionValues=[FunctionValue()] * self.numberOfAllFunctions)
+
+            isAddStartPoint: bool = False
+
+            for i in range(numberOfPoint):
+                x = h * (i + 1)
+                y = Point(self.evolvent.GetImage(x), None)
+                item = SearchDataItem(y, x,
+                                      functionValues=[FunctionValue()] * self.numberOfAllFunctions)
+                if x < xStartPoint < h * (i + 2):
+                    items.append(item)
+                    items.append(itemStartPoint)
+                    isAddStartPoint = True
+                else:
+                    items.append(item)
 
-        left.delta = 0
-        middle.delta = Method.CalculateDelta(left.GetX(), middle.GetX(), self.dimension)
-        right.delta = Method.CalculateDelta(middle.GetX(), right.GetX(), self.dimension)
+            if not isAddStartPoint:
+                items.append(itemStartPoint)
+        else:
+
+            numberOfPoint: int = self.parameters.numberOfParallelPoints
+            h: float = 1.0 / (numberOfPoint + 1)
+
+            for i in range(numberOfPoint):
+                x = h * (i + 1)
+                y = Point(self.evolvent.GetImage(x), None)
+                item = SearchDataItem(y, x,
+                                      functionValues=[FunctionValue()] * self.numberOfAllFunctions)
+                items.append(item)
+
+        if calculator is None:
+            for item in items:
+                self.CalculateFunctionals(item)
+        else:
+            calculator.CalculateFunctionalsForItems(items)
 
-        # Вычисление значения функции в 0.5
-        self.CalculateFunctionals(middle)
-        self.UpdateOptimum(middle)
+        for item in items:
+            self.UpdateOptimum(item)
 
-        # Вычисление характеристик
+        left.delta = 0
         self.CalculateGlobalR(left, None)
-        self.CalculateGlobalR(middle, left)
-        self.CalculateGlobalR(right, middle)
+
+        items[0].delta = self.CalculateDelta(left, items[0], self.dimension)
+        self.CalculateGlobalR(items[0], left)
+        for id_item, item in enumerate(items):
+            if id_item > 0:
+                items[id_item].delta = self.CalculateDelta(items[id_item - 1], items[id_item], self.dimension)
+                self.CalculateGlobalR(items[id_item], items[id_item - 1])
+                self.CalculateM(items[id_item], items[id_item - 1])
+
+        right.delta = self.CalculateDelta(items[-1], right, self.dimension)
+        self.CalculateGlobalR(right, items[-1])
 
         # вставить left  и right, потом middle
         self.searchData.InsertFirstDataItem(left, right)
-        self.searchData.InsertDataItem(middle, right)
+        # self.searchData.InsertDataItem(middle, right)
+
+        for item in items:
+            self.searchData.InsertDataItem(item, right)
+
+        self.recalcR = True
+        self.recalcM = True
+
+        self.iterationsCount = len(items)
+        self.searchData.solution.numberOfGlobalTrials = len(items)
+
+        return items
 
     def CheckStopCondition(self) -> bool:
         r"""
         Проверка условия остановки.
         Алгоритм должен завершить работу, когда достигнута точность eps или превышен лимит итераций.
 
         :return: True, если выполнен критерий остановки; False - в противном случае.
         """
-        if self.min_delta < self.parameters.eps or self.iterationsCount >= self.parameters.itersLimit:
+        if self.min_delta < self.parameters.eps or self.iterationsCount >= self.parameters.globalMethodIterationCount:
             self.stop = True
         else:
             self.stop = False
 
         return self.stop
 
+    def RecalcM(self) -> None:
+        r"""
+        Пересчёт оценки константы Липшица.
+        """
+        if self.recalcM is not True:
+            return
+        for item in self.searchData:
+            self.CalculateM(item, item.GetLeft())
+        self.recalcM = False
+
     def RecalcAllCharacteristics(self) -> None:
         r"""
         Пересчёт характеристик для всех поисковых интервалов.
         """
-        if self.recalc is not True:
+        if self.recalcR is not True:
             return
         self.searchData.ClearQueue()
         for item in self.searchData:  # Должно работать...
             self.CalculateGlobalR(item, item.GetLeft())
             # self.CalculateLocalR(item)
         self.searchData.RefillQueue()
-        self.recalc = False
+        self.recalcR = False
 
     def CalculateNextPointCoordinate(self, point: SearchDataItem) -> float:
         r"""
         Вычисление точки нового испытания :math:`x^{k+1}` в заданном интервале :math:`[x_{t-1},x_t]`.
 
         :param point: интервал, заданный его правой точкой :math:`x_t`.
 
@@ -139,15 +227,15 @@
         if left is None:
             print("CalculateNextPointCoordinate: Left point is NONE")
             raise Exception("CalculateNextPointCoordinate: Left point is NONE")
         xl = left.GetX()
         xr = point.GetX()
         idl = left.GetIndex()
         idr = point.GetIndex()
-        if idl == idr:
+        if idl == idr and idl >= 0:
             v = idr
             dif = point.GetZ() - left.GetZ()
             dg = -1.0
             if dif > 0:
                 dg = 1.0
 
             x = 0.5 * (xl + xr)
@@ -163,43 +251,47 @@
     def CalculateIterationPoint(self) -> Tuple[SearchDataItem, SearchDataItem]:  # return  (new, old)
         r"""
         Вычисление точки нового испытания :math:`x^{k+1}`.
 
         :return: :math:`x^{k+1}` - точка нового испытания, и :math:`x_t` - левая точка интервала :math:`[x_{t-1},x_t]`,
           которому принадлежит :math:`x^{k+1}`, т.е. :math:`x^{k+1} \in [x_{t-1},x_t]`.
         """
-        if self.recalc is True:
+        if self.recalcM is True:
+            self.RecalcM()
+        if self.recalcR is True:
             self.RecalcAllCharacteristics()
 
         old = self.searchData.GetDataItemWithMaxGlobalR()
         self.min_delta = min(old.delta, self.min_delta)
         newx = self.CalculateNextPointCoordinate(old)
         newy = self.evolvent.GetImage(newx)
-        new = copy.deepcopy(SearchDataItem(Point(newy, []), newx))
+        new = copy.deepcopy(SearchDataItem(Point(newy, []), newx,
+                                           functionValues=[FunctionValue()] * self.numberOfAllFunctions))
+
+        # Обновление числа испытаний
+        self.searchData.solution.numberOfGlobalTrials += 1
+
         return new, old
 
     def CalculateFunctionals(self, point: SearchDataItem) -> SearchDataItem:
         r"""
         Проведение поискового испытания в заданной точке.
 
         :param point: точка, в которой надо провести испытание.
 
         :return: точка, в которой сохранены результаты испытания.
         """
-        # point.functionValues = np.array(shape=self.task.problem.numberOfObjectives, dtype=FunctionValue)
-        # for func_id in range(self.task.problem.numberOfObjectives):  # make Calculate Objectives?
-        #    self.task.Calculate(point, func_id)  # SetZ, BUT
-
-        # Завернуть в цикл для индексной схемы
-        point = self.task.Calculate(point, 0)
-        point.SetZ(point.functionValues[0].value)
-        point.SetIndex(0)
+        try:
+            point = self.task.Calculate(point, 0)
+            point.SetZ(point.functionValues[0].value)
+            point.SetIndex(0)
+        except Exception:
+            point.SetZ(sys.float_info.max)
+            point.SetIndex(-10)
 
-        # Обновление числа испытаний
-        self.searchData.solution.numberOfGlobalTrials += 1
         return point
 
     def CalculateM(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
         r"""
         Вычисление оценки константы Гельдера между между curr_point и left_point.
 
         :param curr_point: правая точка интервала
@@ -207,19 +299,19 @@
         """
         if curr_point is None:
             print("CalculateM: curr_point is None")
             raise RuntimeError("CalculateM: curr_point is None")
         if left_point is None:
             return
         index = curr_point.GetIndex()
-        if left_point.GetIndex() == index:  # А если не равны, то надо искать ближайший левый/правый с таким индексом
+        if left_point.GetIndex() == index and index >= 0:  # А если не равны, то надо искать ближайший левый/правый с таким индексом
             m = abs(left_point.GetZ() - curr_point.GetZ()) / curr_point.delta
             if m > self.M[index]:
                 self.M[index] = m
-                self.recalc = True
+                self.recalcR = True
 
     # def CalculateM(self, point: SearchDataItem):  # В python нет такой перегрузки функций, надо менять название
     #     self.CalculateM(point, point.GetLeft())
 
     def CalculateGlobalR(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
         r"""
         Вычисление глобальной характеристики интервала [left_point, curr_point].
@@ -233,15 +325,18 @@
         if left_point is None:
             curr_point.globalR = -np.infty
             return None
         zl = left_point.GetZ()
         zr = curr_point.GetZ()
         r = self.parameters.r
         deltax = curr_point.delta
-        if left_point.GetIndex() == curr_point.GetIndex():
+
+        if left_point.GetIndex() < 0 and curr_point.GetIndex() < 0:
+            globalR = 2 * deltax - 4 * math.fabs(self.Z[0]) / (r * self.M[0])
+        elif left_point.GetIndex() == curr_point.GetIndex():
             v = curr_point.GetIndex()
             globalR = deltax + (zr - zl) * (zr - zl) / (deltax * self.M[v] * self.M[v] * r * r) - \
                       2 * (zr + zl - 2 * self.Z[v]) / (r * self.M[v])
         elif left_point.GetIndex() < curr_point.GetIndex():
             v = curr_point.GetIndex()
             globalR = 2 * deltax - 4 * (zr - self.Z[v]) / (r * self.M[v])
         else:
@@ -254,16 +349,19 @@
         Метод обновляет всю поисковую информацию: длины интервалов, константы Гёльдера, все характеристики и вставляет
           новую точку в хранилище.
 
         :param newpoint: новая точка
         :param oldpoint: правая точка интервала, которому принадлежит новая точка
         """
 
-        oldpoint.delta = Method.CalculateDelta(newpoint.GetX(), oldpoint.GetX(), self.dimension)
-        newpoint.delta = Method.CalculateDelta(oldpoint.GetLeft().GetX(), newpoint.GetX(), self.dimension)
+        # oldpoint.delta = Method.CalculateDelta(newpoint.GetX(), oldpoint.GetX(), self.dimension)
+        # newpoint.delta = Method.CalculateDelta(oldpoint.GetLeft().GetX(), newpoint.GetX(), self.dimension)
+
+        oldpoint.delta = self.CalculateDelta(newpoint, oldpoint, self.dimension)
+        newpoint.delta = self.CalculateDelta(oldpoint.GetLeft(), newpoint, self.dimension)
 
         self.CalculateM(newpoint, oldpoint.GetLeft())
         self.CalculateM(oldpoint, newpoint)
 
         self.CalculateGlobalR(newpoint, oldpoint.GetLeft())
         self.CalculateGlobalR(oldpoint, newpoint)
 
@@ -273,19 +371,19 @@
         r"""
         Обновляет оценку оптимума.
 
         :param point: точка нового испытания.
         """
         if self.best is None or self.best.GetIndex() < point.GetIndex():
             self.best = point
-            self.recalc = True
+            self.recalcR = True
             self.Z[point.GetIndex()] = point.GetZ()
         elif self.best.GetIndex() == point.GetIndex() and point.GetZ() < self.best.GetZ():
             self.best = point
-            self.recalc = True
+            self.recalcR = True
             self.Z[point.GetIndex()] = point.GetZ()
         self.searchData.solution.bestTrials[0] = self.best
 
     def FinalizeIteration(self) -> None:
         r"""
         Заканчивает итерацию, обновляет счётчик итераций.
         """
```

### Comparing `iOpt-0.1.6/iOpt/method/optim_task.py` & `iOpt-0.2.1/iOpt/method/optim_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,8 +32,11 @@
                   type: TypeOfCalculation = TypeOfCalculation.FUNCTION
                   ) -> SearchDataItem:
         """Compute selected function by number."""
         # ???
         dataItem.functionValues[self.perm[functionIndex]] = self.problem.Calculate(dataItem.point,
                                                                                    dataItem.functionValues[
                                                                                        self.perm[functionIndex]])
+        if not(np.isfinite(dataItem.functionValues[self.perm[functionIndex]].value)):
+            raise Exception("Infinity values")
+
         return dataItem
```

### Comparing `iOpt-0.1.6/iOpt/problem.py` & `iOpt-0.2.1/iOpt/problem.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from iOpt.trial import Trial
 
 
 class Problem(ABC):
     """Базовый класс для задач оптимизации"""
 
     def __init__(self):
+        self.name: str = ''
+        self.dimension = 0
         self.numberOfFloatVariables: int = 0
-        self.numberOfDisreteVariables: int = 0
+        self.numberOfDiscreteVariables: int = 0
         self.numberOfObjectives: int = 0
         self.numberOfConstraints: int = 0
 
         self.floatVariableNames: np.ndarray(shape=(1), dtype=str) = []
         self.discreteVariableNames: np.ndarray(shape=(1), dtype=str) = []
 
         self.lowerBoundOfFloatVariables: np.ndarray(shape=(1), dtype=np.double) = []
@@ -27,7 +29,16 @@
     def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
         """
         Метод вычисления функции в заданной точке.
           Для любой новой постановки задачи, которая наследуется от :class:`Problem`, этот метод следует перегрузить.
 
         :return: Вычисленное значение функции."""
         pass
+
+   # @abstractmethod
+    def GetName(self):
+        """
+        Метод позволяет получить имя задачи
+
+        :return: self.name."""
+        return self.name
+        #pass
```

### Comparing `iOpt-0.1.6/iOpt/problems/GKLS.py` & `iOpt-0.2.1/problems/GKLS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from iOpt.problem import Problem
-from iOpt.problems.GKLS_function.gkls_function import GKLSClass, GKLSFuncionType, GKLSFunction
+from problems.GKLS_function.gkls_function import GKLSClass, GKLSFuncionType, GKLSFunction
 from iOpt.trial import Point, FunctionValue, Trial
 
 
 class GKLS(Problem):
     """
     GKLS-генератор, позволяет порождать задачи многоэкстремальной оптимизации с заранее известными свойствами: 
     количеством локальных минимумов, размерами их областей притяжения, точкой глобального минимума, 
@@ -16,16 +16,17 @@
         Конструктор класса GKLS генератора. 
 
         :param dimension: Размерность задачи, :math:`2 <= dimension <= 5`
         :param functionNumber: номер задачи в наборе, :math:`1 <= functionNumber <= 100`
         """
         super(GKLS, self).__init__()
         self.dimension = dimension
+        self.name = "GKLS"
         self.numberOfFloatVariables = dimension
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
 
         self.floatVariableNames = [str(x) for x in range(self.dimension)]
 
         self.lowerBoundOfFloatVariables = dimension * [-1]
         self.upperBoundOfFloatVariables = dimension * [1]
```

### Comparing `iOpt-0.1.6/iOpt/problems/GKLS_function/gkls_function.py` & `iOpt-0.2.1/problems/GKLS_function/gkls_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import math
-from iOpt.problems.GKLS_function.gkls_random import GKLSRandomGenerator
+from problems.GKLS_function.gkls_random import GKLSRandomGenerator
 
 
 # ***************************************************************************#
 #        GKLS-Generator of Classes of ND  (non-differentiable),              #
 #                                 D  (continuously differentiable), and      #
 #                                 D2 (twice continuously differentiable)     #
 #                     Test Functions for Global Optimization                 #
```

### Comparing `iOpt-0.1.6/iOpt/problems/GKLS_function/gkls_random.py` & `iOpt-0.2.1/problems/GKLS_function/gkls_random.py`

 * *Files identical despite different names*

### Comparing `iOpt-0.1.6/iOpt/problems/Hill/hill_generation.py` & `iOpt-0.2.1/problems/Hill/hill_generation.py`

 * *Files identical despite different names*

### Comparing `iOpt-0.1.6/iOpt/problems/Shekel/shekel_generation.py` & `iOpt-0.2.1/problems/Shekel/shekel_generation.py`

 * *Files identical despite different names*

### Comparing `iOpt-0.1.6/iOpt/problems/grishagin.py` & `iOpt-0.2.1/problems/grishagin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
-from iOpt.problems.grishagin_function.grishagin_function import GrishaginFunction
-import math
+from problems.grishagin_function.grishagin_function import GrishaginFunction
 
 
 class Grishagin(Problem):
     """
     Функция Гришагина задана формулой:
        :math:`f(y) = \{ (\sum_{i=1}^{7}\sum_{i=1}^{7} A_{ij}a_{ij}(x)+B_{ij}b_{ij}(x))^{2}+`
        :math:`+(\sum_{i=1}^{7}\sum_{i=1}^{7} C_{ij}a_{ij}(x)+D_{ij}b_{ij}(x))^{2}\}`,
@@ -21,18 +20,18 @@
     def __init__(self, function_number: int):
         """
         Конструктор класса Grishagin problem.
 
         :param functionNumber: номер задачи в наборе, :math:`1 <= functionNumber <= 100`
         """
         super(Grishagin, self).__init__()
-        self.name = Grishagin
+        self.name = "Grishagin"
         self.dimension = 2
         self.numberOfFloatVariables = self.dimension
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
         self.floatVariableNames = np.ndarray(shape=(self.dimension,), dtype=str)
         for i in range(self.dimension):
             self.floatVariableNames[i] = i
 
         self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension,), dtype=np.double)
```

### Comparing `iOpt-0.1.6/iOpt/problems/grishagin_function/grishagin_function.py` & `iOpt-0.2.1/problems/grishagin_function/grishagin_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
-from iOpt.trial import Point
-import iOpt.problems.grishagin_function.grishagin_generation as grishaginGen
+import problems.grishagin_function.grishagin_generation as grishaginGen
 import math
 
 
 class GrishaginFunction:
 
     def __init__(self, function_number: int):
         self.dimension = 2
@@ -112,15 +111,7 @@
                 jct = j
 
     def GetOptimumPoint(self) -> np.ndarray:
         y = np.ndarray(shape=(self.dimension,), dtype=np.double)
         y[0] = grishaginGen.rand_minimums[2 * (self.fn - 1)]
         y[1] = grishaginGen.rand_minimums[2 * (self.fn - 1) + 1]
         return y
-
-
-if __name__ == "__main__":
-    grish = GrishaginFunction(4)
-    point = Point([0.066182, 0.582587], [])
-    functionValue = grish.Calculate([0.066182, 0.582587])
-    print(functionValue)
-    print(grish.GetOptimumPoint())
```

### Comparing `iOpt-0.1.6/iOpt/problems/grishagin_function/grishagin_generation.py` & `iOpt-0.2.1/problems/grishagin_function/grishagin_generation.py`

 * *Files identical despite different names*

### Comparing `iOpt-0.1.6/iOpt/problems/hill.py` & `iOpt-0.2.1/problems/hill.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
-import iOpt.problems.Hill.hill_generation as hillGen
+import problems.Hill.hill_generation as hillGen
 import math
 
 
 class Hill(Problem):
     """
     Функция Хилла - это мультимодальная, непрерывная, детерминированная функция, задана формулой:
        :math:`f(x)=a_{0}+\sum_{i=1}^{m}(a_{i}sin(2i\pi x)+b_{i}cos(2i\pi x))`,
@@ -19,18 +19,18 @@
     def __init__(self, function_number: int):
         """
         Конструктор класса Hill problem.
 
         :param functionNumber: номер задачи в наборе, :math:`1 <= functionNumber <= 1000`
         """
         super(Hill, self).__init__()
-        self.name = Hill
+        self.name = "Hill"
         self.dimension = 1
         self.numberOfFloatVariables = self.dimension
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
         self.fn = function_number
 
         self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
             self.floatVariableNames[i] = i
```

### Comparing `iOpt-0.1.6/iOpt/problems/rastrigin.py` & `iOpt-0.2.1/problems/rastrigin.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     def __init__(self, dimension: int):
         """
         Конструктор класса Rastrigin problem.
 
         :param dimension: Размерность задачи.
         """
         super(Rastrigin, self).__init__()
-        self.name = Rastrigin
+        self.name = "Rastrigin"
         self.dimension = dimension
         self.numberOfFloatVariables = dimension
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
 
         self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
             self.floatVariableNames[i] = i
```

### Comparing `iOpt-0.1.6/iOpt/problems/shekel.py` & `iOpt-0.2.1/problems/shekel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
-import iOpt.problems.Shekel.shekel_generation as shekelGen
+import problems.Shekel.shekel_generation as shekelGen
 
 
 class Shekel(Problem):
     """
     Функция Шекеля - это многомерная, мультимодальная, непрерывная, детерминированная функция, задана формулой:
        :math:`f(x) = \sum_{i=1}^{m}(c_{i}+(x-a_{i})^{2})^{-1}`,
        где :math:`m` – количество максимумов функции,
@@ -21,15 +21,15 @@
 
         :param functionNumber: номер задачи в наборе, :math:`1 <= functionNumber <= 1000`
         """
         super(Shekel, self).__init__()
         self.name = Shekel
         self.dimension = 1
         self.numberOfFloatVariables = self.dimension
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
         self.fn = function_number
 
         self.floatVariableNames = np.ndarray(shape=(self.dimension,), dtype=str)
         for i in range(self.dimension):
             self.floatVariableNames[i] = i
```

### Comparing `iOpt-0.1.6/iOpt/problems/shekel4.py` & `iOpt-0.2.1/problems/shekel4.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
-import iOpt.problems.Shekel4.shekel4_generation as shekelGen
+import problems.Shekel4.shekel4_generation as shekelGen
 
 
 class Shekel4(Problem):
     """
     Функция Шекеля - это многомерная, мультимодальная, непрерывная, детерминированная функция, задана формулой:
        :math:`f(x) = \sum_{i=1}^{m}(c_{i}+\sum_{j=1}^{n}(x-a_{i})^{2})^{-1}`,
        где :math:`m` – количество максимумов функции,
@@ -21,15 +21,15 @@
 
         :param functionNumber: номер задачи в наборе, :math:`1 <= functionNumber <= 3`
         """
         super(Shekel4, self).__init__()
         self.name = Shekel4
         self.dimension = 4
         self.numberOfFloatVariables = self.dimension
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
         self.fn = function_number
 
         self.floatVariableNames = np.ndarray(shape=(self.dimension,), dtype=str)
         for i in range(self.dimension):
             self.floatVariableNames[i] = i
```

### Comparing `iOpt-0.1.6/iOpt/problems/stronginC3.py` & `iOpt-0.2.1/problems/stronginc3.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,43 +3,40 @@
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
 import math
 
 
-class StronginC3(Problem):
+class Stronginc3(Problem):
     def __init__(self):
         """
-        Конструктор класса StronginC3 problem.
+        Конструктор класса Stronginc3 problem.
         """
-        super(StronginC3, self).__init__()
-        self.name = StronginC3
+        super(Stronginc3, self).__init__()
+        self.name = "Stronginc3"
         self.dimension: int = 2
         self.numberOfFloatVariables = self.dimension
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 3
 
         self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
             self.floatVariableNames[i] = i
 
         self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables[0] = 0
-        self.lowerBoundOfFloatVariables[1] = -1
+        self.lowerBoundOfFloatVariables = [0, -1]
         self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables[0] = 4
-        self.upperBoundOfFloatVariables[1] = 3
+        self.upperBoundOfFloatVariables = [4, 3]
 
         self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
 
         pointfv = np.ndarray(shape=(self.dimension), dtype=np.double)
-        pointfv[0] = 0.941176
-        pointfv[1] = 0.941176
+        pointfv = [0.941176, 0.941176]
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
         KOfunV[0].value = -1.489444
         self.knownOptimum[0] = Trial(KOpoint, KOfunV)
 
     def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
@@ -47,28 +44,27 @@
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
         :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
         res: np.double = 0
-        x1: np.double = point.floatVariables[0]
-        x2: np.double = point.floatVariables[1]
+        x: np.double = point.floatVariables
 
         if functionValue.type == FunctionType.OBJECTIV:
-            t1: np.double = pow(0.5 * x1 - 0.5, 4.0)
-            t2: np.double = pow(x2 - 1.0, 4.0)
-            res = np.double(1.5 * x1 * x1 * math.exp(1.0 - x1 * x1 - 20.25 * (x1 - x2) * (x1 - x2)))
+            t1: np.double = pow(0.5 * x[0] - 0.5, 4.0)
+            t2: np.double = pow(x[1] - 1.0, 4.0)
+            res = np.double(1.5 * x[0] * x[0] * math.exp(1.0 - x[0] * x[0] - 20.25 * (x[0] - x[1]) * (x[0] - x[1])))
             res = np.double(res + t1 * t2 * math.exp(2.0 - t1 - t2))
             res = np.double(-res)
         elif functionValue.functionID == 0:  # constraint 1
-            res = np.double(0.01 * ((x1 - 2.2) * (x1 - 2.2) + (x2 - 1.2) * (x2 - 1.2) - 2.25))
+            res = np.double(0.01 * ((x[0] - 2.2) * (x[0] - 2.2) + (x[1] - 1.2) * (x[1] - 1.2) - 2.25))
         elif functionValue.functionID == 1:  # constraint 2
-            res = np.double(100.0 * (1.0 - ((x1 - 2.0) / 1.2) * ((x1 - 2.0) / 1.2) - (x2 / 2.0) * (x2 / 2.0)))
+            res = np.double(100.0 * (1.0 - ((x[0] - 2.0) / 1.2) * ((x[0] - 2.0) / 1.2) - (x[1] / 2.0) * (x[1] / 2.0)))
         elif functionValue.functionID == 2:  # constraint 3
-            res = np.double(10.0 * (x2 - 1.5 - 1.5 * math.sin(6.283 * (x1 - 1.75))))
+            res = np.double(10.0 * (x[1] - 1.5 - 1.5 * math.sin(6.283 * (x[0] - 1.75))))
 
         functionValue.value = res
         return functionValue
 
     def GetName(self):
         return self.name
```

### Comparing `iOpt-0.1.6/iOpt/problems/xsquared.py` & `iOpt-0.2.1/problems/xsquared.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
 
     def __init__(self, dimension: int):
         super(XSquared, self).__init__()
         self.name = XSquared
         self.dimension = dimension
         self.numberOfFloatVariables = dimension
-        self.numberOfDisreteVariables = 0
+        self.numberOfDiscreteVariables = 0
         self.numberOfObjectives = 1
         self.numberOfConstraints = 0
 
         self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
             self.floatVariableNames[i] = i
```

### Comparing `iOpt-0.1.6/iOpt/solution.py` & `iOpt-0.2.1/iOpt/solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """
     Класс описания решения задачи оптимизации
     """
     def __init__(self,
                  problem: Problem,
                  bestTrials: np.ndarray(shape=(1), dtype=Trial) = [Trial([], [])],
 
-                 numberOfGlobalTrials: int = 0,
+                 numberOfGlobalTrials: int = 1,
                  numberOfLocalTrials: int = 0,
                  solvingTime: np.double = 0.0,
                  solutionAccuracy: np.double = 0.0
                  ):
         """
         Конструктор класса
```

### Comparing `iOpt-0.1.6/iOpt/solver.py` & `iOpt-0.2.1/iOpt/output_system/listeners/animate_painters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,109 +1,78 @@
-from typing import List
-import numpy as np
-
-from iOpt.evolvent.evolvent import Evolvent
 from iOpt.method.listener import Listener
-from iOpt.method.method import Method
-from iOpt.method.optim_task import OptimizationTask
-from iOpt.method.search_data import SearchData
-from iOpt.solver_parametrs import SolverParameters
-from iOpt.problem import Problem
+from iOpt.method.search_data import SearchData, SearchDataItem
 from iOpt.solution import Solution
-from iOpt.method.process import Process
+from iOpt.method.method import Method
+
+from iOpt.output_system.painters.animate_painters import AnimatePainter, AnimatePainterND
 
+import numpy as np
 
-class Solver:
+class AnimatePainterListener(Listener):
     """
-    Класс Solver предназначен для выбора оптимальных (в заданной метрике) значений параметров
-    сложных объектов и процессов, например, методов искусственного интеллекта и
-    машинного обучения, а также – методов эвристической оптимизации.
+    Класс AnimationPaintListener - слушатель событий. Содержит методы-обработчики, выдающие в качестве
+      реакции на события динамически обновляющееся изображение процесса оптимизации.
+      Используется для одномерной оптимизации.
     """
 
-    def __init__(self,
-                 problem: Problem,
-                 parameters: SolverParameters = SolverParameters()
-                 ):
+    def __init__(self, fileName: str, pathForSaves="", isPointsAtBottom=False, toPaintObjFunc=True):
         """
-        Конструктор класса Solver
+        Конструктор класса AnimationPaintListener
 
-        :param problem: Постановка задачи оптимизации
-        :param parameters: Параметры поиска оптимальных решений
-        """
-
-        self.problem = problem
-        self.parameters = parameters
-
-        self.__listeners: List[Listener] = []
+        :param fileName: Название файла с указанием формата для сохранения изображения. Обязательный параметр.
+        :param pathForSaves: Директория для сохранения изображения. В случае, если параметр не указан, изображение
+           сохраняется в текущей рабочей директории.
+        :param isPointsAtBottom: Должны ли точки поисковой информации ставиться под графиком или нет. Если False,
+           точки ставятся на графике.
+        :param toPaintObjFunc: Должна ли отрисовываться целевая функция или нет.
+        """
+        self.fileName = fileName
+        self.pathForSaves = pathForSaves
+        self.isPointsAtBottom = isPointsAtBottom
+        self.toPaintObjFunc = toPaintObjFunc
+        self.__painter = AnimatePainter(self.isPointsAtBottom, 0, self.pathForSaves, self.fileName)
+
+    def BeforeMethodStart(self, method: Method):
+        self.__painter.SetProblem(method.task.problem)
+        if self.toPaintObjFunc:
+            self.__painter.PaintObjectiveFunc()
+
+    def OnEndIteration(self, savedNewPoints : np.ndarray(shape=(1), dtype=SearchDataItem), solution: Solution):
+        self.__painter.PaintPoints(savedNewPoints)
+
+    def OnMethodStop(self, searchData: SearchData, solution: Solution, status: bool):
+        self.__painter.PaintOptimum(solution)
+        self.__painter.SaveImage()
 
-        self.searchData = SearchData(problem)
-        self.evolvent = Evolvent(problem.lowerBoundOfFloatVariables, problem.upperBoundOfFloatVariables,
-                                 problem.numberOfFloatVariables)
-        self.task = OptimizationTask(problem)
-        self.method = Method(parameters, self.task, self.evolvent, self.searchData)
-        self.process = Process(parameters=parameters, task=self.task, evolvent=self.evolvent,
-                               searchData=self.searchData, method=self.method, listeners=self.__listeners)
-
-    def Solve(self) -> Solution:
-        """
-        Метод позволяет решить задачу оптимизации. Остановка поиска выполняется согласно критерию,
-        заданному при создании класса Solver.
-
-        :return: решение задачи оптимизации
-        """
-        return self.process.Solve()
-
-    def DoGlobalIteration(self, number: int = 1):
-        """
-        Метод позволяет выполнить несколько итераций глобального поиска
-
-        :param number: число итераций глобального поиска
-        """
-        self.process.DoGlobalIteration(number)
-
-    def DoLocalRefinement(self, number: int = 1):
-        """
-        Метод позволяет выполнить несколько итераций локального поиска
-
-        :param number: число итераций локального поиска
-        """
-        self.process.DoLocalRefinement(number)
-
-    def GetResults(self) -> Solution:
-        """
-        Метод позволяет получить текущую оценку решения задачи оптимизации
-
-        :return: решение задачи оптимизации
-        """
-        return self.process.GetResults()
-
-    def SaveProgress(self, fileName: str) -> None:
-        """
-        Сохранение процесса оптимизации в файл
-
-        :param fileName: имя файла
-        """
-        self.searchData.SaveProgress(fileName=fileName)
-
-    def LoadProgress(self, fileName: str) -> None:
-        """
-        Загрузка процесса оптимизации из файла
-
-        :param fileName: имя файла
-        """
-        self.searchData.LoadProgress(fileName=fileName)
-
-    def RefreshListener(self) -> None:
-        """
-        Метод оповещения наблюдателей о произошедшем событии
-        """
-
-        pass
-
-    def AddListener(self, listener: Listener) -> None:
-        """
-        Добавления наблюдателя за процессом оптимизации
+class AnimatePainterNDListener(Listener):
+    """
+    Класс AnimationPaintListener - слушатель событий. Содержит методы-обработчики, выдающие в качестве
+      реакции на события динамически обновляющееся изображение процесса оптимизации.
+      Используется для многомерной оптимизации.
+    """
 
-        :param listener: объект класса реализующий методы наблюдения
+    def __init__(self, fileName: str, pathForSaves="", varsIndxs=[0, 1], toPaintObjFunc=True):
         """
+        Конструктор класса AnimationNDPaintListener
 
-        self.__listeners.append(listener)
+        :param fileName: Название файла с указанием формата для сохранения изображения. Обязательный параметр.
+        :param pathForSaves: Директория для сохранения изображения. В случае, если параметр не указан, изображение
+           сохраняется в текущей рабочей директории.
+        :param varsIndxs: Пара индексов переменных оптимизационной задачи, для которых будет построен рисунок.
+        :param toPaintObjFunc: Должна ли отрисовываться целевая функция или нет.
+        """
+        self.fileName = fileName
+        self.pathForSaves = pathForSaves
+        self.toPaintObjFunc = toPaintObjFunc
+        self.__painter = AnimatePainterND(varsIndxs, self.pathForSaves, self.fileName)
+
+    def BeforeMethodStart(self, method: Method):
+        self.__painter.SetProblem(method.task.problem)
+
+    def OnEndIteration(self, savedNewPoints : np.ndarray(shape=(1), dtype=SearchDataItem), solution: Solution):
+        self.__painter.PaintPoints(savedNewPoints)
+
+    def OnMethodStop(self, searchData: SearchData, solution: Solution, status: bool):
+        self.__painter.PaintOptimum(solution)
+        if self.toPaintObjFunc:
+            self.__painter.PaintObjectiveFunc()
+        self.__painter.SaveImage()
```

### Comparing `iOpt-0.1.6/iOpt/solver_parametrs.py` & `iOpt-0.2.1/iOpt/solver_parametrs.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,17 +7,19 @@
     Класс SolverParameters позволяет определить параметры поиска оптимального решения
     """
     def __init__(self,
                  eps: np.double = 0.01,
                  r: np.double = 2.0,
                  itersLimit: int = 20000,
                  evolventDensity: int = 10,
-                 epsR: np.double = 0.001,
+                 epsR: np.double = 0.01,
                  refineSolution: bool = False,
-                 startPoint: Point = []
+                 startPoint: Point = [],
+                 numberOfParallelPoints: int = 1,
+                 timeout: int = -1
                  ):
         r"""
         Конструктор класса SolverParameters
 
         :param eps: Точность решения поставленной задачи. Меньше значения -- выше точность поиска,
              меньше вероятность преждевременной остановки.
         :param r: Параметр надежности. Более высокое значение r -- более медленная сходимость,
@@ -26,15 +28,26 @@
         :param evolventDensity: плотность построения развертки.
              По умолчанию плотность :math:`2^{-10}` на гиперкубе :math:`[0,1]^N`,
              что означает, что максимальная точность поиска составляет :math:`2^{-10}`.
         :param epsR: параметр, влияющий на скорость решения задачи с ограничениями. epsR = 0 - медленная сходимоть
              к точному решению, epsR>0 - быстрая сходимть в окрестность решения.
         :param refineSolution: если true, то решение будет уточнено с помощью локального метода.
         :param startPoint: точка начального приближения к решению.
+        :param numberOfParallelPoints: число параллельно вычисляемых испытаний.
+        :param timeout: ограничение на время вычислений в минутах.
         """
         self.eps = eps
         self.r = r
         self.itersLimit = itersLimit
+        if refineSolution:
+            self.globalMethodIterationCount = int(self.itersLimit * 0.95)
+            self.localMethodIterationCount = self.itersLimit - self.globalMethodIterationCount
+        else:
+            self.globalMethodIterationCount = self.itersLimit
+            self.localMethodIterationCount = 0
+
         self.evolventDensity = evolventDensity
         self.epsR = epsR
         self.refineSolution = refineSolution
         self.startPoint = startPoint
+        self.numberOfParallelPoints = numberOfParallelPoints
+        self.timeout = timeout
```

### Comparing `iOpt-0.1.6/iOpt/trial.py` & `iOpt-0.2.1/iOpt/trial.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,24 +6,24 @@
     OBJECTIV = 1
     CONSTRAINT = 2
 
 
 class Point:
     def __init__(self,
                  floatVariables: np.ndarray(shape=(1), dtype=np.double),
-                 discreteVariables: np.ndarray(shape=(1), dtype=str),
+                 discreteVariables: np.ndarray(shape=(1), dtype=str)=None,
                  ):
         self.floatVariables = floatVariables
         self.discreteVariables = discreteVariables
 
 
 class FunctionValue:
     def __init__(self,
                  type: FunctionType = FunctionType.OBJECTIV,
-                 functionID: str = ""
+                 functionID: int = 0
                  ):
         self.type = type
         self.functionID = functionID
         self.value: np.double = 0.0
 
 
 class Trial:
```

### Comparing `iOpt-0.1.6/iOpt.egg-info/PKG-INFO` & `iOpt-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iOpt
-Version: 0.1.6
+Version: 0.2.1
 Summary: Фреймворк для автоматического выбора значений параметров для математических моделей, ИИ и МО.
 Home-page: https://github.com/aimclub/iOpt
 Author: UNN Team
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img src="/docs/iOpt_logo.png" width="200" height="150"/>
 </p>
 
+[![SAI](https://github.com/ITMO-NSS-team/open-source-ops/blob/master/badges/SAI_badge_flat.svg)](https://sai.itmo.ru/)
+[![ITMO](https://github.com/ITMO-NSS-team/open-source-ops/blob/master/badges/ITMO_badge_flat.svg)](https://en.itmo.ru/en/)
+
 [![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-green)](LICENSE)
 [![python: 3.9](https://img.shields.io/badge/python-3.9-44cc12?style=flat-square&logo=python)](https://www.python.org/downloads/release/python-390/)
 [![python: 3.8](https://img.shields.io/badge/python-3.8-44cc12?style=flat-square&logo=python)](https://www.python.org/downloads/release/python-380/)
 [![docs: ](https://readthedocs.org/projects/ebonite/badge/?style=flat-square)](https://iopt.readthedocs.io/ru/latest/)
 [![build:](https://github.com/UNN-ITMM-Software/iOpt/actions/workflows/python-app.yml/badge.svg)](https://github.com/UNN-ITMM-Software/iOpt/actions)
 [![rus:](https://img.shields.io/badge/lang-ru-yellow.svg)](README_ru.md)
 
@@ -34,64 +37,90 @@
 - Integration with external artificial intelligence and machine learning libraries or frameworks as well as applied models.
 - Automation of the preliminary analysis of the models under study, e.g., by identifying different types of model dependencies on different groups of parameters.
 - Visualization of the process of choosing optimal parameters.
 
 
 # **Installation**
 
-## On Unix-like systems:
+
+
+## Automatic installation
+
+The simplest way to install **iOpt** is using *pip*:
 
 ```
-git clone https://github.com/UNN-ITMM-Software/iOpt
+pip install iOpt
+``` 
+
+## Manual installation
+
+### On Unix-like systems:
+
+```
+git clone https://github.com/aimclub/iOpt
 cd iOpt
 pip install virtualenv
 virtualenv ioptenv
 source ioptenv/bin/activate
 python setup.py install
 ```
 
-## On Windows:
+### On Windows:
 
 ```
-git clone https://github.com/UNN-ITMM-Software/iOpt
+git clone https://github.com/aimclub/iOpt
 cd iOpt
 pip install virtualenv
 virtualenv ioptenv
 ioptenv\Scripts\activate.bat
 python setup.py install
 ```
+## Docker
+
+Download the image:
+
+```
+docker pull aimclub/iopt:latest
+```
+
+Using the iOpt image:
+
+```
+docker run -it aimclub/iopt:latest
+```
 
 
 # **How to Use**
 
 Using the iOpt framework to minimize the Rastrigin test function.
 
 ```python
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.method.listener import StaticNDPaintListener, ConsoleFullOutputListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 from subprocess import Popen, PIPE, STDOUT
 
 if __name__ == "__main__":
     """
     Minimization of the Rastrigin test function with visualization
     """
     #Create a test task
     problem = Rastrigin(2)
     #Setup a solver options
     params = SolverParameters(r=2.5, eps=0.01, itersLimit=300, refineSolution=True)
     #Create the solver
     solver = Solver(problem, parameters=params)
     #Print results to console while solving
-    cfol = ConsoleFullOutputListener(mode='full')
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
     #3D visualization at the end of the solution
-    spl = StaticNDPaintListener("rastrigin.png", "output", varsIndxs=[0,1], mode="surface", calc="interpolation")
+    spl = StaticPainterNDListener("rastrigin.png", "output", varsIndxs=[0,1], mode="surface", calc="interpolation")
     solver.AddListener(spl)
     #Run problem solution
     sol = solver.Solve()
 ```
 
 # **Examples**
 
@@ -99,15 +128,17 @@
 
 
 ```python
 import numpy as np
 from sklearn.utils import shuffle
 from sklearn.datasets import load_breast_cancer
 
-from iOpt.method.listener import StaticNDPaintListener, AnimationNDPaintListener, ConsoleFullOutputListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
+from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
 from examples.Machine_learning.SVC._2D.Problems import SVC_2d
 
 
 def load_breast_cancer_data():
     dataset = load_breast_cancer()
@@ -122,21 +153,21 @@
     kernel_coefficient_bound = {'low': -7, 'up': -3}
 
     problem = SVC_2d.SVC_2D(x, y, regularization_value_bound, kernel_coefficient_bound)
 
     method_params = SolverParameters(r=np.double(3.0), itersLimit=100)
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimationNDPaintListener("svc2d_anim.png", "output", varsIndxs=[0, 1], toPaintObjFunc=False)
+    apl = AnimatePainterNDListener("svc2d_anim.png", "output", varsIndxs=[0, 1], toPaintObjFunc=False)
     solver.AddListener(apl)
 
-    spl = StaticNDPaintListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
+    spl = StaticPainterNDListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
     solver.AddListener(spl)
     
-    cfol = ConsoleFullOutputListener(mode='full')
+    cfol = ConsoleOutputListener(mode='full')
     solver.AddListener(cfol)
 
     solver_info = solver.Solve()
 
 ```
 
 # **Project Structure**
@@ -146,7 +177,12 @@
 - The [examples](https://github.com/UNN-ITMM-Software/iOpt/tree/main/examples) directory contains examples of using the framework for both test and applied problems.
 - Unit tests are located in the [test](https://github.com/UNN-ITMM-Software/iOpt/tree/main/test) directory.
 - Documentation source files are located in the [docs](https://github.com/UNN-ITMM-Software/iOpt/tree/main/docs) directory.
 
 # **Documentation**
 
 A detailed description of the iOpt framework API is available at [Read the Docs](https://iopt.readthedocs.io/ru/latest/).
+
+# **Supported by**
+
+The study is supported by the [Research Center Strong Artificial Intelligence in Industry](https://sai.itmo.ru/) 
+of [ITMO University](https://en.itmo.ru/) as part of the plan of the center's program: Framework of intelligent heuristic optimization methods.
```

### Comparing `iOpt-0.1.6/setup.py` & `iOpt-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 def _get_requirements(req_name: str):
     requirements = _extract_requirements(req_name)
     return requirements
 
 setup(
    name='iOpt',
-   version='0.1.6',
+   version='0.2.1',
    description='Фреймворк для автоматического выбора значений параметров для математических моделей, ИИ и МО.',
    author='UNN Team',
    author_email='',
    long_description=read_me_description,
    long_description_content_type="text/markdown",
    url="https://github.com/aimclub/iOpt",
    python_requires='>=3.8',
```

### Comparing `iOpt-0.1.6/test/test_evolvent.py` & `iOpt-0.2.1/test/test_evolvent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
 import numpy as np
-# import iOpt.evolvent
 
 from iOpt.evolvent.evolvent import Evolvent
 
 
 class TestEvolvent(unittest.TestCase):
     def setUp(self):
         self.ev1 = Evolvent([-1], [1])  # N = 1
```

### Comparing `iOpt-0.1.6/test/test_optim_task.py` & `iOpt-0.2.1/test/test_optim_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import unittest
 import numpy as np
 from iOpt.trial import FunctionValue
 from iOpt.trial import Point
-from iOpt.problems.rastrigin import Rastrigin
+from problems.rastrigin import Rastrigin
 from iOpt.method.optim_task import OptimizationTask
 from iOpt.method.search_data import SearchDataItem
 
 
 class TestOptimizationTask(unittest.TestCase):
     """setUp method is overridden from the parent class OptimizationTask"""
```

### Comparing `iOpt-0.1.6/test/test_solving_test_problems.py` & `iOpt-0.2.1/iOpt/method/process.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,212 +1,227 @@
-import unittest
-import numpy as np
-
-from iOpt.problems.GKLS import GKLS
-from iOpt.problems.rastrigin import Rastrigin
-from iOpt.problems.xsquared import XSquared
-from iOpt.problems.hill import Hill
-from iOpt.problems.shekel import Shekel
-from iOpt.problems.grishagin import Grishagin
-from iOpt.solver import Solver
+import sys
+from datetime import datetime
+from typing import List
+
+import traceback
+
+import scipy
+from scipy.optimize import Bounds
+
+from iOpt.evolvent.evolvent import Evolvent
+from iOpt.method.listener import Listener
+from iOpt.method.method import Method
+from iOpt.method.optim_task import OptimizationTask
+from iOpt.method.search_data import SearchData, SearchDataItem
+from iOpt.solution import Solution
 from iOpt.solver_parametrs import SolverParameters
+from iOpt.trial import FunctionValue, FunctionType
+from iOpt.trial import Point
 
 
-class TestRastrigin(unittest.TestCase):
-    """setUp method is overridden from the parent class Rastrigin"""
-
-    def setUp(self):
-        self.epsVal = 0.01
-
-    def test_Rastrigin_Solve(self):
-        self.r = 3.5
-        self.problem = Rastrigin(1)
-        params = SolverParameters(r=self.r, eps=self.epsVal)
-        self.solver = Solver(self.problem, parameters=params)
-        numberOfGlobalTrials = 44
-
-        sol = self.solver.Solve()
-
-        res = True
-        for j in range(self.problem.dimension):
-            fabsx = np.abs(self.problem.knownOptimum[0].point.floatVariables[j] -
-                           sol.bestTrials[0].point.floatVariables[j])
-            fm = self.epsVal * (self.problem.upperBoundOfFloatVariables[j] -
-                                self.problem.lowerBoundOfFloatVariables[j])
-            if (fabsx > fm):
-                res = res and False
-
-        self.assertEqual(res, True)
-        self.assertEqual(sol.numberOfGlobalTrials, numberOfGlobalTrials)
-
-    def test_XSquared_Solve(self):
-        self.r = 3.5
-        self.problem = XSquared(1)
-        params = SolverParameters(r=self.r, eps=self.epsVal)
-        self.solver = Solver(self.problem, parameters=params)
-        numberOfGlobalTrials = 36
-
-        sol = self.solver.Solve()
-
-        res = True
-        for j in range(self.problem.dimension):
-            fabsx = np.abs(
-                self.problem.knownOptimum[0].point.floatVariables[j] - sol.bestTrials[0].point.floatVariables[j])
-            fm = self.epsVal * (
-                    self.problem.upperBoundOfFloatVariables[j] - self.problem.lowerBoundOfFloatVariables[j])
-            if (fabsx > fm):
-                res = res and False
-
-        self.assertEqual(res, True)
-        self.assertEqual(sol.numberOfGlobalTrials, numberOfGlobalTrials)
-
-    def test_Hill_Solve(self):
-        self.r = 3.5
-        self.problem = Hill(1)
-        params = SolverParameters(r=self.r, eps=self.epsVal)
-        self.solver = Solver(self.problem, parameters=params)
-        numberOfGlobalTrials = 52
-
-        sol = self.solver.Solve()
-
-        res = True
-        for j in range(self.problem.dimension):
-            fabsx = np.abs(
-                self.problem.knownOptimum[0].point.floatVariables[j] - sol.bestTrials[0].point.floatVariables[j])
-            fm = self.epsVal * (
-                    self.problem.upperBoundOfFloatVariables[j] - self.problem.lowerBoundOfFloatVariables[j])
-            if (fabsx > fm):
-                res = res and False
-
-        self.assertEqual(res, True)
-        self.assertEqual(sol.numberOfGlobalTrials, numberOfGlobalTrials)
-
-    def test_Shekel_Solve(self):
-        self.r = 3
-        self.problem = Shekel(1)
-        params = SolverParameters(r=self.r, eps=self.epsVal)
-        self.solver = Solver(self.problem, parameters=params)
-        numberOfGlobalTrials = 34
-
-        sol = self.solver.Solve()
-
-        res = True
-        for j in range(self.problem.dimension):
-            fabsx = np.abs(
-                self.problem.knownOptimum[0].point.floatVariables[j] - sol.bestTrials[0].point.floatVariables[j])
-            fm = self.epsVal * (
-                    self.problem.upperBoundOfFloatVariables[j] - self.problem.lowerBoundOfFloatVariables[j])
-            if (fabsx > fm):
-                res = res and False
-
-        self.assertEqual(res, True)
-        self.assertEqual(sol.numberOfGlobalTrials, numberOfGlobalTrials)
-
-    def test_Grishagin_Solve(self):
-        self.r = 3
-        self.problem = Grishagin(1)
-        params = SolverParameters(r=self.r, eps=self.epsVal)
-        self.solver = Solver(self.problem, parameters=params)
-        numberOfGlobalTrials = 543
-
-        sol = self.solver.Solve()
-
-        res = True
-        for j in range(self.problem.dimension):
-            fabsx = np.abs(
-                self.problem.knownOptimum[0].point.floatVariables[j] - sol.bestTrials[0].point.floatVariables[j])
-            fm = self.epsVal * (
-                    self.problem.upperBoundOfFloatVariables[j] - self.problem.lowerBoundOfFloatVariables[j])
-            if (fabsx > fm):
-                res = res and False
-
-        self.assertEqual(res, True)
-        self.assertEqual(sol.numberOfGlobalTrials, numberOfGlobalTrials)
-
-    def test_GKLS_2D_Solve(self):
-        # создание объекта задачи, двухмерная задача с номером 1
-        self.problem = GKLS(2, 1)
-        # Формируем параметры решателя, параметр надежности метода r=3.5, точность поиска eps=0.01
-        params = SolverParameters(r=3.5, eps=0.01)
-        # Создаем решатель
-        self.solver = Solver(self.problem, parameters=params)
-        # Необходимое число итераций алгоритма, для указанной задачи с заданными параметрами
-        numberOfGlobalTrials = 308
-
-        # Решение задачи
-        sol = self.solver.Solve()
-
-        # Проверяем что найденный АГП минимумом соответствуйте априори известному, для этой задачи, с точностью eps
-        res = True
-        for j in range(self.problem.dimension):
-            fabsx = np.abs(
-                self.problem.knownOptimum[0].point.floatVariables[j] - sol.bestTrials[0].point.floatVariables[j])
-            fm = self.epsVal * (
-                    self.problem.upperBoundOfFloatVariables[j] - self.problem.lowerBoundOfFloatVariables[j])
-            if (fabsx > fm):
-                res = res and False
-        # Проверяем что решение задачи действительно сошлось к глобальному минимуму
-        self.assertEqual(res, True)
-        # Проверяем что на решение потребовалось правильное число итераций АГП
-        self.assertEqual(sol.numberOfGlobalTrials, numberOfGlobalTrials)
-
-    def test_Solve_100_GKLS_2D_problem(self):
-        # Необходимое число итераций алгоритма, для каждой из 100 задач, с заданными параметрами решателя
-        numberOfGlobalTrials = [883, 1441, 1061, 723, 732, 687, 684, 775, 754, 1053, 1165, 1361, 465, 760, 701, 887,
-                                1070, 1673, 1576, 744, 392, 878, 1176, 525, 1175, 856, 898, 649, 885, 771, 972, 1042,
-                                1042, 619, 796, 544, 647, 1071, 591, 833, 605, 458, 527, 1003, 473, 988, 1277, 649, 531,
-                                730, 1108, 828, 648, 221, 1502, 849, 632, 641, 609, 749, 922, 693, 991, 894, 716, 575,
-                                952, 1287, 231, 1052, 625, 516, 732, 757, 617, 1455, 490, 1118, 786, 1273, 533, 683,
-                                278, 1456, 1091, 1171, 974, 777, 1227, 700, 767, 728, 962, 1198, 445, 809, 946, 288,
-                                927, 903]
-
-        for i in range(100):
-            # создание объекта задачи, двухмерная задача с номером i+1
-            self.problem = GKLS(2, i + 1)
-            # Формируем параметры решателя, параметр надежности метода r=5.1, точность поиска eps=0.01
-            params = SolverParameters(r=5.1, eps=0.01)
-            # Создаем решатель
-            self.solver = Solver(self.problem, parameters=params)
-
-            # Решение задачи
-            sol = self.solver.Solve()
-
-            # Проверяем что найденный АГП минимумом соответствуйте априори известному, для этой задачи, с точностью eps
-
-            res = True
-            for j in range(self.problem.dimension):
-                fabsx = np.abs(
-                    self.problem.knownOptimum[0].point.floatVariables[j] - sol.bestTrials[0].point.floatVariables[j])
-                fm = self.epsVal * (
-                        self.problem.upperBoundOfFloatVariables[j] - self.problem.lowerBoundOfFloatVariables[j])
-                if (fabsx > fm):
-                    res = res and False
-            # Проверяем что решение задачи действительно сошлось к глобальному минимуму
-            self.assertEqual(res, True)
-            # Проверяем что на решение потребовалось правильное число итераций АГП
-            self.assertEqual(sol.numberOfGlobalTrials, numberOfGlobalTrials[i])
-
-    def test_GKLS_4D_Solve(self):
-        self.r = 3.5
-        self.problem = GKLS(4, 3)
-        params = SolverParameters(r=self.r, eps=self.epsVal, refineSolution=False, itersLimit=5000)
-        self.solver = Solver(self.problem, parameters=params)
-        numberOfGlobalTrials = 2830
-
-        sol = self.solver.Solve()
-
-        res = True
-        for j in range(self.problem.dimension):
-            fabsx = np.abs(
-                self.problem.knownOptimum[0].point.floatVariables[j] - sol.bestTrials[0].point.floatVariables[j])
-            fm = self.epsVal * (
-                    self.problem.upperBoundOfFloatVariables[j] - self.problem.lowerBoundOfFloatVariables[j])
-            if fabsx > fm:
-                res = res and False
-
-        self.assertEqual(res, True)
-        self.assertEqual(sol.numberOfGlobalTrials, numberOfGlobalTrials)
-
-
-"""Executing the tests in the above test case class"""
-if __name__ == "__main__":
-    unittest.main()
+class Process:
+    """
+    Класс Process скрывает внутреннюю имплементацию класса Solver.
+    """
+
+    def __init__(self,
+                 parameters: SolverParameters,
+                 task: OptimizationTask,
+                 evolvent: Evolvent,
+                 searchData: SearchData,
+                 method: Method,
+                 listeners: List[Listener]
+                 ):
+        """
+        Конструктор класса Process
+
+        :param parameters: Параметры решения задачи оптимизации.
+        :param task: Обёртка решаемой задачи.
+        :param evolvent: Развертка Пеано-Гильберта, отображающая отрезок [0,1] на многомерную область D.
+        :param searchData: Структура данных для хранения накопленной поисковой информации.
+        :param method: Метод оптимизации, проводящий поисковые испытания по заданным правилам.
+        :param listeners: Список "наблюдателей" (используется для вывода текущей информации).
+        """
+        self.parameters = parameters
+        self.task = task
+        self.evolvent = evolvent
+        self.searchData = searchData
+        self.method = method
+        self._listeners = listeners
+        self._first_iteration = True
+
+    def Solve(self) -> Solution:
+        """
+        Метод позволяет решить задачу оптимизации. Остановка поиска выполняется согласно критерию,
+        заданному при создании класса Solver.
+
+        :return: Текущая оценка решения задачи оптимизации
+        """
+
+        startTime = datetime.now()
+
+        try:
+            while not self.method.CheckStopCondition():
+                self.DoGlobalIteration()
+
+        except Exception:
+            print('Exception was thrown')
+            print(traceback.format_exc())
+
+        if self.parameters.refineSolution:
+            self.DoLocalRefinement(self.parameters.localMethodIterationCount)
+
+        result = self.GetResults()
+        result.solvingTime = (datetime.now() - startTime).total_seconds()
+
+        for listener in self._listeners:
+            status = self.method.CheckStopCondition()
+            listener.OnMethodStop(self.searchData, self.GetResults(), status)
+
+        return result
+
+    def DoGlobalIteration(self, number: int = 1):
+        """
+        Метод позволяет выполнить несколько итераций глобального поиска
+
+        :param number: Количество итераций глобального поиска
+        """
+        number_ = number
+        doneTrials = []
+        if self._first_iteration is True:
+            for listener in self._listeners:
+                listener.BeforeMethodStart(self.method)
+            doneTrials = self.method.FirstIteration()
+            self._first_iteration = False
+            number = number - 1
+
+        for _ in range(number):
+            newpoint, oldpoint = self.method.CalculateIterationPoint()
+            self.method.CalculateFunctionals(newpoint)
+            self.method.UpdateOptimum(newpoint)
+            self.method.RenewSearchData(newpoint, oldpoint)
+            self.method.FinalizeIteration()
+            doneTrials = self.searchData.GetLastItems(self.parameters.numberOfParallelPoints * number_)
+
+        for listener in self._listeners:
+            listener.OnEndIteration(doneTrials, self.GetResults())
+
+    def problemCalculate(self, y):
+        result = self.GetResults()
+        point = Point(y, result.bestTrials[0].point.discreteVariables)
+        functionValue = FunctionValue(FunctionType.OBJECTIV)
+
+        for i in range(self.task.problem.dimension):
+            if (y[i] < self.task.problem.lowerBoundOfFloatVariables[i]) \
+                    or (y[i] > self.task.problem.upperBoundOfFloatVariables[i]):
+                functionValue.value = sys.float_info.max
+                return functionValue.value
+
+        try:
+            for i in range(self.task.problem.numberOfConstraints):
+                functionConstraintValue = FunctionValue(FunctionType.CONSTRAINT, i)
+                functionConstraintValue = self.task.problem.Calculate(point, functionConstraintValue)
+                if functionConstraintValue.value > 0:
+                    functionValue.value = sys.float_info.max
+                    return functionValue.value
+
+            functionValue = self.task.problem.Calculate(point, functionValue)
+        except Exception:
+            functionValue.value = sys.float_info.max
+
+        return functionValue.value
+
+    def DoLocalRefinement(self, number: int = 1):
+        """
+        Метод позволяет выполнить несколько итераций локального поиска
+
+        :param number: Количество итераций локального поиска
+        """
+        try:
+            localMethodIterationCount = number
+            if number == -1:
+                localMethodIterationCount = self.parameters.localMethodIterationCount
+
+            result = self.GetResults()
+            startPoint = result.bestTrials[0].point.floatVariables
+
+            nelder_mead = scipy.optimize.minimize(self.problemCalculate, x0=startPoint, method='Nelder-Mead',
+                                                  options={'maxiter': localMethodIterationCount})
+
+            if localMethodIterationCount > 0:
+                result.bestTrials[0].point.floatVariables = nelder_mead.x
+
+                point: SearchDataItem = SearchDataItem(result.bestTrials[0].point,
+                                                       self.evolvent.GetInverseImage(
+                                                           result.bestTrials[0].point.floatVariables),
+                                                       functionValues=[FunctionValue()] *
+                                                                      (self.task.problem.numberOfConstraints +
+                                                                       self.task.problem.numberOfObjectives)
+                                                       )
+
+                number_of_constraints = self.task.problem.numberOfConstraints
+                for i in range(number_of_constraints):
+                    point.functionValues[i] = FunctionValue(FunctionType.CONSTRAINT, i)
+                    point.functionValues[i] = self.task.problem.Calculate(point.point, point.functionValues[i])
+                    point.SetZ(point.functionValues[i].value)
+                    point.SetIndex(i)
+                    if point.GetZ() > 0:
+                        break
+                point.functionValues[number_of_constraints] = FunctionValue(FunctionType.OBJECTIV,
+                                                                            number_of_constraints)
+                point.functionValues[number_of_constraints] = \
+                    self.task.problem.Calculate(point.point, point.functionValues[number_of_constraints])
+                point.SetZ(point.functionValues[number_of_constraints].value)
+                point.SetIndex(number_of_constraints)
+
+                result.bestTrials[0].functionValues = point.functionValues
+
+            result.numberOfLocalTrials = nelder_mead.nfev
+        except Exception:
+            print("Local Refinement is not possible")
+
+    def GetResults(self) -> Solution:
+        """
+        Метод возвращает лучшее найденное решение задачи оптимизации
+
+        :return: Решение задачи оптимизации
+        """
+        # ДА, ЭТО КОСТЫЛЬ. т.к. solution хранит trial
+        # self.searchData.solution.bestTrials[0] = self.method.GetOptimumEstimation()
+        return self.searchData.solution
+
+    def SaveProgress(self, fileName: str) -> None:
+        """
+        Сохранение процесса оптимизации из файла
+
+        :param fileName: имя файла
+        """
+        self.searchData.SaveProgress(fileName=fileName)
+
+    def LoadProgress(self, fileName: str) -> None:
+        """
+        Загрузка процесса оптимизации из файла
+
+        :param fileName: имя файла
+        """
+        self.searchData.LoadProgress(fileName=fileName)
+        self.method.iterationsCount = self.searchData.GetCount() - 2
+
+        for ditem in self.searchData:
+            if ditem.GetIndex() >= 0:
+                self.method.UpdateOptimum(ditem)
+
+        self.method.RecalcM()
+        self.method.RecalcAllCharacteristics()
+        self._first_iteration = False
+
+        for listener in self._listeners:
+            listener.BeforeMethodStart(self.method)
+
+    '''
+    def RefreshListener(self):
+        pass
+
+    def AddListener(self, listener: Listener):
+        #self.__listeners.append(listener)
+        pass
+    '''
```

