# Comparing `tmp/pimmi-0.2.0.tar.gz` & `tmp/pimmi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pimmi-0.2.0.tar", last modified: Fri Feb  3 17:50:56 2023, max compression
+gzip compressed data, was "pimmi-0.3.0.tar", last modified: Thu Jun 29 15:57:42 2023, max compression
```

## Comparing `pimmi-0.2.0.tar` & `pimmi-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2023-02-03 17:50:56.000000 pimmi-0.2.0/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    35149 2022-10-06 07:59:34.000000 pimmi-0.2.0/LICENSE
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     6327 2023-02-03 17:50:56.000000 pimmi-0.2.0/PKG-INFO
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     6041 2023-01-26 15:04:15.000000 pimmi-0.2.0/README.md
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2023-02-03 17:50:56.000000 pimmi-0.2.0/pimmi/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      329 2022-10-10 16:06:48.000000 pimmi-0.2.0/pimmi/__init__.py
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2023-02-03 17:50:56.000000 pimmi-0.2.0/pimmi/cli/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-10-06 07:59:34.000000 pimmi-0.2.0/pimmi/cli/__init__.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    14395 2023-02-03 15:42:25.000000 pimmi-0.2.0/pimmi/cli/__main__.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      461 2023-01-16 17:29:26.000000 pimmi-0.2.0/pimmi/cli/config.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     7016 2023-01-18 17:12:01.000000 pimmi-0.2.0/pimmi/cli/config.yml
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     5055 2023-02-03 17:31:03.000000 pimmi-0.2.0/pimmi/clusters.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     4113 2023-01-16 15:56:27.000000 pimmi-0.2.0/pimmi/eval.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    24628 2023-02-03 15:23:54.000000 pimmi-0.2.0/pimmi/pimmi.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     1591 2022-10-06 07:59:34.000000 pimmi-0.2.0/pimmi/pimmi_parameters.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      269 2023-01-27 13:33:39.000000 pimmi-0.2.0/pimmi/sift_create.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     2439 2023-01-16 17:36:59.000000 pimmi-0.2.0/pimmi/toolbox.py
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2023-02-03 17:50:56.000000 pimmi-0.2.0/pimmi.egg-info/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     6327 2023-02-03 17:50:56.000000 pimmi-0.2.0/pimmi.egg-info/PKG-INFO
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      532 2023-02-03 17:50:56.000000 pimmi-0.2.0/pimmi.egg-info/SOURCES.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        1 2023-02-03 17:50:56.000000 pimmi-0.2.0/pimmi.egg-info/dependency_links.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       50 2023-02-03 17:50:56.000000 pimmi-0.2.0/pimmi.egg-info/entry_points.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       88 2023-02-03 17:50:56.000000 pimmi-0.2.0/pimmi.egg-info/requires.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       11 2023-02-03 17:50:56.000000 pimmi-0.2.0/pimmi.egg-info/top_level.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        1 2022-10-06 08:02:42.000000 pimmi-0.2.0/pimmi.egg-info/zip-safe
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       38 2023-02-03 17:50:56.000000 pimmi-0.2.0/setup.cfg
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     1004 2023-02-03 17:47:31.000000 pimmi-0.2.0/setup.py
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2023-02-03 17:50:56.000000 pimmi-0.2.0/test/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-10-06 07:59:34.000000 pimmi-0.2.0/test/__init__.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     4096 2022-11-30 14:18:55.000000 pimmi-0.2.0/test/pipeline_test.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     1478 2022-10-06 07:59:34.000000 pimmi-0.2.0/test/sift_test.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      495 2022-10-06 07:59:34.000000 pimmi-0.2.0/test/toolbox_test.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     2587 2022-10-14 15:36:29.000000 pimmi-0.2.0/test/utils.py
+drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2023-06-29 15:57:42.573795 pimmi-0.3.0/
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    35149 2022-10-06 07:59:34.000000 pimmi-0.3.0/LICENSE
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     6322 2023-06-29 15:57:42.573795 pimmi-0.3.0/PKG-INFO
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     6041 2023-01-26 15:04:15.000000 pimmi-0.3.0/README.md
+drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2023-06-29 15:57:42.573795 pimmi-0.3.0/pimmi/
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      329 2022-10-10 16:06:48.000000 pimmi-0.3.0/pimmi/__init__.py
+drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2023-06-29 15:57:42.573795 pimmi-0.3.0/pimmi/cli/
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-10-06 07:59:34.000000 pimmi-0.3.0/pimmi/cli/__init__.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    14650 2023-06-09 12:49:36.000000 pimmi-0.3.0/pimmi/cli/__main__.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      461 2023-06-09 12:30:16.000000 pimmi-0.3.0/pimmi/cli/config.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     6756 2023-06-09 11:35:29.000000 pimmi-0.3.0/pimmi/cli/config.yml
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     5613 2023-06-09 12:29:52.000000 pimmi-0.3.0/pimmi/clusters.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     4113 2023-05-30 15:42:49.000000 pimmi-0.3.0/pimmi/eval.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    24012 2023-06-09 13:56:53.000000 pimmi-0.3.0/pimmi/pimmi.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     1591 2022-10-06 07:59:34.000000 pimmi-0.3.0/pimmi/pimmi_parameters.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      269 2023-01-27 13:33:39.000000 pimmi-0.3.0/pimmi/sift_create.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     2653 2023-06-22 13:26:52.000000 pimmi-0.3.0/pimmi/toolbox.py
+drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2023-06-29 15:57:42.573795 pimmi-0.3.0/pimmi.egg-info/
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     6322 2023-06-29 15:57:42.000000 pimmi-0.3.0/pimmi.egg-info/PKG-INFO
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      532 2023-06-29 15:57:42.000000 pimmi-0.3.0/pimmi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        1 2023-06-29 15:57:42.000000 pimmi-0.3.0/pimmi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       50 2023-06-29 15:57:42.000000 pimmi-0.3.0/pimmi.egg-info/entry_points.txt
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       66 2023-06-29 15:57:42.000000 pimmi-0.3.0/pimmi.egg-info/requires.txt
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       11 2023-06-29 15:57:42.000000 pimmi-0.3.0/pimmi.egg-info/top_level.txt
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        1 2023-06-29 15:52:24.000000 pimmi-0.3.0/pimmi.egg-info/zip-safe
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       38 2023-06-29 15:57:42.573795 pimmi-0.3.0/setup.cfg
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      945 2023-06-29 15:54:29.000000 pimmi-0.3.0/setup.py
+drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2023-06-29 15:57:42.573795 pimmi-0.3.0/test/
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-10-06 07:59:34.000000 pimmi-0.3.0/test/__init__.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     4084 2023-06-09 12:02:14.000000 pimmi-0.3.0/test/pipeline_test.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     1609 2023-06-10 07:40:06.000000 pimmi-0.3.0/test/sift_test.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      495 2022-10-06 07:59:34.000000 pimmi-0.3.0/test/toolbox_test.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     2592 2023-06-09 13:46:00.000000 pimmi-0.3.0/test/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pimmi-0.2.0/LICENSE` & `pimmi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pimmi-0.2.0/PKG-INFO` & `pimmi-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pimmi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python IMage MIning
 Home-page: http://github.com/nrv/pimmi
 Author: Nicolas Hervé
 Author-email: 
 License: GPL-3.0
 Keywords: image mining
