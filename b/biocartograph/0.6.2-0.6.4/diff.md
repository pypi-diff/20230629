# Comparing `tmp/biocartograph-0.6.2.tar.gz` & `tmp/biocartograph-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocartograph-0.6.2.tar", last modified: Wed Jun  7 09:18:17 2023, max compression
+gzip compressed data, was "biocartograph-0.6.4.tar", last modified: Thu Jun 29 12:43:09 2023, max compression
```

## Comparing `biocartograph-0.6.2.tar` & `biocartograph-0.6.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-07 09:18:17.767916 biocartograph-0.6.2/
--rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-06-01 15:35:36.000000 biocartograph-0.6.2/LICENSE
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-07 09:18:17.767916 biocartograph-0.6.2/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-06-01 15:35:36.000000 biocartograph-0.6.2/README.md
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-07 09:18:17.766916 biocartograph-0.6.2/biocartograph.egg-info/
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-07 09:18:17.000000 biocartograph-0.6.2/biocartograph.egg-info/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)      334 2023-06-07 09:18:17.000000 biocartograph-0.6.2/biocartograph.egg-info/SOURCES.txt
--rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-06-07 09:18:17.000000 biocartograph-0.6.2/biocartograph.egg-info/dependency_links.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-06-07 09:18:17.000000 biocartograph-0.6.2/biocartograph.egg-info/top_level.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-06-07 09:18:17.767916 biocartograph-0.6.2/setup.cfg
--rw-r--r--   0 rictjo    (1000) users      (100)      955 2023-06-07 09:15:40.000000 biocartograph-0.6.2/setup.py
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-07 09:18:17.766916 biocartograph-0.6.2/src/
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-07 09:18:17.767916 biocartograph-0.6.2/src/biocartograph/
--rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-06-01 15:35:36.000000 biocartograph-0.6.2/src/biocartograph/__init__.py
--rw-r--r--   0 rictjo    (1000) users      (100)     3334 2023-06-01 15:35:36.000000 biocartograph-0.6.2/src/biocartograph/composition.py
--rw-r--r--   0 rictjo    (1000) users      (100)    16747 2023-06-02 09:32:03.000000 biocartograph-0.6.2/src/biocartograph/enrichment.py
--rw-r--r--   0 rictjo    (1000) users      (100)    22401 2023-06-01 15:35:36.000000 biocartograph-0.6.2/src/biocartograph/quantification.py
--rw-r--r--   0 rictjo    (1000) users      (100)    26687 2023-06-07 09:15:40.000000 biocartograph-0.6.2/src/biocartograph/special.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-29 12:43:09.759631 biocartograph-0.6.4/
+-rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-06-01 15:35:36.000000 biocartograph-0.6.4/LICENSE
+-rw-r--r--   0 rictjo    (1000) users      (100)     9509 2023-06-29 12:43:09.759631 biocartograph-0.6.4/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)     8966 2023-06-29 12:37:39.000000 biocartograph-0.6.4/README.md
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-29 12:43:09.758631 biocartograph-0.6.4/biocartograph.egg-info/
+-rw-r--r--   0 rictjo    (1000) users      (100)     9509 2023-06-29 12:43:09.000000 biocartograph-0.6.4/biocartograph.egg-info/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)      334 2023-06-29 12:43:09.000000 biocartograph-0.6.4/biocartograph.egg-info/SOURCES.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-06-29 12:43:09.000000 biocartograph-0.6.4/biocartograph.egg-info/dependency_links.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-06-29 12:43:09.000000 biocartograph-0.6.4/biocartograph.egg-info/top_level.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-06-29 12:43:09.759631 biocartograph-0.6.4/setup.cfg
+-rw-r--r--   0 rictjo    (1000) users      (100)      955 2023-06-29 12:37:39.000000 biocartograph-0.6.4/setup.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-29 12:43:09.757631 biocartograph-0.6.4/src/
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-29 12:43:09.758631 biocartograph-0.6.4/src/biocartograph/
+-rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-06-01 15:35:36.000000 biocartograph-0.6.4/src/biocartograph/__init__.py
+-rw-r--r--   0 rictjo    (1000) users      (100)     3334 2023-06-29 08:30:04.000000 biocartograph-0.6.4/src/biocartograph/composition.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    18226 2023-06-29 12:37:39.000000 biocartograph-0.6.4/src/biocartograph/enrichment.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    22513 2023-06-29 12:37:39.000000 biocartograph-0.6.4/src/biocartograph/quantification.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    28048 2023-06-29 12:37:39.000000 biocartograph-0.6.4/src/biocartograph/special.py
```

### Comparing `biocartograph-0.6.2/LICENSE` & `biocartograph-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `biocartograph-0.6.2/setup.py` & `biocartograph-0.6.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name         = "biocartograph",
-    version      = "0.6.2",
+    version      = "0.6.4",
     author       = "Richard Tjörnhammar",
     author_email = "richard.tjornhammar@gmail.com",
     description  = "Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/rictjo/biocarta",
     packages = setuptools.find_packages('src'),
```

