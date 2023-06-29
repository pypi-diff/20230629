# Comparing `tmp/id_translation-0.4.0.tar.gz` & `tmp/id_translation-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_translation-0.4.0.tar", max compression
+gzip compressed data, was "id_translation-0.5.0.tar", max compression
```

## Comparing `id_translation-0.4.0.tar` & `id_translation-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1077 2023-06-16 17:21:04.753364 id_translation-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     5488 2023-06-16 17:21:04.753364 id_translation-0.4.0/README.md
--rw-r--r--   0        0        0     5642 2023-06-16 17:21:04.761364 id_translation-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      784 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/__init__.py
--rw-r--r--   0        0        0      203 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/__version__.py
--rw-r--r--   0        0        0     4571 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/_base_metadata.py
--rw-r--r--   0        0        0     4208 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/_config_utils.py
--rw-r--r--   0        0        0     1467 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/_load_toml.py
--rw-r--r--   0        0        0    47757 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/_translator.py
--rw-r--r--   0        0        0      947 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/_uuid_utils.py
--rw-r--r--   0        0        0      235 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/__init__.py
--rw-r--r--   0        0        0     1568 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_data_structure_io.py
--rw-r--r--   0        0        0     1085 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_dict.py
--rw-r--r--   0        0        0     2481 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_pandas.py
--rw-r--r--   0        0        0      740 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_resolve.py
--rw-r--r--   0        0        0     2697 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_sequence.py
--rw-r--r--   0        0        0     1022 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/_single_value.py
--rw-r--r--   0        0        0      760 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/dio/exceptions.py
--rw-r--r--   0        0        0      453 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/exceptions.py
--rw-r--r--   0        0        0    11744 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/factory.py
--rw-r--r--   0        0        0     1264 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/__init__.py
--rw-r--r--   0        0        0    22689 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_abstract_fetcher.py
--rw-r--r--   0        0        0     7573 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_cache.py
--rw-r--r--   0        0        0     2868 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_fetcher.py
--rw-r--r--   0        0        0     1441 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_memory_fetcher.py
--rw-r--r--   0        0        0    12950 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_multi_fetcher.py
--rw-r--r--   0        0        0     5431 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_pandas_fetcher.py
--rw-r--r--   0        0        0    17318 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/_sql_fetcher.py
--rw-r--r--   0        0        0     2165 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/exceptions.py
--rw-r--r--   0        0        0      686 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/support.py
--rw-r--r--   0        0        0     1154 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/fetching/types.py
--rw-r--r--   0        0        0      601 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/__init__.py
--rw-r--r--   0        0        0     5710 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/_cardinality.py
--rw-r--r--   0        0        0     8043 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/_directional_mapping.py
--rw-r--r--   0        0        0     8004 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/_heuristic_score.py
--rw-r--r--   0        0        0    22026 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/_mapper.py
--rw-r--r--   0        0        0     2371 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/exceptions.py
--rw-r--r--   0        0        0     6171 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/filter_functions.py
--rw-r--r--   0        0        0     6010 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/heuristic_functions.py
--rw-r--r--   0        0        0     3051 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/score_functions.py
--rw-r--r--   0        0        0    13566 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/support.py
--rw-r--r--   0        0        0     2854 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/mapping/types.py
--rw-r--r--   0        0        0      287 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/__init__.py
--rw-r--r--   0        0        0     4822 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/_format.py
--rw-r--r--   0        0        0     3723 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/_format_applier.py
--rw-r--r--   0        0        0     2628 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/_magic_dict.py
--rw-r--r--   0        0        0     7632 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/_translation_map.py
--rw-r--r--   0        0        0     5658 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/parse_format_string.py
--rw-r--r--   0        0        0     3276 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/offline/types.py
--rw-r--r--   0        0        0        0 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/py.typed
--rw-r--r--   0        0        0     3362 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/testing.py
--rw-r--r--   0        0        0     2577 2023-06-16 17:21:04.761364 id_translation-0.4.0/src/id_translation/types.py
--rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 id_translation-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-29 19:58:15.847356 id_translation-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     5488 2023-06-29 19:58:15.847356 id_translation-0.5.0/README.md
+-rw-r--r--   0        0        0     5642 2023-06-29 19:58:15.855356 id_translation-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      962 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/__init__.py
+-rw-r--r--   0        0        0      203 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/__version__.py
+-rw-r--r--   0        0        0     4652 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/_base_metadata.py
+-rw-r--r--   0        0        0     4208 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/_config_utils.py
+-rw-r--r--   0        0        0     1467 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/_load_toml.py
+-rw-r--r--   0        0        0    50044 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/_translator.py
+-rw-r--r--   0        0        0      947 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/_uuid_utils.py
+-rw-r--r--   0        0        0      235 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/__init__.py
+-rw-r--r--   0        0        0     2036 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_data_structure_io.py
+-rw-r--r--   0        0        0     1346 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_dict.py
+-rw-r--r--   0        0        0     4141 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_pandas.py
+-rw-r--r--   0        0        0      771 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_resolve.py
+-rw-r--r--   0        0        0     2572 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_sequence.py
+-rw-r--r--   0        0        0     1094 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_set.py
+-rw-r--r--   0        0        0     1022 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_single_value.py
+-rw-r--r--   0        0        0      760 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/exceptions.py
+-rw-r--r--   0        0        0      898 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/exceptions.py
+-rw-r--r--   0        0        0    11744 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/factory.py
+-rw-r--r--   0        0        0     1264 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/__init__.py
+-rw-r--r--   0        0        0    23102 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_abstract_fetcher.py
+-rw-r--r--   0        0        0     7573 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_cache.py
+-rw-r--r--   0        0        0     3249 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_fetcher.py
+-rw-r--r--   0        0        0     1441 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_memory_fetcher.py
+-rw-r--r--   0        0        0    13706 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_multi_fetcher.py
+-rw-r--r--   0        0        0     5431 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_pandas_fetcher.py
+-rw-r--r--   0        0        0    17244 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_sql_fetcher.py
+-rw-r--r--   0        0        0     2165 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/exceptions.py
+-rw-r--r--   0        0        0     1154 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/types.py
+-rw-r--r--   0        0        0      601 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/mapping/__init__.py
+-rw-r--r--   0        0        0     5710 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/mapping/_cardinality.py
+-rw-r--r--   0        0        0     8043 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/mapping/_directional_mapping.py
+-rw-r--r--   0        0        0     8004 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/mapping/_heuristic_score.py
+-rw-r--r--   0        0        0    21999 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/_mapper.py
+-rw-r--r--   0        0        0     2371 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/exceptions.py
+-rw-r--r--   0        0        0     6171 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/filter_functions.py
+-rw-r--r--   0        0        0     6250 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/heuristic_functions.py
+-rw-r--r--   0        0        0     3051 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/score_functions.py
+-rw-r--r--   0        0        0    13582 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/support.py
+-rw-r--r--   0        0        0     2854 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/types.py
+-rw-r--r--   0        0        0      287 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/__init__.py
+-rw-r--r--   0        0        0     5323 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/_format.py
+-rw-r--r--   0        0        0     3723 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/_format_applier.py
+-rw-r--r--   0        0        0     2628 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/_magic_dict.py
+-rw-r--r--   0        0        0     7603 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/_translation_map.py
+-rw-r--r--   0        0        0     6114 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/parse_format_string.py
+-rw-r--r--   0        0        0     3276 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/types.py
+-rw-r--r--   0        0        0        0 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/py.typed
+-rw-r--r--   0        0        0     3362 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/testing.py
+-rw-r--r--   0        0        0     2741 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/types.py
+-rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 id_translation-0.5.0/PKG-INFO
```

### Comparing `id_translation-0.4.0/LICENSE.md` & `id_translation-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/README.md` & `id_translation-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/pyproject.toml` & `id_translation-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "id-translation"
-version = "0.4.0"
+version = "0.5.0"
 description = "Convert IDs into human-readable labels."
 authors = ["Richard Sundqvist <richard.sundqvist@live.se>"]
 
 readme = "README.md"
 homepage = "https://github.com/rsundqvist/id-translation"
 repository = "https://github.com/rsundqvist/id-translation"
 documentation = "https://id-translation.readthedocs.io"
```

### Comparing `id_translation-0.4.0/src/id_translation/__init__.py` & `id_translation-0.5.0/src/id_translation/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 """Translation of IDs with flexible formatting and name matching.
 
 For an introduction to translation, see :ref:`translation-primer` and :ref:`mapping-primer`.
+
+
+Environment variables
+---------------------
+.. envvar:: ID_TRANSLATION_DISABLED
+
+    Global switch. When ``true``, the :meth:`Translator.translate`-method returns immediately.
 """
 
 import logging
 
 from ._base_metadata import BaseMetadata
 from ._config_utils import ConfigMetadata
 from ._load_toml import load_toml_file