-Requires-Python: >=3.5,<3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PIMMI : Python IMage MIning
 
 PIMMI is a software that performs visual mining in a corpus of images. Its main objective is to find all copies, 
 total or partial, in large volumes of images and to group them together. Our initial goal is to study the reuse
```

### Comparing `pimmi-0.2.0/README.md` & `pimmi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pimmi-0.2.0/pimmi/cli/__main__.py` & `pimmi-0.3.0/pimmi/cli/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,15 @@
                                                                         "if there is one. By default, do not erase and"
                                                                         "fill the existing index with new "
                                                                         "images.")
     parser_fill.add_argument("-f", "--force", action="store_true", help="Avoid confirmation prompt if the index already"
                                                                         "exists.")
     parser_fill.add_argument("--config-path", type=str, help="Path to custom config file. Use 'pimmi create-config' to "
                                                              "create a config file template.")
+    parser_fill.add_argument("-n", "--nb-img", type=int, help="Use only the first n images in `image_dir`")
     parser_fill.set_defaults(func=fill)
 
     # QUERY command
     parser_query = subparsers.add_parser('query', help="Query an existing index. Receive IMAGE-DIR, a directory "
                                                        "containing images, and INDEX-NAME, the name given to the index "
                                                        "when using `pimmi fill`.")
     parser_query.add_argument('image_dir', type=str, metavar='image-dir')