### Comparing `biocartograph-0.6.2/src/biocartograph/composition.py` & `biocartograph-0.6.4/src/biocartograph/composition.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.6.2/src/biocartograph/enrichment.py` & `biocartograph-0.6.4/src/biocartograph/enrichment.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import pandas as pd
 import numpy  as np
+import os
 
 def create_specificity_group_df ( acdf:pd.DataFrame , df_:pd.DataFrame , index_order:list=None ,
                                   label:str = '' , post_fix:str = '' , bSorted:bool=True , slab:str = 'Specificity Class' ,
                                   rename_cats:dict = { '0':'ND' , '1':'LS' , '2':'GE' , '3':'GR' , '4':'TR' } ) :
         from impetuous.quantification import group_classifications , composition_absolute, compositional_analysis
         from collections import Counter
-        lab1 = label
+        lab1		= label
         results		= group_classifications ( acdf.apply(pd.to_numeric) , bLog2=True )
         new		= [ {w:item[0] for w in item[1]} for item in results.items() ]
         lookup		= dict()
         for i in range(len(new)) :
             for item in new[i].items() :
                 lookup[item[0]] = item[1]
         #
@@ -147,54 +148,87 @@
     )
     fig.update_traces(root_color="lightgrey")
     fig.update_layout(margin = dict(t=50, l=25, r=25, b=25))
     fig.show()
     """
     return ( dag_maps )
 
-import pandas as pd
-import numpy  as np
-
 from biocartograph.composition import composition_leading_label_and_metric
+#
+def get_annotation_function(	header_str:str = '../results/DMHMSY_Fri_Jun__2_09_15_35_2023_'	,
+				auto_annotated_df:pd.DataFrame		= None 			,
+				significance_level:float                = 0.1			,
+				enrichment_file_pattern:str     = "(HEADER)treemap_c(CLUSTID).tsv" ) -> list[str] :
+    #
+    # ADD IN TOP ENRICHMENT AS FUNCTION
+    function = []
+    set_all_files = set( os.listdir( '/'.join(header_str.split('/')[:-1]) ) )
+    for cid in auto_annotated_df .index.values.tolist() :
+        filename        = enrichment_file_pattern.replace('(HEADER)',header_str).replace('(CLUSTID)',str(cid))
+        fn              = filename.split('/')[-1]
+        if not fn in set_all_files :
+            function.append( 'Unknown' )
+            continue
+        df              = pd.read_csv(filename,sep='\t',index_col=0)
+        if len(df) > 0 :
+            if df.iloc[ np.argmin( df.loc[:,'p-value'].values ) , : ].loc['p-value'] < significance_level :
+                function .append( df.iloc[ np.argmin( df.loc[:,'p-value'].values ) , : ].loc['description'] )
+                continue
+        function .append( 'Unknown' )
+    return ( function )
+
 
 def auto_annotate_clusters (	header_str:str = '../results/DMHMSY_Fri_Jun__2_09_15_35_2023_'	,
 				alignment_information:str       	= "pcas_df.tsv"		,
 				cluster_information:str         	= "resdf_f.tsv"		,
 				final_cluster_label:str         	= "cids.max"		,
-				enrichment_results_file_pattern:str 	= "(HEADER)treemap_c(CLUSTID).tsv" ) -> pd.DataFrame :
+				significance_level:float		= 0.1			,
+				enrichment_results_file_pattern:list[str] 	= ["(HEADER)treemap_c(CLUSTID).tsv"] ) -> pd.DataFrame :
     #
     df_pca =        pd.read_csv( header_str + alignment_information , sep='\t', index_col=0 )
     df_clu =        pd.read_csv( header_str + cluster_information   , sep='\t', index_col=0 )
     #
     merged_info = pd.concat ( [	df_clu .loc[:,[final_cluster_label]].T	,
 				df_pca .loc[:,[ c for c in df_pca.columns if 'Owner' in c ]].T,
 			 ]).T.rename( columns = { final_cluster_label:'cluster' } )
     merged_info.columns	= [ v.replace('Owner','PCA.owner') for v in  merged_info.columns.values ]
     consolidate		= [ c for c in merged_info.columns if 'owner' in c ]
     #
+    def reformat_local( x , consolidate ) -> pd.Series :
+        rv = [ len(x) ]
+        labs = ['N']
+        for console in consolidate :
+            i = 0
+            for w in composition_leading_label_and_metric( Counter(x.loc[ :, console ].values) ).values()  :
+                rv  .append( w )
+                postfix = ''
+                if i==0 :
+                    postfix = ',Tau'
+                labs.append( console.replace( 'PCA.owner','Specificity' ) + postfix )
+                i += 1
+        return ( pd.Series(rv,index=labs) )
+    #
     from collections import Counter
+    #
     # AUTO ANNOTATIONS
     if len( consolidate ) > 1 :
-        auto_annotated_df = merged_info.groupby('cluster').apply(lambda x: pd.Series( [ len(x) ,
-		*[ v for v in composition_leading_label_and_metric(Counter(x.loc[ :, consolidate[0] ].values)).values() ]   ,
-		*[ v for v in composition_leading_label_and_metric(Counter(x.loc[ :, consolidate[1] ].values)).values() ] ] ,
-			index = [ 'N' , 'Reliability-Spec,Tau' , 'Specificity' ,
-					'Reliability-Aux,Tau'  , 'Auxiliary Annotation' ] ) )
+        auto_annotated_df = merged_info.groupby('cluster').apply( lambda x: reformat_local(x,consolidate) )
     else :
         auto_annotated_df = merged_info.groupby('cluster').apply(lambda x: pd.Series( [ len(x) ,
                 *[ v for v in composition_leading_label_and_metric(Counter(x.loc[ :, consolidate[0] ].values)).values() ] ] ,
                         index = [ 'N' , 'Reliability-Spec,Tau' , 'Specificity' ] ) )
     #
     # ADD IN TOP ENRICHMENT
-    function = []
-    for cid in auto_annotated_df .index.values.tolist() :
-        filename	= enrichment_results_file_pattern.replace('(HEADER)',header_str).replace('(CLUSTID)',str(cid))
-        df		= pd.read_csv(filename,sep='\t',index_col=0)
-        function .append( df.iloc[ np.argmin( df.loc[:,'p-value'].values ) , : ].loc['description'] )
-    auto_annotated_df.loc[:,'Function'] = function
+    for enrichment_file_pattern,i_ in zip( enrichment_results_file_pattern , range(len(enrichment_results_file_pattern)) ) :
+        function = get_annotation_function(	header_str 			= header_str			,
+						auto_annotated_df		= auto_annotated_df		,
+                                		significance_level 		= significance_level 		,
+                                		enrichment_file_pattern		= enrichment_file_pattern	)
+        auto_annotated_df.loc[:,'Function,'+str(i_)] = function
+
     return ( auto_annotated_df )
 
 
 def benchmark_group_expression_with_univariate_foldchange ( group_df:pd.DataFrame , journal_df:pd.DataFrame ,
                         major_group_label:str = None , what_thing:str = None , bRanked:bool=False ,
 			nsamples:int = None, bVerbose:bool = False , bgname:str = 'Background' ,
 			clean_label = lambda x : x.replace(' ','_').replace('/','Or').replace('\\','').replace('-','') ) -> pd.DataFrame :
@@ -292,15 +326,15 @@
             jdf = journal_df
             used_formula = formula
         #
         used_formula = used_formula + block_formula
         if bVerbose :
             print ( 'USING THE FORMULA: ', used_formula )
             print ( 'GROUP MODULATION OF THE VALUES: ',set( jdf.loc[instance_label].values ) )
-
+        #
         if pcfile is None :
             results = gFArEnr ( analyte_df = adf , journal_df = jdf ,
 				formula = used_formula ,
 				grouping_file = gmtfile , bVerbose = bVerbose and bPassOnVerbosity )
         else :
             import impetuous.hierarchical as imph
             dag_df , tree = imph .create_dag_representation_df ( pathway_file = gmtfile , pcfile = pcfile ,
```

### Comparing `biocartograph-0.6.2/src/biocartograph/quantification.py` & `biocartograph-0.6.4/src/biocartograph/quantification.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         umap_seed:int = 42 , hierarchy_cmd:str = 'ward' , divergence = lambda r : np.exp(r) ,
         add_labels:list[str] = None , sample_label:str = None , alignment_label:str = None ,
 	bRemoveCurse:bool = False , bAuxConsensusPCA:bool=True ,
         n_projections:int = 2 , directory:str = './' , bQN:int = None ,
         nNeighborFilter:list[int] = None , heal_symmetry_break_method:str = 'average' ,
         epls_ownership:str = 'angle' , bNonEuclideanBackprojection:bool = False ,
         Sfunc = lambda x:np.mean(x,0) , bAddPies:bool=False , bUseTDA:bool = False ,
-        consensus_function = lambda x:np.sum(x) , consensus_labels:list[str] = None ,
+        consensus_function = lambda x:np.sum(x) , consensus_labels:list[str] = None , bDisbandAggregation:bool = True ,
         bUseGeometricallyCenteredZvalues:bool = False , EPLSformula:str=None ,
         contraction_quantile:float = None   ,
         contraction_depth:float    = None   ) -> tuple[pd.DataFrame] :
     #
     import biocartograph.special	as biox
     import biocartograph.composition	as bioc
     #
@@ -156,17 +156,17 @@
         'umap_dimension:int':umap_dimension , 'umap_n_neighbors:int':umap_n_neighbors , 'umap_local_connectivity:float':umap_local_connectivity ,
         'umap_seed:int':umap_seed , 'hierarchy_cmd:str':hierarchy_cmd , 'divergence:lambda function': divergence ,
         'add_labels:list[str]':add_labels , 'sample_label:str':sample_label , 'alignment_label:str':alignment_label ,
         'bRemoveCurse:bool':bRemoveCurse , 'n_projections:int':n_projections , 'directory:str':directory , 'bQN:int':bQN ,
         'nNeighborFilter:list[int]':nNeighborFilter , 'heal_symmetry_break_method:str':heal_symmetry_break_method ,
         'epls_ownership:str':epls_ownership , 'bNonEuclideanBackprojection:bool':bNonEuclideanBackprojection ,
         'Sfunc':Sfunc , 'bAddPies:bool':bAddPies , 'bUseTDA:bool':bUseTDA , 'bAuxConsensusPCA:bool':bAuxConsensusPCA ,
-        'consensus_function':consensus_function , 'consensus_labels:list[str]' : consensus_labels ,
+        'consensus_function':consensus_function , 'consensus_labels:list[str]' : consensus_labels , 'bDisbandAggregation:bool' : bDisbandAggregation ,
         'bUseGeometricallyCenteredZvalues:bool' : bUseGeometricallyCenteredZvalues , 'EPLSformula:str':EPLSformula ,
-	'contraction_quantile:float': contraction_quantile , ' contraction_depth:float': contraction_depth }
+	'contraction_quantile:float': contraction_quantile , 'contraction_depth:float': contraction_depth }
             ofile = open ( header_str + runinfo_file , 'w' )
             for item in run_dict.items():
                 if 'list' in str(type(item[1])):
                     print ( item[0],'\t=\t [', ','.join([str(i) for i in item[1]]) ,']', file=ofile )
                 else :
                     print ( item[0],'\t=\t [', str(item[1]) ,']', file=ofile )
             print ( 'PYTHON GLOBALS:\n ',
@@ -229,15 +229,15 @@
             MF_f = np.abs( MF_f )
         if 'absolute' in distance_type.split('secondary[')[0] :
             MF_s = np.abs( MF_s )
     #
     # CONSENSUS CONDENSATION IS NOT DONE FOR SAMPLE SPACE
     # THIS WILL AFFECT THE UMAP NOT THE CLUSTERING DISTANCES IF
     # NOT THE bUseUMAP IS SET TRUE
-    if not consensus_labels is None :
+    if not consensus_labels is None and not bDisbandAggregation :
         if 'list' in str(type(consensus_labels)) :
             for label in consensus_labels :
                 if 'str' in str(type(label)) :
                     if label in jdf.index :
                         gdf = adf.T.groupby(jdf.loc[label]).apply( consensus_function ).T
                         if bUseGeometricallyCenteredZvalues :
                             z_values = ( gdf.values - mean_field(gdf.values) ) / std_field(gdf.values)
```

### Comparing `biocartograph-0.6.2/src/biocartograph/special.py` & `biocartograph-0.6.4/src/biocartograph/special.py`

 * *Files 2% similar despite different names*

```diff
@@ -468,23 +468,45 @@
 #
 def quick_check_solution(header_str:str = '../results/DMHMSY_Tue_May__2_10_57_05_2023_' ) :
     file 	= header_str + 'soldf_f.tsv'
     df		= pd.read_csv(file,sep='\t',index_col=0 )
     print ( df.iloc[:,np.argmax(df.iloc[1,:].values)]   )
 
 
+def simple_membership_inference( header_str:str ) :
+        df = pd.read_csv(  header_str[:-1] + '/clustering/final_consensus.tsv' ,sep='\t' ,index_col = 0 )
+        cs = sorted(list(set( df.loc[:,'cluster'].values.tolist() )))
+        N  = len(cs)
+        n_trials = 100.
+        uncertainty = 0.5
+        dfmc = np.abs(pd.DataFrame( [ cs==v for v in df.values ] , index=df.index )*N*n_trials+uncertainty )
+        dfmc .columns = cs
+        dfmc = ( dfmc.T / np.sum(dfmc,1) ) .T
+        #
+        df_ = pd.DataFrame( [ q for q in zip( dfmc.values.reshape(-1) ,
+                [ v for w in dfmc.index.values for v in dfmc.columns.values ] ,
+                [ w for w in dfmc.index.values for v in dfmc.columns.values ] ) ] )
+        df_ .index      = df_.iloc[:,-1]
+        df_ .index.name = 'gene'
+        df_             = df_.iloc[:,[0,1]]
+        df_ .columns    = ['membership','cluster']
+        df_ .loc[:,'nclust'] = [ int(c) for c in df_.loc[:,'cluster'].values.tolist() ]
+        df_ = df_.sort_values('nclust').loc[:,['membership','cluster']]
+        df_ .to_csv( header_str[:-1] + '/clustering/cluster_memberships.tsv',sep='\t')
+
 def generate_atlas_files ( header_str:str ,
                 fcfile:str = 'clustering/final_consensus.tsv' ,
 		nnfile:str = 'distance/nearest_neighbors.tsv' ,
                 umfile:str = 'UMAP/UMAP.tsv' ,
                 ccfile:str = 'UMAP/cluster_centers.tsv' ,
 		pofile:str = 'UMAP/UMAP_polygons.tsv' ,
                 anfile:str = 'enrichment/cluster_annotations.tsv',
                 pcadir:str = 'PCA/',
                 evadir:str = 'evaluation/',
+                enrichment_results_file_pattern:list[str] = ["(HEADER)treemap_c(CLUSTID).tsv"] ,
                 nNN:int=20 ,
                 additional_directories:list[str] = ['data','enrichment','evaluation','graph','PCA','UMAP',
 					'svg'  , 'svg/heatmap','svg/bubble','svg/treemap','svg/fountain',
                                         'html' , 'html']) :
     #
     # START ATLAS GEN
     sep = '\t'
@@ -569,17 +591,19 @@
     id_tag    = header_str.split('/')[-1]
     import os
     enr_files = [ l for l in set(os.listdir(hdr_dir)) if id_tag in l and ('treemap' in l or 'GFA' in l or 'enrichment' in l ) ]
     if len( enr_files ) > 0 :
         for f in enr_files :
             os.system('cp ' + hdr_dir + '/' + f + ' ' +  hdir_str + 'enrichment/' + f )
     from biocartograph.enrichment import auto_annotate_clusters
-    an_df	= auto_annotate_clusters ( header_str )
+    an_df	= auto_annotate_clusters ( header_str , enrichment_results_file_pattern = enrichment_results_file_pattern )
     create_directory ( hdir_str + '/'.join( anfile.split('/')[:-1]) )
     an_df	.to_csv( hdir_str + anfile , sep='\t' )
+    #
+    simple_membership_inference( header_str )
 
 if __name__ == '__main__' :
     #
     reformat_results_and_print_gmtfile_pcfile( header_str = '../results/DMHMSY_Fri_Mar_17_14_37_07_2023_' )
     reformat_results_and_print_gmtfile_pcfile( header_str = '../results/DMHMSY_Fri_Mar_17_16_00_47_2023_' )
     #
     results_dir = '../results/'
```

