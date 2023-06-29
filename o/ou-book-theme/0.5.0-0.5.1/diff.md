# Comparing `tmp/ou_book_theme-0.5.0.tar.gz` & `tmp/ou_book_theme-0.5.1.tar.gz`

## Comparing `ou_book_theme-0.5.0.tar` & `ou_book_theme-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/package-lock.json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/package.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/rollup.config.js
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/__about__.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/scripts/activity.js
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/scripts/external-link.js
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/scripts/index.js
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/_activity.scss
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/_external-link.scss
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/_time.scss
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/_variables.scss
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/_where-next.scss
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/index.scss
--rw-r--r--   0        0        0    24010 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/cli/__init__.py
--rw-r--r--   0        0        0    40533 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/cli/mermaid-cli/package-lock.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/cli/mermaid-cli/package.json
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/extensions/__init__.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/extensions/activity.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/extensions/time.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/extensions/where_next.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/theme.conf
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg
--rw-r--r--   0        0        0    13489 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/.gitignore
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/README.md
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/package-lock.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/package.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/rollup.config.js
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/__about__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/assets/scripts/activity.js
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/assets/scripts/external-link.js
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/assets/scripts/index.js
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/assets/styles/_activity.scss
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/assets/styles/_external-link.scss
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/assets/styles/_time.scss
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/assets/styles/_variables.scss
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/assets/styles/_where-next.scss
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/assets/styles/index.scss
+-rw-r--r--   0        0        0    23955 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/cli/__init__.py
+-rw-r--r--   0        0        0    40533 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/cli/mermaid-cli/package-lock.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/cli/mermaid-cli/package.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/extensions/__init__.py
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/extensions/activity.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/extensions/time.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/extensions/where_next.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/theme/ou_book_theme/theme.conf
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg
+-rw-r--r--   0        0        0    13489 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/theme/ou_book_theme/static/images/logo.svg
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/.gitignore
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/README.md
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ou_book_theme-0.5.1/PKG-INFO
```

### Comparing `ou_book_theme-0.5.0/package-lock.json` & `ou_book_theme-0.5.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/rollup.config.js` & `ou_book_theme-0.5.1/rollup.config.js`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/ou_book_theme/__init__.py` & `ou_book_theme-0.5.1/ou_book_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/ou_book_theme/assets/styles/_activity.scss` & `ou_book_theme-0.5.1/ou_book_theme/assets/styles/_activity.scss`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/ou_book_theme/assets/styles/_where-next.scss` & `ou_book_theme-0.5.1/ou_book_theme/assets/styles/_where-next.scss`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/ou_book_theme/cli/__init__.py` & `ou_book_theme-0.5.1/ou_book_theme/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,16 @@
         presentation: str,
         counters: dict,
         part_title: str
     ) -> None:
     """Apply a range of post-processing fixes."""
     # Postprocessing required:
     # * Remove non-document cross-links
-    if node.tag == 'ComputerDisplayBlock':
+    if node.tag == 'ProgramListing':
         # Add paragraphs into block-level computer displays
-        node.tag = 'ComputerDisplay'
         lines = node.text.split('\n')
         if lines[-1].strip() == '':
             lines = lines[:-1]
         node.text = None
         for line in lines:
             para = etree.Element('Paragraph')
             para.text = line
@@ -218,15 +217,15 @@
     <xsl:template match="inline[@classes = 'guilabel']">
         <ComputerUI><xsl:apply-templates/></ComputerUI>
     </xsl:template>
     <xsl:template match="inline[@classes = 'menuselection']">
         <ComputerUI><xsl:apply-templates/></ComputerUI>
     </xsl:template>
     <xsl:template match="literal_block">
-        <ComputerDisplayBlock><xsl:apply-templates/></ComputerDisplayBlock>
+        <ProgramListing><xsl:apply-templates/></ProgramListing>
     </xsl:template>
     <xsl:template match="literal">
         <ComputerCode><xsl:apply-templates/></ComputerCode>
     </xsl:template>
 
     <!-- List templates -->
     <xsl:template match="bullet_list">
```

### Comparing `ou_book_theme-0.5.0/ou_book_theme/cli/mermaid-cli/package-lock.json` & `ou_book_theme-0.5.1/ou_book_theme/cli/mermaid-cli/package-lock.json`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/ou_book_theme/extensions/activity.py` & `ou_book_theme-0.5.1/ou_book_theme/extensions/activity.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/ou_book_theme/extensions/time.py` & `ou_book_theme-0.5.1/ou_book_theme/extensions/time.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/ou_book_theme/extensions/where_next.py` & `ou_book_theme-0.5.1/ou_book_theme/extensions/where_next.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg` & `ou_book_theme-0.5.1/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg` & `ou_book_theme-0.5.1/ou_book_theme/theme/ou_book_theme/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js` & `ou_book_theme-0.5.1/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css` & `ou_book_theme-0.5.1/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/pyproject.toml` & `ou_book_theme-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.5.0/PKG-INFO` & `ou_book_theme-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ou-book-theme
-Version: 0.5.0
+Version: 0.5.1
 Project-URL: Documentation, https://github.com/unknown/ou-book-theme#readme
 Project-URL: Issues, https://github.com/unknown/ou-book-theme/issues
 Project-URL: Source, https://github.com/unknown/ou-book-theme
 Author-email: Mark Hall <mark.hall@open.ac.uk>
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

