# Comparing `tmp/notion2md-2.8.2.tar.gz` & `tmp/notion2md-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion2md-2.8.2.tar", max compression
+gzip compressed data, was "notion2md-2.8.3.tar", max compression
```

## Comparing `notion2md-2.8.2.tar` & `notion2md-2.8.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1064 2023-02-26 11:09:22.192757 notion2md-2.8.2/LICENSE
--rw-r--r--   0        0        0     2831 2023-02-26 11:09:22.192757 notion2md-2.8.2/README.md
--rw-r--r--   0        0        0       22 2023-02-26 11:10:01.417037 notion2md-2.8.2/notion2md/__init__.py
--rw-r--r--   0        0        0      144 2023-02-26 11:09:22.192757 notion2md-2.8.2/notion2md/__main__.py
--rw-r--r--   0        0        0     1429 2023-02-26 11:09:22.192757 notion2md-2.8.2/notion2md/config.py
--rw-r--r--   0        0        0        0 2023-02-26 11:09:22.192757 notion2md-2.8.2/notion2md/console/__init__.py
--rw-r--r--   0        0        0     2762 2023-02-26 11:09:22.192757 notion2md-2.8.2/notion2md/console/application.py
--rw-r--r--   0        0        0     4072 2023-02-26 11:09:22.192757 notion2md-2.8.2/notion2md/console/commands/export_block.py
--rw-r--r--   0        0        0      235 2023-02-26 11:09:22.192757 notion2md-2.8.2/notion2md/console/formatter.py
--rw-r--r--   0        0        0        0 2023-02-26 11:09:22.192757 notion2md-2.8.2/notion2md/console/ui/__init__.py
--rw-r--r--   0        0        0      690 2023-02-26 11:09:22.192757 notion2md-2.8.2/notion2md/console/ui/indicator.py
--rw-r--r--   0        0        0        0 2023-02-26 11:09:22.192757 notion2md-2.8.2/notion2md/convertor/__init__.py
--rw-r--r--   0        0        0    10003 2023-02-26 11:09:22.196757 notion2md-2.8.2/notion2md/convertor/block.py
--rw-r--r--   0        0        0     2774 2023-02-26 11:09:22.196757 notion2md-2.8.2/notion2md/convertor/richtext.py
--rw-r--r--   0        0        0      726 2023-02-26 11:09:22.196757 notion2md-2.8.2/notion2md/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-26 11:09:22.196757 notion2md-2.8.2/notion2md/exporter/__init__.py
--rw-r--r--   0        0        0     2687 2023-02-26 11:09:22.196757 notion2md-2.8.2/notion2md/exporter/block.py
--rw-r--r--   0        0        0     1202 2023-02-26 11:09:22.196757 notion2md-2.8.2/notion2md/notion_api.py
--rw-r--r--   0        0        0      414 2023-02-26 11:09:22.196757 notion2md-2.8.2/notion2md/util.py
--rw-r--r--   0        0        0     1288 2023-02-26 11:10:01.345036 notion2md-2.8.2/pyproject.toml
--rw-r--r--   0        0        0     3851 1970-01-01 00:00:00.000000 notion2md-2.8.2/setup.py
--rw-r--r--   0        0        0     3638 1970-01-01 00:00:00.000000 notion2md-2.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-29 07:45:10.694565 notion2md-2.8.3/LICENSE
+-rw-r--r--   0        0        0     2833 2023-06-29 07:45:10.694565 notion2md-2.8.3/README.md
+-rw-r--r--   0        0        0       22 2023-06-29 07:45:46.642877 notion2md-2.8.3/notion2md/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/__main__.py
+-rw-r--r--   0        0        0     1429 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/config.py
+-rw-r--r--   0        0        0        0 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/console/__init__.py
+-rw-r--r--   0        0        0     2762 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/console/application.py
+-rw-r--r--   0        0        0     4072 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/console/commands/export_block.py
+-rw-r--r--   0        0        0      235 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/console/formatter.py
+-rw-r--r--   0        0        0        0 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/console/ui/__init__.py
+-rw-r--r--   0        0        0      690 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/console/ui/indicator.py
+-rw-r--r--   0        0        0        0 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/convertor/__init__.py
+-rw-r--r--   0        0        0    10003 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/convertor/block.py
+-rw-r--r--   0        0        0     2774 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/convertor/richtext.py
+-rw-r--r--   0        0        0      726 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/exporter/__init__.py
+-rw-r--r--   0        0        0     2687 2023-06-29 07:45:10.694565 notion2md-2.8.3/notion2md/exporter/block.py
+-rw-r--r--   0        0        0     1202 2023-06-29 07:45:10.698565 notion2md-2.8.3/notion2md/notion_api.py
+-rw-r--r--   0        0        0      414 2023-06-29 07:45:10.698565 notion2md-2.8.3/notion2md/util.py
+-rw-r--r--   0        0        0     1288 2023-06-29 07:45:46.562876 notion2md-2.8.3/pyproject.toml
+-rw-r--r--   0        0        0     3590 1970-01-01 00:00:00.000000 notion2md-2.8.3/PKG-INFO
```

### Comparing `notion2md-2.8.2/LICENSE` & `notion2md-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `notion2md-2.8.2/README.md` & `notion2md-2.8.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -49,18 +49,18 @@
 
 ## Usage: Python
 
 ```Python
 from notion2md.exporter.block import MarkdownExporter, StringExporter
 
 # MarkdownExporter will make markdown file on your output path
