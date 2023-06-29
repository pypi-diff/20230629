# Comparing `tmp/dexcolor-0.1.tar.gz` & `tmp/dexcolor-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexcolor-0.1.tar", last modified: Tue Jun 27 18:11:58 2023, max compression
+gzip compressed data, was "dexcolor-1.0.tar", last modified: Thu Jun 29 07:22:50 2023, max compression
```

## Comparing `dexcolor-0.1.tar` & `dexcolor-1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 18:11:58.240969 dexcolor-0.1/
--rw-rw-rw-   0        0        0     1084 2023-06-27 17:24:27.000000 dexcolor-0.1/LICENSE
--rw-rw-rw-   0        0        0     2733 2023-06-27 18:11:58.240969 dexcolor-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2264 2023-06-27 17:02:31.000000 dexcolor-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 18:11:58.225156 dexcolor-0.1/dexcolor/
--rw-rw-rw-   0        0        0      101 2023-06-27 13:00:07.000000 dexcolor-0.1/dexcolor/__init__.py
--rw-rw-rw-   0        0        0     4167 2023-06-27 13:05:05.000000 dexcolor-0.1/dexcolor/background.py
--rw-rw-rw-   0        0        0     7117 2023-06-27 13:00:01.000000 dexcolor-0.1/dexcolor/dex.py
--rw-rw-rw-   0        0        0     1682 2023-06-27 12:37:02.000000 dexcolor-0.1/dexcolor/styles.py
-drwxrwxrwx   0        0        0        0 2023-06-27 18:11:58.240969 dexcolor-0.1/dexcolor.egg-info/
--rw-rw-rw-   0        0        0     2733 2023-06-27 18:11:58.000000 dexcolor-0.1/dexcolor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-06-27 18:11:58.000000 dexcolor-0.1/dexcolor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 18:11:58.000000 dexcolor-0.1/dexcolor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 18:11:58.000000 dexcolor-0.1/dexcolor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      550 2023-06-27 17:22:28.000000 dexcolor-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-27 18:11:58.240969 dexcolor-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 07:22:50.725499 dexcolor-1.0/
+-rw-rw-rw-   0        0        0     1084 2023-06-27 17:24:27.000000 dexcolor-1.0/LICENSE
+-rw-rw-rw-   0        0        0     4113 2023-06-29 07:22:50.725499 dexcolor-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3541 2023-06-28 15:06:59.000000 dexcolor-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 07:22:50.694268 dexcolor-1.0/dexcolor/
+-rw-rw-rw-   0        0        0      130 2023-06-28 09:54:49.000000 dexcolor-1.0/dexcolor/__init__.py
+-rw-rw-rw-   0        0        0     4167 2023-06-27 13:05:05.000000 dexcolor-1.0/dexcolor/background.py
+-rw-rw-rw-   0        0        0     7117 2023-06-27 13:00:01.000000 dexcolor-1.0/dexcolor/dex.py
+-rw-rw-rw-   0        0        0     2984 2023-06-28 10:14:06.000000 dexcolor-1.0/dexcolor/rt.py
+-rw-rw-rw-   0        0        0     1682 2023-06-27 12:37:02.000000 dexcolor-1.0/dexcolor/styles.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:22:50.725499 dexcolor-1.0/dexcolor.egg-info/
+-rw-rw-rw-   0        0        0     4113 2023-06-29 07:22:50.000000 dexcolor-1.0/dexcolor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-06-29 07:22:50.000000 dexcolor-1.0/dexcolor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:22:50.000000 dexcolor-1.0/dexcolor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 07:22:50.000000 dexcolor-1.0/dexcolor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      644 2023-06-29 07:20:20.000000 dexcolor-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 07:22:50.725499 dexcolor-1.0/setup.cfg
```

### Comparing `dexcolor-0.1/LICENSE` & `dexcolor-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dexcolor-0.1/PKG-INFO` & `dexcolor-1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,123 @@
 Metadata-Version: 2.1
 Name: dexcolor
-Version: 0.1
+Version: 1.0
 Summary: Terminal colored text.
-Author-email: Terong33 <thisterong33@proton.me>
+Author-email: Terong333 <thisterong33@proton.me>
 Project-URL: Homepage, https://github.com/Terong33/dexcolor
+Project-URL: PyPI_page, https://pypi.org/project/dexcolor/
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Terminals
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## dexcolor
 
