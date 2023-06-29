# Comparing `tmp/kgtk-1.5.3.tar.gz` & `tmp/kgtk-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgtk-1.5.3.tar", last modified: Thu Mar  9 18:50:46 2023, max compression
+gzip compressed data, was "kgtk-1.5.4.tar", last modified: Thu Jun 29 20:05:56 2023, max compression
```

## Comparing `kgtk-1.5.3.tar` & `kgtk-1.5.4.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.362993 kgtk-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-09 18:50:35.000000 kgtk-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-09 18:50:35.000000 kgtk-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-09 18:50:46.362993 kgtk-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-03-09 18:50:35.000000 kgtk-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.326991 kgtk-1.5.3/kgtk/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.338992 kgtk-1.5.3/kgtk/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/__dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/__ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/add_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/build-kgtk-search-input.py
--rw-r--r--   0 runner    (1001) docker     (123)   125757 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/calc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/clean_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/community-detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/connected-components.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/convert-embeddings-format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/explode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/export_gt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/export_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/export_wikidata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/extract_wikidata_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/generate_mediawiki_jsons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/generate_wikidata_triples.py
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/graph_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/graph_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/ifempty.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/ifexists.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/ifnotempty.py
--rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/ifnotexists.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/implode.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/import_atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/import_concept_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/import_conceptnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/import_framenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/import_ntriples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/import_visualgenome.py
--rw-r--r--   0 runner    (1001) docker     (123)   127929 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/import_wikidata.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/import_wordnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/join.py
--rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/lexicalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    27180 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/lift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/md.py
--rw-r--r--   0 runner    (1001) docker     (123)    26511 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/normalize_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/reachable_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/remove_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/rename_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/reorder_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/replace-nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    32814 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/unreify_rdf_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/unreify_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/validate-properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/visualize-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli/zconcat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/cli_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/configure_kgtk_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.338992 kgtk-1.5.3/kgtk/exports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33612 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/exports/exportwikidata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/files_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    59342 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.338992 kgtk-1.5.3/kgtk/graph_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/graph_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/graph_analysis/community_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/graph_analysis/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    29479 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/graph_analysis/reachable_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/graph_analysis/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.342992 kgtk-1.5.3/kgtk/graph_embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/graph_embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/graph_embeddings/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/graph_embeddings/export_to_tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17168 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/graph_embeddings/graph_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/graph_embeddings/importers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.342992 kgtk-1.5.3/kgtk/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/gt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/gt/analysis_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/gt/connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/gt/embedding_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/gt/gt_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/gt/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34539 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/gt/lexicalize_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/gt/topology_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.342992 kgtk-1.5.3/kgtk/iff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/iff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/iff/kgtkifempty.py
--rw-r--r--   0 runner    (1001) docker     (123)    59662 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/iff/kgtkifexists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.342992 kgtk-1.5.3/kgtk/imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/imports/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/imports/conceptnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/imports/conceptnetpairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/imports/framenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    58127 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/imports/kgtkntriples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/imports/visualgenome.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/imports/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.346992 kgtk-1.5.3/kgtk/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/io/edgereader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/io/fastreader.py
--rw-r--r--   0 runner    (1001) docker     (123)    41446 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/io/graphcacheadaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/io/kgtkbase.py
--rw-r--r--   0 runner    (1001) docker     (123)   114411 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/io/kgtkreader.py
--rw-r--r--   0 runner    (1001) docker     (123)    77640 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/io/kgtkwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/io/nodereader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.346992 kgtk-1.5.3/kgtk/join/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/join/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24558 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/join/kgtkcat.py
--rw-r--r--   0 runner    (1001) docker     (123)    24021 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/join/kgtkjoiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-03-09 18:50:35.000000 kgtk-1.5.3/kgtk/join/kgtkmergecolumns.py
--rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/join/unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kgtkformat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.346992 kgtk-1.5.3/kgtk/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/knowledge_graph/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/knowledge_graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/knowledge_graph/knowledge_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/knowledge_graph/namespacemanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/knowledge_graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/knowledge_graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/knowledge_graph/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/knowledge_graph/shacl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/knowledge_graph/subject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.350992 kgtk-1.5.3/kgtk/kypher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50229 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/funccore.py
--rw-r--r--   0 runner    (1001) docker     (123)    15495 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/funclit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/funcmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    61681 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/funcvec.py
--rw-r--r--   0 runner    (1001) docker     (123)    16747 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)   301236 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/grammar_compiled.py
--rw-r--r--   0 runner    (1001) docker     (123)    39478 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/indexspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/infotable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/kgtkinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    32939 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    82773 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    88942 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/sqlstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    80943 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/kypher/vecstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.350992 kgtk-1.5.3/kgtk/lift/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/lift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    74797 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/lift/kgtklift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/nomalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.350992 kgtk-1.5.3/kgtk/reshape/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/reshape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/reshape/kgtkcompact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/reshape/kgtkexpand.py
--rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/reshape/kgtkexplode.py
--rw-r--r--   0 runner    (1001) docker     (123)    30966 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/reshape/kgtkidbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)    43827 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/reshape/kgtkimplode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.350992 kgtk-1.5.3/kgtk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/templates/kgtkcopytemplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.354992 kgtk-1.5.3/kgtk/unreify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/unreify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/unreify/kgtksortbuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30385 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/unreify/kgtkunreifyrdfstatements.py
--rw-r--r--   0 runner    (1001) docker     (123)    27956 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/unreify/kgtkunreifyvalues.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.354992 kgtk-1.5.3/kgtk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/argparsehelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/cats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/closableiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/color_styles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/convert_embeddings_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    49317 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/elasticsearch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/enumnameaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    67854 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/gzipprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/remove_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/reorder_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/replace_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    30443 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/update_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/updateversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/utils/validationaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.358992 kgtk-1.5.3/kgtk/value/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92436 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/value/kgtkvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)    25803 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/value/kgtkvalueoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/value/languagevalidator.py
--rw-r--r--   0 runner    (1001) docker     (123)   124097 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/value/propertypatternvalidator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.358992 kgtk-1.5.3/kgtk/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30535 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/visualize/visualize_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.358992 kgtk-1.5.3/kgtk/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/wikidata/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/wikidata/statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/wikidata/truthy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-03-09 18:50:36.000000 kgtk-1.5.3/kgtk/wikidata/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.326991 kgtk-1.5.3/kgtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-09 18:50:46.000000 kgtk-1.5.3/kgtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-03-09 18:50:46.000000 kgtk-1.5.3/kgtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 18:50:46.000000 kgtk-1.5.3/kgtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-09 18:50:46.000000 kgtk-1.5.3/kgtk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-09 18:50:46.000000 kgtk-1.5.3/kgtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-09 18:50:46.000000 kgtk-1.5.3/kgtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-09 18:50:36.000000 kgtk-1.5.3/requirements-full.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-09 18:50:36.000000 kgtk-1.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 18:50:46.362993 kgtk-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-03-09 18:50:36.000000 kgtk-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:46.362993 kgtk-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/__test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/depr_export_gt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_1graph_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_add_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_convert_embeddings_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_graph_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_import_atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_import_concept_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_import_conceptnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_import_framenet.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_import_visualgenome.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_import_wordnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_json_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_kgtk_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_kgtk_ifexists.py
--rw-r--r--   0 runner    (1001) docker     (123)   102141 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_kgtk_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_kgtk_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_normalize_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_triple_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-03-09 18:50:36.000000 kgtk-1.5.3/tests/test_visualize_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.180860 kgtk-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-29 20:05:41.000000 kgtk-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-29 20:05:41.000000 kgtk-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-29 20:05:56.180860 kgtk-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-29 20:05:41.000000 kgtk-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.156860 kgtk-1.5.4/kgtk/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.164860 kgtk-1.5.4/kgtk/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/__dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/__ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/add_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/build-kgtk-search-input.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126825 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/clean_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/community-detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/connected-components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/convert-embeddings-format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/explode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/export_gt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/export_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/export_wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/extract_wikidata_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/generate_mediawiki_jsons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/generate_wikidata_triples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/graph_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/graph_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/ifempty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/ifexists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/ifnotempty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/ifnotexists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/implode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/import_atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/import_concept_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/import_conceptnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/import_framenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/import_ntriples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/import_visualgenome.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127929 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/import_wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/import_wordnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/lexicalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27180 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/lift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26511 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/normalize_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/reachable_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/remove_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/rename_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/reorder_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/replace-nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32814 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/unreify_rdf_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/unreify_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/validate-properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/visualize-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli/zconcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/cli_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/configure_kgtk_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.164860 kgtk-1.5.4/kgtk/exports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33612 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/exports/exportwikidata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/files_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59342 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.164860 kgtk-1.5.4/kgtk/graph_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/graph_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/graph_analysis/community_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/graph_analysis/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29479 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/graph_analysis/reachable_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/graph_analysis/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.164860 kgtk-1.5.4/kgtk/graph_embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/graph_embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/graph_embeddings/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/graph_embeddings/export_to_tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17168 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/graph_embeddings/graph_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/graph_embeddings/importers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.164860 kgtk-1.5.4/kgtk/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/gt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/gt/analysis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/gt/connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/gt/embedding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/gt/gt_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/gt/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34539 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/gt/lexicalize_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/gt/topology_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.164860 kgtk-1.5.4/kgtk/iff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/iff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/iff/kgtkifempty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59662 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/iff/kgtkifexists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.168860 kgtk-1.5.4/kgtk/imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/imports/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/imports/conceptnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/imports/conceptnetpairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/imports/framenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58127 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/imports/kgtkntriples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/imports/visualgenome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/imports/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.168860 kgtk-1.5.4/kgtk/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/io/edgereader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/io/fastreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41446 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/io/graphcacheadaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/io/kgtkbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114411 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/io/kgtkreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77640 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/io/kgtkwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/io/nodereader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.168860 kgtk-1.5.4/kgtk/join/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/join/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24558 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/join/kgtkcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24021 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/join/kgtkjoiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-29 20:05:41.000000 kgtk-1.5.4/kgtk/join/kgtkmergecolumns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/join/unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kgtkformat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.168860 kgtk-1.5.4/kgtk/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/knowledge_graph/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/knowledge_graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/knowledge_graph/knowledge_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/knowledge_graph/namespacemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/knowledge_graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/knowledge_graph/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/knowledge_graph/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/knowledge_graph/shacl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/knowledge_graph/subject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.172860 kgtk-1.5.4/kgtk/kypher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50229 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/funccore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15495 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/funclit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/funcmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61681 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/funcvec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16747 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   301236 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/grammar_compiled.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39478 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/indexspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/infotable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/kgtkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32939 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82773 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88942 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/sqlstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80943 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/kypher/vecstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.172860 kgtk-1.5.4/kgtk/lift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/lift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74797 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/lift/kgtklift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/nomalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.172860 kgtk-1.5.4/kgtk/reshape/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/reshape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/reshape/kgtkcompact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/reshape/kgtkexpand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/reshape/kgtkexplode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30966 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/reshape/kgtkidbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43827 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/reshape/kgtkimplode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.172860 kgtk-1.5.4/kgtk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/templates/kgtkcopytemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.172860 kgtk-1.5.4/kgtk/unreify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/unreify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/unreify/kgtksortbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30385 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/unreify/kgtkunreifyrdfstatements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27956 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/unreify/kgtkunreifyvalues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.176860 kgtk-1.5.4/kgtk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/argparsehelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/cats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/closableiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/color_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/convert_embeddings_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49317 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/elasticsearch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/enumnameaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67854 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/gzipprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/remove_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/reorder_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/replace_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30443 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/update_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/updateversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/utils/validationaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.176860 kgtk-1.5.4/kgtk/value/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92436 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/value/kgtkvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25803 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/value/kgtkvalueoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/value/languagevalidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124097 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/value/propertypatternvalidator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.176860 kgtk-1.5.4/kgtk/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30535 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/visualize/visualize_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.176860 kgtk-1.5.4/kgtk/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/wikidata/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/wikidata/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/wikidata/truthy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-06-29 20:05:42.000000 kgtk-1.5.4/kgtk/wikidata/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.156860 kgtk-1.5.4/kgtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-29 20:05:56.000000 kgtk-1.5.4/kgtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-29 20:05:56.000000 kgtk-1.5.4/kgtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:05:56.000000 kgtk-1.5.4/kgtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 20:05:56.000000 kgtk-1.5.4/kgtk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 20:05:56.000000 kgtk-1.5.4/kgtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 20:05:56.000000 kgtk-1.5.4/kgtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-29 20:05:42.000000 kgtk-1.5.4/requirements-full.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-29 20:05:42.000000 kgtk-1.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:05:56.180860 kgtk-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-29 20:05:42.000000 kgtk-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:56.180860 kgtk-1.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/__test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/depr_export_gt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_1graph_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_add_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_convert_embeddings_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_graph_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_import_atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_import_concept_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_import_conceptnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_import_framenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_import_visualgenome.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_import_wordnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_json_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_kgtk_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_kgtk_ifexists.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102141 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_kgtk_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_kgtk_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_normalize_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_triple_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-06-29 20:05:42.000000 kgtk-1.5.4/tests/test_visualize_graph.py
```

### Comparing `kgtk-1.5.3/LICENSE` & `kgtk-1.5.4/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
- MIT License
+MIT License
 
 Copyright (c) 2017 University of Southern California
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `kgtk-1.5.3/README.md` & `kgtk-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/__dummy.py` & `kgtk-1.5.4/kgtk/cli/__dummy.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/__ticker.py` & `kgtk-1.5.4/kgtk/cli/__ticker.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/add_id.py` & `kgtk-1.5.4/kgtk/cli/add_id.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/build-kgtk-search-input.py` & `kgtk-1.5.4/kgtk/cli/build-kgtk-search-input.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/calc.py` & `kgtk-1.5.4/kgtk/cli/calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 AVERAGE_OP: str = "average"
 DIV_OP: str = "div" # (column / column) or (column / value)
 LIST_SUM_OP: str = "list_sum" # column
 MAX_OP: str = "max"
 MIN_OP: str = "min"
 MINUS_OP: str = "minus" # (column1 - column2) or (column - value)
 MOD_OP: str = "mod" # (column mod column) or (column mod value)
+MULTIPLY_OP: str = "multiply" # (column x column) or (column x value)
 NEGATE_OP: str = "negate" # (column, ...)
 NUMBER_OP: str = "number" # Get a number or the numeric part of a quantity.
 PERCENTAGE_OP: str = "percentage"
 RANDOM_OP: str = "random"
 RANDINT_OP: str = "randint"
 RANDRANGE_OP: str = "randrange"
 REVERSE_DIV_OP: str = "reverse_div" # (column2 / column1) or (column / value)
@@ -1851,14 +1852,35 @@
                 if len(sources) == 2:
                     output_row[into_column_idx] = str(float(row[sources[0]]) % float(row[sources[1]]))
                 else:
                     output_row[into_column_idx] = str(float(row[sources[0]]) % float(values[0]))
                 return True
             opfunc = mod_op
 
+        elif operation == MULTIPLY_OP:
+            if not ((len(sources) == 2 and len(values) == 0) or (len(sources) == 1 and len(values) == 1)):
+                raise KGTKException("Multiply needs two sources or one source and one value, got %d sources and %d values" % (len(sources), len(values)))
+            if len(into_column_idxs) != 1:
+                raise KGTKException("Multiply needs 1 destination columns, got %d" % len(into_column_idxs))
+
+            def multiply_2_op()->bool:
+                # TODO: support quantities.
+                output_row[into_column_idx] = str(float(row[sources[0]]) * float(row[sources[1]]))
+                return True
+
+            def multiply_1op()->bool:
+                # TODO: support quantities.
+                output_row[into_column_idx] = str(float(row[sources[0]]) * float(values[0]))
+                return True
+
+            if len(sources) == 2:
+                opfunc = multiply_2_op
+            else:
+                opfunc = multiply_1_op
+
         elif operation == NAND_OP:
             if len(sources) == 0:
                 raise KGTKException("Nand needs at least one source, got %d" % len(sources))
             if filter:
                 if len(into_column_idxs) > 1:
                     raise KGTKException("Nand needs at most 1 destination column, got %d" % len(into_column_idxs))
             else:
```

