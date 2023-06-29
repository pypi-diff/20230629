# Comparing `tmp/arabica-1.6.5.tar.gz` & `tmp/arabica-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.6.5.tar", last modified: Wed Jun 28 20:53:49 2023, max compression
+gzip compressed data, was "arabica-1.6.6.tar", last modified: Thu Jun 29 20:11:21 2023, max compression
```

## Comparing `arabica-1.6.5.tar` & `arabica-1.6.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 20:53:49.041111 arabica-1.6.5/
--rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 arabica-1.6.5/LICENSE
--rw-rw-rw-   0        0        0     7766 2023-06-28 20:53:49.041111 arabica-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     7000 2023-06-28 19:24:43.000000 arabica-1.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 20:53:49.025343 arabica-1.6.5/arabica/
--rw-rw-rw-   0        0        0      105 2023-06-24 17:39:10.000000 arabica-1.6.5/arabica/__init__.py
--rw-rw-rw-   0        0        0    11892 2023-06-22 16:47:25.000000 arabica-1.6.5/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    31625 2023-06-28 17:37:14.000000 arabica-1.6.5/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.5/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.5/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.5/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.5/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.5/arabica/preprocess.py
--rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.5/arabica/sentiment.py
--rw-rw-rw-   0        0        0      447 2023-06-22 00:51:28.000000 arabica-1.6.5/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-06-28 20:53:49.041111 arabica-1.6.5/arabica.egg-info/
--rw-rw-rw-   0        0        0     7766 2023-06-28 20:53:48.000000 arabica-1.6.5/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-06-28 20:53:49.000000 arabica-1.6.5/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 20:53:48.000000 arabica-1.6.5/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-06-28 20:53:48.000000 arabica-1.6.5/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-28 20:53:48.000000 arabica-1.6.5/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-06-28 20:51:59.000000 arabica-1.6.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 20:53:49.041111 arabica-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1126 2023-06-28 20:51:59.000000 arabica-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:11:21.373956 arabica-1.6.6/
+-rw-rw-rw-   0        0        0       39 2023-06-29 19:51:45.000000 arabica-1.6.6/LICENSE
+-rw-rw-rw-   0        0        0     7856 2023-06-29 20:11:21.373956 arabica-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7051 2023-06-29 20:05:24.000000 arabica-1.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 20:11:21.360312 arabica-1.6.6/arabica/
+-rw-rw-rw-   0        0        0      105 2023-06-29 20:10:39.000000 arabica-1.6.6/arabica/__init__.py
+-rw-rw-rw-   0        0        0    11892 2023-06-22 16:47:25.000000 arabica-1.6.6/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    31618 2023-06-29 18:51:09.000000 arabica-1.6.6/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.6/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.6/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.6/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.6/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.6/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.6/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      447 2023-06-22 00:51:28.000000 arabica-1.6.6/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:11:21.360312 arabica-1.6.6/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7856 2023-06-29 20:11:21.000000 arabica-1.6.6/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-29 20:11:21.000000 arabica-1.6.6/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 20:11:21.000000 arabica-1.6.6/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-06-29 20:11:21.000000 arabica-1.6.6/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-29 20:11:21.000000 arabica-1.6.6/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      559 2023-06-29 20:10:39.000000 arabica-1.6.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 20:11:21.373956 arabica-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1154 2023-06-29 20:10:39.000000 arabica-1.6.6/setup.py
```

### Comparing `arabica-1.6.5/PKG-INFO` & `arabica-1.6.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.5
+Version: 1.6.6
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
-License: MIT License
+License: OSI Approved :: Apache Software License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8, !=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Arabica
 **Python package for exploratory text data analysis**
@@ -25,16 +25,16 @@
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
 * **Structural breaks identification**: Jenks Optimization Method
 
 It automatically cleans data from punctuation on input. It can also apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
-* Remove the standard list(s) of stopwords
-* Remove an additional list of specific strings
+* Remove the standard list(s) of stop words
+* Remove an additional list of stop words
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
 It reads dates in:
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
 * **European-style**: *DD/MM/YYYY* (2013-31-12, 09-Feb-2009, 2013-31-12 11:46:17, etc.) date and datetime formats.
