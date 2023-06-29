# Comparing `tmp/thipster-0.22.0.tar.gz` & `tmp/thipster-0.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.22.0.tar", last modified: Wed Jun 28 15:47:13 2023, max compression
+gzip compressed data, was "thipster-0.22.1.tar", last modified: Thu Jun 29 07:41:36 2023, max compression
```

## Comparing `thipster-0.22.0.tar` & `thipster-0.22.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.583150 thipster-0.22.0/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-28 15:47:08.000000 thipster-0.22.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-28 15:47:08.000000 thipster-0.22.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5376 2023-06-28 15:47:13.583150 thipster-0.22.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4544 2023-06-28 15:47:08.000000 thipster-0.22.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-28 15:47:08.000000 thipster-0.22.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-28 15:47:08.000000 thipster-0.22.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 15:47:13.583150 thipster-0.22.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1848 2023-06-28 15:47:09.000000 thipster-0.22.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.575150 thipster-0.22.0/tests/
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.575150 thipster-0.22.0/tests/engine/
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     6152 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.575150 thipster-0.22.0/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.575150 thipster-0.22.0/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    18947 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    15123 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     5314 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.575150 thipster-0.22.0/tests/repository/
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/repository/test_github_repository.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/repository/test_local_repository.py
--rw-r--r--   0 root         (0) root         (0)     6201 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/repository/test_resourcemodel.py
--rw-r--r--   0 root         (0) root         (0)     3577 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     6483 2023-06-28 15:47:08.000000 thipster-0.22.0/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.575150 thipster-0.22.0/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.575150 thipster-0.22.0/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.579150 thipster-0.22.0/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5610 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      456 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     2166 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     5757 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4646 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.579150 thipster-0.22.0/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.583150 thipster-0.22.0/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12802 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     5311 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14082 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    14974 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3283 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    23825 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2631 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6866 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.583150 thipster-0.22.0/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.583150 thipster-0.22.0/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24467 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     3350 2023-06-28 15:47:08.000000 thipster-0.22.0/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:47:13.575150 thipster-0.22.0/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5376 2023-06-28 15:47:13.000000 thipster-0.22.0/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-28 15:47:13.000000 thipster-0.22.0/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 15:47:13.000000 thipster-0.22.0/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-28 15:47:13.000000 thipster-0.22.0/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-28 15:47:13.000000 thipster-0.22.0/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.115064 thipster-0.22.1/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-29 07:41:32.000000 thipster-0.22.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-29 07:41:32.000000 thipster-0.22.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-06-29 07:41:36.115064 thipster-0.22.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4544 2023-06-29 07:41:32.000000 thipster-0.22.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-29 07:41:32.000000 thipster-0.22.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-29 07:41:32.000000 thipster-0.22.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 07:41:36.115064 thipster-0.22.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-29 07:41:33.000000 thipster-0.22.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.107063 thipster-0.22.1/tests/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.107063 thipster-0.22.1/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6152 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.107063 thipster-0.22.1/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.107063 thipster-0.22.1/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    18947 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    15123 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.107063 thipster-0.22.1/tests/repository/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/repository/test_github_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/repository/test_local_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 root         (0) root         (0)     3525 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     7564 2023-06-29 07:41:32.000000 thipster-0.22.1/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.107063 thipster-0.22.1/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.111063 thipster-0.22.1/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.111063 thipster-0.22.1/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.111063 thipster-0.22.1/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.115064 thipster-0.22.1/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12802 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14082 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    14974 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    23825 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.115064 thipster-0.22.1/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.115064 thipster-0.22.1/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25107 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2023-06-29 07:41:32.000000 thipster-0.22.1/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:41:36.111063 thipster-0.22.1/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-06-29 07:41:36.000000 thipster-0.22.1/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-29 07:41:36.000000 thipster-0.22.1/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:41:36.000000 thipster-0.22.1/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-29 07:41:36.000000 thipster-0.22.1/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-29 07:41:36.000000 thipster-0.22.1/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.22.0/LICENSE` & `thipster-0.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/PKG-INFO` & `thipster-0.22.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.22.0
+Version: 0.22.1
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.22.0 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.22.1 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.22.0/README.md` & `thipster-0.22.1/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/pyproject.toml` & `thipster-0.22.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/setup.py` & `thipster-0.22.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.22.0'
+__version__ = '0.22.1'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.22.0/tests/engine/test_engine.py` & `thipster-0.22.1/tests/engine/test_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,45 +58,45 @@
         return {}
 
 
 class MockTerraform(eng.TerraformPort):
     """Mock engine terraform port."""
 
     @logger('- Terraform:apply')
