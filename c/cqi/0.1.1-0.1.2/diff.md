# Comparing `tmp/cqi-0.1.1.tar.gz` & `tmp/cqi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqi-0.1.1.tar", last modified: Thu Jun 22 10:31:04 2023, max compression
+gzip compressed data, was "cqi-0.1.2.tar", last modified: Thu Jun 29 10:15:01 2023, max compression
```

## Comparing `cqi-0.1.1.tar` & `cqi-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 10:31:04.787203 cqi-0.1.1/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1072 2023-06-22 07:21:07.000000 cqi-0.1.1/LICENSE
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1537 2023-06-22 10:31:04.787203 cqi-0.1.1/PKG-INFO
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1051 2023-06-22 10:12:13.000000 cqi-0.1.1/README.md
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 10:31:04.777203 cqi-0.1.1/cqi/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      166 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/__init__.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 10:31:04.787203 cqi-0.1.1/cqi/api/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       45 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/api/__init__.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    21032 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/api/client.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    12641 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/api/specification.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1934 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/client.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     5821 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/errors.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 10:31:04.787203 cqi-0.1.1/cqi/models/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/models/__init__.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     5485 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/models/attributes.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2520 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/models/corpora.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2422 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/models/resource.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3216 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/models/subcorpora.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1084 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/status.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      145 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/version.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 10:31:04.787203 cqi-0.1.1/cqi.egg-info/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1537 2023-06-22 10:31:04.000000 cqi-0.1.1/cqi.egg-info/PKG-INFO
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      388 2023-06-22 10:31:04.000000 cqi-0.1.1/cqi.egg-info/SOURCES.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        1 2023-06-22 10:31:04.000000 cqi-0.1.1/cqi.egg-info/dependency_links.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        4 2023-06-22 10:31:04.000000 cqi-0.1.1/cqi.egg-info/top_level.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       38 2023-06-22 10:31:04.787203 cqi-0.1.1/setup.cfg
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      781 2023-06-22 07:21:07.000000 cqi-0.1.1/setup.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-29 10:15:01.528545 cqi-0.1.2/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1072 2023-06-22 07:21:07.000000 cqi-0.1.2/LICENSE
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1576 2023-06-29 10:15:01.518545 cqi-0.1.2/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1090 2023-06-29 10:11:38.000000 cqi-0.1.2/README.md
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-29 10:15:01.518545 cqi-0.1.2/cqi/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      166 2023-06-22 09:48:22.000000 cqi-0.1.2/cqi/__init__.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-29 10:15:01.518545 cqi-0.1.2/cqi/api/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       45 2023-06-22 09:48:22.000000 cqi-0.1.2/cqi/api/__init__.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    20849 2023-06-29 09:21:22.000000 cqi-0.1.2/cqi/api/client.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    12641 2023-06-22 09:48:22.000000 cqi-0.1.2/cqi/api/specification.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1934 2023-06-29 08:20:25.000000 cqi-0.1.2/cqi/client.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     5016 2023-06-28 11:38:07.000000 cqi-0.1.2/cqi/errors.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-29 10:15:01.518545 cqi-0.1.2/cqi/models/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 09:48:22.000000 cqi-0.1.2/cqi/models/__init__.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     7097 2023-06-29 08:09:02.000000 cqi-0.1.2/cqi/models/attributes.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2599 2023-06-29 09:22:31.000000 cqi-0.1.2/cqi/models/corpora.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2345 2023-06-29 08:07:30.000000 cqi-0.1.2/cqi/models/resource.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3927 2023-06-29 08:08:13.000000 cqi-0.1.2/cqi/models/subcorpora.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1084 2023-06-22 09:48:22.000000 cqi-0.1.2/cqi/status.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      145 2023-06-29 10:10:28.000000 cqi-0.1.2/cqi/version.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-29 10:15:01.518545 cqi-0.1.2/cqi.egg-info/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1576 2023-06-29 10:15:01.000000 cqi-0.1.2/cqi.egg-info/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      388 2023-06-29 10:15:01.000000 cqi-0.1.2/cqi.egg-info/SOURCES.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        1 2023-06-29 10:15:01.000000 cqi-0.1.2/cqi.egg-info/dependency_links.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        4 2023-06-29 10:15:01.000000 cqi-0.1.2/cqi.egg-info/top_level.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       38 2023-06-29 10:15:01.528545 cqi-0.1.2/setup.cfg
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      781 2023-06-22 07:21:07.000000 cqi-0.1.2/setup.py
```

### Comparing `cqi-0.1.1/LICENSE` & `cqi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cqi-0.1.1/PKG-INFO` & `cqi-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqi
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
 Home-page: https://github.com/Pevtrick/cqi-py
 Author: Patrick Jentsch
 Author-email: patrickjentsch@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,14 +26,15 @@
 
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
 | 0.1.0           | 0.1              |
 | 0.1.1           | 0.1              |
