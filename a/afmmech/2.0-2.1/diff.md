# Comparing `tmp/afmmech-2.0-py3-none-any.whl.zip` & `tmp/afmmech-2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7638 bytes, number of entries: 6
+Zip file size: 7803 bytes, number of entries: 6
 -rw-rw-r--  2.0 unx      426 b- defN 23-Jun-28 02:29 afmmech/__init__.py
--rw-rw-r--  2.0 unx    20510 b- defN 23-Jun-29 18:13 afmmech/helpers.py
--rw-rw-r--  2.0 unx      421 b- defN 23-Jun-29 18:13 afmmech-2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-29 18:13 afmmech-2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Jun-29 18:13 afmmech-2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      439 b- defN 23-Jun-29 18:13 afmmech-2.0.dist-info/RECORD
-6 files, 21896 bytes uncompressed, 6846 bytes compressed:  68.7%
+-rw-rw-r--  2.0 unx    21248 b- defN 23-Jun-29 18:15 afmmech/helpers.py
+-rw-rw-r--  2.0 unx      421 b- defN 23-Jun-29 18:16 afmmech-2.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-29 18:16 afmmech-2.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jun-29 18:16 afmmech-2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      439 b- defN 23-Jun-29 18:16 afmmech-2.1.dist-info/RECORD
+6 files, 22634 bytes uncompressed, 7011 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: afmmech/__init__.py
 Comment: 
 
 Filename: afmmech/helpers.py
 Comment: 
 
-Filename: afmmech-2.0.dist-info/METADATA
+Filename: afmmech-2.1.dist-info/METADATA
 Comment: 
 
-Filename: afmmech-2.0.dist-info/WHEEL
+Filename: afmmech-2.1.dist-info/WHEEL
 Comment: 
 
-Filename: afmmech-2.0.dist-info/top_level.txt
+Filename: afmmech-2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: afmmech-2.0.dist-info/RECORD
+Filename: afmmech-2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## afmmech/helpers.py

```diff
@@ -542,8 +542,25 @@
             if new_column_name is None:
                 new_column_name = [None] * len(column)
             elif not isinstance(new_column_name, list):
                 new_column_name = [new_column_name]
             for c, new_name in zip(column, new_column_name):
                 self.parallel_process(c, func, new_column_name=new_name, *args, **kwargs)
         for d in self.data.values():
-            d.parallel_process(column, func, new_column_name, *args, **kwargs)
+            d.parallel_process(column, func, new_column_name, *args, **kwargs)
+            
+def process_dataframe(df, k, sampling_frequency, ignore_trigger=False):
+    # format
+    formatted_df = format_df(df, k, sampling_frequency)
+    # get trigger point
+    trigger_point = get_trigger_point_index(formatted_df)
+    # get contact point
+    contact_point = get_contact_point_index_fit(formatted_df, trigger_point)
+    # get the repulsive data
+    trigger_point = trigger_point if not ignore_trigger else -1
+    contact_df = cut_repulsive_data(formatted_df, contact_point, trigger_point)
+    # shift the data
+    contact_df = shift_repulsive_data(contact_df)
+    return contact_df
+
+def parallel_load_ibw_data(folder):
+    return joblib.Parallel(n_jobs=-1)(joblib.delayed(ibw2df)(file) for file in get_files(folder))
```