-    def apply(self, file):
+    def apply(self, wdir, file):
         """Mock the terraform apply method."""
         pass
 
     @logger('- Terraform:generate')
     def generate(self, a, b, auth):
         """Mock the terraform generate method."""
         pass
 
     @logger('- Terraform:init')
-    def init(self):
+    def init(self, wdir, upgrade=False):
         """Mock the terraform init method."""
         pass
 
     @logger('- Terraform:plan')
-    def plan(self, file):
+    def plan(self, wdir, file):
         """Mock the terraform plan method."""
         pass
 
 
 def test_engine_calls():
     """Test the engine calls."""
     parser = MockParser()
     repository = MockRepository()
     auth = MockAuth()
     terraform = MockTerraform()
 
     engine = eng.Engine(parser, repository, auth, terraform)
     res = engine.run(test_file)
 
-    assert res is None
+    assert res == ''
 
 
 def test_parser_failure(mocker):
     """Test the parser failure."""
 
     def parser_fail(self, filename: str):  # noqa: ARG001
         msg = 'Parser failure'
```

### Comparing `thipster-0.22.0/tests/engine/test_generation.py` & `thipster-0.22.1/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/parser/dsl_parser/test_ast.py` & `thipster-0.22.1/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.22.1/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.22.1/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/parser/dsl_parser/test_token.py` & `thipster-0.22.1/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.22.1/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/parser/test_parsedfile.py` & `thipster-0.22.1/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/parser/test_parserfactory.py` & `thipster-0.22.1/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/parser/test_yamlparser.py` & `thipster-0.22.1/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/repository/test_github_repository.py` & `thipster-0.22.1/tests/repository/test_github_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/repository/test_local_repository.py` & `thipster-0.22.1/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/repository/test_resourcemodel.py` & `thipster-0.22.1/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/tests/test_e2e.py` & `thipster-0.22.1/tests/test_e2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,37 +71,35 @@
 
     yield
 
     if delete_credentials:
         Path(AUTH_FILE_PATH).unlink()
 
 
-def test_bucket(apply_output, authentication):
+def test_bucket(authentication):
     """Test bucket creation."""
     _ = authentication
     function_name = get_function_name()
 
     bucket_name = f'test-bucket-{uuid.uuid4().int}'
     clean_up = process_file(
         directory=function_name,
         file=f"""
 bucket {bucket_name}:
 \tregion : europe-west1
     """,
+        terraform_apply=True,
     )
 
     try:
         # Assertions on plan
         assert_number_of_resource_type_is('google_storage_bucket', 1)
         bucket = assert_resource_created('google_storage_bucket', bucket_name)
         assert_resource_parameters_are(bucket, ['location'])
 
-        # Test apply
-        _ = list(apply_output(function_name))
-
     except Exception as e:
         raise e
     finally:
         clean_up()
 
 
 def test_lb(apply_output, authentication):
```

### Comparing `thipster-0.22.0/tests/test_tools.py` & `thipster-0.22.1/tests/test_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 
 from cdktf_cdktf_provider_google.provider import GoogleProvider
 
 from thipster import Engine
 from thipster.auth import Google
 from thipster.engine import AuthPort
+from thipster.helpers import execute_subprocess
 from thipster.parser import ParserFactory
 from thipster.repository import LocalRepo
 from thipster.terraform import Terraform
 
 LOCAL_REPO = 'tests/resources/e2e/models'
 REMOTE_REPO = 'THipster/models'
 