+| 0.1.2           | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.1/README.md` & `cqi-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
 | 0.1.0           | 0.1              |
 | 0.1.1           | 0.1              |
+| 0.1.2           | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.1/cqi/api/client.py` & `cqi-0.1.2/cqi/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,16 @@
 
     def ctrl_ping(self) -> status.StatusPingOk:
         self.__send_WORD(specification.CTRL_PING)
         return self.__recv_response()
 
     def ctrl_last_general_error(self) -> str:
         ''' 
-            Full-text error message for the last general error reported by the
-            CQi server
+        Full-text error message for the last general error reported by the CQi
+        server
         '''
         self.__send_WORD(specification.CTRL_LAST_GENERAL_ERROR)
         return self.__recv_response()
 
     def ask_feature_cqi_1_0(self) -> bool:
         self.__send_WORD(specification.ASK_FEATURE_CQI_1_0)
         return self.__recv_response()
@@ -86,15 +86,15 @@
         self.__send_WORD(specification.ASK_FEATURE_CL_2_3)
         return self.__recv_response()
 
     def ask_feature_cqp_2_3(self) -> bool:
         self.__send_WORD(specification.ASK_FEATURE_CL_2_3)
         return self.__recv_response()
 
-    def corpus_list_coprora(self) -> List[str]:
+    def corpus_list_corpora(self) -> List[str]:
         self.__send_WORD(specification.CORPUS_LIST_CORPORA)
         return self.__recv_response()
 
     def corpus_charset(self, corpus: str) -> str:
         self.__send_WORD(specification.CORPUS_CHARSET)
         self.__send_STRING(corpus)
         return self.__recv_response()
@@ -128,44 +128,43 @@
         ''' the full name of <corpus> as specified in its registry entry '''
         self.__send_WORD(specification.CORPUS_FULL_NAME)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
     def corpus_info(self, corpus: str) -> List[str]:
         ''' 
-            returns the contents of the .info file of <corpus> as a list of
-            lines
+        returns the contents of the .info file of <corpus> as a list of lines
         '''
         self.__send_WORD(specification.CORPUS_INFO)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
     def corpus_drop_corpus(self, corpus: str) -> status.StatusOk:
         ''' try to unload a corpus and all its attributes from memory '''
         self.__send_WORD(specification.CORPUS_DROP_CORPUS)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
     def cl_attribute_size(self, attribute: str) -> int:
         ''' 
-            returns the size of <attribute>:
-            - number of tokens        (positional)
-            - number of regions       (structural)
-            - number of alignments    (alignment)
+        returns the size of <attribute>:
+        - number of tokens        (positional)
+        - number of regions       (structural)
+        - number of alignments    (alignment)
         '''
         self.__send_WORD(specification.CL_ATTRIBUTE_SIZE)
         self.__send_STRING(attribute)
         return self.__recv_response()
 
     def cl_lexicon_size(self, attribute: str) -> int:
         '''
-            returns the number of entries in the lexicon of a positional
-            attribute;
+        returns the number of entries in the lexicon of a positional
+        attribute;
 
-            valid lexicon IDs range from 0 .. (lexicon_size - 1)
+        valid lexicon IDs range from 0 .. (lexicon_size - 1)
         '''
         self.__send_WORD(specification.CL_LEXICON_SIZE)
         self.__send_STRING(attribute)
         return self.__recv_response()
 
     def cl_drop_attribute(self, attribute: str) -> status.StatusOk:
         ''' unload attribute from memory '''
@@ -176,16 +175,16 @@
     '''
     ' NOTE: simple (scalar) mappings are applied to lists (the returned list
     '       has exactly the same length as the list passed as an argument)
     '''
 
     def cl_str2id(self, attribute: str, strings: List[str]) -> List[int]:
         '''
-            returns -1 for every string in <strings> that is not found in the
-            lexicon
+        returns -1 for every string in <strings> that is not found in the
+        lexicon
         '''
         self.__send_WORD(specification.CL_STR2ID)
         self.__send_STRING(attribute)
         self.__send_STRING_LIST(strings)
         return self.__recv_response()
 
     def cl_id2str(self, attribute: str, id: List[int]) -> List[str]:
@@ -200,60 +199,58 @@
         self.__send_WORD(specification.CL_ID2FREQ)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(id)
         return self.__recv_response()
 
     def cl_cpos2id(self, attribute: str, cpos: List[int]) -> List[int]:
         ''' 
-            returns -1 for every corpus position in <cpos> that is out of
-            range
+        returns -1 for every corpus position in <cpos> that is out of range
         '''
         self.__send_WORD(specification.CL_CPOS2ID)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
     def cl_cpos2str(self, attribute: str, cpos: List[int]) -> List[str]:
         '''
-            returns "" for every corpus position in <cpos> that is out of
-            range
+        returns "" for every corpus position in <cpos> that is out of range
         '''
         self.__send_WORD(specification.CL_CPOS2STR)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
     def cl_cpos2struc(self, attribute: str, cpos: List[int]) -> List[int]:
         '''
-            returns -1 for every corpus position not inside a structure region
+        returns -1 for every corpus position not inside a structure region
         '''
         self.__send_WORD(specification.CL_CPOS2STRUC)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
     '''
     ' NOTE: temporary addition for the Euralex2000 tutorial, but should
     '       probably be included in CQi specs
     '''
 
     def cl_cpos2lbound(self, attribute: str, cpos: List[int]) -> List[int]:
         '''
-            returns left boundary of s-attribute region enclosing cpos, -1 if
-            not in region
+        returns left boundary of s-attribute region enclosing cpos, -1 if not
+        in region
         '''
         self.__send_WORD(specification.CL_CPOS2LBOUND)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
     def cl_cpos2rbound(self, attribute: str, cpos: List[int]) -> List[int]:
         '''
-            returns right boundary of s-attribute region enclosing cpos, -1 if
-            not in region
+        returns right boundary of s-attribute region enclosing cpos, -1 if not
+        in region
         '''
         self.__send_WORD(specification.CL_CPOS2RBOUND)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
     def cl_cpos2alg(self, attribute: str, cpos: List[int]) -> List[int]:
@@ -261,18 +258,18 @@
         self.__send_WORD(specification.CL_CPOS2ALG)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
     def cl_struc2str(self, attribute: str, strucs: List[int]) -> List[str]:
         '''
-            returns annotated string values of structure regions in <strucs>;
-            "" if out of range
+        returns annotated string values of structure regions in <strucs>;
+        "" if out of range
 
-            check corpus_structural_attribute_has_values(<attribute>) first
+        check corpus_structural_attribute_has_values(<attribute>) first
         '''
         self.__send_WORD(specification.CL_STRUC2STR)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(strucs)
         return self.__recv_response()
 
     '''
@@ -285,35 +282,35 @@
         self.__send_WORD(specification.CL_ID2CPOS)
         self.__send_STRING(attribute)
         self.__send_INT(id)
         return self.__recv_response()
 
     def cl_idlist2cpos(self, attribute: str, id_list: List[int]) -> List[int]:
         '''
-            returns all corpus positions where one of the tokens in <id_list>
-            occurs; the returned list is sorted as a whole, not per token id
+        returns all corpus positions where one of the tokens in <id_list>
+        occurs; the returned list is sorted as a whole, not per token id
         '''
         self.__send_WORD(specification.CL_IDLIST2CPOS)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(id_list)
         return self.__recv_response()
 
     def cl_regex2id(self, attribute: str, regex: str) -> List[int]:
         '''
-            returns lexicon IDs of all tokens that match <regex>; the returned
-            list may be empty (size 0);
+        returns lexicon IDs of all tokens that match <regex>; the returned
+        list may be empty (size 0);
         '''
         self.__send_WORD(specification.CL_REGEX2ID)
         self.__send_STRING(attribute)
         self.__send_STRING(regex)
         return self.__recv_response()
 
     def cl_struc2cpos(self, attribute: str, struc: int) -> Tuple[int, int]:
         '''
-            returns start and end corpus positions of structure region <struc>
+        returns start and end corpus positions of structure region <struc>
         '''
         self.__send_WORD(specification.CL_STRUC2CPOS)
         self.__send_STRING(attribute)
         self.__send_INT(struc)
         return self.__recv_response()
 
     def cl_alg2cpos(self, attribute: str, alg: int) -> Tuple[int, int, int, int]:
@@ -355,16 +352,16 @@
         self,
         subcorpus: str,
         field: int,
         first: int,
         last: int
     ) -> List[int]:
         '''