@@ -65,45 +65,44 @@
 from arabica import coffee_break 
 ```
 
 
 
 * **Choose a method:**
 
-**arabica_freq** enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings 
-removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
+**arabica_freq** enables a set of cleaning operations (lower casing, numbers, common stop words, and additional stop words removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
 
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
                  max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
-                 stopwords: [],            # Languages for stop words
-                 skip: [],                 # Remove additional strings
+                 stopwords: [],            # Languages for common stop words
+                 skip: [],                 # Remove additional list of stopwords
                  numbers: bool = False,    # Remove all digits
                  lower_case: bool = False  # Lowercase text
 ) 
 ```
 
-**cappuccino**  enables cleaning operations (lower casing, numbers, stop words, and additional strings
+**cappuccino** enables cleaning operations (lower casing, numbers, common stop words, and additional stop words 
 removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
-               stopwords: [],            # Languages for stop words
-               skip: [] ,                # Remove additional strings
+               stopwords: [],            # Languages for common stop words
+               skip: [] ,                # Remove additional list of stop words
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
 ```
 
 **coffee_break** provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
 
 * **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See more [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
@@ -114,15 +113,15 @@
 
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
                  model: str,                # Sentiment classifier, 'vader' - general language, 'finvader' - financial text                
-                 skip: [] ,                 # Remove additional strings
+                 skip: [] ,                 # Remove additional list of stop words
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
                  n_breaks: int =''          # Number of breaks: min. 2
 )
 ```
 
 ## Documentation, examples and tutorials
```

### Comparing `arabica-1.6.5/README.md` & `arabica-1.6.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
 * **Structural breaks identification**: Jenks Optimization Method
 
 It automatically cleans data from punctuation on input. It can also apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
-* Remove the standard list(s) of stopwords
-* Remove an additional list of specific strings
+* Remove the standard list(s) of stop words
+* Remove an additional list of stop words
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
 It reads dates in:
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
 * **European-style**: *DD/MM/YYYY* (2013-31-12, 09-Feb-2009, 2013-31-12 11:46:17, etc.) date and datetime formats.
@@ -48,45 +48,44 @@
 from arabica import coffee_break 
 ```
 
 
 
 * **Choose a method:**
 
-**arabica_freq** enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings 
-removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
+**arabica_freq** enables a set of cleaning operations (lower casing, numbers, common stop words, and additional stop words removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
 
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
                  max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
-                 stopwords: [],            # Languages for stop words
-                 skip: [],                 # Remove additional strings
+                 stopwords: [],            # Languages for common stop words
+                 skip: [],                 # Remove additional list of stopwords
                  numbers: bool = False,    # Remove all digits
                  lower_case: bool = False  # Lowercase text
 ) 
 ```
 
-**cappuccino**  enables cleaning operations (lower casing, numbers, stop words, and additional strings
+**cappuccino** enables cleaning operations (lower casing, numbers, common stop words, and additional stop words 
 removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
-               stopwords: [],            # Languages for stop words
-               skip: [] ,                # Remove additional strings
+               stopwords: [],            # Languages for common stop words
+               skip: [] ,                # Remove additional list of stop words
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
 ```
 
 **coffee_break** provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
 
 * **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See more [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
@@ -97,15 +96,15 @@
 
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
                  model: str,                # Sentiment classifier, 'vader' - general language, 'finvader' - financial text                
-                 skip: [] ,                 # Remove additional strings
+                 skip: [] ,                 # Remove additional list of stop words
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
                  n_breaks: int =''          # Number of breaks: min. 2
 )
 ```
 
 ## Documentation, examples and tutorials
```

### Comparing `arabica-1.6.5/arabica/arabica_freq.py` & `arabica-1.6.6/arabica/arabica_freq.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.5/arabica/cappuccino.py` & `arabica-1.6.6/arabica/cappuccino.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,15 @@
                 fig = (ggplot(reshaped_unigram, aes('period', 'bigram', fill='frequency'))
                        + geom_tile(aes(width=.95, height=.95))
                        + geom_text(aes(label='frequency'), size=10)
                        + theme_minimal()
                        + scale_fill_gradient(name = "frequency",
                                              low = "#f0f4ed",
                                              high = "#496160")
-                       + theme(axis_title_x=element_text(colour = "black"), # TADY
+                       + theme(axis_title_x=element_text(colour = "black"),
                                axis_title_y=element_text(colour="black"),
                                axis_text_x=element_text(colour = "black", rotation=45, hjust= 1),
                                legend_text = element_text(size = 5,vjust = 0.2),
                                legend_title = element_text(color = "black", vjust = 0.8, size = 10),
                                figure_size= (3 + ((len(period) /4)), (2 + (max_words * 2.2))),
                                panel_grid_major = element_line(color='black',size = 0.1),
                                panel_background = element_rect(colour = "white", fill = "white"),
```

### Comparing `arabica-1.6.5/arabica/clean_ngram.py` & `arabica-1.6.6/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.5/arabica/coffee_break.py` & `arabica-1.6.6/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.5/arabica/group.py` & `arabica-1.6.6/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.5/arabica/preprocess.py` & `arabica-1.6.6/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.5/arabica/sentiment.py` & `arabica-1.6.6/arabica/sentiment.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.5/arabica.egg-info/PKG-INFO` & `arabica-1.6.6/arabica.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.5
+Version: 1.6.6
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
-License: MIT License
+License: OSI Approved :: Apache Software License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8, !=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Arabica
 **Python package for exploratory text data analysis**
@@ -25,16 +25,16 @@
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
 * **Structural breaks identification**: Jenks Optimization Method
 
 It automatically cleans data from punctuation on input. It can also apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
-* Remove the standard list(s) of stopwords
-* Remove an additional list of specific strings
+* Remove the standard list(s) of stop words
+* Remove an additional list of stop words
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
 It reads dates in:
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
 * **European-style**: *DD/MM/YYYY* (2013-31-12, 09-Feb-2009, 2013-31-12 11:46:17, etc.) date and datetime formats.
@@ -65,45 +65,44 @@
 from arabica import coffee_break 
 ```
 
 
 
 * **Choose a method:**
 
-**arabica_freq** enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings 
-removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
+**arabica_freq** enables a set of cleaning operations (lower casing, numbers, common stop words, and additional stop words removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
 
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
                  max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
-                 stopwords: [],            # Languages for stop words
-                 skip: [],                 # Remove additional strings
+                 stopwords: [],            # Languages for common stop words
+                 skip: [],                 # Remove additional list of stopwords
                  numbers: bool = False,    # Remove all digits
                  lower_case: bool = False  # Lowercase text
 ) 
 ```
 
-**cappuccino**  enables cleaning operations (lower casing, numbers, stop words, and additional strings
+**cappuccino** enables cleaning operations (lower casing, numbers, common stop words, and additional stop words 
 removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
-               stopwords: [],            # Languages for stop words
-               skip: [] ,                # Remove additional strings
+               stopwords: [],            # Languages for common stop words
+               skip: [] ,                # Remove additional list of stop words
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
 ```
 
 **coffee_break** provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
 
 * **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See more [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
@@ -114,15 +113,15 @@
 
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
                  model: str,                # Sentiment classifier, 'vader' - general language, 'finvader' - financial text                
-                 skip: [] ,                 # Remove additional strings
+                 skip: [] ,                 # Remove additional list of stop words
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
                  n_breaks: int =''          # Number of breaks: min. 2
 )
 ```
 
 ## Documentation, examples and tutorials
```

### Comparing `arabica-1.6.5/pyproject.toml` & `arabica-1.6.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 [project]
 name = "arabica"
-version = "1.6.5"
+version = "1.6.6"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
 
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/PetrKorab/Arabica"
 "Bug Tracker" = "https://github.com/PetrKorab/Arabica/issues"
```

### Comparing `arabica-1.6.5/setup.py` & `arabica-1.6.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.6.5",
+        version="1.6.6",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
@@ -24,9 +24,9 @@
                             'matplotlib == 3.6.0',
                             'matplotlib-inline == 0.1.6',
                             'plotnine == 0.10.1',
                             'wordcloud == 1.8.2.2',
                             'jenkspy == 0.3.2',
                             'vaderSentiment == 3.3.2',
                             'cleantext == 1.1.4'],
-        license='MIT License'
+        license='OSI Approved :: Apache Software License'
     )
```