@@ -78,14 +79,15 @@
         f.write(content)
 
 
 def process_file(
         directory: str, file: str,
         local_repo: str = LOCAL_REPO, file_type: str = 'thips',
         mock_auth=False,
+        terraform_apply: bool = False,
 ):
     """Handle the file creation, engine run and clean up for the test.
 
     Parameters
     ----------
     directory : str
         The name of the directory to create.
@@ -114,33 +116,71 @@
 
         if Path('cdktf.out').exists():
             shutil.rmtree('cdktf.out')
 
         if Path('test').exists() and len(os.listdir('test')) == 0:
             shutil.rmtree('test')
 
-    engine = Engine(
-        ParserFactory(),
-        LocalRepo(local_repo),
-        Google() if not mock_auth else MockAuth(),
-        Terraform(),
-    )
+    engine = create_engine(local_repo, mock_auth)
     try:
         engine.run(f'test/{directory}')
         shutil.move(
             Path(Path.cwd(), 'thipster.tf.json'),
             Path(Path.cwd(), f'test/{directory}', 'thipster.tf.json'),
         )
+        if terraform_apply:
+            apply_terraform(engine, f'test/{directory}')
+
     except Exception as e:
         clean_up()
         raise e
 
     return clean_up
 
 
+def apply_terraform(
+    engine: Engine,
+    directory_path: str,
+):
+    """Apply terraform using thipster functions."""
+    working_dir = Path(Path.cwd(), directory_path)
+    assert engine.init_terraform(working_dir)[0] == 0
+    assert engine.plan_terraform(working_dir)[0] == 0
+    assert engine.apply_terraform(working_dir)[0] == 0
+
+    destroy_result = execute_subprocess(
+        ['terraform', 'destroy', '-auto-approve'],
+        cwd=working_dir,
+    )
+
+    if destroy_result[0] != 0:
+        raise Exception(destroy_result[1])
+
+
+def create_engine(
+    local_repo: str = LOCAL_REPO,
+    mock_auth=False,
+) -> Engine:
+    """Create a THipster engine instance.
+
+    Parameters
+    ----------
+    local_repo : str
+        The path to the local repository.
+    mock_auth : bool
+        Whether to mock the authentication to GCP. Defaults to False.
+    """
+    return Engine(
+        ParserFactory(),
+        LocalRepo(local_repo),
+        Google() if not mock_auth else MockAuth(),
+        Terraform(),
+    )
+
+
 def __get_output(test_name):
     with Path(f'test/{test_name}/thipster.tf.json').open() as f:
         file_contents = json.load(f)
         f.close()
     return file_contents
```

### Comparing `thipster-0.22.0/thipster/auth/google.py` & `thipster-0.22.1/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/engine/engine.py` & `thipster-0.22.1/thipster/engine/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Engine.py module."""
+from pathlib import Path
 
 import thipster.engine.parsed_file as pf
 
 from .i_auth import AuthPort
 from .i_parser import ParserPort
 from .i_repository import RepositoryPort
 from .i_terraform import TerraformPort
@@ -89,44 +90,50 @@
     @terraform.setter
     def terraform(self, value):
         if not isinstance(value, TerraformPort):
             raise Exception
 
         self.__terraform = value
 
-    def run(self, path: str) -> tuple[list[str], str]:
+    def run(self, path: str) -> str:
         """Return json Terraform files from the input file name.
 
         Calls the different run methods of the parser, repository,
         auth and terraform modules.
         Transforms the inputed filename into a Cloud architecture plan.
 
         Parameters
         ----------
         path : str
             The path of the files to be processed
 
         Returns
         -------
-        tuple[list[str], str]
-            A tuple made up of the list of directories containing the Terraform json
-            files and a string with the results of the Terraform plan
+        str
+            A string with the results of the Terraform plan
         """
         # Parse file or directory
         parsed_file = self.parse_files(path)
 
         # Get needed models
         models = self.get_models(parsed_file)
 
         # Generate Terraform files
         self.generate_tf_files(parsed_file, models)
 
-        self.__terraform.init()
+        self.init_terraform()
+
+        terraform_plan = self.plan_terraform(
+            plan_file_path=terraform_plan_file,
+        )
+
+        if not terraform_plan:
+            return ''
 
-        return self.__terraform.plan(terraform_plan_file)
+        return terraform_plan[1]
 
     def parse_files(self, path: str) -> pf.ParsedFile:
         """Parse the input file or directory.
 
         Parameters
         ----------
         path : str
@@ -170,40 +177,69 @@
         file : pf.ParsedFile
             The ParsedFile object containing the resources defined in the input file
         models : dict[str, ResourceModel]
             The dictionary of models
         """
         self.__terraform.generate(file, models, self.__auth)
 
-    def init_terraform(self) -> None:
-        """Initialize Terraform."""
-        self.__terraform.init()
+    def init_terraform(
+        self,
+        working_dir: Path = Path.cwd(),
+        upgrade: bool = False,
+    ) -> tuple[int, str]:
+        """Initialize Terraform.
+
+        Parameters
+        ----------
+        working_dir : Path, optional
+            The path of the working directory, by default Path.cwd()
+        upgrade : bool, optional
+            Whether to upgrade the Terraform providers, by default False
+
+        Returns
+        -------
+        tuple[int, str]
+            The terraform init exit code and output
+        """
+        return self.__terraform.init(working_dir, upgrade)
 
