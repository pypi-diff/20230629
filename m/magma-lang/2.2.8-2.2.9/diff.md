# Comparing `tmp/magma-lang-2.2.8.tar.gz` & `tmp/magma-lang-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magma-lang-2.2.8.tar", last modified: Fri Mar  4 14:41:26 2022, max compression
+gzip compressed data, was "magma-lang-2.2.9.tar", last modified: Mon Mar  7 19:34:19 2022, max compression
```

## Comparing `magma-lang-2.2.8.tar` & `magma-lang-2.2.9.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.872034 magma-lang-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-03-04 14:33:48.000000 magma-lang-2.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10623 2022-03-04 14:41:26.872034 magma-lang-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8418 2022-03-04 14:33:48.000000 magma-lang-2.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.852034 magma-lang-2.2.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2538 2022-03-04 14:33:48.000000 magma-lang-2.2.8/bin/magma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.860034 magma-lang-2.2.8/magma/
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36535 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/array.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/ast_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.860034 magma-lang-2.2.8/magma/backend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4294 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/blif.py
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/check_wiring_context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.860034 magma-lang-2.2.8/magma/backend/coreir/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/coreir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/coreir/coreir_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     8037 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/coreir/coreir_compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/coreir/coreir_runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)    22238 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/coreir/coreir_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6266 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/coreir/coreir_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/coreir/insert_coreir_wires.py
--rw-r--r--   0 runner    (1001) docker     (121)     4015 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/coreir/insert_wrap_casts.py
--rw-r--r--   0 runner    (1001) docker     (121)     5133 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/dot.py
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/firrtl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.864034 magma-lang-2.2.8/magma/backend/mlir/
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/build_magma_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/builtin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/comb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/compile_to_mlir.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/graph_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)    28234 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/hardware_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     5726 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/hw.py
--rw-r--r--   0 runner    (1001) docker     (121)     3726 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/magma_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/magma_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     5670 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/mlir.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/mlir_compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/mlir_printer_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/mlir_to_verilog.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/mlir_to_verilog_main.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/printer_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/scoped_name_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/sv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/mlir/translation_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     9056 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/backend/verilog.py
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/bfloat.py
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/bind.py
--rw-r--r--   0 runner    (1001) docker     (121)     4064 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/bit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/bit_primitives.py
--rw-r--r--   0 runner    (1001) docker     (121)    26367 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/bits.py
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/bitutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11289 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/braid.py
--rw-r--r--   0 runner    (1001) docker     (121)    32492 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/circuit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/circuit_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3281 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/clock.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/clock_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     5240 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     3047 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/compile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/compile_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     8363 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/compile_guard.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    11644 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     3454 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/definition_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     7391 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/digital.py
--rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/display.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/family.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.864034 magma-lang-2.2.8/magma/frontend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/frontend/coreir.py
--rw-r--r--   0 runner    (1001) docker     (121)     5432 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/frontend/coreir_.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/frontend/dummy_verilog_importer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/frontend/pyverilog_importer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5218 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/frontend/verilog.py
--rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/frontend/verilog_importer.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/frontend/verilog_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4212 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/if_def.py
--rw-r--r--   0 runner    (1001) docker     (121)    10060 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/inline_verilog.py
--rw-r--r--   0 runner    (1001) docker     (121)    17236 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/ir.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/is_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/is_primitive.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/language_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/linking.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     4827 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/math.py
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/operator_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.868034 magma-lang-2.2.8/magma/passes/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7146 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/passes/clock.py
--rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/passes/debug_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1797 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/passes/drive_undriven.py
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/passes/find_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/passes/ir.py
--rw-r--r--   0 runner    (1001) docker     (121)     4039 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/passes/passes.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/passes/terminate_unused.py
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/passes/tsort.py
--rw-r--r--   0 runner    (1001) docker     (121)     5399 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/placer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.868034 magma-lang-2.2.8/magma/primitives/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/primitives/lut.py
--rw-r--r--   0 runner    (1001) docker     (121)     6933 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/primitives/memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     7197 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/primitives/mux.py
--rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/primitives/register.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/primitives/set_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     2345 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/primitives/slice.py
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/primitives/wire.py
--rw-r--r--   0 runner    (1001) docker     (121)     3320 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/protocol_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     5840 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/ref.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/scope.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/set_name.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.868034 magma-lang-2.2.8/magma/simulator/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11159 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/simulator/coreir_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)    21013 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/simulator/mdb.py
--rw-r--r--   0 runner    (1001) docker     (121)    13858 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/simulator/python_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/simulator/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.868034 magma-lang-2.2.8/magma/smart/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/smart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17619 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/smart/smart_bits.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.868034 magma-lang-2.2.8/magma/ssa/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/ssa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6757 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/ssa/ssa.py
--rw-r--r--   0 runner    (1001) docker     (121)    14021 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/symbol_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    16286 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/symbol_table_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.868034 magma-lang-2.2.8/magma/syntax/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10787 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/combinational.py
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/combinational2.py
--rw-r--r--   0 runner    (1001) docker     (121)    10970 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/coroutine.py
--rw-r--r--   0 runner    (1001) docker     (121)     4690 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/inline_combinational.py
--rw-r--r--   0 runner    (1001) docker     (121)    15172 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/sequential2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.872034 magma-lang-2.2.8/magma/syntax/transforms/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/transforms/inline_yield_from.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/transforms/replace_symbols.py
--rw-r--r--   0 runner    (1001) docker     (121)     2597 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    14406 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/verilog.py
--rw-r--r--   0 runner    (1001) docker     (121)    14548 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/syntax/verilog_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5229 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/t.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.872034 magma-lang-2.2.8/magma/testing/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9924 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    18653 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/tuple.py
--rw-r--r--   0 runner    (1001) docker     (121)     4004 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.872034 magma-lang-2.2.8/magma/types/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/types/bit_pattern.py
--rw-r--r--   0 runner    (1001) docker     (121)    11623 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/types/ready_valid.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/types/valid.py
--rw-r--r--   0 runner    (1001) docker     (121)     3635 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/uniquification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/value_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/verilog_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/view.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/waveform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/wire.py
--rw-r--r--   0 runner    (1001) docker     (121)     4680 2022-03-04 14:33:48.000000 magma-lang-2.2.8/magma/wire_container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 14:41:26.872034 magma-lang-2.2.8/magma_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10623 2022-03-04 14:41:26.000000 magma-lang-2.2.8/magma_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3947 2022-03-04 14:41:26.000000 magma-lang-2.2.8/magma_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-04 14:41:26.000000 magma-lang-2.2.8/magma_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-03-04 14:41:26.000000 magma-lang-2.2.8/magma_lang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-04 14:41:26.000000 magma-lang-2.2.8/magma_lang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-03-04 14:41:26.872034 magma-lang-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-03-04 14:33:48.000000 magma-lang-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.116249 magma-lang-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-03-07 19:26:09.000000 magma-lang-2.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10623 2022-03-07 19:34:19.116249 magma-lang-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8418 2022-03-07 19:26:09.000000 magma-lang-2.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.076248 magma-lang-2.2.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2538 2022-03-07 19:26:09.000000 magma-lang-2.2.9/bin/magma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.092248 magma-lang-2.2.9/magma/
+-rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36614 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/ast_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.092248 magma-lang-2.2.9/magma/backend/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4294 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/blif.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/check_wiring_context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.096248 magma-lang-2.2.9/magma/backend/coreir/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/coreir_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8037 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/coreir_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/coreir_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22238 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/coreir_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6266 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/coreir_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/insert_coreir_wires.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4015 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/insert_wrap_casts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5133 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/dot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/firrtl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.100248 magma-lang-2.2.9/magma/backend/mlir/
+-rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/build_magma_graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)      850 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/comb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/compile_to_mlir.py
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/graph_lib.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28234 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/hardware_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5726 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/hw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3726 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/magma_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/magma_ops.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5670 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/mlir.py
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/mlir_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/mlir_printer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/mlir_to_verilog.py
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/mlir_to_verilog_main.py
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/printer_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/scoped_name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/sv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3026 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/translation_unit.py
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9056 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/verilog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bfloat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bind.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4064 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bit_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26367 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bits.py
+-rw-r--r--   0 runner    (1001) docker     (121)      882 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bitutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11289 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/braid.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32492 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/circuit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3281 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/clock.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/clock_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5240 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3047 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/compile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/compile_exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8363 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/compile_guard.py
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11644 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/debug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3454 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/definition_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7391 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/digital.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/family.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.104248 magma-lang-2.2.9/magma/frontend/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/coreir.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5432 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/coreir_.py
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/dummy_verilog_importer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/pyverilog_importer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5218 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/verilog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/verilog_importer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/verilog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4212 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/if_def.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10060 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/inline_verilog.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17236 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/ir.py
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/is_definition.py
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/is_primitive.py
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/language_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/linking.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4827 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/math.py
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/operator_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.104248 magma-lang-2.2.9/magma/passes/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7146 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/clock.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/debug_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1797 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/drive_undriven.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/find_errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/ir.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4039 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/passes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/terminate_unused.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/tsort.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5399 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/placer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.108249 magma-lang-2.2.9/magma/primitives/
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/lut.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6933 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7197 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/mux.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/register.py
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/set_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2345 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/slice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/wire.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3320 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/protocol_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5840 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/ref.py
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/scope.py
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/set_name.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.108249 magma-lang-2.2.9/magma/simulator/
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11159 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/simulator/coreir_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21013 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/simulator/mdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13858 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/simulator/python_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/simulator/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.108249 magma-lang-2.2.9/magma/smart/
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/smart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17619 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/smart/smart_bits.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.108249 magma-lang-2.2.9/magma/ssa/
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/ssa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6757 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/ssa/ssa.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14021 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/symbol_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16286 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/symbol_table_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.112249 magma-lang-2.2.9/magma/syntax/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10787 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/combinational.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/combinational2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10970 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4690 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/inline_combinational.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15172 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/sequential2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.112249 magma-lang-2.2.9/magma/syntax/transforms/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/transforms/inline_yield_from.py
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/transforms/replace_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2597 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14406 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/verilog.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14548 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/verilog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5229 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/t.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.112249 magma-lang-2.2.9/magma/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9924 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18653 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/tuple.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4004 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.116249 magma-lang-2.2.9/magma/types/
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/types/bit_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11623 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/types/ready_valid.py
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/types/valid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3635 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/uniquification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/value_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/verilog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/view.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/wire.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4680 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/wire_container.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.116249 magma-lang-2.2.9/magma_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10623 2022-03-07 19:34:18.000000 magma-lang-2.2.9/magma_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3947 2022-03-07 19:34:18.000000 magma-lang-2.2.9/magma_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-07 19:34:18.000000 magma-lang-2.2.9/magma_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-03-07 19:34:18.000000 magma-lang-2.2.9/magma_lang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-07 19:34:18.000000 magma-lang-2.2.9/magma_lang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-03-07 19:34:19.116249 magma-lang-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-03-07 19:26:09.000000 magma-lang-2.2.9/setup.py
```

### Comparing `magma-lang-2.2.8/LICENSE.txt` & `magma-lang-2.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/PKG-INFO` & `magma-lang-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magma-lang
-Version: 2.2.8
+Version: 2.2.9
 Summary: An embedded DSL for constructing hardware circuits
 Home-page: https://github.com/phanrahan/magma
 Maintainer: Lenny Truong
 Maintainer-email: lenny@cs.stanford.edu
 License: MIT
 Description: # Magma
         [![Documentation Status](https://readthedocs.org/projects/magma/badge/?version=latest)](https://magma.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `magma-lang-2.2.8/README.md` & `magma-lang-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/bin/magma` & `magma-lang-2.2.9/bin/magma`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/__init__.py` & `magma-lang-2.2.9/magma/__init__.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/array.py` & `magma-lang-2.2.9/magma/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import weakref
 from functools import reduce, lru_cache
+import operator
 from abc import ABCMeta
 from hwtypes import BitVector
 from .common import deprecated
 from .ref import AnonRef, ArrayRef
 from .t import Type, Kind, Direction, In, Out
 from .compatibility import IntegerTypes
 from .digital import Digital
@@ -402,15 +403,16 @@
     def is_clock(cls):
         return False
 
     @output_only("Cannot use == on an input")
     def __eq__(self, rhs):
         if not isinstance(rhs, ArrayType):
             return False
-        return self.ts == rhs.ts
+        return reduce(operator.and_,
+                      (x == y for x, y in zip(self, rhs)))
 
     @output_only("Cannot use != on an input")
     def __ne__(self, rhs):
         return ~(self == rhs)
 
     __hash__ = Type.__hash__
```

### Comparing `magma-lang-2.2.8/magma/ast_utils.py` & `magma-lang-2.2.9/magma/ast_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/blif.py` & `magma-lang-2.2.9/magma/backend/blif.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/check_wiring_context.py` & `magma-lang-2.2.9/magma/backend/check_wiring_context.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/coreir/coreir_backend.py` & `magma-lang-2.2.9/magma/backend/coreir/coreir_backend.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/coreir/coreir_compiler.py` & `magma-lang-2.2.9/magma/backend/coreir/coreir_compiler.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/coreir/coreir_runtime.py` & `magma-lang-2.2.9/magma/backend/coreir/coreir_runtime.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/coreir/coreir_transformer.py` & `magma-lang-2.2.9/magma/backend/coreir/coreir_transformer.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/coreir/coreir_utils.py` & `magma-lang-2.2.9/magma/backend/coreir/coreir_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/coreir/insert_coreir_wires.py` & `magma-lang-2.2.9/magma/backend/coreir/insert_coreir_wires.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/coreir/insert_wrap_casts.py` & `magma-lang-2.2.9/magma/backend/coreir/insert_wrap_casts.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/dot.py` & `magma-lang-2.2.9/magma/backend/dot.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/firrtl.py` & `magma-lang-2.2.9/magma/backend/firrtl.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/build_magma_graph.py` & `magma-lang-2.2.9/magma/backend/mlir/build_magma_graph.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/builtin.py` & `magma-lang-2.2.9/magma/backend/mlir/builtin.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/comb.py` & `magma-lang-2.2.9/magma/backend/mlir/comb.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/common.py` & `magma-lang-2.2.9/magma/backend/mlir/common.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/compile_to_mlir.py` & `magma-lang-2.2.9/magma/backend/mlir/compile_to_mlir.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/hardware_module.py` & `magma-lang-2.2.9/magma/backend/mlir/hardware_module.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/hw.py` & `magma-lang-2.2.9/magma/backend/mlir/hw.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/magma_common.py` & `magma-lang-2.2.9/magma/backend/mlir/magma_common.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/magma_ops.py` & `magma-lang-2.2.9/magma/backend/mlir/magma_ops.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/mlir.py` & `magma-lang-2.2.9/magma/backend/mlir/mlir.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/mlir_compiler.py` & `magma-lang-2.2.9/magma/backend/mlir/mlir_compiler.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/mlir_printer_utils.py` & `magma-lang-2.2.9/magma/backend/mlir/mlir_printer_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/mlir_to_verilog.py` & `magma-lang-2.2.9/magma/backend/mlir/mlir_to_verilog.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/printer_base.py` & `magma-lang-2.2.9/magma/backend/mlir/printer_base.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/scoped_name_generator.py` & `magma-lang-2.2.9/magma/backend/mlir/scoped_name_generator.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/sv.py` & `magma-lang-2.2.9/magma/backend/mlir/sv.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/mlir/translation_unit.py` & `magma-lang-2.2.9/magma/backend/mlir/translation_unit.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/backend/verilog.py` & `magma-lang-2.2.9/magma/backend/verilog.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/bfloat.py` & `magma-lang-2.2.9/magma/bfloat.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/bind.py` & `magma-lang-2.2.9/magma/bind.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/bit.py` & `magma-lang-2.2.9/magma/bit.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/bit_primitives.py` & `magma-lang-2.2.9/magma/bit_primitives.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/bits.py` & `magma-lang-2.2.9/magma/bits.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/bitutils.py` & `magma-lang-2.2.9/magma/bitutils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/braid.py` & `magma-lang-2.2.9/magma/braid.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/circuit.py` & `magma-lang-2.2.9/magma/circuit.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/circuit_utils.py` & `magma-lang-2.2.9/magma/circuit_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/clock.py` & `magma-lang-2.2.9/magma/clock.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/clock_io.py` & `magma-lang-2.2.9/magma/clock_io.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/common.py` & `magma-lang-2.2.9/magma/common.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/compile.py` & `magma-lang-2.2.9/magma/compile.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/compile_exception.py` & `magma-lang-2.2.9/magma/compile_exception.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/compile_guard.py` & `magma-lang-2.2.9/magma/compile_guard.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/compiler.py` & `magma-lang-2.2.9/magma/compiler.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/config.py` & `magma-lang-2.2.9/magma/config.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/conversions.py` & `magma-lang-2.2.9/magma/conversions.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/debug.py` & `magma-lang-2.2.9/magma/debug.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/definition_context.py` & `magma-lang-2.2.9/magma/definition_context.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/digital.py` & `magma-lang-2.2.9/magma/digital.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/display.py` & `magma-lang-2.2.9/magma/display.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/enum.py` & `magma-lang-2.2.9/magma/enum.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/frontend/coreir.py` & `magma-lang-2.2.9/magma/frontend/coreir.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/frontend/coreir_.py` & `magma-lang-2.2.9/magma/frontend/coreir_.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/frontend/pyverilog_importer.py` & `magma-lang-2.2.9/magma/frontend/pyverilog_importer.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/frontend/verilog.py` & `magma-lang-2.2.9/magma/frontend/verilog.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/frontend/verilog_importer.py` & `magma-lang-2.2.9/magma/frontend/verilog_importer.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/frontend/verilog_utils.py` & `magma-lang-2.2.9/magma/frontend/verilog_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/generator.py` & `magma-lang-2.2.9/magma/generator.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/inline_verilog.py` & `magma-lang-2.2.9/magma/inline_verilog.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/interface.py` & `magma-lang-2.2.9/magma/interface.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/ir.py` & `magma-lang-2.2.9/magma/ir.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/linking.py` & `magma-lang-2.2.9/magma/linking.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/log.py` & `magma-lang-2.2.9/magma/log.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/logging.py` & `magma-lang-2.2.9/magma/logging.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/passes/clock.py` & `magma-lang-2.2.9/magma/passes/clock.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/passes/debug_name.py` & `magma-lang-2.2.9/magma/passes/debug_name.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/passes/drive_undriven.py` & `magma-lang-2.2.9/magma/passes/drive_undriven.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/passes/find_errors.py` & `magma-lang-2.2.9/magma/passes/find_errors.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/passes/passes.py` & `magma-lang-2.2.9/magma/passes/passes.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/passes/terminate_unused.py` & `magma-lang-2.2.9/magma/passes/terminate_unused.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/passes/tsort.py` & `magma-lang-2.2.9/magma/passes/tsort.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/placer.py` & `magma-lang-2.2.9/magma/placer.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/primitives/lut.py` & `magma-lang-2.2.9/magma/primitives/lut.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/primitives/memory.py` & `magma-lang-2.2.9/magma/primitives/memory.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/primitives/mux.py` & `magma-lang-2.2.9/magma/primitives/mux.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/primitives/register.py` & `magma-lang-2.2.9/magma/primitives/register.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/primitives/set_index.py` & `magma-lang-2.2.9/magma/primitives/set_index.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/primitives/slice.py` & `magma-lang-2.2.9/magma/primitives/slice.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/primitives/wire.py` & `magma-lang-2.2.9/magma/primitives/wire.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/protocol_type.py` & `magma-lang-2.2.9/magma/protocol_type.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/ref.py` & `magma-lang-2.2.9/magma/ref.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/scope.py` & `magma-lang-2.2.9/magma/scope.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/simulator/coreir_simulator.py` & `magma-lang-2.2.9/magma/simulator/coreir_simulator.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/simulator/mdb.py` & `magma-lang-2.2.9/magma/simulator/mdb.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/simulator/python_simulator.py` & `magma-lang-2.2.9/magma/simulator/python_simulator.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/simulator/simulator.py` & `magma-lang-2.2.9/magma/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/smart/smart_bits.py` & `magma-lang-2.2.9/magma/smart/smart_bits.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/ssa/ssa.py` & `magma-lang-2.2.9/magma/ssa/ssa.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/symbol_table.py` & `magma-lang-2.2.9/magma/symbol_table.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/symbol_table_utils.py` & `magma-lang-2.2.9/magma/symbol_table_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/syntax/combinational.py` & `magma-lang-2.2.9/magma/syntax/combinational.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/syntax/combinational2.py` & `magma-lang-2.2.9/magma/syntax/combinational2.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/syntax/coroutine.py` & `magma-lang-2.2.9/magma/syntax/coroutine.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/syntax/inline_combinational.py` & `magma-lang-2.2.9/magma/syntax/inline_combinational.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/syntax/sequential2.py` & `magma-lang-2.2.9/magma/syntax/sequential2.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/syntax/transforms/inline_yield_from.py` & `magma-lang-2.2.9/magma/syntax/transforms/inline_yield_from.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/syntax/transforms/replace_symbols.py` & `magma-lang-2.2.9/magma/syntax/transforms/replace_symbols.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/syntax/util.py` & `magma-lang-2.2.9/magma/syntax/util.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/syntax/verilog.py` & `magma-lang-2.2.9/magma/syntax/verilog.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/syntax/verilog_utils.py` & `magma-lang-2.2.9/magma/syntax/verilog_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/t.py` & `magma-lang-2.2.9/magma/t.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/testing/utils.py` & `magma-lang-2.2.9/magma/testing/utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/transforms.py` & `magma-lang-2.2.9/magma/transforms.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/tuple.py` & `magma-lang-2.2.9/magma/tuple.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/type_utils.py` & `magma-lang-2.2.9/magma/type_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/types/bit_pattern.py` & `magma-lang-2.2.9/magma/types/bit_pattern.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/types/ready_valid.py` & `magma-lang-2.2.9/magma/types/ready_valid.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/uniquification.py` & `magma-lang-2.2.9/magma/uniquification.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/util.py` & `magma-lang-2.2.9/magma/util.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/value_utils.py` & `magma-lang-2.2.9/magma/value_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/verilog_utils.py` & `magma-lang-2.2.9/magma/verilog_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/view.py` & `magma-lang-2.2.9/magma/view.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/waveform.py` & `magma-lang-2.2.9/magma/waveform.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/wire.py` & `magma-lang-2.2.9/magma/wire.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma/wire_container.py` & `magma-lang-2.2.9/magma/wire_container.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/magma_lang.egg-info/PKG-INFO` & `magma-lang-2.2.9/magma_lang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magma-lang
-Version: 2.2.8
+Version: 2.2.9
 Summary: An embedded DSL for constructing hardware circuits
 Home-page: https://github.com/phanrahan/magma
 Maintainer: Lenny Truong
 Maintainer-email: lenny@cs.stanford.edu
 License: MIT
 Description: # Magma
         [![Documentation Status](https://readthedocs.org/projects/magma/badge/?version=latest)](https://magma.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `magma-lang-2.2.8/magma_lang.egg-info/SOURCES.txt` & `magma-lang-2.2.9/magma_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/setup.cfg` & `magma-lang-2.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.8/setup.py` & `magma-lang-2.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='magma-lang',
-    version='2.2.8',
+    version='2.2.9',
     url='https://github.com/phanrahan/magma',
     license='MIT',
     maintainer='Lenny Truong',
     maintainer_email='lenny@cs.stanford.edu',
     description='An embedded DSL for constructing hardware circuits',
     scripts=['bin/magma'],
     packages=[
```

