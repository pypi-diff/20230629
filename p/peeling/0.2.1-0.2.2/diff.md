# Comparing `tmp/peeling-0.2.1.tar.gz` & `tmp/peeling-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peeling-0.2.1.tar", last modified: Thu Jun  8 13:06:37 2023, max compression
+gzip compressed data, was "peeling-0.2.2.tar", last modified: Thu Jun 29 20:34:55 2023, max compression
```

## Comparing `peeling-0.2.1.tar` & `peeling-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-08 13:06:37.075630 peeling-0.2.1/
--rw-r--r--   0 clementsj   (503) staff       (20)     1518 2023-05-16 19:45:54.000000 peeling-0.2.1/LICENSE
--rw-r--r--   0 clementsj   (503) staff       (20)     9334 2023-06-08 13:06:37.075475 peeling-0.2.1/PKG-INFO
--rw-r--r--   0 clementsj   (503) staff       (20)     7202 2023-06-07 13:14:59.000000 peeling-0.2.1/README.md
-drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-08 13:06:37.074262 peeling-0.2.1/peeling/
--rw-r--r--   0 clementsj   (503) staff       (20)        0 2023-05-16 19:45:54.000000 peeling-0.2.1/peeling/__init__.py
--rw-r--r--   0 clementsj   (503) staff       (20)     3169 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/cellular_compartments.py
--rw-r--r--   0 clementsj   (503) staff       (20)     1337 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/clipantherprocessor.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     6492 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/cliprocessor.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)      267 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/cliuniprotcommunicator.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     3464 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/cliuserinputreader.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     4803 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/main.py
--rw-r--r--   0 clementsj   (503) staff       (20)     6156 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/pantherprocessor.py
--rw-r--r--   0 clementsj   (503) staff       (20)    10823 2023-06-07 18:35:54.000000 peeling-0.2.1/peeling/processor.py
--rw-r--r--   0 clementsj   (503) staff       (20)    12249 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/uniprotcommunicator.py
--rw-r--r--   0 clementsj   (503) staff       (20)     2256 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/userinputreader.py
--rw-r--r--   0 clementsj   (503) staff       (20)     1595 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/webpantherprocessor.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     5620 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/webprocessor.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     6498 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/webuniprotcommunicator.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     1110 2023-06-07 18:42:16.000000 peeling-0.2.1/peeling/webuserinputreader.py
-drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-08 13:06:37.075076 peeling-0.2.1/peeling.egg-info/
--rw-r--r--   0 clementsj   (503) staff       (20)     9334 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/PKG-INFO
--rw-r--r--   0 clementsj   (503) staff       (20)      647 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/SOURCES.txt
--rw-r--r--   0 clementsj   (503) staff       (20)        1 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/dependency_links.txt
--rw-r--r--   0 clementsj   (503) staff       (20)       46 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/entry_points.txt
--rw-r--r--   0 clementsj   (503) staff       (20)      522 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/requires.txt
--rw-r--r--   0 clementsj   (503) staff       (20)        8 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/top_level.txt
--rw-r--r--   0 clementsj   (503) staff       (20)     1479 2023-06-08 12:57:26.000000 peeling-0.2.1/pyproject.toml
--rw-r--r--   0 clementsj   (503) staff       (20)       38 2023-06-08 13:06:37.075665 peeling-0.2.1/setup.cfg
-drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-08 13:06:37.075181 peeling-0.2.1/test/
--rw-r--r--   0 clementsj   (503) staff       (20)    15513 2023-05-16 19:45:54.000000 peeling-0.2.1/test/test.py
+drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-29 20:34:55.727373 peeling-0.2.2/
+-rw-r--r--   0 clementsj   (503) staff       (20)     1518 2023-05-16 19:45:54.000000 peeling-0.2.2/LICENSE
+-rw-r--r--   0 clementsj   (503) staff       (20)     9140 2023-06-29 20:34:55.727216 peeling-0.2.2/PKG-INFO
+-rw-r--r--   0 clementsj   (503) staff       (20)     7008 2023-06-29 19:26:11.000000 peeling-0.2.2/README.md
+drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-29 20:34:55.725899 peeling-0.2.2/peeling/
+-rw-r--r--   0 clementsj   (503) staff       (20)        0 2023-05-16 19:45:54.000000 peeling-0.2.2/peeling/__init__.py
+-rw-r--r--   0 clementsj   (503) staff       (20)     3169 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/cellular_compartments.py
+-rw-r--r--   0 clementsj   (503) staff       (20)     1337 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/clipantherprocessor.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     6492 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/cliprocessor.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)      267 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/cliuniprotcommunicator.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     3606 2023-06-29 18:22:08.000000 peeling-0.2.2/peeling/cliuserinputreader.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     4798 2023-06-28 14:01:23.000000 peeling-0.2.2/peeling/main.py
+-rw-r--r--   0 clementsj   (503) staff       (20)     6156 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/pantherprocessor.py
+-rw-r--r--   0 clementsj   (503) staff       (20)    10929 2023-06-29 18:18:33.000000 peeling-0.2.2/peeling/processor.py
+-rw-r--r--   0 clementsj   (503) staff       (20)    12249 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/uniprotcommunicator.py
+-rw-r--r--   0 clementsj   (503) staff       (20)     2256 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/userinputreader.py
+-rw-r--r--   0 clementsj   (503) staff       (20)     1595 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/webpantherprocessor.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     5478 2023-06-29 18:37:23.000000 peeling-0.2.2/peeling/webprocessor.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     6498 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/webuniprotcommunicator.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     1110 2023-06-07 18:42:16.000000 peeling-0.2.2/peeling/webuserinputreader.py
+drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-29 20:34:55.726774 peeling-0.2.2/peeling.egg-info/
+-rw-r--r--   0 clementsj   (503) staff       (20)     9140 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/PKG-INFO
+-rw-r--r--   0 clementsj   (503) staff       (20)      647 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/SOURCES.txt
+-rw-r--r--   0 clementsj   (503) staff       (20)        1 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/dependency_links.txt
+-rw-r--r--   0 clementsj   (503) staff       (20)       46 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/entry_points.txt
+-rw-r--r--   0 clementsj   (503) staff       (20)      522 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/requires.txt
+-rw-r--r--   0 clementsj   (503) staff       (20)        8 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/top_level.txt
+-rw-r--r--   0 clementsj   (503) staff       (20)     1479 2023-06-29 18:44:27.000000 peeling-0.2.2/pyproject.toml
+-rw-r--r--   0 clementsj   (503) staff       (20)       38 2023-06-29 20:34:55.727410 peeling-0.2.2/setup.cfg
+drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-29 20:34:55.726899 peeling-0.2.2/test/
+-rw-r--r--   0 clementsj   (503) staff       (20)    15513 2023-05-16 19:45:54.000000 peeling-0.2.2/test/test.py
```

### Comparing `peeling-0.2.1/LICENSE` & `peeling-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/PKG-INFO` & `peeling-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peeling
-Version: 0.2.1
+Version: 0.2.2
 Author-email: HHMI Janelia <peeling@janelia.hhmi.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Howard Hughes Medical Institute
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -38,15 +38,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # PEELing
 
 
 ### Introduction
