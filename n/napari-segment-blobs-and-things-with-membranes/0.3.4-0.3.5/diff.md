# Comparing `tmp/napari-segment-blobs-and-things-with-membranes-0.3.4.tar.gz` & `tmp/napari-segment-blobs-and-things-with-membranes-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-segment-blobs-and-things-with-membranes-0.3.4.tar", last modified: Thu Feb 23 18:04:35 2023, max compression
+gzip compressed data, was "napari-segment-blobs-and-things-with-membranes-0.3.5.tar", last modified: Thu Jun 29 14:03:37 2023, max compression
```

## Comparing `napari-segment-blobs-and-things-with-membranes-0.3.4.tar` & `napari-segment-blobs-and-things-with-membranes-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 18:04:35.133690 napari-segment-blobs-and-things-with-membranes-0.3.4/
--rw-rw-rw-   0        0        0     1545 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/LICENSE
--rw-rw-rw-   0        0        0      127 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0    10368 2023-02-23 18:04:35.133690 napari-segment-blobs-and-things-with-membranes-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     8782 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-23 18:04:35.118063 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes/
--rw-rw-rw-   0        0        0    36783 2023-02-23 18:02:40.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-23 18:04:35.133690 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes/_tests/
--rw-rw-rw-   0        0        0        0 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes/_tests/__init__.py
--rw-rw-rw-   0        0        0     3603 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes/_tests/test_function.py
-drwxrwxrwx   0        0        0        0 2023-02-23 18:04:35.118063 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes.egg-info/
--rw-rw-rw-   0        0        0    10368 2023-02-23 18:04:34.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      683 2023-02-23 18:04:35.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 18:04:34.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-02-23 18:04:34.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2023-02-23 18:04:34.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       47 2023-02-23 18:04:34.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      302 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/requirements.txt
--rw-rw-rw-   0        0        0     1848 2023-02-23 18:04:35.133690 napari-segment-blobs-and-things-with-membranes-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0       89 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:03:37.942925 napari-segment-blobs-and-things-with-membranes-0.3.5/
+-rw-rw-rw-   0        0        0     1545 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0      127 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    10368 2023-06-29 14:03:37.942925 napari-segment-blobs-and-things-with-membranes-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8782 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 14:03:37.911671 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/
+-rw-rw-rw-   0        0        0    37937 2023-06-29 14:02:19.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:03:37.942925 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/_tests/
+-rw-rw-rw-   0        0        0        0 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/_tests/__init__.py
+-rw-rw-rw-   0        0        0     3995 2023-06-29 13:51:48.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/_tests/test_function.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:03:37.942925 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/
+-rw-rw-rw-   0        0        0    10368 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       47 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      302 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/requirements.txt
+-rw-rw-rw-   0        0        0     1848 2023-06-29 14:03:37.942925 napari-segment-blobs-and-things-with-membranes-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0       89 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/setup.py
```

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.4/LICENSE` & `napari-segment-blobs-and-things-with-membranes-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.4/PKG-INFO` & `napari-segment-blobs-and-things-with-membranes-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-blobs-and-things-with-membranes
-Version: 0.3.4
+Version: 0.3.5
 Summary: A plugin based on scikit-image for segmenting nuclei and cells based on fluorescent microscopy images with high intensity in nuclei and/or membranes
 Home-page: https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes#README.md
```

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.4/README.md` & `napari-segment-blobs-and-things-with-membranes-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes/__init__.py` & `napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 0d0a 5f5f 7665 7273 696f 6e5f 5f20 3d20  ..__version__ = 
-00000010: 2230 2e33 2e34 220d 0a5f 5f63 6f6d 6d6f  "0.3.4"..__commo
+00000010: 2230 2e33 2e35 220d 0a5f 5f63 6f6d 6d6f  "0.3.5"..__commo
 00000020: 6e5f 616c 6961 735f 5f20 3d20 226e 7362  n_alias__ = "nsb
 00000030: 6174 776d 220d 0a0d 0a66 726f 6d20 6e61  atwm"....from na
 00000040: 7061 7269 5f70 6c75 6769 6e5f 656e 6769  pari_plugin_engi
 00000050: 6e65 2069 6d70 6f72 7420 6e61 7061 7269  ne import napari
 00000060: 5f68 6f6f 6b5f 696d 706c 656d 656e 7461  _hook_implementa
 00000070: 7469 6f6e 0d0a 696d 706f 7274 206e 756d  tion..import num
 00000080: 7079 2061 7320 6e70 0d0a 6672 6f6d 2073  py as np..from s
@@ -35,2265 +35,2338 @@
 00000220: 6c73 5f6d 656e 7520 696d 706f 7274 2072  ls_menu import r
 00000230: 6567 6973 7465 725f 6675 6e63 7469 6f6e  egister_function
 00000240: 0d0a 6672 6f6d 2073 6b69 6d61 6765 2e6d  ..from skimage.m
 00000250: 6561 7375 7265 2069 6d70 6f72 7420 7265  easure import re
 00000260: 6769 6f6e 7072 6f70 730d 0a66 726f 6d20  gionprops..from 
 00000270: 736b 696d 6167 652e 7365 676d 656e 7461  skimage.segmenta
 00000280: 7469 6f6e 2069 6d70 6f72 7420 7265 6c61  tion import rela
-00000290: 6265 6c5f 7365 7175 656e 7469 616c 0d0a  bel_sequential..
-000002a0: 6672 6f6d 2073 6b69 6d61 6765 2e73 6567  from skimage.seg
-000002b0: 6d65 6e74 6174 696f 6e20 696d 706f 7274  mentation import
-000002c0: 2063 6c65 6172 5f62 6f72 6465 720d 0a66   clear_border..f
-000002d0: 726f 6d20 736b 696d 6167 652e 7365 676d  rom skimage.segm
-000002e0: 656e 7461 7469 6f6e 2069 6d70 6f72 7420  entation import 
-000002f0: 6578 7061 6e64 5f6c 6162 656c 7320 6173  expand_labels as
-00000300: 2073 6b5f 6578 7061 6e64 5f6c 6162 656c   sk_expand_label
-00000310: 730d 0a66 726f 6d20 736b 696d 6167 6520  s..from skimage 
-00000320: 696d 706f 7274 2066 696c 7465 7273 0d0a  import filters..
-00000330: 696d 706f 7274 2073 6369 7079 0d0a 6672  import scipy..fr
-00000340: 6f6d 2073 6369 7079 2069 6d70 6f72 7420  om scipy import 
-00000350: 6e64 696d 6167 650d 0a66 726f 6d20 6e61  ndimage..from na
-00000360: 7061 7269 5f74 696d 655f 736c 6963 6572  pari_time_slicer
-00000370: 2069 6d70 6f72 7420 7469 6d65 5f73 6c69   import time_sli
-00000380: 6365 720d 0a66 726f 6d20 7374 6163 6b76  cer..from stackv
-00000390: 6965 7720 696d 706f 7274 206a 7570 7974  iew import jupyt
-000003a0: 6572 5f64 6973 706c 6179 6162 6c65 5f6f  er_displayable_o
-000003b0: 7574 7075 740d 0a0d 0a40 6e61 7061 7269  utput....@napari
-000003c0: 5f68 6f6f 6b5f 696d 706c 656d 656e 7461  _hook_implementa
-000003d0: 7469 6f6e 0d0a 6465 6620 6e61 7061 7269  tion..def napari
-000003e0: 5f65 7870 6572 696d 656e 7461 6c5f 7072  _experimental_pr
-000003f0: 6f76 6964 655f 6675 6e63 7469 6f6e 2829  ovide_function()
-00000400: 3a0d 0a20 2020 2072 6574 7572 6e20 5b0d  :..    return [.
-00000410: 0a20 2020 2020 2020 2067 6175 7373 6961  .        gaussia
-00000420: 6e5f 626c 7572 2c0d 0a20 2020 2020 2020  n_blur,..       
-00000430: 2073 7562 7472 6163 745f 6261 636b 6772   subtract_backgr
-00000440: 6f75 6e64 2c0d 0a20 2020 2020 2020 2074  ound,..        t
-00000450: 6872 6573 686f 6c64 5f6f 7473 752c 0d0a  hreshold_otsu,..
+00000290: 6265 6c5f 7365 7175 656e 7469 616c 2061  bel_sequential a
+000002a0: 7320 736b 5f72 656c 6162 656c 5f73 6571  s sk_relabel_seq
+000002b0: 7565 6e74 6961 6c0d 0a66 726f 6d20 736b  uential..from sk
+000002c0: 696d 6167 652e 7365 676d 656e 7461 7469  image.segmentati
+000002d0: 6f6e 2069 6d70 6f72 7420 636c 6561 725f  on import clear_
+000002e0: 626f 7264 6572 0d0a 6672 6f6d 2073 6b69  border..from ski
+000002f0: 6d61 6765 2e73 6567 6d65 6e74 6174 696f  mage.segmentatio
+00000300: 6e20 696d 706f 7274 2065 7870 616e 645f  n import expand_
+00000310: 6c61 6265 6c73 2061 7320 736b 5f65 7870  labels as sk_exp
+00000320: 616e 645f 6c61 6265 6c73 0d0a 6672 6f6d  and_labels..from
+00000330: 2073 6b69 6d61 6765 2069 6d70 6f72 7420   skimage import 
+00000340: 6669 6c74 6572 730d 0a69 6d70 6f72 7420  filters..import 
+00000350: 7363 6970 790d 0a66 726f 6d20 7363 6970  scipy..from scip
+00000360: 7920 696d 706f 7274 206e 6469 6d61 6765  y import ndimage
+00000370: 0d0a 6672 6f6d 206e 6170 6172 695f 7469  ..from napari_ti
+00000380: 6d65 5f73 6c69 6365 7220 696d 706f 7274  me_slicer import
+00000390: 2074 696d 655f 736c 6963 6572 0d0a 6672   time_slicer..fr
+000003a0: 6f6d 2073 7461 636b 7669 6577 2069 6d70  om stackview imp
+000003b0: 6f72 7420 6a75 7079 7465 725f 6469 7370  ort jupyter_disp
+000003c0: 6c61 7961 626c 655f 6f75 7470 7574 0d0a  layable_output..
+000003d0: 0d0a 406e 6170 6172 695f 686f 6f6b 5f69  ..@napari_hook_i
+000003e0: 6d70 6c65 6d65 6e74 6174 696f 6e0d 0a64  mplementation..d
+000003f0: 6566 206e 6170 6172 695f 6578 7065 7269  ef napari_experi
+00000400: 6d65 6e74 616c 5f70 726f 7669 6465 5f66  mental_provide_f
+00000410: 756e 6374 696f 6e28 293a 0d0a 2020 2020  unction():..    
+00000420: 7265 7475 726e 205b 0d0a 2020 2020 2020  return [..      
+00000430: 2020 6761 7573 7369 616e 5f62 6c75 722c    gaussian_blur,
+00000440: 0d0a 2020 2020 2020 2020 7375 6274 7261  ..        subtra
+00000450: 6374 5f62 6163 6b67 726f 756e 642c 0d0a  ct_background,..
 00000460: 2020 2020 2020 2020 7468 7265 7368 6f6c          threshol
-00000470: 645f 7965 6e2c 0d0a 2020 2020 2020 2020  d_yen,..        
-00000480: 7468 7265 7368 6f6c 645f 6973 6f64 6174  threshold_isodat
-00000490: 612c 0d0a 2020 2020 2020 2020 7468 7265  a,..        thre
-000004a0: 7368 6f6c 645f 6c69 2c0d 0a20 2020 2020  shold_li,..     
-000004b0: 2020 2074 6872 6573 686f 6c64 5f6d 6561     threshold_mea
-000004c0: 6e2c 0d0a 2020 2020 2020 2020 7468 7265  n,..        thre
-000004d0: 7368 6f6c 645f 6d69 6e69 6d75 6d2c 0d0a  shold_minimum,..
-000004e0: 2020 2020 2020 2020 7468 7265 7368 6f6c          threshol
-000004f0: 645f 7472 6961 6e67 6c65 2c0d 0a20 2020  d_triangle,..   
-00000500: 2020 2020 2062 696e 6172 795f 696e 7665       binary_inve
-00000510: 7274 2c0d 0a20 2020 2020 2020 2073 706c  rt,..        spl
-00000520: 6974 5f74 6f75 6368 696e 675f 6f62 6a65  it_touching_obje
-00000530: 6374 732c 0d0a 2020 2020 2020 2020 636f  cts,..        co
-00000540: 6e6e 6563 7465 645f 636f 6d70 6f6e 656e  nnected_componen
-00000550: 745f 6c61 6265 6c69 6e67 2c0d 0a20 2020  t_labeling,..   
-00000560: 2020 2020 2073 6565 6465 645f 7761 7465       seeded_wate
-00000570: 7273 6865 642c 0d0a 2020 2020 2020 2020  rshed,..        
-00000580: 766f 726f 6e6f 695f 6f74 7375 5f6c 6162  voronoi_otsu_lab
-00000590: 656c 696e 672c 0d0a 2020 2020 2020 2020  eling,..        
-000005a0: 6761 7573 735f 6f74 7375 5f6c 6162 656c  gauss_otsu_label
-000005b0: 696e 672c 0d0a 2020 2020 2020 2020 6761  ing,..        ga
-000005c0: 7573 7369 616e 5f6c 6170 6c61 6365 2c0d  ussian_laplace,.
-000005d0: 0a20 2020 2020 2020 206d 6564 6961 6e5f  .        median_
-000005e0: 6669 6c74 6572 2c0d 0a20 2020 2020 2020  filter,..       
-000005f0: 206d 6178 696d 756d 5f66 696c 7465 722c   maximum_filter,
-00000600: 0d0a 2020 2020 2020 2020 6d69 6e69 6d75  ..        minimu
+00000470: 645f 6f74 7375 2c0d 0a20 2020 2020 2020  d_otsu,..       
+00000480: 2074 6872 6573 686f 6c64 5f79 656e 2c0d   threshold_yen,.
+00000490: 0a20 2020 2020 2020 2074 6872 6573 686f  .        thresho
+000004a0: 6c64 5f69 736f 6461 7461 2c0d 0a20 2020  ld_isodata,..   
+000004b0: 2020 2020 2074 6872 6573 686f 6c64 5f6c       threshold_l
+000004c0: 692c 0d0a 2020 2020 2020 2020 7468 7265  i,..        thre
+000004d0: 7368 6f6c 645f 6d65 616e 2c0d 0a20 2020  shold_mean,..   
+000004e0: 2020 2020 2074 6872 6573 686f 6c64 5f6d       threshold_m
+000004f0: 696e 696d 756d 2c0d 0a20 2020 2020 2020  inimum,..       
+00000500: 2074 6872 6573 686f 6c64 5f74 7269 616e   threshold_trian
+00000510: 676c 652c 0d0a 2020 2020 2020 2020 6269  gle,..        bi
+00000520: 6e61 7279 5f69 6e76 6572 742c 0d0a 2020  nary_invert,..  
+00000530: 2020 2020 2020 7370 6c69 745f 746f 7563        split_touc
+00000540: 6869 6e67 5f6f 626a 6563 7473 2c0d 0a20  hing_objects,.. 
+00000550: 2020 2020 2020 2063 6f6e 6e65 6374 6564         connected
+00000560: 5f63 6f6d 706f 6e65 6e74 5f6c 6162 656c  _component_label
+00000570: 696e 672c 0d0a 2020 2020 2020 2020 7365  ing,..        se
+00000580: 6564 6564 5f77 6174 6572 7368 6564 2c0d  eded_watershed,.
+00000590: 0a20 2020 2020 2020 2076 6f72 6f6e 6f69  .        voronoi
+000005a0: 5f6f 7473 755f 6c61 6265 6c69 6e67 2c0d  _otsu_labeling,.
+000005b0: 0a20 2020 2020 2020 2067 6175 7373 5f6f  .        gauss_o
+000005c0: 7473 755f 6c61 6265 6c69 6e67 2c0d 0a20  tsu_labeling,.. 
+000005d0: 2020 2020 2020 2067 6175 7373 6961 6e5f         gaussian_
+000005e0: 6c61 706c 6163 652c 0d0a 2020 2020 2020  laplace,..      
+000005f0: 2020 6d65 6469 616e 5f66 696c 7465 722c    median_filter,
+00000600: 0d0a 2020 2020 2020 2020 6d61 7869 6d75  ..        maximu
 00000610: 6d5f 6669 6c74 6572 2c0d 0a20 2020 2020  m_filter,..     
-00000620: 2020 2070 6572 6365 6e74 696c 655f 6669     percentile_fi
-00000630: 6c74 6572 2c0d 0a20 2020 2020 2020 2062  lter,..        b
-00000640: 6c61 636b 5f74 6f70 6861 742c 0d0a 2020  lack_tophat,..  
-00000650: 2020 2020 2020 7768 6974 655f 746f 7068        white_toph
-00000660: 6174 2c0d 0a20 2020 2020 2020 206d 6f72  at,..        mor
-00000670: 7068 6f6c 6f67 6963 616c 5f67 7261 6469  phological_gradi
-00000680: 656e 742c 0d0a 2020 2020 2020 2020 6c6f  ent,..        lo
-00000690: 6361 6c5f 6d69 6e69 6d61 5f73 6565 6465  cal_minima_seede
-000006a0: 645f 7761 7465 7273 6865 642c 0d0a 2020  d_watershed,..  
-000006b0: 2020 2020 2020 7468 7265 7368 6f6c 6465        thresholde
-000006c0: 645f 6c6f 6361 6c5f 6d69 6e69 6d61 5f73  d_local_minima_s
-000006d0: 6565 6465 645f 7761 7465 7273 6865 642c  eeded_watershed,
-000006e0: 0d0a 2020 2020 2020 2020 7375 6d5f 696d  ..        sum_im
-000006f0: 6167 6573 2c0d 0a20 2020 2020 2020 206d  ages,..        m
-00000700: 756c 7469 706c 795f 696d 6167 6573 2c0d  ultiply_images,.
-00000710: 0a20 2020 2020 2020 2064 6976 6964 655f  .        divide_
-00000720: 696d 6167 6573 2c0d 0a20 2020 2020 2020  images,..       
-00000730: 2069 6e76 6572 745f 696d 6167 652c 0d0a   invert_image,..
-00000740: 2020 2020 2020 2020 736b 656c 6574 6f6e          skeleton
-00000750: 697a 652c 0d0a 2020 2020 2020 2020 4d61  ize,..        Ma
-00000760: 6e75 616c 6c79 5f6d 6572 6765 5f6c 6162  nually_merge_lab
-00000770: 656c 732c 0d0a 2020 2020 2020 2020 4d61  els,..        Ma
-00000780: 6e75 616c 6c79 5f73 706c 6974 5f6c 6162  nually_split_lab
-00000790: 656c 732c 0d0a 2020 2020 2020 2020 7265  els,..        re
-000007a0: 7363 616c 652c 0d0a 2020 2020 2020 2020  scale,..        
-000007b0: 7265 7369 7a65 2c0d 0a20 2020 2020 2020  resize,..       
-000007c0: 2065 7874 7261 6374 5f73 6c69 6365 0d0a   extract_slice..
-000007d0: 2020 2020 5d0d 0a0d 0a0d 0a0d 0a0d 0a0d      ]...........
-000007e0: 0a0d 0a64 6566 205f 736f 6265 6c5f 3364  ...def _sobel_3d
-000007f0: 2869 6d61 6765 293a 0d0a 2020 2020 6b65  (image):..    ke
-00000800: 726e 656c 203d 206e 702e 6173 6172 7261  rnel = np.asarra
-00000810: 7928 5b0d 0a20 2020 2020 2020 205b 0d0a  y([..        [..
-00000820: 2020 2020 2020 2020 2020 2020 5b30 2c20              [0, 
-00000830: 302c 2030 5d2c 0d0a 2020 2020 2020 2020  0, 0],..        
-00000840: 2020 2020 5b30 2c20 312c 2030 5d2c 0d0a      [0, 1, 0],..
-00000850: 2020 2020 2020 2020 2020 2020 5b30 2c20              [0, 
-00000860: 302c 2030 5d0d 0a20 2020 2020 2020 205d  0, 0]..        ]
-00000870: 2c20 5b0d 0a20 2020 2020 2020 2020 2020  , [..           
-00000880: 205b 302c 2031 2c20 305d 2c0d 0a20 2020   [0, 1, 0],..   
-00000890: 2020 2020 2020 2020 205b 312c 202d 362c           [1, -6,
-000008a0: 2031 5d2c 0d0a 2020 2020 2020 2020 2020   1],..          
-000008b0: 2020 5b30 2c20 312c 2030 5d0d 0a20 2020    [0, 1, 0]..   
-000008c0: 2020 2020 205d 2c20 5b0d 0a20 2020 2020       ], [..     
-000008d0: 2020 2020 2020 205b 302c 2030 2c20 305d         [0, 0, 0]
-000008e0: 2c0d 0a20 2020 2020 2020 2020 2020 205b  ,..            [
-000008f0: 302c 2031 2c20 305d 2c0d 0a20 2020 2020  0, 1, 0],..     
-00000900: 2020 2020 2020 205b 302c 2030 2c20 305d         [0, 0, 0]
-00000910: 0d0a 2020 2020 2020 2020 5d0d 0a20 2020  ..        ]..   
-00000920: 205d 290d 0a20 2020 2072 6574 7572 6e20   ])..    return 
-00000930: 6e64 692e 636f 6e76 6f6c 7665 2869 6d61  ndi.convolve(ima
-00000940: 6765 2c20 6b65 726e 656c 290d 0a0d 0a0d  ge, kernel).....
-00000950: 0a40 7265 6769 7374 6572 5f66 756e 6374  .@register_funct
-00000960: 696f 6e28 6d65 6e75 3d22 5365 676d 656e  ion(menu="Segmen
-00000970: 7461 7469 6f6e 2070 6f73 742d 7072 6f63  tation post-proc
-00000980: 6573 7369 6e67 203e 2053 706c 6974 2074  essing > Split t
-00000990: 6f75 6368 696e 6720 6f62 6a65 6374 7320  ouching objects 
-000009a0: 286e 7362 6174 776d 2922 290d 0a40 6a75  (nsbatwm)")..@ju
-000009b0: 7079 7465 725f 6469 7370 6c61 7961 626c  pyter_displayabl
-000009c0: 655f 6f75 7470 7574 286c 6962 7261 7279  e_output(library
-000009d0: 5f6e 616d 653d 276e 7362 6174 776d 272c  _name='nsbatwm',
-000009e0: 2068 656c 705f 7572 6c3d 2768 7474 7073   help_url='https
-000009f0: 3a2f 2f77 7777 2e6e 6170 6172 692d 6875  ://www.napari-hu
-00000a00: 622e 6f72 672f 706c 7567 696e 732f 6e61  b.org/plugins/na
-00000a10: 7061 7269 2d73 6567 6d65 6e74 2d62 6c6f  pari-segment-blo
-00000a20: 6273 2d61 6e64 2d74 6869 6e67 732d 7769  bs-and-things-wi
-00000a30: 7468 2d6d 656d 6272 616e 6573 2729 0d0a  th-membranes')..
-00000a40: 4074 696d 655f 736c 6963 6572 0d0a 6465  @time_slicer..de
-00000a50: 6620 7370 6c69 745f 746f 7563 6869 6e67  f split_touching
-00000a60: 5f6f 626a 6563 7473 2862 696e 6172 793a  _objects(binary:
-00000a70: 226e 6170 6172 692e 7479 7065 732e 4c61  "napari.types.La
-00000a80: 6265 6c73 4461 7461 222c 2073 6967 6d61  belsData", sigma
-00000a90: 3a20 666c 6f61 7420 3d20 332e 3529 202d  : float = 3.5) -
-00000aa0: 3e20 226e 6170 6172 692e 7479 7065 732e  > "napari.types.
-00000ab0: 4c61 6265 6c73 4461 7461 223a 0d0a 2020  LabelsData":..  
-00000ac0: 2020 2222 220d 0a20 2020 2054 616b 6573    """..    Takes
-00000ad0: 2061 2062 696e 6172 7920 696d 6167 6520   a binary image 
-00000ae0: 616e 6420 6472 6177 7320 6375 7473 2069  and draws cuts i
-00000af0: 6e20 7468 6520 6f62 6a65 6374 7320 7369  n the objects si
-00000b00: 6d69 6c61 7220 746f 2074 6865 2049 6d61  milar to the Ima
-00000b10: 6765 4a20 7761 7465 7273 6865 6420 616c  geJ watershed al
-00000b20: 676f 7269 7468 6d20 5b31 5d2e 0d0a 0d0a  gorithm [1].....
-00000b30: 2020 2020 5468 6973 2061 6c6c 6f77 7320      This allows 
-00000b40: 6375 7474 696e 6720 636f 6e6e 6563 7465  cutting connecte
-00000b50: 6420 6f62 6a65 6374 7320 7375 6368 2061  d objects such a
-00000b60: 7320 6e6f 7420 746f 2064 656e 7365 206e  s not to dense n
-00000b70: 7563 6c65 692e 2049 6620 7468 6520 6e75  uclei. If the nu
-00000b80: 636c 6569 2061 7265 2074 6f6f 2064 656e  clei are too den
-00000b90: 7365 2c0d 0a20 2020 2063 6f6e 7369 6465  se,..    conside
-00000ba0: 7220 7573 696e 6720 7374 6172 6469 7374  r using stardist
-00000bb0: 205b 325d 206f 7220 6365 6c6c 706f 7365   [2] or cellpose
-00000bc0: 205b 335d 2e0d 0a0d 0a20 2020 2053 6565   [3].....    See
-00000bd0: 2061 6c73 6f0d 0a20 2020 202d 2d2d 2d2d   also..    -----
-00000be0: 2d2d 2d0d 0a20 2020 202e 2e20 5b31 5d20  ---..    .. [1] 
-00000bf0: 6874 7470 733a 2f2f 696d 6167 656a 2e6e  https://imagej.n
-00000c00: 6968 2e67 6f76 2f69 6a2f 646f 6373 2f6d  ih.gov/ij/docs/m
-00000c10: 656e 7573 2f70 726f 6365 7373 2e68 746d  enus/process.htm
-00000c20: 6c23 7761 7465 7273 6865 640d 0a20 2020  l#watershed..   
-00000c30: 202e 2e20 5b32 5d20 6874 7470 733a 2f2f   .. [2] https://
-00000c40: 7777 772e 6e61 7061 7269 2d68 7562 2e6f  www.napari-hub.o
-00000c50: 7267 2f70 6c75 6769 6e73 2f73 7461 7264  rg/plugins/stard
-00000c60: 6973 742d 6e61 7061 7269 0d0a 2020 2020  ist-napari..    
-00000c70: 2e2e 205b 335d 2068 7474 7073 3a2f 2f77  .. [3] https://w
-00000c80: 7777 2e6e 6170 6172 692d 6875 622e 6f72  ww.napari-hub.or
-00000c90: 672f 706c 7567 696e 732f 6365 6c6c 706f  g/plugins/cellpo
-00000ca0: 7365 2d6e 6170 6172 690d 0a20 2020 2022  se-napari..    "
-00000cb0: 2222 0d0a 2020 2020 6269 6e61 7279 203d  ""..    binary =
-00000cc0: 206e 702e 6173 6172 7261 7928 6269 6e61   np.asarray(bina
-00000cd0: 7279 290d 0a0d 0a20 2020 2023 2074 7970  ry)....    # typ
-00000ce0: 6963 616c 2077 6179 206f 6620 7573 696e  ical way of usin
-00000cf0: 6720 7363 696b 6974 2d69 6d61 6765 2077  g scikit-image w
-00000d00: 6174 6572 7368 6564 0d0a 2020 2020 6469  atershed..    di
-00000d10: 7374 616e 6365 203d 206e 6469 2e64 6973  stance = ndi.dis
-00000d20: 7461 6e63 655f 7472 616e 7366 6f72 6d5f  tance_transform_
-00000d30: 6564 7428 6269 6e61 7279 290d 0a20 2020  edt(binary)..   
-00000d40: 2062 6c75 7272 6564 5f64 6973 7461 6e63   blurred_distanc
-00000d50: 6520 3d20 6761 7573 7369 616e 2864 6973  e = gaussian(dis
-00000d60: 7461 6e63 652c 2073 6967 6d61 3d73 6967  tance, sigma=sig
-00000d70: 6d61 290d 0a20 2020 2066 7020 3d20 6e70  ma)..    fp = np
-00000d80: 2e6f 6e65 7328 2833 2c29 202a 2062 696e  .ones((3,) * bin
-00000d90: 6172 792e 6e64 696d 290d 0a20 2020 2063  ary.ndim)..    c
-00000da0: 6f6f 7264 7320 3d20 7065 616b 5f6c 6f63  oords = peak_loc
-00000db0: 616c 5f6d 6178 2862 6c75 7272 6564 5f64  al_max(blurred_d
-00000dc0: 6973 7461 6e63 652c 2066 6f6f 7470 7269  istance, footpri
-00000dd0: 6e74 3d66 702c 206c 6162 656c 733d 6269  nt=fp, labels=bi
-00000de0: 6e61 7279 290d 0a20 2020 206d 6173 6b20  nary)..    mask 
-00000df0: 3d20 6e70 2e7a 6572 6f73 2864 6973 7461  = np.zeros(dista
-00000e00: 6e63 652e 7368 6170 652c 2064 7479 7065  nce.shape, dtype
-00000e10: 3d62 6f6f 6c29 0d0a 2020 2020 6d61 736b  =bool)..    mask
-00000e20: 5b74 7570 6c65 2863 6f6f 7264 732e 5429  [tuple(coords.T)
-00000e30: 5d20 3d20 5472 7565 0d0a 2020 2020 6d61  ] = True..    ma
-00000e40: 726b 6572 7320 3d20 6c61 6265 6c28 6d61  rkers = label(ma
-00000e50: 736b 290d 0a20 2020 206c 6162 656c 7320  sk)..    labels 
-00000e60: 3d20 7761 7465 7273 6865 6428 2d62 6c75  = watershed(-blu
-00000e70: 7272 6564 5f64 6973 7461 6e63 652c 206d  rred_distance, m
-00000e80: 6172 6b65 7273 2c20 6d61 736b 3d62 696e  arkers, mask=bin
-00000e90: 6172 7929 0d0a 0d0a 2020 2020 2320 6964  ary)....    # id
-00000ea0: 656e 7469 6679 206c 6162 656c 2d63 7574  entify label-cut
-00000eb0: 7469 6e67 2065 6467 6573 0d0a 2020 2020  ting edges..    
-00000ec0: 6966 206c 656e 2862 696e 6172 792e 7368  if len(binary.sh
-00000ed0: 6170 6529 203d 3d20 323a 0d0a 2020 2020  ape) == 2:..    
-00000ee0: 2020 2020 6564 6765 7320 3d20 736f 6265      edges = sobe
-00000ef0: 6c28 6c61 6265 6c73 290d 0a20 2020 2020  l(labels)..     
-00000f00: 2020 2065 6467 6573 3220 3d20 736f 6265     edges2 = sobe
-00000f10: 6c28 6269 6e61 7279 290d 0a20 2020 2065  l(binary)..    e
-00000f20: 6c73 653a 2023 2061 7373 756d 696e 6720  lse: # assuming 
-00000f30: 3344 0d0a 2020 2020 2020 2020 6564 6765  3D..        edge
-00000f40: 7320 3d20 5f73 6f62 656c 5f33 6428 6c61  s = _sobel_3d(la
-00000f50: 6265 6c73 290d 0a20 2020 2020 2020 2065  bels)..        e
-00000f60: 6467 6573 3220 3d20 5f73 6f62 656c 5f33  dges2 = _sobel_3
-00000f70: 6428 6269 6e61 7279 290d 0a0d 0a20 2020  d(binary)....   
-00000f80: 2061 6c6d 6f73 7420 3d20 6e70 2e6c 6f67   almost = np.log
-00000f90: 6963 616c 5f6e 6f74 286e 702e 6c6f 6769  ical_not(np.logi
-00000fa0: 6361 6c5f 786f 7228 6564 6765 7320 213d  cal_xor(edges !=
-00000fb0: 2030 2c20 6564 6765 7332 2021 3d20 3029   0, edges2 != 0)
-00000fc0: 2920 2a20 6269 6e61 7279 0d0a 2020 2020  ) * binary..    
-00000fd0: 7265 7475 726e 2062 696e 6172 795f 6f70  return binary_op
-00000fe0: 656e 696e 6728 616c 6d6f 7374 290d 0a0d  ening(almost)...
-00000ff0: 0a0d 0a40 7265 6769 7374 6572 5f66 756e  ...@register_fun
-00001000: 6374 696f 6e28 6d65 6e75 3d22 5365 676d  ction(menu="Segm
-00001010: 656e 7461 7469 6f6e 202f 2062 696e 6172  entation / binar
-00001020: 697a 6174 696f 6e20 3e20 5468 7265 7368  ization > Thresh
-00001030: 6f6c 6420 284f 7473 7520 6574 2061 6c20  old (Otsu et al 
-00001040: 3139 3739 2c20 7363 696b 6974 2d69 6d61  1979, scikit-ima
-00001050: 6765 2c20 6e73 6261 7477 6d29 2229 0d0a  ge, nsbatwm)")..
-00001060: 406a 7570 7974 6572 5f64 6973 706c 6179  @jupyter_display
-00001070: 6162 6c65 5f6f 7574 7075 7428 6c69 6272  able_output(libr
-00001080: 6172 795f 6e61 6d65 3d27 6e73 6261 7477  ary_name='nsbatw
-00001090: 6d27 2c20 6865 6c70 5f75 726c 3d27 6874  m', help_url='ht
-000010a0: 7470 733a 2f2f 7777 772e 6e61 7061 7269  tps://www.napari
-000010b0: 2d68 7562 2e6f 7267 2f70 6c75 6769 6e73  -hub.org/plugins
-000010c0: 2f6e 6170 6172 692d 7365 676d 656e 742d  /napari-segment-
-000010d0: 626c 6f62 732d 616e 642d 7468 696e 6773  blobs-and-things
-000010e0: 2d77 6974 682d 6d65 6d62 7261 6e65 7327  -with-membranes'
-000010f0: 290d 0a40 7469 6d65 5f73 6c69 6365 720d  )..@time_slicer.
-00001100: 0a64 6566 2074 6872 6573 686f 6c64 5f6f  .def threshold_o
-00001110: 7473 7528 696d 6167 653a 226e 6170 6172  tsu(image:"napar
-00001120: 692e 7479 7065 732e 496d 6167 6544 6174  i.types.ImageDat
-00001130: 6122 2920 2d3e 2022 6e61 7061 7269 2e74  a") -> "napari.t
-00001140: 7970 6573 2e4c 6162 656c 7344 6174 6122  ypes.LabelsData"
-00001150: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-00001160: 4170 706c 6965 7320 4f74 7375 2773 2074  Applies Otsu's t
-00001170: 6872 6573 686f 6c64 2073 656c 6563 7469  hreshold selecti
-00001180: 6f6e 206d 6574 686f 6420 746f 2061 6e20  on method to an 
-00001190: 696e 7465 6e73 6974 7920 696d 6167 6520  intensity image 
-000011a0: 616e 6420 7265 7475 726e 7320 6120 6269  and returns a bi
-000011b0: 6e61 7279 2069 6d61 6765 2077 6974 6820  nary image with 
-000011c0: 7069 7865 6c73 3d3d 3120 7768 6572 650d  pixels==1 where.
-000011d0: 0a20 2020 2069 6e74 656e 7369 7479 2069  .    intensity i
-000011e0: 7320 6162 6f76 6520 7468 6520 6465 7465  s above the dete
-000011f0: 726d 696e 6564 2074 6872 6573 686f 6c64  rmined threshold
-00001200: 2e0d 0a0d 0a20 2020 2053 6565 2061 6c73  .....    See als
-00001210: 6f0d 0a20 2020 202d 2d2d 2d2d 2d2d 2d0d  o..    --------.
-00001220: 0a20 2020 202e 2e20 5b30 5d20 6874 7470  .    .. [0] http
-00001230: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
-00001240: 2e6f 7267 2f77 696b 692f 4f74 7375 2532  .org/wiki/Otsu%2
-00001250: 3773 5f6d 6574 686f 640d 0a20 2020 202e  7s_method..    .
-00001260: 2e20 5b31 5d20 6874 7470 733a 2f2f 6965  . [1] https://ie
-00001270: 6565 7870 6c6f 7265 2e69 6565 652e 6f72  eexplore.ieee.or
-00001280: 672f 646f 6375 6d65 6e74 2f34 3331 3030  g/document/43100
-00001290: 3736 0d0a 2020 2020 2222 220d 0a20 2020  76..    """..   
-000012a0: 2074 6872 6573 686f 6c64 203d 2073 6b5f   threshold = sk_
-000012b0: 7468 7265 7368 6f6c 645f 6f74 7375 286e  threshold_otsu(n
-000012c0: 702e 6173 6172 7261 7928 696d 6167 6529  p.asarray(image)
-000012d0: 290d 0a20 2020 2062 696e 6172 795f 6f74  )..    binary_ot
-000012e0: 7375 203d 2069 6d61 6765 203e 2074 6872  su = image > thr
-000012f0: 6573 686f 6c64 0d0a 0d0a 2020 2020 7265  eshold....    re
-00001300: 7475 726e 2062 696e 6172 795f 6f74 7375  turn binary_otsu
-00001310: 202a 2031 0d0a 0d0a 0d0a 4072 6567 6973   * 1......@regis
-00001320: 7465 725f 6675 6e63 7469 6f6e 286d 656e  ter_function(men
-00001330: 753d 2253 6567 6d65 6e74 6174 696f 6e20  u="Segmentation 
-00001340: 2f20 6269 6e61 7269 7a61 7469 6f6e 203e  / binarization >
-00001350: 2054 6872 6573 686f 6c64 2028 5965 6e20   Threshold (Yen 
-00001360: 6574 2061 6c20 3139 3935 2c20 7363 696b  et al 1995, scik
-00001370: 6974 2d69 6d61 6765 2c20 6e73 6261 7477  it-image, nsbatw
-00001380: 6d29 2229 0d0a 406a 7570 7974 6572 5f64  m)")..@jupyter_d
-00001390: 6973 706c 6179 6162 6c65 5f6f 7574 7075  isplayable_outpu
-000013a0: 7428 6c69 6272 6172 795f 6e61 6d65 3d27  t(library_name='
-000013b0: 6e73 6261 7477 6d27 2c20 6865 6c70 5f75  nsbatwm', help_u
-000013c0: 726c 3d27 6874 7470 733a 2f2f 7777 772e  rl='https://www.
-000013d0: 6e61 7061 7269 2d68 7562 2e6f 7267 2f70  napari-hub.org/p
-000013e0: 6c75 6769 6e73 2f6e 6170 6172 692d 7365  lugins/napari-se
-000013f0: 676d 656e 742d 626c 6f62 732d 616e 642d  gment-blobs-and-
-00001400: 7468 696e 6773 2d77 6974 682d 6d65 6d62  things-with-memb
-00001410: 7261 6e65 7327 290d 0a40 7469 6d65 5f73  ranes')..@time_s
-00001420: 6c69 6365 720d 0a64 6566 2074 6872 6573  licer..def thres
-00001430: 686f 6c64 5f79 656e 2869 6d61 6765 203a  hold_yen(image :
-00001440: 226e 6170 6172 692e 7479 7065 732e 496d  "napari.types.Im
-00001450: 6167 6544 6174 6122 2920 2d3e 2022 6e61  ageData") -> "na
-00001460: 7061 7269 2e74 7970 6573 2e4c 6162 656c  pari.types.Label
-00001470: 7344 6174 6122 3a0d 0a20 2020 2022 2222  sData":..    """
-00001480: 0d0a 2020 2020 4269 6e61 7269 7a65 2061  ..    Binarize a
-00001490: 6e20 696d 6167 6520 7573 696e 6720 5965  n image using Ye
-000014a0: 6e27 7320 6d65 7468 6f64 2e0d 0a0d 0a20  n's method..... 
-000014b0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-000014c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-000014d0: 2020 2069 6d61 6765 3a20 496d 6167 650d     image: Image.
-000014e0: 0a0d 0a20 2020 2053 6565 2041 6c73 6f0d  ...    See Also.
-000014f0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20  .    --------.. 
-00001500: 2020 202e 2e5b 305d 2068 7474 7073 3a2f     ..[0] https:/
-00001510: 2f69 6d61 6765 6a2e 6e65 742f 706c 7567  /imagej.net/plug
-00001520: 696e 732f 6175 746f 2d74 6872 6573 686f  ins/auto-thresho
-00001530: 6c64 2379 656e 0d0a 0d0a 2020 2020 5265  ld#yen....    Re
-00001540: 7475 726e 730d 0a20 2020 202d 2d2d 2d2d  turns..    -----
-00001550: 2d2d 0d0a 2020 2020 6269 6e61 7279 5f69  --..    binary_i
-00001560: 6d61 6765 3a20 6e61 7061 7269 2e74 7970  mage: napari.typ
-00001570: 6573 2e4c 6162 656c 7344 6174 610d 0a20  es.LabelsData.. 
-00001580: 2020 2022 2222 0d0a 2020 2020 7265 7475     """..    retu
-00001590: 726e 2069 6d61 6765 203e 2066 696c 7465  rn image > filte
-000015a0: 7273 2e74 6872 6573 686f 6c64 5f79 656e  rs.threshold_yen
-000015b0: 2869 6d61 6765 290d 0a0d 0a0d 0a40 7265  (image)......@re
-000015c0: 6769 7374 6572 5f66 756e 6374 696f 6e28  gister_function(
-000015d0: 6d65 6e75 3d22 5365 676d 656e 7461 7469  menu="Segmentati
-000015e0: 6f6e 202f 2062 696e 6172 697a 6174 696f  on / binarizatio
-000015f0: 6e20 3e20 5468 7265 7368 6f6c 6420 2849  n > Threshold (I
-00001600: 736f 6461 7461 2c20 5269 646c 6572 2065  sodata, Ridler e
-00001610: 7420 616c 2031 3937 382c 2073 6369 6b69  t al 1978, sciki
-00001620: 742d 696d 6167 652c 206e 7362 6174 776d  t-image, nsbatwm
-00001630: 2922 290d 0a40 6a75 7079 7465 725f 6469  )")..@jupyter_di
-00001640: 7370 6c61 7961 626c 655f 6f75 7470 7574  splayable_output
-00001650: 286c 6962 7261 7279 5f6e 616d 653d 276e  (library_name='n
-00001660: 7362 6174 776d 272c 2068 656c 705f 7572  sbatwm', help_ur
-00001670: 6c3d 2768 7474 7073 3a2f 2f77 7777 2e6e  l='https://www.n
-00001680: 6170 6172 692d 6875 622e 6f72 672f 706c  apari-hub.org/pl
-00001690: 7567 696e 732f 6e61 7061 7269 2d73 6567  ugins/napari-seg
-000016a0: 6d65 6e74 2d62 6c6f 6273 2d61 6e64 2d74  ment-blobs-and-t
-000016b0: 6869 6e67 732d 7769 7468 2d6d 656d 6272  hings-with-membr
-000016c0: 616e 6573 2729 0d0a 4074 696d 655f 736c  anes')..@time_sl
-000016d0: 6963 6572 0d0a 6465 6620 7468 7265 7368  icer..def thresh
-000016e0: 6f6c 645f 6973 6f64 6174 6128 696d 6167  old_isodata(imag
-000016f0: 6520 3a22 6e61 7061 7269 2e74 7970 6573  e :"napari.types
-00001700: 2e49 6d61 6765 4461 7461 2229 202d 3e20  .ImageData") -> 
-00001710: 226e 6170 6172 692e 7479 7065 732e 4c61  "napari.types.La
-00001720: 6265 6c73 4461 7461 223a 0d0a 2020 2020  belsData":..    
-00001730: 2222 220d 0a20 2020 2042 696e 6172 697a  """..    Binariz
-00001740: 6520 616e 2069 6d61 6765 2075 7369 6e67  e an image using
-00001750: 2074 6865 2049 736f 4461 7461 202f 2052   the IsoData / R
-00001760: 6964 6c65 7227 7320 6d65 7468 6f64 2e0d  idler's method..
-00001770: 0a20 2020 2054 6865 206d 6574 686f 6420  .    The method 
-00001780: 6973 2073 696d 696c 6172 2074 6f20 496d  is similar to Im
-00001790: 6167 654a 2773 2022 6465 6661 756c 7422  ageJ's "default"
-000017a0: 2074 6872 6573 686f 6c64 2e0d 0a0d 0a20   threshold..... 
-000017b0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-000017c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-000017d0: 2020 2069 6d61 6765 3a20 496d 6167 650d     image: Image.
-000017e0: 0a0d 0a20 2020 2053 6565 2041 6c73 6f0d  ...    See Also.
-000017f0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20  .    --------.. 
-00001800: 2020 202e 2e5b 305d 2068 7474 7073 3a2f     ..[0] https:/
-00001810: 2f69 6d61 6765 6a2e 6e65 742f 706c 7567  /imagej.net/plug
-00001820: 696e 732f 6175 746f 2d74 6872 6573 686f  ins/auto-thresho
-00001830: 6c64 2369 736f 6461 7461 0d0a 2020 2020  ld#isodata..    
-00001840: 2e2e 5b31 5d20 6874 7470 733a 2f2f 6965  ..[1] https://ie
-00001850: 6565 7870 6c6f 7265 2e69 6565 652e 6f72  eexplore.ieee.or
-00001860: 672f 646f 6375 6d65 6e74 2f34 3331 3030  g/document/43100
-00001870: 3339 0d0a 0d0a 2020 2020 5265 7475 726e  39....    Return
-00001880: 730d 0a20 2020 202d 2d2d 2d2d 2d2d 0d0a  s..    -------..
-00001890: 2020 2020 6269 6e61 7279 5f69 6d61 6765      binary_image
-000018a0: 3a20 6e61 7061 7269 2e74 7970 6573 2e4c  : napari.types.L
-000018b0: 6162 656c 7344 6174 610d 0a20 2020 2022  abelsData..    "
-000018c0: 2222 0d0a 2020 2020 7265 7475 726e 2069  ""..    return i
-000018d0: 6d61 6765 203e 2066 696c 7465 7273 2e74  mage > filters.t
-000018e0: 6872 6573 686f 6c64 5f69 736f 6461 7461  hreshold_isodata
-000018f0: 2869 6d61 6765 290d 0a0d 0a0d 0a40 7265  (image)......@re
-00001900: 6769 7374 6572 5f66 756e 6374 696f 6e28  gister_function(
-00001910: 6d65 6e75 3d22 5365 676d 656e 7461 7469  menu="Segmentati
-00001920: 6f6e 202f 2062 696e 6172 697a 6174 696f  on / binarizatio
-00001930: 6e20 3e20 5468 7265 7368 6f6c 6420 284c  n > Threshold (L
-00001940: 6920 6574 2061 6c20 3139 3933 2c20 7363  i et al 1993, sc
-00001950: 696b 6974 2d69 6d61 6765 2c20 6e73 6261  ikit-image, nsba
-00001960: 7477 6d29 2229 0d0a 406a 7570 7974 6572  twm)")..@jupyter
-00001970: 5f64 6973 706c 6179 6162 6c65 5f6f 7574  _displayable_out
-00001980: 7075 7428 6c69 6272 6172 795f 6e61 6d65  put(library_name
-00001990: 3d27 6e73 6261 7477 6d27 2c20 6865 6c70  ='nsbatwm', help
-000019a0: 5f75 726c 3d27 6874 7470 733a 2f2f 7777  _url='https://ww
-000019b0: 772e 6e61 7061 7269 2d68 7562 2e6f 7267  w.napari-hub.org
-000019c0: 2f70 6c75 6769 6e73 2f6e 6170 6172 692d  /plugins/napari-
-000019d0: 7365 676d 656e 742d 626c 6f62 732d 616e  segment-blobs-an
-000019e0: 642d 7468 696e 6773 2d77 6974 682d 6d65  d-things-with-me
-000019f0: 6d62 7261 6e65 7327 290d 0a40 7469 6d65  mbranes')..@time
-00001a00: 5f73 6c69 6365 720d 0a64 6566 2074 6872  _slicer..def thr
-00001a10: 6573 686f 6c64 5f6c 6928 696d 6167 653a  eshold_li(image:
-00001a20: 226e 6170 6172 692e 7479 7065 732e 496d  "napari.types.Im
-00001a30: 6167 6544 6174 6122 2920 2d3e 2022 6e61  ageData") -> "na
-00001a40: 7061 7269 2e74 7970 6573 2e4c 6162 656c  pari.types.Label
-00001a50: 7344 6174 6122 3a0d 0a20 2020 2022 2222  sData":..    """
-00001a60: 0d0a 2020 2020 4269 6e61 7269 7a65 2061  ..    Binarize a
-00001a70: 6e20 696d 6167 6520 7573 696e 6720 4c69  n image using Li
-00001a80: 2773 206d 6574 686f 6420 6d65 7468 6f64  's method method
-00001a90: 2e0d 0a0d 0a20 2020 2050 6172 616d 6574  .....    Paramet
-00001aa0: 6572 730d 0a20 2020 202d 2d2d 2d2d 2d2d  ers..    -------
-00001ab0: 2d2d 2d0d 0a20 2020 2069 6d61 6765 3a20  ---..    image: 
-00001ac0: 496d 6167 650d 0a0d 0a20 2020 2053 6565  Image....    See
-00001ad0: 2041 6c73 6f0d 0a20 2020 202d 2d2d 2d2d   Also..    -----
-00001ae0: 2d2d 2d0d 0a20 2020 202e 2e5b 305d 2068  ---..    ..[0] h
-00001af0: 7474 7073 3a2f 2f69 6d61 6765 6a2e 6e65  ttps://imagej.ne
-00001b00: 742f 706c 7567 696e 732f 6175 746f 2d74  t/plugins/auto-t
-00001b10: 6872 6573 686f 6c64 236c 690d 0a0d 0a20  hreshold#li.... 
-00001b20: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-00001b30: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2062 696e  -------..    bin
-00001b40: 6172 795f 696d 6167 653a 206e 6170 6172  ary_image: napar
-00001b50: 692e 7479 7065 732e 4c61 6265 6c73 4461  i.types.LabelsDa
-00001b60: 7461 0d0a 2020 2020 2222 220d 0a20 2020  ta..    """..   
-00001b70: 2072 6574 7572 6e20 696d 6167 6520 3e20   return image > 
-00001b80: 6669 6c74 6572 732e 7468 7265 7368 6f6c  filters.threshol
-00001b90: 645f 6c69 2869 6d61 6765 290d 0a0d 0a0d  d_li(image).....
-00001ba0: 0a40 7265 6769 7374 6572 5f66 756e 6374  .@register_funct
-00001bb0: 696f 6e28 6d65 6e75 3d22 5365 676d 656e  ion(menu="Segmen
-00001bc0: 7461 7469 6f6e 202f 2062 696e 6172 697a  tation / binariz
-00001bd0: 6174 696f 6e20 3e20 5468 7265 7368 6f6c  ation > Threshol
-00001be0: 6420 2852 6964 6c65 7220 6574 2061 6c20  d (Ridler et al 
-00001bf0: 3139 3738 2c20 7363 696b 6974 2d69 6d61  1978, scikit-ima
-00001c00: 6765 2c20 6e73 6261 7477 6d29 2229 0d0a  ge, nsbatwm)")..
-00001c10: 406a 7570 7974 6572 5f64 6973 706c 6179  @jupyter_display
-00001c20: 6162 6c65 5f6f 7574 7075 7428 6c69 6272  able_output(libr
-00001c30: 6172 795f 6e61 6d65 3d27 6e73 6261 7477  ary_name='nsbatw
-00001c40: 6d27 2c20 6865 6c70 5f75 726c 3d27 6874  m', help_url='ht
-00001c50: 7470 733a 2f2f 7777 772e 6e61 7061 7269  tps://www.napari
-00001c60: 2d68 7562 2e6f 7267 2f70 6c75 6769 6e73  -hub.org/plugins
-00001c70: 2f6e 6170 6172 692d 7365 676d 656e 742d  /napari-segment-
-00001c80: 626c 6f62 732d 616e 642d 7468 696e 6773  blobs-and-things
-00001c90: 2d77 6974 682d 6d65 6d62 7261 6e65 7327  -with-membranes'
-00001ca0: 290d 0a40 7469 6d65 5f73 6c69 6365 720d  )..@time_slicer.
-00001cb0: 0a64 6566 2074 6872 6573 686f 6c64 5f6d  .def threshold_m
-00001cc0: 6561 6e28 696d 6167 6520 3a22 6e61 7061  ean(image :"napa
-00001cd0: 7269 2e74 7970 6573 2e49 6d61 6765 4461  ri.types.ImageDa
-00001ce0: 7461 2229 202d 3e20 226e 6170 6172 692e  ta") -> "napari.
-00001cf0: 7479 7065 732e 4c61 6265 6c73 4461 7461  types.LabelsData
-00001d00: 223a 0d0a 2020 2020 2222 220d 0a20 2020  ":..    """..   
-00001d10: 2042 696e 6172 697a 6520 616e 2069 6d61   Binarize an ima
-00001d20: 6765 2075 7369 6e67 2074 6865 204d 6561  ge using the Mea
-00001d30: 6e20 6d65 7468 6f64 2e0d 0a0d 0a20 2020  n method.....   
-00001d40: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
-00001d50: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
-00001d60: 2069 6d61 6765 3a20 496d 6167 650d 0a0d   image: Image...
-00001d70: 0a20 2020 2053 6565 2041 6c73 6f0d 0a20  .    See Also.. 
-00001d80: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
-00001d90: 202e 2e5b 305d 2068 7474 7073 3a2f 2f69   ..[0] https://i
-00001da0: 6d61 6765 6a2e 6e65 742f 706c 7567 696e  magej.net/plugin
-00001db0: 732f 6175 746f 2d74 6872 6573 686f 6c64  s/auto-threshold
-00001dc0: 236d 6561 6e0d 0a0d 0a20 2020 2052 6574  #mean....    Ret
-00001dd0: 7572 6e73 0d0a 2020 2020 2d2d 2d2d 2d2d  urns..    ------
-00001de0: 2d0d 0a20 2020 2062 696e 6172 795f 696d  -..    binary_im
-00001df0: 6167 653a 206e 6170 6172 692e 7479 7065  age: napari.type
-00001e00: 732e 4c61 6265 6c73 4461 7461 0d0a 2020  s.LabelsData..  
-00001e10: 2020 2222 220d 0a20 2020 2072 6574 7572    """..    retur
-00001e20: 6e20 696d 6167 6520 3e20 6669 6c74 6572  n image > filter
-00001e30: 732e 7468 7265 7368 6f6c 645f 6d65 616e  s.threshold_mean
-00001e40: 2869 6d61 6765 290d 0a0d 0a0d 0a40 7265  (image)......@re
-00001e50: 6769 7374 6572 5f66 756e 6374 696f 6e28  gister_function(
-00001e60: 6d65 6e75 3d22 5365 676d 656e 7461 7469  menu="Segmentati
-00001e70: 6f6e 202f 2062 696e 6172 697a 6174 696f  on / binarizatio
-00001e80: 6e20 3e20 5468 7265 7368 6f6c 6420 284d  n > Threshold (M
-00001e90: 6561 6e2c 2073 6369 6b69 742d 696d 6167  ean, scikit-imag
-00001ea0: 652c 206e 7362 6174 776d 2922 290d 0a40  e, nsbatwm)")..@
-00001eb0: 6a75 7079 7465 725f 6469 7370 6c61 7961  jupyter_displaya
-00001ec0: 626c 655f 6f75 7470 7574 286c 6962 7261  ble_output(libra
-00001ed0: 7279 5f6e 616d 653d 276e 7362 6174 776d  ry_name='nsbatwm
-00001ee0: 272c 2068 656c 705f 7572 6c3d 2768 7474  ', help_url='htt
-00001ef0: 7073 3a2f 2f77 7777 2e6e 6170 6172 692d  ps://www.napari-
-00001f00: 6875 622e 6f72 672f 706c 7567 696e 732f  hub.org/plugins/
-00001f10: 6e61 7061 7269 2d73 6567 6d65 6e74 2d62  napari-segment-b
-00001f20: 6c6f 6273 2d61 6e64 2d74 6869 6e67 732d  lobs-and-things-
-00001f30: 7769 7468 2d6d 656d 6272 616e 6573 2729  with-membranes')
-00001f40: 0d0a 4074 696d 655f 736c 6963 6572 0d0a  ..@time_slicer..
-00001f50: 6465 6620 7468 7265 7368 6f6c 645f 6d69  def threshold_mi
-00001f60: 6e69 6d75 6d28 696d 6167 6520 3a22 6e61  nimum(image :"na
-00001f70: 7061 7269 2e74 7970 6573 2e49 6d61 6765  pari.types.Image
-00001f80: 4461 7461 2229 202d 3e20 226e 6170 6172  Data") -> "napar
-00001f90: 692e 7479 7065 732e 4c61 6265 6c73 4461  i.types.LabelsDa
-00001fa0: 7461 223a 0d0a 2020 2020 2222 220d 0a20  ta":..    """.. 
-00001fb0: 2020 2042 696e 6172 697a 6520 616e 2069     Binarize an i
-00001fc0: 6d61 6765 2075 7369 6e67 2074 6865 204d  mage using the M
-00001fd0: 696e 696d 756d 206d 6574 686f 642e 0d0a  inimum method...
-00001fe0: 0d0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00001ff0: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  ..    ----------
-00002000: 0d0a 2020 2020 696d 6167 653a 2049 6d61  ..    image: Ima
-00002010: 6765 0d0a 0d0a 2020 2020 5365 6520 416c  ge....    See Al
-00002020: 736f 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d  so..    --------
-00002030: 0d0a 2020 2020 2e2e 5b30 5d20 6874 7470  ..    ..[0] http
-00002040: 733a 2f2f 696d 6167 656a 2e6e 6574 2f70  s://imagej.net/p
-00002050: 6c75 6769 6e73 2f61 7574 6f2d 7468 7265  lugins/auto-thre
-00002060: 7368 6f6c 6423 6d69 6e69 6d75 6d0d 0a0d  shold#minimum...
-00002070: 0a20 2020 2052 6574 7572 6e73 0d0a 2020  .    Returns..  
-00002080: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2062    -------..    b
-00002090: 696e 6172 795f 696d 6167 653a 206e 6170  inary_image: nap
-000020a0: 6172 692e 7479 7065 732e 4c61 6265 6c73  ari.types.Labels
-000020b0: 4461 7461 0d0a 2020 2020 2222 220d 0a20  Data..    """.. 
-000020c0: 2020 2072 6574 7572 6e20 696d 6167 6520     return image 
-000020d0: 3e20 6669 6c74 6572 732e 7468 7265 7368  > filters.thresh
-000020e0: 6f6c 645f 6d69 6e69 6d75 6d28 696d 6167  old_minimum(imag
-000020f0: 6529 0d0a 0d0a 0d0a 4072 6567 6973 7465  e)......@registe
-00002100: 725f 6675 6e63 7469 6f6e 286d 656e 753d  r_function(menu=
-00002110: 2253 6567 6d65 6e74 6174 696f 6e20 2f20  "Segmentation / 
-00002120: 6269 6e61 7269 7a61 7469 6f6e 203e 2054  binarization > T
-00002130: 6872 6573 686f 6c64 2028 5472 6961 6e67  hreshold (Triang
-00002140: 6c65 206d 6574 686f 642c 205a 6163 6b20  le method, Zack 
-00002150: 6574 2061 6c20 3139 3737 2c20 7363 696b  et al 1977, scik
-00002160: 6974 2d69 6d61 6765 2c20 6e73 6261 7477  it-image, nsbatw
-00002170: 6d29 2229 0d0a 406a 7570 7974 6572 5f64  m)")..@jupyter_d
-00002180: 6973 706c 6179 6162 6c65 5f6f 7574 7075  isplayable_outpu
-00002190: 7428 6c69 6272 6172 795f 6e61 6d65 3d27  t(library_name='
-000021a0: 6e73 6261 7477 6d27 2c20 6865 6c70 5f75  nsbatwm', help_u
-000021b0: 726c 3d27 6874 7470 733a 2f2f 7777 772e  rl='https://www.
-000021c0: 6e61 7061 7269 2d68 7562 2e6f 7267 2f70  napari-hub.org/p
-000021d0: 6c75 6769 6e73 2f6e 6170 6172 692d 7365  lugins/napari-se
-000021e0: 676d 656e 742d 626c 6f62 732d 616e 642d  gment-blobs-and-
-000021f0: 7468 696e 6773 2d77 6974 682d 6d65 6d62  things-with-memb
-00002200: 7261 6e65 7327 290d 0a40 7469 6d65 5f73  ranes')..@time_s
-00002210: 6c69 6365 720d 0a64 6566 2074 6872 6573  licer..def thres
-00002220: 686f 6c64 5f74 7269 616e 676c 6528 696d  hold_triangle(im
-00002230: 6167 653a 226e 6170 6172 692e 7479 7065  age:"napari.type
-00002240: 732e 496d 6167 6544 6174 6122 2920 2d3e  s.ImageData") ->
-00002250: 2022 6e61 7061 7269 2e74 7970 6573 2e4c   "napari.types.L
-00002260: 6162 656c 7344 6174 6122 3a0d 0a20 2020  abelsData":..   
-00002270: 2022 2222 0d0a 2020 2020 4269 6e61 7269   """..    Binari
-00002280: 7a65 2061 6e20 696d 6167 6520 7573 696e  ze an image usin
-00002290: 6720 7468 6520 5472 6961 6e67 6c65 206d  g the Triangle m
-000022a0: 6574 686f 642e 0d0a 0d0a 2020 2020 5061  ethod.....    Pa
-000022b0: 7261 6d65 7465 7273 0d0a 2020 2020 2d2d  rameters..    --
-000022c0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 696d  --------..    im
-000022d0: 6167 653a 2049 6d61 6765 0d0a 0d0a 2020  age: Image....  
-000022e0: 2020 5365 6520 416c 736f 0d0a 2020 2020    See Also..    
-000022f0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2e2e  --------..    ..
-00002300: 5b30 5d20 6874 7470 733a 2f2f 696d 6167  [0] https://imag
-00002310: 656a 2e6e 6574 2f70 6c75 6769 6e73 2f61  ej.net/plugins/a
-00002320: 7574 6f2d 7468 7265 7368 6f6c 6423 7472  uto-threshold#tr
-00002330: 6961 6e67 6c65 0d0a 0d0a 2020 2020 5265  iangle....    Re
-00002340: 7475 726e 730d 0a20 2020 202d 2d2d 2d2d  turns..    -----
-00002350: 2d2d 0d0a 2020 2020 6269 6e61 7279 5f69  --..    binary_i
-00002360: 6d61 6765 3a20 6e61 7061 7269 2e74 7970  mage: napari.typ
-00002370: 6573 2e4c 6162 656c 7344 6174 610d 0a20  es.LabelsData.. 
-00002380: 2020 2022 2222 0d0a 2020 2020 7265 7475     """..    retu
-00002390: 726e 2069 6d61 6765 203e 2066 696c 7465  rn image > filte
-000023a0: 7273 2e74 6872 6573 686f 6c64 5f74 7269  rs.threshold_tri
-000023b0: 616e 676c 6528 696d 6167 6529 0d0a 0d0a  angle(image)....
-000023c0: 0d0a 4072 6567 6973 7465 725f 6675 6e63  ..@register_func
-000023d0: 7469 6f6e 286d 656e 753d 2246 696c 7465  tion(menu="Filte
-000023e0: 7269 6e67 202f 206e 6f69 7365 2072 656d  ring / noise rem
-000023f0: 6f76 616c 203e 2047 6175 7373 6961 6e20  oval > Gaussian 
-00002400: 2873 6369 6b69 742d 696d 6167 652c 206e  (scikit-image, n
-00002410: 7362 6174 776d 2922 290d 0a40 6a75 7079  sbatwm)")..@jupy
-00002420: 7465 725f 6469 7370 6c61 7961 626c 655f  ter_displayable_
-00002430: 6f75 7470 7574 286c 6962 7261 7279 5f6e  output(library_n
-00002440: 616d 653d 276e 7362 6174 776d 272c 2068  ame='nsbatwm', h
-00002450: 656c 705f 7572 6c3d 2768 7474 7073 3a2f  elp_url='https:/
-00002460: 2f77 7777 2e6e 6170 6172 692d 6875 622e  /www.napari-hub.
-00002470: 6f72 672f 706c 7567 696e 732f 6e61 7061  org/plugins/napa
-00002480: 7269 2d73 6567 6d65 6e74 2d62 6c6f 6273  ri-segment-blobs
-00002490: 2d61 6e64 2d74 6869 6e67 732d 7769 7468  -and-things-with
-000024a0: 2d6d 656d 6272 616e 6573 2729 0d0a 4074  -membranes')..@t
-000024b0: 696d 655f 736c 6963 6572 0d0a 6465 6620  ime_slicer..def 
-000024c0: 6761 7573 7369 616e 5f62 6c75 7228 696d  gaussian_blur(im
-000024d0: 6167 653a 226e 6170 6172 692e 7479 7065  age:"napari.type
-000024e0: 732e 496d 6167 6544 6174 6122 2c20 7369  s.ImageData", si
-000024f0: 676d 613a 2066 6c6f 6174 203d 2031 2920  gma: float = 1) 
-00002500: 2d3e 2022 6e61 7061 7269 2e74 7970 6573  -> "napari.types
-00002510: 2e49 6d61 6765 4461 7461 223a 0d0a 2020  .ImageData":..  
-00002520: 2020 2222 220d 0a20 2020 2041 7070 6c69    """..    Appli
-00002530: 6573 2061 2047 6175 7373 6961 6e20 626c  es a Gaussian bl
-00002540: 7572 2074 6f20 616e 2069 6d61 6765 2077  ur to an image w
-00002550: 6974 6820 6120 6465 6669 6e65 6420 7369  ith a defined si
-00002560: 676d 612e 2055 7365 6675 6c20 666f 7220  gma. Useful for 
-00002570: 6465 6e6f 6973 696e 672e 0d0a 2020 2020  denoising...    
-00002580: 2222 220d 0a20 2020 2072 6574 7572 6e20  """..    return 
-00002590: 6761 7573 7369 616e 2869 6d61 6765 2c20  gaussian(image, 
-000025a0: 7369 676d 6129 0d0a 0d0a 0d0a 4072 6567  sigma)......@reg
-000025b0: 6973 7465 725f 6675 6e63 7469 6f6e 286d  ister_function(m
-000025c0: 656e 753d 2246 696c 7465 7269 6e67 202f  enu="Filtering /
-000025d0: 2065 6467 6520 656e 6861 6e63 656d 656e   edge enhancemen
-000025e0: 7420 3e20 4761 7573 7369 616e 204c 6170  t > Gaussian Lap
-000025f0: 6c61 6365 2028 7363 6970 792c 206e 7362  lace (scipy, nsb
-00002600: 6174 776d 2922 290d 0a40 6a75 7079 7465  atwm)")..@jupyte
-00002610: 725f 6469 7370 6c61 7961 626c 655f 6f75  r_displayable_ou
-00002620: 7470 7574 286c 6962 7261 7279 5f6e 616d  tput(library_nam
-00002630: 653d 276e 7362 6174 776d 272c 2068 656c  e='nsbatwm', hel
-00002640: 705f 7572 6c3d 2768 7474 7073 3a2f 2f77  p_url='https://w
-00002650: 7777 2e6e 6170 6172 692d 6875 622e 6f72  ww.napari-hub.or
-00002660: 672f 706c 7567 696e 732f 6e61 7061 7269  g/plugins/napari
-00002670: 2d73 6567 6d65 6e74 2d62 6c6f 6273 2d61  -segment-blobs-a
-00002680: 6e64 2d74 6869 6e67 732d 7769 7468 2d6d  nd-things-with-m
-00002690: 656d 6272 616e 6573 2729 0d0a 4074 696d  embranes')..@tim
-000026a0: 655f 736c 6963 6572 0d0a 6465 6620 6761  e_slicer..def ga
-000026b0: 7573 7369 616e 5f6c 6170 6c61 6365 2869  ussian_laplace(i
-000026c0: 6d61 6765 3a22 6e61 7061 7269 2e74 7970  mage:"napari.typ
-000026d0: 6573 2e49 6d61 6765 4461 7461 222c 2073  es.ImageData", s
-000026e0: 6967 6d61 3a20 666c 6f61 7420 3d20 3229  igma: float = 2)
-000026f0: 2d3e 2022 6e61 7061 7269 2e74 7970 6573  -> "napari.types
-00002700: 2e49 6d61 6765 4461 7461 223a 0d0a 2020  .ImageData":..  
-00002710: 2020 2222 220d 0a20 2020 2041 7070 6c79    """..    Apply
-00002720: 204c 6170 6c61 6365 2066 696c 7465 7220   Laplace filter 
-00002730: 666f 7220 6564 6765 2064 6574 6563 7469  for edge detecti
-00002740: 6f6e 202f 2065 6467 6520 656e 6861 6e63  on / edge enhanc
-00002750: 656d 656e 7420 6166 7465 7220 6170 706c  ement after appl
-00002760: 7969 6e67 2061 2047 6175 7373 6961 6e2d  ying a Gaussian-
-00002770: 626c 7572 0d0a 0d0a 2020 2020 5061 7261  blur....    Para
-00002780: 6d65 7465 7273 0d0a 2020 2020 2d2d 2d2d  meters..    ----
-00002790: 2d2d 2d2d 2d2d 0d0a 2020 2020 696d 6167  ------..    imag
-000027a0: 653a 2061 7272 6179 2d6c 696b 650d 0a20  e: array-like.. 
-000027b0: 2020 2020 2020 2049 6d61 6765 2074 6f20         Image to 
-000027c0: 6465 7465 6374 2065 6467 6573 2069 6e0d  detect edges in.
-000027d0: 0a20 2020 2073 6967 6d61 3a20 666c 6f61  .    sigma: floa
-000027e0: 740d 0a20 2020 2020 2020 2054 6865 2066  t..        The f
-000027f0: 696c 7465 7220 7769 6c6c 2062 6520 6170  ilter will be ap
-00002800: 706c 6965 6420 7769 7468 2074 6869 7320  plied with this 
-00002810: 7370 6563 6966 6965 6420 4761 7573 7369  specified Gaussi
-00002820: 616e 2d62 6c75 7220 7369 676d 610d 0a0d  an-blur sigma...
-00002830: 0a20 2020 2052 6574 7572 6e73 0d0a 2020  .    Returns..  
-00002840: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2061    -------..    a
-00002850: 7272 6179 2d6c 696b 650d 0a0d 0a20 2020  rray-like....   
-00002860: 2053 6565 2061 6c73 6f0d 0a20 2020 202d   See also..    -
-00002870: 2d2d 2d2d 2d2d 2d0d 0a20 2020 202e 2e20  -------..    .. 
-00002880: 5b31 5d20 6874 7470 733a 2f2f 656e 2e77  [1] https://en.w
-00002890: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-000028a0: 692f 4c61 706c 6163 655f 6f70 6572 6174  i/Laplace_operat
-000028b0: 6f72 0d0a 2020 2020 2222 220d 0a20 2020  or..    """..   
-000028c0: 2072 6574 7572 6e20 7363 6970 792e 6e64   return scipy.nd
-000028d0: 696d 6167 652e 6761 7573 7369 616e 5f6c  image.gaussian_l
-000028e0: 6170 6c61 6365 2869 6d61 6765 2e61 7374  aplace(image.ast
-000028f0: 7970 6528 666c 6f61 7429 2c20 7369 676d  ype(float), sigm
-00002900: 6129 0d0a 0d0a 0d0a 4072 6567 6973 7465  a)......@registe
-00002910: 725f 6675 6e63 7469 6f6e 286d 656e 753d  r_function(menu=
-00002920: 2246 696c 7465 7269 6e67 202f 206e 6f69  "Filtering / noi
-00002930: 7365 2072 656d 6f76 616c 203e 204d 6564  se removal > Med
-00002940: 6961 6e20 2873 6369 7079 2c20 6e73 6261  ian (scipy, nsba
-00002950: 7477 6d29 2229 0d0a 406a 7570 7974 6572  twm)")..@jupyter
-00002960: 5f64 6973 706c 6179 6162 6c65 5f6f 7574  _displayable_out
-00002970: 7075 7428 6c69 6272 6172 795f 6e61 6d65  put(library_name
-00002980: 3d27 6e73 6261 7477 6d27 2c20 6865 6c70  ='nsbatwm', help
-00002990: 5f75 726c 3d27 6874 7470 733a 2f2f 7777  _url='https://ww
-000029a0: 772e 6e61 7061 7269 2d68 7562 2e6f 7267  w.napari-hub.org
-000029b0: 2f70 6c75 6769 6e73 2f6e 6170 6172 692d  /plugins/napari-
-000029c0: 7365 676d 656e 742d 626c 6f62 732d 616e  segment-blobs-an
-000029d0: 642d 7468 696e 6773 2d77 6974 682d 6d65  d-things-with-me
-000029e0: 6d62 7261 6e65 7327 290d 0a40 7469 6d65  mbranes')..@time
-000029f0: 5f73 6c69 6365 720d 0a64 6566 206d 6564  _slicer..def med
-00002a00: 6961 6e5f 6669 6c74 6572 2869 6d61 6765  ian_filter(image
-00002a10: 3a22 6e61 7061 7269 2e74 7970 6573 2e49  :"napari.types.I
-00002a20: 6d61 6765 4461 7461 222c 2072 6164 6975  mageData", radiu
-00002a30: 733a 2066 6c6f 6174 203d 2032 292d 3e20  s: float = 2)-> 
-00002a40: 226e 6170 6172 692e 7479 7065 732e 496d  "napari.types.Im
-00002a50: 6167 6544 6174 6122 3a0d 0a20 2020 2022  ageData":..    "
-00002a60: 2222 0d0a 2020 2020 5468 6520 6d65 6469  ""..    The medi
-00002a70: 616e 2d66 696c 7465 7220 616c 6c6f 7773  an-filter allows
-00002a80: 2072 656d 6f76 696e 6720 6e6f 6973 6520   removing noise 
-00002a90: 6672 6f6d 2069 6d61 6765 732e 2057 6869  from images. Whi
-00002aa0: 6c65 206c 6f63 616c 6c79 2061 7665 7261  le locally avera
-00002ab0: 6769 6e67 2069 6e74 656e 7369 7479 2c20  ging intensity, 
-00002ac0: 6974 0d0a 2020 2020 6973 2061 6e20 6564  it..    is an ed
-00002ad0: 6765 2d70 7265 7365 7276 696e 6720 6669  ge-preserving fi
-00002ae0: 6c74 6572 2e0d 0a0d 0a20 2020 2049 7420  lter.....    It 
-00002af0: 6973 2065 7175 616c 2074 6f20 6120 7065  is equal to a pe
-00002b00: 7263 656e 7469 6c65 2d66 696c 7465 7220  rcentile-filter 
-00002b10: 7769 7468 2070 6572 6365 6e74 696c 653d  with percentile=
-00002b20: 3d35 302e 0d0a 2020 2020 496e 2063 6173  =50...    In cas
-00002b30: 6520 6170 706c 7969 6e67 2074 6865 2066  e applying the f
-00002b40: 696c 7465 7220 7461 6b65 7320 746f 206d  ilter takes to m
-00002b50: 7563 6820 7469 6d65 2c20 636f 6e73 6964  uch time, consid
-00002b60: 6572 2075 7369 6e67 2061 2047 6175 7373  er using a Gauss
-00002b70: 6961 6e20 626c 7572 2069 6e73 7465 6164  ian blur instead
-00002b80: 2e0d 0a20 2020 2022 2222 0d0a 2020 2020  ...    """..    
-00002b90: 7265 7475 726e 2073 6369 7079 2e6e 6469  return scipy.ndi
-00002ba0: 6d61 6765 2e6d 6564 6961 6e5f 6669 6c74  mage.median_filt
-00002bb0: 6572 2869 6d61 6765 2e61 7374 7970 6528  er(image.astype(
-00002bc0: 666c 6f61 7429 2c20 7369 7a65 3d69 6e74  float), size=int
-00002bd0: 2872 6164 6975 7320 2a20 3220 2b20 3129  (radius * 2 + 1)
-00002be0: 290d 0a0d 0a0d 0a40 7265 6769 7374 6572  )......@register
-00002bf0: 5f66 756e 6374 696f 6e28 6d65 6e75 3d22  _function(menu="
-00002c00: 4669 6c74 6572 696e 6720 2f20 6e6f 6973  Filtering / nois
-00002c10: 6520 7265 6d6f 7661 6c20 3e20 5065 7263  e removal > Perc
-00002c20: 656e 7469 6c65 2028 7363 6970 792c 206e  entile (scipy, n
-00002c30: 7362 6174 776d 2922 290d 0a40 6a75 7079  sbatwm)")..@jupy
-00002c40: 7465 725f 6469 7370 6c61 7961 626c 655f  ter_displayable_
-00002c50: 6f75 7470 7574 286c 6962 7261 7279 5f6e  output(library_n
-00002c60: 616d 653d 276e 7362 6174 776d 272c 2068  ame='nsbatwm', h
-00002c70: 656c 705f 7572 6c3d 2768 7474 7073 3a2f  elp_url='https:/
-00002c80: 2f77 7777 2e6e 6170 6172 692d 6875 622e  /www.napari-hub.
-00002c90: 6f72 672f 706c 7567 696e 732f 6e61 7061  org/plugins/napa
-00002ca0: 7269 2d73 6567 6d65 6e74 2d62 6c6f 6273  ri-segment-blobs
-00002cb0: 2d61 6e64 2d74 6869 6e67 732d 7769 7468  -and-things-with
-00002cc0: 2d6d 656d 6272 616e 6573 2729 0d0a 4074  -membranes')..@t
-00002cd0: 696d 655f 736c 6963 6572 0d0a 6465 6620  ime_slicer..def 
-00002ce0: 7065 7263 656e 7469 6c65 5f66 696c 7465  percentile_filte
-00002cf0: 7228 696d 6167 653a 226e 6170 6172 692e  r(image:"napari.
-00002d00: 7479 7065 732e 496d 6167 6544 6174 6122  types.ImageData"
-00002d10: 2c20 7065 7263 656e 7469 6c65 203a 2066  , percentile : f
-00002d20: 6c6f 6174 203d 2035 302c 2072 6164 6975  loat = 50, radiu
-00002d30: 733a 2066 6c6f 6174 203d 2032 292d 3e20  s: float = 2)-> 
-00002d40: 226e 6170 6172 692e 7479 7065 732e 496d  "napari.types.Im
-00002d50: 6167 6544 6174 6122 3a0d 0a20 2020 2022  ageData":..    "
-00002d60: 2222 5468 6520 7065 7263 656e 7469 6c65  ""The percentile
-00002d70: 2066 696c 7465 7220 6973 2073 696d 696c   filter is simil
-00002d80: 6172 2074 6f20 7468 6520 6d65 6469 616e  ar to the median
-00002d90: 2d66 696c 7465 7220 6275 7420 6974 2061  -filter but it a
-00002da0: 6c6c 6f77 7320 7370 6563 6966 7969 6e67  llows specifying
-00002db0: 2074 6865 2070 6572 6365 6e74 696c 652e   the percentile.
-00002dc0: 0d0a 2020 2020 5468 6520 7065 7263 656e  ..    The percen
-00002dd0: 7469 6c65 2d66 696c 7465 7220 7769 7468  tile-filter with
-00002de0: 2070 6572 6365 6e74 696c 653d 3d35 3020   percentile==50 
-00002df0: 6973 2065 7175 616c 2074 6f20 7468 6520  is equal to the 
-00002e00: 6d65 6469 616e 2d66 696c 7465 722e 0d0a  median-filter...
-00002e10: 2020 2020 2222 220d 0a20 2020 2072 6574      """..    ret
-00002e20: 7572 6e20 7363 6970 792e 6e64 696d 6167  urn scipy.ndimag
-00002e30: 652e 7065 7263 656e 7469 6c65 5f66 696c  e.percentile_fil
-00002e40: 7465 7228 696d 6167 652e 6173 7479 7065  ter(image.astype
-00002e50: 2866 6c6f 6174 292c 2070 6572 6365 6e74  (float), percent
-00002e60: 696c 653d 7065 7263 656e 7469 6c65 2c20  ile=percentile, 
-00002e70: 7369 7a65 3d69 6e74 2872 6164 6975 7320  size=int(radius 
-00002e80: 2a20 3220 2b20 3129 290d 0a0d 0a0d 0a40  * 2 + 1))......@
-00002e90: 7265 6769 7374 6572 5f66 756e 6374 696f  register_functio
-00002ea0: 6e28 6d65 6e75 3d22 4669 6c74 6572 696e  n(menu="Filterin
-00002eb0: 6720 2f20 6261 636b 6772 6f75 6e64 2072  g / background r
-00002ec0: 656d 6f76 616c 203e 2057 6869 7465 2074  emoval > White t
-00002ed0: 6f70 2d68 6174 2028 7363 6970 792c 206e  op-hat (scipy, n
-00002ee0: 7362 6174 776d 2922 290d 0a40 6a75 7079  sbatwm)")..@jupy
-00002ef0: 7465 725f 6469 7370 6c61 7961 626c 655f  ter_displayable_
-00002f00: 6f75 7470 7574 286c 6962 7261 7279 5f6e  output(library_n
-00002f10: 616d 653d 276e 7362 6174 776d 272c 2068  ame='nsbatwm', h
-00002f20: 656c 705f 7572 6c3d 2768 7474 7073 3a2f  elp_url='https:/
-00002f30: 2f77 7777 2e6e 6170 6172 692d 6875 622e  /www.napari-hub.
-00002f40: 6f72 672f 706c 7567 696e 732f 6e61 7061  org/plugins/napa
-00002f50: 7269 2d73 6567 6d65 6e74 2d62 6c6f 6273  ri-segment-blobs
-00002f60: 2d61 6e64 2d74 6869 6e67 732d 7769 7468  -and-things-with
-00002f70: 2d6d 656d 6272 616e 6573 2729 0d0a 4074  -membranes')..@t
-00002f80: 696d 655f 736c 6963 6572 0d0a 6465 6620  ime_slicer..def 
-00002f90: 7768 6974 655f 746f 7068 6174 2869 6d61  white_tophat(ima
-00002fa0: 6765 3a22 6e61 7061 7269 2e74 7970 6573  ge:"napari.types
-00002fb0: 2e49 6d61 6765 4461 7461 222c 2072 6164  .ImageData", rad
-00002fc0: 6975 733a 2066 6c6f 6174 203d 2032 292d  ius: float = 2)-
-00002fd0: 3e20 226e 6170 6172 692e 7479 7065 732e  > "napari.types.
-00002fe0: 496d 6167 6544 6174 6122 3a0d 0a20 2020  ImageData":..   
-00002ff0: 2022 2222 0d0a 2020 2020 5468 6520 7768   """..    The wh
-00003000: 6974 6520 746f 702d 6861 7420 6669 6c74  ite top-hat filt
-00003010: 6572 2072 656d 6f76 6573 2062 7269 6768  er removes brigh
-00003020: 7420 7265 6769 6f6e 7320 6672 6f6d 2061  t regions from a
-00003030: 6e20 696d 6167 6520 7368 6f77 696e 6720  n image showing 
-00003040: 626c 6163 6b20 6973 6c61 6e64 732e 0d0a  black islands...
-00003050: 0d0a 2020 2020 496e 2074 6865 2063 6f6e  ..    In the con
-00003060: 7465 7874 206f 6620 666c 756f 7265 7363  text of fluoresc
-00003070: 656e 6365 206d 6963 726f 7363 6f70 792c  ence microscopy,
-00003080: 2069 7420 616c 6c6f 7773 2072 656d 6f76   it allows remov
-00003090: 696e 6720 696e 7465 6e73 6974 7920 7265  ing intensity re
-000030a0: 7375 6c74 696e 6720 6672 6f6d 206f 7574  sulting from out
-000030b0: 2d6f 662d 666f 6375 7320 6c69 6768 742e  -of-focus light.
-000030c0: 0d0a 2020 2020 2222 220d 0a20 2020 2072  ..    """..    r
-000030d0: 6574 7572 6e20 7363 6970 792e 6e64 696d  eturn scipy.ndim
-000030e0: 6167 652e 7768 6974 655f 746f 7068 6174  age.white_tophat
-000030f0: 2869 6d61 6765 2e61 7374 7970 6528 666c  (image.astype(fl
-00003100: 6f61 7429 2c20 7369 7a65 3d69 6e74 2872  oat), size=int(r
-00003110: 6164 6975 7320 2a20 3220 2b20 3129 290d  adius * 2 + 1)).
-00003120: 0a0d 0a0d 0a40 7265 6769 7374 6572 5f66  .....@register_f
-00003130: 756e 6374 696f 6e28 6d65 6e75 3d22 4669  unction(menu="Fi
-00003140: 6c74 6572 696e 6720 2f20 6261 636b 6772  ltering / backgr
-00003150: 6f75 6e64 2072 656d 6f76 616c 203e 2042  ound removal > B
-00003160: 6c61 636b 2074 6f70 2d68 6174 2028 7363  lack top-hat (sc
-00003170: 6970 792c 206e 7362 6174 776d 2922 290d  ipy, nsbatwm)").
-00003180: 0a40 6a75 7079 7465 725f 6469 7370 6c61  .@jupyter_displa
-00003190: 7961 626c 655f 6f75 7470 7574 286c 6962  yable_output(lib
-000031a0: 7261 7279 5f6e 616d 653d 276e 7362 6174  rary_name='nsbat
-000031b0: 776d 272c 2068 656c 705f 7572 6c3d 2768  wm', help_url='h
-000031c0: 7474 7073 3a2f 2f77 7777 2e6e 6170 6172  ttps://www.napar
-000031d0: 692d 6875 622e 6f72 672f 706c 7567 696e  i-hub.org/plugin
-000031e0: 732f 6e61 7061 7269 2d73 6567 6d65 6e74  s/napari-segment
-000031f0: 2d62 6c6f 6273 2d61 6e64 2d74 6869 6e67  -blobs-and-thing
-00003200: 732d 7769 7468 2d6d 656d 6272 616e 6573  s-with-membranes
-00003210: 2729 0d0a 4074 696d 655f 736c 6963 6572  ')..@time_slicer
-00003220: 0d0a 6465 6620 626c 6163 6b5f 746f 7068  ..def black_toph
-00003230: 6174 2869 6d61 6765 3a22 6e61 7061 7269  at(image:"napari
-00003240: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
-00003250: 222c 2072 6164 6975 733a 2066 6c6f 6174  ", radius: float
-00003260: 203d 2032 292d 3e20 226e 6170 6172 692e   = 2)-> "napari.
-00003270: 7479 7065 732e 496d 6167 6544 6174 6122  types.ImageData"
-00003280: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-00003290: 5468 6520 626c 6163 6b20 746f 702d 6861  The black top-ha
-000032a0: 7420 6669 6c74 6572 2072 656d 6f76 6573  t filter removes
-000032b0: 2062 7269 6768 7420 7265 6769 6f6e 7320   bright regions 
-000032c0: 6672 6f6d 2061 6e20 696d 6167 6520 7368  from an image sh
-000032d0: 6f77 696e 6720 626c 6163 6b20 6973 6c61  owing black isla
-000032e0: 6e64 732e 0d0a 2020 2020 2222 220d 0a20  nds...    """.. 
-000032f0: 2020 2072 6574 7572 6e20 7363 6970 792e     return scipy.
-00003300: 6e64 696d 6167 652e 626c 6163 6b5f 746f  ndimage.black_to
-00003310: 7068 6174 2869 6d61 6765 2e61 7374 7970  phat(image.astyp
-00003320: 6528 666c 6f61 7429 2c20 7369 7a65 3d69  e(float), size=i
-00003330: 6e74 2872 6164 6975 7320 2a20 3220 2b20  nt(radius * 2 + 
-00003340: 3129 290d 0a0d 0a0d 0a40 7265 6769 7374  1))......@regist
-00003350: 6572 5f66 756e 6374 696f 6e28 6d65 6e75  er_function(menu
-00003360: 3d22 4669 6c74 6572 696e 6720 2f20 6261  ="Filtering / ba
-00003370: 636b 6772 6f75 6e64 2072 656d 6f76 616c  ckground removal
-00003380: 203e 204d 696e 696d 756d 2028 7363 6970   > Minimum (scip
-00003390: 792c 206e 7362 6174 776d 2922 290d 0a40  y, nsbatwm)")..@
-000033a0: 6a75 7079 7465 725f 6469 7370 6c61 7961  jupyter_displaya
-000033b0: 626c 655f 6f75 7470 7574 286c 6962 7261  ble_output(libra
-000033c0: 7279 5f6e 616d 653d 276e 7362 6174 776d  ry_name='nsbatwm
-000033d0: 272c 2068 656c 705f 7572 6c3d 2768 7474  ', help_url='htt
-000033e0: 7073 3a2f 2f77 7777 2e6e 6170 6172 692d  ps://www.napari-
-000033f0: 6875 622e 6f72 672f 706c 7567 696e 732f  hub.org/plugins/
-00003400: 6e61 7061 7269 2d73 6567 6d65 6e74 2d62  napari-segment-b
-00003410: 6c6f 6273 2d61 6e64 2d74 6869 6e67 732d  lobs-and-things-
-00003420: 7769 7468 2d6d 656d 6272 616e 6573 2729  with-membranes')
-00003430: 0d0a 4074 696d 655f 736c 6963 6572 0d0a  ..@time_slicer..
-00003440: 6465 6620 6d69 6e69 6d75 6d5f 6669 6c74  def minimum_filt
-00003450: 6572 2869 6d61 6765 3a22 6e61 7061 7269  er(image:"napari
-00003460: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
-00003470: 222c 2072 6164 6975 733a 2066 6c6f 6174  ", radius: float
-00003480: 203d 2032 292d 3e20 226e 6170 6172 692e   = 2)-> "napari.
-00003490: 7479 7065 732e 496d 6167 6544 6174 6122  types.ImageData"
-000034a0: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-000034b0: 4c6f 6361 6c20 6d69 6e69 6d75 6d20 6669  Local minimum fi
-000034c0: 6c74 6572 0d0a 0d0a 2020 2020 4361 6e20  lter....    Can 
-000034d0: 6265 2075 7365 6420 666f 7220 6e6f 6973  be used for nois
-000034e0: 6520 616e 6420 6261 636b 6772 6f75 6e64  e and background
-000034f0: 2072 656d 6f76 616c 2e0d 0a20 2020 2022   removal...    "
-00003500: 2222 0d0a 2020 2020 7265 7475 726e 2073  ""..    return s
-00003510: 6369 7079 2e6e 6469 6d61 6765 2e6d 696e  cipy.ndimage.min
-00003520: 696d 756d 5f66 696c 7465 7228 696d 6167  imum_filter(imag
-00003530: 652e 6173 7479 7065 2866 6c6f 6174 292c  e.astype(float),
-00003540: 2073 697a 653d 7261 6469 7573 202a 2032   size=radius * 2
-00003550: 202b 2031 290d 0a0d 0a0d 0a40 7265 6769   + 1)......@regi
-00003560: 7374 6572 5f66 756e 6374 696f 6e28 6d65  ster_function(me
-00003570: 6e75 3d22 4669 6c74 6572 696e 6720 2f20  nu="Filtering / 
-00003580: 6261 636b 6772 6f75 6e64 2072 656d 6f76  background remov
-00003590: 616c 203e 204d 6178 696d 756d 2028 7363  al > Maximum (sc
-000035a0: 6970 792c 206e 7362 6174 776d 2922 290d  ipy, nsbatwm)").
-000035b0: 0a40 6a75 7079 7465 725f 6469 7370 6c61  .@jupyter_displa
-000035c0: 7961 626c 655f 6f75 7470 7574 286c 6962  yable_output(lib
-000035d0: 7261 7279 5f6e 616d 653d 276e 7362 6174  rary_name='nsbat
-000035e0: 776d 272c 2068 656c 705f 7572 6c3d 2768  wm', help_url='h
-000035f0: 7474 7073 3a2f 2f77 7777 2e6e 6170 6172  ttps://www.napar
-00003600: 692d 6875 622e 6f72 672f 706c 7567 696e  i-hub.org/plugin
-00003610: 732f 6e61 7061 7269 2d73 6567 6d65 6e74  s/napari-segment
-00003620: 2d62 6c6f 6273 2d61 6e64 2d74 6869 6e67  -blobs-and-thing
-00003630: 732d 7769 7468 2d6d 656d 6272 616e 6573  s-with-membranes
-00003640: 2729 0d0a 4074 696d 655f 736c 6963 6572  ')..@time_slicer
-00003650: 0d0a 6465 6620 6d61 7869 6d75 6d5f 6669  ..def maximum_fi
-00003660: 6c74 6572 2869 6d61 6765 3a22 6e61 7061  lter(image:"napa
-00003670: 7269 2e74 7970 6573 2e49 6d61 6765 4461  ri.types.ImageDa
-00003680: 7461 222c 2072 6164 6975 733a 2066 6c6f  ta", radius: flo
-00003690: 6174 203d 2032 292d 3e20 226e 6170 6172  at = 2)-> "napar
-000036a0: 692e 7479 7065 732e 496d 6167 6544 6174  i.types.ImageDat
-000036b0: 6122 3a0d 0a20 2020 2022 2222 0d0a 2020  a":..    """..  
-000036c0: 2020 4c6f 6361 6c20 6d61 7869 6d75 6d20    Local maximum 
-000036d0: 6669 6c74 6572 0d0a 0d0a 2020 2020 496e  filter....    In
-000036e0: 2074 6865 2063 6f6e 7465 7874 206f 6620   the context of 
-000036f0: 6365 6c6c 2073 6567 6d65 6e74 6174 696f  cell segmentatio
-00003700: 6e20 6974 2063 616e 2062 6520 7573 6564  n it can be used
-00003710: 2074 6f20 6d61 6b65 206d 656d 6272 616e   to make membran
-00003720: 6573 2077 6964 6572 0d0a 2020 2020 616e  es wider..    an
-00003730: 6420 636c 6f73 6520 736d 616c 6c20 6761  d close small ga
-00003740: 7073 206f 6620 696e 7375 6666 6963 6965  ps of insufficie
-00003750: 6e74 2073 7461 696e 696e 672e 0d0a 2020  nt staining...  
-00003760: 2020 2222 220d 0a20 2020 2072 6574 7572    """..    retur
-00003770: 6e20 7363 6970 792e 6e64 696d 6167 652e  n scipy.ndimage.
-00003780: 6d61 7869 6d75 6d5f 6669 6c74 6572 2869  maximum_filter(i
-00003790: 6d61 6765 2e61 7374 7970 6528 666c 6f61  mage.astype(floa
-000037a0: 7429 2c20 7369 7a65 3d72 6164 6975 7320  t), size=radius 
-000037b0: 2a20 3220 2b20 3129 0d0a 0d0a 0d0a 4072  * 2 + 1)......@r
-000037c0: 6567 6973 7465 725f 6675 6e63 7469 6f6e  egister_function
-000037d0: 286d 656e 753d 2246 696c 7465 7269 6e67  (menu="Filtering
-000037e0: 202f 2065 6467 6520 656e 6861 6e63 656d   / edge enhancem
-000037f0: 656e 7420 3e20 4d6f 7270 686f 6c6f 6769  ent > Morphologi
-00003800: 6361 6c20 4772 6164 6965 6e74 2028 7363  cal Gradient (sc
-00003810: 6970 792c 206e 7362 6174 776d 2922 290d  ipy, nsbatwm)").
-00003820: 0a40 6a75 7079 7465 725f 6469 7370 6c61  .@jupyter_displa
-00003830: 7961 626c 655f 6f75 7470 7574 286c 6962  yable_output(lib
-00003840: 7261 7279 5f6e 616d 653d 276e 7362 6174  rary_name='nsbat
-00003850: 776d 272c 2068 656c 705f 7572 6c3d 2768  wm', help_url='h
-00003860: 7474 7073 3a2f 2f77 7777 2e6e 6170 6172  ttps://www.napar
-00003870: 692d 6875 622e 6f72 672f 706c 7567 696e  i-hub.org/plugin
-00003880: 732f 6e61 7061 7269 2d73 6567 6d65 6e74  s/napari-segment
-00003890: 2d62 6c6f 6273 2d61 6e64 2d74 6869 6e67  -blobs-and-thing
-000038a0: 732d 7769 7468 2d6d 656d 6272 616e 6573  s-with-membranes
-000038b0: 2729 0d0a 4074 696d 655f 736c 6963 6572  ')..@time_slicer
-000038c0: 0d0a 6465 6620 6d6f 7270 686f 6c6f 6769  ..def morphologi
-000038d0: 6361 6c5f 6772 6164 6965 6e74 2869 6d61  cal_gradient(ima
-000038e0: 6765 3a22 6e61 7061 7269 2e74 7970 6573  ge:"napari.types
-000038f0: 2e49 6d61 6765 4461 7461 222c 2072 6164  .ImageData", rad
-00003900: 6975 733a 2066 6c6f 6174 203d 2032 292d  ius: float = 2)-
-00003910: 3e20 226e 6170 6172 692e 7479 7065 732e  > "napari.types.
-00003920: 496d 6167 6544 6174 6122 3a0d 0a20 2020  ImageData":..   
-00003930: 2022 2222 0d0a 2020 2020 4170 706c 7920   """..    Apply 
-00003940: 6772 6164 6965 6e74 2066 696c 7465 7220  gradient filter 
-00003950: 2873 696d 696c 6172 2074 6f20 7468 6520  (similar to the 
-00003960: 536f 6265 6c20 6f70 6572 6174 6f72 2920  Sobel operator) 
-00003970: 666f 7220 6564 6765 2064 6574 6563 7469  for edge detecti
-00003980: 6f6e 202f 2065 6467 6520 656e 6861 6e63  on / edge enhanc
-00003990: 656d 656e 742e 0d0a 2020 2020 5468 6973  ement...    This
-000039a0: 2069 7320 7369 6d69 6c61 7220 746f 2061   is similar to a
-000039b0: 7070 6c79 696e 6720 6120 4761 7573 7369  pplying a Gaussi
-000039c0: 616e 2d62 6c75 7220 746f 2061 6e20 696d  an-blur to an im
-000039d0: 6167 6520 616e 6420 6166 7465 7277 6172  age and afterwar
-000039e0: 6473 2074 6865 2067 7261 6469 656e 7420  ds the gradient 
-000039f0: 6f70 6572 6174 6f72 0d0a 0d0a 2020 2020  operator....    
-00003a00: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-00003a10: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
-00003a20: 696d 6167 653a 2061 7272 6179 2d6c 696b  image: array-lik
-00003a30: 650d 0a20 2020 2020 2020 2049 6d61 6765  e..        Image
-00003a40: 2074 6f20 6465 7465 6374 2065 6467 6573   to detect edges
-00003a50: 2069 6e0d 0a20 2020 2072 6164 6975 733a   in..    radius:
-00003a60: 2066 6c6f 6174 0d0a 2020 2020 2020 2020   float..        
-00003a70: 5468 6520 6669 6c74 6572 2077 696c 6c20  The filter will 
-00003a80: 6265 2061 7070 6c69 6564 2077 6974 6820  be applied with 
-00003a90: 6120 6b65 726e 656c 2073 697a 6520 6f66  a kernel size of
-00003aa0: 2028 7261 6469 7573 202a 2032 202b 2031   (radius * 2 + 1
-00003ab0: 290d 0a0d 0a20 2020 2052 6574 7572 6e73  )....    Returns
-00003ac0: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20  ..    -------.. 
-00003ad0: 2020 2061 7272 6179 2d6c 696b 650d 0a0d     array-like...
-00003ae0: 0a20 2020 2053 6565 2061 6c73 6f0d 0a20  .    See also.. 
-00003af0: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
-00003b00: 202e 2e20 5b31 5d20 6874 7470 733a 2f2f   .. [1] https://
-00003b10: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
-00003b20: 2f77 696b 692f 4d6f 7270 686f 6c6f 6769  /wiki/Morphologi
-00003b30: 6361 6c5f 6772 6164 6965 6e74 0d0a 2020  cal_gradient..  
-00003b40: 2020 2222 220d 0a20 2020 2072 6574 7572    """..    retur
-00003b50: 6e20 7363 6970 792e 6e64 696d 6167 652e  n scipy.ndimage.
-00003b60: 6d6f 7270 686f 6c6f 6769 6361 6c5f 6772  morphological_gr
-00003b70: 6164 6965 6e74 2869 6d61 6765 2e61 7374  adient(image.ast
-00003b80: 7970 6528 666c 6f61 7429 2c20 7369 7a65  ype(float), size
-00003b90: 3d69 6e74 2872 6164 6975 7320 2a20 3220  =int(radius * 2 
-00003ba0: 2b20 3129 290d 0a0d 0a0d 0a40 7265 6769  + 1))......@regi
-00003bb0: 7374 6572 5f66 756e 6374 696f 6e28 6d65  ster_function(me
-00003bc0: 6e75 3d22 4669 6c74 6572 696e 6720 2f20  nu="Filtering / 
-00003bd0: 6261 636b 6772 6f75 6e64 2072 656d 6f76  background remov
-00003be0: 616c 203e 2052 6f6c 6c69 6e67 2062 616c  al > Rolling bal
-00003bf0: 6c20 2873 6369 6b69 742d 696d 6167 652c  l (scikit-image,
-00003c00: 206e 7362 6174 776d 2922 290d 0a40 6a75   nsbatwm)")..@ju
-00003c10: 7079 7465 725f 6469 7370 6c61 7961 626c  pyter_displayabl
-00003c20: 655f 6f75 7470 7574 286c 6962 7261 7279  e_output(library
-00003c30: 5f6e 616d 653d 276e 7362 6174 776d 272c  _name='nsbatwm',
-00003c40: 2068 656c 705f 7572 6c3d 2768 7474 7073   help_url='https
-00003c50: 3a2f 2f77 7777 2e6e 6170 6172 692d 6875  ://www.napari-hu
-00003c60: 622e 6f72 672f 706c 7567 696e 732f 6e61  b.org/plugins/na
-00003c70: 7061 7269 2d73 6567 6d65 6e74 2d62 6c6f  pari-segment-blo
-00003c80: 6273 2d61 6e64 2d74 6869 6e67 732d 7769  bs-and-things-wi
-00003c90: 7468 2d6d 656d 6272 616e 6573 2729 0d0a  th-membranes')..
-00003ca0: 4074 696d 655f 736c 6963 6572 0d0a 6465  @time_slicer..de
-00003cb0: 6620 7375 6274 7261 6374 5f62 6163 6b67  f subtract_backg
-00003cc0: 726f 756e 6428 696d 6167 653a 226e 6170  round(image:"nap
-00003cd0: 6172 692e 7479 7065 732e 496d 6167 6544  ari.types.ImageD
-00003ce0: 6174 6122 2c20 726f 6c6c 696e 675f 6261  ata", rolling_ba
-00003cf0: 6c6c 5f72 6164 6975 733a 2066 6c6f 6174  ll_radius: float
-00003d00: 203d 2035 2920 2d3e 2022 6e61 7061 7269   = 5) -> "napari
-00003d10: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
-00003d20: 223a 0d0a 2020 2020 2222 220d 0a20 2020  ":..    """..   
-00003d30: 2053 7562 7472 6163 7420 6261 636b 6772   Subtract backgr
-00003d40: 6f75 6e64 2069 6e20 616e 2069 6d61 6765  ound in an image
-00003d50: 2075 7369 6e67 2074 6865 2072 6f6c 6c69   using the rolli
-00003d60: 6e67 2d62 616c 6c20 616c 676f 7269 7468  ng-ball algorith
-00003d70: 6d2e 0d0a 0d0a 2020 2020 5365 6520 616c  m.....    See al
-00003d80: 736f 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d  so..    --------
-00003d90: 0d0a 2020 2020 2e2e 5b30 5d20 6874 7470  ..    ..[0] http
-00003da0: 733a 2f2f 7363 696b 6974 2d69 6d61 6765  s://scikit-image
-00003db0: 2e6f 7267 2f64 6f63 732f 7374 6162 6c65  .org/docs/stable
-00003dc0: 2f61 7574 6f5f 6578 616d 706c 6573 2f73  /auto_examples/s
-00003dd0: 6567 6d65 6e74 6174 696f 6e2f 706c 6f74  egmentation/plot
-00003de0: 5f72 6f6c 6c69 6e67 5f62 616c 6c2e 6874  _rolling_ball.ht
-00003df0: 6d6c 0d0a 2020 2020 2222 220d 0a20 2020  ml..    """..   
-00003e00: 2062 6163 6b67 726f 756e 6420 3d20 726f   background = ro
-00003e10: 6c6c 696e 675f 6261 6c6c 2869 6d61 6765  lling_ball(image
-00003e20: 2c20 7261 6469 7573 203d 2072 6f6c 6c69  , radius = rolli
-00003e30: 6e67 5f62 616c 6c5f 7261 6469 7573 290d  ng_ball_radius).
-00003e40: 0a20 2020 2072 6574 7572 6e20 696d 6167  .    return imag
-00003e50: 6520 2d20 6261 636b 6772 6f75 6e64 0d0a  e - background..
-00003e60: 0d0a 0d0a 4072 6567 6973 7465 725f 6675  ....@register_fu
-00003e70: 6e63 7469 6f6e 286d 656e 753d 2253 6567  nction(menu="Seg
-00003e80: 6d65 6e74 6174 696f 6e20 706f 7374 2d70  mentation post-p
-00003e90: 726f 6365 7373 696e 6720 3e20 496e 7665  rocessing > Inve
-00003ea0: 7274 2062 696e 6172 7920 696d 6167 6520  rt binary image 
-00003eb0: 286e 7362 6174 776d 2922 290d 0a40 6a75  (nsbatwm)")..@ju
-00003ec0: 7079 7465 725f 6469 7370 6c61 7961 626c  pyter_displayabl
-00003ed0: 655f 6f75 7470 7574 286c 6962 7261 7279  e_output(library
-00003ee0: 5f6e 616d 653d 276e 7362 6174 776d 272c  _name='nsbatwm',
-00003ef0: 2068 656c 705f 7572 6c3d 2768 7474 7073   help_url='https
-00003f00: 3a2f 2f77 7777 2e6e 6170 6172 692d 6875  ://www.napari-hu
-00003f10: 622e 6f72 672f 706c 7567 696e 732f 6e61  b.org/plugins/na
-00003f20: 7061 7269 2d73 6567 6d65 6e74 2d62 6c6f  pari-segment-blo
-00003f30: 6273 2d61 6e64 2d74 6869 6e67 732d 7769  bs-and-things-wi
-00003f40: 7468 2d6d 656d 6272 616e 6573 2729 0d0a  th-membranes')..
-00003f50: 4074 696d 655f 736c 6963 6572 0d0a 6465  @time_slicer..de
-00003f60: 6620 6269 6e61 7279 5f69 6e76 6572 7428  f binary_invert(
-00003f70: 6269 6e61 7279 5f69 6d61 6765 3a22 6e61  binary_image:"na
-00003f80: 7061 7269 2e74 7970 6573 2e4c 6162 656c  pari.types.Label
-00003f90: 7344 6174 6122 2920 2d3e 2022 6e61 7061  sData") -> "napa
-00003fa0: 7269 2e74 7970 6573 2e4c 6162 656c 7344  ri.types.LabelsD
-00003fb0: 6174 6122 3a0d 0a20 2020 2022 2222 0d0a  ata":..    """..
-00003fc0: 2020 2020 496e 7665 7274 7320 6120 6269      Inverts a bi
-00003fd0: 6e61 7279 2069 6d61 6765 2e0d 0a20 2020  nary image...   
-00003fe0: 2022 2222 0d0a 2020 2020 7265 7475 726e   """..    return
-00003ff0: 2028 6e70 2e61 7361 7272 6179 2862 696e   (np.asarray(bin
-00004000: 6172 795f 696d 6167 6529 203d 3d20 3029  ary_image) == 0)
-00004010: 202a 2031 0d0a 0d0a 0d0a 4072 6567 6973   * 1......@regis
-00004020: 7465 725f 6675 6e63 7469 6f6e 286d 656e  ter_function(men
-00004030: 753d 2253 6567 6d65 6e74 6174 696f 6e20  u="Segmentation 
-00004040: 2f20 6c61 6265 6c69 6e67 203e 2043 6f6e  / labeling > Con
-00004050: 6e65 6374 6564 2063 6f6d 706f 6e65 6e74  nected component
-00004060: 206c 6162 656c 696e 6720 2873 6369 6b69   labeling (sciki
-00004070: 742d 696d 6167 652c 206e 7362 6174 776d  t-image, nsbatwm
-00004080: 2922 290d 0a40 6a75 7079 7465 725f 6469  )")..@jupyter_di
-00004090: 7370 6c61 7961 626c 655f 6f75 7470 7574  splayable_output
-000040a0: 286c 6962 7261 7279 5f6e 616d 653d 276e  (library_name='n
-000040b0: 7362 6174 776d 272c 2068 656c 705f 7572  sbatwm', help_ur
-000040c0: 6c3d 2768 7474 7073 3a2f 2f77 7777 2e6e  l='https://www.n
-000040d0: 6170 6172 692d 6875 622e 6f72 672f 706c  apari-hub.org/pl
-000040e0: 7567 696e 732f 6e61 7061 7269 2d73 6567  ugins/napari-seg
-000040f0: 6d65 6e74 2d62 6c6f 6273 2d61 6e64 2d74  ment-blobs-and-t
-00004100: 6869 6e67 732d 7769 7468 2d6d 656d 6272  hings-with-membr
-00004110: 616e 6573 2729 0d0a 4074 696d 655f 736c  anes')..@time_sl
-00004120: 6963 6572 0d0a 6465 6620 636f 6e6e 6563  icer..def connec
-00004130: 7465 645f 636f 6d70 6f6e 656e 745f 6c61  ted_component_la
-00004140: 6265 6c69 6e67 2862 696e 6172 795f 696d  beling(binary_im
-00004150: 6167 653a 2022 6e61 7061 7269 2e74 7970  age: "napari.typ
-00004160: 6573 2e4c 6162 656c 7344 6174 6122 2c20  es.LabelsData", 
-00004170: 6578 636c 7564 655f 6f6e 5f65 6467 6573  exclude_on_edges
-00004180: 3a20 626f 6f6c 203d 2046 616c 7365 2920  : bool = False) 
-00004190: 2d3e 2022 6e61 7061 7269 2e74 7970 6573  -> "napari.types
-000041a0: 2e4c 6162 656c 7344 6174 6122 3a0d 0a20  .LabelsData":.. 
-000041b0: 2020 2022 2222 0d0a 2020 2020 5461 6b65     """..    Take
-000041c0: 7320 6120 6269 6e61 7279 2069 6d61 6765  s a binary image
-000041d0: 2061 6e64 2070 726f 6475 6365 7320 6120   and produces a 
-000041e0: 6c61 6265 6c20 696d 6167 6520 7769 7468  label image with
-000041f0: 2061 6c6c 2073 6570 6172 6174 6564 206f   all separated o
-00004200: 626a 6563 7473 206c 6162 656c 6564 2077  bjects labeled w
-00004210: 6974 680d 0a20 2020 2064 6966 6665 7265  ith..    differe
-00004220: 6e74 2069 6e74 6567 6572 206e 756d 6265  nt integer numbe
-00004230: 7273 2e0d 0a0d 0a20 2020 2050 6172 616d  rs.....    Param
-00004240: 6574 6572 730d 0a20 2020 202d 2d2d 2d2d  eters..    -----
-00004250: 2d2d 2d2d 2d0d 0a20 2020 2065 7863 6c75  -----..    exclu
-00004260: 6465 5f6f 6e5f 6564 6765 7320 3a20 626f  de_on_edges : bo
-00004270: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 2020  ol, optional..  
-00004280: 2020 2020 2020 5768 6574 6865 7220 6f72        Whether or
-00004290: 206e 6f74 2074 6f20 636c 6561 7220 6f62   not to clear ob
-000042a0: 6a65 6374 7320 636f 6e6e 6563 7465 6420  jects connected 
-000042b0: 746f 2074 6865 206c 6162 656c 2069 6d61  to the label ima
-000042c0: 6765 2062 6f72 6465 722f 706c 616e 6573  ge border/planes
-000042d0: 2028 6569 7468 6572 2078 792c 2078 7a20   (either xy, xz 
-000042e0: 6f72 2079 7a29 2e0d 0a20 2020 2022 2222  or yz)...    """
-000042f0: 0d0a 2020 2020 6966 2065 7863 6c75 6465  ..    if exclude
-00004300: 5f6f 6e5f 6564 6765 733a 0d0a 2020 2020  _on_edges:..    
-00004310: 2020 2020 2320 7072 6f63 6573 7369 6e67      # processing
-00004320: 2074 6865 2069 6d61 6765 2c20 7768 6963   the image, whic
-00004330: 6820 6973 206e 6f74 2061 2074 696d 656c  h is not a timel
-00004340: 6170 7365 0d0a 2020 2020 2020 2020 7265  apse..        re
-00004350: 7475 726e 2072 656d 6f76 655f 6c61 6265  turn remove_labe
-00004360: 6c73 5f6f 6e5f 6564 6765 7328 6c61 6265  ls_on_edges(labe
-00004370: 6c28 6e70 2e61 7361 7272 6179 2862 696e  l(np.asarray(bin
-00004380: 6172 795f 696d 6167 6529 2929 0d0a 0d0a  ary_image)))....
-00004390: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000043a0: 2020 2072 6574 7572 6e20 6c61 6265 6c28     return label(
-000043b0: 6e70 2e61 7361 7272 6179 2862 696e 6172  np.asarray(binar
-000043c0: 795f 696d 6167 6529 290d 0a0d 0a0d 0a40  y_image))......@
-000043d0: 7265 6769 7374 6572 5f66 756e 6374 696f  register_functio
-000043e0: 6e28 6d65 6e75 3d22 5365 676d 656e 7461  n(menu="Segmenta
-000043f0: 7469 6f6e 2070 6f73 742d 7072 6f63 6573  tion post-proces
-00004400: 7369 6e67 203e 2052 656d 6f76 6520 6c61  sing > Remove la
-00004410: 6265 6c65 6420 6f62 6a65 6374 7320 6174  beled objects at
-00004420: 2074 6865 2069 6d61 6765 2062 6f72 6465   the image borde
-00004430: 7220 2873 6369 6b69 742d 696d 6167 652c  r (scikit-image,
-00004440: 206e 7362 6174 776d 2922 290d 0a40 6a75   nsbatwm)")..@ju
-00004450: 7079 7465 725f 6469 7370 6c61 7961 626c  pyter_displayabl
-00004460: 655f 6f75 7470 7574 286c 6962 7261 7279  e_output(library
-00004470: 5f6e 616d 653d 276e 7362 6174 776d 272c  _name='nsbatwm',
-00004480: 2068 656c 705f 7572 6c3d 2768 7474 7073   help_url='https
-00004490: 3a2f 2f77 7777 2e6e 6170 6172 692d 6875  ://www.napari-hu
-000044a0: 622e 6f72 672f 706c 7567 696e 732f 6e61  b.org/plugins/na
-000044b0: 7061 7269 2d73 6567 6d65 6e74 2d62 6c6f  pari-segment-blo
-000044c0: 6273 2d61 6e64 2d74 6869 6e67 732d 7769  bs-and-things-wi
-000044d0: 7468 2d6d 656d 6272 616e 6573 2729 0d0a  th-membranes')..
-000044e0: 4074 696d 655f 736c 6963 6572 0d0a 6465  @time_slicer..de
-000044f0: 6620 7265 6d6f 7665 5f6c 6162 656c 735f  f remove_labels_
-00004500: 6f6e 5f65 6467 6573 286c 6162 656c 5f69  on_edges(label_i
-00004510: 6d61 6765 3a20 226e 6170 6172 692e 7479  mage: "napari.ty
-00004520: 7065 732e 4c61 6265 6c73 4461 7461 2229  pes.LabelsData")
-00004530: 202d 3e20 226e 6170 6172 692e 7479 7065   -> "napari.type
-00004540: 732e 4c61 6265 6c73 4461 7461 223a 0d0a  s.LabelsData":..
-00004550: 2020 2020 2222 220d 0a20 2020 2054 616b      """..    Tak
-00004560: 6573 2061 206c 6162 656c 2069 6d61 6765  es a label image
-00004570: 2061 6e64 2072 656d 6f76 6573 206f 626a   and removes obj
-00004580: 6563 7473 2074 6861 7420 746f 7563 6820  ects that touch 
-00004590: 7468 6520 696d 6167 6520 626f 7264 6572  the image border
-000045a0: 2e0d 0a20 2020 2054 6865 2072 656d 6169  ...    The remai
-000045b0: 6e69 6e67 206c 6162 656c 7320 6172 6520  ning labels are 
-000045c0: 7265 6c61 6265 6c65 6420 7365 7175 656e  relabeled sequen
-000045d0: 7469 616c 6c79 2e0d 0a0d 0a20 2020 2053  tially.....    S
-000045e0: 6565 2061 6c73 6f0d 0a20 2020 202d 2d2d  ee also..    ---
-000045f0: 2d2d 2d2d 2d0d 0a20 2020 202e 2e5b 305d  -----..    ..[0]
-00004600: 2068 7474 7073 3a2f 2f73 6369 6b69 742d   https://scikit-
-00004610: 696d 6167 652e 6f72 672f 646f 6373 2f73  image.org/docs/s
-00004620: 7461 626c 652f 6170 692f 736b 696d 6167  table/api/skimag
-00004630: 652e 7365 676d 656e 7461 7469 6f6e 2e68  e.segmentation.h
-00004640: 746d 6c23 736b 696d 6167 652e 7365 676d  tml#skimage.segm
-00004650: 656e 7461 7469 6f6e 2e63 6c65 6172 5f62  entation.clear_b
-00004660: 6f72 6465 720d 0a20 2020 2022 2222 0d0a  order..    """..
-00004670: 0d0a 2020 2020 7265 7375 6c74 203d 2063  ..    result = c
-00004680: 6c65 6172 5f62 6f72 6465 7228 6e70 2e61  lear_border(np.a
-00004690: 7361 7272 6179 286c 6162 656c 5f69 6d61  sarray(label_ima
-000046a0: 6765 2929 0d0a 2020 2020 7265 6c61 6265  ge))..    relabe
-000046b0: 6c65 645f 7265 7375 6c74 2c20 5f2c 205f  led_result, _, _
-000046c0: 203d 2072 656c 6162 656c 5f73 6571 7565   = relabel_seque
-000046d0: 6e74 6961 6c28 7265 7375 6c74 290d 0a20  ntial(result).. 
-000046e0: 2020 2072 6574 7572 6e20 7265 6c61 6265     return relabe
-000046f0: 6c65 645f 7265 7375 6c74 0d0a 0d0a 0d0a  led_result......
-00004700: 4072 6567 6973 7465 725f 6675 6e63 7469  @register_functi
-00004710: 6f6e 286d 656e 753d 2253 6567 6d65 6e74  on(menu="Segment
-00004720: 6174 696f 6e20 706f 7374 2d70 726f 6365  ation post-proce
-00004730: 7373 696e 6720 3e20 4578 7061 6e64 206c  ssing > Expand l
-00004740: 6162 656c 7320 2873 6369 6b69 742d 696d  abels (scikit-im
-00004750: 6167 652c 206e 7362 6174 776d 2922 290d  age, nsbatwm)").
-00004760: 0a40 6a75 7079 7465 725f 6469 7370 6c61  .@jupyter_displa
-00004770: 7961 626c 655f 6f75 7470 7574 286c 6962  yable_output(lib
-00004780: 7261 7279 5f6e 616d 653d 276e 7362 6174  rary_name='nsbat
-00004790: 776d 272c 2068 656c 705f 7572 6c3d 2768  wm', help_url='h
-000047a0: 7474 7073 3a2f 2f77 7777 2e6e 6170 6172  ttps://www.napar
-000047b0: 692d 6875 622e 6f72 672f 706c 7567 696e  i-hub.org/plugin
-000047c0: 732f 6e61 7061 7269 2d73 6567 6d65 6e74  s/napari-segment
-000047d0: 2d62 6c6f 6273 2d61 6e64 2d74 6869 6e67  -blobs-and-thing
-000047e0: 732d 7769 7468 2d6d 656d 6272 616e 6573  s-with-membranes
-000047f0: 2729 0d0a 4074 696d 655f 736c 6963 6572  ')..@time_slicer
-00004800: 0d0a 6465 6620 6578 7061 6e64 5f6c 6162  ..def expand_lab
-00004810: 656c 7328 6c61 6265 6c5f 696d 6167 653a  els(label_image:
-00004820: 2022 6e61 7061 7269 2e74 7970 6573 2e4c   "napari.types.L
-00004830: 6162 656c 7344 6174 6122 2c20 6469 7374  abelsData", dist
-00004840: 616e 6365 3a20 666c 6f61 7420 3d20 3129  ance: float = 1)
-00004850: 202d 3e20 226e 6170 6172 692e 7479 7065   -> "napari.type
-00004860: 732e 4c61 6265 6c73 4461 7461 223a 0d0a  s.LabelsData":..
-00004870: 2020 2020 2222 220d 0a20 2020 2054 616b      """..    Tak
-00004880: 6573 2061 206c 6162 656c 2069 6d61 6765  es a label image
-00004890: 2061 6e64 206d 616b 6573 206c 6162 656c   and makes label
-000048a0: 7320 6c61 7267 6572 2075 7020 746f 2061  s larger up to a
-000048b0: 2067 6976 656e 2072 6164 6975 7320 2864   given radius (d
-000048c0: 6973 7461 6e63 6529 2e0d 0a20 2020 204c  istance)...    L
-000048d0: 6162 656c 7320 7769 6c6c 206e 6f74 206f  abels will not o
-000048e0: 7665 7277 7269 7465 2065 6163 6820 6f74  verwrite each ot
-000048f0: 6865 7220 7768 696c 6520 6578 7061 6e64  her while expand
-00004900: 696e 672e 2054 6869 7320 6f70 6572 6174  ing. This operat
-00004910: 696f 6e20 6973 2061 6c73 6f20 6b6e 6f77  ion is also know
-00004920: 6e20 6173 206c 6162 656c 2064 696c 6174  n as label dilat
-00004930: 696f 6e2e 0d0a 0d0a 2020 2020 5365 6520  ion.....    See 
-00004940: 616c 736f 0d0a 2020 2020 2d2d 2d2d 2d2d  also..    ------
-00004950: 2d2d 0d0a 2020 2020 2e2e 5b30 5d20 6874  --..    ..[0] ht
-00004960: 7470 733a 2f2f 7363 696b 6974 2d69 6d61  tps://scikit-ima
-00004970: 6765 2e6f 7267 2f64 6f63 732f 7374 6162  ge.org/docs/stab
-00004980: 6c65 2f61 7069 2f73 6b69 6d61 6765 2e73  le/api/skimage.s
-00004990: 6567 6d65 6e74 6174 696f 6e2e 6874 6d6c  egmentation.html
-000049a0: 2373 6b69 6d61 6765 2e73 6567 6d65 6e74  #skimage.segment
-000049b0: 6174 696f 6e2e 6578 7061 6e64 5f6c 6162  ation.expand_lab
-000049c0: 656c 730d 0a20 2020 2022 2222 0d0a 0d0a  els..    """....
-000049d0: 2020 2020 7265 7475 726e 2073 6b5f 6578      return sk_ex
-000049e0: 7061 6e64 5f6c 6162 656c 7328 6e70 2e61  pand_labels(np.a
-000049f0: 7361 7272 6179 286c 6162 656c 5f69 6d61  sarray(label_ima
-00004a00: 6765 292c 2064 6973 7461 6e63 653d 6469  ge), distance=di
-00004a10: 7374 616e 6365 290d 0a0d 0a0d 0a40 7265  stance)......@re
-00004a20: 6769 7374 6572 5f66 756e 6374 696f 6e28  gister_function(
-00004a30: 6d65 6e75 3d22 5365 676d 656e 7461 7469  menu="Segmentati
-00004a40: 6f6e 202f 206c 6162 656c 696e 6720 3e20  on / labeling > 
-00004a50: 566f 726f 6e6f 692d 4f74 7375 2d6c 6162  Voronoi-Otsu-lab
-00004a60: 656c 696e 6720 286e 7362 6174 776d 2922  eling (nsbatwm)"
-00004a70: 290d 0a40 6a75 7079 7465 725f 6469 7370  )..@jupyter_disp
-00004a80: 6c61 7961 626c 655f 6f75 7470 7574 286c  layable_output(l
-00004a90: 6962 7261 7279 5f6e 616d 653d 276e 7362  ibrary_name='nsb
-00004aa0: 6174 776d 272c 2068 656c 705f 7572 6c3d  atwm', help_url=
-00004ab0: 2768 7474 7073 3a2f 2f77 7777 2e6e 6170  'https://www.nap
-00004ac0: 6172 692d 6875 622e 6f72 672f 706c 7567  ari-hub.org/plug
-00004ad0: 696e 732f 6e61 7061 7269 2d73 6567 6d65  ins/napari-segme
-00004ae0: 6e74 2d62 6c6f 6273 2d61 6e64 2d74 6869  nt-blobs-and-thi
-00004af0: 6e67 732d 7769 7468 2d6d 656d 6272 616e  ngs-with-membran
-00004b00: 6573 2729 0d0a 4074 696d 655f 736c 6963  es')..@time_slic
-00004b10: 6572 0d0a 6465 6620 766f 726f 6e6f 695f  er..def voronoi_
-00004b20: 6f74 7375 5f6c 6162 656c 696e 6728 696d  otsu_labeling(im
-00004b30: 6167 653a 226e 6170 6172 692e 7479 7065  age:"napari.type
-00004b40: 732e 496d 6167 6544 6174 6122 2c20 7370  s.ImageData", sp
-00004b50: 6f74 5f73 6967 6d61 3a20 666c 6f61 7420  ot_sigma: float 
-00004b60: 3d20 322c 206f 7574 6c69 6e65 5f73 6967  = 2, outline_sig
-00004b70: 6d61 3a20 666c 6f61 7420 3d20 3229 202d  ma: float = 2) -
-00004b80: 3e20 226e 6170 6172 692e 7479 7065 732e  > "napari.types.
-00004b90: 4c61 6265 6c73 4461 7461 223a 0d0a 2020  LabelsData":..  
-00004ba0: 2020 2222 2256 6f72 6f6e 6f69 2d4f 7473    """Voronoi-Ots
-00004bb0: 752d 4c61 6265 6c69 6e67 2069 7320 6120  u-Labeling is a 
-00004bc0: 7365 676d 656e 7461 7469 6f6e 2061 6c67  segmentation alg
-00004bd0: 6f72 6974 686d 2066 6f72 2062 6c6f 622d  orithm for blob-
-00004be0: 6c69 6b65 2073 7472 7563 7475 7265 7320  like structures 
-00004bf0: 7375 6368 2061 7320 6e75 636c 6569 2061  such as nuclei a
-00004c00: 6e64 0d0a 2020 2020 6772 616e 756c 6573  nd..    granules
-00004c10: 2077 6974 6820 6869 6768 2073 6967 6e61   with high signa
-00004c20: 6c20 696e 7465 6e73 6974 7920 6f6e 206c  l intensity on l
-00004c30: 6f77 2d69 6e74 656e 7369 7479 2062 6163  ow-intensity bac
-00004c40: 6b67 726f 756e 642e 0d0a 0d0a 2020 2020  kground.....    
-00004c50: 5468 6520 7477 6f20 7369 676d 6120 7061  The two sigma pa
-00004c60: 7261 6d65 7465 7273 2061 6c6c 6f77 2074  rameters allow t
-00004c70: 756e 696e 6720 7468 6520 7365 676d 656e  uning the segmen
-00004c80: 7461 7469 6f6e 2072 6573 756c 742e 2054  tation result. T
-00004c90: 6865 2066 6972 7374 2073 6967 6d61 2063  he first sigma c
-00004ca0: 6f6e 7472 6f6c 7320 686f 7720 636c 6f73  ontrols how clos
-00004cb0: 6520 6465 7465 6374 6564 2063 656c 6c73  e detected cells
-00004cc0: 0d0a 2020 2020 6361 6e20 6265 2028 7370  ..    can be (sp
-00004cd0: 6f74 5f73 6967 6d61 2920 616e 6420 7468  ot_sigma) and th
-00004ce0: 6520 7365 636f 6e64 2063 6f6e 7472 6f6c  e second control
-00004cf0: 7320 686f 7720 7072 6563 6973 6520 7365  s how precise se
-00004d00: 676d 656e 7465 6420 6f62 6a65 6374 7320  gmented objects 
-00004d10: 6172 6520 6f75 746c 696e 6564 2028 6f75  are outlined (ou
-00004d20: 746c 696e 655f 7369 676d 6129 2e20 556e  tline_sigma). Un
-00004d30: 6465 7220 7468 650d 0a20 2020 2068 6f6f  der the..    hoo
-00004d40: 642c 2074 6869 7320 6669 6c74 6572 2061  d, this filter a
-00004d50: 7070 6c69 6573 2074 776f 2047 6175 7373  pplies two Gauss
-00004d60: 6961 6e20 626c 7572 732c 2073 706f 7420  ian blurs, spot 
-00004d70: 6465 7465 6374 696f 6e2c 204f 7473 752d  detection, Otsu-
-00004d80: 7468 7265 7368 6f6c 6469 6e67 2061 6e64  thresholding and
-00004d90: 2056 6f72 6f6e 6f69 2d6c 6162 656c 696e   Voronoi-labelin
-00004da0: 672e 2054 6865 0d0a 2020 2020 7468 7265  g. The..    thre
-00004db0: 7368 6f6c 6465 6420 6269 6e61 7279 2069  sholded binary i
-00004dc0: 6d61 6765 2069 7320 666c 6f6f 6465 6420  mage is flooded 
-00004dd0: 7573 696e 6720 7468 6520 566f 726f 6e6f  using the Vorono
-00004de0: 6920 6170 7072 6f61 6368 2073 7461 7274  i approach start
-00004df0: 696e 6720 6672 6f6d 2074 6865 2066 6f75  ing from the fou
-00004e00: 6e64 206c 6f63 616c 206d 6178 696d 612e  nd local maxima.
-00004e10: 204e 6f69 7365 2d72 656d 6f76 616c 0d0a   Noise-removal..
-00004e20: 2020 2020 7369 676d 6120 666f 7220 7370      sigma for sp
-00004e30: 6f74 2064 6574 6563 7469 6f6e 2061 6e64  ot detection and
-00004e40: 2074 6872 6573 686f 6c64 696e 6720 6361   thresholding ca
-00004e50: 6e20 6265 2063 6f6e 6669 6775 7265 6420  n be configured 
-00004e60: 7365 7061 7261 7465 6c79 2e0d 0a0d 0a20  separately..... 
-00004e70: 2020 2054 6869 7320 616c 6c6f 7773 2073     This allows s
-00004e80: 6567 6d65 6e74 696e 6720 636f 6e6e 6563  egmenting connec
-00004e90: 7465 6420 6f62 6a65 6374 7320 7375 6368  ted objects such
-00004ea0: 2061 7320 6e6f 7420 746f 2064 656e 7365   as not to dense
-00004eb0: 206e 7563 6c65 692e 0d0a 2020 2020 4966   nuclei...    If
-00004ec0: 2074 6865 206e 7563 6c65 6920 6172 6520   the nuclei are 
-00004ed0: 746f 6f20 6465 6e73 652c 2063 6f6e 7369  too dense, consi
-00004ee0: 6465 7220 7573 696e 6720 7374 6172 6469  der using stardi
-00004ef0: 7374 205b 315d 206f 7220 6365 6c6c 706f  st [1] or cellpo
-00004f00: 7365 205b 325d 2e0d 0a0d 0a20 2020 2053  se [2].....    S
-00004f10: 6565 2061 6c73 6f0d 0a20 2020 202d 2d2d  ee also..    ---
-00004f20: 2d2d 2d2d 2d0d 0a20 2020 202e 2e20 5b30  -----..    .. [0
-00004f30: 5d20 6874 7470 733a 2f2f 6769 7468 7562  ] https://github
-00004f40: 2e63 6f6d 2f63 6c45 7370 6572 616e 746f  .com/clEsperanto
-00004f50: 2f70 7963 6c65 7370 6572 616e 746f 5f70  /pyclesperanto_p
-00004f60: 726f 746f 7479 7065 2f62 6c6f 622f 6d61  rototype/blob/ma
-00004f70: 7374 6572 2f64 656d 6f2f 7365 676d 656e  ster/demo/segmen
-00004f80: 7461 7469 6f6e 2f76 6f72 6f6e 6f69 5f6f  tation/voronoi_o
-00004f90: 7473 755f 6c61 6265 6c69 6e67 2e69 7079  tsu_labeling.ipy
-00004fa0: 6e62 0d0a 2020 2020 2e2e 205b 315d 2068  nb..    .. [1] h
-00004fb0: 7474 7073 3a2f 2f77 7777 2e6e 6170 6172  ttps://www.napar
-00004fc0: 692d 6875 622e 6f72 672f 706c 7567 696e  i-hub.org/plugin
-00004fd0: 732f 7374 6172 6469 7374 2d6e 6170 6172  s/stardist-napar
-00004fe0: 690d 0a20 2020 202e 2e20 5b32 5d20 6874  i..    .. [2] ht
-00004ff0: 7470 733a 2f2f 7777 772e 6e61 7061 7269  tps://www.napari
-00005000: 2d68 7562 2e6f 7267 2f70 6c75 6769 6e73  -hub.org/plugins
-00005010: 2f63 656c 6c70 6f73 652d 6e61 7061 7269  /cellpose-napari
-00005020: 0d0a 2020 2020 2222 220d 0a20 2020 2069  ..    """..    i
-00005030: 6d61 6765 203d 206e 702e 6173 6172 7261  mage = np.asarra
-00005040: 7928 696d 6167 6529 0d0a 0d0a 2020 2020  y(image)....    
-00005050: 2320 626c 7572 2061 6e64 2064 6574 6563  # blur and detec
-00005060: 7420 6c6f 6361 6c20 6d61 7869 6d61 0d0a  t local maxima..
-00005070: 2020 2020 626c 7572 7265 645f 7370 6f74      blurred_spot
-00005080: 7320 3d20 6761 7573 7369 616e 2869 6d61  s = gaussian(ima
-00005090: 6765 2c20 7370 6f74 5f73 6967 6d61 290d  ge, spot_sigma).
-000050a0: 0a20 2020 2073 706f 745f 6365 6e74 726f  .    spot_centro
-000050b0: 6964 7320 3d20 6c6f 6361 6c5f 6d61 7869  ids = local_maxi
-000050c0: 6d61 2862 6c75 7272 6564 5f73 706f 7473  ma(blurred_spots
-000050d0: 290d 0a0d 0a20 2020 2023 2062 6c75 7220  )....    # blur 
-000050e0: 616e 6420 7468 7265 7368 6f6c 640d 0a20  and threshold.. 
-000050f0: 2020 2062 6c75 7272 6564 5f6f 7574 6c69     blurred_outli
-00005100: 6e65 203d 2067 6175 7373 6961 6e28 696d  ne = gaussian(im
-00005110: 6167 652c 206f 7574 6c69 6e65 5f73 6967  age, outline_sig
-00005120: 6d61 290d 0a20 2020 2074 6872 6573 686f  ma)..    thresho
-00005130: 6c64 203d 2073 6b5f 7468 7265 7368 6f6c  ld = sk_threshol
-00005140: 645f 6f74 7375 2862 6c75 7272 6564 5f6f  d_otsu(blurred_o
-00005150: 7574 6c69 6e65 290d 0a20 2020 2062 696e  utline)..    bin
-00005160: 6172 795f 6f74 7375 203d 2062 6c75 7272  ary_otsu = blurr
-00005170: 6564 5f6f 7574 6c69 6e65 203e 2074 6872  ed_outline > thr
-00005180: 6573 686f 6c64 0d0a 0d0a 2020 2020 2320  eshold....    # 
-00005190: 6465 7465 726d 696e 6520 6c6f 6361 6c20  determine local 
-000051a0: 6d61 7869 6d61 2077 6974 6869 6e20 7468  maxima within th
-000051b0: 6520 7468 7265 7368 6f6c 6465 6420 6172  e thresholded ar
-000051c0: 6561 0d0a 2020 2020 7265 6d61 696e 696e  ea..    remainin
-000051d0: 675f 7370 6f74 7320 3d20 7370 6f74 5f63  g_spots = spot_c
-000051e0: 656e 7472 6f69 6473 202a 2062 696e 6172  entroids * binar
-000051f0: 795f 6f74 7375 0d0a 0d0a 2020 2020 2320  y_otsu....    # 
-00005200: 7374 6172 7420 6672 6f6d 2072 656d 6169  start from remai
-00005210: 6e69 6e67 2073 706f 7473 2061 6e64 2066  ning spots and f
-00005220: 6c6f 6f64 2062 696e 6172 7920 696d 6167  lood binary imag
-00005230: 6520 7769 7468 206c 6162 656c 730d 0a20  e with labels.. 
-00005240: 2020 206c 6162 656c 6564 5f73 706f 7473     labeled_spots
-00005250: 203d 206c 6162 656c 2872 656d 6169 6e69   = label(remaini
-00005260: 6e67 5f73 706f 7473 290d 0a20 2020 206c  ng_spots)..    l
-00005270: 6162 656c 7320 3d20 7761 7465 7273 6865  abels = watershe
-00005280: 6428 6269 6e61 7279 5f6f 7473 752c 206c  d(binary_otsu, l
-00005290: 6162 656c 6564 5f73 706f 7473 2c20 6d61  abeled_spots, ma
-000052a0: 736b 3d62 696e 6172 795f 6f74 7375 290d  sk=binary_otsu).
-000052b0: 0a0d 0a20 2020 2072 6574 7572 6e20 6c61  ...    return la
-000052c0: 6265 6c73 0d0a 0d0a 0d0a 4072 6567 6973  bels......@regis
-000052d0: 7465 725f 6675 6e63 7469 6f6e 286d 656e  ter_function(men
-000052e0: 753d 2253 6567 6d65 6e74 6174 696f 6e20  u="Segmentation 
-000052f0: 2f20 6c61 6265 6c69 6e67 203e 2047 6175  / labeling > Gau
-00005300: 7373 2d4f 7473 752d 6c61 6265 6c69 6e67  ss-Otsu-labeling
-00005310: 2028 6e73 6261 7477 6d29 2229 0d0a 406a   (nsbatwm)")..@j
-00005320: 7570 7974 6572 5f64 6973 706c 6179 6162  upyter_displayab
-00005330: 6c65 5f6f 7574 7075 7428 6c69 6272 6172  le_output(librar
-00005340: 795f 6e61 6d65 3d27 6e73 6261 7477 6d27  y_name='nsbatwm'
-00005350: 2c20 6865 6c70 5f75 726c 3d27 6874 7470  , help_url='http
-00005360: 733a 2f2f 7777 772e 6e61 7061 7269 2d68  s://www.napari-h
-00005370: 7562 2e6f 7267 2f70 6c75 6769 6e73 2f6e  ub.org/plugins/n
-00005380: 6170 6172 692d 7365 676d 656e 742d 626c  apari-segment-bl
-00005390: 6f62 732d 616e 642d 7468 696e 6773 2d77  obs-and-things-w
-000053a0: 6974 682d 6d65 6d62 7261 6e65 7327 290d  ith-membranes').
-000053b0: 0a40 7469 6d65 5f73 6c69 6365 720d 0a64  .@time_slicer..d
-000053c0: 6566 2067 6175 7373 5f6f 7473 755f 6c61  ef gauss_otsu_la
-000053d0: 6265 6c69 6e67 2869 6d61 6765 3a22 6e61  beling(image:"na
-000053e0: 7061 7269 2e74 7970 6573 2e49 6d61 6765  pari.types.Image
-000053f0: 4461 7461 222c 206f 7574 6c69 6e65 5f73  Data", outline_s
-00005400: 6967 6d61 3a20 666c 6f61 7420 3d20 3229  igma: float = 2)
-00005410: 202d 3e20 226e 6170 6172 692e 7479 7065   -> "napari.type
-00005420: 732e 4c61 6265 6c73 4461 7461 223a 0d0a  s.LabelsData":..
-00005430: 2020 2020 2222 2247 6175 7373 2d4f 7473      """Gauss-Ots
-00005440: 752d 4c61 6265 6c69 6e67 2063 616e 2062  u-Labeling can b
-00005450: 6520 7573 6564 2074 6f20 7365 676d 656e  e used to segmen
-00005460: 7420 6f62 6a65 6374 7320 7375 6368 2061  t objects such a
-00005470: 7320 6e75 636c 6569 2077 6974 6820 6272  s nuclei with br
-00005480: 6967 6874 2069 6e74 656e 7369 7479 206f  ight intensity o
-00005490: 6e0d 0a20 2020 206c 6f77 2069 6e74 656e  n..    low inten
-000054a0: 7369 7479 2062 6163 6b67 726f 756e 6420  sity background 
-000054b0: 696d 6167 6573 2e0d 0a0d 0a20 2020 2054  images.....    T
-000054c0: 6865 206f 7574 6c69 6e65 5f73 6967 6d61  he outline_sigma
-000054d0: 2070 6172 616d 6574 6572 2061 6c6c 6f77   parameter allow
-000054e0: 7320 7475 6e69 6e67 2068 6f77 2070 7265  s tuning how pre
-000054f0: 6369 7365 2073 6567 6d65 6e74 6564 206f  cise segmented o
-00005500: 626a 6563 7473 2061 7265 206f 7574 6c69  bjects are outli
-00005510: 6e65 642e 2055 6e64 6572 2074 6865 0d0a  ned. Under the..
-00005520: 2020 2020 686f 6f64 2c20 7468 6973 2066      hood, this f
-00005530: 696c 7465 7220 6170 706c 6965 7320 6120  ilter applies a 
-00005540: 4761 7573 7369 616e 2062 6c75 722c 204f  Gaussian blur, O
-00005550: 7473 752d 7468 7265 7368 6f6c 6469 6e67  tsu-thresholding
-00005560: 2061 6e64 2063 6f6e 6e65 6374 6564 2063   and connected c
-00005570: 6f6d 706f 6e65 6e74 206c 6162 656c 696e  omponent labelin
-00005580: 672e 0d0a 0d0a 2020 2020 5365 6520 616c  g.....    See al
-00005590: 736f 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d  so..    --------
-000055a0: 0d0a 2020 2020 2e2e 205b 305d 2068 7474  ..    .. [0] htt
-000055b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000055c0: 636c 4573 7065 7261 6e74 6f2f 7079 636c  clEsperanto/pycl
-000055d0: 6573 7065 7261 6e74 6f5f 7072 6f74 6f74  esperanto_protot
-000055e0: 7970 652f 626c 6f62 2f6d 6173 7465 722f  ype/blob/master/
-000055f0: 6465 6d6f 2f73 6567 6d65 6e74 6174 696f  demo/segmentatio
-00005600: 6e2f 6761 7573 735f 6f74 7375 5f6c 6162  n/gauss_otsu_lab
-00005610: 656c 696e 672e 6970 796e 620d 0a20 2020  eling.ipynb..   
-00005620: 2022 2222 0d0a 2020 2020 696d 6167 6520   """..    image 
-00005630: 3d20 6e70 2e61 7361 7272 6179 2869 6d61  = np.asarray(ima
-00005640: 6765 290d 0a0d 0a20 2020 2023 2062 6c75  ge)....    # blu
-00005650: 720d 0a20 2020 2062 6c75 7272 6564 5f6f  r..    blurred_o
-00005660: 7574 6c69 6e65 203d 2067 6175 7373 6961  utline = gaussia
-00005670: 6e28 696d 6167 652c 206f 7574 6c69 6e65  n(image, outline
-00005680: 5f73 6967 6d61 290d 0a0d 0a20 2020 2023  _sigma)....    #
-00005690: 2074 6872 6573 686f 6c64 0d0a 2020 2020   threshold..    
-000056a0: 7468 7265 7368 6f6c 6420 3d20 736b 5f74  threshold = sk_t
-000056b0: 6872 6573 686f 6c64 5f6f 7473 7528 626c  hreshold_otsu(bl
-000056c0: 7572 7265 645f 6f75 746c 696e 6529 0d0a  urred_outline)..
-000056d0: 2020 2020 6269 6e61 7279 5f6f 7473 7520      binary_otsu 
-000056e0: 3d20 626c 7572 7265 645f 6f75 746c 696e  = blurred_outlin
-000056f0: 6520 3e20 7468 7265 7368 6f6c 640d 0a0d  e > threshold...
-00005700: 0a20 2020 2023 2063 6f6e 6e65 6374 6564  .    # connected
-00005710: 2063 6f6d 706f 6e65 6e74 206c 6162 656c   component label
-00005720: 696e 670d 0a20 2020 206c 6162 656c 7320  ing..    labels 
-00005730: 3d20 6c61 6265 6c28 6269 6e61 7279 5f6f  = label(binary_o
-00005740: 7473 7529 0d0a 0d0a 2020 2020 7265 7475  tsu)....    retu
-00005750: 726e 206c 6162 656c 730d 0a0d 0a0d 0a40  rn labels......@
-00005760: 7265 6769 7374 6572 5f66 756e 6374 696f  register_functio
-00005770: 6e28 6d65 6e75 3d22 5365 676d 656e 7461  n(menu="Segmenta
-00005780: 7469 6f6e 202f 206c 6162 656c 696e 6720  tion / labeling 
-00005790: 3e20 5365 6564 6564 2077 6174 6572 7368  > Seeded watersh
-000057a0: 6564 2028 7363 696b 6974 2d69 6d61 6765  ed (scikit-image
-000057b0: 2c20 6e73 6261 7477 6d29 2229 0d0a 406a  , nsbatwm)")..@j
-000057c0: 7570 7974 6572 5f64 6973 706c 6179 6162  upyter_displayab
-000057d0: 6c65 5f6f 7574 7075 7428 6c69 6272 6172  le_output(librar
-000057e0: 795f 6e61 6d65 3d27 6e73 6261 7477 6d27  y_name='nsbatwm'
-000057f0: 2c20 6865 6c70 5f75 726c 3d27 6874 7470  , help_url='http
-00005800: 733a 2f2f 7777 772e 6e61 7061 7269 2d68  s://www.napari-h
-00005810: 7562 2e6f 7267 2f70 6c75 6769 6e73 2f6e  ub.org/plugins/n
-00005820: 6170 6172 692d 7365 676d 656e 742d 626c  apari-segment-bl
-00005830: 6f62 732d 616e 642d 7468 696e 6773 2d77  obs-and-things-w
-00005840: 6974 682d 6d65 6d62 7261 6e65 7327 290d  ith-membranes').
-00005850: 0a40 7469 6d65 5f73 6c69 6365 720d 0a64  .@time_slicer..d
-00005860: 6566 2073 6565 6465 645f 7761 7465 7273  ef seeded_waters
-00005870: 6865 6428 6d65 6d62 7261 6e65 733a 226e  hed(membranes:"n
-00005880: 6170 6172 692e 7479 7065 732e 496d 6167  apari.types.Imag
-00005890: 6544 6174 6122 2c20 6c61 6265 6c65 645f  eData", labeled_
-000058a0: 6e75 636c 6569 3a22 6e61 7061 7269 2e74  nuclei:"napari.t
-000058b0: 7970 6573 2e4c 6162 656c 7344 6174 6122  ypes.LabelsData"
-000058c0: 2920 2d3e 2022 6e61 7061 7269 2e74 7970  ) -> "napari.typ
-000058d0: 6573 2e4c 6162 656c 7344 6174 6122 3a0d  es.LabelsData":.
-000058e0: 0a20 2020 2022 2222 0d0a 2020 2020 5461  .    """..    Ta
-000058f0: 6b65 7320 6120 696d 6167 6520 7769 7468  kes a image with
-00005900: 2062 7269 6768 7420 2868 6967 6820 696e   bright (high in
-00005910: 7465 6e73 6974 7929 206d 656d 6272 616e  tensity) membran
-00005920: 6573 2061 6e64 2061 6e20 696d 6167 6520  es and an image 
-00005930: 7769 7468 206c 6162 656c 6564 206f 626a  with labeled obj
-00005940: 6563 7473 2073 7563 6820 6173 206e 7563  ects such as nuc
-00005950: 6c65 692e 0d0a 2020 2020 5468 6520 6c61  lei...    The la
-00005960: 7474 6572 2073 6572 7665 7320 6173 2073  tter serves as s
-00005970: 6565 6473 2069 6d61 6765 2066 6f72 2061  eeds image for a
-00005980: 2077 6174 6572 7368 6564 206c 6162 656c   watershed label
-00005990: 696e 672e 0d0a 0d0a 2020 2020 5365 6520  ing.....    See 
-000059a0: 616c 736f 0d0a 2020 2020 2d2d 2d2d 2d2d  also..    ------
-000059b0: 2d2d 0d0a 2020 2020 2e2e 205b 315d 2068  --..    .. [1] h
-000059c0: 7474 7073 3a2f 2f73 6369 6b69 742d 696d  ttps://scikit-im
-000059d0: 6167 652e 6f72 672f 646f 6373 2f64 6576  age.org/docs/dev
-000059e0: 2f61 7574 6f5f 6578 616d 706c 6573 2f73  /auto_examples/s
-000059f0: 6567 6d65 6e74 6174 696f 6e2f 706c 6f74  egmentation/plot
-00005a00: 5f77 6174 6572 7368 6564 2e68 746d 6c0d  _watershed.html.
-00005a10: 0a20 2020 2022 2222 0d0a 2020 2020 6365  .    """..    ce
-00005a20: 6c6c 7320 3d20 7761 7465 7273 6865 6428  lls = watershed(
-00005a30: 0d0a 2020 2020 2020 2020 6e70 2e61 7361  ..        np.asa
-00005a40: 7272 6179 286d 656d 6272 616e 6573 292c  rray(membranes),
-00005a50: 0d0a 2020 2020 2020 2020 6e70 2e61 7361  ..        np.asa
-00005a60: 7272 6179 286c 6162 656c 6564 5f6e 7563  rray(labeled_nuc
-00005a70: 6c65 6929 0d0a 2020 2020 290d 0a20 2020  lei)..    )..   
-00005a80: 2072 6574 7572 6e20 6365 6c6c 730d 0a0d   return cells...
-00005a90: 0a40 7265 6769 7374 6572 5f66 756e 6374  .@register_funct
-00005aa0: 696f 6e28 6d65 6e75 3d22 5365 676d 656e  ion(menu="Segmen
-00005ab0: 7461 7469 6f6e 202f 206c 6162 656c 696e  tation / labelin
-00005ac0: 6720 3e20 5365 6564 6564 2077 6174 6572  g > Seeded water
-00005ad0: 7368 6564 2077 6974 6820 6d61 736b 2028  shed with mask (
-00005ae0: 7363 696b 6974 2d69 6d61 6765 2c20 6e73  scikit-image, ns
-00005af0: 6261 7477 6d29 2229 0d0a 406a 7570 7974  batwm)")..@jupyt
-00005b00: 6572 5f64 6973 706c 6179 6162 6c65 5f6f  er_displayable_o
-00005b10: 7574 7075 7428 6c69 6272 6172 795f 6e61  utput(library_na
-00005b20: 6d65 3d27 6e73 6261 7477 6d27 2c20 6865  me='nsbatwm', he
-00005b30: 6c70 5f75 726c 3d27 6874 7470 733a 2f2f  lp_url='https://
-00005b40: 7777 772e 6e61 7061 7269 2d68 7562 2e6f  www.napari-hub.o
-00005b50: 7267 2f70 6c75 6769 6e73 2f6e 6170 6172  rg/plugins/napar
-00005b60: 692d 7365 676d 656e 742d 626c 6f62 732d  i-segment-blobs-
-00005b70: 616e 642d 7468 696e 6773 2d77 6974 682d  and-things-with-
-00005b80: 6d65 6d62 7261 6e65 7327 290d 0a40 7469  membranes')..@ti
-00005b90: 6d65 5f73 6c69 6365 720d 0a64 6566 2073  me_slicer..def s
-00005ba0: 6565 6465 645f 7761 7465 7273 6865 645f  eeded_watershed_
-00005bb0: 7769 7468 5f6d 6173 6b28 6d65 6d62 7261  with_mask(membra
-00005bc0: 6e65 733a 226e 6170 6172 692e 7479 7065  nes:"napari.type
-00005bd0: 732e 496d 6167 6544 6174 6122 2c20 6c61  s.ImageData", la
-00005be0: 6265 6c65 645f 6e75 636c 6569 3a22 6e61  beled_nuclei:"na
-00005bf0: 7061 7269 2e74 7970 6573 2e4c 6162 656c  pari.types.Label
-00005c00: 7344 6174 6122 2c20 6d61 736b 3a22 6e61  sData", mask:"na
-00005c10: 7061 7269 2e74 7970 6573 2e4c 6162 656c  pari.types.Label
-00005c20: 7344 6174 6122 2920 2d3e 2022 6e61 7061  sData") -> "napa
-00005c30: 7269 2e74 7970 6573 2e4c 6162 656c 7344  ri.types.LabelsD
-00005c40: 6174 6122 3a0d 0a20 2020 2022 2222 0d0a  ata":..    """..
-00005c50: 2020 2020 5461 6b65 7320 6120 696d 6167      Takes a imag
-00005c60: 6520 7769 7468 2062 7269 6768 7420 2868  e with bright (h
-00005c70: 6967 6820 696e 7465 6e73 6974 7929 206d  igh intensity) m
-00005c80: 656d 6272 616e 6573 2c20 616e 2069 6d61  embranes, an ima
-00005c90: 6765 2077 6974 6820 6c61 6265 6c65 6420  ge with labeled 
-00005ca0: 6f62 6a65 6374 7320 7375 6368 2061 7320  objects such as 
-00005cb0: 6e75 636c 6569 2061 6e64 2061 206d 6173  nuclei and a mas
-00005cc0: 6b20 696d 6765 2c20 652e 672e 2061 2062  k imge, e.g. a b
-00005cd0: 696e 6172 7920 696d 6167 6520 6f66 2074  inary image of t
-00005ce0: 6865 2065 6e74 6972 6520 7469 7373 7565  he entire tissue
-00005cf0: 206f 6620 696e 7465 7265 7374 2e0d 0a20   of interest... 
-00005d00: 2020 2054 6865 206c 6162 656c 6564 206e     The labeled n
-00005d10: 7563 6c65 6920 7365 7276 6520 6173 2073  uclei serve as s
-00005d20: 6565 6473 2069 6d61 6765 2066 6f72 2061  eeds image for a
-00005d30: 2077 6174 6572 7368 6564 206c 6162 656c   watershed label
-00005d40: 696e 6720 616e 6420 7468 6520 6d61 736b  ing and the mask
-00005d50: 2066 6f72 2063 6f6e 7374 7261 696e 7469   for constrainti
-00005d60: 6e67 2074 6865 2066 6c6f 6f64 696e 672e  ng the flooding.
-00005d70: 0d0a 0d0a 2020 2020 5365 6520 616c 736f  ....    See also
-00005d80: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a  ..    --------..
-00005d90: 2020 2020 2e2e 205b 315d 2068 7474 7073      .. [1] https
-00005da0: 3a2f 2f73 6369 6b69 742d 696d 6167 652e  ://scikit-image.
-00005db0: 6f72 672f 646f 6373 2f64 6576 2f61 7574  org/docs/dev/aut
-00005dc0: 6f5f 6578 616d 706c 6573 2f73 6567 6d65  o_examples/segme
-00005dd0: 6e74 6174 696f 6e2f 706c 6f74 5f77 6174  ntation/plot_wat
-00005de0: 6572 7368 6564 2e68 746d 6c0d 0a20 2020  ershed.html..   
-00005df0: 2022 2222 0d0a 2020 2020 6365 6c6c 7320   """..    cells 
-00005e00: 3d20 7761 7465 7273 6865 6428 0d0a 2020  = watershed(..  
-00005e10: 2020 2020 2020 6e70 2e61 7361 7272 6179        np.asarray
-00005e20: 286d 656d 6272 616e 6573 292c 0d0a 2020  (membranes),..  
-00005e30: 2020 2020 2020 6e70 2e61 7361 7272 6179        np.asarray
-00005e40: 286c 6162 656c 6564 5f6e 7563 6c65 6929  (labeled_nuclei)
-00005e50: 2c0d 0a20 2020 2020 2020 206d 6173 6b3d  ,..        mask=
-00005e60: 6d61 736b 0d0a 2020 2020 290d 0a20 2020  mask..    )..   
-00005e70: 2072 6574 7572 6e20 6365 6c6c 730d 0a0d   return cells...
-00005e80: 0a0d 0a40 7265 6769 7374 6572 5f66 756e  ...@register_fun
-00005e90: 6374 696f 6e28 6d65 6e75 3d22 5365 676d  ction(menu="Segm
-00005ea0: 656e 7461 7469 6f6e 202f 206c 6162 656c  entation / label
-00005eb0: 696e 6720 3e20 5365 6564 6564 2077 6174  ing > Seeded wat
-00005ec0: 6572 7368 6564 2075 7369 6e67 206c 6f63  ershed using loc
-00005ed0: 616c 206d 696e 696d 6120 6173 2073 6565  al minima as see
-00005ee0: 6473 2028 6e73 6261 7477 6d29 2229 0d0a  ds (nsbatwm)")..
-00005ef0: 406a 7570 7974 6572 5f64 6973 706c 6179  @jupyter_display
-00005f00: 6162 6c65 5f6f 7574 7075 7428 6c69 6272  able_output(libr
-00005f10: 6172 795f 6e61 6d65 3d27 6e73 6261 7477  ary_name='nsbatw
-00005f20: 6d27 2c20 6865 6c70 5f75 726c 3d27 6874  m', help_url='ht
-00005f30: 7470 733a 2f2f 7777 772e 6e61 7061 7269  tps://www.napari
-00005f40: 2d68 7562 2e6f 7267 2f70 6c75 6769 6e73  -hub.org/plugins
-00005f50: 2f6e 6170 6172 692d 7365 676d 656e 742d  /napari-segment-
-00005f60: 626c 6f62 732d 616e 642d 7468 696e 6773  blobs-and-things
-00005f70: 2d77 6974 682d 6d65 6d62 7261 6e65 7327  -with-membranes'
-00005f80: 290d 0a40 7469 6d65 5f73 6c69 6365 720d  )..@time_slicer.
-00005f90: 0a64 6566 206c 6f63 616c 5f6d 696e 696d  .def local_minim
-00005fa0: 615f 7365 6564 6564 5f77 6174 6572 7368  a_seeded_watersh
-00005fb0: 6564 2869 6d61 6765 3a22 6e61 7061 7269  ed(image:"napari
-00005fc0: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
-00005fd0: 222c 2073 706f 745f 7369 676d 613a 2066  ", spot_sigma: f
-00005fe0: 6c6f 6174 203d 2031 302c 206f 7574 6c69  loat = 10, outli
-00005ff0: 6e65 5f73 6967 6d61 3a20 666c 6f61 7420  ne_sigma: float 
-00006000: 3d20 3029 202d 3e20 226e 6170 6172 692e  = 0) -> "napari.
-00006010: 7479 7065 732e 4c61 6265 6c73 4461 7461  types.LabelsData
-00006020: 223a 0d0a 2020 2020 2222 220d 0a20 2020  ":..    """..   
-00006030: 2053 6567 6d65 6e74 2063 656c 6c73 2069   Segment cells i
-00006040: 6e20 696d 6167 6573 2077 6974 6820 666c  n images with fl
-00006050: 756f 7265 7363 656e 746c 7920 6d61 726b  uorescently mark
-00006060: 6564 206d 656d 6272 616e 6573 2e0d 0a0d  ed membranes....
-00006070: 0a20 2020 2054 6865 2074 776f 2073 6967  .    The two sig
-00006080: 6d61 2070 6172 616d 6574 6572 7320 616c  ma parameters al
-00006090: 6c6f 7720 7475 6e69 6e67 2074 6865 2073  low tuning the s
-000060a0: 6567 6d65 6e74 6174 696f 6e20 7265 7375  egmentation resu
-000060b0: 6c74 2e20 5468 6520 6669 7273 7420 7369  lt. The first si
-000060c0: 676d 6120 636f 6e74 726f 6c73 2068 6f77  gma controls how
-000060d0: 2063 6c6f 7365 2064 6574 6563 7465 6420   close detected 
-000060e0: 6365 6c6c 730d 0a20 2020 2063 616e 2062  cells..    can b
-000060f0: 6520 2873 706f 745f 7369 676d 6129 2061  e (spot_sigma) a
-00006100: 6e64 2074 6865 2073 6563 6f6e 6420 636f  nd the second co
-00006110: 6e74 726f 6c73 2068 6f77 2070 7265 6369  ntrols how preci
-00006120: 7365 2073 6567 6d65 6e74 6564 206f 626a  se segmented obj
-00006130: 6563 7473 2061 7265 206f 7574 6c69 6e65  ects are outline
-00006140: 6420 286f 7574 6c69 6e65 5f73 6967 6d61  d (outline_sigma
-00006150: 292e 2055 6e64 6572 2074 6865 0d0a 2020  ). Under the..  
-00006160: 2020 686f 6f64 2c20 7468 6973 2066 696c    hood, this fil
-00006170: 7465 7220 6170 706c 6965 7320 7477 6f20  ter applies two 
-00006180: 4761 7573 7369 616e 2062 6c75 7273 2c20  Gaussian blurs, 
-00006190: 6c6f 6361 6c20 6d69 6e69 6d61 2064 6574  local minima det
-000061a0: 6563 7469 6f6e 2061 6e64 2061 2073 6565  ection and a see
-000061b0: 6465 6420 7761 7465 7273 6865 642e 0d0a  ded watershed...
-000061c0: 0d0a 2020 2020 5365 6520 616c 736f 0d0a  ..    See also..
-000061d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020      --------..  
-000061e0: 2020 2e2e 205b 315d 2068 7474 7073 3a2f    .. [1] https:/
-000061f0: 2f73 6369 6b69 742d 696d 6167 652e 6f72  /scikit-image.or
-00006200: 672f 646f 6373 2f64 6576 2f61 7574 6f5f  g/docs/dev/auto_
-00006210: 6578 616d 706c 6573 2f73 6567 6d65 6e74  examples/segment
-00006220: 6174 696f 6e2f 706c 6f74 5f77 6174 6572  ation/plot_water
-00006230: 7368 6564 2e68 746d 6c0d 0a20 2020 2022  shed.html..    "
-00006240: 2222 0d0a 0d0a 2020 2020 696d 6167 6520  ""....    image 
-00006250: 3d20 6e70 2e61 7361 7272 6179 2869 6d61  = np.asarray(ima
-00006260: 6765 290d 0a0d 0a20 2020 2073 706f 745f  ge)....    spot_
-00006270: 626c 7572 7265 6420 3d20 6761 7573 7369  blurred = gaussi
-00006280: 616e 2869 6d61 6765 2c20 7369 676d 613d  an(image, sigma=
-00006290: 7370 6f74 5f73 6967 6d61 290d 0a0d 0a20  spot_sigma).... 
-000062a0: 2020 2073 706f 7473 203d 206c 6162 656c     spots = label
-000062b0: 286c 6f63 616c 5f6d 696e 696d 6128 7370  (local_minima(sp
-000062c0: 6f74 5f62 6c75 7272 6564 2929 0d0a 0d0a  ot_blurred))....
-000062d0: 2020 2020 6966 206f 7574 6c69 6e65 5f73      if outline_s
-000062e0: 6967 6d61 203d 3d20 7370 6f74 5f73 6967  igma == spot_sig
-000062f0: 6d61 3a0d 0a20 2020 2020 2020 206f 7574  ma:..        out
-00006300: 6c69 6e65 5f62 6c75 7272 6564 203d 2073  line_blurred = s
-00006310: 706f 745f 626c 7572 7265 640d 0a20 2020  pot_blurred..   
-00006320: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00006330: 6f75 746c 696e 655f 626c 7572 7265 6420  outline_blurred 
-00006340: 3d20 6761 7573 7369 616e 2869 6d61 6765  = gaussian(image
-00006350: 2c20 7369 676d 613d 6f75 746c 696e 655f  , sigma=outline_
-00006360: 7369 676d 6129 0d0a 0d0a 2020 2020 7265  sigma)....    re
-00006370: 7475 726e 2077 6174 6572 7368 6564 286f  turn watershed(o
-00006380: 7574 6c69 6e65 5f62 6c75 7272 6564 2c20  utline_blurred, 
-00006390: 7370 6f74 7329 0d0a 0d0a 0d0a 4072 6567  spots)......@reg
-000063a0: 6973 7465 725f 6675 6e63 7469 6f6e 286d  ister_function(m
-000063b0: 656e 753d 2253 6567 6d65 6e74 6174 696f  enu="Segmentatio
-000063c0: 6e20 2f20 6c61 6265 6c69 6e67 203e 2053  n / labeling > S
-000063d0: 6565 6465 6420 7761 7465 7273 6865 6420  eeded watershed 
-000063e0: 7573 696e 6720 6c6f 6361 6c20 6d69 6e69  using local mini
-000063f0: 6d61 2061 7320 7365 6564 7320 616e 6420  ma as seeds and 
-00006400: 616e 2069 6e74 656e 7369 7479 2074 6872  an intensity thr
-00006410: 6573 686f 6c64 2028 6e73 6261 7477 6d29  eshold (nsbatwm)
-00006420: 2229 0d0a 406a 7570 7974 6572 5f64 6973  ")..@jupyter_dis
-00006430: 706c 6179 6162 6c65 5f6f 7574 7075 7428  playable_output(
-00006440: 6c69 6272 6172 795f 6e61 6d65 3d27 6e73  library_name='ns
-00006450: 6261 7477 6d27 2c20 6865 6c70 5f75 726c  batwm', help_url
-00006460: 3d27 6874 7470 733a 2f2f 7777 772e 6e61  ='https://www.na
-00006470: 7061 7269 2d68 7562 2e6f 7267 2f70 6c75  pari-hub.org/plu
-00006480: 6769 6e73 2f6e 6170 6172 692d 7365 676d  gins/napari-segm
-00006490: 656e 742d 626c 6f62 732d 616e 642d 7468  ent-blobs-and-th
-000064a0: 696e 6773 2d77 6974 682d 6d65 6d62 7261  ings-with-membra
-000064b0: 6e65 7327 290d 0a40 7469 6d65 5f73 6c69  nes')..@time_sli
-000064c0: 6365 720d 0a64 6566 2074 6872 6573 686f  cer..def thresho
-000064d0: 6c64 6564 5f6c 6f63 616c 5f6d 696e 696d  lded_local_minim
-000064e0: 615f 7365 6564 6564 5f77 6174 6572 7368  a_seeded_watersh
-000064f0: 6564 2869 6d61 6765 3a22 6e61 7061 7269  ed(image:"napari
-00006500: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
-00006510: 222c 2073 706f 745f 7369 676d 613a 2066  ", spot_sigma: f
-00006520: 6c6f 6174 203d 2033 2c20 6f75 746c 696e  loat = 3, outlin
-00006530: 655f 7369 676d 613a 2066 6c6f 6174 203d  e_sigma: float =
-00006540: 2030 2c20 6d69 6e69 6d75 6d5f 696e 7465   0, minimum_inte
-00006550: 6e73 6974 793a 2066 6c6f 6174 203d 2035  nsity: float = 5
-00006560: 3030 2920 2d3e 2022 6e61 7061 7269 2e74  00) -> "napari.t
-00006570: 7970 6573 2e4c 6162 656c 7344 6174 6122  ypes.LabelsData"
-00006580: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-00006590: 5365 676d 656e 7420 6365 6c6c 7320 696e  Segment cells in
-000065a0: 2069 6d61 6765 7320 7769 7468 206d 6172   images with mar
-000065b0: 6b65 6420 6d65 6d62 7261 6e65 7320 7468  ked membranes th
-000065c0: 6174 2068 6176 6520 6120 6869 6768 2073  at have a high s
-000065d0: 6967 6e61 6c20 696e 7465 6e73 6974 792e  ignal intensity.
-000065e0: 0d0a 0d0a 2020 2020 5468 6520 7477 6f20  ....    The two 
-000065f0: 7369 676d 6120 7061 7261 6d65 7465 7273  sigma parameters
-00006600: 2061 6c6c 6f77 2074 756e 696e 6720 7468   allow tuning th
-00006610: 6520 7365 676d 656e 7461 7469 6f6e 2072  e segmentation r
-00006620: 6573 756c 742e 2054 6865 2066 6972 7374  esult. The first
-00006630: 2073 6967 6d61 2063 6f6e 7472 6f6c 7320   sigma controls 
-00006640: 686f 7720 636c 6f73 6520 6465 7465 6374  how close detect
-00006650: 6564 2063 656c 6c73 0d0a 2020 2020 6361  ed cells..    ca
-00006660: 6e20 6265 2028 7370 6f74 5f73 6967 6d61  n be (spot_sigma
-00006670: 2920 616e 6420 7468 6520 7365 636f 6e64  ) and the second
-00006680: 2063 6f6e 7472 6f6c 7320 686f 7720 7072   controls how pr
-00006690: 6563 6973 6520 7365 676d 656e 7465 6420  ecise segmented 
-000066a0: 6f62 6a65 6374 7320 6172 6520 6f75 746c  objects are outl
-000066b0: 696e 6564 2028 6f75 746c 696e 655f 7369  ined (outline_si
-000066c0: 676d 6129 2e20 556e 6465 7220 7468 650d  gma). Under the.
-000066d0: 0a20 2020 2068 6f6f 642c 2074 6869 7320  .    hood, this 
-000066e0: 6669 6c74 6572 2061 7070 6c69 6573 2074  filter applies t
-000066f0: 776f 2047 6175 7373 6961 6e20 626c 7572  wo Gaussian blur
-00006700: 732c 206c 6f63 616c 206d 696e 696d 6120  s, local minima 
-00006710: 6465 7465 6374 696f 6e20 616e 6420 6120  detection and a 
-00006720: 7365 6564 6564 2077 6174 6572 7368 6564  seeded watershed
-00006730: 2e0d 0a0d 0a20 2020 2041 6674 6572 7761  .....    Afterwa
-00006740: 7264 732c 2061 6c6c 206f 626a 6563 7473  rds, all objects
-00006750: 2061 7265 2072 656d 6f76 6564 2074 6861   are removed tha
-00006760: 7420 6861 7665 2061 6e20 6176 6572 6167  t have an averag
-00006770: 6520 696e 7465 6e73 6974 7920 6265 6c6f  e intensity belo
-00006780: 7720 6120 6769 7665 6e20 6d69 6e69 6d75  w a given minimu
-00006790: 6d5f 696e 7465 6e73 6974 790d 0a20 2020  m_intensity..   
-000067a0: 2022 2222 0d0a 2020 2020 6c61 6265 6c73   """..    labels
-000067b0: 203d 206c 6f63 616c 5f6d 696e 696d 615f   = local_minima_
-000067c0: 7365 6564 6564 5f77 6174 6572 7368 6564  seeded_watershed
-000067d0: 2869 6d61 6765 2c20 7370 6f74 5f73 6967  (image, spot_sig
-000067e0: 6d61 3d73 706f 745f 7369 676d 612c 206f  ma=spot_sigma, o
-000067f0: 7574 6c69 6e65 5f73 6967 6d61 3d6f 7574  utline_sigma=out
-00006800: 6c69 6e65 5f73 6967 6d61 290d 0a0d 0a20  line_sigma).... 
-00006810: 2020 2023 206d 6561 7375 7265 2069 6e74     # measure int
-00006820: 656e 7369 7469 6573 0d0a 2020 2020 7374  ensities..    st
-00006830: 6174 7320 3d20 7265 6769 6f6e 7072 6f70  ats = regionprop
-00006840: 7328 6c61 6265 6c73 2c20 696d 6167 6529  s(labels, image)
-00006850: 0d0a 2020 2020 696e 7465 6e73 6974 6965  ..    intensitie
-00006860: 7320 3d20 5b72 2e6d 6561 6e5f 696e 7465  s = [r.mean_inte
-00006870: 6e73 6974 7920 666f 7220 7220 696e 2073  nsity for r in s
-00006880: 7461 7473 5d0d 0a0d 0a20 2020 2023 2066  tats]....    # f
-00006890: 696c 7465 7220 6c61 6265 6c73 2077 6974  ilter labels wit
-000068a0: 6820 6c6f 7720 696e 7465 6e73 6974 790d  h low intensity.
-000068b0: 0a20 2020 206e 6577 5f6c 6162 656c 5f69  .    new_label_i
-000068c0: 6e64 6963 6573 2c20 5f2c 205f 203d 2072  ndices, _, _ = r
-000068d0: 656c 6162 656c 5f73 6571 7565 6e74 6961  elabel_sequentia
-000068e0: 6c28 286e 702e 6173 6172 7261 7928 696e  l((np.asarray(in
-000068f0: 7465 6e73 6974 6965 7329 203e 206d 696e  tensities) > min
-00006900: 696d 756d 5f69 6e74 656e 7369 7479 2920  imum_intensity) 
-00006910: 2a20 6e70 2e61 7261 6e67 6528 6c61 6265  * np.arange(labe
-00006920: 6c73 2e6d 6178 2829 2929 0d0a 2020 2020  ls.max()))..    
-00006930: 6e65 775f 6c61 6265 6c5f 696e 6469 6365  new_label_indice
-00006940: 7320 3d20 6e70 2e69 6e73 6572 7428 6e65  s = np.insert(ne
-00006950: 775f 6c61 6265 6c5f 696e 6469 6365 732c  w_label_indices,
-00006960: 2030 2c20 3029 0d0a 2020 2020 6e65 775f   0, 0)..    new_
-00006970: 6c61 6265 6c73 203d 206e 702e 7461 6b65  labels = np.take
-00006980: 286e 702e 6173 6172 7261 7928 6e65 775f  (np.asarray(new_
-00006990: 6c61 6265 6c5f 696e 6469 6365 732c 206e  label_indices, n
-000069a0: 702e 7569 6e74 3332 292c 206c 6162 656c  p.uint32), label
-000069b0: 7329 0d0a 0d0a 2020 2020 7265 7475 726e  s)....    return
-000069c0: 206e 6577 5f6c 6162 656c 730d 0a0d 0a40   new_labels....@
-000069d0: 7265 6769 7374 6572 5f66 756e 6374 696f  register_functio
-000069e0: 6e28 6d65 6e75 3d22 496d 6167 6520 6d61  n(menu="Image ma
-000069f0: 7468 203e 2053 756d 2069 6d61 6765 7320  th > Sum images 
-00006a00: 286e 756d 7079 2c20 6e73 6261 7477 6d29  (numpy, nsbatwm)
-00006a10: 222c 2066 6163 746f 7231 3d7b 276d 696e  ", factor1={'min
-00006a20: 273a 202d 3130 3030 3030 302c 2027 6d61  ': -1000000, 'ma
-00006a30: 7827 3a20 3130 3030 3030 307d 2c20 6661  x': 1000000}, fa
-00006a40: 6374 6f72 323d 7b27 6d69 6e27 3a20 2d31  ctor2={'min': -1
-00006a50: 3030 3030 3030 2c20 276d 6178 273a 2031  000000, 'max': 1
-00006a60: 3030 3030 3030 7d29 0d0a 406a 7570 7974  000000})..@jupyt
-00006a70: 6572 5f64 6973 706c 6179 6162 6c65 5f6f  er_displayable_o
-00006a80: 7574 7075 7428 6c69 6272 6172 795f 6e61  utput(library_na
-00006a90: 6d65 3d27 6e73 6261 7477 6d27 2c20 6865  me='nsbatwm', he
-00006aa0: 6c70 5f75 726c 3d27 6874 7470 733a 2f2f  lp_url='https://
-00006ab0: 7777 772e 6e61 7061 7269 2d68 7562 2e6f  www.napari-hub.o
-00006ac0: 7267 2f70 6c75 6769 6e73 2f6e 6170 6172  rg/plugins/napar
-00006ad0: 692d 7365 676d 656e 742d 626c 6f62 732d  i-segment-blobs-
-00006ae0: 616e 642d 7468 696e 6773 2d77 6974 682d  and-things-with-
-00006af0: 6d65 6d62 7261 6e65 7327 290d 0a40 7469  membranes')..@ti
-00006b00: 6d65 5f73 6c69 6365 720d 0a64 6566 2073  me_slicer..def s
-00006b10: 756d 5f69 6d61 6765 7328 696d 6167 6531  um_images(image1
-00006b20: 3a20 226e 6170 6172 692e 7479 7065 732e  : "napari.types.
-00006b30: 496d 6167 6544 6174 6122 2c20 696d 6167  ImageData", imag
-00006b40: 6532 3a20 226e 6170 6172 692e 7479 7065  e2: "napari.type
-00006b50: 732e 496d 6167 6544 6174 6122 2c20 6661  s.ImageData", fa
-00006b60: 6374 6f72 313a 2066 6c6f 6174 203d 2031  ctor1: float = 1
-00006b70: 2c20 6661 6374 6f72 323a 2066 6c6f 6174  , factor2: float
-00006b80: 203d 2031 2920 2d3e 2022 6e61 7061 7269   = 1) -> "napari
-00006b90: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
-00006ba0: 223a 0d0a 2020 2020 2222 2241 6464 2074  ":..    """Add t
-00006bb0: 776f 2069 6d61 6765 7322 2222 0d0a 2020  wo images"""..  
-00006bc0: 2020 7265 7475 726e 2069 6d61 6765 3120    return image1 
-00006bd0: 2a20 6661 6374 6f72 3120 2b20 696d 6167  * factor1 + imag
-00006be0: 6532 202a 2066 6163 746f 7232 0d0a 0d0a  e2 * factor2....
-00006bf0: 0d0a 4072 6567 6973 7465 725f 6675 6e63  ..@register_func
-00006c00: 7469 6f6e 286d 656e 753d 2249 6d61 6765  tion(menu="Image
-00006c10: 206d 6174 6820 3e20 4d75 6c74 6970 6c79   math > Multiply
-00006c20: 2069 6d61 6765 7320 286e 756d 7079 2c20   images (numpy, 
-00006c30: 6e73 6261 7477 6d29 2229 0d0a 406a 7570  nsbatwm)")..@jup
-00006c40: 7974 6572 5f64 6973 706c 6179 6162 6c65  yter_displayable
-00006c50: 5f6f 7574 7075 7428 6c69 6272 6172 795f  _output(library_
-00006c60: 6e61 6d65 3d27 6e73 6261 7477 6d27 2c20  name='nsbatwm', 
-00006c70: 6865 6c70 5f75 726c 3d27 6874 7470 733a  help_url='https:
-00006c80: 2f2f 7777 772e 6e61 7061 7269 2d68 7562  //www.napari-hub
-00006c90: 2e6f 7267 2f70 6c75 6769 6e73 2f6e 6170  .org/plugins/nap
-00006ca0: 6172 692d 7365 676d 656e 742d 626c 6f62  ari-segment-blob
-00006cb0: 732d 616e 642d 7468 696e 6773 2d77 6974  s-and-things-wit
-00006cc0: 682d 6d65 6d62 7261 6e65 7327 290d 0a40  h-membranes')..@
-00006cd0: 7469 6d65 5f73 6c69 6365 720d 0a64 6566  time_slicer..def
-00006ce0: 206d 756c 7469 706c 795f 696d 6167 6573   multiply_images
-00006cf0: 2869 6d61 6765 313a 2022 6e61 7061 7269  (image1: "napari
-00006d00: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
-00006d10: 222c 2069 6d61 6765 323a 2022 6e61 7061  ", image2: "napa
-00006d20: 7269 2e74 7970 6573 2e49 6d61 6765 4461  ri.types.ImageDa
-00006d30: 7461 2229 202d 3e20 226e 6170 6172 692e  ta") -> "napari.
-00006d40: 7479 7065 732e 496d 6167 6544 6174 6122  types.ImageData"
-00006d50: 3a0d 0a20 2020 2022 2222 4d75 6c74 6970  :..    """Multip
-00006d60: 6c79 2074 776f 2069 6d61 6765 7322 2222  ly two images"""
-00006d70: 0d0a 2020 2020 7265 7475 726e 2069 6d61  ..    return ima
-00006d80: 6765 3120 2a20 696d 6167 6532 0d0a 0d0a  ge1 * image2....
-00006d90: 0d0a 4072 6567 6973 7465 725f 6675 6e63  ..@register_func
-00006da0: 7469 6f6e 286d 656e 753d 2249 6d61 6765  tion(menu="Image
-00006db0: 206d 6174 6820 3e20 4469 7669 6465 2069   math > Divide i
-00006dc0: 6d61 6765 7320 286e 756d 7079 2c20 6e73  mages (numpy, ns
-00006dd0: 6261 7477 6d29 2229 0d0a 406a 7570 7974  batwm)")..@jupyt
-00006de0: 6572 5f64 6973 706c 6179 6162 6c65 5f6f  er_displayable_o
-00006df0: 7574 7075 7428 6c69 6272 6172 795f 6e61  utput(library_na
-00006e00: 6d65 3d27 6e73 6261 7477 6d27 2c20 6865  me='nsbatwm', he
-00006e10: 6c70 5f75 726c 3d27 6874 7470 733a 2f2f  lp_url='https://
-00006e20: 7777 772e 6e61 7061 7269 2d68 7562 2e6f  www.napari-hub.o
-00006e30: 7267 2f70 6c75 6769 6e73 2f6e 6170 6172  rg/plugins/napar
-00006e40: 692d 7365 676d 656e 742d 626c 6f62 732d  i-segment-blobs-
-00006e50: 616e 642d 7468 696e 6773 2d77 6974 682d  and-things-with-
-00006e60: 6d65 6d62 7261 6e65 7327 290d 0a40 7469  membranes')..@ti
-00006e70: 6d65 5f73 6c69 6365 720d 0a64 6566 2064  me_slicer..def d
-00006e80: 6976 6964 655f 696d 6167 6573 2869 6d61  ivide_images(ima
-00006e90: 6765 313a 2022 6e61 7061 7269 2e74 7970  ge1: "napari.typ
-00006ea0: 6573 2e49 6d61 6765 4461 7461 222c 2069  es.ImageData", i
-00006eb0: 6d61 6765 323a 2022 6e61 7061 7269 2e74  mage2: "napari.t
-00006ec0: 7970 6573 2e49 6d61 6765 4461 7461 2229  ypes.ImageData")
-00006ed0: 202d 3e20 226e 6170 6172 692e 7479 7065   -> "napari.type
-00006ee0: 732e 496d 6167 6544 6174 6122 3a0d 0a20  s.ImageData":.. 
-00006ef0: 2020 2022 2222 4469 7669 6465 206f 6e65     """Divide one
-00006f00: 2069 6d61 6765 2062 7920 616e 6f74 6865   image by anothe
-00006f10: 7222 2222 0d0a 2020 2020 7265 7475 726e  r"""..    return
-00006f20: 2069 6d61 6765 3120 2f20 696d 6167 6532   image1 / image2
-00006f30: 0d0a 0d0a 0d0a 4072 6567 6973 7465 725f  ......@register_
-00006f40: 6675 6e63 7469 6f6e 286d 656e 753d 2249  function(menu="I
-00006f50: 6d61 6765 206d 6174 6820 3e20 496e 7665  mage math > Inve
-00006f60: 7274 2069 6d61 6765 2028 7363 696b 6974  rt image (scikit
-00006f70: 2d69 6d61 6765 2c20 6e73 6261 7477 6d29  -image, nsbatwm)
-00006f80: 2229 0d0a 406a 7570 7974 6572 5f64 6973  ")..@jupyter_dis
-00006f90: 706c 6179 6162 6c65 5f6f 7574 7075 7428  playable_output(
-00006fa0: 6c69 6272 6172 795f 6e61 6d65 3d27 6e73  library_name='ns
-00006fb0: 6261 7477 6d27 2c20 6865 6c70 5f75 726c  batwm', help_url
-00006fc0: 3d27 6874 7470 733a 2f2f 7777 772e 6e61  ='https://www.na
-00006fd0: 7061 7269 2d68 7562 2e6f 7267 2f70 6c75  pari-hub.org/plu
-00006fe0: 6769 6e73 2f6e 6170 6172 692d 7365 676d  gins/napari-segm
-00006ff0: 656e 742d 626c 6f62 732d 616e 642d 7468  ent-blobs-and-th
-00007000: 696e 6773 2d77 6974 682d 6d65 6d62 7261  ings-with-membra
-00007010: 6e65 7327 290d 0a40 7469 6d65 5f73 6c69  nes')..@time_sli
-00007020: 6365 720d 0a64 6566 2069 6e76 6572 745f  cer..def invert_
-00007030: 696d 6167 6528 696d 6167 653a 2022 6e61  image(image: "na
-00007040: 7061 7269 2e74 7970 6573 2e49 6d61 6765  pari.types.Image
-00007050: 4461 7461 2229 202d 3e20 226e 6170 6172  Data") -> "napar
-00007060: 692e 7479 7065 732e 496d 6167 6544 6174  i.types.ImageDat
-00007070: 6122 3a0d 0a20 2020 2022 2222 496e 7665  a":..    """Inve
-00007080: 7274 2061 6e20 696d 6167 652e 2054 6865  rt an image. The
-00007090: 2065 7861 6374 206d 6174 6820 6265 6869   exact math behi
-000070a0: 6e64 2064 6570 656e 6473 206f 6e20 7468  nd depends on th
-000070b0: 6520 696d 6167 6520 7479 7065 2e0d 0a0d  e image type....
-000070c0: 0a20 2020 2053 6565 2061 6c73 6f0d 0a20  .    See also.. 
-000070d0: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
-000070e0: 202e 2e20 5b30 5d20 6874 7470 733a 2f2f   .. [0] https://
-000070f0: 7363 696b 6974 2d69 6d61 6765 2e6f 7267  scikit-image.org
-00007100: 2f64 6f63 732f 6465 762f 6170 692f 736b  /docs/dev/api/sk
-00007110: 696d 6167 652e 7574 696c 2e68 746d 6c3f  image.util.html?
-00007120: 6869 6768 6c69 6768 743d 696e 7665 7274  highlight=invert
-00007130: 2373 6b69 6d61 6765 2e75 7469 6c2e 696e  #skimage.util.in
-00007140: 7665 7274 0d0a 2020 2020 2222 220d 0a20  vert..    """.. 
-00007150: 2020 2066 726f 6d20 736b 696d 6167 6520     from skimage 
-00007160: 696d 706f 7274 2075 7469 6c0d 0a20 2020  import util..   
-00007170: 2072 6574 7572 6e20 7574 696c 2e69 6e76   return util.inv
-00007180: 6572 7428 696d 6167 6529 0d0a 0d0a 0d0a  ert(image)......
-00007190: 4072 6567 6973 7465 725f 6675 6e63 7469  @register_functi
-000071a0: 6f6e 286d 656e 753d 2253 6567 6d65 6e74  on(menu="Segment
-000071b0: 6174 696f 6e20 706f 7374 2d70 726f 6365  ation post-proce
-000071c0: 7373 696e 6720 3e20 536b 656c 6574 6f6e  ssing > Skeleton
-000071d0: 697a 6520 2873 6369 6b69 742d 696d 6167  ize (scikit-imag
-000071e0: 652c 206e 7362 6174 776d 2922 290d 0a40  e, nsbatwm)")..@
-000071f0: 6a75 7079 7465 725f 6469 7370 6c61 7961  jupyter_displaya
-00007200: 626c 655f 6f75 7470 7574 286c 6962 7261  ble_output(libra
-00007210: 7279 5f6e 616d 653d 276e 7362 6174 776d  ry_name='nsbatwm
-00007220: 272c 2068 656c 705f 7572 6c3d 2768 7474  ', help_url='htt
-00007230: 7073 3a2f 2f77 7777 2e6e 6170 6172 692d  ps://www.napari-
-00007240: 6875 622e 6f72 672f 706c 7567 696e 732f  hub.org/plugins/
-00007250: 6e61 7061 7269 2d73 6567 6d65 6e74 2d62  napari-segment-b
-00007260: 6c6f 6273 2d61 6e64 2d74 6869 6e67 732d  lobs-and-things-
-00007270: 7769 7468 2d6d 656d 6272 616e 6573 2729  with-membranes')
-00007280: 0d0a 4074 696d 655f 736c 6963 6572 0d0a  ..@time_slicer..
-00007290: 6465 6620 736b 656c 6574 6f6e 697a 6528  def skeletonize(
-000072a0: 696d 6167 653a 2022 6e61 7061 7269 2e74  image: "napari.t
-000072b0: 7970 6573 2e4c 6162 656c 7344 6174 6122  ypes.LabelsData"
-000072c0: 2920 2d3e 2022 6e61 7061 7269 2e74 7970  ) -> "napari.typ
-000072d0: 6573 2e4c 6162 656c 7344 6174 6122 3a0d  es.LabelsData":.
-000072e0: 0a20 2020 2022 2222 0d0a 2020 2020 536b  .    """..    Sk
-000072f0: 656c 6574 6f6e 697a 6520 6c61 6265 6c65  eletonize labele
-00007300: 6420 6f62 6a65 6374 7320 696e 2061 6e20  d objects in an 
-00007310: 696d 6167 652e 2054 6869 7320 6361 6e20  image. This can 
-00007320: 6265 2075 7365 6675 6c20 746f 2072 6564  be useful to red
-00007330: 7563 6520 6f62 6a65 6374 7320 7375 6368  uce objects such
-00007340: 2061 7320 6e65 7572 6f6e 732c 2072 6f6f   as neurons, roo
-00007350: 7473 2061 6e64 2076 6573 7365 6c73 0d0a  ts and vessels..
-00007360: 2020 2020 7769 7468 2076 6172 6961 626c      with variabl
-00007370: 6520 7468 6963 6b6e 6573 7320 746f 2073  e thickness to s
-00007380: 696e 676c 6520 7069 7865 6c20 6c69 6e65  ingle pixel line
-00007390: 7320 666f 7220 6675 7274 6865 7220 616e  s for further an
-000073a0: 616c 7973 6973 2e0d 0a0d 0a20 2020 2053  alysis.....    S
-000073b0: 6565 2061 6c73 6f0d 0a20 2020 202d 2d2d  ee also..    ---
-000073c0: 2d2d 2d2d 2d0d 0a20 2020 202e 2e20 5b30  -----..    .. [0
-000073d0: 5d20 6874 7470 733a 2f2f 656e 2e77 696b  ] https://en.wik
-000073e0: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-000073f0: 546f 706f 6c6f 6769 6361 6c5f 736b 656c  Topological_skel
-00007400: 6574 6f6e 0d0a 2020 2020 2222 220d 0a20  eton..    """.. 
-00007410: 2020 2066 726f 6d20 736b 696d 6167 6520     from skimage 
-00007420: 696d 706f 7274 206d 6f72 7068 6f6c 6f67  import morpholog
-00007430: 790d 0a20 2020 2069 6620 696d 6167 652e  y..    if image.
-00007440: 6d61 7828 2920 3d3d 2031 3a0d 0a20 2020  max() == 1:..   
-00007450: 2020 2020 2072 6574 7572 6e20 6d6f 7270       return morp
-00007460: 686f 6c6f 6779 2e73 6b65 6c65 746f 6e69  hology.skeletoni
-00007470: 7a65 2869 6d61 6765 290d 0a20 2020 2065  ze(image)..    e
-00007480: 6c73 653a 0d0a 2020 2020 2020 2020 7265  lse:..        re
-00007490: 7375 6c74 203d 206e 702e 7a65 726f 7328  sult = np.zeros(
-000074a0: 696d 6167 652e 7368 6170 6529 0d0a 2020  image.shape)..  
-000074b0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-000074c0: 616e 6765 2831 2c20 696d 6167 652e 6d61  ange(1, image.ma
-000074d0: 7828 2920 2b20 3129 3a0d 0a20 2020 2020  x() + 1):..     
-000074e0: 2020 2020 2020 2073 6b65 6c65 746f 6e20         skeleton 
-000074f0: 3d20 6d6f 7270 686f 6c6f 6779 2e73 6b65  = morphology.ske
-00007500: 6c65 746f 6e69 7a65 2869 6d61 6765 203d  letonize(image =
-00007510: 3d20 6929 0d0a 2020 2020 2020 2020 2020  = i)..          
-00007520: 2020 7265 7375 6c74 203d 2073 6b65 6c65    result = skele
-00007530: 746f 6e20 2a20 6920 2b20 7265 7375 6c74  ton * i + result
-00007540: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00007550: 2072 6573 756c 742e 6173 7479 7065 2869   result.astype(i
-00007560: 6e74 290d 0a0d 0a0d 0a40 7265 6769 7374  nt)......@regist
-00007570: 6572 5f66 756e 6374 696f 6e28 6d65 6e75  er_function(menu
-00007580: 3d22 5472 616e 7366 6f72 6d73 203e 2052  ="Transforms > R
-00007590: 6573 6361 6c65 2028 7363 696b 6974 2d69  escale (scikit-i
-000075a0: 6d61 6765 2c20 6e73 6261 7477 6d29 2229  mage, nsbatwm)")
-000075b0: 0d0a 4074 696d 655f 736c 6963 6572 0d0a  ..@time_slicer..
-000075c0: 6465 6620 7265 7363 616c 6528 696d 6167  def rescale(imag
-000075d0: 653a 2022 6e61 7061 7269 2e74 7970 6573  e: "napari.types
-000075e0: 2e49 6d61 6765 4461 7461 222c 0d0a 2020  .ImageData",..  
-000075f0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-00007600: 783a 2066 6c6f 6174 203d 2031 2e30 2c0d  x: float = 1.0,.
-00007610: 0a20 2020 2020 2020 2020 2020 2073 6361  .            sca
-00007620: 6c65 5f79 3a20 666c 6f61 7420 3d20 312e  le_y: float = 1.
-00007630: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00007640: 7363 616c 655f 7a3a 2066 6c6f 6174 203d  scale_z: float =
-00007650: 2031 2e30 2920 2d3e 2022 6e61 7061 7269   1.0) -> "napari
-00007660: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
-00007670: 223a 0d0a 2020 2020 2222 220d 0a20 2020  ":..    """..   
-00007680: 2052 6573 6361 6c65 2061 6e20 696d 6167   Rescale an imag
-00007690: 6520 6279 2061 2067 6976 656e 2073 6574  e by a given set
-000076a0: 206f 6620 7363 616c 6520 6661 6374 6f72   of scale factor
-000076b0: 732e 0d0a 0d0a 2020 2020 5061 7261 6d65  s.....    Parame
-000076c0: 7465 7273 0d0a 2020 2020 2d2d 2d2d 2d2d  ters..    ------
-000076d0: 2d2d 2d2d 0d0a 2020 2020 696d 6167 6520  ----..    image 
-000076e0: 3a20 496d 6167 6544 6174 610d 0a20 2020  : ImageData..   
-000076f0: 2073 6361 6c65 5f78 203a 2066 6c6f 6174   scale_x : float
-00007700: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00007710: 2020 2020 6661 6374 6f72 2062 7920 7768      factor by wh
-00007720: 6963 6820 746f 2073 6361 6c65 2074 6865  ich to scale the
-00007730: 2069 6d61 6765 2061 6c6f 6e67 2074 6865   image along the
-00007740: 2078 2061 7869 732e 2054 6865 2064 6566   x axis. The def
-00007750: 6175 6c74 2069 7320 312e 302e 0d0a 2020  ault is 1.0...  
-00007760: 2020 7363 616c 655f 7920 3a20 666c 6f61    scale_y : floa
-00007770: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-00007780: 2020 2020 2066 6163 746f 7220 6279 2077       factor by w
-00007790: 6869 6368 2074 6f20 7363 616c 6520 7468  hich to scale th
-000077a0: 6520 696d 6167 6520 616c 6f6e 6720 7468  e image along th
-000077b0: 6520 7920 6469 6d65 6e73 696f 6e2e 2054  e y dimension. T
-000077c0: 6865 2064 6566 6175 6c74 2069 7320 312e  he default is 1.
-000077d0: 302e 0d0a 2020 2020 7363 616c 655f 7a20  0...    scale_z 
-000077e0: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
-000077f0: 6c0d 0a20 2020 2020 2020 2066 6163 746f  l..        facto
-00007800: 7220 6279 2077 6869 6368 2074 6f20 7363  r by which to sc
-00007810: 616c 6520 7468 6520 696d 6167 6520 616c  ale the image al
-00007820: 6f6e 6720 7468 6520 7a20 6469 6d65 6e73  ong the z dimens
-00007830: 696f 6e2e 2054 6865 2064 6566 6175 6c74  ion. The default
-00007840: 2069 7320 312e 302e 0d0a 0d0a 2020 2020   is 1.0.....    
-00007850: 5265 7475 726e 730d 0a20 2020 202d 2d2d  Returns..    ---
-00007860: 2d2d 2d2d 0d0a 2020 2020 496d 6167 6544  ----..    ImageD
-00007870: 6174 610d 0a0d 0a20 2020 2053 6565 2041  ata....    See A
-00007880: 6c73 6f0d 0a20 2020 202d 2d2d 2d2d 2d2d  lso..    -------
-00007890: 2d0d 0a20 2020 2068 7474 7073 3a2f 2f73  -..    https://s
-000078a0: 6369 6b69 742d 696d 6167 652e 6f72 672f  cikit-image.org/
-000078b0: 646f 6373 2f73 7461 626c 652f 6170 692f  docs/stable/api/
-000078c0: 736b 696d 6167 652e 7472 616e 7366 6f72  skimage.transfor
-000078d0: 6d2e 6874 6d6c 2372 6573 6361 6c65 0d0a  m.html#rescale..
-000078e0: 2020 2020 2222 220d 0a20 2020 2066 726f      """..    fro
-000078f0: 6d20 736b 696d 6167 6520 696d 706f 7274  m skimage import
-00007900: 2074 7261 6e73 666f 726d 0d0a 0d0a 2020   transform....  
-00007910: 2020 6966 206c 656e 2869 6d61 6765 2e73    if len(image.s
-00007920: 6861 7065 2920 3d3d 2033 3a0d 0a20 2020  hape) == 3:..   
-00007930: 2020 2020 2073 6361 6c65 5f66 6163 746f       scale_facto
-00007940: 7273 203d 206e 702e 6173 6172 7261 7928  rs = np.asarray(
-00007950: 5b73 6361 6c65 5f7a 2c20 7363 616c 655f  [scale_z, scale_
-00007960: 792c 2073 6361 6c65 5f78 5d29 0d0a 2020  y, scale_x])..  
-00007970: 2020 656c 6966 206c 656e 2869 6d61 6765    elif len(image
-00007980: 2e73 6861 7065 2920 3d3d 2032 3a0d 0a20  .shape) == 2:.. 
-00007990: 2020 2020 2020 2073 6361 6c65 5f66 6163         scale_fac
-000079a0: 746f 7273 203d 206e 702e 6173 6172 7261  tors = np.asarra
-000079b0: 7928 5b73 6361 6c65 5f79 2c20 7363 616c  y([scale_y, scal
-000079c0: 655f 785d 290d 0a20 2020 2065 6c73 653a  e_x])..    else:
-000079d0: 0d0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
-000079e0: 5661 6c75 6545 7272 6f72 2822 5265 7363  ValueError("Resc
-000079f0: 616c 696e 6720 6f6e 6c79 2073 7570 706f  aling only suppo
-00007a00: 7274 6564 2066 6f72 2032 4420 616e 6420  rted for 2D and 
-00007a10: 3344 2069 6d61 6765 7322 290d 0a0d 0a20  3D images").... 
-00007a20: 2020 2072 6574 7572 6e20 7472 616e 7366     return transf
-00007a30: 6f72 6d2e 7265 7363 616c 6528 696d 6167  orm.rescale(imag
-00007a40: 652c 2073 6361 6c65 3d73 6361 6c65 5f66  e, scale=scale_f
-00007a50: 6163 746f 7273 2c20 7072 6573 6572 7665  actors, preserve
-00007a60: 5f72 616e 6765 3d54 7275 6529 0d0a 0d0a  _range=True)....
-00007a70: 0d0a 4072 6567 6973 7465 725f 6675 6e63  ..@register_func
-00007a80: 7469 6f6e 286d 656e 753d 2254 7261 6e73  tion(menu="Trans
-00007a90: 666f 726d 7320 3e20 5265 7369 7a65 2028  forms > Resize (
-00007aa0: 7363 696b 6974 2d69 6d61 6765 2c20 6e73  scikit-image, ns
-00007ab0: 6261 7477 6d29 2229 0d0a 4074 696d 655f  batwm)")..@time_
-00007ac0: 736c 6963 6572 0d0a 6465 6620 7265 7369  slicer..def resi
-00007ad0: 7a65 2869 6d61 6765 3a20 226e 6170 6172  ze(image: "napar
-00007ae0: 692e 7479 7065 732e 496d 6167 6544 6174  i.types.ImageDat
-00007af0: 6122 2c0d 0a20 2020 2020 2020 2020 2020  a",..           
-00007b00: 206e 6577 5f77 6964 7468 3a20 696e 7420   new_width: int 
-00007b10: 3d20 3130 2e30 2c0d 0a20 2020 2020 2020  = 10.0,..       
-00007b20: 2020 2020 206e 6577 5f68 6569 6768 743a       new_height:
-00007b30: 2069 6e74 203d 2031 302e 302c 0d0a 2020   int = 10.0,..  
-00007b40: 2020 2020 2020 2020 2020 6e65 775f 6465            new_de
-00007b50: 7074 683a 2069 6e74 203d 2031 302e 3029  pth: int = 10.0)
-00007b60: 202d 3e20 226e 6170 6172 692e 7479 7065   -> "napari.type
-00007b70: 732e 496d 6167 6544 6174 6122 3a0d 0a20  s.ImageData":.. 
-00007b80: 2020 2022 2222 0d0a 2020 2020 5265 7363     """..    Resc
-00007b90: 616c 6520 616e 2069 6d61 6765 2074 6f20  ale an image to 
-00007ba0: 6669 7420 696e 2061 2067 6976 656e 206e  fit in a given n
-00007bb0: 6577 2073 697a 652e 0d0a 0d0a 2020 2020  ew size.....    
-00007bc0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-00007bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
-00007be0: 696d 6167 6520 3a20 496d 6167 6544 6174  image : ImageDat
-00007bf0: 610d 0a20 2020 206e 6577 5f77 6964 7468  a..    new_width
-00007c00: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
-00007c10: 0d0a 2020 2020 2020 2020 6661 6374 6f72  ..        factor
-00007c20: 2062 7920 7768 6963 6820 746f 2073 6361   by which to sca
-00007c30: 6c65 2074 6865 2069 6d61 6765 2061 6c6f  le the image alo
-00007c40: 6e67 2074 6865 2078 2061 7869 732e 2054  ng the x axis. T
-00007c50: 6865 2064 6566 6175 6c74 2069 7320 312e  he default is 1.
-00007c60: 302e 0d0a 2020 2020 6e65 775f 6865 6967  0...    new_heig
-00007c70: 6874 203a 2069 6e74 2c20 6f70 7469 6f6e  ht : int, option
-00007c80: 616c 0d0a 2020 2020 2020 2020 6661 6374  al..        fact
-00007c90: 6f72 2062 7920 7768 6963 6820 746f 2073  or by which to s
-00007ca0: 6361 6c65 2074 6865 2069 6d61 6765 2061  cale the image a
-00007cb0: 6c6f 6e67 2074 6865 2079 2064 696d 656e  long the y dimen
-00007cc0: 7369 6f6e 2e20 5468 6520 6465 6661 756c  sion. The defaul
-00007cd0: 7420 6973 2031 2e30 2e0d 0a20 2020 206e  t is 1.0...    n
-00007ce0: 6577 5f64 6570 7468 203a 2069 6e74 2c20  ew_depth : int, 
-00007cf0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00007d00: 2020 6661 6374 6f72 2062 7920 7768 6963    factor by whic
-00007d10: 6820 746f 2073 6361 6c65 2074 6865 2069  h to scale the i
-00007d20: 6d61 6765 2061 6c6f 6e67 2074 6865 207a  mage along the z
-00007d30: 2064 696d 656e 7369 6f6e 2e20 5468 6520   dimension. The 
-00007d40: 6465 6661 756c 7420 6973 2031 2e30 2e0d  default is 1.0..
-00007d50: 0a0d 0a20 2020 2052 6574 7572 6e73 0d0a  ...    Returns..
-00007d60: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-00007d70: 2049 6d61 6765 4461 7461 0d0a 0d0a 2020   ImageData....  
-00007d80: 2020 5365 6520 416c 736f 0d0a 2020 2020    See Also..    
-00007d90: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 6874  --------..    ht
-00007da0: 7470 733a 2f2f 7363 696b 6974 2d69 6d61  tps://scikit-ima
-00007db0: 6765 2e6f 7267 2f64 6f63 732f 7374 6162  ge.org/docs/stab
-00007dc0: 6c65 2f61 7069 2f73 6b69 6d61 6765 2e74  le/api/skimage.t
-00007dd0: 7261 6e73 666f 726d 2e68 746d 6c23 7265  ransform.html#re
-00007de0: 7369 7a65 0d0a 2020 2020 2222 220d 0a20  size..    """.. 
-00007df0: 2020 2066 726f 6d20 736b 696d 6167 6520     from skimage 
-00007e00: 696d 706f 7274 2074 7261 6e73 666f 726d  import transform
-00007e10: 0d0a 0d0a 2020 2020 6966 206c 656e 2869  ....    if len(i
-00007e20: 6d61 6765 2e73 6861 7065 2920 3d3d 2033  mage.shape) == 3
-00007e30: 3a0d 0a20 2020 2020 2020 206f 7574 7075  :..        outpu
-00007e40: 745f 7368 6170 6520 3d20 6e70 2e61 7361  t_shape = np.asa
-00007e50: 7272 6179 285b 6e65 775f 6465 7074 682c  rray([new_depth,
-00007e60: 206e 6577 5f68 6569 6768 742c 206e 6577   new_height, new
-00007e70: 5f77 6964 7468 5d29 0d0a 2020 2020 656c  _width])..    el
-00007e80: 6966 206c 656e 2869 6d61 6765 2e73 6861  if len(image.sha
-00007e90: 7065 2920 3d3d 2032 3a0d 0a20 2020 2020  pe) == 2:..     
-00007ea0: 2020 206f 7574 7075 745f 7368 6170 6520     output_shape 
-00007eb0: 3d20 6e70 2e61 7361 7272 6179 285b 6e65  = np.asarray([ne
-00007ec0: 775f 6865 6967 6874 2c20 6e65 775f 7769  w_height, new_wi
-00007ed0: 6474 685d 290d 0a20 2020 2065 6c73 653a  dth])..    else:
-00007ee0: 0d0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
-00007ef0: 5661 6c75 6545 7272 6f72 2822 5265 7369  ValueError("Resi
-00007f00: 7a69 6e67 206f 6e6c 7920 7375 7070 6f72  zing only suppor
-00007f10: 7465 6420 666f 7220 3244 2061 6e64 2033  ted for 2D and 3
-00007f20: 4420 696d 6167 6573 2229 0d0a 0d0a 2020  D images")....  
-00007f30: 2020 7265 7475 726e 2074 7261 6e73 666f    return transfo
-00007f40: 726d 2e72 6573 697a 6528 696d 6167 652c  rm.resize(image,
-00007f50: 206f 7574 7075 745f 7368 6170 652c 2070   output_shape, p
-00007f60: 7265 7365 7276 655f 7261 6e67 653d 5472  reserve_range=Tr
-00007f70: 7565 290d 0a0d 0a0d 0a40 7265 6769 7374  ue)......@regist
-00007f80: 6572 5f66 756e 6374 696f 6e28 6d65 6e75  er_function(menu
-00007f90: 3d22 5574 696c 6974 6965 7320 3e20 4d61  ="Utilities > Ma
-00007fa0: 6e75 616c 6c79 206d 6572 6765 206c 6162  nually merge lab
-00007fb0: 656c 7320 286e 7362 6174 776d 2922 290d  els (nsbatwm)").
-00007fc0: 0a64 6566 204d 616e 7561 6c6c 795f 6d65  .def Manually_me
-00007fd0: 7267 655f 6c61 6265 6c73 286c 6162 656c  rge_labels(label
-00007fe0: 735f 6c61 7965 723a 2022 6e61 7061 7269  s_layer: "napari
-00007ff0: 2e6c 6179 6572 732e 4c61 6265 6c73 222c  .layers.Labels",
-00008000: 2070 6f69 6e74 735f 6c61 7965 723a 2022   points_layer: "
-00008010: 6e61 7061 7269 2e6c 6179 6572 732e 506f  napari.layers.Po
-00008020: 696e 7473 222c 2076 6965 7765 7220 3a20  ints", viewer : 
-00008030: 226e 6170 6172 692e 5669 6577 6572 2229  "napari.Viewer")
-00008040: 3a0d 0a20 2020 2069 6620 706f 696e 7473  :..    if points
-00008050: 5f6c 6179 6572 2069 7320 4e6f 6e65 3a0d  _layer is None:.
-00008060: 0a20 2020 2020 2020 2070 6f69 6e74 735f  .        points_
-00008070: 6c61 7965 7220 3d20 7669 6577 6572 2e61  layer = viewer.a
-00008080: 6464 5f70 6f69 6e74 7328 5b5d 290d 0a20  dd_points([]).. 
-00008090: 2020 2020 2020 2070 6f69 6e74 735f 6c61         points_la
-000080a0: 7965 722e 6d6f 6465 203d 2027 4144 4427  yer.mode = 'ADD'
-000080b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000080c0: 0d0a 2020 2020 6c61 6265 6c73 203d 206e  ..    labels = n
-000080d0: 702e 6173 6172 7261 7928 6c61 6265 6c73  p.asarray(labels
-000080e0: 5f6c 6179 6572 2e64 6174 6129 0d0a 2020  _layer.data)..  
-000080f0: 2020 706f 696e 7473 203d 2070 6f69 6e74    points = point
-00008100: 735f 6c61 7965 722e 6461 7461 0d0a 0d0a  s_layer.data....
-00008110: 2020 2020 6c61 6265 6c5f 6964 7320 3d20      label_ids = 
-00008120: 5b6c 6162 656c 732e 6974 656d 2874 7570  [labels.item(tup
-00008130: 6c65 285b 696e 7428 6a29 2066 6f72 206a  le([int(j) for j
-00008140: 2069 6e20 695d 2929 2066 6f72 2069 2069   in i])) for i i
-00008150: 6e20 706f 696e 7473 5d0d 0a0d 0a20 2020  n points]....   
-00008160: 2023 2072 6570 6c61 6365 206c 6162 656c   # replace label
-00008170: 7320 7769 7468 206d 696e 696d 756d 206f  s with minimum o
-00008180: 6620 7468 6520 7365 6c65 6374 6564 206c  f the selected l
-00008190: 6162 656c 730d 0a20 2020 206e 6577 5f6c  abels..    new_l
-000081a0: 6162 656c 5f69 6420 3d20 6d69 6e28 6c61  abel_id = min(la
-000081b0: 6265 6c5f 6964 7329 0d0a 2020 2020 666f  bel_ids)..    fo
-000081c0: 7220 6c20 696e 206c 6162 656c 5f69 6473  r l in label_ids
-000081d0: 3a0d 0a20 2020 2020 2020 2069 6620 6c20  :..        if l 
-000081e0: 213d 206e 6577 5f6c 6162 656c 5f69 643a  != new_label_id:
-000081f0: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-00008200: 6265 6c73 5b6c 6162 656c 7320 3d3d 206c  bels[labels == l
-00008210: 5d20 3d20 6e65 775f 6c61 6265 6c5f 6964  ] = new_label_id
-00008220: 0d0a 0d0a 2020 2020 6c61 6265 6c73 5f6c  ....    labels_l
-00008230: 6179 6572 2e64 6174 6120 3d20 6c61 6265  ayer.data = labe
-00008240: 6c73 0d0a 2020 2020 706f 696e 7473 5f6c  ls..    points_l
-00008250: 6179 6572 2e64 6174 6120 3d20 5b5d 0d0a  ayer.data = []..
-00008260: 0d0a 4072 6567 6973 7465 725f 6675 6e63  ..@register_func
-00008270: 7469 6f6e 286d 656e 753d 2255 7469 6c69  tion(menu="Utili
-00008280: 7469 6573 203e 204d 616e 7561 6c6c 7920  ties > Manually 
-00008290: 7370 6c69 7420 6c61 6265 6c73 2028 6e73  split labels (ns
-000082a0: 6261 7477 6d29 2229 0d0a 6465 6620 4d61  batwm)")..def Ma
-000082b0: 6e75 616c 6c79 5f73 706c 6974 5f6c 6162  nually_split_lab
-000082c0: 656c 7328 6c61 6265 6c73 5f6c 6179 6572  els(labels_layer
-000082d0: 3a20 226e 6170 6172 692e 6c61 7965 7273  : "napari.layers
-000082e0: 2e4c 6162 656c 7322 2c20 706f 696e 7473  .Labels", points
-000082f0: 5f6c 6179 6572 3a20 226e 6170 6172 692e  _layer: "napari.
-00008300: 6c61 7965 7273 2e50 6f69 6e74 7322 2c20  layers.Points", 
-00008310: 7669 6577 6572 3a20 226e 6170 6172 692e  viewer: "napari.
-00008320: 5669 6577 6572 2229 3a0d 0a20 2020 2069  Viewer"):..    i
-00008330: 6620 706f 696e 7473 5f6c 6179 6572 2069  f points_layer i
-00008340: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00008350: 2070 6f69 6e74 735f 6c61 7965 7220 3d20   points_layer = 
-00008360: 7669 6577 6572 2e61 6464 5f70 6f69 6e74  viewer.add_point
-00008370: 7328 5b5d 290d 0a20 2020 2020 2020 2070  s([])..        p
-00008380: 6f69 6e74 735f 6c61 7965 722e 6d6f 6465  oints_layer.mode
-00008390: 203d 2027 4144 4427 0d0a 2020 2020 2020   = 'ADD'..      
-000083a0: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-000083b0: 6c61 6265 6c73 203d 206e 702e 6173 6172  labels = np.asar
-000083c0: 7261 7928 6c61 6265 6c73 5f6c 6179 6572  ray(labels_layer
-000083d0: 2e64 6174 6129 0d0a 2020 2020 706f 696e  .data)..    poin
-000083e0: 7473 203d 2070 6f69 6e74 735f 6c61 7965  ts = points_laye
-000083f0: 722e 6461 7461 0d0a 0d0a 2020 2020 6c61  r.data....    la
-00008400: 6265 6c5f 6964 7320 3d20 5b6c 6162 656c  bel_ids = [label
-00008410: 732e 6974 656d 2874 7570 6c65 285b 696e  s.item(tuple([in
-00008420: 7428 6a29 2066 6f72 206a 2069 6e20 695d  t(j) for j in i]
-00008430: 2929 2066 6f72 2069 2069 6e20 706f 696e  )) for i in poin
-00008440: 7473 5d0d 0a0d 0a20 2020 2023 206d 616b  ts]....    # mak
-00008450: 6520 6120 6269 6e61 7279 2069 6d61 6765  e a binary image
-00008460: 2066 6972 7374 0d0a 2020 2020 6269 6e61   first..    bina
-00008470: 7279 203d 206e 702e 7a65 726f 7328 6c61  ry = np.zeros(la
-00008480: 6265 6c73 2e73 6861 7065 2c20 6474 7970  bels.shape, dtyp
-00008490: 653d 626f 6f6c 290d 0a20 2020 206e 6577  e=bool)..    new
-000084a0: 5f6c 6162 656c 5f69 6420 3d20 6d69 6e28  _label_id = min(
-000084b0: 6c61 6265 6c5f 6964 7329 0d0a 2020 2020  label_ids)..    
-000084c0: 666f 7220 6c20 696e 206c 6162 656c 5f69  for l in label_i
-000084d0: 6473 3a0d 0a20 2020 2020 2020 2062 696e  ds:..        bin
-000084e0: 6172 795b 6c61 6265 6c73 203d 3d20 6c5d  ary[labels == l]
-000084f0: 203d 2054 7275 650d 0a0d 0a20 2020 2023   = True....    #
-00008500: 206f 7269 6769 6e3a 2068 7474 7073 3a2f   origin: https:/
-00008510: 2f73 6369 6b69 742d 696d 6167 652e 6f72  /scikit-image.or
-00008520: 672f 646f 6373 2f64 6576 2f61 7574 6f5f  g/docs/dev/auto_
-00008530: 6578 616d 706c 6573 2f73 6567 6d65 6e74  examples/segment
-00008540: 6174 696f 6e2f 706c 6f74 5f77 6174 6572  ation/plot_water
-00008550: 7368 6564 2e68 746d 6c0d 0a20 2020 2066  shed.html..    f
-00008560: 726f 6d20 7363 6970 7920 696d 706f 7274  rom scipy import
-00008570: 206e 6469 6d61 6765 2061 7320 6e64 690d   ndimage as ndi.
-00008580: 0a20 2020 2066 726f 6d20 736b 696d 6167  .    from skimag
-00008590: 652e 7365 676d 656e 7461 7469 6f6e 2069  e.segmentation i
-000085a0: 6d70 6f72 7420 7761 7465 7273 6865 640d  mport watershed.
-000085b0: 0a20 2020 2023 6672 6f6d 2073 6b69 6d61  .    #from skima
-000085c0: 6765 2e66 6561 7475 7265 2069 6d70 6f72  ge.feature impor
-000085d0: 7420 7065 616b 5f6c 6f63 616c 5f6d 6178  t peak_local_max
-000085e0: 0d0a 0d0a 2020 2020 2364 6973 7461 6e63  ....    #distanc
-000085f0: 6520 3d20 6e64 692e 6469 7374 616e 6365  e = ndi.distance
-00008600: 5f74 7261 6e73 666f 726d 5f65 6474 2862  _transform_edt(b
-00008610: 696e 6172 7929 0d0a 2020 2020 2363 6f6f  inary)..    #coo
-00008620: 7264 7320 3d20 7065 616b 5f6c 6f63 616c  rds = peak_local
-00008630: 5f6d 6178 2864 6973 7461 6e63 652c 2066  _max(distance, f
-00008640: 6f6f 7470 7269 6e74 3d6e 702e 6f6e 6573  ootprint=np.ones
-00008650: 2828 332c 2033 2929 2c20 6c61 6265 6c73  ((3, 3)), labels
-00008660: 3d62 696e 6172 7929 0d0a 2020 2020 6d61  =binary)..    ma
-00008670: 736b 203d 206e 702e 7a65 726f 7328 6c61  sk = np.zeros(la
-00008680: 6265 6c73 2e73 6861 7065 2c20 6474 7970  bels.shape, dtyp
-00008690: 653d 626f 6f6c 290d 0a20 2020 2066 6f72  e=bool)..    for
-000086a0: 2069 2069 6e20 706f 696e 7473 3a0d 0a20   i in points:.. 
-000086b0: 2020 2020 2020 2023 6d61 736b 5b74 7570         #mask[tup
-000086c0: 6c65 2870 6f69 6e74 7329 5d20 3d20 5472  le(points)] = Tr
-000086d0: 7565 0d0a 2020 2020 2020 2020 6d61 736b  ue..        mask
-000086e0: 5b74 7570 6c65 285b 696e 7428 6a29 2066  [tuple([int(j) f
-000086f0: 6f72 206a 2069 6e20 695d 295d 203d 2054  or j in i])] = T
-00008700: 7275 650d 0a0d 0a20 2020 206d 6172 6b65  rue....    marke
-00008710: 7273 2c20 5f20 3d20 6e64 692e 6c61 6265  rs, _ = ndi.labe
-00008720: 6c28 6d61 736b 290d 0a20 2020 206e 6577  l(mask)..    new
-00008730: 5f6c 6162 656c 7320 3d20 7761 7465 7273  _labels = waters
-00008740: 6865 6428 6269 6e61 7279 2c20 6d61 726b  hed(binary, mark
-00008750: 6572 732c 206d 6173 6b3d 6269 6e61 7279  ers, mask=binary
-00008760: 290d 0a20 2020 206c 6162 656c 735b 6269  )..    labels[bi
-00008770: 6e61 7279 5d20 3d20 6e65 775f 6c61 6265  nary] = new_labe
-00008780: 6c73 5b62 696e 6172 795d 202b 206c 6162  ls[binary] + lab
-00008790: 656c 732e 6d61 7828 290d 0a0d 0a20 2020  els.max()....   
-000087a0: 206c 6162 656c 735f 6c61 7965 722e 6461   labels_layer.da
-000087b0: 7461 203d 206c 6162 656c 730d 0a20 2020  ta = labels..   
-000087c0: 2070 6f69 6e74 735f 6c61 7965 722e 6461   points_layer.da
-000087d0: 7461 203d 205b 5d0d 0a0d 0a0d 0a40 7265  ta = []......@re
-000087e0: 6769 7374 6572 5f66 756e 6374 696f 6e28  gister_function(
-000087f0: 6d65 6e75 3d22 4669 6c74 6572 696e 6720  menu="Filtering 
-00008800: 2f20 6e6f 6973 6520 7265 6d6f 7661 6c20  / noise removal 
-00008810: 3e20 4275 7474 6572 776f 7274 6820 2873  > Butterworth (s
-00008820: 6369 6b69 742d 696d 6167 652c 206e 7362  cikit-image, nsb
-00008830: 6174 776d 2922 290d 0a40 6a75 7079 7465  atwm)")..@jupyte
-00008840: 725f 6469 7370 6c61 7961 626c 655f 6f75  r_displayable_ou
-00008850: 7470 7574 286c 6962 7261 7279 5f6e 616d  tput(library_nam
-00008860: 653d 276e 7362 6174 776d 272c 2068 656c  e='nsbatwm', hel
-00008870: 705f 7572 6c3d 2768 7474 7073 3a2f 2f77  p_url='https://w
-00008880: 7777 2e6e 6170 6172 692d 6875 622e 6f72  ww.napari-hub.or
-00008890: 672f 706c 7567 696e 732f 6e61 7061 7269  g/plugins/napari
-000088a0: 2d73 6567 6d65 6e74 2d62 6c6f 6273 2d61  -segment-blobs-a
-000088b0: 6e64 2d74 6869 6e67 732d 7769 7468 2d6d  nd-things-with-m
-000088c0: 656d 6272 616e 6573 2729 0d0a 4074 696d  embranes')..@tim
-000088d0: 655f 736c 6963 6572 0d0a 6465 6620 6275  e_slicer..def bu
-000088e0: 7474 6572 776f 7274 6828 696d 6167 653a  tterworth(image:
-000088f0: 2022 6e61 7061 7269 2e74 7970 6573 2e49   "napari.types.I
-00008900: 6d61 6765 4461 7461 222c 2063 7574 6f66  mageData", cutof
-00008910: 665f 6672 6571 7565 6e63 795f 7261 7469  f_frequency_rati
-00008920: 6f3a 2066 6c6f 6174 203d 2030 2e30 3035  o: float = 0.005
-00008930: 2c20 6869 6768 5f70 6173 733a 2062 6f6f  , high_pass: boo
-00008940: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
-00008950: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
-00008960: 723a 2066 6c6f 6174 203d 2032 2920 2d3e  r: float = 2) ->
-00008970: 2022 6e61 7061 7269 2e74 7970 6573 2e49   "napari.types.I
-00008980: 6d61 6765 4461 7461 223a 0d0a 2020 2020  mageData":..    
-00008990: 2222 2241 7070 6c79 2061 2042 7574 7465  """Apply a Butte
-000089a0: 7277 6f72 7468 2066 696c 7465 7220 746f  rworth filter to
-000089b0: 2065 6e68 616e 6365 2068 6967 6820 6f72   enhance high or
-000089c0: 206c 6f77 2066 7265 7175 656e 6379 2066   low frequency f
-000089d0: 6561 7475 7265 732e 0d0a 0d0a 2020 2020  eatures.....    
-000089e0: 5468 6973 2066 696c 7465 7220 6973 2064  This filter is d
-000089f0: 6566 696e 6564 2069 6e20 7468 6520 466f  efined in the Fo
-00008a00: 7572 6965 7220 646f 6d61 696e 2e0d 0a0d  urier domain....
-00008a10: 0a20 2020 2050 6172 616d 6574 6572 730d  .    Parameters.
-00008a20: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d  .    ----------.
-00008a30: 0a20 2020 2069 6d61 6765 203a 2028 4d5b  .    image : (M[
-00008a40: 2c20 4e5b 2c20 2e2e 2e2c 2050 5d5d 5b2c  , N[, ..., P]][,
-00008a50: 2043 5d29 206e 6461 7272 6179 0d0a 2020   C]) ndarray..  
-00008a60: 2020 2020 2020 496e 7075 7420 696d 6167        Input imag
-00008a70: 652e 0d0a 2020 2020 6375 746f 6666 5f66  e...    cutoff_f
-00008a80: 7265 7175 656e 6379 5f72 6174 696f 203a  requency_ratio :
-00008a90: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
-00008aa0: 0d0a 2020 2020 2020 2020 4465 7465 726d  ..        Determ
-00008ab0: 696e 6573 2074 6865 2070 6f73 6974 696f  ines the positio
-00008ac0: 6e20 6f66 2074 6865 2063 7574 2d6f 6666  n of the cut-off
-00008ad0: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
-00008ae0: 2073 6861 7065 206f 6620 7468 650d 0a20   shape of the.. 
-00008af0: 2020 2020 2020 2046 4654 2e0d 0a20 2020         FFT...   
-00008b00: 2068 6967 685f 7061 7373 203a 2062 6f6f   high_pass : boo
-00008b10: 6c2c 206f 7074 696f 6e61 6c0d 0a20 2020  l, optional..   
-00008b20: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00008b30: 7065 7266 6f72 6d20 6120 6869 6768 2070  perform a high p
-00008b40: 6173 7320 6669 6c74 6572 2e20 4966 2046  ass filter. If F
-00008b50: 616c 7365 2c20 6120 6c6f 7720 7061 7373  alse, a low pass
-00008b60: 2066 696c 7465 7220 6973 0d0a 2020 2020   filter is..    
-00008b70: 2020 2020 7065 7266 6f72 6d65 642e 0d0a      performed...
-00008b80: 2020 2020 6f72 6465 7220 3a20 666c 6f61      order : floa
-00008b90: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-00008ba0: 2020 2020 204f 7264 6572 206f 6620 7468       Order of th
-00008bb0: 6520 6669 6c74 6572 2077 6869 6368 2061  e filter which a
-00008bc0: 6666 6563 7473 2074 6865 2073 6c6f 7065  ffects the slope
-00008bd0: 206e 6561 7220 7468 6520 6375 742d 6f66   near the cut-of
-00008be0: 662e 2048 6967 6865 720d 0a20 2020 2020  f. Higher..     
-00008bf0: 2020 206f 7264 6572 206d 6561 6e73 2073     order means s
-00008c00: 7465 6570 6572 2073 6c6f 7065 2069 6e20  teeper slope in 
-00008c10: 6672 6571 7565 6e63 7920 7370 6163 652e  frequency space.
-00008c20: 0d0a 0d0a 2020 2020 5365 6520 616c 736f  ....    See also
-00008c30: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a  ..    --------..
-00008c40: 2020 2020 2e2e 5b30 5d20 6874 7470 733a      ..[0] https:
-00008c50: 2f2f 7363 696b 6974 2d69 6d61 6765 2e6f  //scikit-image.o
-00008c60: 7267 2f64 6f63 732f 7374 6162 6c65 2f61  rg/docs/stable/a
-00008c70: 7069 2f73 6b69 6d61 6765 2e66 696c 7465  pi/skimage.filte
-00008c80: 7273 2e68 746d 6c23 736b 696d 6167 652e  rs.html#skimage.
-00008c90: 6669 6c74 6572 732e 6275 7474 6572 776f  filters.butterwo
-00008ca0: 7274 680d 0a20 2020 2022 2222 0d0a 2020  rth..    """..  
-00008cb0: 2020 6672 6f6d 2073 6b69 6d61 6765 2e66    from skimage.f
-00008cc0: 696c 7465 7273 2069 6d70 6f72 7420 6275  ilters import bu
-00008cd0: 7474 6572 776f 7274 6820 6173 2073 6b69  tterworth as ski
-00008ce0: 6d61 6765 5f62 7574 7465 7277 6f72 7468  mage_butterworth
-00008cf0: 0d0a 2020 2020 7265 7475 726e 2073 6b69  ..    return ski
-00008d00: 6d61 6765 5f62 7574 7465 7277 6f72 7468  mage_butterworth
-00008d10: 2869 6d61 6765 2c20 6375 746f 6666 5f66  (image, cutoff_f
-00008d20: 7265 7175 656e 6379 5f72 6174 696f 2c20  requency_ratio, 
-00008d30: 6869 6768 5f70 6173 732c 206f 7264 6572  high_pass, order
-00008d40: 290d 0a0d 0a0d 0a40 7265 6769 7374 6572  )......@register
-00008d50: 5f66 756e 6374 696f 6e28 6d65 6e75 3d22  _function(menu="
-00008d60: 5574 696c 6974 6965 7320 3e20 4578 7472  Utilities > Extr
-00008d70: 6163 7420 736c 6963 6520 286e 7362 6174  act slice (nsbat
-00008d80: 776d 2922 290d 0a40 7265 6769 7374 6572  wm)")..@register
-00008d90: 5f66 756e 6374 696f 6e28 6d65 6e75 3d22  _function(menu="
-00008da0: 5472 616e 7366 6f72 6d73 203e 2045 7874  Transforms > Ext
-00008db0: 7261 6374 2073 6c69 6365 2028 6e73 6261  ract slice (nsba
-00008dc0: 7477 6d29 2229 0d0a 406a 7570 7974 6572  twm)")..@jupyter
-00008dd0: 5f64 6973 706c 6179 6162 6c65 5f6f 7574  _displayable_out
-00008de0: 7075 7428 6c69 6272 6172 795f 6e61 6d65  put(library_name
-00008df0: 3d27 6e73 6261 7477 6d27 2c20 6865 6c70  ='nsbatwm', help
-00008e00: 5f75 726c 3d27 6874 7470 733a 2f2f 7777  _url='https://ww
-00008e10: 772e 6e61 7061 7269 2d68 7562 2e6f 7267  w.napari-hub.org
-00008e20: 2f70 6c75 6769 6e73 2f6e 6170 6172 692d  /plugins/napari-
-00008e30: 7365 676d 656e 742d 626c 6f62 732d 616e  segment-blobs-an
-00008e40: 642d 7468 696e 6773 2d77 6974 682d 6d65  d-things-with-me
-00008e50: 6d62 7261 6e65 7327 290d 0a40 7469 6d65  mbranes')..@time
-00008e60: 5f73 6c69 6365 720d 0a64 6566 2065 7874  _slicer..def ext
-00008e70: 7261 6374 5f73 6c69 6365 2869 6d61 6765  ract_slice(image
-00008e80: 3a22 6e61 7061 7269 2e74 7970 6573 2e49  :"napari.types.I
-00008e90: 6d61 6765 4461 7461 222c 2073 6c69 6365  mageData", slice
-00008ea0: 5f69 6e64 6578 3a69 6e74 203d 2030 2c20  _index:int = 0, 
-00008eb0: 6178 6973 3a69 6e74 203d 2030 2920 2d3e  axis:int = 0) ->
-00008ec0: 2022 6e61 7061 7269 2e74 7970 6573 2e49   "napari.types.I
-00008ed0: 6d61 6765 4461 7461 223a 0d0a 2020 2020  mageData":..    
-00008ee0: 2222 2245 7874 7261 6374 2028 7461 6b65  """Extract (take
-00008ef0: 2920 6120 736c 6963 6520 6672 6f6d 2061  ) a slice from a
-00008f00: 2073 7461 636b 2e0d 0a0d 0a20 2020 2053   stack.....    S
-00008f10: 6565 2061 6c73 6f0d 0a20 2020 202d 2d2d  ee also..    ---
-00008f20: 2d2d 2d2d 2d0d 0a20 2020 202e 2e5b 305d  -----..    ..[0]
-00008f30: 2068 7474 7073 3a2f 2f6e 756d 7079 2e6f   https://numpy.o
-00008f40: 7267 2f64 6f63 2f73 7461 626c 652f 7265  rg/doc/stable/re
-00008f50: 6665 7265 6e63 652f 6765 6e65 7261 7465  ference/generate
-00008f60: 642f 6e75 6d70 792e 7461 6b65 2e68 746d  d/numpy.take.htm
-00008f70: 6c0d 0a20 2020 2022 2222 0d0a 2020 2020  l..    """..    
-00008f80: 7265 7475 726e 206e 702e 7461 6b65 2869  return np.take(i
-00008f90: 6d61 6765 2c20 736c 6963 655f 696e 6465  mage, slice_inde
-00008fa0: 782c 2061 7869 733d 6178 6973 290d 0a    x, axis=axis)..
+00000620: 2020 206d 696e 696d 756d 5f66 696c 7465     minimum_filte
+00000630: 722c 0d0a 2020 2020 2020 2020 7065 7263  r,..        perc
+00000640: 656e 7469 6c65 5f66 696c 7465 722c 0d0a  entile_filter,..
+00000650: 2020 2020 2020 2020 626c 6163 6b5f 746f          black_to
+00000660: 7068 6174 2c0d 0a20 2020 2020 2020 2077  phat,..        w
+00000670: 6869 7465 5f74 6f70 6861 742c 0d0a 2020  hite_tophat,..  
+00000680: 2020 2020 2020 6d6f 7270 686f 6c6f 6769        morphologi
+00000690: 6361 6c5f 6772 6164 6965 6e74 2c0d 0a20  cal_gradient,.. 
+000006a0: 2020 2020 2020 206c 6f63 616c 5f6d 696e         local_min
+000006b0: 696d 615f 7365 6564 6564 5f77 6174 6572  ima_seeded_water
+000006c0: 7368 6564 2c0d 0a20 2020 2020 2020 2074  shed,..        t
+000006d0: 6872 6573 686f 6c64 6564 5f6c 6f63 616c  hresholded_local
+000006e0: 5f6d 696e 696d 615f 7365 6564 6564 5f77  _minima_seeded_w
+000006f0: 6174 6572 7368 6564 2c0d 0a20 2020 2020  atershed,..     
+00000700: 2020 2073 756d 5f69 6d61 6765 732c 0d0a     sum_images,..
+00000710: 2020 2020 2020 2020 6d75 6c74 6970 6c79          multiply
+00000720: 5f69 6d61 6765 732c 0d0a 2020 2020 2020  _images,..      
+00000730: 2020 6469 7669 6465 5f69 6d61 6765 732c    divide_images,
+00000740: 0d0a 2020 2020 2020 2020 696e 7665 7274  ..        invert
+00000750: 5f69 6d61 6765 2c0d 0a20 2020 2020 2020  _image,..       
+00000760: 2073 6b65 6c65 746f 6e69 7a65 2c0d 0a20   skeletonize,.. 
+00000770: 2020 2020 2020 204d 616e 7561 6c6c 795f         Manually_
+00000780: 6d65 7267 655f 6c61 6265 6c73 2c0d 0a20  merge_labels,.. 
+00000790: 2020 2020 2020 204d 616e 7561 6c6c 795f         Manually_
+000007a0: 7370 6c69 745f 6c61 6265 6c73 2c0d 0a20  split_labels,.. 
+000007b0: 2020 2020 2020 2072 6573 6361 6c65 2c0d         rescale,.
+000007c0: 0a20 2020 2020 2020 2072 6573 697a 652c  .        resize,
+000007d0: 0d0a 2020 2020 2020 2020 6578 7472 6163  ..        extrac
+000007e0: 745f 736c 6963 650d 0a20 2020 205d 0d0a  t_slice..    ]..
+000007f0: 0d0a 0d0a 0d0a 0d0a 0d0a 0d0a 6465 6620  ............def 
+00000800: 5f73 6f62 656c 5f33 6428 696d 6167 6529  _sobel_3d(image)
+00000810: 3a0d 0a20 2020 206b 6572 6e65 6c20 3d20  :..    kernel = 
+00000820: 6e70 2e61 7361 7272 6179 285b 0d0a 2020  np.asarray([..  
+00000830: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
+00000840: 2020 2020 205b 302c 2030 2c20 305d 2c0d       [0, 0, 0],.
+00000850: 0a20 2020 2020 2020 2020 2020 205b 302c  .            [0,
+00000860: 2031 2c20 305d 2c0d 0a20 2020 2020 2020   1, 0],..       
+00000870: 2020 2020 205b 302c 2030 2c20 305d 0d0a       [0, 0, 0]..
+00000880: 2020 2020 2020 2020 5d2c 205b 0d0a 2020          ], [..  
+00000890: 2020 2020 2020 2020 2020 5b30 2c20 312c            [0, 1,
+000008a0: 2030 5d2c 0d0a 2020 2020 2020 2020 2020   0],..          
+000008b0: 2020 5b31 2c20 2d36 2c20 315d 2c0d 0a20    [1, -6, 1],.. 
+000008c0: 2020 2020 2020 2020 2020 205b 302c 2031             [0, 1
+000008d0: 2c20 305d 0d0a 2020 2020 2020 2020 5d2c  , 0]..        ],
+000008e0: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+000008f0: 5b30 2c20 302c 2030 5d2c 0d0a 2020 2020  [0, 0, 0],..    
+00000900: 2020 2020 2020 2020 5b30 2c20 312c 2030          [0, 1, 0
+00000910: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00000920: 5b30 2c20 302c 2030 5d0d 0a20 2020 2020  [0, 0, 0]..     
+00000930: 2020 205d 0d0a 2020 2020 5d29 0d0a 2020     ]..    ])..  
+00000940: 2020 7265 7475 726e 206e 6469 2e63 6f6e    return ndi.con
+00000950: 766f 6c76 6528 696d 6167 652c 206b 6572  volve(image, ker
+00000960: 6e65 6c29 0d0a 0d0a 0d0a 4072 6567 6973  nel)......@regis
+00000970: 7465 725f 6675 6e63 7469 6f6e 286d 656e  ter_function(men
+00000980: 753d 2253 6567 6d65 6e74 6174 696f 6e20  u="Segmentation 
+00000990: 706f 7374 2d70 726f 6365 7373 696e 6720  post-processing 
+000009a0: 3e20 5370 6c69 7420 746f 7563 6869 6e67  > Split touching
+000009b0: 206f 626a 6563 7473 2028 6e73 6261 7477   objects (nsbatw
+000009c0: 6d29 2229 0d0a 406a 7570 7974 6572 5f64  m)")..@jupyter_d
+000009d0: 6973 706c 6179 6162 6c65 5f6f 7574 7075  isplayable_outpu
+000009e0: 7428 6c69 6272 6172 795f 6e61 6d65 3d27  t(library_name='
+000009f0: 6e73 6261 7477 6d27 2c20 6865 6c70 5f75  nsbatwm', help_u
+00000a00: 726c 3d27 6874 7470 733a 2f2f 7777 772e  rl='https://www.
+00000a10: 6e61 7061 7269 2d68 7562 2e6f 7267 2f70  napari-hub.org/p
+00000a20: 6c75 6769 6e73 2f6e 6170 6172 692d 7365  lugins/napari-se
+00000a30: 676d 656e 742d 626c 6f62 732d 616e 642d  gment-blobs-and-
+00000a40: 7468 696e 6773 2d77 6974 682d 6d65 6d62  things-with-memb
+00000a50: 7261 6e65 7327 290d 0a40 7469 6d65 5f73  ranes')..@time_s
+00000a60: 6c69 6365 720d 0a64 6566 2073 706c 6974  licer..def split
+00000a70: 5f74 6f75 6368 696e 675f 6f62 6a65 6374  _touching_object
+00000a80: 7328 6269 6e61 7279 3a22 6e61 7061 7269  s(binary:"napari
+00000a90: 2e74 7970 6573 2e4c 6162 656c 7344 6174  .types.LabelsDat
+00000aa0: 6122 2c20 7369 676d 613a 2066 6c6f 6174  a", sigma: float
+00000ab0: 203d 2033 2e35 2920 2d3e 2022 6e61 7061   = 3.5) -> "napa
+00000ac0: 7269 2e74 7970 6573 2e4c 6162 656c 7344  ri.types.LabelsD
+00000ad0: 6174 6122 3a0d 0a20 2020 2022 2222 0d0a  ata":..    """..
+00000ae0: 2020 2020 5461 6b65 7320 6120 6269 6e61      Takes a bina
+00000af0: 7279 2069 6d61 6765 2061 6e64 2064 7261  ry image and dra
+00000b00: 7773 2063 7574 7320 696e 2074 6865 206f  ws cuts in the o
+00000b10: 626a 6563 7473 2073 696d 696c 6172 2074  bjects similar t
+00000b20: 6f20 7468 6520 496d 6167 654a 2077 6174  o the ImageJ wat
+00000b30: 6572 7368 6564 2061 6c67 6f72 6974 686d  ershed algorithm
+00000b40: 205b 315d 2e0d 0a0d 0a20 2020 2054 6869   [1].....    Thi
+00000b50: 7320 616c 6c6f 7773 2063 7574 7469 6e67  s allows cutting
+00000b60: 2063 6f6e 6e65 6374 6564 206f 626a 6563   connected objec
+00000b70: 7473 2073 7563 6820 6173 206e 6f74 2074  ts such as not t
+00000b80: 6f20 6465 6e73 6520 6e75 636c 6569 2e20  o dense nuclei. 
+00000b90: 4966 2074 6865 206e 7563 6c65 6920 6172  If the nuclei ar
+00000ba0: 6520 746f 6f20 6465 6e73 652c 0d0a 2020  e too dense,..  
+00000bb0: 2020 636f 6e73 6964 6572 2075 7369 6e67    consider using
+00000bc0: 2073 7461 7264 6973 7420 5b32 5d20 6f72   stardist [2] or
+00000bd0: 2063 656c 6c70 6f73 6520 5b33 5d2e 0d0a   cellpose [3]...
+00000be0: 0d0a 2020 2020 5365 6520 616c 736f 0d0a  ..    See also..
+00000bf0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020      --------..  
+00000c00: 2020 2e2e 205b 315d 2068 7474 7073 3a2f    .. [1] https:/
+00000c10: 2f69 6d61 6765 6a2e 6e69 682e 676f 762f  /imagej.nih.gov/
+00000c20: 696a 2f64 6f63 732f 6d65 6e75 732f 7072  ij/docs/menus/pr
+00000c30: 6f63 6573 732e 6874 6d6c 2377 6174 6572  ocess.html#water
+00000c40: 7368 6564 0d0a 2020 2020 2e2e 205b 325d  shed..    .. [2]
+00000c50: 2068 7474 7073 3a2f 2f77 7777 2e6e 6170   https://www.nap
+00000c60: 6172 692d 6875 622e 6f72 672f 706c 7567  ari-hub.org/plug
+00000c70: 696e 732f 7374 6172 6469 7374 2d6e 6170  ins/stardist-nap
+00000c80: 6172 690d 0a20 2020 202e 2e20 5b33 5d20  ari..    .. [3] 
+00000c90: 6874 7470 733a 2f2f 7777 772e 6e61 7061  https://www.napa
+00000ca0: 7269 2d68 7562 2e6f 7267 2f70 6c75 6769  ri-hub.org/plugi
+00000cb0: 6e73 2f63 656c 6c70 6f73 652d 6e61 7061  ns/cellpose-napa
+00000cc0: 7269 0d0a 2020 2020 2222 220d 0a20 2020  ri..    """..   
+00000cd0: 2062 696e 6172 7920 3d20 6e70 2e61 7361   binary = np.asa
+00000ce0: 7272 6179 2862 696e 6172 7929 0d0a 0d0a  rray(binary)....
+00000cf0: 2020 2020 2320 7479 7069 6361 6c20 7761      # typical wa
+00000d00: 7920 6f66 2075 7369 6e67 2073 6369 6b69  y of using sciki
+00000d10: 742d 696d 6167 6520 7761 7465 7273 6865  t-image watershe
+00000d20: 640d 0a20 2020 2064 6973 7461 6e63 6520  d..    distance 
+00000d30: 3d20 6e64 692e 6469 7374 616e 6365 5f74  = ndi.distance_t
+00000d40: 7261 6e73 666f 726d 5f65 6474 2862 696e  ransform_edt(bin
+00000d50: 6172 7929 0d0a 2020 2020 626c 7572 7265  ary)..    blurre
+00000d60: 645f 6469 7374 616e 6365 203d 2067 6175  d_distance = gau
+00000d70: 7373 6961 6e28 6469 7374 616e 6365 2c20  ssian(distance, 
+00000d80: 7369 676d 613d 7369 676d 6129 0d0a 2020  sigma=sigma)..  
+00000d90: 2020 6670 203d 206e 702e 6f6e 6573 2828    fp = np.ones((
+00000da0: 332c 2920 2a20 6269 6e61 7279 2e6e 6469  3,) * binary.ndi
+00000db0: 6d29 0d0a 2020 2020 636f 6f72 6473 203d  m)..    coords =
+00000dc0: 2070 6561 6b5f 6c6f 6361 6c5f 6d61 7828   peak_local_max(
+00000dd0: 626c 7572 7265 645f 6469 7374 616e 6365  blurred_distance
+00000de0: 2c20 666f 6f74 7072 696e 743d 6670 2c20  , footprint=fp, 
+00000df0: 6c61 6265 6c73 3d62 696e 6172 7929 0d0a  labels=binary)..
+00000e00: 2020 2020 6d61 736b 203d 206e 702e 7a65      mask = np.ze
+00000e10: 726f 7328 6469 7374 616e 6365 2e73 6861  ros(distance.sha
+00000e20: 7065 2c20 6474 7970 653d 626f 6f6c 290d  pe, dtype=bool).
+00000e30: 0a20 2020 206d 6173 6b5b 7475 706c 6528  .    mask[tuple(
+00000e40: 636f 6f72 6473 2e54 295d 203d 2054 7275  coords.T)] = Tru
+00000e50: 650d 0a20 2020 206d 6172 6b65 7273 203d  e..    markers =
+00000e60: 206c 6162 656c 286d 6173 6b29 0d0a 2020   label(mask)..  
+00000e70: 2020 6c61 6265 6c73 203d 2077 6174 6572    labels = water
+00000e80: 7368 6564 282d 626c 7572 7265 645f 6469  shed(-blurred_di
+00000e90: 7374 616e 6365 2c20 6d61 726b 6572 732c  stance, markers,
+00000ea0: 206d 6173 6b3d 6269 6e61 7279 290d 0a0d   mask=binary)...
+00000eb0: 0a20 2020 2023 2069 6465 6e74 6966 7920  .    # identify 
+00000ec0: 6c61 6265 6c2d 6375 7474 696e 6720 6564  label-cutting ed
+00000ed0: 6765 730d 0a20 2020 2069 6620 6c65 6e28  ges..    if len(
+00000ee0: 6269 6e61 7279 2e73 6861 7065 2920 3d3d  binary.shape) ==
+00000ef0: 2032 3a0d 0a20 2020 2020 2020 2065 6467   2:..        edg
+00000f00: 6573 203d 2073 6f62 656c 286c 6162 656c  es = sobel(label
+00000f10: 7329 0d0a 2020 2020 2020 2020 6564 6765  s)..        edge
+00000f20: 7332 203d 2073 6f62 656c 2862 696e 6172  s2 = sobel(binar
+00000f30: 7929 0d0a 2020 2020 656c 7365 3a20 2320  y)..    else: # 
+00000f40: 6173 7375 6d69 6e67 2033 440d 0a20 2020  assuming 3D..   
+00000f50: 2020 2020 2065 6467 6573 203d 205f 736f       edges = _so
+00000f60: 6265 6c5f 3364 286c 6162 656c 7329 0d0a  bel_3d(labels)..
+00000f70: 2020 2020 2020 2020 6564 6765 7332 203d          edges2 =
+00000f80: 205f 736f 6265 6c5f 3364 2862 696e 6172   _sobel_3d(binar
+00000f90: 7929 0d0a 0d0a 2020 2020 616c 6d6f 7374  y)....    almost
+00000fa0: 203d 206e 702e 6c6f 6769 6361 6c5f 6e6f   = np.logical_no
+00000fb0: 7428 6e70 2e6c 6f67 6963 616c 5f78 6f72  t(np.logical_xor
+00000fc0: 2865 6467 6573 2021 3d20 302c 2065 6467  (edges != 0, edg
+00000fd0: 6573 3220 213d 2030 2929 202a 2062 696e  es2 != 0)) * bin
+00000fe0: 6172 790d 0a20 2020 2072 6574 7572 6e20  ary..    return 
+00000ff0: 6269 6e61 7279 5f6f 7065 6e69 6e67 2861  binary_opening(a
+00001000: 6c6d 6f73 7429 0d0a 0d0a 0d0a 4072 6567  lmost)......@reg
+00001010: 6973 7465 725f 6675 6e63 7469 6f6e 286d  ister_function(m
+00001020: 656e 753d 2253 6567 6d65 6e74 6174 696f  enu="Segmentatio
+00001030: 6e20 2f20 6269 6e61 7269 7a61 7469 6f6e  n / binarization
+00001040: 203e 2054 6872 6573 686f 6c64 2028 4f74   > Threshold (Ot
+00001050: 7375 2065 7420 616c 2031 3937 392c 2073  su et al 1979, s
+00001060: 6369 6b69 742d 696d 6167 652c 206e 7362  cikit-image, nsb
+00001070: 6174 776d 2922 290d 0a40 6a75 7079 7465  atwm)")..@jupyte
+00001080: 725f 6469 7370 6c61 7961 626c 655f 6f75  r_displayable_ou
+00001090: 7470 7574 286c 6962 7261 7279 5f6e 616d  tput(library_nam
+000010a0: 653d 276e 7362 6174 776d 272c 2068 656c  e='nsbatwm', hel
+000010b0: 705f 7572 6c3d 2768 7474 7073 3a2f 2f77  p_url='https://w
+000010c0: 7777 2e6e 6170 6172 692d 6875 622e 6f72  ww.napari-hub.or
+000010d0: 672f 706c 7567 696e 732f 6e61 7061 7269  g/plugins/napari
+000010e0: 2d73 6567 6d65 6e74 2d62 6c6f 6273 2d61  -segment-blobs-a
+000010f0: 6e64 2d74 6869 6e67 732d 7769 7468 2d6d  nd-things-with-m
+00001100: 656d 6272 616e 6573 2729 0d0a 4074 696d  embranes')..@tim
+00001110: 655f 736c 6963 6572 0d0a 6465 6620 7468  e_slicer..def th
+00001120: 7265 7368 6f6c 645f 6f74 7375 2869 6d61  reshold_otsu(ima
+00001130: 6765 3a22 6e61 7061 7269 2e74 7970 6573  ge:"napari.types
+00001140: 2e49 6d61 6765 4461 7461 2229 202d 3e20  .ImageData") -> 
+00001150: 226e 6170 6172 692e 7479 7065 732e 4c61  "napari.types.La
+00001160: 6265 6c73 4461 7461 223a 0d0a 2020 2020  belsData":..    
+00001170: 2222 220d 0a20 2020 2041 7070 6c69 6573  """..    Applies
+00001180: 204f 7473 7527 7320 7468 7265 7368 6f6c   Otsu's threshol
+00001190: 6420 7365 6c65 6374 696f 6e20 6d65 7468  d selection meth
+000011a0: 6f64 2074 6f20 616e 2069 6e74 656e 7369  od to an intensi
+000011b0: 7479 2069 6d61 6765 2061 6e64 2072 6574  ty image and ret
+000011c0: 7572 6e73 2061 2062 696e 6172 7920 696d  urns a binary im
+000011d0: 6167 6520 7769 7468 2070 6978 656c 733d  age with pixels=
+000011e0: 3d31 2077 6865 7265 0d0a 2020 2020 696e  =1 where..    in
+000011f0: 7465 6e73 6974 7920 6973 2061 626f 7665  tensity is above
+00001200: 2074 6865 2064 6574 6572 6d69 6e65 6420   the determined 
+00001210: 7468 7265 7368 6f6c 642e 0d0a 0d0a 2020  threshold.....  
+00001220: 2020 5365 6520 616c 736f 0d0a 2020 2020    See also..    
+00001230: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2e2e  --------..    ..
+00001240: 205b 305d 2068 7474 7073 3a2f 2f65 6e2e   [0] https://en.
+00001250: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
+00001260: 6b69 2f4f 7473 7525 3237 735f 6d65 7468  ki/Otsu%27s_meth
+00001270: 6f64 0d0a 2020 2020 2e2e 205b 315d 2068  od..    .. [1] h
+00001280: 7474 7073 3a2f 2f69 6565 6578 706c 6f72  ttps://ieeexplor
+00001290: 652e 6965 6565 2e6f 7267 2f64 6f63 756d  e.ieee.org/docum
+000012a0: 656e 742f 3433 3130 3037 360d 0a20 2020  ent/4310076..   
+000012b0: 2022 2222 0d0a 2020 2020 7468 7265 7368   """..    thresh
+000012c0: 6f6c 6420 3d20 736b 5f74 6872 6573 686f  old = sk_thresho
+000012d0: 6c64 5f6f 7473 7528 6e70 2e61 7361 7272  ld_otsu(np.asarr
+000012e0: 6179 2869 6d61 6765 2929 0d0a 2020 2020  ay(image))..    
+000012f0: 6269 6e61 7279 5f6f 7473 7520 3d20 696d  binary_otsu = im
+00001300: 6167 6520 3e20 7468 7265 7368 6f6c 640d  age > threshold.
+00001310: 0a0d 0a20 2020 2072 6574 7572 6e20 6269  ...    return bi
+00001320: 6e61 7279 5f6f 7473 7520 2a20 310d 0a0d  nary_otsu * 1...
+00001330: 0a0d 0a40 7265 6769 7374 6572 5f66 756e  ...@register_fun
+00001340: 6374 696f 6e28 6d65 6e75 3d22 5365 676d  ction(menu="Segm
+00001350: 656e 7461 7469 6f6e 202f 2062 696e 6172  entation / binar
+00001360: 697a 6174 696f 6e20 3e20 5468 7265 7368  ization > Thresh
+00001370: 6f6c 6420 2859 656e 2065 7420 616c 2031  old (Yen et al 1
+00001380: 3939 352c 2073 6369 6b69 742d 696d 6167  995, scikit-imag
+00001390: 652c 206e 7362 6174 776d 2922 290d 0a40  e, nsbatwm)")..@
+000013a0: 6a75 7079 7465 725f 6469 7370 6c61 7961  jupyter_displaya
+000013b0: 626c 655f 6f75 7470 7574 286c 6962 7261  ble_output(libra
+000013c0: 7279 5f6e 616d 653d 276e 7362 6174 776d  ry_name='nsbatwm
+000013d0: 272c 2068 656c 705f 7572 6c3d 2768 7474  ', help_url='htt
+000013e0: 7073 3a2f 2f77 7777 2e6e 6170 6172 692d  ps://www.napari-
+000013f0: 6875 622e 6f72 672f 706c 7567 696e 732f  hub.org/plugins/
+00001400: 6e61 7061 7269 2d73 6567 6d65 6e74 2d62  napari-segment-b
+00001410: 6c6f 6273 2d61 6e64 2d74 6869 6e67 732d  lobs-and-things-
+00001420: 7769 7468 2d6d 656d 6272 616e 6573 2729  with-membranes')
+00001430: 0d0a 4074 696d 655f 736c 6963 6572 0d0a  ..@time_slicer..
+00001440: 6465 6620 7468 7265 7368 6f6c 645f 7965  def threshold_ye
+00001450: 6e28 696d 6167 6520 3a22 6e61 7061 7269  n(image :"napari
+00001460: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
+00001470: 2229 202d 3e20 226e 6170 6172 692e 7479  ") -> "napari.ty
+00001480: 7065 732e 4c61 6265 6c73 4461 7461 223a  pes.LabelsData":
+00001490: 0d0a 2020 2020 2222 220d 0a20 2020 2042  ..    """..    B
+000014a0: 696e 6172 697a 6520 616e 2069 6d61 6765  inarize an image
+000014b0: 2075 7369 6e67 2059 656e 2773 206d 6574   using Yen's met
+000014c0: 686f 642e 0d0a 0d0a 2020 2020 5061 7261  hod.....    Para
+000014d0: 6d65 7465 7273 0d0a 2020 2020 2d2d 2d2d  meters..    ----
+000014e0: 2d2d 2d2d 2d2d 0d0a 2020 2020 696d 6167  ------..    imag
+000014f0: 653a 2049 6d61 6765 0d0a 0d0a 2020 2020  e: Image....    
+00001500: 5365 6520 416c 736f 0d0a 2020 2020 2d2d  See Also..    --
+00001510: 2d2d 2d2d 2d2d 0d0a 2020 2020 2e2e 5b30  ------..    ..[0
+00001520: 5d20 6874 7470 733a 2f2f 696d 6167 656a  ] https://imagej
+00001530: 2e6e 6574 2f70 6c75 6769 6e73 2f61 7574  .net/plugins/aut
+00001540: 6f2d 7468 7265 7368 6f6c 6423 7965 6e0d  o-threshold#yen.
+00001550: 0a0d 0a20 2020 2052 6574 7572 6e73 0d0a  ...    Returns..
+00001560: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+00001570: 2062 696e 6172 795f 696d 6167 653a 206e   binary_image: n
+00001580: 6170 6172 692e 7479 7065 732e 4c61 6265  apari.types.Labe
+00001590: 6c73 4461 7461 0d0a 2020 2020 2222 220d  lsData..    """.
+000015a0: 0a20 2020 2072 6574 7572 6e20 696d 6167  .    return imag
+000015b0: 6520 3e20 6669 6c74 6572 732e 7468 7265  e > filters.thre
+000015c0: 7368 6f6c 645f 7965 6e28 696d 6167 6529  shold_yen(image)
+000015d0: 0d0a 0d0a 0d0a 4072 6567 6973 7465 725f  ......@register_
+000015e0: 6675 6e63 7469 6f6e 286d 656e 753d 2253  function(menu="S
+000015f0: 6567 6d65 6e74 6174 696f 6e20 2f20 6269  egmentation / bi
+00001600: 6e61 7269 7a61 7469 6f6e 203e 2054 6872  narization > Thr
+00001610: 6573 686f 6c64 2028 4973 6f64 6174 612c  eshold (Isodata,
+00001620: 2052 6964 6c65 7220 6574 2061 6c20 3139   Ridler et al 19
+00001630: 3738 2c20 7363 696b 6974 2d69 6d61 6765  78, scikit-image
+00001640: 2c20 6e73 6261 7477 6d29 2229 0d0a 406a  , nsbatwm)")..@j
+00001650: 7570 7974 6572 5f64 6973 706c 6179 6162  upyter_displayab
+00001660: 6c65 5f6f 7574 7075 7428 6c69 6272 6172  le_output(librar
+00001670: 795f 6e61 6d65 3d27 6e73 6261 7477 6d27  y_name='nsbatwm'
+00001680: 2c20 6865 6c70 5f75 726c 3d27 6874 7470  , help_url='http
+00001690: 733a 2f2f 7777 772e 6e61 7061 7269 2d68  s://www.napari-h
+000016a0: 7562 2e6f 7267 2f70 6c75 6769 6e73 2f6e  ub.org/plugins/n
+000016b0: 6170 6172 692d 7365 676d 656e 742d 626c  apari-segment-bl
+000016c0: 6f62 732d 616e 642d 7468 696e 6773 2d77  obs-and-things-w
+000016d0: 6974 682d 6d65 6d62 7261 6e65 7327 290d  ith-membranes').
+000016e0: 0a40 7469 6d65 5f73 6c69 6365 720d 0a64  .@time_slicer..d
+000016f0: 6566 2074 6872 6573 686f 6c64 5f69 736f  ef threshold_iso
+00001700: 6461 7461 2869 6d61 6765 203a 226e 6170  data(image :"nap
+00001710: 6172 692e 7479 7065 732e 496d 6167 6544  ari.types.ImageD
+00001720: 6174 6122 2920 2d3e 2022 6e61 7061 7269  ata") -> "napari
+00001730: 2e74 7970 6573 2e4c 6162 656c 7344 6174  .types.LabelsDat
+00001740: 6122 3a0d 0a20 2020 2022 2222 0d0a 2020  a":..    """..  
+00001750: 2020 4269 6e61 7269 7a65 2061 6e20 696d    Binarize an im
+00001760: 6167 6520 7573 696e 6720 7468 6520 4973  age using the Is
+00001770: 6f44 6174 6120 2f20 5269 646c 6572 2773  oData / Ridler's
+00001780: 206d 6574 686f 642e 0d0a 2020 2020 5468   method...    Th
+00001790: 6520 6d65 7468 6f64 2069 7320 7369 6d69  e method is simi
+000017a0: 6c61 7220 746f 2049 6d61 6765 4a27 7320  lar to ImageJ's 
+000017b0: 2264 6566 6175 6c74 2220 7468 7265 7368  "default" thresh
+000017c0: 6f6c 642e 0d0a 0d0a 2020 2020 5061 7261  old.....    Para
+000017d0: 6d65 7465 7273 0d0a 2020 2020 2d2d 2d2d  meters..    ----
+000017e0: 2d2d 2d2d 2d2d 0d0a 2020 2020 696d 6167  ------..    imag
+000017f0: 653a 2049 6d61 6765 0d0a 0d0a 2020 2020  e: Image....    
+00001800: 5365 6520 416c 736f 0d0a 2020 2020 2d2d  See Also..    --
+00001810: 2d2d 2d2d 2d2d 0d0a 2020 2020 2e2e 5b30  ------..    ..[0
+00001820: 5d20 6874 7470 733a 2f2f 696d 6167 656a  ] https://imagej
+00001830: 2e6e 6574 2f70 6c75 6769 6e73 2f61 7574  .net/plugins/aut
+00001840: 6f2d 7468 7265 7368 6f6c 6423 6973 6f64  o-threshold#isod
+00001850: 6174 610d 0a20 2020 202e 2e5b 315d 2068  ata..    ..[1] h
+00001860: 7474 7073 3a2f 2f69 6565 6578 706c 6f72  ttps://ieeexplor
+00001870: 652e 6965 6565 2e6f 7267 2f64 6f63 756d  e.ieee.org/docum
+00001880: 656e 742f 3433 3130 3033 390d 0a0d 0a20  ent/4310039.... 
+00001890: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
+000018a0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2062 696e  -------..    bin
+000018b0: 6172 795f 696d 6167 653a 206e 6170 6172  ary_image: napar
+000018c0: 692e 7479 7065 732e 4c61 6265 6c73 4461  i.types.LabelsDa
+000018d0: 7461 0d0a 2020 2020 2222 220d 0a20 2020  ta..    """..   
+000018e0: 2072 6574 7572 6e20 696d 6167 6520 3e20   return image > 
+000018f0: 6669 6c74 6572 732e 7468 7265 7368 6f6c  filters.threshol
+00001900: 645f 6973 6f64 6174 6128 696d 6167 6529  d_isodata(image)
+00001910: 0d0a 0d0a 0d0a 4072 6567 6973 7465 725f  ......@register_
+00001920: 6675 6e63 7469 6f6e 286d 656e 753d 2253  function(menu="S
+00001930: 6567 6d65 6e74 6174 696f 6e20 2f20 6269  egmentation / bi
+00001940: 6e61 7269 7a61 7469 6f6e 203e 2054 6872  narization > Thr
+00001950: 6573 686f 6c64 2028 4c69 2065 7420 616c  eshold (Li et al
+00001960: 2031 3939 332c 2073 6369 6b69 742d 696d   1993, scikit-im
+00001970: 6167 652c 206e 7362 6174 776d 2922 290d  age, nsbatwm)").
+00001980: 0a40 6a75 7079 7465 725f 6469 7370 6c61  .@jupyter_displa
+00001990: 7961 626c 655f 6f75 7470 7574 286c 6962  yable_output(lib
+000019a0: 7261 7279 5f6e 616d 653d 276e 7362 6174  rary_name='nsbat
+000019b0: 776d 272c 2068 656c 705f 7572 6c3d 2768  wm', help_url='h
+000019c0: 7474 7073 3a2f 2f77 7777 2e6e 6170 6172  ttps://www.napar
+000019d0: 692d 6875 622e 6f72 672f 706c 7567 696e  i-hub.org/plugin
+000019e0: 732f 6e61 7061 7269 2d73 6567 6d65 6e74  s/napari-segment
+000019f0: 2d62 6c6f 6273 2d61 6e64 2d74 6869 6e67  -blobs-and-thing
+00001a00: 732d 7769 7468 2d6d 656d 6272 616e 6573  s-with-membranes
+00001a10: 2729 0d0a 4074 696d 655f 736c 6963 6572  ')..@time_slicer
+00001a20: 0d0a 6465 6620 7468 7265 7368 6f6c 645f  ..def threshold_
+00001a30: 6c69 2869 6d61 6765 3a22 6e61 7061 7269  li(image:"napari
+00001a40: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
+00001a50: 2229 202d 3e20 226e 6170 6172 692e 7479  ") -> "napari.ty
+00001a60: 7065 732e 4c61 6265 6c73 4461 7461 223a  pes.LabelsData":
+00001a70: 0d0a 2020 2020 2222 220d 0a20 2020 2042  ..    """..    B
+00001a80: 696e 6172 697a 6520 616e 2069 6d61 6765  inarize an image
+00001a90: 2075 7369 6e67 204c 6927 7320 6d65 7468   using Li's meth
+00001aa0: 6f64 206d 6574 686f 642e 0d0a 0d0a 2020  od method.....  
+00001ab0: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
+00001ac0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
+00001ad0: 2020 696d 6167 653a 2049 6d61 6765 0d0a    image: Image..
+00001ae0: 0d0a 2020 2020 5365 6520 416c 736f 0d0a  ..    See Also..
+00001af0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020      --------..  
+00001b00: 2020 2e2e 5b30 5d20 6874 7470 733a 2f2f    ..[0] https://
+00001b10: 696d 6167 656a 2e6e 6574 2f70 6c75 6769  imagej.net/plugi
+00001b20: 6e73 2f61 7574 6f2d 7468 7265 7368 6f6c  ns/auto-threshol
+00001b30: 6423 6c69 0d0a 0d0a 2020 2020 5265 7475  d#li....    Retu
+00001b40: 726e 730d 0a20 2020 202d 2d2d 2d2d 2d2d  rns..    -------
+00001b50: 0d0a 2020 2020 6269 6e61 7279 5f69 6d61  ..    binary_ima
+00001b60: 6765 3a20 6e61 7061 7269 2e74 7970 6573  ge: napari.types
+00001b70: 2e4c 6162 656c 7344 6174 610d 0a20 2020  .LabelsData..   
+00001b80: 2022 2222 0d0a 2020 2020 7265 7475 726e   """..    return
+00001b90: 2069 6d61 6765 203e 2066 696c 7465 7273   image > filters
+00001ba0: 2e74 6872 6573 686f 6c64 5f6c 6928 696d  .threshold_li(im
+00001bb0: 6167 6529 0d0a 0d0a 0d0a 4072 6567 6973  age)......@regis
+00001bc0: 7465 725f 6675 6e63 7469 6f6e 286d 656e  ter_function(men
+00001bd0: 753d 2253 6567 6d65 6e74 6174 696f 6e20  u="Segmentation 
+00001be0: 2f20 6269 6e61 7269 7a61 7469 6f6e 203e  / binarization >
+00001bf0: 2054 6872 6573 686f 6c64 2028 5269 646c   Threshold (Ridl
+00001c00: 6572 2065 7420 616c 2031 3937 382c 2073  er et al 1978, s
+00001c10: 6369 6b69 742d 696d 6167 652c 206e 7362  cikit-image, nsb
+00001c20: 6174 776d 2922 290d 0a40 6a75 7079 7465  atwm)")..@jupyte
+00001c30: 725f 6469 7370 6c61 7961 626c 655f 6f75  r_displayable_ou
+00001c40: 7470 7574 286c 6962 7261 7279 5f6e 616d  tput(library_nam
+00001c50: 653d 276e 7362 6174 776d 272c 2068 656c  e='nsbatwm', hel
+00001c60: 705f 7572 6c3d 2768 7474 7073 3a2f 2f77  p_url='https://w
+00001c70: 7777 2e6e 6170 6172 692d 6875 622e 6f72  ww.napari-hub.or
+00001c80: 672f 706c 7567 696e 732f 6e61 7061 7269  g/plugins/napari
+00001c90: 2d73 6567 6d65 6e74 2d62 6c6f 6273 2d61  -segment-blobs-a
+00001ca0: 6e64 2d74 6869 6e67 732d 7769 7468 2d6d  nd-things-with-m
+00001cb0: 656d 6272 616e 6573 2729 0d0a 4074 696d  embranes')..@tim
+00001cc0: 655f 736c 6963 6572 0d0a 6465 6620 7468  e_slicer..def th
+00001cd0: 7265 7368 6f6c 645f 6d65 616e 2869 6d61  reshold_mean(ima
+00001ce0: 6765 203a 226e 6170 6172 692e 7479 7065  ge :"napari.type
+00001cf0: 732e 496d 6167 6544 6174 6122 2920 2d3e  s.ImageData") ->
+00001d00: 2022 6e61 7061 7269 2e74 7970 6573 2e4c   "napari.types.L
+00001d10: 6162 656c 7344 6174 6122 3a0d 0a20 2020  abelsData":..   
+00001d20: 2022 2222 0d0a 2020 2020 4269 6e61 7269   """..    Binari
+00001d30: 7a65 2061 6e20 696d 6167 6520 7573 696e  ze an image usin
+00001d40: 6720 7468 6520 4d65 616e 206d 6574 686f  g the Mean metho
+00001d50: 642e 0d0a 0d0a 2020 2020 5061 7261 6d65  d.....    Parame
+00001d60: 7465 7273 0d0a 2020 2020 2d2d 2d2d 2d2d  ters..    ------
+00001d70: 2d2d 2d2d 0d0a 2020 2020 696d 6167 653a  ----..    image:
+00001d80: 2049 6d61 6765 0d0a 0d0a 2020 2020 5365   Image....    Se
+00001d90: 6520 416c 736f 0d0a 2020 2020 2d2d 2d2d  e Also..    ----
+00001da0: 2d2d 2d2d 0d0a 2020 2020 2e2e 5b30 5d20  ----..    ..[0] 
+00001db0: 6874 7470 733a 2f2f 696d 6167 656a 2e6e  https://imagej.n
+00001dc0: 6574 2f70 6c75 6769 6e73 2f61 7574 6f2d  et/plugins/auto-
+00001dd0: 7468 7265 7368 6f6c 6423 6d65 616e 0d0a  threshold#mean..
+00001de0: 0d0a 2020 2020 5265 7475 726e 730d 0a20  ..    Returns.. 
+00001df0: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
+00001e00: 6269 6e61 7279 5f69 6d61 6765 3a20 6e61  binary_image: na
+00001e10: 7061 7269 2e74 7970 6573 2e4c 6162 656c  pari.types.Label
+00001e20: 7344 6174 610d 0a20 2020 2022 2222 0d0a  sData..    """..
+00001e30: 2020 2020 7265 7475 726e 2069 6d61 6765      return image
+00001e40: 203e 2066 696c 7465 7273 2e74 6872 6573   > filters.thres
+00001e50: 686f 6c64 5f6d 6561 6e28 696d 6167 6529  hold_mean(image)
+00001e60: 0d0a 0d0a 0d0a 4072 6567 6973 7465 725f  ......@register_
+00001e70: 6675 6e63 7469 6f6e 286d 656e 753d 2253  function(menu="S
+00001e80: 6567 6d65 6e74 6174 696f 6e20 2f20 6269  egmentation / bi
+00001e90: 6e61 7269 7a61 7469 6f6e 203e 2054 6872  narization > Thr
+00001ea0: 6573 686f 6c64 2028 4d65 616e 2c20 7363  eshold (Mean, sc
+00001eb0: 696b 6974 2d69 6d61 6765 2c20 6e73 6261  ikit-image, nsba
+00001ec0: 7477 6d29 2229 0d0a 406a 7570 7974 6572  twm)")..@jupyter
+00001ed0: 5f64 6973 706c 6179 6162 6c65 5f6f 7574  _displayable_out
+00001ee0: 7075 7428 6c69 6272 6172 795f 6e61 6d65  put(library_name
+00001ef0: 3d27 6e73 6261 7477 6d27 2c20 6865 6c70  ='nsbatwm', help
+00001f00: 5f75 726c 3d27 6874 7470 733a 2f2f 7777  _url='https://ww
+00001f10: 772e 6e61 7061 7269 2d68 7562 2e6f 7267  w.napari-hub.org
+00001f20: 2f70 6c75 6769 6e73 2f6e 6170 6172 692d  /plugins/napari-
+00001f30: 7365 676d 656e 742d 626c 6f62 732d 616e  segment-blobs-an
+00001f40: 642d 7468 696e 6773 2d77 6974 682d 6d65  d-things-with-me
+00001f50: 6d62 7261 6e65 7327 290d 0a40 7469 6d65  mbranes')..@time
+00001f60: 5f73 6c69 6365 720d 0a64 6566 2074 6872  _slicer..def thr
+00001f70: 6573 686f 6c64 5f6d 696e 696d 756d 2869  eshold_minimum(i
+00001f80: 6d61 6765 203a 226e 6170 6172 692e 7479  mage :"napari.ty
+00001f90: 7065 732e 496d 6167 6544 6174 6122 2920  pes.ImageData") 
+00001fa0: 2d3e 2022 6e61 7061 7269 2e74 7970 6573  -> "napari.types
+00001fb0: 2e4c 6162 656c 7344 6174 6122 3a0d 0a20  .LabelsData":.. 
+00001fc0: 2020 2022 2222 0d0a 2020 2020 4269 6e61     """..    Bina
+00001fd0: 7269 7a65 2061 6e20 696d 6167 6520 7573  rize an image us
+00001fe0: 696e 6720 7468 6520 4d69 6e69 6d75 6d20  ing the Minimum 
+00001ff0: 6d65 7468 6f64 2e0d 0a0d 0a20 2020 2050  method.....    P
+00002000: 6172 616d 6574 6572 730d 0a20 2020 202d  arameters..    -
+00002010: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2069  ---------..    i
+00002020: 6d61 6765 3a20 496d 6167 650d 0a0d 0a20  mage: Image.... 
+00002030: 2020 2053 6565 2041 6c73 6f0d 0a20 2020     See Also..   
+00002040: 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020 202e   --------..    .
+00002050: 2e5b 305d 2068 7474 7073 3a2f 2f69 6d61  .[0] https://ima
+00002060: 6765 6a2e 6e65 742f 706c 7567 696e 732f  gej.net/plugins/
+00002070: 6175 746f 2d74 6872 6573 686f 6c64 236d  auto-threshold#m
+00002080: 696e 696d 756d 0d0a 0d0a 2020 2020 5265  inimum....    Re
+00002090: 7475 726e 730d 0a20 2020 202d 2d2d 2d2d  turns..    -----
+000020a0: 2d2d 0d0a 2020 2020 6269 6e61 7279 5f69  --..    binary_i
+000020b0: 6d61 6765 3a20 6e61 7061 7269 2e74 7970  mage: napari.typ
+000020c0: 6573 2e4c 6162 656c 7344 6174 610d 0a20  es.LabelsData.. 
+000020d0: 2020 2022 2222 0d0a 2020 2020 7265 7475     """..    retu
+000020e0: 726e 2069 6d61 6765 203e 2066 696c 7465  rn image > filte
+000020f0: 7273 2e74 6872 6573 686f 6c64 5f6d 696e  rs.threshold_min
+00002100: 696d 756d 2869 6d61 6765 290d 0a0d 0a0d  imum(image).....
+00002110: 0a40 7265 6769 7374 6572 5f66 756e 6374  .@register_funct
+00002120: 696f 6e28 6d65 6e75 3d22 5365 676d 656e  ion(menu="Segmen
+00002130: 7461 7469 6f6e 202f 2062 696e 6172 697a  tation / binariz
+00002140: 6174 696f 6e20 3e20 5468 7265 7368 6f6c  ation > Threshol
+00002150: 6420 2854 7269 616e 676c 6520 6d65 7468  d (Triangle meth
+00002160: 6f64 2c20 5a61 636b 2065 7420 616c 2031  od, Zack et al 1
+00002170: 3937 372c 2073 6369 6b69 742d 696d 6167  977, scikit-imag
+00002180: 652c 206e 7362 6174 776d 2922 290d 0a40  e, nsbatwm)")..@
+00002190: 6a75 7079 7465 725f 6469 7370 6c61 7961  jupyter_displaya
+000021a0: 626c 655f 6f75 7470 7574 286c 6962 7261  ble_output(libra
+000021b0: 7279 5f6e 616d 653d 276e 7362 6174 776d  ry_name='nsbatwm
+000021c0: 272c 2068 656c 705f 7572 6c3d 2768 7474  ', help_url='htt
+000021d0: 7073 3a2f 2f77 7777 2e6e 6170 6172 692d  ps://www.napari-
+000021e0: 6875 622e 6f72 672f 706c 7567 696e 732f  hub.org/plugins/
+000021f0: 6e61 7061 7269 2d73 6567 6d65 6e74 2d62  napari-segment-b
+00002200: 6c6f 6273 2d61 6e64 2d74 6869 6e67 732d  lobs-and-things-
+00002210: 7769 7468 2d6d 656d 6272 616e 6573 2729  with-membranes')
+00002220: 0d0a 4074 696d 655f 736c 6963 6572 0d0a  ..@time_slicer..
+00002230: 6465 6620 7468 7265 7368 6f6c 645f 7472  def threshold_tr
+00002240: 6961 6e67 6c65 2869 6d61 6765 3a22 6e61  iangle(image:"na
+00002250: 7061 7269 2e74 7970 6573 2e49 6d61 6765  pari.types.Image
+00002260: 4461 7461 2229 202d 3e20 226e 6170 6172  Data") -> "napar
+00002270: 692e 7479 7065 732e 4c61 6265 6c73 4461  i.types.LabelsDa
+00002280: 7461 223a 0d0a 2020 2020 2222 220d 0a20  ta":..    """.. 
+00002290: 2020 2042 696e 6172 697a 6520 616e 2069     Binarize an i
+000022a0: 6d61 6765 2075 7369 6e67 2074 6865 2054  mage using the T
+000022b0: 7269 616e 676c 6520 6d65 7468 6f64 2e0d  riangle method..
+000022c0: 0a0d 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+000022d0: 730d 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  s..    ---------
+000022e0: 2d0d 0a20 2020 2069 6d61 6765 3a20 496d  -..    image: Im
+000022f0: 6167 650d 0a0d 0a20 2020 2053 6565 2041  age....    See A
+00002300: 6c73 6f0d 0a20 2020 202d 2d2d 2d2d 2d2d  lso..    -------
+00002310: 2d0d 0a20 2020 202e 2e5b 305d 2068 7474  -..    ..[0] htt
+00002320: 7073 3a2f 2f69 6d61 6765 6a2e 6e65 742f  ps://imagej.net/
+00002330: 706c 7567 696e 732f 6175 746f 2d74 6872  plugins/auto-thr
+00002340: 6573 686f 6c64 2374 7269 616e 676c 650d  eshold#triangle.
+00002350: 0a0d 0a20 2020 2052 6574 7572 6e73 0d0a  ...    Returns..
+00002360: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+00002370: 2062 696e 6172 795f 696d 6167 653a 206e   binary_image: n
+00002380: 6170 6172 692e 7479 7065 732e 4c61 6265  apari.types.Labe
+00002390: 6c73 4461 7461 0d0a 2020 2020 2222 220d  lsData..    """.
+000023a0: 0a20 2020 2072 6574 7572 6e20 696d 6167  .    return imag
+000023b0: 6520 3e20 6669 6c74 6572 732e 7468 7265  e > filters.thre
+000023c0: 7368 6f6c 645f 7472 6961 6e67 6c65 2869  shold_triangle(i
+000023d0: 6d61 6765 290d 0a0d 0a0d 0a40 7265 6769  mage)......@regi
+000023e0: 7374 6572 5f66 756e 6374 696f 6e28 6d65  ster_function(me
+000023f0: 6e75 3d22 4669 6c74 6572 696e 6720 2f20  nu="Filtering / 
+00002400: 6e6f 6973 6520 7265 6d6f 7661 6c20 3e20  noise removal > 
+00002410: 4761 7573 7369 616e 2028 7363 696b 6974  Gaussian (scikit
+00002420: 2d69 6d61 6765 2c20 6e73 6261 7477 6d29  -image, nsbatwm)
+00002430: 2229 0d0a 406a 7570 7974 6572 5f64 6973  ")..@jupyter_dis
+00002440: 706c 6179 6162 6c65 5f6f 7574 7075 7428  playable_output(
+00002450: 6c69 6272 6172 795f 6e61 6d65 3d27 6e73  library_name='ns
+00002460: 6261 7477 6d27 2c20 6865 6c70 5f75 726c  batwm', help_url
+00002470: 3d27 6874 7470 733a 2f2f 7777 772e 6e61  ='https://www.na
+00002480: 7061 7269 2d68 7562 2e6f 7267 2f70 6c75  pari-hub.org/plu
+00002490: 6769 6e73 2f6e 6170 6172 692d 7365 676d  gins/napari-segm
+000024a0: 656e 742d 626c 6f62 732d 616e 642d 7468  ent-blobs-and-th
+000024b0: 696e 6773 2d77 6974 682d 6d65 6d62 7261  ings-with-membra
+000024c0: 6e65 7327 290d 0a40 7469 6d65 5f73 6c69  nes')..@time_sli
+000024d0: 6365 720d 0a64 6566 2067 6175 7373 6961  cer..def gaussia
+000024e0: 6e5f 626c 7572 2869 6d61 6765 3a22 6e61  n_blur(image:"na
+000024f0: 7061 7269 2e74 7970 6573 2e49 6d61 6765  pari.types.Image
+00002500: 4461 7461 222c 2073 6967 6d61 3a20 666c  Data", sigma: fl
+00002510: 6f61 7420 3d20 3129 202d 3e20 226e 6170  oat = 1) -> "nap
+00002520: 6172 692e 7479 7065 732e 496d 6167 6544  ari.types.ImageD
+00002530: 6174 6122 3a0d 0a20 2020 2022 2222 0d0a  ata":..    """..
+00002540: 2020 2020 4170 706c 6965 7320 6120 4761      Applies a Ga
+00002550: 7573 7369 616e 2062 6c75 7220 746f 2061  ussian blur to a
+00002560: 6e20 696d 6167 6520 7769 7468 2061 2064  n image with a d
+00002570: 6566 696e 6564 2073 6967 6d61 2e20 5573  efined sigma. Us
+00002580: 6566 756c 2066 6f72 2064 656e 6f69 7369  eful for denoisi
+00002590: 6e67 2e0d 0a20 2020 2022 2222 0d0a 2020  ng...    """..  
+000025a0: 2020 7265 7475 726e 2067 6175 7373 6961    return gaussia
+000025b0: 6e28 696d 6167 652c 2073 6967 6d61 290d  n(image, sigma).
+000025c0: 0a0d 0a0d 0a40 7265 6769 7374 6572 5f66  .....@register_f
+000025d0: 756e 6374 696f 6e28 6d65 6e75 3d22 4669  unction(menu="Fi
+000025e0: 6c74 6572 696e 6720 2f20 6564 6765 2065  ltering / edge e
+000025f0: 6e68 616e 6365 6d65 6e74 203e 2047 6175  nhancement > Gau
+00002600: 7373 6961 6e20 4c61 706c 6163 6520 2873  ssian Laplace (s
+00002610: 6369 7079 2c20 6e73 6261 7477 6d29 2229  cipy, nsbatwm)")
+00002620: 0d0a 406a 7570 7974 6572 5f64 6973 706c  ..@jupyter_displ
+00002630: 6179 6162 6c65 5f6f 7574 7075 7428 6c69  ayable_output(li
+00002640: 6272 6172 795f 6e61 6d65 3d27 6e73 6261  brary_name='nsba
+00002650: 7477 6d27 2c20 6865 6c70 5f75 726c 3d27  twm', help_url='
+00002660: 6874 7470 733a 2f2f 7777 772e 6e61 7061  https://www.napa
+00002670: 7269 2d68 7562 2e6f 7267 2f70 6c75 6769  ri-hub.org/plugi
+00002680: 6e73 2f6e 6170 6172 692d 7365 676d 656e  ns/napari-segmen
+00002690: 742d 626c 6f62 732d 616e 642d 7468 696e  t-blobs-and-thin
+000026a0: 6773 2d77 6974 682d 6d65 6d62 7261 6e65  gs-with-membrane
+000026b0: 7327 290d 0a40 7469 6d65 5f73 6c69 6365  s')..@time_slice
+000026c0: 720d 0a64 6566 2067 6175 7373 6961 6e5f  r..def gaussian_
+000026d0: 6c61 706c 6163 6528 696d 6167 653a 226e  laplace(image:"n
+000026e0: 6170 6172 692e 7479 7065 732e 496d 6167  apari.types.Imag
+000026f0: 6544 6174 6122 2c20 7369 676d 613a 2066  eData", sigma: f
+00002700: 6c6f 6174 203d 2032 292d 3e20 226e 6170  loat = 2)-> "nap
+00002710: 6172 692e 7479 7065 732e 496d 6167 6544  ari.types.ImageD
+00002720: 6174 6122 3a0d 0a20 2020 2022 2222 0d0a  ata":..    """..
+00002730: 2020 2020 4170 706c 7920 4c61 706c 6163      Apply Laplac
+00002740: 6520 6669 6c74 6572 2066 6f72 2065 6467  e filter for edg
+00002750: 6520 6465 7465 6374 696f 6e20 2f20 6564  e detection / ed
+00002760: 6765 2065 6e68 616e 6365 6d65 6e74 2061  ge enhancement a
+00002770: 6674 6572 2061 7070 6c79 696e 6720 6120  fter applying a 
+00002780: 4761 7573 7369 616e 2d62 6c75 720d 0a0d  Gaussian-blur...
+00002790: 0a20 2020 2050 6172 616d 6574 6572 730d  .    Parameters.
+000027a0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d  .    ----------.
+000027b0: 0a20 2020 2069 6d61 6765 3a20 6172 7261  .    image: arra
+000027c0: 792d 6c69 6b65 0d0a 2020 2020 2020 2020  y-like..        
+000027d0: 496d 6167 6520 746f 2064 6574 6563 7420  Image to detect 
+000027e0: 6564 6765 7320 696e 0d0a 2020 2020 7369  edges in..    si
+000027f0: 676d 613a 2066 6c6f 6174 0d0a 2020 2020  gma: float..    
+00002800: 2020 2020 5468 6520 6669 6c74 6572 2077      The filter w
+00002810: 696c 6c20 6265 2061 7070 6c69 6564 2077  ill be applied w
+00002820: 6974 6820 7468 6973 2073 7065 6369 6669  ith this specifi
+00002830: 6564 2047 6175 7373 6961 6e2d 626c 7572  ed Gaussian-blur
+00002840: 2073 6967 6d61 0d0a 0d0a 2020 2020 5265   sigma....    Re
+00002850: 7475 726e 730d 0a20 2020 202d 2d2d 2d2d  turns..    -----
+00002860: 2d2d 0d0a 2020 2020 6172 7261 792d 6c69  --..    array-li
+00002870: 6b65 0d0a 0d0a 2020 2020 5365 6520 616c  ke....    See al
+00002880: 736f 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d  so..    --------
+00002890: 0d0a 2020 2020 2e2e 205b 315d 2068 7474  ..    .. [1] htt
+000028a0: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+000028b0: 612e 6f72 672f 7769 6b69 2f4c 6170 6c61  a.org/wiki/Lapla
+000028c0: 6365 5f6f 7065 7261 746f 720d 0a20 2020  ce_operator..   
+000028d0: 2022 2222 0d0a 2020 2020 7265 7475 726e   """..    return
+000028e0: 2073 6369 7079 2e6e 6469 6d61 6765 2e67   scipy.ndimage.g
+000028f0: 6175 7373 6961 6e5f 6c61 706c 6163 6528  aussian_laplace(
+00002900: 696d 6167 652e 6173 7479 7065 2866 6c6f  image.astype(flo
+00002910: 6174 292c 2073 6967 6d61 290d 0a0d 0a0d  at), sigma).....
+00002920: 0a40 7265 6769 7374 6572 5f66 756e 6374  .@register_funct
+00002930: 696f 6e28 6d65 6e75 3d22 4669 6c74 6572  ion(menu="Filter
+00002940: 696e 6720 2f20 6e6f 6973 6520 7265 6d6f  ing / noise remo
+00002950: 7661 6c20 3e20 4d65 6469 616e 2028 7363  val > Median (sc
+00002960: 6970 792c 206e 7362 6174 776d 2922 290d  ipy, nsbatwm)").
+00002970: 0a40 6a75 7079 7465 725f 6469 7370 6c61  .@jupyter_displa
+00002980: 7961 626c 655f 6f75 7470 7574 286c 6962  yable_output(lib
+00002990: 7261 7279 5f6e 616d 653d 276e 7362 6174  rary_name='nsbat
+000029a0: 776d 272c 2068 656c 705f 7572 6c3d 2768  wm', help_url='h
+000029b0: 7474 7073 3a2f 2f77 7777 2e6e 6170 6172  ttps://www.napar
+000029c0: 692d 6875 622e 6f72 672f 706c 7567 696e  i-hub.org/plugin
+000029d0: 732f 6e61 7061 7269 2d73 6567 6d65 6e74  s/napari-segment
+000029e0: 2d62 6c6f 6273 2d61 6e64 2d74 6869 6e67  -blobs-and-thing
+000029f0: 732d 7769 7468 2d6d 656d 6272 616e 6573  s-with-membranes
+00002a00: 2729 0d0a 4074 696d 655f 736c 6963 6572  ')..@time_slicer
+00002a10: 0d0a 6465 6620 6d65 6469 616e 5f66 696c  ..def median_fil
+00002a20: 7465 7228 696d 6167 653a 226e 6170 6172  ter(image:"napar
+00002a30: 692e 7479 7065 732e 496d 6167 6544 6174  i.types.ImageDat
+00002a40: 6122 2c20 7261 6469 7573 3a20 666c 6f61  a", radius: floa
+00002a50: 7420 3d20 3229 2d3e 2022 6e61 7061 7269  t = 2)-> "napari
+00002a60: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
+00002a70: 223a 0d0a 2020 2020 2222 220d 0a20 2020  ":..    """..   
+00002a80: 2054 6865 206d 6564 6961 6e2d 6669 6c74   The median-filt
+00002a90: 6572 2061 6c6c 6f77 7320 7265 6d6f 7669  er allows removi
+00002aa0: 6e67 206e 6f69 7365 2066 726f 6d20 696d  ng noise from im
+00002ab0: 6167 6573 2e20 5768 696c 6520 6c6f 6361  ages. While loca
+00002ac0: 6c6c 7920 6176 6572 6167 696e 6720 696e  lly averaging in
+00002ad0: 7465 6e73 6974 792c 2069 740d 0a20 2020  tensity, it..   
+00002ae0: 2069 7320 616e 2065 6467 652d 7072 6573   is an edge-pres
+00002af0: 6572 7669 6e67 2066 696c 7465 722e 0d0a  erving filter...
+00002b00: 0d0a 2020 2020 4974 2069 7320 6571 7561  ..    It is equa
+00002b10: 6c20 746f 2061 2070 6572 6365 6e74 696c  l to a percentil
+00002b20: 652d 6669 6c74 6572 2077 6974 6820 7065  e-filter with pe
+00002b30: 7263 656e 7469 6c65 3d3d 3530 2e0d 0a20  rcentile==50... 
+00002b40: 2020 2049 6e20 6361 7365 2061 7070 6c79     In case apply
+00002b50: 696e 6720 7468 6520 6669 6c74 6572 2074  ing the filter t
+00002b60: 616b 6573 2074 6f20 6d75 6368 2074 696d  akes to much tim
+00002b70: 652c 2063 6f6e 7369 6465 7220 7573 696e  e, consider usin
+00002b80: 6720 6120 4761 7573 7369 616e 2062 6c75  g a Gaussian blu
+00002b90: 7220 696e 7374 6561 642e 0d0a 2020 2020  r instead...    
+00002ba0: 2222 220d 0a20 2020 2072 6574 7572 6e20  """..    return 
+00002bb0: 7363 6970 792e 6e64 696d 6167 652e 6d65  scipy.ndimage.me
+00002bc0: 6469 616e 5f66 696c 7465 7228 696d 6167  dian_filter(imag
+00002bd0: 652e 6173 7479 7065 2866 6c6f 6174 292c  e.astype(float),
+00002be0: 2073 697a 653d 696e 7428 7261 6469 7573   size=int(radius
+00002bf0: 202a 2032 202b 2031 2929 0d0a 0d0a 0d0a   * 2 + 1))......
+00002c00: 4072 6567 6973 7465 725f 6675 6e63 7469  @register_functi
+00002c10: 6f6e 286d 656e 753d 2246 696c 7465 7269  on(menu="Filteri
+00002c20: 6e67 202f 206e 6f69 7365 2072 656d 6f76  ng / noise remov
+00002c30: 616c 203e 2050 6572 6365 6e74 696c 6520  al > Percentile 
+00002c40: 2873 6369 7079 2c20 6e73 6261 7477 6d29  (scipy, nsbatwm)
+00002c50: 2229 0d0a 406a 7570 7974 6572 5f64 6973  ")..@jupyter_dis
+00002c60: 706c 6179 6162 6c65 5f6f 7574 7075 7428  playable_output(
+00002c70: 6c69 6272 6172 795f 6e61 6d65 3d27 6e73  library_name='ns
+00002c80: 6261 7477 6d27 2c20 6865 6c70 5f75 726c  batwm', help_url
+00002c90: 3d27 6874 7470 733a 2f2f 7777 772e 6e61  ='https://www.na
+00002ca0: 7061 7269 2d68 7562 2e6f 7267 2f70 6c75  pari-hub.org/plu
+00002cb0: 6769 6e73 2f6e 6170 6172 692d 7365 676d  gins/napari-segm
+00002cc0: 656e 742d 626c 6f62 732d 616e 642d 7468  ent-blobs-and-th
+00002cd0: 696e 6773 2d77 6974 682d 6d65 6d62 7261  ings-with-membra
+00002ce0: 6e65 7327 290d 0a40 7469 6d65 5f73 6c69  nes')..@time_sli
+00002cf0: 6365 720d 0a64 6566 2070 6572 6365 6e74  cer..def percent
+00002d00: 696c 655f 6669 6c74 6572 2869 6d61 6765  ile_filter(image
+00002d10: 3a22 6e61 7061 7269 2e74 7970 6573 2e49  :"napari.types.I
+00002d20: 6d61 6765 4461 7461 222c 2070 6572 6365  mageData", perce
+00002d30: 6e74 696c 6520 3a20 666c 6f61 7420 3d20  ntile : float = 
+00002d40: 3530 2c20 7261 6469 7573 3a20 666c 6f61  50, radius: floa
+00002d50: 7420 3d20 3229 2d3e 2022 6e61 7061 7269  t = 2)-> "napari
+00002d60: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
+00002d70: 223a 0d0a 2020 2020 2222 2254 6865 2070  ":..    """The p
+00002d80: 6572 6365 6e74 696c 6520 6669 6c74 6572  ercentile filter
+00002d90: 2069 7320 7369 6d69 6c61 7220 746f 2074   is similar to t
+00002da0: 6865 206d 6564 6961 6e2d 6669 6c74 6572  he median-filter
+00002db0: 2062 7574 2069 7420 616c 6c6f 7773 2073   but it allows s
+00002dc0: 7065 6369 6679 696e 6720 7468 6520 7065  pecifying the pe
+00002dd0: 7263 656e 7469 6c65 2e0d 0a20 2020 2054  rcentile...    T
+00002de0: 6865 2070 6572 6365 6e74 696c 652d 6669  he percentile-fi
+00002df0: 6c74 6572 2077 6974 6820 7065 7263 656e  lter with percen
+00002e00: 7469 6c65 3d3d 3530 2069 7320 6571 7561  tile==50 is equa
+00002e10: 6c20 746f 2074 6865 206d 6564 6961 6e2d  l to the median-
+00002e20: 6669 6c74 6572 2e0d 0a20 2020 2022 2222  filter...    """
+00002e30: 0d0a 2020 2020 7265 7475 726e 2073 6369  ..    return sci
+00002e40: 7079 2e6e 6469 6d61 6765 2e70 6572 6365  py.ndimage.perce
+00002e50: 6e74 696c 655f 6669 6c74 6572 2869 6d61  ntile_filter(ima
+00002e60: 6765 2e61 7374 7970 6528 666c 6f61 7429  ge.astype(float)
+00002e70: 2c20 7065 7263 656e 7469 6c65 3d70 6572  , percentile=per
+00002e80: 6365 6e74 696c 652c 2073 697a 653d 696e  centile, size=in
+00002e90: 7428 7261 6469 7573 202a 2032 202b 2031  t(radius * 2 + 1
+00002ea0: 2929 0d0a 0d0a 0d0a 4072 6567 6973 7465  ))......@registe
+00002eb0: 725f 6675 6e63 7469 6f6e 286d 656e 753d  r_function(menu=
+00002ec0: 2246 696c 7465 7269 6e67 202f 2062 6163  "Filtering / bac
+00002ed0: 6b67 726f 756e 6420 7265 6d6f 7661 6c20  kground removal 
+00002ee0: 3e20 5768 6974 6520 746f 702d 6861 7420  > White top-hat 
+00002ef0: 2873 6369 7079 2c20 6e73 6261 7477 6d29  (scipy, nsbatwm)
+00002f00: 2229 0d0a 406a 7570 7974 6572 5f64 6973  ")..@jupyter_dis
+00002f10: 706c 6179 6162 6c65 5f6f 7574 7075 7428  playable_output(
+00002f20: 6c69 6272 6172 795f 6e61 6d65 3d27 6e73  library_name='ns
+00002f30: 6261 7477 6d27 2c20 6865 6c70 5f75 726c  batwm', help_url
+00002f40: 3d27 6874 7470 733a 2f2f 7777 772e 6e61  ='https://www.na
+00002f50: 7061 7269 2d68 7562 2e6f 7267 2f70 6c75  pari-hub.org/plu
+00002f60: 6769 6e73 2f6e 6170 6172 692d 7365 676d  gins/napari-segm
+00002f70: 656e 742d 626c 6f62 732d 616e 642d 7468  ent-blobs-and-th
+00002f80: 696e 6773 2d77 6974 682d 6d65 6d62 7261  ings-with-membra
+00002f90: 6e65 7327 290d 0a40 7469 6d65 5f73 6c69  nes')..@time_sli
+00002fa0: 6365 720d 0a64 6566 2077 6869 7465 5f74  cer..def white_t
+00002fb0: 6f70 6861 7428 696d 6167 653a 226e 6170  ophat(image:"nap
+00002fc0: 6172 692e 7479 7065 732e 496d 6167 6544  ari.types.ImageD
+00002fd0: 6174 6122 2c20 7261 6469 7573 3a20 666c  ata", radius: fl
+00002fe0: 6f61 7420 3d20 3229 2d3e 2022 6e61 7061  oat = 2)-> "napa
+00002ff0: 7269 2e74 7970 6573 2e49 6d61 6765 4461  ri.types.ImageDa
+00003000: 7461 223a 0d0a 2020 2020 2222 220d 0a20  ta":..    """.. 
+00003010: 2020 2054 6865 2077 6869 7465 2074 6f70     The white top
+00003020: 2d68 6174 2066 696c 7465 7220 7265 6d6f  -hat filter remo
+00003030: 7665 7320 6272 6967 6874 2072 6567 696f  ves bright regio
+00003040: 6e73 2066 726f 6d20 616e 2069 6d61 6765  ns from an image
+00003050: 2073 686f 7769 6e67 2062 6c61 636b 2069   showing black i
+00003060: 736c 616e 6473 2e0d 0a0d 0a20 2020 2049  slands.....    I
+00003070: 6e20 7468 6520 636f 6e74 6578 7420 6f66  n the context of
+00003080: 2066 6c75 6f72 6573 6365 6e63 6520 6d69   fluorescence mi
+00003090: 6372 6f73 636f 7079 2c20 6974 2061 6c6c  croscopy, it all
+000030a0: 6f77 7320 7265 6d6f 7669 6e67 2069 6e74  ows removing int
+000030b0: 656e 7369 7479 2072 6573 756c 7469 6e67  ensity resulting
+000030c0: 2066 726f 6d20 6f75 742d 6f66 2d66 6f63   from out-of-foc
+000030d0: 7573 206c 6967 6874 2e0d 0a20 2020 2022  us light...    "
+000030e0: 2222 0d0a 2020 2020 7265 7475 726e 2073  ""..    return s
+000030f0: 6369 7079 2e6e 6469 6d61 6765 2e77 6869  cipy.ndimage.whi
+00003100: 7465 5f74 6f70 6861 7428 696d 6167 652e  te_tophat(image.
+00003110: 6173 7479 7065 2866 6c6f 6174 292c 2073  astype(float), s
+00003120: 697a 653d 696e 7428 7261 6469 7573 202a  ize=int(radius *
+00003130: 2032 202b 2031 2929 0d0a 0d0a 0d0a 4072   2 + 1))......@r
+00003140: 6567 6973 7465 725f 6675 6e63 7469 6f6e  egister_function
+00003150: 286d 656e 753d 2246 696c 7465 7269 6e67  (menu="Filtering
+00003160: 202f 2062 6163 6b67 726f 756e 6420 7265   / background re
+00003170: 6d6f 7661 6c20 3e20 426c 6163 6b20 746f  moval > Black to
+00003180: 702d 6861 7420 2873 6369 7079 2c20 6e73  p-hat (scipy, ns
+00003190: 6261 7477 6d29 2229 0d0a 406a 7570 7974  batwm)")..@jupyt
+000031a0: 6572 5f64 6973 706c 6179 6162 6c65 5f6f  er_displayable_o
+000031b0: 7574 7075 7428 6c69 6272 6172 795f 6e61  utput(library_na
+000031c0: 6d65 3d27 6e73 6261 7477 6d27 2c20 6865  me='nsbatwm', he
+000031d0: 6c70 5f75 726c 3d27 6874 7470 733a 2f2f  lp_url='https://
+000031e0: 7777 772e 6e61 7061 7269 2d68 7562 2e6f  www.napari-hub.o
+000031f0: 7267 2f70 6c75 6769 6e73 2f6e 6170 6172  rg/plugins/napar
+00003200: 692d 7365 676d 656e 742d 626c 6f62 732d  i-segment-blobs-
+00003210: 616e 642d 7468 696e 6773 2d77 6974 682d  and-things-with-
+00003220: 6d65 6d62 7261 6e65 7327 290d 0a40 7469  membranes')..@ti
+00003230: 6d65 5f73 6c69 6365 720d 0a64 6566 2062  me_slicer..def b
+00003240: 6c61 636b 5f74 6f70 6861 7428 696d 6167  lack_tophat(imag
+00003250: 653a 226e 6170 6172 692e 7479 7065 732e  e:"napari.types.
+00003260: 496d 6167 6544 6174 6122 2c20 7261 6469  ImageData", radi
+00003270: 7573 3a20 666c 6f61 7420 3d20 3229 2d3e  us: float = 2)->
+00003280: 2022 6e61 7061 7269 2e74 7970 6573 2e49   "napari.types.I
+00003290: 6d61 6765 4461 7461 223a 0d0a 2020 2020  mageData":..    
+000032a0: 2222 220d 0a20 2020 2054 6865 2062 6c61  """..    The bla
+000032b0: 636b 2074 6f70 2d68 6174 2066 696c 7465  ck top-hat filte
+000032c0: 7220 7265 6d6f 7665 7320 6272 6967 6874  r removes bright
+000032d0: 2072 6567 696f 6e73 2066 726f 6d20 616e   regions from an
+000032e0: 2069 6d61 6765 2073 686f 7769 6e67 2062   image showing b
+000032f0: 6c61 636b 2069 736c 616e 6473 2e0d 0a20  lack islands... 
+00003300: 2020 2022 2222 0d0a 2020 2020 7265 7475     """..    retu
+00003310: 726e 2073 6369 7079 2e6e 6469 6d61 6765  rn scipy.ndimage
+00003320: 2e62 6c61 636b 5f74 6f70 6861 7428 696d  .black_tophat(im
+00003330: 6167 652e 6173 7479 7065 2866 6c6f 6174  age.astype(float
+00003340: 292c 2073 697a 653d 696e 7428 7261 6469  ), size=int(radi
+00003350: 7573 202a 2032 202b 2031 2929 0d0a 0d0a  us * 2 + 1))....
+00003360: 0d0a 4072 6567 6973 7465 725f 6675 6e63  ..@register_func
+00003370: 7469 6f6e 286d 656e 753d 2246 696c 7465  tion(menu="Filte
+00003380: 7269 6e67 202f 2062 6163 6b67 726f 756e  ring / backgroun
+00003390: 6420 7265 6d6f 7661 6c20 3e20 4d69 6e69  d removal > Mini
+000033a0: 6d75 6d20 2873 6369 7079 2c20 6e73 6261  mum (scipy, nsba
+000033b0: 7477 6d29 2229 0d0a 406a 7570 7974 6572  twm)")..@jupyter
+000033c0: 5f64 6973 706c 6179 6162 6c65 5f6f 7574  _displayable_out
+000033d0: 7075 7428 6c69 6272 6172 795f 6e61 6d65  put(library_name
+000033e0: 3d27 6e73 6261 7477 6d27 2c20 6865 6c70  ='nsbatwm', help
+000033f0: 5f75 726c 3d27 6874 7470 733a 2f2f 7777  _url='https://ww
+00003400: 772e 6e61 7061 7269 2d68 7562 2e6f 7267  w.napari-hub.org
+00003410: 2f70 6c75 6769 6e73 2f6e 6170 6172 692d  /plugins/napari-
+00003420: 7365 676d 656e 742d 626c 6f62 732d 616e  segment-blobs-an
+00003430: 642d 7468 696e 6773 2d77 6974 682d 6d65  d-things-with-me
+00003440: 6d62 7261 6e65 7327 290d 0a40 7469 6d65  mbranes')..@time
+00003450: 5f73 6c69 6365 720d 0a64 6566 206d 696e  _slicer..def min
+00003460: 696d 756d 5f66 696c 7465 7228 696d 6167  imum_filter(imag
+00003470: 653a 226e 6170 6172 692e 7479 7065 732e  e:"napari.types.
+00003480: 496d 6167 6544 6174 6122 2c20 7261 6469  ImageData", radi
+00003490: 7573 3a20 666c 6f61 7420 3d20 3229 2d3e  us: float = 2)->
+000034a0: 2022 6e61 7061 7269 2e74 7970 6573 2e49   "napari.types.I
+000034b0: 6d61 6765 4461 7461 223a 0d0a 2020 2020  mageData":..    
+000034c0: 2222 220d 0a20 2020 204c 6f63 616c 206d  """..    Local m
+000034d0: 696e 696d 756d 2066 696c 7465 720d 0a0d  inimum filter...
+000034e0: 0a20 2020 2043 616e 2062 6520 7573 6564  .    Can be used
+000034f0: 2066 6f72 206e 6f69 7365 2061 6e64 2062   for noise and b
+00003500: 6163 6b67 726f 756e 6420 7265 6d6f 7661  ackground remova
+00003510: 6c2e 0d0a 2020 2020 2222 220d 0a20 2020  l...    """..   
+00003520: 2072 6574 7572 6e20 7363 6970 792e 6e64   return scipy.nd
+00003530: 696d 6167 652e 6d69 6e69 6d75 6d5f 6669  image.minimum_fi
+00003540: 6c74 6572 2869 6d61 6765 2e61 7374 7970  lter(image.astyp
+00003550: 6528 666c 6f61 7429 2c20 7369 7a65 3d72  e(float), size=r
+00003560: 6164 6975 7320 2a20 3220 2b20 3129 0d0a  adius * 2 + 1)..
+00003570: 0d0a 0d0a 4072 6567 6973 7465 725f 6675  ....@register_fu
+00003580: 6e63 7469 6f6e 286d 656e 753d 2246 696c  nction(menu="Fil
+00003590: 7465 7269 6e67 202f 2062 6163 6b67 726f  tering / backgro
+000035a0: 756e 6420 7265 6d6f 7661 6c20 3e20 4d61  und removal > Ma
+000035b0: 7869 6d75 6d20 2873 6369 7079 2c20 6e73  ximum (scipy, ns
+000035c0: 6261 7477 6d29 2229 0d0a 406a 7570 7974  batwm)")..@jupyt
+000035d0: 6572 5f64 6973 706c 6179 6162 6c65 5f6f  er_displayable_o
+000035e0: 7574 7075 7428 6c69 6272 6172 795f 6e61  utput(library_na
+000035f0: 6d65 3d27 6e73 6261 7477 6d27 2c20 6865  me='nsbatwm', he
+00003600: 6c70 5f75 726c 3d27 6874 7470 733a 2f2f  lp_url='https://
+00003610: 7777 772e 6e61 7061 7269 2d68 7562 2e6f  www.napari-hub.o
+00003620: 7267 2f70 6c75 6769 6e73 2f6e 6170 6172  rg/plugins/napar
+00003630: 692d 7365 676d 656e 742d 626c 6f62 732d  i-segment-blobs-
+00003640: 616e 642d 7468 696e 6773 2d77 6974 682d  and-things-with-
+00003650: 6d65 6d62 7261 6e65 7327 290d 0a40 7469  membranes')..@ti
+00003660: 6d65 5f73 6c69 6365 720d 0a64 6566 206d  me_slicer..def m
+00003670: 6178 696d 756d 5f66 696c 7465 7228 696d  aximum_filter(im
+00003680: 6167 653a 226e 6170 6172 692e 7479 7065  age:"napari.type
+00003690: 732e 496d 6167 6544 6174 6122 2c20 7261  s.ImageData", ra
+000036a0: 6469 7573 3a20 666c 6f61 7420 3d20 3229  dius: float = 2)
+000036b0: 2d3e 2022 6e61 7061 7269 2e74 7970 6573  -> "napari.types
+000036c0: 2e49 6d61 6765 4461 7461 223a 0d0a 2020  .ImageData":..  
+000036d0: 2020 2222 220d 0a20 2020 204c 6f63 616c    """..    Local
+000036e0: 206d 6178 696d 756d 2066 696c 7465 720d   maximum filter.
+000036f0: 0a0d 0a20 2020 2049 6e20 7468 6520 636f  ...    In the co
+00003700: 6e74 6578 7420 6f66 2063 656c 6c20 7365  ntext of cell se
+00003710: 676d 656e 7461 7469 6f6e 2069 7420 6361  gmentation it ca
+00003720: 6e20 6265 2075 7365 6420 746f 206d 616b  n be used to mak
+00003730: 6520 6d65 6d62 7261 6e65 7320 7769 6465  e membranes wide
+00003740: 720d 0a20 2020 2061 6e64 2063 6c6f 7365  r..    and close
+00003750: 2073 6d61 6c6c 2067 6170 7320 6f66 2069   small gaps of i
+00003760: 6e73 7566 6669 6369 656e 7420 7374 6169  nsufficient stai
+00003770: 6e69 6e67 2e0d 0a20 2020 2022 2222 0d0a  ning...    """..
+00003780: 2020 2020 7265 7475 726e 2073 6369 7079      return scipy
+00003790: 2e6e 6469 6d61 6765 2e6d 6178 696d 756d  .ndimage.maximum
+000037a0: 5f66 696c 7465 7228 696d 6167 652e 6173  _filter(image.as
+000037b0: 7479 7065 2866 6c6f 6174 292c 2073 697a  type(float), siz
+000037c0: 653d 7261 6469 7573 202a 2032 202b 2031  e=radius * 2 + 1
+000037d0: 290d 0a0d 0a0d 0a40 7265 6769 7374 6572  )......@register
+000037e0: 5f66 756e 6374 696f 6e28 6d65 6e75 3d22  _function(menu="
+000037f0: 4669 6c74 6572 696e 6720 2f20 6564 6765  Filtering / edge
+00003800: 2065 6e68 616e 6365 6d65 6e74 203e 204d   enhancement > M
+00003810: 6f72 7068 6f6c 6f67 6963 616c 2047 7261  orphological Gra
+00003820: 6469 656e 7420 2873 6369 7079 2c20 6e73  dient (scipy, ns
+00003830: 6261 7477 6d29 2229 0d0a 406a 7570 7974  batwm)")..@jupyt
+00003840: 6572 5f64 6973 706c 6179 6162 6c65 5f6f  er_displayable_o
+00003850: 7574 7075 7428 6c69 6272 6172 795f 6e61  utput(library_na
+00003860: 6d65 3d27 6e73 6261 7477 6d27 2c20 6865  me='nsbatwm', he
+00003870: 6c70 5f75 726c 3d27 6874 7470 733a 2f2f  lp_url='https://
+00003880: 7777 772e 6e61 7061 7269 2d68 7562 2e6f  www.napari-hub.o
+00003890: 7267 2f70 6c75 6769 6e73 2f6e 6170 6172  rg/plugins/napar
+000038a0: 692d 7365 676d 656e 742d 626c 6f62 732d  i-segment-blobs-
+000038b0: 616e 642d 7468 696e 6773 2d77 6974 682d  and-things-with-
+000038c0: 6d65 6d62 7261 6e65 7327 290d 0a40 7469  membranes')..@ti
+000038d0: 6d65 5f73 6c69 6365 720d 0a64 6566 206d  me_slicer..def m
+000038e0: 6f72 7068 6f6c 6f67 6963 616c 5f67 7261  orphological_gra
+000038f0: 6469 656e 7428 696d 6167 653a 226e 6170  dient(image:"nap
+00003900: 6172 692e 7479 7065 732e 496d 6167 6544  ari.types.ImageD
+00003910: 6174 6122 2c20 7261 6469 7573 3a20 666c  ata", radius: fl
+00003920: 6f61 7420 3d20 3229 2d3e 2022 6e61 7061  oat = 2)-> "napa
+00003930: 7269 2e74 7970 6573 2e49 6d61 6765 4461  ri.types.ImageDa
+00003940: 7461 223a 0d0a 2020 2020 2222 220d 0a20  ta":..    """.. 
+00003950: 2020 2041 7070 6c79 2067 7261 6469 656e     Apply gradien
+00003960: 7420 6669 6c74 6572 2028 7369 6d69 6c61  t filter (simila
+00003970: 7220 746f 2074 6865 2053 6f62 656c 206f  r to the Sobel o
+00003980: 7065 7261 746f 7229 2066 6f72 2065 6467  perator) for edg
+00003990: 6520 6465 7465 6374 696f 6e20 2f20 6564  e detection / ed
+000039a0: 6765 2065 6e68 616e 6365 6d65 6e74 2e0d  ge enhancement..
+000039b0: 0a20 2020 2054 6869 7320 6973 2073 696d  .    This is sim
+000039c0: 696c 6172 2074 6f20 6170 706c 7969 6e67  ilar to applying
+000039d0: 2061 2047 6175 7373 6961 6e2d 626c 7572   a Gaussian-blur
+000039e0: 2074 6f20 616e 2069 6d61 6765 2061 6e64   to an image and
+000039f0: 2061 6674 6572 7761 7264 7320 7468 6520   afterwards the 
+00003a00: 6772 6164 6965 6e74 206f 7065 7261 746f  gradient operato
+00003a10: 720d 0a0d 0a20 2020 2050 6172 616d 6574  r....    Paramet
+00003a20: 6572 730d 0a20 2020 202d 2d2d 2d2d 2d2d  ers..    -------
+00003a30: 2d2d 2d0d 0a20 2020 2069 6d61 6765 3a20  ---..    image: 
+00003a40: 6172 7261 792d 6c69 6b65 0d0a 2020 2020  array-like..    
+00003a50: 2020 2020 496d 6167 6520 746f 2064 6574      Image to det
+00003a60: 6563 7420 6564 6765 7320 696e 0d0a 2020  ect edges in..  
+00003a70: 2020 7261 6469 7573 3a20 666c 6f61 740d    radius: float.
+00003a80: 0a20 2020 2020 2020 2054 6865 2066 696c  .        The fil
+00003a90: 7465 7220 7769 6c6c 2062 6520 6170 706c  ter will be appl
+00003aa0: 6965 6420 7769 7468 2061 206b 6572 6e65  ied with a kerne
+00003ab0: 6c20 7369 7a65 206f 6620 2872 6164 6975  l size of (radiu
+00003ac0: 7320 2a20 3220 2b20 3129 0d0a 0d0a 2020  s * 2 + 1)....  
+00003ad0: 2020 5265 7475 726e 730d 0a20 2020 202d    Returns..    -
+00003ae0: 2d2d 2d2d 2d2d 0d0a 2020 2020 6172 7261  ------..    arra
+00003af0: 792d 6c69 6b65 0d0a 0d0a 2020 2020 5365  y-like....    Se
+00003b00: 6520 616c 736f 0d0a 2020 2020 2d2d 2d2d  e also..    ----
+00003b10: 2d2d 2d2d 0d0a 2020 2020 2e2e 205b 315d  ----..    .. [1]
+00003b20: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
+00003b30: 7065 6469 612e 6f72 672f 7769 6b69 2f4d  pedia.org/wiki/M
+00003b40: 6f72 7068 6f6c 6f67 6963 616c 5f67 7261  orphological_gra
+00003b50: 6469 656e 740d 0a20 2020 2022 2222 0d0a  dient..    """..
+00003b60: 2020 2020 7265 7475 726e 2073 6369 7079      return scipy
+00003b70: 2e6e 6469 6d61 6765 2e6d 6f72 7068 6f6c  .ndimage.morphol
+00003b80: 6f67 6963 616c 5f67 7261 6469 656e 7428  ogical_gradient(
+00003b90: 696d 6167 652e 6173 7479 7065 2866 6c6f  image.astype(flo
+00003ba0: 6174 292c 2073 697a 653d 696e 7428 7261  at), size=int(ra
+00003bb0: 6469 7573 202a 2032 202b 2031 2929 0d0a  dius * 2 + 1))..
+00003bc0: 0d0a 0d0a 4072 6567 6973 7465 725f 6675  ....@register_fu
+00003bd0: 6e63 7469 6f6e 286d 656e 753d 2246 696c  nction(menu="Fil
+00003be0: 7465 7269 6e67 202f 2062 6163 6b67 726f  tering / backgro
+00003bf0: 756e 6420 7265 6d6f 7661 6c20 3e20 526f  und removal > Ro
+00003c00: 6c6c 696e 6720 6261 6c6c 2028 7363 696b  lling ball (scik
+00003c10: 6974 2d69 6d61 6765 2c20 6e73 6261 7477  it-image, nsbatw
+00003c20: 6d29 2229 0d0a 406a 7570 7974 6572 5f64  m)")..@jupyter_d
+00003c30: 6973 706c 6179 6162 6c65 5f6f 7574 7075  isplayable_outpu
+00003c40: 7428 6c69 6272 6172 795f 6e61 6d65 3d27  t(library_name='
+00003c50: 6e73 6261 7477 6d27 2c20 6865 6c70 5f75  nsbatwm', help_u
+00003c60: 726c 3d27 6874 7470 733a 2f2f 7777 772e  rl='https://www.
+00003c70: 6e61 7061 7269 2d68 7562 2e6f 7267 2f70  napari-hub.org/p
+00003c80: 6c75 6769 6e73 2f6e 6170 6172 692d 7365  lugins/napari-se
+00003c90: 676d 656e 742d 626c 6f62 732d 616e 642d  gment-blobs-and-
+00003ca0: 7468 696e 6773 2d77 6974 682d 6d65 6d62  things-with-memb
+00003cb0: 7261 6e65 7327 290d 0a40 7469 6d65 5f73  ranes')..@time_s
+00003cc0: 6c69 6365 720d 0a64 6566 2073 7562 7472  licer..def subtr
+00003cd0: 6163 745f 6261 636b 6772 6f75 6e64 2869  act_background(i
+00003ce0: 6d61 6765 3a22 6e61 7061 7269 2e74 7970  mage:"napari.typ
+00003cf0: 6573 2e49 6d61 6765 4461 7461 222c 2072  es.ImageData", r
+00003d00: 6f6c 6c69 6e67 5f62 616c 6c5f 7261 6469  olling_ball_radi
+00003d10: 7573 3a20 666c 6f61 7420 3d20 3529 202d  us: float = 5) -
+00003d20: 3e20 226e 6170 6172 692e 7479 7065 732e  > "napari.types.
+00003d30: 496d 6167 6544 6174 6122 3a0d 0a20 2020  ImageData":..   
+00003d40: 2022 2222 0d0a 2020 2020 5375 6274 7261   """..    Subtra
+00003d50: 6374 2062 6163 6b67 726f 756e 6420 696e  ct background in
+00003d60: 2061 6e20 696d 6167 6520 7573 696e 6720   an image using 
+00003d70: 7468 6520 726f 6c6c 696e 672d 6261 6c6c  the rolling-ball
+00003d80: 2061 6c67 6f72 6974 686d 2e0d 0a0d 0a20   algorithm..... 
+00003d90: 2020 2053 6565 2061 6c73 6f0d 0a20 2020     See also..   
+00003da0: 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020 202e   --------..    .
+00003db0: 2e5b 305d 2068 7474 7073 3a2f 2f73 6369  .[0] https://sci
+00003dc0: 6b69 742d 696d 6167 652e 6f72 672f 646f  kit-image.org/do
+00003dd0: 6373 2f73 7461 626c 652f 6175 746f 5f65  cs/stable/auto_e
+00003de0: 7861 6d70 6c65 732f 7365 676d 656e 7461  xamples/segmenta
+00003df0: 7469 6f6e 2f70 6c6f 745f 726f 6c6c 696e  tion/plot_rollin
+00003e00: 675f 6261 6c6c 2e68 746d 6c0d 0a20 2020  g_ball.html..   
+00003e10: 2022 2222 0d0a 2020 2020 6261 636b 6772   """..    backgr
+00003e20: 6f75 6e64 203d 2072 6f6c 6c69 6e67 5f62  ound = rolling_b
+00003e30: 616c 6c28 696d 6167 652c 2072 6164 6975  all(image, radiu
+00003e40: 7320 3d20 726f 6c6c 696e 675f 6261 6c6c  s = rolling_ball
+00003e50: 5f72 6164 6975 7329 0d0a 2020 2020 7265  _radius)..    re
+00003e60: 7475 726e 2069 6d61 6765 202d 2062 6163  turn image - bac
+00003e70: 6b67 726f 756e 640d 0a0d 0a0d 0a40 7265  kground......@re
+00003e80: 6769 7374 6572 5f66 756e 6374 696f 6e28  gister_function(
+00003e90: 6d65 6e75 3d22 5365 676d 656e 7461 7469  menu="Segmentati
+00003ea0: 6f6e 2070 6f73 742d 7072 6f63 6573 7369  on post-processi
+00003eb0: 6e67 203e 2049 6e76 6572 7420 6269 6e61  ng > Invert bina
+00003ec0: 7279 2069 6d61 6765 2028 6e73 6261 7477  ry image (nsbatw
+00003ed0: 6d29 2229 0d0a 406a 7570 7974 6572 5f64  m)")..@jupyter_d
+00003ee0: 6973 706c 6179 6162 6c65 5f6f 7574 7075  isplayable_outpu
+00003ef0: 7428 6c69 6272 6172 795f 6e61 6d65 3d27  t(library_name='
+00003f00: 6e73 6261 7477 6d27 2c20 6865 6c70 5f75  nsbatwm', help_u
+00003f10: 726c 3d27 6874 7470 733a 2f2f 7777 772e  rl='https://www.
+00003f20: 6e61 7061 7269 2d68 7562 2e6f 7267 2f70  napari-hub.org/p
+00003f30: 6c75 6769 6e73 2f6e 6170 6172 692d 7365  lugins/napari-se
+00003f40: 676d 656e 742d 626c 6f62 732d 616e 642d  gment-blobs-and-
+00003f50: 7468 696e 6773 2d77 6974 682d 6d65 6d62  things-with-memb
+00003f60: 7261 6e65 7327 290d 0a40 7469 6d65 5f73  ranes')..@time_s
+00003f70: 6c69 6365 720d 0a64 6566 2062 696e 6172  licer..def binar
+00003f80: 795f 696e 7665 7274 2862 696e 6172 795f  y_invert(binary_
+00003f90: 696d 6167 653a 226e 6170 6172 692e 7479  image:"napari.ty
+00003fa0: 7065 732e 4c61 6265 6c73 4461 7461 2229  pes.LabelsData")
+00003fb0: 202d 3e20 226e 6170 6172 692e 7479 7065   -> "napari.type
+00003fc0: 732e 4c61 6265 6c73 4461 7461 223a 0d0a  s.LabelsData":..
+00003fd0: 2020 2020 2222 220d 0a20 2020 2049 6e76      """..    Inv
+00003fe0: 6572 7473 2061 2062 696e 6172 7920 696d  erts a binary im
+00003ff0: 6167 652e 0d0a 2020 2020 2222 220d 0a20  age...    """.. 
+00004000: 2020 2072 6574 7572 6e20 286e 702e 6173     return (np.as
+00004010: 6172 7261 7928 6269 6e61 7279 5f69 6d61  array(binary_ima
+00004020: 6765 2920 3d3d 2030 2920 2a20 310d 0a0d  ge) == 0) * 1...
+00004030: 0a0d 0a40 7265 6769 7374 6572 5f66 756e  ...@register_fun
+00004040: 6374 696f 6e28 6d65 6e75 3d22 5365 676d  ction(menu="Segm
+00004050: 656e 7461 7469 6f6e 202f 206c 6162 656c  entation / label
+00004060: 696e 6720 3e20 436f 6e6e 6563 7465 6420  ing > Connected 
+00004070: 636f 6d70 6f6e 656e 7420 6c61 6265 6c69  component labeli
+00004080: 6e67 2028 7363 696b 6974 2d69 6d61 6765  ng (scikit-image
+00004090: 2c20 6e73 6261 7477 6d29 2229 0d0a 406a  , nsbatwm)")..@j
+000040a0: 7570 7974 6572 5f64 6973 706c 6179 6162  upyter_displayab
+000040b0: 6c65 5f6f 7574 7075 7428 6c69 6272 6172  le_output(librar
+000040c0: 795f 6e61 6d65 3d27 6e73 6261 7477 6d27  y_name='nsbatwm'
+000040d0: 2c20 6865 6c70 5f75 726c 3d27 6874 7470  , help_url='http
+000040e0: 733a 2f2f 7777 772e 6e61 7061 7269 2d68  s://www.napari-h
+000040f0: 7562 2e6f 7267 2f70 6c75 6769 6e73 2f6e  ub.org/plugins/n
+00004100: 6170 6172 692d 7365 676d 656e 742d 626c  apari-segment-bl
+00004110: 6f62 732d 616e 642d 7468 696e 6773 2d77  obs-and-things-w
+00004120: 6974 682d 6d65 6d62 7261 6e65 7327 290d  ith-membranes').
+00004130: 0a40 7469 6d65 5f73 6c69 6365 720d 0a64  .@time_slicer..d
+00004140: 6566 2063 6f6e 6e65 6374 6564 5f63 6f6d  ef connected_com
+00004150: 706f 6e65 6e74 5f6c 6162 656c 696e 6728  ponent_labeling(
+00004160: 6269 6e61 7279 5f69 6d61 6765 3a20 226e  binary_image: "n
+00004170: 6170 6172 692e 7479 7065 732e 4c61 6265  apari.types.Labe
+00004180: 6c73 4461 7461 222c 2065 7863 6c75 6465  lsData", exclude
+00004190: 5f6f 6e5f 6564 6765 733a 2062 6f6f 6c20  _on_edges: bool 
+000041a0: 3d20 4661 6c73 6529 202d 3e20 226e 6170  = False) -> "nap
+000041b0: 6172 692e 7479 7065 732e 4c61 6265 6c73  ari.types.Labels
+000041c0: 4461 7461 223a 0d0a 2020 2020 2222 220d  Data":..    """.
+000041d0: 0a20 2020 2054 616b 6573 2061 2062 696e  .    Takes a bin
+000041e0: 6172 7920 696d 6167 6520 616e 6420 7072  ary image and pr
+000041f0: 6f64 7563 6573 2061 206c 6162 656c 2069  oduces a label i
+00004200: 6d61 6765 2077 6974 6820 616c 6c20 7365  mage with all se
+00004210: 7061 7261 7465 6420 6f62 6a65 6374 7320  parated objects 
+00004220: 6c61 6265 6c65 6420 7769 7468 0d0a 2020  labeled with..  
+00004230: 2020 6469 6666 6572 656e 7420 696e 7465    different inte
+00004240: 6765 7220 6e75 6d62 6572 732e 0d0a 0d0a  ger numbers.....
+00004250: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
+00004260: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00004270: 2020 2020 6578 636c 7564 655f 6f6e 5f65      exclude_on_e
+00004280: 6467 6573 203a 2062 6f6f 6c2c 206f 7074  dges : bool, opt
+00004290: 696f 6e61 6c0d 0a20 2020 2020 2020 2057  ional..        W
+000042a0: 6865 7468 6572 206f 7220 6e6f 7420 746f  hether or not to
+000042b0: 2063 6c65 6172 206f 626a 6563 7473 2063   clear objects c
+000042c0: 6f6e 6e65 6374 6564 2074 6f20 7468 6520  onnected to the 
+000042d0: 6c61 6265 6c20 696d 6167 6520 626f 7264  label image bord
+000042e0: 6572 2f70 6c61 6e65 7320 2865 6974 6865  er/planes (eithe
+000042f0: 7220 7879 2c20 787a 206f 7220 797a 292e  r xy, xz or yz).
+00004300: 0d0a 2020 2020 2222 220d 0a20 2020 2069  ..    """..    i
+00004310: 6620 6578 636c 7564 655f 6f6e 5f65 6467  f exclude_on_edg
+00004320: 6573 3a0d 0a20 2020 2020 2020 2023 2070  es:..        # p
+00004330: 726f 6365 7373 696e 6720 7468 6520 696d  rocessing the im
+00004340: 6167 652c 2077 6869 6368 2069 7320 6e6f  age, which is no
+00004350: 7420 6120 7469 6d65 6c61 7073 650d 0a20  t a timelapse.. 
+00004360: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00004370: 6d6f 7665 5f6c 6162 656c 735f 6f6e 5f65  move_labels_on_e
+00004380: 6467 6573 286c 6162 656c 286e 702e 6173  dges(label(np.as
+00004390: 6172 7261 7928 6269 6e61 7279 5f69 6d61  array(binary_ima
+000043a0: 6765 2929 290d 0a0d 0a20 2020 2065 6c73  ge)))....    els
+000043b0: 653a 0d0a 2020 2020 2020 2020 7265 7475  e:..        retu
+000043c0: 726e 206c 6162 656c 286e 702e 6173 6172  rn label(np.asar
+000043d0: 7261 7928 6269 6e61 7279 5f69 6d61 6765  ray(binary_image
+000043e0: 2929 0d0a 0d0a 0d0a 4072 6567 6973 7465  ))......@registe
+000043f0: 725f 6675 6e63 7469 6f6e 286d 656e 753d  r_function(menu=
+00004400: 2253 6567 6d65 6e74 6174 696f 6e20 706f  "Segmentation po
+00004410: 7374 2d70 726f 6365 7373 696e 6720 3e20  st-processing > 
+00004420: 5265 6d6f 7665 206c 6162 656c 6564 206f  Remove labeled o
+00004430: 626a 6563 7473 2061 7420 7468 6520 696d  bjects at the im
+00004440: 6167 6520 626f 7264 6572 2028 7363 696b  age border (scik
+00004450: 6974 2d69 6d61 6765 2c20 6e73 6261 7477  it-image, nsbatw
+00004460: 6d29 2229 0d0a 406a 7570 7974 6572 5f64  m)")..@jupyter_d
+00004470: 6973 706c 6179 6162 6c65 5f6f 7574 7075  isplayable_outpu
+00004480: 7428 6c69 6272 6172 795f 6e61 6d65 3d27  t(library_name='
+00004490: 6e73 6261 7477 6d27 2c20 6865 6c70 5f75  nsbatwm', help_u
+000044a0: 726c 3d27 6874 7470 733a 2f2f 7777 772e  rl='https://www.
+000044b0: 6e61 7061 7269 2d68 7562 2e6f 7267 2f70  napari-hub.org/p
+000044c0: 6c75 6769 6e73 2f6e 6170 6172 692d 7365  lugins/napari-se
+000044d0: 676d 656e 742d 626c 6f62 732d 616e 642d  gment-blobs-and-
+000044e0: 7468 696e 6773 2d77 6974 682d 6d65 6d62  things-with-memb
+000044f0: 7261 6e65 7327 290d 0a40 7469 6d65 5f73  ranes')..@time_s
+00004500: 6c69 6365 720d 0a64 6566 2072 656d 6f76  licer..def remov
+00004510: 655f 6c61 6265 6c73 5f6f 6e5f 6564 6765  e_labels_on_edge
+00004520: 7328 6c61 6265 6c5f 696d 6167 653a 2022  s(label_image: "
+00004530: 6e61 7061 7269 2e74 7970 6573 2e4c 6162  napari.types.Lab
+00004540: 656c 7344 6174 6122 2920 2d3e 2022 6e61  elsData") -> "na
+00004550: 7061 7269 2e74 7970 6573 2e4c 6162 656c  pari.types.Label
+00004560: 7344 6174 6122 3a0d 0a20 2020 2022 2222  sData":..    """
+00004570: 0d0a 2020 2020 5461 6b65 7320 6120 6c61  ..    Takes a la
+00004580: 6265 6c20 696d 6167 6520 616e 6420 7265  bel image and re
+00004590: 6d6f 7665 7320 6f62 6a65 6374 7320 7468  moves objects th
+000045a0: 6174 2074 6f75 6368 2074 6865 2069 6d61  at touch the ima
+000045b0: 6765 2062 6f72 6465 722e 0d0a 2020 2020  ge border...    
+000045c0: 5468 6520 7265 6d61 696e 696e 6720 6c61  The remaining la
+000045d0: 6265 6c73 2061 7265 2072 656c 6162 656c  bels are relabel
+000045e0: 6564 2073 6571 7565 6e74 6961 6c6c 792e  ed sequentially.
+000045f0: 0d0a 0d0a 2020 2020 5365 6520 616c 736f  ....    See also
+00004600: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a  ..    --------..
+00004610: 2020 2020 2e2e 5b30 5d20 6874 7470 733a      ..[0] https:
+00004620: 2f2f 7363 696b 6974 2d69 6d61 6765 2e6f  //scikit-image.o
+00004630: 7267 2f64 6f63 732f 7374 6162 6c65 2f61  rg/docs/stable/a
+00004640: 7069 2f73 6b69 6d61 6765 2e73 6567 6d65  pi/skimage.segme
+00004650: 6e74 6174 696f 6e2e 6874 6d6c 2373 6b69  ntation.html#ski
+00004660: 6d61 6765 2e73 6567 6d65 6e74 6174 696f  mage.segmentatio
+00004670: 6e2e 636c 6561 725f 626f 7264 6572 0d0a  n.clear_border..
+00004680: 2020 2020 2222 220d 0a0d 0a20 2020 2072      """....    r
+00004690: 6573 756c 7420 3d20 636c 6561 725f 626f  esult = clear_bo
+000046a0: 7264 6572 286e 702e 6173 6172 7261 7928  rder(np.asarray(
+000046b0: 6c61 6265 6c5f 696d 6167 6529 290d 0a20  label_image)).. 
+000046c0: 2020 2072 656c 6162 656c 6564 5f72 6573     relabeled_res
+000046d0: 756c 742c 205f 2c20 5f20 3d20 736b 5f72  ult, _, _ = sk_r
+000046e0: 656c 6162 656c 5f73 6571 7565 6e74 6961  elabel_sequentia
+000046f0: 6c28 7265 7375 6c74 290d 0a20 2020 2072  l(result)..    r
+00004700: 6574 7572 6e20 7265 6c61 6265 6c65 645f  eturn relabeled_
+00004710: 7265 7375 6c74 0d0a 0d0a 0d0a 4072 6567  result......@reg
+00004720: 6973 7465 725f 6675 6e63 7469 6f6e 286d  ister_function(m
+00004730: 656e 753d 2253 6567 6d65 6e74 6174 696f  enu="Segmentatio
+00004740: 6e20 706f 7374 2d70 726f 6365 7373 696e  n post-processin
+00004750: 6720 3e20 4578 7061 6e64 206c 6162 656c  g > Expand label
+00004760: 7320 2873 6369 6b69 742d 696d 6167 652c  s (scikit-image,
+00004770: 206e 7362 6174 776d 2922 290d 0a40 6a75   nsbatwm)")..@ju
+00004780: 7079 7465 725f 6469 7370 6c61 7961 626c  pyter_displayabl
+00004790: 655f 6f75 7470 7574 286c 6962 7261 7279  e_output(library
+000047a0: 5f6e 616d 653d 276e 7362 6174 776d 272c  _name='nsbatwm',
+000047b0: 2068 656c 705f 7572 6c3d 2768 7474 7073   help_url='https
+000047c0: 3a2f 2f77 7777 2e6e 6170 6172 692d 6875  ://www.napari-hu
+000047d0: 622e 6f72 672f 706c 7567 696e 732f 6e61  b.org/plugins/na
+000047e0: 7061 7269 2d73 6567 6d65 6e74 2d62 6c6f  pari-segment-blo
+000047f0: 6273 2d61 6e64 2d74 6869 6e67 732d 7769  bs-and-things-wi
+00004800: 7468 2d6d 656d 6272 616e 6573 2729 0d0a  th-membranes')..
+00004810: 4074 696d 655f 736c 6963 6572 0d0a 6465  @time_slicer..de
+00004820: 6620 6578 7061 6e64 5f6c 6162 656c 7328  f expand_labels(
+00004830: 6c61 6265 6c5f 696d 6167 653a 2022 6e61  label_image: "na
+00004840: 7061 7269 2e74 7970 6573 2e4c 6162 656c  pari.types.Label
+00004850: 7344 6174 6122 2c20 6469 7374 616e 6365  sData", distance
+00004860: 3a20 666c 6f61 7420 3d20 3129 202d 3e20  : float = 1) -> 
+00004870: 226e 6170 6172 692e 7479 7065 732e 4c61  "napari.types.La
+00004880: 6265 6c73 4461 7461 223a 0d0a 2020 2020  belsData":..    
+00004890: 2222 220d 0a20 2020 2054 616b 6573 2061  """..    Takes a
+000048a0: 206c 6162 656c 2069 6d61 6765 2061 6e64   label image and
+000048b0: 206d 616b 6573 206c 6162 656c 7320 6c61   makes labels la
+000048c0: 7267 6572 2075 7020 746f 2061 2067 6976  rger up to a giv
+000048d0: 656e 2072 6164 6975 7320 2864 6973 7461  en radius (dista
+000048e0: 6e63 6529 2e0d 0a20 2020 204c 6162 656c  nce)...    Label
+000048f0: 7320 7769 6c6c 206e 6f74 206f 7665 7277  s will not overw
+00004900: 7269 7465 2065 6163 6820 6f74 6865 7220  rite each other 
+00004910: 7768 696c 6520 6578 7061 6e64 696e 672e  while expanding.
+00004920: 2054 6869 7320 6f70 6572 6174 696f 6e20   This operation 
+00004930: 6973 2061 6c73 6f20 6b6e 6f77 6e20 6173  is also known as
+00004940: 206c 6162 656c 2064 696c 6174 696f 6e2e   label dilation.
+00004950: 0d0a 0d0a 2020 2020 5365 6520 616c 736f  ....    See also
+00004960: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a  ..    --------..
+00004970: 2020 2020 2e2e 5b30 5d20 6874 7470 733a      ..[0] https:
+00004980: 2f2f 7363 696b 6974 2d69 6d61 6765 2e6f  //scikit-image.o
+00004990: 7267 2f64 6f63 732f 7374 6162 6c65 2f61  rg/docs/stable/a
+000049a0: 7069 2f73 6b69 6d61 6765 2e73 6567 6d65  pi/skimage.segme
+000049b0: 6e74 6174 696f 6e2e 6874 6d6c 2373 6b69  ntation.html#ski
+000049c0: 6d61 6765 2e73 6567 6d65 6e74 6174 696f  mage.segmentatio
+000049d0: 6e2e 6578 7061 6e64 5f6c 6162 656c 730d  n.expand_labels.
+000049e0: 0a20 2020 2022 2222 0d0a 0d0a 2020 2020  .    """....    
+000049f0: 7265 7475 726e 2073 6b5f 6578 7061 6e64  return sk_expand
+00004a00: 5f6c 6162 656c 7328 6e70 2e61 7361 7272  _labels(np.asarr
+00004a10: 6179 286c 6162 656c 5f69 6d61 6765 292c  ay(label_image),
+00004a20: 2064 6973 7461 6e63 653d 6469 7374 616e   distance=distan
+00004a30: 6365 290d 0a0d 0a0d 0a40 7265 6769 7374  ce)......@regist
+00004a40: 6572 5f66 756e 6374 696f 6e28 6d65 6e75  er_function(menu
+00004a50: 3d22 5365 676d 656e 7461 7469 6f6e 202f  ="Segmentation /
+00004a60: 206c 6162 656c 696e 6720 3e20 566f 726f   labeling > Voro
+00004a70: 6e6f 692d 4f74 7375 2d6c 6162 656c 696e  noi-Otsu-labelin
+00004a80: 6720 286e 7362 6174 776d 2922 290d 0a40  g (nsbatwm)")..@
+00004a90: 6a75 7079 7465 725f 6469 7370 6c61 7961  jupyter_displaya
+00004aa0: 626c 655f 6f75 7470 7574 286c 6962 7261  ble_output(libra
+00004ab0: 7279 5f6e 616d 653d 276e 7362 6174 776d  ry_name='nsbatwm
+00004ac0: 272c 2068 656c 705f 7572 6c3d 2768 7474  ', help_url='htt
+00004ad0: 7073 3a2f 2f77 7777 2e6e 6170 6172 692d  ps://www.napari-
+00004ae0: 6875 622e 6f72 672f 706c 7567 696e 732f  hub.org/plugins/
+00004af0: 6e61 7061 7269 2d73 6567 6d65 6e74 2d62  napari-segment-b
+00004b00: 6c6f 6273 2d61 6e64 2d74 6869 6e67 732d  lobs-and-things-
+00004b10: 7769 7468 2d6d 656d 6272 616e 6573 2729  with-membranes')
+00004b20: 0d0a 4074 696d 655f 736c 6963 6572 0d0a  ..@time_slicer..
+00004b30: 6465 6620 766f 726f 6e6f 695f 6f74 7375  def voronoi_otsu
+00004b40: 5f6c 6162 656c 696e 6728 696d 6167 653a  _labeling(image:
+00004b50: 226e 6170 6172 692e 7479 7065 732e 496d  "napari.types.Im
+00004b60: 6167 6544 6174 6122 2c20 7370 6f74 5f73  ageData", spot_s
+00004b70: 6967 6d61 3a20 666c 6f61 7420 3d20 322c  igma: float = 2,
+00004b80: 206f 7574 6c69 6e65 5f73 6967 6d61 3a20   outline_sigma: 
+00004b90: 666c 6f61 7420 3d20 3229 202d 3e20 226e  float = 2) -> "n
+00004ba0: 6170 6172 692e 7479 7065 732e 4c61 6265  apari.types.Labe
+00004bb0: 6c73 4461 7461 223a 0d0a 2020 2020 2222  lsData":..    ""
+00004bc0: 2256 6f72 6f6e 6f69 2d4f 7473 752d 4c61  "Voronoi-Otsu-La
+00004bd0: 6265 6c69 6e67 2069 7320 6120 7365 676d  beling is a segm
+00004be0: 656e 7461 7469 6f6e 2061 6c67 6f72 6974  entation algorit
+00004bf0: 686d 2066 6f72 2062 6c6f 622d 6c69 6b65  hm for blob-like
+00004c00: 2073 7472 7563 7475 7265 7320 7375 6368   structures such
+00004c10: 2061 7320 6e75 636c 6569 2061 6e64 0d0a   as nuclei and..
+00004c20: 2020 2020 6772 616e 756c 6573 2077 6974      granules wit
+00004c30: 6820 6869 6768 2073 6967 6e61 6c20 696e  h high signal in
+00004c40: 7465 6e73 6974 7920 6f6e 206c 6f77 2d69  tensity on low-i
+00004c50: 6e74 656e 7369 7479 2062 6163 6b67 726f  ntensity backgro
+00004c60: 756e 642e 0d0a 0d0a 2020 2020 5468 6520  und.....    The 
+00004c70: 7477 6f20 7369 676d 6120 7061 7261 6d65  two sigma parame
+00004c80: 7465 7273 2061 6c6c 6f77 2074 756e 696e  ters allow tunin
+00004c90: 6720 7468 6520 7365 676d 656e 7461 7469  g the segmentati
+00004ca0: 6f6e 2072 6573 756c 742e 2054 6865 2066  on result. The f
+00004cb0: 6972 7374 2073 6967 6d61 2063 6f6e 7472  irst sigma contr
+00004cc0: 6f6c 7320 686f 7720 636c 6f73 6520 6465  ols how close de
+00004cd0: 7465 6374 6564 2063 656c 6c73 0d0a 2020  tected cells..  
+00004ce0: 2020 6361 6e20 6265 2028 7370 6f74 5f73    can be (spot_s
+00004cf0: 6967 6d61 2920 616e 6420 7468 6520 7365  igma) and the se
+00004d00: 636f 6e64 2063 6f6e 7472 6f6c 7320 686f  cond controls ho
+00004d10: 7720 7072 6563 6973 6520 7365 676d 656e  w precise segmen
+00004d20: 7465 6420 6f62 6a65 6374 7320 6172 6520  ted objects are 
+00004d30: 6f75 746c 696e 6564 2028 6f75 746c 696e  outlined (outlin
+00004d40: 655f 7369 676d 6129 2e20 556e 6465 7220  e_sigma). Under 
+00004d50: 7468 650d 0a20 2020 2068 6f6f 642c 2074  the..    hood, t
+00004d60: 6869 7320 6669 6c74 6572 2061 7070 6c69  his filter appli
+00004d70: 6573 2074 776f 2047 6175 7373 6961 6e20  es two Gaussian 
+00004d80: 626c 7572 732c 2073 706f 7420 6465 7465  blurs, spot dete
+00004d90: 6374 696f 6e2c 204f 7473 752d 7468 7265  ction, Otsu-thre
+00004da0: 7368 6f6c 6469 6e67 2061 6e64 2056 6f72  sholding and Vor
+00004db0: 6f6e 6f69 2d6c 6162 656c 696e 672e 2054  onoi-labeling. T
+00004dc0: 6865 0d0a 2020 2020 7468 7265 7368 6f6c  he..    threshol
+00004dd0: 6465 6420 6269 6e61 7279 2069 6d61 6765  ded binary image
+00004de0: 2069 7320 666c 6f6f 6465 6420 7573 696e   is flooded usin
+00004df0: 6720 7468 6520 566f 726f 6e6f 6920 6170  g the Voronoi ap
+00004e00: 7072 6f61 6368 2073 7461 7274 696e 6720  proach starting 
+00004e10: 6672 6f6d 2074 6865 2066 6f75 6e64 206c  from the found l
+00004e20: 6f63 616c 206d 6178 696d 612e 204e 6f69  ocal maxima. Noi
+00004e30: 7365 2d72 656d 6f76 616c 0d0a 2020 2020  se-removal..    
+00004e40: 7369 676d 6120 666f 7220 7370 6f74 2064  sigma for spot d
+00004e50: 6574 6563 7469 6f6e 2061 6e64 2074 6872  etection and thr
+00004e60: 6573 686f 6c64 696e 6720 6361 6e20 6265  esholding can be
+00004e70: 2063 6f6e 6669 6775 7265 6420 7365 7061   configured sepa
+00004e80: 7261 7465 6c79 2e0d 0a0d 0a20 2020 2054  rately.....    T
+00004e90: 6869 7320 616c 6c6f 7773 2073 6567 6d65  his allows segme
+00004ea0: 6e74 696e 6720 636f 6e6e 6563 7465 6420  nting connected 
+00004eb0: 6f62 6a65 6374 7320 7375 6368 2061 7320  objects such as 
+00004ec0: 6e6f 7420 746f 2064 656e 7365 206e 7563  not to dense nuc
+00004ed0: 6c65 692e 0d0a 2020 2020 4966 2074 6865  lei...    If the
+00004ee0: 206e 7563 6c65 6920 6172 6520 746f 6f20   nuclei are too 
+00004ef0: 6465 6e73 652c 2063 6f6e 7369 6465 7220  dense, consider 
+00004f00: 7573 696e 6720 7374 6172 6469 7374 205b  using stardist [
+00004f10: 315d 206f 7220 6365 6c6c 706f 7365 205b  1] or cellpose [
+00004f20: 325d 2e0d 0a0d 0a20 2020 2053 6565 2061  2].....    See a
+00004f30: 6c73 6f0d 0a20 2020 202d 2d2d 2d2d 2d2d  lso..    -------
+00004f40: 2d0d 0a20 2020 202e 2e20 5b30 5d20 6874  -..    .. [0] ht
+00004f50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004f60: 2f63 6c45 7370 6572 616e 746f 2f70 7963  /clEsperanto/pyc
+00004f70: 6c65 7370 6572 616e 746f 5f70 726f 746f  lesperanto_proto
+00004f80: 7479 7065 2f62 6c6f 622f 6d61 7374 6572  type/blob/master
+00004f90: 2f64 656d 6f2f 7365 676d 656e 7461 7469  /demo/segmentati
+00004fa0: 6f6e 2f76 6f72 6f6e 6f69 5f6f 7473 755f  on/voronoi_otsu_
+00004fb0: 6c61 6265 6c69 6e67 2e69 7079 6e62 0d0a  labeling.ipynb..
+00004fc0: 2020 2020 2e2e 205b 315d 2068 7474 7073      .. [1] https
+00004fd0: 3a2f 2f77 7777 2e6e 6170 6172 692d 6875  ://www.napari-hu
+00004fe0: 622e 6f72 672f 706c 7567 696e 732f 7374  b.org/plugins/st
+00004ff0: 6172 6469 7374 2d6e 6170 6172 690d 0a20  ardist-napari.. 
+00005000: 2020 202e 2e20 5b32 5d20 6874 7470 733a     .. [2] https:
+00005010: 2f2f 7777 772e 6e61 7061 7269 2d68 7562  //www.napari-hub
+00005020: 2e6f 7267 2f70 6c75 6769 6e73 2f63 656c  .org/plugins/cel
+00005030: 6c70 6f73 652d 6e61 7061 7269 0d0a 2020  lpose-napari..  
+00005040: 2020 2222 220d 0a20 2020 2069 6d61 6765    """..    image
+00005050: 203d 206e 702e 6173 6172 7261 7928 696d   = np.asarray(im
+00005060: 6167 6529 0d0a 0d0a 2020 2020 2320 626c  age)....    # bl
+00005070: 7572 2061 6e64 2064 6574 6563 7420 6c6f  ur and detect lo
+00005080: 6361 6c20 6d61 7869 6d61 0d0a 2020 2020  cal maxima..    
+00005090: 626c 7572 7265 645f 7370 6f74 7320 3d20  blurred_spots = 
+000050a0: 6761 7573 7369 616e 2869 6d61 6765 2c20  gaussian(image, 
+000050b0: 7370 6f74 5f73 6967 6d61 290d 0a20 2020  spot_sigma)..   
+000050c0: 2073 706f 745f 6365 6e74 726f 6964 7320   spot_centroids 
+000050d0: 3d20 6c6f 6361 6c5f 6d61 7869 6d61 2862  = local_maxima(b
+000050e0: 6c75 7272 6564 5f73 706f 7473 290d 0a0d  lurred_spots)...
+000050f0: 0a20 2020 2023 2062 6c75 7220 616e 6420  .    # blur and 
+00005100: 7468 7265 7368 6f6c 640d 0a20 2020 2062  threshold..    b
+00005110: 6c75 7272 6564 5f6f 7574 6c69 6e65 203d  lurred_outline =
+00005120: 2067 6175 7373 6961 6e28 696d 6167 652c   gaussian(image,
+00005130: 206f 7574 6c69 6e65 5f73 6967 6d61 290d   outline_sigma).
+00005140: 0a20 2020 2074 6872 6573 686f 6c64 203d  .    threshold =
+00005150: 2073 6b5f 7468 7265 7368 6f6c 645f 6f74   sk_threshold_ot
+00005160: 7375 2862 6c75 7272 6564 5f6f 7574 6c69  su(blurred_outli
+00005170: 6e65 290d 0a20 2020 2062 696e 6172 795f  ne)..    binary_
+00005180: 6f74 7375 203d 2062 6c75 7272 6564 5f6f  otsu = blurred_o
+00005190: 7574 6c69 6e65 203e 2074 6872 6573 686f  utline > thresho
+000051a0: 6c64 0d0a 0d0a 2020 2020 2320 6465 7465  ld....    # dete
+000051b0: 726d 696e 6520 6c6f 6361 6c20 6d61 7869  rmine local maxi
+000051c0: 6d61 2077 6974 6869 6e20 7468 6520 7468  ma within the th
+000051d0: 7265 7368 6f6c 6465 6420 6172 6561 0d0a  resholded area..
+000051e0: 2020 2020 7265 6d61 696e 696e 675f 7370      remaining_sp
+000051f0: 6f74 7320 3d20 7370 6f74 5f63 656e 7472  ots = spot_centr
+00005200: 6f69 6473 202a 2062 696e 6172 795f 6f74  oids * binary_ot
+00005210: 7375 0d0a 0d0a 2020 2020 2320 7374 6172  su....    # star
+00005220: 7420 6672 6f6d 2072 656d 6169 6e69 6e67  t from remaining
+00005230: 2073 706f 7473 2061 6e64 2066 6c6f 6f64   spots and flood
+00005240: 2062 696e 6172 7920 696d 6167 6520 7769   binary image wi
+00005250: 7468 206c 6162 656c 730d 0a20 2020 206c  th labels..    l
+00005260: 6162 656c 6564 5f73 706f 7473 203d 206c  abeled_spots = l
+00005270: 6162 656c 2872 656d 6169 6e69 6e67 5f73  abel(remaining_s
+00005280: 706f 7473 290d 0a20 2020 206c 6162 656c  pots)..    label
+00005290: 7320 3d20 7761 7465 7273 6865 6428 6269  s = watershed(bi
+000052a0: 6e61 7279 5f6f 7473 752c 206c 6162 656c  nary_otsu, label
+000052b0: 6564 5f73 706f 7473 2c20 6d61 736b 3d62  ed_spots, mask=b
+000052c0: 696e 6172 795f 6f74 7375 290d 0a0d 0a20  inary_otsu).... 
+000052d0: 2020 2072 6574 7572 6e20 6c61 6265 6c73     return labels
+000052e0: 0d0a 0d0a 0d0a 4072 6567 6973 7465 725f  ......@register_
+000052f0: 6675 6e63 7469 6f6e 286d 656e 753d 2253  function(menu="S
+00005300: 6567 6d65 6e74 6174 696f 6e20 2f20 6c61  egmentation / la
+00005310: 6265 6c69 6e67 203e 2047 6175 7373 2d4f  beling > Gauss-O
+00005320: 7473 752d 6c61 6265 6c69 6e67 2028 6e73  tsu-labeling (ns
+00005330: 6261 7477 6d29 2229 0d0a 406a 7570 7974  batwm)")..@jupyt
+00005340: 6572 5f64 6973 706c 6179 6162 6c65 5f6f  er_displayable_o
+00005350: 7574 7075 7428 6c69 6272 6172 795f 6e61  utput(library_na
+00005360: 6d65 3d27 6e73 6261 7477 6d27 2c20 6865  me='nsbatwm', he
+00005370: 6c70 5f75 726c 3d27 6874 7470 733a 2f2f  lp_url='https://
+00005380: 7777 772e 6e61 7061 7269 2d68 7562 2e6f  www.napari-hub.o
+00005390: 7267 2f70 6c75 6769 6e73 2f6e 6170 6172  rg/plugins/napar
+000053a0: 692d 7365 676d 656e 742d 626c 6f62 732d  i-segment-blobs-
+000053b0: 616e 642d 7468 696e 6773 2d77 6974 682d  and-things-with-
+000053c0: 6d65 6d62 7261 6e65 7327 290d 0a40 7469  membranes')..@ti
+000053d0: 6d65 5f73 6c69 6365 720d 0a64 6566 2067  me_slicer..def g
+000053e0: 6175 7373 5f6f 7473 755f 6c61 6265 6c69  auss_otsu_labeli
+000053f0: 6e67 2869 6d61 6765 3a22 6e61 7061 7269  ng(image:"napari
+00005400: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
+00005410: 222c 206f 7574 6c69 6e65 5f73 6967 6d61  ", outline_sigma
+00005420: 3a20 666c 6f61 7420 3d20 3229 202d 3e20  : float = 2) -> 
+00005430: 226e 6170 6172 692e 7479 7065 732e 4c61  "napari.types.La
+00005440: 6265 6c73 4461 7461 223a 0d0a 2020 2020  belsData":..    
+00005450: 2222 2247 6175 7373 2d4f 7473 752d 4c61  """Gauss-Otsu-La
+00005460: 6265 6c69 6e67 2063 616e 2062 6520 7573  beling can be us
+00005470: 6564 2074 6f20 7365 676d 656e 7420 6f62  ed to segment ob
+00005480: 6a65 6374 7320 7375 6368 2061 7320 6e75  jects such as nu
+00005490: 636c 6569 2077 6974 6820 6272 6967 6874  clei with bright
+000054a0: 2069 6e74 656e 7369 7479 206f 6e0d 0a20   intensity on.. 
+000054b0: 2020 206c 6f77 2069 6e74 656e 7369 7479     low intensity
+000054c0: 2062 6163 6b67 726f 756e 6420 696d 6167   background imag
+000054d0: 6573 2e0d 0a0d 0a20 2020 2054 6865 206f  es.....    The o
+000054e0: 7574 6c69 6e65 5f73 6967 6d61 2070 6172  utline_sigma par
+000054f0: 616d 6574 6572 2061 6c6c 6f77 7320 7475  ameter allows tu
+00005500: 6e69 6e67 2068 6f77 2070 7265 6369 7365  ning how precise
+00005510: 2073 6567 6d65 6e74 6564 206f 626a 6563   segmented objec
+00005520: 7473 2061 7265 206f 7574 6c69 6e65 642e  ts are outlined.
+00005530: 2055 6e64 6572 2074 6865 0d0a 2020 2020   Under the..    
+00005540: 686f 6f64 2c20 7468 6973 2066 696c 7465  hood, this filte
+00005550: 7220 6170 706c 6965 7320 6120 4761 7573  r applies a Gaus
+00005560: 7369 616e 2062 6c75 722c 204f 7473 752d  sian blur, Otsu-
+00005570: 7468 7265 7368 6f6c 6469 6e67 2061 6e64  thresholding and
+00005580: 2063 6f6e 6e65 6374 6564 2063 6f6d 706f   connected compo
+00005590: 6e65 6e74 206c 6162 656c 696e 672e 0d0a  nent labeling...
+000055a0: 0d0a 2020 2020 5365 6520 616c 736f 0d0a  ..    See also..
+000055b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020      --------..  
+000055c0: 2020 2e2e 205b 305d 2068 7474 7073 3a2f    .. [0] https:/
+000055d0: 2f67 6974 6875 622e 636f 6d2f 636c 4573  /github.com/clEs
+000055e0: 7065 7261 6e74 6f2f 7079 636c 6573 7065  peranto/pyclespe
+000055f0: 7261 6e74 6f5f 7072 6f74 6f74 7970 652f  ranto_prototype/
+00005600: 626c 6f62 2f6d 6173 7465 722f 6465 6d6f  blob/master/demo
+00005610: 2f73 6567 6d65 6e74 6174 696f 6e2f 6761  /segmentation/ga
+00005620: 7573 735f 6f74 7375 5f6c 6162 656c 696e  uss_otsu_labelin
+00005630: 672e 6970 796e 620d 0a20 2020 2022 2222  g.ipynb..    """
+00005640: 0d0a 2020 2020 696d 6167 6520 3d20 6e70  ..    image = np
+00005650: 2e61 7361 7272 6179 2869 6d61 6765 290d  .asarray(image).
+00005660: 0a0d 0a20 2020 2023 2062 6c75 720d 0a20  ...    # blur.. 
+00005670: 2020 2062 6c75 7272 6564 5f6f 7574 6c69     blurred_outli
+00005680: 6e65 203d 2067 6175 7373 6961 6e28 696d  ne = gaussian(im
+00005690: 6167 652c 206f 7574 6c69 6e65 5f73 6967  age, outline_sig
+000056a0: 6d61 290d 0a0d 0a20 2020 2023 2074 6872  ma)....    # thr
+000056b0: 6573 686f 6c64 0d0a 2020 2020 7468 7265  eshold..    thre
+000056c0: 7368 6f6c 6420 3d20 736b 5f74 6872 6573  shold = sk_thres
+000056d0: 686f 6c64 5f6f 7473 7528 626c 7572 7265  hold_otsu(blurre
+000056e0: 645f 6f75 746c 696e 6529 0d0a 2020 2020  d_outline)..    
+000056f0: 6269 6e61 7279 5f6f 7473 7520 3d20 626c  binary_otsu = bl
+00005700: 7572 7265 645f 6f75 746c 696e 6520 3e20  urred_outline > 
+00005710: 7468 7265 7368 6f6c 640d 0a0d 0a20 2020  threshold....   
+00005720: 2023 2063 6f6e 6e65 6374 6564 2063 6f6d   # connected com
+00005730: 706f 6e65 6e74 206c 6162 656c 696e 670d  ponent labeling.
+00005740: 0a20 2020 206c 6162 656c 7320 3d20 6c61  .    labels = la
+00005750: 6265 6c28 6269 6e61 7279 5f6f 7473 7529  bel(binary_otsu)
+00005760: 0d0a 0d0a 2020 2020 7265 7475 726e 206c  ....    return l
+00005770: 6162 656c 730d 0a0d 0a0d 0a40 7265 6769  abels......@regi
+00005780: 7374 6572 5f66 756e 6374 696f 6e28 6d65  ster_function(me
+00005790: 6e75 3d22 5365 676d 656e 7461 7469 6f6e  nu="Segmentation
+000057a0: 202f 206c 6162 656c 696e 6720 3e20 5365   / labeling > Se
+000057b0: 6564 6564 2077 6174 6572 7368 6564 2028  eded watershed (
+000057c0: 7363 696b 6974 2d69 6d61 6765 2c20 6e73  scikit-image, ns
+000057d0: 6261 7477 6d29 2229 0d0a 406a 7570 7974  batwm)")..@jupyt
+000057e0: 6572 5f64 6973 706c 6179 6162 6c65 5f6f  er_displayable_o
+000057f0: 7574 7075 7428 6c69 6272 6172 795f 6e61  utput(library_na
+00005800: 6d65 3d27 6e73 6261 7477 6d27 2c20 6865  me='nsbatwm', he
+00005810: 6c70 5f75 726c 3d27 6874 7470 733a 2f2f  lp_url='https://
+00005820: 7777 772e 6e61 7061 7269 2d68 7562 2e6f  www.napari-hub.o
+00005830: 7267 2f70 6c75 6769 6e73 2f6e 6170 6172  rg/plugins/napar
+00005840: 692d 7365 676d 656e 742d 626c 6f62 732d  i-segment-blobs-
+00005850: 616e 642d 7468 696e 6773 2d77 6974 682d  and-things-with-
+00005860: 6d65 6d62 7261 6e65 7327 290d 0a40 7469  membranes')..@ti
+00005870: 6d65 5f73 6c69 6365 720d 0a64 6566 2073  me_slicer..def s
+00005880: 6565 6465 645f 7761 7465 7273 6865 6428  eeded_watershed(
+00005890: 6d65 6d62 7261 6e65 733a 226e 6170 6172  membranes:"napar
+000058a0: 692e 7479 7065 732e 496d 6167 6544 6174  i.types.ImageDat
+000058b0: 6122 2c20 6c61 6265 6c65 645f 6e75 636c  a", labeled_nucl
+000058c0: 6569 3a22 6e61 7061 7269 2e74 7970 6573  ei:"napari.types
+000058d0: 2e4c 6162 656c 7344 6174 6122 2920 2d3e  .LabelsData") ->
+000058e0: 2022 6e61 7061 7269 2e74 7970 6573 2e4c   "napari.types.L
+000058f0: 6162 656c 7344 6174 6122 3a0d 0a20 2020  abelsData":..   
+00005900: 2022 2222 0d0a 2020 2020 5461 6b65 7320   """..    Takes 
+00005910: 6120 696d 6167 6520 7769 7468 2062 7269  a image with bri
+00005920: 6768 7420 2868 6967 6820 696e 7465 6e73  ght (high intens
+00005930: 6974 7929 206d 656d 6272 616e 6573 2061  ity) membranes a
+00005940: 6e64 2061 6e20 696d 6167 6520 7769 7468  nd an image with
+00005950: 206c 6162 656c 6564 206f 626a 6563 7473   labeled objects
+00005960: 2073 7563 6820 6173 206e 7563 6c65 692e   such as nuclei.
+00005970: 0d0a 2020 2020 5468 6520 6c61 7474 6572  ..    The latter
+00005980: 2073 6572 7665 7320 6173 2073 6565 6473   serves as seeds
+00005990: 2069 6d61 6765 2066 6f72 2061 2077 6174   image for a wat
+000059a0: 6572 7368 6564 206c 6162 656c 696e 672e  ershed labeling.
+000059b0: 0d0a 0d0a 2020 2020 5365 6520 616c 736f  ....    See also
+000059c0: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a  ..    --------..
+000059d0: 2020 2020 2e2e 205b 315d 2068 7474 7073      .. [1] https
+000059e0: 3a2f 2f73 6369 6b69 742d 696d 6167 652e  ://scikit-image.
+000059f0: 6f72 672f 646f 6373 2f64 6576 2f61 7574  org/docs/dev/aut
+00005a00: 6f5f 6578 616d 706c 6573 2f73 6567 6d65  o_examples/segme
+00005a10: 6e74 6174 696f 6e2f 706c 6f74 5f77 6174  ntation/plot_wat
+00005a20: 6572 7368 6564 2e68 746d 6c0d 0a20 2020  ershed.html..   
+00005a30: 2022 2222 0d0a 2020 2020 6365 6c6c 7320   """..    cells 
+00005a40: 3d20 7761 7465 7273 6865 6428 0d0a 2020  = watershed(..  
+00005a50: 2020 2020 2020 6e70 2e61 7361 7272 6179        np.asarray
+00005a60: 286d 656d 6272 616e 6573 292c 0d0a 2020  (membranes),..  
+00005a70: 2020 2020 2020 6e70 2e61 7361 7272 6179        np.asarray
+00005a80: 286c 6162 656c 6564 5f6e 7563 6c65 6929  (labeled_nuclei)
+00005a90: 0d0a 2020 2020 290d 0a20 2020 2072 6574  ..    )..    ret
+00005aa0: 7572 6e20 6365 6c6c 730d 0a0d 0a40 7265  urn cells....@re
+00005ab0: 6769 7374 6572 5f66 756e 6374 696f 6e28  gister_function(
+00005ac0: 6d65 6e75 3d22 5365 676d 656e 7461 7469  menu="Segmentati
+00005ad0: 6f6e 202f 206c 6162 656c 696e 6720 3e20  on / labeling > 
+00005ae0: 5365 6564 6564 2077 6174 6572 7368 6564  Seeded watershed
+00005af0: 2077 6974 6820 6d61 736b 2028 7363 696b   with mask (scik
+00005b00: 6974 2d69 6d61 6765 2c20 6e73 6261 7477  it-image, nsbatw
+00005b10: 6d29 2229 0d0a 406a 7570 7974 6572 5f64  m)")..@jupyter_d
+00005b20: 6973 706c 6179 6162 6c65 5f6f 7574 7075  isplayable_outpu
+00005b30: 7428 6c69 6272 6172 795f 6e61 6d65 3d27  t(library_name='
+00005b40: 6e73 6261 7477 6d27 2c20 6865 6c70 5f75  nsbatwm', help_u
+00005b50: 726c 3d27 6874 7470 733a 2f2f 7777 772e  rl='https://www.
+00005b60: 6e61 7061 7269 2d68 7562 2e6f 7267 2f70  napari-hub.org/p
+00005b70: 6c75 6769 6e73 2f6e 6170 6172 692d 7365  lugins/napari-se
+00005b80: 676d 656e 742d 626c 6f62 732d 616e 642d  gment-blobs-and-
+00005b90: 7468 696e 6773 2d77 6974 682d 6d65 6d62  things-with-memb
+00005ba0: 7261 6e65 7327 290d 0a40 7469 6d65 5f73  ranes')..@time_s
+00005bb0: 6c69 6365 720d 0a64 6566 2073 6565 6465  licer..def seede
+00005bc0: 645f 7761 7465 7273 6865 645f 7769 7468  d_watershed_with
+00005bd0: 5f6d 6173 6b28 6d65 6d62 7261 6e65 733a  _mask(membranes:
+00005be0: 226e 6170 6172 692e 7479 7065 732e 496d  "napari.types.Im
+00005bf0: 6167 6544 6174 6122 2c20 6c61 6265 6c65  ageData", labele
+00005c00: 645f 6e75 636c 6569 3a22 6e61 7061 7269  d_nuclei:"napari
+00005c10: 2e74 7970 6573 2e4c 6162 656c 7344 6174  .types.LabelsDat
+00005c20: 6122 2c20 6d61 736b 3a22 6e61 7061 7269  a", mask:"napari
+00005c30: 2e74 7970 6573 2e4c 6162 656c 7344 6174  .types.LabelsDat
+00005c40: 6122 2920 2d3e 2022 6e61 7061 7269 2e74  a") -> "napari.t
+00005c50: 7970 6573 2e4c 6162 656c 7344 6174 6122  ypes.LabelsData"
+00005c60: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
+00005c70: 5461 6b65 7320 6120 696d 6167 6520 7769  Takes a image wi
+00005c80: 7468 2062 7269 6768 7420 2868 6967 6820  th bright (high 
+00005c90: 696e 7465 6e73 6974 7929 206d 656d 6272  intensity) membr
+00005ca0: 616e 6573 2c20 616e 2069 6d61 6765 2077  anes, an image w
+00005cb0: 6974 6820 6c61 6265 6c65 6420 6f62 6a65  ith labeled obje
+00005cc0: 6374 7320 7375 6368 2061 7320 6e75 636c  cts such as nucl
+00005cd0: 6569 2061 6e64 2061 206d 6173 6b20 696d  ei and a mask im
+00005ce0: 6765 2c20 652e 672e 2061 2062 696e 6172  ge, e.g. a binar
+00005cf0: 7920 696d 6167 6520 6f66 2074 6865 2065  y image of the e
+00005d00: 6e74 6972 6520 7469 7373 7565 206f 6620  ntire tissue of 
+00005d10: 696e 7465 7265 7374 2e0d 0a20 2020 2054  interest...    T
+00005d20: 6865 206c 6162 656c 6564 206e 7563 6c65  he labeled nucle
+00005d30: 6920 7365 7276 6520 6173 2073 6565 6473  i serve as seeds
+00005d40: 2069 6d61 6765 2066 6f72 2061 2077 6174   image for a wat
+00005d50: 6572 7368 6564 206c 6162 656c 696e 6720  ershed labeling 
+00005d60: 616e 6420 7468 6520 6d61 736b 2066 6f72  and the mask for
+00005d70: 2063 6f6e 7374 7261 696e 7469 6e67 2074   constrainting t
+00005d80: 6865 2066 6c6f 6f64 696e 672e 0d0a 0d0a  he flooding.....
+00005d90: 2020 2020 5365 6520 616c 736f 0d0a 2020      See also..  
+00005da0: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
+00005db0: 2e2e 205b 315d 2068 7474 7073 3a2f 2f73  .. [1] https://s
+00005dc0: 6369 6b69 742d 696d 6167 652e 6f72 672f  cikit-image.org/
+00005dd0: 646f 6373 2f64 6576 2f61 7574 6f5f 6578  docs/dev/auto_ex
+00005de0: 616d 706c 6573 2f73 6567 6d65 6e74 6174  amples/segmentat
+00005df0: 696f 6e2f 706c 6f74 5f77 6174 6572 7368  ion/plot_watersh
+00005e00: 6564 2e68 746d 6c0d 0a20 2020 2022 2222  ed.html..    """
+00005e10: 0d0a 2020 2020 6365 6c6c 7320 3d20 7761  ..    cells = wa
+00005e20: 7465 7273 6865 6428 0d0a 2020 2020 2020  tershed(..      
+00005e30: 2020 6e70 2e61 7361 7272 6179 286d 656d    np.asarray(mem
+00005e40: 6272 616e 6573 292c 0d0a 2020 2020 2020  branes),..      
+00005e50: 2020 6e70 2e61 7361 7272 6179 286c 6162    np.asarray(lab
+00005e60: 656c 6564 5f6e 7563 6c65 6929 2c0d 0a20  eled_nuclei),.. 
+00005e70: 2020 2020 2020 206d 6173 6b3d 6d61 736b         mask=mask
+00005e80: 0d0a 2020 2020 290d 0a20 2020 2072 6574  ..    )..    ret
+00005e90: 7572 6e20 6365 6c6c 730d 0a0d 0a0d 0a40  urn cells......@
+00005ea0: 7265 6769 7374 6572 5f66 756e 6374 696f  register_functio
+00005eb0: 6e28 6d65 6e75 3d22 5365 676d 656e 7461  n(menu="Segmenta
+00005ec0: 7469 6f6e 202f 206c 6162 656c 696e 6720  tion / labeling 
+00005ed0: 3e20 5365 6564 6564 2077 6174 6572 7368  > Seeded watersh
+00005ee0: 6564 2075 7369 6e67 206c 6f63 616c 206d  ed using local m
+00005ef0: 696e 696d 6120 6173 2073 6565 6473 2028  inima as seeds (
+00005f00: 6e73 6261 7477 6d29 2229 0d0a 406a 7570  nsbatwm)")..@jup
+00005f10: 7974 6572 5f64 6973 706c 6179 6162 6c65  yter_displayable
+00005f20: 5f6f 7574 7075 7428 6c69 6272 6172 795f  _output(library_
+00005f30: 6e61 6d65 3d27 6e73 6261 7477 6d27 2c20  name='nsbatwm', 
+00005f40: 6865 6c70 5f75 726c 3d27 6874 7470 733a  help_url='https:
+00005f50: 2f2f 7777 772e 6e61 7061 7269 2d68 7562  //www.napari-hub
+00005f60: 2e6f 7267 2f70 6c75 6769 6e73 2f6e 6170  .org/plugins/nap
+00005f70: 6172 692d 7365 676d 656e 742d 626c 6f62  ari-segment-blob
+00005f80: 732d 616e 642d 7468 696e 6773 2d77 6974  s-and-things-wit
+00005f90: 682d 6d65 6d62 7261 6e65 7327 290d 0a40  h-membranes')..@
+00005fa0: 7469 6d65 5f73 6c69 6365 720d 0a64 6566  time_slicer..def
+00005fb0: 206c 6f63 616c 5f6d 696e 696d 615f 7365   local_minima_se
+00005fc0: 6564 6564 5f77 6174 6572 7368 6564 2869  eded_watershed(i
+00005fd0: 6d61 6765 3a22 6e61 7061 7269 2e74 7970  mage:"napari.typ
+00005fe0: 6573 2e49 6d61 6765 4461 7461 222c 2073  es.ImageData", s
+00005ff0: 706f 745f 7369 676d 613a 2066 6c6f 6174  pot_sigma: float
+00006000: 203d 2031 302c 206f 7574 6c69 6e65 5f73   = 10, outline_s
+00006010: 6967 6d61 3a20 666c 6f61 7420 3d20 3029  igma: float = 0)
+00006020: 202d 3e20 226e 6170 6172 692e 7479 7065   -> "napari.type
+00006030: 732e 4c61 6265 6c73 4461 7461 223a 0d0a  s.LabelsData":..
+00006040: 2020 2020 2222 220d 0a20 2020 2053 6567      """..    Seg
+00006050: 6d65 6e74 2063 656c 6c73 2069 6e20 696d  ment cells in im
+00006060: 6167 6573 2077 6974 6820 666c 756f 7265  ages with fluore
+00006070: 7363 656e 746c 7920 6d61 726b 6564 206d  scently marked m
+00006080: 656d 6272 616e 6573 2e0d 0a0d 0a20 2020  embranes.....   
+00006090: 2054 6865 2074 776f 2073 6967 6d61 2070   The two sigma p
+000060a0: 6172 616d 6574 6572 7320 616c 6c6f 7720  arameters allow 
+000060b0: 7475 6e69 6e67 2074 6865 2073 6567 6d65  tuning the segme
+000060c0: 6e74 6174 696f 6e20 7265 7375 6c74 2e20  ntation result. 
+000060d0: 5468 6520 6669 7273 7420 7369 676d 6120  The first sigma 
+000060e0: 636f 6e74 726f 6c73 2068 6f77 2063 6c6f  controls how clo
+000060f0: 7365 2064 6574 6563 7465 6420 6365 6c6c  se detected cell
+00006100: 730d 0a20 2020 2063 616e 2062 6520 2873  s..    can be (s
+00006110: 706f 745f 7369 676d 6129 2061 6e64 2074  pot_sigma) and t
+00006120: 6865 2073 6563 6f6e 6420 636f 6e74 726f  he second contro
+00006130: 6c73 2068 6f77 2070 7265 6369 7365 2073  ls how precise s
+00006140: 6567 6d65 6e74 6564 206f 626a 6563 7473  egmented objects
+00006150: 2061 7265 206f 7574 6c69 6e65 6420 286f   are outlined (o
+00006160: 7574 6c69 6e65 5f73 6967 6d61 292e 2055  utline_sigma). U
+00006170: 6e64 6572 2074 6865 0d0a 2020 2020 686f  nder the..    ho
+00006180: 6f64 2c20 7468 6973 2066 696c 7465 7220  od, this filter 
+00006190: 6170 706c 6965 7320 7477 6f20 4761 7573  applies two Gaus
+000061a0: 7369 616e 2062 6c75 7273 2c20 6c6f 6361  sian blurs, loca
+000061b0: 6c20 6d69 6e69 6d61 2064 6574 6563 7469  l minima detecti
+000061c0: 6f6e 2061 6e64 2061 2073 6565 6465 6420  on and a seeded 
+000061d0: 7761 7465 7273 6865 642e 0d0a 0d0a 2020  watershed.....  
+000061e0: 2020 5365 6520 616c 736f 0d0a 2020 2020    See also..    
+000061f0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2e2e  --------..    ..
+00006200: 205b 315d 2068 7474 7073 3a2f 2f73 6369   [1] https://sci
+00006210: 6b69 742d 696d 6167 652e 6f72 672f 646f  kit-image.org/do
+00006220: 6373 2f64 6576 2f61 7574 6f5f 6578 616d  cs/dev/auto_exam
+00006230: 706c 6573 2f73 6567 6d65 6e74 6174 696f  ples/segmentatio
+00006240: 6e2f 706c 6f74 5f77 6174 6572 7368 6564  n/plot_watershed
+00006250: 2e68 746d 6c0d 0a20 2020 2022 2222 0d0a  .html..    """..
+00006260: 0d0a 2020 2020 696d 6167 6520 3d20 6e70  ..    image = np
+00006270: 2e61 7361 7272 6179 2869 6d61 6765 290d  .asarray(image).
+00006280: 0a0d 0a20 2020 2073 706f 745f 626c 7572  ...    spot_blur
+00006290: 7265 6420 3d20 6761 7573 7369 616e 2869  red = gaussian(i
+000062a0: 6d61 6765 2c20 7369 676d 613d 7370 6f74  mage, sigma=spot
+000062b0: 5f73 6967 6d61 290d 0a0d 0a20 2020 2073  _sigma)....    s
+000062c0: 706f 7473 203d 206c 6162 656c 286c 6f63  pots = label(loc
+000062d0: 616c 5f6d 696e 696d 6128 7370 6f74 5f62  al_minima(spot_b
+000062e0: 6c75 7272 6564 2929 0d0a 0d0a 2020 2020  lurred))....    
+000062f0: 6966 206f 7574 6c69 6e65 5f73 6967 6d61  if outline_sigma
+00006300: 203d 3d20 7370 6f74 5f73 6967 6d61 3a0d   == spot_sigma:.
+00006310: 0a20 2020 2020 2020 206f 7574 6c69 6e65  .        outline
+00006320: 5f62 6c75 7272 6564 203d 2073 706f 745f  _blurred = spot_
+00006330: 626c 7572 7265 640d 0a20 2020 2065 6c73  blurred..    els
+00006340: 653a 0d0a 2020 2020 2020 2020 6f75 746c  e:..        outl
+00006350: 696e 655f 626c 7572 7265 6420 3d20 6761  ine_blurred = ga
+00006360: 7573 7369 616e 2869 6d61 6765 2c20 7369  ussian(image, si
+00006370: 676d 613d 6f75 746c 696e 655f 7369 676d  gma=outline_sigm
+00006380: 6129 0d0a 0d0a 2020 2020 7265 7475 726e  a)....    return
+00006390: 2077 6174 6572 7368 6564 286f 7574 6c69   watershed(outli
+000063a0: 6e65 5f62 6c75 7272 6564 2c20 7370 6f74  ne_blurred, spot
+000063b0: 7329 0d0a 0d0a 0d0a 4072 6567 6973 7465  s)......@registe
+000063c0: 725f 6675 6e63 7469 6f6e 286d 656e 753d  r_function(menu=
+000063d0: 2253 6567 6d65 6e74 6174 696f 6e20 2f20  "Segmentation / 
+000063e0: 6c61 6265 6c69 6e67 203e 2053 6565 6465  labeling > Seede
+000063f0: 6420 7761 7465 7273 6865 6420 7573 696e  d watershed usin
+00006400: 6720 6c6f 6361 6c20 6d69 6e69 6d61 2061  g local minima a
+00006410: 7320 7365 6564 7320 616e 6420 616e 2069  s seeds and an i
+00006420: 6e74 656e 7369 7479 2074 6872 6573 686f  ntensity thresho
+00006430: 6c64 2028 6e73 6261 7477 6d29 2229 0d0a  ld (nsbatwm)")..
+00006440: 406a 7570 7974 6572 5f64 6973 706c 6179  @jupyter_display
+00006450: 6162 6c65 5f6f 7574 7075 7428 6c69 6272  able_output(libr
+00006460: 6172 795f 6e61 6d65 3d27 6e73 6261 7477  ary_name='nsbatw
+00006470: 6d27 2c20 6865 6c70 5f75 726c 3d27 6874  m', help_url='ht
+00006480: 7470 733a 2f2f 7777 772e 6e61 7061 7269  tps://www.napari
+00006490: 2d68 7562 2e6f 7267 2f70 6c75 6769 6e73  -hub.org/plugins
+000064a0: 2f6e 6170 6172 692d 7365 676d 656e 742d  /napari-segment-
+000064b0: 626c 6f62 732d 616e 642d 7468 696e 6773  blobs-and-things
+000064c0: 2d77 6974 682d 6d65 6d62 7261 6e65 7327  -with-membranes'
+000064d0: 290d 0a40 7469 6d65 5f73 6c69 6365 720d  )..@time_slicer.
+000064e0: 0a64 6566 2074 6872 6573 686f 6c64 6564  .def thresholded
+000064f0: 5f6c 6f63 616c 5f6d 696e 696d 615f 7365  _local_minima_se
+00006500: 6564 6564 5f77 6174 6572 7368 6564 2869  eded_watershed(i
+00006510: 6d61 6765 3a22 6e61 7061 7269 2e74 7970  mage:"napari.typ
+00006520: 6573 2e49 6d61 6765 4461 7461 222c 2073  es.ImageData", s
+00006530: 706f 745f 7369 676d 613a 2066 6c6f 6174  pot_sigma: float
+00006540: 203d 2033 2c20 6f75 746c 696e 655f 7369   = 3, outline_si
+00006550: 676d 613a 2066 6c6f 6174 203d 2030 2c20  gma: float = 0, 
+00006560: 6d69 6e69 6d75 6d5f 696e 7465 6e73 6974  minimum_intensit
+00006570: 793a 2066 6c6f 6174 203d 2035 3030 2920  y: float = 500) 
+00006580: 2d3e 2022 6e61 7061 7269 2e74 7970 6573  -> "napari.types
+00006590: 2e4c 6162 656c 7344 6174 6122 3a0d 0a20  .LabelsData":.. 
+000065a0: 2020 2022 2222 0d0a 2020 2020 5365 676d     """..    Segm
+000065b0: 656e 7420 6365 6c6c 7320 696e 2069 6d61  ent cells in ima
+000065c0: 6765 7320 7769 7468 206d 6172 6b65 6420  ges with marked 
+000065d0: 6d65 6d62 7261 6e65 7320 7468 6174 2068  membranes that h
+000065e0: 6176 6520 6120 6869 6768 2073 6967 6e61  ave a high signa
+000065f0: 6c20 696e 7465 6e73 6974 792e 0d0a 0d0a  l intensity.....
+00006600: 2020 2020 5468 6520 7477 6f20 7369 676d      The two sigm
+00006610: 6120 7061 7261 6d65 7465 7273 2061 6c6c  a parameters all
+00006620: 6f77 2074 756e 696e 6720 7468 6520 7365  ow tuning the se
+00006630: 676d 656e 7461 7469 6f6e 2072 6573 756c  gmentation resul
+00006640: 742e 2054 6865 2066 6972 7374 2073 6967  t. The first sig
+00006650: 6d61 2063 6f6e 7472 6f6c 7320 686f 7720  ma controls how 
+00006660: 636c 6f73 6520 6465 7465 6374 6564 2063  close detected c
+00006670: 656c 6c73 0d0a 2020 2020 6361 6e20 6265  ells..    can be
+00006680: 2028 7370 6f74 5f73 6967 6d61 2920 616e   (spot_sigma) an
+00006690: 6420 7468 6520 7365 636f 6e64 2063 6f6e  d the second con
+000066a0: 7472 6f6c 7320 686f 7720 7072 6563 6973  trols how precis
+000066b0: 6520 7365 676d 656e 7465 6420 6f62 6a65  e segmented obje
+000066c0: 6374 7320 6172 6520 6f75 746c 696e 6564  cts are outlined
+000066d0: 2028 6f75 746c 696e 655f 7369 676d 6129   (outline_sigma)
+000066e0: 2e20 556e 6465 7220 7468 650d 0a20 2020  . Under the..   
+000066f0: 2068 6f6f 642c 2074 6869 7320 6669 6c74   hood, this filt
+00006700: 6572 2061 7070 6c69 6573 2074 776f 2047  er applies two G
+00006710: 6175 7373 6961 6e20 626c 7572 732c 206c  aussian blurs, l
+00006720: 6f63 616c 206d 696e 696d 6120 6465 7465  ocal minima dete
+00006730: 6374 696f 6e20 616e 6420 6120 7365 6564  ction and a seed
+00006740: 6564 2077 6174 6572 7368 6564 2e0d 0a0d  ed watershed....
+00006750: 0a20 2020 2041 6674 6572 7761 7264 732c  .    Afterwards,
+00006760: 2061 6c6c 206f 626a 6563 7473 2061 7265   all objects are
+00006770: 2072 656d 6f76 6564 2074 6861 7420 6861   removed that ha
+00006780: 7665 2061 6e20 6176 6572 6167 6520 696e  ve an average in
+00006790: 7465 6e73 6974 7920 6265 6c6f 7720 6120  tensity below a 
+000067a0: 6769 7665 6e20 6d69 6e69 6d75 6d5f 696e  given minimum_in
+000067b0: 7465 6e73 6974 790d 0a20 2020 2022 2222  tensity..    """
+000067c0: 0d0a 2020 2020 6c61 6265 6c73 203d 206c  ..    labels = l
+000067d0: 6f63 616c 5f6d 696e 696d 615f 7365 6564  ocal_minima_seed
+000067e0: 6564 5f77 6174 6572 7368 6564 2869 6d61  ed_watershed(ima
+000067f0: 6765 2c20 7370 6f74 5f73 6967 6d61 3d73  ge, spot_sigma=s
+00006800: 706f 745f 7369 676d 612c 206f 7574 6c69  pot_sigma, outli
+00006810: 6e65 5f73 6967 6d61 3d6f 7574 6c69 6e65  ne_sigma=outline
+00006820: 5f73 6967 6d61 290d 0a0d 0a20 2020 2023  _sigma)....    #
+00006830: 206d 6561 7375 7265 2069 6e74 656e 7369   measure intensi
+00006840: 7469 6573 0d0a 2020 2020 7374 6174 7320  ties..    stats 
+00006850: 3d20 7265 6769 6f6e 7072 6f70 7328 6c61  = regionprops(la
+00006860: 6265 6c73 2c20 696d 6167 6529 0d0a 2020  bels, image)..  
+00006870: 2020 696e 7465 6e73 6974 6965 7320 3d20    intensities = 
+00006880: 5b72 2e6d 6561 6e5f 696e 7465 6e73 6974  [r.mean_intensit
+00006890: 7920 666f 7220 7220 696e 2073 7461 7473  y for r in stats
+000068a0: 5d0d 0a0d 0a20 2020 2023 2066 696c 7465  ]....    # filte
+000068b0: 7220 6c61 6265 6c73 2077 6974 6820 6c6f  r labels with lo
+000068c0: 7720 696e 7465 6e73 6974 790d 0a20 2020  w intensity..   
+000068d0: 206e 6577 5f6c 6162 656c 5f69 6e64 6963   new_label_indic
+000068e0: 6573 2c20 5f2c 205f 203d 2073 6b5f 7265  es, _, _ = sk_re
+000068f0: 6c61 6265 6c5f 7365 7175 656e 7469 616c  label_sequential
+00006900: 2828 6e70 2e61 7361 7272 6179 2869 6e74  ((np.asarray(int
+00006910: 656e 7369 7469 6573 2920 3e20 6d69 6e69  ensities) > mini
+00006920: 6d75 6d5f 696e 7465 6e73 6974 7929 202a  mum_intensity) *
+00006930: 206e 702e 6172 616e 6765 286c 6162 656c   np.arange(label
+00006940: 732e 6d61 7828 2929 290d 0a20 2020 206e  s.max()))..    n
+00006950: 6577 5f6c 6162 656c 5f69 6e64 6963 6573  ew_label_indices
+00006960: 203d 206e 702e 696e 7365 7274 286e 6577   = np.insert(new
+00006970: 5f6c 6162 656c 5f69 6e64 6963 6573 2c20  _label_indices, 
+00006980: 302c 2030 290d 0a20 2020 206e 6577 5f6c  0, 0)..    new_l
+00006990: 6162 656c 7320 3d20 6e70 2e74 616b 6528  abels = np.take(
+000069a0: 6e70 2e61 7361 7272 6179 286e 6577 5f6c  np.asarray(new_l
+000069b0: 6162 656c 5f69 6e64 6963 6573 2c20 6e70  abel_indices, np
+000069c0: 2e75 696e 7433 3229 2c20 6c61 6265 6c73  .uint32), labels
+000069d0: 290d 0a0d 0a20 2020 2072 6574 7572 6e20  )....    return 
+000069e0: 6e65 775f 6c61 6265 6c73 0d0a 0d0a 4072  new_labels....@r
+000069f0: 6567 6973 7465 725f 6675 6e63 7469 6f6e  egister_function
+00006a00: 286d 656e 753d 2249 6d61 6765 206d 6174  (menu="Image mat
+00006a10: 6820 3e20 5375 6d20 696d 6167 6573 2028  h > Sum images (
+00006a20: 6e75 6d70 792c 206e 7362 6174 776d 2922  numpy, nsbatwm)"
+00006a30: 2c20 6661 6374 6f72 313d 7b27 6d69 6e27  , factor1={'min'
+00006a40: 3a20 2d31 3030 3030 3030 2c20 276d 6178  : -1000000, 'max
+00006a50: 273a 2031 3030 3030 3030 7d2c 2066 6163  ': 1000000}, fac
+00006a60: 746f 7232 3d7b 276d 696e 273a 202d 3130  tor2={'min': -10
+00006a70: 3030 3030 302c 2027 6d61 7827 3a20 3130  00000, 'max': 10
+00006a80: 3030 3030 307d 290d 0a40 6a75 7079 7465  00000})..@jupyte
+00006a90: 725f 6469 7370 6c61 7961 626c 655f 6f75  r_displayable_ou
+00006aa0: 7470 7574 286c 6962 7261 7279 5f6e 616d  tput(library_nam
+00006ab0: 653d 276e 7362 6174 776d 272c 2068 656c  e='nsbatwm', hel
+00006ac0: 705f 7572 6c3d 2768 7474 7073 3a2f 2f77  p_url='https://w
+00006ad0: 7777 2e6e 6170 6172 692d 6875 622e 6f72  ww.napari-hub.or
+00006ae0: 672f 706c 7567 696e 732f 6e61 7061 7269  g/plugins/napari
+00006af0: 2d73 6567 6d65 6e74 2d62 6c6f 6273 2d61  -segment-blobs-a
+00006b00: 6e64 2d74 6869 6e67 732d 7769 7468 2d6d  nd-things-with-m
+00006b10: 656d 6272 616e 6573 2729 0d0a 4074 696d  embranes')..@tim
+00006b20: 655f 736c 6963 6572 0d0a 6465 6620 7375  e_slicer..def su
+00006b30: 6d5f 696d 6167 6573 2869 6d61 6765 313a  m_images(image1:
+00006b40: 2022 6e61 7061 7269 2e74 7970 6573 2e49   "napari.types.I
+00006b50: 6d61 6765 4461 7461 222c 2069 6d61 6765  mageData", image
+00006b60: 323a 2022 6e61 7061 7269 2e74 7970 6573  2: "napari.types
+00006b70: 2e49 6d61 6765 4461 7461 222c 2066 6163  .ImageData", fac
+00006b80: 746f 7231 3a20 666c 6f61 7420 3d20 312c  tor1: float = 1,
+00006b90: 2066 6163 746f 7232 3a20 666c 6f61 7420   factor2: float 
+00006ba0: 3d20 3129 202d 3e20 226e 6170 6172 692e  = 1) -> "napari.
+00006bb0: 7479 7065 732e 496d 6167 6544 6174 6122  types.ImageData"
+00006bc0: 3a0d 0a20 2020 2022 2222 4164 6420 7477  :..    """Add tw
+00006bd0: 6f20 696d 6167 6573 2222 220d 0a20 2020  o images"""..   
+00006be0: 2072 6574 7572 6e20 696d 6167 6531 202a   return image1 *
+00006bf0: 2066 6163 746f 7231 202b 2069 6d61 6765   factor1 + image
+00006c00: 3220 2a20 6661 6374 6f72 320d 0a0d 0a0d  2 * factor2.....
+00006c10: 0a40 7265 6769 7374 6572 5f66 756e 6374  .@register_funct
+00006c20: 696f 6e28 6d65 6e75 3d22 496d 6167 6520  ion(menu="Image 
+00006c30: 6d61 7468 203e 204d 756c 7469 706c 7920  math > Multiply 
+00006c40: 696d 6167 6573 2028 6e75 6d70 792c 206e  images (numpy, n
+00006c50: 7362 6174 776d 2922 290d 0a40 6a75 7079  sbatwm)")..@jupy
+00006c60: 7465 725f 6469 7370 6c61 7961 626c 655f  ter_displayable_
+00006c70: 6f75 7470 7574 286c 6962 7261 7279 5f6e  output(library_n
+00006c80: 616d 653d 276e 7362 6174 776d 272c 2068  ame='nsbatwm', h
+00006c90: 656c 705f 7572 6c3d 2768 7474 7073 3a2f  elp_url='https:/
+00006ca0: 2f77 7777 2e6e 6170 6172 692d 6875 622e  /www.napari-hub.
+00006cb0: 6f72 672f 706c 7567 696e 732f 6e61 7061  org/plugins/napa
+00006cc0: 7269 2d73 6567 6d65 6e74 2d62 6c6f 6273  ri-segment-blobs
+00006cd0: 2d61 6e64 2d74 6869 6e67 732d 7769 7468  -and-things-with
+00006ce0: 2d6d 656d 6272 616e 6573 2729 0d0a 4074  -membranes')..@t
+00006cf0: 696d 655f 736c 6963 6572 0d0a 6465 6620  ime_slicer..def 
+00006d00: 6d75 6c74 6970 6c79 5f69 6d61 6765 7328  multiply_images(
+00006d10: 696d 6167 6531 3a20 226e 6170 6172 692e  image1: "napari.
+00006d20: 7479 7065 732e 496d 6167 6544 6174 6122  types.ImageData"
+00006d30: 2c20 696d 6167 6532 3a20 226e 6170 6172  , image2: "napar
+00006d40: 692e 7479 7065 732e 496d 6167 6544 6174  i.types.ImageDat
+00006d50: 6122 2920 2d3e 2022 6e61 7061 7269 2e74  a") -> "napari.t
+00006d60: 7970 6573 2e49 6d61 6765 4461 7461 223a  ypes.ImageData":
+00006d70: 0d0a 2020 2020 2222 224d 756c 7469 706c  ..    """Multipl
+00006d80: 7920 7477 6f20 696d 6167 6573 2222 220d  y two images""".
+00006d90: 0a20 2020 2072 6574 7572 6e20 696d 6167  .    return imag
+00006da0: 6531 202a 2069 6d61 6765 320d 0a0d 0a0d  e1 * image2.....
+00006db0: 0a40 7265 6769 7374 6572 5f66 756e 6374  .@register_funct
+00006dc0: 696f 6e28 6d65 6e75 3d22 496d 6167 6520  ion(menu="Image 
+00006dd0: 6d61 7468 203e 2044 6976 6964 6520 696d  math > Divide im
+00006de0: 6167 6573 2028 6e75 6d70 792c 206e 7362  ages (numpy, nsb
+00006df0: 6174 776d 2922 290d 0a40 6a75 7079 7465  atwm)")..@jupyte
+00006e00: 725f 6469 7370 6c61 7961 626c 655f 6f75  r_displayable_ou
+00006e10: 7470 7574 286c 6962 7261 7279 5f6e 616d  tput(library_nam
+00006e20: 653d 276e 7362 6174 776d 272c 2068 656c  e='nsbatwm', hel
+00006e30: 705f 7572 6c3d 2768 7474 7073 3a2f 2f77  p_url='https://w
+00006e40: 7777 2e6e 6170 6172 692d 6875 622e 6f72  ww.napari-hub.or
+00006e50: 672f 706c 7567 696e 732f 6e61 7061 7269  g/plugins/napari
+00006e60: 2d73 6567 6d65 6e74 2d62 6c6f 6273 2d61  -segment-blobs-a
+00006e70: 6e64 2d74 6869 6e67 732d 7769 7468 2d6d  nd-things-with-m
+00006e80: 656d 6272 616e 6573 2729 0d0a 4074 696d  embranes')..@tim
+00006e90: 655f 736c 6963 6572 0d0a 6465 6620 6469  e_slicer..def di
+00006ea0: 7669 6465 5f69 6d61 6765 7328 696d 6167  vide_images(imag
+00006eb0: 6531 3a20 226e 6170 6172 692e 7479 7065  e1: "napari.type
+00006ec0: 732e 496d 6167 6544 6174 6122 2c20 696d  s.ImageData", im
+00006ed0: 6167 6532 3a20 226e 6170 6172 692e 7479  age2: "napari.ty
+00006ee0: 7065 732e 496d 6167 6544 6174 6122 2920  pes.ImageData") 
+00006ef0: 2d3e 2022 6e61 7061 7269 2e74 7970 6573  -> "napari.types
+00006f00: 2e49 6d61 6765 4461 7461 223a 0d0a 2020  .ImageData":..  
+00006f10: 2020 2222 2244 6976 6964 6520 6f6e 6520    """Divide one 
+00006f20: 696d 6167 6520 6279 2061 6e6f 7468 6572  image by another
+00006f30: 2222 220d 0a20 2020 2072 6574 7572 6e20  """..    return 
+00006f40: 696d 6167 6531 202f 2069 6d61 6765 320d  image1 / image2.
+00006f50: 0a0d 0a0d 0a40 7265 6769 7374 6572 5f66  .....@register_f
+00006f60: 756e 6374 696f 6e28 6d65 6e75 3d22 496d  unction(menu="Im
+00006f70: 6167 6520 6d61 7468 203e 2049 6e76 6572  age math > Inver
+00006f80: 7420 696d 6167 6520 2873 6369 6b69 742d  t image (scikit-
+00006f90: 696d 6167 652c 206e 7362 6174 776d 2922  image, nsbatwm)"
+00006fa0: 290d 0a40 6a75 7079 7465 725f 6469 7370  )..@jupyter_disp
+00006fb0: 6c61 7961 626c 655f 6f75 7470 7574 286c  layable_output(l
+00006fc0: 6962 7261 7279 5f6e 616d 653d 276e 7362  ibrary_name='nsb
+00006fd0: 6174 776d 272c 2068 656c 705f 7572 6c3d  atwm', help_url=
+00006fe0: 2768 7474 7073 3a2f 2f77 7777 2e6e 6170  'https://www.nap
+00006ff0: 6172 692d 6875 622e 6f72 672f 706c 7567  ari-hub.org/plug
+00007000: 696e 732f 6e61 7061 7269 2d73 6567 6d65  ins/napari-segme
+00007010: 6e74 2d62 6c6f 6273 2d61 6e64 2d74 6869  nt-blobs-and-thi
+00007020: 6e67 732d 7769 7468 2d6d 656d 6272 616e  ngs-with-membran
+00007030: 6573 2729 0d0a 4074 696d 655f 736c 6963  es')..@time_slic
+00007040: 6572 0d0a 6465 6620 696e 7665 7274 5f69  er..def invert_i
+00007050: 6d61 6765 2869 6d61 6765 3a20 226e 6170  mage(image: "nap
+00007060: 6172 692e 7479 7065 732e 496d 6167 6544  ari.types.ImageD
+00007070: 6174 6122 2920 2d3e 2022 6e61 7061 7269  ata") -> "napari
+00007080: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
+00007090: 223a 0d0a 2020 2020 2222 2249 6e76 6572  ":..    """Inver
+000070a0: 7420 616e 2069 6d61 6765 2e20 5468 6520  t an image. The 
+000070b0: 6578 6163 7420 6d61 7468 2062 6568 696e  exact math behin
+000070c0: 6420 6465 7065 6e64 7320 6f6e 2074 6865  d depends on the
+000070d0: 2069 6d61 6765 2074 7970 652e 0d0a 0d0a   image type.....
+000070e0: 2020 2020 5365 6520 616c 736f 0d0a 2020      See also..  
+000070f0: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
+00007100: 2e2e 205b 305d 2068 7474 7073 3a2f 2f73  .. [0] https://s
+00007110: 6369 6b69 742d 696d 6167 652e 6f72 672f  cikit-image.org/
+00007120: 646f 6373 2f64 6576 2f61 7069 2f73 6b69  docs/dev/api/ski
+00007130: 6d61 6765 2e75 7469 6c2e 6874 6d6c 3f68  mage.util.html?h
+00007140: 6967 686c 6967 6874 3d69 6e76 6572 7423  ighlight=invert#
+00007150: 736b 696d 6167 652e 7574 696c 2e69 6e76  skimage.util.inv
+00007160: 6572 740d 0a20 2020 2022 2222 0d0a 2020  ert..    """..  
+00007170: 2020 6672 6f6d 2073 6b69 6d61 6765 2069    from skimage i
+00007180: 6d70 6f72 7420 7574 696c 0d0a 2020 2020  mport util..    
+00007190: 7265 7475 726e 2075 7469 6c2e 696e 7665  return util.inve
+000071a0: 7274 2869 6d61 6765 290d 0a0d 0a0d 0a40  rt(image)......@
+000071b0: 7265 6769 7374 6572 5f66 756e 6374 696f  register_functio
+000071c0: 6e28 6d65 6e75 3d22 5365 676d 656e 7461  n(menu="Segmenta
+000071d0: 7469 6f6e 2070 6f73 742d 7072 6f63 6573  tion post-proces
+000071e0: 7369 6e67 203e 2053 6b65 6c65 746f 6e69  sing > Skeletoni
+000071f0: 7a65 2028 7363 696b 6974 2d69 6d61 6765  ze (scikit-image
+00007200: 2c20 6e73 6261 7477 6d29 2229 0d0a 406a  , nsbatwm)")..@j
+00007210: 7570 7974 6572 5f64 6973 706c 6179 6162  upyter_displayab
+00007220: 6c65 5f6f 7574 7075 7428 6c69 6272 6172  le_output(librar
+00007230: 795f 6e61 6d65 3d27 6e73 6261 7477 6d27  y_name='nsbatwm'
+00007240: 2c20 6865 6c70 5f75 726c 3d27 6874 7470  , help_url='http
+00007250: 733a 2f2f 7777 772e 6e61 7061 7269 2d68  s://www.napari-h
+00007260: 7562 2e6f 7267 2f70 6c75 6769 6e73 2f6e  ub.org/plugins/n
+00007270: 6170 6172 692d 7365 676d 656e 742d 626c  apari-segment-bl
+00007280: 6f62 732d 616e 642d 7468 696e 6773 2d77  obs-and-things-w
+00007290: 6974 682d 6d65 6d62 7261 6e65 7327 290d  ith-membranes').
+000072a0: 0a40 7469 6d65 5f73 6c69 6365 720d 0a64  .@time_slicer..d
+000072b0: 6566 2073 6b65 6c65 746f 6e69 7a65 2869  ef skeletonize(i
+000072c0: 6d61 6765 3a20 226e 6170 6172 692e 7479  mage: "napari.ty
+000072d0: 7065 732e 4c61 6265 6c73 4461 7461 2229  pes.LabelsData")
+000072e0: 202d 3e20 226e 6170 6172 692e 7479 7065   -> "napari.type
+000072f0: 732e 4c61 6265 6c73 4461 7461 223a 0d0a  s.LabelsData":..
+00007300: 2020 2020 2222 220d 0a20 2020 2053 6b65      """..    Ske
+00007310: 6c65 746f 6e69 7a65 206c 6162 656c 6564  letonize labeled
+00007320: 206f 626a 6563 7473 2069 6e20 616e 2069   objects in an i
+00007330: 6d61 6765 2e20 5468 6973 2063 616e 2062  mage. This can b
+00007340: 6520 7573 6566 756c 2074 6f20 7265 6475  e useful to redu
+00007350: 6365 206f 626a 6563 7473 2073 7563 6820  ce objects such 
+00007360: 6173 206e 6575 726f 6e73 2c20 726f 6f74  as neurons, root
+00007370: 7320 616e 6420 7665 7373 656c 730d 0a20  s and vessels.. 
+00007380: 2020 2077 6974 6820 7661 7269 6162 6c65     with variable
+00007390: 2074 6869 636b 6e65 7373 2074 6f20 7369   thickness to si
+000073a0: 6e67 6c65 2070 6978 656c 206c 696e 6573  ngle pixel lines
+000073b0: 2066 6f72 2066 7572 7468 6572 2061 6e61   for further ana
+000073c0: 6c79 7369 732e 0d0a 0d0a 2020 2020 5365  lysis.....    Se
+000073d0: 6520 616c 736f 0d0a 2020 2020 2d2d 2d2d  e also..    ----
+000073e0: 2d2d 2d2d 0d0a 2020 2020 2e2e 205b 305d  ----..    .. [0]
+000073f0: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
+00007400: 7065 6469 612e 6f72 672f 7769 6b69 2f54  pedia.org/wiki/T
+00007410: 6f70 6f6c 6f67 6963 616c 5f73 6b65 6c65  opological_skele
+00007420: 746f 6e0d 0a20 2020 2022 2222 0d0a 2020  ton..    """..  
+00007430: 2020 6672 6f6d 2073 6b69 6d61 6765 2069    from skimage i
+00007440: 6d70 6f72 7420 6d6f 7270 686f 6c6f 6779  mport morphology
+00007450: 0d0a 2020 2020 6966 2069 6d61 6765 2e6d  ..    if image.m
+00007460: 6178 2829 203d 3d20 313a 0d0a 2020 2020  ax() == 1:..    
+00007470: 2020 2020 7265 7475 726e 206d 6f72 7068      return morph
+00007480: 6f6c 6f67 792e 736b 656c 6574 6f6e 697a  ology.skeletoniz
+00007490: 6528 696d 6167 6529 0d0a 2020 2020 656c  e(image)..    el
+000074a0: 7365 3a0d 0a20 2020 2020 2020 2072 6573  se:..        res
+000074b0: 756c 7420 3d20 6e70 2e7a 6572 6f73 2869  ult = np.zeros(i
+000074c0: 6d61 6765 2e73 6861 7065 290d 0a20 2020  mage.shape)..   
+000074d0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+000074e0: 6e67 6528 312c 2069 6d61 6765 2e6d 6178  nge(1, image.max
+000074f0: 2829 202b 2031 293a 0d0a 2020 2020 2020  () + 1):..      
+00007500: 2020 2020 2020 736b 656c 6574 6f6e 203d        skeleton =
+00007510: 206d 6f72 7068 6f6c 6f67 792e 736b 656c   morphology.skel
+00007520: 6574 6f6e 697a 6528 696d 6167 6520 3d3d  etonize(image ==
+00007530: 2069 290d 0a20 2020 2020 2020 2020 2020   i)..           
+00007540: 2072 6573 756c 7420 3d20 736b 656c 6574   result = skelet
+00007550: 6f6e 202a 2069 202b 2072 6573 756c 740d  on * i + result.
+00007560: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007570: 7265 7375 6c74 2e61 7374 7970 6528 696e  result.astype(in
+00007580: 7429 0d0a 0d0a 0d0a 4072 6567 6973 7465  t)......@registe
+00007590: 725f 6675 6e63 7469 6f6e 286d 656e 753d  r_function(menu=
+000075a0: 2254 7261 6e73 666f 726d 7320 3e20 5265  "Transforms > Re
+000075b0: 7363 616c 6520 2873 6369 6b69 742d 696d  scale (scikit-im
+000075c0: 6167 652c 206e 7362 6174 776d 2922 290d  age, nsbatwm)").
+000075d0: 0a40 7469 6d65 5f73 6c69 6365 720d 0a64  .@time_slicer..d
+000075e0: 6566 2072 6573 6361 6c65 2869 6d61 6765  ef rescale(image
+000075f0: 3a20 226e 6170 6172 692e 7479 7065 732e  : "napari.types.
+00007600: 496d 6167 6544 6174 6122 2c0d 0a20 2020  ImageData",..   
+00007610: 2020 2020 2020 2020 2073 6361 6c65 5f78           scale_x
+00007620: 3a20 666c 6f61 7420 3d20 312e 302c 0d0a  : float = 1.0,..
+00007630: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+00007640: 655f 793a 2066 6c6f 6174 203d 2031 2e30  e_y: float = 1.0
+00007650: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00007660: 6361 6c65 5f7a 3a20 666c 6f61 7420 3d20  cale_z: float = 
+00007670: 312e 3029 202d 3e20 226e 6170 6172 692e  1.0) -> "napari.
+00007680: 7479 7065 732e 496d 6167 6544 6174 6122  types.ImageData"
+00007690: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
+000076a0: 5265 7363 616c 6520 616e 2069 6d61 6765  Rescale an image
+000076b0: 2062 7920 6120 6769 7665 6e20 7365 7420   by a given set 
+000076c0: 6f66 2073 6361 6c65 2066 6163 746f 7273  of scale factors
+000076d0: 2e0d 0a0d 0a20 2020 2050 6172 616d 6574  .....    Paramet
+000076e0: 6572 730d 0a20 2020 202d 2d2d 2d2d 2d2d  ers..    -------
+000076f0: 2d2d 2d0d 0a20 2020 2069 6d61 6765 203a  ---..    image :
+00007700: 2049 6d61 6765 4461 7461 0d0a 2020 2020   ImageData..    
+00007710: 7363 616c 655f 7820 3a20 666c 6f61 742c  scale_x : float,
+00007720: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00007730: 2020 2066 6163 746f 7220 6279 2077 6869     factor by whi
+00007740: 6368 2074 6f20 7363 616c 6520 7468 6520  ch to scale the 
+00007750: 696d 6167 6520 616c 6f6e 6720 7468 6520  image along the 
+00007760: 7820 6178 6973 2e20 5468 6520 6465 6661  x axis. The defa
+00007770: 756c 7420 6973 2031 2e30 2e0d 0a20 2020  ult is 1.0...   
+00007780: 2073 6361 6c65 5f79 203a 2066 6c6f 6174   scale_y : float
+00007790: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+000077a0: 2020 2020 6661 6374 6f72 2062 7920 7768      factor by wh
+000077b0: 6963 6820 746f 2073 6361 6c65 2074 6865  ich to scale the
+000077c0: 2069 6d61 6765 2061 6c6f 6e67 2074 6865   image along the
+000077d0: 2079 2064 696d 656e 7369 6f6e 2e20 5468   y dimension. Th
+000077e0: 6520 6465 6661 756c 7420 6973 2031 2e30  e default is 1.0
+000077f0: 2e0d 0a20 2020 2073 6361 6c65 5f7a 203a  ...    scale_z :
+00007800: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+00007810: 0d0a 2020 2020 2020 2020 6661 6374 6f72  ..        factor
+00007820: 2062 7920 7768 6963 6820 746f 2073 6361   by which to sca
+00007830: 6c65 2074 6865 2069 6d61 6765 2061 6c6f  le the image alo
+00007840: 6e67 2074 6865 207a 2064 696d 656e 7369  ng the z dimensi
+00007850: 6f6e 2e20 5468 6520 6465 6661 756c 7420  on. The default 
+00007860: 6973 2031 2e30 2e0d 0a0d 0a20 2020 2052  is 1.0.....    R
+00007870: 6574 7572 6e73 0d0a 2020 2020 2d2d 2d2d  eturns..    ----
+00007880: 2d2d 2d0d 0a20 2020 2049 6d61 6765 4461  ---..    ImageDa
+00007890: 7461 0d0a 0d0a 2020 2020 5365 6520 416c  ta....    See Al
+000078a0: 736f 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d  so..    --------
+000078b0: 0d0a 2020 2020 6874 7470 733a 2f2f 7363  ..    https://sc
+000078c0: 696b 6974 2d69 6d61 6765 2e6f 7267 2f64  ikit-image.org/d
+000078d0: 6f63 732f 7374 6162 6c65 2f61 7069 2f73  ocs/stable/api/s
+000078e0: 6b69 6d61 6765 2e74 7261 6e73 666f 726d  kimage.transform
+000078f0: 2e68 746d 6c23 7265 7363 616c 650d 0a20  .html#rescale.. 
+00007900: 2020 2022 2222 0d0a 2020 2020 6672 6f6d     """..    from
+00007910: 2073 6b69 6d61 6765 2069 6d70 6f72 7420   skimage import 
+00007920: 7472 616e 7366 6f72 6d0d 0a0d 0a20 2020  transform....   
+00007930: 2069 6620 6c65 6e28 696d 6167 652e 7368   if len(image.sh
+00007940: 6170 6529 203d 3d20 333a 0d0a 2020 2020  ape) == 3:..    
+00007950: 2020 2020 7363 616c 655f 6661 6374 6f72      scale_factor
+00007960: 7320 3d20 6e70 2e61 7361 7272 6179 285b  s = np.asarray([
+00007970: 7363 616c 655f 7a2c 2073 6361 6c65 5f79  scale_z, scale_y
+00007980: 2c20 7363 616c 655f 785d 290d 0a20 2020  , scale_x])..   
+00007990: 2065 6c69 6620 6c65 6e28 696d 6167 652e   elif len(image.
+000079a0: 7368 6170 6529 203d 3d20 323a 0d0a 2020  shape) == 2:..  
+000079b0: 2020 2020 2020 7363 616c 655f 6661 6374        scale_fact
+000079c0: 6f72 7320 3d20 6e70 2e61 7361 7272 6179  ors = np.asarray
+000079d0: 285b 7363 616c 655f 792c 2073 6361 6c65  ([scale_y, scale
+000079e0: 5f78 5d29 0d0a 2020 2020 656c 7365 3a0d  _x])..    else:.
+000079f0: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+00007a00: 616c 7565 4572 726f 7228 2252 6573 6361  alueError("Resca
+00007a10: 6c69 6e67 206f 6e6c 7920 7375 7070 6f72  ling only suppor
+00007a20: 7465 6420 666f 7220 3244 2061 6e64 2033  ted for 2D and 3
+00007a30: 4420 696d 6167 6573 2229 0d0a 0d0a 2020  D images")....  
+00007a40: 2020 7265 7475 726e 2074 7261 6e73 666f    return transfo
+00007a50: 726d 2e72 6573 6361 6c65 2869 6d61 6765  rm.rescale(image
+00007a60: 2c20 7363 616c 653d 7363 616c 655f 6661  , scale=scale_fa
+00007a70: 6374 6f72 732c 2070 7265 7365 7276 655f  ctors, preserve_
+00007a80: 7261 6e67 653d 5472 7565 290d 0a0d 0a0d  range=True).....
+00007a90: 0a40 7265 6769 7374 6572 5f66 756e 6374  .@register_funct
+00007aa0: 696f 6e28 6d65 6e75 3d22 5472 616e 7366  ion(menu="Transf
+00007ab0: 6f72 6d73 203e 2052 6573 697a 6520 2873  orms > Resize (s
+00007ac0: 6369 6b69 742d 696d 6167 652c 206e 7362  cikit-image, nsb
+00007ad0: 6174 776d 2922 290d 0a40 7469 6d65 5f73  atwm)")..@time_s
+00007ae0: 6c69 6365 720d 0a64 6566 2072 6573 697a  licer..def resiz
+00007af0: 6528 696d 6167 653a 2022 6e61 7061 7269  e(image: "napari
+00007b00: 2e74 7970 6573 2e49 6d61 6765 4461 7461  .types.ImageData
+00007b10: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00007b20: 6e65 775f 7769 6474 683a 2069 6e74 203d  new_width: int =
+00007b30: 2031 302e 302c 0d0a 2020 2020 2020 2020   10.0,..        
+00007b40: 2020 2020 6e65 775f 6865 6967 6874 3a20      new_height: 
+00007b50: 696e 7420 3d20 3130 2e30 2c0d 0a20 2020  int = 10.0,..   
+00007b60: 2020 2020 2020 2020 206e 6577 5f64 6570           new_dep
+00007b70: 7468 3a20 696e 7420 3d20 3130 2e30 2920  th: int = 10.0) 
+00007b80: 2d3e 2022 6e61 7061 7269 2e74 7970 6573  -> "napari.types
+00007b90: 2e49 6d61 6765 4461 7461 223a 0d0a 2020  .ImageData":..  
+00007ba0: 2020 2222 220d 0a20 2020 2052 6573 6361    """..    Resca
+00007bb0: 6c65 2061 6e20 696d 6167 6520 746f 2066  le an image to f
+00007bc0: 6974 2069 6e20 6120 6769 7665 6e20 6e65  it in a given ne
+00007bd0: 7720 7369 7a65 2e0d 0a0d 0a20 2020 2050  w size.....    P
+00007be0: 6172 616d 6574 6572 730d 0a20 2020 202d  arameters..    -
+00007bf0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2069  ---------..    i
+00007c00: 6d61 6765 203a 2049 6d61 6765 4461 7461  mage : ImageData
+00007c10: 0d0a 2020 2020 6e65 775f 7769 6474 6820  ..    new_width 
+00007c20: 3a20 696e 742c 206f 7074 696f 6e61 6c0d  : int, optional.
+00007c30: 0a20 2020 2020 2020 2066 6163 746f 7220  .        factor 
+00007c40: 6279 2077 6869 6368 2074 6f20 7363 616c  by which to scal
+00007c50: 6520 7468 6520 696d 6167 6520 616c 6f6e  e the image alon
+00007c60: 6720 7468 6520 7820 6178 6973 2e20 5468  g the x axis. Th
+00007c70: 6520 6465 6661 756c 7420 6973 2031 2e30  e default is 1.0
+00007c80: 2e0d 0a20 2020 206e 6577 5f68 6569 6768  ...    new_heigh
+00007c90: 7420 3a20 696e 742c 206f 7074 696f 6e61  t : int, optiona
+00007ca0: 6c0d 0a20 2020 2020 2020 2066 6163 746f  l..        facto
+00007cb0: 7220 6279 2077 6869 6368 2074 6f20 7363  r by which to sc
+00007cc0: 616c 6520 7468 6520 696d 6167 6520 616c  ale the image al
+00007cd0: 6f6e 6720 7468 6520 7920 6469 6d65 6e73  ong the y dimens
+00007ce0: 696f 6e2e 2054 6865 2064 6566 6175 6c74  ion. The default
+00007cf0: 2069 7320 312e 302e 0d0a 2020 2020 6e65   is 1.0...    ne
+00007d00: 775f 6465 7074 6820 3a20 696e 742c 206f  w_depth : int, o
+00007d10: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+00007d20: 2066 6163 746f 7220 6279 2077 6869 6368   factor by which
+00007d30: 2074 6f20 7363 616c 6520 7468 6520 696d   to scale the im
+00007d40: 6167 6520 616c 6f6e 6720 7468 6520 7a20  age along the z 
+00007d50: 6469 6d65 6e73 696f 6e2e 2054 6865 2064  dimension. The d
+00007d60: 6566 6175 6c74 2069 7320 312e 302e 0d0a  efault is 1.0...
+00007d70: 0d0a 2020 2020 5265 7475 726e 730d 0a20  ..    Returns.. 
+00007d80: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
+00007d90: 496d 6167 6544 6174 610d 0a0d 0a20 2020  ImageData....   
+00007da0: 2053 6565 2041 6c73 6f0d 0a20 2020 202d   See Also..    -
+00007db0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2068 7474  -------..    htt
+00007dc0: 7073 3a2f 2f73 6369 6b69 742d 696d 6167  ps://scikit-imag
+00007dd0: 652e 6f72 672f 646f 6373 2f73 7461 626c  e.org/docs/stabl
+00007de0: 652f 6170 692f 736b 696d 6167 652e 7472  e/api/skimage.tr
+00007df0: 616e 7366 6f72 6d2e 6874 6d6c 2372 6573  ansform.html#res
+00007e00: 697a 650d 0a20 2020 2022 2222 0d0a 2020  ize..    """..  
+00007e10: 2020 6672 6f6d 2073 6b69 6d61 6765 2069    from skimage i
+00007e20: 6d70 6f72 7420 7472 616e 7366 6f72 6d0d  mport transform.
+00007e30: 0a0d 0a20 2020 2069 6620 6c65 6e28 696d  ...    if len(im
+00007e40: 6167 652e 7368 6170 6529 203d 3d20 333a  age.shape) == 3:
+00007e50: 0d0a 2020 2020 2020 2020 6f75 7470 7574  ..        output
+00007e60: 5f73 6861 7065 203d 206e 702e 6173 6172  _shape = np.asar
+00007e70: 7261 7928 5b6e 6577 5f64 6570 7468 2c20  ray([new_depth, 
+00007e80: 6e65 775f 6865 6967 6874 2c20 6e65 775f  new_height, new_
+00007e90: 7769 6474 685d 290d 0a20 2020 2065 6c69  width])..    eli
+00007ea0: 6620 6c65 6e28 696d 6167 652e 7368 6170  f len(image.shap
+00007eb0: 6529 203d 3d20 323a 0d0a 2020 2020 2020  e) == 2:..      
+00007ec0: 2020 6f75 7470 7574 5f73 6861 7065 203d    output_shape =
+00007ed0: 206e 702e 6173 6172 7261 7928 5b6e 6577   np.asarray([new
+00007ee0: 5f68 6569 6768 742c 206e 6577 5f77 6964  _height, new_wid
+00007ef0: 7468 5d29 0d0a 2020 2020 656c 7365 3a0d  th])..    else:.
+00007f00: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+00007f10: 616c 7565 4572 726f 7228 2252 6573 697a  alueError("Resiz
+00007f20: 696e 6720 6f6e 6c79 2073 7570 706f 7274  ing only support
+00007f30: 6564 2066 6f72 2032 4420 616e 6420 3344  ed for 2D and 3D
+00007f40: 2069 6d61 6765 7322 290d 0a0d 0a20 2020   images")....   
+00007f50: 2072 6574 7572 6e20 7472 616e 7366 6f72   return transfor
+00007f60: 6d2e 7265 7369 7a65 2869 6d61 6765 2c20  m.resize(image, 
+00007f70: 6f75 7470 7574 5f73 6861 7065 2c20 7072  output_shape, pr
+00007f80: 6573 6572 7665 5f72 616e 6765 3d54 7275  eserve_range=Tru
+00007f90: 6529 0d0a 0d0a 0d0a 4072 6567 6973 7465  e)......@registe
+00007fa0: 725f 6675 6e63 7469 6f6e 286d 656e 753d  r_function(menu=
+00007fb0: 2255 7469 6c69 7469 6573 203e 204d 616e  "Utilities > Man
+00007fc0: 7561 6c6c 7920 6d65 7267 6520 6c61 6265  ually merge labe
+00007fd0: 6c73 2028 6e73 6261 7477 6d29 2229 0d0a  ls (nsbatwm)")..
+00007fe0: 6465 6620 4d61 6e75 616c 6c79 5f6d 6572  def Manually_mer
+00007ff0: 6765 5f6c 6162 656c 7328 6c61 6265 6c73  ge_labels(labels
+00008000: 5f6c 6179 6572 3a20 226e 6170 6172 692e  _layer: "napari.
+00008010: 6c61 7965 7273 2e4c 6162 656c 7322 2c20  layers.Labels", 
+00008020: 706f 696e 7473 5f6c 6179 6572 3a20 226e  points_layer: "n
+00008030: 6170 6172 692e 6c61 7965 7273 2e50 6f69  apari.layers.Poi
+00008040: 6e74 7322 2c20 7669 6577 6572 203a 2022  nts", viewer : "
+00008050: 6e61 7061 7269 2e56 6965 7765 7222 293a  napari.Viewer"):
+00008060: 0d0a 2020 2020 6966 2070 6f69 6e74 735f  ..    if points_
+00008070: 6c61 7965 7220 6973 204e 6f6e 653a 0d0a  layer is None:..
+00008080: 2020 2020 2020 2020 706f 696e 7473 5f6c          points_l
+00008090: 6179 6572 203d 2076 6965 7765 722e 6164  ayer = viewer.ad
+000080a0: 645f 706f 696e 7473 285b 5d29 0d0a 2020  d_points([])..  
+000080b0: 2020 2020 2020 706f 696e 7473 5f6c 6179        points_lay
+000080c0: 6572 2e6d 6f64 6520 3d20 2741 4444 270d  er.mode = 'ADD'.
+000080d0: 0a20 2020 2020 2020 2072 6574 7572 6e0d  .        return.
+000080e0: 0a20 2020 206c 6162 656c 7320 3d20 6e70  .    labels = np
+000080f0: 2e61 7361 7272 6179 286c 6162 656c 735f  .asarray(labels_
+00008100: 6c61 7965 722e 6461 7461 290d 0a20 2020  layer.data)..   
+00008110: 2070 6f69 6e74 7320 3d20 706f 696e 7473   points = points
+00008120: 5f6c 6179 6572 2e64 6174 610d 0a0d 0a20  _layer.data.... 
+00008130: 2020 206c 6162 656c 5f69 6473 203d 205b     label_ids = [
+00008140: 6c61 6265 6c73 2e69 7465 6d28 7475 706c  labels.item(tupl
+00008150: 6528 5b69 6e74 286a 2920 666f 7220 6a20  e([int(j) for j 
+00008160: 696e 2069 5d29 2920 666f 7220 6920 696e  in i])) for i in
+00008170: 2070 6f69 6e74 735d 0d0a 0d0a 2020 2020   points]....    
+00008180: 2320 7265 706c 6163 6520 6c61 6265 6c73  # replace labels
+00008190: 2077 6974 6820 6d69 6e69 6d75 6d20 6f66   with minimum of
+000081a0: 2074 6865 2073 656c 6563 7465 6420 6c61   the selected la
+000081b0: 6265 6c73 0d0a 2020 2020 6e65 775f 6c61  bels..    new_la
+000081c0: 6265 6c5f 6964 203d 206d 696e 286c 6162  bel_id = min(lab
+000081d0: 656c 5f69 6473 290d 0a20 2020 2066 6f72  el_ids)..    for
+000081e0: 206c 2069 6e20 6c61 6265 6c5f 6964 733a   l in label_ids:
+000081f0: 0d0a 2020 2020 2020 2020 6966 206c 2021  ..        if l !
+00008200: 3d20 6e65 775f 6c61 6265 6c5f 6964 3a0d  = new_label_id:.
+00008210: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00008220: 656c 735b 6c61 6265 6c73 203d 3d20 6c5d  els[labels == l]
+00008230: 203d 206e 6577 5f6c 6162 656c 5f69 640d   = new_label_id.
+00008240: 0a0d 0a20 2020 206c 6162 656c 735f 6c61  ...    labels_la
+00008250: 7965 722e 6461 7461 203d 206c 6162 656c  yer.data = label
+00008260: 730d 0a20 2020 2070 6f69 6e74 735f 6c61  s..    points_la
+00008270: 7965 722e 6461 7461 203d 205b 5d0d 0a0d  yer.data = []...
+00008280: 0a40 7265 6769 7374 6572 5f66 756e 6374  .@register_funct
+00008290: 696f 6e28 6d65 6e75 3d22 5574 696c 6974  ion(menu="Utilit
+000082a0: 6965 7320 3e20 4d61 6e75 616c 6c79 2073  ies > Manually s
+000082b0: 706c 6974 206c 6162 656c 7320 286e 7362  plit labels (nsb
+000082c0: 6174 776d 2922 290d 0a64 6566 204d 616e  atwm)")..def Man
+000082d0: 7561 6c6c 795f 7370 6c69 745f 6c61 6265  ually_split_labe
+000082e0: 6c73 286c 6162 656c 735f 6c61 7965 723a  ls(labels_layer:
+000082f0: 2022 6e61 7061 7269 2e6c 6179 6572 732e   "napari.layers.
+00008300: 4c61 6265 6c73 222c 2070 6f69 6e74 735f  Labels", points_
+00008310: 6c61 7965 723a 2022 6e61 7061 7269 2e6c  layer: "napari.l
+00008320: 6179 6572 732e 506f 696e 7473 222c 2076  ayers.Points", v
+00008330: 6965 7765 723a 2022 6e61 7061 7269 2e56  iewer: "napari.V
+00008340: 6965 7765 7222 293a 0d0a 2020 2020 6966  iewer"):..    if
+00008350: 2070 6f69 6e74 735f 6c61 7965 7220 6973   points_layer is
+00008360: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00008370: 706f 696e 7473 5f6c 6179 6572 203d 2076  points_layer = v
+00008380: 6965 7765 722e 6164 645f 706f 696e 7473  iewer.add_points
+00008390: 285b 5d29 0d0a 2020 2020 2020 2020 706f  ([])..        po
+000083a0: 696e 7473 5f6c 6179 6572 2e6d 6f64 6520  ints_layer.mode 
+000083b0: 3d20 2741 4444 270d 0a20 2020 2020 2020  = 'ADD'..       
+000083c0: 2072 6574 7572 6e0d 0a0d 0a20 2020 206c   return....    l
+000083d0: 6162 656c 7320 3d20 6e70 2e61 7361 7272  abels = np.asarr
+000083e0: 6179 286c 6162 656c 735f 6c61 7965 722e  ay(labels_layer.
+000083f0: 6461 7461 290d 0a20 2020 2070 6f69 6e74  data)..    point
+00008400: 7320 3d20 706f 696e 7473 5f6c 6179 6572  s = points_layer
+00008410: 2e64 6174 610d 0a0d 0a20 2020 206c 6162  .data....    lab
+00008420: 656c 5f69 6473 203d 205b 6c61 6265 6c73  el_ids = [labels
+00008430: 2e69 7465 6d28 7475 706c 6528 5b69 6e74  .item(tuple([int
+00008440: 286a 2920 666f 7220 6a20 696e 2069 5d29  (j) for j in i])
+00008450: 2920 666f 7220 6920 696e 2070 6f69 6e74  ) for i in point
+00008460: 735d 0d0a 0d0a 2020 2020 2320 6d61 6b65  s]....    # make
+00008470: 2061 2062 696e 6172 7920 696d 6167 6520   a binary image 
+00008480: 6669 7273 740d 0a20 2020 2062 696e 6172  first..    binar
+00008490: 7920 3d20 6e70 2e7a 6572 6f73 286c 6162  y = np.zeros(lab
+000084a0: 656c 732e 7368 6170 652c 2064 7479 7065  els.shape, dtype
+000084b0: 3d62 6f6f 6c29 0d0a 2020 2020 6e65 775f  =bool)..    new_
+000084c0: 6c61 6265 6c5f 6964 203d 206d 696e 286c  label_id = min(l
+000084d0: 6162 656c 5f69 6473 290d 0a20 2020 2066  abel_ids)..    f
+000084e0: 6f72 206c 2069 6e20 6c61 6265 6c5f 6964  or l in label_id
+000084f0: 733a 0d0a 2020 2020 2020 2020 6269 6e61  s:..        bina
+00008500: 7279 5b6c 6162 656c 7320 3d3d 206c 5d20  ry[labels == l] 
+00008510: 3d20 5472 7565 0d0a 0d0a 2020 2020 2320  = True....    # 
+00008520: 6f72 6967 696e 3a20 6874 7470 733a 2f2f  origin: https://
+00008530: 7363 696b 6974 2d69 6d61 6765 2e6f 7267  scikit-image.org
+00008540: 2f64 6f63 732f 6465 762f 6175 746f 5f65  /docs/dev/auto_e
+00008550: 7861 6d70 6c65 732f 7365 676d 656e 7461  xamples/segmenta
+00008560: 7469 6f6e 2f70 6c6f 745f 7761 7465 7273  tion/plot_waters
+00008570: 6865 642e 6874 6d6c 0d0a 2020 2020 6672  hed.html..    fr
+00008580: 6f6d 2073 6369 7079 2069 6d70 6f72 7420  om scipy import 
+00008590: 6e64 696d 6167 6520 6173 206e 6469 0d0a  ndimage as ndi..
+000085a0: 2020 2020 6672 6f6d 2073 6b69 6d61 6765      from skimage
+000085b0: 2e73 6567 6d65 6e74 6174 696f 6e20 696d  .segmentation im
+000085c0: 706f 7274 2077 6174 6572 7368 6564 0d0a  port watershed..
+000085d0: 2020 2020 2366 726f 6d20 736b 696d 6167      #from skimag
+000085e0: 652e 6665 6174 7572 6520 696d 706f 7274  e.feature import
+000085f0: 2070 6561 6b5f 6c6f 6361 6c5f 6d61 780d   peak_local_max.
+00008600: 0a0d 0a20 2020 2023 6469 7374 616e 6365  ...    #distance
+00008610: 203d 206e 6469 2e64 6973 7461 6e63 655f   = ndi.distance_
+00008620: 7472 616e 7366 6f72 6d5f 6564 7428 6269  transform_edt(bi
+00008630: 6e61 7279 290d 0a20 2020 2023 636f 6f72  nary)..    #coor
+00008640: 6473 203d 2070 6561 6b5f 6c6f 6361 6c5f  ds = peak_local_
+00008650: 6d61 7828 6469 7374 616e 6365 2c20 666f  max(distance, fo
+00008660: 6f74 7072 696e 743d 6e70 2e6f 6e65 7328  otprint=np.ones(
+00008670: 2833 2c20 3329 292c 206c 6162 656c 733d  (3, 3)), labels=
+00008680: 6269 6e61 7279 290d 0a20 2020 206d 6173  binary)..    mas
+00008690: 6b20 3d20 6e70 2e7a 6572 6f73 286c 6162  k = np.zeros(lab
+000086a0: 656c 732e 7368 6170 652c 2064 7479 7065  els.shape, dtype
+000086b0: 3d62 6f6f 6c29 0d0a 2020 2020 666f 7220  =bool)..    for 
+000086c0: 6920 696e 2070 6f69 6e74 733a 0d0a 2020  i in points:..  
+000086d0: 2020 2020 2020 236d 6173 6b5b 7475 706c        #mask[tupl
+000086e0: 6528 706f 696e 7473 295d 203d 2054 7275  e(points)] = Tru
+000086f0: 650d 0a20 2020 2020 2020 206d 6173 6b5b  e..        mask[
+00008700: 7475 706c 6528 5b69 6e74 286a 2920 666f  tuple([int(j) fo
+00008710: 7220 6a20 696e 2069 5d29 5d20 3d20 5472  r j in i])] = Tr
+00008720: 7565 0d0a 0d0a 2020 2020 6d61 726b 6572  ue....    marker
+00008730: 732c 205f 203d 206e 6469 2e6c 6162 656c  s, _ = ndi.label
+00008740: 286d 6173 6b29 0d0a 2020 2020 6e65 775f  (mask)..    new_
+00008750: 6c61 6265 6c73 203d 2077 6174 6572 7368  labels = watersh
+00008760: 6564 2862 696e 6172 792c 206d 6172 6b65  ed(binary, marke
+00008770: 7273 2c20 6d61 736b 3d62 696e 6172 7929  rs, mask=binary)
+00008780: 0d0a 2020 2020 6c61 6265 6c73 5b62 696e  ..    labels[bin
+00008790: 6172 795d 203d 206e 6577 5f6c 6162 656c  ary] = new_label
+000087a0: 735b 6269 6e61 7279 5d20 2b20 6c61 6265  s[binary] + labe
+000087b0: 6c73 2e6d 6178 2829 0d0a 0d0a 2020 2020  ls.max()....    
+000087c0: 6c61 6265 6c73 5f6c 6179 6572 2e64 6174  labels_layer.dat
+000087d0: 6120 3d20 6c61 6265 6c73 0d0a 2020 2020  a = labels..    
+000087e0: 706f 696e 7473 5f6c 6179 6572 2e64 6174  points_layer.dat
+000087f0: 6120 3d20 5b5d 0d0a 0d0a 0d0a 4072 6567  a = []......@reg
+00008800: 6973 7465 725f 6675 6e63 7469 6f6e 286d  ister_function(m
+00008810: 656e 753d 2246 696c 7465 7269 6e67 202f  enu="Filtering /
+00008820: 206e 6f69 7365 2072 656d 6f76 616c 203e   noise removal >
+00008830: 2042 7574 7465 7277 6f72 7468 2028 7363   Butterworth (sc
+00008840: 696b 6974 2d69 6d61 6765 2c20 6e73 6261  ikit-image, nsba
+00008850: 7477 6d29 2229 0d0a 406a 7570 7974 6572  twm)")..@jupyter
+00008860: 5f64 6973 706c 6179 6162 6c65 5f6f 7574  _displayable_out
+00008870: 7075 7428 6c69 6272 6172 795f 6e61 6d65  put(library_name
+00008880: 3d27 6e73 6261 7477 6d27 2c20 6865 6c70  ='nsbatwm', help
+00008890: 5f75 726c 3d27 6874 7470 733a 2f2f 7777  _url='https://ww
+000088a0: 772e 6e61 7061 7269 2d68 7562 2e6f 7267  w.napari-hub.org
+000088b0: 2f70 6c75 6769 6e73 2f6e 6170 6172 692d  /plugins/napari-
+000088c0: 7365 676d 656e 742d 626c 6f62 732d 616e  segment-blobs-an
+000088d0: 642d 7468 696e 6773 2d77 6974 682d 6d65  d-things-with-me
+000088e0: 6d62 7261 6e65 7327 290d 0a40 7469 6d65  mbranes')..@time
+000088f0: 5f73 6c69 6365 720d 0a64 6566 2062 7574  _slicer..def but
+00008900: 7465 7277 6f72 7468 2869 6d61 6765 3a20  terworth(image: 
+00008910: 226e 6170 6172 692e 7479 7065 732e 496d  "napari.types.Im
+00008920: 6167 6544 6174 6122 2c20 6375 746f 6666  ageData", cutoff
+00008930: 5f66 7265 7175 656e 6379 5f72 6174 696f  _frequency_ratio
+00008940: 3a20 666c 6f61 7420 3d20 302e 3030 352c  : float = 0.005,
+00008950: 2068 6967 685f 7061 7373 3a20 626f 6f6c   high_pass: bool
+00008960: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
+00008970: 2020 2020 2020 2020 2020 206f 7264 6572             order
+00008980: 3a20 666c 6f61 7420 3d20 3229 202d 3e20  : float = 2) -> 
+00008990: 226e 6170 6172 692e 7479 7065 732e 496d  "napari.types.Im
+000089a0: 6167 6544 6174 6122 3a0d 0a20 2020 2022  ageData":..    "
+000089b0: 2222 4170 706c 7920 6120 4275 7474 6572  ""Apply a Butter
+000089c0: 776f 7274 6820 6669 6c74 6572 2074 6f20  worth filter to 
+000089d0: 656e 6861 6e63 6520 6869 6768 206f 7220  enhance high or 
+000089e0: 6c6f 7720 6672 6571 7565 6e63 7920 6665  low frequency fe
+000089f0: 6174 7572 6573 2e0d 0a0d 0a20 2020 2054  atures.....    T
+00008a00: 6869 7320 6669 6c74 6572 2069 7320 6465  his filter is de
+00008a10: 6669 6e65 6420 696e 2074 6865 2046 6f75  fined in the Fou
+00008a20: 7269 6572 2064 6f6d 6169 6e2e 0d0a 0d0a  rier domain.....
+00008a30: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
+00008a40: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00008a50: 2020 2020 696d 6167 6520 3a20 284d 5b2c      image : (M[,
+00008a60: 204e 5b2c 202e 2e2e 2c20 505d 5d5b 2c20   N[, ..., P]][, 
+00008a70: 435d 2920 6e64 6172 7261 790d 0a20 2020  C]) ndarray..   
+00008a80: 2020 2020 2049 6e70 7574 2069 6d61 6765       Input image
+00008a90: 2e0d 0a20 2020 2063 7574 6f66 665f 6672  ...    cutoff_fr
+00008aa0: 6571 7565 6e63 795f 7261 7469 6f20 3a20  equency_ratio : 
+00008ab0: 666c 6f61 742c 206f 7074 696f 6e61 6c0d  float, optional.
+00008ac0: 0a20 2020 2020 2020 2044 6574 6572 6d69  .        Determi
+00008ad0: 6e65 7320 7468 6520 706f 7369 7469 6f6e  nes the position
+00008ae0: 206f 6620 7468 6520 6375 742d 6f66 6620   of the cut-off 
+00008af0: 7265 6c61 7469 7665 2074 6f20 7468 6520  relative to the 
+00008b00: 7368 6170 6520 6f66 2074 6865 0d0a 2020  shape of the..  
+00008b10: 2020 2020 2020 4646 542e 0d0a 2020 2020        FFT...    
+00008b20: 6869 6768 5f70 6173 7320 3a20 626f 6f6c  high_pass : bool
+00008b30: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00008b40: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
+00008b50: 6572 666f 726d 2061 2068 6967 6820 7061  erform a high pa
+00008b60: 7373 2066 696c 7465 722e 2049 6620 4661  ss filter. If Fa
+00008b70: 6c73 652c 2061 206c 6f77 2070 6173 7320  lse, a low pass 
+00008b80: 6669 6c74 6572 2069 730d 0a20 2020 2020  filter is..     
+00008b90: 2020 2070 6572 666f 726d 6564 2e0d 0a20     performed... 
+00008ba0: 2020 206f 7264 6572 203a 2066 6c6f 6174     order : float
+00008bb0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00008bc0: 2020 2020 4f72 6465 7220 6f66 2074 6865      Order of the
+00008bd0: 2066 696c 7465 7220 7768 6963 6820 6166   filter which af
+00008be0: 6665 6374 7320 7468 6520 736c 6f70 6520  fects the slope 
+00008bf0: 6e65 6172 2074 6865 2063 7574 2d6f 6666  near the cut-off
+00008c00: 2e20 4869 6768 6572 0d0a 2020 2020 2020  . Higher..      
+00008c10: 2020 6f72 6465 7220 6d65 616e 7320 7374    order means st
+00008c20: 6565 7065 7220 736c 6f70 6520 696e 2066  eeper slope in f
+00008c30: 7265 7175 656e 6379 2073 7061 6365 2e0d  requency space..
+00008c40: 0a0d 0a20 2020 2053 6565 2061 6c73 6f0d  ...    See also.
+00008c50: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20  .    --------.. 
+00008c60: 2020 202e 2e5b 305d 2068 7474 7073 3a2f     ..[0] https:/
+00008c70: 2f73 6369 6b69 742d 696d 6167 652e 6f72  /scikit-image.or
+00008c80: 672f 646f 6373 2f73 7461 626c 652f 6170  g/docs/stable/ap
+00008c90: 692f 736b 696d 6167 652e 6669 6c74 6572  i/skimage.filter
+00008ca0: 732e 6874 6d6c 2373 6b69 6d61 6765 2e66  s.html#skimage.f
+00008cb0: 696c 7465 7273 2e62 7574 7465 7277 6f72  ilters.butterwor
+00008cc0: 7468 0d0a 2020 2020 2222 220d 0a20 2020  th..    """..   
+00008cd0: 2066 726f 6d20 736b 696d 6167 652e 6669   from skimage.fi
+00008ce0: 6c74 6572 7320 696d 706f 7274 2062 7574  lters import but
+00008cf0: 7465 7277 6f72 7468 2061 7320 736b 696d  terworth as skim
+00008d00: 6167 655f 6275 7474 6572 776f 7274 680d  age_butterworth.
+00008d10: 0a20 2020 2072 6574 7572 6e20 736b 696d  .    return skim
+00008d20: 6167 655f 6275 7474 6572 776f 7274 6828  age_butterworth(
+00008d30: 696d 6167 652c 2063 7574 6f66 665f 6672  image, cutoff_fr
+00008d40: 6571 7565 6e63 795f 7261 7469 6f2c 2068  equency_ratio, h
+00008d50: 6967 685f 7061 7373 2c20 6f72 6465 7229  igh_pass, order)
+00008d60: 0d0a 0d0a 4072 6567 6973 7465 725f 6675  ....@register_fu
+00008d70: 6e63 7469 6f6e 286d 656e 753d 2253 6567  nction(menu="Seg
+00008d80: 6d65 6e74 6174 696f 6e20 706f 7374 2d70  mentation post-p
+00008d90: 726f 6365 7373 696e 6720 3e20 5265 6c61  rocessing > Rela
+00008da0: 6265 6c20 7365 7175 656e 7469 616c 2028  bel sequential (
+00008db0: 7363 696b 6974 2d69 6d61 6765 2c20 6e73  scikit-image, ns
+00008dc0: 6261 7477 6d29 2229 0d0a 406a 7570 7974  batwm)")..@jupyt
+00008dd0: 6572 5f64 6973 706c 6179 6162 6c65 5f6f  er_displayable_o
+00008de0: 7574 7075 7428 6c69 6272 6172 795f 6e61  utput(library_na
+00008df0: 6d65 3d27 6e73 6261 7477 6d27 2c20 6865  me='nsbatwm', he
+00008e00: 6c70 5f75 726c 3d27 6874 7470 733a 2f2f  lp_url='https://
+00008e10: 7777 772e 6e61 7061 7269 2d68 7562 2e6f  www.napari-hub.o
+00008e20: 7267 2f70 6c75 6769 6e73 2f6e 6170 6172  rg/plugins/napar
+00008e30: 692d 7365 676d 656e 742d 626c 6f62 732d  i-segment-blobs-
+00008e40: 616e 642d 7468 696e 6773 2d77 6974 682d  and-things-with-
+00008e50: 6d65 6d62 7261 6e65 7327 290d 0a40 7469  membranes')..@ti
+00008e60: 6d65 5f73 6c69 6365 720d 0a64 6566 2072  me_slicer..def r
+00008e70: 656c 6162 656c 5f73 6571 7565 6e74 6961  elabel_sequentia
+00008e80: 6c28 6c61 6265 6c5f 696d 6167 653a 226e  l(label_image:"n
+00008e90: 6170 6172 692e 7479 7065 732e 4c61 6265  apari.types.Labe
+00008ea0: 6c73 4461 7461 2229 202d 3e20 226e 6170  lsData") -> "nap
+00008eb0: 6172 692e 7479 7065 732e 4c61 6265 6c73  ari.types.Labels
+00008ec0: 4461 7461 223a 0d0a 2020 2020 2222 2252  Data":..    """R
+00008ed0: 656c 6162 656c 2061 206c 6162 656c 2069  elabel a label i
+00008ee0: 6d61 6765 2073 6571 7565 6e74 6961 6c6c  mage sequentiall
+00008ef0: 7922 2222 0d0a 2020 2020 7265 7475 726e  y"""..    return
+00008f00: 2073 6b5f 7265 6c61 6265 6c5f 7365 7175   sk_relabel_sequ
+00008f10: 656e 7469 616c 286c 6162 656c 5f69 6d61  ential(label_ima
+00008f20: 6765 295b 305d 0d0a 0d0a 0d0a 4072 6567  ge)[0]......@reg
+00008f30: 6973 7465 725f 6675 6e63 7469 6f6e 286d  ister_function(m
+00008f40: 656e 753d 2255 7469 6c69 7469 6573 203e  enu="Utilities >
+00008f50: 2045 7874 7261 6374 2073 6c69 6365 2028   Extract slice (
+00008f60: 6e73 6261 7477 6d29 2229 0d0a 4072 6567  nsbatwm)")..@reg
+00008f70: 6973 7465 725f 6675 6e63 7469 6f6e 286d  ister_function(m
+00008f80: 656e 753d 2254 7261 6e73 666f 726d 7320  enu="Transforms 
+00008f90: 3e20 4578 7472 6163 7420 736c 6963 6520  > Extract slice 
+00008fa0: 286e 7362 6174 776d 2922 290d 0a40 6a75  (nsbatwm)")..@ju
+00008fb0: 7079 7465 725f 6469 7370 6c61 7961 626c  pyter_displayabl
+00008fc0: 655f 6f75 7470 7574 286c 6962 7261 7279  e_output(library
+00008fd0: 5f6e 616d 653d 276e 7362 6174 776d 272c  _name='nsbatwm',
+00008fe0: 2068 656c 705f 7572 6c3d 2768 7474 7073   help_url='https
+00008ff0: 3a2f 2f77 7777 2e6e 6170 6172 692d 6875  ://www.napari-hu
+00009000: 622e 6f72 672f 706c 7567 696e 732f 6e61  b.org/plugins/na
+00009010: 7061 7269 2d73 6567 6d65 6e74 2d62 6c6f  pari-segment-blo
+00009020: 6273 2d61 6e64 2d74 6869 6e67 732d 7769  bs-and-things-wi
+00009030: 7468 2d6d 656d 6272 616e 6573 2729 0d0a  th-membranes')..
+00009040: 4074 696d 655f 736c 6963 6572 0d0a 6465  @time_slicer..de
+00009050: 6620 6578 7472 6163 745f 736c 6963 6528  f extract_slice(
+00009060: 696d 6167 653a 226e 6170 6172 692e 7479  image:"napari.ty
+00009070: 7065 732e 496d 6167 6544 6174 6122 2c20  pes.ImageData", 
+00009080: 736c 6963 655f 696e 6465 783a 696e 7420  slice_index:int 
+00009090: 3d20 302c 2061 7869 733a 696e 7420 3d20  = 0, axis:int = 
+000090a0: 3029 202d 3e20 226e 6170 6172 692e 7479  0) -> "napari.ty
+000090b0: 7065 732e 496d 6167 6544 6174 6122 3a0d  pes.ImageData":.
+000090c0: 0a20 2020 2022 2222 4578 7472 6163 7420  .    """Extract 
+000090d0: 2874 616b 6529 2061 2073 6c69 6365 2066  (take) a slice f
+000090e0: 726f 6d20 6120 7374 6163 6b2e 0d0a 0d0a  rom a stack.....
+000090f0: 2020 2020 5365 6520 616c 736f 0d0a 2020      See also..  
+00009100: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
+00009110: 2e2e 5b30 5d20 6874 7470 733a 2f2f 6e75  ..[0] https://nu
+00009120: 6d70 792e 6f72 672f 646f 632f 7374 6162  mpy.org/doc/stab
+00009130: 6c65 2f72 6566 6572 656e 6365 2f67 656e  le/reference/gen
+00009140: 6572 6174 6564 2f6e 756d 7079 2e74 616b  erated/numpy.tak
+00009150: 652e 6874 6d6c 0d0a 2020 2020 2222 220d  e.html..    """.
+00009160: 0a20 2020 2072 6574 7572 6e20 6e70 2e74  .    return np.t
+00009170: 616b 6528 696d 6167 652c 2073 6c69 6365  ake(image, slice
+00009180: 5f69 6e64 6578 2c20 6178 6973 3d61 7869  _index, axis=axi
+00009190: 7329 0d0a 0d0a 0d0a 4072 6567 6973 7465  s)......@registe
+000091a0: 725f 6675 6e63 7469 6f6e 286d 656e 753d  r_function(menu=
+000091b0: 2254 7261 6e73 666f 726d 7320 3e20 5375  "Transforms > Su
+000091c0: 622d 7361 6d70 6c65 2028 6e73 6261 7477  b-sample (nsbatw
+000091d0: 6d29 2229 0d0a 406a 7570 7974 6572 5f64  m)")..@jupyter_d
+000091e0: 6973 706c 6179 6162 6c65 5f6f 7574 7075  isplayable_outpu
+000091f0: 7428 6c69 6272 6172 795f 6e61 6d65 3d27  t(library_name='
+00009200: 6e73 6261 7477 6d27 2c20 6865 6c70 5f75  nsbatwm', help_u
+00009210: 726c 3d27 6874 7470 733a 2f2f 7777 772e  rl='https://www.
+00009220: 6e61 7061 7269 2d68 7562 2e6f 7267 2f70  napari-hub.org/p
+00009230: 6c75 6769 6e73 2f6e 6170 6172 692d 7365  lugins/napari-se
+00009240: 676d 656e 742d 626c 6f62 732d 616e 642d  gment-blobs-and-
+00009250: 7468 696e 6773 2d77 6974 682d 6d65 6d62  things-with-memb
+00009260: 7261 6e65 7327 290d 0a40 7469 6d65 5f73  ranes')..@time_s
+00009270: 6c69 6365 720d 0a64 6566 2073 7562 5f73  licer..def sub_s
+00009280: 616d 706c 6528 696d 6167 653a 226e 6170  ample(image:"nap
+00009290: 6172 692e 7479 7065 732e 496d 6167 6544  ari.types.ImageD
+000092a0: 6174 6122 2c20 7361 6d70 6c65 5f78 3a20  ata", sample_x: 
+000092b0: 696e 7420 3d20 312c 2073 616d 706c 655f  int = 1, sample_
+000092c0: 793a 2069 6e74 203d 2031 2c20 7361 6d70  y: int = 1, samp
+000092d0: 6c65 5f7a 3a20 696e 7420 3d20 3129 202d  le_z: int = 1) -
+000092e0: 3e20 226e 6170 6172 692e 7479 7065 732e  > "napari.types.
+000092f0: 496d 6167 6544 6174 6122 3a0d 0a20 2020  ImageData":..   
+00009300: 2022 2222 5361 6d70 6c65 2065 7665 7279   """Sample every
+00009310: 206e 7468 2070 6978 656c 2069 6e20 782c   nth pixel in x,
+00009320: 2079 2061 6e64 207a 2e22 2222 0d0a 2020   y and z."""..  
+00009330: 2020 6966 206c 656e 2869 6d61 6765 2e73    if len(image.s
+00009340: 6861 7065 2920 3d3d 2032 3a0d 0a20 2020  hape) == 2:..   
+00009350: 2020 2020 2072 6574 7572 6e20 696d 6167       return imag
+00009360: 655b 3a3a 7361 6d70 6c65 5f79 2c20 3a3a  e[::sample_y, ::
+00009370: 7361 6d70 6c65 5f78 5d0d 0a20 2020 2065  sample_x]..    e
+00009380: 6c69 6620 6c65 6e28 696d 6167 652e 7368  lif len(image.sh
+00009390: 6170 6529 203d 3d20 333a 0d0a 2020 2020  ape) == 3:..    
+000093a0: 2020 2020 7265 7475 726e 2069 6d61 6765      return image
+000093b0: 5b3a 3a73 616d 706c 655f 7a2c 203a 3a73  [::sample_z, ::s
+000093c0: 616d 706c 655f 792c 203a 3a73 616d 706c  ample_y, ::sampl
+000093d0: 655f 785d 0d0a 2020 2020 656c 7365 3a0d  e_x]..    else:.
+000093e0: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+000093f0: 616c 7565 4572 726f 7228 2253 7562 2d73  alueError("Sub-s
+00009400: 616d 706c 696e 6720 6f6e 6c79 2073 7570  ampling only sup
+00009410: 706f 7274 6564 2066 6f72 2032 4420 616e  ported for 2D an
+00009420: 6420 3344 2069 6d61 6765 7322 290d 0a0d  d 3D images")...
+00009430: 0a                                       .
```

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes/_tests/test_function.py` & `napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/_tests/test_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,16 @@
         multiply_images,\
         divide_images,\
         invert_image, \
         skeletonize, \
         rescale, \
         resize, \
         butterworth, \
-        extract_slice
+        extract_slice, \
+        sub_sample
 
     import numpy as np
 
     image = np.asarray([[0, 1, 2, 3],
                         [2, 0, 1, 3],
                         [2, 253, 1, 3],
                         [255, 253, 1, 3]])
@@ -69,17 +70,18 @@
         percentile_filter,
         black_tophat,
         white_tophat,
         morphological_gradient,
         local_minima_seeded_watershed,
         invert_image,
         rescale,
-        resize.
+        resize,
         butterworth,
-        extract_slice]:
+        extract_slice,
+        sub_sample]:
 
         print(operation)
 
         operation(image)
 
     for operation in [
         seeded_watershed,
@@ -137,7 +139,20 @@
     result = connected_component_labeling(image, exclude_on_edges=True)
 
     print(result)
     print(reference)
 
     assert np.array_equal(result, reference)
 
+
+def test_relabel_sequential():
+    image = np.asarray([[0, 0, 0, 1, 3, 4]])
+    reference = np.asarray([[0, 0, 0, 1, 2, 3]])
+
+    from napari_segment_blobs_and_things_with_membranes import relabel_sequential
+    result = relabel_sequential(image)
+
+    print(result)
+    print(reference)
+
+    assert np.array_equal(result, reference)
+
```

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes.egg-info/PKG-INFO` & `napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-blobs-and-things-with-membranes
-Version: 0.3.4
+Version: 0.3.5
 Summary: A plugin based on scikit-image for segmenting nuclei and cells based on fluorescent microscopy images with high intensity in nuclei and/or membranes
 Home-page: https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes#README.md
```

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.4/napari_segment_blobs_and_things_with_membranes.egg-info/SOURCES.txt` & `napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.4/setup.cfg` & `napari-segment-blobs-and-things-with-membranes-0.3.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 7365 676d 656e   = napari-segmen
 00000020: 742d 626c 6f62 732d 616e 642d 7468 696e  t-blobs-and-thin
 00000030: 6773 2d77 6974 682d 6d65 6d62 7261 6e65  gs-with-membrane
 00000040: 730d 0a76 6572 7369 6f6e 203d 2030 2e33  s..version = 0.3
-00000050: 2e34 0d0a 6175 7468 6f72 203d 2052 6f62  .4..author = Rob
+00000050: 2e35 0d0a 6175 7468 6f72 203d 2052 6f62  .5..author = Rob
 00000060: 6572 7420 4861 6173 650d 0a61 7574 686f  ert Haase..autho
 00000070: 725f 656d 6169 6c20 3d20 726f 6265 7274  r_email = robert
 00000080: 2e68 6161 7365 4074 752d 6472 6573 6465  .haase@tu-dresde
 00000090: 6e2e 6465 0d0a 7572 6c20 3d20 6874 7470  n.de..url = http
 000000a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
 000000b0: 6165 736c 6569 6e68 7565 7066 2f6e 6170  aesleinhuepf/nap
 000000c0: 6172 692d 7365 676d 656e 742d 626c 6f62  ari-segment-blob
```

