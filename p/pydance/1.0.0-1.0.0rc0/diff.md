# Comparing `tmp/pydance-1.0.0.tar.gz` & `tmp/pydance-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydance-1.0.0.tar", last modified: Thu Jun 29 17:00:35 2023, max compression
+gzip compressed data, was "pydance-1.0.0rc0.tar", last modified: Sun Aug 21 01:03:23 2022, max compression
```

## Comparing `pydance-1.0.0.tar` & `pydance-1.0.0rc0.tar`

### file list

```diff
@@ -1,126 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.188492 pydance-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    28556 2023-06-29 17:00:35.188492 pydance-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27840 2023-06-29 17:00:28.000000 pydance-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.176492 pydance-1.0.0/dance/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.176492 pydance-1.0.0/dance/data/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/data/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.180492 pydance-1.0.0/dance/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/datasets/multimodality.py
--rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/datasets/singlemodality.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/datasets/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.180492 pydance-1.0.0/dance/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.180492 pydance-1.0.0/dance/models/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/models/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/models/nn/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/models/nn/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.180492 pydance-1.0.0/dance/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.180492 pydance-1.0.0/dance/modules/multi_modality/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.180492 pydance-1.0.0/dance/modules/multi_modality/joint_embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/joint_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40513 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/joint_embedding/dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/joint_embedding/jae.py
--rw-r--r--   0 runner    (1001) docker     (123)    13476 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/joint_embedding/scmogcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    46284 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/joint_embedding/scmogcnv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30504 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/joint_embedding/scmvae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.180492 pydance-1.0.0/dance/modules/multi_modality/match_modality/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/match_modality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/match_modality/cmae.py
--rw-r--r--   0 runner    (1001) docker     (123)    24559 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/match_modality/scmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13638 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/match_modality/scmogcn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.180492 pydance-1.0.0/dance/modules/multi_modality/predict_modality/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/predict_modality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31706 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/predict_modality/babel.py
--rw-r--r--   0 runner    (1001) docker     (123)    22497 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/predict_modality/cmae.py
--rw-r--r--   0 runner    (1001) docker     (123)    24926 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/predict_modality/scmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    30722 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/multi_modality/predict_modality/scmogcn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.180492 pydance-1.0.0/dance/modules/single_modality/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.180492 pydance-1.0.0/dance/modules/single_modality/cell_type_annotation/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/cell_type_annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/cell_type_annotation/actinn.py
--rw-r--r--   0 runner    (1001) docker     (123)    42191 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/cell_type_annotation/celltypist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/cell_type_annotation/scdeepsort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/cell_type_annotation/singlecellnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/cell_type_annotation/svm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.184492 pydance-1.0.0/dance/modules/single_modality/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/clustering/graphsc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/clustering/scdcc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/clustering/scdeepcluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    18183 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/clustering/scdsc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/clustering/sctag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.184492 pydance-1.0.0/dance/modules/single_modality/imputation/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/imputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/imputation/deepimpute.py
--rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/imputation/graphsci.py
--rw-r--r--   0 runner    (1001) docker     (123)    51951 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/single_modality/imputation/scgnn2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.184492 pydance-1.0.0/dance/modules/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/spatial/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.184492 pydance-1.0.0/dance/modules/spatial/cell_type_deconvo/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/spatial/cell_type_deconvo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/spatial/cell_type_deconvo/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/spatial/cell_type_deconvo/dstg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/spatial/cell_type_deconvo/spatialdecon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/spatial/cell_type_deconvo/spotlight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.184492 pydance-1.0.0/dance/modules/spatial/spatial_domain/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/spatial/spatial_domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22048 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/spatial/spatial_domain/louvain.py
--rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/spatial/spatial_domain/spagcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/spatial/spatial_domain/stagate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/modules/spatial/spatial_domain/stlearn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.184492 pydance-1.0.0/dance/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.184492 pydance-1.0.0/dance/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/cell_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22974 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/gene_holdout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.184492 pydance-1.0.0/dance/transforms/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/graph/cell_feature_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/graph/dstg_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/graph/feature_feature_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/graph/neighbor_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/graph/scmogcn_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/graph/spatial_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    38959 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/graph_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    31875 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/pseudo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/scn_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/spatial_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/transforms/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.188492 pydance-1.0.0/dance/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    26007 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/utils/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-29 17:00:28.000000 pydance-1.0.0/dance/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:35.188492 pydance-1.0.0/pydance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28556 2023-06-29 17:00:35.000000 pydance-1.0.0/pydance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-29 17:00:35.000000 pydance-1.0.0/pydance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:00:35.000000 pydance-1.0.0/pydance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 17:00:35.000000 pydance-1.0.0/pydance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 17:00:35.000000 pydance-1.0.0/pydance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-29 17:00:28.000000 pydance-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-29 17:00:35.188492 pydance-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:00:28.000000 pydance-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.791247 pydance-1.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (121)    27343 2022-08-21 01:03:23.791247 pydance-1.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    26564 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.779247 pydance-1.0.0rc0/dance/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.779247 pydance-1.0.0rc0/dance/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.783247 pydance-1.0.0rc0/dance/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24392 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/datasets/multimodality.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32362 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/datasets/singlemodality.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12479 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/datasets/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.783247 pydance-1.0.0rc0/dance/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.783247 pydance-1.0.0rc0/dance/modules/multi_modality/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.783247 pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40714 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/dcca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9599 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/jae.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9865 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/scmogcn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46284 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/scmogcnv2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30760 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/scmvae.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.783247 pydance-1.0.0rc0/dance/modules/multi_modality/match_modality/
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/match_modality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22954 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/match_modality/cmae.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24653 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/match_modality/scmm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10160 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/match_modality/scmogcn.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.783247 pydance-1.0.0rc0/dance/modules/multi_modality/predict_modality/
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/predict_modality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37264 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/predict_modality/babel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22770 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/predict_modality/cmae.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24782 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/predict_modality/scmm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30099 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/multi_modality/predict_modality/scmogcn.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.783247 pydance-1.0.0rc0/dance/modules/single_modality/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.787247 pydance-1.0.0rc0/dance/modules/single_modality/cell_type_annotation/
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/cell_type_annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6190 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/cell_type_annotation/actinn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68913 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/cell_type_annotation/celltypist.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18802 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/cell_type_annotation/scdeepsort.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11793 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/cell_type_annotation/singlecellnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5353 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/cell_type_annotation/svm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.787247 pydance-1.0.0rc0/dance/modules/single_modality/clustering/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19352 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/clustering/graphsc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20015 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/clustering/scdcc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16925 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/clustering/scdeepcluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20149 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/clustering/scdsc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13772 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/clustering/sctag.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.787247 pydance-1.0.0rc0/dance/modules/single_modality/imputation/
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/imputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15559 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/imputation/deepimpute.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17505 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/imputation/graphsci.py
+-rw-r--r--   0 runner    (1001) docker     (121)    70888 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/single_modality/imputation/scgnn.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.787247 pydance-1.0.0rc0/dance/modules/spatial/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/spatial/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.787247 pydance-1.0.0rc0/dance/modules/spatial/cell_type_deconvo/
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/spatial/cell_type_deconvo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15421 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/spatial/cell_type_deconvo/card.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11158 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/spatial/cell_type_deconvo/dstg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7262 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/spatial/cell_type_deconvo/spatialdecon.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10548 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/spatial/cell_type_deconvo/spotlight.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.787247 pydance-1.0.0rc0/dance/modules/spatial/spatial_domain/
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/spatial/spatial_domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21734 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/spatial/spatial_domain/louvain.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24420 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/spatial/spatial_domain/spagcn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13271 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/spatial/spatial_domain/stagate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6262 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/modules/spatial/spatial_domain/stlearn.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.787247 pydance-1.0.0rc0/dance/plotting/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.791247 pydance-1.0.0rc0/dance/transforms/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    59402 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/transforms/graph_construct.py
+-rw-r--r--   0 runner    (1001) docker     (121)   130471 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/transforms/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.791247 pydance-1.0.0rc0/dance/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     3138 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26056 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6852 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/dance/utils/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 01:03:23.791247 pydance-1.0.0rc0/pydance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    27343 2022-08-21 01:03:23.000000 pydance-1.0.0rc0/pydance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2914 2022-08-21 01:03:23.000000 pydance-1.0.0rc0/pydance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-21 01:03:23.000000 pydance-1.0.0rc0/pydance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-08-21 01:03:23.000000 pydance-1.0.0rc0/pydance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-21 01:03:23.000000 pydance-1.0.0rc0/pydance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-08-21 01:03:23.791247 pydance-1.0.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-21 01:03:15.000000 pydance-1.0.0rc0/setup.py
```

### Comparing `pydance-1.0.0/PKG-INFO` & `pydance-1.0.0rc0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pydance
-Version: 1.0.0
+Version: 1.0.0rc0
 Summary: Deep Learning for Single-cell Analysis
 Home-page: https://github.com/OmicsML/dance
 Author: "DANCE Team"
 Author-email: "danceteamgnn@gmail.com"
 License: BSD 2-Clause License
 Keywords: Single-cell Biology,Deep Learning,Graph Neural Networks
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: doc
 
 <p align="center">
   <img
        src="https://github.com/OmicsML/dance/blob/main/imgs/dance_logo.jpg"
        style="width:100%; height:100%; object-fit:cover;"
   />
 </p>
@@ -29,170 +29,124 @@
 ______________________________________________________________________
 
 [![PyPI version](https://badge.fury.io/py/pydance.svg)](https://badge.fury.io/py/pydance)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Documentation Status](https://readthedocs.org/projects/pydance/badge/?version=latest)](https://pydance.readthedocs.io/en/latest/?badge=latest)
 [![Test Examples](https://github.com/OmicsML/dance/actions/workflows/test_examples.yml/badge.svg)](https://github.com/OmicsML/dance/actions/workflows/test_examples.yml)
 
-[![Slack](https://img.shields.io/badge/slack-OmicsML-brightgreen)](https://omicsml.slack.com)
-[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Ftwitter.com%2FOmicsML)](https://twitter.com/OmicsML)
-
-DANCE is a Python toolkit to support deep learning models for analyzing single-cell gene expression at scale. Our goal is to build up a deep learning community and benchmark platform for computational models in single-cell analysis. It includes three modules at present:
+DANCE is a Python toolkit to support deep learning models for analyzing single-cell gene expression at scale. It includes three modules at present:
 
 1. **Single-modality analysis**
 1. **Single-cell multimodal omics**
 1. **Spatially resolved transcriptomics**
 
-### Useful links
-
-OmicsML Homepage: https://omicsml.ai \
-DANCE Open Source: https://github.com/OmicsML/dance \
-DANCE Documentation: https://pydance.readthedocs.io/en/latest/ \
-DANCE Tutorials: https://github.com/OmicsML/dance-tutorials \
-DANCE Package Paper: https://www.biorxiv.org/content/10.1101/2022.10.19.512741v2 \
-Survey Paper: https://arxiv.org/abs/2210.12385
-
-### Join the Community
-
-Slack: https://join.slack.com/t/omicsml/shared_invite/zt-1hxdz7op3-E5K~EwWF1xDvhGZFrB9AbA \
-Twitter: https://twitter.com/OmicsML \
-Wechat Group Assistant: 736180290 \
-Email: danceteamgnn@gmail.com
-
-### Contributing
-
-Community-wide contribution is the key for a sustainable development and
-continual growth of the DANCE package. We deeply appreciate any contribution
-made to improve the DANCE code base. If you would like to get started, please
-refer to our brief [guidelines](CONTRIBUTING.md) about our automated quality
-controls, as well as setting up the `dev` environments.
-
-## Citation
-
-If you find our work useful in your research, please consider citing our DANCE package or survey paper:
-
-```bibtex
-@article{ding2022dance,
-  title={DANCE: A Deep Learning Library and Benchmark for Single-Cell Analysis},
-  author={Ding, Jiayuan and Wen, Hongzhi and Tang, Wenzhuo and Liu, Renming and Li, Zhaoheng and Venegas, Julian and Su, Runze and Molho, Dylan and Jin, Wei and Zuo, Wangyang and others},
-  journal={bioRxiv},
-  year={2022},
-  publisher={Cold Spring Harbor Laboratory}
-}
-```
-
-```bibtex
-@article{molho2022deep,
-  title={Deep Learning in Single-Cell Analysis},
-  author={Molho, Dylan and Ding, Jiayuan and Li, Zhaoheng and Wen, Hongzhi and Tang, Wenzhuo and Wang, Yixin and Venegas, Julian and Jin, Wei and Liu, Renming and Su, Runze and others},
-  journal={arXiv preprint arXiv:2210.12385},
-  year={2022}
-}
-```
+Our goal is to build up a deep learning community for single cell analysis and provide GNN based architecture for users for further development in single cell analysis.
 
 ## Usage
 
 ### Overview
 
-In release 1.0, the main usage of the DANCE is to provide readily available experiment reproduction
+In release 1.0, the main usage of the PyDANCE is to provide readily available experiment reproduction
 (see detail information about the reproduced performance [below](#implemented-algorithms)).
-Users can easily reproduce selected experiments presented in the original papers for the computational single-cell methods implemented in DANCE, which can be found under [`examples/`](examples).
+Users can easily reproduce selected experiments presented in the original papers for the computational single-cell methods implemented in PyDANCE, which can be found under [`examples/`](examples).
 
 ### Motivation
 
 Computational methods for single-cell analysis are quickly emerging, and the field is revolutionizing the usage of single-cell data to gain biological insights.
 A key challenge to continually developing computational single-cell methods that achieve new state-of-the-art performance is reproducing previous benchmarks.
 More specifically, different studies prepare their datasets and perform evaluation differently,
 and not to mention the compatibility of different methods, as they could be written in different languages or using incompatible library versions.
 
-DANCE addresses these challenges by providing a unified Python package implementing many popular computational single-cell methods (see [Implemented Algorithms](#implemented-algorithms)),
+PyDANCE addresses these challenges by providing a unified Python packge implementing many popular computational single-cell methods (see [Implemented Algorithms](#implemented-algorithms)),
 as well as easily reproducible experiments by providing unified tools for
 
 - Data downloading
 - Data (pre-)processing and transformation (e.g. graph construction)
 - Model training and evaluation
 
-### Example: run cell-type annotation benchmark using scDeepSort
+### Example: runing cell-type annotation benchmark using scDeepSort
 
-- Step0. Install DANCE (see [Installation](#installation))
+- Step0. Install PyDANCE (see [Installation](#installation))
 - Step1. Navigate to the folder containing the corresponding example scrtip.
   In this case, it is [`examples/single_modality/cell_type_annotation`](examples/single_modality/cell_type_annotation).
 - Step2. Obtain command line interface (CLI) options for a particular experiment to reproduce at the end of the
   [script](examples/single_modality/cell_type_annotation/scdeepsort.py).
   For example, the CLI options for reproducing the `Mouse Brain` experiment is
   ```bash
-  python scdeepsort.py --species mouse --tissue Brain --train_dataset 753 3285 --test_dataset 2695
+  python scdeepsort.py --data_type scdeepsort --tissue Brain --test_data 2695
   ```
-- Step3. Wait for the experiment to finish and check results.
+- Step3. Wait for the experiment to finsh and check results.
 
 ## Installation
 
 <H3>Quick install</H3>
 
 The full installation process might be a bit tedious and could involve some debugging when using CUDA enabled packages.
 Thus, we provide an `install.sh` script that simplifies the installation process, assuming the user have [conda](https://conda.io/projects/conda/en/latest/index.html) set up on their machines.
-The installation script creates a conda environment `dance` and install the DANCE package along with all its dependencies with a apseicifc CUDA version.
-Currently, two options are accepted: `cpu` and  `cu117`.
-For example, to install the DANCE package using CUDA11.7 in a `dance-env` conda environment, simply run:
+The installation script creates a conda environment `pydance` and install the PyDANCE package along with all its dependencies with a apseicifc CUDA version.
+Currently, three options are accepted: `cpu`, `cu102`, and `cu113`.
+For example, to install the DANCE package using CUDA10.2, simply run:
 
 ```bash
-# Clone the repository via SSH
-git clone git@github.com:OmicsML/dance.git && cd dance
-# Alternatively, use HTTPS if you have not set up SSH
-# git clone https://github.com/OmicsML/dance.git  && cd dance
+git clone git@github.com:OmicsML/dance.git
+cd dance
 
-# Run the auto installation script to install DANCE and its dependencies in a conda environment
-source install.sh cu117 dance-env
+source install.sh cu102
 ```
 
-**Note**: the first argument for cuda version is mandatory, while the second argument for conda environment name is optional (default is `dance`).
-
 <details>
 <summary><H3>Custom install</H3></summary>
 <br>
 
 **Step1. Setup environment**
 
-First create a conda environment for dance (optional)
+First create a conda environment for pydance (optional)
 
 ```bash
-conda create -n dance python=3.8 -y && conda activate dance-dev
+conda create -n pydance python=3.8 -y && conda activate dance-dev
 ```
 
-Then, install CUDA enabled packages (PyTorch, PyG, DGL):
+Then, install CUDA enabled packages (PyTorch, PyG, DGL) with CUDA 10.2:
 
 ```bash
-conda install pytorch=2.0.0 torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia -y
-conda install pyg=2.3.0 -c pyg -y
-conda install dgl=1.0.1 -c dglteam/label/cu117 -y
+conda install pytorch=1.12.1 torchvision cudatoolkit=10.2 -c pytorch -y
+conda install dgl-cu102 -c dglteam -y
+pip install torch-geometric==2.1.0 torch-scatter torch-sparse torch-cluster -f https://data.pyg.org/whl/torch-1.12.1+cu102.html
 ```
 
 Alternatively, install these dependencies for CPU only:
 
 ```bash
-conda install pytorch=2.0.0 torchvision torchaudio cpuonly -c pytorch -y
-conda install pyg=2.3.0 -c pyg -y
-conda install dgl -c dglteam -y
+conda install pytorch=1.12.1 torchvision cpuonly -c pytorch -y
+conda install dgl -c dglteam
+pip install torch-geometric==2.1.0 torch-scatter torch-sparse torch-cluster -f https://data.pyg.org/whl/torch-1.12.1+cpu.html
+```
+
+**Note:** If you installed PyG using conda and encountered an issue with `GLIBC_2.27` when importing `torch_geometric.nn`,
+then you may need to uninstall `torch-spline-conv` (see https://github.com/pyg-team/pytorch_geometric/issues/3593)
+
+```bash
+pip uninstall torch-spline-conv
 ```
 
-For more information about installation or other CUDA version options, check out the installation pages for the corresponding packages
+For more information about installation or other CUDA version options, check out the installation pages for the corresponding packges
 
 - [PyTorch](https://pytorch.org/get-started/)
 - [PyG](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html)
 - [DGL](https://www.dgl.ai/pages/start.html)
 
-**Step2. Install DANCE**
+**Step2. Install PyDANCE**
 
 Install from PyPI
 
 ```bash
 pip install pydance
 ```
 
-Or, install the latest dev version from source
+Install the latest dev version from source
 
 ```bash
 git clone https://github.com/OmicsML/dance.git
 cd dance
 pip install -e .
 ```
 
@@ -214,41 +168,43 @@
 | GNN                 | GNNImpute    | An efficient scRNA-seq dropout imputation method using graph attention network                               | 2021 | P1      |
 | Graph Diffusion     | MAGIC        | MAGIC: A diffusion-based imputation method reveals gene-gene interactions in single-cell RNA-sequencing data | 2018 | P1      |
 | Probabilistic Model | scImpute     | An accurate and robust imputation method scImpute for single-cell RNA-seq data                               | 2018 | P1      |
 | GAN                 | scGAIN       | scGAIN: Single Cell RNA-seq Data Imputation using Generative Adversarial Networks                            | 2019 | P1      |
 | NN                  | DeepImpute   | DeepImpute: an accurate, fast, and scalable deep neural network method to impute single-cell RNA-seq data    | 2019 | ✅       |
 | NN + TF             | Saver-X      | Transfer learning in single-cell transcriptomics improves data denoising and pattern discovery               | 2019 | P1      |
 
-| Model      | Evaluation Metric | Mouse Brain (current/reported) | Mouse Embryo (current/reported) | PBMC (current/reported) |
-| ---------- | ----------------- | ------------------------------ | ------------------------------- | ----------------------- |
-| DeepImpute | RMSE              | 0.87 / N/A                     | 1.20 / N/A                      | 2.30 / N/A              |
-| GraphSCI   | RMSE              | 1.55 / N/A                     | 1.81 / N/A                      | 3.68 / N/A              |
-| scGNN2.0   | MSE               | 1.04 / N/A                     | 1.12 / N/A                      | 1.22 / N/A              |
+| Model      | Evaluation Metric | Mouse Brain (current/reported) | Mouse Embryo (current/reported) |
+| ---------- | ----------------- | ------------------------------ | ------------------------------- |
+| DeepImpute | MSE               | 0.12 / N/A                     | 0.12 / N/A                      |
+| ScGNN      | MSE               | 0.47 / N/A                     | 1.10 / N/A                      |
+| GraphSCI   | MSE               | 0.42 / N/A                     | 0.87 / N/A                      |
 
-**Note**: scGNN2.0 is evaluated on 2,000 genes with highest variance following the original paper.
+Note: the data split modality of DeepImpute is different from ScGNN and GraphSCI, so the results are not comparable.
 
 #### 2）Cell Type Annotation
 
-| BackBone                | Model         | Algorithm                                                                                                     | Year | CheckIn |
-| ----------------------- | ------------- | ------------------------------------------------------------------------------------------------------------- | ---- | ------- |
-| GNN                     | ScDeepsort    | Single-cell transcriptomics with weighted GNN                                                                 | 2021 | ✅       |
-| Logistic Regression     | Celltypist    | Cross-tissue immune cell analysis reveals tissue-specific features in humans.                                 | 2021 | ✅       |
-| Random Forest           | singleCellNet | SingleCellNet: a computational tool to classify single cell RNA-Seq data across platforms and across species. | 2019 | ✅       |
-| Neural Network          | ACTINN        | ACTINN: automated identification of cell types in single cell RNA sequencing.                                 | 2020 | ✅       |
-| Hierarchical Clustering | SingleR       | Reference-based analysis of lung single-cell sequencing reveals a transitional profibrotic macrophage.        | 2019 | P1      |
-| SVM                     | SVM           | A comparison of automatic cell identification methods for single-cell RNA sequencing data.                    | 2018 | ✅       |
+| BackBone                | Model         | Algorithm                                                                                                    | Year | CheckIn |
+| ----------------------- | ------------- | ------------------------------------------------------------------------------------------------------------ | ---- | ------- |
+| GNN                     | ScDeepsort    | Single-cell transcriptomics with weighted GNN                                                                | 2021 | ✅       |
+| Logistic Regression     | Celltypist    | Automated cell type annotation for scRNA-seq datasets                                                        | 2021 | ✅       |
+| Random Forest           | singleCellNet | SingleCellNet: a computational tool to classify single cell RNA-Seq data across platforms and across species | 2019 | ✅       |
+| Neural Network          | ACTINN        | ACTINN: automated identification of cell types in single cell RNA sequencing.                                | 2020 | ✅       |
+| Hierarchical Clustering | SingleR       | Reference-based analysis of lung single-cell sequencing reveals a transitional profibrotic macrophage.       | 2019 | P1      |
+| SVM                     | SVM           | A comparison of automatic cell identification methods for single-cell RNA sequencing data.                   | 2018 | ✅       |
 
 | Model         | Evaluation Metric | Mouse Brain 2695 (current/reported) | Mouse Spleen 1759 (current/reported) | Mouse Kidney 203 (current/reported) |
 | ------------- | ----------------- | ----------------------------------- | ------------------------------------ | ----------------------------------- |
-| scDeepsort    | ACC               | 0.542/0.363                         | 0.969/0.965                          | 0.847/0.911                         |
-| Celltypist    | ACC               | 0.824/0.666                         | 0.908/0.848                          | 0.823/0.832                         |
+| scDeepsort    | ACC               | 0.363/0.363                         | 0.965 /0.965                         | 0.901/0.911                         |
+| Celltypist\*  | ACC               | 0.680/0.666                         | 0.966/0.848                          | 0.879/0.832                         |
 | singleCellNet | ACC               | 0.693/0.803                         | 0.975/0.975                          | 0.795/0.842                         |
-| ACTINN        | ACC               | 0.727/0.778                         | 0.657/0.236                          | 0.762/0.798                         |
+| ACTINN        | ACC               | 0.860/0.778                         | 0.516/0.236                          | 0.829/0.798                         |
 | SVM           | ACC               | 0.683/0.683                         | 0.056/0.049                          | 0.704/0.695                         |
 
+Note: * Benchmark datasets were renormalied before running the original implementation of Celltypist to match its form requirements.
+
 #### 3）Clustering
 
 | BackBone    | Model         | Algorithm                                                                                                    | Year | CheckIn |
 | ----------- | ------------- | ------------------------------------------------------------------------------------------------------------ | ---- | ------- |
 | GNN         | graph-sc      | GNN-based embedding for clustering scRNA-seq data                                                            | 2022 | ✅       |
 | GNN         | scTAG         | ZINB-based Graph Embedding Autoencoder for Single-cell RNA-seq Interpretations                               | 2022 | ✅       |
 | GNN         | scDSC         | Deep structural clustering for single-cell RNA-seq data jointly through autoencoder and graph neural network | 2022 | ✅       |
@@ -259,24 +215,25 @@
 
 | Model         | Evaluation Metric | 10x PBMC (current/reported) | Mouse ES (current/reported) | Worm Neuron (current/reported) | Mouse Bladder (current/reported) |
 | ------------- | ----------------- | --------------------------- | --------------------------- | ------------------------------ | -------------------------------- |
 | graph-sc      | ARI               | 0.72 / 0.70                 | 0.82 / 0.78                 | 0.57 / 0.46                    | 0.68 / 0.63                      |
 | scDCC         | ARI               | 0.82 / 0.81                 | 0.98 / N/A                  | 0.51 / 0.58                    | 0.60 / 0.66                      |
 | scDeepCluster | ARI               | 0.81 / 0.78                 | 0.98 / 0.97                 | 0.51 / 0.52                    | 0.56 / 0.58                      |
 | scDSC         | ARI               | 0.72 / 0.78                 | 0.84 / N/A                  | 0.46 / 0.65                    | 0.65 / 0.72                      |
-| scTAG         | ARI               | 0.77 / N/A                  | 0.96 / N/A                  | 0.49 / N/A                     | 0.69 / N/A                       |
+| scTAG         | ARI               | 0.75 / N/A                  | 0.96 / N/A                  | 0.53 / N/A                     | 0.60 / N/A                       |
 
 ### Multimodality Module
 
 #### 1）Modality Prediction
 
 | BackBone         | Model                    | Algorithm                                                                                          | Year | CheckIn |
 | ---------------- | ------------------------ | -------------------------------------------------------------------------------------------------- | ---- | ------- |
 | GNN              | ScMoGCN                  | Graph Neural Networks for Multimodal Single-Cell Data Integration                                  | 2022 | ✅       |
 | GNN              | ScMoLP                   | Link Prediction Variant of ScMoGCN                                                                 | 2022 | P1      |
+| GNN              | scGNN                    | scGNN is a novel graph neural network framework for single-cell RNA-Seq analyses                   | 2021 | P1      |
 | GNN              | GRAPE                    | Handling Missing Data with Graph Representation Learning                                           | 2020 | P1      |
 | Generative Model | SCMM                     | SCMM: MIXTURE-OF-EXPERTS MULTIMODAL DEEP GENERATIVE MODEL FOR SINGLE-CELL MULTIOMICS DATA ANALYSIS | 2021 | ✅       |
 | Auto-encoder     | Cross-modal autoencoders | Multi-domain translation between single-cell imaging and sequencing data using autoencoders        | 2021 | ✅       |
 | Auto-encoder     | BABEL                    | BABEL enables cross-modality translation between multiomic profiles at single-cell resolution      | 2021 | ✅       |
 
 | Model                    | Evaluation Metric | GEX2ADT (current/reported) | ADT2GEX (current/reported) | GEX2ATAC (current/reported) | ATAC2GEX (current/reported) |
 | ------------------------ | ----------------- | -------------------------- | -------------------------- | --------------------------- | --------------------------- |
@@ -286,15 +243,15 @@
 | BABEL                    | RMSE              | 0.4335 / N/A               | 0.3673 / N/A               | 0.1816 / N/A                | 0.2394 / N/A                |
 
 #### 2) Modality Matching
 
 | BackBone         | Model                    | Algorithm                                                                                          | Year | CheckIn |
 | ---------------- | ------------------------ | -------------------------------------------------------------------------------------------------- | ---- | ------- |
 | GNN              | ScMoGCN                  | Graph Neural Networks for Multimodal Single-Cell Data Integration                                  | 2022 | ✅       |
-| GNN/Auto-ecnoder | GLUE                     | Multi-omics single-cell data integration and regulatory inference with graph-linked embedding      | 2021 | P1      |
+| GNN              | scGNN                    | scGNN is a novel graph neural network framework for single-cell RNA-Seq analyses                   | 2021 | P1      |
 | Generative Model | SCMM                     | SCMM: MIXTURE-OF-EXPERTS MULTIMODAL DEEP GENERATIVE MODEL FOR SINGLE-CELL MULTIOMICS DATA ANALYSIS | 2021 | ✅       |
 | Auto-encoder     | Cross-modal autoencoders | Multi-domain translation between single-cell imaging and sequencing data using autoencoders        | 2021 | ✅       |
 
 | Model                    | Evaluation Metric | GEX2ADT (current/reported) | GEX2ATAC (current/reported) |
 | ------------------------ | ----------------- | -------------------------- | --------------------------- |
 | ScMoGCN                  | Accuracy          | 0.0827 / 0.0810            | 0.0600 / 0.0630             |
 | SCMM                     | Accuracy          | 0.005 / N/A                | 5e-5 / N/A                  |
@@ -364,13 +321,47 @@
 | GNN                        | DSTG         | DSTG: deconvoluting spatial transcriptomics data through graph-based artificial intelligence                  | 2021 | ✅       |
 | logNormReg                 | SpatialDecon | Advances in mixed cell deconvolution enable quantification of cell types in spatial transcriptomic data       | 2022 | ✅       |
 | NNMFreg                    | SPOTlight    | SPOTlight: seeded NMF regression to deconvolute spatial transcriptomics spots with single-cell transcriptomes | 2021 | ✅       |
 | NN Linear + CAR assumption | CARD         | Spatially informed cell-type deconvolution for spatial transcriptomics                                        | 2022 | ✅       |
 
 | Model        | Evaluation Metric | GSE174746 (current/reported) | CARD Synthetic (current/reported) | SPOTlight Synthetic (current/reported) |
 | ------------ | ----------------- | ---------------------------- | --------------------------------- | -------------------------------------- |
-| DSTG         | MSE               | .1722 / N/A                  | .0239 / N/A                       | .0315 / N/A                            |
+| DSTG         | MSE               | .172 / N/A                   | .0247 / N/A                       | .042 / N/A                             |
 | SpatialDecon | MSE               | .0014 / .009                 | .0077 / N/A                       | .0055 / N/A                            |
 | SPOTlight    | MSE               | .0098 / N/A                  | .0246 / 0.118                     | .0109 / .16                            |
 | CARD         | MSE               | .0012 / N/A                  | .0078 / 0.0062                    | .0076 / N/A                            |
 
+## Dev notes
+
+### Dev installation
+
+Install PyDANCE with extra dependencies for dev
+
+```bash
+pip install -e ."[dev]"
+```
+
+Make sure dependencies have specific pinned versions
 
+```bash
+pip install -r requirements.txt
+```
+
+Install pre-commit hooks for code quality checks
+
+```bash
+pre-commit install
+```
+
+### Run tests
+
+Run all tests on current environment using pytest
+
+```bash
+pytest -v
+```
+
+Run full test from the ground up including environment set up using [tox](https://tox.wiki/en/latest/) on CPU
+
+```bash
+tox -e python3.8-cpu
+```
```

### Comparing `pydance-1.0.0/README.md` & `pydance-1.0.0rc0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,170 +8,124 @@
 ______________________________________________________________________
 
 [![PyPI version](https://badge.fury.io/py/pydance.svg)](https://badge.fury.io/py/pydance)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Documentation Status](https://readthedocs.org/projects/pydance/badge/?version=latest)](https://pydance.readthedocs.io/en/latest/?badge=latest)
 [![Test Examples](https://github.com/OmicsML/dance/actions/workflows/test_examples.yml/badge.svg)](https://github.com/OmicsML/dance/actions/workflows/test_examples.yml)
 
-[![Slack](https://img.shields.io/badge/slack-OmicsML-brightgreen)](https://omicsml.slack.com)
-[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Ftwitter.com%2FOmicsML)](https://twitter.com/OmicsML)
-
-DANCE is a Python toolkit to support deep learning models for analyzing single-cell gene expression at scale. Our goal is to build up a deep learning community and benchmark platform for computational models in single-cell analysis. It includes three modules at present:
+DANCE is a Python toolkit to support deep learning models for analyzing single-cell gene expression at scale. It includes three modules at present:
 
 1. **Single-modality analysis**
 1. **Single-cell multimodal omics**
 1. **Spatially resolved transcriptomics**
 
-### Useful links
-
-OmicsML Homepage: https://omicsml.ai \
-DANCE Open Source: https://github.com/OmicsML/dance \
-DANCE Documentation: https://pydance.readthedocs.io/en/latest/ \
-DANCE Tutorials: https://github.com/OmicsML/dance-tutorials \
-DANCE Package Paper: https://www.biorxiv.org/content/10.1101/2022.10.19.512741v2 \
-Survey Paper: https://arxiv.org/abs/2210.12385
-
-### Join the Community
-
-Slack: https://join.slack.com/t/omicsml/shared_invite/zt-1hxdz7op3-E5K~EwWF1xDvhGZFrB9AbA \
-Twitter: https://twitter.com/OmicsML \
-Wechat Group Assistant: 736180290 \
-Email: danceteamgnn@gmail.com
-
-### Contributing
-
-Community-wide contribution is the key for a sustainable development and
-continual growth of the DANCE package. We deeply appreciate any contribution
-made to improve the DANCE code base. If you would like to get started, please
-refer to our brief [guidelines](CONTRIBUTING.md) about our automated quality
-controls, as well as setting up the `dev` environments.
-
-## Citation
-
-If you find our work useful in your research, please consider citing our DANCE package or survey paper:
-
-```bibtex
-@article{ding2022dance,
-  title={DANCE: A Deep Learning Library and Benchmark for Single-Cell Analysis},
-  author={Ding, Jiayuan and Wen, Hongzhi and Tang, Wenzhuo and Liu, Renming and Li, Zhaoheng and Venegas, Julian and Su, Runze and Molho, Dylan and Jin, Wei and Zuo, Wangyang and others},
-  journal={bioRxiv},
-  year={2022},
-  publisher={Cold Spring Harbor Laboratory}
-}
-```
-
-```bibtex
-@article{molho2022deep,
-  title={Deep Learning in Single-Cell Analysis},
-  author={Molho, Dylan and Ding, Jiayuan and Li, Zhaoheng and Wen, Hongzhi and Tang, Wenzhuo and Wang, Yixin and Venegas, Julian and Jin, Wei and Liu, Renming and Su, Runze and others},
-  journal={arXiv preprint arXiv:2210.12385},
-  year={2022}
-}
-```
+Our goal is to build up a deep learning community for single cell analysis and provide GNN based architecture for users for further development in single cell analysis.
 
 ## Usage
 
 ### Overview
 
-In release 1.0, the main usage of the DANCE is to provide readily available experiment reproduction
+In release 1.0, the main usage of the PyDANCE is to provide readily available experiment reproduction
 (see detail information about the reproduced performance [below](#implemented-algorithms)).
-Users can easily reproduce selected experiments presented in the original papers for the computational single-cell methods implemented in DANCE, which can be found under [`examples/`](examples).
+Users can easily reproduce selected experiments presented in the original papers for the computational single-cell methods implemented in PyDANCE, which can be found under [`examples/`](examples).
 
 ### Motivation
 
 Computational methods for single-cell analysis are quickly emerging, and the field is revolutionizing the usage of single-cell data to gain biological insights.
 A key challenge to continually developing computational single-cell methods that achieve new state-of-the-art performance is reproducing previous benchmarks.
 More specifically, different studies prepare their datasets and perform evaluation differently,
 and not to mention the compatibility of different methods, as they could be written in different languages or using incompatible library versions.
 
-DANCE addresses these challenges by providing a unified Python package implementing many popular computational single-cell methods (see [Implemented Algorithms](#implemented-algorithms)),
+PyDANCE addresses these challenges by providing a unified Python packge implementing many popular computational single-cell methods (see [Implemented Algorithms](#implemented-algorithms)),
 as well as easily reproducible experiments by providing unified tools for
 
 - Data downloading
 - Data (pre-)processing and transformation (e.g. graph construction)
 - Model training and evaluation
 
-### Example: run cell-type annotation benchmark using scDeepSort
+### Example: runing cell-type annotation benchmark using scDeepSort
 
-- Step0. Install DANCE (see [Installation](#installation))
+- Step0. Install PyDANCE (see [Installation](#installation))
 - Step1. Navigate to the folder containing the corresponding example scrtip.
   In this case, it is [`examples/single_modality/cell_type_annotation`](examples/single_modality/cell_type_annotation).
 - Step2. Obtain command line interface (CLI) options for a particular experiment to reproduce at the end of the
   [script](examples/single_modality/cell_type_annotation/scdeepsort.py).
   For example, the CLI options for reproducing the `Mouse Brain` experiment is
   ```bash
-  python scdeepsort.py --species mouse --tissue Brain --train_dataset 753 3285 --test_dataset 2695
+  python scdeepsort.py --data_type scdeepsort --tissue Brain --test_data 2695
   ```
-- Step3. Wait for the experiment to finish and check results.
+- Step3. Wait for the experiment to finsh and check results.
 
 ## Installation
 
 <H3>Quick install</H3>
 
 The full installation process might be a bit tedious and could involve some debugging when using CUDA enabled packages.
 Thus, we provide an `install.sh` script that simplifies the installation process, assuming the user have [conda](https://conda.io/projects/conda/en/latest/index.html) set up on their machines.
-The installation script creates a conda environment `dance` and install the DANCE package along with all its dependencies with a apseicifc CUDA version.
-Currently, two options are accepted: `cpu` and  `cu117`.
-For example, to install the DANCE package using CUDA11.7 in a `dance-env` conda environment, simply run:
+The installation script creates a conda environment `pydance` and install the PyDANCE package along with all its dependencies with a apseicifc CUDA version.
+Currently, three options are accepted: `cpu`, `cu102`, and `cu113`.
+For example, to install the DANCE package using CUDA10.2, simply run:
 
 ```bash
-# Clone the repository via SSH
-git clone git@github.com:OmicsML/dance.git && cd dance
-# Alternatively, use HTTPS if you have not set up SSH
-# git clone https://github.com/OmicsML/dance.git  && cd dance
+git clone git@github.com:OmicsML/dance.git
+cd dance
 
-# Run the auto installation script to install DANCE and its dependencies in a conda environment
-source install.sh cu117 dance-env
+source install.sh cu102
 ```
 
-**Note**: the first argument for cuda version is mandatory, while the second argument for conda environment name is optional (default is `dance`).
-
 <details>
 <summary><H3>Custom install</H3></summary>
 <br>
 
 **Step1. Setup environment**
 
-First create a conda environment for dance (optional)
+First create a conda environment for pydance (optional)
 
 ```bash
-conda create -n dance python=3.8 -y && conda activate dance-dev
+conda create -n pydance python=3.8 -y && conda activate dance-dev
 ```
 
-Then, install CUDA enabled packages (PyTorch, PyG, DGL):
+Then, install CUDA enabled packages (PyTorch, PyG, DGL) with CUDA 10.2:
 
 ```bash
-conda install pytorch=2.0.0 torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia -y
-conda install pyg=2.3.0 -c pyg -y
-conda install dgl=1.0.1 -c dglteam/label/cu117 -y
+conda install pytorch=1.12.1 torchvision cudatoolkit=10.2 -c pytorch -y
+conda install dgl-cu102 -c dglteam -y
+pip install torch-geometric==2.1.0 torch-scatter torch-sparse torch-cluster -f https://data.pyg.org/whl/torch-1.12.1+cu102.html
 ```
 
 Alternatively, install these dependencies for CPU only:
 
 ```bash
-conda install pytorch=2.0.0 torchvision torchaudio cpuonly -c pytorch -y
-conda install pyg=2.3.0 -c pyg -y
-conda install dgl -c dglteam -y
+conda install pytorch=1.12.1 torchvision cpuonly -c pytorch -y
+conda install dgl -c dglteam
+pip install torch-geometric==2.1.0 torch-scatter torch-sparse torch-cluster -f https://data.pyg.org/whl/torch-1.12.1+cpu.html
+```
+
+**Note:** If you installed PyG using conda and encountered an issue with `GLIBC_2.27` when importing `torch_geometric.nn`,
+then you may need to uninstall `torch-spline-conv` (see https://github.com/pyg-team/pytorch_geometric/issues/3593)
+
+```bash
+pip uninstall torch-spline-conv
 ```
 
-For more information about installation or other CUDA version options, check out the installation pages for the corresponding packages
+For more information about installation or other CUDA version options, check out the installation pages for the corresponding packges
 
 - [PyTorch](https://pytorch.org/get-started/)
 - [PyG](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html)
 - [DGL](https://www.dgl.ai/pages/start.html)
 
-**Step2. Install DANCE**
+**Step2. Install PyDANCE**
 
 Install from PyPI
 
 ```bash
 pip install pydance
 ```
 
-Or, install the latest dev version from source
+Install the latest dev version from source
 
 ```bash
 git clone https://github.com/OmicsML/dance.git
 cd dance
 pip install -e .
 ```
 
@@ -193,41 +147,43 @@
 | GNN                 | GNNImpute    | An efficient scRNA-seq dropout imputation method using graph attention network                               | 2021 | P1      |
 | Graph Diffusion     | MAGIC        | MAGIC: A diffusion-based imputation method reveals gene-gene interactions in single-cell RNA-sequencing data | 2018 | P1      |
 | Probabilistic Model | scImpute     | An accurate and robust imputation method scImpute for single-cell RNA-seq data                               | 2018 | P1      |
 | GAN                 | scGAIN       | scGAIN: Single Cell RNA-seq Data Imputation using Generative Adversarial Networks                            | 2019 | P1      |
 | NN                  | DeepImpute   | DeepImpute: an accurate, fast, and scalable deep neural network method to impute single-cell RNA-seq data    | 2019 | ✅       |
 | NN + TF             | Saver-X      | Transfer learning in single-cell transcriptomics improves data denoising and pattern discovery               | 2019 | P1      |
 
-| Model      | Evaluation Metric | Mouse Brain (current/reported) | Mouse Embryo (current/reported) | PBMC (current/reported) |
-| ---------- | ----------------- | ------------------------------ | ------------------------------- | ----------------------- |
-| DeepImpute | RMSE              | 0.87 / N/A                     | 1.20 / N/A                      | 2.30 / N/A              |
-| GraphSCI   | RMSE              | 1.55 / N/A                     | 1.81 / N/A                      | 3.68 / N/A              |
-| scGNN2.0   | MSE               | 1.04 / N/A                     | 1.12 / N/A                      | 1.22 / N/A              |
+| Model      | Evaluation Metric | Mouse Brain (current/reported) | Mouse Embryo (current/reported) |
+| ---------- | ----------------- | ------------------------------ | ------------------------------- |
+| DeepImpute | MSE               | 0.12 / N/A                     | 0.12 / N/A                      |
+| ScGNN      | MSE               | 0.47 / N/A                     | 1.10 / N/A                      |
+| GraphSCI   | MSE               | 0.42 / N/A                     | 0.87 / N/A                      |
 
-**Note**: scGNN2.0 is evaluated on 2,000 genes with highest variance following the original paper.
+Note: the data split modality of DeepImpute is different from ScGNN and GraphSCI, so the results are not comparable.
 
 #### 2）Cell Type Annotation
 
-| BackBone                | Model         | Algorithm                                                                                                     | Year | CheckIn |
-| ----------------------- | ------------- | ------------------------------------------------------------------------------------------------------------- | ---- | ------- |
-| GNN                     | ScDeepsort    | Single-cell transcriptomics with weighted GNN                                                                 | 2021 | ✅       |
-| Logistic Regression     | Celltypist    | Cross-tissue immune cell analysis reveals tissue-specific features in humans.                                 | 2021 | ✅       |
-| Random Forest           | singleCellNet | SingleCellNet: a computational tool to classify single cell RNA-Seq data across platforms and across species. | 2019 | ✅       |
-| Neural Network          | ACTINN        | ACTINN: automated identification of cell types in single cell RNA sequencing.                                 | 2020 | ✅       |
-| Hierarchical Clustering | SingleR       | Reference-based analysis of lung single-cell sequencing reveals a transitional profibrotic macrophage.        | 2019 | P1      |
-| SVM                     | SVM           | A comparison of automatic cell identification methods for single-cell RNA sequencing data.                    | 2018 | ✅       |
+| BackBone                | Model         | Algorithm                                                                                                    | Year | CheckIn |
+| ----------------------- | ------------- | ------------------------------------------------------------------------------------------------------------ | ---- | ------- |
+| GNN                     | ScDeepsort    | Single-cell transcriptomics with weighted GNN                                                                | 2021 | ✅       |
+| Logistic Regression     | Celltypist    | Automated cell type annotation for scRNA-seq datasets                                                        | 2021 | ✅       |
+| Random Forest           | singleCellNet | SingleCellNet: a computational tool to classify single cell RNA-Seq data across platforms and across species | 2019 | ✅       |
+| Neural Network          | ACTINN        | ACTINN: automated identification of cell types in single cell RNA sequencing.                                | 2020 | ✅       |
+| Hierarchical Clustering | SingleR       | Reference-based analysis of lung single-cell sequencing reveals a transitional profibrotic macrophage.       | 2019 | P1      |
+| SVM                     | SVM           | A comparison of automatic cell identification methods for single-cell RNA sequencing data.                   | 2018 | ✅       |
 
 | Model         | Evaluation Metric | Mouse Brain 2695 (current/reported) | Mouse Spleen 1759 (current/reported) | Mouse Kidney 203 (current/reported) |
 | ------------- | ----------------- | ----------------------------------- | ------------------------------------ | ----------------------------------- |
-| scDeepsort    | ACC               | 0.542/0.363                         | 0.969/0.965                          | 0.847/0.911                         |
-| Celltypist    | ACC               | 0.824/0.666                         | 0.908/0.848                          | 0.823/0.832                         |
+| scDeepsort    | ACC               | 0.363/0.363                         | 0.965 /0.965                         | 0.901/0.911                         |
+| Celltypist\*  | ACC               | 0.680/0.666                         | 0.966/0.848                          | 0.879/0.832                         |
 | singleCellNet | ACC               | 0.693/0.803                         | 0.975/0.975                          | 0.795/0.842                         |
-| ACTINN        | ACC               | 0.727/0.778                         | 0.657/0.236                          | 0.762/0.798                         |
+| ACTINN        | ACC               | 0.860/0.778                         | 0.516/0.236                          | 0.829/0.798                         |
 | SVM           | ACC               | 0.683/0.683                         | 0.056/0.049                          | 0.704/0.695                         |
 
+Note: * Benchmark datasets were renormalied before running the original implementation of Celltypist to match its form requirements.
+
 #### 3）Clustering
 
 | BackBone    | Model         | Algorithm                                                                                                    | Year | CheckIn |
 | ----------- | ------------- | ------------------------------------------------------------------------------------------------------------ | ---- | ------- |
 | GNN         | graph-sc      | GNN-based embedding for clustering scRNA-seq data                                                            | 2022 | ✅       |
 | GNN         | scTAG         | ZINB-based Graph Embedding Autoencoder for Single-cell RNA-seq Interpretations                               | 2022 | ✅       |
 | GNN         | scDSC         | Deep structural clustering for single-cell RNA-seq data jointly through autoencoder and graph neural network | 2022 | ✅       |
@@ -238,24 +194,25 @@
 
 | Model         | Evaluation Metric | 10x PBMC (current/reported) | Mouse ES (current/reported) | Worm Neuron (current/reported) | Mouse Bladder (current/reported) |
 | ------------- | ----------------- | --------------------------- | --------------------------- | ------------------------------ | -------------------------------- |
 | graph-sc      | ARI               | 0.72 / 0.70                 | 0.82 / 0.78                 | 0.57 / 0.46                    | 0.68 / 0.63                      |
 | scDCC         | ARI               | 0.82 / 0.81                 | 0.98 / N/A                  | 0.51 / 0.58                    | 0.60 / 0.66                      |
 | scDeepCluster | ARI               | 0.81 / 0.78                 | 0.98 / 0.97                 | 0.51 / 0.52                    | 0.56 / 0.58                      |
 | scDSC         | ARI               | 0.72 / 0.78                 | 0.84 / N/A                  | 0.46 / 0.65                    | 0.65 / 0.72                      |
-| scTAG         | ARI               | 0.77 / N/A                  | 0.96 / N/A                  | 0.49 / N/A                     | 0.69 / N/A                       |
+| scTAG         | ARI               | 0.75 / N/A                  | 0.96 / N/A                  | 0.53 / N/A                     | 0.60 / N/A                       |
 
 ### Multimodality Module
 
 #### 1）Modality Prediction
 
 | BackBone         | Model                    | Algorithm                                                                                          | Year | CheckIn |
 | ---------------- | ------------------------ | -------------------------------------------------------------------------------------------------- | ---- | ------- |
 | GNN              | ScMoGCN                  | Graph Neural Networks for Multimodal Single-Cell Data Integration                                  | 2022 | ✅       |
 | GNN              | ScMoLP                   | Link Prediction Variant of ScMoGCN                                                                 | 2022 | P1      |
+| GNN              | scGNN                    | scGNN is a novel graph neural network framework for single-cell RNA-Seq analyses                   | 2021 | P1      |
 | GNN              | GRAPE                    | Handling Missing Data with Graph Representation Learning                                           | 2020 | P1      |
 | Generative Model | SCMM                     | SCMM: MIXTURE-OF-EXPERTS MULTIMODAL DEEP GENERATIVE MODEL FOR SINGLE-CELL MULTIOMICS DATA ANALYSIS | 2021 | ✅       |
 | Auto-encoder     | Cross-modal autoencoders | Multi-domain translation between single-cell imaging and sequencing data using autoencoders        | 2021 | ✅       |
 | Auto-encoder     | BABEL                    | BABEL enables cross-modality translation between multiomic profiles at single-cell resolution      | 2021 | ✅       |
 
 | Model                    | Evaluation Metric | GEX2ADT (current/reported) | ADT2GEX (current/reported) | GEX2ATAC (current/reported) | ATAC2GEX (current/reported) |
 | ------------------------ | ----------------- | -------------------------- | -------------------------- | --------------------------- | --------------------------- |
@@ -265,15 +222,15 @@
 | BABEL                    | RMSE              | 0.4335 / N/A               | 0.3673 / N/A               | 0.1816 / N/A                | 0.2394 / N/A                |
 
 #### 2) Modality Matching
 
 | BackBone         | Model                    | Algorithm                                                                                          | Year | CheckIn |
 | ---------------- | ------------------------ | -------------------------------------------------------------------------------------------------- | ---- | ------- |
 | GNN              | ScMoGCN                  | Graph Neural Networks for Multimodal Single-Cell Data Integration                                  | 2022 | ✅       |
-| GNN/Auto-ecnoder | GLUE                     | Multi-omics single-cell data integration and regulatory inference with graph-linked embedding      | 2021 | P1      |
+| GNN              | scGNN                    | scGNN is a novel graph neural network framework for single-cell RNA-Seq analyses                   | 2021 | P1      |
 | Generative Model | SCMM                     | SCMM: MIXTURE-OF-EXPERTS MULTIMODAL DEEP GENERATIVE MODEL FOR SINGLE-CELL MULTIOMICS DATA ANALYSIS | 2021 | ✅       |
 | Auto-encoder     | Cross-modal autoencoders | Multi-domain translation between single-cell imaging and sequencing data using autoencoders        | 2021 | ✅       |
 
 | Model                    | Evaluation Metric | GEX2ADT (current/reported) | GEX2ATAC (current/reported) |
 | ------------------------ | ----------------- | -------------------------- | --------------------------- |
 | ScMoGCN                  | Accuracy          | 0.0827 / 0.0810            | 0.0600 / 0.0630             |
 | SCMM                     | Accuracy          | 0.005 / N/A                | 5e-5 / N/A                  |
@@ -343,11 +300,47 @@
 | GNN                        | DSTG         | DSTG: deconvoluting spatial transcriptomics data through graph-based artificial intelligence                  | 2021 | ✅       |
 | logNormReg                 | SpatialDecon | Advances in mixed cell deconvolution enable quantification of cell types in spatial transcriptomic data       | 2022 | ✅       |
 | NNMFreg                    | SPOTlight    | SPOTlight: seeded NMF regression to deconvolute spatial transcriptomics spots with single-cell transcriptomes | 2021 | ✅       |
 | NN Linear + CAR assumption | CARD         | Spatially informed cell-type deconvolution for spatial transcriptomics                                        | 2022 | ✅       |
 
 | Model        | Evaluation Metric | GSE174746 (current/reported) | CARD Synthetic (current/reported) | SPOTlight Synthetic (current/reported) |
 | ------------ | ----------------- | ---------------------------- | --------------------------------- | -------------------------------------- |
-| DSTG         | MSE               | .1722 / N/A                  | .0239 / N/A                       | .0315 / N/A                            |
+| DSTG         | MSE               | .172 / N/A                   | .0247 / N/A                       | .042 / N/A                             |
 | SpatialDecon | MSE               | .0014 / .009                 | .0077 / N/A                       | .0055 / N/A                            |
 | SPOTlight    | MSE               | .0098 / N/A                  | .0246 / 0.118                     | .0109 / .16                            |
 | CARD         | MSE               | .0012 / N/A                  | .0078 / 0.0062                    | .0076 / N/A                            |
+
+## Dev notes
+
+### Dev installation
+
+Install PyDANCE with extra dependencies for dev
+
+```bash
+pip install -e ."[dev]"
+```
+
+Make sure dependencies have specific pinned versions
+
+```bash
+pip install -r requirements.txt
+```
+
+Install pre-commit hooks for code quality checks
+
+```bash
+pre-commit install
+```
+
+### Run tests
+
+Run all tests on current environment using pytest
+
+```bash
+pytest -v
+```
+
+Run full test from the ground up including environment set up using [tox](https://tox.wiki/en/latest/) on CPU
+
+```bash
+tox -e python3.8-cpu
+```
```

### Comparing `pydance-1.0.0/dance/datasets/multimodality.py` & `pydance-1.0.0rc0/dance/datasets/multimodality.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,464 +1,497 @@
 import os
-import os.path as osp
 import pickle
-from abc import ABC
 
 import anndata as ad
-import mudata as md
 import numpy as np
 import scanpy as sc
+import torch
 
-from dance import logger
-from dance.data import Data
-from dance.datasets.base import BaseDataset
+from dance.data import *
 from dance.transforms.preprocess import lsiTransformer
-from dance.typing import List
-from dance.utils.download import download_file, unzip_file
 
 
-class MultiModalityDataset(BaseDataset, ABC):
+class MultiModalityDataset():
 
-    TASK = "N/A"
-    URL_DICT = {}
-    SUBTASK_NAME_MAP = {}
-    AVAILABLE_DATA = []
+    def __init__(self, task, data_url, subtask, data_dir="./data"):
 
-    def __init__(self, subtask, root="./data"):
-        assert subtask in self.AVAILABLE_DATA, f"Undefined subtask {subtask!r}."
-        assert self.TASK in ["predict_modality", "match_modality", "joint_embedding"]
-
-        self.subtask = self.SUBTASK_NAME_MAP.get(subtask, subtask)
-        self.data_url = self.URL_DICT[self.subtask]
-
-        super().__init__(root=root, full_download=False)
-
-    def download(self):
-        self.download_data()
+        assert (subtask in [
+            'openproblems_bmmc_multiome_phase2_mod2', 'openproblems_bmmc_multiome_phase2_rna',
+            'openproblems_bmmc_cite_phase2_rna', 'openproblems_bmmc_cite_phase2_mod2', 'openproblems_bmmc_cite_phase2',
+            'openproblems_bmmc_multiome_phase2', 'adt2gex', 'gex2adt', 'atac2gex', 'gex2atac'
+        ]), 'Undefined subtask.'
+
+        assert (task in ['predict_modality', 'match_modality', 'joint_embedding']), 'Undefined task.'
+
+        # regularize subtask name
+        if task == 'joint_embedding':
+            if subtask == 'adt':
+                subtask = 'openproblems_bmmc_cite_phase2'
+            elif subtask == 'atac':
+                subtask = 'openproblems_bmmc_multiome_phase2'
+        else:
+            if subtask == 'adt2gex':
+                subtask = 'openproblems_bmmc_cite_phase2_mod2'
+            elif subtask == 'gex2adt':
+                subtask = 'openproblems_bmmc_cite_phase2_rna'
+            elif subtask == 'atac2gex':
+                subtask = 'openproblems_bmmc_multiome_phase2_mod2'
+            elif subtask == 'gex2atac':
+                subtask = 'openproblems_bmmc_multiome_phase2_rna'
+
+        self.task = task
+        self.subtask = subtask
+        self.data_dir = data_dir
+        self.loaded = False
+        self.data_url = data_url
 
     def download_data(self):
-        download_file(self.data_url, osp.join(self.root, f"{self.subtask}.zip"))
-        unzip_file(osp.join(self.root, f"{self.subtask}.zip"), self.root)
+        # download data
+        download_file(self.data_url, self.data_dir + "/{}.zip".format(self.subtask))
+        unzip_file(self.data_dir + "/{}.zip".format(self.subtask), self.data_dir)
+        return self
 
     def download_pathway(self):
-        download_file("https://www.dropbox.com/s/uqoakpalr3albiq/h.all.v7.4.entrez.gmt?dl=1",
-                      osp.join(self.root, "h.all.v7.4.entrez.gmt"))
-        download_file("https://www.dropbox.com/s/yjrcsd2rpmahmfo/h.all.v7.4.symbols.gmt?dl=1",
-                      osp.join(self.root, "h.all.v7.4.symbols.gmt"))
-
-    @property
-    def data_paths(self) -> List[str]:
-        if self.TASK == "joint_embedding":
-            mod = "adt" if "cite" in self.subtask else "atac"
-            meta = "cite" if "cite" in self.subtask else "multiome"
-            paths = [
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_mod1.h5ad"),
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_mod2.h5ad"),
-                osp.join(self.root, self.subtask, f"{meta}_gex_processed_training.h5ad"),
-                osp.join(self.root, self.subtask, f"{meta}_{mod}_processed_training.h5ad"),
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_solution.h5ad"),
-            ]
-        elif self.TASK == "predict_modality":
-            paths = [
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_train_mod1.h5ad"),
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_train_mod2.h5ad"),
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_test_mod1.h5ad"),
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_test_mod2.h5ad"),
+        download_file('https://www.dropbox.com/s/uqoakpalr3albiq/h.all.v7.4.entrez.gmt?dl=1',
+                      self.data_dir + "/h.all.v7.4.entrez.gmt")
+        download_file('https://www.dropbox.com/s/yjrcsd2rpmahmfo/h.all.v7.4.symbols.gmt?dl=1',
+                      self.data_dir + "/h.all.v7.4.symbols.gmt")
+        return self
+
+    def is_complete(self):
+        # judge data is complete or not
+        if self.task == 'joint_embedding':
+            return os.path.exists(
+                os.path.join(
+                    self.data_dir, self.subtask, f'{self.subtask}.censor_dataset.output_mod1.h5ad')) and os.path.exists(
+                        os.path.join(self.data_dir, self.subtask, f'{self.subtask}.censor_dataset.output_mod2.h5ad'))
+        else:
+            return os.path.exists(
+                os.path.join(
+                    self.data_dir, self.subtask,
+                    f'{self.subtask}.censor_dataset.output_train_mod1.h5ad')) and os.path.exists(
+                        os.path.join(
+                            self.data_dir, self.subtask,
+                            f'{self.subtask}.censor_dataset.output_train_mod2.h5ad')) and os.path.exists(
+                                os.path.join(
+                                    self.data_dir, self.subtask,
+                                    f'{self.subtask}.censor_dataset.output_test_mod1.h5ad')) and os.path.exists(
+                                        os.path.join(self.data_dir, self.subtask,
+                                                     f'{self.subtask}.censor_dataset.output_test_mod2.h5ad'))
+
+    def load_data(self):
+        # Load data from existing h5ad files, or download files and load data.
+        if self.is_complete():
+            pass
+        else:
+            self.download_data()
+            assert self.is_complete()
+
+        if self.task == 'joint_embedding':
+            mod_path_list = [
+                os.path.join(self.data_dir, self.subtask, f'{self.subtask}.censor_dataset.output_mod1.h5ad'),
+                os.path.join(self.data_dir, self.subtask, f'{self.subtask}.censor_dataset.output_mod2.h5ad')
             ]
-        elif self.TASK == "match_modality":
-            paths = [
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_train_mod1.h5ad"),
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_train_mod2.h5ad"),
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_train_sol.h5ad"),
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_test_mod1.h5ad"),
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_test_mod2.h5ad"),
-                osp.join(self.root, self.subtask, f"{self.subtask}.censor_dataset.output_test_sol.h5ad"),
+        else:
+            mod_path_list = [
+                os.path.join(self.data_dir, self.subtask, f'{self.subtask}.censor_dataset.output_train_mod1.h5ad'),
+                os.path.join(self.data_dir, self.subtask, f'{self.subtask}.censor_dataset.output_train_mod2.h5ad'),
+                os.path.join(self.data_dir, self.subtask, f'{self.subtask}.censor_dataset.output_test_mod1.h5ad'),
+                os.path.join(self.data_dir, self.subtask, f'{self.subtask}.censor_dataset.output_test_mod2.h5ad')
             ]
-        return paths
 
-    def is_complete(self) -> bool:
-        return all(map(osp.exists, self.data_paths))
+        self.modalities = []
+        for mod_path in mod_path_list:
+            self.modalities.append(ad.read_h5ad(mod_path))
+        self.loaded = True
+        return self
+
+    def sparse_features(self, index=None, count=False):
+        assert self.loaded, 'Data have not been loaded.'
+        if not count:
+            if index is None:
+                return [mod.X for mod in self.modalities]
+            else:
+                return self.modalities[index].X
+        else:
+            if index is None:
+                return [mod.layers['counts'] for mod in self.modalities]
+            else:
+                return self.modalities[index].layers['counts']
+
+    def numpy_features(self, index=None, count=False):
+        assert self.loaded, 'Data have not been loaded.'
+        if not count:
+            if index is None:
+                return [mod.X.toarray() for mod in self.modalities]
+            else:
+                return self.modalities[index].X.toarray()
+        else:
+            if index is None:
+                return [mod.layers['counts'].toarray() for mod in self.modalities]
+            else:
+                return self.modalities[index].layers['counts'].toarray()
+
+    def tensor_features(self, index=None, count=False, device='cpu'):
+        assert self.loaded, 'Data have not been loaded.'
+        if not count:
+            if index is None:
+                return [torch.from_numpy(mod.X.toarray()).to(device) for mod in self.modalities]
+            else:
+                return torch.from_numpy(self.modalities[index].X.toarray()).to(device)
+        else:
+            if index is None:
+                return [torch.from_numpy(mod.layers['counts'].toarray()).to(device) for mod in self.modalities]
+            else:
+                return torch.from_numpy(self.modalities[index].layers['counts'].toarray()).to(device)
 
-    def _load_raw_data(self) -> List[ad.AnnData]:
-        modalities = []
-        for mod_path in self.data_paths:
-            logger.info(f"Loading {mod_path}")
-            modalities.append(ad.read_h5ad(mod_path))
-        return modalities
+    def get_modalities(self):
+        assert self.loaded, 'Data have not been loaded.'
+        return self.modalities
 
 
 class ModalityPredictionDataset(MultiModalityDataset):
 
-    TASK = "predict_modality"
-    URL_DICT = {
-        "openproblems_bmmc_cite_phase2_mod2":
-        "https://www.dropbox.com/s/snh8knscnlcq4um/openproblems_bmmc_cite_phase2_mod2.zip?dl=1",
-        "openproblems_bmmc_cite_phase2_rna":
-        "https://www.dropbox.com/s/xbfyhv830u9pupv/openproblems_bmmc_cite_phase2_rna.zip?dl=1",
-        "openproblems_bmmc_multiome_phase2_mod2":
-        "https://www.dropbox.com/s/p9ve2ljyy4yqna4/openproblems_bmmc_multiome_phase2_mod2.zip?dl=1",
-        "openproblems_bmmc_multiome_phase2_rna":
-        "https://www.dropbox.com/s/cz60vp7bwapz0kw/openproblems_bmmc_multiome_phase2_rna.zip?dl=1",
-        "openproblems_bmmc_cite_phase2_rna_subset":
-        "https://www.dropbox.com/s/veytldxkgzyoa8j/openproblems_bmmc_cite_phase2_rna_subset.zip?dl=1",
-    }
-    SUBTASK_NAME_MAP = {
-        "adt2gex": "openproblems_bmmc_cite_phase2_mod2",
-        "atac2gex": "openproblems_bmmc_multiome_phase2_mod2",
-        "gex2adt": "openproblems_bmmc_cite_phase2_rna",
-        "gex2atac": "openproblems_bmmc_multiome_phase2_rna",
-        "gex2adt_subset": "openproblems_bmmc_cite_phase2_rna_subset",
-    }
-    AVAILABLE_DATA = sorted(list(URL_DICT) + list(SUBTASK_NAME_MAP))
-
-    def __init__(self, subtask, root="./data", preprocess=None):
-        # TODO: factor our preprocess
-        self.preprocess = preprocess
-        super().__init__(subtask, root)
-
-    def _raw_to_dance(self, raw_data):
-        train_mod1, train_mod2, test_mod1, test_mod2 = self._maybe_preprocess(raw_data)
-
-        mod1 = ad.concat((train_mod1, test_mod1))
-        mod2 = ad.concat((train_mod2, test_mod2))
-        mod1.var_names_make_unique()
-        mod2.var_names_make_unique()
-
-        mdata = md.MuData({"mod1": mod1, "mod2": mod2})
-        mdata.var_names_make_unique()
-
-        data = Data(mdata, train_size=train_mod1.shape[0])
-        data.set_config(feature_mod="mod1", label_mod="mod2")
-
-        return data
-
-    def _maybe_preprocess(self, raw_data, selection_threshold=10000):
-        if self.preprocess == "feature_selection":
-            if raw_data[0].shape[1] > selection_threshold:
-                sc.pp.highly_variable_genes(raw_data[0], layer="counts", flavor="seurat_v3",
+    def __init__(self, subtask, data_dir="./data"):
+        assert (subtask in [
+            'openproblems_bmmc_multiome_phase2_mod2', 'openproblems_bmmc_multiome_phase2_rna',
+            'openproblems_bmmc_cite_phase2_rna', 'openproblems_bmmc_cite_phase2_mod2', 'adt2gex', 'gex2adt', 'atac2gex',
+            'gex2atac'
+        ]), 'Undefined subtask.'
+
+        if subtask == 'adt2gex':
+            subtask = 'openproblems_bmmc_cite_phase2_mod2'
+        elif subtask == 'gex2adt':
+            subtask = 'openproblems_bmmc_cite_phase2_rna'
+        elif subtask == 'atac2gex':
+            subtask = 'openproblems_bmmc_multiome_phase2_mod2'
+        elif subtask == 'gex2atac':
+            subtask = 'openproblems_bmmc_multiome_phase2_rna'
+
+        data_url = {
+            'openproblems_bmmc_cite_phase2_mod2':
+            'https://www.dropbox.com/s/snh8knscnlcq4um/openproblems_bmmc_cite_phase2_mod2.zip?dl=1',
+            'openproblems_bmmc_cite_phase2_rna':
+            'https://www.dropbox.com/s/xbfyhv830u9pupv/openproblems_bmmc_cite_phase2_rna.zip?dl=1',
+            'openproblems_bmmc_multiome_phase2_mod2':
+            'https://www.dropbox.com/s/p9ve2ljyy4yqna4/openproblems_bmmc_multiome_phase2_mod2.zip?dl=1',
+            'openproblems_bmmc_multiome_phase2_rna':
+            'https://www.dropbox.com/s/cz60vp7bwapz0kw/openproblems_bmmc_multiome_phase2_rna.zip?dl=1'
+        }
+
+        super().__init__('predict_modality', data_url.get(subtask), subtask, data_dir)
+
+    def preprocess(self, kind='feature_selection', selection_threshold=10000):
+        if kind == 'pca':
+            print('Preprocessing method not supported.')
+            return self
+        elif kind == 'feature_selection':
+            if self.modalities[0].shape[1] > selection_threshold:
+                sc.pp.highly_variable_genes(self.modalities[0], layer='counts', flavor='seurat_v3',
                                             n_top_genes=selection_threshold)
-                raw_data[2].var["highly_variable"] = raw_data[0].var["highly_variable"]
+                self.modalities[2].var['highly_variable'] = self.modalities[0].var['highly_variable']
                 for i in [0, 2]:
-                    raw_data[i] = raw_data[i][:, raw_data[i].var["highly_variable"]]
-        elif self.preprocess not in (None, "none"):
-            logger.info(f"Preprocessing method {self.preprocess!r} not supported.")
-        logger.info("Preprocessing done.")
-        return raw_data
+                    self.modalities[i] = self.modalities[i][:, self.modalities[i].var['highly_variable']]
+        else:
+            print('Preprocessing method not supported.')
+            return self
+        print('Preprocessing done.')
+        return self
 
 
 class ModalityMatchingDataset(MultiModalityDataset):
 
-    TASK = "match_modality"
-    URL_DICT = {
-        "openproblems_bmmc_cite_phase2_mod2":
-        "https://www.dropbox.com/s/fa6zut89xx73itz/openproblems_bmmc_cite_phase2_mod2.zip?dl=1",
-        "openproblems_bmmc_cite_phase2_rna":
-        "https://www.dropbox.com/s/ep00mqcjmdu0b7v/openproblems_bmmc_cite_phase2_rna.zip?dl=1",
-        "openproblems_bmmc_multiome_phase2_mod2":
-        "https://www.dropbox.com/s/31qi5sckx768acw/openproblems_bmmc_multiome_phase2_mod2.zip?dl=1",
-        "openproblems_bmmc_multiome_phase2_rna":
-        "https://www.dropbox.com/s/h1s067wkefs1jh2/openproblems_bmmc_multiome_phase2_rna.zip?dl=1",
-        "openproblems_bmmc_cite_phase2_rna_subset":
-        "https://www.dropbox.com/s/3q4xwpzjbe81x58/openproblems_bmmc_cite_phase2_rna_subset.zip?dl=1",
-    }
-    SUBTASK_NAME_MAP = {
-        "adt2gex": "openproblems_bmmc_cite_phase2_mod2",
-        "atac2gex": "openproblems_bmmc_multiome_phase2_mod2",
-        "gex2adt": "openproblems_bmmc_cite_phase2_rna",
-        "gex2atac": "openproblems_bmmc_multiome_phase2_rna",
-        "gex2adt_subset": "openproblems_bmmc_cite_phase2_rna_subset",
-    }
-    AVAILABLE_DATA = sorted(list(URL_DICT) + list(SUBTASK_NAME_MAP))
-
-    def __init__(self, subtask, root="./data", preprocess=None, pkl_path=None):
-        # TODO: factor our preprocess
-        self.preprocess = preprocess
-        self.pkl_path = pkl_path
-        super().__init__(subtask, root)
-
-    def _raw_to_dance(self, raw_data):
-        train_mod1, train_mod2, train_label, test_mod1, test_mod2, test_label = self._maybe_preprocess(raw_data)
-
-        mod1 = ad.concat((train_mod1, test_mod1))
-        mod2 = ad.concat((train_mod2, test_mod2))
-        mod1.var_names_make_unique()
-        mod2.var_names_make_unique()
-        mod2.obs_names = mod1.obs_names
-        train_size = train_mod1.shape[0]
-
-        # Align matched cells
-        train_mod2 = train_mod2[train_label.to_df().values.argmax(1)]
-        mod1.obsm["labels"] = np.concatenate([np.zeros(train_size), np.argmax(test_label.X.toarray(), 1)])
-
-        # Combine modalities into mudata
-        mdata = md.MuData({"mod1": mod1, "mod2": mod2})
-        mdata.var_names_make_unique()
-
-        data = Data(mdata, train_size=train_size)
-
-        return data
-
-    def _maybe_preprocess(self, raw_data, selection_threshold=10000):
-        if self.preprocess is None:
-            return raw_data
+    def __init__(self, subtask, data_dir="./data"):
+        assert (subtask in [
+            'openproblems_bmmc_multiome_phase2_mod2', 'openproblems_bmmc_multiome_phase2_rna',
+            'openproblems_bmmc_cite_phase2_rna', 'openproblems_bmmc_cite_phase2_mod2', 'adt2gex', 'gex2adt', 'atac2gex',
+            'gex2atac'
+        ]), 'Undefined subtask.'
+
+        if subtask == 'adt2gex':
+            subtask = 'openproblems_bmmc_cite_phase2_mod2'
+        elif subtask == 'gex2adt':
+            subtask = 'openproblems_bmmc_cite_phase2_rna'
+        elif subtask == 'atac2gex':
+            subtask = 'openproblems_bmmc_multiome_phase2_mod2'
+        elif subtask == 'gex2atac':
+            subtask = 'openproblems_bmmc_multiome_phase2_rna'
+
+        data_url = {
+            'openproblems_bmmc_cite_phase2_mod2':
+            'https://www.dropbox.com/s/fa6zut89xx73itz/openproblems_bmmc_cite_phase2_mod2.zip?dl=1',
+            'openproblems_bmmc_cite_phase2_rna':
+            'https://www.dropbox.com/s/ep00mqcjmdu0b7v/openproblems_bmmc_cite_phase2_rna.zip?dl=1',
+            'openproblems_bmmc_multiome_phase2_mod2':
+            'https://www.dropbox.com/s/31qi5sckx768acw/openproblems_bmmc_multiome_phase2_mod2.zip?dl=1',
+            'openproblems_bmmc_multiome_phase2_rna':
+            'https://www.dropbox.com/s/h1s067wkefs1jh2/openproblems_bmmc_multiome_phase2_rna.zip?dl=1'
+        }
+
+        super().__init__('match_modality', data_url.get(subtask), subtask, data_dir)
+        self.preprocessed = False
+
+    def load_sol(self):
+        assert (self.loaded)
+        self.train_sol = ad.read_h5ad(
+            os.path.join(self.data_dir, self.subtask, f'{self.subtask}.censor_dataset.output_train_sol.h5ad'))
+        self.test_sol = ad.read_h5ad(
+            os.path.join(self.data_dir, self.subtask, f'{self.subtask}.censor_dataset.output_test_sol.h5ad'))
+        self.modalities[1] = self.modalities[1][self.train_sol.to_df().values.argmax(1)]
+        return self
 
-        train_mod1, train_mod2, train_label, test_mod1, test_mod2, test_label = raw_data
-        modalities = [train_mod1, train_mod2, test_mod1, test_mod2]
+    def preprocess(self, kind='pca', pkl_path=None, selection_threshold=10000):
 
         # TODO: support other two subtasks
-        assert self.subtask in ("openproblems_bmmc_cite_phase2_rna", "openproblems_bmmc_cite_phase2_rna_subset",
-                                "openproblems_bmmc_multiome_phase2_rna"), "Currently not available."
+        assert self.subtask in ('openproblems_bmmc_cite_phase2_rna',
+                                'openproblems_bmmc_multiome_phase2_rna'), 'Currently not available.'
 
-        if self.preprocess == "pca":
-            if self.pkl_path and osp.exists(self.pkl_path):
-                with open(self.pkl_path, "rb") as f:
-                    preprocessed_features = pickle.load(f)
+        if kind == 'pca':
+            if pkl_path and (not os.path.exists(pkl_path)):
 
-            else:
-                if self.subtask in ("openproblems_bmmc_cite_phase2_rna", "openproblems_bmmc_cite_phase2_rna_subset"):
+                if self.subtask == 'openproblems_bmmc_cite_phase2_rna':
                     lsi_transformer_gex = lsiTransformer(n_components=256, drop_first=True)
-                    m1_train = lsi_transformer_gex.fit_transform(modalities[0]).values
-                    m1_test = lsi_transformer_gex.transform(modalities[2]).values
-                    m2_train = modalities[1].X.toarray()
-                    m2_test = modalities[3].X.toarray()
+                    m1_train = lsi_transformer_gex.fit_transform(self.modalities[0]).values
+                    m1_test = lsi_transformer_gex.transform(self.modalities[2]).values
+                    m2_train = self.modalities[1].X.toarray()
+                    m2_test = self.modalities[3].X.toarray()
 
-                elif self.subtask == "openproblems_bmmc_multiome_phase2_rna":
+                if self.subtask == 'openproblems_bmmc_multiome_phase2_rna':
                     lsi_transformer_gex = lsiTransformer(n_components=256, drop_first=True)
-                    m1_train = lsi_transformer_gex.fit_transform(modalities[0]).values
-                    m1_test = lsi_transformer_gex.transform(modalities[2]).values
+                    m1_train = lsi_transformer_gex.fit_transform(self.modalities[0]).values
+                    m1_test = lsi_transformer_gex.transform(self.modalities[2]).values
                     lsi_transformer_atac = lsiTransformer(n_components=512, drop_first=True)
-                    m2_train = lsi_transformer_atac.fit_transform(modalities[1]).values
-                    m2_test = lsi_transformer_atac.transform(modalities[3]).values
-
-                else:
-                    raise ValueError(f"Unrecognized subtask name: {self.subtask}")
+                    m2_train = lsi_transformer_atac.fit_transform(self.modalities[1]).values
+                    m2_test = lsi_transformer_atac.transform(self.modalities[3]).values
 
-                preprocessed_features = {
-                    "mod1_train": m1_train,
-                    "mod2_train": m2_train,
-                    "mod1_test": m1_test,
-                    "mod2_test": m2_test
+                self.preprocessed_features = {
+                    'mod1_train': m1_train,
+                    'mod2_train': m2_train,
+                    'mod1_test': m1_test,
+                    'mod2_test': m2_test
                 }
+                pickle.dump(self.preprocessed_features, open(pkl_path, 'wb'))
 
-                if self.pkl_path:
-                    with open(self.pkl_path, "wb") as f:
-                        pickle.dump(preprocessed_features, f)
-
-            modalities[0].obsm["X_pca"] = preprocessed_features["mod1_train"]
-            modalities[1].obsm["X_pca"] = preprocessed_features["mod2_train"]
-            modalities[2].obsm["X_pca"] = preprocessed_features["mod1_test"]
-            modalities[3].obsm["X_pca"] = preprocessed_features["mod2_test"]
-
-        elif self.preprocess == "feature_selection":
+            else:
+                self.preprocessed_features = pickle.load(open(pkl_path, 'rb'))
+        elif kind == 'feature_selection':
             for i in range(2):
-                if modalities[i].shape[1] > selection_threshold:
-                    sc.pp.highly_variable_genes(modalities[i], layer="counts", flavor="seurat_v3",
+                if self.modalities[i].shape[1] > selection_threshold:
+                    sc.pp.highly_variable_genes(self.modalities[i], layer='counts', flavor='seurat_v3',
                                                 n_top_genes=selection_threshold)
-                    modalities[i + 2].var["highly_variable"] = modalities[i].var["highly_variable"]
-                    modalities[i] = modalities[i][:, modalities[i].var["highly_variable"]]
-                    modalities[i + 2] = modalities[i + 2][:, modalities[i + 2].var["highly_variable"]]
-
+                    self.modalities[i + 2].var['highly_variable'] = self.modalities[i].var['highly_variable']
+                    self.modalities[i] = self.modalities[i][:, self.modalities[i].var['highly_variable']]
+                    self.modalities[i + 2] = self.modalities[i + 2][:, self.modalities[i + 2].var['highly_variable']]
         else:
-            logger.info("Preprocessing method not supported.")
-
-        logger.info("Preprocessing done.")
-
-        train_mod1, train_mod2, test_mod1, test_mod2 = modalities
-        return train_mod1, train_mod2, train_label, test_mod1, test_mod2, test_label
+            print('Preprocessing method not supported.')
+            return self
+        print('Preprocessing done.')
+        self.preprocessed = True
+        return self
+
+    def get_preprocessed_features(self):
+        assert self.preprocessed, 'Transformed features do not exist.'
+        return self.preprocessed_features
 
 
 class JointEmbeddingNIPSDataset(MultiModalityDataset):
 
-    TASK = "joint_embedding"
-    URL_DICT = {
-        "openproblems_bmmc_cite_phase2":
-        "https://www.dropbox.com/s/hjr4dxuw55vin5z/openproblems_bmmc_cite_phase2.zip?dl=1",
-        "openproblems_bmmc_multiome_phase2":
-        "https://www.dropbox.com/s/40kjslupxhkg92s/openproblems_bmmc_multiome_phase2.zip?dl=1"
-    }
-    SUBTASK_NAME_MAP = {
-        "adt": "openproblems_bmmc_cite_phase2",
-        "atac": "openproblems_bmmc_multiome_phase2",
-    }
-    AVAILABLE_DATA = sorted(list(URL_DICT) + list(SUBTASK_NAME_MAP))
-
-    def __init__(self, subtask, root="./data", preprocess=None, normalize=False, pretrained_folder="."):
-        # TODO: factor our preprocess
-        self.preprocess = preprocess
-        self.normalize = normalize
-        self.pretrained_folder = pretrained_folder
-        super().__init__(subtask, root)
-
-    def _raw_to_dance(self, raw_data):
-        mod1, mod2, meta1, meta2, test_sol = self._maybe_preprocess(raw_data)
-
-        assert all(mod2.obs_names == mod1.obs_names), "Modalities not aligned"
-        mdata = md.MuData({"mod1": mod1, "mod2": mod2, "meta1": meta1, "meta2": meta2, "test_sol": test_sol})
-
-        train_size = meta1.shape[0]
-        data = Data(mdata, train_size=train_size)
-
-        return data
-
-    def _maybe_preprocess(self, raw_data, selection_threshold=10000):
-        if self.preprocess is None:
-            return raw_data
-
-        mod1, mod2, meta1, meta2, test_sol = raw_data
-        train_size = meta1.shape[0]
-
-        # aux -> cell cycle analysis
-        if self.preprocess == "aux":
-            os.makedirs(self.pretrained_folder, exist_ok=True)
-
-            if osp.exists(osp.join(self.pretrained_folder, f"preprocessed_data_{self.subtask}.pkl")):
-
-                with open(osp.join(self.pretrained_folder, f"preprocessed_data_{self.subtask}.pkl"), "rb") as f:
-                    preprocessed_data = pickle.load(f)
-
-                    y_train = preprocessed_data["y_train"]
-                    mod1.obsm["X_pca"] = preprocessed_data["X_pca_0"]
-                    mod2.obsm["X_pca"] = preprocessed_data["X_pca_1"]
-
-                    mod1.obsm["cell_type"] = y_train[0]
-                    mod1.obsm["batch_label"] = np.concatenate(
-                        [y_train[1], np.zeros(y_train[0].shape[0] - train_size)], 0)
-                    mod1.obsm["phase_labels"] = np.concatenate(
-                        [y_train[2], np.zeros(y_train[0].shape[0] - train_size)], 0)
-                    mod1.obsm["S_scores"] = np.concatenate([y_train[3], np.zeros(y_train[0].shape[0] - train_size)], 0)
-                    mod1.obsm["G2M_scores"] = np.concatenate(
-                        [y_train[4], np.zeros(y_train[0].shape[0] - train_size)], 0)
-
-                with open(osp.join(self.pretrained_folder, f"{self.subtask}_config.pk"), "rb") as f:
-                    # cell types, batch labels, cell cycle
+    def __init__(self, subtask, data_dir="./data"):
+        assert (subtask in ['openproblems_bmmc_multiome_phase2', 'openproblems_bmmc_cite_phase2', 'adt',
+                            'atac']), 'Undefined subtask.'
+
+        if subtask == 'adt':
+            subtask = 'openproblems_bmmc_cite_phase2'
+        elif subtask == 'atac':
+            subtask = 'openproblems_bmmc_multiome_phase2'
+
+        data_url = {
+            'openproblems_bmmc_cite_phase2':
+            'https://www.dropbox.com/s/hjr4dxuw55vin5z/openproblems_bmmc_cite_phase2.zip?dl=1',
+            'openproblems_bmmc_multiome_phase2':
+            'https://www.dropbox.com/s/40kjslupxhkg92s/openproblems_bmmc_multiome_phase2.zip?dl=1'
+        }
+        super().__init__('joint_embedding', data_url.get(subtask), subtask, data_dir)
+        self.preprocessed = False
+
+    def load_metadata(self):
+        assert (self.loaded)
+
+        if self.subtask.find('cite') != -1:
+            mod = 'adt'
+            meta = 'cite'
+        else:
+            mod = 'atac'
+            meta = 'multiome'
+        self.exploration = [
+            ad.read_h5ad(os.path.join(self.data_dir, self.subtask, f'{meta}_gex_processed_training.h5ad')),
+            ad.read_h5ad(os.path.join(self.data_dir, self.subtask, f'{meta}_{mod}_processed_training.h5ad')),
+        ]
+        return self
+
+    def load_sol(self):
+        assert (self.loaded)
+        self.test_sol = ad.read_h5ad(
+            os.path.join(self.data_dir, self.subtask, f'{self.subtask}.censor_dataset.output_solution.h5ad'))
+        return self
+
+    def preprocess(self, kind='aux', pretrained_folder='.', selection_threshold=10000):
+        if kind == 'aux':
+            os.makedirs(pretrained_folder, exist_ok=True)
+
+            if os.path.exists(os.path.join(pretrained_folder, f'preprocessed_data_{self.subtask}.pkl')):
+
+                with open(os.path.join(pretrained_folder, f'preprocessed_data_{self.subtask}.pkl'), 'rb') as f:
+                    self.preprocessed_data = pickle.load(f)
+                with open(os.path.join(pretrained_folder, f'{self.subtask}_config.pk'), 'rb') as f:
                     self.nb_cell_types, self.nb_batches, self.nb_phases = pickle.load(f)
-                logger.info("Preprocessing done.")
-                return mod1, mod2, meta1, meta2, test_sol
-
-            # PCA
-            mod1_name = mod1.var["feature_types"][0]
-            mod2_name = mod2.var["feature_types"][0]
-            if mod2_name == "ADT":
-                if osp.exists(osp.join(self.pretrained_folder, f"lsi_cite_{mod1_name}.pkl")):
-                    with open(osp.join(self.pretrained_folder, f"lsi_cite_{mod1_name}.pkl"), "rb") as f:
-                        lsi_transformer_gex = pickle.load(f)
+                self.preprocessed = True
+                print('Preprocessing done.')
+                return self
+
+            ##########################################
+            ##             PCA PRETRAIN             ##
+            ##########################################
+
+            # scale and log transform
+            scale = 1e4
+            n_components_mod1, n_components_mod2 = 256, 100
+
+            mod1 = self.modalities[0].var["feature_types"][0]
+            mod2 = self.modalities[1].var["feature_types"][0]
+
+            if mod2 == "ADT":
+                if os.path.exists(os.path.join(pretrained_folder, f"lsi_cite_{mod1}.pkl")):
+                    lsi_transformer_gex = pickle.load(
+                        open(os.path.join(pretrained_folder, f"lsi_cite_{mod1}.pkl"), "rb"))
                 else:
                     lsi_transformer_gex = lsiTransformer(n_components=256, drop_first=True)
-                    lsi_transformer_gex.fit(mod1)
-                    with open(osp.join(self.pretrained_folder, f"lsi_cite_{mod1_name}.pkl"), "wb") as f:
-                        pickle.dump(lsi_transformer_gex, f)
+                    lsi_transformer_gex.fit(self.modalities[0])
+                    pickle.dump(lsi_transformer_gex, open(os.path.join(pretrained_folder, f"lsi_cite_{mod1}.pkl"),
+                                                          "wb"))
 
-            if mod2_name == "ATAC":
+            if mod2 == "ATAC":
 
-                if osp.exists(osp.join(self.pretrained_folder, f"lsi_multiome_{mod1_name}.pkl")):
-                    with open(osp.join(self.pretrained_folder, f"lsi_multiome_{mod1_name}.pkl"), "rb") as f:
+                if os.path.exists(os.path.join(pretrained_folder, f"lsi_multiome_{mod1}.pkl")):
+                    with open(os.path.join(pretrained_folder, f"lsi_multiome_{mod1}.pkl"), "rb") as f:
                         lsi_transformer_gex = pickle.load(f)
                 else:
                     lsi_transformer_gex = lsiTransformer(n_components=64, drop_first=True)
-                    lsi_transformer_gex.fit(mod1)
-                    with open(osp.join(self.pretrained_folder, f"lsi_multiome_{mod1_name}.pkl"), "wb") as f:
+                    lsi_transformer_gex.fit(self.modalities[0])
+                    with open(os.path.join(pretrained_folder, f"lsi_multiome_{mod1}.pkl"), "wb") as f:
                         pickle.dump(lsi_transformer_gex, f)
 
-                if osp.exists(osp.join(self.pretrained_folder, f"lsi_multiome_{mod2_name}.pkl")):
-                    with open(osp.join(self.pretrained_folder, f"lsi_multiome_{mod2_name}.pkl"), "rb") as f:
+                if os.path.exists(os.path.join(pretrained_folder, f"lsi_multiome_{mod2}.pkl")):
+                    with open(os.path.join(pretrained_folder, f"lsi_multiome_{mod2}.pkl"), "rb") as f:
                         lsi_transformer_atac = pickle.load(f)
                 else:
                     #         lsi_transformer_atac = TruncatedSVD(n_components=100, random_state=random_seed)
                     lsi_transformer_atac = lsiTransformer(n_components=512, drop_first=True)
-                    lsi_transformer_atac.fit(mod2)
-                    with open(osp.join(self.pretrained_folder, f"lsi_multiome_{mod2_name}.pkl"), "wb") as f:
+                    lsi_transformer_atac.fit(self.modalities[1])
+                    with open(os.path.join(pretrained_folder, f"lsi_multiome_{mod2}.pkl"), "wb") as f:
                         pickle.dump(lsi_transformer_atac, f)
 
-            # Data preprocessing
-            # Only exploration dataset provides cell type information.
-            # The exploration dataset is a subset of the full dataset.
-            ad_mod1 = meta1
+            ##########################################
+            ##           DATA PREPROCESSING         ##
+            ##########################################
+
+            ad_mod1 = self.exploration[0]
+            ad_mod2 = self.exploration[1]
             mod1_obs = ad_mod1.obs
 
             # Make sure exploration data match the full data
-            assert ((mod1.obs["batch"].index[:mod1_obs.shape[0]] == mod1_obs["batch"].index).mean() == 1)
+            assert ((self.modalities[0].obs['batch'].index[:mod1_obs.shape[0]] == mod1_obs['batch'].index).mean() == 1)
 
-            if mod2_name == "ADT":
-                mod1_pca = lsi_transformer_gex.transform(mod1).values
-                mod2_pca = mod2.X.toarray()
-            elif mod2_name == "ATAC":
-                mod1_pca = lsi_transformer_gex.transform(mod1).values
-                mod2_pca = lsi_transformer_atac.transform(mod2).values
-            else:
-                raise ValueError(f"Unknown modality 2: {mod2_name}")
+            if mod2 == "ADT":
+                mod1_pca = lsi_transformer_gex.transform(ad_mod1).values
+                mod1_pca_test = lsi_transformer_gex.transform(self.modalities[0][mod1_obs.shape[0]:]).values
+                mod2_pca = ad_mod2.X.toarray()
+                mod2_pca_test = self.numpy_features(1)[mod1_obs.shape[0]:]
+
+            if mod2 == "ATAC":
+                mod1_pca = lsi_transformer_gex.transform(ad_mod1).values
+                mod1_pca_test = lsi_transformer_gex.transform(self.modalities[0][mod1_obs.shape[0]:]).values
+                mod2_pca = lsi_transformer_atac.transform(ad_mod2).values
+                mod2_pca_test = lsi_transformer_atac.transform(self.modalities[1][mod1_obs.shape[0]:]).values
 
             cell_cycle_genes = [
-                "MCM5", "PCNA", "TYMS", "FEN1", "MCM2", "MCM4", "RRM1", "UNG", "GINS2", "MCM6", "CDCA7", "DTL", "PRIM1",
-                "UHRF1", "MLF1IP", "HELLS", "RFC2", "RPA2", "NASP", "RAD51AP1", "GMNN", "WDR76", "SLBP", "CCNE2",
-                "UBR7", "POLD3", "MSH2", "ATAD2", "RAD51", "RRM2", "CDC45", "CDC6", "EXO1", "TIPIN", "DSCC1", "BLM",
-                "CASP8AP2", "USP1", "CLSPN", "POLA1", "CHAF1B", "BRIP1", "E2F8", "HMGB2", "CDK1", "NUSAP1", "UBE2C",
-                "BIRC5", "TPX2", "TOP2A", "NDC80", "CKS2", "NUF2", "CKS1B", "MKI67", "TMPO", "CENPF", "TACC3", "FAM64A",
-                "SMC4", "CCNB2", "CKAP2L", "CKAP2", "AURKB", "BUB1", "KIF11", "ANP32E", "TUBB4B", "GTSE1", "KIF20B",
-                "HJURP", "CDCA3", "HN1", "CDC20", "TTK", "CDC25C", "KIF2C", "RANGAP1", "NCAPD2", "DLGAP5", "CDCA2",
-                "CDCA8", "ECT2", "KIF23", "HMMR", "AURKA", "PSRC1", "ANLN", "LBR", "CKAP5", "CENPE", "CTCF", "NEK2",
-                "G2E3", "GAS2L3", "CBX5", "CENPA"
-            ]
-            logger.info(f"Data loading and pca done: {mod1_pca.shape=}, {mod2_pca.shape=}")
-            logger.info("Start to calculate cell_cycle score. It may roughly take an hour.")
-
-            cell_type_labels = test_sol.obs["cell_type"].to_numpy()
-            batch_ids = mod1_obs["batch"]
-            phase_labels = mod1_obs["phase"]
+                'MCM5', 'PCNA', 'TYMS', 'FEN1', 'MCM2', \
+                'MCM4', 'RRM1', 'UNG', 'GINS2', 'MCM6', \
+                'CDCA7', 'DTL', 'PRIM1', 'UHRF1', 'MLF1IP', \
+                'HELLS', 'RFC2', 'RPA2', 'NASP', 'RAD51AP1', \
+                'GMNN', 'WDR76', 'SLBP', 'CCNE2', 'UBR7', \
+                'POLD3', 'MSH2', 'ATAD2', 'RAD51', 'RRM2', 'CDC45', \
+                'CDC6', 'EXO1', 'TIPIN', 'DSCC1', 'BLM', 'CASP8AP2', \
+                'USP1', 'CLSPN', 'POLA1', 'CHAF1B', 'BRIP1', 'E2F8', \
+                'HMGB2', 'CDK1', 'NUSAP1', 'UBE2C', 'BIRC5', 'TPX2', \
+                'TOP2A', 'NDC80', 'CKS2', 'NUF2', 'CKS1B', 'MKI67', \
+                'TMPO', 'CENPF', 'TACC3', 'FAM64A', 'SMC4', 'CCNB2', \
+                'CKAP2L', 'CKAP2', 'AURKB', 'BUB1', 'KIF11', 'ANP32E', \
+                'TUBB4B', 'GTSE1', 'KIF20B', 'HJURP', 'CDCA3', 'HN1', \
+                'CDC20', 'TTK', 'CDC25C', 'KIF2C', 'RANGAP1', 'NCAPD2', \
+                'DLGAP5', 'CDCA2', 'CDCA8', 'ECT2', 'KIF23', 'HMMR', \
+                'AURKA', 'PSRC1', 'ANLN', 'LBR', 'CKAP5', 'CENPE', 'CTCF', \
+                'NEK2', 'G2E3', 'GAS2L3', 'CBX5', 'CENPA']
+
+            print('Data loading and pca done', mod1_pca.shape, mod2_pca.shape)
+            print('Start to calculate cell_cycle score. It may roughly take an hour.')
+
+            pca_combined = np.concatenate([mod1_pca, mod2_pca], axis=1)
+
+            del mod1_pca, mod2_pca
+
+            cell_type_labels = mod1_obs['cell_type']
+            batch_ids = mod1_obs['batch']
+            phase_labels = mod1_obs['phase']
             nb_cell_types = len(np.unique(cell_type_labels))
             nb_batches = len(np.unique(batch_ids))
             nb_phases = len(np.unique(phase_labels)) - 1  # 2
-            cell_type_labels_unique = list(np.unique(cell_type_labels))
-            batch_ids_unique = list(np.unique(batch_ids))
-            phase_labels_unique = list(np.unique(phase_labels))
-            c_labels = np.array([cell_type_labels_unique.index(item) for item in cell_type_labels])
-            b_labels = np.array([batch_ids_unique.index(item) for item in batch_ids])
-            p_labels = np.array([phase_labels_unique.index(item) for item in phase_labels])
+            c_labels = np.array([list(np.unique(cell_type_labels)).index(item) for item in cell_type_labels])
+            b_labels = np.array([list(np.unique(batch_ids)).index(item) for item in batch_ids])
+            p_labels = np.array([list(np.unique(phase_labels)).index(item) for item in phase_labels])
             # 0:G1, 1:G2M, 2: S, only consider the last two
             s_genes = cell_cycle_genes[:43]
             g2m_genes = cell_cycle_genes[43:]
             sc.pp.log1p(ad_mod1)
             sc.pp.scale(ad_mod1)
             sc.tl.score_genes_cell_cycle(ad_mod1, s_genes=s_genes, g2m_genes=g2m_genes)
-            S_scores = ad_mod1.obs["S_score"].values
-            G2M_scores = ad_mod1.obs["G2M_score"].values
-            # phase_scores = np.stack([S_scores, G2M_scores]).T  # (nb_cells, 2)
-
-            y_train = [c_labels, b_labels, p_labels, S_scores, G2M_scores]
-            mod1.obsm["X_pca"] = mod1_pca
-            mod2.obsm["X_pca"] = mod2_pca
-            train_size = mod1_obs.shape[0]
-            mod1.obsm["cell_type"] = c_labels
-            mod1.obsm["batch_label"] = np.concatenate([y_train[1], np.zeros(mod1.shape[0] - train_size)], 0)
-            mod1.obsm["phase_labels"] = np.concatenate([y_train[2], np.zeros(mod1.shape[0] - train_size)], 0)
-            mod1.obsm["S_scores"] = np.concatenate([y_train[3], np.zeros(mod1.shape[0] - train_size)], 0)
-            mod1.obsm["G2M_scores"] = np.concatenate([y_train[4], np.zeros(mod1.shape[0] - train_size)], 0)
-
-            preprocessed_data = {"X_pca_0": mod1.obsm["X_pca"], "X_pca_1": mod2.obsm["X_pca"], "y_train": y_train}
-
-            with open(osp.join(self.pretrained_folder, f"preprocessed_data_{self.subtask}.pkl"), "wb") as f:
-                pickle.dump(preprocessed_data, f)
-
-            with open(osp.join(self.pretrained_folder, f"{self.subtask}_config.pk"), "wb") as f:
-                pickle.dump([nb_cell_types, nb_batches, nb_phases], f)
+            S_scores = ad_mod1.obs['S_score'].values
+            G2M_scores = ad_mod1.obs['G2M_score'].values
+            phase_scores = np.stack([S_scores, G2M_scores]).T  # (nb_cells, 2)
+
+            X_train = pca_combined
+            # c_labels: cell type; b_labels: batch ids; p_labels: phase_labels; phase_scores
+            Y_train = [c_labels, b_labels, p_labels, phase_scores]
+            X_test = np.concatenate([mod1_pca_test, mod2_pca_test], axis=1)
+
+            self.preprocessed_data = {'X_train': X_train, 'Y_train': Y_train, 'X_test': X_test}
+            pickle.dump(self.preprocessed_data,
+                        open(os.path.join(pretrained_folder, f'preprocessed_data_{self.subtask}.pkl'), 'wb'))
+            pickle.dump([nb_cell_types, nb_batches, nb_phases],
+                        open(os.path.join(pretrained_folder, f'{self.subtask}_config.pk'), 'wb'))
 
             self.nb_cell_types, self.nb_batches, self.nb_phases = nb_cell_types, nb_batches, nb_phases
-
-        elif self.preprocess == "feature_selection":
-            if mod1.shape[1] > selection_threshold:
-                sc.pp.highly_variable_genes(mod1, layer="counts", flavor="seurat_v3", n_top_genes=selection_threshold)
-                mod1 = mod1[:, mod1.var["highly_variable"]]
-
-            if mod2.shape[1] > selection_threshold:
-                sc.pp.highly_variable_genes(mod2, layer="counts", flavor="seurat_v3", n_top_genes=selection_threshold)
-                mod2 = mod2[:, mod2.var["highly_variable"]]
-
+        elif kind == 'feature_selection':
+            for i in range(2):
+                if self.modalities[i].shape[1] > selection_threshold:
+                    sc.pp.highly_variable_genes(self.modalities[i], layer='counts', flavor='seurat_v3',
+                                                n_top_genes=selection_threshold)
+                    self.modalities[i] = self.modalities[i][:, self.modalities[i].var['highly_variable']]
         else:
-            logger.info(f"Preprocessing method {self.preprocess!r} not supported.")
-
-        # Normalization
-        if self.normalize:
-            sc.pp.scale(mod1)
-            sc.pp.scale(mod2)
-
-        logger.info("Preprocessing done.")
+            print('Preprocessing method not supported.')
+            return self
+        self.preprocessed = True
+        print('Preprocessing done.')
+        return self
+
+    def get_preprocessed_data(self):
+        return self.preprocessed_data
+
+    def normalize(self):
+        assert self.preprocessed, 'Normalization must be conducted after preprocessing.'
+
+        self.mean = np.concatenate([self.preprocessed_data['X_train'], self.preprocessed_data['X_test']], 0).mean()
+        self.std = np.concatenate([self.preprocessed_data['X_train'], self.preprocessed_data['X_test']], 0).std()
+        self.preprocessed_data['X_train'] = (self.preprocessed_data['X_train'] - self.mean) / self.std
+        self.preprocessed_data['X_test'] = (self.preprocessed_data['X_test'] - self.mean) / self.std
 
-        return mod1, mod2, meta1, meta2, test_sol
+        return self
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/joint_embedding/dcca.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/dcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 # from DCCA.loss_function import log_zinb_positive, log_nb_positive, binary_cross_entropy, mse_loss, KL_diver
 from dance.utils.loss import Attention, Correlation, Eucli_dis, FactorTransfer, KL_diver, L1_dis, NSTLoss, Similarity
 
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 
 
 def mse_loss(y_true, y_pred):
+
     mask = torch.sign(y_true)
 
     y_pred = y_pred.float()
     y_true = y_true.float()
 
     ret = torch.pow((y_pred - y_true) * mask, 2)
 
@@ -119,14 +120,15 @@
                 ),
             ) for i, (n_in, n_out) in enumerate(zip(layers[:-1], layers[1:]))]))
 
     return fc_layers
 
 
 def adjust_learning_rate(init_lr, optimizer, iteration, max_lr, adjust_epoch):
+
     lr = max(init_lr * (0.9**(iteration // adjust_epoch)), max_lr)
     for param_group in optimizer.param_groups:
         param_group["lr"] = lr
 
     return lr
 
 
@@ -667,32 +669,34 @@
         Latent space dimension for VAE2.
     layer_d_2 : int
         Hidden layer specification for decoder2. List the dimensions of each hidden layer sequentially.
     hidden2_2 : int
         Hidden dimension for decoder2. It should be consistent with the last layer in layer_d_1.
     args : argparse.Namespace
         A Namespace object that contains arguments of DCCA. For details of parameters in parser args, please refer to link (parser help document).
-    ground_truth1 : torch.Tensor
+    ground_truth1 : pandas.Series
         Extra labels for VAE1.
+    ground_truth2 :
+        Extra labels for VAE2.
     Type_1 : str optional
         Loss type for VAE1. Default: 'NB'. By default to be 'NB'.
     Type_2 : str optional
         Loss type for VAE2. Default: 'Bernoulli'. By default to be 'Bernoulli'.
     cycle : int optional
         Number of multiple training cycles. In each cycle iteratively update VAE1 and VAE2. By default to be 1.
     attention_loss : str optional
         Loss type of attention loss. By default to be 'Eucli'.
     droprate : float optional
         Dropout rate for encoder/decoder layers. By default to be 0.1.
 
     """
 
     def __init__(self, layer_e_1, hidden1_1, Zdim_1, layer_d_1, hidden2_1, layer_e_2, hidden1_2, Zdim_2, layer_d_2,
-                 hidden2_2, args, ground_truth1, Type_1='NB', Type_2='Bernoulli', cycle=1, attention_loss='Eucli',
-                 droprate=0.1):
+                 hidden2_2, args, ground_truth1, ground_truth2, Type_1='NB', Type_2='Bernoulli', cycle=1,
+                 attention_loss='Eucli', droprate=0.1):
 
         super().__init__()
         # cycle indicates the mutual learning, 0 for initiation of model1 with scRNA-seq data,
         # and odd for training other models, even for scRNA-seq
 
         self.model1 = VAE(layer_e=layer_e_1, hidden1=hidden1_1, Zdim=Zdim_1, layer_d=layer_d_1, hidden2=hidden2_1,
                           Type=Type_1, droprate=droprate).to(args.device)
@@ -721,19 +725,20 @@
             self.attention = L1_dis()
 
         else:
             self.attention = Eucli_dis()
 
         self.cycle = cycle
         self.args = args
-        self.ground_truth1 = ground_truth1.numpy()
+        self.ground_truth1 = ground_truth1
+        self.ground_truth2 = ground_truth2
         self.attention_loss = attention_loss
 
     def fit(self, train_loader, test_loader, total_loader, first="RNA"):
-        """Fit function for training.
+        """fit function for training.
 
         Parameters
         ----------
         train_loader : torch.utils.data.DataLoader
             Dataloader for training dataset.
         test_loader : torch.utils.data.DataLoader
             Dataloader for testing dataset.
@@ -820,15 +825,15 @@
                     else:
                         self.model1.fit(train_loader, test_loader, total_loader, self.model2, self.args, self.attention,
                                         used_cycle, 1, first, self.attention_loss)
 
             used_cycle = used_cycle + 1
 
     def score(self, dataloader):
-        """Score function to get score of prediction.
+        """score function to get score of prediction.
 
         Parameters
         ----------
         dataloader : torch.utils.data.DataLoader
             Dataloader for testing dataset.
 
         Returns
@@ -851,14 +856,17 @@
 
             kmeans1 = KMeans(n_clusters=self.args.cluster1, n_init=5, random_state=200)
             kmeans2 = KMeans(n_clusters=self.args.cluster2, n_init=5, random_state=200)
 
             latent_code_rna = []
             latent_code_atac = []
 
+            ARI_score1, NMI_score1 = -100, -100
+            ARI_score2, NMI_score2 = -100, -100
+
             for batch_idx, (X1, _, size_factor1, X2, _, size_factor2) in enumerate(dataloader):
 
                 X1, size_factor1 = X1.to(self.args.device), size_factor1.to(self.args.device)
                 X2, size_factor2 = X2.to(self.args.device), size_factor2.to(self.args.device)
 
                 X1, size_factor1 = Variable(X1), Variable(size_factor1)
                 X2, size_factor2 = Variable(X2), Variable(size_factor2)
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/joint_embedding/jae.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/jae.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Reimplementation of the JAE model, which is adapted from scDEC.
 
 Extended from https://github.com/kimmo1019/JAE
 
 Reference
 ---------
-Liu Q, Chen S, Jiang R, et al. Simultaneous deep generative modelling and clustering of single-cell genomic data[J].
-Nature machine intelligence, 2021, 3(6): 536-544.
+Liu Q, Chen S, Jiang R, et al. Simultaneous deep generative modelling and clustering of single-cell genomic data[J]. Nature machine intelligence, 2021, 3(6): 536-544.
 
 """
 
+import math
 import os
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+import torch.optim as optim
 from torch.utils.data import DataLoader
 
 from dance.utils import SimpleIndexDataset
 from dance.utils.metrics import *
 
 
 def random_classification_loss(y_pred, nb_batches):
@@ -29,47 +30,46 @@
 
 class JAEWrapper:
     """JAE class.
 
     Parameters
     ----------
     args : argparse.Namespace
-        A Namespace object that contains arguments of JAE. For details of parameters in parser args, please refer to
-        link (parser help document).
+        A Namespace object that contains arguments of JAE. For details of parameters in parser args, please refer to link (parser help document).
     dataset : dance.datasets.multimodality.JointEmbeddingNIPSDataset
         Joint embedding dataset.
 
     """
 
-    def __init__(self, args, num_celL_types, num_batches, num_phases, num_features):
-        self.model = JAE(num_celL_types, num_batches, num_phases, num_features).to(args.device)
-        print(num_celL_types, num_batches, num_phases, num_features)
+    def __init__(self, args, dataset):
+        self.model = JAE(dataset.nb_cell_types, dataset.nb_batches, dataset.nb_phases,
+                         dataset.preprocessed_data['X_train'].shape[1]).to(args.device)
         self.args = args
 
-    def fit(self, inputs, cell_type, batch_label, phase_score):
-        """Fit function for training.
+    def fit(self, inputs, labels):
+        """fit function for training.
 
         Parameters
         ----------
         inputs : torch.Tensor
             Modality features.
-        cell_type : torch.Tensor
-            Cell type labels.
-        batch_label : torch.Tensor
-            Batch labels.
-        phase_score : torch.Tensor
-            Phase scores.
+        labels : list[torch.Tensor]
+            Multiple auxiliary labels for supervision.
 
         Returns
         -------
         None.
 
         """
-        X = inputs.float().to(self.args.device)
-        Y = [cell_type.to(self.args.device), batch_label.to(self.args.device), phase_score.float().to(self.args.device)]
+        X = torch.from_numpy(inputs).float().to(self.args.device)
+        Y = [
+            torch.from_numpy(labels[0]).long().to(self.args.device),
+            torch.from_numpy(labels[1]).long().to(self.args.device),
+            torch.from_numpy(labels[3]).float().to(self.args.device)
+        ]
 
         idx = np.random.permutation(X.shape[0])
         train_idx = idx[:int(idx.shape[0] * 0.9)]
         val_idx = idx[int(idx.shape[0] * 0.9):]
 
         train_dataset = SimpleIndexDataset(train_idx)
         train_loader = DataLoader(
@@ -115,15 +115,15 @@
                 loss.backward()
                 optimizer.step()
 
             for i in range(4):
                 print(f'loss{i + 1}', total_loss[i] / len(train_loader), end=', ')
             print()
 
-            loss1, loss2, loss3, loss4 = self.score(X, val_idx, Y[0], Y[1], Y[2])
+            loss1, loss2, loss3, loss4 = self.score(X, val_idx, Y)
             weighted_loss = loss1 * 0.7 + loss2 * 0.2 + loss3 * 0.05 + loss4 * 0.05
             print('val-loss1', loss1, 'val-loss2', loss2, 'val-loss3', loss3, 'val-loss4', loss4)
             print('val score', weighted_loss)
             vals.append(weighted_loss)
             if min(vals) == vals[-1]:
                 if not os.path.exists('models'):
                     os.mkdir('models')
@@ -187,27 +187,25 @@
 
         """
         self.model.eval()
         with torch.no_grad():
             prediction = self.model.encoder(inputs[idx])
         return prediction
 
-    def score(self, inputs, idx, cell_type, batch_label=None, phase_score=None, metric='loss'):
+    def score(self, inputs, idx, labels, metric='loss'):
         """Score function to get score of prediction.
 
         Parameters
         ----------
         inputs : torch.Tensor
             Multimodality features.
         idx : Iterable[int]
             Index of testing cells for scoring.
-        cell_type : torch.Tensor
-            Cell type labels.
-        phase_score : torch.Tensor
-            Cell cycle phase labels.
+        labels : list[torch.Tensor]
+            Multiple labels for evaluation.
         metric : str optional
             The type of evaluation metric, by default to be 'loss'.
 
         Returns
         -------
         loss1 : float
             Reconstruction loss.
@@ -225,29 +223,28 @@
 
             if metric == 'loss':
                 ce = nn.CrossEntropyLoss()
                 mse = nn.MSELoss()
                 X = inputs[idx]
                 output = self.model(X)
                 loss1 = mse(output[0], X).item()
-                loss2 = ce(output[1], cell_type[idx]).item()
-                loss3 = random_classification_loss(output[2], batch_label[idx]).item()
-                loss4 = mse(output[3], phase_score[idx]).item()
+                loss2 = ce(output[1], labels[0][idx]).item()
+                loss3 = random_classification_loss(output[2], labels[1][idx]).item()
+                loss4 = mse(output[3], labels[2][idx]).item()
 
                 return loss1, loss2, loss3, loss4
             else:
                 emb = self.predict(inputs, idx).cpu().numpy()
 
                 kmeans = KMeans(n_clusters=10, n_init=5, random_state=200)
 
                 # adata.obs['batch'] = adata_sol.obs['batch'][adata.obs_names]
                 # adata.obs['cell_type'] = adata_sol.obs['cell_type'][adata.obs_names]
-                true_labels = cell_type
+                true_labels = labels
                 pred_labels = kmeans.fit_predict(emb)
-                print(true_labels, pred_labels)
                 NMI_score = round(normalized_mutual_info_score(true_labels, pred_labels, average_method='max'), 3)
                 ARI_score = round(adjusted_rand_score(true_labels, pred_labels), 3)
 
                 # print('ARI: ' + str(ARI_score) + ' NMI: ' + str(NMI_score))
                 return NMI_score, ARI_score
 
 
@@ -299,13 +296,9 @@
         return x
 
     def forward(self, x):
         x = self.encoder(x)
         x0 = x
         x = self.decoder(x)
 
-        return (
-            x,
-            x0[:, :self.nb_cell_types],
-            x0[:, self.nb_cell_types:self.nb_cell_types + self.nb_batches],
-            x0[:, self.nb_cell_types + self.nb_batches:self.nb_cell_types + self.nb_batches + self.nb_phases],
-        )
+        return x, x0[:, :self.nb_cell_types], x0[:, self.nb_cell_types:self.nb_cell_types + self.nb_batches], \
+               x0[:, self.nb_cell_types + self.nb_batches:self.nb_cell_types + self.nb_batches + self.nb_phases]
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/joint_embedding/scmogcn.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/scmogcn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,162 +1,92 @@
 """Official release of scMoGNN method.
 
 Reference
 ---------
-Wen, Hongzhi, et al. "Graph Neural Networks for Multimodal Single-Cell Data Integration." arXiv:2203.01884 (2022).
+Wen, Hongzhi, et al. "Graph Neural Networks for Multimodal Single-Cell Data Integration." arXiv preprint arXiv:2203.01884 (2022).
 
 """
+
+import math
 import os
 
-import dgl.nn.pytorch as dglnn
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from sklearn.cluster import KMeans
-from sklearn.metrics import adjusted_rand_score
-from sklearn.metrics.cluster import normalized_mutual_info_score
+import torch.optim as optim
 from torch.utils.data import DataLoader
 
-from dance import logger
 from dance.utils import SimpleIndexDataset
+from dance.utils.metrics import *
 
 
 def propagation_layer_combination(X, idx, wt, from_logits=True):
     if from_logits:
         wt = torch.softmax(wt, -1)
 
     x = 0
     for i in range(wt.shape[0]):
         x += wt[i] * X[i][idx]
 
     return x
 
 
-def cell_feature_propagation(g, alpha: float = 0.5, beta: float = 0.5, cell_init: str = None, feature_init: str = 'id',
-                             device: str = 'cuda', layers: int = 3):
-    g = g.to(device)
-    gconv = dglnn.HeteroGraphConv(
-        {
-            'cell2feature': dglnn.GraphConv(in_feats=0, out_feats=0, norm='none', weight=False, bias=False),
-            'rev_cell2feature': dglnn.GraphConv(in_feats=0, out_feats=0, norm='none', weight=False, bias=False),
-        }, aggregate='sum')
-
-    if feature_init is None:
-        feature_X = torch.zeros((g.nodes('feature').shape[0], g.srcdata[cell_init]['cell'].shape[1])).float().to(device)
-    elif feature_init == 'id':
-        feature_X = F.one_hot(g.srcdata['id']['feature']).float().to(device)
-    else:
-        raise NotImplementedError(f'Not implemented feature init feature {feature_init}.')
-
-    if cell_init is None:
-        cell_X = torch.zeros(g.nodes('cell').shape[0], feature_X.shape[1]).float().to(device)
-    else:
-        cell_X = g.srcdata[cell_init]['cell'].float().to(device)
-
-    h = {'feature': feature_X, 'cell': cell_X}
-    hcell = []
-    for i in range(layers):
-        h1 = gconv(
-            g, h, mod_kwargs={
-                'cell2feature': {
-                    'edge_weight': g.edges['cell2feature'].data['weight'].float()
-                },
-                'rev_cell2feature': {
-                    'edge_weight': g.edges['rev_cell2feature'].data['weight'].float()
-                }
-            })
-        logger.debug(f"{i} cell {h['cell'].abs().mean()} {h1['cell'].abs().mean()}")
-        logger.debug(f"{i} feature {h['feature'].abs().mean()} {h1['feature'].abs().mean()}")
-
-        h1['feature'] = (h1['feature'] -
-                         h1['feature'].mean()) / (h1['feature'].std() if h1['feature'].mean() != 0 else 1)
-        h1['cell'] = (h1['cell'] - h1['cell'].mean()) / (h1['cell'].std() if h1['cell'].mean() != 0 else 1)
-
-        h = {
-            'feature': h['feature'] * alpha + h1['feature'] * (1 - alpha),
-            'cell': h['cell'] * beta + h1['cell'] * (1 - beta)
-        }
-
-        h['feature'] = (h['feature'] - h['feature'].mean()) / h['feature'].std()
-        h['cell'] = (h['cell'] - h['cell'].mean()) / h['cell'].std()
-
-        hcell.append(h['cell'])
-
-    logger.debug(f"{hcell[-1].abs().mean()=}")
-
-    return hcell[1:]
-
-
 class ScMoGCNWrapper:
     """ScMoGCN class.
 
     Parameters
     ----------
     args : argparse.Namespace
-        A Namespace object that contains arguments of ScMoGCN. For details of parameters in parser args, please refer
-        to link (parser help document).
+        A Namespace object that contains arguments of ScMoGCN. For details of parameters in parser args, please refer to link (parser help document).
     dataset : dance.datasets.multimodality.JointEmbeddingNIPSDataset
         Joint embedding dataset.
 
     """
 
-    def __init__(self, args, num_celL_types, num_batches, num_phases, num_features):
-        self.model = ScMoGCN(num_celL_types, num_batches, num_phases, num_features).to(args.device)
+    def __init__(self, args, dataset):
+        self.model = Transformation(dataset.nb_cell_types, dataset.nb_batches, dataset.nb_phases,
+                                    dataset.preprocessed_data['X_train'].shape[1]).to(args.device)
         self.args = args
         self.wt = torch.tensor([0.] * (args.layers - 1)).to(args.device).requires_grad_(True)
 
-    def fit(self, g_mod1, g_mod2, train_size, cell_type, batch_label, phase_score):
-        """Fit function for training.
+    def fit(self, dataset, inputs, labels):
+        """fit function for training.
 
         Parameters
         ----------
-        g_mod1 : dgl.DGLGraph
-            Bipartite expression feature graph for modality 1.
-        g_mod2 : dgl.DGLGraph
-            Bipartite expression feature graph for modality 2.
-        train_size : int
-            Number of training samples.
-        labels : torch.Tensor
-            Labels for training samples.
-        cell_type :torch.Tensor
-            Cell type labels for training samples.
-        batch_label : torch.Tensor
-            Batch labels for training samples.
-        phase_score : torch.Tensor
-            Phase labels for training samples.
+        dataset : dance.datasets.multimodality.JointEmbeddingNIPSDataset
+            Modality features.
+        inputs : torch.Tensor
+            Modality features.
+        labels : list[torch.Tensor]
+            Multiple auxiliary labels for supervision.
 
         Returns
         -------
         None.
 
         """
 
         wt = self.wt
-        hcell_mod1 = cell_feature_propagation(g_mod1, layers=self.args.layers, device=self.args.device)
-        hcell_mod2 = cell_feature_propagation(g_mod2, layers=self.args.layers, device=self.args.device)
-        self.feat_mod1 = hcell_mod1
-        self.feat_mod2 = hcell_mod2
-        X = []
-        for i in range(len(self.feat_mod1)):
-            X.append(torch.cat([self.feat_mod1[i], self.feat_mod2[i]], dim=1).float().to(self.args.device))
-        self.X = X
-        Y = [cell_type.to(self.args.device), batch_label.to(self.args.device), phase_score.float().to(self.args.device)]
+        X = inputs
+        Y = [
+            torch.from_numpy(labels[0]).long().to(self.args.device),
+            torch.from_numpy(labels[1]).long().to(self.args.device),
+            torch.from_numpy(labels[3]).float().to(self.args.device)
+        ]
 
-        idx = np.random.permutation(train_size)
+        idx = np.random.permutation(dataset.preprocessed_data['X_train'].shape[0])
         train_idx = idx[:int(idx.shape[0] * 0.9)]
         val_idx = idx[int(idx.shape[0] * 0.9):]
 
-        # Make sure the batch size is small enough to cover all splits
-        batch_size = min(self.args.batch_size, len(val_idx))
-
         train_dataset = SimpleIndexDataset(train_idx)
         train_loader = DataLoader(
             dataset=train_dataset,
-            batch_size=batch_size,
+            batch_size=self.args.batch_size,
             shuffle=True,
             num_workers=1,
         )
 
         ce = nn.CrossEntropyLoss()
         mse = nn.MSELoss()
 
@@ -193,30 +123,29 @@
                 loss.backward()
                 optimizer.step()
 
             for i in range(4):
                 print(f'loss{i + 1}', total_loss[i] / len(train_loader), end=', ')
             print()
 
-            loss1, loss2, loss3, loss4 = self.score(val_idx, Y[0], Y[2])
+            loss1, loss2, loss3, loss4 = self.score(X, val_idx, Y)
             weighted_loss = loss1 * 0.7 + loss2 * 0.2 + loss3 * 0.05 + loss4 * 0.05
             print('val-loss1', loss1, 'val-loss2', loss2, 'val-loss3', loss3, 'val-loss4', loss4)
             print('val score', weighted_loss)
             vals.append(weighted_loss)
             if min(vals) == vals[-1]:
                 if not os.path.exists('models'):
                     os.mkdir('models')
                 torch.save(self.model.state_dict(), f'models/model_joint_embedding_{self.args.rnd_seed}.pth')
                 weight_record = wt.detach()
 
             if min(vals) != min(vals[-10:]):
                 break
 
         self.wt = weight_record
-        self.fitted = True
 
     def to(self, device):
         """Performs device conversion.
 
         Parameters
         ----------
         device : str
@@ -227,17 +156,14 @@
         self : ScMoGCNWrapper
             Converted model.
 
         """
 
         self.args.device = device
         self.model = self.model.to(device)
-        self.feat_mod1 = self.feat_mod1.to(device)
-        self.feat_mod2 = self.feat_mod2.to(device)
-        self.X = self.X.to(device)
         return self
 
     def load(self, path, map_location=None):
         """Load model parameters from checkpoint file.
 
         Parameters
         ----------
@@ -247,56 +173,52 @@
             Mapped device. This parameter will be passed to torch.load function if not none.
 
         Returns
         -------
         None.
 
         """
-        self.fitted = True
         if map_location is not None:
             self.model.load_state_dict(torch.load(path, map_location=map_location))
         else:
             self.model.load_state_dict(torch.load(path))
 
-    def predict(self, idx):
+    def predict(self, inputs, idx):
         """Predict function to get latent representation of data.
 
         Parameters
         ----------
-        idx : Iterable[int]
-            Index of testing samples for prediction.
+        inputs : torch.Tensor
+            Multimodality features.
 
         Returns
         -------
         prediction : torch.Tensor
             Joint embedding of input data.
 
         """
-        if not self.fitted:
-            raise RuntimeError('Model is not fitted yet.')
         self.model.eval()
         wt = self.wt
-        inputs = self.X
 
         with torch.no_grad():
             X = propagation_layer_combination(inputs, idx, wt)
 
         return self.model.encoder(X)
 
-    def score(self, idx, cell_type, phase_score=None, metric='loss'):
+    def score(self, inputs, idx, labels, metric='loss'):
         """Score function to get score of prediction.
 
         Parameters
         ----------
+        inputs : torch.Tensor
+            Multimodality features.
         idx : Iterable[int]
             Index of testing samples for scoring.
-        cell_type : torch.Tensor
-            Cell type labels of testing samples.
-        phase_score : torch.Tensor optional
-            Cell cycle score of testing samples.
+        labels: list[torch.Tensor]
+            Multiple cell labels for evaluation.
         metric : str optional
             The type of evaluation metric, by default to be 'loss'.
 
         Returns
         -------
         loss1 : float
             Reconstruction loss.
@@ -308,42 +230,41 @@
             Cell cycle score loss.
 
         """
 
         self.model.eval()
         ce = nn.CrossEntropyLoss()
         mse = nn.MSELoss()
-        inputs = self.X
 
         with torch.no_grad():
             if metric == 'loss':
                 X = propagation_layer_combination(inputs, idx, self.wt)
                 output = self.model(X)
                 loss1 = mse(output[0], X).item()
-                loss2 = ce(output[1], cell_type[idx]).item()
+                loss2 = ce(output[1], labels[0][idx]).item()
                 loss3 = (torch.norm(output[2], p=2, dim=-1).sum() * 1e-2).item()
-                loss4 = mse(output[3], phase_score[idx]).item()
+                loss4 = mse(output[3], labels[2][idx]).item()
 
                 return loss1, loss2, loss3, loss4
             else:
-                emb = self.predict(idx).cpu().numpy()
+                emb = self.predict(inputs, idx).cpu().numpy()
                 kmeans = KMeans(n_clusters=10, n_init=5, random_state=200)
 
                 # adata.obs['batch'] = adata_sol.obs['batch'][adata.obs_names]
                 # adata.obs['cell_type'] = adata_sol.obs['cell_type'][adata.obs_names]
-                true_labels = cell_type
+                true_labels = labels
                 pred_labels = kmeans.fit_predict(emb)
                 NMI_score = round(normalized_mutual_info_score(true_labels, pred_labels, average_method='max'), 3)
                 ARI_score = round(adjusted_rand_score(true_labels, pred_labels), 3)
 
                 # print('ARI: ' + str(ARI_score) + ' NMI: ' + str(NMI_score))
                 return NMI_score, ARI_score
 
 
-class ScMoGCN(nn.Module):
+class Transformation(nn.Module):
 
     def __init__(self, nb_cell_types, nb_batches, nb_phases, input_dimension):
         super().__init__()
         self.nb_cell_types = nb_cell_types
         self.nb_batches = nb_batches
         self.nb_phases = nb_phases
 
@@ -387,13 +308,9 @@
         return x
 
     def forward(self, x):
         x = self.encoder(x)
         x0 = x
         x = self.decoder(x)
 
-        return (
-            x,
-            x0[:, :self.nb_cell_types],
-            x0[:, self.nb_cell_types:self.nb_cell_types + self.nb_batches],
-            x0[:, self.nb_cell_types + self.nb_batches:self.nb_cell_types + self.nb_batches + self.nb_phases],
-        )
+        return x, x0[:, :self.nb_cell_types], x0[:, self.nb_cell_types:self.nb_cell_types + self.nb_batches], \
+               x0[:, self.nb_cell_types + self.nb_batches:self.nb_cell_types + self.nb_batches + self.nb_phases]
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/joint_embedding/scmogcnv2.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/scmogcnv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
 
     def __init__(self, args):
         super().__init__()
         self.args = args
         self.model = ScMoGCN(args).to(args.device)
 
     def fit(self, g, y, train_labels=None, epochs=500):
-        """Fit function for training.
+        """fit function for training.
 
         Parameters
         ----------
         g : dgl.DGLGraph
             Constructed cell-feature graph.
         y : torch.Tensor
             Modality features, used as labels for reconstruction.
@@ -942,15 +942,15 @@
 
     def __init__(self, args):
         super().__init__()
         self.args = args
         self.model = ScMoGCN(args).to(args.device)
 
     def fit(self, g, y, train_labels=None, epochs=500):
-        """Fit function for training.
+        """fit function for training.
 
         Parameters
         ----------
         g : dgl.DGLGraph
             Constructed cell-feature graph.
         y : torch.Tensor
             Modality features, used as labels for reconstruction.
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/joint_embedding/scmvae.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/joint_embedding/scmvae.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 def save_checkpoint(model, fileName='./saved_model/model_best.pth.tar'):
     folder = os.path.dirname(fileName)
     os.makedirs(folder, exist_ok=True)
     torch.save(model.state_dict(), fileName)
 
 
 def load_checkpoint(file_path, model, device):
+
     model.load_state_dict(torch.load(file_path))
     model.to(device)
 
     return model
 
 
 def binary_cross_entropy(recon_x, x):
@@ -111,14 +112,15 @@
 
     ret = y_pred - y_true * torch.log(y_pred + 1e-10) + torch.lgamma(y_true + 1.0)
 
     return torch.sum(ret, dim=1)
 
 
 def adjust_learning_rate(init_lr, optimizer, iteration, max_lr, adjust_epoch):
+
     lr = max(init_lr * (0.9**(iteration // adjust_epoch)), max_lr)
     for param_group in optimizer.param_groups:
         param_group["lr"] = lr
 
     return lr
 
 
@@ -616,15 +618,15 @@
         recon_x1 = np.concatenate(recon_x1)
         norm_x1 = np.concatenate(norm_x1)
         norm_x2 = np.concatenate(norm_x2)
 
         return latent_z, recon_x1, norm_x1, recon_x_2, norm_x2
 
     def fit(self, args, train, valid, final_rate, scale_factor, device):
-        """Fit function for training.
+        """fit function for training.
 
         Parameters
         ----------
         train : torch.utils.data.DataLoader
             Dataloader for training dataset.
         valid : torch.utils.data.DataLoader
             Dataloader for testing dataset.
@@ -791,72 +793,75 @@
             elif out == 'recon_X2':
                 return result["recon_x_2"]
             elif out == 'logit':
                 print('Logit not supported.')
                 # output.append(self.get_gamma(z)[0].cpu().detach())
                 return None
 
-    def score(self, X1, X2, labels):
-        """Score function to get score of prediction.
+    def score(self, X1, X2, adata_sol):
+        """score function to get score of prediction.
 
         Parameters
         ----------
         X1 : torch.Tensor
             Features of modality 1.
         X2 : torch.Tensor
             Features of modality 2.
-        labels : torch.Tensor
+        adata_sol : anndata.Anndata
             The ground truth labels for evaluation.
 
         Returns
         -------
         NMI_score : float
             NMI eval score.
         ARI_score : float
             ARI eval score.
 
         """
 
         emb = self.predict(X1, X2).cpu().numpy()
+
         kmeans = KMeans(n_clusters=10, n_init=5, random_state=200)
 
-        true_labels = labels.numpy()
-        pred_labels = kmeans.fit_predict(emb)
+        # adata.obs['batch'] = adata_sol.obs['batch'][adata.obs_names]
+        # adata.obs['cell_type'] = adata_sol.obs['cell_type'][adata.obs_names]
+        true_labels = adata_sol.obs['cell_type'].to_numpy()
 
+        pred_labels = kmeans.fit_predict(emb)
         NMI_score = round(normalized_mutual_info_score(true_labels, pred_labels, average_method='max'), 3)
         ARI_score = round(adjusted_rand_score(true_labels, pred_labels), 3)
 
+        # print('ARI: ' + str(ARI_score) + ' NMI: ' + str(NMI_score))
         return NMI_score, ARI_score
 
 
 class ProductOfExperts(nn.Module):
     """Return parameters for product of independent experts. See
     https://arxiv.org/pdf/1410.7827.pdf for equations.
 
-    @param mu: M x D for M experts @param logvar: M x D for M experts
+    @param mu: M x D for M experts
+    @param logvar: M x D for M experts
 
     """
 
     def forward(self, mu, logvar, eps=1e-8):
         var = torch.exp(logvar) + eps
         # precision of i-th Gaussian expert at point x
         T = 1. / var
         pd_mu = torch.sum(mu * T, dim=0) / torch.sum(T, dim=0)
         pd_var = 1. / torch.sum(T, dim=0)
         pd_logvar = torch.log(pd_var)
         return pd_mu, pd_logvar
 
 
 def prior_expert(size):
-    """Universal prior expert. Here we use a spherical.
-
+    """Universal prior expert. Here we use a spherical
     Gaussian: N(0, 1).
     @param size: integer
                  dimensionality of Gaussian
-
     """
     mu = Variable(torch.zeros(size))
     logvar = Variable(torch.log(torch.ones(size)))
 
     return mu, logvar
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/match_modality/cmae.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/match_modality/cmae.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Reimplementation of Cross-Model AutoEncoder method.
 
 Extended from https://github.com/uhlerlab/cross-modal-autoencoders
 
 Reference
 ---------
-Yang, Karren Dai, et al. "Multi-domain translation between single-cell imaging and sequencing data using autoencoders."
-Nature communications 12.1 (2021): 1-10.
+Yang, Karren Dai, et al. "Multi-domain translation between single-cell imaging and sequencing data using autoencoders." Nature communications 12.1 (2021): 1-10.
 
 """
 import math
 import os
+import sys
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.nn.init as init
 from sklearn.neighbors import NearestNeighbors
 from torch.autograd import Variable
@@ -155,18 +155,17 @@
         else:
             encoder_layers += [nn.Linear(self.dim, self.latent), nn.LeakyReLU(0.2, inplace=True)]
             decoder_layers = [nn.Linear(self.latent, self.dim)] + decoder_layers
         self.enc = nn.Sequential(*encoder_layers)
         self.dec = nn.Sequential(*decoder_layers)
 
     def forward(self, images):
-        # This is a reduced VAE implementation where we assume the outputs are multivariate Gaussian distribution
-        # with mean = hiddens and std_dev = all ones.
+        # This is a reduced VAE implementation where we assume the outputs are multivariate Gaussian distribution with mean = hiddens and std_dev = all ones.
         hiddens = self.encode(images)
-        if self.training:
+        if self.training == True:
             noise = Variable(torch.randn(hiddens.size()).cuda(hiddens.data.get_device()))
             images_recon = self.decode(hiddens + noise)
         else:
             images_recon = self.decode(hiddens)
         return images_recon, hiddens
 
     def encode(self, images):
@@ -256,16 +255,15 @@
 
 class CMAE(nn.Module):
     """CMAE class.
 
     Parameters
     ----------
     hyperparameters : dictionary
-        A dictionary that contains arguments of CMAE. For details of parameters in parser args, please refer to link
-        (parser help document).
+        A dictionary that contains arguments of CMAE. For details of parameters in parser args, please refer to link (parser help document).
 
     """
 
     def __init__(self, hyperparameters):
         super().__init__()
         lr = hyperparameters['lr']
         # Initiate the networks
@@ -317,45 +315,45 @@
 
         Returns
         -------
         pred : torch.Tensor
             Joint embedding of input modalities.
 
         """
+
         with torch.no_grad():
             emb1, _ = self.gen_a.encode(mod1)
             emb2, _ = self.gen_b.encode(mod2)
             nn = NearestNeighbors(metric=metric)
             nn.fit(emb1.cpu())
             transp_nearest_neighbor = torch.tensor(nn.kneighbors(emb2.cpu(), 1, return_distance=False))
-            pred = torch.zeros(emb1.shape[0], emb1.shape[0], device=mod1.device)
+            pred = torch.zeros(emb1.shape[0], emb1.shape[0])
             pred[torch.arange(emb1.shape[0]), transp_nearest_neighbor.squeeze(-1)] = 1
         return pred
 
     def score(self, mod1, mod2, labels):
         """Score function to get score of prediction.
 
         Parameters
         ----------
         mod1 : torch.Tensor
             Features of modality 1.
         mod2 : torch.Tensor
             Features of modality 2.
-        labels: torch.Tensor
-            Ground truth mapping of modality 2.
 
         Returns
         -------
         score : float
             Matching accuracy.
 
         """
+
         with torch.no_grad():
             pred = self.predict(mod1, mod2)
-            return (pred[torch.arange(pred.shape[0]).long(), labels.long()].mean()).item()
+            return ((pred * labels).sum() / mod1.shape[0]).item()
 
     def forward(self, mod1, mod2):
         """Forward function for torch.nn.Module.
 
         Parameters
         ----------
         mod1 : torch.Tensor
@@ -376,26 +374,39 @@
         h_b, _ = self.gen_b.encode(mod2)
         x_ba = self.gen_a.decode(h_b)
         x_ab = self.gen_b.decode(h_a)
         self.train()
         return x_ab, x_ba
 
     def _gen_update(self, x_a, x_b, super_a, super_b, hyperparameters, a_labels=None, b_labels=None, variational=True):
+        true_samples = Variable(torch.randn(200, hyperparameters['gen']['latent']), requires_grad=False).cuda()
+
         self.gen_opt.zero_grad()
         # encode
         h_a, n_a = self.gen_a.encode(x_a)
         h_b, n_b = self.gen_b.encode(x_b)
         # decode (within domain)
         if variational:
             h_a = h_a + n_a
             h_b = h_b + n_b
 
         x_a_recon = self.gen_a.decode(h_a)
         x_b_recon = self.gen_b.decode(h_b)
 
+        # decode (cross domain)
+        x_ba = self.gen_a.decode(h_b)
+        x_ab = self.gen_b.decode(h_a)
+        # encode again
+        h_b_recon, n_b_recon = self.gen_a.encode(x_ba)
+        h_a_recon, n_a_recon = self.gen_b.encode(x_ab)
+        # decode again (if needed)
+        if variational:
+            h_a_recon = h_a_recon + n_a_recon
+            h_b_recon = h_b_recon + n_b_recon
+
         classes_a = self.classifier.forward(h_a)
         classes_b = self.classifier.forward(h_b)
 
         # reconstruction loss
         self.loss_gen_recon_x_a = self._mae_loss(x_a_recon, x_a)
         self.loss_gen_recon_x_b = self._mae_loss(x_b_recon, x_b)
 
@@ -415,29 +426,25 @@
         s_b, n_b = self.gen_b.encode(super_b)
 
         self.loss_supervision = self._mae_loss(s_a, s_b)
 
         class_weight = hyperparameters['gan_w'] if "class_w" not in hyperparameters else hyperparameters["class_w"]
 
         # total loss
-        self.loss_gen_total = (
-            hyperparameters['gan_w'] * self.loss_latent_a
-            + hyperparameters['gan_w'] * self.loss_latent_b
-            + class_weight * self.loss_class_a
-            + class_weight * self.loss_class_b
-            + hyperparameters['recon_x_w'] * self.loss_gen_recon_x_a
-            + hyperparameters['recon_x_w'] * self.loss_gen_recon_x_b
-            + hyperparameters['super_w'] * self.loss_supervision
-        )  # yapf: disable
+        self.loss_gen_total = hyperparameters['gan_w'] * self.loss_latent_a + \
+                              hyperparameters['gan_w'] * self.loss_latent_b + \
+                              class_weight * self.loss_class_a + \
+                              class_weight * self.loss_class_b + \
+                              hyperparameters['recon_x_w'] * self.loss_gen_recon_x_a + \
+                              hyperparameters['recon_x_w'] * self.loss_gen_recon_x_b + \
+                              hyperparameters['super_w'] * self.loss_supervision
 
         if variational:
-            self.loss_gen_total += (
-                hyperparameters['recon_kl_w'] * self.loss_gen_recon_kl_a
-                + hyperparameters['recon_kl_w'] * self.loss_gen_recon_kl_b
-            )  # yapf: disable
+            self.loss_gen_total += hyperparameters['recon_kl_w'] * self.loss_gen_recon_kl_a + \
+                                   hyperparameters['recon_kl_w'] * self.loss_gen_recon_kl_b
 
         self.loss_gen_total.backward()
         self.gen_opt.step()
 
     def _sample(self, x_a, x_b):
         self.eval()
         x_a_recon, x_b_recon, x_ba, x_ab = [], [], [], []
@@ -496,15 +503,15 @@
         last_model_name = get_model_list(checkpoint_dir, "dis")
         state_dict = torch.load(last_model_name)
         self.dis_latent.load_state_dict(state_dict['latent'])
         # Load optimizers
         state_dict = torch.load(os.path.join(checkpoint_dir, 'optimizer.pt'))
         self.dis_opt.load_state_dict(state_dict['dis'])
         self.gen_opt.load_state_dict(state_dict['gen'])
-        # Reinitialize schedulers
+        # Reinitilize schedulers
         self.dis_scheduler = get_scheduler(self.dis_opt, hyperparameters, iterations)
         self.gen_scheduler = get_scheduler(self.gen_opt, hyperparameters, iterations)
         print('Resume from iteration %d' % iterations)
         return iterations
 
     def save(self, snapshot_dir, iterations):
         """Save function to save parameters to checkpoint file.
@@ -512,49 +519,55 @@
         Parameters
         ----------
         checkpoint_dir : str
             Path to the checkpoint file.
         iterations : int
             Current number of training iterations.
 
+        Returns
+        -------
+        None.
+
         """
         # Save generators, discriminators, and optimizers
         gen_name = os.path.join(snapshot_dir, 'gen_%08d.pt' % (iterations + 1))
         dis_name = os.path.join(snapshot_dir, 'dis_%08d.pt' % (iterations + 1))
         opt_name = os.path.join(snapshot_dir, 'optimizer.pt')
         torch.save(
             {
                 'a': self.gen_a.state_dict(),
                 'b': self.gen_b.state_dict(),
                 "classifier": self.classifier.state_dict()
             }, gen_name)
         torch.save({'latent': self.dis_latent.state_dict()}, dis_name)
         torch.save({'gen': self.gen_opt.state_dict(), 'dis': self.dis_opt.state_dict()}, opt_name)
 
-    def fit(self, train_mod1, train_mod2, aux_labels=None, checkpoint_directory='./checkpoint', val_ratio=0.15):
+    def fit(self, train_mod1, train_mod2, aux_labels=None, checkpoint_directory='./checkpoint'):
         """Train CMAE.
 
         Parameters
         ----------
         train_mod1 : torch.Tensor
             Features of input modality.
         train_mod2 : torch.Tensor
             Features of target modality.
         aux_labels : torch.Tensor optional
             Auxiliary labels for extra supervision during training.
         checkpoint_directory : str optional
             Path to the checkpoint file, by default to be './checkpoint'.
-        val_ratio : float
-            Ratio for automatic train-validation split.
+
+        Returns
+        -------
+        None.
 
         """
         hyperparameters = self.hyperparameters
         idx = torch.randperm(train_mod1.shape[0])
-        train_idx = idx[:int(idx.shape[0] * (1 - val_ratio))]
-        val_idx = idx[int(idx.shape[0] * (1 - val_ratio)):]
+        train_idx = idx[:-4096]
+        val_idx = idx[-4096:]
 
         train_dataset = SimpleIndexDataset(train_idx)
         train_loader = DataLoader(
             dataset=train_dataset,
             batch_size=hyperparameters['batch_size'],
             shuffle=True,
             num_workers=0,
@@ -566,24 +579,27 @@
                                  hyperparameters=hyperparameters) if hyperparameters['resume'] else 0
         num_disc = 1 if "num_disc" not in hyperparameters else hyperparameters["num_disc"]
         num_gen = 1 if "num_gen" not in hyperparameters else hyperparameters["num_gen"]
 
         while True:
             print('Iteration: ', iterations)
             for it, batch_idx in enumerate(train_loader):
+                self._update_learning_rate()
                 mod1, mod2 = train_mod1[batch_idx], train_mod2[batch_idx]
+
                 for _ in range(num_disc):
                     self._dis_update(mod1, mod2, hyperparameters)
                 for _ in range(num_gen):
                     if aux_labels is not None:
                         self._gen_update(mod1, mod2, mod1, mod2, hyperparameters, aux_labels[batch_idx],
                                          aux_labels[batch_idx], variational=False)
                     else:
                         self._gen_update(mod1, mod2, mod1, mod2, hyperparameters, variational=False)
-                self._update_learning_rate()
-            print('Matching score:', self.score(train_mod1[val_idx], train_mod2[val_idx],
-                                                torch.arange(val_idx.shape[0])))
+
+            print('Matching score:', self.score(train_mod1[val_idx], train_mod2[val_idx], torch.eye(val_idx.shape[0])))
+            # print('Matching score:',
+            #       self.evaluate(test_mod1, test_mod2, labels))
 
             iterations += 1
             if iterations >= hyperparameters['max_epochs']:
                 print('Finish training')
                 return self
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/match_modality/scmm.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/match_modality/scmm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Reimplementation of scMM method.
 
 Extended from https://github.com/kodaim1115/scMM
 
 Reference
 ---------
-Minoura, Kodai, et al. A mixture-of-experts deep generative model for integrated analysis of single-cell multiomics
-data. Cell reports methods 1.5 (2021): 100071.
+Minoura, Kodai, et al. "A mixture-of-experts deep generative model for integrated analysis of single-cell multiomics data." Cell reports methods 1.5 (2021): 100071.
 
 """
 import math
 import os
 
 import numpy as np
+import pandas as pd
+import scipy.sparse as sp
 import torch
 import torch.distributions as dist
 import torch.nn as nn
 import torch.nn.functional as F
-from numpy import prod
+from numpy import prod, sqrt
 from pyro.distributions.zero_inflated import ZeroInflatedNegativeBinomial
 from sklearn.cluster import DBSCAN, KMeans
 from sklearn.neighbors import NearestNeighbors
 from torch import optim
 from torch.utils.data import DataLoader
 
 from dance.utils import SimpleIndexDataset
@@ -126,15 +127,15 @@
     @property
     def pz_params(self):
         return self._pz_params
 
     @property
     def qz_x_params(self):
         if self._qz_x_params is None:
-            raise NameError("qz_x params not initialized yet!")
+            raise NameError("qz_x params not initalised yet!")
         return self._qz_x_params
 
     @staticmethod
     def getDataLoaders(batch_size, shuffle=True, device="cuda"):
         # handle merging individual datasets appropriately in sub-class
         raise NotImplementedError
 
@@ -360,19 +361,17 @@
 
 class MMVAE(nn.Module):
     """MMVAE class.
 
     Parameters
     ----------
     subtask : str
-        Name of the subtask which is composed of the name of two modality. This parameter will indicate some
-        modality-specific features in the model.
+        Name of the subtask which is composed of the name of two modality. This parameter will indicate some modality-specific features in the model.
     params : argparse.Namespace
-        A Namespace object that contains arguments of MMVAE. For details of parameters in parser args, please refer to
-        link (parser help document).
+        A Namespace object that contains arguments of MMVAE. For details of parameters in parser args, please refer to link (parser help document).
 
     """
 
     def __init__(self, subtask, params):
         super().__init__()
         self.pz = dist.Laplace
         assert subtask in ('rna-dna', 'rna-protein')
@@ -492,50 +491,54 @@
             qz_xs, _, _ = self.forward(data)
             if not sampling:
                 lats = [get_mean(qz_x) for qz_x in qz_xs]
             else:
                 lats = [qz_x._sample() for qz_x in qz_xs]
         return lats
 
-    def fit(self, x_train, y_train, val_ratio=0.15):
-        """Fit function for training.
+    def fit(self, dataset):
+        """fit function for training.
 
         Parameters
         ----------
-        x_train : torch.Tensor
-            Input modality for training.
-        y_train : torch.Tensor
-            Target modality for training.
-        val_ratio : float
-            Ratio for automatic train-validation split.
+        dataset : dance.datasets.multimodality.ModalityMatchingDataset
+            Dataset for modality matching.
+
+        Returns
+        -------
+        None.
 
         """
 
         start_early_stop = self.params.deterministic_warmup
 
-        idx = np.random.permutation(x_train.shape[0])
-        train_idx = idx[:int(idx.shape[0] * val_ratio)]
-        val_idx = idx[int(idx.shape[0] * val_ratio):]
+        idx = np.random.permutation(dataset.modalities[0].shape[0])
+        train_idx = idx[:int(idx.shape[0] * 0.85)]
+        val_idx = idx[int(idx.shape[0] * 0.85):]
 
         optimizer = optim.Adam(filter(lambda p: p.requires_grad, self.parameters()), lr=self.params.lr, amsgrad=True)
         assert (self.params.obj in ['m_elbo_naive', 'm_elbo_naive_warmup'])
         objective = m_elbo_naive_warmup if self.params.obj == 'm_elbo_naive_warmup' else m_elbo_naive
         train_dataset = SimpleIndexDataset(train_idx)
         train_loader = DataLoader(
             dataset=train_dataset,
             batch_size=self.params.batch_size,
             shuffle=True,
             num_workers=0,
             drop_last=True,
         )
 
-        train_mod1 = x_train.float().to(self.params.device)
-        train_mod2 = y_train.float().to(self.params.device)
+        train_mod1 = torch.from_numpy(dataset.numpy_features(0, True)).float().to(self.params.device)
+        train_mod2 = torch.from_numpy(dataset.numpy_features(1, True)).float().to(self.params.device)
+        test_mod1 = torch.from_numpy(dataset.numpy_features(2, True)).float().to(self.params.device)
+        test_mod2 = torch.from_numpy(dataset.numpy_features(3, True)).float().to(self.params.device)
+        labels = torch.from_numpy(dataset.test_sol.X.toarray())
+        vals = []
+        tr = []
 
-        tr, vals = [], []
         for epoch in range(1, self.params.epochs + 1):
             self.train()
             b_loss = 0
             for i, batch_idx in enumerate(train_loader):
                 dataT = (train_mod1[batch_idx], train_mod2[batch_idx])
                 beta = (epoch - 1) / start_early_stop if epoch <= start_early_stop else 1
                 if dataT[0].size()[0] == 1:
@@ -562,14 +565,15 @@
                 if not os.path.exists('models'):
                     os.mkdir('models')
                 torch.save(self.state_dict(), f'models/model_{self.params.rnd_seed}.pth')
 
             if epoch % 10 == 0:
                 print('Valid Matching score:',
                       self.score(train_mod1[val_idx], train_mod2[val_idx], torch.eye(val_idx.shape[0])))
+                print('Test Matching score:', self.score(test_mod1, test_mod2, labels))
 
             if epoch > start_early_stop and min(vals) != min(vals[-10:]):
                 print('Early stopped.')
                 self.load_state_dict(torch.load(f'models/model_{self.params.rnd_seed}.pth'))
                 break
 
     def score(self, mod1, mod2, labels=None, metric='minkowski'):
@@ -578,28 +582,25 @@
         Parameters
         ----------
         mod1 : torch.Tensor
             Features of modality 1.
         mod2 : torch.Tensor
             Features of modality 2.
         labels : torch.Tensor optional
-            Labels of matching modality, i.e. cell correspondence between two modalities. Required when metric is not
-            'loss'.
+            Labels of matching modality, i.e. cell correspondence between two modalities. Required when metric is not 'loss'.
         metric : str optional
             Metric of the score function, by default to be 'minkowski'.
 
         Returns
         -------
         score : float
             Score of predicted matching, according to specified metric.
 
         """
         self.eval()
-        mod1 = mod1.float().to(self.params.device)
-        mod2 = mod2.float().to(self.params.device)
         if labels is None:
             assert metric == 'loss', 'Unable to evaluate without labels.'
         if metric == 'loss':
             b_loss = 0
             idx = np.arange(mod1.shape[0])
             dataset = SimpleIndexDataset(idx)
             data_loader = DataLoader(
@@ -612,51 +613,47 @@
             with torch.no_grad():
                 for i, batch_idx in enumerate(data_loader):
                     objective = m_elbo_naive_warmup if self.params.obj == 'm_elbo_naive_warmup' else 'm_elbo_naive'
                     loss = -objective(self, [mod1[batch_idx], mod2[batch_idx]], 1).item()
                     b_loss += loss
             return b_loss / mod1.shape[0]
         else:
-            pred = self.predict(mod1, mod2, metric=metric)
-        return (pred[torch.arange(pred.shape[0]).long(), labels.long()].mean()).item()
+            pred = self.predict([mod1, mod2], metric=metric)
+        return ((pred * labels).sum() / mod1.shape[0]).item()
 
-    def predict(self, mod1, mod2, metric='minkowski'):
+    def predict(self, feats, metric='minkowski'):
         """Predict function to get score of prediction.
 
         Parameters
         ----------
-        mod1 : torch.Tensor
-            Features of the first modality.
-        mod2 : torch.Tensor
-            Features of the second modality.
+        feats : list[torch.Tensor]
+            Features of two modalities.
         metric : str optional
             Metric of the matching function, by default to be 'minkowski'.
 
         Returns
         -------
         pred : float
             Predicted matching between two modalities.
 
         """
         self.eval()
-        idx = np.arange(mod1.shape[0])
-        mod1 = mod1.float().to(self.params.device)
-        mod2 = mod2.float().to(self.params.device)
+        idx = np.arange(feats[0].shape[0])
         dataset = SimpleIndexDataset(idx)
         data_loader = DataLoader(
             dataset=dataset,
             batch_size=self.params.batch_size * 10,
             shuffle=False,
             num_workers=0,
             drop_last=False,
         )
         pred = []
         with torch.no_grad():
             for i, batch_idx in enumerate(data_loader):
-                dataT = [mod1[batch_idx], mod2[batch_idx]]
+                dataT = [feats[0][batch_idx], feats[1][batch_idx]]
                 lats = self._get_latents(dataT, sampling=False)
                 if i == 0:
                     pred = lats
                 else:
                     for m, lat in enumerate(lats):
                         pred[m] = torch.cat([pred[m], lat], dim=0)
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/match_modality/scmogcn.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/match_modality/scmogcn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 """Official release of scMoGNN method.
 
 Reference
 ---------
-Wen, Hongzhi, et al. "Graph Neural Networks for Multimodal Single-Cell Data Integration." arXiv preprint
-arXiv:2203.01884 (2022).
+Wen, Hongzhi, et al. "Graph Neural Networks for Multimodal Single-Cell Data Integration." arXiv preprint arXiv:2203.01884 (2022).
 
 """
 import math
 import os
 
-import dgl.nn.pytorch as dglnn
 import numpy as np
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 import torch.optim as optim
 from torch.utils.data import DataLoader
 
-from dance import logger
 from dance.utils import SimpleIndexDataset
 from dance.utils.metrics import batch_separated_bipartite_matching
 
 
 def propagation_layer_combination(X, Y, idx, wt1, wt2, from_logits=True):
     if from_logits:
         wt1 = torch.softmax(wt1, -1)
@@ -33,78 +29,23 @@
         wt2 = torch.softmax(wt2, -1)
     y = 0
     for i in range(wt2.shape[0]):
         y += wt2[i] * Y[i][idx]
     return x, y
 
 
-def cell_feature_propagation(g, alpha: float = 0.5, beta: float = 0.5, cell_init: str = None, feature_init: str = 'id',
-                             device: str = 'cuda', layers: int = 3):
-    g = g.to(device)
-    gconv = dglnn.HeteroGraphConv(
-        {
-            'cell2feature': dglnn.GraphConv(in_feats=0, out_feats=0, norm='none', weight=False, bias=False),
-            'rev_cell2feature': dglnn.GraphConv(in_feats=0, out_feats=0, norm='none', weight=False, bias=False),
-        }, aggregate='sum')
-
-    if feature_init is None:
-        feature_X = torch.zeros((g.nodes('feature').shape[0], g.srcdata[cell_init]['cell'].shape[1])).float().to(device)
-    elif feature_init == 'id':
-        feature_X = F.one_hot(g.srcdata['id']['feature']).float().to(device)
-    else:
-        raise NotImplementedError(f'Not implemented feature init feature {feature_init}.')
-
-    if cell_init is None:
-        cell_X = torch.zeros(g.nodes('cell').shape[0], feature_X.shape[1]).float().to(device)
-    else:
-        cell_X = g.srcdata[cell_init]['cell'].float().to(device)
-
-    h = {'feature': feature_X, 'cell': cell_X}
-    hcell = []
-    for i in range(layers):
-        h1 = gconv(
-            g, h, mod_kwargs={
-                'cell2feature': {
-                    'edge_weight': g.edges['cell2feature'].data['weight'].float()
-                },
-                'rev_cell2feature': {
-                    'edge_weight': g.edges['rev_cell2feature'].data['weight'].float()
-                }
-            })
-        logger.debug(f"{i} cell {h['cell'].abs().mean()} {h1['cell'].abs().mean()}")
-        logger.debug(f"{i} feature {h['feature'].abs().mean()} {h1['feature'].abs().mean()}")
-
-        h1['feature'] = (h1['feature'] -
-                         h1['feature'].mean()) / (h1['feature'].std() if h1['feature'].mean() != 0 else 1)
-        h1['cell'] = (h1['cell'] - h1['cell'].mean()) / (h1['cell'].std() if h1['cell'].mean() != 0 else 1)
-
-        h = {
-            'feature': h['feature'] * alpha + h1['feature'] * (1 - alpha),
-            'cell': h['cell'] * beta + h1['cell'] * (1 - beta)
-        }
-
-        h['feature'] = (h['feature'] - h['feature'].mean()) / h['feature'].std()
-        h['cell'] = (h['cell'] - h['cell'].mean()) / h['cell'].std()
-
-        hcell.append(h['cell'])
-
-    logger.debug(f"{hcell[-1].abs().mean()=}")
-    return hcell[1:]
-
-
 class ScMoGCNWrapper:
     """ScMoGCN class.
 
     Parameters
     ----------
     args : argparse.Namespace
-        A Namespace object that contains arguments of ScMoGCN. For details of parameters in parser args, please refer
-        to link (parser help document).
-    layers : List[List[Union[int, float]]]
-        Specification of hidden layers.
+        A Namespace object that contains arguments of ScMoGCN. For details of parameters in parser args, please refer to link (parser help document).
+    layers : list[int]
+        Specification of dimensions of hidden layers.
     temp : int optional
         Temperature for softmax, by default to be 1.
 
     """
 
     def __init__(self, args, layers, temp=1):
         self.model = ScMoGCN(args, layers, temp).to(args.device)
@@ -125,17 +66,14 @@
         -------
         self : ScMoGCNWrapper
             Converted model.
 
         """
         self.args.device = device
         self.model = self.model.to(device)
-        self.feat_mod1 = self.feat_mod1.to(device)
-        self.feat_mod2 = self.feat_mod2.to(device)
-        return self
 
     def load(self, path, map_location=None):
         """Load model parameters from checkpoint file.
 
         Parameters
         ----------
         path : str
@@ -149,76 +87,69 @@
 
         """
         if map_location is not None:
             self.model.load_state_dict(torch.load(path, map_location=map_location))
         else:
             self.model.load_state_dict(torch.load(path))
 
-    def fit(self, g_mod1, g_mod2, labels1, labels2, train_size):
-        """Fit function for training.
+    def fit(self, dataset, feats, labels):
+        """fit function for training.
 
         Parameters
         ----------
-        g_mod1 : dgl.DGLGraph
-            DGLGraph for modality 1.
-        g_mod2 : dgl.DGLGraph
-            DGLGraph for modality 2.
-        labels1 : torch.Tensor
-            Column-wise matching labels.
-        labels2 : torch.Tensor
-            Row-wise matching labels.
-        train_size : int
-            Number of training samples.
+        dataset : dance.datasets.multimodality.ModalityMatchingNIPSDataset
+            Dataset for mdality matching.
+        feats : torch.Tensor
+            Modality features.
 
         Returns
         -------
         None.
 
         """
 
         device = self.args.device
         wt = self.wt
-        hcell_mod1 = cell_feature_propagation(g_mod1, layers=self.args.layers, device=self.args.device)
-        hcell_mod2 = cell_feature_propagation(g_mod2, layers=self.args.layers, device=self.args.device)
-        self.feat_mod1 = hcell_mod1
-        self.feat_mod2 = hcell_mod2
+        hcell_mod1, hcell_mod2 = feats
+
+        labels0, labels1 = labels
 
         criterion = nn.CrossEntropyLoss()
         criterion2 = nn.MSELoss()
 
         assert wt[0].requires_grad == wt[1].requires_grad
         opt = optim.AdamW([{
             'params': self.model.parameters()
         }, {
             'params': wt[0]
         }, {
             'params': wt[1]
         }], lr=self.args.learning_rate)
 
-        # Make sure the batch size is small enough to cover all splits
-        BATCH_SIZE = min(4096, math.floor(train_size / 2))
+        BATCH_SIZE = 4096
 
-        idx = torch.randperm(train_size)
+        idx = torch.randperm(dataset.sparse_features()[0].shape[0])
         train_idx = idx[:-BATCH_SIZE]
         val_idx = idx[-BATCH_SIZE:]
-        test_idx = np.arange(train_size, hcell_mod1[0].shape[0])
+        test_idx = np.arange(dataset.sparse_features()[0].shape[0],
+                             dataset.sparse_features()[0].shape[0] + dataset.sparse_features()[2].shape[0])
         train_dataset = SimpleIndexDataset(train_idx)
         train_loader = DataLoader(
             dataset=train_dataset,
             batch_size=BATCH_SIZE,
             shuffle=True,
             num_workers=0,
             drop_last=True,
         )
 
         maxval = -1
         vals = []
         for epoch in range(self.args.epochs):
             self.model.train()
-            logger.info(f'epoch {epoch}')
+            print('epoch', epoch)
             total_loss = 0
             accum_acc = [0, 0]
 
             for step, batch_idx in enumerate(train_loader):
                 X, Y = propagation_layer_combination(hcell_mod1, hcell_mod2, batch_idx, wt[0], wt[1])
 
                 logits = self.model(X, Y)
@@ -242,118 +173,110 @@
                 if self.args.auxiliary_loss > 0:
                     loss = loss + loss2 + loss3
 
                 opt.zero_grad()
                 loss.backward()
                 opt.step()
 
-            logger.info('training loss: %.5f, forward: %.4f, backward: %.4f', total_loss / len(train_loader),
-                        accum_acc[0] / len(train_loader), accum_acc[1] / len(train_loader))
+            print('training loss: %.5f, foward: %.4f, backward: %.4f' %
+                  (total_loss / len(train_loader), accum_acc[0] / len(train_loader), accum_acc[1] / len(train_loader)))
 
             temp = torch.arange(val_idx.shape[0]).to(device)
-            vals.append(self.score(val_idx, labels1=temp, labels2=temp))
-            logger.info('validation score: %.5f', vals[-1])
+            vals.append(self.score([hcell_mod1, hcell_mod2], val_idx, [temp, temp]))
+            print('validation score: %.5f' % vals[-1])
             if epoch % 10 == 9:
-                logger.info('testing score: %.5f', self.score(test_idx, labels1=labels1, labels2=labels2))
+                print('testing score: %.5f' % self.score([hcell_mod1, hcell_mod2], test_idx, [labels0, labels1]))
 
             if vals[-1] > maxval:
                 maxval = vals[-1]
                 if not os.path.exists('models'):
                     os.mkdir('models')
                 torch.save(self.model.state_dict(), f'models/model_{self.args.rnd_seed}.pth')
                 weight_record = [wt[0].detach(), wt[1].detach()]
 
             if max(vals) != max(vals[-20:]):
-                logger.info('Early stopped.')
+                print('Early stopped.')
                 break
 
-        logger.info(f'Valid: {maxval}')
+        print('Valid: ', maxval)
 
         self.wt = weight_record
         return self
 
-    def predict(self, idx, enhance=False, batch1=None, batch2=None, threshold_quantile=0.95):
+    def predict(self, inputs, idx, enhance=False, dataset=None):
         """Predict function to get latent representation of data.
 
         Parameters
         ----------
+        inputs : list[torch.Tensor]
+            Multimodality features.
         idx : Iterable[int]
             Cell indices for prediction.
         enhance : bool optional
             Whether enable enhancement matching (e.g. bipartite matching), by default to be False.
-        batch1 : torch.Tensor optional
-            Batch labels of modality 1, by default to be None.
-        batch2 : torch.Tensor optional
-            Batch labels of modality 2, by default to be None.
-        threshold_quantile: float
-            Parameter for batch_separated_bipartite_matching when enhance is set to true, which controls the sparsity.
+        dataset : dance.datasets.multimodality.ModalityMatchingNIPSDataset optional
+            Dataset for modality matching, needed when enhance parameter set to be True.
 
         Returns
         -------
         pred : torch.Tensor
             Predicted matching matrix.
 
         """
         # inputs: [train_mod1, train_mod2], idx: valid_idx, labels: [sol, sol.T], wt: [wt0, wt1]
         self.model.eval()
 
         with torch.no_grad():
             wt = self.wt
-            m1, m2 = propagation_layer_combination(self.feat_mod1, self.feat_mod2, idx, wt[0], wt[1])
+            m1, m2 = propagation_layer_combination(inputs[0], inputs[1], idx, wt[0], wt[1])
 
             if not enhance:
                 pred = self.model(m1, m2)
                 return pred
 
             else:
                 emb1, emb2 = self.model.encode(m1, m2)
-                pred = batch_separated_bipartite_matching(batch1[idx], batch2[idx], emb1, emb2, threshold_quantile)
+                pred = batch_separated_bipartite_matching(dataset, emb1, emb2)
                 return pred
 
-    def score(self, idx, labels1=None, labels2=None, labels_matrix=None, enhance=False, batch1=None, batch2=None,
-              threshold_quantile=0.95):
+    def score(self, inputs, idx, labels, enhance=False, dataset=None):
         """Score function to get score of prediction.
 
         Parameters
         ----------
+        inputs : list[torch.Tensor]
+            Multimodality features.
         idx : Iterable[int]
             Index of testing cells for scoring.
-        labels1 : torch.Tensor
-            Column-wise matching labels.
-        labels2 : torch.Tensor
-            Row-wise matching labels.
-        labels_matrix: torch.Tensor
-            Matching labels.
+        labels : torch.Tensor
+            Ground truth label of cell matching matrix
         enhance : bool optional
             Whether enable enhancement matching (e.g. bipartite matching), by default to be False.
-        batch1 : torch.Tensor optional
-            Batch labels of modality 1, by default to be None.
-        batch2 : torch.Tensor optional
-            Batch labels of modality 2, by default to be None.
-        threshold_quantile: float
-            Parameter for batch_separated_bipartite_matching when enhance is set to true, which controls the sparsity.
+        dataset : dance.datasets.multimodality.ModalityMatchingNIPSDataset optional
+            Dataset for modality matching, needed when enhance parameter set to be True.
 
         Returns
         -------
         score : float
             Accuracy of predicted matching between two modalities.
 
         """
 
         if not enhance:
 
-            logits = self.predict(idx, enhance, batch1, batch2)
-            backward_accuracy = (torch.argmax(logits, dim=0) == labels1).float().mean().item()
-            forward_accuracy = (torch.argmax(logits, dim=1) == labels2).float().mean().item()
+            logits = self.predict(inputs, idx, enhance, dataset)
+            forward_accuracy = (torch.argmax(logits, dim=1) == labels[1]).float().mean().item()
+            backward_accuracy = (torch.argmax(logits, dim=0) == labels[0]).float().mean().item()
+
             return (forward_accuracy + backward_accuracy) / 2
 
         else:
 
-            matrix = self.predict(idx, enhance, batch1, batch2, threshold_quantile)
-            score = (matrix * labels_matrix.numpy()).sum() / labels_matrix.shape[0]
+            matrix = self.predict(inputs, idx, enhance, dataset)
+            score = (matrix * labels.numpy()).sum() / labels.shape[0]
 
             return score
 
 
 class ScMoGCN(nn.Module):
 
     def __init__(self, args, layers, temp=1):
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/predict_modality/babel.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/predict_modality/babel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """Reimplementation of BABEL method.
 
 Extended from https://github.com/wukevin/babel
 
 Reference
 ---------
-Wu, Kevin E., Kathryn E. Yost, Howard Y. Chang, and James Zou. "BABEL enables cross-modality translation between
-multiomic profiles at single-cell resolution." Proceedings of the National Academy of Sciences 118, no. 15 (2021).
+Wu, Kevin E., Kathryn E. Yost, Howard Y. Chang, and James Zou. "BABEL enables cross-modality translation between multiomic profiles at single-cell resolution." Proceedings of the National Academy of Sciences 118, no. 15 (2021).
 
 """
+import functools
+import logging
 import math
+import os
+import sys
 from typing import Callable, List, Tuple, Union
 
+import numpy as np
+import skorch
+import skorch.utils
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+from scipy import sparse
 from torch.utils.data import DataLoader
 
 import dance.utils.loss as loss_functions
-from dance import logger
 
 REDUCE_LR_ON_PLATEAU_PARAMS = {
     "mode": "min",
     "factor": 0.1,
     "patience": 10,
     "min_lr": 1e-6,
 }
@@ -142,24 +148,26 @@
             return mu_scaled, theta
 
     def forward_with_decode(self, x, size_factors):
         """Return the parameters mu, theta, and pi The denoised matrix is generated by
         replacing the original count values with the mean of the negative binomial
         component as predicted in the output layer.
 
-        This matrix represents the denoised and library size normalized expression
-        matrix, the final output of the method.
+        This matrix represents the denoised and library size normalized expression matrix, the final output of the
+        method.
 
         """
         return self.decode(self.encode(x), size_factors)
 
     def forward_no_decode(self, x, _size_factors):
-        """Return the hidden representation instead of decoding it as well Useful for
-        probing the latent dimension using pytorch_eval Use by setting model.forward =
-        model.forward_no_decode."""
+        """
+        Return the hidden representation instead of decoding it as well
+        Useful for probing the latent dimension using pytorch_eval
+        Use by setting model.forward = model.forward_no_decode
+        """
         return self.encode(x)
 
 
 class Encoder(nn.Module):
 
     def __init__(self, num_inputs: int, num_units=32, activation=nn.PReLU):
         super().__init__()
@@ -218,15 +226,15 @@
                     self.final_activations[f"act{i+1}"] = act
             elif isinstance(final_activation, nn.Module):
                 self.final_activations["act1"] = final_activation
             else:
                 raise ValueError(f"Unrecognized type for final_activation: {type(final_activation)}")
 
     def forward(self, x, size_factors=None):
-        """Include size factor here because we may want to scale the output by that."""
+        """include size factor here because we may want to scale the output by that."""
         x = self.act1(self.bn1(self.decode1(x)))
 
         retval1 = self.decode21(x)  # This is invariably the counts
         if "act1" in self.final_activations.keys():
             retval1 = self.final_activations["act1"](retval1)
         if size_factors is not None:
             sf_scaled = size_factors.view(-1, 1).repeat(1, retval1.shape[1])
@@ -311,15 +319,15 @@
                     if act is None:
                         continue
                     self.final_activations[f"act{i+1}"] = act
             elif isinstance(final_activations, nn.Module):
                 self.final_activations["act1"] = final_activations
             else:
                 raise ValueError(f"Unrecognized type for final_activation: {type(final_activations)}")
-        logger.info(f"ChromDecoder with {len(self.final_activations)} output activations")
+        logging.info(f"ChromDecoder with {len(self.final_activations)} output activations")
 
         self.final_decoders = nn.ModuleList()  # List[List[Module]]
         for n in self.num_outputs:
             layer0 = nn.Linear(16, 32)
             nn.init.xavier_uniform_(layer0.weight)
             bn0 = nn.BatchNorm1d(32)
             act0 = activation()
@@ -424,15 +432,15 @@
 
     def __init__(self, model1, model2):
         super().__init__()
         self.model1 = model1
         self.model2 = model2
 
     def forward(self, x):
-        """X is expected to be a tuple of two inputs."""
+        """x is expected to be a tuple of two inputs."""
         x1, x2 = x
         y1 = self.model1(x1)
         y2 = self.model2(x2)
         return (y1, y2)
 
     def translate_1_to_2(self, encoded1):
         """Given data from domain 1 output domain 2."""
@@ -694,36 +702,155 @@
 
     def split_catted_input(self, x):
         """Split the input into chunks that goes to each input to model."""
         a, b = torch.split(x, [self.input_dim1, sum(self.input_dim2)], dim=-1)
         return (a, torch.split(b, self.input_dim2, dim=-1))
 
 
+class PairedAutoEncoderSkorchNet(skorch.NeuralNet):
+
+    def forward_iter(self, X, training=False, device="cpu"):
+        """Subclassed to work with tuples."""
+        dataset = self.get_dataset(X)
+        iterator = self.get_iterator(dataset, training=training)
+        for i, data in enumerate(iterator):
+            Xi = skorch.dataset.unpack_data(data)[0]
+            with torch.set_grad_enabled(training):
+                self.module_.train(training)
+                yp = self.infer(Xi)
+
+            if isinstance(yp, tuple):
+                yield recursive_to_device(yp)  # <- modification here
+            else:
+                yield yp.to(device)
+
+    def predict_proba(self, x):
+        """Subclassed so calling predict produces a tuple of outputs."""
+        y_probas1, y_probas2 = [], []
+        for yp in self.forward_iter(x, training=False):
+            assert isinstance(yp, tuple)
+            yp1 = yp[0][0]
+            yp2 = yp[1][0]
+            y_probas1.append(skorch.utils.to_numpy(yp1))
+            y_probas2.append(skorch.utils.to_numpy(yp2))
+        y_proba1 = np.concatenate(y_probas1, 0)
+        y_proba2 = np.concatenate(y_probas2, 0)
+        return y_proba1, y_proba2
+
+    def get_encoded_layer(self, x):
+        """Get the encoded representation as a TUPLE of two elements."""
+        encoded1, encoded2 = [], []
+        for out1, out2, *_other in self.forward_iter(x, training=False):
+            encoded1.append(out1[-1])
+            encoded2.append(out2[-1])
+        return np.concatenate(encoded1, axis=0), np.concatenate(encoded2, axis=0)
+
+    def translate_1_to_2(self, x):
+        enc1, enc2 = self.get_encoded_layer(x)
+        device = next(self.module_.parameters()).device
+        enc1_torch = torch.from_numpy(enc1).to(device)
+        return self.module_.translate_1_to_2(enc1_torch)[0].detach().cpu().numpy()
+
+    def translate_2_to_1(self, x):
+        enc1, enc2 = self.get_encoded_layer(x)
+        device = next(self.module_.parameters()).device
+        enc2_torch = torch.from_numpy(enc2).to(device)
+        return self.module_.translate_2_to_1(enc2_torch)[0].detach().cpu().numpy()
+
+
+class SplicedAutoEncoderSkorchNet(PairedAutoEncoderSkorchNet):
+    """Skorch wrapper for the SplicedAutoEncoder above.
+
+    Mostly here to take care of how we calculate loss
+
+    """
+
+    def predict_proba(self, x):
+        """Subclassed so that calling predict produces a tuple of 4 outputs."""
+        y_probas1, y_probas2, y_probas3, y_probas4 = [], [], [], []
+        for yp in self.forward_iter(x, training=False):
+            assert isinstance(yp, tuple)
+            yp1 = yp[0][0]
+            yp2 = yp[1][0]
+            yp3 = yp[2][0]
+            yp4 = yp[3][0]
+            y_probas1.append(skorch.utils.to_numpy(yp1))
+            y_probas2.append(skorch.utils.to_numpy(yp2))
+            y_probas3.append(skorch.utils.to_numpy(yp3))
+            y_probas4.append(skorch.utils.to_numpy(yp4))
+        y_proba1 = np.concatenate(y_probas1)
+        y_proba2 = np.concatenate(y_probas2)
+        y_proba3 = np.concatenate(y_probas3)
+        y_proba4 = np.concatenate(y_probas4)
+        # Order: 1to1, 1to2, 2to1, 2to2
+        return y_proba1, y_proba2, y_proba3, y_proba4
+
+    def get_encoded_layer(self, x):
+        """Get the encoded representation as a TUPLE of two elements."""
+        encoded1, encoded2 = [], []
+        for out11, out12, out21, out22 in self.forward_iter(x, training=False):
+            encoded1.append(out11[-1])
+            encoded2.append(out22[-1])
+        return np.concatenate(encoded1, axis=0), np.concatenate(encoded2, axis=0)
+
+    def translate_1_to_1(self, x) -> sparse.csr_matrix:
+        retval = [sparse.csr_matrix(skorch.utils.to_numpy(yp[0][0])) for yp in self.forward_iter(x, training=False)]
+        return sparse.vstack(retval)
+
+    def translate_1_to_2(self, x) -> sparse.csr_matrix:
+        retval = [sparse.csr_matrix(skorch.utils.to_numpy(yp[1][0])) for yp in self.forward_iter(x, training=False)]
+        return sparse.vstack(retval)
+
+    def translate_2_to_1(self, x) -> sparse.csr_matrix:
+        retval = [sparse.csr_matrix(skorch.utils.to_numpy(yp[2][0])) for yp in self.forward_iter(x, training=False)]
+        return sparse.vstack(retval)
+
+    def translate_2_to_2(self, x) -> sparse.csr_matrix:
+        retval = [sparse.csr_matrix(skorch.utils.to_numpy(yp[3][0])) for yp in self.forward_iter(x, training=False)]
+        return sparse.vstack(retval)
+
+    def score(self, true, pred):
+        return self.get_loss(pred, true)
+
+
+class PairedInvertibleAutoEncoderSkorchNet(PairedAutoEncoderSkorchNet):
+
+    def translate_1_to_2(self, x):
+        enc1, enc2 = self.get_encoded_layer(x)
+        device = next(self.module_.parameters()).device
+        enc1_torch = torch.from_numpy(enc1).to(device)
+        return self.module_.translate_1_to_2(enc1_torch)[0].detach().cpu().numpy()
+
+    def translate_2_to_1(self, x):
+        enc1, enc2 = self.get_encoded_layer(x)
+        device = next(self.module_.parameters()).device
+        enc2_torch = torch.from_numpy(enc2).to(device)
+        return self.module_.translate_2_to_1(enc2_torch)[0].detach().cpu().numpy()
+
+
+# BabelWrapper = SplicedAutoEncoderSkorchNet
 class BabelWrapper:
     """Babel class.
 
     Parameters
     ----------
     args : argparse.Namespace
-        A Namespace object that contains arguments of Babel. For details of parameters in parser args, please refer to
-        link (parser help document).
-    dim_in : int
-        Input dimension.
-    dim_out: int
-        Output dimension.
+        A Namespace object that contains arguments of Babel. For details of parameters in parser args, please refer to link (parser help document).
+    dataset : dance.datasets.multimodality.ModalityPredictionDataset
+        Modality prediction dataset.
 
     """
 
-    def __init__(self, args, dim_in, dim_out):
+    def __init__(self, args, dataset):
         self.args = args
         model_class = (NaiveSplicedAutoEncoder if args.naive else AssymSplicedAutoEncoder)
         self.model = model_class(
             hidden_dim=args.hidden,
-            input_dim1=dim_in,
-            input_dim2=[dim_out],
+            input_dim1=dataset.modalities[0].shape[1],
+            input_dim2=[dataset.modalities[1].shape[1]],
             final_activations1=nn.ReLU(),
             final_activations2=nn.ReLU(),
             flat_mode=True,
             seed=args.rnd_seed,
         ).to(args.device)
 
     def to(self, device):
@@ -787,68 +914,81 @@
                 emb = self.model.model12[0](test_mod1.to(self.args.device))
                 pred = self.model.model12[1](emb)[0]
             else:
                 emb = self.model.encoder1(test_mod1.to(self.args.device))
                 pred = self.model.decoder2(emb)[0]
             return pred
 
-    def fit(self, x_train, y_train, max_epochs=500, val_ratio=0.15):
-        """Fit function for training.
+    def fit(self, train_dual, valid_dual, max_epochs=500):
+        """fit function for training.
 
         Parameters
         ----------
-        x_train : torch.Tensor
-            Training input modality.
-        y_train : torch.Tensor
-            Training output modality.
+        train_dual : dance.utils.PairedDataset
+            Training dataset.
+        valid_dual : dance.utils.PairedDataset
+            Validation dataset.
         max_epochs : int optional
             Maximum number of training epochs, by default to be 500.
-        val_ratio : int
-            Validation ratio.
+
+        Returns
+        -------
+        None.
 
         """
+
+        #TODO: add callbacks
+        # callbacks = [
+        #                 skorch.callbacks.EarlyStopping(patience=self.args.earlystop),
+        #                 skorch.callbacks.GradientNormClipping(gradient_clip_value=5),
+        #             ],
+        # train_dual = sc_dual_train_dataset
+        # valid_dual = sc_dual_valid_dataset
         criterion = loss_functions.QuadLoss(loss1=loss_functions.RMSELoss, loss2=loss_functions.RMSELoss,
                                             loss2_weight=self.args.lossweight)
         device = self.args.device
 
-        total_size = x_train.shape[0]
-        val_size = int(total_size * val_ratio)
-        rand_idx = torch.randperm(total_size)
-        train_idx = rand_idx[:-val_size]
-        val_idx = rand_idx[-val_size:]
-
-        train_loader = DataLoader(torch.hstack((x_train[train_idx], y_train[train_idx])), shuffle=True,
-                                  batch_size=self.args.batchsize)
-        val_loader = DataLoader(torch.hstack((x_train[val_idx], y_train[val_idx])), batch_size=self.args.batchsize)
         optimizer = torch.optim.Adam(self.model.parameters(), lr=self.args.lr)
+        train_loader = DataLoader(
+            dataset=train_dual,
+            batch_size=self.args.batchsize,
+            shuffle=True,
+            num_workers=1,
+        )
+        valid_loader = DataLoader(
+            dataset=valid_dual,
+            batch_size=len(valid_dual),
+            shuffle=False,
+            num_workers=1,
+        )
 
         val = []
         for i in range(max_epochs):
             self.model.train()
             total_loss = 0
-            for train_batch in train_loader:
-                logits = self.model(train_batch.to(device))
-                loss = criterion(logits, train_batch.to(device))
+            for idx, data in enumerate(train_loader):
+                logits = self.model(data[0].to(device))
+                loss = criterion(logits, data[1].to(device))
                 total_loss += loss.item()
 
                 optimizer.zero_grad()
                 loss.backward()
 
                 nn.utils.clip_grad_norm_(self.model.parameters(), 5)
                 optimizer.step()
 
             mse = nn.MSELoss()
             self.model.eval()
 
             with torch.no_grad():
                 loss = 0
-                for val_batch in val_loader:
-                    logits = self.model(val_batch.to(device))
-                    loss += mse(logits[1][0], val_batch[:, -logits[1][0].shape[1]:].to(device)).item()
-            val.append(math.sqrt(loss / len(val_loader)))
+                for _, data in enumerate(valid_loader):
+                    logits = self.model(data[0].to(device))
+                    loss += mse(logits[1][0], data[1][:, -logits[1][0].shape[1]:].to(device)).item()
+            val.append(math.sqrt(loss / len(valid_loader)))
             print('epoch: ', i + 1)
             print('training (sum of 4 losses):', total_loss / len(train_loader))
             print('validation (prediction loss):', val[-1])
 
             if min(val) == val[-1]:
                 torch.save(self.model.state_dict(), f'{self.args.outdir}/BABEL_best_{self.args.rnd_seed}.pth')
             if i > self.args.earlystop and min(val) != min(val[-self.args.earlystop:]):
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/predict_modality/cmae.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/predict_modality/cmae.py`

 * *Files 3% similar despite different names*

```diff
@@ -395,14 +395,25 @@
         if variational:
             h_a = h_a + n_a
             h_b = h_b + n_b
 
         x_a_recon = self.gen_a.decode(h_a)
         x_b_recon = self.gen_b.decode(h_b)
 
+        # decode (cross domain)
+        x_ba = self.gen_a.decode(h_b)
+        x_ab = self.gen_b.decode(h_a)
+        # encode again
+        h_b_recon, n_b_recon = self.gen_a.encode(x_ba)
+        h_a_recon, n_a_recon = self.gen_b.encode(x_ab)
+        # decode again (if needed)
+        if variational:
+            h_a_recon = h_a_recon + n_a_recon
+            h_b_recon = h_b_recon + n_b_recon
+
         classes_a = self.classifier.forward(h_a)
         classes_b = self.classifier.forward(h_b)
 
         # reconstruction loss
         self.loss_gen_recon_x_a = self._mae_loss(x_a_recon, x_a)
         self.loss_gen_recon_x_b = self._mae_loss(x_b_recon, x_b)
 
@@ -534,40 +545,38 @@
                 'a': self.gen_a.state_dict(),
                 'b': self.gen_b.state_dict(),
                 "classifier": self.classifier.state_dict()
             }, gen_name)
         torch.save({'latent': self.dis_latent.state_dict()}, dis_name)
         torch.save({'gen': self.gen_opt.state_dict(), 'dis': self.dis_opt.state_dict()}, opt_name)
 
-    def fit(self, train_mod1, train_mod2, aux_labels=None, checkpoint_directory='./checkpoint', val_ratio=0.15):
+    def fit(self, train_mod1, train_mod2, aux_labels=None, checkpoint_directory='./checkpoint'):
         """Train CMAE.
 
         Parameters
         ----------
         train_mod1 : torch.Tensor
             Features of input modality.
         train_mod2 : torch.Tensor
             Features of target modality.
         aux_labels : torch.Tensor optional
             Auxiliary labels for extra supervision during training.
         checkpoint_directory : str optional
             Path to the checkpoint file, by default to be './checkpoint'.
-        val_ratio : float
-            Ratio for automatic train-validation split.
 
         Returns
         -------
         None.
 
         """
 
         hyperparameters = self.hyperparameters
         idx = torch.randperm(train_mod1.shape[0])
-        train_idx = idx[:int(idx.shape[0] * (1 - val_ratio))]
-        val_idx = idx[int(idx.shape[0] * (1 - val_ratio)):]
+        train_idx = idx[:int(idx.shape[0] * 0.85)]
+        val_idx = idx[int(idx.shape[0] * 0.85):]
 
         train_dataset = SimpleIndexDataset(train_idx)
         train_loader = DataLoader(
             dataset=train_dataset,
             batch_size=hyperparameters['batch_size'],
             shuffle=True,
             num_workers=0,
@@ -579,25 +588,25 @@
                                  hyperparameters=hyperparameters) if hyperparameters['resume'] else 0
         num_disc = 1 if "num_disc" not in hyperparameters else hyperparameters["num_disc"]
         num_gen = 1 if "num_gen" not in hyperparameters else hyperparameters["num_gen"]
 
         while True:
             print('Iteration: ', iterations)
             for it, batch_idx in enumerate(train_loader):
+                self._update_learning_rate()
                 mod1, mod2 = train_mod1[batch_idx], train_mod2[batch_idx]
 
                 for _ in range(num_disc):
                     self._dis_update(mod1, mod2, hyperparameters)
                 for _ in range(num_gen):
                     if aux_labels is not None:
                         self._gen_update(mod1, mod2, mod1, mod2, hyperparameters, aux_labels[batch_idx],
                                          aux_labels[batch_idx], variational=False)
                     else:
                         self._gen_update(mod1, mod2, mod1, mod2, hyperparameters, variational=False)
-                self._update_learning_rate()
 
             print('RMSE Loss:', self.score(train_mod1[val_idx], train_mod2[val_idx]))
 
             iterations += 1
             if iterations >= hyperparameters['max_epochs']:
                 print('Finish training')
                 break
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/predict_modality/scmm.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/predict_modality/scmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,54 +489,48 @@
             qz_xs, _, _ = self.forward(data)
             if not sampling:
                 lats = [get_mean(qz_x) for qz_x in qz_xs]
             else:
                 lats = [qz_x._sample() for qz_x in qz_xs]
         return lats
 
-    def fit(self, x_train, y_train, val_ratio=0.15):
-        """Fit function for training.
+    def fit(self, dataset):
+        """fit function for training.
 
         Parameters
         ----------
-        x_train : torch.Tensor
-            Input modality for training.
-
-        y_train : torch.Tensor
-            Target modality for training.
-
-        val_ratio : float
-            Ratio for automatic train-validation split.
+        dataset : dance.datasets.multimodality.ModalityPredictionDataset
+            Dataset for modality prediction.
 
         Returns
         -------
         None.
 
         """
 
         start_early_stop = self.params.deterministic_warmup
 
-        idx = np.random.permutation(x_train.shape[0])
-        train_idx = idx[:int(idx.shape[0] * (1 - val_ratio))]
-        val_idx = idx[int(idx.shape[0] * (1 - val_ratio)):]
+        idx = np.random.permutation(dataset.modalities[0].shape[0])
+        train_idx = idx[:int(idx.shape[0] * 0.85)]
+        val_idx = idx[int(idx.shape[0] * 0.85):]
 
         optimizer = optim.Adam(filter(lambda p: p.requires_grad, self.parameters()), lr=self.params.lr, amsgrad=True)
         assert (self.params.obj in ['m_elbo_naive', 'm_elbo_naive_warmup'])
         objective = m_elbo_naive_warmup if self.params.obj == 'm_elbo_naive_warmup' else 'm_elbo_naive'
         train_dataset = SimpleIndexDataset(train_idx)
         train_loader = DataLoader(
             dataset=train_dataset,
             batch_size=self.params.batch_size,
             shuffle=True,
             num_workers=0,
             drop_last=True,
         )
 
-        train_mod1 = x_train.float().to(self.params.device)
-        train_mod2 = y_train.float().to(self.params.device)
+        train_mod1 = torch.from_numpy(dataset.numpy_features(0, True)).float().to(self.params.device)
+        train_mod2 = torch.from_numpy(dataset.numpy_features(1, True)).float().to(self.params.device)
         self.ratio = train_mod2.sum() / train_mod1.sum()
         vals = []
         tr = []
 
         for epoch in range(1, self.params.epochs + 1):
             self.train()
             b_loss = 0
@@ -591,17 +585,15 @@
         Returns
         -------
         score : float
             Score of predicted matching, according to specified metric.
 
         """
         self.eval()
-        self.eval()
-        X = X.float().to(self.params.device)
-        Y = Y.float().to(self.params.device)
+
         if metric == 'loss':
             b_loss = 0
             idx = np.arange(X.shape[0])
             dataset = SimpleIndexDataset(idx)
             data_loader = DataLoader(
                 dataset=dataset,
                 batch_size=self.params.batch_size,
@@ -621,14 +613,15 @@
             pred = self.preprocessing(pred_test)
             pred = torch.nan_to_num(pred)
             label = self.preprocessing(Y)
             return math.sqrt(mse(pred, label).item())
         else:
             print('Warning: undefined evaluation metric.')
 
+    #TODO: predict function need to be modified to remove label input
     def predict(self, X):
         """Score function to get score of prediction.
 
         Parameters
         ----------
         X : torch.Tensor
             Features of input modality and target modality.
@@ -636,15 +629,14 @@
         Returns
         -------
         pred : torch.Tensor
             Prediction of target modality from input modality.
 
         """
         self.eval()
-        X = X.float().to(self.params.device)
         idx = np.arange(X.shape[0])
         dataset = SimpleIndexDataset(idx)
         data_loader = DataLoader(
             dataset=dataset,
             batch_size=self.params.batch_size * 10,
             shuffle=False,
             num_workers=0,
```

### Comparing `pydance-1.0.0/dance/modules/multi_modality/predict_modality/scmogcn.py` & `pydance-1.0.0rc0/dance/modules/multi_modality/predict_modality/scmogcn.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
 
     def __init__(self, args):
         super().__init__()
         self.args = args
         self.model = ScMoGCN(args).to(args.device)
 
-    def predict(self, graph, idx=None, device='cpu'):
+    def predict(self, graph, idx=None, device='gpu'):
         """Predict function to get latent representation of data.
 
         Parameters
         ----------
         graph : dgl.DGLGraph
             Cell-feature graph contructed from the dataset.
         idx : Iterable[int] optional
@@ -60,17 +60,18 @@
             model = self.model
         model.eval()
         with torch.no_grad():
             if idx is None:
                 pred = model.forward(graph)
             else:
                 pred = model.forward(graph)[idx]
-        return pred.to(device)
+        pred = pred.to(self.args.device)
+        return pred
 
-    def score(self, g, idx, labels, device='cpu'):
+    def score(self, g, idx, labels, device='gpu'):
         """Score function to get score of prediction.
 
         Parameters
         ----------
         g : dgl.DGLGraph
             Cell-feature graph contructed from the dataset.
         idx : Iterable[int] optional
@@ -90,16 +91,16 @@
         with torch.no_grad():
             logits = F.relu(self.predict(g, idx, device))
             loss = math.sqrt(F.mse_loss(logits, labels).item())
             return loss
 
     # TODO: need to modify the logic of validation and test to adapt Inductive learning;
     #  w. test = Transductive learning, w/o = Inductive learning
-    def fit(self, g, y, split=None, eval=True, verbose=2, y_test=None, logger=None, sampling=False, eval_interval=1):
-        """Fit function for training.
+    def fit(self, g, y, split=None, eval=True, verbose=2, y_test=None, logger=None, sampling=False):
+        """fit function for training.
 
         Parameters
         ----------
         g : dgl.DGLGraph
             Cell-feature graph contructed from the dataset.
         y : torch.Tensor
             Labels of each training cell, a.k.a target modality features.
@@ -124,32 +125,29 @@
         if sampling:
             return self.fit_with_sampling(g, y, split, eval, verbose, y_test, logger)
         kwargs = vars(self.args)
         PREFIX = kwargs['prefix']
         CELL_SIZE = kwargs['CELL_SIZE']
         TRAIN_SIZE = kwargs['TRAIN_SIZE']
 
-        g = g.to(self.args.device)
-        y = y.float().to(self.args.device)
-        y_test = y_test.float().to(self.args.device) if y_test is not None else None
-
         if verbose > 1 and logger is None:
             logger = open(f'{kwargs["log_folder"]}/{PREFIX}.log', 'w')
         if verbose > 1:
             logger.write(str(self.model) + '\n')
             logger.flush()
 
         opt = torch.optim.AdamW(self.model.parameters(), lr=kwargs['learning_rate'],
                                 weight_decay=kwargs['weight_decay'])
         criterion = nn.MSELoss()
         val = []
         tr = []
         te = []
         minval = 100
         minvep = -1
+        BATCH_SIZE = kwargs['batch_size']
 
         for epoch in range(kwargs['epoch']):
             if verbose > 1:
                 logger.write(f'epoch:  {epoch}\n')
 
             self.model.train()
             logits = self.model(g)
@@ -159,50 +157,49 @@
             opt.zero_grad()
             loss.backward()
             opt.step()
 
             torch.cuda.empty_cache()
             tr.append(math.sqrt(running_loss))
 
-            if epoch % eval_interval == 0:
-                val.append(self.score(g, split['valid'], y[split['valid']], self.args.device))
+            val.append(self.score(g, split['valid'], y[split['valid']]))
+            if verbose > 1:
+                logger.write(f'training loss:  {tr[-1]}\n')
+                logger.flush()
+                logger.write(f'validation loss:  {val[-1]}\n')
+                logger.flush()
+
+            if eval:
+                te.append(self.score(g, np.arange(TRAIN_SIZE, CELL_SIZE), y_test))
                 if verbose > 1:
-                    logger.write(f'training loss:  {tr[-1]}\n')
-                    logger.flush()
-                    logger.write(f'validation loss:  {val[-1]}\n')
+                    logger.write(f'testing loss:  {te[-1]}\n')
                     logger.flush()
 
+            if val[-1] < minval:
+                minval = val[-1]
+                minvep = epoch
+                if kwargs['save_best']:
+                    torch.save(self.model, f'{kwargs["model_folder"]}/{PREFIX}.best.pth')
+
+            if epoch > 1500 and kwargs['early_stopping'] > 0 and min(val[-kwargs['early_stopping']:]) > minval:
+                if verbose > 1:
+                    logger.write('Early stopped.\n')
+                break
+
+            if epoch > 1200:
+                if epoch % 15 == 0:
+                    for p in opt.param_groups:
+                        p['lr'] *= kwargs['lr_decay']
+
+            if verbose > 0:
+                print('epoch', epoch)
+                print('training: ', tr[-1])
+                print('valid: ', val[-1])
                 if eval:
-                    te.append(self.score(g, np.arange(TRAIN_SIZE, CELL_SIZE), y_test, self.args.device))
-                    if verbose > 1:
-                        logger.write(f'testing loss:  {te[-1]}\n')
-                        logger.flush()
-
-                if val[-1] < minval:
-                    minval = val[-1]
-                    minvep = epoch // eval_interval
-                    if kwargs['save_best']:
-                        torch.save(self.model, f'{kwargs["model_folder"]}/{PREFIX}.best.pth')
-
-                if epoch > 1500 and kwargs['early_stopping'] > 0 and min(val[-kwargs['early_stopping']:]) > minval:
-                    if verbose > 1:
-                        logger.write('Early stopped.\n')
-                    break
-
-                if epoch > 1200:
-                    if epoch % 15 == 0:
-                        for p in opt.param_groups:
-                            p['lr'] *= kwargs['lr_decay']
-
-                if verbose > 0:
-                    print('epoch', epoch)
-                    print('training: ', tr[-1])
-                    print('valid: ', val[-1])
-                    if eval:
-                        print('testing: ', te[-1])
+                    print('testing: ', te[-1])
 
         if kwargs['save_final']:
             state = {'model': self.model, 'optimizer': opt.state_dict(), 'epoch': epoch - 1}
             torch.save(state, f'{kwargs["model_folder"]}/{PREFIX}.epoch{epoch}.pth')
 
         if verbose > 1:
             if eval:
@@ -210,20 +207,20 @@
                     f'epoch {minvep} minimal val {minval} with training:  {tr[minvep]} and testing: {te[minvep]}\n')
             else:
                 logger.write(f'epoch {minvep} minimal val {minval} with training:  {tr[minvep]}\n')
             logger.close()
 
         if verbose > 0 and eval:
             print('min testing', min(te), te.index(min(te)))
-            print('converged testing', minvep * eval_interval, te[minvep])
+            print('converged testing', minvep, te[minvep])
 
         return self.model
 
-    def fit_with_sampling(self, g, y, split=None, eval=True, verbose=2, y_test=None, logger=None, eval_interval=1):
-        """Fit function for training with graph sampling.
+    def fit_with_sampling(self, g, y, split=None, eval=True, verbose=2, y_test=None, logger=None):
+        """fit function for training with graph sampling.
 
         Parameters
         ----------
         g : dgl.DGLGraph
             Cell-feature graph contructed from the dataset.
         y : torch.Tensor
             Labels of each training cell, a.k.a target modality features.
@@ -243,16 +240,15 @@
         None.
 
         """
         kwargs = vars(self.args)
         PREFIX = kwargs['prefix']
         CELL_SIZE = kwargs['CELL_SIZE']
         TRAIN_SIZE = kwargs['TRAIN_SIZE']
-        # Make sure the batch size is small enough to cover all splits
-        BATCH_SIZE = min(kwargs['batch_size'], min(map(len, split.values())))
+        BATCH_SIZE = kwargs['batch_size']
 
         if verbose > 1 and logger is None:
             logger = open(f'{kwargs["log_folder"]}/{PREFIX}.log', 'w')
         if verbose > 1:
             logger.write(str(self.model) + '\n')
             logger.flush()
         g.nodes['cell'].data['label'] = torch.cat([y, y_test], 0)
@@ -316,26 +312,24 @@
 
             # for input_nodes, output_nodes, blocks in dataloader:
 
             self.model.train()
             for i, batch_idx in enumerate(dataloader):
                 # feature_sampled = np.random.choice(g.nodes('feature'), 0.5*len(g.nodes('feature'), replace=False),
                 #                  p=feature_weight)
-                if self.args.node_sampling_rate < 1:
-                    feature_sampled = torch.multinomial(feature_weight,
-                                                        int(self.args.node_sampling_rate * len(g.nodes('feature'))),
-                                                        replacement=False)
-                else:
-                    feature_sampled = torch.arange(len(g.nodes('feature')))
+                feature_sampled = torch.multinomial(feature_weight,
+                                                    int(self.args.node_sampling_rate * len(g.nodes('feature'))),
+                                                    replacement=False).to(self.args.device)
+                # feature_sampled = g.nodes('feature')[feature_sampled]
                 subgraph = dgl.node_subgraph(g, {
-                    'cell': batch_idx,
-                    'feature': feature_sampled,
-                }).to(self.args.device)  # XXX: bottlenect
+                    'cell': batch_idx.to(self.args.device),
+                    'feature': feature_sampled
+                })  # g.nodes('feature')})
                 logits = self.model(subgraph)
-                output_labels = subgraph.nodes['cell'].data['label'].float()
+                output_labels = subgraph.nodes['cell'].data['label']
 
                 # blocks = [b.to(torch.device(self.args.device)) for b in blocks]
                 # logits = self.model(blocks, sampled = True)
 
                 # output_labels = blocks[-1].dstdata['label']['cell']
 
                 loss = criterion(logits, output_labels)
@@ -348,51 +342,50 @@
 
                 del subgraph
                 del output_labels
                 del loss
                 torch.cuda.empty_cache()
             tr.append(math.sqrt(running_loss / len(dataloader)))
 
-            if epoch % eval_interval == 0:
-                val.append(self.score(g_origin, split['valid'], y[split['valid']], 'cpu'))
+            val.append(self.score(g_origin, split['valid'], y[split['valid']], 'cpu'))
 
+            if verbose > 1:
+                logger.write(f'training loss:  {tr[-1]}\n')
+                logger.flush()
+                logger.write(f'validation loss:  {val[-1]}\n')
+                logger.flush()
+
+            if eval:
+                te.append(self.score(g_origin, np.arange(TRAIN_SIZE, CELL_SIZE), y_test, 'cpu'))
                 if verbose > 1:
-                    logger.write(f'training loss:  {tr[-1]}\n')
-                    logger.flush()
-                    logger.write(f'validation loss:  {val[-1]}\n')
+                    logger.write(f'testing loss:  {te[-1]}\n')
                     logger.flush()
 
+            if val[-1] < minval:
+                minval = val[-1]
+                minvep = epoch
+                if kwargs['save_best']:
+                    torch.save(self.model, f'{kwargs["model_folder"]}/{PREFIX}.best.pth')
+
+            if epoch > 1500 and kwargs['early_stopping'] > 0 and min(val[-kwargs['early_stopping']:]) > minval:
+                if verbose > 1:
+                    logger.write('Early stopped.\n')
+                break
+
+            if epoch > 1200:
+                if epoch % 15 == 0:
+                    for p in opt.param_groups:
+                        p['lr'] *= kwargs['lr_decay']
+
+            if verbose > 0:
+                print('epoch', epoch)
+                print('training: ', tr[-1])
+                print('valid: ', val[-1])
                 if eval:
-                    te.append(self.score(g_origin, np.arange(TRAIN_SIZE, CELL_SIZE), y_test, 'cpu'))
-                    if verbose > 1:
-                        logger.write(f'testing loss:  {te[-1]}\n')
-                        logger.flush()
-
-                if val[-1] < minval:
-                    minval = val[-1]
-                    minvep = epoch // eval_interval
-                    if kwargs['save_best']:
-                        torch.save(self.model, f'{kwargs["model_folder"]}/{PREFIX}.best.pth')
-
-                if epoch > 1500 and kwargs['early_stopping'] > 0 and min(val[-kwargs['early_stopping']:]) > minval:
-                    if verbose > 1:
-                        logger.write('Early stopped.\n')
-                    break
-
-                if epoch > 1200:
-                    if epoch % 15 == 0:
-                        for p in opt.param_groups:
-                            p['lr'] *= kwargs['lr_decay']
-
-                if verbose > 0:
-                    print('epoch', epoch)
-                    print('training: ', tr[-1])
-                    print('valid: ', val[-1])
-                    if eval:
-                        print('testing: ', te[-1])
+                    print('testing: ', te[-1])
 
             torch.cuda.empty_cache()
 
         if kwargs['save_final']:
             state = {'model': self.model, 'optimizer': opt.state_dict(), 'epoch': epoch - 1}
             torch.save(state, f'{kwargs["model_folder"]}/{PREFIX}.epoch{epoch}.pth')
 
@@ -402,25 +395,26 @@
                     f'epoch {minvep} minimal val {minval} with training:  {tr[minvep]} and testing: {te[minvep]}\n')
             else:
                 logger.write(f'epoch {minvep} minimal val {minval} with training:  {tr[minvep]}\n')
             logger.close()
 
         if verbose > 0 and eval:
             print('min testing', min(te), te.index(min(te)))
-            print('converged testing', minvep * eval_interval, te[minvep])
+            print('converged testing', minvep, te[minvep])
 
         return self.model
 
 
 class ScMoGCN(nn.Module):
 
     def __init__(self, args):
         super().__init__()
         self.args = args
-        self.npw = not args.pathway
+        self.opw = args.only_pathway
+        self.npw = args.no_pathway
         self.nrc = args.no_readout_concatenate
 
         hid_feats = args.hidden_size
         out_feats = args.OUTPUT_SIZE
         FEATURE_SIZE = args.FEATURE_SIZE
 
         if not args.no_batch_features:
@@ -456,15 +450,17 @@
         elif args.normalization == 'layer':
             for i in range((args.embedding_layers - 1) * 2):
                 self.input_norm.append(nn.LayerNorm(hid_feats))
         elif args.normalization == 'group':
             for i in range((args.embedding_layers - 1) * 2):
                 self.input_norm.append(nn.GroupNorm(4, hid_feats))
 
-        if self.npw:
+        if self.opw:
+            self.edges = ['feature2cell', 'pathway']
+        elif self.npw:
             self.edges = ['feature2cell', 'cell2feature']
         else:
             self.edges = ['feature2cell', 'cell2feature', 'pathway']
 
         self.conv_layers = nn.ModuleList()
         if args.residual == 'res_cat':
             self.conv_layers.append(
```

### Comparing `pydance-1.0.0/dance/modules/single_modality/cell_type_annotation/actinn.py` & `pydance-1.0.0rc0/dance/modules/single_modality/cell_type_annotation/actinn.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,190 +2,215 @@
 
 Reference
 ---------
 Ma, Feiyang, and Matteo Pellegrini. "ACTINN: automated identification of cell types in single cell RNA sequencing."
 Bioinformatics 36.2 (2020): 533-538.
 
 """
+import itertools
+from typing import Tuple
+
 import numpy as np
-import scanpy as sc
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from torch import Tensor
 
-from dance.models.nn import VanillaMLP
-from dance.modules.base import BaseClassificationMethod
-from dance.transforms import AnnDataTransform, Compose, FilterGenesPercentile, SetConfig
-from dance.typing import LogLevel, Optional, Tuple
-
-
-class ACTINN(BaseClassificationMethod):
-    """The ACTINN cell-type classification model.
-
-    Parameters
-    ----------
-    hidden_dims
-        Hidden layer dimensions.
-    lambd
-        Regularization parameter
-    device
-        Training device
 
-    """
+class ACTINN(nn.Module):
+    """The ACTINN cell-type classification model."""
 
     def __init__(
         self,
+        input_dim: int,
+        output_dim: int,
         *,
+        batch_size: int = 128,
+        device: str = "cpu",
         hidden_dims: Tuple[int, ...] = (100, 50, 25),
         lambd: float = 0.01,
-        device: str = "cpu",
-        random_seed: Optional[int] = None,
+        lr: float = 0.01,
+        num_epochs: int = 50,
+        print_cost: bool = False,
     ):
-        super().__init__()
+        """Initialize the ACTINN model.
 
-        self.hidden_dims = hidden_dims
-        self.lambd = lambd
-        self.device = device
-        self.random_seed = random_seed
-
-        self.model_size = len(hidden_dims) + 2
-
-    @staticmethod
-    def preprocessing_pipeline(normalize: bool = True, filter_genes: bool = True, log_level: LogLevel = "INFO"):
-        transforms = []
-
-        if normalize:
-            transforms.append(AnnDataTransform(sc.pp.normalize_total, target_sum=1e4))
-            transforms.append(AnnDataTransform(sc.pp.log1p, base=2))
+        Parameters
+        ----------
+        input_dim : int
+            Input dimension (number of genes)
+        output_dim : int
+            Output dimension (number of cell types)
+        hidden_dims : :obj:`tuple` of int
+            Hidden layer dimensions.
+        batch_size : int
+            Training batch size
+        device : str
+            Training device
+        lambd : float
+            Regularization parameter
+        lr : float
+            Initial learning rate
+        num_epochs : int
+            Number of epochs to run
+        print_cost : bool
+            Print training loss if set to True
 
-        if filter_genes:
-            transforms.append(AnnDataTransform(sc.pp.filter_genes, min_cells=1))
-            transforms.append(FilterGenesPercentile(min_val=1, max_val=99, mode="sum"))
-            transforms.append(FilterGenesPercentile(min_val=1, max_val=99, mode="cv"))
+        """
+        super().__init__()
 
-        transforms.append(SetConfig({"label_channel": "cell_type"}))
+        # Save attributes
+        self.batch_size = batch_size
+        self.device = device
+        self.lambd = lambd
+        self.lr = lr
+        self.num_epochs = num_epochs
+        self.print_cost = print_cost
+
+        # Build MLP
+        self.model = nn.Sequential(
+            nn.Linear(input_dim, hidden_dims[0]),
+            nn.ReLU(),
+            *itertools.chain.from_iterable(
+                zip(
+                    map(nn.Linear, hidden_dims[:-1], hidden_dims[1:]),
+                    itertools.repeat(nn.ReLU()),
+                )),
+            nn.Linear(hidden_dims[-1], output_dim),
+        ).to(device)
+        print(self.model)
+
+    def forward(self, x):
+        """Forward propagation."""
+        return self.model(x)
 
-        return Compose(*transforms, log_level=log_level)
+    @torch.no_grad()
+    def initialize_parameters(self, seed=None):
+        """Initialize parameters."""
+        if seed is not None:
+            torch.manual_seed(seed)
+
+        for i in range(0, len(self.model), 2):
+            nn.init.xavier_normal_(self.model[i].weight)
+            self.model[i].bias[:] = 0
 
-    def compute_loss(self, z: Tensor, y: Tensor):
+    def compute_loss(self, z, y):
         """Compute loss function.
 
         Parameters
         ----------
-        z
+        z : torch.Tensor
             Output of forward propagation (cells by cell-types).
-        y
+        y : torch.Tensor
             Cell labels (cells).
 
         Returns
         -------
         torch.Tensor
             Loss.
 
         """
         log_prob = F.log_softmax(z, dim=-1)
         loss = nn.NLLLoss()(log_prob, y)
-        for i, p in enumerate(self.model.model):
-            if (i % 2) == 0:  # skip activation layers
-                loss += self.lambd * (p.weight**2).sum() / 2
+        for i in range(0, len(self.model), 2):  # TODO: replace with weight_decay
+            loss += self.lambd * torch.sum(self.model[i].weight**2) / 2
+
+        if self.print_cost:
+            print(loss)
+
         return loss
 
-    def random_batches(self, x: Tensor, y: Tensor, batch_size: int = 32, seed: Optional[int] = None):
+    def random_batches(self, x, y, batch_size=32, seed=None):
         """Shuffle data and split into batches.
 
         Parameters
         ----------
-        x
+        x : torch.Tensor
             Training data (cells by genes).
-        y
+        y : torch.Tensor
             True labels (cells by cell-types).
 
         Yields
         ------
         Tuple[torch.Tensor, torch.Tensor]
             Batch of training data (x, y).
 
         """
         ns = x.shape[0]
         perm = np.random.default_rng(seed).permutation(ns).tolist()
         slices = [perm[i:i + batch_size] for i in range(0, ns, batch_size)]
         yield from map(lambda slice_: (x[slice_], y[slice_]), slices)
 
-    def fit(
-        self,
-        x_train: Tensor,
-        y_train: Tensor,
-        *,
-        batch_size: int = 128,
-        lr: float = 0.01,
-        num_epochs: int = 50,
-        print_cost: bool = False,
-        seed: Optional[int] = None,
-    ):
+    def fit(self, x_train, y_train, seed=None):
         """Fit the classifier.
 
         Parameters
         ----------
-        x_train
-            training data (cells by genes).
-        y_train
-            training labels (cells by cell-types).
-        batch_size
-            Training batch size.
-        lr
-            Initial learning rate.
-        num_epochs
-            Number of epochs to run.
-        print_cost
-            Print training loss if set to True.
-        seed
+        x_train : torch.Tensor
+            training data (genes by cells).
+        y_train : torch.Tensor
+            training labels (cell-types by cells).
+        seed : int, optional
             Random seed, if set to None, then random.
 
         """
-        input_dim, output_dim = x_train.shape[1], y_train.shape[1]
-        x_train = x_train.clone().detach().float().to(self.device)  # cells by genes
-        y_train = torch.where(y_train)[1].to(self.device)  # cells
+        x_train = x_train.T.clone().detach().float().to(self.device)  # cells by genes
+        y_train = torch.where(y_train.T)[1].to(self.device)  # cells
 
         # Initialize weights, optimizer, and scheduler
-        self.model = VanillaMLP(input_dim, output_dim, hidden_dims=self.hidden_dims, device=self.device)
-        optimizer = torch.optim.Adam(self.model.parameters(), lr=lr)
+        self.initialize_parameters(seed)
+        optimizer = torch.optim.Adam(self.parameters(), lr=self.lr)
         lr_scheduler = torch.optim.lr_scheduler.ExponentialLR(optimizer=optimizer, gamma=0.95)
 
         # Start training loop
-        for epoch in range(num_epochs):
+        for epoch in range(self.num_epochs):
             epoch_seed = seed if seed is None else seed + epoch
-            batches = self.random_batches(x_train, y_train, batch_size, epoch_seed)
+            batches = self.random_batches(x_train, y_train, self.batch_size, epoch_seed)
 
-            tot_cost = tot_size = 0
             for batch_x, batch_y in batches:
-                batch_cost = self.compute_loss(self.model(batch_x), batch_y)
-                tot_cost += batch_cost.item()
-                tot_size += 1
+                batch_cost = self.compute_loss(self.forward(batch_x), batch_y)
 
                 optimizer.zero_grad()
                 batch_cost.backward()
                 optimizer.step()
                 lr_scheduler.step()
 
-            if print_cost and (epoch % 10 == 0):
-                print(f"Epoch: {epoch:>4d} Loss: {tot_cost / tot_size:6.4f}")
+        print("Parameters have been trained!")
 
     @torch.no_grad()
-    def predict(self, x: Tensor):
+    def predict(self, x):
         """Predict cell labels.
 
         Parameters
         ----------
-        x
-            Gene expression input features (cells by genes).
+        x : torch.Tensor
+            Gene expression input features (genes by cells).
 
         Returns
         -------
         torch.Tensor
             Predicted cell-label indices.
 
         """
-        x = x.clone().detach().to(self.device)
-        z = self.model(x)
+        x = x.T.clone().detach().to(self.device)
+        z = self.forward(x)
         prediction = torch.argmax(z, dim=-1)
         return prediction
+
+    def score(self, x, y):
+        """Model performance score measured by accuracy.
+
+        Parameters
+        ----------
+        x : torch.Tensor
+            Gene expression input features (genes by cells).
+        y : torch.Tensor
+            One-hot encoded ground truth labels (cell-types by cells).
+
+        Returns
+        -------
+        float
+            Prediction accuracy
+
+        """
+        pred = self.predict(x).detach().cpu()
+        label = torch.where(y.T)[1]
+        return (pred == label).detach().float().mean().tolist()
```

### Comparing `pydance-1.0.0/dance/modules/single_modality/cell_type_annotation/celltypist.py` & `pydance-1.0.0rc0/dance/modules/single_modality/cell_type_annotation/celltypist.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,64 @@
+import json
+import logging
 import os
+import pathlib
+import pickle
+import warnings
+from datetime import datetime
+from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
+import requests
 import scanpy as sc
 from anndata import AnnData
 from matplotlib import pyplot as plt
+from scipy.sparse import spmatrix
 from scipy.special import expit
-from sklearn.linear_model import LogisticRegression, SGDClassifier
+from sklearn.linear_model import LogisticRegression
 from sklearn.preprocessing import StandardScaler
 
-from dance import logger
-from dance.modules.base import BaseClassificationMethod
-from dance.transforms import SetConfig
-from dance.typing import LogLevel, Optional, Union
+from dance.transforms.preprocess import (LRClassifier_celltypist, SGDClassifier_celltypist, downsample_adata,
+                                         get_sample_csv_celltypist, get_sample_data_celltypist, prepare_data_celltypist,
+                                         to_array_celltypist, to_vector_celltypist)
+
+logging.basicConfig(level=logging.INFO, format="%(message)s")
+logger = logging.getLogger(__name__)
+set_level = logger.setLevel
+info = logger.info
+warn = logger.warning
+error = logger.error
+debug = logger.debug
+
+celltypist_path = os.getenv('CELLTYPIST_FOLDER', default=os.path.join(str(pathlib.Path.home()), '.celltypist'))
+pathlib.Path(celltypist_path).mkdir(parents=True, exist_ok=True)
+data_path = os.path.join(celltypist_path, "data")
+models_path = os.path.join(data_path, "models")
+pathlib.Path(models_path).mkdir(parents=True, exist_ok=True)
+
+_samples_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "data", "samples")
+
+
+def _collapse_mean(arr: np.ndarray) -> Union[float, np.ndarray]:
+    """For internal use.
+
+    Average 1D array, or 2D array by row.
+
+    """
+    return np.mean(arr, axis=-1)
+
+
+def _collapse_random(arr: np.ndarray) -> Union[float, np.ndarray]:
+    """For internal use.
+
+    Choose a random number from 1D array, or a random column from 2D array.
+
+    """
+    return np.random.choice(arr, 1)[0] if arr.ndim == 1 else arr[:, np.random.choice(arr.shape[1], 1)[0]]
 
 
 class Model():
     """Class that wraps the logistic Classifier and the StandardScaler.
 
     Parameters
     ----------
@@ -39,14 +81,43 @@
     """
 
     def __init__(self, clf, scaler, description):
         self.classifier = clf
         self.scaler = scaler
         self.description = description
 
+    @staticmethod
+    def load(self, model: Optional[str] = None):
+        """Load the desired model.
+
+        Parameters
+        ----------
+        model: Optional[str]
+            Model name specifying the model you want to load. Default to `'Immune_All_Low.pkl'` if not provided.
+            To see all available models and their descriptions, use :func:`~celltypist.models.models_description`.
+
+        Returns
+        ----------
+        :class:`~celltypist.models.Model`
+            A :class:`~celltypist.models.Model` object.
+
+        """
+        if not model:
+            model = get_default_model()
+        if model in get_all_models():
+            model = get_model_path(model)
+        if not os.path.isfile(model):
+            raise FileNotFoundError(f" No such file: {model}")
+        with open(model, "rb") as fh:
+            try:
+                pkl_obj = pickle.load(fh)
+                return Model(pkl_obj['Model'], pkl_obj['Scaler_'], pkl_obj['description'])
+            except Exception as exception:
+                raise Exception(f" Invalid model: {model}. {exception}")
+
     @property
     def cell_types(self) -> np.ndarray:
         """Get cell types included in the model."""
         return self.classifier.classes_
 
     @property
     def features(self) -> np.ndarray:
@@ -56,55 +127,76 @@
     def __repr__(self):
         """General the description."""
         base = f"CellTypist model with {len(self.cell_types)} cell types and {len(self.features)} features"
         for x in ['date', 'details', 'source', 'version']:
             if self.description[x] != '':
                 base += f"\n    {x}: {self.description[x]}"
         if len(self.cell_types) == 2:
-            base += f"\n    cell types: {self.cell_types[0]}, {self.cell_types[1]}"
-            base += f"\n    features: {self.features[0]}, {self.features[1]}, ..., {self.features[-1]}"
+            base += f"\n    cell types: {self.cell_types[0]}, {self.cell_types[1]}\n    features: {self.features[0]}, {self.features[1]}, ..., {self.features[-1]}"
         else:
-            base += f"\n    cell types: {self.cell_types[0]}, {self.cell_types[1]}, ..., {self.cell_types[-1]}"
-            base += "\n    features: {self.features[0]}, {self.features[1]}, ..., {self.features[-1]}"
+            base += f"\n    cell types: {self.cell_types[0]}, {self.cell_types[1]}, ..., {self.cell_types[-1]}\n    features: {self.features[0]}, {self.features[1]}, ..., {self.features[-1]}"
         return base
 
-    def predict_labels_and_prob(self, indata) -> tuple:
+    def predict_labels_and_prob(self, indata, mode: str = 'best match', p_thres: float = 0.5) -> tuple:
         """Get the decision matrix, probability matrix, and predicted cell types for the
         input data.
 
         Parameters
         ----------
         indata
             The input array-like object used as a query.
+        mode: str
+            The way cell prediction is performed.
+            For each query cell, the default (`'best match'`) is to choose the cell type with the largest score/probability as the final prediction.
+            Setting to `'prob match'` will enable a multi-label classification, which assigns 0 (i.e., unassigned), 1, or >=2 cell type labels to each query cell.
+            (Default: `'best match'`)
+        p_thres: float
+            Probability threshold for the multi-label classification. Ignored if `mode` is `'best match'`.
+            (Default: 0.5)
 
         Returns
         ----------
         tuple
             A tuple of decision score matrix, raw probability matrix, and predicted cell type labels.
 
         """
         scores = self.classifier.decision_function(indata)
         if len(self.cell_types) == 2:
             scores = np.column_stack([-scores, scores])
         probs = expit(scores)
-        return scores, probs, self.classifier.classes_[scores.argmax(axis=1)]
+        if mode == 'best match':
+            return scores, probs, self.classifier.classes_[scores.argmax(axis=1)]
+        elif mode == 'prob match':
+            flags = probs > p_thres
+            labs = np.array(['|'.join(self.classifier.classes_[np.where(x)[0]]) for x in flags])
+            labs[labs == ''] = 'Unassigned'
+            return scores, probs, labs
+        else:
+            raise ValueError(f" Unrecognized `mode` value, should be one of `'best match'` or `'prob match'`")
+
+    def write(self, file: str) -> None:
+        """Write out the model."""
+        obj = dict(Model=self.classifier, Scaler_=self.scaler, description=self.description)
+        file = os.path.splitext(file)[0] + '.pkl'
+        with open(file, 'wb') as output:
+            pickle.dump(obj, output)
 
     def extract_top_markers(self, cell_type: str, top_n: int = 10, only_positive: bool = True) -> np.ndarray:
         """Extract the top driving genes for a given cell type.
 
         Parameters
         ----------
         cell_type: str
             The cell type to extract markers for.
         top_n: int optional
             Number of markers to extract for a given cell type.
             (Default: 10)
         only_positive: bool optional
-            Whether to extract positive markers only. Set to ``False`` to include negative markers as well.
-            (Default: ``True``)
+            Whether to extract positive markers only. Set to `False` to include negative markers as well.
+            (Default: `True`)
 
         Returns
         ----------
         :class:`~numpy.ndarray`
             A list of marker genes for the query cell type.
 
         """
@@ -114,46 +206,330 @@
             coef_vector = self.classifier.coef_[0] if cell_type == self.cell_types[1] else -self.classifier.coef_[0]
         else:
             coef_vector = self.classifier.coef_[self.cell_types == cell_type][0]
         if not only_positive:
             coef_vector = np.abs(coef_vector)
         return self.features[np.argsort(-coef_vector)][:top_n]
 
+    def convert(self, map_file: Optional[str] = None, sep: str = ',', convert_from: Optional[int] = None,
+                convert_to: Optional[int] = None, unique_only: bool = True, collapse: str = 'average',
+                random_state: int = 0) -> None:
+        """Convert the model of one species to another species by mapping orthologous
+        genes.
 
-# TODO: repurpose this to general purpose anlaysis tools
-# (dance.tools? -> e.g., dance.tools.SummaryFrequency(data), how about preds?)
-class AnnotationResult():
-    """Class that represents the result of a celltyping annotation process.
+        Parameters
+        ----------
+        map_file: str optional
+            A two-column gene mapping file between two species.
+            Default to a human-mouse (mouse-human) conversion using the built-in mapping file provided by CellTypist.
+        sep: str
+            Delimiter of the mapping file. Default to comma (i.e., a csv file is by default expected from the user if provided).
+        convert_from: int optional
+            Column index (0 or 1) of the mapping file corresponding to the species converted from.
+            Default to an automatic detection.
+        convert_to: int optional
+            Column index (0 or 1) of the mapping file corresponding to the species converted to.
+            Default to an automatic detection.
+        unique_only: bool  optional
+            Whether to leverage only 1:1 orthologs between the two species.
+            (Default: `True`)
+        collapse: str optional
+            The way 1:N orthologs are handled. Possible values are `'average'` which averages the classifier weights and `'random'` which randomly chooses one gene's weights from all its orthologs.
+            This argument is ignored if `unique_only = True`.
+            (Default: `'average'`)
+        random_state: int optional
+            Random seed for reproducibility. This argument is only relevant if `unique_only = False` and `collapse = 'random'`.
+
+        Returns
+        ----------
+        None
+            The original model is modified by converting to the other species.
+
+        """
+        map_file = get_sample_data_celltypist('Ensembl105_Human2Mouse_Genes.csv') if map_file is None else map_file
+        if not os.path.isfile(map_file):
+            raise FileNotFoundError(f" No such file: {map_file}")
+        #with and without headers are both ok -> real headers become fake genes and are removed afterwards
+        map_content = pd.read_csv(map_file, sep=sep, header=None)
+        map_content.dropna(axis=0, inplace=True)
+        map_content.drop_duplicates(inplace=True)
+        #From & To detection
+        if (convert_from is None) and (convert_to is None):
+            column1_overlap = map_content[0].isin(self.features).sum()
+            column2_overlap = map_content[1].isin(self.features).sum()
+            convert_from = 0 if column1_overlap > column2_overlap else 1
+            convert_to = 1 - convert_from
+        elif convert_from is None:
+            if convert_to not in [0, 1]:
+                raise ValueError(f" `convert_to` should be either 0 or 1")
+            convert_from = 1 - convert_to
+        elif convert_to is None:
+            if convert_from not in [0, 1]:
+                raise ValueError(f" `convert_from` should be either 0 or 1")
+            convert_to = 1 - convert_from
+        else:
+            if {convert_from, convert_to} != {0, 1}:
+                raise ValueError(f" `convert_from` and `convert_to` should be 0 (or 1) and 1 (or 0)")
+        #filter
+        map_content = map_content[map_content[convert_from].isin(self.features)]
+        if unique_only:
+            map_content.drop_duplicates([0], inplace=True)
+            map_content.drop_duplicates([1], inplace=True)
+        map_content['index_from'] = pd.DataFrame(
+            self.features, columns=['features']).reset_index().set_index('features').loc[map_content[convert_from],
+                                                                                         'index'].values
+        #main
+        logger.info(f" Number of genes in the original model: {len(self.features)}")
+        features_to = map_content[convert_to].values if unique_only else np.unique(map_content[convert_to])
+        if unique_only:
+            index_from = map_content['index_from'].values
+            self.classifier.coef_ = self.classifier.coef_[:, index_from]
+            self.scaler.mean_ = self.scaler.mean_[index_from]
+            self.scaler.var_ = self.scaler.var_[index_from]
+            self.scaler.scale_ = self.scaler.scale_[index_from]
+        else:
+            if collapse not in ['average', 'random']:
+                raise ValueError(f" Unrecognized `collapse` value, should be one of `'average'` or `'random'`")
+            if collapse == 'random':
+                np.random.seed(random_state)
+            collapse_func = _collapse_mean if collapse == 'average' else _collapse_random
+            coef_to = []
+            mean_to = []
+            var_to = []
+            scale_to = []
+            for feature_to in features_to:
+                index_from = map_content[map_content[convert_to] == feature_to].index_from.values
+                if len(index_from) == 1:
+                    coef_to.append(self.classifier.coef_[:, index_from[0]])
+                    mean_to.append(self.scaler.mean_[index_from[0]])
+                    var_to.append(self.scaler.var_[index_from[0]])
+                    scale_to.append(self.scaler.scale_[index_from[0]])
+                else:
+                    coef_to.append(collapse_func(self.classifier.coef_[:, index_from]))
+                    mean_to.append(collapse_func(self.scaler.mean_[index_from]))
+                    var_to.append(collapse_func(self.scaler.var_[index_from]))
+                    scale_to.append(collapse_func(self.scaler.scale_[index_from]))
+            self.classifier.coef_ = np.column_stack(coef_to)
+            self.scaler.mean_ = np.array(mean_to)
+            self.scaler.var_ = np.array(var_to)
+            self.scaler.scale_ = np.array(scale_to)
+        self.classifier.n_features_in_ = len(features_to)
+        self.classifier.features = features_to
+        self.scaler.n_features_in_ = len(features_to)
+        logger.info(f" Conversion done! Number of genes in the converted model: {len(features_to)}")
+
+
+def get_model_path(file: str) -> str:
+    """Get the full path to a file in the `models` folder.
 
     Parameters
     ----------
+    file: str
+        File name as a string.
+        To see all available models and their descriptions, use :func:`~celltypist.models.models_description`.
+
+    Returns
+    ----------
+    str
+        A string of the full path to the desired file.
+
+    """
+    return os.path.join(models_path, f"{file}")
+
+
+def get_default_model() -> str:
+    """Get the default model name.
+
+    Returns
+    ----------
+    str
+        A string showing the default model name (should be `'Immune_All_Low.pkl'`).
+
+    """
+    models_json = get_models_index()
+    default_model = [m["filename"] for m in models_json["models"] if ("default" in m and m["default"])]
+    if not default_model:
+        first_model = models_json["models"][0]["filename"]
+        logger.warn(f" No model marked as 'default', using {first_model}")
+        return first_model
+    if len(default_model) > 1:
+        logger.warn(f" More than one model marked as 'default', using {default_model[0]}")
+    return default_model[0]
+
+
+def get_all_models() -> list:
+    """
+    Get a list of all the available models.
+    Returns
+    ----------
+    list
+        A list of available models.
+    """
+    download_if_required()
+    available_models = []
+    for model_filename in os.listdir(models_path):
+        if model_filename.endswith(".pkl"):
+            model_name = os.path.basename(model_filename)
+            available_models.append(model_name)
+    return available_models
+
+
+def download_if_required() -> None:
+    """Download models if there are none present in the `models` directory."""
+    if len([m for m in os.listdir(models_path) if m.endswith(".pkl")]) == 0:
+        logger.info(f" No available models. Downloading...")
+        download_models()
+
+
+def get_models_index(force_update: bool = False) -> dict:
+    """Get the model json object containing the model list.
+
+    Parameters
+    ----------
+    force_update: bool optional
+        If set to `True`, will download the latest model json file from the remote.
+        (Default: `False`)
+
+    Returns
+    ----------
+    dict: dict
+        A dict object converted from the model json file.
+
+    """
+    models_json_path = get_model_path("models.json")
+    if not os.path.exists(models_json_path) or force_update:
+        download_model_index()
+    with open(models_json_path) as f:
+        return json.load(f)
+
+
+def download_model_index(only_model: bool = True) -> None:
+    """Download the `models.json` file from the remote server.
+
+    Parameters
+    ----------
+    only_model: bool
+        If set to `False`, will also download the models in addition to the json file.
+        (Default: `True`)
+
+    Returns
+    ----------
+    No return
+
+    """
+    url = 'https://celltypist.cog.sanger.ac.uk/models/models.json'
+    logger.info(f" Retrieving model list from server {url}")
+    with open(get_model_path("models.json"), "wb") as f:
+        f.write(requests.get(url).content)
+    model_count = len(requests.get(url).json()["models"])
+    logger.info(f" Total models in list: {model_count}")
+    if not only_model:
+        download_models()
+
+
+def download_models(force_update: bool = False, model: Optional[Union[str, list, tuple]] = None) -> None:
+    """Download all the available or selected models.
+
+    Parameters
+    ----------
+    force_update: bool
+        Whether to fetch a latest JSON index for downloading all available or selected models.
+        Set to `True` if you want to parallel the latest celltypist model releases.
+        (Default: `False`)
+    model: Optional[Union[str, list, tuple]]
+        Specific model(s) to download. By default, all available models are downloaded.
+        Set to a specific model name or a list of model names to only download a subset of models.
+        For example, set to `["ModelA.pkl", "ModelB.pkl"]` to only download ModelA and ModelB.
+        To check all available models, use :func:`~celltypist.models.models_description`.
+
+    """
+    models_json = get_models_index(force_update)
+    logger.info(f" Storing models in {models_path}")
+    if model is not None:
+        model_list = {model} if isinstance(model, str) else set(model)
+        models_json["models"] = [m for m in models_json["models"] if m["filename"] in model_list]
+        provided_no = len(model_list)
+        filtered_no = len(models_json["models"])
+        if filtered_no == 0:
+            raise ValueError(f" No models match the celltypist model repertoire. Please provide valid model names")
+        elif provided_no == filtered_no:
+            logger.info(f" Total models to download: {provided_no}")
+        else:
+            ignored_models = model_list.difference({m["filename"] for m in models_json["models"]})
+            logger.warn(
+                f" Total models to download: {filtered_no}. {len(ignored_models)} not available: {ignored_models}")
+    model_count = len(models_json["models"])
+    for idx, model in enumerate(models_json["models"]):
+        model_path = get_model_path(model["filename"])
+        if os.path.exists(model_path) and not force_update:
+            logger.info(f" Skipping [{idx+1}/{model_count}]: {model['filename']} (file exists)")
+            continue
+        logger.info(f" Downloading model [{idx+1}/{model_count}]: {model['filename']}")
+        try:
+            with open(model_path, "wb") as f:
+                f.write(requests.get(model["url"]).content)
+        except Exception as exception:
+            logger.error(f" {model['filename']} failed {exception}")
+
+
+def models_description(on_the_fly: bool = False) -> pd.DataFrame:
+    """Get the descriptions of all available models.
+
+    Parameters
+    ----------
+    on_the_fly: bool
+        Whether to fetch the model information from downloaded model files.
+        If set to `True`, will fetch the information by loading downloaded models.
+        Default to fetching the information for all available models from the JSON file.
+        (Default: `False`)
+
+    Returns
+    ----------
+    :class:`~pandas.DataFrame`
+        A :class:`~pandas.DataFrame` object with model descriptions.
+
+    """
+    logger.info(f" Detailed model information can be found at `https://www.celltypist.org/models`")
+    if on_the_fly:
+        filenames = get_all_models()
+        descriptions = [Model.load(filename).description['details'] for filename in filenames]
+    else:
+        models_json = get_models_index()
+        models = models_json["models"]
+        filenames = [model['filename'] for model in models]
+        descriptions = [model['details'] for model in models]
+    return pd.DataFrame({'model': filenames, 'description': descriptions})
+
+
+class AnnotationResult():
+    """
+    Class that represents the result of a celltyping annotation process.
+    Parameters
+    ----------
     labels
         A :class:`~pandas.DataFrame` object returned from the celltyping process, showing the predicted labels.
     decision_mat
         A :class:`~pandas.DataFrame` object returned from the celltyping process, showing the decision matrix.
     prob_mat
         A :class:`~pandas.DataFrame` object returned from the celltyping process, showing the probability matrix.
     adata
         An :class:`~anndata.AnnData` object representing the input object.
 
     Attributes
     ----------
     predicted_labels
-        Predicted labels including the individual prediction results and (if majority voting is done) majority voting
-        results.
+        Predicted labels including the individual prediction results and (if majority voting is done) majority voting results.
     decision_matrix
         Decision matrix with the decision score of each cell belonging to a given cell type.
     probability_matrix
-        Probability matrix representing the probability each cell belongs to a given cell type (transformed from
-        decision matrix by the sigmoid function).
+        Probability matrix representing the probability each cell belongs to a given cell type (transformed from decision matrix by the sigmoid function).
     cell_count
         Number of input cells which undergo the prediction process.
     adata
         An :class:`~anndata.AnnData` object representing the input data.
-
     """
 
     def __init__(self, labels: pd.DataFrame, decision_mat: pd.DataFrame, prob_mat: pd.DataFrame, adata: AnnData):
         self.predicted_labels = labels
         self.decision_matrix = decision_mat
         self.probability_matrix = prob_mat
         self.adata = adata
@@ -162,18 +538,17 @@
     def summary_frequency(self, by: str = 'predicted_labels') -> pd.DataFrame:
         """
         Get the frequency of cells belonging to each cell type predicted by celltypist.
         Parameters
 
         ----------
         by: str
-            Column name of :attr:`~celltypist.classifier.AnnotationResult.predicted_labels` specifying the prediction
-            type which the summary is based on. Set to ``'majority_voting'`` if you want to summarize for the majority
-            voting classifier.
-            (Default: ``'predicted_labels'``)
+            Column name of :attr:`~celltypist.classifier.AnnotationResult.predicted_labels` specifying the prediction type which the summary is based on.
+            Set to `'majority_voting'` if you want to summarize for the majority voting classifier.
+            (Default: `'predicted_labels'`)
 
         Returns
         ----------
         :class:`~pandas.DataFrame`
             A :class:`~pandas.DataFrame` object with cell type frequencies.
         """
         unique, counts = np.unique(self.predicted_labels[by], return_counts=True)
@@ -185,111 +560,108 @@
                  insert_decision: bool = False, insert_prob: bool = False, prefix: str = '') -> AnnData:
         """Insert the predicted labels, decision or probability matrix, and (if majority
         voting is done) majority voting results into the AnnData object.
 
         Parameters
         ----------
         insert_labels: bool optional
-            Whether to insert the predicted cell type labels and (if majority voting is done) majority voting-based
-            labels into the AnnData object. (Default: ``True``)
+            Whether to insert the predicted cell type labels and (if majority voting is done) majority voting-based labels into the AnnData object.
+            (Default: `True`)
         insert_conf: bool optional
-            Whether to insert the confidence scores into the AnnData object. (Default: ``True``)
+            Whether to insert the confidence scores into the AnnData object.
+            (Default: `True`)
         insert_conf_by: str optional
-            Column name of :attr:`~celltypist.classifier.AnnotationResult.predicted_labels` specifying the prediction
-            type which the confidence scores are based on. Setting to ``'majority_voting'`` will insert the confidence
-            scores corresponding to the majority-voting result.
-            (Default: ``'predicted_labels'``)
+            Column name of :attr:`~celltypist.classifier.AnnotationResult.predicted_labels` specifying the prediction type which the confidence scores are based on.
+            Setting to `'majority_voting'` will insert the confidence scores corresponding to the majority-voting result.
+            (Default: `'predicted_labels'`)
         insert_decision: bool optional
-            Whether to insert the decision matrix into the AnnData object. (Default: ``False``)
+            Whether to insert the decision matrix into the AnnData object.
+            (Default: `False`)
         insert_prob: bool optional
-            Whether to insert the probability matrix into the AnnData object. This will override the decision matrix
-            even when ``insert_decision`` is set to ``True``. (Default: ``False``)
+            Whether to insert the probability matrix into the AnnData object. This will override the decision matrix even when `insert_decision` is set to `True`.
+            (Default: `False`)
         prefix:  str optional
             Prefix for the inserted columns in the AnnData object. Default to no prefix used.
 
         Returns
         ----------
         :class:`~anndata.AnnData`
-            Depending on whether majority voting is done, an :class:`~anndata.AnnData` object with the following columns
-            (prefixed with ``prefix``) added to the observation metadata:
+            Depending on whether majority voting is done, an :class:`~anndata.AnnData` object with the following columns (prefixed with `prefix`) added to the observation metadata:
             1) **predicted_labels**, individual prediction outcome for each cell.
             2) **over_clustering**, over-clustering result for the cells.
             3) **majority_voting**, the cell type label assigned to each cell after the majority voting process.
             4) **conf_score**, the confidence score of each cell.
-            5) **name of each cell type**, which represents the decision scores (or probabilities if ``insert_prob`` is
-               ``True``) of a given cell type across cells.
+            5) **name of each cell type**, which represents the decision scores (or probabilities if `insert_prob` is `True`) of a given cell type across cells.
 
         """
         if insert_labels:
             self.adata.obs[[f"{prefix}{x}" for x in self.predicted_labels.columns]] = self.predicted_labels
         if insert_conf:
             if insert_conf_by == 'predicted_labels':
                 self.adata.obs[f"{prefix}conf_score"] = self.probability_matrix.max(axis=1).values
             elif insert_conf_by == 'majority_voting':
                 if insert_conf_by not in self.predicted_labels:
-                    raise KeyError(" Did not find the column `majority_voting` in the "
-                                   "`AnnotationResult.predicted_labels`, perform majority voting beforehand or use "
-                                   "`insert_conf_by = 'predicted_labels'` instead")
+                    raise KeyError(
+                        f" Did not find the column `majority_voting` in the `AnnotationResult.predicted_labels`, perform majority voting beforehand or use `insert_conf_by = 'predicted_labels'` instead"
+                    )
                 self.adata.obs[f"{prefix}conf_score"] = [
                     row[self.predicted_labels.majority_voting[index]]
                     for index, row in self.probability_matrix.iterrows()
                 ]
             else:
-                raise KeyError(f" Unrecognized `insert_conf_by` value ('{insert_conf_by}'), should be one of "
-                               "`'predicted_labels'` or `'majority_voting'`")
+                raise KeyError(
+                    f" Unrecognized `insert_conf_by` value ('{insert_conf_by}'), should be one of `'predicted_labels'` or `'majority_voting'`"
+                )
         if insert_prob:
             self.adata.obs[[f"{prefix}{x}" for x in self.probability_matrix.columns]] = self.probability_matrix
         elif insert_decision:
             self.adata.obs[[f"{prefix}{x}" for x in self.decision_matrix.columns]] = self.decision_matrix
         return self.adata
 
     def to_plots(self, folder: str, plot_probability: bool = False, format: str = 'pdf', prefix: str = '') -> None:
         """Plot the celltyping and (if majority voting is done) majority-voting results.
 
         Parameters
         ----------
         folder: str
             Path to a folder which stores the output figures.
         plot_probability: bool optional
-            Whether to also plot the decision score and probability distributions of each cell type across the test
-            cells. If ``True``, a number of figures will be generated (may take some time if the input data is large).
-            (Default: ``False``)
+            Whether to also plot the decision score and probability distributions of each cell type across the test cells.
+            If `True`, a number of figures will be generated (may take some time if the input data is large).
+            (Default: `False`)
         format: str optional
             Format of output figures. Default to vector PDF files (note dots are still drawn with png backend).
-            (Default: ``'pdf'``)
+            (Default: `'pdf'`)
         prefix: str optional
             Prefix for the output figures. Default to no prefix used.
 
         Returns
         ----------
         None
-            Depending on whether majority voting is done and ``plot_probability``, multiple UMAP plots showing the
-            prediction and majority voting results in the ``folder``:
+            Depending on whether majority voting is done and `plot_probability`, multiple UMAP plots showing the prediction and majority voting results in the `folder`:
             1) **predicted_labels**, individual prediction outcome for each cell overlaid onto the UMAP.
             2) **over_clustering**, over-clustering result of the cells overlaid onto the UMAP.
-            3) **majority_voting**, the cell type label assigned to each cell after the majority voting process overlaid
-               onto the UMAP.
-            4) **name of each cell type**, which represents the decision scores and probabilities of a given cell type
-               distributed across cells overlaid onto the UMAP.
+            3) **majority_voting**, the cell type label assigned to each cell after the majority voting process overlaid onto the UMAP.
+            4) **name of each cell type**, which represents the decision scores and probabilities of a given cell type distributed across cells overlaid onto the UMAP.
 
         """
         if not os.path.isdir(folder):
             raise FileNotFoundError(f" Output folder {folder} does not exist. Please provide a valid folder")
         if 'X_umap' in self.adata.obsm:
-            logger.info("Detected existing UMAP coordinates, will plot the results accordingly")
+            logger.info(" Detected existing UMAP coordinates, will plot the results accordingly")
         elif 'connectivities' in self.adata.obsp:
             logger.info(" Generating UMAP coordinates based on the neighborhood graph")
             sc.tl.umap(self.adata)
         else:
-            logger.info("Constructing the neighborhood graph and generating UMAP coordinates")
+            logger.info(" Constructing the neighborhood graph and generating UMAP coordinates")
             adata = self.adata.copy()
             self.adata.obsm['X_pca'], self.adata.obsp['connectivities'], self.adata.obsp['distances'], self.adata.uns[
                 'neighbors'] = Classifier._construct_neighbor_graph(adata)
             sc.tl.umap(self.adata)
-        logger.info("Plotting the results")
+        logger.info(" Plotting the results")
         sc.settings.set_figure_params(figsize=[6.4, 6.4], format=format)
         self.adata.obs[self.predicted_labels.columns] = self.predicted_labels
         for column in self.predicted_labels:
             sc.pl.umap(self.adata, color=column, legend_loc='on data', show=False, legend_fontweight='normal',
                        title=column.replace('_', ' '))
             plt.savefig(os.path.join(folder, prefix + column + '.' + format))
         if plot_probability:
@@ -308,20 +680,20 @@
         ----------
         folder: str
             Path to a folder which stores the output table/tables.
         prefix: str
             Prefix for the output table/tables. Default to no prefix used.
         xlsx: bool optional
             Whether to merge output tables into a single Excel (.xlsx).
-            (Default: ``False``)
+            (Default: `False`)
 
         Returns
         ----------
         None
-            Depending on ``xlsx``, return table(s) of predicted labels, decision matrix and probability matrix.
+            Depending on `xlsx`, return table(s) of predicted labels, decision matrix and probability matrix.
 
         """
         if not os.path.isdir(folder):
             raise FileNotFoundError(f" Output folder {folder} does not exist. Please provide a valid folder")
         if not xlsx:
             self.predicted_labels.to_csv(os.path.join(folder, f"{prefix}predicted_labels.csv"))
             self.decision_matrix.to_csv(os.path.join(folder, f"{prefix}decision_matrix.csv"))
@@ -330,101 +702,189 @@
             with pd.ExcelWriter(os.path.join(folder, f"{prefix}annotation_result.xlsx")) as writer:
                 self.predicted_labels.to_excel(writer, sheet_name="Predicted Labels")
                 self.decision_matrix.to_excel(writer, sheet_name="Decision Matrix")
                 self.probability_matrix.to_excel(writer, sheet_name="Probability Matrix")
 
     def __repr__(self):
         base = f"CellTypist prediction result for {self.cell_count} query cells"
-        base += f"\n    predicted_labels: data frame with {self.predicted_labels.shape[1]} "
-        base += f"{'columns' if self.predicted_labels.shape[1] > 1 else 'column'} "
-        base += f"({str(list(self.predicted_labels.columns))[1:-1]})"
-        base += f"\n    decision_matrix: data frame with {self.cell_count} query cells and "
-        base += f"{self.decision_matrix.shape[1]} cell types"
-        base += f"\n    probability_matrix: data frame with {self.cell_count} query cells and "
-        base += f"{self.probability_matrix.shape[1]} cell types"
-        base += "\n    adata: AnnData object referred"
+        base += f"\n    predicted_labels: data frame with {self.predicted_labels.shape[1]} {'columns' if self.predicted_labels.shape[1] > 1 else 'column'} ({str(list(self.predicted_labels.columns))[1:-1]})"
+        base += f"\n    decision_matrix: data frame with {self.cell_count} query cells and {self.decision_matrix.shape[1]} cell types"
+        base += f"\n    probability_matrix: data frame with {self.cell_count} query cells and {self.probability_matrix.shape[1]} cell types"
+        base += f"\n    adata: AnnData object referred"
         return base
 
 
 class Classifier():
-    """Class that wraps the celltyping and majority voting processes.
-
+    """
+    Class that wraps the celltyping and majority voting processes.
     Parameters
     ----------
-    x: np.ndarray
-        Input expression matrix (cell x gene).
-    model: Model
-        A :class:`~celltypist.models.Model` object that wraps the logistic Classifier and the StandardScaler.
-
+    filename: Union[AnnData,str]
+        Path to the input count matrix (supported types are csv, txt, tsv, tab and mtx) or AnnData object (h5ad).
+        If it's the former, a cell-by-gene format is desirable (see `transpose` for more information).
+        Also accepts the input as an :class:`~anndata.AnnData` object already loaded in memory.
+        Genes should be gene symbols. Non-expressed genes are preferred to be provided as well.
+    model: Union[Model,str]
+        A :class:`~celltypist.models.Model` object that wraps the logistic Classifier and the StandardScaler, the
+        path to the desired model file, or the model name.
+    transpose: bool
+        Whether to transpose the input matrix. Set to `True` if `filename` is provided in a gene-by-cell format.
+        (Default: `False`)
+    gene_file: Optional[str]
+        Path to the file which stores each gene per line corresponding to the genes used in the provided mtx file.
+        Ignored if `filename` is not provided in the mtx format.
+    cell_file: Optional[str]
+        Path to the file which stores each cell per line corresponding to the cells used in the provided mtx file.
+        Ignored if `filename` is not provided in the mtx format.
     Attributes
     ----------
+    filename:
+        Path to the input dataset. This attribute exists only when the input is a file path.
     adata:
-        An :class:`~anndata.AnnData` object which stores the log1p normalized expression data in ``.X`` or ``.raw.X``.
+        An :class:`~anndata.AnnData` object which stores the log1p normalized expression data in `.X` or `.raw.X`.
     indata:
         The expression matrix used for predictions stored in the log1p normalized format.
     indata_genes:
         All the genes included in the input data.
     indata_names:
         All the cells included in the input data.
     model:
         A :class:`~celltypist.models.Model` object that wraps the logistic Classifier and the StandardScaler.
-
     """
 
-    def __init__(self, x: np.ndarray, model: Model):
+    def __init__(
+        self,
+        filename: Union[AnnData, str] = "",
+        model: Union[Model, str] = "",
+        transpose: bool = False,
+        gene_file: Optional[str] = None,
+        cell_file: Optional[str] = None,
+        check_expression: bool = False,
+    ):
+        if isinstance(model, str):
+            model = Model.load(model)
         self.model = model
+        if not filename:
+            logger.warn(f" No input file provided to the classifier")
+            return
+        if isinstance(filename, str):
+            self.filename = filename
+            logger.info(f" Input file is '{self.filename}'")
+            logger.info(f" Loading data")
+        if isinstance(filename, str) and filename.endswith(('.csv', '.txt', '.tsv', '.tab', '.mtx', '.mtx.gz')):
+            self.adata = sc.read(self.filename)
+            if transpose:
+                self.adata = self.adata.transpose()
+            if self.filename.endswith(('.mtx', '.mtx.gz')):
+                if (gene_file is None) or (cell_file is None):
+                    raise FileNotFoundError(
+                        " Missing `gene_file` and/or `cell_file`. Please provide both arguments together with the input mtx file"
+                    )
+                genes_mtx = pd.read_csv(gene_file, header=None)[0].values
+                cells_mtx = pd.read_csv(cell_file, header=None)[0].values
+                if len(genes_mtx) != self.adata.n_vars:
+                    raise ValueError(
+                        f" The number of genes in {gene_file} does not match the number of genes in {self.filename}")
+                if len(cells_mtx) != self.adata.n_obs:
+                    raise ValueError(
+                        f" The number of cells in {cell_file} does not match the number of cells in {self.filename}")
+                self.adata.var_names = genes_mtx
+                self.adata.obs_names = cells_mtx
+            self.adata.var_names_make_unique()
+            if not float(self.adata.X.max()).is_integer():
+                logger.warn(
+                    f" Warning: the input file seems not a raw count matrix. The prediction result may be biased")
+            if (self.adata.n_vars >= 80000) or (len(self.adata.var_names[0]) >= 30) or (len(
+                    self.adata.obs_names.intersection(pd.Index(['GAPDH', 'ACTB', 'CALM1', 'PTPRC']))) >= 1):
+                raise ValueError(
+                    f" The input matrix is detected to be a gene-by-cell matrix. Please provide a cell-by-gene matrix or add the input transpose option"
+                )
+            sc.pp.normalize_total(self.adata, target_sum=1e4)
+            sc.pp.log1p(self.adata)
+            self.indata = self.adata.X
+            self.indata_genes = self.adata.var_names
+            self.indata_names = self.adata.obs_names
+        elif isinstance(filename, AnnData) or (isinstance(filename, str) and filename.endswith('.h5ad')):
+            self.adata = sc.read(filename) if isinstance(filename, str) else filename
+            self.adata.var_names_make_unique()
+            if self.adata.X.min() < 0:
+                logger.info(" Detected scaled expression in the input data, will try the `.raw` attribute")
+                try:
+                    self.indata = self.adata.raw.X
+                    self.indata_genes = self.adata.raw.var_names
+                    self.indata_names = self.adata.raw.obs_names
+                except Exception as e:
+                    raise Exception(f" Fail to use the `.raw` attribute in the input object. {e}")
+            else:
+                self.indata = self.adata.X
+                self.indata_genes = self.adata.var_names
+                self.indata_names = self.adata.obs_names
+            if check_expression and np.abs(np.expm1(self.indata[0]).sum() - 10000) > 1:
+                raise ValueError(
+                    " Invalid expression matrix, expect log1p normalized expression to 10000 counts per cell")
+        else:
+            raise ValueError(
+                " Invalid input. Supported types: .csv, .txt, .tsv, .tab, .mtx, .mtx.gz and .h5ad, or AnnData loaded in memory"
+            )
 
-        self.adata = AnnData(x)
-        self.adata.var_names_make_unique()
-
-        self.indata = self.adata.X
-        self.indata_genes = self.adata.var_names
-        self.indata_names = self.adata.obs_names
-        logger.info(f"Input data has {self.indata.shape[0]:,} cells and {len(self.indata_genes):,} genes")
+        logger.info(f" Input data has {self.indata.shape[0]} cells and {len(self.indata_genes)} genes")
 
-    def celltype(self) -> AnnotationResult:
+    def celltype(self, mode: str = 'best match', p_thres: float = 0.5) -> AnnotationResult:
         """Run celltyping jobs to predict cell types of input data.
 
+        Parameters
+        ----------
+        mode: str optional
+            The way cell prediction is performed.
+            For each query cell, the default (`'best match'`) is to choose the cell type with the largest score/probability as the final prediction.
+            Setting to `'prob match'` will enable a multi-label classification, which assigns 0 (i.e., unassigned), 1, or >=2 cell type labels to each query cell.
+            (Default: `'best match'`)
+        p_thres: float optional
+            Probability threshold for the multi-label classification. Ignored if `mode` is `'best match'`.
+            (Default: 0.5)
+
         Returns
         ----------
         :class:`~celltypist.classifier.AnnotationResult`
             An :class:`~celltypist.classifier.AnnotationResult` object. Four important attributes within this class are:
             1) :attr:`~celltypist.classifier.AnnotationResult.predicted_labels`, predicted labels from celltypist.
             2) :attr:`~celltypist.classifier.AnnotationResult.decision_matrix`, decision matrix from celltypist.
             3) :attr:`~celltypist.classifier.AnnotationResult.probability_matrix`, probability matrix from celltypist.
             4) :attr:`~celltypist.classifier.AnnotationResult.adata`, AnnData object representation of the input data.
 
         """
-        logger.info("Matching reference genes in the model")
+        logger.info(f" Matching reference genes in the model")
         k_x = np.isin(self.indata_genes, self.model.classifier.features)
         if k_x.sum() == 0:
-            raise ValueError("No features overlap with the model. Please provide gene symbols")
+            raise ValueError(f" No features overlap with the model. Please provide gene symbols")
         else:
-            logger.info(f"{k_x.sum():,} features used for prediction")
+            logger.info(f" {k_x.sum()} features used for prediction")
         k_x_idx = np.where(k_x)[0]
+        #self.indata = self.indata[:, k_x_idx]
         self.indata_genes = self.indata_genes[k_x_idx]
-        lr_idx = np.where(np.isin(self.model.classifier.features, self.indata_genes))[0]
+        lr_idx = pd.DataFrame(self.model.classifier.features,
+                              columns=['features']).reset_index().set_index('features').loc[self.indata_genes,
+                                                                                            'index'].values
 
-        logger.info("Scaling input data")
+        logger.info(f" Scaling input data")
         means_ = self.model.scaler.mean_[lr_idx]
         sds_ = self.model.scaler.scale_[lr_idx]
         self.indata = (self.indata[:, k_x_idx] - means_) / sds_
         self.indata[self.indata > 10] = 10
 
-        # Temporarily replace with subsetted features, will recover after running the prediction function
         ni, fs, cf = self.model.classifier.n_features_in_, self.model.classifier.features, self.model.classifier.coef_
         self.model.classifier.n_features_in_ = lr_idx.size
         self.model.classifier.features = self.model.classifier.features[lr_idx]
         self.model.classifier.coef_ = self.model.classifier.coef_[:, lr_idx]
 
-        logger.info("Predicting labels")
-        decision_mat, prob_mat, lab = self.model.predict_labels_and_prob(self.indata)
-        logger.info("Prediction done")
+        logger.info(" Predicting labels")
+        decision_mat, prob_mat, lab = self.model.predict_labels_and_prob(self.indata, mode=mode, p_thres=p_thres)
+        logger.info(" Prediction done!")
 
-        # Restore model after prediction
+        #restore model after prediction
         self.model.classifier.n_features_in_, self.model.classifier.features, self.model.classifier.coef_ = ni, fs, cf
 
         cells = self.indata_names
         return AnnotationResult(pd.DataFrame(lab, columns=['predicted_labels'], index=cells, dtype='category'),
                                 pd.DataFrame(decision_mat, columns=self.model.classifier.classes_, index=cells),
                                 pd.DataFrame(prob_mat, columns=self.model.classifier.classes_, index=cells), self.adata)
 
@@ -451,64 +911,63 @@
         """Over-clustering input data with a canonical Scanpy pipeline. A neighborhood
         graph will be used (or constructed if not found) for the over-clustering.
 
         Parameters
         ----------
         resolution: float optional
             Resolution parameter for leiden clustering which controls the coarseness of the clustering.
-            Default to 5, 10, 15, 20, 25 and 30 for datasets with cell numbers less than 5k, 20k, 40k, 100k, 200k and
-            above, respectively.
+            Default to 5, 10, 15, 20, 25 and 30 for datasets with cell numbers less than 5k, 20k, 40k, 100k, 200k and above, respectively.
 
         Returns
         ----------
         :class:`~pandas.Series`
             A :class:`~pandas.Series` object showing the over-clustering result.
 
         """
         if 'connectivities' not in self.adata.obsp:
-            logger.info("Can not detect a neighborhood graph, will construct one before the over-clustering")
+            logger.info(" Can not detect a neighborhood graph, will construct one before the over-clustering")
             adata = self.adata.copy()
             self.adata.obsm['X_pca'], self.adata.obsp['connectivities'], self.adata.obsp['distances'], self.adata.uns[
                 'neighbors'] = Classifier._construct_neighbor_graph(adata)
         else:
-            logger.info("Detected a neighborhood graph in the input object, will run overclustering on the basis of it")
+            logger.info(
+                " Detected a neighborhood graph in the input object, will run over-clustering on the basis of it")
         if resolution is None:
             if self.adata.n_obs < 5000:
                 resolution = 5
             elif self.adata.n_obs < 20000:
                 resolution = 10
             elif self.adata.n_obs < 40000:
                 resolution = 15
             elif self.adata.n_obs < 100000:
                 resolution = 20
             elif self.adata.n_obs < 200000:
                 resolution = 25
             else:
                 resolution = 30
-        logger.info(f"Over-clustering input data with resolution set to {resolution}")
+        logger.info(f" Over-clustering input data with resolution set to {resolution}")
         sc.tl.leiden(self.adata, resolution=resolution, key_added='over_clustering')
         return self.adata.obs.pop('over_clustering')
 
     @staticmethod
     def majority_vote(predictions: AnnotationResult, over_clustering: Union[list, tuple, np.ndarray, pd.Series,
                                                                             pd.Index],
                       min_prop: float = 0) -> AnnotationResult:
         """Majority vote the celltypist predictions using the result from the over-
         clustering.
 
         Parameters
         ----------
         predictions: AnnotationResult
-            An :class:`~celltypist.classifier.AnnotationResult` object containing the
-            :attr:`~celltypist.classifier.AnnotationResult.predicted_labels`.
+            An :class:`~celltypist.classifier.AnnotationResult` object containing the :attr:`~celltypist.classifier.AnnotationResult.predicted_labels`.
         over_clustering: Union[list, tuple, np.ndarray, pd.Series, pd.Index]
             A list, tuple, numpy array, pandas series or index containing the over-clustering information.
         min_prop: float
-            For the dominant cell type within a subcluster, the minimum proportion of cells required to support naming
-            of the subcluster by this cell type. (Default: 0)
+            For the dominant cell type within a subcluster, the minimum proportion of cells required to support naming of the subcluster by this cell type.
+            (Default: 0)
 
         Returns
         ----------
         output:class:`~celltypist.classifier.AnnotationResult`
             An :class:`~celltypist.classifier.AnnotationResult` object. Four important attributes within this class are:
             1) :attr:`~celltypist.classifier.AnnotationResult.predicted_labels`, predicted labels from celltypist.
             2) :attr:`~celltypist.classifier.AnnotationResult.decision_matrix`, decision matrix from celltypist.
@@ -528,291 +987,379 @@
         majority.columns = ['over_clustering', 'majority_voting']
         majority['majority_voting'] = majority['majority_voting'].astype('category')
         predictions.predicted_labels = predictions.predicted_labels.join(majority)
         logger.info(" Majority voting done!")
         return predictions
 
 
-class Celltypist(BaseClassificationMethod):
-    """The CellTypist cell annotation method.
+class Celltypist():
+    r"""Build the ACTINN model.
 
     Parameters
     ----------
-    majority_voting
-        Whether to refine the predicted labels by running the majority voting classifier after over-clustering.
+    classifier : Classification function
+        Class that wraps the celltyping and majority voting processes, as defined above
+    scaler : StandardScaler
+        The scale factor for normalization.
+    description : str
+        text description of the model.
 
     """
 
-    def __init__(self, majority_voting: bool = False, clf=None, scaler=None, description=None):
-        self.majority_voting = majority_voting
+    def __init__(self, clf=None, scaler=None, description=None):
         self.classifier = clf
         self.scaler = scaler
         self.description = description
 
-    @staticmethod
-    def preprocessing_pipeline(log_level: LogLevel = "INFO"):
-        return SetConfig({"label_channel": "cell_type"}, log_level=log_level)
-
-    def fit(self, indata: np.array, labels: Optional[Union[str, list, tuple, np.ndarray, pd.Series, pd.Index]] = None,
-            C: float = 1.0, solver: Optional[str] = None, max_iter: int = 1000, n_jobs: Optional[int] = None,
-            use_SGD: bool = False, alpha: float = 0.0001, mini_batch: bool = False, batch_number: int = 100,
-            batch_size: int = 1000, epochs: int = 10, balance_cell_type: bool = False, feature_selection: bool = False,
-            top_genes: int = 300, **kwargs):
+    def fit(
+            self,
+            X=None,
+            labels: Optional[Union[str, list, tuple, np.ndarray, pd.Series, pd.Index]] = None,
+            genes: Optional[Union[str, list, tuple, np.ndarray, pd.Series, pd.Index]] = None,
+            transpose_input: bool = False,
+            check_expression: bool = True,
+            #LR param
+            C: float = 1.0,
+            solver: Optional[str] = None,
+            max_iter: int = 1000,
+            n_jobs: Optional[int] = None,
+            #SGD param
+            use_SGD: bool = False,
+            alpha: float = 0.0001,
+            #mini-batch
+            mini_batch: bool = False,
+            batch_number: int = 100,
+            batch_size: int = 1000,
+            epochs: int = 10,
+            balance_cell_type: bool = False,
+            #feature selection
+            feature_selection: bool = False,
+            top_genes: int = 300,
+            #description
+            date: str = '',
+            details: str = '',
+            url: str = '',
+            source: str = '',
+            version: str = '',
+            #other param
+            **kwargs):
         """Train a celltypist model using mini-batch (optional) logistic classifier with
         a global solver or stochastic gradient descent (SGD) learning.
 
         Parameters
         ----------
-        indata: np.ndarray
-            Input gene expression matrix (cell x gene).
-        labels: np.array
-            1-D numpy array indicating cell-type identities of each cell (in index of the cell-types).
+        X: Path optional
+            Path to the input count matrix (supported types are csv, txt, tsv, tab and mtx) or AnnData (h5ad).
+            Also accepts the input as an :class:`~anndata.AnnData` object, or any array-like objects already loaded in memory.
+            See `check_expression` for detailed format requirements.
+            A cell-by-gene format is desirable (see `transpose_input` for more information).
+        labels: Union[str, list, tuple, np.ndarray, pd.Series, pd.Index] optional
+            Path to the file containing cell type label per line corresponding to the cells in `X`.
+            Also accepts any list-like objects already loaded in memory (such as an array).
+            If `X` is specified as an AnnData, this argument can also be set as a column name from cell metadata.
+        genes: Union[str, list, tuple, np.ndarray, pd.Series, pd.Index] Optional
+            Path to the file containing one gene per line corresponding to the genes in `X`.
+            Also accepts any list-like objects already loaded in memory (such as an array).
+            Note `genes` will be extracted from `X` where possible (e.g., `X` is an AnnData or data frame).
+        transpose_input: bool
+            Whether to transpose the input matrix. Set to `True` if `X` is provided in a gene-by-cell format.
+            (Default: `False`)
+        check_expression: bool optional
+            Check whether the expression matrix in the input data is supplied as required.
+            Except the case where a path to the raw count table file is specified, all other inputs for `X` should be in log1p normalized expression to 10000 counts per cell.
+            Set to `False` if you want to train the data regardless of the expression formats.
+            (Default: `True`)
         C: float optional
-            Inverse of L2 regularization strength for traditional logistic classifier. A smaller value can possibly
-            improve model generalization while at the cost of decreased accuracy. This argument is ignored if SGD
-            learning is enabled (``use_SGD = True``). (Default: 1.0)
+            Inverse of L2 regularization strength for traditional logistic classifier. A smaller value can possibly improve model generalization while at the cost of decreased accuracy.
+            This argument is ignored if SGD learning is enabled (`use_SGD = True`).
+            (Default: 1.0)
         solver: str optional
-            Algorithm to use in the optimization problem for traditional logistic classifier. The default behavior is
-            to choose the solver according to the size of the input data. This argument is ignored if SGD learning is
-            enabled (``use_SGD = True``).
+            Algorithm to use in the optimization problem for traditional logistic classifier.
+            The default behavior is to choose the solver according to the size of the input data.
+            This argument is ignored if SGD learning is enabled (`use_SGD = True`).
         max_iter: int optional
             Maximum number of iterations before reaching the minimum of the cost function.
-            Try to decrease ``max_iter`` if the cost function does not converge for a long time.
-            This argument is for both traditional and SGD logistic classifiers, and will be ignored if mini-batch SGD
-            training is conducted (``use_SGD = True`` and ``mini_batch = True``). (Default: 1000)
+            Try to decrease `max_iter` if the cost function does not converge for a long time.
+            This argument is for both traditional and SGD logistic classifiers, and will be ignored if mini-batch SGD training is conducted (`use_SGD = True` and `mini_batch = True`).
+            (Default: 1000)
         n_jobs: int optional
-            Number of CPUs used. Default to one CPU. ``-1`` means all CPUs are used.
+            Number of CPUs used. Default to one CPU. `-1` means all CPUs are used.
             This argument is for both traditional and SGD logistic classifiers.
         use_SGD: bool optional
-            Whether to implement SGD learning for the logistic classifier. (Default: ``False``)
+            Whether to implement SGD learning for the logistic classifier.
+            (Default: `False`)
         alpha: float optional
-            L2 regularization strength for SGD logistic classifier. A larger value can possibly improve model
-            generalization while at the cost of decreased accuracy. This argument is ignored if SGD learning is disabled
-            (``use_SGD = False``). (Default: 0.0001)
+            L2 regularization strength for SGD logistic classifier. A larger value can possibly improve model generalization while at the cost of decreased accuracy.
+            This argument is ignored if SGD learning is disabled (`use_SGD = False`).
+            (Default: 0.0001)
         mini_batch: bool optional
             Whether to implement mini-batch training for the SGD logistic classifier.
-            Setting to ``True`` may improve the training efficiency for large datasets (for example, >100k cells).
-            This argument is ignored if SGD learning is disabled (``use_SGD = False``). (Default: ``False``)
+            Setting to `True` may improve the training efficiency for large datasets (for example, >100k cells).
+            This argument is ignored if SGD learning is disabled (`use_SGD = False`).
+            (Default: `False`)
         batch_number: int optional
-            The number of batches used for training in each epoch. Each batch contains ``batch_size`` cells. For
-            datasets which cannot be binned into ``batch_number`` batches, all batches will be used. This argument is
-            relevant only if mini-batch SGD training is conducted (``use_SGD = True`` and ``mini_batch = True``).
+            The number of batches used for training in each epoch. Each batch contains `batch_size` cells.
+            For datasets which cannot be binned into `batch_number` batches, all batches will be used.
+            This argument is relevant only if mini-batch SGD training is conducted (`use_SGD = True` and `mini_batch = True`).
             (Default: 100)
         batch_size: int optional
-            The number of cells within each batch. This argument is relevant only if mini-batch SGD training is
-            conducted (``use_SGD = True`` and ``mini_batch = True``). (Default: 1000)
+            The number of cells within each batch.
+            This argument is relevant only if mini-batch SGD training is conducted (`use_SGD = True` and `mini_batch = True`).
+            (Default: 1000)
         epochs: int optional
-            The number of epochs for the mini-batch training procedure. The default values of ``batch_number``,
-            ``batch_size``, and ``epochs`` together allow observing ~10^6 training cells. This argument is relevant
-            only if mini-batch SGD training is conducted (``use_SGD = True`` and ``mini_batch = True``). (Default: 10)
+            The number of epochs for the mini-batch training procedure.
+            The default values of `batch_number`, `batch_size`, and `epochs` together allow observing ~10^6 training cells.
+            This argument is relevant only if mini-batch SGD training is conducted (`use_SGD = True` and `mini_batch = True`).
+            (Default: 10)
         balance_cell_type: bool optional
-            Whether to balance the cell type frequencies in mini-batches during each epoch. Setting to ``True`` will
-            sample rare cell types with a higher probability, ensuring close-to-even cell type distributions in
-            mini-batches. This argument is relevant only if mini-batch SGD training is conducted (``use_SGD = True`` and
-            ``mini_batch = True``). (Default: ``False``)
+            Whether to balance the cell type frequencies in mini-batches during each epoch.
+            Setting to `True` will sample rare cell types with a higher probability, ensuring close-to-even cell type distributions in mini-batches.
+            This argument is relevant only if mini-batch SGD training is conducted (`use_SGD = True` and `mini_batch = True`).
+            (Default: `False`)
         feature_selection: bool optional
-            Whether to perform two-pass data training where the first round is used for selecting important
-            features/genes using SGD learning. If ``True``, the training time will be longer. (Default: ``False``)
+            Whether to perform two-pass data training where the first round is used for selecting important features/genes using SGD learning.
+            If `True`, the training time will be longer.
+            (Default: `False`)
         top_genes: int optional
             The number of top genes selected from each class/cell-type based on their absolute regression coefficients.
-            The final feature set is combined across all classes (i.e., union). (Default: 300)
+            The final feature set is combined across all classes (i.e., union).
+            (Default: 300)
+        date: str optional
+            Free text of the date of the model. Default to the time when the training is completed.
+        details: str optional
+            Free text of the description of the model.
+        url: str optional
+            Free text of the (possible) download url of the model.
+        source: str optional
+            Free text of the source (publication, database, etc.) of the model.
+        version: str optional
+            Free text of the version of the model.
         **kwargs
-            Other keyword arguments passed to :class:`~sklearn.linear_model.LogisticRegression` (``use_SGD = False``) or
-            :class:`~sklearn.linear_model.SGDClassifier` (``use_SGD = True``).
+            Other keyword arguments passed to :class:`~sklearn.linear_model.LogisticRegression` (`use_SGD = False`) or :class:`~sklearn.linear_model.SGDClassifier` (`use_SGD = True`).
 
         Returns
         -------
         :class:`~celltypist.models.Model`
             An instance of the :class:`~celltypist.models.Model` trained by celltypist.
 
         """
-        # Prepare
-        logger.info("Preparing data before training")
-        genes = np.arange(indata.shape[1]).astype(str)
-
-        # Scaler
-        logger.info("Scaling input data")
+        #prepare
+        logger.info(" Preparing data before training")
+        indata, labels, genes = prepare_data_celltypist(X, labels, genes, transpose_input)
+        indata = to_array_celltypist(indata)
+        labels = np.array(labels)
+        genes = np.array(genes)
+        #check
+        if check_expression and (np.abs(np.expm1(indata[0]).sum() - 10000) > 1):
+            raise ValueError(" Invalid expression matrix, expect log1p normalized expression to 10000 counts per cell")
+        if len(labels) != indata.shape[0]:
+            raise ValueError(
+                f" Length of training labels ({len(labels)}) does not match the number of input cells ({indata.shape[0]})"
+            )
+        if len(genes) != indata.shape[1]:
+            raise ValueError(
+                f" The number of genes ({len(genes)}) provided does not match the number of genes in the training data ({indata.shape[1]})"
+            )
+        #filter
+        flag = indata.sum(axis=0) == 0
+        if flag.sum() > 0:
+            logger.info(f" {flag.sum()} non-expressed genes are filtered out")
+            #indata = indata[:, ~flag]
+            genes = genes[~flag]
+        #scaler
+        logger.info(f" Scaling input data")
         scaler = StandardScaler()
-        indata = scaler.fit_transform(indata)
+        indata = scaler.fit_transform(indata[:, ~flag] if flag.sum() > 0 else indata)
         indata[indata > 10] = 10
-
-        # Classifier
+        #classifier
         if use_SGD or feature_selection:
             classifier = SGDClassifier_celltypist(indata=indata, labels=labels, alpha=alpha, max_iter=max_iter,
                                                   n_jobs=n_jobs, mini_batch=mini_batch, batch_number=batch_number,
                                                   batch_size=batch_size, epochs=epochs,
                                                   balance_cell_type=balance_cell_type, **kwargs)
         else:
             classifier = LRClassifier_celltypist(indata=indata, labels=labels, C=C, solver=solver, max_iter=max_iter,
                                                  n_jobs=n_jobs, **kwargs)
-
-        # Feature selection -> new classifier and scaler
+        #feature selection -> new classifier and scaler
         if feature_selection:
-            logger.info("Selecting features")
+            logger.info(f" Selecting features")
             if len(genes) <= top_genes:
-                raise ValueError(f" The number of genes ({len(genes)}) is fewer than the `top_genes` ({top_genes}). "
-                                 "Unable to perform feature selection")
+                raise ValueError(
+                    f" The number of genes ({len(genes)}) is fewer than the `top_genes` ({top_genes}). Unable to perform feature selection"
+                )
             gene_index = np.argpartition(np.abs(classifier.coef_), -top_genes, axis=1)[:, -top_genes:]
             gene_index = np.unique(gene_index)
-            logger.info(f"{len(gene_index)} features are selected")
+            logger.info(f" {len(gene_index)} features are selected")
             genes = genes[gene_index]
-
-            logger.info("Starting the second round of training")
+            #indata = indata[:, gene_index]
+            logger.info(f" Starting the second round of training")
             if use_SGD:
                 classifier = SGDClassifier_celltypist(indata=indata[:, gene_index], labels=labels, alpha=alpha,
                                                       max_iter=max_iter, n_jobs=n_jobs, mini_batch=mini_batch,
                                                       batch_number=batch_number, batch_size=batch_size, epochs=epochs,
                                                       balance_cell_type=balance_cell_type, **kwargs)
             else:
                 classifier = LRClassifier_celltypist(indata=indata[:, gene_index], labels=labels, C=C, solver=solver,
                                                      max_iter=max_iter, n_jobs=n_jobs, **kwargs)
             scaler.mean_ = scaler.mean_[gene_index]
             scaler.var_ = scaler.var_[gene_index]
             scaler.scale_ = scaler.scale_[gene_index]
             scaler.n_features_in_ = len(gene_index)
-
-        # Model finalization
+        #model finalization
         classifier.features = genes
-        description = {'number_celltypes': len(classifier.classes_)}
-        logger.info("Model training done")
+        if not date:
+            date = str(datetime.now())
+        description = {
+            'date': date,
+            'details': details,
+            'url': url,
+            'source': source,
+            'version': version,
+            'number_celltypes': len(classifier.classes_)
+        }
+        logger.info(f" Model training done!")
 
         self.classifier = classifier
         self.scaler = scaler
         self.description = description
 
-    def predict(self, x: np.ndarray, as_obj: bool = False, over_clustering: Optional[Union[str, list, tuple, np.ndarray,
-                                                                                           pd.Series, pd.Index]] = None,
-                min_prop: float = 0) -> Union[np.ndarray, AnnotationResult]:
+    def predict(self, filename: Union[AnnData, str] = "", check_expression: bool = False, load_model: bool = False,
+                model: Optional[Union[str, Model]] = None, transpose_input: bool = False,
+                gene_file: Optional[str] = None, cell_file: Optional[str] = None, mode: str = 'best match',
+                p_thres: float = 0.5, majority_voting: bool = False,
+                over_clustering: Optional[Union[str, list, tuple, np.ndarray, pd.Series,
+                                                pd.Index]] = None, min_prop: float = 0) -> AnnotationResult:
         """Run the prediction and (optional) majority voting to annotate the input
         dataset.
 
         Parameters
         ----------
-        x: np.ndarray
-            Input expression matrix (cell x gene).
-        as_obj: bool
-            If set to ``True``, then return the prediction results are :class:`~AnnotationResult`. Otherwise, return the
-            predicted cell-label indexes ad 1-d numpy array instead. (Default: ``False``)
+        filename: Union[AnnData,str]  optional
+            Path to the input count matrix (supported types are csv, txt, tsv, tab and mtx) or AnnData (h5ad).
+            If it's the former, a cell-by-gene format is desirable (see `transpose_input` for more information).
+            Also accepts the input as an :class:`~anndata.AnnData` object already loaded in memory.
+            Genes should be gene symbols. Non-expressed genes are preferred to be provided as well.
+        model: Union[str, Model] optional
+            Model used to predict the input cells. Default to using the `'Immune_All_Low.pkl'` model.
+            Can be a :class:`~celltypist.models.Model` object that wraps the logistic Classifier and the StandardScaler, the
+            path to the desired model file, or the model name.
+            To see all available models and their descriptions, use :func:`~celltypist.models.models_description`.
+        transpose_input: boolUnion[str, Model]
+            Whether to transpose the input matrix. Set to `True` if `filename` is provided in a gene-by-cell format.
+            (Default: `False`)
+        gene_file: str optional
+            Path to the file which stores each gene per line corresponding to the genes used in the provided mtx file.
+            Ignored if `filename` is not provided in the mtx format.
+        cell_file: str optional
+            Path to the file which stores each cell per line corresponding to the cells used in the provided mtx file.
+            Ignored if `filename` is not provided in the mtx format.
+        mode: str optional
+            The way cell prediction is performed.
+            For each query cell, the default (`'best match'`) is to choose the cell type with the largest score/probability as the final prediction.
+            Setting to `'prob match'` will enable a multi-label classification, which assigns 0 (i.e., unassigned), 1, or >=2 cell type labels to each query cell.
+            (Default: `'best match'`)
+        p_thres: float optional
+            Probability threshold for the multi-label classification. Ignored if `mode` is `'best match'`.
+            (Default: 0.5)
+        majority_voting: bool optional
+            Whether to refine the predicted labels by running the majority voting classifier after over-clustering.
+            (Default: `False`)
         over_clustering: Union[str, list, tuple, np.ndarray, pd.Series, pd.Index] optional
             This argument can be provided in several ways:
             1) an input plain file with the over-clustering result of one cell per line.
             2) a string key specifying an existing metadata column in the AnnData (pre-created by the user).
-            3) a python list, tuple, numpy array, pandas series or index representing the over-clustering result of the
-               input cells.
-            4) if none of the above is provided, will use a heuristic over-clustering approach according to the size of
-               input data.
-            Ignored if ``majority_voting`` is set to ``False``.
+            3) a python list, tuple, numpy array, pandas series or index representing the over-clustering result of the input cells.
+            4) if none of the above is provided, will use a heuristic over-clustering approach according to the size of input data.
+            Ignored if `majority_voting` is set to `False`.
         min_prop: float optional
-            For the dominant cell type within a subcluster, the minimum proportion of cells required to support naming
-            of the subcluster by this cell type. Ignored if ``majority_voting`` is set to ``False``. Subcluster that
-            fails to pass this proportion threshold will be assigned ``'Heterogeneous'``. (Default: 0)
-
-        """
-        # Construct classifier
-        lr_classifier = Model(self.classifier, self.scaler, self.description)
-        clf = Classifier(x=x, model=lr_classifier)
-
-        # Predict
-        predictions = clf.celltype()
-
-        if self.majority_voting:
-            if predictions.cell_count <= 50:
-                logger.warn("The input number of cells ({predictions.cell_count}) is too few to conduct "
-                            "proper over-clustering; no majority voting is performed")
-            else:
-                predictions = self._majority_voting(predictions, clf, over_clustering, min_prop)
-
-        if not as_obj:
-            predictions = np.array(predictions.predicted_labels["predicted_labels"].values)
+            For the dominant cell type within a subcluster, the minimum proportion of cells required to support naming of the subcluster by this cell type.
+            Ignored if `majority_voting` is set to `False`.
+            Subcluster that fails to pass this proportion threshold will be assigned `'Heterogeneous'`.
+            (Default: 0)
 
-        return predictions
+        Returns
+        ----------
+        output :class:`~celltypist.classifier.AnnotationResult`
+            An :class:`~celltypist.classifier.AnnotationResult` object. Four important attributes within this class are:
+            1) :attr:`~celltypist.classifier.AnnotationResult.predicted_labels`, predicted labels from celltypist.
+            2) :attr:`~celltypist.classifier.AnnotationResult.decision_matrix`, decision matrix from celltypist.
+            3) :attr:`~celltypist.classifier.AnnotationResult.probability_matrix`, probability matrix from celltypist.
+            4) :attr:`~celltypist.classifier.AnnotationResult.adata`, AnnData representation of the input data.
 
-    def _majority_voting(self, predictions, clf, over_clustering, min_prop) -> AnnotationResult:
-        # Over clustering
+        """
+        #load model
+        # lr_classifier = Model(self.classifier, self.scaler, self.description) if isinstance(model, Model) else Model.load(model)
+        if load_model:
+            lr_classifier = Model.load(model)
+        else:
+            lr_classifier = Model(self.classifier, self.scaler, self.description)
+        #construct Classifier class
+        clf = Classifier(filename=filename, model=lr_classifier, transpose=transpose_input, gene_file=gene_file,
+                         cell_file=cell_file, check_expression=check_expression)
+        #predict
+        predictions = clf.celltype(mode=mode, p_thres=p_thres)
+        if not majority_voting:
+            return predictions
+        if predictions.cell_count <= 50:
+            logger.warn(
+                f" Warning: the input number of cells ({predictions.cell_count}) is too few to conduct proper over-clustering; no majority voting is performed"
+            )
+            return predictions
+        #over clustering
         if over_clustering is None:
             over_clustering = clf.over_cluster()
             predictions.adata = clf.adata
         elif isinstance(over_clustering, str):
             if over_clustering in clf.adata.obs:
                 over_clustering = clf.adata.obs[over_clustering]
             else:
-                logger.info(f"Did not identify '{over_clustering}' as a cell metadata column, "
-                            "assume it to be a plain text file")
+                logger.info(
+                    f" Did not identify '{over_clustering}' as a cell metadata column, assume it to be a plain text file"
+                )
                 try:
                     with open(over_clustering) as f:
                         over_clustering = [x.strip() for x in f.readlines()]
                 except Exception as e:
                     raise Exception(f" {e}")
-
         if len(over_clustering) != clf.adata.n_obs:
-            raise ValueError(f"Length of `over_clustering` ({len(over_clustering)}) does not match "
-                             f"the number of input cells ({clf.adata.n_obs})")
-
-        # Majority voting
+            raise ValueError(
+                f" Length of `over_clustering` ({len(over_clustering)}) does not match the number of input cells ({clf.adata.n_obs})"
+            )
+        #majority voting
+        print(predictions)
         return Classifier.majority_vote(predictions, over_clustering, min_prop=min_prop)
 
+    def score(self, input_adata, predictions, labels, map, label_conversion=False):
+        """Run the prediction and (optional) majority voting to evaluate the model
+        performance.
 
-def LRClassifier_celltypist(indata, labels, C, solver, max_iter, n_jobs, **kwargs) -> LogisticRegression:
-    """For internal use.
-
-    Get the logistic Classifier.
-
-    """
-    no_cells = len(labels)
-    if solver is None:
-        solver = 'sag' if no_cells > 50000 else 'lbfgs'
-    elif solver not in ('liblinear', 'lbfgs', 'newton-cg', 'sag', 'saga'):
-        raise ValueError("?? Invalid `solver`, should be one of `'liblinear'`, `'lbfgs'`, `'newton-cg'`, "
-                         "`'sag'`, and `'saga'`")
-    logger.info("Training data using logistic regression")
-    if (no_cells > 100000) and (indata.shape[1] > 10000):
-        logger.warn(f"?? Warning: it may take a long time to train this dataset with {no_cells} cells and "
-                    f"{indata.shape[1]} genes, try to downsample cells and/or restrict genes to a subset (e.g., hvgs)")
-    logger.info("LRClassifier training start...")
-    classifier = LogisticRegression(C=C, solver=solver, max_iter=max_iter, multi_class='ovr', n_jobs=n_jobs, **kwargs)
-    classifier.fit(indata, labels)
-    return classifier
-
-
-def SGDClassifier_celltypist(indata, labels, alpha, max_iter, n_jobs, mini_batch, batch_number, batch_size, epochs,
-                             balance_cell_type, **kwargs) -> SGDClassifier:
-    """For internal use.
+        Parameters
+        ----------
+        input_adata: Anndata
+            Input data anndata with label ground truth
+        predictions: classifier.AnnotationResult
+            Output from prediction function.
+        labels : string
+            column name for annotated cell types in the input Anndata
+        label_conversion: boolean optional
+            whether to match predicted labels to annotated cell type labels provided in input_adata
+        map: dictionary
+            a dictionary for label conversion
 
-    Get the SGDClassifier.
+        Returns
+        -------
+        correct: int
+            Number of correct predictions
+        Accuracy: float
+            Prediction accuracy from the model
 
-    """
-    classifier = SGDClassifier(loss='log_loss', alpha=alpha, max_iter=max_iter, n_jobs=n_jobs, **kwargs)
-    if not mini_batch:
-        logger.info("Training data using SGD logistic regression")
-        if (len(labels) > 100000) and (indata.shape[1] > 10000):
-            logger.warn(f"?? Warning: it may take a long time to train this dataset with {len(labels)} cells and "
-                        f"{indata.shape[1]} genes, try to downsample cells and/or restrict genes to a subset "
-                        "(e.g., hvgs)")
-        logger.info("SGDlassifier training start...")
-        classifier.fit(indata, labels)
-    else:
-        logger.info("Training data using mini-batch SGD logistic regression")
-        no_cells = len(labels)
-        if no_cells < 10000:
-            logger.warn(f"?? Warning: the number of cells ({no_cells}) is not big enough to conduct a proper "
-                        "mini-batch training. You may consider using traditional SGD classifier (mini_batch = False)")
-        if no_cells <= batch_size:
-            raise ValueError(f"?? Number of cells ({no_cells}) is fewer than the batch size ({batch_size}). Decrease "
-                             "`batch_size`, or use SGD directly (mini_batch = False)")
-        no_cells_sample = min([batch_number * batch_size, no_cells])
-        starts = np.arange(0, no_cells_sample, batch_size)
-        if balance_cell_type:
-            celltype_freq = np.unique(labels, return_counts=True)
-            len_celltype = len(celltype_freq[0])
-            mapping = pd.Series(1 / (celltype_freq[1] * len_celltype), index=celltype_freq[0])
-            p = mapping[labels].values
-        for epoch in range(1, (epochs + 1)):
-            logger.info(f"Epochs: [{epoch}/{epochs}]")
-            if not balance_cell_type:
-                sampled_cell_index = np.random.choice(no_cells, no_cells_sample, replace=False)
-            else:
-                sampled_cell_index = np.random.choice(no_cells, no_cells_sample, replace=False, p=p)
-            for start in starts:
-                logger.info("SGDlassifier training start...")
-                classifier.partial_fit(indata[sampled_cell_index[start:start + batch_size]],
-                                       labels[sampled_cell_index[start:start + batch_size]], classes=np.unique(labels))
-    return classifier
+        """
+        pred_labels = np.array(predictions.predicted_labels)[:, 0]
+        if label_conversion:
+            correct = 0
+            #for i, cell in enumerate(np.array(adVal.obs.Cell_type)):
+            for i, cell in enumerate(np.array(input_adata.obs[labels])):
+                if pred_labels[i] in map[cell]:
+                    correct += 1
+        else:
+            correct = sum(np.array(input_adata.obs[labels]) == pred_labels)
+        return (correct / len(predictions.predicted_labels))
```

### Comparing `pydance-1.0.0/dance/modules/single_modality/cell_type_annotation/scdeepsort.py` & `pydance-1.0.0rc0/dance/modules/spatial/cell_type_deconvo/dstg.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,346 +1,379 @@
-"""Reimplementation of the scDeepSort cell-type annotation method.
+"""A PyTorch reimplementation of the DSTG cell-type deconvolution method.
+
+Adapted from https://github.com/Su-informatics-lab/DSTG
 
 Reference
 ---------
-Shao, Xin, et al. "scDeepSort: a pre-trained cell-type annotation method for single-cell transcriptomics using deep
-learning with a weighted graph neural network." Nucleic acids research 49.21 (2021): e122-e122.
+Song, and Su. "DSTG: deconvoluting spatial transcriptomics data through graph-based artificial intelligence."
+Briefings in Bioinformatics (2021)
 
 """
+import math
 import time
-from copy import deepcopy
-from pathlib import Path
 
-import dgl
+import numpy as np
+import scanpy as sc
 import torch
 import torch.nn as nn
-from dgl.dataloading import DataLoader, NeighborSampler
+import torch.nn.functional as F
+import torch.optim as optim
+from torch.autograd import Variable
+from torch.nn.parameter import Parameter
 
-from dance.models.nn import AdaptiveSAGE
-from dance.modules.base import BaseClassificationMethod
-from dance.transforms import Compose, SetConfig
-from dance.transforms.graph import PCACellFeatureGraph
-from dance.typing import LogLevel, Optional
-
-
-class GNN(nn.Module):
-    """The scDeepSort GNN model.
-
-    Message passing between cell and genes to learn cell representations for cell-type annotations. The graph contains
-    both cell and gene nodes. The gene features are initialized as PCA embeddings from the (normalized) scRNA-seq
-    samples matrix, and the cell features are computed as the weighted aggregation of the gene features according to
-    each cell's gene expressions.
+from dance.transforms.graph_construct import stAdjConstruct
+from dance.transforms.preprocess import preprocess_adj, pseudo_spatial_process, split
 
-    Parameters
-    ----------
-    dim_in
-        Input dimension (PCA embeddings dimension).
-    dim_out
-        Output dimension (number of unique cell labels).
-    n_layers
-        Number of convolution layers.
-    gene_num
-        Number of genes.
-    dropout
-        Dropout ratio.
-    activation
-        Activation layer.
-    norm
-        Normalization layer.
 
-    """
+class GraphConvolution(nn.Module):
+    """Simple GCN layer, similar to https://arxiv.org/abs/1609.02907."""
 
-    def __init__(
-        self,
-        dim_in: int,
-        dim_out: int,
-        dim_hid: int,
-        n_layers: int,
-        gene_num: int,
-        activation: Optional[nn.Module] = None,
-        norm: Optional[nn.Module] = None,
-        dropout: Optional[float] = 0.,
-    ):
-        super().__init__()
+    def __init__(self, in_features, out_features, support, bias=False):
+        """GraphConvolution.
 
-        self.n_layers = n_layers
-        self.gene_num = gene_num
+        Parameters
+        ----------
+        in_features : int
+            input dimension.
+        out_features : int
+            output dimension.
+        support :
+            support for graph convolution.
+        bias : boolean optional
+            include bias term, default False.
 
-        # [gene_num] is alpha of gene-gene self loop, [gene_num+1] is alpha of cell-cell self loop, the rest are betas
-        self.alpha = nn.Parameter(torch.tensor([1] * (self.gene_num + 2), dtype=torch.float32).unsqueeze(-1))
+        Returns
+        -------
+        None.
 
-        dropout_layer = nn.Dropout(p=dropout) if dropout > 0 else nn.Identity()
-        act_layer = activation or nn.Identity()
-        norm_layer = norm or nn.Identity()
+        """
+        super().__init__()
+        self.support = support
+        self.in_features = in_features
+        self.out_features = out_features
+        self.weight = Parameter(torch.FloatTensor(in_features, out_features))
+        if bias:
+            self.bias = Parameter(torch.FloatTensor(out_features))
+        else:
+            self.register_parameter('bias', None)
+        self.reset_parameters()
+
+    def reset_parameters(self):
+        #glorot
+        init_range = np.sqrt(6.0 / (self.in_features + self.out_features))
+        self.weight.data.uniform_(-init_range, init_range)
+        # similar to kaiming normal/uniform
+        stdv = 1. / math.sqrt(self.weight.size(1))
+        #self.weight.data.uniform_(-stdv, stdv)
+        if self.bias is not None:
+            self.bias.data.uniform_(-stdv, stdv)
 
-        self.layers = nn.ModuleList()
-        for i in range(n_layers):
-            input_dimension = dim_in if i == 0 else dim_hid
-            self.layers.append(AdaptiveSAGE(input_dimension, dim_hid, self.alpha, dropout_layer, act_layer, norm_layer))
+    def forward(self, input, adj):
+        """forward function.
 
-        self.linear = nn.Linear(dim_hid, dim_out)
-        nn.init.xavier_uniform_(self.linear.weight, gain=nn.init.calculate_gain("relu"))
+        Parameters
+        ----------
+        input :
+            node features.
+        adj :
+            adjacency matrix.
 
-    def forward(self, blocks, x):
-        assert len(blocks) == len(self.layers), f"Inonsistent layer info: {len(blocks)=} vs {len(self.layers)=}"
-        for block, layer in zip(blocks, self.layers):
-            x = layer(block, x)
-        return self.linear(x)
+        Returns
+        -------
+        output : float
+            output of graph convolution layer.
 
+        """
+        #convolution
+        if input.is_sparse:
+            #sparse input features
+            support = torch.spmm(input, self.weight)
+        else:
+            support = torch.mm(input, self.weight)
+
+        #adj should always be sparse
+        #### add a ReLU or other activation!!
+        output = torch.spmm(adj, support)
+        if self.bias is not None:
+            return output + self.bias
+        else:
+            return output
+
+    def __repr__(self):
+        return self.__class__.__name__ + ' (' \
+               + str(self.in_features) + ' -> ' \
+               + str(self.out_features) + ')'
 
-class ScDeepSort(BaseClassificationMethod):
-    """The ScDeepSort cell-type annotation model.
 
-    Parameters
-    ----------
-    dim_in
-        Input dimension, i.e., the number of PCA used for cell and gene features.
-    dim_hid
-        Hidden dimension.
-    num_layers
-        Number of convolution layers.
-    species
-        Species name (only used for determining the read/write path).
-    tissue
-        Tissue name (only used for determining the read/write path).
-    dropout
-        Drop-out rate.
-    batch_size
-        Batch size.
-    device
-        Computation device, e.g., 'cpu', 'cuda'.
+class GCN(nn.Module):
+    """dropout + GC + activation."""
 
-    """
+    def __init__(self, nfeat, nhid1, nout, bias=False, dropout=0., act=F.relu):
+        super().__init__()
 
-    def __init__(self, dim_in: int, dim_hid: int, num_layers: int, species: str, tissue: str, *, dropout: int = 0,
-                 batch_size: int = 500, device: str = "cpu"):
-        self.dense_dim = dim_in
-        self.hidden_dim = dim_hid
-        self.n_layers = num_layers
+        self.gc1 = GraphConvolution(nfeat, nhid1, bias)
+        self.gc2 = GraphConvolution(nhid1, nout, bias)
         self.dropout = dropout
-        self.species = species
-        self.tissue = tissue
-        self.batch_size = batch_size
-        self.device = device
+        self.act = act
 
-        self.postfix = time.strftime("%d_%m_%Y") + "_" + time.strftime("%H:%M:%S")
-        self.prj_path = Path(__file__).resolve().parents[4]
-        self.save_path = (self.prj_path / "saved_models" / "single_modality" / "cell_type_annotation" / "pretrained" /
-                          self.species / "models")
-
-        if not self.save_path.exists():
-            self.save_path.mkdir(parents=True)
-
-    @staticmethod
-    def preprocessing_pipeline(n_components: int = 400, log_level: LogLevel = "INFO"):
-        return Compose(
-            PCACellFeatureGraph(n_components=n_components, split_name="train"),
-            SetConfig({"label_channel": "cell_type"}),
-            log_level=log_level,
-        )
-
-    def fit(self, graph: dgl.DGLGraph, labels: torch.Tensor, epochs: int = 300, lr: float = 1e-3,
-            weight_decay: float = 0, val_ratio: float = 0.2):
-        """Train scDeepsort model.
+    def forward(self, x, adj):
+        """forward function.
 
         Parameters
         ----------
-        graph
-            Training graph.
-        labels
-            Node (cell, gene) labels, -1 for genes.
-        epochs
-            Number of epochs to train the model.
-        lr
-            Learning rate.
-        weight_decay
-            Weight decay regularization strength.
-        val_ratio
-            Ratio of the training data to hold out for validation.
+        x :
+            node features.
+        adj :
+            adjacency matrix.
+
+        Returns
+        -------
+        output : float
+            output of graph convolution network.
 
         """
-        gene_mask = graph.ndata["cell_id"] != -1
-        cell_mask = graph.ndata["cell_id"] == -1
-        num_genes = gene_mask.sum()
-        num_cells = cell_mask.sum()
-        # TODO: remove reliance on num_labels in other methods
-        self.num_labels = labels.max().item() + 1
-
-        perm = torch.randperm(num_cells) + num_genes
-        num_val = int(num_cells * val_ratio)
-        val_idx = perm[:num_val].to(self.device)
-        train_idx = perm[num_val:].to(self.device)
-
-        full_labels = -torch.ones(num_genes + num_cells, dtype=torch.long)
-        full_labels[-num_cells:] = labels
-        graph = graph.to(self.device)
-        graph.ndata["label"] = full_labels.to(self.device)
-
-        self.model = GNN(self.dense_dim, self.num_labels, self.hidden_dim, self.n_layers, num_genes,
-                         activation=nn.ReLU(), dropout=self.dropout).to(self.device)
-        print(self.model)
-
-        self.sampler = NeighborSampler(fanouts=[-1] * self.n_layers, edge_dir="in")
-        self.optimizer = torch.optim.Adam(self.model.parameters(), lr=lr, weight_decay=weight_decay)
-        self.loss_fn = nn.CrossEntropyLoss(reduction="sum")
-
-        print(f"Train Number: {len(train_idx)}, Val Number: {len(val_idx)}")
-        max_val_acc, _train_acc, _epoch = 0, 0, 0
-        best_state_dict = None
-        for epoch in range(epochs):
-            loss = self.cal_loss(graph, train_idx)
-            train_acc = self.evaluate(graph, train_idx)[-1]
-            val_correct, val_unsure, val_acc = self.evaluate(graph, val_idx)
-            if max_val_acc <= val_acc:
-                final_val_correct_num = val_correct
-                final_val_unsure_num = val_unsure
-                _train_acc = train_acc
-                _epoch = epoch
-                max_val_acc = val_acc
-                self.save_model()
-                best_state_dict = deepcopy(self.model.state_dict())
-            print(f">>>>Epoch {epoch:04d}: Train Acc {train_acc:.4f}, Loss {loss / len(train_idx):.4f}, "
-                  f"Val correct {val_correct}, Val unsure {val_unsure}, Val Acc {val_acc:.4f}")
-
-        if best_state_dict is not None:
-            self.model.load_state_dict(best_state_dict)
-
-        print(f"---{self.species} {self.tissue} Best val result:---")
-        print(f"Epoch {_epoch:04d}, Train Acc {_train_acc:.4f}, Val Correct Num {final_val_correct_num}, "
-              f"Val Total Num {len(val_idx)}, Val Unsure Num {final_val_unsure_num}, "
-              f"Val Acc {final_val_correct_num / len(val_idx):.4f}")
+        #self.nnz = x._nnz() if sparse_inputs else None
+
+        #dropout + convolution
+        x = dropout_layer(x, self.dropout)
+        x = self.gc1(x, adj)
+        x = self.act(x)
+        x = dropout_layer(x, self.dropout)
+        x = self.gc2(x, adj)
+
+        return x
+
+
+class DSTGLearner:
+    """DSTGLearner.
+
+    Parameters
+    ----------
+    nfeat : int
+        input dimension.
+    nhid1 : int
+        number of units in the hidden layer (graph convolution).
+    nout : int
+        output dimension.
+    bias : boolean optional
+        include bias term, default False.
+    dropout : float optional
+        dropout rate, default 0.
+    act : optional
+        activation function, default torch functional relu.
+
+    Returns
+    -------
+    None.
+
+    """
+
+    def __init__(self, sc_count, sc_annot, scRNA, mix_count, clust_vr, mix_annot=None, n_hvg=2000, N_p=1000, k_filter=0,
+                 nhid=32, bias=False, dropout=0., device=torch.device("cuda" if torch.cuda.is_available() else "cpu")):
+        super().__init__()
+        self.device = device
+
+        #set adata objects for sc ref and cell mixtures
+        sc_adata = sc.AnnData(sc_count)
+        sc_adata.obs = sc_annot
+        mix_adata = sc.AnnData(mix_count)
+        #mix_adata.obs = true_p
+
+        #pre-process: get variable genes --> normalize --> log1p --> standardize --> out
+        #set scRNA to false if already using pseudo spot data with real spot data
+        #set to true if the reference data is scRNA (to be used for generating pseudo spots)
+        mix_counts, mix_labels, hvgs = pseudo_spatial_process([sc_adata, mix_adata], [sc_annot, mix_annot], clust_vr,
+                                                              scRNA, n_hvg, N_p)
+        mix_labels = [lab.drop(['cell_count', 'total_umi_count', 'n_counts'], axis=1) for lab in mix_labels]
+
+        # create train/val/test split
+        adj_data, features, labels_binary_train, labels_binary_val, labels_binary_test, train_mask, pred_mask, val_mask, test_mask, new_label, true_label = split(
+            mix_counts, mix_labels, pre_process=1, split_val=.8)
+
+        self.labels_binary_train = torch.FloatTensor(labels_binary_train).to(device)
+        self.features = torch.sparse.FloatTensor(
+            torch.LongTensor([features[0][:, 0].tolist(), features[0][:, 1].tolist()]),
+            torch.FloatTensor(features[1])).to(device)
+        self.train_mask = torch.FloatTensor(train_mask).to(device)
+
+        #construct adjacency matrix
+        adj = stAdjConstruct(mix_counts, mix_labels, adj_data, k_filter=k_filter)
+        #preprocess adjacency matrix
+        adj = preprocess_adj(adj)
+
+        self.adj = torch.sparse.FloatTensor(torch.LongTensor([adj.row.tolist(), adj.col.tolist()]),
+                                            torch.FloatTensor(adj.data.astype(np.int32))).to(device)
+
+        nfeat = self.features.size()[1]
+        nout = self.labels_binary_train.size()[1]
+        #initialize GCN module
+        self.model = GCN(nfeat, nhid, nout, bias, dropout).to(device)
 
-    def cal_loss(self, graph: dgl.DGLGraph, idx: torch.Tensor):
-        """Calculate loss.
+    def fit(self, lr=0.005, max_epochs=50, weight_decay=0):
+        """fit function for model training.
 
         Parameters
         ----------
-        graph
-            Input cell-gene graph object.
-        idx
-            1-D tensor containing the indexes of the cell nodes to calculate the loss.
+        lr : float optional
+            learning rate.
+        max_epochs : int optional
+            maximum number of epochs to train.
+        weight_decay : float optional
+            weight decay parameter for optimization (Adam).
 
         Returns
         -------
-        float
-            Averaged loss over all batches.
+        None.
 
         """
-        self.model.train()
-        total_loss = total_size = 0
+        X = self.features  # node features
+        adj = self.adj  # ajacency matrix
+        labels = self.labels_binary_train  # labels of pseudo spots (and real spots if provided)
+        labels_mask = self.train_mask  # mask to indicate which samples to use for training
+
+        #device = self.device
+        model = self.model
+        model.train()
+        optimizer = optim.Adam(model.parameters(), lr=lr, weight_decay=weight_decay)
+
+        for epoch in range(max_epochs):
+            t = time.time()
+
+            y_hat = model(X, adj)
+            loss = masked_softmax_cross_entropy(y_hat, labels, labels_mask)
+
+            if (epoch + 1) % 5 == 0:
+                print("Epoch:", '%04d' % (epoch + 1), "train_loss=", "{:.5f}".format(loss), "time=",
+                      "{:.5f}".format(time.time() - t))
+            #    _ = model(X, adj)
 
-        dataloader = DataLoader(graph=graph, indices=idx, graph_sampler=self.sampler, batch_size=self.batch_size,
-                                shuffle=True)
-        for _, _, blocks in dataloader:
-            blocks = [b.to(self.device) for b in blocks]
-            input_features = blocks[0].srcdata["features"]
-            output_labels = blocks[-1].dstdata["label"]
-            output_predictions = self.model(blocks, input_features)
-
-            loss = self.loss_fn(output_predictions, output_labels)
-            self.optimizer.zero_grad()
+            optimizer.zero_grad()
             loss.backward()
-            self.optimizer.step()
-
-            total_size += (size := blocks[-1].num_dst_nodes())
-            total_loss += loss.item() * size
-
-        return total_loss / total_size
-
-    @torch.no_grad()
-    def evaluate(self, graph: dgl.DGLGraph, idx: torch.Tensor, unsure_rate: float = 2.0):
-        """Evaluate the model on certain cell nodes.
+            optimizer.step()
 
+    def predict(self):
+        """prediction function.
         Parameters
         ----------
-        idx
-            1-D tensor containing the indexes of the cell nodes to be evaluated.
 
         Returns
         -------
-        Tuple[int, int, float]
-            The total number of correct prediction, the total number of unsure prediction, and the accuracy score.
+
+        pred : torch tensor
+            predictions of cell-type proportions.
 
         """
         self.model.eval()
-        total_correct = total_unsure = 0
+        X = self.features
+        adj = self.adj
+        fX = self.model(X, adj)
+        pred = F.softmax(fX, dim=1)
+        return pred
 
-        dataloader = DataLoader(graph=graph, indices=idx, graph_sampler=self.sampler, batch_size=self.batch_size,
-                                shuffle=True)
-        for _, _, blocks in dataloader:
-            blocks = [b.to(self.device) for b in blocks]
-            input_features = blocks[0].srcdata["features"]
-            output_labels = blocks[-1].dstdata["label"]
-            output_predictions = self.model(blocks, input_features)
-
-            for pred, label in zip(output_predictions.cpu(), output_labels.cpu()):
-                max_prob = pred.max().item()
-                if max_prob < unsure_rate / self.num_labels:
-                    total_unsure += 1
-                elif pred.argmax().item() == label:
-                    total_correct += 1
-
-        return total_correct, total_unsure, total_correct / len(idx)
-
-    def save_model(self):
-        """Save the model at the save_path."""
-        state = {"model": self.model.state_dict(), "optimizer": self.optimizer.state_dict()}
-        torch.save(state, self.save_path / f"{self.species}-{self.tissue}.pt")
-
-    def load_model(self):
-        """Load the model from the model path."""
-        filename = f"{self.species}-{self.tissue}.pt"
-        model_path = self.prj_path / "pretrained" / self.species / "models" / filename
-        state = torch.load(model_path, map_location=self.device)
-        self.model.load_state_dict(state["model"])
-
-    @torch.no_grad()
-    def predict_proba(self, graph: dgl.DGLGraph):
-        """Perform inference on a test dataset.
+    def score(self, pred, true_prop, score_metric='ce'):
+        """Model performance score.
 
         Parameters
         ----------
-        graph
-            Input cell-gene graph to be predicted.
+        pred :
+            predicted cell-type proportions.
+        true_prop :
+            true cell-type proportions.
+        score_metric :
+            metric used to assess prediction performance.
 
         Returns
         -------
-        np.ndarray
-            2-D array of predicted probabilities of the cell-types, where rows are cells and columns are cell-types.
+        loss : float
+            loss between predicted and true labels.
 
         """
+        true_prop = true_prop.to(self.device)
         self.model.eval()
+        if score_metric == 'ce':
+            loss = F.cross_entropy(pred, true_prop)
+        elif score_metric == 'mse':
+            loss = ((pred / torch.sum(pred, 1, keepdims=True) -
+                     true_prop / torch.sum(true_prop, 1, keepdims=True))**2).mean()
+        return loss.detach().item()
 
-        cell_mask = graph.ndata["cell_id"] == -1
-        idx = torch.where(cell_mask)[0].to(self.device)
-        graph = graph.to(self.device)
-
-        logits = torch.zeros(graph.number_of_nodes(), self.num_labels)
-        dataloader = DataLoader(graph=graph, indices=idx, graph_sampler=self.sampler, batch_size=self.batch_size)
-        for _, output_nodes, blocks in dataloader:
-            blocks = [b.to(self.device) for b in blocks]
-            input_features = blocks[0].srcdata["features"]
-            logits[output_nodes] = self.model(blocks, input_features).detach().cpu()
 
-        pred_prob = nn.functional.softmax(logits[cell_mask], dim=-1).numpy()
-        return pred_prob
+def dropout_layer(x, dropout):
+    """dropout_layer.
+    Parameters
+    ----------
+    x:
+        input to dropout layer.
+    dropout : float
+        dropout rate (between 0 and 1).
+
+    Returns
+    -------
+    out : torch tensor
+        dropout output.
+    """
+    if x.is_sparse:
+        #sparse input features
+        out = sparse_dropout(x, dropout)
+        return out
+    else:
+        out = F.dropout(x, dropout)
+        return out
 
-    def predict(self, graph: dgl.DGLGraph, unsure_rate: float = 2.0, return_unsure: bool = False):
-        """Perform prediction on all test datasets.
 
-        Parameters
-        ----------
-        graph
-            Input cell-gene grahp to be predicted.
-        unsure_rate
-            Determine the threshold of the maximum predicted probability under which the predictions are considered
-            uncertain.
-        return_unsure
-            If set to ``True``, then return an indicator array that indicates whether a prediction is uncertain.
+def sparse_dropout(x, dropout):
+    """sparse_dropout.
+    Parameters
+    ----------
+    x:
+        input to dropout layer.
+    dropout : float
+        dropout rate (between 0 and 1).
+
+    Returns
+    -------
+    out * (1. / (1-dropout)) : torch tensor
+        dropout output.
+    """
 
-        """
-        pred_prob = self.predict_proba(graph)
+    noise_shape = x._nnz()
+    random_tensor = (1 - dropout) + torch.rand(noise_shape).to(x.device)
+    dropout_mask = torch.floor(random_tensor).type(torch.bool)
+    i = x._indices()
+    v = x._values()
 
-        pred = pred_prob.argmax(1)
-        unsure = pred_prob.max(1) < unsure_rate / self.num_labels
+    i = i[:, dropout_mask]
+    v = v[dropout_mask]
 
-        return (pred, unsure) if return_unsure else pred
+    out = torch.sparse.FloatTensor(i, v, x.shape).to(x.device)
+    return out * (1. / (1 - dropout))
+
+
+"""Softmax cross-entropy loss with masking."""
+
+
+def masked_softmax_cross_entropy(preds, labels, mask):
+    """masked_softmax_cross_entropy.
+    Parameters
+    ----------
+    preds:
+        cell-type proportion predictions from dstg model.
+    labels :
+        true cell-type proportion labels.
+    mask :
+        mask to indicate which samples to use in computing loss.
+
+    Returns
+    -------
+    loss : float
+        cross entropy loss between true and predicted cell-type proportions (mean reduced).
+    """
+    if (mask is None):
+        loss = F.cross_entropy(preds, labels, reduction='mean')
+        return loss
+    else:
+        loss = F.cross_entropy(preds, labels, reduction='none')
+        mask = mask.type(torch.float32)
+        mask /= torch.mean(mask)
+        loss *= mask
+        loss = torch.mean(loss)
+        return loss
```

### Comparing `pydance-1.0.0/dance/modules/single_modality/clustering/graphsc.py` & `pydance-1.0.0rc0/dance/modules/single_modality/clustering/graphsc.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,212 +4,95 @@
 
 Reference
 ----------
 Ciortan, Madalina, and Matthieu Defrance. "GNN-based embedding for clustering scRNA-seq data." Bioinformatics 38.4
 (2022) 1037-1044.
 
 """
-import dgl
+
+import time
+
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from dgl import DGLError
+from dgl import DGLError, DGLGraph
 from dgl import function as fn
 from dgl.nn.pytorch import GraphConv
 from dgl.utils import expand_as_pair
 from sklearn.cluster import KMeans
+from sklearn.decomposition import PCA
+from sklearn.metrics import adjusted_rand_score, calinski_harabasz_score, normalized_mutual_info_score, silhouette_score
 from torch.nn.functional import binary_cross_entropy_with_logits as BCELoss
 from tqdm import tqdm
 
-from dance import logger
-from dance.modules.base import BaseClusteringMethod
-from dance.transforms import AnnDataTransform, Compose, SetConfig
-from dance.transforms.graph import PCACellFeatureGraph
-from dance.typing import Any, Literal, LogLevel, Optional
-from dance.utils import get_device
-
 
-class GraphSC(BaseClusteringMethod):
+class GraphSC:
     """GraphSC class.
 
     Parameters
     ----------
-    agg
-        Aggregation layer.
-    activation
-        Activation function.
-    in_feats
-        Dimension of input feature
-    n_hidden
-        Number of hidden layer.
-    hidden_dim
-        Input dimension of hidden layer 1.
-    hidden_1
-        Output dimension of hidden layer 1.
-    hidden_2
-        Output dimension of hidden layer 2.
-    dropout
-        Dropout rate.
-    n_layers
-        Number of graph convolutional layers.
-    hidden_relu
-        Use relu activation in hidden layers or not.
-    hidden_bn
-        Use batch norm in hidden layers or not.
-    cluster_method
-        Method for clustering.
-    num_workers
-        Number of workers.
-    device
-        Computation device to use.
+    args : argparse.Namespace
+        a Namespace contains arguments of GCNAE. For details of parameters in parser args, please refer to link (parser help document).
 
     """
 
-    def __init__(
-        self,
-        agg: str = "sum",
-        activation: str = "relu",
-        in_feats: int = 50,
-        n_hidden: int = 1,
-        hidden_dim: int = 200,
-        hidden_1: int = 300,
-        hidden_2: int = 0,
-        dropout: float = 0.1,
-        n_layers: int = 1,
-        hidden_relu: bool = False,
-        hidden_bn: bool = False,
-        n_clusters: int = 10,
-        cluster_method: Literal["kmeans", "leiden"] = "kmeans",
-        num_workers: int = 1,
-        device: str = "auto",
-    ):
+    def __init__(self, args):
         super().__init__()
-        self.n_layers = n_layers
-        self.n_clusters = n_clusters
-        self.cluster_method = cluster_method
-        self.num_workers = num_workers
-        self.device = get_device(device)
-
-        self.model = GCNAE(
-            agg=agg,
-            activation=activation,
-            in_feats=in_feats,
-            n_hidden=n_hidden,
-            hidden_dim=hidden_dim,
-            hidden_1=hidden_1,
-            hidden_2=hidden_2,
-            dropout=dropout,
-            n_layers=n_layers,
-            hidden_relu=hidden_relu,
-            hidden_bn=hidden_bn,
-        ).to(self.device)
-
-    @staticmethod
-    def preprocessing_pipeline(n_top_genes: int = 3000, normalize_weights: str = "log_per_cell", n_components: int = 50,
-                               normalize_edges: bool = False, log_level: LogLevel = "INFO"):
-        transforms = [
-            AnnDataTransform(sc.pp.filter_genes, min_counts=3),
-            AnnDataTransform(sc.pp.filter_cells, min_counts=1),
-            AnnDataTransform(sc.pp.normalize_total),
-            AnnDataTransform(sc.pp.log1p),
-            AnnDataTransform(sc.pp.highly_variable_genes, min_mean=0.0125, max_mean=4, flavor="cell_ranger",
-                             min_disp=0.5, n_top_genes=n_top_genes, subset=True),
-        ]
-
-        if normalize_weights == "log_per_cell":
-            transforms.extend([
-                AnnDataTransform(sc.pp.log1p),
-                AnnDataTransform(sc.pp.normalize_total, target_sum=1),
-            ])
-        elif normalize_weights == "per_cell":
-            transforms.append(AnnDataTransform(sc.pp.normalize_total, target_sum=1))
-        elif normalize_weights != "none":
-            raise ValueError(f"Unknown normalization option {normalize_weights!r}."
-                             "Available options are: 'none', 'log_per_cell', 'per_cell'")
-
-        # Cell-gene graph construction
-        transforms.extend([
-            PCACellFeatureGraph(
-                n_components=n_components,
-                normalize_edges=normalize_edges,
-                feat_norm_mode="standardize",
-            ),
-            SetConfig({
-                "feature_channel": "CellFeatureGraph",
-                "feature_channel_type": "uns",
-                "label_channel": "Group",
-            }),
-        ])
-
-        return Compose(*transforms, log_level=log_level)
-
-    def fit(
-        self,
-        g: dgl.DGLGraph,
-        y: Optional[Any] = None,
-        *,
-        epochs: int = 100,
-        lr: float = 1e-5,
-        batch_size: int = 128,
-        show_epoch_ari: bool = False,
-        eval_epoch: bool = False,
-    ):
+        self.args = args
+        self.model = GCNAE(args).to(get_device(args.use_cpu))
+
+    def fit(self, n_epochs, dataloader, n_clusters, lr, cluster=["KMeans"]):
         """Train graph-sc.
 
         Parameters
         ----------
-        g
-            Input cell-gene graph.
-        y
-            Not used, for compatibility with the BaseClusteringMethod class.
-        epochs
-            Number of epochs.
-        lr
-            Learning rate.
-        batch_size
-            Batch size.
-        show_epoch_ari
-            Show ARI score for each epoch
-        eval_epoch
-            Evaluate every epoch.
+        n_epochs : int
+            number of epochs.
+        dataloader :
+            dataloader for training.
+        n_clusters : int
+            number of clusters.
+        lr : float
+            learning rate.
+        cluster : list optional
+            clustering method.
 
-        """
-        g.ndata["order"] = g.ndata["label"] = g.ndata["feat_id"]
-        train_ids = np.where(g.ndata["label"] != -1)[0]
-        sampler = dgl.dataloading.MultiLayerFullNeighborSampler(self.n_layers)
-        dataloader = dgl.dataloading.NodeDataLoader(g, train_ids, sampler, batch_size=batch_size, shuffle=True,
-                                                    drop_last=False, num_workers=self.num_workers)
+        Returns
+        -------
+        None.
 
-        device = get_device(self.device)
+        """
+        device = get_device(self.args.use_cpu)
         optim = torch.optim.Adam(self.model.parameters(), lr=lr)
         losses = []
-        aris = []
+        aris_kmeans = []
         Z = {}
-
-        for epoch in tqdm(range(epochs)):
+        for epoch in tqdm(range(n_epochs)):
             self.model.train()
             z = []
             y = []
             order = []
 
             for input_nodes, output_nodes, blocks in dataloader:
                 blocks = [b.to(device) for b in blocks]
-                input_features = blocks[0].srcdata["features"]
+                input_features = blocks[0].srcdata['features']
                 g = blocks[-1]
+                degs = g.in_degrees().float()
 
                 adj_logits, emb = self.model.forward(blocks, input_features)
                 z.extend(emb.detach().cpu().numpy())
                 if "label" in blocks[-1].dstdata:
                     y.extend(blocks[-1].dstdata["label"].cpu().numpy())
                 order.extend(blocks[-1].dstdata["order"].cpu().numpy())
 
-                adj = g.adjacency_matrix().to_dense().to(device)
+                adj = g.adjacency_matrix().to_dense()
                 adj = adj[g.dstnodes()]
                 pos_weight = torch.Tensor([float(adj.shape[0] * adj.shape[0] - adj.sum()) / adj.sum()])
                 factor = float((adj.shape[0] * adj.shape[0] - adj.sum()) * 2)
                 if factor == 0:
                     factor = 1
                 norm = adj.shape[0] * adj.shape[0] / factor
                 adj_logits, _ = self.model.forward(blocks, input_features)
@@ -225,155 +108,238 @@
             order = np.argsort(order)
             z = z[order]
             y = y[order]
             if pd.isnull(y[0]):
                 y = None
             self.z = z
 
-            if eval_epoch:
-                score = self.score(None, y)
-                aris.append(score)
-                if show_epoch_ari:
-                    logger.info(f"epoch {epoch:4d}, ARI {score:.4f}")
-                z_ = {f"epoch{epoch}": z}
+            if self.args.eval_epoch:
+                score = self.score(y, n_clusters, cluster=cluster)
+                aris_kmeans.append(score["kmeans_ari"])
+                if self.args.show_epoch_ari:
+                    print(f'epoch {epoch}, ARI {score.get("kmeans_ari")}')
+                z_ = {f'epoch{epoch}': z}
                 Z = {**Z, **z_}
 
-            elif epoch == epochs - 1:
+            elif epoch == n_epochs - 1:
                 self.z = z
 
-        if eval_epoch:
-            index = np.argmax(aris)
-            self.z = Z[f"epoch{index}"]
+        if self.args.eval_epoch:
+            index = np.argmax(aris_kmeans)
+            self.z = Z[f'epoch{index}']
 
-    def predict(self, x: Optional[Any] = None):
+    def predict(self, n_clusters, cluster=["KMeans"]):
         """Get predictions from the graph autoencoder model.
 
         Parameters
         ----------
-        x
-            Not used, for compatibility with BaseClusteringMethod class.
+        n_clusters : int
+            number of clusters.
+        cluster : list optional
+            clustering method.
 
         Returns
         -------
-        pred
-            Prediction of given clustering method.
+        pred : dict
+            prediction of given clustering method.
 
         """
-        if self.cluster_method == "kmeans":
-            kmeans = KMeans(n_clusters=self.n_clusters, init="k-means++", random_state=5, n_init=10)
-            pred = kmeans.fit_predict(self.z)
-        elif self.cluster_method == "leiden":
-            pred = run_leiden(self.z)
-        else:
-            raise ValueError(f"Unknown clustering {self.cluster_method}, available options are: 'kmeans', 'leiden'")
+        z = self.z
+        device = get_device(self.args.use_cpu)
+        pred = {}
+
+        if "KMeans" in cluster:
+            kmeans = KMeans(n_clusters=n_clusters, init="k-means++", random_state=5)
+            kmeans_pred = {"kmeans_pred": kmeans.fit_predict(z)}
+            pred = {**pred, **kmeans_pred}
+
+        if "Leiden" in cluster:
+            leiden_pred = {"leiden_pred": run_leiden(z)}
+            pred = {**pred, **leiden_pred}
+
         return pred
 
+    def score(self, y, n_clusters, plot=False, cluster=["KMeans"]):
+        """Evaluate the graph autoencoder model.
+
+        Parameters
+        ----------
+        y : list
+            true labels.
+        n_clusters : int
+            number of clusters.
+        plot : bool optional
+            show plot or not.
+        cluster : list optional
+            clustering method.
+
+        Returns
+        -------
+        scores : dict
+            metric evaluation scores.
+
+        """
+        z = self.z
+        device = get_device(self.args.use_cpu)
+        self.model.eval()
+
+        k_start = time.time()
+        scores = {"ae_end": k_start}
+
+        if "KMeans" in cluster:
+            kmeans = KMeans(n_clusters=n_clusters, init="k-means++", random_state=5)
+            kmeans_pred = kmeans.fit_predict(z)
+            ari_k = None
+            nmi_k = None
+            if y is not None:
+                ari_k = round(adjusted_rand_score(y, kmeans_pred), 4)
+                nmi_k = round(normalized_mutual_info_score(y, kmeans_pred), 4)
+            sil_k = silhouette_score(z, kmeans_pred)
+            cal_k = calinski_harabasz_score(z, kmeans_pred)
+            k_end = time.time()
+            scores_k = {
+                "kmeans_ari": ari_k,
+                "kmeans_nmi": nmi_k,
+                "kmeans_sil": sil_k,
+                "kmeans_cal": cal_k,
+                "kmeans_pred": kmeans_pred,
+                "kmeans_time": k_end - k_start,
+            }
+            scores = {**scores, **scores_k}
+
+        if "Leiden" in cluster:
+            l_start = time.time()
+            leiden_pred = run_leiden(z)
+            ari_l = None
+            nmi_l = None
+            if y is not None:
+                ari_l = round(adjusted_rand_score(y, leiden_pred), 4)
+                nmi_l = round(normalized_mutual_info_score(y, leiden_pred), 4)
+            sil_l = silhouette_score(z, leiden_pred)
+            cal_l = calinski_harabasz_score(z, leiden_pred)
+            l_end = time.time()
+            scores_l = {
+                "leiden_ari": ari_l,
+                "leiden_nmi": nmi_l,
+                "leiden_sil": sil_l,
+                "leiden_cal": cal_l,
+                "leiden_pred": leiden_pred,
+                "leiden_time": l_end - l_start,
+            }
+            scores = {**scores, **scores_l}
+
+        if plot:
+            pca = PCA(2).fit_transform(z)
+            plt.figure(figsize=(12, 4))
+            plt.subplot(131)
+            plt.title("Ground truth")
+            plt.scatter(pca[:, 0], pca[:, 1], c=y, s=4)
+
+            plt.subplot(132)
+            plt.title("K-Means pred")
+            plt.scatter(pca[:, 0], pca[:, 1], c=kmeans_pred, s=4)
+
+            plt.subplot(133)
+            plt.title("Leiden pred")
+            plt.scatter(pca[:, 0], pca[:, 1], c=leiden_pred, s=4)
+            plt.show()
+        return scores
+
 
 class GCNAE(nn.Module):
     """Graph convolutional autoencoder class.
 
     Parameters
     ----------
-    agg
-        Aggregation layer.
-    activation
-        Activation function.
-    in_feats
-        Dimension of input feature
-    n_hidden
-        Number of hidden layer.
-    hidden_dim
-        Input dimension of hidden layer 1.
-    hidden_1
-        Output dimension of hidden layer 1.
-    hidden_2
-        Output dimension of hidden layer 2.
-    dropout
-        Dropout rate.
-    n_layers
-        Number of graph convolutional layers.
-    hidden_relu
-        Use relu activation in hidden layers or not.
-    hidden_bn
-        Use batch norm in hidden layers or not.
+    args : argparse.Namespace
+        a Namespace contains arguments of scDSC. For details of parameters in parser args, please refer to link (parser help document).
+    agg : str
+        aggregation layer.
+    activation :str
+        activation function.
+    in_feats : int
+        dimension of input feature
+    n_hidden : int
+        number of hidden layer.
+    hidden_dim :int
+        input dimension of hidden layer 1.
+    hidden_1 : int
+        output dimension of hidden layer 1.
+    hidden_2 : int
+        output dimension of hidden layer 2.
+    dropout : float
+        dropout rate.
+    n_layers :int
+        number of graph convolutional layers.
+    hidden_relu : bool
+        use relu activation in hidden layers or not.
+    hidden_bn : bool
+        use batch norm in hidden layers or not.
 
     Returns
     -------
-    adj_rec
-        Reconstructed adjacency matrix.
-    x
-        Embedding.
+    adj_rec :
+        reconstructed adjacency matrix.
+    x :
+        embedding.
 
     """
 
-    def __init__(
-        self,
-        *,
-        agg: str,
-        activation: str,
-        in_feats: int,
-        n_hidden: int,
-        hidden_dim: int,
-        hidden_1: int,
-        hidden_2: int,
-        dropout: float,
-        n_layers: int,
-        hidden_relu: bool,
-        hidden_bn: bool,
-    ):
-        super().__init__()
+    def __init__(self, args):
 
-        self.agg = agg
+        super().__init__()
+        self.args = args
+        self.agg = args.agg
 
-        if activation == "gelu":
+        if args.activation == 'gelu':
             activation = F.gelu
-        elif activation == "prelu":
+        elif args.activation == 'prelu':
             activation = F.prelu
-        elif activation == "relu":
+        elif args.activation == 'relu':
             activation = F.relu
-        elif activation == "leaky_relu":
+        elif args.activation == 'leaky_relu':
             activation = F.leaky_relu
 
-        if n_hidden == 0:
+        if args.n_hidden == 0:
             hidden = None
-        elif n_hidden == 1:
-            hidden = [hidden_1]
-        elif n_hidden == 2:
-            hidden = [hidden_1, hidden_2]
+        elif args.n_hidden == 1:
+            hidden = [args.hidden_1]
+        elif args.n_hidden == 2:
+            hidden = [args.hidden_1, args.hidden_2]
 
-        if dropout != 0:
-            self.dropout = nn.Dropout(p=dropout)
+        if args.dropout != 0:
+            self.dropout = nn.Dropout(p=args.dropout)
         else:
             self.dropout = None
 
-        self.layer1 = WeightedGraphConv(in_feats=in_feats, out_feats=hidden_dim, activation=activation)
-        if n_layers == 2:
-            self.layer2 = WeightedGraphConv(in_feats=hidden_dim, out_feats=hidden_dim, activation=activation)
+        self.layer1 = WeightedGraphConv(in_feats=args.in_feats, out_feats=args.hidden_dim, activation=activation)
+        if args.n_layers == 2:
+            self.layer2 = WeightedGraphConv(in_feats=args.hidden_dim, out_feats=args.hidden_dim, activation=activation)
         self.decoder = InnerProductDecoder(activation=lambda x: x)
         self.hidden = hidden
         if hidden is not None:
             enc = []
             for i, s in enumerate(hidden):
                 if i == 0:
-                    enc.append(nn.Linear(hidden_dim, hidden[i]))
+                    enc.append(nn.Linear(args.hidden_dim, hidden[i]))
                 else:
                     enc.append(nn.Linear(hidden[i - 1], hidden[i]))
-                if hidden_bn and i != len(hidden):
+                if args.hidden_bn and i != len(hidden):
                     enc.append(nn.BatchNorm1d(hidden[i]))
-                if hidden_relu and i != len(hidden):
+                if args.hidden_relu and i != len(hidden):
                     enc.append(nn.ReLU())
             self.encoder = nn.Sequential(*enc)
 
     def forward(self, blocks, features):
-        x = blocks[0].srcdata["features"]
+        x = blocks[0].srcdata['features']
         for i in range(len(blocks)):
             with blocks[i].local_scope():
                 if self.dropout is not None:
                     x = self.dropout(x)
-                blocks[i].srcdata["h"] = x
+                blocks[i].srcdata['h'] = x
                 if i == 0:
                     x = self.layer1(blocks[i], x, agg=self.agg)
                 else:
                     x = self.layer2(blocks[i], x, agg=self.agg)
         if self.hidden is not None:
             x = self.encoder(x)
         adj_rec = self.decoder(x)
@@ -381,23 +347,23 @@
 
 
 class InnerProductDecoder(nn.Module):
     """Inner product decoder class.
 
     Parameters
     ----------
-    activation
-        Activation function.
-    dropout
-        Dropout rate.
+    activation : optional
+        activation function.
+    dropout : float optional
+        dropout rate.
 
     Returns
     -------
-    adj
-        Reconstructed adjacency matrix.
+    adj :
+        reconstructed adjacency matrix.
 
     """
 
     def __init__(self, activation=torch.sigmoid, dropout=0.1):
         super().__init__()
         self.dropout = dropout
         self.activation = activation
@@ -412,63 +378,63 @@
     """Adaptation of the dgl GraphConv model to use edge weights."""
 
     def edge_selection_simple(self, edges):
         """Edge selection.
 
         Parameters
         ----------
-        edges
-            Edges of graph.
+        edges :
+            edges of graph.
 
         """
-        return {"m": edges.src["h"] * edges.data["weight"]}
+        return {'m': edges.src['h'] * edges.data['weight']}
 
     def forward(self, graph, feat, weight=None, agg="sum"):
         with graph.local_scope():
             if not self._allow_zero_in_degree:
                 if (graph.in_degrees() == 0).any():
-                    raise DGLError("There are 0-in-degree nodes in the graph, "
-                                   "output for those nodes will be invalid. "
-                                   "This is harmful for some applications, "
-                                   "causing silent performance regression. "
-                                   "Adding self-loop on the input graph by "
-                                   "calling `g = dgl.add_self_loop(g)` will resolve "
-                                   "the issue. Setting ``allow_zero_in_degree`` "
-                                   "to be `True` when constructing this module will "
-                                   "suppress the check and let the code run.")
+                    raise DGLError('There are 0-in-degree nodes in the graph, '
+                                   'output for those nodes will be invalid. '
+                                   'This is harmful for some applications, '
+                                   'causing silent performance regression. '
+                                   'Adding self-loop on the input graph by '
+                                   'calling `g = dgl.add_self_loop(g)` will resolve '
+                                   'the issue. Setting ``allow_zero_in_degree`` '
+                                   'to be `True` when constructing this module will '
+                                   'suppress the check and let the code run.')
 
             # (BarclayII) For RGCN on heterogeneous graphs we need to support GCN on bipartite.
             feat_src, feat_dst = expand_as_pair(feat, graph)
-            if self._norm == "both":
+            if self._norm == 'both':
                 degs = graph.out_degrees().float().clamp(min=1)
                 norm = torch.pow(degs, -0.5)
                 shp = norm.shape + (1, ) * (feat_src.dim() - 1)
                 norm = torch.reshape(norm, shp)
                 feat_src = feat_src * norm
 
             if weight is not None:
                 if self.weight is not None:
-                    raise DGLError("External weight is provided while at the same time the"
-                                   " module has defined its own weight parameter. Please"
-                                   " create the module with flag weight=False.")
+                    raise DGLError('External weight is provided while at the same time the'
+                                   ' module has defined its own weight parameter. Please'
+                                   ' create the module with flag weight=False.')
             else:
                 weight = self.weight
 
             if weight is not None:
                 feat_src = torch.matmul(feat_src, weight)
-            graph.srcdata["h"] = feat_src
+            graph.srcdata['h'] = feat_src
             if agg == "sum":
-                graph.update_all(self.edge_selection_simple, fn.sum(msg="m", out="h"))
+                graph.update_all(self.edge_selection_simple, fn.sum(msg='m', out='h'))
             if agg == "mean":
-                graph.update_all(self.edge_selection_simple, fn.mean(msg="m", out="h"))
-            rst = graph.dstdata["h"]
-            if self._norm != "none":
+                graph.update_all(self.edge_selection_simple, fn.mean(msg='m', out='h'))
+            rst = graph.dstdata['h']
+            if self._norm != 'none':
 
                 degs = graph.in_degrees().float().clamp(min=1)
-                if self._norm == "both":
+                if self._norm == 'both':
                     norm = torch.pow(degs, -0.5)
                 else:
                     norm = 1.0 / degs
                 shp = norm.shape + (1, ) * (feat_dst.dim() - 1)
                 norm = torch.reshape(norm, shp)
                 rst = rst * norm
 
@@ -486,70 +452,73 @@
     parameter."""
 
     def edge_selection_simple(self, edges):
         """Edge selection.
 
         Parameters
         ----------
-        edges
-            Edges of graph.
+        edges :
+            edges of graph.
 
         """
-        number_of_edges = edges.src["h"].shape[0]
+        number_of_edges = edges.src['h'].shape[0]
         indices = np.expand_dims(np.array([self.gene_num + 1] * number_of_edges, dtype=np.int32), axis=1)
-        src_id, dst_id = edges.src["id"].cpu().numpy(), edges.dst["id"].cpu().numpy()
+        src_id, dst_id = edges.src['id'].cpu().numpy(), edges.dst['id'].cpu().numpy()
         indices = np.where((src_id >= 0) & (dst_id < 0), src_id, indices)  # gene->cell
         indices = np.where((dst_id >= 0) & (src_id < 0), dst_id, indices)  # cell->gene
         indices = np.where((dst_id >= 0) & (src_id >= 0), self.gene_num, indices)  # gene-gene
-        h = edges.src["h"] * self.alpha[indices.squeeze()]
-        return {"m": h}
+        h = edges.src['h'] * self.alpha[indices.squeeze()]
+        return {'m': h}
+
+    #         return {'m': h * edges.data['weight']}
 
     def forward(self, graph, feat, weight=None, alpha=None, gene_num=None):
         self.alpha = alpha
         self.gene_num = gene_num
         with graph.local_scope():
             if not self._allow_zero_in_degree:
                 if (graph.in_degrees() == 0).any():
-                    raise DGLError("There are 0-in-degree nodes in the graph, "
-                                   "output for those nodes will be invalid. "
-                                   "This is harmful for some applications, "
-                                   "causing silent performance regression. "
-                                   "Adding self-loop on the input graph by "
-                                   "calling `g = dgl.add_self_loop(g)` will resolve "
-                                   "the issue. Setting ``allow_zero_in_degree`` "
-                                   "to be `True` when constructing this module will "
-                                   "suppress the check and let the code run.")
+                    raise DGLError('There are 0-in-degree nodes in the graph, '
+                                   'output for those nodes will be invalid. '
+                                   'This is harmful for some applications, '
+                                   'causing silent performance regression. '
+                                   'Adding self-loop on the input graph by '
+                                   'calling `g = dgl.add_self_loop(g)` will resolve '
+                                   'the issue. Setting ``allow_zero_in_degree`` '
+                                   'to be `True` when constructing this module will '
+                                   'suppress the check and let the code run.')
 
             # (BarclayII) For RGCN on heterogeneous graphs we need to support GCN on bipartite.
             feat_src, feat_dst = expand_as_pair(feat, graph)
-            if self._norm == "both":
+            #             print(f"feat_src : {feat_src.shape}, feat_dst {feat_dst.shape}")
+            if self._norm == 'both':
                 degs = graph.out_degrees().float().clamp(min=1)
                 norm = torch.pow(degs, -0.5)
                 shp = norm.shape + (1, ) * (feat_src.dim() - 1)
                 norm = torch.reshape(norm, shp)
                 feat_src = feat_src * norm
 
             if weight is not None:
                 if self.weight is not None:
-                    raise DGLError("External weight is provided while at the same time the"
-                                   " module has defined its own weight parameter. Please"
-                                   " create the module with flag weight=False.")
+                    raise DGLError('External weight is provided while at the same time the'
+                                   ' module has defined its own weight parameter. Please'
+                                   ' create the module with flag weight=False.')
                 else:
                     feat_src = torch.matmul(feat_src, weight)
             else:
                 weight = self.weight
 
-            graph.srcdata["h"] = feat_src
-            graph.update_all(self.edge_selection_simple, fn.sum(msg="m", out="h"))
-            rst = graph.dstdata["h"]
+            graph.srcdata['h'] = feat_src
+            graph.update_all(self.edge_selection_simple, fn.sum(msg='m', out='h'))
+            rst = graph.dstdata['h']
 
-            if self._norm != "none":
+            if self._norm != 'none':
 
                 degs = graph.in_degrees().float().clamp(min=1)
-                if self._norm == "both":
+                if self._norm == 'both':
                     norm = torch.pow(degs, -0.5)
                 else:
                     norm = 1.0 / degs
                 shp = norm.shape + (1, ) * (feat_dst.dim() - 1)
                 norm = torch.reshape(norm, shp)
                 rst = rst * norm
 
@@ -563,22 +532,43 @@
 
 
 def run_leiden(data):
     """Performs Leiden community detection on given data.
 
     Parameters
     ----------
-    data
-        Aata for leiden
+    data :
+        data for leiden
 
     Returns
     -------
-    pred
-        Prediction of leiden.
+    pred : list
+        prediction of leiden.
 
     """
     adata = sc.AnnData(data)
-    sc.pp.neighbors(adata, use_rep="X", n_neighbors=300, n_pcs=0)
+    sc.pp.neighbors(adata, use_rep='X', n_neighbors=300, n_pcs=0)
     sc.tl.leiden(adata)
-    pred = adata.obs["leiden"].to_list()
+    pred = adata.obs['leiden'].to_list()
     pred = [int(x) for x in pred]
     return pred
+
+
+def get_device(use_cpu=False):
+    """Get device for training.
+
+    Parameters
+    ----------
+    use_cpu : bool optional
+        use cpu or not.
+
+    Returns
+    -------
+    device :
+        torch device.
+
+    """
+    if torch.cuda.is_available() and use_cpu == False:
+        device = torch.device('cuda')
+    else:
+        device = torch.device('cpu')
+    return device
```

### Comparing `pydance-1.0.0/dance/modules/single_modality/clustering/scdcc.py` & `pydance-1.0.0rc0/dance/modules/single_modality/clustering/scdcc.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,207 +4,202 @@
 
 Reference
 ----------
 Tian, Tian, et al. "Model-based deep embedding for constrained clustering analysis of single cell RNA-seq data."
 Nature communications 12.1 (2021): 1-12.
 
 """
+
 import math
+import os
 
 import numpy as np
-import scanpy as sc
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
+from sklearn import metrics
 from sklearn.cluster import KMeans
+from torch.autograd import Variable
 from torch.nn import Parameter
 from torch.utils.data import DataLoader, TensorDataset
 
-from dance import logger
-from dance.modules.base import BaseClusteringMethod, TorchNNPretrain
-from dance.transforms import AnnDataTransform, Compose, SaveRaw, SetConfig
-from dance.typing import Any, List, LogLevel, Optional, Tuple
-from dance.utils import get_device
 from dance.utils.loss import ZINBLoss
+from dance.utils.metrics import cluster_acc
 
 
-def buildNetwork(layers: List[int], network_type: str, activation: str = "relu"):
+def buildNetwork(layers, type, activation="relu"):
     """Build network layer.
 
     Parameters
     ----------
-    layers
-        Dimensions of layers.
-    network_type
-        Type of network.
-    activation
-        Activation function.
-
+    layers : list
+        dimensions of layers.
+    type : str
+        type of network.
+    activation : str optional
+        activation function.
 
     Returns
     -------
-    Built network.
+    net :
+        torch.nn network.
 
     """
     net = []
     for i in range(1, len(layers)):
         net.append(nn.Linear(layers[i - 1], layers[i]))
         if activation == "relu":
             net.append(nn.ReLU())
         elif activation == "sigmoid":
             net.append(nn.Sigmoid())
     net = nn.Sequential(*net)
     return net
 
 
-class ScDCC(nn.Module, TorchNNPretrain, BaseClusteringMethod):
-    """ScDCC class.
+class ScDCC(nn.Module):
+    """scDCC class.
 
     Parameters
     ----------
-    input_dim
-        Dimension of encoder input.
-    z_dim
-        Dimension of embedding.
-    n_clusters
-        Number of clusters.
-    encodeLayer
-        Dimensions of encoder layers.
-    decodeLayer
-        Dimensions of decoder layers.
-    activation
-        Activation function.
-    sigma
-        Parameter of Gaussian noise.
-    alpha
-        Parameter of soft assign.
-    gamma
-        Parameter of cluster loss.
-    ml_weight
-        Parameter of must-link loss.
-    cl_weight
-        Parameter of cannot-link loss.
-    device
-        Computation device.
+    input_dim : int
+        dimension of encoder input.
+    z_dim : int
+        dimension of embedding.
+    n_clusters : int
+        number of clusters.
+    encodeLayer : list optional
+        dimensions of encoder layers.
+    decodeLayer : list optional
+        dimensions of decoder layers.
+    activation : str optional
+        activation function.
+    sigma : float optional
+        parameter of Gaussian noise.
+    alpha : float optional
+        parameter of soft assign.
+    gamma : float optional
+        parameter of cluster loss.
+    ml_weight : float optional
+        parameter of must-link loss.
+    cl_weight : float optional
+        parameter of cannot-link loss.
 
     """
 
-    def __init__(
-        self,
-        input_dim: int,
-        z_dim: int,
-        n_clusters: int,
-        encodeLayer: List[int],
-        decodeLayer: List[int],
-        activation: str = "relu",
-        sigma: float = 1.,
-        alpha: float = 1.,
-        gamma: float = 1.,
-        ml_weight: float = 1.,
-        cl_weight: float = 1.,
-        device: str = "auto",
-        pretrain_path: Optional[str] = None,
-    ):
+    def __init__(self, input_dim, z_dim, n_clusters, encodeLayer=[], decodeLayer=[], activation="relu", sigma=1.,
+                 alpha=1., gamma=1., ml_weight=1., cl_weight=1.):
         super().__init__()
         self.z_dim = z_dim
         self.n_clusters = n_clusters
         self.activation = activation
         self.sigma = sigma
         self.alpha = alpha
         self.gamma = gamma
         self.ml_weight = ml_weight
         self.cl_weight = cl_weight
-        self.device = get_device(device)
-        self.pretrain_path = pretrain_path
-
-        self.encoder = buildNetwork([input_dim] + encodeLayer, network_type="encode", activation=activation)
-        self.decoder = buildNetwork([z_dim] + decodeLayer, network_type="decode", activation=activation)
+        self.encoder = buildNetwork([input_dim] + encodeLayer, type="encode", activation=activation)
+        self.decoder = buildNetwork([z_dim] + decodeLayer, type="decode", activation=activation)
         self._enc_mu = nn.Linear(encodeLayer[-1], z_dim)
         self._dec_mean = nn.Sequential(nn.Linear(decodeLayer[-1], input_dim), MeanAct())
         self._dec_disp = nn.Sequential(nn.Linear(decodeLayer[-1], input_dim), DispAct())
         self._dec_pi = nn.Sequential(nn.Linear(decodeLayer[-1], input_dim), nn.Sigmoid())
         self.mu = Parameter(torch.Tensor(n_clusters, z_dim))
-        self.zinb_loss = ZINBLoss().to(self.device)
+        self.zinb_loss = ZINBLoss().cpu()
+
+    def save_model(self, path):
+        """Save model to path.
+
+        Parameters
+        ----------
+        path : str
+            path to save model.
+
+        Returns
+        -------
+        None.
 
-        self.to(self.device)
+        """
+        torch.save(self.state_dict(), path)
 
-    @staticmethod
-    def preprocessing_pipeline(log_level: LogLevel = "INFO"):
-        return Compose(
-            AnnDataTransform(sc.pp.filter_genes, min_counts=1),
-            AnnDataTransform(sc.pp.filter_cells, min_counts=1),
-            SaveRaw(),
-            AnnDataTransform(sc.pp.normalize_total),
-            AnnDataTransform(sc.pp.log1p),
-            AnnDataTransform(sc.pp.scale),
-            SetConfig({
-                "feature_channel": [None, None, "n_counts"],
-                "feature_channel_type": ["X", "raw_X", "obs"],
-                "label_channel": "Group"
-            }),
-            log_level=log_level,
-        )
+    def load_model(self, path):
+        """Load model from path.
+
+        Parameters
+        ----------
+        path : str
+            path to load model.
+
+        Returns
+        -------
+        None.
+
+        """
+        pretrained_dict = torch.load(path, map_location=lambda storage, loc: storage)
+        model_dict = self.state_dict()
+        pretrained_dict = {k: v for k, v in pretrained_dict.items() if k in model_dict}
+        model_dict.update(pretrained_dict)
+        self.load_state_dict(model_dict)
 
     def soft_assign(self, z):
         """Soft assign q with z.
 
         Parameters
         ----------
-        z
-            Embedding.
+        z :
+            embedding.
 
         Returns
         -------
-        q
-            Soft label.
+        q :
+            soft label.
 
         """
         q = 1.0 / (1.0 + torch.sum((z.unsqueeze(1) - self.mu)**2, dim=2) / self.alpha)
         q = q**((self.alpha + 1.0) / 2.0)
         q = (q.t() / torch.sum(q, dim=1)).t()
         return q
 
     def target_distribution(self, q):
         """Calculate auxiliary target distribution p with q.
 
         Parameters
         ----------
-        q
-            Soft label.
+        q :
+            soft label.
 
         Returns
         -------
-        p
-            Target distribution.
+        p :
+            target distribution.
 
         """
         p = q**2 / q.sum(0)
         return (p.t() / p.sum(1)).t()
 
     def forward(self, x):
         """Forward propagation.
 
         Parameters
         ----------
-        x
-            Input features.
+        x :
+            input features.
 
         Returns
         -------
-        z0
-            Embedding.
-        q
-            Soft label.
-        _mean
-            Data mean from ZINB.
-        _disp
-            Data dispersion from ZINB.
-        _pi
-            Data dropout probability from ZINB.
+        z0 :
+            embedding.
+        q :
+            soft label.
+        _mean :
+            data mean from ZINB.
+        _disp :
+            data dispersion from ZINB.
+        _pi :
+            data dropout probability from ZINB.
 
         """
         h = self.encoder(x + torch.randn_like(x) * self.sigma)
         z = self._enc_mu(h)
         h = self.decoder(z)
         _mean = self._dec_mean(h)
         _disp = self._dec_disp(h)
@@ -216,49 +211,58 @@
         return z0, q, _mean, _disp, _pi
 
     def encodeBatch(self, X, batch_size=256):
         """Batch encoder.
 
         Parameters
         ----------
-        X
-            Input features.
-        batch_size
-            Size of batch.
+        X :
+            input features.
+        batch_size : int optional
+            size of batch.
 
         Returns
         -------
-        Embedding.
+        encoded :
+            embedding.
 
         """
+        use_cuda = torch.cuda.is_available()
+        if use_cuda:
+            device = 'cuda'
+        else:
+            device = 'cpu'
+        self.to(device)
+
         encoded = []
         num = X.shape[0]
         num_batch = int(math.ceil(1.0 * X.shape[0] / batch_size))
         for batch_idx in range(num_batch):
             xbatch = X[batch_idx * batch_size:min((batch_idx + 1) * batch_size, num)]
-            inputs = xbatch
+            inputs = Variable(xbatch)
             z, _, _, _, _ = self.forward(inputs)
             encoded.append(z.data)
 
         encoded = torch.cat(encoded, dim=0)
         return encoded
 
     def cluster_loss(self, p, q):
         """Calculate cluster loss.
 
         Parameters
         ----------
-        p
-            Target distribution.
-        q
-            Soft label.
+        p :
+            target distribution.
+        q :
+            soft label.
 
         Returns
         -------
-        Cluster loss.
+        loss :
+            cluster loss.
 
         """
 
         def kld(target, pred):
             return torch.mean(torch.sum(target * torch.log(target / (pred + 1e-6)), dim=-1))
 
         kldloss = kld(p, q)
@@ -266,134 +270,165 @@
         return loss
 
     def pairwise_loss(self, p1, p2, cons_type):
         """Calculate pairwise loss.
 
         Parameters
         ----------
-        p1
-            Distribution 1.
-        p2
-            Distribution 2.
-        cons_type
-            Type of loss.
+        p1 :
+            distribution 1.
+        p2 :
+            distribution 2.
+        cons_type : str
+            type of loss.
 
         Returns
         -------
-        Pairwise loss.
+        loss :
+            pairwise loss.
 
         """
         if cons_type == "ML":
             ml_loss = torch.mean(-torch.log(torch.sum(p1 * p2, dim=1)))
             loss = self.ml_weight * ml_loss
             return loss
         else:
             cl_loss = torch.mean(-torch.log(1.0 - torch.sum(p1 * p2, dim=1)))
             loss = self.cl_weight * cl_loss
             return loss
 
-    def pretrain(self, x, X_raw, n_counts, batch_size=256, lr=0.001, epochs=400):
+    def pretrain_autoencoder(self, x, X_raw, size_factor, batch_size=256, lr=0.001, epochs=400, ae_save=True,
+                             ae_weights='AE_weights.pth.tar'):
         """Pretrain autoencoder.
 
         Parameters
         ----------
-        x
-            Input features.
-        X_raw
-            Raw input features.
-        n_counts
-            Total counts for each cell.
-        batch_size
-            Size of batch.
-        lr
-            Learning rate.
-        epochs
-            Number of epochs.
+        x :
+            input features.
+        X_raw :
+            raw input features.
+        size_factor : list
+            size factor of input features and raw input features.
+        batch_size : int optional
+            size of batch.
+        lr : float optional
+            learning rate.
+        epochs : int optional
+            number of epochs.
+        ae_save : bool optional
+            save autoencoder weights or not.
+        ae_weights : str optional
+            path to save autoencoder weights.
+
+        Returns
+        -------
+        None.
 
         """
-        size_factor = torch.tensor(n_counts / np.median(n_counts))
+        use_cuda = torch.cuda.is_available()
+        if use_cuda:
+            device = 'cuda'
+        else:
+            device = 'cpu'
+        self.to(device)
         dataset = TensorDataset(torch.Tensor(x), torch.Tensor(X_raw), torch.Tensor(size_factor))
         dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True)
+        print("Pretraining stage")
         optimizer = optim.Adam(filter(lambda p: p.requires_grad, self.parameters()), lr=lr, amsgrad=True)
         for epoch in range(epochs):
             for batch_idx, (x_batch, x_raw_batch, sf_batch) in enumerate(dataloader):
-                x_tensor = x_batch.to(self.device)
-                x_raw_tensor = x_raw_batch.to(self.device)
-                sf_tensor = sf_batch.to(self.device)
+                x_tensor = Variable(x_batch).to(device)
+                x_raw_tensor = Variable(x_raw_batch).to(device)
+                sf_tensor = Variable(sf_batch).to(device)
                 _, _, mean_tensor, disp_tensor, pi_tensor = self.forward(x_tensor)
                 loss = self.zinb_loss(x=x_raw_tensor, mean=mean_tensor, disp=disp_tensor, pi=pi_tensor,
                                       scale_factor=sf_tensor)
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
-                logger.info("Pretrain epoch [%2d/%3d], ZINB loss: %.4f", batch_idx + 1, epoch + 1, loss.item())
+                print('Pretrain epoch [{}/{}], ZINB loss:{:.4f}'.format(batch_idx + 1, epoch + 1, loss.item()))
+
+        if ae_save:
+            torch.save({'ae_state_dict': self.state_dict(), 'optimizer_state_dict': optimizer.state_dict()}, ae_weights)
+
+    def save_checkpoint(self, state, index, filename):
+        """Save training checkpoint.
+
+        Parameters
+        ----------
+        state :
+            model state
+        index : int
+            checkpoint index
+        filename : str
+            filename to save
+
+        Returns
+        -------
+        None.
+
+        """
+        newfilename = os.path.join(filename, 'FTcheckpoint_%d.pth.tar' % index)
+        torch.save(state, newfilename)
 
-    def fit(
-        self,
-        inputs: Tuple[np.ndarray, np.ndarray, np.ndarray],
-        y: np.ndarray = None,
-        ml_ind1: np.ndarray = np.array([]),
-        ml_ind2: np.ndarray = np.array([]),
-        cl_ind1: np.ndarray = np.array([]),
-        cl_ind2: np.ndarray = np.array([]),
-        ml_p: float = 1.,
-        cl_p: float = 1.,
-        lr: float = 1.,
-        batch_size: int = 256,
-        epochs: int = 10,
-        update_interval: int = 1,
-        tol: float = 1e-3,
-        pt_batch_size: int = 256,
-        pt_lr: float = 0.001,
-        pt_epochs: int = 400,
-    ):
+    def fit(self, X, X_raw, sf, ml_ind1=np.array([]), ml_ind2=np.array([]), cl_ind1=np.array([]), cl_ind2=np.array([]),
+            ml_p=1., cl_p=1., y=None, lr=1., batch_size=256, num_epochs=10, update_interval=1, tol=1e-3, save_dir=""):
         """Train model.
 
         Parameters
         ----------
-        inputs
-            A tuple containing (1) the input features, (2) the raw input features, and (3) the total counts per cell.
-        y
-            True label. Used for model selection.
-        ml_ind1
-            Index 1 of must-link pairs.
-        ml_ind2
-            Index 2 of must-link pairs.
-        cl_ind1
-            Index 1 of cannot-link pairs.
-        cl_ind2
-            Index 2 of cannot-link pairs.
-        ml_p
-            Parameter of must-link loss.
-        cl_p
-            Parameter of cannot-link loss.
-        lr
-            Learning rate.
-        batch_size
-            Size of batch.
-        epochs
-            Number of epochs.
-        update_interval
-            Update interval of soft label and target distribution.
-        tol
-            Tolerance for training loss.
-        pt_batch_size
-            Pretrain batch size.
-        pt_lr
-            Pretrain learning rate.
-        pt_epochs
-            Pretrain epochs.
-
-        """
-        X, X_raw, n_counts = inputs
-        self._pretrain(X, X_raw, n_counts, batch_size=pt_batch_size, lr=pt_lr, epochs=pt_epochs)
-
-        X = torch.tensor(X).to(self.device)
-        X_raw = torch.tensor(X_raw).to(self.device)
-        sf = torch.tensor(n_counts / np.median(n_counts)).to(self.device)
+        X :
+            input features.
+        X_raw :
+            raw input features.
+        sf : float
+            size factor of input features and raw input features.
+        ml_ind1 : np.array optional
+            index 1 of must-link pairs.
+        ml_ind2 : np.array optional
+            index 2 of must-link pairs.
+        cl_ind1 : np.array optional
+            index 1 of cannot-link pairs.
+        cl_ind2 : np.array optional
+            index 2 of cannot-link pairs.
+        ml_p : float optional
+            parameter of must-link loss.
+        cl_p : float optional
+            parameter of cannot-link loss.
+        y : list optional
+            true label. Used for model selection.
+        lr : float optional
+            learning rate.
+        batch_size : int optional
+            size of batch.
+        num_epochs : int optional
+            number of epochs.
+        update_interval : int optional
+            update interval of soft label and target distribution.
+        tol : float optional
+            tolerance for training loss.
+        save_dir : str optional
+            path to save model weights.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        print("Training stage")
+        use_cuda = torch.cuda.is_available()
+        if use_cuda:
+            device = 'cuda'
+        else:
+            device = 'cpu'
+        self.to(device)
+        X = torch.tensor(X).to(device)
+        X_raw = torch.tensor(X_raw).to(device)
+        sf = torch.tensor(sf).to(device)
         optimizer = optim.Adadelta(filter(lambda p: p.requires_grad, self.parameters()), lr=lr, rho=.95)
 
         # Initializing cluster centers with kmeans
         kmeans = KMeans(self.n_clusters, n_init=20)
         data = self.encodeBatch(X)
         self.y_pred = kmeans.fit_predict(data.data.cpu().numpy())
         self.y_pred_last = self.y_pred
@@ -410,85 +445,96 @@
         update_ml = 1
         update_cl = 1
 
         aris = []
         P = {}
         Q = {}
 
-        delta_label = np.inf
-        for epoch in range(epochs):
+        for epoch in range(num_epochs):
             if epoch % update_interval == 0:
                 # update the targe distribution p
                 latent = self.encodeBatch(X)
                 q = self.soft_assign(latent)
                 self.q = q
                 p = self.target_distribution(q).data
                 self.y_pred = self.predict()
 
-                p_ = {f"epoch{epoch}": p}
-                q_ = {f"epoch{epoch}": q}
+                # save current model
+                if (epoch > 0 and delta_label < tol) or epoch % 10 == 0:
+                    self.save_checkpoint(
+                        {
+                            'epoch': epoch + 1,
+                            'state_dict': self.state_dict(),
+                            'mu': self.mu,
+                            'p': p,
+                            'q': q,
+                            'y': y
+                        }, epoch + 1, filename=save_dir)
+                p_ = {f'epoch{epoch}': p}
+                q_ = {f'epoch{epoch}': q}
                 P = {**P, **p_}
                 Q = {**Q, **q_}
 
                 # check stop criterion
                 delta_label = np.sum(self.y_pred != self.y_pred_last).astype(np.float32) / num
                 self.y_pred_last = self.y_pred
                 if epoch > 0 and delta_label < tol:
-                    logger.info("Reach tolerance threshold (%.3e < %.3e). Stopping training.", delta_label, tol)
+                    print('delta_label ', delta_label, '< tol ', tol)
+                    print("Reach tolerance threshold. Stopping training.")
                     break
 
                 # calculate ari score for model selection
-                ari = self.score(None, y)
+                _, _, ari = self.score(y)
                 aris.append(ari)
 
             # train 1 epoch for clustering loss
             train_loss = 0.0
             recon_loss_val = 0.0
             cluster_loss_val = 0.0
             for batch_idx in range(num_batch):
                 xbatch = X[batch_idx * batch_size:min((batch_idx + 1) * batch_size, num)]
                 xrawbatch = X_raw[batch_idx * batch_size:min((batch_idx + 1) * batch_size, num)]
                 sfbatch = sf[batch_idx * batch_size:min((batch_idx + 1) * batch_size, num)]
                 pbatch = p[batch_idx * batch_size:min((batch_idx + 1) * batch_size, num)]
                 optimizer.zero_grad()
-                inputs = xbatch
-                rawinputs = xrawbatch
-                sfinputs = sfbatch
-                target = pbatch
+                inputs = Variable(xbatch)
+                rawinputs = Variable(xrawbatch)
+                sfinputs = Variable(sfbatch)
+                target = Variable(pbatch)
 
                 z, qbatch, meanbatch, dispbatch, pibatch = self.forward(inputs)
 
                 cluster_loss = self.cluster_loss(target, qbatch)
                 recon_loss = self.zinb_loss(rawinputs, meanbatch, dispbatch, pibatch, sfinputs)
                 loss = cluster_loss + recon_loss
                 loss.backward()
                 optimizer.step()
                 cluster_loss_val += cluster_loss.data * len(inputs)
                 recon_loss_val += recon_loss.data * len(inputs)
                 train_loss = cluster_loss_val + recon_loss_val
 
-            logger.info("#Epoch %3d: Total: %.4f, Clustering Loss: %.4f, ZINB Loss: %.4f", epoch + 1, train_loss / num,
-                        cluster_loss_val / num, recon_loss_val / num)
+            print("#Epoch %3d: Total: %.4f, Clustering Loss: %.4f, ZINB Loss: %.4f" %
+                  (epoch + 1, train_loss / num, cluster_loss_val / num, recon_loss_val / num))
 
             ml_loss = 0.0
             if epoch % update_ml == 0:
                 for ml_batch_idx in range(ml_num_batch):
                     px1 = X[ml_ind1[ml_batch_idx * batch_size:min(ml_num, (ml_batch_idx + 1) * batch_size)]]
                     pxraw1 = X_raw[ml_ind1[ml_batch_idx * batch_size:min(ml_num, (ml_batch_idx + 1) * batch_size)]]
                     sf1 = sf[ml_ind1[ml_batch_idx * batch_size:min(ml_num, (ml_batch_idx + 1) * batch_size)]]
                     px2 = X[ml_ind2[ml_batch_idx * batch_size:min(ml_num, (ml_batch_idx + 1) * batch_size)]]
                     sf2 = sf[ml_ind2[ml_batch_idx * batch_size:min(ml_num, (ml_batch_idx + 1) * batch_size)]]
                     pxraw2 = X_raw[ml_ind2[ml_batch_idx * batch_size:min(ml_num, (ml_batch_idx + 1) * batch_size)]]
                     optimizer.zero_grad()
-                    inputs1 = px1
-                    rawinputs1 = pxraw1
-                    sfinput1 = sf1
-                    inputs2 = px2
-                    rawinputs2 = pxraw2
-                    sfinput2 = sf2
+                    inputs1 = Variable(px1)
+                    rawinputs1 = Variable(pxraw1)
+                    sfinput1 = Variable(sf1)
+                    inputs2 = Variable(px2)
+                    rawinputs2 = Variable(pxraw2)
+                    sfinput2 = Variable(sf2)
                     z1, q1, mean1, disp1, pi1 = self.forward(inputs1)
                     z2, q2, mean2, disp2, pi2 = self.forward(inputs2)
                     loss = (ml_p * self.pairwise_loss(q1, q2, "ML") +
                             self.zinb_loss(rawinputs1, mean1, disp1, pi1, sfinput1) +
                             self.zinb_loss(rawinputs2, mean2, disp2, pi2, sfinput2))
                     # 0.1 for mnist/reuters, 1 for fashion, the parameters are tuned via grid search on validation set
                     ml_loss += loss.data
@@ -497,63 +543,69 @@
 
             cl_loss = 0.0
             if epoch % update_cl == 0:
                 for cl_batch_idx in range(cl_num_batch):
                     px1 = X[cl_ind1[cl_batch_idx * batch_size:min(cl_num, (cl_batch_idx + 1) * batch_size)]]
                     px2 = X[cl_ind2[cl_batch_idx * batch_size:min(cl_num, (cl_batch_idx + 1) * batch_size)]]
                     optimizer.zero_grad()
-                    inputs1 = px1
-                    inputs2 = px2
+                    inputs1 = Variable(px1)
+                    inputs2 = Variable(px2)
                     z1, q1, _, _, _ = self.forward(inputs1)
                     z2, q2, _, _, _ = self.forward(inputs2)
                     loss = cl_p * self.pairwise_loss(q1, q2, "CL")
                     cl_loss += loss.data
                     loss.backward()
                     optimizer.step()
 
             if ml_num_batch > 0 and cl_num_batch > 0:
-                logger.info("Pairwise Total: %.4f, ML loss: %.4f, CL loss: %.4f",
-                            float(ml_loss.cpu()) + float(cl_loss.cpu()), ml_loss.cpu(), cl_loss.cpu())
+                print("Pairwise Total: %.4f, ML loss: %.4f, CL loss: %.4f" %
+                      (float(ml_loss.cpu()) + float(cl_loss.cpu()), ml_loss.cpu(), cl_loss.cpu()))
 
         index = update_interval * np.argmax(aris)
-        self.q = Q[f"epoch{index}"]
+        self.q = Q[f'epoch{index}']
 
-    def predict_proba(self, x: Optional[Any] = None) -> np.ndarray:
-        """Get the predicted propabilities for each cell.
+    def predict(self):
+        """Get predictions from the trained model.
 
         Parameters
         ----------
-        x
-            Not used, for compatibility with the BaseClusteringMethod class.
+        None.
 
         Returns
         -------
-        pred_prop
-            Predicted probability for each cell.
+        y_pred : np.array
+            prediction of given clustering method.
 
         """
-        pred_prob = self.q.detach().clone().cpu().numpy()
-        return pred_prob
+        y_pred = torch.argmax(self.q, dim=1).data.cpu().numpy()
+        return y_pred
 
-    def predict(self, x: Optional[Any] = None) -> np.ndarray:
-        """Get predictions from the trained model.
+    def score(self, y):
+        """Evaluate the trained model.
 
         Parameters
         ----------
-        x
-            Not used, for compatibility with the BaseClusteringMethod class.
+        y : list
+            true labels.
 
         Returns
         -------
-        pred
-            Predicted clustering assignment for each cell.
+        acc : float
+            accuracy.
+        nmi : float
+            normalized mutual information.
+        ari : float
+            adjusted Rand index.
 
         """
-        pred = self.predict_proba().argmax(1)
-        return pred
+        y_pred = torch.argmax(self.q, dim=1).data.cpu().numpy()
+        acc = np.round(cluster_acc(y, y_pred), 5)
+        nmi = np.round(metrics.normalized_mutual_info_score(y, y_pred), 5)
+        ari = np.round(metrics.adjusted_rand_score(y, y_pred), 5)
+        return acc, nmi, ari
 
 
 class MeanAct(nn.Module):
     """Mean activation class."""
 
     def __init__(self):
         super().__init__()
```

### Comparing `pydance-1.0.0/dance/modules/single_modality/clustering/scdeepcluster.py` & `pydance-1.0.0rc0/dance/modules/single_modality/cell_type_annotation/scdeepsort.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,535 +1,476 @@
-"""Reimplementation of scDeepCluster.
-
-Extended from https://github.com/ttgump/scDeepCluster
+"""Reimplementation of the scDeepSort cell-type annotation method.
 
 Reference
-----------
-Tian, Tian, et al. "Clustering single-cell RNA-seq data with a model-based deep learning approach." Nature Machine
-Intelligence 1.4 (2019): 191-198.
+---------
+Shao, Xin, et al. "scDeepSort: a pre-trained cell-type annotation method for single-cell transcriptomics using deep
+learning with a weighted graph neural network." Nucleic acids research 49.21 (2021): e122-e122.
 
 """
-import math
+import os
+import time
+from pathlib import Path
 
+import dgl.function as fn
 import numpy as np
-import scanpy as sc
+import pandas as pd
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
-import torch.optim as optim
-from sklearn.cluster import KMeans
-from torch.nn import Parameter
-from torch.utils.data import DataLoader, TensorDataset
-
-from dance import logger
-from dance.modules.base import BaseClusteringMethod, TorchNNPretrain
-from dance.transforms import AnnDataTransform, Compose, SaveRaw, SetConfig
-from dance.typing import Any, List, LogLevel, Optional, Tuple
-from dance.utils.loss import ZINBLoss
+from dgl.dataloading import DataLoader, NeighborSampler
 
+DEBUG = os.environ.get("DANCE_DEBUG")
 
-def buildNetwork(layers: List[int], network_type: str, activation: str = "relu"):
-    """Build network layer.
 
-    Parameters
-    ----------
-    layers
-        Dimensions of layers.
-    network_type
-        Type of network.
-    activation
-        Activation function.
-
-    Returns
-    -------
-    Built network.
+class AdaptiveSAGE(nn.Module):
+    """The AdaptiveSAGE graph convolution layer.
 
-    """
-    net = []
-    for i in range(1, len(layers)):
-        net.append(nn.Linear(layers[i - 1], layers[i]))
-        if activation == "relu":
-            net.append(nn.ReLU())
-        elif activation == "sigmoid":
-            net.append(nn.Sigmoid())
-    net = nn.Sequential(*net)
-    return net
-
-
-def euclidean_dist(x, y):
-    """Calculate Euclidean distance between x and y."""
-    return torch.sum(torch.square(x - y), dim=1)
+    Similar to SAGE convolution with mean aggregation, but with additional flexibility that adaptively assigns
+    importance to gene-cell interactions, as well as gene and cell self-loops. In particular, each gene will be
+    associated with an importance score `beta` that are used as aggregation weights by the cell nodes. Additionally,
+    there are two `alpha` parameters indicating how much each cell or gene should retain its previous representations.
 
+    Note
+    ----
+    In practice, `alpha` and `beta` are stored in a unified tensor called `alpha`. The first #gene elements of this
+    tensor are the `beta` values and the last two elements are the actual `alpha` values.
 
-class ScDeepCluster(nn.Module, TorchNNPretrain, BaseClusteringMethod):
-    """ScDeepCluster class.
+    """
 
-    Parameters
-    ----------
-    input_dim
-        Dimension of encoder input.
-    z_dim
-        Dimension of embedding.
-    encodeLayer
-        Dimensions of encoder layers.
-    decodeLayer
-        Dimensions of decoder layers.
-    activation
-        Activation function.
-    sigma
-        Parameter of Gaussian noise.
-    alpha
-        Parameter of soft assign.
-    gamma
-        Parameter of cluster loss.
-    device
-        Computing device.
-    pretrain_path
-        Path to pretrained weights.
+    def __init__(self, dim_in, dim_out, alpha, dropout_layer, act_layer, norm_layer):
+        """Initialize the AdaptiveSAGE convolution layer.
 
-    """
+        Parameters
+        ----------
+        dim_in : int
+            Input feature dimensions.
+        dim_out : int
+            output feature dimensinos.
+        alpha : Tensor
+            Shared learnable parameters containing gene-cell interaction strengths and those for the cell and gene
+            self-loops.
+        dropout_layer : torch.nn
+            Dropout layer.
+        act_layer : torch.nn
+            Activation layer.
+        norm_layer : torch.nn
+            Normalization layer.
 
-    def __init__(self, input_dim, z_dim, encodeLayer=[], decodeLayer=[], activation="relu", sigma=1., alpha=1.,
-                 gamma=1., device="cuda", pretrain_path: Optional[str] = None):
+        """
         super().__init__()
-        self.z_dim = z_dim
-        self.activation = activation
-        self.sigma = sigma
+
         self.alpha = alpha
-        self.gamma = gamma
-        self.device = device
-        self.pretrain_path = pretrain_path
-
-        self.encoder = buildNetwork([input_dim] + encodeLayer, network_type="encode", activation=activation)
-        self.decoder = buildNetwork([z_dim] + decodeLayer, network_type="decode", activation=activation)
-        self._enc_mu = nn.Linear(encodeLayer[-1], z_dim)
-        self._dec_mean = nn.Sequential(nn.Linear(decodeLayer[-1], input_dim), MeanAct())
-        self._dec_disp = nn.Sequential(nn.Linear(decodeLayer[-1], input_dim), DispAct())
-        self._dec_pi = nn.Sequential(nn.Linear(decodeLayer[-1], input_dim), nn.Sigmoid())
-
-        self.zinb_loss = ZINBLoss().to(self.device)
-        self.to(device)
-
-    @staticmethod
-    def preprocessing_pipeline(log_level: LogLevel = "INFO"):
-        return Compose(
-            AnnDataTransform(sc.pp.filter_genes, min_counts=1),
-            AnnDataTransform(sc.pp.filter_cells, min_counts=1),
-            SaveRaw(),
-            AnnDataTransform(sc.pp.normalize_total),
-            AnnDataTransform(sc.pp.log1p),
-            AnnDataTransform(sc.pp.scale),
-            SetConfig({
-                "feature_channel": [None, None, "n_counts"],
-                "feature_channel_type": ["X", "raw_X", "obs"],
-                "label_channel": "Group",
-            }),
-            log_level=log_level,
-        )
+        self.gene_num = len(alpha) - 2
+
+        self.layers = nn.ModuleList()
+        self.layers.append(dropout_layer)
+        self.layers.append(nn.Linear(dim_in, dim_out))
+        nn.init.xavier_uniform_(self.layers[-1].weight, gain=nn.init.calculate_gain("relu"))
+        self.layers.append(act_layer)
+        self.layers.append(norm_layer)
+
+    def message_func(self, edges):
+        """Message update function.
+
+        Reweight messages based on 1) the shared learnable interaction strengths and 2) the underlying edgeweights of
+        the graph. In particular, for 1), gene-cell interaction (undirectional) will be weighted by the gene specific
+        `beta` value, and the cell and gene self-interactions will be weighted based on the corresponding `alpha`
+        values.
+
+        """
+        number_of_edges = edges.src["h"].shape[0]
+        indices = np.expand_dims(np.array([self.gene_num + 1] * number_of_edges, dtype=np.int32), axis=1)
+        src_id, dst_id = edges.src["id"].cpu().numpy(), edges.dst["id"].cpu().numpy()
+        indices = np.where((src_id >= 0) & (dst_id < 0), src_id, indices)  # gene->cell
+        indices = np.where((dst_id >= 0) & (src_id < 0), dst_id, indices)  # cell->gene
+        indices = np.where((dst_id >= 0) & (src_id >= 0), self.gene_num, indices)  # gene-gene
+        if DEBUG:
+            print(
+                f"{((src_id >= 0) & (dst_id < 0)).sum():>10,} (geen->cell), "
+                f"{((src_id < 0) & (dst_id >= 0)).sum():>10,} (cell->gene), "
+                f"{((src_id >= 0) & (dst_id >= 0)).sum():>10,} (self-gene), "
+                f"{((src_id < 0) & (dst_id < 0)).sum():>10,} (self-cell), ", )
+        h = edges.src["h"] * self.alpha[indices.squeeze()]
+        return {"m": h * edges.data["weight"]}
+
+    def forward(self, block, h):
+        with block.local_scope():
+            h_src = h
+            h_dst = h[:block.number_of_dst_nodes()]
+            block.srcdata["h"] = h_src
+            block.dstdata["h"] = h_dst
+            block.update_all(self.message_func, fn.mean("m", "neigh"))
+
+            z = block.dstdata["h"]
+            for layer in self.layers:
+                z = layer(z)
+
+            return z
+
+
+class GNN(nn.Module):
+    """The scDeepSort GNN model.
+
+    Message passing between cell and genes to learn cell representations for cell-type annotations. The graph contains
+    both cell and gene nodes. The gene features are initialized as PCA embeddings from the (normalized) scRNA-seq
+    samples matrix, and the cell features are computed as the weighted aggregation of the gene features according to
+    each cell's gene expressions.
 
-    def save_model(self, path):
-        """Save model to path.
+    """
+
+    def __init__(self, dim_in, dim_out, dim_hid, n_layers, gene_num, activation=None, norm=None, dropout=0.):
+        """Initialize the scDeepSort GNN model.
 
         Parameters
         ----------
-        path
-            Path to save model.
+        dim_in : int
+            Input dimension (PCA embeddings dimension).
+        dim_out : int
+            Output dimension (number of unique cell labels).
+        n_layers : int
+            Number of convolution layers.
+        gene_num : int
+            Number of genes.
+        dropout : float
+            Dropout ratio.
+        activation : torch.nn, optional
+            Activation layer.
+        norm : torch.nn, optional
+            Normalization layer.
 
         """
-        torch.save(self.state_dict(), path)
+        super().__init__()
 
-    def load_model(self, path):
-        """Load model from path.
+        self.n_layers = n_layers
+        self.gene_num = gene_num
 
-        Parameters
-        ----------
-        path
-            Path to load model.
+        # [gene_num] is alpha of gene-gene self loop, [gene_num+1] is alpha of cell-cell self loop, the rest are betas
+        self.alpha = nn.Parameter(torch.tensor([1] * (self.gene_num + 2), dtype=torch.float32).unsqueeze(-1))
 
-        """
-        pretrained_dict = torch.load(path, map_location=lambda storage, loc: storage)
-        model_dict = self.state_dict()
-        pretrained_dict = {k: v for k, v in pretrained_dict.items() if k in model_dict}
-        model_dict.update(pretrained_dict)
-        self.load_state_dict(model_dict)
+        dropout_layer = nn.Dropout(p=dropout) if dropout > 0 else nn.Identity()
+        act_layer = activation or nn.Identity()
+        norm_layer = norm or nn.Identity()
 
-    def soft_assign(self, z):
-        """Soft assign q with z.
+        self.layers = nn.ModuleList()
+        for i in range(n_layers):
+            input_dimension = dim_in if i == 0 else dim_hid
+            self.layers.append(AdaptiveSAGE(input_dimension, dim_hid, self.alpha, dropout_layer, act_layer, norm_layer))
 
-        Parameters
-        ----------
-        z
-            Embedding.
+        self.linear = nn.Linear(dim_hid, dim_out)
+        nn.init.xavier_uniform_(self.linear.weight, gain=nn.init.calculate_gain("relu"))
 
-        Returns
-        -------
-        q
-            Soft label.
+    def forward(self, blocks, x):
+        assert len(blocks) == len(self.layers), f"Inonsistent layer info: {len(blocks)=} vs {len(self.layers)=}"
+        for block, layer in zip(blocks, self.layers):
+            x = layer(block, x)
+        return self.linear(x)
 
-        """
-        q = 1.0 / (1.0 + torch.sum((z.unsqueeze(1) - self.mu)**2, dim=2) / self.alpha)
-        q = q**((self.alpha + 1.0) / 2.0)
-        q = (q.t() / torch.sum(q, dim=1)).t()
-        return q
 
-    def target_distribution(self, q):
-        """Calculate auxiliary target distribution p with q.
+class ScDeepSort:
+    """The ScDeepSort cell-type annotation model.
 
-        Parameters
-        ----------
-        q
-            Soft label.
+    Parameters
+    ----------
+    params : argparse.Namespace
+        A Namespace contains arguments of Scdeepsort. See parser documnetation for more details.
 
-        Returns
-        -------
-        p
-            Target distribution.
+    """
 
-        """
-        p = q**2 / q.sum(0)
-        return (p.t() / p.sum(1)).t()
+    def __init__(self, params):
+        self.params = params
+        self.postfix = time.strftime("%d_%m_%Y") + "_" + time.strftime("%H:%M:%S")
+        self.prj_path = Path(__file__).resolve().parents[4]
+        # TODO: change the prefix from `example` to `saved_models`
+        self.save_path = (self.prj_path / "example" / "single_modality" / "cell_type_annotation" / "pretrained" /
+                          self.params.species / "models")
+
+        if not self.save_path.exists():
+            self.save_path.mkdir(parents=True)
+        self.device = torch.device("cpu" if self.params.gpu == -1 else f"cuda:{params.gpu}")
+
+        # Define the variables during training
+        self.num_cells = None
+        self.num_genes = None
+        self.num_labels = None
+        self.graph = None
+        self.train_ids = None
+        self.test_ids = None
+        self.labels = None
+
+        # Define the variables during prediction
+        self.id2label = None
+        self.test_dict = None
+
+    def fit(self, num_cells, num_genes, num_labels, graph, train_ids, test_ids, labels):
+        """Train scDeepsort model.
+
+        Parameters
+        ----------
+        num_cells : int
+            The number of cells in the training set.
+        num_genes : int
+            The number of genes in the training set.
+        num_labels : int
+            The number of labels in the training set.
+        graph : dgl.DGLGraph
+            Training graph.
+        train_ids : Tensor
+            The training ids.
+        test_ids : Tensor
+            The testing ids.
+        labels : Tensor
+            Node (cell, gene) labels, -1 for genes.
+
+        """
+        self.num_cells = num_cells
+        self.num_genes = num_genes
+        self.num_labels = num_labels
+
+        self.train_ids = train_ids.to(self.device)
+        self.test_ids = test_ids.to(self.device)
+        self.labels = labels.to(self.device)
+        self.graph = graph.to(self.device)
+        self.graph.ndata["label"] = self.labels
+
+        self.model = GNN(self.params.dense_dim, self.num_labels, self.params.hidden_dim, self.params.n_layers,
+                         self.num_genes, activation=nn.ReLU(), dropout=self.params.dropout).to(self.device)
+        print(self.model)
+
+        self.sampler = NeighborSampler(fanouts=[-1] * self.params.n_layers, edge_dir="in")
+        self.optimizer = torch.optim.Adam(self.model.parameters(), lr=self.params.lr,
+                                          weight_decay=self.params.weight_decay)
+        self.loss_fn = nn.CrossEntropyLoss(reduction="sum")
+        if self.params.num_neighbors == 0:
+            self.num_neighbors = self.num_cells + self.num_genes
+        else:
+            self.num_neighbors = self.params.num_neighbors
 
-    def forwardAE(self, x):
-        """Forward propagation of autoencoder.
+        print(f"Train Number: {len(self.train_ids)}, Test Number: {len(self.test_ids)}")
+        max_test_acc, _train_acc, _epoch = 0, 0, 0
+        for epoch in range(self.params.n_epochs):
+            loss = self.cal_loss()
+            train_acc = self.evaluate(self.train_ids)[-1]
+            test_correct, test_unsure, test_acc = self.evaluate(self.test_ids)
+            if max_test_acc <= test_acc:
+                final_test_correct_num = test_correct
+                final_test_unsure_num = test_unsure
+                _train_acc = train_acc
+                _epoch = epoch
+                max_test_acc = test_acc
+                self.save_model()
+            print(f">>>>Epoch {epoch:04d}: Train Acc {train_acc:.4f}, Loss {loss / len(self.train_ids):.4f}, "
+                  f"Test correct {test_correct}, Test unsure {test_unsure}, Test Acc {test_acc:.4f}")
+
+        print(f"---{self.params.species} {self.params.tissue} Best test result:---")
+        print(f"Epoch {_epoch:04d}, Train Acc {_train_acc:.4f}, Test Correct Num {final_test_correct_num}, "
+              f"Test Total Num {len(self.test_ids)}, Test Unsure Num {final_test_unsure_num}, "
+              f"Test Acc {final_test_correct_num / len(self.test_ids):.4f}")
 
-        Parameters
-        ----------
-        x
-            Input features.
+    def cal_loss(self):
+        """Calculate loss.
 
         Returns
         -------
-        z0
-            Embedding.
-        _mean
-            Data mean from ZINB.
-        _disp
-            Data dispersion from ZINB.
-        _pi
-            Data dropout probability from ZINB.
+        float
+            Loss function value.
 
         """
-        h = self.encoder(x + torch.randn_like(x) * self.sigma)
-        z = self._enc_mu(h)
-        h = self.decoder(z)
-        _mean = self._dec_mean(h)
-        _disp = self._dec_disp(h)
-        _pi = self._dec_pi(h)
-
-        h0 = self.encoder(x)
-        z0 = self._enc_mu(h0)
-        return z0, _mean, _disp, _pi
+        self.model.train()
+        total_loss = 0
 
-    def forward(self, x):
-        """Forward propagation.
+        dataloader = DataLoader(graph=self.graph, indices=self.train_ids, graph_sampler=self.sampler,
+                                batch_size=self.params.batch_size, shuffle=True)
+        for _, _, blocks in dataloader:
+            blocks = [b.to(self.device) for b in blocks]
+            input_features = blocks[0].srcdata["features"]
+            output_labels = blocks[-1].dstdata["label"]
+            output_predictions = self.model(blocks, input_features)
 
-        Parameters
-        ----------
-        x
-            Input features.
+            loss = self.loss_fn(output_predictions, output_labels)
+            self.optimizer.zero_grad()
+            loss.backward()
+            self.optimizer.step()
 
-        Returns
-        -------
-        z0
-            Embedding.
-        q
-            Soft label.
-        _mean
-            Data mean from ZINB.
-        _disp
-            Data dispersion from ZINB.
-        _pi
-            Data dropout probability from ZINB.
+            total_loss += loss.item()
 
-        """
-        h = self.encoder(x + torch.randn_like(x) * self.sigma)
-        z = self._enc_mu(h)
-        h = self.decoder(z)
-        _mean = self._dec_mean(h)
-        _disp = self._dec_disp(h)
-        _pi = self._dec_pi(h)
-
-        h0 = self.encoder(x)
-        z0 = self._enc_mu(h0)
-        q = self.soft_assign(z0)
-        return z0, q, _mean, _disp, _pi
+        return total_loss
 
-    def encodeBatch(self, x, batch_size=256):
-        """Batch encoder.
+    @torch.no_grad()
+    def evaluate(self, ids):
+        """Evaluate the trained scDeepsort model.
 
         Parameters
         ----------
-        x
-            Input features.
-        batch_size
-            Size of batch.
+        ids : Tensor
+            A 1-D tensor containing node IDs to be evaluated on.
 
         Returns
         -------
-        encoded
-            Embedding.
+        Tuple[int, int, float]
+            The total number of correct prediction, the total number of unsure prediction, and the accuracy score.
 
         """
-        self.eval()
-        encoded = []
-        num = x.shape[0]
-        num_batch = int(math.ceil(1.0 * x.shape[0] / batch_size))
-        for batch_idx in range(num_batch):
-            xbatch = x[batch_idx * batch_size:min((batch_idx + 1) * batch_size, num)]
-            inputs = xbatch.to(self.device)
-            z, _, _, _ = self.forwardAE(inputs)
-            encoded.append(z.data)
+        self.model.eval()
+        total_correct, total_unsure = 0, 0
 
-        encoded = torch.cat(encoded, dim=0)
-        return encoded.to(self.device)
-
-    def cluster_loss(self, p, q):
-        """Calculate cluster loss.
+        dataloader = DataLoader(graph=self.graph, indices=ids, graph_sampler=self.sampler,
+                                batch_size=self.params.batch_size, shuffle=True)
+        for _, _, blocks in dataloader:
+            blocks = [b.to(self.device) for b in blocks]
+            input_features = blocks[0].srcdata["features"]
+            output_labels = blocks[-1].dstdata["label"]
+            output_predictions = self.model(blocks, input_features)
+
+            for pred, label in zip(output_predictions.cpu(), output_labels.cpu()):
+                max_prob = pred.max().item()
+                if max_prob < self.params.unsure_rate / self.num_labels:
+                    total_unsure += 1
+                elif pred.argmax().item() == label:
+                    total_correct += 1
+
+        return total_correct, total_unsure, total_correct / len(ids)
+
+    def save_model(self):
+        """Save the model at the save_path."""
+        state = {"model": self.model.state_dict(), "optimizer": self.optimizer.state_dict()}
+        torch.save(state, self.save_path / f"{self.params.species}-{self.params.tissue}.pt")
+
+    def load_model(self):
+        """Load the model from the model path."""
+        filename = f"{self.params.species}-{self.params.tissue}.pt"
+        model_path = self.prj_path / "pretrained" / self.params.species / "models" / filename
+        state = torch.load(model_path, map_location=self.device)
+        self.model.load_state_dict(state["model"])
+
+    @torch.no_grad()
+    def inference(self, num):
+        """Perform inference on a test dataset.
 
         Parameters
         ----------
-        p
-            Target distribution.
-        q
-            Soft label.
+        num : int
+            Test dataset number.
 
         Returns
         -------
-        loss
-            Cluster loss.
+        list
+            Predicted labels.
 
         """
+        self.model.eval()
 
-        def kld(target, pred):
-            return torch.mean(torch.sum(target * torch.log(target / (pred + 1e-6)), dim=-1))
+        unsure_threshold = self.params.unsure_rate / self.num_labels
 
-        kldloss = kld(p, q)
-        return self.gamma * kldloss
+        graph = self.test_dict["graph"][num].to(self.device)
+        test_indices = self.test_dict["nid"][num].to(self.device)
+        new_logits = torch.zeros((graph.number_of_nodes(), self.num_labels))
 
-    def pretrain(self, x, x_raw, n_counts, batch_size=256, lr=0.001, epochs=400):
-        """Pretrain autoencoder.
+        dataloader = DataLoader(graph=graph, indices=test_indices, graph_sampler=self.sampler,
+                                batch_size=self.params.batch_size, shuffle=True)
+        for _, output_nodes, blocks in dataloader:
+            blocks = [b.to(torch.device(self.device)) for b in blocks]
+            input_features = blocks[0].srcdata["features"]
+            new_logits[output_nodes] = self.model(blocks, input_features).detach().cpu()
 
-        Parameters
-        ----------
-        x
-            Input features.
-        x_raw
-            Raw input features.
-        n_counts
-            Total counts for each cell.
-        batch_size
-            Size of batch.
-        lr
-            Learning rate.
-        epochs
-            Number of epochs.
+        new_logits = new_logits[self.test_dict["mask"][num]]
+        new_logits = nn.functional.softmax(new_logits, dim=1).numpy()
+        predict_label = []
+        for pred in new_logits:
+            pred_label = self.id2label[pred.argmax().item()]
+            predict_label.append("unsure" if pred.max().item() < unsure_threshold else pred_label)
+        return predict_label
 
-        """
-        self.train()
-        size_factor = torch.tensor(n_counts / np.median(n_counts))
-        dataset = TensorDataset(torch.Tensor(x), torch.Tensor(x_raw), size_factor)
-        dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True)
-        optimizer = optim.Adam(filter(lambda p: p.requires_grad, self.parameters()), lr=lr, amsgrad=True)
-        for epoch in range(epochs):
-            loss_val = 0
-            for batch_idx, (x_batch, x_raw_batch, sf_batch) in enumerate(dataloader):
-                x_tensor = x_batch.to(self.device)
-                x_raw_tensor = x_raw_batch.to(self.device)
-                sf_tensor = sf_batch.to(self.device)
-                _, mean_tensor, disp_tensor, pi_tensor = self.forwardAE(x_tensor)
-                loss = self.zinb_loss(x=x_raw_tensor, mean=mean_tensor, disp=disp_tensor, pi=pi_tensor,
-                                      scale_factor=sf_tensor)
-                optimizer.zero_grad()
-                loss.backward()
-                optimizer.step()
-                loss_val += loss.item() * len(x_batch)
-            logger.info("Pretrain epoch %3d, ZINB loss: %.8f", epoch + 1, loss_val / x.shape[0])
-
-    def fit(
-        self,
-        inputs: Tuple[np.ndarray, np.ndarray, np.ndarray],
-        y: np.ndarray,
-        n_clusters: int = 10,
-        init_centroid: Optional[List[int]] = None,
-        y_pred_init: Optional[List[int]] = None,
-        lr: float = 1,
-        batch_size: int = 256,
-        epochs: int = 10,
-        update_interval: int = 1,
-        tol: float = 1e-3,
-        pt_batch_size: int = 256,
-        pt_lr: float = 0.001,
-        pt_epochs: int = 400,
-    ):
-        """Train model.
+    def predict(self, id2label, test_dict):
+        """Perform prediction on all test datasets.
 
         Parameters
         ----------
-        inputs
-            A tuple containing (1) the input features, (2) the raw input features, and (3) the total counts per cell.
-        y
-            True label. Used for model selection.
-        n_clusters
-            Number of clusters.
-        init_centroid
-            Initialization of centroids. If None, perform kmeans to initialize cluster centers.
-        y_pred_init
-            Predicted label for initialization.
-        lr
-            Learning rate.
-        batch_size
-            Size of batch.
-        epochs
-            Number of epochs.
-        update_interval
-            Update interval of soft label and target distribution.
-        tol
-            Tolerance for training loss.
-        pt_batch_size
-            Pretraining batch size.
-        pt_lr
-            Pretraining learning rate.
-        pt_epochs
-            pretraining epochs.
-
-        """
-        x, x_raw, n_counts = inputs
-        self._pretrain(x, x_raw, n_counts, batch_size=pt_batch_size, lr=pt_lr, epochs=pt_epochs)
-
-        self.train()
-        x = torch.tensor(x, dtype=torch.float32)
-        x_raw = torch.tensor(x_raw, dtype=torch.float32)
-        size_factor = torch.FloatTensor(n_counts / np.median(n_counts))
-        self.mu = Parameter(torch.Tensor(n_clusters, self.z_dim).to(self.device))
-        optimizer = optim.Adadelta(filter(lambda p: p.requires_grad, self.parameters()), lr=lr, rho=.95)
-
-        logger.info("Initializing cluster centers with kmeans.")
-        if init_centroid is None:
-            kmeans = KMeans(n_clusters, n_init=20)
-            data = self.encodeBatch(x)
-            self.y_pred = kmeans.fit_predict(data.data.cpu().numpy())
-            self.y_pred_last = self.y_pred
-            self.mu.data.copy_(torch.tensor(kmeans.cluster_centers_, dtype=torch.float32))
-        else:
-            self.mu.data.copy_(torch.tensor(init_centroid, dtype=torch.float32))
-            self.y_pred = y_pred_init
-            self.y_pred_last = self.y_pred
-
-        num = x.shape[0]
-        num_batch = int(math.ceil(1.0 * x.shape[0] / batch_size))
-
-        aris = []
-        P = {}
-        Q = {}
-
-        delta_label = np.inf
-        for epoch in range(epochs):
-            if epoch % update_interval == 0:
-                # update the targe distribution p
-                latent = self.encodeBatch(x.to(self.device))
-                q = self.soft_assign(latent)
-                self.q = q
-                p = self.target_distribution(q).data
-                self.y_pred = self.predict()
-
-                p_ = {f"epoch{epoch}": p}
-                q_ = {f"epoch{epoch}": q}
-                P = {**P, **p_}
-                Q = {**Q, **q_}
-
-                # check stop criterion
-                delta_label = np.sum(self.y_pred != self.y_pred_last).astype(np.float32) / num
-                self.y_pred_last = self.y_pred
-                if epoch > 0 and delta_label < tol:
-                    logger.info("Reach tolerance threshold (%.3e < %.3e). Stopping training.", delta_label, tol)
-                    break
-
-                # calculate ari score for model selection
-                ari = self.score(None, y)
-                aris.append(ari)
-
-            # train 1 epoch for clustering loss
-            train_loss = 0.0
-            recon_loss_val = 0.0
-            cluster_loss_val = 0.0
-            for batch_idx in range(num_batch):
-                xbatch = x[batch_idx * batch_size:min((batch_idx + 1) * batch_size, num)]
-                xrawbatch = x_raw[batch_idx * batch_size:min((batch_idx + 1) * batch_size, num)]
-                sfbatch = size_factor[batch_idx * batch_size:min((batch_idx + 1) * batch_size, num)]
-                pbatch = p[batch_idx * batch_size:min((batch_idx + 1) * batch_size, num)]
-                optimizer.zero_grad()
-                inputs = xbatch.to(self.device)
-                rawinputs = xrawbatch.to(self.device)
-                sfinputs = sfbatch.to(self.device)
-                target = pbatch.to(self.device)
-
-                zbatch, qbatch, meanbatch, dispbatch, pibatch = self.forward(inputs)
-
-                cluster_loss = self.cluster_loss(target, qbatch)
-                recon_loss = self.zinb_loss(rawinputs, meanbatch, dispbatch, pibatch, sfinputs)
-
-                loss = cluster_loss * self.gamma + recon_loss
-                loss.backward()
-                optimizer.step()
-                cluster_loss_val += cluster_loss.item() * len(inputs)
-                recon_loss_val += recon_loss.item() * len(inputs)
-                train_loss += loss.item() * len(inputs)
-
-            logger.info("Epoch %3d: Total: %.8f, Clustering Loss: %.8f, ZINB Loss: %.8f", epoch + 1, train_loss / num,
-                        cluster_loss_val / num, recon_loss_val / num)
-
-        index = update_interval * np.argmax(aris)
-        self.q = Q[f"epoch{index}"]
-
-    def predict_proba(self, x: Optional[Any] = None) -> np.ndarray:
-        """Get the predicted propabilities for each cell.
-
-        Parameters
-        ----------
-        x
-            Not used, for compatibility with the BaseClusteringMethod class.
+        id2label : np.ndarray
+            Id to label diction.
+        test_dict : dict
+            The test dictionary.
 
         Returns
         -------
-        pred_prop
-            Predicted probability for each cell.
+        dict
+            A dictionary where the keys are the test dataset IDs and the values are the corresponding predictions.
 
         """
-        pred_prob = self.q.detach().clone().cpu().numpy()
-        return pred_prob
+        self.id2label = id2label
+        self.test_dict = test_dict
+        return {num: self.inference(num) for num in self.params.test_dataset}
 
-    def predict(self, x: Optional[Any] = None) -> np.ndarray:
-        """Get predictions from the trained model.
+    @torch.no_grad()
+    def score(self, predicted_labels, true_labels):
+        """Compute model performance on test datasets based on accuracy.
 
         Parameters
         ----------
-        x
-            Not used, for compatibility with the BaseClusteringMethod class.
+        predicted_labels : dict
+            A dictionary where the keys are test dataset IDs and the values are the predicted labels.
+        true_labels : dict
+            A dictionary where the keys are test dataset IDs and the values are the true labels of the cells. Each
+            element, i.e., the label, can be either a specific value (e.g., string or intger) or a set of values,
+            allowing multiple mappings.
 
         Returns
         -------
-        pred
-            Predicted clustering assignment for each cell.
+        dict
+            A diction of correct prediction numbers, total samples, unsured prediction numbers, and accuracy.
 
         """
-        pred = self.predict_proba().argmax(1)
-        return pred
-
-
-class MeanAct(nn.Module):
-    """Mean activation class."""
-
-    def __init__(self):
-        super().__init__()
+        output_score = {}
+        for num in set(predicted_labels) & set(true_labels):
+            total_num = len(predicted_labels[num])
+            unsure_num = correct = 0
+            for pred, true in zip(predicted_labels[num], true_labels[num]):
+                if pred == "unsure":
+                    unsure_num += 1
+                elif pred == true or pred in true:  # either a single mapping or multiple mappings
+                    correct += 1
+
+            output_score[num] = {
+                "Total number of predictions": total_num,
+                "Number of correct predictions": correct,
+                "Number of unsure predictions": unsure_num,
+                "Accuracy": correct / total_num,
+            }
+
+        return output_score
+
+    def save_pred(self, num, pred):
+        """Save predictions for a particular test dataset.
 
-    def forward(self, x):
-        return torch.clamp(torch.exp(x), min=1e-5, max=1e6)
-
-
-class DispAct(nn.Module):
-    """Dispersion activation class."""
-
-    def __init__(self):
-        super().__init__()
-
-    def forward(self, x):
-        return torch.clamp(F.softplus(x), min=1e-4, max=1e4)
+        Parameters
+        ----------
+        num : int
+            Test file number.
+        pred : list np.array or dataframe
+            Predicted labels.
+
+        """
+        label_map = pd.read_excel("./map/celltype2subtype.xlsx", sheet_name=self.params.species, header=0,
+                                  names=["species", "old_type", "new_type", "new_subtype"])
+        label_map = label_map.fillna("N/A", inplace=False)
+        oldtype2newtype = {}
+        oldtype2newsubtype = {}
+        for _, old_type, new_type, new_subtype in label_map.itertuples(index=False):
+            oldtype2newtype[old_type] = new_type
+            oldtype2newsubtype[old_type] = new_subtype
+
+        save_path = self.prj_path / self.params.save_dir
+        if not save_path.exists():
+            save_path.mkdir()
+        if self.params.score:
+            df = pd.DataFrame({
+                "index": self.test_dict["origin_id"][num],
+                "original label": self.test_dict["label"][num],
+                "cell_type": [oldtype2newtype.get(p, p) for p in pred],
+                "cell_subtype": [oldtype2newsubtype.get(p, p) for p in pred]
+            })
+        else:
+            df = pd.DataFrame({
+                "index": self.test_dict["origin_id"][num],
+                "cell_type": [oldtype2newtype.get(p, p) for p in pred],
+                "cell_subtype": [oldtype2newsubtype.get(p, p) for p in pred]
+            })
+        df.to_csv(save_path / (self.params.species + f"_{self.params.tissue}_{num}.csv"), index=False)
+        print(f"output has been stored in {self.params.species}_{self.params.tissue}_{num}.csv")
```

### Comparing `pydance-1.0.0/dance/modules/single_modality/clustering/scdsc.py` & `pydance-1.0.0rc0/dance/modules/single_modality/clustering/scdsc.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,453 +4,352 @@
 
 Reference
 ----------
 Gan, Yanglan, et al. "Deep structural clustering for single-cell RNA-seq data jointly through autoencoder and graph
 neural network." Briefings in Bioinformatics 23.2 (2022): bbac018.
 
 """
+
+import math
+
 import numpy as np
-import pandas as pd
-import scanpy as sc
-import scipy.sparse as sp
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+from sklearn import metrics
 from torch.nn import Linear
 from torch.nn.parameter import Parameter
 from torch.optim import Adam
-from torch.utils.data import DataLoader, TensorDataset
+from torch.optim.optimizer import Optimizer
+from torch.utils.data import DataLoader
+from tqdm import tqdm
 
-from dance import logger
-from dance.modules.base import BaseClusteringMethod, TorchNNPretrain
-from dance.transforms import AnnDataTransform, Compose, SaveRaw, SetConfig
-from dance.transforms.graph import NeighborGraph
-from dance.transforms.preprocess import sparse_mx_to_torch_sparse_tensor
-from dance.typing import Any, LogLevel, Optional, Tuple
-from dance.utils import get_device
+from dance.transforms.preprocess import load_graph
 from dance.utils.loss import ZINBLoss
+from dance.utils.metrics import cluster_acc
 
 
-class ScDSC(TorchNNPretrain, BaseClusteringMethod):
-    """ScDSC wrapper class.
+class SCDSCWrapper:
+    """scDSC wrapper class.
 
     Parameters
     ----------
-    pretrain_path
-        Path of saved autoencoder weights.
-    sigma
-        Balance parameter.
-    n_enc_1
-        Output dimension of encoder layer 1.
-    n_enc_2
-        Output dimension of encoder layer 2.
-    n_enc_3
-        Output dimension of encoder layer 3.
-    n_dec_1
-        Output dimension of decoder layer 1.
-    n_dec_2
-        Output dimension of decoder layer 2.
-    n_dec_3
-        Output dimension of decoder layer 3.
-    n_z1
-        Output dimension of hidden layer 1.
-    n_z2
-        Output dimension of hidden layer 2.
-    n_z3
-        Output dimension of hidden layer 3.
-    n_clusters
-        Number of clusters.
-    n_input
-        Input feature dimension.
-    v
-        Parameter of soft assignment.
-    device
-        Computing device.
+    args : argparse.Namespace
+        a Namespace contains arguments of scDSC. For details of parameters in parser args, please refer to link (parser help document).
 
     """
 
-    def __init__(
-        self,
-        pretrain_path: str,
-        sigma: float = 1,
-        n_enc_1: int = 512,
-        n_enc_2: int = 256,
-        n_enc_3: int = 256,
-        n_dec_1: int = 256,
-        n_dec_2: int = 256,
-        n_dec_3: int = 512,
-        n_z1: int = 256,
-        n_z2: int = 128,
-        n_z3: int = 32,
-        n_clusters: int = 100,
-        n_input: int = 10,
-        v: float = 1,
-        device: str = "auto",
-    ):
+    def __init__(self, args):
         super().__init__()
-        self.pretrain_path = pretrain_path
-        self.device = get_device(device)
-        self.model = ScDSCModel(
-            sigma=sigma,
-            n_enc_1=n_enc_1,
-            n_enc_2=n_enc_2,
-            n_enc_3=n_enc_3,
-            n_dec_1=n_dec_1,
-            n_dec_2=n_dec_2,
-            n_dec_3=n_dec_3,
-            n_z1=n_z1,
-            n_z2=n_z2,
-            n_z3=n_z3,
-            n_clusters=n_clusters,
-            n_input=n_input,
-            v=v,
-            device=self.device,
-        ).to(self.device)
-        self.fix_module("model.ae")
-
-    @staticmethod
-    def preprocessing_pipeline(n_top_genes: int = 2000, n_neighbors: int = 50, log_level: LogLevel = "INFO"):
-        return Compose(
-            # Filter data
-            AnnDataTransform(sc.pp.filter_genes, min_counts=3),
-            AnnDataTransform(sc.pp.filter_cells, min_counts=1),
-            AnnDataTransform(sc.pp.normalize_per_cell),
-            AnnDataTransform(sc.pp.log1p),
-            AnnDataTransform(sc.pp.highly_variable_genes, min_mean=0.0125, max_mean=4, flavor="cell_ranger",
-                             min_disp=0.5, n_top_genes=n_top_genes, subset=True),
-            # Normalize data
-            AnnDataTransform(sc.pp.filter_genes, min_counts=1),
-            AnnDataTransform(sc.pp.filter_cells, min_counts=1),
-            SaveRaw(),
-            AnnDataTransform(sc.pp.normalize_total),
-            AnnDataTransform(sc.pp.log1p),
-            AnnDataTransform(sc.pp.scale),
-            # Construct k-neighbors graph using the noramlized feature matrix
-            NeighborGraph(n_neighbors=n_neighbors, metric="correlation", channel="X"),
-            SetConfig({
-                "feature_channel": ["NeighborGraph", None, None, "n_counts"],
-                "feature_channel_type": ["obsp", "X", "raw_X", "obs"],
-                "label_channel": "Group"
-            }),
-            log_level=log_level,
-        )
+        self.args = args
+        self.device = args.device
+        self.model = SCDSC(args).to(self.device)
+        self.model_pre = AE(n_enc_1=args.n_enc_1, n_enc_2=args.n_enc_2, n_enc_3=args.n_enc_3, n_dec_1=args.n_dec_1,
+                            n_dec_2=args.n_dec_2, n_dec_3=args.n_dec_3, n_input=args.n_input, n_z1=args.n_z1,
+                            n_z2=args.n_z2, n_z3=args.n_z3).to(self.device)
 
     def target_distribution(self, q):
         """Calculate auxiliary target distribution p with q.
 
         Parameters
         ----------
-        q
-            Soft label.
+        q :
+            soft label.
 
         Returns
         -------
-        p
-            Target distribution.
+        p :
+            target distribution.
 
         """
         p = q**2 / q.sum(0)
         return (p.t() / p.sum(1)).t()
 
-    def pretrain(self, x, batch_size=256, epochs=200, lr=1e-3):
+    def pretrain_ae(self, dataset, batch_size, n_epochs, fname, lr=1e-3):
         """Pretrain autoencoder.
 
         Parameters
         ----------
-        x
-            Input features.
-        batch_size
-            Size of batch.
-        epochs
-            Number of epochs.
-        lr
-            Learning rate.
+        dataset :
+            input dataset.
+        batch_size : int
+            size of batch.
+        n_epochs : int
+            number of epochs.
+        lr : float optional
+            learning rate.
+        fname : str
+            path to save autoencoder weights.
+
+        Returns
+        -------
+        None.
 
         """
-        with self.pretrain_context("model.ae"):
-            x_tensor = torch.from_numpy(x)
-            train_loader = DataLoader(TensorDataset(x_tensor), batch_size, shuffle=True)
-            model = self.model.ae
-            optimizer = Adam(model.parameters(), lr=lr)
-            for epoch in range(epochs):
-
-                total_loss = total_size = 0
-                for batch_idx, (x_batch, ) in enumerate(train_loader):
-                    x_batch = x_batch.to(self.device)
-                    x_bar, _, _, _, _, _, _, _ = model(x_batch)
-
-                    loss = F.mse_loss(x_bar, x_batch)
-                    optimizer.zero_grad()
-                    loss.backward()
-                    optimizer.step()
-
-                    size = x_batch.shape[0]
-                    total_size += size
-                    total_loss += loss.item() * size
-
-                logger.info(f"Pretrain epoch {epoch + 1:4d}, MSE loss:{total_loss / total_size:.8f}")
-
-    def save_pretrained(self, path):
-        torch.save(self.model.ae.state_dict(), path)
-
-    def load_pretrained(self, path):
-        checkpoint = torch.load(self.pretrain_path, map_location=self.device)
-        self.model.ae.load_state_dict(checkpoint)
-
-    def fit(
-        self,
-        inputs: Tuple[sp.spmatrix, np.ndarray, np.ndarray, pd.Series],
-        y: np.ndarray,
-        lr: float = 1e-03,
-        epochs: int = 300,
-        bcl: float = 0.1,
-        cl: float = 0.01,
-        rl: float = 1,
-        zl: float = 0.1,
-        pt_epochs: int = 200,
-        pt_batch_size: int = 256,
-        pt_lr: float = 1e-3,
-    ):
+        device = self.device
+        train_loader = DataLoader(dataset, batch_size, shuffle=True)
+        model = self.model_pre
+        optimizer = Adam(model.parameters(), lr=lr)
+        for epoch in range(n_epochs):
+            for batch_idx, (x, _) in enumerate(train_loader):
+                x = x.to(device)
+                x_bar, _, _, _, _, _, _, _ = model(x)
+
+                x_bar = x_bar.cpu()
+                x = x.cpu()
+                loss = F.mse_loss(x_bar, x)
+                optimizer.zero_grad()
+                loss.backward()
+                optimizer.step()
+
+            with torch.no_grad():
+                x = torch.Tensor(dataset.x).to(device).float()
+                x_bar, _, _, _, z3, _, _, _ = model(x)
+                loss = F.mse_loss(x_bar, x)
+                print('Pretrain epoch %3d, MSE loss: %.8f' % (epoch + 1, loss))
+
+        torch.save(model.state_dict(), fname)
+
+    def fit(self, dataset, X_raw, sf, graph_path, lr=1e-03, n_epochs=300, bcl=0.1, cl=0.01, rl=1, zl=0.1):
         """Train model.
 
         Parameters
         ----------
-        inputs
-            A tuple containing (1) the adjacency matrix, (2) the input features, (3) the raw input features, and (4)
-            the total counts for each cell.
-        y
-            Label.
-        lr
-            Learning rate.
-        epochs
-            Number of epochs.
-        bcl
-            Parameter of binary crossentropy loss.
-        cl
-            Parameter of Kullback–Leibler divergence loss.
-        rl
-            Parameter of reconstruction loss.
-        zl
-            Parameter of ZINB loss.
+        dataset :
+            input dataset.
+        X_raw :
+            raw input features.
+        sf : list
+            scale factor of ZINB loss.
+        graph_path : str
+            path of graph file.
+        lr : float optional
+            learning rate.
+        n_epochs : int optional
+            number of epochs.
+        bcl : float optional
+            parameter of binary crossentropy loss.
+        cl : float optional
+            parameter of Kullback–Leibler divergence loss.
+        rl : float optional
+            parameter of reconstruction loss.
+        zl : float optional
+            parameter of ZINB loss.
 
-        """
-        adj, x, x_raw, n_counts = inputs
-        self._pretrain(x, batch_size=pt_batch_size, epochs=pt_epochs, lr=pt_lr)
+        Returns
+        -------
+        None.
 
+        """
         device = self.device
         model = self.model
-        optimizer = Adam(filter(lambda x: x.requires_grad, model.parameters()), lr=lr)
+        optimizer = Adam(model.parameters(), lr=lr)
+        # optimizer = RAdam(model.parameters(), lr=lr)
 
-        adj = sparse_mx_to_torch_sparse_tensor(adj).to(device)
-        x_raw = torch.tensor(x_raw).to(device)
-        sf = torch.tensor(n_counts / np.median(n_counts)).to(device)
-        data = torch.from_numpy(x).to(device)
+        adj = load_graph(graph_path, dataset.x)
+        adj = adj.to(device)
+        X_raw = torch.tensor(X_raw).to(device)
+        sf = torch.tensor(sf).to(device)
+        data = torch.Tensor(dataset.x).to(device)
+        y = dataset.y
 
         aris = []
-        keys = []
         P = {}
         Q = {}
 
         with torch.no_grad():
             _, _, _, _, z, _, _, _ = model.ae(data)
 
-        for epoch in range(epochs):
+        for epoch in range(n_epochs):
             if epoch % 10 == 0:
                 model.eval()
                 with torch.no_grad():
                     x_bar, tmp_q, pred, z, meanbatch, dispbatch, pibatch, zinb_loss = model(data, adj)
                     tmp_q = tmp_q.data
                     self.q = tmp_q
                     p = self.target_distribution(tmp_q)
 
                     # calculate ari score for model selection
-                    ari = self.score(None, y)
+                    _, _, ari = self.score(y)
                     aris.append(ari)
-                    keys.append(key := f"epoch{epoch}")
-                    logger.info("Epoch %3d, ARI: %.4f, Best ARI: %.4f", epoch + 1, ari, max(aris))
+                    print("Epoch %3d, ARI: %.4f, Best ARI: %.4f" % (epoch + 1, ari, max(aris)))
 
-                    P[key] = p
-                    Q[key] = tmp_q
+                    p_ = {f'epoch{epoch}': p}
+                    q_ = {f'epoch{epoch}': tmp_q}
+                    P = {**P, **p_}
+                    Q = {**Q, **q_}
 
             model.train()
             x_bar, q, pred, z, meanbatch, dispbatch, pibatch, zinb_loss = model(data, adj)
 
             binary_crossentropy_loss = F.binary_cross_entropy(q, p)
-            ce_loss = F.kl_div(pred.log(), p, reduction="batchmean")
+            ce_loss = F.kl_div(pred.log(), p, reduction='batchmean')
             re_loss = F.mse_loss(x_bar, data)
-            zinb_loss = zinb_loss(x_raw, meanbatch, dispbatch, pibatch, sf)
+            zinb_loss = zinb_loss(X_raw, meanbatch, dispbatch, pibatch, sf)
             loss = bcl * binary_crossentropy_loss + cl * ce_loss + rl * re_loss + zl * zinb_loss
 
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
 
         index = np.argmax(aris)
-        self.q = Q[keys[index]]
+        self.q = Q[f'epoch{index}']
 
-    def predict_proba(self, x: Optional[Any] = None) -> np.ndarray:
-        """Get the predicted propabilities for each cell.
+    def predict(self):
+        """Get predictions from the trained model.
 
         Parameters
         ----------
-        x
-            Not used, for compatibility with the BaseClusteringMethod class.
+        None.
 
         Returns
         -------
-        pred_prop
-            Predicted probability for each cell.
+        y_pred : np.array
+            prediction of given clustering method.
 
         """
-        pred_prob = self.q.detach().clone().cpu().numpy()
-        return pred_prob
+        y_pred = torch.argmax(self.q, dim=1).data.cpu().numpy()
+        return y_pred
 
-    def predict(self, x: Optional[Any] = None) -> np.ndarray:
-        """Get predictions from the trained model.
+    def score(self, y):
+        """Evaluate the trained model.
 
         Parameters
         ----------
-        x
-            Not used, for compatibility with the BaseClusteringMethod class.
+        y : list
+            true labels.
 
         Returns
         -------
-        pred
-            Predicted clustering assignment for each cell.
+        acc : float
+            accuracy.
+        nmi : float
+            normalized mutual information.
+        ari : float
+            adjusted Rand index.
 
         """
-        pred = self.predict_proba().argmax(1)
-        return pred
+        y_pred = torch.argmax(self.q, dim=1).data.cpu().numpy()
+        acc = np.round(cluster_acc(y, y_pred), 5)
+        nmi = np.round(metrics.normalized_mutual_info_score(y, y_pred), 5)
+        ari = np.round(metrics.adjusted_rand_score(y, y_pred), 5)
+        return acc, nmi, ari
 
 
-class ScDSCModel(nn.Module):
-    """ScDSC class.
+class SCDSC(nn.Module):
+    """scDSC class.
 
     Parameters
     ----------
-    sigma
-        Balance parameter.
-    n_enc_1
-        Output dimension of encoder layer 1.
-    n_enc_2
-        Output dimension of encoder layer 2.
-    n_enc_3
-        Output dimension of encoder layer 3.
-    n_dec_1
-        Output dimension of decoder layer 1.
-    n_dec_2
-        Output dimension of decoder layer 2.
-    n_dec_3
-        Output dimension of decoder layer 3.
-    n_z1
-        Output dimension of hidden layer 1.
-    n_z2
-        Output dimension of hidden layer 2.
-    n_z3
-        Output dimension of hidden layer 3.
-    n_clusters
-        Number of clusters.
-    n_input
-        Input feature dimension.
-    v
-        Parameter of soft assignment.
-    device
-        Computing device.
+    args : argparse.Namespace
+        a Namespace contains arguments of GCNAE. For details of parameters in parser args, please refer to link (parser help document).
+    device : str
+        computing device.
+    sigma : float
+        balance parameter.
+    pretrain_path : str
+        path of saved autoencoder weights.
+    n_enc_1 : int
+        output dimension of encoder layer 1.
+    n_enc_2 : int
+        output dimension of encoder layer 2.
+    n_enc_3 : int
+        output dimension of encoder layer 3.
+    n_dec_1 : int
+        output dimension of decoder layer 1.
+    n_dec_2 : int
+        output dimension of decoder layer 2.
+    n_dec_3 : int
+        output dimension of decoder layer 3.
+    n_z1 : int
+        output dimension of hidden layer 1.
+    n_z2 : int
+        output dimension of hidden layer 2.
+    n_z3 : int
+        output dimension of hidden layer 3.
+    n_clusters : int
+        number of clusters.
+    n_input : int
+        input feature dimension.
+    v : float
+        parameter of soft assignment.
 
     """
 
-    def __init__(
-        self,
-        sigma: float = 1,
-        n_enc_1: int = 512,
-        n_enc_2: int = 256,
-        n_enc_3: int = 256,
-        n_dec_1: int = 256,
-        n_dec_2: int = 256,
-        n_dec_3: int = 512,
-        n_z1: int = 256,
-        n_z2: int = 128,
-        n_z3: int = 32,
-        n_clusters: int = 10,
-        n_input: int = 100,
-        v: float = 1,
-        device: str = "auto",
-    ):
+    def __init__(self, args):
         super().__init__()
-        self.device = get_device(device)
-        self.sigma = sigma
-
+        device = args.device
+        self.sigma = args.sigma
+        self.pretrain_path = args.pretrain_path
         self.ae = AE(
-            n_enc_1=n_enc_1,
-            n_enc_2=n_enc_2,
-            n_enc_3=n_enc_3,
-            n_dec_1=n_dec_1,
-            n_dec_2=n_dec_2,
-            n_dec_3=n_dec_3,
-            n_input=n_input,
-            n_z1=n_z1,
-            n_z2=n_z2,
-            n_z3=n_z3,
+            n_enc_1=args.n_enc_1,
+            n_enc_2=args.n_enc_2,
+            n_enc_3=args.n_enc_3,
+            n_dec_1=args.n_dec_1,
+            n_dec_2=args.n_dec_2,
+            n_dec_3=args.n_dec_3,
+            n_input=args.n_input,
+            n_z1=args.n_z1,
+            n_z2=args.n_z2,
+            n_z3=args.n_z3,
         )
-
-        self.gnn_1 = GNNLayer(n_input, n_enc_1)
-        self.gnn_2 = GNNLayer(n_enc_1, n_enc_2)
-        self.gnn_3 = GNNLayer(n_enc_2, n_enc_3)
-        self.gnn_4 = GNNLayer(n_enc_3, n_z1)
-        self.gnn_5 = GNNLayer(n_z1, n_z2)
-        self.gnn_6 = GNNLayer(n_z2, n_z3)
-        self.gnn_7 = GNNLayer(n_z3, n_clusters)
+        self.gnn_1 = GNNLayer(args.n_input, args.n_enc_1)
+        self.gnn_2 = GNNLayer(args.n_enc_1, args.n_enc_2)
+        self.gnn_3 = GNNLayer(args.n_enc_2, args.n_enc_3)
+        self.gnn_4 = GNNLayer(args.n_enc_3, args.n_z1)
+        self.gnn_5 = GNNLayer(args.n_z1, args.n_z2)
+        self.gnn_6 = GNNLayer(args.n_z2, args.n_z3)
+        self.gnn_7 = GNNLayer(args.n_z3, args.n_clusters)
 
         # cluster layer
-        self.cluster_layer = Parameter(torch.Tensor(n_clusters, n_z3))
+        self.cluster_layer = Parameter(torch.Tensor(args.n_clusters, args.n_z3))
         torch.nn.init.xavier_normal_(self.cluster_layer.data)
-        self._dec_mean = nn.Sequential(nn.Linear(n_dec_3, n_input), MeanAct())
-        self._dec_disp = nn.Sequential(nn.Linear(n_dec_3, n_input), DispAct())
-        self._dec_pi = nn.Sequential(nn.Linear(n_dec_3, n_input), nn.Sigmoid())
+        self._dec_mean = nn.Sequential(nn.Linear(args.n_dec_3, args.n_input), MeanAct())
+        self._dec_disp = nn.Sequential(nn.Linear(args.n_dec_3, args.n_input), DispAct())
+        self._dec_pi = nn.Sequential(nn.Linear(args.n_dec_3, args.n_input), nn.Sigmoid())
         # degree
-        self.v = v
-        self.zinb_loss = ZINBLoss().to(self.device)
-
-        self.to(self.device)
+        self.v = args.v
+        self.zinb_loss = ZINBLoss().to(device)
 
     def forward(self, x, adj):
         """Forward propagation.
 
         Parameters
         ----------
-        x
-            Input features.
-        adj
-            Adjacency matrix
+        x :
+            input features.
+        adj :
+            adjacency matrix
 
         Returns
         -------
         x_bar:
-            Reconstructed features.
-        q
-            Soft label.
+            reconstructed features.
+        q :
+            soft label.
         predict:
-            Prediction given by softmax assignment of embedding of GCN module
-        z3
-            Embedding of autoencoder.
-        _mean
-            Data mean from ZINB.
-        _disp
-            Data dispersion from ZINB.
-        _pi
-            Data dropout probability from ZINB.
+            prediction given by softmax assignment of embedding of GCN module
+        z3 :
+            embedding of autoencoder.
+        _mean :
+            data mean from ZINB.
+        _disp :
+            data dispersion from ZINB.
+        _pi :
+            data dropout probability from ZINB.
         zinb_loss:
             ZINB loss class.
 
         """
         # DNN Module
+        self.ae.load_state_dict(torch.load(self.pretrain_path, map_location='cpu'))
         x_bar, tra1, tra2, tra3, z3, z2, z1, dec_h3 = self.ae(x)
 
-        # GCN Module
         sigma = self.sigma
+        # GCN Module
         h = self.gnn_1(x, adj)
         h = self.gnn_2((1 - sigma) * h + sigma * tra1, adj)
         h = self.gnn_3((1 - sigma) * h + sigma * tra2, adj)
         h = self.gnn_4((1 - sigma) * h + sigma * tra3, adj)
         h = self.gnn_5((1 - sigma) * h + sigma * z1, adj)
         h = self.gnn_6((1 - sigma) * h + sigma * z2, adj)
         h = self.gnn_7((1 - sigma) * h + sigma * z3, adj, active=False)
@@ -470,18 +369,18 @@
 
 
 class GNNLayer(nn.Module):
     """GNN layer class. Construct a GNN layer with corresponding dimensions.
 
     Parameters
     ----------
-    in_features
-        Input dimension of GNN layer.
-    out_features
-        Output dimension of GNN layer.
+    in_features : int
+        input dimension of GNN layer.
+    out_features : int
+        output dimension of GNN layer.
 
     """
 
     def __init__(self, in_features, out_features):
         super().__init__()
         self.in_features = in_features
         self.out_features = out_features
@@ -499,34 +398,34 @@
 
 
 class AE(nn.Module):
     """Autoencoder class.
 
     Parameters
     ----------
-    n_enc_1
-        Output dimension of encoder layer 1.
-    n_enc_2
-        Output dimension of encoder layer 2.
-    n_enc_3
-        Output dimension of encoder layer 3.
-    n_dec_1
-        Output dimension of decoder layer 1.
-    n_dec_2
-        Output dimension of decoder layer 2.
-    n_dec_3
-        Output dimension of decoder layer 3.
-    n_input
-        Input feature dimension.
-    n_z1
-        Output dimension of hidden layer 1.
-    n_z2
-        Output dimension of hidden layer 2.
-    n_z3
-        Output dimension of hidden layer 3.
+    n_enc_1 : int
+        output dimension of encoder layer 1.
+    n_enc_2 : int
+        output dimension of encoder layer 2.
+    n_enc_3 : int
+        output dimension of encoder layer 3.
+    n_dec_1 : int
+        output dimension of decoder layer 1.
+    n_dec_2 : int
+        output dimension of decoder layer 2.
+    n_dec_3 : int
+        output dimension of decoder layer 3.
+    n_input : int
+        input feature dimension.
+    n_z1 : int
+        output dimension of hidden layer 1.
+    n_z2 : int
+        output dimension of hidden layer 2.
+    n_z3 : int
+        output dimension of hidden layer 3.
 
     """
 
     def __init__(self, n_enc_1, n_enc_2, n_enc_3, n_dec_1, n_dec_2, n_dec_3, n_input, n_z1, n_z2, n_z3):
         super().__init__()
 
         self.enc_1 = Linear(n_input, n_enc_1)
@@ -552,35 +451,35 @@
         self.x_bar_layer = Linear(n_dec_3, n_input)
 
     def forward(self, x):
         """Forward propagation.
 
         Parameters
         ----------
-        x
-            Input features.
+        x :
+            input features.
 
         Returns
         -------
-        x_bar
-            Reconstructed features.
-        enc_h1
-            Output of encoder layer 1.
-        enc_h2
-            Output of encoder layer 2.
-        enc_h3
-            Output of encoder layer 3.
-        z3
-            Output of hidden layer 3.
-        z2
-            Output of hidden layer 2.
-        z1
-            Output of hidden layer 1.
-        dec_h3
-            Output of decoder layer 3.
+        x_bar:
+            reconstructed features.
+        enc_h1:
+            output of encoder layer 1.
+        enc_h2:
+            output of encoder layer 2.
+        enc_h3:
+            output of encoder layer 3.
+        z3 :
+            output of hidden layer 3.
+        z2 :
+            output of hidden layer 2.
+        z1 :
+            output of hidden layer 1.
+        dec_h3 :
+            output of decoder layer 3.
 
         """
         enc_h1 = F.relu(self.BN1(self.enc_1(x)))
         enc_h2 = F.relu(self.BN2(self.enc_2(enc_h1)))
         enc_h3 = F.relu(self.BN3(self.enc_3(enc_h2)))
 
         z1 = self.BN4(self.z1_layer(enc_h3))
@@ -591,14 +490,127 @@
         dec_h2 = F.relu(self.BN8(self.dec_2(dec_h1)))
         dec_h3 = F.relu(self.BN9(self.dec_3(dec_h2)))
         x_bar = self.x_bar_layer(dec_h3)
 
         return x_bar, enc_h1, enc_h2, enc_h3, z3, z2, z1, dec_h3
 
 
+class RAdam(Optimizer):
+    """RAdam optimizer class.
+
+    Parameters
+    ----------
+    params :
+        model parameters.
+    lr : float optional
+        learning rate.
+    betas : tuple optional
+        coefficients used for computing running averages of gradient and its square.
+    eps : float optional
+        term added to the denominator to improve numerical stability.
+    weight decay : float optional
+        weight decay (L2 penalty).
+    degenerated_to_sgd : bool optional
+        degenerated to SGD or not.
+
+    """
+
+    def __init__(self, params, lr=1e-3, betas=(0.9, 0.999), eps=1e-8, weight_decay=0, degenerated_to_sgd=True):
+        if not 0.0 <= lr:
+            raise ValueError("Invalid learning rate: {}".format(lr))
+        if not 0.0 <= eps:
+            raise ValueError("Invalid epsilon value: {}".format(eps))
+        if not 0.0 <= betas[0] < 1.0:
+            raise ValueError("Invalid beta parameter at index 0: {}".format(betas[0]))
+        if not 0.0 <= betas[1] < 1.0:
+            raise ValueError("Invalid beta parameter at index 1: {}".format(betas[1]))
+
+        self.degenerated_to_sgd = degenerated_to_sgd
+        if isinstance(params, (list, tuple)) and len(params) > 0 and isinstance(params[0], dict):
+            for param in params:
+                if 'betas' in param and (param['betas'][0] != betas[0] or param['betas'][1] != betas[1]):
+                    param['buffer'] = [[None, None, None] for _ in range(10)]
+        defaults = dict(lr=lr, betas=betas, eps=eps, weight_decay=weight_decay,
+                        buffer=[[None, None, None] for _ in range(10)])
+        super().__init__(params, defaults)
+
+    def __setstate__(self, state):
+        super().__setstate__(state)
+
+    def step(self, closure=None):
+
+        loss = None
+        if closure is not None:
+            loss = closure()
+
+        for group in self.param_groups:
+
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+                grad = p.grad.data.float()
+                if grad.is_sparse:
+                    raise RuntimeError('RAdam does not support sparse gradients')
+
+                p_data_fp32 = p.data.float()
+
+                state = self.state[p]
+
+                if len(state) == 0:
+                    state['step'] = 0
+                    state['exp_avg'] = torch.zeros_like(p_data_fp32)
+                    state['exp_avg_sq'] = torch.zeros_like(p_data_fp32)
+                else:
+                    state['exp_avg'] = state['exp_avg'].type_as(p_data_fp32)
+                    state['exp_avg_sq'] = state['exp_avg_sq'].type_as(p_data_fp32)
+
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
+                beta1, beta2 = group['betas']
+
+                exp_avg_sq.mul_(beta2).addcmul_(1 - beta2, grad, grad)
+                exp_avg.mul_(beta1).add_(1 - beta1, grad)
+
+                state['step'] += 1
+                buffered = group['buffer'][int(state['step'] % 10)]
+                if state['step'] == buffered[0]:
+                    N_sma, step_size = buffered[1], buffered[2]
+                else:
+                    buffered[0] = state['step']
+                    beta2_t = beta2**state['step']
+                    N_sma_max = 2 / (1 - beta2) - 1
+                    N_sma = N_sma_max - 2 * state['step'] * beta2_t / (1 - beta2_t)
+                    buffered[1] = N_sma
+
+                    # more conservative since it's an approximated value
+                    if N_sma >= 5:
+                        step_size = math.sqrt(
+                            (1 - beta2_t) * (N_sma - 4) / (N_sma_max - 4) * (N_sma - 2) / N_sma * N_sma_max /
+                            (N_sma_max - 2)) / (1 - beta1**state['step'])
+                    elif self.degenerated_to_sgd:
+                        step_size = 1.0 / (1 - beta1**state['step'])
+                    else:
+                        step_size = -1
+                    buffered[2] = step_size
+
+                # more conservative since it's an approximated value
+                if N_sma >= 5:
+                    if group['weight_decay'] != 0:
+                        p_data_fp32.add_(-group['weight_decay'] * group['lr'], p_data_fp32)
+                    denom = exp_avg_sq.sqrt().add_(group['eps'])
+                    p_data_fp32.addcdiv_(-step_size * group['lr'], exp_avg, denom)
+                    p.data.copy_(p_data_fp32)
+                elif step_size > 0:
+                    if group['weight_decay'] != 0:
+                        p_data_fp32.add_(-group['weight_decay'] * group['lr'], p_data_fp32)
+                    p_data_fp32.add_(-step_size * group['lr'], exp_avg)
+                    p.data.copy_(p_data_fp32)
+
+        return loss
+
+
 class MeanAct(nn.Module):
     """Mean activation class."""
 
     def __init__(self):
         super().__init__()
 
     def forward(self, x):
```

### Comparing `pydance-1.0.0/dance/modules/single_modality/imputation/deepimpute.py` & `pydance-1.0.0rc0/dance/modules/single_modality/clustering/sctag.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,414 +1,470 @@
-"""Reimplementation of DeepImpute.
+"""Reimplementation of scTAG.
 
-Extended from https://github.com/lanagarmire/DeepImpute
+Extended from https://github.com/Philyzh8/scTAG
 
 Reference
 ----------
-Arisdakessian, Cédric, et al. "DeepImpute: an accurate, fast, and scalable deep neural network method to impute
-single-cell RNA-seq data." Genome biology 20.1 (2019): 1-14.
+Yu, Z., Y. Lu, Y. Wang, F. Tang, K.-C. Wong, and X. Li. “ZINB-Based Graph Embedding Autoencoder for Single-Cell RNA-Seq
+Interpretations”. Proceedings of the AAAI Conference on Artificial Intelligence, vol. 36, no. 4, June 2022, pp. 4671-9,
+doi:10.1609/aaai.v36i4.20392.
 
 """
 
-import tempfile
-from math import floor
-from pathlib import Path
-
-import anndata as ad
+import dgl
 import numpy as np
-import pandas as pd
-import scanpy as sc
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
-from sklearn.metrics import adjusted_rand_score
-from torch.utils.data import DataLoader, TensorDataset
+from dgl.nn import TAGConv
+from sklearn import metrics
+from sklearn.cluster import KMeans
+from torch.nn import Parameter
+from tqdm import tqdm
 
-from dance.modules.base import BaseRegressionMethod
-from dance.transforms import (AnnDataTransform, CellwiseMaskData, Compose, FilterCellsScanpy, FilterGenesScanpy,
-                              GeneHoldout, SaveRaw, SetConfig)
-from dance.typing import Any, List, LogLevel, Optional, Tuple
+from dance.utils.loss import ZINBLoss, dist_loss
+from dance.utils.metrics import cluster_acc
 
 
-class NeuralNetworkModel(nn.Module):
-    """Model class.
+class SCTAG(nn.Module):
+    """scTAG class.
 
     Parameters
     ----------
-    None
-    Returns
-    -------
-    None
+    X :
+        input features.
+    adj :
+        adjacency matrix.
+    adj_n :
+        normalized adjacency matrix.
+    n_clusters : int
+        number of clusters.
+    k : int optional
+        number of hops of TAG convolutional layer.
+    hidden_dim : int optional
+        dimension of hidden layer.
+    latent_dim : int optional
+        dimension of latent embedding.
+    dec_dim : list optional
+        dimensions of decoder layers.
+    adj_dim : int optional
+        dimension of adjacency matrix.
+    dropout : float optional
+        dropout rate.
+    device : str optional
+        computing device.
+    alpha : float optional
+        parameter of soft assign.
 
     """
 
-    def __init__(self, inputdim, sub_outputdim, hidden_dim=None, dropout=0.2):
+    def __init__(self, X, adj, adj_n, n_clusters, k=3, hidden_dim=128, latent_dim=15, dec_dim=None, adj_dim=32,
+                 dropout=0.2, device="cuda", alpha=1.0):
         super().__init__()
-        if (hidden_dim is None):
-            hidden_dim = floor(sub_outputdim / 2)
-        self.layer1 = nn.Linear(inputdim, hidden_dim)
-        self.layer2 = nn.Dropout(p=dropout)
-        self.layer3 = nn.Linear(hidden_dim, sub_outputdim)
-
-    def forward(self, x):
-        x = F.relu(self.layer1(x))
-        x = self.layer2(x)
-        x = F.softplus(self.layer3(x))
-        return (x)
-
+        if dec_dim is None:
+            dec_dim = [128, 256, 512]
+        self.latent_dim = latent_dim
+        self.hidden_dim = hidden_dim
+        self.adj = adj
+        self.adj_n = adj_n
+        self.n_sample = X.shape[0]
+        self.in_dim = X.shape[1]
+        self.device = device
+        self.dropout = dropout
+        self.n_clusters = n_clusters
+        self.alpha = alpha
+        self.k = k
+        self.adj_dim = adj_dim
+        self.mu = Parameter(torch.Tensor(self.n_clusters, self.latent_dim).to(self.device))
+
+        src, dist = np.nonzero(adj)
+        self.G = dgl.graph((src, dist)).to(device)
+
+        src_n, dist_n = np.nonzero(adj_n)
+        self.G_n = dgl.graph((src_n, dist_n)).to(device)
+
+        self.encoder1 = TAGConv(self.in_dim, self.hidden_dim, k=k)
+        self.encoder2 = TAGConv(self.hidden_dim, self.latent_dim, k=k)
+        self.decoderA = DecoderA(latent_dim=self.latent_dim, adj_dim=self.adj_dim, activation=torch.sigmoid,
+                                 dropout=self.dropout)
+        self.decoderX = DecoderX(self.in_dim, self.latent_dim, n_dec_1=dec_dim[0], n_dec_2=dec_dim[1],
+                                 n_dec_3=dec_dim[2])
+        self.zinb_loss = ZINBLoss().to(self.device)
+        self.to(self.device)
 
-class DeepImpute(nn.Module, BaseRegressionMethod):
-    """DeepImpute class.
+    def forward(self, A_in, X_input):
+        """Forward propagation.
 
-    Parameters
-    ----------
-    learning_rate : float optional
-        learning rate
-    batch_size : int optional
-        batch size
-    max_epochs : int optional
-        maximum epochs
-
-    patience : int optional
-        number of epochs before stopping once loss stops to improve
-    gpu : int optional
-        option to use gpu
-    loss : string optional
-        loss function
-    output_prefix : string optinal
-        directory to save outputs
-    sub_outputdim : int optional
-        output dimensions in each subnetwork
-    hidden_dim : int optional
-        dimension of the dense layer in each subnetwork
+        Parameters
+        ----------
+        A_in :
+            input adjacency matrix.
+        X_input :
+            input features.
 
-    verbose: int optional
-        verbose option
+        Returns
+        -------
+        A_out :
+            reconstructed adjacency matrix.
+        z :
+            embedding.
+        q :
+            soft label.
+        _mean :
+            data mean from ZINB.
+        _disp :
+            data dispersion from ZINB.
+        _pi :
+            data dropout probability from ZINB.
 
-    seed: int optional
-        random seed
-    architecture: optional
-        network architecture
+        """
+        enc_h = self.encoder1(A_in, X_input)
+        z = self.encoder2(A_in, enc_h)
+        A_out = self.decoderA(z)
+        _mean, _disp, _pi = self.decoderX(z)
+        q = self.soft_assign(z)
+
+        return A_out, z, q, _mean, _disp, _pi
+
+    def pre_train(self, x, x_raw, fname, scale_factor, epochs=1000, info_step=10, lr=5e-4, W_a=0.3, W_x=1, W_d=0,
+                  min_dist=0.5, max_dist=20.):
+        """Pretrain autoencoder.
 
-    imputed_only: boolean optional
-        whether to return imputed genes only
+        Parameters
+        ----------
+        x :
+            input features.
+        x_raw :
+            raw input features.
+        fname : str
+            path to save autoencoder weights.
+        scale_factor : list
+            scale factor of input features and raw input features.
+        epochs : int optional
+            number of epochs.
+        info_step : int optional
+            interval of showing pretraining loss.
+        lr : float optional
+            learning rate.
+        W_a : float optional
+            parameter of reconstruction loss.
+        W_x : float optional
+            parameter of ZINB loss.
+        W_d : float optional
+            parameter of pairwise distance loss.
+        min_dist : float optional
+            minimum distance of pairwise distance loss.
+        max_dist : float optional
+            maximum distance of pairwise distance loss.
 
-    policy: string optional
-        imputation policy
+        Returns
+        -------
+        None.
 
-    """
+        """
+        x = torch.Tensor(x).to(self.device)
+        x_raw = torch.Tensor(x_raw).to(self.device)
+        scale_factor = torch.tensor(scale_factor).to(self.device)
+
+        self.train()
+        optimizer = optim.Adam(filter(lambda p: p.requires_grad, self.parameters()), lr=lr, amsgrad=True)
+        print("Pretraining stage")
+        for epoch in range(epochs):
+            A_out, z, _, mean, disp, pi = self.forward(self.G_n, x)
+
+            if W_d:
+                Dist_loss = torch.mean(dist_loss(z, min_dist, max_dist=max_dist))
+            A_rec_loss = torch.mean(F.mse_loss(A_out, torch.Tensor(self.adj).to(self.device)))
+            Zinb_loss = self.zinb_loss(x_raw, mean, disp, pi, scale_factor)
+            loss = W_a * A_rec_loss + W_x * Zinb_loss
+            if W_d:
+                loss += W_d * Dist_loss
+
+            if epoch % info_step == 0:
+                if W_d:
+                    print("Epoch %3d: ZINB Loss: %.8f, MSE Loss: %.8f, Dist Loss: %.8f" %
+                          (epoch + 1, Zinb_loss.item(), A_rec_loss.item(), Dist_loss.item()))
+                else:
+                    print("Epoch %3d: ZINB Loss: %.8f, MSE Loss: %.8f" %
+                          (epoch + 1, Zinb_loss.item(), A_rec_loss.item()))
 
-    def __init__(self, predictors, targets, dataset, sub_outputdim=512, hidden_dim=256, dropout=0.2, seed=1, gpu=-1):
-        super().__init__()
-        self.seed = seed
-        self.predictors = predictors
-        self.targets = targets
-        self.dataset = dataset
-        self.sub_outputdim = sub_outputdim
-        self.dropout = dropout
-        self.hidden_dim = hidden_dim
-        self.prj_path = Path(__file__).parent.resolve()
-        self.save_path = self.prj_path / "deepimpute"
-        if not self.save_path.exists():
-            self.save_path.mkdir(parents=True)
-        self.device = torch.device(f'cuda:{gpu}' if gpu != -1 and torch.cuda.is_available() else 'cpu')
-        self.models = self.build([len(genes) for genes in predictors], [len(genes) for genes in targets], self.device)
-
-    @staticmethod
-    def preprocessing_pipeline(min_cells: float = 0.1, n_top: int = 5, sub_outputdim: int = 512, mask: bool = True,
-                               distr: str = "exp", mask_rate: float = 0.1, seed: int = 1, log_level: LogLevel = "INFO"):
-
-        transforms = [
-            FilterGenesScanpy(min_cells=min_cells),
-            FilterCellsScanpy(min_counts=1),
-            SaveRaw(),
-            AnnDataTransform(sc.pp.log1p),
-            GeneHoldout(n_top=n_top, batch_size=sub_outputdim),
-        ]
-        if mask:
-            transforms.extend([
-                CellwiseMaskData(distr=distr, mask_rate=mask_rate, seed=seed),
-                SetConfig({
-                    "feature_channel": [None, None, "targets", "predictors", "train_mask"],
-                    "feature_channel_type": ["X", "raw_X", "uns", "uns", "layers"],
-                    "label_channel": [None, None],
-                    "label_channel_type": ["X", "raw_X"],
-                })
-            ])
-        else:
-            transforms.extend([
-                SetConfig({
-                    "feature_channel": [None, None, "targets", "predictors"],
-                    "feature_channel_type": ["X", "raw_X", "uns", "uns"],
-                    "label_channel": [None, None],
-                    "label_channel_type": ["X", "raw_X"],
-                })
-            ])
+            optimizer.zero_grad()
+            loss.backward()
+            optimizer.step()
 
-        return Compose(*transforms, log_level=log_level)
+        torch.save(self.state_dict(), fname)
+        print("Pre_train Finish!")
 
-    def wMSE(self, y_true, y_pred, binary=False):
-        """Weighted MSE.
+    def fit(self, x, x_raw, y, scale_factor, epochs=300, lr=5e-4, W_a=0.3, W_x=1, W_c=1.5, info_step=1):
+        """Pretrain autoencoder.
 
         Parameters
         ----------
-        y_true: array
-            true expression
-        Y_train: array
-            predicted expression
-        binary: boolean optional
-            whether to use binary weights
+        x :
+            input features.
+        x_raw :
+            raw input features.
+        y : list
+            true label.
+        scale_factor : list
+            scale factor of input features and raw input features.
+        epochs : int optional
+            number of epochs.
+        lr : float optional
+            learning rate.
+        W_a : float optional
+            parameter of reconstruction loss.
+        W_x : float optional
+            parameter of ZINB loss.
+        W_c : float optional
+            parameter of clustering loss.
+        info_step : int optional
+            interval of showing pretraining loss.
+
         Returns
         -------
-        val: float
-            weighted MSE
+        None.
 
         """
+        x = torch.Tensor(x).to(self.device)
+        x_raw = torch.Tensor(x_raw).to(self.device)
+        scale_factor = torch.tensor(scale_factor).to(self.device)
+
+        # Initializing cluster centers with kmeans
+        kmeans = KMeans(self.n_clusters, n_init=20)
+        enc_h = self.encoder1(self.G_n, x)
+        z = self.encoder2(self.G_n, enc_h)
+        kmeans.fit_predict(z.detach().cpu().numpy())
+        self.mu.data.copy_(torch.tensor(kmeans.cluster_centers_, dtype=torch.float32).to(self.device))
+
+        self.train()
+        optimizer = optim.Adam(filter(lambda p: p.requires_grad, self.parameters()), lr=lr, amsgrad=True)
+
+        aris = []
+        P = {}
+        Q = {}
+
+        for epoch in range(epochs):
+            A_out, _, q, mean, disp, pi = self.forward(self.G_n, x)
+            self.q = q
+            p = self.target_distribution(q)
+            self.y_pred = self.predict()
+
+            # calculate ari score for model selection
+            _, _, ari = self.score(y)
+            aris.append(ari)
+            p_ = {f'epoch{epoch}': p}
+            q_ = {f'epoch{epoch}': q}
+            P = {**P, **p_}
+            Q = {**Q, **q_}
+            if epoch % info_step == 0:
+                print("Epoch %3d, ARI: %.4f, Best ARI: %.4f" % (epoch + 1, ari, max(aris)))
+
+            A_rec_loss = torch.mean(F.mse_loss(A_out, torch.Tensor(self.adj).to(self.device)))
+            Zinb_loss = self.zinb_loss(x_raw, mean, disp, pi, scale_factor)
+            Cluster_loss = torch.mean(
+                F.kl_div(
+                    torch.Tensor(self.y_pred).to(self.device),
+                    torch.Tensor(y).to(self.device), reduction='batchmean'))
+            loss = W_a * A_rec_loss + W_x * Zinb_loss + W_c * Cluster_loss
+
+            optimizer.zero_grad()
+            loss.backward()
+            optimizer.step()
 
-        if binary:
-            tmp = y_true > 0
-            weights = tmp.type(torch.FloatTensor)
-        else:
-            weights = y_true
-        val = torch.mean(weights * torch.square(y_true - y_pred))
-        return val
+        index = np.argmax(aris)
+        self.q = Q[f'epoch{index}']
 
-    def build(self, inputdims, outputdims, device="cpu"):
-        """Build model.
+    def predict(self):
+        """Get predictions from the trained model.
 
         Parameters
         ----------
-        inputdims: int
-            number of neurons as input in the first layer
+        None.
+
         Returns
         -------
-        models : array
-            array of subnetworks
+        y_pred : np.array
+            prediction of given clustering method.
 
         """
-        models = []
-        for i in range(len(inputdims)):
-            models.append(
-                NeuralNetworkModel(inputdims[i], outputdims[i], hidden_dim=self.hidden_dim,
-                                   dropout=self.dropout).to(device))
-
-        return models
-
-    def maskdata(self, X, mask, idx=None):
-        if idx is None:
-            idx = range(len(X))
-        submask = mask[idx]
-        X_masked = torch.zeros_like(X).to(X.device)
-        X_masked[submask] = X[submask]
-        counter_submask = ~submask
+        y_pred = torch.argmax(self.q, dim=1).data.cpu().numpy()
+        return y_pred
 
-        return X_masked, submask, counter_submask
-
-    def fit(self, X, Y, train_idx, mask=None, batch_size=64, lr=1e-3, n_epochs=100, patience=5):
-        """Train model.
+    def score(self, y):
+        """Evaluate the trained model.
 
         Parameters
         ----------
-        X_train: optional
-            Training data including input genes
-        Y_train: optional
-            Training data including target genes to be inputed
-        X_valid:  optional
-            Validation data including input predictor genes
-        Y_valid:  optional
-            Validation data including target genes to be inputed
-        predictors: array optional
-            input genes as predictors for target genes
+        y : list
+            true labels.
+
         Returns
         -------
-        None
+        acc : float
+            accuracy.
+        nmi : float
+            normalized mutual information.
+        ari : float
+            adjusted Rand index.
 
         """
-        predictors = self.predictors
-        targets = self.targets
-        device = self.device
-
-        # Specify train validation split
-        if mask is not None:
-            X_train, _, valid_mask = self.maskdata(X, mask, train_idx)
-            X_valid = X_train
-            Y_valid = Y_train = Y
-        else:
-            rng = np.random.default_rng(self.seed)
-            train_data_masked = train_data
-            train_idx_permuted = rng.permutation(range(len(X)))
-            train_idx = train_idx_permuted[:int(len(train_idx_permuted) * 0.9)]
-            valid_idx = train_idx_permuted[int(len(train_idx_permuted) * 0.9):]
-            X_train = X[train_idx]
-            X_valid = X[valid_idx]
-            Y_train = Y[train_idx]
-            Y_valid = Y[valid_idx]
-            valid_mask = np.ones_like(X_valid.cpu()).astype(bool)
-
-        X_train_list, X_valid_list, Y_train_list, Y_valid_list, valid_mask_list = [], [], [], [], []
-        for j, inputgenes in enumerate(predictors):
-            X_train_list.append(X_train[:, inputgenes])
-            X_valid_list.append(X_valid[:, inputgenes])
-            Y_train_list.append(Y_train[:, targets[j]])
-            Y_valid_list.append(Y_valid[:, targets[j]])
-            valid_mask_list.append(valid_mask[:, targets[j]])
-
-        data = [TensorDataset(X_train_list[i], Y_train_list[i]) for i in range(len(predictors))]
-        train_loaders = [DataLoader(data[i], batch_size=batch_size, shuffle=True) for i in range(len(data))]
-        optimizers = [optim.Adam(model.parameters(), lr=lr) for model in self.models]
-
-        for i, model in enumerate(self.models):
-            optimizer = optimizers[i]
-            train_loader = train_loaders[i]
-            val_losses = []
-            counter = 0
-            for epoch in range(n_epochs):
-                model.train()
-                train_loss = 0
-                for batch_idx, (x_batch, y_batch) in enumerate(train_loader):
-                    y_pred = model(x_batch.to(device))
-                    loss = self.wMSE(y_batch.to(device), y_pred)
-                    loss.backward()
-                    optimizer.step()
-                    train_loss += loss.item() * len(x_batch)
-                train_loss = train_loss / len(X_train_list[i])
-
-                model.eval()
-                with torch.no_grad():
-                    y_pred = model(torch.Tensor(X_valid_list[i]).to(device))
-                    val_loss = F.mse_loss(y_pred[valid_mask_list[i]],
-                                          Y_valid_list[i].to(device)[valid_mask_list[i]]).item()
-                print("Model {:d}, epoch {:d}, train loss: {:f}, valid loss: {:f}.".format(
-                    i, epoch, train_loss, val_loss))
-
-                val_losses.append(val_loss)
-                min_val = min(val_losses)
-                if val_loss == min_val:
-                    self.save_model(model, optimizer, i)
-                else:
-                    counter += 1
-                    if counter == patience:
-                        print("Early stopped")
-                        break
+        y_pred = torch.argmax(self.q, dim=1).data.cpu().numpy()
+        acc = np.round(cluster_acc(y, y_pred), 5)
+        nmi = np.round(metrics.normalized_mutual_info_score(y, y_pred), 5)
+        ari = np.round(metrics.adjusted_rand_score(y, y_pred), 5)
+        return acc, nmi, ari
 
-    def save_model(self, model, optimizer, i):
-        """Save model.
+    def soft_assign(self, z):
+        """Soft assign q with z.
 
         Parameters
         ----------
-        model:
-            model to be saved
+        z :
+            embedding.
 
-        optimizer:
-            optimizer
-
-        i: int
-            index of the subnetwork to be loaded
         Returns
         -------
-        None
+        q :
+            soft label.
 
         """
+        q = 1.0 / (1.0 + torch.sum((z.unsqueeze(1) - self.mu)**2, dim=2) / self.alpha)
+        q = q**((self.alpha + 1.0) / 2.0)
+        q = (q.t() / torch.sum(q, dim=1)).t()
+        return q
 
-        model_string = 'model_' + str(i)
-        opt_string = 'optimizer_' + str(i)
-        state = {model_string: model.state_dict(), opt_string: optimizer.state_dict()}
-        torch.save(state, self.save_path / f"{self.dataset}_{i}.pt")
-
-    def load_model(self, model, i):
-        """Load model.
+    def target_distribution(self, q):
+        """Calculate auxiliary target distribution p with q.
 
         Parameters
         ----------
-        model:
-            model to be loaded
+        q :
+            soft label.
 
-        i: int
-            index of the subnetwork to be loaded
         Returns
         -------
-        model :
-            loaded model
+        p :
+            target distribution.
 
         """
+        p = q**2 / q.sum(0)
+        return (p.t() / p.sum(1)).t()
 
-        model_path = self.save_path / f"{self.dataset}_{i}.pt"
-        state = torch.load(model_path, map_location=self.device)
-        model_string = 'model_' + str(i)
-        model.load_state_dict(state[model_string])
-        return model
 
-    def predict(self, X_test, test_idx, mask=None):
-        """Get predictions from the trained model.
+class DecoderA(nn.Module):
+    """Decoder class for adjacency matrix reconstruction.
+
+    Parameters
+    ----------
+    latent_dim : int optional
+        dimension of latent embedding.
+    adj_dim : int optional
+        dimension of adjacency matrix.
+    activation : optional
+        activation function.
+    dropout : float optional
+        dropout rate.
+
+    """
+
+    def __init__(self, latent_dim=15, adj_dim=32, activation=torch.sigmoid, dropout=0):
+        super().__init__()
+        self.dropout = dropout
+        self.activation = activation
+        self.dec_1 = nn.Linear(latent_dim, adj_dim)
+
+    def forward(self, z):
+        """Forward propagation.
 
         Parameters
         ----------
-        targetgenes: array optional
-            genes to be imputed
+        z :
+            embedding.
+
         Returns
         -------
-        imputed : DataFrame
-            imputed gene expression
+        adj :
+            reconstructed adjacency matrix.
 
         """
-        predictors = self.predictors
-        targets = self.targets
+        dec_h = self.dec_1(z)
+        z0 = F.dropout(dec_h, self.dropout)
+        adj = self.activation(torch.mm(z0, z0.t()))
+        return adj
 
-        if mask is not None:
-            X_test, _, _ = self.maskdata(X_test, mask, test_idx)
-        X_test_list = []
-        for j, inputgenes in enumerate(predictors):
-            X_test_list.append(X_test[:, inputgenes])
-
-        # Make predictions using each subnetwork
-        Y_pred_lst = []
-        for i, model in enumerate(self.models):
-            model = self.load_model(model, i)
-            model.eval()
-            with torch.no_grad():
-                Y_pred_lst.append(model.forward(X_test_list[i].to(self.device)))
-        # Concatenate predicted values
-        Y_pred = torch.cat(Y_pred_lst, 1)
-        gene_order = np.concatenate(targets)
-        Y_pred = Y_pred[:, gene_order]
 
-        # Convert back to counts
-        Y_pred = torch.expm1(Y_pred)
+class DecoderX(nn.Module):
+    """scTAG class.
 
-        return Y_pred
+    Parameters
+    ----------
+    input_dim : int
+        dimension of input feature.
+    n_z : int
+        dimension of latent embedding.
+    n_dec_1 : int optional
+        number of nodes of decoder layer 1.
+    n_dec_2 : int optional
+        number of nodes of decoder layer 2.
+    n_dec_3 : int optional
+        number of nodes of decoder layer 3.
 
-    def score(self, true_expr, imputed_expr, test_idx, mask=None, metric="MSE"):
-        """Scoring function of model.
+    """
+
+    def __init__(self, input_dim, n_z, n_dec_1=128, n_dec_2=256, n_dec_3=512):
+        super().__init__()
+        self.n_dec_3 = n_dec_3
+        self.input_dim = input_dim
+        self.dec_1 = nn.Linear(n_z, n_dec_1)
+        self.dec_2 = nn.Linear(n_dec_1, n_dec_2)
+        self.dec_3 = nn.Linear(n_dec_2, n_dec_3)
+        self.dec_mean = nn.Sequential(nn.Linear(self.n_dec_3, self.input_dim), MeanAct())
+        self.dec_disp = nn.Sequential(nn.Linear(self.n_dec_3, self.input_dim), DispAct())
+        self.dec_pi = nn.Sequential(nn.Linear(self.n_dec_3, self.input_dim), nn.Sigmoid())
+
+    def forward(self, z):
+        """Forward propagation.
 
         Parameters
         ----------
-        true_expr :
-            True underlying expression values
-        imputed_expr :
-            Imputed expression values
-        test_idx :
-            index of testing cells
-        metric :
-            Choice of scoring metric - 'RMSE' or 'ARI'
+        z :
+            embedding.
 
         Returns
         -------
-        score :
-            evaluation score
+        _mean :
+            data mean from ZINB.
+        _disp :
+            data dispersion from ZINB.
+        _pi :
+            data dropout probability from ZINB.
 
         """
-        allowd_metrics = {"RMSE", "PCC"}
-        if metric not in allowd_metrics:
-            raise ValueError("scoring metric %r." % allowd_metrics)
-
-        true_target = true_expr.to(self.device)
-        imputed_target = imputed_expr.to(self.device)
-        if mask is not None:  # and metric == 'MSE':
-            # true_target = true_target[~mask[test_idx]]
-            # imputed_target = imputed_target[~mask[test_idx]]
-            imputed_target[mask[test_idx]] = true_target[mask[test_idx]]
-        if metric == 'RMSE':
-            return np.sqrt(F.mse_loss(true_target, imputed_target).item())
-        elif metric == 'PCC':
-            corr_cells = np.corrcoef(true_target.cpu(), imputed_target.cpu())
-            return corr_cells
+        dec_h1 = F.relu(self.dec_1(z))
+        dec_h2 = F.relu(self.dec_2(dec_h1))
+        dec_h3 = F.relu(self.dec_3(dec_h2))
+        _mean = self.dec_mean(dec_h3)
+        _disp = self.dec_disp(dec_h3)
+        _pi = self.dec_pi(dec_h3)
+        return _mean, _disp, _pi
+
+
+class MeanAct(nn.Module):
+    """Mean activation class."""
+
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, x):
+        return torch.clamp(torch.exp(x), min=1e-5, max=1e6)
+
+
+class DispAct(nn.Module):
+    """Dispersion activation class."""
+
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, x):
+        return torch.clamp(F.softplus(x), min=1e-4, max=1e4)
```

### Comparing `pydance-1.0.0/dance/modules/spatial/cell_type_deconvo/spotlight.py` & `pydance-1.0.0rc0/dance/modules/spatial/cell_type_deconvo/spatialdecon.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,210 +1,246 @@
-"""PyTorch reimplementation of the SPOTlight cell-type deconvolution method.
+"""A PyTorch reimplementation of the SpatialDecon cell-type deconvolution method.
 
-Adaptded from https://github.com/MarcElosua/SPOTlight
+Adapted from https: https://github.com/Nanostring-Biostats/SpatialDecon
 
 Reference
 ---------
-Elosua-Bayes, Nieto, Mereu, Gut, and Heyn H. "SPOTlight: seeded NMF regression to deconvolute spatial transcriptomics
-spots with single-cell transcriptomes." Nucleic Acids Research (2021)
+Danaher, Kim, Nelson, et al. "Advances in mixed cell deconvolution enable quantification of cell types in spatial transcriptomic data."
+Nature Communications (2022)
 
 """
-from functools import partial
-
 import numpy as np
 import torch
-from torch import nn, optim
-from torchnmf.nmf import NMF
-
-from dance import logger
-from dance.modules.base import BaseRegressionMethod
-from dance.transforms import SetConfig
-from dance.transforms.pseudo_gen import get_ct_profile
-from dance.typing import Any, List, LogLevel, Optional
-from dance.utils import get_device
-from dance.utils.wrappers import CastOutputType
+import torch.nn as nn
+import torch.nn.functional as F
+from torch import optim
+from torch.autograd import Variable
 
-get_ct_profile_tensor = CastOutputType(torch.FloatTensor)(partial(get_ct_profile, method="median"))
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 
-class NNLS(nn.Module):
-    """NNLS.
+class MSLELoss(nn.Module):
+    """MSLELoss.
 
     Parameters
     ----------
-    in_dim
-        Input dimension.
-    out_dim
-        Output dimension.
-    bias
-        Include bias term, default False.
+    None
+
+    Returns
+    -------
+    None.
 
     """
 
-    def __init__(self, in_dim, out_dim, bias=False, init_bias=None, device="auto"):
+    def __init__(self):
         super().__init__()
-        self.device = get_device(device)
-        self.model = nn.Linear(in_features=in_dim, out_features=out_dim, bias=bias)
-        self.model.bias = init_bias
-        self.model = self.model.to(self.device)
-
-    def forward(self, x: torch.Tensor):
-        out = self.model(x)
-        return (out)
+        self.mse = nn.MSELoss()
 
-    def fit(self, x, y, max_iter, lr, print_res=False, print_period=100):
-        """Fit function for model training.
+    def forward(self, pred, actual):
+        """forward function.
 
         Parameters
         ----------
-        x
-            Input.
-        y
-            Output.
-        max_iter
-            Maximum number of iterations for optimizat.
-        lr
-            Learning rate.
-        print_res
-            Indicates to print live training results, default False.
-        print_period
-            Indicates number of iterations until training results print.
+        pred : torch tensor
+            linear transformation of cell profile (reference basis) matrix.
+        actual : torch tensor
+            mixture expression matrix.
+
+        Returns
+        -------
+        loss : float
+            mean squared log error loss.
 
         """
-        criterion = nn.MSELoss()
-        optimizer = optim.Adam(self.model.parameters(), lr=lr)
+        pred_clamp = pred.clamp(min=0)
+        actual_clamp = actual.clamp(min=0)
+        loss = self.mse(torch.log1p(pred_clamp), torch.log1p(actual_clamp))
+        return loss
 
-        self.model.train()
-        for iteration in range(max_iter):
-            iteration += 1
-            y_pred = self.model(x)
 
-            # Compute and print loss
-            loss = criterion(y_pred, y)
+def cell_topic_profile(X, groups, ct_select, axis=0, method='median'):
+    """cell_topic_profile.
 
-            optimizer.zero_grad()
-            loss.backward()
-            optimizer.step()
+    Parameters
+    ----------
+    X : torch 2-d tensor
+        gene expression matrix, genes (rows) by sample cells (cols).
+    groups : int
+        cell-type labels of each sample cell in X.
+    ct_select:
+        cell types to profile.
+    method : string optional
+         method for reduction of cell-types for cell profile, default median.
 
-            # Force non-negative weights only
-            with torch.no_grad():
-                self.model.weight.copy_(self.model.weight.data.clamp(min=0))
+    Returns
+        -------
+    X_profile : torch 2-d tensor
+         cell profile matrix from scRNA-seq reference.
 
-            if iteration % print_period == 0:
-                logger.info(f"Epoch: {iteration:02}/{max_iter} Loss: {loss.item():.5e}")
+    """
+    if method == "median":
+        X_profile = np.array([
+            np.median(X[[i for i in range(len(groups)) if groups[i] == ct_select[j]], :], axis=0)
+            for j in range(len(ct_select))
+        ]).T
+    else:
+        X_profile = np.array([
+            np.mean(X[[i for i in range(len(groups)) if groups[i] == ct_select[j]], :], axis=0)
+            for j in range(len(ct_select))
+        ]).T
+    return X_profile
 
 
-class SPOTlight(BaseRegressionMethod):
-    """SPOTlight.
+class SpatialDecon:
+    """SpatialDecon.
 
     Parameters
     ----------
-    ref_count
-        Reference single cell RNA-seq counts data (cell x gene).
-    ref_annot
+    sc_count : pd.DataFrame
+        Reference single cell RNA-seq counts data.
+    sc_annot : pd.DataFrame
         Reference cell-type label information.
-    ct_select
+    mix_count : pd.DataFrame
+        Target mixed-cell RNA-seq counts data to be deconvoluted.
+    ct_varname : str, optional
+        Name of the cell-types column.
+    ct_select : str, optional
         Selected cell-types to be considered for deconvolution.
-    rank
-        Rank of the matrix factorization.
-    bias
-        Include bias term, default False.
-    init_bias
-        Initial bias term (background estimate).
+    sc_profile: numpy array optional
+        pre-constructed cell profile matrix.
+    bias : boolean optional
+        include bias term, default False.
+    init_bias: numpy array optional
+        initial bias term (background estimate).
+
+    Returns
+    -------
+    None.
 
     """
 
-    def __init__(
-        self,
-        ref_count: np.ndarray,
-        ref_annot: np.ndarray,
-        ct_select: List[str],
-        rank: int = 2,
-        bias=False,
-        init_bias=None,
-        device="auto",
-    ):
-        self.ref_count = ref_count
-        self.ref_annot = ref_annot
-        self.ct_select = ct_select
-
-        self.bias = bias
-        self.rank = rank
-
-        self.device = get_device(device)
-
-    @staticmethod
-    def preprocessing_pipeline(log_level: LogLevel = "INFO"):
-        return SetConfig({"label_channel": "cell_type_portion"}, log_level=log_level)
-
-    def _init_model(self, dim_out, ref_count, ref_annot):
-        hid_dim = len(self.ct_select)
-        self.nmf_model = NMF(Vshape=ref_count.T.shape, rank=self.rank).to(self.device)
-        if self.rank == len(self.ct_select):  # initialize basis as cell profile
-            self.nmf_model.H = nn.Parameter(get_ct_profile_tensor(ref_count, ref_annot, ct_select=self.ct_select))
-
-        self.nnls_reg1 = NNLS(in_dim=self.rank, out_dim=dim_out, bias=self.bias, device=self.device)
-        self.nnls_reg2 = NNLS(in_dim=hid_dim, out_dim=dim_out, bias=self.bias, device=self.device)
-
-        self.model = nn.Sequential(self.nmf_model, self.nnls_reg1, self.nnls_reg2)
-
-    def fit(
-        self,
-        x: torch.Tensor,
-        lr: float = 1e-3,
-        max_iter: int = 1000,
-    ):
-        """Fit function for model training.
+    def __init__(self, sc_count, sc_annot, mix_count, ct_varname, ct_select, sc_profile=None, bias=False,
+                 init_bias=None, device=torch.device("cuda" if torch.cuda.is_available() else "cpu")):
+        super().__init__()
+
+        self.device = device
+
+        #subset sc samples on selected cell types (mutual between sc and mix cell data)
+        ct_select_ix = sc_annot[sc_annot[ct_varname].isin(ct_select)].index
+        self.sc_annot = sc_annot.loc[ct_select_ix]
+        self.sc_count = sc_count.loc[ct_select_ix]
+        cellTypes = self.sc_annot[ct_varname].values.tolist()
+
+        #construct a cell profile matrix if not profided
+        if sc_profile is None:
+            self.ref_sc_profile = cell_topic_profile(self.sc_count.values, cellTypes, ct_select, method='median')
+        else:
+            self.ref_sc_profile = sc_profile
+
+        self.mix_count = mix_count.values.T
+
+        in_dim = self.ref_sc_profile.shape[1]
+        out_dim = self.mix_count.shape[1]
+        self.model = nn.Linear(in_features=in_dim, out_features=out_dim, bias=bias)
+        if init_bias is not None:
+            self.model.bias = nn.Parameter(torch.Tensor(init_bias.values.T.copy()))
+        self.model = self.model.to(device)
+
+    def forward(self, x: torch.Tensor):
+        """forward function.
 
         Parameters
         ----------
-        x
-            Mixed cell expression to be deconvoluted (cell x gene).
-        lr
-            Learning rate.
-        max_iter
-            Maximum iterations allowed for matrix factorization solver.
+        x : torch tensor
+            input features.
+
+        Returns
+        -------
+        output : torch tensor
+            linear projection of input.
 
         """
-        ref_annot = self.ref_annot
-        ct_select = self.ct_select
-        device = self.device
-
-        self._init_model(x.shape[0], self.ref_count, ref_annot)
-        x = x.T.to(device)
-        x_ref = torch.FloatTensor(self.ref_count.T).to(device)
-
-        # Run NMF on scRNA X
-        self.nmf_model.fit(x_ref, max_iter=max_iter)
-        self.nmf_model.requires_grad_(False)
-        self.W = self.nmf_model.H.clone()
-        self.H = self.nmf_model.W.clone().T
-
-        # Get cell-topic profiles H_profile: cell-type group medians of coef H (topic x cells)
-        self.H_profile = get_ct_profile_tensor(self.H.cpu().numpy().T, ref_annot, ct_select=ct_select).to(device)
-
-        # Get mix-topic profiles B: NNLS of basis W onto mix expression X ~ W*b
-        # nnls ran for each spot
-        self.nnls_reg1.fit(self.W, x, max_iter=max_iter, lr=lr)
-        self.nnls_reg1.requires_grad_(False)
-        self.B = self.nnls_reg1.model.weight.clone().T
-
-        # Get cell-type proportions P: NNLS of cell-topic profile H_profile onoto mix-topic profile B -- b ~ h_profile*p
-        self.nnls_reg2.fit(self.H_profile, self.B, max_iter=max_iter, lr=lr)
-        self.nnls_reg2.requires_grad_(False)
-        self.P = self.nnls_reg2.model.weight.clone().T
+        out = self.model(x)
+        return (out)
+
+    def predict(self):
+        """prediction function.
+        Parameters
+        ----------
+
+        Returns
+        -------
+
+        proportion_preds : torch tensor
+            predictions of cell-type proportions.
+
+        """
+        proportion_preds = self.model.weight.T
+        proportion_preds = proportion_preds / torch.sum(proportion_preds, axis=0, keepdims=True).clamp(min=1e-6)
+        return (proportion_preds)
+
+    def fit(self, lr, max_iter, print_res=False, print_period=100):
+        """fit function for model training.
+
+        Parameters
+        ----------
+        max_iter : int
+            maximum number of iterations for optimizat.
+        lr : float
+            learning rate.
+        print_res : bool optional
+            indicates to print live training results, default False.
+        print_period : int optional
+            indicates number of iterations until training results print.
+
+        Returns
+        -------
+        None.
 
-    def predict(self, x: Optional[Any] = None):
-        """Prediction function.
+        """
+        ref_sc_profile = Variable(torch.FloatTensor(self.ref_sc_profile), requires_grad=True).to(self.device)
+        mix_count = Variable(torch.FloatTensor(self.mix_count)).to(self.device)
+
+        criterion = MSLELoss()
+        optimizer = optim.Adam(self.model.parameters(), lr=lr)
+
+        self.model.train()
+        for iteration in range(max_iter):
+            iteration += 1
+            mix_pred = self.model(ref_sc_profile)
+
+            # Compute and print loss
+            loss = criterion(mix_pred, mix_count)
+            self.loss = loss
+            # Zero gradients, perform a backward pass,
+            # and update the weights.
+            optimizer.zero_grad()
+            loss.backward()
+            optimizer.step()
+
+            with torch.no_grad():
+                self.model.weight.copy_(self.model.weight.data.clamp(min=0))
+            if iteration % print_period == 0:
+                print(f"Epoch: {iteration:02}/{max_iter} Loss: {loss.item():.5e}")
+
+    def score(self, pred, true_prop):
+        """score.
 
         Parameters
         ----------
-        x
-            Not used, for compatibility with the BaseRegressionMethod class.
+        pred :
+            predicted cell-type proportions.
+        true_prop :
+            true cell-type proportions.
 
         Returns
         -------
-        pred
-            Predicted cell-type proportions (cell x cell-type).
+        loss : float
+            mse loss between predicted and true cell-type proportions.
 
         """
-        return nn.functional.normalize(self.P.detach().clone().cpu().T, dim=1, p=1)
+        true_prop = true_prop.to(self.device)
+        pred = pred / torch.sum(pred, 1, keepdims=True).clamp(min=1e-6)
+        true_prop = true_prop / torch.sum(true_prop, 1, keepdims=True).clamp(min=1e-6)
+        loss = ((pred - true_prop)**2).mean()
+
+        return loss.detach().item()
```

### Comparing `pydance-1.0.0/dance/modules/spatial/spatial_domain/louvain.py` & `pydance-1.0.0rc0/dance/modules/spatial/spatial_domain/louvain.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,36 +3,30 @@
 Extended from https://github.com/taynaud/python-louvain
 
 Reference
 ----------
 Blondel, V. D., et al. "Fast Unfolding of Community Hierarchies in Large Networks, 1–6 (2008)." arXiv:0803.0476.
 
 """
+
 import array
 import numbers
 import warnings
 
 import networkx as nx
 import numpy as np
-import scanpy as sc
-
-from dance import logger
-from dance.modules.base import BaseClusteringMethod
-from dance.transforms import AnnDataTransform, CellPCA, Compose, FilterGenesMatch, SetConfig
-from dance.transforms.graph import NeighborGraph
-from dance.typing import LogLevel
 
-PASS_MAX = -1
-MIN = 0.0000001
+# coding=utf-8
 
 
 class Status:
     """To handle several data in one struct.
 
-    Could be replaced by named tuple, but don't want to depend on python 2.6
+    Could be replaced by named tuple, but don't want to depend on python
+    2.6
 
     """
     node2com = {}
     total_weight = 0
     internals = {}
     degrees = {}
     gdegrees = {}
@@ -84,27 +78,31 @@
             for node in graph.nodes():
                 com = part[node]
                 self.node2com[node] = com
                 deg = float(graph.degree(node, weight=weight))
                 self.degrees[com] = self.degrees.get(com, 0) + deg
                 self.gdegrees[node] = deg
                 inc = 0.
-                for neighbor, data in graph[node].items():
-                    edge_weight = data.get(weight, 1)
+                for neighbor, datas in graph[node].items():
+                    edge_weight = datas.get(weight, 1)
                     if edge_weight <= 0:
                         error = "Bad graph type ({})".format(type(graph))
                         raise ValueError(error)
                     if part[neighbor] == com:
                         if neighbor == node:
                             inc += float(edge_weight)
                         else:
                             inc += float(edge_weight) / 2.
                 self.internals[com] = self.internals.get(com, 0) + inc
 
 
+__PASS_MAX = -1
+__MIN = 0.0000001
+
+
 def check_random_state(seed):
     """Turn seed into a np.random.RandomState instance.
 
     Parameters
     ----------
     seed : None | int | instance of RandomState
         If seed is None, return the RandomState singleton used by np.random.
@@ -130,22 +128,22 @@
     Level 0 is the first partition, which contains the smallest communities,
     and the best is len(dendrogram) - 1.
     The higher the level is, the bigger are the communities
 
     Parameters
     ----------
     dendrogram : list of dict
-       a list of partitions, ie dictionaries where keys of the i+1 are the
+       a list of partitions, ie dictionnaries where keys of the i+1 are the
        values of the i.
     level : int
        the level which belongs to [0..len(dendrogram)-1]
 
     Returns
     -------
-    partition : dictionary
+    partition : dictionnary
        A dictionary where keys are the nodes and the values are the set it
        belongs to
 
     Raises
     ------
     KeyError
        If the dendrogram is not well formed or the level is too high
@@ -166,26 +164,26 @@
     partition = dendrogram[0].copy()
     for index in range(1, level + 1):
         for node, community in partition.items():
             partition[node] = dendrogram[index][community]
     return partition
 
 
-def modularity(partition, graph, weight="weight"):
+def modularity(partition, graph, weight='weight'):
     """Compute the modularity of a partition of a graph.
 
     Parameters
     ----------
     partition : dict
        the partition of the nodes, i.e a dictionary where keys are their nodes
        and values the communities
     graph : networkx.Graph
        the networkx graph which is decomposed
-    weight : str
-        the key in graph to use as weight. Default to "weight"
+    weight : str, optional
+        the key in graph to use as weight. Default to 'weight'
 
 
     Returns
     -------
     modularity : float
        The modularity
 
@@ -220,62 +218,62 @@
     links = graph.size(weight=weight)
     if links == 0:
         raise ValueError("A graph without link has an undefined modularity")
 
     for node in graph:
         com = partition[node]
         deg[com] = deg.get(com, 0.) + graph.degree(node, weight=weight)
-        for neighbor, data in graph[node].items():
-            edge_weight = data.get(weight, 1)
+        for neighbor, datas in graph[node].items():
+            edge_weight = datas.get(weight, 1)
             if partition[neighbor] == com:
                 if neighbor == node:
                     inc[com] = inc.get(com, 0.) + float(edge_weight)
                 else:
                     inc[com] = inc.get(com, 0.) + float(edge_weight) / 2.
 
     res = 0.
     for com in set(partition.values()):
         res += (inc.get(com, 0.) / links) - \
                (deg.get(com, 0.) / (2. * links)) ** 2
     return res
 
 
-def best_partition(graph, partition=None, weight="weight", resolution=1., randomize=None, random_state=None):
+def best_partition(graph, partition=None, weight='weight', resolution=1., randomize=None, random_state=None):
     """Compute the partition of the graph nodes which maximises the modularity (or
     try..) using the Louvain heuristices.
 
     This is the partition of highest modularity, i.e. the highest partition
     of the dendrogram generated by the Louvain algorithm.
 
     Parameters
     ----------
     graph : networkx.Graph
        the networkx graph which is decomposed
-    partition : dict
+    partition : dict, optional
        the algorithm will start using this partition of the nodes.
        It's a dictionary where keys are their nodes and values the communities
-    weight : str
-        the key in graph to use as weight. Default to "weight"
-    resolution :  double
+    weight : str, optional
+        the key in graph to use as weight. Default to 'weight'
+    resolution :  double, optional
         Will change the size of the communities, default to 1.
         represents the time described in
         "Laplacian Dynamics and Multiscale Modular Structure in Networks",
         R. Lambiotte, J.-C. Delvenne, M. Barahona
-    randomize : boolean
+    randomize : boolean, optional
         Will randomize the node evaluation order and the community evaluation
         order to get different partitions at each call
-    random_state : int, RandomState instance or None
+    random_state : int, RandomState instance or None, optional (default=None)
         If int, random_state is the seed used by the random number generator;
         If RandomState instance, random_state is the random number generator;
         If None, the random number generator is the RandomState instance used
-        by :func:`numpy.random`.
+        by `np.random`.
 
     Returns
     -------
-    partition : dictionary
+    partition : dictionnary
        The partition, with communities numbered from 0 to number of communities
 
     Raises
     ------
     NetworkXError
        If the graph is not undirected.
 
@@ -294,15 +292,15 @@
 
     Examples
     --------
     >>> # basic usage
     >>> import community as community_louvain
     >>> import networkx as nx
     >>> G = nx.erdos_renyi_graph(100, 0.01)
-    >>> partition = community_louvain.best_partition(G)
+    >>> partion = community_louvain.best_partition(G)
 
     >>> # display a graph with its communities:
     >>> # as Erdos-Renyi graphs don't have true community structure,
     >>> # instead load the karate club graph
     >>> import community as community_louvain
     >>> import matplotlib.cm as cm
     >>> import matplotlib.pyplot as plt
@@ -310,111 +308,120 @@
     >>> G = nx.karate_club_graph()
     >>> # compute the best partition
     >>> partition = community_louvain.best_partition(G)
 
     >>> # draw the graph
     >>> pos = nx.spring_layout(G)
     >>> # color the nodes according to their partition
-    >>> cmap = cm.get_cmap("viridis", max(partition.values()) + 1)
+    >>> cmap = cm.get_cmap('viridis', max(partition.values()) + 1)
     >>> nx.draw_networkx_nodes(G, pos, partition.keys(), node_size=40,
     >>>                        cmap=cmap, node_color=list(partition.values()))
     >>> nx.draw_networkx_edges(G, pos, alpha=0.5)
     >>> plt.show()
 
     """
     dendo = generate_dendrogram(graph, partition, weight, resolution, randomize, random_state)
     return partition_at_level(dendo, len(dendo) - 1)
 
 
-class Louvain(BaseClusteringMethod):
-    """Louvain classBaseClassificationMethod.
-
-    Parameters
-    ----------
-    resolution
-        Resolution parameter.
-
-    """
-
-    def __init__(self, resolution: float = 1):
-        self.resolution = resolution
-
-    @staticmethod
-    def preprocessing_pipeline(dim: int = 50, n_neighbors: int = 17, log_level: LogLevel = "INFO"):
-        return Compose(
-            FilterGenesMatch(prefixes=["ERCC", "MT-"]),
-            AnnDataTransform(sc.pp.normalize_total, target_sum=1e4),
-            AnnDataTransform(sc.pp.log1p),
-            CellPCA(n_components=dim),
-            NeighborGraph(n_neighbors=n_neighbors),
-            SetConfig({
-                "feature_channel": "NeighborGraph",
-                "feature_channel_type": "obsp",
-                "label_channel": "label",
-                "label_channel_type": "obs"
-            }),
-            log_level=log_level,
-        )
+class Louvain:
+    """Louvain class."""
 
-    def fit(self, adj, partition=None, weight="weight", randomize=None, random_state=None):
-        """Fit function for model training.
+    def fit(self, adata, adj, partition=None, weight='weight', resolution=1., randomize=None, random_state=None):
+        """fit function for model training.
 
         Parameters
         ----------
+        adata :
+            input data.
         adj :
             adjacent matrix.
-        partition : dict
+        partition : dict optional
             a dictionary where keys are graph nodes and values the part the node
             belongs to
-        weight : str
-            the key in graph to use as weight. Default to "weight"
-        randomize : boolean
+        weight : str, optional
+            the key in graph to use as weight. Default to 'weight'
+        resolution : float optional
+            resolution.
+        randomize : boolean, optional
             Will randomize the node evaluation order and the community evaluation
             order to get different partitions at each call
-        random_state : int, RandomState instance or None
+        random_state : int, RandomState instance or None, optional (default=None)
             If int, random_state is the seed used by the random number generator;
             If RandomState instance, random_state is the random number generator;
             If None, the random number generator is the RandomState instance used
-            by :func:`numpy.random`.
+            by `np.random`.
+        Returns
+        -------
+        None.
 
         """
         # convert adata,adj into networkx
-        logger.info("Converting adjacency matrix to networkx graph...")
+        print("adj to networkx graph .... ")
         if (adj - adj.T).sum() != 0:
             ValueError("louvain use no direction graph, but the input is not")
-        g = nx.from_numpy_array(adj)
-        logger.info("Conversion done. Start fitting...")
-        self.dendo = generate_dendrogram(g, partition, weight, self.resolution, randomize, random_state)
-        logger.info("Fitting done.")
+        g = nx.from_numpy_matrix(adj)
+        print("convert over")
+        print("start fit ... ")
+        self.dendo = generate_dendrogram(g, partition, weight, resolution, randomize, random_state)
 
-    def predict(self, x=None):
-        """Prediction function.
+        print("fit over ")
 
+    def predict(self):
+        """prediction function.
         Parameters
         ----------
-        x
-            Not used. For compatibility with :func:`dance.modules.base.BaseMethod.fit_score`,  which calls :meth:`fit`
-            with ``x``.
+
+        Returns
+        -------
+        self.predict_result :
+            predicted label.
 
         """
-        pred_dict = partition_at_level(self.dendo, len(self.dendo) - 1)
-        pred = np.array(list(map(pred_dict.get, sorted(pred_dict))))
-        return pred
+        self.predict_result = partition_at_level(self.dendo, len(self.dendo) - 1)
+        self.y_pred = self.predict_result
+        return self.predict_result
+
+    def score(self, y_true):
+        """score function to get score of prediction.
+        Parameters
+        ----------
+        y_true :
+            ground truth label.
+
+        Returns
+        -------
+        score : float
+            metric eval score.
+
+        """
+        pred_val = []
+        for key in self.y_pred:
+            pred_val.append(self.y_pred[key])
+
+        from sklearn.metrics.cluster import adjusted_rand_score
+        score = adjusted_rand_score(y_true, np.array(pred_val))
+        print("ARI {}".format(adjusted_rand_score(y_true, np.array(pred_val))))
+        return score
+
+
+# add by us
+
 
+def generate_dendrogram(graph, part_init=None, weight='weight', resolution=1., randomize=None, random_state=None):
 
-def generate_dendrogram(graph, part_init=None, weight="weight", resolution=1., randomize=None, random_state=None):
     if graph.is_directed():
         raise TypeError("Bad graph type, use only non directed graph")
 
     # Properly handle random state, eventually remove old `randomize` parameter
     # NOTE: when `randomize` is removed, delete code up to random_state = ...
     if randomize is not None:
         warnings.warn("The `randomize` parameter will be deprecated in future "
                       "versions. Use `random_state` instead.", DeprecationWarning)
-        # If shouldn't randomize, we set a fixed seed to get deterministic results
+        # If shouldn't randomize, we set a fixed seed to get determinisitc results
         if randomize is False:
             random_state = 0
 
     # We don't know what to do if both `randomize` and `random_state` are defined
     if randomize and random_state is not None:
         raise ValueError("`randomize` and `random_state` cannot be used at the "
                          "same time")
@@ -429,26 +436,26 @@
             part[node] = i
         return [part]
 
     current_graph = graph.copy()
     status = Status()
     status.init(current_graph, weight, part_init)
     status_list = list()
-    _one_level(current_graph, status, weight, resolution, random_state)
-    new_mod = _modularity(status, resolution)
+    __one_level(current_graph, status, weight, resolution, random_state)
+    new_mod = __modularity(status, resolution)
     partition = __renumber(status.node2com)
     status_list.append(partition)
     mod = new_mod
     current_graph = induced_graph(partition, current_graph, weight)
     status.init(current_graph, weight)
 
     while True:
-        _one_level(current_graph, status, weight, resolution, random_state)
-        new_mod = _modularity(status, resolution)
-        if new_mod - mod < MIN:
+        __one_level(current_graph, status, weight, resolution, random_state)
+        new_mod = __modularity(status, resolution)
+        if new_mod - mod < __MIN:
             break
         partition = __renumber(status.node2com)
         status_list.append(partition)
         mod = new_mod
         current_graph = induced_graph(partition, current_graph, weight)
         status.init(current_graph, weight)
     return status_list[:]
@@ -464,15 +471,15 @@
     ----------
     partition : dict
        a dictionary where keys are graph nodes and  values the part the node
        belongs to
     graph : networkx.Graph
         the initial graph
     weight : str, optional
-        the key in graph to use as weight. Default to "weight"
+        the key in graph to use as weight. Default to 'weight'
 
 
     Returns
     -------
     g : networkx.Graph
        a networkx graph where nodes are the parts
 
@@ -489,16 +496,16 @@
     >>> nx.is_isomorphic(ind, goal)
     True
 
     """
     ret = nx.Graph()
     ret.add_nodes_from(partition.values())
 
-    for node1, node2, data in graph.edges(data=True):
-        edge_weight = data.get(weight, 1)
+    for node1, node2, datas in graph.edges(data=True):
+        edge_weight = datas.get(weight, 1)
         com1 = partition[node1]
         com2 = partition[node2]
         w_prec = ret.get_edge_data(com1, com2, {weight: 0}).get(weight, 1)
         ret.add_edge(com1, com2, **{weight: w_prec + edge_weight})
 
     return ret
 
@@ -544,87 +551,87 @@
         neighbors = links[prec_deg:last_deg]
         graph.add_edges_from([(index, int(neigh)) for neigh in neighbors])
         prec_deg = last_deg
 
     return graph
 
 
-def _one_level(graph, status, weight_key, resolution, random_state):
+def __one_level(graph, status, weight_key, resolution, random_state):
     """Compute one level of communities."""
     modified = True
     nb_pass_done = 0
-    cur_mod = _modularity(status, resolution)
+    cur_mod = __modularity(status, resolution)
     new_mod = cur_mod
 
-    while modified and nb_pass_done != PASS_MAX:
+    while modified and nb_pass_done != __PASS_MAX:
         cur_mod = new_mod
         modified = False
         nb_pass_done += 1
 
-        for node in _randomize(graph.nodes(), random_state):
+        for node in __randomize(graph.nodes(), random_state):
             com_node = status.node2com[node]
             degc_totw = status.gdegrees.get(node, 0.) / (status.total_weight * 2.)  # NOQA
-            neigh_communities = _neighcom(node, graph, status, weight_key)
-            remove_cost = - neigh_communities.get(com_node, 0) + \
+            neigh_communities = __neighcom(node, graph, status, weight_key)
+            remove_cost = - neigh_communities.get(com_node,0) + \
                 resolution * (status.degrees.get(com_node, 0.) - status.gdegrees.get(node, 0.)) * degc_totw
-            _remove(node, com_node, neigh_communities.get(com_node, 0.), status)
+            __remove(node, com_node, neigh_communities.get(com_node, 0.), status)
             best_com = com_node
             best_increase = 0
-            for com, dnc in _randomize(neigh_communities.items(), random_state):
+            for com, dnc in __randomize(neigh_communities.items(), random_state):
                 incr = remove_cost + dnc - \
                        resolution * status.degrees.get(com, 0.) * degc_totw
                 if incr > best_increase:
                     best_increase = incr
                     best_com = com
-            _insert(node, best_com, neigh_communities.get(best_com, 0.), status)
+            __insert(node, best_com, neigh_communities.get(best_com, 0.), status)
             if best_com != com_node:
                 modified = True
-        new_mod = _modularity(status, resolution)
-        if new_mod - cur_mod < MIN:
+        new_mod = __modularity(status, resolution)
+        if new_mod - cur_mod < __MIN:
             break
 
 
-def _neighcom(node, graph, status, weight_key):
+def __neighcom(node, graph, status, weight_key):
     """Compute the communities in the neighborhood of node in the graph given with the
     decomposition node2com."""
     weights = {}
-    for neighbor, data in graph[node].items():
+    for neighbor, datas in graph[node].items():
         if neighbor != node:
-            edge_weight = data.get(weight_key, 1)
+            edge_weight = datas.get(weight_key, 1)
             neighborcom = status.node2com[neighbor]
             weights[neighborcom] = weights.get(neighborcom, 0) + edge_weight
 
     return weights
 
 
-def _remove(node, com, weight, status):
+def __remove(node, com, weight, status):
     """Remove node from community com and modify status."""
     status.degrees[com] = (status.degrees.get(com, 0.) - status.gdegrees.get(node, 0.))
     status.internals[com] = float(status.internals.get(com, 0.) - weight - status.loops.get(node, 0.))
     status.node2com[node] = -1
 
 
-def _insert(node, com, weight, status):
+def __insert(node, com, weight, status):
     """Insert node into community and modify status."""
     status.node2com[node] = com
     status.degrees[com] = (status.degrees.get(com, 0.) + status.gdegrees.get(node, 0.))
     status.internals[com] = float(status.internals.get(com, 0.) + weight + status.loops.get(node, 0.))
 
 
-def _modularity(status, resolution):
+def __modularity(status, resolution):
     """Fast compute the modularity of the partition of the graph using status
     precomputed."""
     links = float(status.total_weight)
     result = 0.
     for community in set(status.node2com.values()):
         in_degree = status.internals.get(community, 0.)
         degree = status.degrees.get(community, 0.)
         if links > 0:
             result += in_degree * resolution / links - ((degree / (2. * links))**2)
     return result
 
 
-def _randomize(items, random_state):
+def __randomize(items, random_state):
     """Returns a List containing a random permutation of items."""
     randomized_items = list(items)
     random_state.shuffle(randomized_items)
     return randomized_items
```

### Comparing `pydance-1.0.0/dance/modules/spatial/spatial_domain/spagcn.py` & `pydance-1.0.0rc0/dance/utils/loss.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,670 +1,843 @@
-"""Reimplementation of SpaGCN.
+# Copyright 2022 DSE lab.  All rights reserved.
 
-Extended from https://github.com/jianhuupenn/SpaGCN
+import math
+from typing import *
 
-Reference
-----------
-Hu, Jian, et al. "SpaGCN: Integrating gene expression, spatial location and histology to identify spatial domains and
-spatially variable genes by graph convolutional network." Nature methods 18.11 (2021): 1342-1351.
-
-"""
 import numpy as np
-import pandas as pd
-import scanpy as sc
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-import torch.optim as optim
-from sklearn.cluster import KMeans
-from torch.nn.parameter import Parameter
-
-from dance import logger
-from dance.modules.base import BaseClusteringMethod
-from dance.transforms import AnnDataTransform, CellPCA, Compose, FilterGenesMatch, SetConfig
-from dance.transforms.graph import SpaGCNGraph, SpaGCNGraph2D
-from dance.typing import LogLevel
-
-
-def calculate_p(adj, l):
-    adj_exp = np.exp(-1 * (adj**2) / (2 * (l**2)))
-    return np.mean(np.sum(adj_exp, 1)) - 1
-
-
-def search_l(p, adj, start=0.01, end=1000, tol=0.01, max_run=100):
-    run = 0
-    p_low = calculate_p(adj, start)
-    p_high = calculate_p(adj, end)
-    if p_low > p + tol:
-        logger.info("l not found, try smaller start point.")
-        return None
-    elif p_high < p - tol:
-        logger.info("l not found, try bigger end point.")
-        return None
-    elif np.abs(p_low - p) <= tol:
-        logger.info(f"recommended l: {start}")
-        return start
-    elif np.abs(p_high - p) <= tol:
-        logger.info(f"recommended l: {end}")
-        return end
-    while (p_low + tol) < p < (p_high - tol):
-        run += 1
-        logger.info(f"Run {run}: l [{start}, {end}], p [{p_low}, {p_high}]")
-        if run > max_run:
-            logger.info(f"Exact l not found, closest values are:\nl={start}: p={p_low}\nl={end}: p={p_high}")
-            return None
-        mid = (start + end) / 2
-        p_mid = calculate_p(adj, mid)
-        if np.abs(p_mid - p) <= tol:
-            logger.info(f"recommended l: {mid}")
-            return mid
-        if p_mid <= p:
-            start = mid
-            p_low = p_mid
-        else:
-            end = mid
-            p_high = p_mid
-    return None
-
-
-def refine(sample_id, pred, dis, shape="hexagon"):
-    """An optional refinement step for the clustering result. In this step, SpaGCN
-    examines the domain assignment of each spot and its surrounding spots. For a given
-    spot, if more than half of its surrounding spots are assigned to a different domain,
-    this spot will be relabeled to the same domain as the major label of its surrounding
-    spots.
-
-    Parameters
-    ----------
-    sample_id
-        Sample id.
-    pred
-        Initial prediction.
-    dis
-        Graph structure.
-    shape : str
-        Shape parameter.
-
-    Returns
-    -------
-    refined_pred
-        Refined predictions.
-
-    """
-    refined_pred = []
-    pred = pd.DataFrame({"pred": pred}, index=sample_id)
-    dis_df = pd.DataFrame(dis, index=sample_id, columns=sample_id)
-    if shape == "hexagon":
-        num_nbs = 6
-    elif shape == "square":
-        num_nbs = 4
-    else:
-        logger.info("Shape not recognized, shape='hexagon' for Visium data, 'square' for ST data.")
-    for i in range(len(sample_id)):
-        index = sample_id[i]
-        dis_tmp = dis_df.loc[index, :].sort_values()
-        nbs = dis_tmp[0:num_nbs + 1]
-        nbs_pred = pred.loc[nbs.index, "pred"]
-        self_pred = pred.loc[index, "pred"]
-        v_c = nbs_pred.value_counts()
-        if (v_c.loc[self_pred] < num_nbs / 2) and (np.max(v_c) > num_nbs / 2):
-            refined_pred.append(v_c.idxmax())
-        else:
-            refined_pred.append(self_pred)
-    return refined_pred
 
 
-class GraphConvolution(nn.Module):
-    """Simple GCN layer, similar to https://arxiv.org/abs/1609.02907."""
+def kld_loss(p, q):
+
+    def kld(target, pred):
+        return torch.mean(torch.sum(target * torch.log(target / (pred + 1e-6)), dim=1))
+
+    loss = kld(p, q)
+    return loss
+
+
+###############################################
+##    Created by BABEL
+###############################################
+class BCELoss(nn.BCELoss):
+    """Custom BCE loss that can correctly ignore the encoded latent space output."""
+
+    def forward(self, x, target):
+        input = x[0]
+        return F.binary_cross_entropy(input, target, weight=self.weight, reduction=self.reduction)
+
+
+class MSELoss(nn.MSELoss):
+    """Custom MSE loss that can correctly ignore the encoded latent space output."""
 
-    def __init__(self, in_features, out_features, bias=True):
+    def forward(self, x: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
+        return F.mse_loss(x[0], target, reduction=self.reduction)
+
+
+class RMSELoss(nn.MSELoss):
+    """Custom RMSE loss that can correctly ignore the encoded latent space output."""
+
+    def forward(self, x: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
+        return torch.sqrt(F.mse_loss(x[0], target, reduction=self.reduction))
+
+
+class DistanceProbLoss(nn.Module):
+    """Analog of above log prob loss, but using distances May be useful for aligning
+    latent spaces."""
+
+    def __init__(self, weight: float = 5.0, norm: int = 1):
         super().__init__()
-        self.in_features = in_features
-        self.out_features = out_features
-        self.weight = Parameter(torch.FloatTensor(in_features, out_features))
-        if bias:
-            self.bias = Parameter(torch.FloatTensor(out_features))
-        else:
-            self.register_parameter("bias", None)
-        self.reset_parameters()
+        assert weight > 0
+        self.weight = weight
+        self.norm = norm
+
+    def forward(self, x, target_z):
+        z, logp = x[:2]
+        d = F.pairwise_distance(
+            z,
+            target_z,
+            p=self.norm,
+            eps=1e-6,
+            keepdim=False,  # Default value
+        )
+        if len(d.shape) == 2:
+            d = torch.mean(d, dim=1)  # Drop 1 dimension
+        per_ex = self.weight * d - logp
+        retval = torch.mean(per_ex)
+        if retval != retval:
+            raise ValueError("NaN")
+        return retval
+        return torch.mean(d)
 
-    def reset_parameters(self):
-        stdv = 1. / np.sqrt(self.weight.size(1))
-        self.weight.data.uniform_(-stdv, stdv)
-        if self.bias is not None:
-            self.bias.data.uniform_(-stdv, stdv)
-
-    def forward(self, input, adj):
-        support = torch.mm(input, self.weight)
-        output = torch.spmm(adj, support)
-        if self.bias is not None:
-            return output + self.bias
-        else:
-            return output
 
-    def __repr__(self):
-        return f"{self.__class__.__name__}({self.in_features} -> {self.out_features})"
+class NegativeBinomialLoss(nn.Module):
+    """Negative binomial loss.
 
+    Preds should be a tuple of (mean, dispersion)
 
-class SimpleGCDEC(nn.Module):
-    """Basic model used in SpaGCN training.
+    """
+
+    def __init__(
+        self,
+        scale_factor: float = 1.0,
+        eps: float = 1e-10,
+        l1_lambda: float = 0.0,
+        mean: bool = True,
+    ):
+        super().__init__()
+        self.loss = negative_binom_loss(
+            scale_factor=scale_factor,
+            eps=eps,
+            mean=mean,
+            debug=True,
+        )
+        self.l1_lambda = l1_lambda
+
+    def forward(self, preds, target):
+        preds, theta = preds[:2]
+        l = self.loss(
+            preds=preds,
+            theta=theta,
+            truth=target,
+        )
+        encoded = preds[:-1]
+        l += self.l1_lambda * torch.abs(encoded).sum()
+        return l
+
+
+class ZeroInflatedNegativeBinomialLoss(nn.Module):
+    """ZINB loss.
 
-    Parameters
-    ----------
-    nfeat : int
-        Input feature dimension.
-    nhid : int
-        Output feature dimension.
-    alpha : float optional
-        Alphat parameter.
+    Preds should be a tuple of (mean, dispersion, dropout) General
+    notes: total variation seems to do poorly (at least for atacseq)
 
     """
 
-    def __init__(self, nfeat, nhid, alpha=0.2, device="cpu"):
+    def __init__(
+        self,
+        ridge_lambda: float = 0.0,
+        tv_lambda: float = 0.0,
+        l1_lambda: float = 0.0,
+        eps: float = 1e-10,
+        scale_factor: float = 1.0,
+        debug: bool = True,
+    ):
         super().__init__()
-        self.gc = GraphConvolution(nfeat, nhid)
-        self.nhid = nhid
-        # self.mu is determined by the init method
-        self.alpha = alpha
-        self.device = device
+        self.loss = zero_inflated_negative_binom_loss(
+            ridge_lambda=ridge_lambda,
+            tv_lambda=tv_lambda,
+            eps=eps,
+            scale_factor=scale_factor,
+            debug=debug,
+        )
+        self.l1_lambda = l1_lambda
+
+    def forward(self, preds, target):
+        preds, theta, pi = preds[:3]
+        l = self.loss(
+            preds=preds,
+            theta_disp=theta,
+            pi_dropout=pi,
+            truth=target,
+        )
+        encoded = preds[:-1]
+        l += self.l1_lambda * torch.abs(encoded).sum()
+        return l
+
 
-    def forward(self, x, adj):
-        """Forward function."""
-        x = self.gc(x, adj)
-        q = 1.0 / ((1.0 + torch.sum((x.unsqueeze(1) - self.mu)**2, dim=2) / self.alpha) + 1e-8)
-        q = q**(self.alpha + 1.0) / 2.0
-        q = q / torch.sum(q, dim=1, keepdim=True)
-        return x, q
+class PairedLoss(nn.Module):
+    """Paired loss function.
 
-    def loss_function(self, p, q):
-        """Objective function as a Kullback–Leibler (KL) divergence loss."""
+    Automatically unpacks and encourages the encoded representation to
+    be similar using a given distance function. link_strength parameter
+    controls how strongly we encourage this loss2_weight controls how
+    strongly we weight the second loss, relative to the first A value of
+    1.0 indicates that they receive equal weight, and a value larger
+    indicates that the second loss receives greater weight. link_func
+    should be a callable that takes in the two encoded representations
+    and outputs a metric where a larger value indicates greater
+    divergence
 
-        def kld(target, pred):
-            return torch.mean(torch.sum(target * torch.log(target / (pred + 1e-6)), dim=1))
+    """
+
+    def __init__(
+            self,
+            loss1=NegativeBinomialLoss,
+            loss2=ZeroInflatedNegativeBinomialLoss,
+            link_func=lambda x, y: (x - y).abs().mean(),
+            link_strength=1e-3,
+    ):
+        super().__init__()
+        self.loss1 = loss1()
+        self.loss2 = loss2()
+        self.link = link_strength
+        self.link_f = link_func
+
+        self.warmup = SigmoidWarmup(
+            midpoint=1000,
+            maximum=link_strength,
+        )
 
-        loss = kld(p, q)
+    def forward(self, preds, target):
+        """Unpack and feed to each loss, averaging at end."""
+        preds1, preds2 = preds
+        target1, target2 = target
+
+        loss1 = self.loss1(preds1, target1)
+        loss2 = self.loss2(preds2, target2)
+        retval = loss1 + loss2
+
+        # Align the encoded representation assuming the last output is encoded representation
+        encoded1 = preds1[-1]
+        encoded2 = preds2[-1]
+        if self.link > 0:
+            l = next(self.warmup)
+            if l > 1e-6:
+                d = self.link_f(encoded1, encoded2).mean()
+                retval += l * d
+
+        return retval
+
+
+class PairedLossInvertible(nn.Module):
+    """Paired loss function with additional invertible (RealNVP) layer loss Loss 1 is
+    for the first autoencoder Loss 2 is for the second autoencoder Loss 3 is for the
+    invertible network at bottleneck."""
+
+    def __init__(
+            self,
+            loss1=NegativeBinomialLoss,
+            loss2=ZeroInflatedNegativeBinomialLoss,
+            loss3=DistanceProbLoss,
+            link_func=lambda x, y: (x - y).abs().mean(),
+            link_strength=1e-3,
+            inv_strength=1.0,
+    ):
+        super().__init__()
+        self.loss1 = loss1()
+        self.loss2 = loss2()
+        self.loss3 = loss3()
+        self.link = link_strength
+        self.link_f = link_func
+
+        # self.link_warmup = layers.SigmoidWarmup(
+        #     midpoint=1000,
+        #     maximum=link_strength,
+        # )
+        self.link_warmup = DelayedLinearWarmup(
+            delay=1000,
+            inc=5e-3,
+            t_max=link_strength,
+        )
+
+        self.inv_warmup = DelayedLinearWarmup(
+            delay=2000,
+            inc=5e-3,
+            t_max=inv_strength,
+        )
+
+    def forward(self, preds, target):
+        """Unpack and feed to each loss."""
+        # Both enc1_pred and enc2_pred are tuples of 2 values
+        preds1, preds2, (enc1_pred, enc2_pred) = preds
+        target1, target2 = target
+
+        loss1 = self.loss1(preds1, target1)
+        loss2 = self.loss2(preds2, target2)
+        retval = loss1 + loss2
+
+        # Align the encoded representations
+        encoded1 = preds1[-1]
+        encoded2 = preds2[-1]
+        if self.link > 0:
+            l = next(self.link_warmup)
+            if l > 1e-6:
+                d = self.link_f(encoded1, encoded2).mean()
+                retval += l * d
+
+        # Add a term for invertible network
+        inv_loss1 = self.loss3(enc1_pred, enc2_pred[0])
+        inv_loss2 = self.loss3(enc2_pred, enc1_pred[0])
+        retval += next(self.inv_warmup) * (inv_loss1 + inv_loss2)
+
+        return retval
+
+
+class QuadLoss(PairedLoss):
+    """Paired loss, but for the spliced autoencoder with 4 outputs."""
+
+    def __init__(
+        self,
+        loss1=NegativeBinomialLoss,
+        loss2=BCELoss,
+        loss2_weight: float = 3.0,
+        cross_weight: float = 1.0,
+        cross_warmup_delay: int = 0,
+        link_strength: float = 0.0,
+        link_func: Callable = lambda x, y: (x - y).abs().mean(),
+        link_warmup_delay: int = 0,
+        record_history: bool = False,
+    ):
+        super().__init__()
+        self.loss1 = loss1()
+        self.loss2 = loss2()
+        self.loss2_weight = loss2_weight
+        self.history = []  # Eventually contains list of tuples per call
+        self.record_history = record_history
+
+        if link_warmup_delay:
+            self.warmup = SigmoidWarmup(
+                midpoint=link_warmup_delay,
+                maximum=link_strength,
+            )
+            # self.warmup = layers.DelayedLinearWarmup(
+            #     delay=warmup_delay,
+            #     t_max=link_strength,
+            #     inc=1e-3,
+            # )
+        else:
+            self.warmup = NullWarmup(t_max=link_strength)
+        if cross_warmup_delay:
+            self.cross_warmup = SigmoidWarmup(
+                midpoint=cross_warmup_delay,
+                maximum=cross_weight,
+            )
+        else:
+            self.cross_warmup = NullWarmup(t_max=cross_weight)
+
+        self.link_strength = link_strength
+        self.link_func = link_func
+
+    def get_component_losses(self, preds, target):
+        """Return the four losses that go into the overall loss, without scaling."""
+        preds11, preds12, preds21, preds22 = preds
+        if not isinstance(target, (list, tuple)):
+            # Try to unpack into the correct parts
+            target = torch.split(target, [preds11[0].shape[-1], preds22[0].shape[-1]], dim=-1)
+        target1, target2 = target  # Both are torch tensors
+
+        loss11 = self.loss1(preds11, target1)
+        loss21 = self.loss1(preds21, target1)
+        loss12 = self.loss2(preds12, target2)
+        loss22 = self.loss2(preds22, target2)
+
+        return loss11, loss21, loss12, loss22
+
+    def forward(self, preds, target):
+        loss11, loss21, loss12, loss22 = self.get_component_losses(preds, target)
+        if self.record_history:
+            detensor = lambda x: x.detach().cpu().numpy().item()
+            self.history.append([detensor(l) for l in (loss11, loss21, loss12, loss22)])
+
+        loss = loss11 + self.loss2_weight * loss22
+        loss += next(self.cross_warmup) * (loss21 + self.loss2_weight * loss12)
+
+        if self.link_strength > 0:
+            l = next(self.warmup)
+            if l > 1e-6:  # If too small we disregard
+                preds11, preds12, preds21, preds22 = preds
+                encoded1 = preds11[-1]  # Could be preds12
+                encoded2 = preds22[-1]  # Could be preds21
+                d = self.link_func(encoded1, encoded2)
+                loss += self.link_strength * d
         return loss
 
-    def target_distribution(self, q):
-        """Generate an auxiliary target distribution based on q the probability of
-        assigning cell i to cluster j.
 
-        Parameters
-        ----------
-        q
-            The probability of assigning cell i to cluster j.
+def scvi_log_nb_positive(x, mu, theta, eps=1e-8):
+    """
+    Taken from scVI log_likelihood.py - scVI invocation is:
+    reconst_loss = -log_nb_positive(x, px_rate, px_r).sum(dim=-1)
+    scVI decoder outputs px_scale, px_r, px_rate, px_dropout
+    px_scale is subject to Softmax
+    px_r is just a Linear layer
+    px_rate = torch.exp(library) * px_scale
+    mu = mean of NB
+    theta = indverse dispersion parameter
+    Here, x appears to correspond to y_true in the below negative_binom_loss (aka the observed counts)
+    """
+    # if theta.ndimension() == 1:
+    #     theta = theta.view(
+    #         1, theta.size(0)
+    #     )  # In this case, we reshape theta for broadcasting
+
+    log_theta_mu_eps = torch.log(theta + mu + eps)
+    res = (
+        theta * (torch.log(theta + eps) - log_theta_mu_eps) + x * (torch.log(mu + eps) - log_theta_mu_eps) +
+        torch.lgamma(x + theta) - torch.lgamma(theta)  # Present (in negative) for DCA
+        - torch.lgamma(x + 1))
+
+    return res.mean()
+
+
+def scvi_log_zinb_positive(x, mu, theta, pi, eps=1e-8):
+    """https://github.com/YosefLab/scVI/blob/6c9f43e3332e728831b174c1c1f0c9127b
+    77cba0/scvi/models/log_likelihood.py#L206."""
+    # theta is the dispersion rate. If .ndimension() == 1, it is shared for all cells (regardless of batch or labels)
+    if theta.ndimension() == 1:
+        theta = theta.view(1, theta.size(0))  # In this case, we reshape theta for broadcasting
+
+    softplus_pi = F.softplus(-pi)
+    log_theta_eps = torch.log(theta + eps)
+    log_theta_mu_eps = torch.log(theta + mu + eps)
+    pi_theta_log = -pi + theta * (log_theta_eps - log_theta_mu_eps)
+
+    case_zero = F.softplus(pi_theta_log) - softplus_pi
+    mul_case_zero = torch.mul((x < eps).type(torch.float32), case_zero)
+
+    case_non_zero = (
+        -softplus_pi + pi_theta_log + x * (torch.log(mu + eps) - log_theta_mu_eps)  # Found above
+        + torch.lgamma(x + theta)  # Found above
+        - torch.lgamma(theta)  # Found above
+        - torch.lgamma(x + 1)  # Found above
+    )
+    mul_case_non_zero = torch.mul((x > eps).type(torch.float32), case_non_zero)
+
+    res = mul_case_zero + mul_case_non_zero
+
+    return res.mean()
+
+
+def negative_binom_loss(
+    scale_factor: float = 1.0,
+    eps: float = 1e-10,
+    mean: bool = True,
+    debug: bool = False,
+) -> Callable:
+    """Return a function that calculates the binomial loss
+    https://github.com/theislab/dca/blob/master/dca/loss.py combination of the Poisson
+    distribution and a gamma distribution is a negative binomial distribution."""
+
+    def loss(preds, theta, truth):
+        """Calculates negative binomial loss as defined in the NB class in link
+        above."""
+        y_true = truth
+        y_pred = preds * scale_factor
+
+        if debug:  # Sanity check before loss calculation
+            assert not torch.isnan(y_pred).any(), y_pred
+            assert not torch.isinf(y_pred).any(), y_pred
+            assert not (y_pred < 0).any()  # should be non-negative
+            assert not (theta < 0).any()
+
+        # Clip theta values
+        theta = torch.clamp(theta, max=1e6)
+
+        t1 = (torch.lgamma(theta + eps) + torch.lgamma(y_true + 1.0) - torch.lgamma(y_true + theta + eps))
+        t2 = (theta + y_true) * torch.log1p(y_pred /
+                                            (theta + eps)) + (y_true *
+                                                              (torch.log(theta + eps) - torch.log(y_pred + eps)))
+        if debug:  # Sanity check after calculating loss
+            assert not torch.isnan(t1).any(), t1
+            assert not torch.isinf(t1).any(), (t1, torch.sum(torch.isinf(t1)))
+            assert not torch.isnan(t2).any(), t2
+            assert not torch.isinf(t2).any(), t2
+
+        retval = t1 + t2
+        if debug:
+            assert not torch.isnan(retval).any(), retval
+            assert not torch.isinf(retval).any(), retval
+
+        return torch.mean(retval) if mean else retval
+
+    return loss
+
+
+def zero_inflated_negative_binom_loss(
+    ridge_lambda: float = 0.0,
+    tv_lambda: float = 0.0,
+    eps: float = 1e-10,
+    scale_factor: float = 1.0,
+    debug: bool = False,
+):
+    """Return a function that calculates ZINB loss
+    https://github.com/theislab/dca/blob/master/dca/loss.py."""
+    nb_loss_func = negative_binom_loss(mean=False, eps=eps, scale_factor=scale_factor, debug=debug)
+
+    def loss(preds, theta_disp, pi_dropout, truth):
+        if debug:
+            assert not (pi_dropout > 1.0).any()
+            assert not (pi_dropout < 0.0).any()
+        nb_case = nb_loss_func(preds, theta_disp, truth) - torch.log(1.0 - pi_dropout + eps)
+
+        y_true = truth
+        y_pred = preds * scale_factor
+        theta = torch.clamp(theta_disp, max=1e6)
+
+        zero_nb = torch.pow(theta / (theta + y_pred + eps), theta)
+        zero_case = -torch.log(pi_dropout + ((1.0 - pi_dropout) * zero_nb) + eps)
+        result = torch.where(y_true < 1e-8, zero_case, nb_case)
+
+        # Ridge regularization on pi dropout term
+        ridge = ridge_lambda * torch.pow(pi_dropout, 2)
+        result += ridge
+
+        # Total variation regularization on pi dropout term
+        tv = tv_lambda * total_variation(pi_dropout)
+        result += tv
+
+        retval = torch.mean(result)
+        # if debug:
+        #     assert retval.item() > 0
+        return retval
+
+    return loss
+
+
+def total_variation(x):
+    """Given a 2D input (where one dimension is a batch dimension, the actual values are
+    one dimensional) compute the total variation (within a 1 position shift)"""
+    t = torch.sum(torch.abs(x[:, :-1] - x[:, 1:]))
+    return t
 
-        Returns
-        -------
-        p
-            Target distribution.
 
-        """
-        p = q**2 / torch.sum(q, dim=0)
-        p = p / torch.sum(p, dim=1, keepdim=True)
-        return p
-
-    def fit(self, X, adj, lr=0.001, epochs=5000, update_interval=3, trajectory_interval=50, weight_decay=5e-4,
-            opt="sgd", init="louvain", n_neighbors=10, res=0.4, n_clusters=10, init_spa=True, tol=1e-3):
-        """Fit function for model training.
+class Warmup:  # Doesn't have to be nn.Module because it's not learned
+    """Warmup layer similar to.
 
-        Parameters
-        ----------
-        X
-            Node features.
-        adj
-            Adjacent matrix.
-        lr : float
-            Learning rate.
-        epochs : int
-            Maximum number of epochs.
-        update_interval : int
-            Interval for update.
-        trajectory_interval: int
-            Trajectory interval.
-        weight_decay : float
-            Weight decay.
-        opt : str
-            Optimizer.
-        init : str
-            "louvain" or "kmeans".
-        n_neighbors : int
-            The number of neighbors used in louvain.
-        res : float
-            Used for louvain.
-        n_clusters : int
-            The number of clusters usedd in kmeans.
-        init_spa : bool
-            Initialize spatial.
-        tol : float
-            Tolerant value for searching l.
+    Sonderby 2016 - Linear deterministic warm-up
 
-        """
-        self.trajectory = []
-        if opt == "sgd":
-            optimizer = optim.SGD(self.parameters(), lr=lr, momentum=0.9)
-        elif opt == "admin":
-            optimizer = optim.Adam(self.parameters(), lr=lr, weight_decay=weight_decay)
-
-        features = self.gc(torch.FloatTensor(X), torch.FloatTensor(adj))
-        # ---------------------------------------------------------------------
-        if init == "kmeans":
-            logger.info("Initializing cluster centers with kmeans, n_clusters known")
-            self.n_clusters = n_clusters
-            kmeans = KMeans(self.n_clusters, n_init=20)
-            if init_spa:
-                # Kmeans using both expression and spatial information
-                y_pred = kmeans.fit_predict(features.detach().numpy())
-            else:
-                # Kmeans using only expression information
-                y_pred = kmeans.fit_predict(X)  # use X as numpy
-        elif init == "louvain":
-            logger.info(f"Initializing cluster centers with louvain, resolution = {res}")
-            if init_spa:
-                adata = sc.AnnData(features.detach().numpy())
-            else:
-                adata = sc.AnnData(X)
-            sc.pp.neighbors(adata, n_neighbors=n_neighbors)
-            # sc.tl.louvain(adata,resolution=res)
-            sc.tl.leiden(adata, resolution=res, key_added="louvain")
-
-            y_pred = adata.obs["louvain"].astype(int).to_numpy()
-            self.n_clusters = len(np.unique(y_pred))
-        # ---------------------------------------------------------------------
-        y_pred_last = y_pred
-        self.mu = Parameter(torch.Tensor(self.n_clusters, self.nhid))
-        X = torch.FloatTensor(X)
-        adj = torch.FloatTensor(adj)
-        self.trajectory.append(y_pred)
-        features = pd.DataFrame(features.detach().numpy(), index=np.arange(0, features.shape[0]))
-        Group = pd.Series(y_pred, index=np.arange(0, features.shape[0]), name="Group")
-        Mergefeature = pd.concat([features, Group], axis=1)
-        cluster_centers = np.asarray(Mergefeature.groupby("Group").mean())
-        self.mu.data.copy_(torch.Tensor(cluster_centers))
-
-        # Copy data and model in cuda
-        device = self.device
-        self = self.to(device)
-        X = X.to(device)
-        adj = adj.to(device)
-
-        self.train()
-        for epoch in range(epochs):
-            if epoch % update_interval == 0:
-                _, q = self.forward(X, adj)
-                p = self.target_distribution(q).data
-            if epoch % 10 == 0:
-                logger.info(f"Epoch {epoch}")
-            optimizer.zero_grad()
-            z, q = self(X, adj)
-            loss = self.loss_function(p, q)
-            loss.backward()
-            optimizer.step()
-            if epoch % trajectory_interval == 0:
-                self.trajectory.append(torch.argmax(q, dim=1).data.cpu().numpy())
-
-            # Check stop criterion
-            y_pred = torch.argmax(q, dim=1).data.detach().cpu().numpy()
-            delta_label = np.sum(y_pred != y_pred_last).astype(np.float32) / X.shape[0]
-            y_pred_last = y_pred
-            if epoch > 0 and (epoch - 1) % update_interval == 0 and delta_label < tol:
-                logger.info(f"delta_label {delta_label} < tol {tol}")
-                logger.info("Reach tolerance threshold. Stopping training.")
-                logger.info(f"Total epoch: {epoch}")
-                break
-
-        # Recover model and data in cpu
-        self = self.cpu()
-        X = X.cpu()
-        adj = adj.cpu()
-
-    def fit_with_init(self, X, adj, init_y, lr=0.001, epochs=5000, update_interval=1, weight_decay=5e-4, opt="sgd"):
-        """Initializing cluster centers with kmeans."""
-        logger.info("Initializing cluster centers with kmeans.")
-        if opt == "sgd":
-            optimizer = optim.SGD(self.parameters(), lr=lr, momentum=0.9)
-        elif opt == "admin":
-            optimizer = optim.Adam(self.parameters(), lr=lr, weight_decay=weight_decay)
-        X = torch.FloatTensor(X)
-        adj = torch.FloatTensor(adj)
-        features, _ = self.forward(X, adj)
-        features = pd.DataFrame(features.detach().numpy(), index=np.arange(0, features.shape[0]))
-        Group = pd.Series(init_y, index=np.arange(0, features.shape[0]), name="Group")
-        Mergefeature = pd.concat([features, Group], axis=1)
-        cluster_centers = np.asarray(Mergefeature.groupby("Group").mean())
-        self.mu.data.copy_(torch.Tensor(cluster_centers))
-
-        # Copy data and model in cuda
-        device = self.device
-        self = self.to(device)
-        X = X.to(device)
-        adj = adj.to(device)
-
-        self.train()
-        for epoch in range(epochs):
-            if epoch % update_interval == 0:
-                _, q = self.forward(torch.FloatTensor(X), torch.FloatTensor(adj))
-                p = self.target_distribution(q).data
-            X = torch.FloatTensor(X)
-            adj = torch.FloatTensor(adj)
-            optimizer.zero_grad()
-            z, q = self(X, adj)
-            loss = self.loss_function(p, q)
-            loss.backward()
-            optimizer.step()
-
-        # Recover model and data in cpu
-        self = self.cpu()
-        X = X.cpu()
-        adj = adj.cpu()
-
-    def predict(self, X, adj):
-        """Transform to float tensor."""
-        z, q = self(torch.FloatTensor(X), torch.FloatTensor(adj))
-        return z, q
-
-
-# Not used in SpaGCN
-class GC_DEC(nn.Module):
-
-    def __init__(self, nfeat, nhid1, nhid2, n_clusters=None, dropout=0.5, alpha=0.2):
-        super().__init__()
-
-        self.gc1 = GraphConvolution(nfeat, nhid1)
-        self.gc2 = GraphConvolution(nhid1, nhid2)
-        self.dropout = dropout
-        self.mu = Parameter(torch.Tensor(n_clusters, nhid2))
-        self.n_clusters = n_clusters
-        self.alpha = alpha
-
-    def forward(self, x, adj):
-        x = self.gc1(x, adj)
-        x = F.relu(x)
-        x = F.dropout(x, self.dropout, training=True)
-        x = self.gc2(x, adj)
-        q = 1.0 / ((1.0 + torch.sum((x.unsqueeze(1) - self.mu)**2, dim=2) / self.alpha) + 1e-6)
-        q = q**(self.alpha + 1.0) / 2.0
-        q = q / torch.sum(q, dim=1, keepdim=True)
-        return x, q
+    """
 
-    def loss_function(self, p, q):
+    def __init__(self, inc: float = 5e-3, t_max: float = 1.0):
+        self.t = 0.0
+        self.t_max = t_max
+        self.inc = inc
+        self.counter = 0  # Track number of times called next
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        retval = self.t
+        t_next = self.t + self.inc
+        self.t = min(t_next, self.t_max)
+        self.counter += 1
+        return retval
+
+
+class DelayedLinearWarmup:
+    """"""
+
+    def __init__(self, delay: int = 2000, inc: float = 5e-3, t_max: float = 1.0):
+        self.t = 0.0
+        self.t_max = t_max
+        self.inc = inc
+        self.delay = delay
+        self.counter = 0
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        self.counter += 1
+        retval = self.t
+        if self.counter < self.delay:
+            return retval
+        self.t = min(self.t + self.inc, self.t_max)
+        return retval
+
+
+class SigmoidWarmup:
+    """Sigmoid warmup Midpoints defines the number of iterations before we hit
+    0.5 Scale determines how quickly we hit 1 after this point."""
+
+    def __init__(self, midpoint: int = 500, scale: float = 0.1, maximum: float = 1.0):
+        self.midpoint = midpoint
+        self.scale = scale
+        self.maximum = maximum
+        self.counter = 0
+        self.t = 0.0
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        retval = self.t
+        t_next = 1.0 / (1.0 + np.exp(-self.scale * (self.counter - self.midpoint)))
+        self.t = t_next
+        self.counter += 1
+        return self.maximum * retval
 
-        def kld(target, pred):
-            return torch.mean(torch.sum(target * torch.log(target / (pred + 1e-6)), dim=1))
 
-        loss = kld(p, q)
-        return loss
+class NullWarmup(Warmup):
+    """
+    No warmup - but provides a consistent API
+    """
 
-    def target_distribution(self, q):
-        p = q**2 / torch.sum(q, dim=0)
-        p = p / torch.sum(p, dim=1, keepdim=True)
-        return p
-
-    def fit(self, X, adj, lr=0.001, epochs=10, update_interval=5, weight_decay=5e-4, opt="sgd", init="louvain",
-            n_neighbors=10, res=0.4):
-        self.trajectory = []
-        logger.info("Initializing cluster centers with kmeans.")
-        if opt == "sgd":
-            optimizer = optim.SGD(self.parameters(), lr=lr, momentum=0.9)
-        elif opt == "admin":
-            optimizer = optim.Adam(self.parameters(), lr=lr, weight_decay=weight_decay)
-
-        features, _ = self.forward(torch.FloatTensor(X), torch.FloatTensor(adj))
-        # ---------------------------------------------------------------------
-        if init == "kmeans":
-            # Kmeans using only expression information
-            kmeans = KMeans(self.n_clusters, n_init=20)
-            y_pred = kmeans.fit_predict(features.detach().numpy())
-        elif init == "louvain":
-            # Louvain using only expression information
-            adata = sc.AnnData(features.detach().numpy())
-            sc.pp.neighbors(adata, n_neighbors=n_neighbors)
-            sc.tl.louvain(adata, resolution=res)
-            y_pred = adata.obs["louvain"].astype(int).to_numpy()
-        # ---------------------------------------------------------------------
-        X = torch.FloatTensor(X)
-        adj = torch.FloatTensor(adj)
-        self.trajectory.append(y_pred)
-        features = pd.DataFrame(features.detach().numpy(), index=np.arange(0, features.shape[0]))
-        Group = pd.Series(y_pred, index=np.arange(0, features.shape[0]), name="Group")
-        Mergefeature = pd.concat([features, Group], axis=1)
-        cluster_centers = np.asarray(Mergefeature.groupby("Group").mean())
-
-        self.mu.data.copy_(torch.Tensor(cluster_centers))
-        self.train()
-        for epoch in range(epochs):
-            if epoch % update_interval == 0:
-                _, q = self.forward(X, adj)
-                p = self.target_distribution(q).data
-            if epoch % 100 == 0:
-                logger.info(f"Epoch {epoch}")
-            optimizer.zero_grad()
-            z, q = self(X, adj)
-            loss = self.loss_function(p, q)
-            loss.backward()
-            optimizer.step()
-            self.trajectory.append(torch.argmax(q, dim=1).data.cpu().numpy())
-
-    def fit_with_init(self, X, adj, init_y, lr=0.001, epochs=10, update_interval=1, weight_decay=5e-4, opt="sgd"):
-        logger.info("Initializing cluster centers with kmeans.")
-        if opt == "sgd":
-            optimizer = optim.SGD(self.parameters(), lr=lr, momentum=0.9)
-        elif opt == "admin":
-            optimizer = optim.Adam(self.parameters(), lr=lr, weight_decay=weight_decay)
-        X = torch.FloatTensor(X)
-        adj = torch.FloatTensor(adj)
-        features, _ = self.forward(X, adj)
-        features = pd.DataFrame(features.detach().numpy(), index=np.arange(0, features.shape[0]))
-        Group = pd.Series(init_y, index=np.arange(0, features.shape[0]), name="Group")
-        Mergefeature = pd.concat([features, Group], axis=1)
-        cluster_centers = np.asarray(Mergefeature.groupby("Group").mean())
-        self.mu.data.copy_(torch.Tensor(cluster_centers))
-        self.train()
-        for epoch in range(epochs):
-            if epoch % update_interval == 0:
-                _, q = self.forward(torch.FloatTensor(X), torch.FloatTensor(adj))
-                p = self.target_distribution(q).data
-            X = torch.FloatTensor(X)
-            adj = torch.FloatTensor(adj)
-            optimizer.zero_grad()
-            z, q = self(X, adj)
-            loss = self.loss_function(p, q)
-            loss.backward()
-            optimizer.step()
-
-    def predict(self, X, adj):
-        z, q = self(torch.FloatTensor(X), torch.FloatTensor(adj))
-        return z, q
-
-
-class SpaGCN(BaseClusteringMethod):
-    """SpaGCN class.
-
-    Parameters
-    ----------
-    l : float
-        the parameter to control percentage p
-
-    """
-
-    def __init__(self, l=None):
-        self.l = l
-        self.res = None
-
-    @staticmethod
-    def preprocessing_pipeline(alpha: float = 1, beta: int = 49, dim: int = 50, log_level: LogLevel = "INFO"):
-        return Compose(
-            FilterGenesMatch(prefixes=["ERCC", "MT-"]),
-            AnnDataTransform(sc.pp.normalize_total, target_sum=1e4),
-            AnnDataTransform(sc.pp.log1p),
-            SpaGCNGraph(alpha=alpha, beta=beta),
-            SpaGCNGraph2D(),
-            CellPCA(n_components=dim),
-            SetConfig({
-                "feature_channel": ["CellPCA", "SpaGCNGraph", "SpaGCNGraph2D"],
-                "feature_channel_type": ["obsm", "obsp", "obsp"],
-                "label_channel": "label",
-                "label_channel_type": "obs"
-            }),
-            log_level=log_level,
-        )
+    def __init__(self, delay: int = 0, t_max: float = 1.0):
+        self.val = t_max
 
-    def search_l(self, p, adj, start=0.01, end=1000, tol=0.01, max_run=100):
-        """Search best l.
+    def __next__(self):
+        return self.val
 
-        Parameters
-        ----------
-        p : float
-            Percentage.
-        adj :
-            Adjacent matrix.
-        start : float
-            Starting value for searching l.
-        end : float
-            Ending value for searching l.
-        tol : float
-            Tolerant value for searching l.
-        max_run : int
-            Maximum number of runs.
 
-        Returns
-        -------
-        l : float
-            best l, the parameter to control percentage p.
+####################################
+## Created by scMVAE
+####################################
 
-        """
-        l = search_l(p, adj, start, end, tol, max_run)
-        return l
 
-    def set_l(self, l):
-        """Set l.
+def GMM_loss(gamma, c_params, z_params):
+    """
+    L elbo(x) = Eq(z,c|x)[ log p(x|z) ] - KL(q(z,c|x)||p(z,c))
+              = Eq(z,c|x)[ log p(x|z) + log p(z|c) + log p(c) - log q(z|x) - log q(c|x) ]
+    """
+    mu_c, var_c, pi = c_params
+    # print(mu_c.size(), var_c.size(), pi.size())
+    n_centroids = pi.size(1)
+    mu, logvar = z_params
+    mu_expand = mu.unsqueeze(2).expand(mu.size(0), mu.size(1), n_centroids)
+    logvar_expand = logvar.unsqueeze(2).expand(logvar.size(0), logvar.size(1), n_centroids)
 
-        Parameters
-        ----------
-        l : float
-            The parameter to control percentage p.
+    # log p(z|c)
+    logpzc = -0.5 * torch.sum(gamma * torch.sum(math.log(2 * math.pi) + \
+                                                torch.log(var_c) + \
+                                                torch.exp(logvar_expand) / var_c + \
+                                                (mu_expand - mu_c) ** 2 / var_c, dim=1), dim=1)
+    # log p(c)
+    logpc = torch.sum(gamma * torch.log(pi), 1)
 
-        """
-        self.l = l
+    # log q(z|x) or q entropy
+    qentropy = -0.5 * torch.sum(1 + logvar + math.log(2 * math.pi), 1)
 
-    def search_set_res(self, x, l, target_num, start=0.4, step=0.1, tol=5e-3, lr=0.05, epochs=10, max_run=10):
-        """Search for optimal resolution parameter."""
-        res = start
-        logger.info(f"Start at {res = :.4f}, {step = :.4f}")
-        clf = SpaGCN(l)
-        y_pred = clf.fit_predict(x, init_spa=True, init="louvain", res=res, tol=tol, lr=lr, epochs=epochs)
-        old_num = len(set(y_pred))
-        logger.info(f"Res = {res:.4f}, Num of clusters = {old_num}")
-        run = 0
-        while old_num != target_num:
-            old_sign = 1 if (old_num < target_num) else -1
-            clf = SpaGCN(l)
-            y_pred = clf.fit_predict(x, init_spa=True, init="louvain", res=res + step * old_sign, tol=tol, lr=lr,
-                                     epochs=epochs)
-            new_num = len(set(y_pred))
-            logger.info(f"Res = {res + step * old_sign:.3e}, Num of clusters = {new_num}")
-            if new_num == target_num:
-                res = res + step * old_sign
-                logger.info(f"recommended res = {res:.4f}")
-                return res
-            new_sign = 1 if (new_num < target_num) else -1
-            if new_sign == old_sign:
-                res = res + step * old_sign
-                logger.info(f"Res changed to {res}")
-                old_num = new_num
-            else:
-                step = step / 2
-                logger.info(f"Step changed to {step:.4f}")
-            if run > max_run:
-                logger.info(f"Exact resolution not found. Recommended res = {res:.4f}")
-                return res
-            run += 1
-        logger.info("Recommended res = {res:.4f}")
-        self.res = res
+    # log q(c|x)
+    logqcx = torch.sum(gamma * torch.log(gamma), 1)
+
+    kld = -logpzc - logpc + qentropy + logqcx
+
+    return kld
+
+
+####################################
+## Created by DCCA
+####################################
+
+
+class Eucli_dis(nn.Module):
+    """like what you like: knowledge distill via neuron selectivity transfer."""
+
+    def __init__(self):
+        super().__init__()
+        pass
+
+    def forward(self, g_s, g_t):
+        g_s = g_s.float()
+        g_t = g_t.float()
+        ret = torch.pow((g_s - g_t), 2)
+
+        return torch.sum(ret, dim=1)
+
+
+class L1_dis(nn.Module):
+    """like what you like: knowledge distill via neuron selectivity transfer."""
+
+    def __init__(self):
+        super().__init__()
+        pass
+
+    def forward(self, g_s, g_t):
+        g_s = g_s.float()
+        g_t = g_t.float()
+
+        ret = torch.abs(g_s - g_t)
+
+        return torch.sum(ret, dim=1)
+
+
+class NSTLoss(nn.Module):
+    """like what you like: knowledge distill via neuron selectivity transfer."""
+
+    def __init__(self):
+        super().__init__()
+        pass
+
+    def forward(self, g_s, g_t):
+        return [self.nst_loss(f_s, f_t) for f_s, f_t in zip(g_s, g_t)]
+
+    def nst_loss(self, f_s, f_t):
+
+        f_s = f_s.view(f_s.shape[0], f_s.shape[1], -1)
+        f_s = F.normalize(f_s, dim=2)
+        f_t = f_t.view(f_t.shape[0], f_t.shape[1], -1)
+        f_t = F.normalize(f_t, dim=2)
+
+        # set full_loss as False to avoid unnecessary computation
+        full_loss = False
+        if full_loss:
+            return (self.poly_kernel(f_t, f_t).mean().detach() + self.poly_kernel(f_s, f_s).mean() -
+                    2 * self.poly_kernel(f_s, f_t).mean())
+        else:
+            return self.poly_kernel(f_s, f_s).mean() - 2 * self.poly_kernel(f_s, f_t).mean()
+
+    def poly_kernel(self, a, b):
+        a = a.unsqueeze(1)
+        b = b.unsqueeze(2)
+        res = (a * b).sum(-1).pow(2)
         return res
 
-    def calc_adj_exp(self, adj: np.ndarray) -> np.ndarray:
-        adj_exp = np.exp(-1 * (adj**2) / (2 * (self.l**2)))
-        return adj_exp
-
-    def fit(self, x, y=None, *, num_pcs=50, lr=0.005, epochs=2000, weight_decay=0, opt="admin", init_spa=True,
-            init="louvain", n_neighbors=10, n_clusters=None, res=0.4, tol=1e-3):
-        """Fit function for model training.
 
-        Parameters
-        ----------
-        embed
-            Input data.
-        adj
-            Adjacent matrix.
-        num_pcs : int
-            The number of component used in PCA.
-        lr : float
-            Learning rate.
-        epochs : int
-            Maximum number of epochs.
-        weight_decay : float
-            Weight decay.
-        opt : str
-            Optimizer.
-        init_spa : bool
-            Initialize spatial.
-        init : str
-            "louvain" or "kmeans".
-        n_neighbors : int
-            The number of neighbors used by Louvain.
-        n_clusters : int
-            The number of clusters usedd by kmeans.
-        res : float
-            The resolution parameter used by Louvain.
-        tol : float
-            Oolerant value for searching l.
+class FactorTransfer(nn.Module):
+    """Paraphrasing Complex Network: Network Compression via Factor Transfer, NeurIPS
+    2018."""
 
-        """
-        embed, adj = x
-        self.num_pcs = num_pcs
-        self.res = res
-        self.lr = lr
-        self.epochs = epochs
-        self.weight_decay = weight_decay
-        self.opt = opt
-        self.init_spa = init_spa
-        self.init = init
-        self.n_neighbors = n_neighbors
-        self.n_clusters = n_clusters
-        self.res = res
-        self.tol = tol
-        if self.l is None:
-            raise ValueError("l should be set before fitting the model!")
-
-        self.model = SimpleGCDEC(embed.shape[1], embed.shape[1])
-        adj_exp = self.calc_adj_exp(adj)
-        self.model.fit(embed, adj_exp, lr=self.lr, epochs=self.epochs, weight_decay=self.weight_decay, opt=self.opt,
-                       init_spa=self.init_spa, init=self.init, n_neighbors=self.n_neighbors, n_clusters=self.n_clusters,
-                       res=self.res, tol=self.tol)
+    def __init__(self, p1=2, p2=1):
+        super().__init__()
+        self.p1 = p1
+        self.p2 = p2
 
-    def predict_proba(self, x):
-        """Prediction function.
+    def forward(self, f_s, f_t):
+        return self.factor_loss(f_s, f_t)
 
-        Returns
-        -------
-        Tuple[np.ndarray, np.ndarray]
-            The predicted labels and the predicted probabilities.
+    def factor_loss(self, f_s, f_t):
+        s_H, t_H = f_s.shape[2], f_t.shape[2]
+        if s_H > t_H:
+            f_s = F.adaptive_avg_pool2d(f_s, (t_H, t_H))
+        elif s_H < t_H:
+            f_t = F.adaptive_avg_pool2d(f_t, (s_H, s_H))
+        else:
+            pass
+        if self.p2 == 1:
+            return (self.factor(f_s) - self.factor(f_t)).abs().mean()
+        else:
+            return (self.factor(f_s) - self.factor(f_t)).pow(self.p2).mean()
 
-        """
-        embed, adj = x
-        adj_exp = self.calc_adj_exp(adj)
-        _, pred_prob = self.model.predict(embed, adj_exp)
-        return pred_prob
+    def factor(self, f):
+        return F.normalize(f.pow(self.p1).mean(1).view(f.size(0), -1))
+
+
+class Similarity(nn.Module):
+    """Similarity-Preserving Knowledge Distillation, ICCV2019, verified by original
+    author."""
 
-    def predict(self, x):
-        """Prediction function.
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, g_s, g_t):
+        return [self.similarity_loss(f_s, f_t) for f_s, f_t in zip(g_s, g_t)]
+
+    def similarity_loss(self, f_s, f_t):
+        bsz = f_s.shape[0]
+        f_s = f_s.view(bsz, -1)
+        f_t = f_t.view(bsz, -1)
+
+        G_s = torch.mm(f_s, torch.t(f_s))
+        # G_s = G_s / G_s.norm(2)
+        G_s = torch.nn.functional.normalize(G_s)
+        G_t = torch.mm(f_t, torch.t(f_t))
+        # G_t = G_t / G_t.norm(2)
+        G_t = torch.nn.functional.normalize(G_t)
+
+        G_diff = G_t - G_s
+        loss = (G_diff * G_diff).view(-1, 1).sum(0) / (bsz * bsz)
+        return loss
+
+
+class Correlation(nn.Module):
+    """Correlation Congruence for Knowledge Distillation, ICCV 2019.
+
+    The authors nicely shared the code with me. I restructured their code to be compatible with my running framework.
+    Credits go to the original author
+
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, f_s, f_t):
+        delta = torch.abs(f_s - f_t)
+        loss = torch.mean((delta[:-1] * delta[1:]).sum(1))
+        return loss
+
+
+class KL_diver(nn.Module):
+
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, mean_1, logvar_1, mean_2, logvar_2):
+        loss = kl(Normal(mean_1, logvar_1), Normal(mean_2, logvar_2)).sum(dim=1)
+
+        return loss
+
+
+class Attention(nn.Module):
+    """Paying More Attention to Attention: Improving the Performance of Convolutional Neural Networks
+    via Attention Transfer
+    code: https://github.com/szagoruyko/attention-transfer"""
+
+    def __init__(self, p=2):
+        super().__init__()
+        self.p = p
+
+    def forward(self, g_s, g_t):
+        g_s_norm = F.normalize(g_s, p=2, dim=1)
+        g_t_norm = F.normalize(g_t, p=2, dim=1)
+        diff_g = g_s_norm - g_t_norm
+
+        result = (diff_g.norm(p=2, dim=1, keepdim=True)).sum(dim=1)
+
+        return result
+
+
+class ZINBLoss(nn.Module):
+    """ZINB loss class."""
+
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, x, mean, disp, pi, scale_factor, ridge_lambda=0.0):
+        """Forward propagation.
+
+        Parameters
+        ----------
+        x :
+            input features.
+        mean :
+            data mean.
+        disp :
+            data dispersion.
+        pi :
+            data dropout probability.
+        scale_factor : list
+            scale factor of mean.
+        ridge_lambda : float optional
+            ridge parameter.
 
         Returns
         -------
-        Tuple[np.ndarray, np.ndarray]
-            The predicted labels and the predicted probabilities.
+        result : float
+            ZINB loss.
 
         """
-        pred_prob = self.predict_proba(x)
-        pred = torch.argmax(pred_prob, dim=1).data.cpu().numpy()
-        return pred
+        eps = 1e-10
+        scale_factor = scale_factor[:, None]
+        mean = mean * scale_factor
+
+        t1 = torch.lgamma(disp + eps) + torch.lgamma(x + 1.0) - torch.lgamma(x + disp + eps)
+        t2 = (disp + x) * torch.log(1.0 + (mean / (disp + eps))) + (x * (torch.log(disp + eps) - torch.log(mean + eps)))
+        nb_final = t1 + t2
+
+        nb_case = nb_final - torch.log(1.0 - pi + eps)
+        zero_nb = torch.pow(disp / (disp + mean + eps), disp)
+        zero_case = -torch.log(pi + ((1.0 - pi) * zero_nb) + eps)
+        result = torch.where(torch.le(x, 1e-8), zero_case, nb_case)
+
+        if ridge_lambda > 0:
+            ridge = ridge_lambda * torch.square(pi)
+            result += ridge
+
+        result = torch.mean(result)
+        return result
+
+
+def dist_loss(data, min_dist, max_dist=20):
+    pairwise_dist = cdisttf(data, data)
+    dist = pairwise_dist - min_dist
+    bigdist = max_dist - pairwise_dist
+    loss = torch.exp(-dist) + torch.exp(-bigdist)
+    return loss
+
+
+def cdisttf(data_1, data_2):
+    prod = torch.sum((data_1.unsqueeze(1) - data_2.unsqueeze(0))**2, 2)
+    return (prod + 1e-10)**(1 / 2)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydance-1.0.0/dance/modules/spatial/spatial_domain/stagate.py` & `pydance-1.0.0rc0/dance/modules/spatial/spatial_domain/stagate.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,41 +4,105 @@
 
 Reference
 ----------
 Dong, Kangning, and Shihua Zhang. "Deciphering spatial domains from spatially resolved transcriptomics with an adaptive
 graph attention auto-encoder." Nature communications 13.1 (2022): 1-12.
 
 """
+
+# import seaborn as sns
+import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
 import scanpy as sc
+import scipy.sparse as sp
+import sklearn.neighbors
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from sklearn.mixture import GaussianMixture
+from sklearn import mixture
 from torch import Tensor
 from torch.nn import Parameter
+from torch_geometric.data import Data
 from torch_geometric.nn.conv import MessagePassing
+from torch_geometric.nn.dense.linear import Linear
 from torch_geometric.utils import add_self_loops, remove_self_loops, softmax
+from torch_sparse import SparseTensor, set_diag
 from tqdm import tqdm
 
-from dance import logger
-from dance.modules.base import BaseClusteringMethod, BasePretrain
-from dance.transforms import AnnDataTransform, Compose, SetConfig
-from dance.transforms.graph import StagateGraph
-from dance.typing import Any, LogLevel, Optional, Tuple
-from dance.utils import get_device
+
+def transfer_pytorch_data(adata, adj):
+    edgeList = adj
+    if type(adata.X) == np.ndarray:
+        data = Data(edge_index=torch.LongTensor(np.array([edgeList[0], edgeList[1]])),
+                    x=torch.FloatTensor(adata.X))  # .todense()
+    else:
+        data = Data(edge_index=torch.LongTensor(np.array([edgeList[0], edgeList[1]])),
+                    x=torch.FloatTensor(adata.X.todense()))  # .todense()
+    return data
+
+
+def Stats_Spatial_Net(adata):
+    import matplotlib.pyplot as plt
+    Num_edge = adata.uns['Spatial_Net']['Cell1'].shape[0]
+    Mean_edge = Num_edge / adata.shape[0]
+    plot_df = pd.value_counts(pd.value_counts(adata.uns['Spatial_Net']['Cell1']))
+    plot_df = plot_df / adata.shape[0]
+    fig, ax = plt.subplots(figsize=[3, 2])
+    plt.ylabel('Percentage')
+    plt.xlabel('')
+    plt.title('Number of Neighbors (Mean=%.2f)' % Mean_edge)
+    ax.bar(plot_df.index, plot_df)
+
+
+def mclust_P(adata, num_cluster, used_obsm='STAGATE', modelNames='EEE'):
+
+    from sklearn import mixture
+    g = mixture.GaussianMixture(n_components=num_cluster, covariance_type='tied', warm_start=True, n_init=100,
+                                max_iter=300, reg_covar=1.4663143602030552e-04, random_state=36282,
+                                tol=0.00022187708009762592)
+    res = g.fit_predict(adata.obsm[used_obsm])
+    adata.obs['mclust'] = res
+    return adata
+
+
+'''
+def mclust_R(adata, num_cluster, modelNames='EEE', used_obsm='STAGATE', random_seed=2020):
+    """\
+    Clustering using the mclust algorithm.
+    The parameters are the same as those in the R package mclust.
+    """
+
+    np.random.seed(random_seed)
+    import rpy2.robjects as robjects
+    robjects.r.library("mclust")
+
+    import rpy2.robjects.numpy2ri
+    rpy2.robjects.numpy2ri.activate()
+    r_random_seed = robjects.r['set.seed']
+    r_random_seed(random_seed)
+    rmclust = robjects.r['Mclust']
+
+    res = rmclust(rpy2.robjects.numpy2ri.numpy2rpy(adata.obsm[used_obsm]), num_cluster, modelNames)
+    mclust_res = np.array(res[-2])
+
+    adata.obs['mclust'] = mclust_res
+    adata.obs['mclust'] = adata.obs['mclust'].astype('int')
+    adata.obs['mclust'] = adata.obs['mclust'].astype('category')
+    return adata
+'''
 
 
 class GATConv(MessagePassing):
     """Graph attention layer from Graph Attention Network."""
     _alpha = None
 
     def __init__(self, in_channels, out_channels, heads: int = 1, concat: bool = True, negative_slope: float = 0.2,
                  dropout: float = 0.0, add_self_loops=True, bias=True, **kwargs):
-        kwargs.setdefault("aggr", "add")
+        kwargs.setdefault('aggr', 'add')
         super().__init__(node_dim=0, **kwargs)
 
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.heads = heads
         self.concat = concat
         self.negative_slope = negative_slope
@@ -61,224 +125,253 @@
     def forward(self, x, edge_index, size=None, return_attention_weights=None, attention=True, tied_attention=None):
 
         H, C = self.heads, self.out_channels
 
         # We first transform the input node features. If a tuple is passed, we
         # transform source and target node features via separate weights:
         if isinstance(x, Tensor):
-            assert x.dim() == 2, "Static graphs not supported in GATConv"
+            assert x.dim() == 2, "Static graphs not supported in 'GATConv'"
             # x_src = x_dst = self.lin_src(x).view(-1, H, C)
             x_src = x_dst = torch.mm(x, self.lin_src).view(-1, H, C)
         else:  # Tuple of source and target node features:
             x_src, x_dst = x
-            assert x_src.dim() == 2, "Static graphs not supported in GATConv"
+            assert x_src.dim() == 2, "Static graphs not supported in 'GATConv'"
             x_src = self.lin_src(x_src).view(-1, H, C)
             if x_dst is not None:
                 x_dst = self.lin_dst(x_dst).view(-1, H, C)
 
         x = (x_src, x_dst)
 
         if not attention:
             return x[0].mean(dim=1)
+            # return x[0].view(-1, self.heads * self.out_channels)
 
-        if tied_attention is None:
+        if tied_attention == None:
             # Next, we compute node-level attention coefficients, both for source
             # and target nodes (if present):
             alpha_src = (x_src * self.att_src).sum(dim=-1)
             alpha_dst = None if x_dst is None else (x_dst * self.att_dst).sum(-1)
             alpha = (alpha_src, alpha_dst)
             self.attentions = alpha
         else:
             alpha = tied_attention
 
         if self.add_self_loops:
-            # We only want to add self-loops for nodes that appear both as
-            # source and target nodes:
-            num_nodes = x_src.size(0)
-            if x_dst is not None:
-                num_nodes = min(num_nodes, x_dst.size(0))
-            num_nodes = min(size) if size is not None else num_nodes
-            edge_index, _ = remove_self_loops(edge_index)
-            edge_index, _ = add_self_loops(edge_index, num_nodes=num_nodes)
+            if isinstance(edge_index, Tensor):
+                # We only want to add self-loops for nodes that appear both as
+                # source and target nodes:
+                num_nodes = x_src.size(0)
+                if x_dst is not None:
+                    num_nodes = min(num_nodes, x_dst.size(0))
+                num_nodes = min(size) if size is not None else num_nodes
+                edge_index, _ = remove_self_loops(edge_index)
+                edge_index, _ = add_self_loops(edge_index, num_nodes=num_nodes)
+            elif isinstance(edge_index, SparseTensor):
+                edge_index = set_diag(edge_index)
 
         out = self.propagate(edge_index, x=x, alpha=alpha, size=size)
 
         alpha = self._alpha
         assert alpha is not None
         self._alpha = None
 
         if self.concat:
             out = out.view(-1, self.heads * self.out_channels)
         else:
             out = out.mean(dim=1)
 
         if isinstance(return_attention_weights, bool):
-            return out, (edge_index, alpha)
+            if isinstance(edge_index, Tensor):
+                return out, (edge_index, alpha)
+            elif isinstance(edge_index, SparseTensor):
+                return out, edge_index.set_value(alpha, layout='coo')
         else:
             return out
 
     def message(self, x_j, alpha_j, alpha_i, index, ptr, size_i):
         alpha = alpha_j if alpha_i is None else alpha_j + alpha_i
+
+        # alpha = F.leaky_relu(alpha, self.negative_slope)
         alpha = torch.sigmoid(alpha)
+
         alpha = softmax(alpha, index, ptr, size_i)
         self._alpha = alpha  # Save for later use.
         alpha = F.dropout(alpha, p=self.dropout, training=self.training)
         return x_j * alpha.unsqueeze(-1)
 
     def __repr__(self):
-        return "{}({}, {}, heads={})".format(self.__class__.__name__, self.in_channels, self.out_channels, self.heads)
+        return '{}({}, {}, heads={})'.format(self.__class__.__name__, self.in_channels, self.out_channels, self.heads)
 
 
-class Stagate(nn.Module, BasePretrain, BaseClusteringMethod):
+class Stagate(torch.nn.Module):
     """Stagate class.
 
     Parameters
     ----------
-    hidden_dims
-        Hidden dimensions.
-    device
-        Computation device.
-    pretrain_path
-        Save the cell representations from the trained STAGATE model to the specified path. Do not save if unspecified.
+    hidden_dims : int
+        hidden dimensions
 
     """
 
-    def __init__(self, hidden_dims, device: str = "auto", pretrain_path: Optional[str] = None):
+    def __init__(self, hidden_dims):
         super().__init__()
-        self.pretrain_path = pretrain_path
 
         [in_dim, num_hidden, out_dim] = hidden_dims
         self.conv1 = GATConv(in_dim, num_hidden, heads=1, concat=False, dropout=0, add_self_loops=False, bias=False)
         self.conv2 = GATConv(num_hidden, out_dim, heads=1, concat=False, dropout=0, add_self_loops=False, bias=False)
         self.conv3 = GATConv(out_dim, num_hidden, heads=1, concat=False, dropout=0, add_self_loops=False, bias=False)
         self.conv4 = GATConv(num_hidden, in_dim, heads=1, concat=False, dropout=0, add_self_loops=False, bias=False)
 
-        self.device = get_device(device)
-        self.to(self.device)
-
-    @staticmethod
-    def preprocessing_pipeline(hvg_flavor: str = "seurat_v3", n_top_hvgs: int = 3000, model_name: str = "radius",
-                               radius: float = 150, n_neighbors: int = 5, log_level: LogLevel = "INFO"):
-        return Compose(
-            AnnDataTransform(sc.pp.highly_variable_genes, flavor=hvg_flavor, n_top_genes=n_top_hvgs, subset=True),
-            AnnDataTransform(sc.pp.normalize_total, target_sum=1e4),
-            AnnDataTransform(sc.pp.log1p),
-            StagateGraph(model_name, radius=radius, n_neighbors=n_neighbors),
-            SetConfig({
-                "feature_channel": "StagateGraph",
-                "feature_channel_type": "obsp",
-                "label_channel": "label",
-                "label_channel_type": "obs"
-            }),
-            log_level=log_level,
-        )
-
     def forward(self, features, edge_index):
-        """Forward function for training.
+        """forward function for training.
 
         Parameters
         ----------
-        features
-            Node features.
-        edge_index
-            Adjacent matrix.
+        features :
+            node features.
+        edge_index :
+            adjacent matrix.
 
         Returns
         -------
-        Tuple[Tensor, Tensor]
-            The second and the forth hidden layerx.
+        h2 :
+            the second hidden layer.
+        h4 :
+            the forth hidden layer.
 
         """
         h1 = F.elu(self.conv1(features, edge_index))
         h2 = self.conv2(h1, edge_index, attention=False)
         self.conv3.lin_src.data = self.conv2.lin_src.transpose(0, 1)
         self.conv3.lin_dst.data = self.conv2.lin_dst.transpose(0, 1)
         self.conv4.lin_src.data = self.conv1.lin_src.transpose(0, 1)
         self.conv4.lin_dst.data = self.conv1.lin_dst.transpose(0, 1)
         h3 = F.elu(self.conv3(h2, edge_index, attention=True, tied_attention=self.conv1.attentions))
         h4 = self.conv4(h3, edge_index, attention=False)
 
-        return h2, h4
+        return h2, h4  # F.log_softmax(x, dim=-1)
+
+    def fit(self, adata, graph, n_epochs=1, lr=0.001, key_added='STAGATE', gradient_clipping=5., pre_resolution=0.2,
+            weight_decay=0.0001, verbose=True, random_seed=0, save_loss=False, save_reconstrction=False,
+            device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
+        """fit function for training.
+
+        Parameters
+        ----------
+        adata :
+            input data.
+        graph :
+            graph structure.
+        n_epochs : int optional
+            number of epochs.
+        lr : float optional
+            learning rate.
+        key_added : str optional
+            by default 'STAGATE'.
+        gradient_clipping : float optional
+            gradient clipping.
+        pre_resolution : float optional
+            pre resolution.
+        weight_decay : float optional
+            weight decay.
+        verbose : bool optional
+            verbose, by default to be True.
+        random_seed : int optional
+            random seed by default to be 0.
+        save_loss : bool optional
+            by default to be False.
+        save_reconstrction : bool optional
+            by default to be False.
+        device : str optional
+            to indicate gpu or cpu device.
+
+        Returns
+        -------
+        None.
+
+        """
+        adata.X = sp.csr_matrix(adata.X)
+
+        if 'highly_variable' in adata.var.columns:
+            adata_Vars = adata[:, adata.var['highly_variable']]
+        else:
+            adata_Vars = adata
+
+        if verbose:
+            print('Size of Input: ', adata_Vars.shape)
+        if 'Spatial_Net' not in adata.uns.keys():
+            raise ValueError("Spatial_Net is not existed! Run Cal_Spatial_Net first!")
+
+        data = transfer_pytorch_data(adata_Vars, graph)
+
+        model = self.to(device)
+        data = data.to(device)
+
+        optimizer = torch.optim.Adam(model.parameters(), lr=lr, weight_decay=weight_decay)
 
-    def pretrain(
-        self,
-        x: np.ndarray,
-        edge_index_array: np.ndarray,
-        lr: float = 1e-3,
-        weight_decay: float = 1e-4,
-        epochs: int = 100,
-        gradient_clipping: float = 5,
-    ):
-        x_tensor = torch.from_numpy(x.astype(np.float32)).to(self.device)
-        edge_index_tensor = torch.from_numpy(edge_index_array.astype(int)).to(self.device)
-
-        optimizer = torch.optim.Adam(self.parameters(), lr=lr, weight_decay=weight_decay)
-        self.train()
-        for epoch in tqdm(range(1, epochs + 1)):
+        # loss_list = []
+        for epoch in tqdm(range(1, n_epochs + 1)):
+            model.train()
             optimizer.zero_grad()
-            z, out = self(x_tensor, edge_index_tensor)
-            loss = F.mse_loss(x_tensor, out)
+            z, out = model(data.x, data.edge_index)
+            loss = F.mse_loss(data.x, out)
+            # loss_list.append(loss)
             loss.backward()
-            torch.nn.utils.clip_grad_norm_(self.parameters(), gradient_clipping)
+            torch.nn.utils.clip_grad_norm_(model.parameters(), gradient_clipping)
             optimizer.step()
 
-        self.eval()
-        z, _ = self(x_tensor, edge_index_tensor)
-        self.rep = z.detach().clone().cpu().numpy()
-
-    def save_pretrained(self, path):
-        np.save(path, self.rep)
-
-    def load_pretrained(self, path):
-        self.rep = np.load(path)
-
-    def fit(
-        self,
-        inputs: Tuple[np.ndarray, np.ndarray],
-        epochs: int = 100,
-        lr: float = 0.001,
-        gradient_clipping: float = 5,
-        weight_decay: float = 1e-4,
-        num_cluster: int = 7,
-        gmm_reg_covar: float = 1.5e-4,
-        gmm_n_init: int = 10,
-        gmm_max_iter: int = 300,
-        gmm_tol: float = 2e-4,
-        random_state: Optional[int] = None,
-    ):
-        """Fit function for training.
+        print("eval ....")
+        model.eval()
+        z, out = model(data.x, data.edge_index)
+
+        STAGATE_rep = z.to('cpu').detach().numpy()
+        adata.obsm[key_added] = STAGATE_rep
+
+        if save_loss:
+            adata.uns['STAGATE_loss'] = loss
+        if save_reconstrction:
+            ReX = out.to('cpu').detach().numpy()
+            ReX[ReX < 0] = 0
+            adata.layers['STAGATE_ReX'] = ReX
+
+        print("post process...")
+        sc.pp.neighbors(adata, use_rep='STAGATE')
+        sc.tl.umap(adata)
+        #adata = mclust_R(adata, used_obsm='STAGATE', num_cluster=7)
+        adata = mclust_P(adata, used_obsm='STAGATE', num_cluster=7)
+        self.adata = adata
+
+    def predict(self, ):
+        """prediction function.
 
         Parameters
         ----------
-        inputs
-            A tuple containing (1) the input features and (2) the edge index array (coo representation) of the
-            adjacency matrix.
-        epochs
-            Number of epochs.
-        lr
-            Learning rate.
-        gradient_clipping
-            Gradient clipping.
-        weight_decay
-            Weight decay.
-        num_cluster
-            Number of cluster.
 
-        """
-        x, edge_index_array = inputs
-        self._pretrain(x, edge_index_array, lr, weight_decay, epochs, gradient_clipping)
+        Returns
+        -------
+        self.y_pred :
+            predicted label.
 
-        logger.info("Fitting Gaussian Mixture model for cluster assignments.")
-        gmm = GaussianMixture(n_components=num_cluster, covariance_type="tied", n_init=gmm_n_init, tol=gmm_tol,
-                              max_iter=gmm_max_iter, reg_covar=gmm_reg_covar, random_state=random_state)
-        self.clust_res = gmm.fit_predict(self.rep)
+        """
+        data_dropna = self.adata.obs.dropna()
+        self.y_pred = data_dropna['mclust']
+        self.target = data_dropna['ground_truth']
+        return data_dropna['mclust']
 
-    def predict(self, x: Optional[Any] = None):
-        """Prediction function.
+    def score(self, y_true=None):
+        """score function to get score of prediction.
 
         Parameters
         ----------
-        x
-            Not used, for compatibility with :class:`BaseClusteringMethod`.
+        y_true :
+            ground truth label.
+
+        Returns
+        -------
+        score : float
+            metric eval score.
 
         """
-        return self.clust_res
+        from sklearn.metrics.cluster import adjusted_rand_score
+        score = adjusted_rand_score(self.target, self.y_pred)
+        print("ARI {}".format(adjusted_rand_score(self.target, self.y_pred)))
+        return score
```

### Comparing `pydance-1.0.0/pydance.egg-info/PKG-INFO` & `pydance-1.0.0rc0/pydance.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pydance
-Version: 1.0.0
+Version: 1.0.0rc0
 Summary: Deep Learning for Single-cell Analysis
 Home-page: https://github.com/OmicsML/dance
 Author: "DANCE Team"
 Author-email: "danceteamgnn@gmail.com"
 License: BSD 2-Clause License
 Keywords: Single-cell Biology,Deep Learning,Graph Neural Networks
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: doc
 
 <p align="center">
   <img
        src="https://github.com/OmicsML/dance/blob/main/imgs/dance_logo.jpg"
        style="width:100%; height:100%; object-fit:cover;"
   />
 </p>
@@ -29,170 +29,124 @@
 ______________________________________________________________________
 
 [![PyPI version](https://badge.fury.io/py/pydance.svg)](https://badge.fury.io/py/pydance)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Documentation Status](https://readthedocs.org/projects/pydance/badge/?version=latest)](https://pydance.readthedocs.io/en/latest/?badge=latest)
 [![Test Examples](https://github.com/OmicsML/dance/actions/workflows/test_examples.yml/badge.svg)](https://github.com/OmicsML/dance/actions/workflows/test_examples.yml)
 
-[![Slack](https://img.shields.io/badge/slack-OmicsML-brightgreen)](https://omicsml.slack.com)
-[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Ftwitter.com%2FOmicsML)](https://twitter.com/OmicsML)
-
-DANCE is a Python toolkit to support deep learning models for analyzing single-cell gene expression at scale. Our goal is to build up a deep learning community and benchmark platform for computational models in single-cell analysis. It includes three modules at present:
+DANCE is a Python toolkit to support deep learning models for analyzing single-cell gene expression at scale. It includes three modules at present:
 
 1. **Single-modality analysis**
 1. **Single-cell multimodal omics**
 1. **Spatially resolved transcriptomics**
 
-### Useful links
-
-OmicsML Homepage: https://omicsml.ai \
-DANCE Open Source: https://github.com/OmicsML/dance \
-DANCE Documentation: https://pydance.readthedocs.io/en/latest/ \
-DANCE Tutorials: https://github.com/OmicsML/dance-tutorials \
-DANCE Package Paper: https://www.biorxiv.org/content/10.1101/2022.10.19.512741v2 \
-Survey Paper: https://arxiv.org/abs/2210.12385
-
-### Join the Community
-
-Slack: https://join.slack.com/t/omicsml/shared_invite/zt-1hxdz7op3-E5K~EwWF1xDvhGZFrB9AbA \
-Twitter: https://twitter.com/OmicsML \
-Wechat Group Assistant: 736180290 \
-Email: danceteamgnn@gmail.com
-
-### Contributing
-
-Community-wide contribution is the key for a sustainable development and
-continual growth of the DANCE package. We deeply appreciate any contribution
-made to improve the DANCE code base. If you would like to get started, please
-refer to our brief [guidelines](CONTRIBUTING.md) about our automated quality
-controls, as well as setting up the `dev` environments.
-
-## Citation
-
-If you find our work useful in your research, please consider citing our DANCE package or survey paper:
-
-```bibtex
-@article{ding2022dance,
-  title={DANCE: A Deep Learning Library and Benchmark for Single-Cell Analysis},
-  author={Ding, Jiayuan and Wen, Hongzhi and Tang, Wenzhuo and Liu, Renming and Li, Zhaoheng and Venegas, Julian and Su, Runze and Molho, Dylan and Jin, Wei and Zuo, Wangyang and others},
-  journal={bioRxiv},
-  year={2022},
-  publisher={Cold Spring Harbor Laboratory}
-}
-```
-
-```bibtex
-@article{molho2022deep,
-  title={Deep Learning in Single-Cell Analysis},
-  author={Molho, Dylan and Ding, Jiayuan and Li, Zhaoheng and Wen, Hongzhi and Tang, Wenzhuo and Wang, Yixin and Venegas, Julian and Jin, Wei and Liu, Renming and Su, Runze and others},
-  journal={arXiv preprint arXiv:2210.12385},
-  year={2022}
-}
-```
+Our goal is to build up a deep learning community for single cell analysis and provide GNN based architecture for users for further development in single cell analysis.
 
 ## Usage
 
 ### Overview
 
-In release 1.0, the main usage of the DANCE is to provide readily available experiment reproduction
+In release 1.0, the main usage of the PyDANCE is to provide readily available experiment reproduction
 (see detail information about the reproduced performance [below](#implemented-algorithms)).
-Users can easily reproduce selected experiments presented in the original papers for the computational single-cell methods implemented in DANCE, which can be found under [`examples/`](examples).
+Users can easily reproduce selected experiments presented in the original papers for the computational single-cell methods implemented in PyDANCE, which can be found under [`examples/`](examples).
 
 ### Motivation
 
 Computational methods for single-cell analysis are quickly emerging, and the field is revolutionizing the usage of single-cell data to gain biological insights.
 A key challenge to continually developing computational single-cell methods that achieve new state-of-the-art performance is reproducing previous benchmarks.
 More specifically, different studies prepare their datasets and perform evaluation differently,
 and not to mention the compatibility of different methods, as they could be written in different languages or using incompatible library versions.
 
-DANCE addresses these challenges by providing a unified Python package implementing many popular computational single-cell methods (see [Implemented Algorithms](#implemented-algorithms)),
+PyDANCE addresses these challenges by providing a unified Python packge implementing many popular computational single-cell methods (see [Implemented Algorithms](#implemented-algorithms)),
 as well as easily reproducible experiments by providing unified tools for
 
 - Data downloading
 - Data (pre-)processing and transformation (e.g. graph construction)
 - Model training and evaluation
 
-### Example: run cell-type annotation benchmark using scDeepSort
+### Example: runing cell-type annotation benchmark using scDeepSort
 
-- Step0. Install DANCE (see [Installation](#installation))
+- Step0. Install PyDANCE (see [Installation](#installation))
 - Step1. Navigate to the folder containing the corresponding example scrtip.
   In this case, it is [`examples/single_modality/cell_type_annotation`](examples/single_modality/cell_type_annotation).
 - Step2. Obtain command line interface (CLI) options for a particular experiment to reproduce at the end of the
   [script](examples/single_modality/cell_type_annotation/scdeepsort.py).
   For example, the CLI options for reproducing the `Mouse Brain` experiment is
   ```bash
-  python scdeepsort.py --species mouse --tissue Brain --train_dataset 753 3285 --test_dataset 2695
+  python scdeepsort.py --data_type scdeepsort --tissue Brain --test_data 2695
   ```
-- Step3. Wait for the experiment to finish and check results.
+- Step3. Wait for the experiment to finsh and check results.
 
 ## Installation
 
 <H3>Quick install</H3>
 
 The full installation process might be a bit tedious and could involve some debugging when using CUDA enabled packages.
 Thus, we provide an `install.sh` script that simplifies the installation process, assuming the user have [conda](https://conda.io/projects/conda/en/latest/index.html) set up on their machines.
-The installation script creates a conda environment `dance` and install the DANCE package along with all its dependencies with a apseicifc CUDA version.
-Currently, two options are accepted: `cpu` and  `cu117`.
-For example, to install the DANCE package using CUDA11.7 in a `dance-env` conda environment, simply run:
+The installation script creates a conda environment `pydance` and install the PyDANCE package along with all its dependencies with a apseicifc CUDA version.
+Currently, three options are accepted: `cpu`, `cu102`, and `cu113`.
+For example, to install the DANCE package using CUDA10.2, simply run:
 
 ```bash
-# Clone the repository via SSH
-git clone git@github.com:OmicsML/dance.git && cd dance
-# Alternatively, use HTTPS if you have not set up SSH
-# git clone https://github.com/OmicsML/dance.git  && cd dance
+git clone git@github.com:OmicsML/dance.git
+cd dance
 
-# Run the auto installation script to install DANCE and its dependencies in a conda environment
-source install.sh cu117 dance-env
+source install.sh cu102
 ```
 
-**Note**: the first argument for cuda version is mandatory, while the second argument for conda environment name is optional (default is `dance`).
-
 <details>
 <summary><H3>Custom install</H3></summary>
 <br>
 
 **Step1. Setup environment**
 
-First create a conda environment for dance (optional)
+First create a conda environment for pydance (optional)
 
 ```bash
-conda create -n dance python=3.8 -y && conda activate dance-dev
+conda create -n pydance python=3.8 -y && conda activate dance-dev
 ```
 
-Then, install CUDA enabled packages (PyTorch, PyG, DGL):
+Then, install CUDA enabled packages (PyTorch, PyG, DGL) with CUDA 10.2:
 
 ```bash
-conda install pytorch=2.0.0 torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia -y
-conda install pyg=2.3.0 -c pyg -y
-conda install dgl=1.0.1 -c dglteam/label/cu117 -y
+conda install pytorch=1.12.1 torchvision cudatoolkit=10.2 -c pytorch -y
+conda install dgl-cu102 -c dglteam -y
+pip install torch-geometric==2.1.0 torch-scatter torch-sparse torch-cluster -f https://data.pyg.org/whl/torch-1.12.1+cu102.html
 ```
 
 Alternatively, install these dependencies for CPU only:
 
 ```bash
-conda install pytorch=2.0.0 torchvision torchaudio cpuonly -c pytorch -y
-conda install pyg=2.3.0 -c pyg -y
-conda install dgl -c dglteam -y
+conda install pytorch=1.12.1 torchvision cpuonly -c pytorch -y
+conda install dgl -c dglteam
+pip install torch-geometric==2.1.0 torch-scatter torch-sparse torch-cluster -f https://data.pyg.org/whl/torch-1.12.1+cpu.html
+```
+
+**Note:** If you installed PyG using conda and encountered an issue with `GLIBC_2.27` when importing `torch_geometric.nn`,
+then you may need to uninstall `torch-spline-conv` (see https://github.com/pyg-team/pytorch_geometric/issues/3593)
+
+```bash
+pip uninstall torch-spline-conv
 ```
 
-For more information about installation or other CUDA version options, check out the installation pages for the corresponding packages
+For more information about installation or other CUDA version options, check out the installation pages for the corresponding packges
 
 - [PyTorch](https://pytorch.org/get-started/)
 - [PyG](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html)
 - [DGL](https://www.dgl.ai/pages/start.html)
 
-**Step2. Install DANCE**
+**Step2. Install PyDANCE**
 
 Install from PyPI
 
 ```bash
 pip install pydance
 ```
 
-Or, install the latest dev version from source
+Install the latest dev version from source
 
 ```bash
 git clone https://github.com/OmicsML/dance.git
 cd dance
 pip install -e .
 ```
 
@@ -214,41 +168,43 @@
 | GNN                 | GNNImpute    | An efficient scRNA-seq dropout imputation method using graph attention network                               | 2021 | P1      |
 | Graph Diffusion     | MAGIC        | MAGIC: A diffusion-based imputation method reveals gene-gene interactions in single-cell RNA-sequencing data | 2018 | P1      |
 | Probabilistic Model | scImpute     | An accurate and robust imputation method scImpute for single-cell RNA-seq data                               | 2018 | P1      |
 | GAN                 | scGAIN       | scGAIN: Single Cell RNA-seq Data Imputation using Generative Adversarial Networks                            | 2019 | P1      |
 | NN                  | DeepImpute   | DeepImpute: an accurate, fast, and scalable deep neural network method to impute single-cell RNA-seq data    | 2019 | ✅       |
 | NN + TF             | Saver-X      | Transfer learning in single-cell transcriptomics improves data denoising and pattern discovery               | 2019 | P1      |
 
-| Model      | Evaluation Metric | Mouse Brain (current/reported) | Mouse Embryo (current/reported) | PBMC (current/reported) |
-| ---------- | ----------------- | ------------------------------ | ------------------------------- | ----------------------- |
-| DeepImpute | RMSE              | 0.87 / N/A                     | 1.20 / N/A                      | 2.30 / N/A              |
-| GraphSCI   | RMSE              | 1.55 / N/A                     | 1.81 / N/A                      | 3.68 / N/A              |
-| scGNN2.0   | MSE               | 1.04 / N/A                     | 1.12 / N/A                      | 1.22 / N/A              |
+| Model      | Evaluation Metric | Mouse Brain (current/reported) | Mouse Embryo (current/reported) |
+| ---------- | ----------------- | ------------------------------ | ------------------------------- |
+| DeepImpute | MSE               | 0.12 / N/A                     | 0.12 / N/A                      |
+| ScGNN      | MSE               | 0.47 / N/A                     | 1.10 / N/A                      |
+| GraphSCI   | MSE               | 0.42 / N/A                     | 0.87 / N/A                      |
 
-**Note**: scGNN2.0 is evaluated on 2,000 genes with highest variance following the original paper.
+Note: the data split modality of DeepImpute is different from ScGNN and GraphSCI, so the results are not comparable.
 
 #### 2）Cell Type Annotation
 
-| BackBone                | Model         | Algorithm                                                                                                     | Year | CheckIn |
-| ----------------------- | ------------- | ------------------------------------------------------------------------------------------------------------- | ---- | ------- |
-| GNN                     | ScDeepsort    | Single-cell transcriptomics with weighted GNN                                                                 | 2021 | ✅       |
-| Logistic Regression     | Celltypist    | Cross-tissue immune cell analysis reveals tissue-specific features in humans.                                 | 2021 | ✅       |
-| Random Forest           | singleCellNet | SingleCellNet: a computational tool to classify single cell RNA-Seq data across platforms and across species. | 2019 | ✅       |
-| Neural Network          | ACTINN        | ACTINN: automated identification of cell types in single cell RNA sequencing.                                 | 2020 | ✅       |
-| Hierarchical Clustering | SingleR       | Reference-based analysis of lung single-cell sequencing reveals a transitional profibrotic macrophage.        | 2019 | P1      |
-| SVM                     | SVM           | A comparison of automatic cell identification methods for single-cell RNA sequencing data.                    | 2018 | ✅       |
+| BackBone                | Model         | Algorithm                                                                                                    | Year | CheckIn |
+| ----------------------- | ------------- | ------------------------------------------------------------------------------------------------------------ | ---- | ------- |
+| GNN                     | ScDeepsort    | Single-cell transcriptomics with weighted GNN                                                                | 2021 | ✅       |
+| Logistic Regression     | Celltypist    | Automated cell type annotation for scRNA-seq datasets                                                        | 2021 | ✅       |
+| Random Forest           | singleCellNet | SingleCellNet: a computational tool to classify single cell RNA-Seq data across platforms and across species | 2019 | ✅       |
+| Neural Network          | ACTINN        | ACTINN: automated identification of cell types in single cell RNA sequencing.                                | 2020 | ✅       |
+| Hierarchical Clustering | SingleR       | Reference-based analysis of lung single-cell sequencing reveals a transitional profibrotic macrophage.       | 2019 | P1      |
+| SVM                     | SVM           | A comparison of automatic cell identification methods for single-cell RNA sequencing data.                   | 2018 | ✅       |
 
 | Model         | Evaluation Metric | Mouse Brain 2695 (current/reported) | Mouse Spleen 1759 (current/reported) | Mouse Kidney 203 (current/reported) |
 | ------------- | ----------------- | ----------------------------------- | ------------------------------------ | ----------------------------------- |
-| scDeepsort    | ACC               | 0.542/0.363                         | 0.969/0.965                          | 0.847/0.911                         |
-| Celltypist    | ACC               | 0.824/0.666                         | 0.908/0.848                          | 0.823/0.832                         |
+| scDeepsort    | ACC               | 0.363/0.363                         | 0.965 /0.965                         | 0.901/0.911                         |
+| Celltypist\*  | ACC               | 0.680/0.666                         | 0.966/0.848                          | 0.879/0.832                         |
 | singleCellNet | ACC               | 0.693/0.803                         | 0.975/0.975                          | 0.795/0.842                         |
-| ACTINN        | ACC               | 0.727/0.778                         | 0.657/0.236                          | 0.762/0.798                         |
+| ACTINN        | ACC               | 0.860/0.778                         | 0.516/0.236                          | 0.829/0.798                         |
 | SVM           | ACC               | 0.683/0.683                         | 0.056/0.049                          | 0.704/0.695                         |
 
+Note: * Benchmark datasets were renormalied before running the original implementation of Celltypist to match its form requirements.
+
 #### 3）Clustering
 
 | BackBone    | Model         | Algorithm                                                                                                    | Year | CheckIn |
 | ----------- | ------------- | ------------------------------------------------------------------------------------------------------------ | ---- | ------- |
 | GNN         | graph-sc      | GNN-based embedding for clustering scRNA-seq data                                                            | 2022 | ✅       |
 | GNN         | scTAG         | ZINB-based Graph Embedding Autoencoder for Single-cell RNA-seq Interpretations                               | 2022 | ✅       |
 | GNN         | scDSC         | Deep structural clustering for single-cell RNA-seq data jointly through autoencoder and graph neural network | 2022 | ✅       |
@@ -259,24 +215,25 @@
 
 | Model         | Evaluation Metric | 10x PBMC (current/reported) | Mouse ES (current/reported) | Worm Neuron (current/reported) | Mouse Bladder (current/reported) |
 | ------------- | ----------------- | --------------------------- | --------------------------- | ------------------------------ | -------------------------------- |
 | graph-sc      | ARI               | 0.72 / 0.70                 | 0.82 / 0.78                 | 0.57 / 0.46                    | 0.68 / 0.63                      |
 | scDCC         | ARI               | 0.82 / 0.81                 | 0.98 / N/A                  | 0.51 / 0.58                    | 0.60 / 0.66                      |
 | scDeepCluster | ARI               | 0.81 / 0.78                 | 0.98 / 0.97                 | 0.51 / 0.52                    | 0.56 / 0.58                      |
 | scDSC         | ARI               | 0.72 / 0.78                 | 0.84 / N/A                  | 0.46 / 0.65                    | 0.65 / 0.72                      |
-| scTAG         | ARI               | 0.77 / N/A                  | 0.96 / N/A                  | 0.49 / N/A                     | 0.69 / N/A                       |
+| scTAG         | ARI               | 0.75 / N/A                  | 0.96 / N/A                  | 0.53 / N/A                     | 0.60 / N/A                       |
 
 ### Multimodality Module
 
 #### 1）Modality Prediction
 
 | BackBone         | Model                    | Algorithm                                                                                          | Year | CheckIn |
 | ---------------- | ------------------------ | -------------------------------------------------------------------------------------------------- | ---- | ------- |
 | GNN              | ScMoGCN                  | Graph Neural Networks for Multimodal Single-Cell Data Integration                                  | 2022 | ✅       |
 | GNN              | ScMoLP                   | Link Prediction Variant of ScMoGCN                                                                 | 2022 | P1      |
+| GNN              | scGNN                    | scGNN is a novel graph neural network framework for single-cell RNA-Seq analyses                   | 2021 | P1      |
 | GNN              | GRAPE                    | Handling Missing Data with Graph Representation Learning                                           | 2020 | P1      |
 | Generative Model | SCMM                     | SCMM: MIXTURE-OF-EXPERTS MULTIMODAL DEEP GENERATIVE MODEL FOR SINGLE-CELL MULTIOMICS DATA ANALYSIS | 2021 | ✅       |
 | Auto-encoder     | Cross-modal autoencoders | Multi-domain translation between single-cell imaging and sequencing data using autoencoders        | 2021 | ✅       |
 | Auto-encoder     | BABEL                    | BABEL enables cross-modality translation between multiomic profiles at single-cell resolution      | 2021 | ✅       |
 
 | Model                    | Evaluation Metric | GEX2ADT (current/reported) | ADT2GEX (current/reported) | GEX2ATAC (current/reported) | ATAC2GEX (current/reported) |
 | ------------------------ | ----------------- | -------------------------- | -------------------------- | --------------------------- | --------------------------- |
@@ -286,15 +243,15 @@
 | BABEL                    | RMSE              | 0.4335 / N/A               | 0.3673 / N/A               | 0.1816 / N/A                | 0.2394 / N/A                |
 
 #### 2) Modality Matching
 
 | BackBone         | Model                    | Algorithm                                                                                          | Year | CheckIn |
 | ---------------- | ------------------------ | -------------------------------------------------------------------------------------------------- | ---- | ------- |
 | GNN              | ScMoGCN                  | Graph Neural Networks for Multimodal Single-Cell Data Integration                                  | 2022 | ✅       |
-| GNN/Auto-ecnoder | GLUE                     | Multi-omics single-cell data integration and regulatory inference with graph-linked embedding      | 2021 | P1      |
+| GNN              | scGNN                    | scGNN is a novel graph neural network framework for single-cell RNA-Seq analyses                   | 2021 | P1      |
 | Generative Model | SCMM                     | SCMM: MIXTURE-OF-EXPERTS MULTIMODAL DEEP GENERATIVE MODEL FOR SINGLE-CELL MULTIOMICS DATA ANALYSIS | 2021 | ✅       |
 | Auto-encoder     | Cross-modal autoencoders | Multi-domain translation between single-cell imaging and sequencing data using autoencoders        | 2021 | ✅       |
 
 | Model                    | Evaluation Metric | GEX2ADT (current/reported) | GEX2ATAC (current/reported) |
 | ------------------------ | ----------------- | -------------------------- | --------------------------- |
 | ScMoGCN                  | Accuracy          | 0.0827 / 0.0810            | 0.0600 / 0.0630             |
 | SCMM                     | Accuracy          | 0.005 / N/A                | 5e-5 / N/A                  |
@@ -364,13 +321,47 @@
 | GNN                        | DSTG         | DSTG: deconvoluting spatial transcriptomics data through graph-based artificial intelligence                  | 2021 | ✅       |
 | logNormReg                 | SpatialDecon | Advances in mixed cell deconvolution enable quantification of cell types in spatial transcriptomic data       | 2022 | ✅       |
 | NNMFreg                    | SPOTlight    | SPOTlight: seeded NMF regression to deconvolute spatial transcriptomics spots with single-cell transcriptomes | 2021 | ✅       |
 | NN Linear + CAR assumption | CARD         | Spatially informed cell-type deconvolution for spatial transcriptomics                                        | 2022 | ✅       |
 
 | Model        | Evaluation Metric | GSE174746 (current/reported) | CARD Synthetic (current/reported) | SPOTlight Synthetic (current/reported) |
 | ------------ | ----------------- | ---------------------------- | --------------------------------- | -------------------------------------- |
-| DSTG         | MSE               | .1722 / N/A                  | .0239 / N/A                       | .0315 / N/A                            |
+| DSTG         | MSE               | .172 / N/A                   | .0247 / N/A                       | .042 / N/A                             |
 | SpatialDecon | MSE               | .0014 / .009                 | .0077 / N/A                       | .0055 / N/A                            |
 | SPOTlight    | MSE               | .0098 / N/A                  | .0246 / 0.118                     | .0109 / .16                            |
 | CARD         | MSE               | .0012 / N/A                  | .0078 / 0.0062                    | .0076 / N/A                            |
 
+## Dev notes
+
+### Dev installation
+
+Install PyDANCE with extra dependencies for dev
+
+```bash
+pip install -e ."[dev]"
+```
+
+Make sure dependencies have specific pinned versions
 
+```bash
+pip install -r requirements.txt
+```
+
+Install pre-commit hooks for code quality checks
+
+```bash
+pre-commit install
+```
+
+### Run tests
+
+Run all tests on current environment using pytest
+
+```bash
+pytest -v
+```
+
+Run full test from the ground up including environment set up using [tox](https://tox.wiki/en/latest/) on CPU
+
+```bash
+tox -e python3.8-cpu
+```
```

### Comparing `pydance-1.0.0/pydance.egg-info/SOURCES.txt` & `pydance-1.0.0rc0/pydance.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,18 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 dance/__init__.py
-dance/config.py
-dance/exceptions.py
-dance/registers.py
-dance/typing.py
 dance/data/__init__.py
-dance/data/base.py
 dance/datasets/__init__.py
-dance/datasets/base.py
 dance/datasets/multimodality.py
 dance/datasets/singlemodality.py
 dance/datasets/spatial.py
-dance/models/__init__.py
-dance/models/nn/__init__.py
-dance/models/nn/gnn.py
-dance/models/nn/mlp.py
 dance/modules/__init__.py
-dance/modules/base.py
 dance/modules/multi_modality/__init__.py
 dance/modules/multi_modality/joint_embedding/__init__.py
 dance/modules/multi_modality/joint_embedding/dcca.py
 dance/modules/multi_modality/joint_embedding/jae.py
 dance/modules/multi_modality/joint_embedding/scmogcn.py
 dance/modules/multi_modality/joint_embedding/scmogcnv2.py
 dance/modules/multi_modality/joint_embedding/scmvae.py
@@ -48,55 +37,31 @@
 dance/modules/single_modality/clustering/scdcc.py
 dance/modules/single_modality/clustering/scdeepcluster.py
 dance/modules/single_modality/clustering/scdsc.py
 dance/modules/single_modality/clustering/sctag.py
 dance/modules/single_modality/imputation/__init__.py
 dance/modules/single_modality/imputation/deepimpute.py
 dance/modules/single_modality/imputation/graphsci.py
-dance/modules/single_modality/imputation/scgnn2.py
+dance/modules/single_modality/imputation/scgnn.py
 dance/modules/spatial/__init__.py
 dance/modules/spatial/cell_type_deconvo/__init__.py
 dance/modules/spatial/cell_type_deconvo/card.py
 dance/modules/spatial/cell_type_deconvo/dstg.py
 dance/modules/spatial/cell_type_deconvo/spatialdecon.py
 dance/modules/spatial/cell_type_deconvo/spotlight.py
 dance/modules/spatial/spatial_domain/__init__.py
 dance/modules/spatial/spatial_domain/louvain.py
 dance/modules/spatial/spatial_domain/spagcn.py
 dance/modules/spatial/spatial_domain/stagate.py
 dance/modules/spatial/spatial_domain/stlearn.py
 dance/plotting/__init__.py
 dance/transforms/__init__.py
-dance/transforms/base.py
-dance/transforms/cell_feature.py
-dance/transforms/filter.py
-dance/transforms/gene_holdout.py
 dance/transforms/graph_construct.py
-dance/transforms/interface.py
-dance/transforms/mask.py
-dance/transforms/misc.py
-dance/transforms/normalize.py
 dance/transforms/preprocess.py
-dance/transforms/pseudo_gen.py
-dance/transforms/scn_feature.py
-dance/transforms/spatial_feature.py
-dance/transforms/stats.py
-dance/transforms/graph/__init__.py
-dance/transforms/graph/cell_feature_graph.py
-dance/transforms/graph/dstg_graph.py
-dance/transforms/graph/feature_feature_graph.py
-dance/transforms/graph/neighbor_graph.py
-dance/transforms/graph/scmogcn_graph.py
-dance/transforms/graph/spatial_graph.py
 dance/utils/__init__.py
-dance/utils/deprecate.py
-dance/utils/download.py
 dance/utils/loss.py
-dance/utils/matrix.py
 dance/utils/metrics.py
-dance/utils/preprocess.py
-dance/utils/wrappers.py
 pydance.egg-info/PKG-INFO
 pydance.egg-info/SOURCES.txt
 pydance.egg-info/dependency_links.txt
 pydance.egg-info/requires.txt
 pydance.egg-info/top_level.txt
```

### Comparing `pydance-1.0.0/pyproject.toml` & `pydance-1.0.0rc0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,14 @@
 
 [tool.yapf]
 based_on_style = "pep8"
 blank_line_before_nested_class_or_def = true
 column_limit = 120
 split_before_named_assigns = false
 
-[tool.docformatter]
-wrap-summaries = 88
-wrap-descriptions = 88
-in-place = true
-blank = true
-
 [tool.pytest.ini_options]
 addopts = [
     "--strict-markers",
     "-m",
     "not full_test",
 ]
 markers = [
```

### Comparing `pydance-1.0.0/setup.cfg` & `pydance-1.0.0rc0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,65 @@
 [metadata]
 name = pydance
-version = 1.0.0
+version = 1.0.0-rc
 description = Deep Learning for Single-cell Analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = "DANCE Team"
 author_email = "danceteamgnn@gmail.com"
 url = https://github.com/OmicsML/dance
 license_files = file: LICENSE.md
 license = BSD 2-Clause License
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
+	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 keywords = 
 	Single-cell Biology
 	Deep Learning
 	Graph Neural Networks
 
 [options]
 install_requires = 
 	h5py
 	leidenalg
-	mudata
 	networkx
 	numba
 	numpy
 	opencv-python
 	openpyxl
 	pandas
-	pyro-ppl
+	psutil>=5.8.0
 	python-igraph
+	rdata
 	requests
 	scanpy
+	scanpy
 	scikit-learn
 	scikit-misc
 	scipy
+	seaborn
+	skorch
 	statsmodels
 	tables
-	threadpoolctl>=3.1.0  # https://github.com/scikit-learn/scikit-learn/issues/24238
 	tqdm
 zip_save = false
 include_package_data = true
-python_requires = >=3.8
+python_requires = >=3.6
 packages = find:
 
 [options.extras_require]
 dev = 
-	pre-commit==3.3.3
-	pytest-subtests==0.11.0
-	pytest-xdist==3.3.1
-	pytest==7.4.0
-	tox==4.6.3
-doc = 
-	sphinx
-	sphinx-autodoc-typehints
-	sphinx_rtd_theme
-	sphinxcontrib-napoleon
+	pre-commit
+	pytest
+	pytest-xdist
+	tox
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