-    def plan_terraform(self, plan_file_path: str = terraform_plan_file) -> str:
+    def plan_terraform(
+        self,
+        working_dir: Path = Path.cwd(),
+        plan_file_path: str = terraform_plan_file,
+    ) -> tuple[int, str]:
         """Plan Terraform.
 
         Parameters
         ----------
+        working_dir : Path, optional
+            The path of the working directory, by default Path.cwd()
         plan_file_path : str, optional
             The path of the plan file, by default thipster.tfplan
 
         Returns
         -------
-        str
-            The results of the Terraform plan
+        tuple[int, str]
+            The terraform plan exit code and output
         """
-        return self.__terraform.plan(plan_file_path)
+        return self.__terraform.plan(working_dir, plan_file_path)
 
-    def apply_terraform(self, plan_file_path: str = terraform_plan_file) -> str:
+    def apply_terraform(
+        self,
+        working_dir: Path = Path.cwd(),
+        plan_file_path: str = terraform_plan_file,
+    ) -> tuple[int, str]:
         """Apply Terraform.
 
         Parameters
         ----------
+        working_dir : Path, optional
+            The path of the working directory, by default Path.cwd()
         plan_file_path : str, optional
             The path of the plan file, by default thipster.tfplan
 
         Returns
         -------
-        str
-            The results of the Terraform apply
+        tuple[int, str]
+            The terraform apply exit code and output
         """
-        return self.__terraform.apply(plan_file_path)
+        return self.__terraform.apply(working_dir, plan_file_path)
```

### Comparing `thipster-0.22.0/thipster/engine/i_parser.py` & `thipster-0.22.1/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/engine/i_repository.py` & `thipster-0.22.1/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/engine/i_terraform.py` & `thipster-0.22.1/thipster/engine/i_terraform.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 """Terraform module interface."""
 from abc import ABC, abstractclassmethod
+from pathlib import Path
 
 import thipster.engine.parsed_file as pf
 import thipster.engine.resource_model as rm
 
 from .i_auth import AuthPort
 
 
 class TerraformPort(ABC):
     """Terraform port."""
 
     @classmethod
     @abstractclassmethod
     def apply(
         cls,
+        working_dir: Path,  # noqa: ARG003
         plan_file_path: str | None = None,  # noqa: ARG003
-    ):
+    ) -> tuple[int, str]:
         """Apply generated terraform code.
 
         Parameters
         ----------
+        working_dir : Path
+            Path to the working directory
         plan_file_path : str, optional
             Path to plan file, by default None
 
+        Returns
+        -------
+        tuple[int, str]
+            The Terraform apply exit code and output
+
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
         msg = 'Should implement apply()'
@@ -56,31 +65,54 @@
 
         """
         msg = 'Should implement generate()'
         raise NotImplementedError(msg)
 
     @classmethod
     @abstractclassmethod
-    def init(cls):
+    def init(cls, working_dir: Path, upgrade: bool):  # noqa: ARG003
         """Init Terraform for generated terraform code.
 
+        Parameters
+        ----------
+        working_dir : Path
+            Path to the working directory
+        upgrade : bool
+            Whether to upgrade Terraform providers or not
+
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
         msg = 'Should implement generate()'
         raise NotImplementedError(msg)
 
     @classmethod
     @abstractclassmethod
-    def plan(cls):
+    def plan(
+        cls,
+        working_dir: Path,  # noqa: ARG003
+        plan_file_path: str,  # noqa: ARG003
+    ) -> tuple[int, str]:
         """Get plan from generated terraform code.
 
+        Parameters
+        ----------
+        working_dir : Path
+            Path to the working directory
+        plan_file_path : str
+            Path and name of the plan file
+
+        Returns
+        -------
+        tuple[int, str]
+            Terraform plan exitcode and output
+
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
         msg = 'Should implement plan()'
```

### Comparing `thipster-0.22.0/thipster/engine/parsed_file.py` & `thipster-0.22.1/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/engine/resource_model.py` & `thipster-0.22.1/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/parser/dsl_parser/ast.py` & `thipster-0.22.1/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.22.1/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.22.1/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/parser/dsl_parser/lexer.py` & `thipster-0.22.1/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.22.1/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/parser/dsl_parser/parser.py` & `thipster-0.22.1/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/parser/dsl_parser/token.py` & `thipster-0.22.1/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.22.1/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/parser/exceptions.py` & `thipster-0.22.1/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/parser/parser_factory.py` & `thipster-0.22.1/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/parser/yaml_parser.py` & `thipster-0.22.1/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/repository/exceptions.py` & `thipster-0.22.1/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/repository/github.py` & `thipster-0.22.1/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/repository/json.py` & `thipster-0.22.1/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/repository/local.py` & `thipster-0.22.1/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster/terraform/cdk.py` & `thipster-0.22.1/thipster/terraform/cdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 import subprocess
 import sys
 import uuid
 from pathlib import Path
 
 from cdktf import App, TerraformStack
 from constructs import Construct
