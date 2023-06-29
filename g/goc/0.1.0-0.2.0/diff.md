# Comparing `tmp/goc-0.1.0.tar.gz` & `tmp/goc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goc-0.1.0.tar", max compression
+gzip compressed data, was "goc-0.2.0.tar", max compression
```

## Comparing `goc-0.1.0.tar` & `goc-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1929 2023-06-29 11:48:21.014409 goc-0.1.0/README.md
--rw-r--r--   0        0        0     1952 2023-06-29 11:37:13.710834 goc-0.1.0/goc/goc.py
--rw-r--r--   0        0        0      365 2023-06-29 11:56:32.711657 goc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 goc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1929 2023-06-29 11:48:21.014409 goc-0.2.0/README.md
+-rw-r--r--   0        0        0     1642 2023-06-29 12:11:57.261384 goc-0.2.0/goc/goc.py
+-rw-r--r--   0        0        0      365 2023-06-29 12:14:07.262852 goc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 goc-0.2.0/PKG-INFO
```

### Comparing `goc-0.1.0/README.md` & `goc-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `goc-0.1.0/goc/goc.py` & `goc-0.2.0/goc/goc.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,25 +14,17 @@
     git_diff = exec_bash_cmd(cmd)
     prompt_chain = [
         'I send you a git diff, and you write documentation of the commit in markdown',
         git_diff
     ]
     return prompt_chain
 
-def document_comparison_vs_current_commit(benchmark):
-    cmd = f"git diff {benchmark}"
-    git_diff = exec_bash_cmd(cmd)
-    prompt_chain = [
-        'I send you a git diff, and you write documentation of the commit in markdown',
-        git_diff
-    ]
-    return prompt_chain
-
-def document_comparison_of_2_commits(commit_a, commit_b):
-    cmd = f"git diff {commit_a, commit_b}"
+def document_git_diff_wrap(args):
+    fmt_args = " ".join(args)
+    cmd = f"git diff {fmt_args}"
     git_diff = exec_bash_cmd(cmd)
     prompt_chain = [
         'I send you a git diff, and you write documentation of the commit in markdown',
         git_diff
     ]
     return prompt_chain
 
@@ -43,25 +35,25 @@
             {"role": "assistant", "content": cmd}
             for cmd in prompt_chain
         ]
     )    
     return resp
 
 def parse_gpt_resp(resp):
-    md_output = resp['choices'][0]['message']['content']
+    md_output = resp['choices'][-1]['message']['content']
     return md_output
 
 def goc():
     n_args = len(sys.argv) - 1
     if n_args == 0:
+        # compare the latest 2 commits
         prompt_chain = document_latest_commit()
-    elif n_args == 1:
-        prompt_chain = document_comparison_vs_current_commit(sys.argv[1])
-    elif n_args == 2:
-        prompt_chain = document_comparison_of_2_commits(sys.argv[1], sys.argv[2])
+    elif n_args > 0:
+        # just pass the args directly into git diff
+        prompt_chain = document_git_diff_wrap(sys.argv[1:])
     resp = execute_prompt_chain(prompt_chain)
     md_output = parse_gpt_resp(resp)
     print(md_output)
 
 
 if __name__ == '__main__':
     goc()
```

### Comparing `goc-0.1.0/PKG-INFO` & `goc-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goc
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Todd Perry
 Author-email: toddperry171@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