@@ -73,23 +74,26 @@
     parser_query.add_argument("--index-path", type=str, help="Directory where the index should be stored/loaded from. "
                                                              "Defaults to './index'", default="./index")
     parser_query.add_argument("--nb-per-split", default=10000, type=int, help="Number of images to query per pack. "
                                                                               "Defaults to 10000.")
     parser_query.add_argument("--config-path", type=str, help="Path to custom config file. Use 'pimmi create-config' to"
                                                               " create a config file template.")
     parser_query.add_argument("--simple", action="store_true", default=False)
+    parser_query.add_argument("-n", "--nb-img", type=int, help="Query only the first n images in `image_dir`")
     parser_query.set_defaults(func=query)
 
     # CLUSTERS command
     clusters_query = subparsers.add_parser('clusters', help="Create clusters from query results.")
     clusters_query.add_argument('index_name', type=str, metavar='index-name')
     clusters_query.add_argument("--index-path", type=str, help="Directory where the index should be stored/loaded from. "
                                                              "Defaults to './index'", default="./index")
     clusters_query.add_argument("--config-path", type=str, help="Path to custom config file. Use 'pimmi create-config' to"
                                                               " create a config file template.")
+    clusters_query.add_argument("--algo", type=str, default='components',
+                                help="'components' or 'louvain'. Defaults to 'components'")
     clusters_query.add_argument("-o", "--output", type=str, help="Path to output file. If not provided, print to stdout.")
     clusters_query.set_defaults(func=clusters)
 
     # VIZ command
     parser_viz = subparsers.add_parser('viz', help="Generate pimmi-ui viz data")
     parser_viz.add_argument("--clusters", type=str, help="Input clusters CSV file")
     parser_viz.add_argument("--viz", type=str, help="Output pimmi-ui viz JSON file")
@@ -119,21 +123,19 @@
     parser_create_config.add_argument('path', type=str, help="Path of the file to be created.")
     parser_create_config.set_defaults(func=create_config)
 
     cli_parameters = vars(parser.parse_args(namespace=prm))
     return cli_parameters
 
 
-def fill(image_dir, index_name, index_path, config_path, erase=False, force=False, **kwargs):
+def fill(image_dir, index_name, index_path, nb_img, erase=False, force=False, **kwargs):
     if not os.path.isdir(image_dir):
         logger.error("The provided image-dir is not a directory.")
         sys.exit(1)
 
-    check_custom_config(config_path)
-
     if not os.path.isdir(index_path):
         index_exists = False
         if confirm("{} is not a directory. Do you want to create one? y/n".format(
             os.path.abspath(index_path)
         )):
             os.mkdir(index_path)
             faiss_index, faiss_meta = make_index_path(index_path, index_name, prm.index_type)
@@ -165,40 +167,35 @@
             index_exists = False
         #todo: error if one file exists but not the other
 
     if not index_name:
         index_name = os.path.basename(os.path.normpath(image_dir))
 
     logger.info("listing images recursively from : " + image_dir)
-    images = tbx.get_all_images(image_dir)
+    images = tbx.get_all_images(image_dir, nb_img)
 
     sift = tbx.Sift(prm.sift_nfeatures, prm.sift_nOctaveLayers, prm.sift_contrastThreshold, prm.sift_edgeThreshold,
                     prm.sift_sigma, prm.nb_threads)
 
     if erase or not index_exists:
         filled_index = create_index_mt(prm.index_type, images, image_dir, sift, verbose=not prm.silent)
     else:
         previous_index = load_index(faiss_index, faiss_meta)
         filled_index = fill_index_mt(previous_index, images, image_dir, sift)
 
     save_index(filled_index, faiss_index, faiss_meta)
 
 