-            Dump the values of <field> for match ranges <first> .. <last>
-            in <subcorpus>. <field> is one of the CQI_CONST_FIELD_* constants.
+        Dump the values of <field> for match ranges <first> .. <last> in
+        <subcorpus>. <field> is one of the CQI_CONST_FIELD_* constants.
         '''
         self.__send_WORD(specification.CQP_DUMP_SUBCORPUS)
         self.__send_STRING(subcorpus)
         self.__send_BYTE(field)
         self.__send_INT(first)
         self.__send_INT(last)
         return self.__recv_response()
@@ -383,24 +380,25 @@
     def cqp_fdist_1(
         self,
         subcorpus: str,
         cutoff: int,
         field: int,
         attribute: str
     ) -> List[int]:
-        ''' frequency distribution of single tokens
+        '''
+        frequency distribution of single tokens
+
+        returns <n> (id, frequency) pairs flattened into a list of size 2*<n>
 
-            returns <n> (id, frequency) pairs flattened into a list of size
-            2*<n>
-            field is one of
-            - CQI_CONST_FIELD_MATCH
-            - CQI_CONST_FIELD_TARGET
-            - CQI_CONST_FIELD_KEYWORD
+        field is one of
+        - CQI_CONST_FIELD_MATCH
+        - CQI_CONST_FIELD_TARGET
+        - CQI_CONST_FIELD_KEYWORD
 
-            NB: pairs are sorted by frequency desc.
+        NB: pairs are sorted by frequency desc.
         '''
         self.__send_WORD(specification.CQP_FDIST_1)
         self.__send_STRING(subcorpus)
         self.__send_INT(cutoff)
         self.__send_BYTE(field)
         self.__send_STRING(attribute)
         return self.__recv_response()
@@ -410,20 +408,21 @@
         subcorpus: str,
         cutoff: int,
         field1: int,
         attribute1: str,
         field2: int,
         attribute2: str
     ) -> List[int]:
-        ''' frequency distribution of pairs of tokens
+        '''
+        frequency distribution of pairs of tokens
 
-            returns <n> (id1, id2, frequency) pairs flattened into a list of
-            size 3*<n>
+        returns <n> (id1, id2, frequency) pairs flattened into a list of size
+        3*<n>
 
-            NB: triples are sorted by frequency desc.
+        NB: triples are sorted by frequency desc.
         '''
         self.__send_WORD(specification.CQP_FDIST_2)
         self.__send_STRING(subcorpus)
         self.__send_INT(cutoff)
         self.__send_BYTE(field1)
         self.__send_STRING(attribute1)
         self.__send_BYTE(field2)
```

### Comparing `cqi-0.1.1/cqi/api/specification.py` & `cqi-0.1.2/cqi/api/specification.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.1/cqi/client.py` & `cqi-0.1.2/cqi/client.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.1/cqi/errors.py` & `cqi-0.1.2/cqi/errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,111 +7,99 @@
     If you want to catch all errors that the CQi package might raise,
     catch this base exception.
     '''
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = None
-        self.name = None
         self.description = None
 
 
 class Error(CQiException):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.ERROR
 
 
 class ErrorGeneralError(Error):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.ERROR_GENERAL_ERROR
-        self.name = specification.lookup[self.code]
 
 
 class ErrorConnectRefused(Error):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.ERROR_CONNECT_REFUSED
-        self.name = specification.lookup[self.code]
 
 
 class ErrorUserAbort(Error):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.ERROR_USER_ABORT
-        self.name = specification.lookup[self.code]
 
 
 class ErrorSyntaxError(Error):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.ERROR_SYNTAX_ERROR
