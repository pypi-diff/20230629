# Comparing `tmp/asp_chef_cli-0.1.4.tar.gz` & `tmp/asp_chef_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asp_chef_cli-0.1.4.tar", max compression
+gzip compressed data, was "asp_chef_cli-0.1.5.tar", max compression
```

## Comparing `asp_chef_cli-0.1.4.tar` & `asp_chef_cli-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-06-09 19:16:09.263790 asp_chef_cli-0.1.4/LICENSE
--rw-r--r--   0        0        0     2991 2023-06-10 05:18:18.990369 asp_chef_cli-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-09 17:38:58.650957 asp_chef_cli-0.1.4/asp_chef_cli/__init__.py
--rw-r--r--   0        0        0      102 2023-06-09 20:54:07.739786 asp_chef_cli-0.1.4/asp_chef_cli/__main__.py
--rwxr-xr-x   0        0        0     4155 2023-06-09 21:07:32.879890 asp_chef_cli-0.1.4/asp_chef_cli/cli.py
--rw-r--r--   0        0        0      399 2023-06-10 05:18:45.986104 asp_chef_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.4/setup.py
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 19:16:09.263790 asp_chef_cli-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2991 2023-06-10 05:18:18.990369 asp_chef_cli-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 17:38:58.650957 asp_chef_cli-0.1.5/asp_chef_cli/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-09 20:54:07.739786 asp_chef_cli-0.1.5/asp_chef_cli/__main__.py
+-rwxr-xr-x   0        0        0     4379 2023-06-29 15:49:15.999199 asp_chef_cli-0.1.5/asp_chef_cli/cli.py
+-rw-r--r--   0        0        0      399 2023-06-29 15:35:04.704265 asp_chef_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.5/setup.py
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.5/PKG-INFO
```

### Comparing `asp_chef_cli-0.1.4/LICENSE` & `asp_chef_cli-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asp_chef_cli-0.1.4/README.md` & `asp_chef_cli-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `asp_chef_cli-0.1.4/asp_chef_cli/cli.py` & `asp_chef_cli-0.1.5/asp_chef_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import dataclasses
+import fileinput
 from enum import Enum
 
 import typer
 from dumbo_utils.console import console
 from dumbo_utils.url import compress_object_for_url
 from dumbo_utils.validation import validate
 from playwright.sync_api import sync_playwright, Playwright, Error
@@ -53,15 +54,15 @@
         else:
             console.print(f"[red bold]Error:[/red bold] {e}")
 
 
 def version_callback(value: bool):
     if value:
         import importlib.metadata
-        __version__ = importlib.metadata.version("dumbo-esse3")
+        __version__ = importlib.metadata.version("asp-chef-cli")
         console.print("asp-chef-headless", __version__)
         raise typer.Exit()
 
 
 def fetch(url: str):
     with sync_playwright() as playwright:
         browser = app_options.browser.get(playwright).launch(headless=app_options.headless and not app_options.debug)
@@ -117,23 +118,27 @@
         result = fetch(app_options.recipe_url)
 
     console.print(result)
 
 
 @app.command(name="run-with")
 def command_run_with(
-        the_input: str = typer.Option(..., "--input", "-i", prompt=True, help="A custom input for the recipe"),
+        the_input: str = typer.Option("--", "--input", "-i",
+                                      help="A custom input for the recipe (read from STDIN by default; "
+                                           "use CTRL+D to close the input)"),
 ) -> None:
     """
     Run a recipe with the input specified from STDIN or via the --input option.
     """
+    if the_input == "--":
+        the_input = ''.join(line for line in fileinput.input("-"))
+
     url = app_options.recipe_url
     if not app_options.headless:
         url = url.replace("/#", "/open#", 1)
     url = url.replace(r"#.*;", "#", 1)
     url = url.replace("#", "#" + compress_object_for_url({"input": the_input}, suffix="") + ";", 1)
 
     with console.status("Processing..."):
         result = fetch(url)
 
-    console.print()
     console.print(result)
```

### Comparing `asp_chef_cli-0.1.4/setup.py` & `asp_chef_cli-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['dumbo-utils>=0.1.9,<0.2.0',
  'pytest-playwright>=0.3.3,<0.4.0',
  'rich>=13.4.1,<14.0.0',
  'typer>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'asp-chef-cli',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'A simple CLI to run ASP Chef recipes',
     'long_description': '# ASP Chef CLI\n\nA simple CLI to run ASP Chef, in headed or headless mode.\n\n\n## Install\n\nThe suggested way is via pip:\n```bash\n$ pip install asp-chef-cli\n$ playwright install\n```\n\nDocker is another option (headed mode needs extra parameters):\n```bash\n$ docker run malvi/asp-chef-cli\n$ docker run docker run --net=host --env="DISPLAY" --volume="$HOME/.Xauthority:/root/.Xauthority:rw" malvi/asp-chef-cli\n```\n\n\n\n\n## Usage\n\nRun with one of the following commands:\n```bash\n$ python -m asp_chef_cli --help\n$ docker run malvi/asp-chef-cli --help\n```\n\nAdd the recipe (an ASP Chef sharable URL) with the option `--url` (quote the URL as it contains characters like # that breaks bash and other terminals).\nThe headless mode can be activated with the flag `--headless` (always active in the docker image).\nPossibly change the default browser used by playwright with the option `--browser`.\nFinally, give a command to execute:\n* `run` simply runs the recipe as it is;\n* `run-with` runs the recipe with the input replaced by the one specified either with the option `--input` or via the prompt.\n\nThe flag `--help` can be specified after a command to get a list of arguments for that command.\n\n\n## Examples\n\nLet us consider [this simple recipe](https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21) with no input and guessing the atom `world`.\nThe recipe can be run headless by giving the following command:\n```bash\n$ python -m asp_chef_cli --headless --browser=chromium --url="https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21" run\nEMPTY MODEL\n§\nworld.\n```\n\nIt is possible to specify a different input as follows:\n```bash\n$ python -m asp_chef_headless --headless --browser=chromium --url="https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21" run-with --input "hello."\nhello.\n§\nhello.\nworld.\n```',
     'author': 'Mario Alviano',
     'author_email': 'mario.alviano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `asp_chef_cli-0.1.4/PKG-INFO` & `asp_chef_cli-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asp-chef-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple CLI to run ASP Chef recipes
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