-`dexcolor` is a Python module that provides functionality for printing text with different colors, styles, and backgrounds in the terminal. It offers a convenient way to add visual enhancements to your console output.
+dexcolor is a Python module that provides various functions for working with colors, styles, and backgrounds in the terminal.
+
+### Table of Contents
+
+- [Installation](#installation)
+- [Usage](#usage)
+- [Color Examples](#color-examples)
+- [Style Examples](#style-examples)
+- [Background Examples](#background-examples)
+- [Rainbow Text Example](#rainbow-text-example)
+- [Additional information](#Additional-Information)
+- [Contribution and Feedback](#Contribution-and-Feedback)
 
 ### Installation
 
-You can install `dexcolor` using pip:
+To install dexcolor, you can use pip:
 
-```
+```shell
 pip install dexcolor
 ```
 
 ### Usage
 
-Here are some examples of how to use `dexcolor`:
+Here is an example of how to use dexcolor:
 
-#### Example 1: Using color, style, and background
+```python
+from dexcolor import DEX, style, back, RESET
+
+# Color, Style, and Background Example
+print(DEX.purple('Example', style='bold', back='yellow'))
+# Output: The word "Example" will be printed in purple color, bold style, and yellow background.
+
+# Style Example
+print(style.bold('Example'))
+# Output: The word "Example" will be printed in the default color with bold style.
+
+# Background Example
+print(back.red('Example'))
+# Output: The word "Example" will be printed in the default color with a red background.
+
+# Reset Example
+print(DEX.purple('Example', style='bold', back='yellow') + RESET)
+print(style.bold('Example') + RESET)
+print(back.red('Example') + RESET)
+# Output: The word "Example" in each line will be printed with the specified color, style, and background, followed by a reset to revert to the default settings.
+```
+
+### Color Examples
+
+Here are some examples of using colors with dexcolor:
 
 ```python
 from dexcolor import DEX
 
-print(DEX.purple('Example', style='bold', back='yellow'))
+print(DEX.red('This text is in red color'))
+print(DEX.green('This text is in green color'))
+print(DEX.blue('This text is in blue color'))
 ```
 
-Output: The word "Example" will be printed in purple color, bold style, and yellow background.
+### Style Examples
 
-#### Example 2: Using style only
+Here are some examples of using styles with dexcolor:
 
 ```python
 from dexcolor import style
 
-print(style.bold('Example'))
+print(style.bold('This text is bold'))
+print(style.underline('This text is underlined'))
+print(style.inverse('This text is inversed'))
 ```
 
-Output: The word "Example" will be printed in the default color with bold style.
+### Background Examples
 
-#### Example 3: Using background only
+Here are some examples of using backgrounds with dexcolor:
 
 ```python
 from dexcolor import back
 
-print(back.red('Example'))
+print(back.red('This text has a red background'))
+print(back.green('This text has a green background'))
+print(back.blue('This text has a blue background'))
 ```
 
-Output: The word "Example" will be printed in the default color with a red background.
+### Rainbow Text Example
 
-#### Example 4: Using reset
+Here is an example of using the RainbowText function from dexcolor to print text in rainbow colors:
 
 ```python
-from dexcolor import DEX, style, back, RESET
+from dexcolor import RainbowText
 
-print(DEX.purple('Example', style='bold', back='yellow') + RESET)
-print(style.bold('Example') + RESET)
-print(back.red('Example') + RESET)
+print(RainbowText.dex('text here', 'red', 'dark_gray', 'blue'))
 ```
 
-Output: The word "Example" in each line will be printed with the specified color, style, and background, followed by a reset to revert to the default settings.
+The `RainbowText` function takes a string as input and generates a string with each character having a different rainbow color.
 
 ### Additional Information
 
-For more information and additional features provided by `dexcolor`, you can refer to the [dexcolor GitHub repository](https://github.com/Terong33/dexcolor) or the [dexcolor PyPI page](https://pypi.org/project/dexcolor/).
+For more information and additional features provided by `dexcolor`, you can refer to the [dexcolor GitHub repository](https://github.com/Terong33/dexcolor/) or the [dexcolor PyPI page](https://pypi.org/project/dexcolor/).
 
 Please note that the provided examples are just a subset of the capabilities of `dexcolor`. You can explore the module further to discover more options and customization possibilities.
 
 ### Contribution and Feedback
 
 If you have any suggestions, feature requests, or bug reports related to `dexcolor`, please feel free to contribute to the project on GitHub or provide feedback to the module's maintainers. Your input is valuable in improving the module and making it more versatile for a wider range of use cases.
```

### Comparing `dexcolor-0.1/README.md` & `dexcolor-1.0/dexcolor.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,124 @@
+Metadata-Version: 2.1
+Name: dexcolor
+Version: 1.0
+Summary: Terminal colored text.
+Author-email: Terong333 <thisterong33@proton.me>
+Project-URL: Homepage, https://github.com/Terong33/dexcolor
+Project-URL: PyPI_page, https://pypi.org/project/dexcolor/
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Terminals
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## dexcolor
 
-`dexcolor` is a Python module that provides functionality for printing text with different colors, styles, and backgrounds in the terminal. It offers a convenient way to add visual enhancements to your console output.
+dexcolor is a Python module that provides various functions for working with colors, styles, and backgrounds in the terminal.
+
+### Table of Contents
+
+- [Installation](#installation)
+- [Usage](#usage)
+- [Color Examples](#color-examples)
+- [Style Examples](#style-examples)
+- [Background Examples](#background-examples)
+- [Rainbow Text Example](#rainbow-text-example)
+- [Additional information](#Additional-Information)
+- [Contribution and Feedback](#Contribution-and-Feedback)
 
 ### Installation
 
-You can install `dexcolor` using pip:
+To install dexcolor, you can use pip:
 
-```
+```shell
 pip install dexcolor
 ```
 
 ### Usage
 
-Here are some examples of how to use `dexcolor`:
+Here is an example of how to use dexcolor:
+
+```python
+from dexcolor import DEX, style, back, RESET
+
+# Color, Style, and Background Example
+print(DEX.purple('Example', style='bold', back='yellow'))
+# Output: The word "Example" will be printed in purple color, bold style, and yellow background.
+
+# Style Example
+print(style.bold('Example'))
+# Output: The word "Example" will be printed in the default color with bold style.
+
+# Background Example
+print(back.red('Example'))
+# Output: The word "Example" will be printed in the default color with a red background.
+
+# Reset Example
+print(DEX.purple('Example', style='bold', back='yellow') + RESET)
+print(style.bold('Example') + RESET)
+print(back.red('Example') + RESET)
+# Output: The word "Example" in each line will be printed with the specified color, style, and background, followed by a reset to revert to the default settings.
+```
+
+### Color Examples
 
-#### Example 1: Using color, style, and background
+Here are some examples of using colors with dexcolor:
 
 ```python
 from dexcolor import DEX
 
-print(DEX.purple('Example', style='bold', back='yellow'))
+print(DEX.red('This text is in red color'))
+print(DEX.green('This text is in green color'))
+print(DEX.blue('This text is in blue color'))
 ```
 
-Output: The word "Example" will be printed in purple color, bold style, and yellow background.
+### Style Examples
 
-#### Example 2: Using style only
+Here are some examples of using styles with dexcolor:
 
 ```python
 from dexcolor import style
 
-print(style.bold('Example'))
+print(style.bold('This text is bold'))
+print(style.underline('This text is underlined'))
+print(style.inverse('This text is inversed'))
 ```
 
-Output: The word "Example" will be printed in the default color with bold style.
+### Background Examples
 
-#### Example 3: Using background only
+Here are some examples of using backgrounds with dexcolor:
 
 ```python
 from dexcolor import back
 
-print(back.red('Example'))
+print(back.red('This text has a red background'))
+print(back.green('This text has a green background'))
+print(back.blue('This text has a blue background'))
 ```
 
-Output: The word "Example" will be printed in the default color with a red background.
+### Rainbow Text Example
 
-#### Example 4: Using reset
+Here is an example of using the RainbowText function from dexcolor to print text in rainbow colors:
 
 ```python
-from dexcolor import DEX, style, back, RESET
+from dexcolor import RainbowText
 
-print(DEX.purple('Example', style='bold', back='yellow') + RESET)
-print(style.bold('Example') + RESET)
-print(back.red('Example') + RESET)
+print(RainbowText.dex('text here', 'red', 'dark_gray', 'blue'))
 ```
 
-Output: The word "Example" in each line will be printed with the specified color, style, and background, followed by a reset to revert to the default settings.
+The `RainbowText` function takes a string as input and generates a string with each character having a different rainbow color.
 
 ### Additional Information
 
-For more information and additional features provided by `dexcolor`, you can refer to the [dexcolor GitHub repository](https://github.com/Terong33/dexcolor) or the [dexcolor PyPI page](https://pypi.org/project/dexcolor/).
+For more information and additional features provided by `dexcolor`, you can refer to the [dexcolor GitHub repository](https://github.com/Terong33/dexcolor/) or the [dexcolor PyPI page](https://pypi.org/project/dexcolor/).
 
 Please note that the provided examples are just a subset of the capabilities of `dexcolor`. You can explore the module further to discover more options and customization possibilities.
 
 ### Contribution and Feedback
 
 If you have any suggestions, feature requests, or bug reports related to `dexcolor`, please feel free to contribute to the project on GitHub or provide feedback to the module's maintainers. Your input is valuable in improving the module and making it more versatile for a wider range of use cases.
 
-Happy coding with `dexcolor`!
+Happy coding with `dexcolor`!
```

### Comparing `dexcolor-0.1/dexcolor/background.py` & `dexcolor-1.0/dexcolor/background.py`

 * *Files identical despite different names*

### Comparing `dexcolor-0.1/dexcolor/dex.py` & `dexcolor-1.0/dexcolor/dex.py`

 * *Files identical despite different names*

### Comparing `dexcolor-0.1/dexcolor/styles.py` & `dexcolor-1.0/dexcolor/styles.py`

 * *Files identical despite different names*

### Comparing `dexcolor-0.1/pyproject.toml` & `dexcolor-1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dexcolor"
-version = "0.1"
+version = "1.0"
 authors = [
-  { name="Terong33", email="thisterong33@proton.me" },
+  { name="Terong333", email="thisterong33@proton.me" },
 ]
 description = "Terminal colored text."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
+    "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Terminals",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/Terong33/dexcolor"
+"Homepage" = "https://github.com/Terong33/dexcolor"
+"PyPI_page" = "https://pypi.org/project/dexcolor/"
```