-def query(index_name, image_dir, index_path, config_path, nb_per_split, simple, **kwargs):
-    check_custom_config(config_path)
+def query(index_name, image_dir, index_path, nb_per_split, simple, nb_img, **kwargs):
 
     faiss_index, faiss_meta = make_index_path(index_path, index_name, prm.index_type)
 
     index = load_index(faiss_index, faiss_meta)
 
-    images = get_index_images(index, image_dir)
-
-    nb_img = kwargs.get("nb_img")
-    if nb_img:
-        images = images.head(nb_img)
+    images = get_index_images(index, image_dir, nb_img)
 
     if simple:
         prm.query_dist_filter = False
         prm.query_adaptative_sift_knn = False
 
     logger.info("total number of queries " + str(len(images)))
     # images = images.sort_values(by=constants.dff_image_path)
@@ -215,26 +212,24 @@
             image_dir,
             pack=pack[constants.dff_pack_id]
         )
         if query_result:
             query_result.to_csv(pack_result_file)
 
 
-def clusters(index_name, index_path, config_path, output, **kwargs):
-    check_custom_config(config_path)
+def clusters(index_name, index_path, output, algo, **kwargs):
     faiss_index, faiss_meta = make_index_path(index_path, index_name, prm.index_type)
     mining_files = faiss_index.replace("faiss", "mining")
     mining_files_pattern = mining_files + "_*"
     generate_clusters(
         mining_files_pattern,
         faiss_meta,
         output,
         prm.nb_match_ransac,
-        prm.algo,
-        prm.edge_collapse
+        algo,
     )
 
 
 def viz(clusters, viz, **kwargs):
     from_clusters_to_viz(clusters, viz)
 
 
@@ -305,14 +300,17 @@
 
 
 def main():
     cli_params = load_cli_parameters()
     if cli_params["silent"]:
         logger.setLevel(level=logging.ERROR)
     if "func" in cli_params:
+        config_path = cli_params.pop("config_path", None)
+        check_custom_config(config_path)
+
         command = cli_params.pop("func")
         command(**cli_params)
     else:
         parser.print_help()
 
 
 if __name__ == '__main__':
```

### Comparing `pimmi-0.2.0/pimmi/cli/config.yml` & `pimmi-0.3.0/pimmi/cli/config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -36,47 +36,47 @@
   help: "OpenCV parameter : the number of best features to retain. The features are ranked by their scores
   (measured in SIFT algorithm as the local contrast).
   See https://docs.opencv.org/3.4/d7/d60/classcv_1_1SIFT.html.
   Defaults to 1000 in Pimmi."
 
 sift_nOctaveLayers:
   value: 1
-  help: "OpenCV parameter : the number of layers in each octave. 3 is the value used in D. Lowe paper. 
+  help: "OpenCV parameter : the number of layers in each octave. 3 is the value used in D. Lowe paper.
   The number of octaves is computed automatically from the image resolution.
   See https://docs.opencv.org/3.4/d7/d60/classcv_1_1SIFT.html.
   Defaults to 1 in Pimmi."
 
 sift_contrastThreshold:
   value: 0.1
   help: "OpenCV parameter : the contrast threshold used to filter out weak features in semi-uniform (low-contrast)
   regions. The larger the threshold, the less features are produced by the detector.
   See https://docs.opencv.org/3.4/d7/d60/classcv_1_1SIFT.html.
   Defaults to 0.1 in Pimmi."
 
 sift_edgeThreshold:
   value: 10
-  help: "OpenCV parameter : the threshold used to filter out edge-like features. Note that its meaning is different from 
+  help: "OpenCV parameter : the threshold used to filter out edge-like features. Note that its meaning is different from
   the contrastThreshold, i.e. the larger the edgeThreshold, the less features are filtered out
   (more features are retained).
   See https://docs.opencv.org/3.4/d7/d60/classcv_1_1SIFT.html.
   Defaults to 10 in Pimmi."
 
 sift_sigma:
   value: 1.6
   help: "OpenCV parameter : the sigma of the Gaussian applied to the input image at the octave #0. If your image
-  is captured with a weak camera with soft lenses, you might want to reduce the number. 
+  is captured with a weak camera with soft lenses, you might want to reduce the number.
   See https://docs.opencv.org/3.4/d7/d60/classcv_1_1SIFT.html.
   Defaults to 1.6 in Pimmi."
 
 
 # ==================================================================================================
 # Part 2.1 - FAISS index creation
 index_type:
   value: "IVF1024,Flat"
