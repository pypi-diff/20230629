# Comparing `tmp/findlike-1.2.2.tar.gz` & `tmp/findlike-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/soldeace/projects/findlike/dist/.tmp-cs6evx_7/findlike-1.2.2.tar", last modified: Thu Jun 29 13:51:06 2023, max compression
+gzip compressed data, was "findlike-1.3.0.tar", last modified: Thu Jun 29 15:13:17 2023, max compression
```

## Comparing `findlike-1.2.2.tar` & `findlike-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 13:51:06.000000 findlike-1.2.2/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1067 2023-06-27 14:06:31.000000 findlike-1.2.2/LICENSE
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     5716 2023-06-29 13:51:06.000000 findlike-1.2.2/PKG-INFO
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     5091 2023-06-29 00:03:20.000000 findlike-1.2.2/README.md
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 13:51:06.000000 findlike-1.2.2/findlike/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        0 2022-12-31 23:26:30.000000 findlike-1.2.2/findlike/__init__.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       59 2023-06-23 20:53:39.000000 findlike-1.2.2/findlike/__main__.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     5204 2023-06-29 11:53:21.000000 findlike-1.2.2/findlike/cli.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     4330 2023-06-28 17:12:04.000000 findlike-1.2.2/findlike/format.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3234 2023-06-28 17:48:12.000000 findlike-1.2.2/findlike/preprocessing.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)      433 2023-06-28 17:12:13.000000 findlike-1.2.2/findlike/utils.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1706 2023-06-28 17:51:37.000000 findlike-1.2.2/findlike/wrappers.py
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 13:51:06.000000 findlike-1.2.2/findlike.egg-info/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     5716 2023-06-29 13:51:06.000000 findlike-1.2.2/findlike.egg-info/PKG-INFO
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)      452 2023-06-29 13:51:06.000000 findlike-1.2.2/findlike.egg-info/SOURCES.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        1 2023-06-29 13:51:06.000000 findlike-1.2.2/findlike.egg-info/dependency_links.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       46 2023-06-29 13:51:06.000000 findlike-1.2.2/findlike.egg-info/entry_points.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)      186 2023-06-29 13:51:06.000000 findlike-1.2.2/findlike.egg-info/requires.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        9 2023-06-29 13:51:06.000000 findlike-1.2.2/findlike.egg-info/top_level.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1095 2023-06-29 13:47:55.000000 findlike-1.2.2/pyproject.toml
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       38 2023-06-29 13:51:06.000000 findlike-1.2.2/setup.cfg
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 13:51:06.000000 findlike-1.2.2/tests/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     8276 2023-06-28 14:38:17.000000 findlike-1.2.2/tests/test_cli.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1898 2023-06-28 13:14:54.000000 findlike-1.2.2/tests/test_corpus.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     2937 2023-06-27 19:22:45.000000 findlike-1.2.2/tests/test_format.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1967 2023-06-28 17:48:50.000000 findlike-1.2.2/tests/test_processor.py
+drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 15:13:17.277779 findlike-1.3.0/
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1067 2023-06-27 14:06:31.000000 findlike-1.3.0/LICENSE
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     7877 2023-06-29 15:13:17.274445 findlike-1.3.0/PKG-INFO
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     7252 2023-06-29 15:08:05.000000 findlike-1.3.0/README.md
+drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 15:13:17.274445 findlike-1.3.0/findlike/
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)        0 2022-12-31 23:26:30.000000 findlike-1.3.0/findlike/__init__.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)       59 2023-06-23 20:53:39.000000 findlike-1.3.0/findlike/__main__.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     5049 2023-06-29 14:33:51.000000 findlike-1.3.0/findlike/cli.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3300 2023-06-29 14:20:03.000000 findlike-1.3.0/findlike/constants.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     4330 2023-06-28 17:12:04.000000 findlike-1.3.0/findlike/format.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3234 2023-06-28 17:48:12.000000 findlike-1.3.0/findlike/preprocessing.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1218 2023-06-29 14:30:47.000000 findlike-1.3.0/findlike/utils.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1706 2023-06-28 17:51:37.000000 findlike-1.3.0/findlike/wrappers.py
+drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 15:13:17.274445 findlike-1.3.0/findlike.egg-info/
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     7877 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/PKG-INFO
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)      474 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/SOURCES.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)        1 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/dependency_links.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)       46 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/entry_points.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)      186 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/requires.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)        9 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/top_level.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1095 2023-06-29 15:11:29.000000 findlike-1.3.0/pyproject.toml
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)       38 2023-06-29 15:13:17.277779 findlike-1.3.0/setup.cfg
+drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 15:13:17.274445 findlike-1.3.0/tests/
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     8276 2023-06-28 14:38:17.000000 findlike-1.3.0/tests/test_cli.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1898 2023-06-28 13:14:54.000000 findlike-1.3.0/tests/test_corpus.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     2937 2023-06-27 19:22:45.000000 findlike-1.3.0/tests/test_format.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1967 2023-06-28 17:48:50.000000 findlike-1.3.0/tests/test_processor.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `findlike-1.2.2/LICENSE` & `findlike-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findlike-1.2.2/PKG-INFO` & `findlike-1.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: findlike
-Version: 1.2.2
-Summary: findlike is a package to retrieve similar documents
-Author-email: Bruno Arine <bruno.arine@runbox.com>
-Project-URL: Homepage, http://www.github.com/brunoarine/findlike
-Project-URL: Repository, https://github.com/brunoarine/findlike.git
-Project-URL: Bug Tracker, http://www.github.com/brunoarine/findlike/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # findlike
 
 [![PyPI](https://img.shields.io/pypi/v/findlike.svg)](https://pypi.org/project/findlike/)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/brunoarine/findlike/blob/master/LICENSE)
 [![Tests](https://github.com/brunoarine/findlike/workflows/Test/badge.svg)](https://github.com/brunoarine/findlike/actions?query=workflow%3ATest)
 
 `findlike` is a command-line tool written in Python that retrieves a list of similar files in relation to a reference file or an ad-hoc query. The tool is highly configurable and can be used as backend for other programs (e.g. personal knowledge management systems, Emacs, etc.) 
@@ -97,41 +81,125 @@
 findlike [OPTIONS] [REFERENCE_FILE]
 ```
 
 `findlike` works with either a reference file or a `--query` option. Once the reference text is set, `findlike` will scan a given directory (default is the current working dir), and return the most similar documents against the reference.
 
 ## Options
 