-        self.name = specification.lookup[self.code]
 
 
 class CLError(CQiException):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR
 
 
 class CLErrorNoSuchAttribute(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_NO_SUCH_ATTRIBUTE
-        self.name = specification.lookup[self.code]
         self.description = 'CQi server couldn\'t open attribute'
 
 
 class CLErrorWrongAttributeType(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_WRONG_ATTRIBUTE_TYPE
-        self.name = specification.lookup[self.code]
 
 
 class CLErrorOutOfRange(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_OUT_OF_RANGE
-        self.name = specification.lookup[self.code]
 
 
 class CLErrorRegex(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_REGEX
-        self.name = specification.lookup[self.code]
 
 
 class CLErrorCorpusAccess(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_CORPUS_ACCESS
-        self.name = specification.lookup[self.code]
         self.description = ''
 
 
 class CLErrorOutOfMemory(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_OUT_OF_MEMORY
-        self.name = specification.lookup[self.code]
         self.description = (
             'CQi server has run out of memory; try discarding some other '
             'corpora and/or subcorpora'
         )
 
 
 class CLErrorInternal(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_INTERNAL
-        self.name = specification.lookup[self.code]
         self.description = (
             'The classical \'please contact technical support\' error'
         )
 
 
 class CQPError(CQiException):
     # CQP error messages yet to be defined
@@ -120,36 +108,32 @@
         self.code = specification.CQP_ERROR
 
 
 class CQPErrorGeneral(CQPError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CQP_ERROR_GENERAL
-        self.name = specification.lookup[self.code]
 
 
 class CQPErrorNoSuchCorpus(CQPError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CQP_ERROR_NO_SUCH_CORPUS
-        self.name = specification.lookup[self.code]
 
 
 class CQPErrorInvalidField(CQPError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CQP_ERROR_INVALID_FIELD
-        self.name = specification.lookup[self.code]
 
 
 class CQPErrorOutOfRange(CQPError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CQP_ERROR_OUT_OF_RANGE
-        self.name = specification.lookup[self.code]
         self.description = 'A number is out of range'
 
 
 error_lookup = {
     specification.ERROR: Error,
     specification.ERROR_GENERAL_ERROR: ErrorGeneralError,
     specification.ERROR_CONNECT_REFUSED: ErrorConnectRefused,
```

### Comparing `cqi-0.1.1/cqi/models/attributes.py` & `cqi-0.1.2/cqi/models/attributes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-from typing import Dict, List, Tuple, TYPE_CHECKING
+from typing import Dict, List, Tuple, Type, TYPE_CHECKING
 if TYPE_CHECKING:
     from ..client import CQiClient
     from ..status import StatusOk
     from .corpora import Corpus
 from .resource import Collection, Model
 
 
 class Attribute(Model):
-    id_attribute: str = 'api_name'
-
     @property
     def api_name(self) -> str:
         return self.attrs.get('api_name')
 
     @property
     def name(self) -> str:
         return self.attrs.get('name')
 
     @property
     def size(self) -> int:
         return self.attrs.get('size')
 
     def drop(self) -> 'StatusOk':
+        ''' unload attribute from memory '''
         return self.client.api.cl_drop_attribute(self.api_name)
 
 
 class AttributeCollection(Collection):
-    model: Attribute = Attribute
+    model: Type[Attribute] = Attribute
 
     def __init__(self, client: 'CQiClient' = None, corpus: 'Corpus' = None):
         super().__init__(client=client)
         self.corpus: 'Corpus' = corpus
 
     def _get(self, attribute_name: str) -> Dict:
         api_name: str = f'{self.corpus.api_name}.{attribute_name}'
@@ -44,109 +43,155 @@
         return self.prepare_model(self._get(attribute_name))
 
     def list(self) -> List[Attribute]:
         raise NotImplementedError
 
 
 class AlignmentAttribute(Attribute):
-    def cpos_by_ids(self, id: int) -> Tuple[int, int, int, int]:
+    def cpos_by_id(self, id: int) -> Tuple[int, int, int, int]:
+        ''' returns (src_start, src_end, target_start, target_end) '''
         return self.client.api.cl_alg2cpos(self.api_name, id)
 
     def ids_by_cpos(self, cpos_list: List[int]) -> List[int]:
+        ''' returns -1 for every corpus position not inside an alignment '''
         return self.client.api.cl_cpos2alg(self.api_name, cpos_list)
 
 
 class AlignmentAttributeCollection(AttributeCollection):
-    model: AlignmentAttribute = AlignmentAttribute
+    model: Type[AlignmentAttribute] = AlignmentAttribute
 
     def list(self) -> List[AlignmentAttribute]:
         return [
-            self.prepare_model(self._get(x)) for x
-            in self.client.api.corpus_alignment_attributes(self.corpus.api_name)
+            self.get(x) for x in
+            self.client.api.corpus_alignment_attributes(self.corpus.api_name)
         ]
 
 
 class PositionalAttribute(Attribute):
     @property
     def lexicon_size(self) -> int:
         return self.attrs.get('lexicon_size')
 
     def cpos_by_id(self, id: int) -> List[int]:
+        ''' returns all corpus positions where the given token occurs '''
         return self.client.api.cl_id2cpos(self.api_name, id)
 
     def cpos_by_ids(self, id_list: List[int]) -> List[int]:
+        '''
+        returns all corpus positions where one of the tokens in <id_list>
+        occurs; the returned list is sorted as a whole, not per token id
+        '''
         return self.client.api.cl_idlist2cpos(self.api_name, id_list)
 
     def freqs_by_ids(self, id_list: List[int]) -> List[int]:
+        ''' returns 0 for every ID in <id_list> that is out of range '''
         return self.client.api.cl_id2freq(self.api_name, id_list)
 
     def ids_by_cpos(self, cpos_list: List[int]) -> List[int]:
+        '''
+        returns -1 for every corpus position in <cpos_list> that is out of
+        range
+        '''
         return self.client.api.cl_cpos2id(self.api_name, cpos_list)
 
     def ids_by_regex(self, regex: str) -> List[int]:
+        '''
+        returns lexicon IDs of all tokens that match <regex>; the returned
+        list may be empty (size 0);
+        '''
         return self.client.api.cl_regex2id(self.api_name, regex)
 
     def ids_by_values(self, value_list: List[str]) -> List[int]:
+        '''
+        returns -1 for every string in <value_list> that is not found in the
+        lexicon
+        '''
         return self.client.api.cl_str2id(self.api_name, value_list)
 
     def values_by_cpos(self, cpos_list: List[int]) -> List[str]:
+        '''
+        returns "" for every corpus position in <cpos_list> that is out of
+        range
+        '''
         return self.client.api.cl_cpos2str(self.api_name, cpos_list)
 
     def values_by_ids(self, id_list: List[int]) -> List[str]:
+        ''' returns "" for every ID in <id_list> that is out of range '''
         return self.client.api.cl_id2str(self.api_name, id_list)
 
 
 class PositionalAttributeCollection(AttributeCollection):
-    model: PositionalAttribute = PositionalAttribute
+    model: Type[PositionalAttribute] = PositionalAttribute
 
     def _get(self, positional_attribute_name: str) -> Dict:
         attrs = super()._get(positional_attribute_name)
         attrs['lexicon_size'] = self.client.api.cl_lexicon_size(attrs['api_name'])
         return attrs
 
     def list(self) -> List[PositionalAttribute]:
         return [
-            self.prepare_model(self._get(x)) for x
-            in self.client.api.corpus_positional_attributes(self.corpus.api_name)
+            self.get(x) for x in
+            self.client.api.corpus_positional_attributes(self.corpus.api_name)
         ]
 
 
 class StructuralAttribute(Attribute):
     @property
     def has_values(self) -> bool:
         return self.attrs.get('has_values')
 
     def cpos_by_id(self, id: int) -> Tuple[int, int]:
+        '''
+        returns start and end corpus positions of structure region with id
+        <id>
+        '''
         return self.client.api.cl_struc2cpos(self.api_name, id)
 
     def ids_by_cpos(self, cpos_list: List[int]) -> List[int]:
+        '''
+        returns -1 for every corpus position not inside a structure region
+        '''
         return self.client.api.cl_cpos2struc(self.api_name, cpos_list)
 
     def lbound_by_cpos(self, cpos_list: List[int]) -> List[int]:
+        '''
+        returns left boundary of s-attribute region enclosing cpos, -1 if not
+        in region
+        '''
         return self.client.api.cl_cpos2lbound(self.api_name, cpos_list)
 
     def rbound_by_cpos(self, cpos_list: List[int]) -> List[int]:
+        '''
+        returns right boundary of s-attribute region enclosing cpos, -1 if not
+        in region
+        '''
         return self.client.api.cl_cpos2rbound(self.api_name, cpos_list)
 
-    def values_by_ids(self, id_list: List[int]) -> List[int]:
+    def values_by_ids(self, id_list: List[int]) -> List[str]:
+        '''
+        returns annotated string values of structure regions in <id_list>; ""
+        if out of range
+
+        check has_values property first
+        '''
         return self.client.api.cl_struc2str(self.api_name, id_list)
 
 
 class StructuralAttributeCollection(AttributeCollection):
-    model: StructuralAttribute = StructuralAttribute
+    model: Type[StructuralAttribute] = StructuralAttribute
 
     def _get(self, structural_attribute_name: str) -> Dict:
         attrs = super()._get(structural_attribute_name)
         attrs['has_values'] = self.client.api.corpus_structural_attribute_has_values(attrs['api_name'])
         return attrs
 
     def list(self, filters: Dict = {}) -> List[StructuralAttribute]:
         structural_attributes = [
-            self.prepare_model(self._get(x)) for x
-            in self.client.api.corpus_structural_attributes(self.corpus.api_name)
+            self.get(x) for x in
+            self.client.api.corpus_structural_attributes(self.corpus.api_name)
         ]
         for k, v in filters.items():
             if k == 'has_values':
                 structural_attributes = [
                     x for x in structural_attributes
                     if x.has_values == v
                 ]
```

### Comparing `cqi-0.1.1/cqi/models/corpora.py` & `cqi-0.1.2/cqi/models/corpora.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from typing import Dict, List, TYPE_CHECKING
+from typing import Dict, List, Type, TYPE_CHECKING
 if TYPE_CHECKING:
     from ..status import StatusOk
 from .attributes import (
     AlignmentAttributeCollection,
     PositionalAttributeCollection,
     StructuralAttributeCollection
 )
 from .resource import Collection, Model
 from .subcorpora import SubcorpusCollection
 
 
 class Corpus(Model):
-    id_attribute: str = 'api_name'
-
     @property
     def api_name(self) -> str:
         return self.attrs.get('api_name')
 
     @property
     def name(self) -> str:
         return self.attrs.get('name')
@@ -46,36 +44,35 @@
         return StructuralAttributeCollection(client=self.client, corpus=self)
 
     @property
     def subcorpora(self) -> SubcorpusCollection:
         return SubcorpusCollection(client=self.client, corpus=self)
 
     def drop(self) -> 'StatusOk':
+        ''' try to unload a corpus and all its attributes from memory '''
         return self.client.api.corpus_drop_corpus(self.api_name)
 
     def query(self, subcorpus_name: str, query: str) -> 'StatusOk':
+        ''' <query> must include the ';' character terminating the query. '''
         return self.client.api.cqp_query(self.api_name, subcorpus_name, query)
 
 
 class CorpusCollection(Collection):
-    model: Corpus = Corpus
+    model: Type[Corpus] = Corpus
 
     def _get(self, corpus_name: str) -> Dict:
         api_name: str = corpus_name
         return {
-            'api_name': corpus_name,
+            'api_name': api_name,
             'charset': self.client.api.corpus_charset(api_name),
-            # 'full_name' = client.api.corpus_full_name(api_name),
-            # 'info': client.api.corpus_info(api_name),
+            # 'full_name': self.client.api.corpus_full_name(api_name),
+            # 'info': self.client.api.corpus_info(api_name),
             'name': corpus_name,
             'properties': self.client.api.corpus_properties(api_name),
             'size': self.client.api.cl_attribute_size(f'{api_name}.word')
         }
 
     def get(self, corpus_name: str) -> Corpus:
         return self.prepare_model(self._get(corpus_name))
 
     def list(self) -> List[Corpus]:
-        return [
-            self.prepare_model(self._get(x)) for x
-            in self.client.api.corpus_list_coprora()
-        ]
+        return [self.get(x) for x in self.client.api.corpus_list_corpora()]
```

### Comparing `cqi-0.1.1/cqi/models/resource.py` & `cqi-0.1.2/cqi/models/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import Dict, List, TYPE_CHECKING
+from typing import Dict, List, Type, TYPE_CHECKING
 if TYPE_CHECKING:
     from ..client import CQiClient
 
 
 class Model:
     '''
     A base class for representing a single object on the server.
     '''
-    id_attribute: str = 'Id'
 
     def __init__(
         self,
         attrs: Dict = None,
         client: 'CQiClient' = None,
         collection: 'Collection' = None
     ):
@@ -30,46 +29,43 @@
     def __eq__(self, other) -> bool:
         return isinstance(other, self.__class__) and self.id == other.id
 
     def __hash__(self) -> int:
         return hash(f'{self.__class__.__name__}:{self.id}')
 
     @property
-    def id(self) -> str:
-        '''
-        The ID of the object.
-        '''
-        return self.attrs.get(self.id_attribute)
+    def api_name(self) -> str:
+        raise NotImplementedError
 
     def reload(self):
         '''
         Load this object from the server again and update ``attrs`` with the
         new data.
         '''
-        self.attrs = self.collection.get(self.id).attrs
+        self.attrs = self.collection.get(self.api_name).attrs
 
 
 class Collection:
     '''
     A base class for representing all objects of a particular type on the
     server.
     '''
 
     #: The type of object this collection represents, set by subclasses
-    model: None = None
+    model: Type[Model] = Model
 
     def __init__(self, client: 'CQiClient' = None):
         #: The client pointing at the server that this collection of objects
         #: is on.
         self.client: 'CQiClient' = client
 
     def list(self) -> List[Model]:
         raise NotImplementedError
 
-    def get(self, key) -> Model:
+    def get(self) -> Model:
         raise NotImplementedError
 
     def prepare_model(self, attrs) -> Model:
         '''
         Create a model from a set of attributes.
         '''
         if isinstance(attrs, Model):
```

### Comparing `cqi-0.1.1/cqi/models/subcorpora.py` & `cqi-0.1.2/cqi/models/subcorpora.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, TYPE_CHECKING
+from typing import Dict, List, Type, TYPE_CHECKING
 if TYPE_CHECKING:
     from ..client import CQiClient
     from ..status import StatusOk
     from .attributes import PositionalAttribute
     from .corpora import Corpus
 from ..api.specification import (
     CONST_FIELD_KEYWORD,
@@ -10,16 +10,14 @@
     CONST_FIELD_MATCHEND,
     CONST_FIELD_TARGET
 )
 from .resource import Collection, Model
 
 
 class Subcorpus(Model):
-    id_attribute: str = 'api_name'
-
     @property
     def api_name(self) -> str:
         return self.attrs.get('api_name')
 
     @property
     def fields(self) -> Dict[str, int]:
         return self.attrs.get('fields')
@@ -29,30 +27,47 @@
         return self.attrs.get('name')
 
     @property
     def size(self) -> int:
         return self.attrs.get('size')
 
     def drop(self) -> 'StatusOk':
+        ''' delete a subcorpus from memory '''
         return self.client.api.cqp_drop_subcorpus(self.api_name)
 
     def dump(self, field: int, first: int, last: int) -> List[int]:
+        '''
+        Dump the values of <field> for match ranges <first> .. <last> in
+        subcorpus. <field> is one of the CQI_CONST_FIELD_* constants.
+        '''
         return self.client.api.cqp_dump_subcorpus(
             self.api_name,
             field,
             first,
             last
         )
 
     def fdist_1(
         self,
         cutoff: int,
         field: int,
         attribute: 'PositionalAttribute'
     ) -> List[int]:
+        '''
+        frequency distribution of single tokens
+
+        returns <n> (id, frequency) pairs flattened into a list of size 2*<n>
+
+        field is one of
+        - CQI_CONST_FIELD_MATCH
+        - CQI_CONST_FIELD_TARGET
+        - CQI_CONST_FIELD_KEYWORD
+
+        NB: pairs are sorted by frequency desc.
+        '''
         return self.client.api.cqp_fdist_1(
             self.api_name,
             cutoff,
             field,
             attribute.api_name
         )
 
@@ -60,26 +75,34 @@
         self,
         cutoff: int,
         field_1: int,
         attribute_1: 'PositionalAttribute',
         field_2: int,
         attribute_2: 'PositionalAttribute'
     ) -> List[int]:
+        '''
+        frequency distribution of pairs of tokens
+
+        returns <n> (id1, id2, frequency) pairs flattened into a list of size
+        3*<n>
+
+        NB: triples are sorted by frequency desc.
+        '''
         return self.client.api.cqp_fdist_2(
             self.api_name,
             cutoff,
             field_1,
             attribute_1.api_name,
             field_2,
             attribute_2.api_name
         )
 
 
 class SubcorpusCollection(Collection):
-    model: Subcorpus = Subcorpus
+    model: Type[Subcorpus] = Subcorpus
 
     def __init__(self, client: 'CQiClient' = None, corpus: 'Corpus' = None):
         super().__init__(client=client)
         self.corpus: 'Corpus' = corpus
 
     def _get(self, subcorpus_name: str) -> Dict:
         api_name: str = f'{self.corpus.api_name}:{subcorpus_name}'
@@ -100,10 +123,10 @@
         }
 
     def get(self, subcorpus_name: str) -> Subcorpus:
         return self.prepare_model(self._get(subcorpus_name))
 
     def list(self) -> List[Subcorpus]:
         return [
-            self.prepare_model(self._get(x)) for x
-            in self.client.api.cqp_list_subcorpora(self.corpus.api_name)
+            self.get(x) for x in
+            self.client.api.cqp_list_subcorpora(self.corpus.api_name)
         ]
```

### Comparing `cqi-0.1.1/cqi/status.py` & `cqi-0.1.2/cqi/status.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.1/cqi.egg-info/PKG-INFO` & `cqi-0.1.2/cqi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqi
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
 Home-page: https://github.com/Pevtrick/cqi-py
 Author: Patrick Jentsch
 Author-email: patrickjentsch@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,14 +26,15 @@
 
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
 | 0.1.0           | 0.1              |
 | 0.1.1           | 0.1              |
+| 0.1.2           | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.1/setup.py` & `cqi-0.1.2/setup.py`

 * *Files identical despite different names*