-  help: "Faiss index type. See all possible values at 
+  help: "Faiss index type. See all possible values at
   https://github.com/facebookresearch/faiss/wiki/Lower-memory-footprint#simplifying-index-construction.
   Defaults to 'IVF1024,Flat', for huge database, you may consider 'OPQ16_64,IVF65536_HNSW32,PQ16'."
 
 index_nb_images_to_train:
   value: 25000
   help: "Max nb. of image used to train the index structure. Defaults to 25000."
 
@@ -157,15 +157,9 @@
   value: 10
   help: "Images are filtered out if less than 'nb_match_ransac' query points
   have matched. Defaults to 10"
 
 algo:
   value: "components"
   help: "Method used to detect communities in the image similarity graph. Use 'components' for connected components,
-  and 'louvain' for multi-level modularity optimization (Blondel, V. D., Guillaume, J.-L., Lambiotte, R., & 
+  and 'louvain' for multi-level modularity optimization (Blondel, V. D., Guillaume, J.-L., Lambiotte, R., &
   Lefebvre, E. (2008))"
-
-edge_collapse:
-  value: "mean"
-  help: "If the chosen algo is 'louvain', method used to combine the edges of the image similarity graph when 
-  it is transformed into an undirected graph. Available values: 'mean', 'min', 'max', 'first', 'last', 'sum'."
-
```

### Comparing `pimmi-0.2.0/pimmi/eval.py` & `pimmi-0.3.0/pimmi/eval.py`

 * *Files identical despite different names*

### Comparing `pimmi-0.2.0/pimmi/pimmi.py` & `pimmi-0.3.0/pimmi/pimmi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import math
 import numpy as np
 import cv2 as cv
 import faiss
 import pickle
 import logging
 import csv
-import json
+from tqdm import tqdm
 from json import JSONEncoder
 import os.path
-from multiprocessing import Queue, Process
+from multiprocessing import Queue, Process, set_start_method
 
 from typing import List
 from itertools import groupby
 
 import pimmi.pimmi_parameters as constants
 from pimmi.cli.config import parameters as prm
 from pimmi.toolbox import Sift
@@ -30,14 +30,16 @@
 dff_internal_pack_id = "pack_id"
 dff_internal_query_result = "query_result"
 dff_internal_faiss = "faiss"
 dff_internal_faiss_type = "faiss_type"
 dff_internal_faiss_nb_images = "faiss_nb_images"
 dff_internal_faiss_nb_features = "faiss_nb_features"
 
+# Configure multiprocessing
+set_start_method('fork')
 
 logging.basicConfig(format='%(asctime)s : %(levelname)s : %(name)s - %(message)s', level=logging.INFO)
 logger = logging.getLogger("pimmi")
 
 
 def resize_if_needed(img):
     resized = False
@@ -68,19 +70,14 @@
     kp, desc = extract_sift_img(img, sift)
     if image_id % 100 == 0:
         h, w = img.shape
         if pack >= 0:
             pfx = str(pack) + " :: " + str(image_id)
         else:
             pfx = str(image_id)
-        logger.info(
-            "~ [" + pfx + "] (" + str(prm.sift_nfeatures) + ", " + str(prm.sift_nOctaveLayers) + ", " +
-            str(prm.sift_contrastThreshold) + ", " + str(prm.sift_edgeThreshold) + ", " + str(prm.sift_sigma)
-            + ") extracting " + str(len(kp)) + " sift points for (" + str(w) + " x " +
-            str(h) + ", " + str(resized) + ") " + file)
     ids = None
     if image_id is not None:
         ids = np.empty(len(kp), dtype="int64")
         for sift_point in range(0, len(kp)):
             ids[sift_point] = point_to_full_id(image_id, kp[sift_point].pt, img.shape[1], img.shape[0])
     return ids, kp, desc, img.shape[1], img.shape[0]
 
@@ -138,38 +135,36 @@
             constants.dff_image_path: rel_image_path,
             constants.dff_width: None,
             constants.dff_height: None,
             constants.dff_nb_points: None,
             constants.dff_image_id: index[dff_internal_id_generator]
         }
         task_queue.put({
-            constants.dff_image_path: image_path, 
+            constants.dff_image_path: image_path,
             constants.dff_image_id: index[dff_internal_id_generator]})
         index[dff_internal_id_generator] = index[dff_internal_id_generator] + 1
         task_launched += 1
         if only_empty_index and task_launched >= prm.index_nb_images_to_train:
             break
 
     logger.info(
         "nb tasks launched : " + str(task_launched) + " / " + str(prm.index_nb_images_to_train))
 
     all_ids = None
     all_features = None
