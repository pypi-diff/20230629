# Comparing `tmp/afmmech-2.1-py3-none-any.whl.zip` & `tmp/afmmech-2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7803 bytes, number of entries: 6
--rw-rw-r--  2.0 unx      426 b- defN 23-Jun-28 02:29 afmmech/__init__.py
--rw-rw-r--  2.0 unx    21248 b- defN 23-Jun-29 18:15 afmmech/helpers.py
--rw-rw-r--  2.0 unx      421 b- defN 23-Jun-29 18:16 afmmech-2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-29 18:16 afmmech-2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Jun-29 18:16 afmmech-2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      439 b- defN 23-Jun-29 18:16 afmmech-2.1.dist-info/RECORD
-6 files, 22634 bytes uncompressed, 7011 bytes compressed:  69.0%
+Zip file size: 7836 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx      496 b- defN 23-Jun-29 18:47 afmmech/__init__.py
+-rw-rw-r--  2.0 unx    21252 b- defN 23-Jun-29 18:46 afmmech/helpers.py
+-rw-rw-r--  2.0 unx      421 b- defN 23-Jun-29 18:47 afmmech-2.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-29 18:47 afmmech-2.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jun-29 18:47 afmmech-2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      439 b- defN 23-Jun-29 18:47 afmmech-2.2.dist-info/RECORD
+6 files, 22708 bytes uncompressed, 7044 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: afmmech/__init__.py
 Comment: 
 
 Filename: afmmech/helpers.py
 Comment: 
 
-Filename: afmmech-2.1.dist-info/METADATA
+Filename: afmmech-2.2.dist-info/METADATA
 Comment: 
 
-Filename: afmmech-2.1.dist-info/WHEEL
+Filename: afmmech-2.2.dist-info/WHEEL
 Comment: 
 
-Filename: afmmech-2.1.dist-info/top_level.txt
+Filename: afmmech-2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: afmmech-2.1.dist-info/RECORD
+Filename: afmmech-2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## afmmech/__init__.py

```diff
@@ -1 +1 @@
-from .helpers import get_files, get_folders, ibw2df, format_df, smooth_sma, get_trigger_point_index, get_contact_point_index_basic, get_contact_point_index_fit, cut_repulsive_data, shift_repulsive_data, force_hertz, force_conv, get_speed, get_speed_spline, force_ramp, indentation_creep_sls, q_sls, q_abs_sls, viscoelastic_constraint, fit_function_to_data, fit_complex_function_to_data, get_fft, get_fft_frequency, get_r, mdft
+from .helpers import get_files, get_folders, ibw2df, format_df, smooth_sma, get_trigger_point_index, get_contact_point_index_basic, get_contact_point_index_fit, cut_repulsive_data, shift_repulsive_data, force_hertz, force_conv, get_speed, get_speed_spline, force_ramp, indentation_creep_sls, q_sls, q_abs_sls, viscoelastic_constraint, fit_function_to_data, fit_complex_function_to_data, get_fft, get_fft_frequency, get_r, mdft, dataset, dataset_dict, process_afm_dataframe, parallel_load_ibw_data
```

## afmmech/helpers.py

```diff
@@ -544,15 +544,15 @@
             elif not isinstance(new_column_name, list):
                 new_column_name = [new_column_name]
             for c, new_name in zip(column, new_column_name):
                 self.parallel_process(c, func, new_column_name=new_name, *args, **kwargs)
         for d in self.data.values():
             d.parallel_process(column, func, new_column_name, *args, **kwargs)
             
-def process_dataframe(df, k, sampling_frequency, ignore_trigger=False):
+def process_afm_dataframe(df, k, sampling_frequency, ignore_trigger=False):
     # format
     formatted_df = format_df(df, k, sampling_frequency)
     # get trigger point
     trigger_point = get_trigger_point_index(formatted_df)
     # get contact point
     contact_point = get_contact_point_index_fit(formatted_df, trigger_point)
     # get the repulsive data
```

