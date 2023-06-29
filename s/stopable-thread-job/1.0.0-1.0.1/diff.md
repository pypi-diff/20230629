# Comparing `tmp/stopable_thread_job-1.0.0-py3-none-any.whl.zip` & `tmp/stopable_thread_job-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7365 bytes, number of entries: 9
+Zip file size: 7369 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-07 05:00 FlexableThreadPoolExecutor/__init__.py
 -rw-rw-rw-  2.0 fat     8511 b- defN 22-Nov-07 05:02 FlexableThreadPoolExecutor/flexable_thread.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-29 06:55 StopableThreadJob/__init__.py
--rw-rw-rw-  2.0 fat     2873 b- defN 23-Jun-29 07:04 StopableThreadJob/job_manager.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-29 07:10 stopable_thread_job-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1852 b- defN 23-Jun-29 07:10 stopable_thread_job-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-29 07:10 stopable_thread_job-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-29 07:10 stopable_thread_job-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      812 b- defN 23-Jun-29 07:10 stopable_thread_job-1.0.0.dist-info/RECORD
-9 files, 15249 bytes uncompressed, 5933 bytes compressed:  61.1%
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-29 07:17 StopableThreadJob/__init__.py
+-rw-rw-rw-  2.0 fat     2951 b- defN 23-Jun-29 07:58 StopableThreadJob/job_manager.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-29 08:06 stopable_thread_job-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1852 b- defN 23-Jun-29 08:06 stopable_thread_job-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-29 08:06 stopable_thread_job-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-29 08:06 stopable_thread_job-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      812 b- defN 23-Jun-29 08:06 stopable_thread_job-1.0.1.dist-info/RECORD
+9 files, 15327 bytes uncompressed, 5937 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: StopableThreadJob/__init__.py
 Comment: 
 
 Filename: StopableThreadJob/job_manager.py
 Comment: 
 
-Filename: stopable_thread_job-1.0.0.dist-info/LICENSE
+Filename: stopable_thread_job-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: stopable_thread_job-1.0.0.dist-info/METADATA
+Filename: stopable_thread_job-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: stopable_thread_job-1.0.0.dist-info/WHEEL
+Filename: stopable_thread_job-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: stopable_thread_job-1.0.0.dist-info/top_level.txt
+Filename: stopable_thread_job-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: stopable_thread_job-1.0.0.dist-info/RECORD
+Filename: stopable_thread_job-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## StopableThreadJob/job_manager.py

```diff
@@ -53,22 +53,24 @@
                 self.semaphore.acquire()
                 ret = target(*args, **kwargs)
                 print(f"{job_id} is finished.")
                 return ret
             except StopRunningCommand as e:
                 print(f"{job_id} has been stopped.")
             except Exception as e:
+                print(f"{job_id} is finished.")
                 raise e
             finally:
                 if job_id in self.job_store:
                     self.job_store.pop(job_id)
                 self.semaphore.release()
 
         with self.job_lock:
             t = TerminableThread(target=inner_job, *args, **kwargs)
+            t.daemon = True
             # if job_id in self.job:
             #     self.job[job_id].terminate(StopRunningCommand)
             self.job_store[job_id] = t
         return self.job_store[job_id]
 
     def remove_job(self, job_id):
         with self.job_lock:
```

## Comparing `stopable_thread_job-1.0.0.dist-info/LICENSE` & `stopable_thread_job-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `stopable_thread_job-1.0.0.dist-info/METADATA` & `stopable_thread_job-1.0.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopable-thread-job
-Version: 1.0.0
+Version: 1.0.1
 Summary: 可停止线程任务管理器
 Home-page: https://github.com/AlitaIcon/StopableThreadJob
 Author: alita
 Author-email: 1906321518@qq.com
 License: MIT
 Project-URL: Documentation, https://github.com/AlitaIcon/StopableThreadJob
 Classifier: Programming Language :: Python :: 3
```

## Comparing `stopable_thread_job-1.0.0.dist-info/RECORD` & `stopable_thread_job-1.0.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 FlexableThreadPoolExecutor/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 FlexableThreadPoolExecutor/flexable_thread.py,sha256=uq9cY8RASyLX9_Yf9yAV0Uv5_iiXECaDUHhBPOoboSA,8511
 StopableThreadJob/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-StopableThreadJob/job_manager.py,sha256=NGy89hl8BSNfubqP_Pq8VGcDJoZDNvHFPOdjR3U9MGQ,2873
-stopable_thread_job-1.0.0.dist-info/LICENSE,sha256=aGTxmVMJK1Bu3A51P5fz-elrB_brWzFZtX1yGprArkw,1091
-stopable_thread_job-1.0.0.dist-info/METADATA,sha256=Yc9GF0ZREb3jsH9kvxNVv3e711pToLXMO5a-Ly44Gb0,1852
-stopable_thread_job-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-stopable_thread_job-1.0.0.dist-info/top_level.txt,sha256=DqlT31O4mjRgOqP9zLJiJwIa4YeXesM4CYiMcy-M5W4,18
-stopable_thread_job-1.0.0.dist-info/RECORD,,
+StopableThreadJob/job_manager.py,sha256=8LAOD5xuFYNVQgWfHGuudkkjdWyVz9pn1_7Y1X2so_A,2951
+stopable_thread_job-1.0.1.dist-info/LICENSE,sha256=aGTxmVMJK1Bu3A51P5fz-elrB_brWzFZtX1yGprArkw,1091
+stopable_thread_job-1.0.1.dist-info/METADATA,sha256=GD7UAGN9rqpFMVtVF1Y03wh7veUZ1g-WE1hQBUjrjpY,1852
+stopable_thread_job-1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+stopable_thread_job-1.0.1.dist-info/top_level.txt,sha256=DqlT31O4mjRgOqP9zLJiJwIa4YeXesM4CYiMcy-M5W4,18
+stopable_thread_job-1.0.1.dist-info/RECORD,,
```