-    for i in range(task_launched):
+    for i in tqdm(range(task_launched)):
         result = result_queue.get()
         image_id = result[constants.dff_image_id]
         ids = result[constants.dff_ids]
         if ids is not None and len(ids) > 0:
             desc = result[constants.dff_desc]
             index[dff_internal_meta][image_id][constants.dff_width] = result[constants.dff_width]
             index[dff_internal_meta][image_id][constants.dff_height] = result[constants.dff_height]
             index[dff_internal_meta][image_id][constants.dff_nb_points] = len(ids)
             index[dff_internal_faiss_nb_images] = index[dff_internal_faiss_nb_images] + 1
-            if image_id % 100 == 0:
-                logger.info("~ [" + str(image_id) + "] result retrieved from queue : " + str(len(ids)))
             if all_features is None:
                 all_features = []
                 all_ids = []
             all_features.append(desc)
             all_ids.append(ids)
         if all_ids is not None and len(all_ids) >= prm.index_nb_images_to_train:
             all_features = np.vstack(all_features)
@@ -268,19 +263,23 @@
             logger.info("meta loaded " + meta_file)
     logger.info("index has " + str(index[dff_internal_faiss_nb_images]) + "/" + str(index[dff_internal_id_generator]) +
                 " images with " + str(index[dff_internal_faiss_nb_features]) + " feature points")
     logger.info(" - type : " + index[dff_internal_faiss_type])
     return index
 
 
-def get_index_images(index, path_prefix):
-    # TODO simplify these 3 lines !
-    all_path = [path_prefix + "/" + image[constants.dff_image_path] for image in index[dff_internal_meta].values()]
-    all_image_ids = [image[constants.dff_image_id] for image in index[dff_internal_meta].values()]
-    all_images = [{constants.dff_image_path: p, constants.dff_image_id: i} for p, i in zip(all_path, all_image_ids)]
+def get_index_images(index, path_prefix, nb_img=None):
+
+    all_images = []
+    for image in index[dff_internal_meta].values():
+        image_path = os.path.join(path_prefix, image[constants.dff_image_path])
+        image_id = image[constants.dff_image_id]
+        all_images.append({constants.dff_image_path: image_path, constants.dff_image_id: image_id})
+        if nb_img and len(all_images) >= nb_img:
+            return all_images
 
     logger.info("found " + str(len(all_images)) + " images in index")
     return all_images
 
 
 def query_index_extract_single_image(index, image_file, relative_image_path, sift, query_image_id=0, pack=-1):
     query_ids, query_kp, query_desc, query_width, query_height = extract_sift(
@@ -460,16 +459,14 @@
                     if len(knn_dist) > 0:
                         first_non_zero_dist = knn_dist[0]
                         filter_on_dist_ratio = first_non_zero_dist / knn_dist > prm.query_dist_ratio_threshold
                         knn_ids_nonzero = knn_ids_nonzero[filter_on_dist_ratio]
                         knn_ids_filtered = np.concatenate((knn_ids_zero, knn_ids_nonzero))
                         if prm.query_adaptative_sift_knn and len(knn_ids_filtered) == len(knn_ids):
                             current_nn_is_enough = False
-                            logger.info("    . " + str(sift_query_id) + " reached knn (" + str(current_nn) + ") limit "
-                                        + str(knn_dist[-1]) + " / " + str(first_non_zero_dist))
                             break
                         else:
                             knn_ids = knn_ids_filtered
 
                 if prm.query_ransac:
                     kept_matches.add_new_matched_points(sift_query_id, knn_ids)
 
@@ -573,15 +570,15 @@
                 }
             )
             task_launched += 1
         else:
             logger.warning("unable to find image, will not query it : " + image_path)
 
     all_result = ImageResultList()