-from python_terraform import Terraform
 
 import thipster.engine.parsed_file as pf
 import thipster.engine.resource_model as rm
 import thipster.terraform.exceptions as cdk_exceptions
 from thipster.engine import AuthPort, TerraformPort
-from thipster.helpers import create_logger
+from thipster.helpers import create_logger, execute_subprocess
 
 
 class ResourceCreationContext:
     """Context from which a resource is created."""
 
     def __init__(
         self,
@@ -132,34 +131,37 @@
     _resources_to_create: list[ResourceCreationContext] = []
 
     _inherited_attributes: list[pf.ParsedAttribute] = []
     _created_resources = {}
     _logger = create_logger(__name__)
 
     @classmethod
-    def apply(cls, plan_file_path: str):
+    def apply(
+        cls,
+        working_dir: Path,
+        plan_file_path: str,
+    ) -> tuple[int, str]:
         """Apply generated Terraform plan.
 
         Parameters
         ----------
+        working_dir : Path
+            Path to the working directory
         plan_file_path : str
             Path to the plan file
 
         Returns
         -------
-        str
-            Terraform apply output
+        tuple[int, str]
+            Terraform apply exitcode and output
         """
-        output = subprocess.run(
-            ['terrraform', 'apply', plan_file_path],
-            shell=True,
-            capture_output=True,
-            encoding='utf-8',
+        return execute_subprocess(
+            ['terraform', 'apply', plan_file_path],
+            cwd=working_dir,
         )
-        return output.stdout + output.stderr
 
     @classmethod
     def generate(
         cls, file: pf.ParsedFile, models: dict[str, rm.ResourceModel],
         _authenticator: AuthPort,
     ):
         """Generate Terraform file from given parsed file and models.
@@ -236,43 +238,67 @@
             Path(dirname).rmdir()
         for content in os.listdir(Path(Path.cwd(), 'cdktf.out')):
             d = f'cdktf.out/{content}'
             Path(d).rmdir() if Path(d).is_dir() else Path(d).unlink()
         Path('cdktf.out').rmdir()
 
     @classmethod
-    def init(cls):
+    def init(
+        cls,
+        working_dir: Path,
+        upgrade: bool = False,
+    ) -> tuple[int, str]:
         """Initilize terraform.
 
+        Parameters
+        ----------
+        working_dir : Path
+            Path to the working directory
+        upgrade : bool, optional
+            If terraform providers should be upgraded, by default False
+
         Returns
         -------
-        str
-            Terraform init output
+        tuple[int, str]
+            Terraform init exitcode and output
         """
-        t = Terraform()
-        _, stdout, stderr = t.init(upgrade=True)
-        return stdout + stderr
+        cmd = ['terraform', 'init']
+
+        if upgrade:
+            cmd.append('-upgrade')
+
+        return execute_subprocess(
+            cmd,
+            cwd=working_dir,
+        )
 
     @classmethod
-    def plan(cls, plan_file_path: str):
+    def plan(
+        cls,
+        working_dir: Path,
+        plan_file_path: str,
+    ) -> tuple[int, str]:
         """Get plan from generated terraform code.
 
         Parameters
         ----------
+        working_dir : Path
+            Path to the working directory
         plan_file_path : str
             Path and name of the plan file
 
         Returns
         -------
-        str
-            Terraform plan output
+        tuple[int, str]
+            Terraform plan exitcode and output
         """
-        t = Terraform()
-        _, stdout, stderr = t.plan(out=plan_file_path)
-        return stdout + stderr
+        return execute_subprocess(
+            ['terraform', 'plan', f'-out={plan_file_path}'],
+            cwd=working_dir,
+        )
 
     @classmethod
     def _pip_install(cls, package: str):
         """Install a package if it wasn't already installed by thipster.
 
         Parameters
         ----------
```

### Comparing `thipster-0.22.0/thipster/terraform/exceptions.py` & `thipster-0.22.1/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.22.0/thipster.egg-info/PKG-INFO` & `thipster-0.22.1/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.22.0
+Version: 0.22.1
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.22.0 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.22.1 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.22.0/thipster.egg-info/SOURCES.txt` & `thipster-0.22.1/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

