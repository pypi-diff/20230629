# Comparing `tmp/goc-0.2.0.tar.gz` & `tmp/goc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goc-0.2.0.tar", max compression
+gzip compressed data, was "goc-0.3.0.tar", max compression
```

## Comparing `goc-0.2.0.tar` & `goc-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1929 2023-06-29 11:48:21.014409 goc-0.2.0/README.md
--rw-r--r--   0        0        0     1642 2023-06-29 12:11:57.261384 goc-0.2.0/goc/goc.py
--rw-r--r--   0        0        0      365 2023-06-29 12:14:07.262852 goc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 goc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2826 2023-06-29 12:41:14.732571 goc-0.3.0/README.md
+-rw-r--r--   0        0        0     1642 2023-06-29 12:11:57.261384 goc-0.3.0/goc/goc.py
+-rw-r--r--   0        0        0      414 2023-06-29 12:41:39.532537 goc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 goc-0.3.0/PKG-INFO
```

### Comparing `goc-0.2.0/goc/goc.py` & `goc-0.3.0/goc/goc.py`

 * *Files identical despite different names*

### Comparing `goc-0.2.0/PKG-INFO` & `goc-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,87 @@
-Metadata-Version: 2.1
-Name: goc
-Version: 0.2.0
-Summary: 
-Author: Todd Perry
-Author-email: toddperry171@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openai (>=0.27.8,<0.28.0)
-Description-Content-Type: text/markdown
-
 # GOC
 
-This script, `goc.py`, is a utility tool that leverages the OpenAI GPT-3.5 Turbo model to generate Markdown documentation for Git diffs and commits. It provides three main functionalities:
+This script, `goc.py`, is a utility tool that leverages the OpenAI GPT-3.5 Turbo model to generate Markdown documentation for Git diffs and commits. It can be used to automatically generate a markdown document based on the output of git diff:
 
-1. **Document Latest Commit**: This function compares the latest two commits and generates documentation based on the differences between them.
 
-2. **Document Comparison vs Current Commit**: This function compares the changes made in a specific commit to the current state of the repository and generates documentation accordingly.
+## Prerequisites
 
-3. **Document Comparison of Two Commits**: This function compares the differences between two specific commits and generates documentation based on the changes.
+You will need an OpenAI API key, configure it to the environment variable like below:
 
-## Prerequisites
+```bash
+export OPENAI_API_KEY=<your_key_here>
+```
 
-To use this tool, ensure that you have the following prerequisites installed:
+You will need a python version higher than 3.8
 
-- `openai` Python library
-- Git (version control system)
+## Installation
+
+You can either install from Pypi (https://pypi.org/project/goc/)
+```bash
+pip install goc
+```
+
+Or you can download this repository and run
+
+```bash
+poetry install
+```
 
 ## Usage
 
 To execute the script, run the following command:
 
 ```bash
-python goc.py [arguments]
+goc [arguments]
 ```
 
 Replace `[arguments]` with the appropriate options based on your requirement:
 
 - **Document Latest Commit**:
   ```bash
-  python goc.py
+  goc
   ```
 
 - **Document Comparison vs Current Commit**:
   ```bash
-  python goc.py [commit_hash]
+  goc [commit_hash]
   ```
 
 - **Document Comparison of Two Commits**:
   ```bash
-  python goc.py [commit_a] [commit_b]
+  goc [commit_a] [commit_b]
   ```
 
 ## Output
 
 The script generates Markdown documentation by utilizing the OpenAI GPT-3.5 Turbo model. The resulting documentation will be displayed in the console output.
 
+
+## Examples
+
+```bash
+$ goc a0f72101be85667a362425c2cdc30ef794e2a738
+## Commit Details
+
+- **Commit Type:** Code update
+- **Commit Scope:** goc.py, pyproject.toml
+- **Commit Description:**
+
+### goc.py
+1. Removed the `document_comparison_vs_current_commit` and `document_comparison_of_2_commits` functions as they were not being used.
+2. Created a new function `document_git_diff_wrap` that takes command line arguments and runs the `git diff` command with those arguments. This allows for easy comparison of commits by passing the commit hashes or branches directly as arguments.
+3. Modified the `goc` function to handle different scenarios based on the number of command line arguments passed. If no arguments are provided, it compares the latest two commits. If one or more arguments are provided, it passes them directly to `document_git_diff_wrap` for comparison.
+4. updated the `parse_gpt_resp` function to return the content of the last choice/message in the response, as the final generated markdown content is usually the last choice.
+
+### pyproject.toml
+1. Updated the version to `"0.2.0"`.
+
+Please review and merge these changes.
+```
+
 ## Note
 
 Make sure you have the necessary permissions and access to the Git repository you intend to analyze. Also, ensure that the repository is properly cloned on your local machine.
 
 ## Disclaimer
 
 This tool relies on the OpenAI GPT-3.5 Turbo model for generating documentation. The accuracy and quality of the generated content depend on the model's training data and the provided input. Please review and validate the generated documentation before using it in your projects.
-
```