-    for i in range(task_launched):
+    for i in tqdm(range(task_launched)):
         result = result_queue.get()
         query_result: ImageResultList = result
 
         if query_result is None or len(query_result) == 0:
             continue
         for ir in query_result:
             if ir.keep:
```

### Comparing `pimmi-0.2.0/pimmi/pimmi_parameters.py` & `pimmi-0.3.0/pimmi/pimmi_parameters.py`

 * *Files identical despite different names*

### Comparing `pimmi-0.2.0/pimmi/toolbox.py` & `pimmi-0.3.0/pimmi/toolbox.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,34 @@
-import glob
+import os
+import re
 import json
 import math
+import random
 import cv2 as cv
-from os.path import join
 import pimmi.pimmi_parameters as constants
 import logging
 
 logger = logging.getLogger("pimmi")
 
-ALLOWLIST_FORMATS = (".jpeg", ".jpg", ".png")
+ALLOWED_FORMATS = ("jpeg", "jpg", "png")
+ALLOWED_FORMATS_PATTERN = r".*\.({})$".format("|".join(ALLOWED_FORMATS))
 
 
-def get_all_images(image_dir):
-    files = []
-    for extension in ALLOWLIST_FORMATS:
-        files.extend(glob.glob(join(image_dir, "**", "*{}".format(extension)), recursive=True))
-    return files
+def get_all_images(image_dir, nb_img=None):
+
+    image_files = []
+    for root, dirs, files in os.walk(image_dir):
+        for f in files:
+            if re.search(ALLOWED_FORMATS_PATTERN, f):
+                image_files.append(os.path.join(root, f))
+                if nb_img and len(image_files) >= nb_img:
+                    return image_files
+
+    random.shuffle(image_files)
+    return image_files
 
 
 def parse_mex(file):
     with open(file, encoding="utf-8") as f:
         for line in f:
             yield json.loads(line)
     f.close()
@@ -72,9 +81,8 @@
             sift_sigma,
             nb_threads
     ):
 
         self.config = cv.SIFT_create(nfeatures=sift_nfeatures, nOctaveLayers=sift_nOctaveLayers,
                               contrastThreshold=sift_contrastThreshold, edgeThreshold=sift_edgeThreshold,
                               sigma=sift_sigma)
-        logger.info("Using opencv : " + cv.__version__)
         cv.setNumThreads(nb_threads)
```

### Comparing `pimmi-0.2.0/pimmi.egg-info/PKG-INFO` & `pimmi-0.3.0/pimmi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pimmi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python IMage MIning
 Home-page: http://github.com/nrv/pimmi
 Author: Nicolas Hervé
 Author-email: 
 License: GPL-3.0
 Keywords: image mining
-Requires-Python: >=3.5,<3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PIMMI : Python IMage MIning
 
 PIMMI is a software that performs visual mining in a corpus of images. Its main objective is to find all copies, 
 total or partial, in large volumes of images and to group them together. Our initial goal is to study the reuse