```

### Comparing `id_translation-0.4.0/src/id_translation/_base_metadata.py` & `id_translation-0.5.0/src/id_translation/_base_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,15 +119,18 @@
 
         reason_not_equivalent = self.is_equivalent(stored_config)
         if reason_not_equivalent:
             log_reject(f"cached instance is not equivalent. {reason_not_equivalent}")
             return False
 
         expires_at = stored_config.created + max_age
-        offset = timedelta(abs(datetime.now() - expires_at).total_seconds() // 60)
+        offset = timedelta(seconds=round(abs(datetime.now() - expires_at).total_seconds()))
 
+        fmt = "%Y-%m-%dT%H:%M:%S"
         if expires_at <= stored_config.created:
-            log_reject(f"cache expired at {expires_at} ({offset} ago)")
+            log_reject(f"cache expired at {expires_at:{fmt}} ({offset} ago)")
             return False
 
-        self._log_accept(f"Accept cached {{kind}} in '{metadata_path.parent}'. Expires at {expires_at} (in {offset}).")
+        self._log_accept(
+            f"Accept cached {{kind}} in '{metadata_path.parent}'. " f"Expires at {expires_at:{fmt}} (in {offset})."
+        )
         return True
```

### Comparing `id_translation-0.4.0/src/id_translation/_config_utils.py` & `id_translation-0.5.0/src/id_translation/_config_utils.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/_load_toml.py` & `id_translation-0.5.0/src/id_translation/_load_toml.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/_translator.py` & `id_translation-0.5.0/src/id_translation/_translator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 import logging
 import warnings
-from collections import defaultdict
 from datetime import timedelta
 from inspect import signature
+from os import getenv
 from pathlib import Path
 from time import perf_counter
-from typing import Any, Dict, Generic, Iterable, List, Optional, Set, Tuple, Type, Union
+from typing import Any, Dict, Generic, Iterable, List, Literal, Optional, Set, Tuple, Type, Union
 
 import numpy
 import pandas as pd
 from rics._internal_support.types import PathLikeType
 from rics.collections.dicts import InheritedKeysDict, MakeType
 from rics.collections.misc import as_list
 from rics.misc import tname
 from rics.performance import format_perf_counter, format_seconds
 
 from . import _uuid_utils
 from ._config_utils import ConfigMetadata
 from .dio import DataStructureIO, resolve_io
-from .exceptions import ConnectionStatusError, TooManyFailedTranslationsError
+from .dio.exceptions import UntranslatableTypeError
+from .exceptions import (
+    ConnectionStatusError,
+    MissingNamesError,
+    TooManyFailedTranslationsError,
+    TranslationDisabledWarning,
+)
 from .factory import TranslatorFactory
 from .fetching import Fetcher
 from .fetching.types import IdsToFetch
 from .mapping import DirectionalMapping, Mapper
 from .mapping.exceptions import MappingError, MappingWarning
 from .mapping.types import UserOverrideFunction
 from .offline import Format, TranslationMap
 from .offline.types import FormatType, PlaceholderTranslations, SourcePlaceholderTranslations
-from .types import ID, HasSources, IdType, Names, NamesPredicate, NameType, NameTypes, SourceType, Translatable
-
-_NAME_ATTRIBUTES = ("name", "columns", "keys")
+from .types import ID, HasSources, IdType, Names, NameToSource, NameType, NameTypes, SourceType, Translatable
 
 LOGGER = logging.getLogger(__package__).getChild("Translator")
 
 FetcherTypes = Union[
     TranslationMap[NameType, SourceType, IdType],
     Fetcher[SourceType, IdType],
     SourcePlaceholderTranslations[SourceType],
     Dict[SourceType, PlaceholderTranslations.MakeTypes],
 ]
 
+ID_TRANSLATION_DISABLED: Literal["ID_TRANSLATION_DISABLED"] = "ID_TRANSLATION_DISABLED"
+
 
 class Translator(Generic[NameType, SourceType, IdType], HasSources[SourceType]):
     """Translate IDs to human-readable labels.
 
     For an introduction to translation, see the :ref:`translation-primer` page.
 
     The recommended way of initializing ``Translator`` instances is the :meth:`from_config` method. For configuration
@@ -80,22 +86,32 @@
                  id | name    | gender       id | name   | is_nice
               ------+---------+--------     ----+--------+---------
                1991 | Richard | Male          0 | Tarzan | false
                1999 | Sofia   | Female        1 | Morris | true
                1904 | Fred    | Male          2 | Simba  | true
 
         In most real cases we'd fetch this table from somewhere. In this case, however, there's so little data that we
-        can simply enumerate the components needed for translation ourselves to create a :class:`.MemoryFetcher`.
+        can simply enumerate the components needed for translation ourselves.
 
         >>> from id_translation import Translator
         >>> translation_data = {
-        ...     'animals': {'id': [0, 1, 2], 'name': ['Tarzan', 'Morris', 'Simba'], 'is_nice': [False, True, True]},
-        ...     'people': {'id': [1999, 1991, 1904], 'name': ['Sofia', 'Richard', 'Fred']},
+        ...   'animals': {
+        ...     'id': [0, 1, 2],
+        ...     'name': ['Tarzan', 'Morris', 'Simba'],
+        ...     'is_nice': [False, True, True]
+        ...   },
+        ...   'people': {
+        ...     'id': [1999, 1991, 1904],
+        ...     'name': ['Sofia', 'Richard', 'Fred']
+        ...   },
         ... }
         >>> translator = Translator(translation_data, fmt='{id}:{name}[, nice={is_nice}]')
+
+        We didn't define a :class:`.Mapper`, so the names must match exactly.
+
         >>> data = {'animals': [0, 2], 'people': [1991, 1999]}
         >>> for key, translated_table in translator.translate(data).items():
         >>>     print(f'Translations for {repr(key)}:')
         >>>     for translated_id in translated_table:
         >>>         print(f'    {repr(translated_id)}')
         Translations for 'animals':
             '0:Tarzan, nice=False'
@@ -103,23 +119,25 @@
         Translations for 'people':
             '1991:Richard'
             '1999:Sofia'
 
         Handling unknown IDs.
 
         >>> default_fmt_placeholders = dict(
-        ...     default={'is_nice': 'Maybe?', 'name': "Bob"},
-        ...     specific={'animals': {'name': 'Fido'}},
+        ...   default={'is_nice': 'Maybe?', 'name': "Bob"},
+        ...   specific={'animals': {'name': 'Fido'}},
         >>> )
         >>> useless_database = {
-        ...     'animals': {'id': [], 'name': []},
-        ...     'people': {'id': [], 'name': []}
+        ...   'animals': {'id': [], 'name': []},
+        ...   'people': {'id': [], 'name': []}
         >>> }
-        >>> translator = Translator(useless_database, default_fmt_placeholders=default_fmt_placeholders,
-        ...                         fmt='{id}:{name}[, nice={is_nice}]')
+        >>> translator = Translator(
+        ...   useless_database, default_fmt_placeholders=default_fmt_placeholders,
+        ...   fmt='{id}:{name}[, nice={is_nice}]'
+        ... )
         >>> data = {'animals': [0], 'people': [0]}
         >>> for key, translated_table in translator.translate(data).items():
         >>>     print(f'Translations for {repr(key)}:')
         >>>     for translated_id in translated_table:
         >>>         print(f'    {repr(translated_id)}')
         Translations for 'animals':
             '0:Fido, nice=Maybe?'
@@ -151,15 +169,15 @@
         self._enable_uuid_heuristics = enable_uuid_heuristics
 
         self._cached_tmap: TranslationMap[NameType, SourceType, IdType] = TranslationMap({})
         self._fetcher: Fetcher[SourceType, IdType]
         if fetcher is None:
             from .testing import TestFetcher, TestMapper
 
-            self._fetcher = TestFetcher([])  # No explicit sources
+            self._fetcher = TestFetcher([])  # No explidecit sources
             if mapper:  # pragma: no cover
                 warnings.warn(
                     f"Mapper instance {mapper} given; consider creating a TestFetcher([sources..])-instance manually.",
                     UserWarning,
                     stacklevel=2,
                 )
             else:
@@ -184,14 +202,15 @@
         else:
             raise TypeError(type(fetcher))  # pragma: no cover
 
         self._mapper: Mapper[NameType, SourceType, None] = mapper or Mapper()
         self._mapper.logger = logging.getLogger(__package__).getChild("mapping").getChild("name-to-source")
 
         self._config_metadata: Optional[ConfigMetadata] = None
+        self._translated_names: Optional[List[NameType]] = None
 
     @classmethod
     def from_config(
         cls,
         path: PathLikeType,
         extra_fetchers: Iterable[PathLikeType] = (),
         clazz: Union[str, Type["Translator[NameType, SourceType, IdType]"]] = None,
@@ -254,15 +273,15 @@
             kwargs["fetcher"] = self.fetcher if self.online else self._cached_tmap.copy()
 
         return type(self)(**kwargs)
 
     def translate(
         self,
         translatable: Translatable,
-        names: NameTypes[NameType] = None,
+        names: Union[NameTypes[NameType], NameToSource[NameType, SourceType]] = None,
         ignore_names: Names[NameType] = None,
         inplace: bool = False,
         override_function: UserOverrideFunction[NameType, SourceType, None] = None,
         maximal_untranslated_fraction: float = 1.0,
         reverse: bool = False,
         attribute: str = None,
         fmt: FormatType = None,
@@ -273,15 +292,16 @@
 
         See Also:
             🔑 This is a key event method. Exit-events are emitted on the ``ℹ️INFO``-level if the ``Translator`` is
             :attr:`online`. Enter-events are always emitted on the ``🪲DEBUG``-level. See :ref:`key-events` for details.
 
         Args:
             translatable: A data structure to translate.
-            names: Explicit names to translate. Derive from `translatable` if ``None``.
+            names: Explicit names to translate. Derive from `translatable` if ``None``. Alternatively, you may pass a
+                ``dict`` on the form ``{name_in_translatable: source_to_use}``.
             ignore_names: Names **not** to translate, or a predicate ``(str) -> bool``.
             inplace: If ``True``, translate in-place and return ``None``.
             override_function: A callable ``(name, fetcher.sources, ids) -> Source | None``. See :meth:`.Mapper.apply`
                 for details.
             maximal_untranslated_fraction: The maximum fraction of IDs for which translation may fail before an error is
                 raised. 1=disabled. Ignored in `reverse` mode.
             reverse: If ``True``, perform translations back to IDs. Offline mode only.
@@ -289,52 +309,73 @@
                 attribute will be assigned to `translatable` using
                 ``setattr(translatable, attribute, <translated-attribute>)``.
             fmt: Format to use. If ``None``, fall back to init format.
 
         Returns:
             A translated copy of `translatable` if ``inplace=False``, otherwise ``None``.
 
+        Examples:
+            Manual `name-to-source <../documentation/translation-primer.html#name-to-source-mapping>`__ mapping with a
+            temporary name-only :class:`.Format`.
+
+            ..
+               # Hidden setup code
+               >>> translator = Translator({'animals': {'id': [2], 'name': ['Simba']}})
+
+            >>> n2s = {'lions': 'animals', 'big_cats': 'animals'}
+            >>> translator.translate({'lions': 2, 'big_cats': 2}, names=n2s, fmt="{name}")
+            {'lions': 'Simba', 'big_cats': 'Simba'}
+
+            Name mappings must be complete; any name not present in the keys will be ignored (left as-is).
+
         Raises:
             UntranslatableTypeError: If ``type(translatable)`` cannot be translated.
-            AttributeError: If `names` are not given and cannot be derived from `translatable`.
+            MissingNamesError: If `names` are not given and cannot be derived from `translatable`.
             MappingError: If any required (explicitly given) names fail to map to a source.
             MappingError: If name-to-source mapping is ambiguous.
             ValueError: If `maximal_untranslated_fraction` is not a valid fraction.
             TooManyFailedTranslationsError: If translation fails for more than `maximal_untranslated_fraction` of IDs.
             ConnectionStatusError: If ``reverse=True`` while the ``Translator`` is online.
             UserMappingError: If `override_function` returns a source which is not known, and
                 ``self.mapper.unknown_user_override_action != 'ignore'``.
         """  # noqa: DAR101 darglint is bugged here
+        if getenv(ID_TRANSLATION_DISABLED, "").lower() == "true":
+            message = "Translation aborted; ID_TRANSLATION_DISABLED is set."
+            LOGGER.warning(message)
+            warnings.warn(message, category=TranslationDisabledWarning, stacklevel=2)
+            return None if inplace else translatable
+
         if fmt is not None:
             real_fmt = self._fmt
             try:
                 parameters = set(signature(Translator.translate).parameters)
                 parameters.remove("self")
                 parameters.remove("fmt")
                 kwargs = {key: value for key, value in locals().items() if key in parameters}
                 self._fmt = Format.parse(fmt)
                 return self.translate(**kwargs)
             finally:
                 self._fmt = real_fmt
 
         start = perf_counter()
 
-        should_emit_key_event = LOGGER.isEnabledFor(logging.INFO) if self.online else LOGGER.isEnabledFor(logging.DEBUG)
+        key_event_level = logging.INFO if self.online else logging.DEBUG
+        should_emit_key_event = LOGGER.isEnabledFor(key_event_level)
         if should_emit_key_event:
             event_key = f"{self.__class__.__name__.upper()}.TRANSLATE"
 
             type_name = _resolve_type_name(translatable, attribute)
-            name_info = "Derive based on type" if names is None else repr(names)
+            name_info = f"Derive based on type={type_name}" if names is None else repr(names)
             if ignore_names is not None:
                 name_info += f", excluding those given by {ignore_names=}"
 
             sources = self.sources  # Ensures that the fetcher is warmed up; good for log organization.
             LOGGER.log(
                 level=logging.DEBUG,
-                msg=f"Begin translation of {type_name!r}-type data. Names to translate: {name_info}.",
+                msg=f"Begin translation of {type_name}-type data. Names to translate: {name_info}.",
                 extra=dict(
                     event_key=event_key,
                     event_stage="ENTER",
                     event_title=f"{event_key}.ENTER",
                     translatable_type=type_name,
                     names=names,
                     ignore_names=tname(ignore_names, prefix_classname=True) if callable(ignore_names) else ignore_names,
@@ -355,27 +396,27 @@
             raise ValueError(f"Argument {maximal_untranslated_fraction=} is not a valid fraction")
 
         if attribute:
             obj, translatable = translatable, getattr(translatable, attribute)
         else:
             obj = None
 
-        names = None if names is None else as_list(names)
+        names, override_function = _handle_input_names(names, override_function)
         translation_map, names_to_translate = self._get_updated_tmap(
             translatable,
             names,
             ignore_names=ignore_names,
             override_function=override_function,
             parent=obj if (obj is not None and self._allow_name_inheritance) else None,
         )
         if not translation_map:
             return None if inplace else translatable  # pragma: no cover
 
         translatable_io = resolve_io(translatable)
-        if LOGGER.isEnabledFor(logging.DEBUG) or maximal_untranslated_fraction < 1:
+        if LOGGER.isEnabledFor(logging.DEBUG) or maximal_untranslated_fraction < 1.0:
             self._verify_translations(
                 translatable,
                 names_to_translate if names is None else names,
                 translation_map,
                 translatable_io,
                 maximal_untranslated_fraction,
             )
@@ -398,19 +439,19 @@
                 ans.name = translatable.name
             ans = obj
 
         if should_emit_key_event:
             execution_time = perf_counter() - start
             inplace_info = "Original values have been replaced" if inplace else "Returning a translated copy"
 
-            pretty_n2s = _make_pretty_names_to_source(names_to_translate, translation_map.name_to_source)
+            n2s_with_none = {name: translation_map.name_to_source.get(name) for name in names_to_translate}
             LOGGER.log(
-                level=logging.INFO if self.online else logging.DEBUG,
-                msg=f"Finished translation of {type_name!r}-type data in {format_seconds(execution_time)}"
-                f" using names-to-source mapping: {pretty_n2s}. {inplace_info} (since {inplace=}).",
+                level=key_event_level,
+                msg=f"Finished translation of {type_name}-type data in {format_seconds(execution_time)}"
+                f" using name-to-source mapping: {n2s_with_none}. {inplace_info} (since {inplace=}).",
                 extra=dict(
                     event_key=event_key,
                     event_stage="EXIT",
                     event_title=f"{event_key}.EXIT",
                     execution_time=execution_time,
                     translatable_type=type_name,
                     names=names_to_translate,
@@ -420,16 +461,31 @@
                     maximal_untranslated_fraction=maximal_untranslated_fraction,
                     attribute=attribute,
                     reverse=reverse,
                     online=self.online,
                 ),
             )
 
+        self._translated_names = names_to_translate
+
         return ans
 
+    def translated_names(self) -> List[NameType]:
+        """Return the names that were translated by the most recent :meth:`translate`-call.
+
+        Returns:
+            Recent names translated by this ``Translator``, in **arbitrary** order.
+
+        Raises:
+            ValueError: If no names have been translated using this ``Translator``.
+        """
+        if self._translated_names is None:
+            raise ValueError("No names have been translated using this Translator.")
+        return list(self._translated_names)
+
     def map(  # noqa: A003
         self,
         translatable: Translatable,
         names: NameTypes[NameType] = None,
         ignore_names: Names[NameType] = None,
         override_function: UserOverrideFunction[NameType, SourceType, None] = None,
     ) -> Optional[DirectionalMapping[NameType, SourceType]]:
@@ -442,15 +498,15 @@
             override_function: A callable ``(name, fetcher.sources, ids) -> Source | None``. See
                 :meth:`Mapper.apply <.mapping.Mapper.apply>` for details.
 
         Returns:
             A mapping of names to translation sources. Returns ``None`` if mapping failed.
 
         Raises:
-            AttributeError: If `names` are not given and cannot be derived from `translatable`.
+            MissingNamesError: If `names` are not given and cannot be derived from `translatable`.
             MappingError: If any required (explicitly given) names fail to map to a source.
             MappingError: If name-to-source mapping is ambiguous.
             UserMappingError: If `override_function` returns a source which is not known, and
                 ``self.mapper.unknown_user_override_action != 'ignore'``.
 
         See Also:
             🔑 This is a key event method. See :ref:`key-events` for details.
@@ -491,14 +547,31 @@
         ignore_names: Names[NameType] = None,
         override_function: UserOverrideFunction[NameType, SourceType, None] = None,
         parent: Translatable = None,
     ) -> Optional[DirectionalMapping[NameType, SourceType]]:
         start = perf_counter()
         names_to_translate = self._resolve_names(translatable, names, ignore_names, parent)
 
+        def format_params() -> str:
+            params = []
+            if ignore_names is not None:
+                params.append(f"{ignore_names=}")
+            if override_function is not None:
+                params.append(f"{override_function=}")
+            if parent is not None:
+                params.append(f"parent={tname(parent)}")
+            return f". Parameters: ({', '.join(params)})" if params else ""
+
+        if names is not None and not names:
+            type_name = _resolve_type_name(translatable)
+            msg = f"Translation aborted; no names to translate in {type_name}{format_params()}."
+            warnings.warn(msg, MappingWarning, stacklevel=2)
+            LOGGER.warning(msg)
+            return None
+
         if LOGGER.isEnabledFor(logging.DEBUG):
             event_key = f"{self.__class__.__name__.upper()}.MAP"
             type_name = _resolve_type_name(translatable)
             sources = self.sources
             LOGGER.debug(
                 f"Begin name-to-source mapping of names={names_to_translate} in {type_name} against {sources=}.",
                 extra=dict(
@@ -526,32 +599,25 @@
                     mapping=name_to_source.left_to_right,
                     context=None,
                 ),
             )
 
         unmapped = set() if names is None else set(as_list(names)).difference(name_to_source.left)
         if unmapped or not name_to_source.left:
-            params_info = (
-                f"could not be mapped to sources={self.sources}. "
-                "Additional parameters: ("
-                f"{ignore_names=}, "
-                f"override_function={tname(override_function)}, "
-                f"parent={tname(parent)}"
-                ")"
-            )
+            tail = f"could not be mapped to sources={self.sources}{format_params()}"
 
             if names is None:
-                derived_names = self._extract_from_attribute_or_parent(translatable, parent)
-                msg = f"Translation aborted; none of the derived names {derived_names} {params_info}."
+                derived_names = self._resolve_names(translatable, None, None, parent)
+                msg = f"Translation aborted; none of the derived names {derived_names} {tail}."
                 warnings.warn(msg, MappingWarning, stacklevel=2)
                 LOGGER.warning(msg)
                 return None
             elif unmapped:
                 # Fail if any of the explicitly given names fail to map to a source.
-                msg = f"Required names {unmapped} {params_info}."
+                msg = f"Required names {unmapped} {tail}."
                 LOGGER.error(msg)
                 raise MappingError(msg)
 
         if name_to_source.cardinality.many_right:  # pragma: no cover
             for value, candidates in name_to_source.left_to_right.items():
                 if len(candidates) > 1:
                     raise MappingError(
@@ -790,27 +856,28 @@
             2. Resolve name-to-source mappings. If none are found, return ``None``.
             3. Create a new translation map, or update the cached one.
 
         See the :meth:`translate`-method for more detailed documentation.
         """
         translatable_io = resolve_io(translatable)  # Fail fast if untranslatable type
 
-        names = None if names is None else as_list(names)
+        names, override_function = _handle_input_names(names, override_function)
         name_to_source = self._map_inner(translatable, names, ignore_names, override_function, parent)
         if name_to_source is None:
             # Nothing to translate.
             return None, []  # pragma: no cover
 
         translation_map = (
             self.fetch(translatable, name_to_source, translatable_io, names)
             if force_fetch or not self.cache
             else self.cache
         )
 
         translation_map.enable_uuid_heuristics = self._enable_uuid_heuristics
+        translation_map.fmt = self._fmt
         n2s = name_to_source.flatten()
         translation_map.name_to_source = n2s  # Update
         return translation_map, list(n2s)
 
     def _get_ids_to_fetch(
         self,
         name_to_source: DirectionalMapping[NameType, SourceType],
@@ -930,81 +997,41 @@
         return f"{tname(self)}({online=}: {more})"
 
     def _resolve_names(
         self,
         translatable: Translatable,
         names: NameTypes[NameType] = None,
         ignored_names: Names[NameType] = None,
-        parent: Translatable = None,  # This isn't correct; should be different typevars.
+        parent: Any = None,
     ) -> List[NameType]:
         if names is None:
-            names = self._extract_from_attribute_or_parent(translatable, parent)
-        else:
-            names = as_list(names)
-        ignored_names = ignored_names if callable(ignored_names) else set(as_list(ignored_names))
-        return self._resolve_names_inner(names, ignored_names)
+            names = resolve_io(translatable).names(translatable)
+            if names is None and parent is not None and self._allow_name_inheritance:
+                try:
+                    names = resolve_io(parent).names(parent)
+                except UntranslatableTypeError:
+                    LOGGER.debug(f"Cannot use {tname(parent)!r}-type parent to derive names; not a translatable type.")
 
-    def _extract_from_attribute_or_parent(
-        self, translatable: Translatable, parent: Optional[Translatable]
-    ) -> List[NameType]:
-        if parent is None:
-            names = self._extract_from_attribute(translatable)
-        else:
-            try:
-                names = self._extract_from_attribute(translatable)
-            except AttributeError:
-                names = self._extract_from_attribute(parent)
-                LOGGER.debug(
-                    f"Using {names=} from parent of type {tname(parent)} for child of type {tname(translatable)}"
+            if names is None:
+                raise MissingNamesError(
+                    f"Failed to derive names for {tname(translatable)!r}-type data."
+                    "\nHint: Use the 'names'-argument to specify names to translate."
                 )
-        return names
-
-    @classmethod
-    def _extract_from_attribute(cls, translatable: Translatable) -> List[NameType]:
-        no_use_keys = False
-        for attr_name in _NAME_ATTRIBUTES:
-            if attr_name == "keys" and no_use_keys:
-                continue  # Pandas Series have keys, but should not be used.
-
-            if hasattr(translatable, attr_name):
-                attr = getattr(translatable, attr_name)
-                if attr is None:
-                    no_use_keys = True
-                else:
-                    return as_list(attr() if callable(attr) else attr)
-
-        raise AttributeError(
-            "Must pass 'names' since no valid name could be found for data of type "
-            f"'{tname(translatable)}'."
-            f" Attributes checked: {_NAME_ATTRIBUTES}."
-        )
-
-    @classmethod
-    def _resolve_names_inner(
-        cls, names: List[NameType], ignored_names: Union[NamesPredicate[NameType], Set[NameType]]
-    ) -> List[NameType]:
-        predicate = _IgnoredNamesPredicate(ignored_names).apply
-        names_to_translate = list(filter(predicate, names))
-        if not names_to_translate and names:
-            warnings.warn(
-                f"No names left to translate. Ignored names: {ignored_names}, explicit names: {names}.", stacklevel=3
-            )
-        return names_to_translate
-
+            if LOGGER.isEnabledFor(logging.DEBUG):
+                LOGGER.debug(f"Name resolution complete. Found {names=} for {tname(translatable)!r}-type data.")
 
-class _IgnoredNamesPredicate(Generic[NameType]):
-    def __init__(self, ignored_names: Union[NamesPredicate[NameType], Set[NameType]]) -> None:
-        self._func: NamesPredicate[NameType]
-        if callable(ignored_names):
-            self._func = ignored_names
+            if ignored_names is not None:
+                predicate = ignored_names if callable(ignored_names) else set(as_list(ignored_names)).__contains__
+                names = [name for name in names if not predicate(name)]
         else:
-            self._func = ignored_names.__contains__
+            if ignored_names is not None:
+                raise ValueError(f"Required {names=} cannot be used with {ignored_names=}.")
+            names = as_list(names)
 
-    def apply(self, name: NameType) -> bool:
-        return not self._func(name)
+        return names
 
 
 def _handle_default(
     fmt: Format,
     default_fmt: Optional[FormatType],
     default_fmt_placeholders: Optional[MakeType[SourceType, str, Any]],
 ) -> Tuple[Optional[InheritedKeysDict[SourceType, str, Any]], Optional[Format]]:  # pragma: no cover
@@ -1035,21 +1062,45 @@
 
     return dt, dfmt
 
 
 def _resolve_type_name(translatable: Translatable, attribute: str = None) -> str:
     type_name = tname(translatable, prefix_classname=True)
     if attribute:
-        type_name = f"{type_name}.{attribute}"
+        real_type_name = tname(getattr(translatable, attribute), prefix_classname=True)
+        type_name = f"{real_type_name!r} (from {type_name}.{attribute})"
+    else:
+        type_name = repr(type_name)
     return type_name
 
 
-def _make_pretty_names_to_source(names: List[NameType], name_to_source: Dict[NameType, SourceType]) -> str:
-    source_to_names = defaultdict(list)
-    for name in names:
-        source = name_to_source.get(name)
-        source_to_names[source].append(name)
-
-    return " | ".join(
-        f"{tuple(set(names))} -> {'<Not translated>' if source is None else repr(source)}"
-        for source, names in source_to_names.items()
-    )
+def _handle_input_names(
+    names: Optional[Union[NameTypes[NameType], NameToSource[NameType, SourceType]]],
+    override_function: Optional[UserOverrideFunction[NameType, SourceType, None]],
+) -> Tuple[Optional[List[NameType]], Optional[UserOverrideFunction[NameType, SourceType, None]]]:
+    if names is None:
+        return None, override_function
+
+    if isinstance(names, dict):
+        if override_function is not None:
+            raise ValueError(f"Dict-type {names=} cannot be combined with {override_function=}.")
+
+        override_function = _UserDefinedNameToSourceMapping(dict(names))
+
+    return as_list(names), override_function
+
+
+class _UserDefinedNameToSourceMapping:
+    def __init__(self, name_to_source: NameToSource[NameType, SourceType]) -> None:
+        for name, source in name_to_source.items():
+            if source is None:
+                raise ValueError(
+                    f"Bad name-to-source mapping: {name!r} -> {source!r}."
+                    f"\nHint: Remove None-values from names={name_to_source}."
+                )
+        self._name_to_source = name_to_source
+
+    def __call__(self, name: NameType, sources: Set[SourceType], context: None) -> Optional[SourceType]:
+        return self._name_to_source.get(name)
+
+    def __repr__(self) -> str:
+        return f"UserArgument(names={self._name_to_source})"
```

### Comparing `id_translation-0.4.0/src/id_translation/_uuid_utils.py` & `id_translation-0.5.0/src/id_translation/_uuid_utils.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/dio/_dict.py` & `id_translation-0.5.0/src/id_translation/dio/_single_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from typing import Any, Dict, List, Optional, Sequence, TypeVar
+from typing import Any, Dict, List, Sequence
+from uuid import UUID
 
 from ..offline import TranslationMap
 from ..types import IdType, NameType, SourceType
-from ._data_structure_io import DataStructureIO
+from . import DataStructureIO
+from .exceptions import NotInplaceTranslatableError
 
-T = TypeVar("T", bound=Dict)  # type: ignore[type-arg]  # TODO: Higher-Kinded TypeVars
 
-
-class DictIO(DataStructureIO):
-    """Implementation for dicts."""
+class SingleValueIO(DataStructureIO):
+    """Implementation for non-iterables. And strings."""
 
     @staticmethod
     def handles_type(arg: Any) -> bool:
-        return isinstance(arg, dict)
+        return isinstance(arg, (int, str, UUID))
 
     @staticmethod
-    def extract(translatable: T, names: List[NameType]) -> Dict[NameType, Sequence[IdType]]:
-        return {name: translatable[name] for name in names}
+    def extract(translatable: IdType, names: List[NameType]) -> Dict[NameType, Sequence[IdType]]:
+        if len(names) != 1:  # pragma: no cover
+            raise ValueError("Length of names must be one.")
+
+        return {names[0]: (translatable,)}
 
     @staticmethod
     def insert(
-        translatable: T, names: List[NameType], tmap: TranslationMap[NameType, SourceType, IdType], copy: bool
-    ) -> Optional[T]:
-        translatable = dict(translatable) if copy else translatable  # type: ignore
-
-        for name in filter(translatable.__contains__, names):
-            translatable[name] = type(translatable[name])(map(tmap[name].get, translatable[name]))
+        translatable: IdType, names: List[NameType], tmap: TranslationMap[NameType, SourceType, IdType], copy: bool
+    ) -> str:
+        if not copy:  # pragma: no cover
+            raise NotInplaceTranslatableError(translatable)
 
-        return translatable if copy else None
+        return tmap[names[0]][translatable]
```

### Comparing `id_translation-0.4.0/src/id_translation/dio/_pandas.py` & `id_translation-0.5.0/src/id_translation/dio/_sequence.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,74 @@
-from collections import defaultdict
-from typing import Any, Dict, Iterable, List, Optional, Sequence, TypeVar
+from typing import Any, Callable, Dict, List, Optional, Sequence, TypeVar
 
-import pandas as pd
+import numpy as np
+from rics.collections.misc import as_list
 
 from ..offline import TranslationMap
 from ..types import IdType, NameType, SourceType
-from ._data_structure_io import DataStructureIO
-from ._sequence import SequenceIO, translate_sequence, verify_names
+from . import DataStructureIO
+from .exceptions import NotInplaceTranslatableError
 
-T = TypeVar("T", pd.DataFrame, pd.Series)
+T = TypeVar("T", list, np.ndarray, tuple)  # type: ignore[type-arg]  # TODO: Higher-Kinded TypeVars
 
 
-def _cast_series(series: pd.Series) -> pd.Series:
-    return series.dropna().astype(int) if series.dtype == float else series
-
-
-class PandasIO(DataStructureIO):
-    """Implementation for Pandas data types."""
+class SequenceIO(DataStructureIO):
+    """Implementation for numpy arrays, Python lists and tuples."""
 
     @staticmethod
     def handles_type(arg: Any) -> bool:
-        return isinstance(arg, (pd.DataFrame, pd.Series))
+        return isinstance(arg, (list, np.ndarray, tuple))
 
     @staticmethod
     def extract(translatable: T, names: List[NameType]) -> Dict[NameType, Sequence[IdType]]:
-        if isinstance(translatable, pd.DataFrame):
-            ans = defaultdict(list)
-            for i, name in enumerate(translatable.columns):
-                if name in names:
-                    ans[name].extend(_cast_series(translatable.iloc[:, i]))
-            return dict(ans)
-        else:
-            return SequenceIO.extract(_cast_series(translatable), names)
+        verify_names(len(translatable), names)
+        return (
+            {names[0]: as_list(translatable)}
+            if len(names) == 1
+            else {n: as_list(r) for n, r in zip(names, translatable)}
+        )
 
     @staticmethod
     def insert(
         translatable: T, names: List[NameType], tmap: TranslationMap[NameType, SourceType, IdType], copy: bool
     ) -> Optional[T]:
-        translatable = translatable.copy() if copy else translatable
+        verify_names(len(translatable), names)
+        t = translate_sequence(translatable, names, tmap)
 
-        if isinstance(translatable, pd.DataFrame):
-            for i, name in enumerate(translatable.columns):
-                if name in names:
-                    translatable.iloc[:, i] = _translate_series(translatable.iloc[:, i], [name], tmap)
-        else:
-            verify_names(len(translatable), names)
-            translatable[:] = _translate_series(translatable, names, tmap)
-
-        return translatable if copy else None
-
-
-def _translate_series(
-    series: pd.Series, names: List[NameType], tmap: TranslationMap[NameType, SourceType, IdType]
-) -> Iterable[Optional[str]]:
-    verify_names(len(series), names)
-
-    if len(names) == 1 and len(series) > 100:
-        # Optimization for large series. Suboptimal if "many" values are
-        # unique. Not worth the additional overhead for small series.
-        magic_dict = tmap[names[0]]
-        mapping = {idx: magic_dict.get(idx) for idx in series.unique()}
-        return series.map(mapping)  # type: ignore[no-any-return]
-    else:
-        return translate_sequence(series, names, tmap)
+        ctor: Callable[[List[Optional[str]]], T]
+        if copy:
+            if isinstance(translatable, np.ndarray):
+                ctor = np.array
+            else:
+                ctor = type(translatable)
+            return ctor(t)
+
+        try:
+            translatable[:] = t[:]  # type: ignore
+            return None
+        except TypeError as e:
+            raise NotInplaceTranslatableError(translatable) from e
+
+
+def translate_sequence(
+    s: T, names: List[NameType], tmap: TranslationMap[NameType, SourceType, IdType]
+) -> List[Optional[str]]:
+    """Return a translated copy of the sequence `s`."""
+    if len(names) == 1:
+        return list(map(tmap[names[0]].get, s))
+
+    return [
+        translate_sequence(element, [name], tmap)  # type: ignore
+        if SequenceIO.handles_type(element)
+        else tmap[name].get(element)
+        for name, element in zip(names, s)
+    ]
+
+
+def verify_names(data_len: int, names: List[NameType]) -> None:  # pragma: no cover
+    """Verify that the length of names is either 1 or equal to the length of the data."""
+    num_names = len(names)
+    if num_names != 1 and num_names != data_len:
+        raise ValueError(
+            f"Number of names {len(names)} must be 1 or equal to the length of the data ({data_len}) to "
+            f"translate, but got {names=}."
+        )
```

### Comparing `id_translation-0.4.0/src/id_translation/dio/_resolve.py` & `id_translation-0.5.0/src/id_translation/dio/_resolve.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Type
 
 from ..types import Translatable
 from . import DataStructureIO
 from ._dict import DictIO
 from ._pandas import PandasIO
 from ._sequence import SequenceIO
+from ._set import SetIO
 from ._single_value import SingleValueIO
 from .exceptions import UntranslatableTypeError
 
 
 def resolve_io(arg: Translatable) -> Type[DataStructureIO]:
     """Get an IO instance for `arg`.
 
@@ -17,12 +18,12 @@
 
     Returns:
         A data structure IO instance for `arg`.
 
     Raises:
         UntranslatableTypeError: If not IO could be found.
     """
-    for tio_class in DictIO, PandasIO, SequenceIO, SingleValueIO:
+    for tio_class in DictIO, SetIO, PandasIO, SequenceIO, SingleValueIO:
         if tio_class.handles_type(arg):
             return tio_class
 
     raise UntranslatableTypeError(type(arg))
```

### Comparing `id_translation-0.4.0/src/id_translation/dio/exceptions.py` & `id_translation-0.5.0/src/id_translation/dio/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/factory.py` & `id_translation-0.5.0/src/id_translation/factory.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/fetching/__init__.py` & `id_translation-0.5.0/src/id_translation/fetching/__init__.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/fetching/_abstract_fetcher.py` & `id_translation-0.5.0/src/id_translation/fetching/_abstract_fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,22 @@
         mapper: A :class:`.Mapper` instance used to adapt placeholder names in sources to wanted names, i.e.
             the names of the placeholders that are in the translation :class:`.Format` being used.
         allow_fetch_all: If ``False``, an error will be raised when :meth:`fetch_all` is called.
         fetch_all_unmapped_values_action: A temporary value to use for :attr:`Mapper.unmapped_values_action
             <.Mapper.unmapped_values_action>` while :meth:`fetch_all` is executing. Setting
             ``fetch_all_unmapped_values_action='raise'`` is mutually exclusive with ``selective_fetch_all=True``.
         selective_fetch_all: If ``True``, fetch only from those :attr:`~.HasSources.sources` that contain the required
-            :attr:`~.HasSources.placeholders` (after mapping).
+            :attr:`~.HasSources.placeholders` (after mapping). May also reduce the number of placeholders retrieved.
         fetch_all_cache_max_age: If given, determines validity lifetime of data cached when :func:`fetch_all`-calls are
             made. The regular ``fetch`` function will draw from this cache as well, but only ``fetch_all`` will update
             the cache. Furthermore, caching will never be used (read or write) if :attr:`online` is ``False``.
         cache_keys: A collection of hierarchical cache-key elements, see :class:`CacheMetadata`. If given, element zero
             of the `cache_keys` is added to the :attr:`logger` name for the fetcher.
+        optional: If ``True``, this fetcher may be discarded if source/placeholder-enumeration fails in multi-fetcher
+            mode.
 
     Raises:
         rics.action_level.BadActionLevelError: If `selective_fetch_all` is ``True`` and
             `fetch_all_unmapped_values_action` is ``'raise'``.
         ValueError:  If only one of `fetch_all_cache_max_age` and `cache_keys` are given.
     """
 
@@ -60,14 +62,15 @@
         self,
         mapper: Mapper[str, str, SourceType] = None,
         allow_fetch_all: bool = True,
         fetch_all_unmapped_values_action: ActionLevel.ParseType = None,
         selective_fetch_all: bool = True,
         fetch_all_cache_max_age: Union[str, pd.Timedelta, timedelta] = None,
         cache_keys: Sequence[str] = None,
+        optional: bool = False,
     ) -> None:
         self._mapper: Mapper[str, str, SourceType] = mapper or Mapper(**self.default_mapper_kwargs())
         if self._mapper.unmapped_values_action is ActionLevel.RAISE:
             warnings.warn(
                 "Using unmapped_values_action='raise' will treat optional placeholders as "
                 "required placeholders during normal operation.",
                 category=MappingWarning,
@@ -103,15 +106,15 @@
             cache_keys = list(cache_keys)
             adder = _ExtrasAdder(config_file=cache_keys[0])
             key0 = cache_keys[0].replace(".", "-")
             logger = logger.getChild(key0)
             mapper_logger = mapper_logger.getChild(key0)
             logger.addFilter(adder)
             mapper_logger.addFilter(adder)
-
+        self._optional: bool = optional
         self._cache_keys: Optional[List[str]] = cache_keys
         self.logger = logger
         self._mapper.logger = mapper_logger
 
     def map_placeholders(
         self,
         source: SourceType,
@@ -244,14 +247,18 @@
         """Return the ``Logger`` that is used by this instance."""
         return self._logger
 
     @logger.setter
     def logger(self, logger: logging.Logger) -> None:
         self._logger = logger
 
+    @property
+    def optional(self) -> bool:
+        return self._optional
+
     @contextmanager
     def _start_operation(self, operation):  # type: ignore  # noqa
         if self._active_operation:  # pragma: no cover
             raise exceptions.ConcurrentOperationError(operation, self._active_operation)
 
         self._active_operation = operation
         try:
@@ -369,14 +376,17 @@
     def _fetch_translations(
         self,
         source: SourceType,
         placeholders: PlaceholdersTuple,
         required_placeholders: Set[str],
         ids: Set[IdType] = None,
     ) -> Tuple[PlaceholderTranslations[SourceType], bool]:
+        start = perf_counter()
+
+        placeholders = tuple(dict.fromkeys(placeholders))  # Deduplicate
         reverse_mappings, instr = self._make_fetch_instruction(source, placeholders, required_placeholders, ids)
 
         cached_translations = self._get_cached_translations(instr.source)
         if cached_translations is not None:
             self.logger.debug(f"Returning cached translations for {source=}.")
             return cached_translations, True
 
@@ -391,15 +401,15 @@
                     source=source,
                     placeholders=instr.placeholders,
                     required_placeholders=list(instr.required),
                     num_ids=None if instr.ids is None else len(instr.ids),
                     fetch_all=instr.fetch_all,
                 ),
             )
-        start = perf_counter()
+
         translations = self.fetch_translations(instr)
         if self.logger.isEnabledFor(logging.DEBUG):
             execution_time = perf_counter() - start
             self.logger.debug(
                 f"Finished fetching placeholders={translations.placeholders} for {len(translations.records)} IDs "
                 f"from source '{translations.source}' in {format_seconds(execution_time)} using {self}.",
                 extra=dict(
```

### Comparing `id_translation-0.4.0/src/id_translation/fetching/_cache.py` & `id_translation-0.5.0/src/id_translation/fetching/_cache.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/fetching/_fetcher.py` & `id_translation-0.5.0/src/id_translation/fetching/_fetcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,26 @@
         """Close the ``Fetcher``. Does nothing by default."""
 
     @property
     @abstractmethod
     def online(self) -> bool:
         """Return connectivity status. If ``False``, no new translations may be fetched."""
 
+    @property
+    def optional(self) -> bool:
+        """Return ``True`` if this fetcher has been marked as `optional`.
+
+        In multi-fetcher mode, optional fetchers may be discarded if :attr:`~.HasSources.sources` cannot be resolved
+        (raises an exception). Default value is ``False``.
+
+        Returns:
+            Optionality status.
+        """
+        return False
+
     @abstractmethod
     def fetch(
         self,
         ids_to_fetch: Iterable[IdsToFetch[SourceType, IdType]],
         placeholders: Iterable[str] = (),
         required: Iterable[str] = (),
     ) -> SourcePlaceholderTranslations[SourceType]:
```

### Comparing `id_translation-0.4.0/src/id_translation/fetching/_memory_fetcher.py` & `id_translation-0.5.0/src/id_translation/fetching/_memory_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/fetching/_multi_fetcher.py` & `id_translation-0.5.0/src/id_translation/fetching/_multi_fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,30 +213,46 @@
     @property
     def _source_to_fetcher_id(self) -> Dict[SourceType, int]:
         if not self._source_to_fetcher_id_actual:
             source_ranks: Dict[SourceType, int] = {}
             source_to_fetcher_id: Dict[SourceType, int] = {}
 
             for fid, fetcher in list(self._id_to_fetcher.items()):
-                sources = fetcher.sources
+                if fetcher.optional:
+                    try:
+                        sources = fetcher.sources
+                    except Exception as e:  # noqa: B902
+                        sources = None
+                        exception_info = f"{type(e).__name__}: {e}"
+                else:
+                    sources = fetcher.sources
 
                 if not sources:
-                    LOGGER.warning(f"Discarding {self._fmt_fetcher(fetcher)}: No sources.")
+                    if sources is None:
+                        LOGGER.warning(
+                            f"Discarding optional {self._fmt_fetcher(fetcher)}: "
+                            f"Raised {exception_info!r} when getting sources."
+                        )
+                    else:
+                        LOGGER.warning(f"Discarding {self._fmt_fetcher(fetcher)}: No sources.")
                     fetcher.close()
                     del self._id_to_rank[fid]
                     del self._id_to_fetcher[fid]
                     continue
 
                 rank = self._id_to_rank[fid]
                 for source in sources:
                     if source in source_to_fetcher_id:
                         self._log_rejection(source, rank, source_ranks[source], translation=False)
                     else:
                         source_to_fetcher_id[source] = fid
                         source_ranks[source] = rank
+
+            if not source_to_fetcher_id:
+                warnings.warn("No fetchers left. See log output for more information.", UserWarning, stacklevel=2)
             self._source_to_fetcher_id_actual = source_to_fetcher_id
 
         return self._source_to_fetcher_id_actual
 
     def _gather(self, futures: Iterable[Future[FetchResult[SourceType]]]) -> SourcePlaceholderTranslations[SourceType]:
         ans: SourcePlaceholderTranslations[SourceType] = {}
         source_ranks: Dict[SourceType, int] = {}
```

### Comparing `id_translation-0.4.0/src/id_translation/fetching/_pandas_fetcher.py` & `id_translation-0.5.0/src/id_translation/fetching/_pandas_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/fetching/_sql_fetcher.py` & `id_translation-0.5.0/src/id_translation/fetching/_sql_fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import sqlalchemy
 from rics.misc import tname
 from rics.performance import format_perf_counter
 
 from ..offline.types import PlaceholderTranslations
 from ..types import ID, IdType
-from . import exceptions, support
+from . import exceptions
 from ._abstract_fetcher import AbstractFetcher
 from .exceptions import FetcherWarning
 from .types import FetchInstruction
 
 
 class SqlFetcher(AbstractFetcher[str, IdType]):
     """Fetch data from a SQL source. Requires SQLAlchemy.
@@ -104,26 +104,30 @@
             self._table_ts_dict = self._get_summaries()
 
         return self._table_ts_dict
 
     def fetch_translations(self, instr: FetchInstruction[str, IdType]) -> PlaceholderTranslations[str]:
         """Fetch columns from a SQL database."""
         ts = self._summaries[instr.source]
-        columns = ts.select_columns(instr)
-        select = sqlalchemy.select(*map(ts.columns.get, columns))  # type: ignore[arg-type]
+        if self._selective_fetch_all or not instr.fetch_all:
+            known = set(ts.columns.keys())
+            select = sqlalchemy.select(*(ts.columns[c] for c in instr.placeholders if c in known))
+        else:
+            select = ts.id_column.table.select()
 
         if instr.ids is None and not ts.fetch_all_permitted:  # pragma: no cover
             raise exceptions.ForbiddenOperationError(self._FETCH_ALL, f"disabled for table '{ts.name}'.")
 
         stmt = select if instr.ids is None else self._make_query(ts, select, set(instr.ids))
         stmt = self.finalize_statement(stmt, ts.id_column, ts.id_column.table)
 
         with self.engine.connect() as conn:
-            records = tuple(map(tuple, conn.execute(stmt)))
-        return PlaceholderTranslations(instr.source, tuple(columns), records)
+            cursor = conn.execute(stmt)
+            records = tuple(map(tuple, cursor))
+        return PlaceholderTranslations(instr.source, tuple(cursor.keys()), records)
 
     StatementType = TypeVar("StatementType", bound=sqlalchemy.sql.Executable)
     """Input and return bounds for :meth:`.finalize_statement`."""
 
     def finalize_statement(
         self,
         statement: StatementType,
@@ -403,11 +407,7 @@
         """Approximate size of the table."""
         columns: sqlalchemy.sql.ColumnCollection  # type: ignore[type-arg]
         """A flag indicating that the FETCH_ALL-operation is permitted for this table."""
         fetch_all_permitted: bool
         """A flag indicating that the FETCH_ALL-operation is permitted for this table."""
         id_column: sqlalchemy.Column  # type: ignore[type-arg]
         """The ID column of the table."""
-
-        def select_columns(self, instr: FetchInstruction[str, IdType]) -> List[str]:
-            """Return required and optional columns of the table."""
-            return support.select_placeholders(instr, self.columns.keys())
```

### Comparing `id_translation-0.4.0/src/id_translation/fetching/exceptions.py` & `id_translation-0.5.0/src/id_translation/fetching/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/fetching/types.py` & `id_translation-0.5.0/src/id_translation/fetching/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/mapping/__init__.py` & `id_translation-0.5.0/src/id_translation/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/mapping/_cardinality.py` & `id_translation-0.5.0/src/id_translation/mapping/_cardinality.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/mapping/_directional_mapping.py` & `id_translation-0.5.0/src/id_translation/mapping/_directional_mapping.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/mapping/_heuristic_score.py` & `id_translation-0.5.0/src/id_translation/mapping/_heuristic_score.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/mapping/_mapper.py` & `id_translation-0.5.0/src/id_translation/mapping/_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,16 +214,14 @@
                 )
             return scores
 
         if self.logger.isEnabledFor(logging.DEBUG):
             self.logger.debug(f"Begin computing match scores{extra} for {values}x{candidates} using {self._score}.")
 
         unmapped_values = self._handle_overrides(scores, context, override_function)
-        if not unmapped_values:
-            return scores
 
         verbose_logger = self._get_verbose_logger()
         for value in unmapped_values:
             filtered_candidates = self._apply_filters(value, candidates, context, kwargs)
             if not filtered_candidates:
                 continue
 
@@ -321,15 +319,15 @@
 
         if override_function:
             for value, override_candidate in self._get_function_overrides(
                 override_function, scores.index, scores.columns, context
             ):
                 if self.logger.isEnabledFor(logging.DEBUG):
                     self.logger.debug(
-                        f"Using override {repr(value)} -> {repr(override_candidate)} returned by {override_function}."
+                        f"Using override {repr(value)} -> {repr(override_candidate)} returned by {override_function=}."
                     )
                 apply(value, override_candidate)
 
         for value, override_candidate in self._get_static_overrides(unmapped_values, context).items():
             apply(value, override_candidate)
 
         if self.logger.isEnabledFor(logging.DEBUG) and (self._overrides or override_function is not None):
@@ -372,15 +370,16 @@
         for value in values:
             user_override = func(value, candidates, context)
             if user_override is None:
                 continue
             if self.unknown_user_override_action is not ActionLevel.IGNORE and user_override not in candidates:
                 msg = (
                     f"The user-defined override function {func} returned an unknown candidate={repr(user_override)} for"
-                    f" {value=}. If this is intended behaviour, set unknown_user_override_action='ignore' to allow."
+                    f" {value=}."
+                    "\nHint: If this is intended behaviour, set unknown_user_override_action='ignore' to allow."
                 )
                 if self.unknown_user_override_action is ActionLevel.RAISE:
                     self.logger.error(msg)
                     raise UserMappingError(msg, value, candidates)
                 elif self.unknown_user_override_action is ActionLevel.WARN:
                     msg += " The override has been ignored."
                     self.logger.warning(msg)
```

### Comparing `id_translation-0.4.0/src/id_translation/mapping/exceptions.py` & `id_translation-0.5.0/src/id_translation/mapping/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/mapping/filter_functions.py` & `id_translation-0.5.0/src/id_translation/mapping/filter_functions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/mapping/heuristic_functions.py` & `id_translation-0.5.0/src/id_translation/mapping/heuristic_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,27 @@
     name: str,
     candidates: Iterable[str],
     context: Any,
 ) -> Tuple[str, List[str]]:
     """Try to make `value` look like the name of a database table."""
 
     def apply(s: str) -> str:
-        s = s.lower().replace("_", "").replace(".", "")
+        s = s.lower()
+        if s == "id":
+            return "id"
         s = s[: -len("id")] if s.endswith("id") else s
-        s = s if s.endswith("s") else s + "s"
+        s = s.replace("_", "").replace(".", "")
+
+        if s[-1] == "s":
+            pass  # Assume that any word ending in "s" is already pluralized.
+        elif s[-1] in "xz" or (s[-1] == "h" and s[-2] in "sc"):
+            s += "es"
+        else:
+            s += "s"
+
         return s
 
     return apply(name), list(map(apply, candidates))
 
 
 def short_circuit(
     value: str,
```

### Comparing `id_translation-0.4.0/src/id_translation/mapping/score_functions.py` & `id_translation-0.5.0/src/id_translation/mapping/score_functions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/mapping/support.py` & `id_translation-0.5.0/src/id_translation/mapping/support.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         for record in list(matches):
             supersedes: List[MatchScores.Reject[ValueType, CandidateType]] = []
             if self.logger.isEnabledFor(logging.DEBUG) and rejections:
                 for rr in rejections:
                     if record in (rr.superseding_value, rr.superseding_candidate):
                         supersedes.append(rr)
 
-            if self.logger.isEnabledFor(logging.INFO):
+            if self.logger.isEnabledFor(logging.DEBUG):
                 reason = "(short-circuit or override)" if record.score == np.inf else f">= {self._min_score}"
                 self.logger.debug(f"Accepted: {record} {reason}.")
 
             if supersedes:
                 s = "\n".join("    " + rr.explain(self._min_score) for rr in supersedes)
                 self.logger.debug(f"This match supersedes {len(supersedes)} other matches:\n{s}")
 
@@ -146,15 +146,15 @@
         else:
             matches = self._select_many_to_many(records, rejections)
 
         return list(matches), rejections or []
 
     def _get_sorted(self) -> pd.Series:
         sorted_scores: pd.Series = self._matrix.stack()
-        sorted_scores.sort_values(ascending=False, inplace=True)
+        sorted_scores.sort_values(ascending=False, inplace=True, kind="stable")
         return sorted_scores
 
     def get_above(self) -> List["MatchScores.Record[ValueType, CandidateType]"]:
         """Get all records with scores `above` the threshold."""
         s = self._get_sorted()
         return self._from_series(s[s >= self._min_score])
```

### Comparing `id_translation-0.4.0/src/id_translation/mapping/types.py` & `id_translation-0.5.0/src/id_translation/mapping/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/offline/_format.py` & `id_translation-0.5.0/src/id_translation/offline/_format.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,16 +37,33 @@
         >>> fmt.fstring(), fmt.fstring().format(id=0, name='Tarzan')
         ('{id}:{name}', '0:Tarzan')
 
         ..but the `placeholders` attribute can be used to retrieve all placeholders, required and optional:
 
         >>> fmt.placeholders
         ('id', 'name', 'is_nice')
-        >>> fmt.fstring(fmt.placeholders), fmt.fstring(fmt.placeholders).format(id=1, name='Morris', is_nice=True)
-        ('{id}:{name}, nice={is_nice}', '1:Morris, nice=True')
+        >>> fmt.fstring(fmt.placeholders).format(id=1, name='Morris', is_nice=True)
+        '1:Morris, nice=True'
+
+    The :class:`.Translator` will automatically add optional placeholders, if they are present in the source.
+
+    .. note::
+       Python format specifications and conversions are preserved.
+
+    This is especially useful for long values such as UUIDs.
+
+    >>> from uuid import UUID
+    >>> uuid = UUID("550e8400-e29b-41d4-a716-446655440000")
+
+    Convert to string and truncate to eight characters.
+
+    >>> Format('{id!s:.8}:{name!r}').fstring().format(id=uuid, name='Sofia')
+    "550e8400:'Sofia'"
+
+    See the :py:ref:`formatspec` documentation for details.
     """
 
     def __init__(self, fmt: str) -> None:
         self._fmt = fmt
         self._elements: List[parse_format_string.Element] = self._parse_format_string(fmt)
 
     def fstring(self, placeholders: Iterable[str] = None, positional: bool = False) -> str:
```

### Comparing `id_translation-0.4.0/src/id_translation/offline/_format_applier.py` & `id_translation-0.5.0/src/id_translation/offline/_format_applier.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/offline/_magic_dict.py` & `id_translation-0.5.0/src/id_translation/offline/_magic_dict.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/offline/_translation_map.py` & `id_translation-0.5.0/src/id_translation/offline/_translation_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from copy import copy
 from typing import Any, Dict, Generic, Iterator, List, Mapping, Optional, Set, Union
 
 from rics.collections.dicts import InheritedKeysDict, reverse_dict
 from rics.misc import tname
 
-from ..types import HasSources, IdType, NameType, SourceType
+from ..types import HasSources, IdType, NameToSource, NameType, SourceType
 from ._format import Format
 from ._format_applier import FormatApplier
 from ._magic_dict import MagicDict
 from .types import FormatType, SourcePlaceholderTranslations
 
-NameToSource = Dict[NameType, SourceType]
-
 
 class TranslationMap(
     Generic[NameType, SourceType, IdType],
     HasSources[SourceType],
     Mapping[Union[NameType, SourceType], MagicDict[IdType]],
 ):
     """Storage class for fetched translations.
```

### Comparing `id_translation-0.4.0/src/id_translation/offline/parse_format_string.py` & `id_translation-0.5.0/src/id_translation/offline/parse_format_string.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,42 +75,50 @@
 
     part: str
     """String literal."""
     placeholders: _List[str]
     """Placeholder names in `part`, if any."""
     required: bool
     """Flag indicating whether the element may be excluded."""
-
-    @property
-    def positional_part(self) -> str:
-        """Return a positional version of the `part` attribute."""
-        if not self.placeholders:
-            return self.part
-
-        return self.part.format(**{p: "{}" for p in self.placeholders})
+    positional_part: str
+    """Return a positional version of the `part` attribute."""
 
     @staticmethod
     def make(s: str, in_optional_block: bool) -> "Element":
         """Create an ``Element`` from an input string `s`.
 
         Args:
             s: Input data.
             in_optional_block: Flag indicating whether `s` was found inside an optional block.
 
         Returns:
             A new ``Element``.
         """
         parsed_block = s.replace("[[", "[").replace("]]", "]")
-        placeholders = [x[1] for x in _formatter.parse(parsed_block) if x[1]]
 
-        return Element(
-            parsed_block,
-            placeholders,
-            not (placeholders and in_optional_block),
-        )
+        parts = []
+        placeholders: List[str] = []
+        for literal_text, field_name, format_spec, conversion in _formatter.parse(parsed_block):
+            parts.append(literal_text)
+            if field_name:
+                placeholder, _, attribute = field_name.partition(".")
+                parts.append("{")
+
+                if attribute:
+                    parts.append(".")
+                    parts.append(attribute)
+
+                placeholders.append(placeholder)
+                if conversion is not None:
+                    parts.extend(("!", conversion))
+                if format_spec is not None:
+                    parts.extend((":", format_spec))
+                parts.append("}")
+
+        return Element(parsed_block, placeholders, not (placeholders and in_optional_block), "".join(parts))
 
 
 def get_elements(fmt: str) -> List[Element]:
     """Split a format string into elements.
 
     Args:
         fmt: User input string.
@@ -119,15 +127,15 @@
         A list of parsed elements.
 
     Raises:
         BadDelimiterError: For unbalanced optional block delimitation characters.
         UnusedOptionalBlockError: If optional blocks are defined without placeholders.
     """
     if not fmt:
-        return [Element("", [], required=True)]
+        return [Element("", [], required=True, positional_part="")]
 
     same_count = 1
     ans = []
 
     in_optional_block = fmt[0] == OPTIONAL_BLOCK_START_DELIMITER
     open_idx = 0 if in_optional_block else -1
     prev_idx = int(in_optional_block)
```

### Comparing `id_translation-0.4.0/src/id_translation/offline/types.py` & `id_translation-0.5.0/src/id_translation/offline/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/testing.py` & `id_translation-0.5.0/src/id_translation/testing.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.4.0/src/id_translation/types.py` & `id_translation-0.5.0/src/id_translation/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 Translatable = _type.TypeVar(
     "Translatable",
     # Primitive types
     str,
     int,
     _type.Dict,  # type: ignore[type-arg]  # TODO: Need Higher-Kinded TypeVars
+    _type.Set,  # type: ignore[type-arg]  # TODO: Need Higher-Kinded TypeVars
     _type.Sequence,  # type: ignore[type-arg]  # TODO: Need Higher-Kinded TypeVars
     "NDArray",  # type: ignore[type-arg]  # TODO: Need Higher-Kinded TypeVars
     "pandas.DataFrame",
     "pandas.Index",
     "pandas.Series",
 )
 """Enumeration of translatable types.
@@ -39,14 +40,17 @@
 
 IdType = _type.TypeVar("IdType", int, str, _UUID)
 """Type of the value being translated into human-readable labels."""
 
 SourceType = _type.TypeVar("SourceType", bound=_type.Hashable)
 """Type used to describe sources. Typically a string for things like files and database tables."""
 
+NameToSource = _type.Dict[NameType, SourceType]
+"""A mapping from name to source."""
+
 NamesPredicate = _type.Callable[[NameType], bool]
 """A predicate type on names."""
 NameTypes = _type.Union[NameType, _type.Iterable[NameType]]
 """A union of a name type, or an iterable thereof."""
 Names = _type.Union[NameTypes[NameType], NamesPredicate[NameType]]
 """Acceptable name types."""
```

### Comparing `id_translation-0.4.0/PKG-INFO` & `id_translation-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id-translation
-Version: 0.4.0
+Version: 0.5.0
 Summary: Convert IDs into human-readable labels.
 Home-page: https://github.com/rsundqvist/id-translation
 Keywords: id-translation
 Author: Richard Sundqvist
 Author-email: richard.sundqvist@live.se
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 4 - Beta
```