-In the evolutionary transition from unicellular to multicellular organisms, single cells assemble into highly organized tissues and cooperatively carry out physiological functions. To act as an integrated system, individual cells communicate with each other extensively through signaling at the cellular interface. Cell-surface signaling thus controls almost every aspect of the development, physiology, and pathogenesis of multicellular organisms. In situ cell-surface proteomics or `iPEEL` (in situ cell-surface proteome extraction by extracellular labeling; developed by [Li, Han et al., 2020](https://pubmed.ncbi.nlm.nih.gov/31955847/) — `PMID: 31955847` and [Shuster, Li et al., 2022](https://pubmed.ncbi.nlm.nih.gov/36220098/) — `PMID: 36220098`) provides a method for quantitatively profiling cell-surface proteomes in native tissues with cell-type and spatiotemporal specificities. 
+Molecular compartmentalization is vital for cellular physiology. Spatially-resolved proteomics allows biologists to survey protein composition and dynamics with subcellular resolution. Here, we present **PEELing** (***p***roteome ***e***xtraction from ***e***nzymatic ***l***abel***ing*** data), an integrated package and user-friendly web service for analyzing spatially-resolved proteomics data. PEELing assesses data quality using curated or user-defined references, performs cutoff analysis to remove contaminants, connects to databases for functional annotation, and generates data visualizations—providing a streamlined and reproducible workflow to explore spatially-resolved proteomics data.
 
 This `PEELing` program provides an automated, standardized, and easy-to-use analysis pipeline for iPEEL or any other cell-surface proteomics data. PEELing evaluates data quality using curated [Swiss-Prot](https://www.sib.swiss/swiss-prot)  references, performs cut-off analysis to remove contaminants (modified from [Hung et al., 2014](https://pubmed.ncbi.nlm.nih.gov/25002142/) — `PMID:  25002142`), connects to [UniProt](https://www.uniprot.org/) and [Panther](http://www.pantherdb.org/) databases for functional annotation, and generates data visualizations. Together with iPEEL transgenic tools (The Jackson Laboratory: 037697, 037698; Bloomington Drosophila Stock Center: 8763, 9906, 9908), PEELing enables a complete pipeline, from wet lab method to data analysis, for in situ cell-surface proteomics.
 
 `PEELing` also provides a web portal. Please refer to [link](http://peeling.janelia.org)
 
 
 ### Installation
```

### Comparing `peeling-0.2.1/README.md` & `peeling-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PEELing
 
 
 ### Introduction
-In the evolutionary transition from unicellular to multicellular organisms, single cells assemble into highly organized tissues and cooperatively carry out physiological functions. To act as an integrated system, individual cells communicate with each other extensively through signaling at the cellular interface. Cell-surface signaling thus controls almost every aspect of the development, physiology, and pathogenesis of multicellular organisms. In situ cell-surface proteomics or `iPEEL` (in situ cell-surface proteome extraction by extracellular labeling; developed by [Li, Han et al., 2020](https://pubmed.ncbi.nlm.nih.gov/31955847/) — `PMID: 31955847` and [Shuster, Li et al., 2022](https://pubmed.ncbi.nlm.nih.gov/36220098/) — `PMID: 36220098`) provides a method for quantitatively profiling cell-surface proteomes in native tissues with cell-type and spatiotemporal specificities. 
+Molecular compartmentalization is vital for cellular physiology. Spatially-resolved proteomics allows biologists to survey protein composition and dynamics with subcellular resolution. Here, we present **PEELing** (***p***roteome ***e***xtraction from ***e***nzymatic ***l***abel***ing*** data), an integrated package and user-friendly web service for analyzing spatially-resolved proteomics data. PEELing assesses data quality using curated or user-defined references, performs cutoff analysis to remove contaminants, connects to databases for functional annotation, and generates data visualizations—providing a streamlined and reproducible workflow to explore spatially-resolved proteomics data.
 
 This `PEELing` program provides an automated, standardized, and easy-to-use analysis pipeline for iPEEL or any other cell-surface proteomics data. PEELing evaluates data quality using curated [Swiss-Prot](https://www.sib.swiss/swiss-prot)  references, performs cut-off analysis to remove contaminants (modified from [Hung et al., 2014](https://pubmed.ncbi.nlm.nih.gov/25002142/) — `PMID:  25002142`), connects to [UniProt](https://www.uniprot.org/) and [Panther](http://www.pantherdb.org/) databases for functional annotation, and generates data visualizations. Together with iPEEL transgenic tools (The Jackson Laboratory: 037697, 037698; Bloomington Drosophila Stock Center: 8763, 9906, 9908), PEELing enables a complete pipeline, from wet lab method to data analysis, for in situ cell-surface proteomics.
 
 `PEELing` also provides a web portal. Please refer to [link](http://peeling.janelia.org)
 
 
 ### Installation
```

### Comparing `peeling-0.2.1/peeling/cellular_compartments.py` & `peeling-0.2.2/peeling/cellular_compartments.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/peeling/clipantherprocessor.py` & `peeling-0.2.2/peeling/clipantherprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/peeling/cliprocessor.py` & `peeling-0.2.2/peeling/cliprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/peeling/cliuserinputreader.py` & `peeling-0.2.2/peeling/cliuserinputreader.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,86 +17,88 @@
         self.__no_id_mapping = no_id_mapping
 
 
     def __read_file(self, filename):
         try:
             df = pd.read_table(filename, sep='\t', header=0)
         except UnicodeDecodeError as e1:
-            logger.error(e1) 
+            logger.error(e1)
             logger.error('Check the input file is tab delimited (.tsv)')
             raise
         except FileNotFoundError as e2:
             logger.error(e2)
             raise
-        
+
         self._check_file(df)
         return df
 
 
     # implement abstract method
     def get_mass_data(self):
         data = self.__read_file(self.__mass_filename)
         self._check_mass_spec_file(data)
         logger.info('Read in %d rows and %d columns from mass spec data' % data.shape)
         return data
-    
+
 
     # implement abstract method
     def get_mass_spec_filename(self):
         return self.__mass_filename
-    
+
 
     def get_latest_ids_filename(self):
         return self.__ids_filename
-    
+
 
     def get_true_positive_filename(self):
         return self.__true_positive_filename
-    
+
 
     def get_false_positive_filename(self):
         return self.__false_positive_filename
 
 
     def get_latest_ids(self):
         df = self.__read_file(self.__ids_filename)
         try:
             assert(df.shape[1] >= 2), 'Latest ids file should have at least two columns'
             logger.info('Read in %d rows from latest_ids file' % (len(df)))
             return df
         except AssertionError as e:
             logger.error(e)
             raise
-        
+
 
     def get_annotation_true_positive(self):
+        logger.debug('Reading from true positive file: %s' % (self.__true_positive_filename))
         df = self.__read_file(self.__true_positive_filename)
         try:
             assert(df.shape[1] >= 1), 'Annotation_true_positive file should have at least one column containing ids of proteins in your selected cellular compartment'
             logger.info('Read in %d rows from annotation_true_positive file' % (len(df)))
             return df
         except AssertionError as e:
             logger.error(e)
             raise
-       
+
 
     def get_annotation_false_positive(self):
+        logger.debug('Reading from false positive file: %s' % (self.__false_positive_filename))
         df = self.__read_file(self.__false_positive_filename)
         try:
             assert(df.shape[1] >= 1), 'Annotation_false_positive file should have at least one column containing ids of proteins that are not found in your selected cellular compartment'
             logger.info('Read in %d rows from annotation_false_positive file' % (len(df)))
             return df
         except AssertionError as e:
             logger.error(e)
             raise
 
-    
+
     def get_output_directory(self):
         return self.__output_directory
 
 
     def get_save(self):
         return self.__save
-    
+
 
     def get_id_mapping(self):
         return self.__no_id_mapping
```

### Comparing `peeling-0.2.1/peeling/main.py` & `peeling-0.2.2/peeling/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,11 +95,10 @@
         panther_processor = CliPantherProcessor(panther_organism, path)
         panther_processor.start()
 
     logger.info(f'Results saved at {path}')
     end_time = datetime.now()
     logger.info(f'{end_time} Analysis finished! Time: {end_time - start_time}')
 
-    
 
 if __name__ == "__main__":
     main()
```

### Comparing `peeling-0.2.1/peeling/pantherprocessor.py` & `peeling-0.2.2/peeling/pantherprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/peeling/processor.py` & `peeling-0.2.2/peeling/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,16 @@
         raise NotImplementedError()
 
 
     def __merge_annotation(self, mass_data, annotation, type):
         '''
         type: 'true_positive' or 'false_positive'
         '''
+        logger.debug(f'Adding annotation_{type} started.')
+        logger.debug(f'\n{annotation.head()}')
         annotation['Add'] = 1
         annotation.drop_duplicates(keep='first', inplace=True)
         annotation.dropna(axis=0, how='any', inplace=True)
         annotation.set_index('Entry', inplace=True)
 
         mass_data = mass_data.merge(annotation, how='left', left_index=True, right_index=True)
         new_col_name = 'TP' if type=='true_positive' else 'FP'
```

### Comparing `peeling-0.2.1/peeling/uniprotcommunicator.py` & `peeling-0.2.2/peeling/uniprotcommunicator.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/peeling/userinputreader.py` & `peeling-0.2.2/peeling/userinputreader.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/peeling/webpantherprocessor.py` & `peeling-0.2.2/peeling/webpantherprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/peeling/webprocessor.py` & `peeling-0.2.2/peeling/webprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 
     # implement abstract method
     async def _get_annotation_data(self, type):
         '''
         type: 'true_positive' or 'false_positive'
         '''
         annotation = await self._get_uniprot_communicator().get_annotation(type)
-        # logger.debug(f'\n{annotation.head()}')
+        annotation.columns = ['Entry']
+        logger.debug(f'\n{annotation.head()}')
         return annotation.copy()
 
 
     # implement abstract method
     def _plot_supplemental(self, fig_name): #plt,
         plt.savefig(f'{self.__web_plots_path}/{fig_name}.jpeg', dpi=130, bbox_inches='tight')
         plt.close()
@@ -89,16 +90,14 @@
         results_path = self._construct_path()
         data = self._mass_data_clean(data)
         columns = list(data.columns[1:])
         await self._analyze(data, results_path)
         self.__true_positive_proteins_raw_data.to_csv(f'../results/{self.__uuid}/post-cutoff-proteome_with_raw_data.tsv', sep='\t', index=False)
         self._write_args(results_path)
         logger.info(f'Results saved at {self.__uuid}')
-        #shutil.make_archive(f'../results/{self.__uuid}/results', 'zip', root_dir=f'../results/{self.__uuid}/results')
-        #shutil.rmtree(f'../results/{self.__uuid}/results')
         return  self.__uuid, self.__failed_id_mapping, columns
 
 
     def plot_scatter(self):
         try:
             parent_path = f'../results/{self.__uuid}'
             results_path = f'{parent_path}/results'
```

### Comparing `peeling-0.2.1/peeling/webuniprotcommunicator.py` & `peeling-0.2.2/peeling/webuniprotcommunicator.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/peeling/webuserinputreader.py` & `peeling-0.2.2/peeling/webuserinputreader.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/peeling.egg-info/PKG-INFO` & `peeling-0.2.2/peeling.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peeling
-Version: 0.2.1
+Version: 0.2.2
 Author-email: HHMI Janelia <peeling@janelia.hhmi.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Howard Hughes Medical Institute
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -38,15 +38,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # PEELing
 
 
 ### Introduction
-In the evolutionary transition from unicellular to multicellular organisms, single cells assemble into highly organized tissues and cooperatively carry out physiological functions. To act as an integrated system, individual cells communicate with each other extensively through signaling at the cellular interface. Cell-surface signaling thus controls almost every aspect of the development, physiology, and pathogenesis of multicellular organisms. In situ cell-surface proteomics or `iPEEL` (in situ cell-surface proteome extraction by extracellular labeling; developed by [Li, Han et al., 2020](https://pubmed.ncbi.nlm.nih.gov/31955847/) — `PMID: 31955847` and [Shuster, Li et al., 2022](https://pubmed.ncbi.nlm.nih.gov/36220098/) — `PMID: 36220098`) provides a method for quantitatively profiling cell-surface proteomes in native tissues with cell-type and spatiotemporal specificities. 
+Molecular compartmentalization is vital for cellular physiology. Spatially-resolved proteomics allows biologists to survey protein composition and dynamics with subcellular resolution. Here, we present **PEELing** (***p***roteome ***e***xtraction from ***e***nzymatic ***l***abel***ing*** data), an integrated package and user-friendly web service for analyzing spatially-resolved proteomics data. PEELing assesses data quality using curated or user-defined references, performs cutoff analysis to remove contaminants, connects to databases for functional annotation, and generates data visualizations—providing a streamlined and reproducible workflow to explore spatially-resolved proteomics data.
 
 This `PEELing` program provides an automated, standardized, and easy-to-use analysis pipeline for iPEEL or any other cell-surface proteomics data. PEELing evaluates data quality using curated [Swiss-Prot](https://www.sib.swiss/swiss-prot)  references, performs cut-off analysis to remove contaminants (modified from [Hung et al., 2014](https://pubmed.ncbi.nlm.nih.gov/25002142/) — `PMID:  25002142`), connects to [UniProt](https://www.uniprot.org/) and [Panther](http://www.pantherdb.org/) databases for functional annotation, and generates data visualizations. Together with iPEEL transgenic tools (The Jackson Laboratory: 037697, 037698; Bloomington Drosophila Stock Center: 8763, 9906, 9908), PEELing enables a complete pipeline, from wet lab method to data analysis, for in situ cell-surface proteomics.
 
 `PEELing` also provides a web portal. Please refer to [link](http://peeling.janelia.org)
 
 
 ### Installation
```

### Comparing `peeling-0.2.1/peeling.egg-info/SOURCES.txt` & `peeling-0.2.2/peeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/peeling.egg-info/requires.txt` & `peeling-0.2.2/peeling.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `peeling-0.2.1/pyproject.toml` & `peeling-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "peeling"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="HHMI Janelia", email="peeling@janelia.hhmi.org" },
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `peeling-0.2.1/test/test.py` & `peeling-0.2.2/test/test.py`

 * *Files identical despite different names*