### Comparing `kgtk-1.5.3/kgtk/cli/cat.py` & `kgtk-1.5.4/kgtk/cli/cat.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/clean_data.py` & `kgtk-1.5.4/kgtk/cli/clean_data.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/community-detection.py` & `kgtk-1.5.4/kgtk/cli/community-detection.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/compact.py` & `kgtk-1.5.4/kgtk/cli/compact.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/connected-components.py` & `kgtk-1.5.4/kgtk/cli/connected-components.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/convert-embeddings-format.py` & `kgtk-1.5.4/kgtk/cli/convert-embeddings-format.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/count.py` & `kgtk-1.5.4/kgtk/cli/count.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/expand.py` & `kgtk-1.5.4/kgtk/cli/expand.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/explode.py` & `kgtk-1.5.4/kgtk/cli/explode.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/export_gt.py` & `kgtk-1.5.4/kgtk/cli/export_gt.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/export_neo4j.py` & `kgtk-1.5.4/kgtk/cli/export_neo4j.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/export_wikidata.py` & `kgtk-1.5.4/kgtk/cli/export_wikidata.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/extract_wikidata_json.py` & `kgtk-1.5.4/kgtk/cli/extract_wikidata_json.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/filter.py` & `kgtk-1.5.4/kgtk/cli/filter.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/generate_mediawiki_jsons.py` & `kgtk-1.5.4/kgtk/cli/generate_mediawiki_jsons.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/generate_wikidata_triples.py` & `kgtk-1.5.4/kgtk/cli/generate_wikidata_triples.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/graph_embeddings.py` & `kgtk-1.5.4/kgtk/cli/graph_embeddings.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/graph_statistics.py` & `kgtk-1.5.4/kgtk/cli/graph_statistics.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/head.py` & `kgtk-1.5.4/kgtk/cli/head.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/html.py` & `kgtk-1.5.4/kgtk/cli/html.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/ifempty.py` & `kgtk-1.5.4/kgtk/cli/ifempty.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/ifexists.py` & `kgtk-1.5.4/kgtk/cli/ifexists.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/ifnotempty.py` & `kgtk-1.5.4/kgtk/cli/ifnotempty.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/ifnotexists.py` & `kgtk-1.5.4/kgtk/cli/ifnotexists.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/implode.py` & `kgtk-1.5.4/kgtk/cli/implode.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/import_atomic.py` & `kgtk-1.5.4/kgtk/cli/import_atomic.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/import_concept_pairs.py` & `kgtk-1.5.4/kgtk/cli/import_concept_pairs.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/import_conceptnet.py` & `kgtk-1.5.4/kgtk/cli/import_conceptnet.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/import_framenet.py` & `kgtk-1.5.4/kgtk/cli/import_framenet.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/import_ntriples.py` & `kgtk-1.5.4/kgtk/cli/import_ntriples.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/import_visualgenome.py` & `kgtk-1.5.4/kgtk/cli/import_visualgenome.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/import_wikidata.py` & `kgtk-1.5.4/kgtk/cli/import_wikidata.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/import_wordnet.py` & `kgtk-1.5.4/kgtk/cli/import_wordnet.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/join.py` & `kgtk-1.5.4/kgtk/cli/join.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/lexicalize.py` & `kgtk-1.5.4/kgtk/cli/lexicalize.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/lift.py` & `kgtk-1.5.4/kgtk/cli/lift.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/md.py` & `kgtk-1.5.4/kgtk/cli/md.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/normalize.py` & `kgtk-1.5.4/kgtk/cli/normalize.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/normalize_nodes.py` & `kgtk-1.5.4/kgtk/cli/normalize_nodes.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/paths.py` & `kgtk-1.5.4/kgtk/cli/paths.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/query.py` & `kgtk-1.5.4/kgtk/cli/query.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/reachable_nodes.py` & `kgtk-1.5.4/kgtk/cli/reachable_nodes.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/remove_columns.py` & `kgtk-1.5.4/kgtk/cli/remove_columns.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/rename_columns.py` & `kgtk-1.5.4/kgtk/cli/rename_columns.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/reorder_columns.py` & `kgtk-1.5.4/kgtk/cli/reorder_columns.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/replace-nodes.py` & `kgtk-1.5.4/kgtk/cli/replace-nodes.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/sample.py` & `kgtk-1.5.4/kgtk/cli/sample.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/sort.py` & `kgtk-1.5.4/kgtk/cli/sort.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/split.py` & `kgtk-1.5.4/kgtk/cli/split.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/table.py` & `kgtk-1.5.4/kgtk/cli/table.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/tail.py` & `kgtk-1.5.4/kgtk/cli/tail.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/tee.py` & `kgtk-1.5.4/kgtk/cli/tee.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/text_embedding.py` & `kgtk-1.5.4/kgtk/cli/text_embedding.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/unique.py` & `kgtk-1.5.4/kgtk/cli/unique.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/unreify_rdf_statements.py` & `kgtk-1.5.4/kgtk/cli/unreify_rdf_statements.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/unreify_values.py` & `kgtk-1.5.4/kgtk/cli/unreify_values.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/validate-properties.py` & `kgtk-1.5.4/kgtk/cli/validate-properties.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/validate.py` & `kgtk-1.5.4/kgtk/cli/validate.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/visualize-graph.py` & `kgtk-1.5.4/kgtk/cli/visualize-graph.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli/zconcat.py` & `kgtk-1.5.4/kgtk/cli/zconcat.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli_argparse.py` & `kgtk-1.5.4/kgtk/cli_argparse.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/cli_entry.py` & `kgtk-1.5.4/kgtk/cli_entry.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/configure_kgtk_notebooks.py` & `kgtk-1.5.4/kgtk/configure_kgtk_notebooks.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/dependencies.py` & `kgtk-1.5.4/kgtk/dependencies.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/exceptions.py` & `kgtk-1.5.4/kgtk/exceptions.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/exports/exportwikidata.py` & `kgtk-1.5.4/kgtk/exports/exportwikidata.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/files_config.py` & `kgtk-1.5.4/kgtk/files_config.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/functions.py` & `kgtk-1.5.4/kgtk/functions.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/generator.py` & `kgtk-1.5.4/kgtk/generator.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/graph_analysis/community_detection.py` & `kgtk-1.5.4/kgtk/graph_analysis/community_detection.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/graph_analysis/paths.py` & `kgtk-1.5.4/kgtk/graph_analysis/paths.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/graph_analysis/reachable_nodes.py` & `kgtk-1.5.4/kgtk/graph_analysis/reachable_nodes.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/graph_analysis/statistics.py` & `kgtk-1.5.4/kgtk/graph_analysis/statistics.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/graph_embeddings/export_to_tsv.py` & `kgtk-1.5.4/kgtk/graph_embeddings/export_to_tsv.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/graph_embeddings/graph_embeddings.py` & `kgtk-1.5.4/kgtk/graph_embeddings/graph_embeddings.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/graph_embeddings/importers.py` & `kgtk-1.5.4/kgtk/graph_embeddings/importers.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/gt/analysis_utils.py` & `kgtk-1.5.4/kgtk/gt/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/gt/connected_components.py` & `kgtk-1.5.4/kgtk/gt/connected_components.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/gt/embedding_utils.py` & `kgtk-1.5.4/kgtk/gt/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/gt/gt_load.py` & `kgtk-1.5.4/kgtk/gt/gt_load.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/gt/io_utils.py` & `kgtk-1.5.4/kgtk/gt/io_utils.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/gt/lexicalize_utils.py` & `kgtk-1.5.4/kgtk/gt/lexicalize_utils.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/gt/topology_utils.py` & `kgtk-1.5.4/kgtk/gt/topology_utils.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/iff/kgtkifempty.py` & `kgtk-1.5.4/kgtk/iff/kgtkifempty.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/iff/kgtkifexists.py` & `kgtk-1.5.4/kgtk/iff/kgtkifexists.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/imports/atomic.py` & `kgtk-1.5.4/kgtk/imports/atomic.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/imports/conceptnet.py` & `kgtk-1.5.4/kgtk/imports/conceptnet.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/imports/conceptnetpairs.py` & `kgtk-1.5.4/kgtk/imports/conceptnetpairs.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/imports/framenet.py` & `kgtk-1.5.4/kgtk/imports/framenet.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/imports/kgtkntriples.py` & `kgtk-1.5.4/kgtk/imports/kgtkntriples.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/imports/visualgenome.py` & `kgtk-1.5.4/kgtk/imports/visualgenome.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/imports/wordnet.py` & `kgtk-1.5.4/kgtk/imports/wordnet.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/io/edgereader.py` & `kgtk-1.5.4/kgtk/io/edgereader.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/io/fastreader.py` & `kgtk-1.5.4/kgtk/io/fastreader.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/io/graphcacheadaptor.py` & `kgtk-1.5.4/kgtk/io/graphcacheadaptor.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/io/kgtkbase.py` & `kgtk-1.5.4/kgtk/io/kgtkbase.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/io/kgtkreader.py` & `kgtk-1.5.4/kgtk/io/kgtkreader.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/io/kgtkwriter.py` & `kgtk-1.5.4/kgtk/io/kgtkwriter.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/io/nodereader.py` & `kgtk-1.5.4/kgtk/io/nodereader.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/join/kgtkcat.py` & `kgtk-1.5.4/kgtk/join/kgtkcat.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/join/kgtkjoiner.py` & `kgtk-1.5.4/kgtk/join/kgtkjoiner.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/join/kgtkmergecolumns.py` & `kgtk-1.5.4/kgtk/join/kgtkmergecolumns.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/join/unique.py` & `kgtk-1.5.4/kgtk/join/unique.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kgtkformat.py` & `kgtk-1.5.4/kgtk/kgtkformat.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/knowledge_graph/graph.py` & `kgtk-1.5.4/kgtk/knowledge_graph/graph.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/knowledge_graph/knowledge_graph.py` & `kgtk-1.5.4/kgtk/knowledge_graph/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/knowledge_graph/namespacemanager.py` & `kgtk-1.5.4/kgtk/knowledge_graph/namespacemanager.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/knowledge_graph/node.py` & `kgtk-1.5.4/kgtk/knowledge_graph/node.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/knowledge_graph/ontology.py` & `kgtk-1.5.4/kgtk/knowledge_graph/ontology.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/knowledge_graph/schema.py` & `kgtk-1.5.4/kgtk/knowledge_graph/schema.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/knowledge_graph/shacl.py` & `kgtk-1.5.4/kgtk/knowledge_graph/shacl.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/knowledge_graph/subject.py` & `kgtk-1.5.4/kgtk/knowledge_graph/subject.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/api.py` & `kgtk-1.5.4/kgtk/kypher/api.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/funccore.py` & `kgtk-1.5.4/kgtk/kypher/funccore.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/funclit.py` & `kgtk-1.5.4/kgtk/kypher/funclit.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/funcmath.py` & `kgtk-1.5.4/kgtk/kypher/funcmath.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/functions.py` & `kgtk-1.5.4/kgtk/kypher/functions.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/funcvec.py` & `kgtk-1.5.4/kgtk/kypher/funcvec.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/grammar.py` & `kgtk-1.5.4/kgtk/kypher/grammar.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/grammar_compiled.py` & `kgtk-1.5.4/kgtk/kypher/grammar_compiled.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/indexspec.py` & `kgtk-1.5.4/kgtk/kypher/indexspec.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/infotable.py` & `kgtk-1.5.4/kgtk/kypher/infotable.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/kgtkinfo.py` & `kgtk-1.5.4/kgtk/kypher/kgtkinfo.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/parser.py` & `kgtk-1.5.4/kgtk/kypher/parser.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/query.py` & `kgtk-1.5.4/kgtk/kypher/query.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/sqlstore.py` & `kgtk-1.5.4/kgtk/kypher/sqlstore.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/utils.py` & `kgtk-1.5.4/kgtk/kypher/utils.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/kypher/vecstore.py` & `kgtk-1.5.4/kgtk/kypher/vecstore.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/lift/kgtklift.py` & `kgtk-1.5.4/kgtk/lift/kgtklift.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/nomalizer.py` & `kgtk-1.5.4/kgtk/nomalizer.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/reshape/kgtkcompact.py` & `kgtk-1.5.4/kgtk/reshape/kgtkcompact.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/reshape/kgtkexpand.py` & `kgtk-1.5.4/kgtk/reshape/kgtkexpand.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/reshape/kgtkexplode.py` & `kgtk-1.5.4/kgtk/reshape/kgtkexplode.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/reshape/kgtkidbuilder.py` & `kgtk-1.5.4/kgtk/reshape/kgtkidbuilder.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/reshape/kgtkimplode.py` & `kgtk-1.5.4/kgtk/reshape/kgtkimplode.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/templates/kgtkcopytemplate.py` & `kgtk-1.5.4/kgtk/templates/kgtkcopytemplate.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/unreify/kgtksortbuffer.py` & `kgtk-1.5.4/kgtk/unreify/kgtksortbuffer.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/unreify/kgtkunreifyrdfstatements.py` & `kgtk-1.5.4/kgtk/unreify/kgtkunreifyrdfstatements.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/unreify/kgtkunreifyvalues.py` & `kgtk-1.5.4/kgtk/unreify/kgtkunreifyvalues.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/argparsehelpers.py` & `kgtk-1.5.4/kgtk/utils/argparsehelpers.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/cats.py` & `kgtk-1.5.4/kgtk/utils/cats.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/closableiter.py` & `kgtk-1.5.4/kgtk/utils/closableiter.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/color_styles.py` & `kgtk-1.5.4/kgtk/utils/color_styles.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/convert_embeddings_format.py` & `kgtk-1.5.4/kgtk/utils/convert_embeddings_format.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/elasticsearch_manager.py` & `kgtk-1.5.4/kgtk/utils/elasticsearch_manager.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/enumnameaction.py` & `kgtk-1.5.4/kgtk/utils/enumnameaction.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/filter.py` & `kgtk-1.5.4/kgtk/utils/filter.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/gzipprocess.py` & `kgtk-1.5.4/kgtk/utils/gzipprocess.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/head.py` & `kgtk-1.5.4/kgtk/utils/head.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/remove_columns.py` & `kgtk-1.5.4/kgtk/utils/remove_columns.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/reorder_columns.py` & `kgtk-1.5.4/kgtk/utils/reorder_columns.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/replace_nodes.py` & `kgtk-1.5.4/kgtk/utils/replace_nodes.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/update_documentation.py` & `kgtk-1.5.4/kgtk/utils/update_documentation.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/updateversion.py` & `kgtk-1.5.4/kgtk/utils/updateversion.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/utils/validationaction.py` & `kgtk-1.5.4/kgtk/utils/validationaction.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/value/kgtkvalue.py` & `kgtk-1.5.4/kgtk/value/kgtkvalue.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/value/kgtkvalueoptions.py` & `kgtk-1.5.4/kgtk/value/kgtkvalueoptions.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/value/languagevalidator.py` & `kgtk-1.5.4/kgtk/value/languagevalidator.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/value/propertypatternvalidator.py` & `kgtk-1.5.4/kgtk/value/propertypatternvalidator.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/visualize/visualize_api.py` & `kgtk-1.5.4/kgtk/visualize/visualize_api.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/wikidata/__init__.py` & `kgtk-1.5.4/kgtk/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/wikidata/entity.py` & `kgtk-1.5.4/kgtk/wikidata/entity.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/wikidata/statement.py` & `kgtk-1.5.4/kgtk/wikidata/statement.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/wikidata/truthy.py` & `kgtk-1.5.4/kgtk/wikidata/truthy.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk/wikidata/value.py` & `kgtk-1.5.4/kgtk/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/kgtk.egg-info/SOURCES.txt` & `kgtk-1.5.4/kgtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/setup.py` & `kgtk-1.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/__test_dummy.py` & `kgtk-1.5.4/tests/__test_dummy.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/depr_export_gt.py` & `kgtk-1.5.4/tests/depr_export_gt.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_1graph_statistics.py` & `kgtk-1.5.4/tests/test_1graph_statistics.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_add_id.py` & `kgtk-1.5.4/tests/test_add_id.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_cat.py` & `kgtk-1.5.4/tests/test_cat.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_convert_embeddings_format.py` & `kgtk-1.5.4/tests/test_convert_embeddings_format.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_embedding.py` & `kgtk-1.5.4/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_graph_embeddings.py` & `kgtk-1.5.4/tests/test_graph_embeddings.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_import_atomic.py` & `kgtk-1.5.4/tests/test_import_atomic.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_import_concept_pairs.py` & `kgtk-1.5.4/tests/test_import_concept_pairs.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_import_conceptnet.py` & `kgtk-1.5.4/tests/test_import_conceptnet.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_import_framenet.py` & `kgtk-1.5.4/tests/test_import_framenet.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_import_visualgenome.py` & `kgtk-1.5.4/tests/test_import_visualgenome.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_import_wordnet.py` & `kgtk-1.5.4/tests/test_import_wordnet.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_json_generation.py` & `kgtk-1.5.4/tests/test_json_generation.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_kgtk_filter.py` & `kgtk-1.5.4/tests/test_kgtk_filter.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_kgtk_ifexists.py` & `kgtk-1.5.4/tests/test_kgtk_ifexists.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_kgtk_query.py` & `kgtk-1.5.4/tests/test_kgtk_query.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_kgtk_split.py` & `kgtk-1.5.4/tests/test_kgtk_split.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_normalize_nodes.py` & `kgtk-1.5.4/tests/test_normalize_nodes.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_triple_generation.py` & `kgtk-1.5.4/tests/test_triple_generation.py`

 * *Files identical despite different names*

### Comparing `kgtk-1.5.3/tests/test_visualize_graph.py` & `kgtk-1.5.4/tests/test_visualize_graph.py`

 * *Files identical despite different names*