-Here's the breakdown of the available options in Findlike:
+Here's the breakdown of the available options in findlike:
+
+#### `--help`
+
+Displays a short summary of the available options.
+
+#### `-d, --directory PATH`
+
+Specify the directory that is going to be scanned. Default is current working directory. Example:
+
+```sh
+findlike -d /path/to/another/directory
+```
+
+#### `-q, --query TEXT`
+
+Passes an ad-hoc query to the program, so that no reference file is required. Useful when you want to quickly find documents by an overall theme. Example:
+
+```sh
+findlike -q "earthquakes"
+```
+
+#### `-f, --file-pattern`
+
+Specifies the file pattern to use when scanning the directories for similar files. The pattern uses [glob](https://en.wikipedia.org/wiki/Glob_(programming)) convention, and should be passed with single or double quotes, otherwise your shell environment will likely try to expand it. Default is common plain-text file extensions (the full list can be seen [here](./findlike/constants.py)).
+
+```sh
+findlike -f "*.md" reference_file.txt
+```
+
+#### `-R, --recursive`
+
+If used, this option makes `findlike` scans directories and their sub-directories as well. Example:
+
+```sh
+findlike reference_file.txt -R
+```
+
+#### `-l, --language TEXT`
+
+Changing this value will impact stopwords filtering and word stemmer. The following languages are supported: Arabic, Danish, Dutch, English, Finnish, French, German, Hungarian, Italian, Norwegian, Portuguese, Romanian, Russian, Spanish and Swedish. Default is English.
+
+```sh
+findlike reference_file.txt -l "portuguese"
+```
+
+#### `-c, --min-chars INTEGER`
+
+Minimum document size (in number of characters) to be included in the corpus. Default is 1. Example:
+
+```sh
+findlike reference_file.txt -c 50
+```
+
+#### `-A, --absolute-paths`
 
+Show the absolute path of each result instead of relative paths. Example:
+
+```sh
+findlike reference_file.txt -A
+```
+
+#### `-m, --max-results INTEGER`
+
+Number of items to show in the final results. Default is 10.
+
+```sh
+findlike reference_file.txt -m 5
+```
+
+#### `-p, --prefix TEXT`
+
+String to prepend each entry in the final results. You can set it to "* " or "- " to turn them into a Markdown or Org-mode list. Default is "", so that no prefix is shown. Example: 
+
+```sh
+findlike reference_file.txt -p "- "
+```
+
+#### `-h, --hide-reference`
+
+Remove the first result from the scores list. Useful if the reference file is in the scanned directory, and you don't want to see it included in the top of the results. This option has no effect if the `--query` option is used.
+
+```sh
+findlike reference_file.txt -h
 ```
-  --version                     Show the version and exit.
-  -q, --query TEXT              query option if no reference file is provided
-  -d, --directory PATH          directory to scan for similar files  [default:
-                                (current directory)]
-  -f, --filename-pattern TEXT   filename pattern matching  [default: *.*]
-  -R, --recursive               recursive search
-  -a, --algorithm [bm25|tfidf]  text similarity algorithm  [default: tfidf]
-  -l, --language TEXT           stemmer and stopwords language  [default:
-                                english]
-  -c, --min-chars INTEGER       minimum document size (in number of
-                                characters) to be considered  [default: 1]
-  -A, --absolute-paths          show absolute rather than relative paths
-  -m, --max-results INTEGER     maximum number of results  [default: 10]
-  -p, --prefix TEXT             result lines prefix
-  -s, --show-scores             show similarity scores
-  -h, --hide-reference          remove REFERENCE_FILE from results
-  -H, --heading TEXT            results list heading
-  -F, --format [plain|json]     output format  [default: plain]
-  -t, --threshold FLOAT         minimum score for a result to be shown
-                                [default: 0.0]
-  --help                        Show this message and exit.
+
+#### `-H, --heading TEXT`
+
+Text to show as the list heading. Default is "", so no heading title is shown. Example:
+
+```sh
+findlike reference_file.txt -H "## Similar files"
+```
+
+#### `-F, --format [plain|json]`
+
+This option sets the output format. `plain` will print the results as a simple list, one entry per line. `json` will print the results as a valid JSON list with `score` and `target` as keys for each entry. Default is "plain". Example:
+
+```sh
+findlike reference_file.txt -F json
 ```
 
-## Examples
+#### `-t, --threshold FLOAT`
+
+Similarity score threshold. All results whose score are below the determined threshold will be omitted. Default is 0.05. Set it to 0 if you wish to show all results. Example:
+
+```sh
+findlike reference_file.txt -t 0
+```
+
+## More Examples
 
 To find similar documents in a directory (recursively):
 
 ```sh
 findlike -R -d /path/to/directory reference_file.md 
 ```
 
@@ -161,18 +229,25 @@
 cd findlike
 python -m venv venv
 source venv/bin/activate
 ```
 
 Now install the development dependencies:
 
+```sh
 pip install -e '.[dev]'
+`` 
 
 To run the tests:
 
 ```bash
 pytest
 ```
 
 ## License
 
 This project is licensed under the terms of the MIT license. See [LICENSE](LICENSE) for more details.
+
+## Acknowledgements
+
+- [Simon Willison](https://simonwillison.net/) for being an inspiration on releasing small but useful tools more often.
+- [Sindre Sorhus](https://raw.githubusercontent.com/sindresorhus/text-extensions) for the comprehensive list of plain-text file extensions.
```

### Comparing `findlike-1.2.2/findlike/cli.py` & `findlike-1.3.0/findlike/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,20 @@
 
 from pathlib import Path
 
 import click
 from nltk.stem import SnowballStemmer
 from stop_words import get_stop_words
 
-from .format import BaseFormatter, JsonFormatter
 from .preprocessing import (
     Corpus,
     Processor,
 )
-from .utils import try_read_file
-from .wrappers import BM25, Tfidf
-
-FORMATTER_CLASSES = {"plain": BaseFormatter, "json": JsonFormatter}
-ALGORITHM_CLASSES = {"bm25": BM25, "tfidf": Tfidf}
+from .utils import try_read_file, collect_paths
+from .constants import FORMATTER_CLASSES, ALGORITHM_CLASSES, TEXT_FILE_EXT
 
 
 @click.command()
 @click.version_option()
 @click.argument("reference-file", type=click.Path(), nargs=1, required=False)
 @click.option(
     "-q",
@@ -39,15 +35,15 @@
 )
 @click.option(
     "--filename-pattern",
     "-f",
     type=str,
     default="*.*",
     help="filename pattern matching",
-    show_default=True,
+    show_default="plain-text file extensions",
     required=False,
 )
 @click.option(
     "--recursive",
     "-R",
     is_flag=True,
     help="recursive search",
@@ -158,15 +154,15 @@
     heading,
     show_scores,
     recursive,
     hide_reference,
     query,
     format,
     threshold,
-    absolute_paths
+    absolute_paths,
 ):
     """'findlike' is a program that scans a given directory and returns the most
     similar documents in relation to REFERENCE_FILE or --query QUERY.
 
     Example using a reference file:
 
     $ findlike -d /path/to/my/notes my_recipe.md
@@ -184,23 +180,20 @@
     else:
         raise click.UsageError(
             "Neither REFERENCE_FILE nor --query QUERY was provided."
         )
 
     # Put together the list of documents to be analyzed.
     directory_path = Path(directory)
-    glob_func = (
-        directory_path.rglob
-        if recursive
-        else directory_path.glob
+    document_paths = collect_paths(
+        directory=directory_path, extensions=TEXT_FILE_EXT, recursive=recursive
     )
-    documents_paths = [x for x in glob_func(filename_pattern) if x.is_file()]
 
     # Create a corpus with the collected documents.
-    corpus = Corpus(paths=documents_paths, min_chars=min_chars)
+    corpus = Corpus(paths=document_paths, min_chars=min_chars)
 
     # Set up the documents pre-processor.
     stemmer = SnowballStemmer(language).stem
     processor = Processor(
         stopwords=get_stop_words(language=language),
         stemmer=stemmer,
     )
@@ -219,11 +212,11 @@
         max_results=max_results,
         show_scores=show_scores,
         hide_reference=hide_reference,
         prefix=prefix,
         heading=heading,
         threshold=threshold,
         absolute_paths=absolute_paths,
-        is_query=bool(query)
-        )
+        is_query=bool(query),
+    )
     formatted_results = formatter.format()
     print(formatted_results)
```

### Comparing `findlike-1.2.2/findlike/format.py` & `findlike-1.3.0/findlike/format.py`

 * *Files identical despite different names*

### Comparing `findlike-1.2.2/findlike/preprocessing.py` & `findlike-1.3.0/findlike/preprocessing.py`

 * *Files identical despite different names*

### Comparing `findlike-1.2.2/findlike/wrappers.py` & `findlike-1.3.0/findlike/wrappers.py`

 * *Files identical despite different names*

### Comparing `findlike-1.2.2/pyproject.toml` & `findlike-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "findlike"
-version = "1.2.2"
+version = "1.3.0"
 authors = [{ name = "Bruno Arine", email = "bruno.arine@runbox.com" }]
 description = "findlike is a package to retrieve similar documents"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `findlike-1.2.2/tests/test_cli.py` & `findlike-1.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `findlike-1.2.2/tests/test_corpus.py` & `findlike-1.3.0/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `findlike-1.2.2/tests/test_format.py` & `findlike-1.3.0/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `findlike-1.2.2/tests/test_processor.py` & `findlike-1.3.0/tests/test_processor.py`

 * *Files identical despite different names*