```

### Comparing `pimmi-0.2.0/pimmi.egg-info/SOURCES.txt` & `pimmi-0.3.0/pimmi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pimmi-0.2.0/setup.py` & `pimmi-0.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 from setuptools import setup, find_packages
 
 with open('./README.md', 'r') as f:
     long_description = f.read()
 
 setup(name='pimmi',
-      version='0.2.0',
+      version='0.3.0',
       description='Python IMage MIning',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='http://github.com/nrv/pimmi',
       license='GPL-3.0',
       author='Nicolas Hervé',
       author_email='',
       keywords='image mining',
-      python_requires='>=3.5,<3.9',
+      python_requires='>=3.8',
       package_data={'pimmi': ['cli/config.yml']},
       packages=find_packages(exclude=["collect*", "dist", "build"]),
       include_package_data=True,
       install_requires=[
-        "fog",
-        "numpy",
-        "pandas",
+        "casanova",
         "faiss-cpu",
-        "click",
-        "matplotlib",
-        "python-igraph",
+        "fog",
+        "networkx>=2.7,<3",
         "opencv-python",
         "pyyaml",
-        "casanova"
+        "tqdm",
       ],
       entry_points={
         'console_scripts': [
             'pimmi=pimmi.cli.__main__:main',
         ]
       },
       zip_safe=True
```

### Comparing `pimmi-0.2.0/test/pipeline_test.py` & `pimmi-0.3.0/test/pipeline_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # =============================================================================
 # Pimmi Functional Tests
 # =============================================================================
 import csv
-import json
 from glob import glob
 from collections import defaultdict
 from os import remove
 from os.path import join, dirname
 
 RESSOURCES_PATH = join(dirname(__file__), "ressources")
 SMALL_DATASET_QUERY_RESULTS = join(RESSOURCES_PATH, "query_results.csv")
```

### Comparing `pimmi-0.2.0/test/sift_test.py` & `pimmi-0.3.0/test/sift_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # =============================================================================
 # Pimmi SIFT Points Unit Tests
 # =============================================================================
 import numpy as np
-from os.path import join, dirname
 
 from pimmi.pimmi import extract_sift
 from pimmi.toolbox import Sift
-from test.utils import load_sifts_from_file, EXAMPLE_IMAGE_FILE, SMALL_DATASET_DIR, kp_fieldnames, prm
-
-IMAGE_PATH = join(SMALL_DATASET_DIR, "000010.jpg")
+from test.utils import load_sifts_from_file, EXAMPLE_IMAGE_FILE, IMAGE_PATH, kp_fieldnames, prm
 
 IMAGE_WIDTH = 512
 IMAGE_HEIGHT = 341
+ROUND_DECIMALS = 2
 
 
 class TestSift(object):
     def test_extract_sift(self):
         sift = Sift(prm.sift_nfeatures, prm.sift_nOctaveLayers, prm.sift_contrastThreshold, prm.sift_edgeThreshold,
                     prm.sift_sigma, prm.nb_threads)
 
         assert extract_sift("wrong_path.jpg", 0, sift) == (None, None, None, None, None)
 
         ids, desc, kp = load_sifts_from_file(EXAMPLE_IMAGE_FILE)
 
         tested_ids, tested_kp, tested_desc, tested_width, tested_height = extract_sift(IMAGE_PATH, 0, sift)
 
-        assert np.array_equal(desc, tested_desc)
+        assert desc.shape == tested_desc.shape
+        assert np.allclose(desc, tested_desc, atol=1.)
         assert np.array_equal(ids, tested_ids)
         assert IMAGE_HEIGHT == tested_height
         assert IMAGE_WIDTH == tested_width
         for kp_item, tested_kp_item in zip(kp, tested_kp):
-            assert kp_item.pt[0] == tested_kp_item.pt[0]
-            assert kp_item.pt[1] == tested_kp_item.pt[1]
+            assert round(kp_item.pt[0], ROUND_DECIMALS) == round(tested_kp_item.pt[0], ROUND_DECIMALS)
+            assert round(kp_item.pt[1], ROUND_DECIMALS) == round(tested_kp_item.pt[1], ROUND_DECIMALS)
             for attr in kp_fieldnames[2:]:
-                assert getattr(kp_item, attr) == getattr(tested_kp_item, attr)
+                assert round(float(getattr(kp_item, attr)), ROUND_DECIMALS) == round(float(getattr(tested_kp_item, attr)), ROUND_DECIMALS)
```

### Comparing `pimmi-0.2.0/test/utils.py` & `pimmi-0.3.0/test/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os.path import join, dirname
 
 from pimmi.pimmi import resize_if_needed, point_to_full_id
 from pimmi.cli.config import parameters as prm
 
 
 SMALL_DATASET_DIR = join(dirname(dirname(__file__)), 'demo_dataset', 'small_dataset')
-IMAGE_PATH = join(SMALL_DATASET_DIR, "000010.jpg")
+IMAGE_PATH = join(SMALL_DATASET_DIR, "1", "000010.jpg")
 EXAMPLE_IMAGE_FILE = join(dirname(__file__), "ressources", "image_000010_sifts.csv")
 IMAGE_ID = 0
 
 config_path = join(dirname(__file__), "ressources", "config.yml")
 config_dict = prm.load_config_file(config_path)
 prm.set_config_as_attributes(config_dict)
```

