# Comparing `tmp/kmer_tools-0.1.0.tar.gz` & `tmp/kmer_tools-0.1.2.tar.gz`

## Comparing `kmer_tools-0.1.0.tar` & `kmer_tools-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      282 1970-01-01 00:00:00.000000 kmer_tools-0.1.0/Cargo.toml
--rw-r--r--   0 407757713 1311385079     1548 2022-12-02 10:09:47.000000 kmer_tools-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0 407757713 1311385079      317 2022-12-08 17:21:20.000000 kmer_tools-0.1.0/.github/workflows/rust.yml
--rw-r--r--   0 407757713 1311385079      685 2022-12-02 10:09:47.000000 kmer_tools-0.1.0/.gitignore
--rw-r--r--   0 407757713 1311385079      223 2023-01-24 16:34:00.000000 kmer_tools-0.1.0/Dockerfile
--rw-r--r--   0 407757713 1311385079      135 2022-12-08 17:23:24.000000 kmer_tools-0.1.0/README.md
--rw-r--r--   0 407757713 1311385079      320 2022-12-02 10:09:47.000000 kmer_tools-0.1.0/pyproject.toml
--rw-r--r--   0 407757713 1311385079    19310 2022-12-06 13:43:04.000000 kmer_tools-0.1.0/src/lib.rs
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 kmer_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 kmer_tools-0.1.2/Cargo.toml
+-rw-r--r--   0        0        0      317 2022-12-08 17:21:20.000000 kmer_tools-0.1.2/.github/workflows/rust.yml
+-rw-r--r--   0        0        0      707 2023-06-29 10:51:44.000000 kmer_tools-0.1.2/.gitignore
+-rw-r--r--   0        0        0    20131 2023-06-29 10:42:57.000000 kmer_tools-0.1.2/LICENSE
+-rw-r--r--   0        0        0      135 2022-12-08 17:23:24.000000 kmer_tools-0.1.2/README.md
+-rw-r--r--   0        0        0      320 2022-12-02 10:09:47.000000 kmer_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    19310 2023-06-29 10:43:10.000000 kmer_tools-0.1.2/src/lib.rs
+-rw-r--r--   0        0        0   233485 2023-06-29 11:12:04.000000 kmer_tools-0.1.2/target/wheels/kmer_tools-0.1.2-cp311-cp311-macosx_11_0_arm64.whl
+-rw-r--r--   0        0        0   243148 2023-06-29 11:32:01.000000 kmer_tools-0.1.2/target/wheels/kmer_tools-0.1.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+-rw-r--r--   0        0        0     9893 2023-06-29 10:49:00.000000 kmer_tools-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 kmer_tools-0.1.2/PKG-INFO
```

### Comparing `kmer_tools-0.1.0/.gitignore` & `kmer_tools-0.1.2/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 /target
 
+.gitignore
+Dockerfile
 # Byte-compiled / optimized / DLL files
 __pycache__/
 .pytest_cache/
 *.py[cod]
 
 # C extensions
 *.so
```

### Comparing `kmer_tools-0.1.0/src/lib.rs` & `kmer_tools-0.1.2/src/lib.rs`

 * *Files identical despite different names*