-MarkdownExporter(page_id='...',output_path='...',download=True).export()
+MarkdownExporter(block_id='...',output_path='...',download=True).export()
 
 # StringExporter will return output as String type
-md = StringExporter(page_id='...',output_path='...').export()
+md = StringExporter(block_id='...',output_path='...').export()
 ```
 
 ## To-do
 
 - [x] Download file object(image and files)
 - [x] Table blocks
 - [x] Synced Block
```

#### html2text {}

```diff
@@ -20,15 +20,15 @@
 **download** option will download files/images in the `path` directory. -
 **unzipped** option makes Notion2Md export ***unzipped*** output of Notion
 block. ```Bash notion2md --download -n post -p ~/MyBlog/content/posts -u https:
 //notion.so/... ``` - This command will generate "**post.zip**" in your '**~/
 MyBlog/content/posts**' directory. ## Usage: Python ```Python from
 notion2md.exporter.block import MarkdownExporter, StringExporter #
 MarkdownExporter will make markdown file on your output path MarkdownExporter
-(page_id='...',output_path='...',download=True).export() # StringExporter will
+(block_id='...',output_path='...',download=True).export() # StringExporter will
 return output as String type md = StringExporter
-(page_id='...',output_path='...').export() ``` ## To-do - [x] Download file
+(block_id='...',output_path='...').export() ``` ## To-do - [x] Download file
 object(image and files) - [x] Table blocks - [x] Synced Block - [ ] Page
 Exporter - [ ] Child page - [ ] Column List and Column Blocks ## Contribution
 Please read [Contribution Guide](CONTRIBUTION.md) ## Donation If you think
 **Notion2Md** is helpful to you, you can support me here: [Buy_Me_A_Coffee] ##
 License [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `notion2md-2.8.2/notion2md/config.py` & `notion2md-2.8.3/notion2md/config.py`

 * *Files identical despite different names*

### Comparing `notion2md-2.8.2/notion2md/console/application.py` & `notion2md-2.8.3/notion2md/console/application.py`

 * *Files identical despite different names*

### Comparing `notion2md-2.8.2/notion2md/console/commands/export_block.py` & `notion2md-2.8.3/notion2md/console/commands/export_block.py`

 * *Files identical despite different names*

### Comparing `notion2md-2.8.2/notion2md/console/ui/indicator.py` & `notion2md-2.8.3/notion2md/console/ui/indicator.py`

 * *Files identical despite different names*

### Comparing `notion2md-2.8.2/notion2md/convertor/block.py` & `notion2md-2.8.3/notion2md/convertor/block.py`

 * *Files identical despite different names*

### Comparing `notion2md-2.8.2/notion2md/convertor/richtext.py` & `notion2md-2.8.3/notion2md/convertor/richtext.py`

 * *Files identical despite different names*

### Comparing `notion2md-2.8.2/notion2md/exceptions.py` & `notion2md-2.8.3/notion2md/exceptions.py`

 * *Files identical despite different names*

### Comparing `notion2md-2.8.2/notion2md/exporter/block.py` & `notion2md-2.8.3/notion2md/exporter/block.py`

 * *Files identical despite different names*

### Comparing `notion2md-2.8.2/notion2md/notion_api.py` & `notion2md-2.8.3/notion2md/notion_api.py`

 * *Files identical despite different names*

### Comparing `notion2md-2.8.2/pyproject.toml` & `notion2md-2.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "notion2md"
-version = "2.8.2"
+version = "2.8.3"
 description = "Notion Markdown Exporter with Python Cli"
 license = "MIT"
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: OS Independent", "Programming Language :: Python :: 3.9"]
 homepage = "https://github.com/echo724/notion2md.git"
 authors = ["echo724 <eunchan1001@gmail.com>"]
 readme = "README.md"
 exclude = ["Test/test_*"]
```

### Comparing `notion2md-2.8.2/setup.py` & `notion2md-2.8.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,104 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: notion2md
+Version: 2.8.3
+Summary: Notion Markdown Exporter with Python Cli
+Home-page: https://github.com/echo724/notion2md.git
+License: MIT
+Author: echo724
+Author-email: eunchan1001@gmail.com
+Requires-Python: >=3.7,<4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cleo (>=1.0.0a4)
+Requires-Dist: notion-client (>=1.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['notion2md',
- 'notion2md.console',
- 'notion2md.console.commands',
- 'notion2md.console.ui',
- 'notion2md.convertor',
- 'notion2md.exporter']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cleo>=1.0.0a4', 'notion-client>=1.0.0']
-
-entry_points = \
-{'console_scripts': ['notion2md = notion2md.console.application:main']}
-
-setup_kwargs = {
-    'name': 'notion2md',
-    'version': '2.8.2',
-    'description': 'Notion Markdown Exporter with Python Cli',
-    'long_description': '![Notion2Md logo - an arrow pointing from "N" to "MD"](Notion2md.jpg)\n\n<br/>\n\n## About Notion2Md\n\n[![Downloads](https://pepy.tech/badge/notion2md)](https://pepy.tech/project/notion2md)\n[![PyPI version](https://badge.fury.io/py/notion2md.svg)](https://badge.fury.io/py/notion2md)\n[![Code Quality](https://github.com/echo724/notion2md/actions/workflows/code_quality.yaml/badge.svg)](https://github.com/echo724/notion2md/actions/workflows/code_quality.yaml)\n<a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fecho724%2Fnotion2md&count_bg=%23949191&title_bg=%23555555&icon=github.svg&icon_color=%23E7E7E7&title=visited&edge_flat=false"/></a>\n\n- Notion Markdown Exporter using **official notion api** by [notion-sdk-py](https://github.com/ramnes/notion-sdk-py)\n\n### Notion2Medium\n\n- Check out [Notion2Medium](https://github.com/echo724/notion2medium) that publishes a **Medium** post from **Notion** using Notion2Md.\n\n## API Key(Token)\n\n- Before getting started, create [an integration and find the token](https://www.notion.so/my-integrations). → [Learn more about authorization](https://developers.notion.com/docs/authorization).\n\n- Then save your api key(token) as your os environment variable\n\n```Bash\n$ export NOTION_TOKEN="{your integration token key}"\n```\n\n## Install\n\n```Bash\n$ pip install notion2md\n```\n\n## Usage: Shell Command\n\n![Terminal output of the `notion2md -h` command](notion2md_options.png)\n\n- Notion2md requires either `id` or `url` of the Notion page/block.\n\n- **download** option will download files/images in the `path` directory.\n\n- **unzipped** option makes Notion2Md export ***unzipped*** output of Notion block.\n\n```Bash\nnotion2md --download -n post -p ~/MyBlog/content/posts -u https://notion.so/...\n```\n\n- This command will generate "**post.zip**" in your \'**~/MyBlog/content/posts**\' directory.\n\n## Usage: Python\n\n```Python\nfrom notion2md.exporter.block import MarkdownExporter, StringExporter\n\n# MarkdownExporter will make markdown file on your output path\nMarkdownExporter(page_id=\'...\',output_path=\'...\',download=True).export()\n\n# StringExporter will return output as String type\nmd = StringExporter(page_id=\'...\',output_path=\'...\').export()\n```\n\n## To-do\n\n- [x] Download file object(image and files)\n- [x] Table blocks\n- [x] Synced Block\n- [ ] Page Exporter\n- [ ] Child page\n- [ ] Column List and Column Blocks\n\n## Contribution\n\nPlease read [Contribution Guide](CONTRIBUTION.md)\n\n## Donation\n\nIf you think **Notion2Md** is helpful to you, you can support me here:\n\n<a href="https://www.buymeacoffee.com/echo724" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 54px;" height="54"></a>\n\n## License\n[MIT](https://choosealicense.com/licenses/mit/)\n',
-    'author': 'echo724',
-    'author_email': 'eunchan1001@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/echo724/notion2md.git',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4',
-}
+![Notion2Md logo - an arrow pointing from "N" to "MD"](Notion2md.jpg)
 
+<br/>
+
+## About Notion2Md
+
+[![Downloads](https://pepy.tech/badge/notion2md)](https://pepy.tech/project/notion2md)
+[![PyPI version](https://badge.fury.io/py/notion2md.svg)](https://badge.fury.io/py/notion2md)
+[![Code Quality](https://github.com/echo724/notion2md/actions/workflows/code_quality.yaml/badge.svg)](https://github.com/echo724/notion2md/actions/workflows/code_quality.yaml)
+<a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fecho724%2Fnotion2md&count_bg=%23949191&title_bg=%23555555&icon=github.svg&icon_color=%23E7E7E7&title=visited&edge_flat=false"/></a>
+
+- Notion Markdown Exporter using **official notion api** by [notion-sdk-py](https://github.com/ramnes/notion-sdk-py)
+
+### Notion2Medium
+
+- Check out [Notion2Medium](https://github.com/echo724/notion2medium) that publishes a **Medium** post from **Notion** using Notion2Md.
+
+## API Key(Token)
+
+- Before getting started, create [an integration and find the token](https://www.notion.so/my-integrations). → [Learn more about authorization](https://developers.notion.com/docs/authorization).
+
+- Then save your api key(token) as your os environment variable
+
+```Bash
+$ export NOTION_TOKEN="{your integration token key}"
+```
+
+## Install
+
+```Bash
+$ pip install notion2md
+```
+
+## Usage: Shell Command
+
+![Terminal output of the `notion2md -h` command](notion2md_options.png)
+
+- Notion2md requires either `id` or `url` of the Notion page/block.
+
+- **download** option will download files/images in the `path` directory.
+
+- **unzipped** option makes Notion2Md export ***unzipped*** output of Notion block.
+
+```Bash
+notion2md --download -n post -p ~/MyBlog/content/posts -u https://notion.so/...
+```
+
+- This command will generate "**post.zip**" in your '**~/MyBlog/content/posts**' directory.
+
+## Usage: Python
+
+```Python
+from notion2md.exporter.block import MarkdownExporter, StringExporter
+
+# MarkdownExporter will make markdown file on your output path
+MarkdownExporter(block_id='...',output_path='...',download=True).export()
+
+# StringExporter will return output as String type
+md = StringExporter(block_id='...',output_path='...').export()
+```
+
+## To-do
+
+- [x] Download file object(image and files)
+- [x] Table blocks
+- [x] Synced Block
+- [ ] Page Exporter
+- [ ] Child page
+- [ ] Column List and Column Blocks
+
+## Contribution
+
+Please read [Contribution Guide](CONTRIBUTION.md)
+
+## Donation
+
+If you think **Notion2Md** is helpful to you, you can support me here:
+
+<a href="https://www.buymeacoffee.com/echo724" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 54px;" height="54"></a>
+
+## License
+[MIT](https://choosealicense.com/licenses/mit/)
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,48 +1,44 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['notion2md',
-'notion2md.console', 'notion2md.console.commands', 'notion2md.console.ui',
-'notion2md.convertor', 'notion2md.exporter'] package_data = \ {'': ['*']}
-install_requires = \ ['cleo>=1.0.0a4', 'notion-client>=1.0.0'] entry_points = \
-{'console_scripts': ['notion2md = notion2md.console.application:main']}
-setup_kwargs = { 'name': 'notion2md', 'version': '2.8.2', 'description':
-'Notion Markdown Exporter with Python Cli', 'long_description': '![Notion2Md
-logo - an arrow pointing from "N" to "MD"](Notion2md.jpg)\n\n
-\n\n## About Notion2Md\n\n[![Downloads](https://pepy.tech/badge/notion2md)]
-(https://pepy.tech/project/notion2md)\n[![PyPI version](https://badge.fury.io/
-py/notion2md.svg)](https://badge.fury.io/py/notion2md)\n[![Code Quality](https:
-//github.com/echo724/notion2md/actions/workflows/code_quality.yaml/badge.svg)]
-(https://github.com/echo724/notion2md/actions/workflows/code_quality.yaml)\n
+Metadata-Version: 2.1 Name: notion2md Version: 2.8.3 Summary: Notion Markdown
+Exporter with Python Cli Home-page: https://github.com/echo724/notion2md.git
+License: MIT Author: echo724 Author-email: eunchan1001@gmail.com Requires-
+Python: >=3.7,<4 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: cleo (>=1.0.0a4) Requires-Dist:
+notion-client (>=1.0.0) Description-Content-Type: text/markdown ![Notion2Md
+logo - an arrow pointing from "N" to "MD"](Notion2md.jpg)
+## About Notion2Md [![Downloads](https://pepy.tech/badge/notion2md)](https://
+pepy.tech/project/notion2md) [![PyPI version](https://badge.fury.io/py/
+notion2md.svg)](https://badge.fury.io/py/notion2md) [![Code Quality](https://
+github.com/echo724/notion2md/actions/workflows/code_quality.yaml/badge.svg)]
+(https://github.com/echo724/notion2md/actions/workflows/code_quality.yaml)
 [https://hits.seeyoufarm.com/api/count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2Fecho724%2Fnotion2md&count_bg=%23949191&title_bg=%23555555&icon=github.svg&icon_color=%23E7E7E7&title=visited&edge_flat=false]\n\n-
-Notion Markdown Exporter using **official notion api** by [notion-sdk-py]
-(https://github.com/ramnes/notion-sdk-py)\n\n### Notion2Medium\n\n- Check out
+badge.svg?url=https%3A%2F%2Fgithub.com%2Fecho724%2Fnotion2md&count_bg=%23949191&title_bg=%23555555&icon=github.svg&icon_color=%23E7E7E7&title=visited&edge_flat=false]
+- Notion Markdown Exporter using **official notion api** by [notion-sdk-py]
+(https://github.com/ramnes/notion-sdk-py) ### Notion2Medium - Check out
 [Notion2Medium](https://github.com/echo724/notion2medium) that publishes a
-**Medium** post from **Notion** using Notion2Md.\n\n## API Key(Token)\n\n-
-Before getting started, create [an integration and find the token](https://
+**Medium** post from **Notion** using Notion2Md. ## API Key(Token) - Before
+getting started, create [an integration and find the token](https://
 www.notion.so/my-integrations). â [Learn more about authorization](https://
-developers.notion.com/docs/authorization).\n\n- Then save your api key(token)
-as your os environment variable\n\n```Bash\n$ export NOTION_TOKEN="{your
-integration token key}"\n```\n\n## Install\n\n```Bash\n$ pip install
-notion2md\n```\n\n## Usage: Shell Command\n\n![Terminal output of the
-`notion2md -h` command](notion2md_options.png)\n\n- Notion2md requires either
-`id` or `url` of the Notion page/block.\n\n- **download** option will download
-files/images in the `path` directory.\n\n- **unzipped** option makes Notion2Md
-export ***unzipped*** output of Notion block.\n\n```Bash\nnotion2md --download
--n post -p ~/MyBlog/content/posts -u https://notion.so/...\n```\n\n- This
-command will generate "**post.zip**" in your \'**~/MyBlog/content/posts**\'
-directory.\n\n## Usage: Python\n\n```Python\nfrom notion2md.exporter.block
-import MarkdownExporter, StringExporter\n\n# MarkdownExporter will make
-markdown file on your output path\nMarkdownExporter
-(page_id=\'...\',output_path=\'...\',download=True).export()\n\n#
-StringExporter will return output as String type\nmd = StringExporter
-(page_id=\'...\',output_path=\'...\').export()\n```\n\n## To-do\n\n- [x]
-Download file object(image and files)\n- [x] Table blocks\n- [x] Synced
-Block\n- [ ] Page Exporter\n- [ ] Child page\n- [ ] Column List and Column
-Blocks\n\n## Contribution\n\nPlease read [Contribution Guide]
-(CONTRIBUTION.md)\n\n## Donation\n\nIf you think **Notion2Md** is helpful to
-you, you can support me here:\n\n[Buy_Me_A_Coffee]\n\n## License\n[MIT](https:/
-/choosealicense.com/licenses/mit/)\n', 'author': 'echo724', 'author_email':
-'eunchan1001@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'https://github.com/echo724/notion2md.git', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.7,<4', } setup
-(**setup_kwargs)
+developers.notion.com/docs/authorization). - Then save your api key(token) as
+your os environment variable ```Bash $ export NOTION_TOKEN="{your integration
+token key}" ``` ## Install ```Bash $ pip install notion2md ``` ## Usage: Shell
+Command ![Terminal output of the `notion2md -h` command](notion2md_options.png)
+- Notion2md requires either `id` or `url` of the Notion page/block. -
+**download** option will download files/images in the `path` directory. -
+**unzipped** option makes Notion2Md export ***unzipped*** output of Notion
+block. ```Bash notion2md --download -n post -p ~/MyBlog/content/posts -u https:
+//notion.so/... ``` - This command will generate "**post.zip**" in your '**~/
+MyBlog/content/posts**' directory. ## Usage: Python ```Python from
+notion2md.exporter.block import MarkdownExporter, StringExporter #
+MarkdownExporter will make markdown file on your output path MarkdownExporter
+(block_id='...',output_path='...',download=True).export() # StringExporter will
+return output as String type md = StringExporter
+(block_id='...',output_path='...').export() ``` ## To-do - [x] Download file
+object(image and files) - [x] Table blocks - [x] Synced Block - [ ] Page
+Exporter - [ ] Child page - [ ] Column List and Column Blocks ## Contribution
+Please read [Contribution Guide](CONTRIBUTION.md) ## Donation If you think
+**Notion2Md** is helpful to you, you can support me here: [Buy_Me_A_Coffee] ##
+License [MIT](https://choosealicense.com/licenses/mit/)
```

