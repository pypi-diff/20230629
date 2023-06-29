# Comparing `tmp/pve_cli-0.2.5.tar.gz` & `tmp/pve_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pve_cli-0.2.5.tar", max compression
+gzip compressed data, was "pve_cli-0.3.0.tar", max compression
```

## Comparing `pve_cli-0.2.5.tar` & `pve_cli-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      594 2022-12-27 01:14:55.392146 pve_cli-0.2.5/README.md
--rw-r--r--   0        0        0      198 2022-12-26 18:04:35.108829 pve_cli-0.2.5/pve_cli/__init__.py
--rw-r--r--   0        0        0     3462 2023-01-10 19:46:49.826654 pve_cli-0.2.5/pve_cli/guest.py
--rw-r--r--   0        0        0     1820 2023-01-07 01:27:20.522672 pve_cli-0.2.5/pve_cli/main.py
--rw-r--r--   0        0        0      233 2022-12-27 00:26:34.747572 pve_cli-0.2.5/pve_cli/proxmox/__init__.py
--rw-r--r--   0        0        0     2692 2023-01-07 01:27:20.522672 pve_cli-0.2.5/pve_cli/proxmox/api.py
--rw-r--r--   0        0        0      392 2023-01-07 01:27:20.522672 pve_cli-0.2.5/pve_cli/proxmox/exceptions.py
--rw-r--r--   0        0        0       96 2022-12-26 18:04:35.108829 pve_cli-0.2.5/pve_cli/proxmox/types.py
--rw-r--r--   0        0        0        0 2022-12-26 18:04:35.108829 pve_cli-0.2.5/pve_cli/util/__init__.py
--rw-r--r--   0        0        0      763 2022-12-27 00:50:15.351766 pve_cli-0.2.5/pve_cli/util/callbacks.py
--rw-r--r--   0        0        0      129 2022-12-27 00:55:53.992688 pve_cli-0.2.5/pve_cli/util/exceptions.py
--rw-r--r--   0        0        0     1554 2022-12-27 01:16:56.300523 pve_cli-0.2.5/pve_cli/util/validators.py
--rw-r--r--   0        0        0     1548 2023-01-10 19:56:06.315598 pve_cli-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 pve_cli-0.2.5/setup.py
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 pve_cli-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      594 2023-06-29 18:50:03.816852 pve_cli-0.3.0/README.md
+-rw-r--r--   0        0        0      198 2023-06-29 18:50:03.816852 pve_cli-0.3.0/pve_cli/__init__.py
+-rw-r--r--   0        0        0     3744 2023-06-29 21:18:18.067834 pve_cli-0.3.0/pve_cli/guest_cmd.py
+-rw-r--r--   0        0        0     1861 2023-06-29 18:50:03.820852 pve_cli-0.3.0/pve_cli/main.py
+-rw-r--r--   0        0        0     5658 2023-06-29 21:18:18.067834 pve_cli-0.3.0/pve_cli/nodes_cmd.py
+-rw-r--r--   0        0        0      233 2023-06-29 18:50:03.820852 pve_cli-0.3.0/pve_cli/proxmox/__init__.py
+-rw-r--r--   0        0        0     3917 2023-06-29 21:18:18.067834 pve_cli-0.3.0/pve_cli/proxmox/api.py
+-rw-r--r--   0        0        0      449 2023-06-29 18:50:03.820852 pve_cli-0.3.0/pve_cli/proxmox/exceptions.py
+-rw-r--r--   0        0        0       96 2023-06-29 18:50:03.820852 pve_cli-0.3.0/pve_cli/proxmox/types.py
+-rw-r--r--   0        0        0        0 2023-06-29 21:21:29.404556 pve_cli-0.3.0/pve_cli/util/__init__.py
+-rw-r--r--   0        0        0      839 2023-06-29 18:50:03.824853 pve_cli-0.3.0/pve_cli/util/callbacks.py
+-rw-r--r--   0        0        0      129 2023-06-29 18:50:03.824853 pve_cli-0.3.0/pve_cli/util/exceptions.py
+-rw-r--r--   0        0        0     1570 2023-06-29 18:50:03.824853 pve_cli-0.3.0/pve_cli/util/validators.py
+-rw-r--r--   0        0        0     1593 2023-06-29 21:18:18.071834 pve_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 pve_cli-0.3.0/PKG-INFO
```

### Comparing `pve_cli-0.2.5/README.md` & `pve_cli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pve_cli-0.2.5/pve_cli/guest.py` & `pve_cli-0.3.0/pve_cli/guest_cmd.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from pathlib import Path
 
 import typer
 from rich import print as rprint
-from rich.markup import escape
 from rich.progress import Progress, SpinnerColumn, TextColumn
+from typing_extensions import Annotated
 
 from .proxmox import ProxmoxVMNotFoundError, ProxmoxMissingPermissionError
 from .util.exceptions import PVECLIError
 
 guest_cli = typer.Typer()
 
 
 @guest_cli.callback()
 def guest(
         ctx: typer.Context,
-        vm: str = typer.Argument(..., help='VM Name or ID')
+        vm: Annotated[str, typer.Argument(help='VM Name or ID')]
 ):
     proxmox_api = ctx.obj['proxmox_api']
 
     try:
         proxmox_api.check_permission('/vms', 'VM.Audit')
     except ProxmoxMissingPermissionError as exc:
         raise PVECLIError(f'Missing permission for VM-Management ({exc.path}): {exc.permission}')
@@ -32,66 +32,68 @@
         raise PVECLIError(f'VM {vm} was not found.')
 
     try:
         proxmox_api.check_permission(f'/vms/{vm_obj["vmid"]}', 'VM.Monitor')
     except ProxmoxMissingPermissionError as exc:
         raise PVECLIError(f'Missing permission for VM {vm_obj["name"]} ({exc.path}): {exc.permission}')
 
-    ctx.ensure_object(dict)
     ctx.obj['vm'] = vm_obj
 
 
 @guest_cli.command()
 def start(
         ctx: typer.Context,
-        command: list[str] = typer.Argument(...)
+        command: Annotated[list[str], typer.Argument()]
 ):
     """Start command on guest"""
     proxmox_api = ctx.obj['proxmox_api']
     vm = ctx.obj['vm']
     command_string = ' '.join(command)
 
+    rprint(f'[blue]Starting {command_string} on {vm["name"]} ({vm["vmid"]})')
     pid = proxmox_api.exec(node=vm['node'], vm_id=vm['vmid'], command=command_string)
-    rprint(pid)
+    rprint(f'[blue]PID: [green]{pid}')
 
 
 @guest_cli.command()
 def run(
         ctx: typer.Context,
-        command: list[str] = typer.Argument(...)
+        command: Annotated[list[str], typer.Argument()]
 ):
     """Execute command on guest and return output.
 
     Exits with the exitcode of the command inside the VM."""
     proxmox_api = ctx.obj['proxmox_api']
     vm = ctx.obj['vm']
     command_string = ' '.join(command)
 
+    rprint(f'[blue]Running {command_string} on {vm["name"]} ({vm["vmid"]})')
     pid = proxmox_api.exec(node=vm['node'], vm_id=vm['vmid'], command=command_string)
     result = proxmox_api.check_exec_status(node=vm['node'], vm_id=vm['vmid'], pid=pid)
     if result['out_data']:
-        rprint(escape(result['out_data']))
+        print(result['out_data'])
     raise typer.Exit(code=result['exitcode'])
 
 
 @guest_cli.command()
 def upload(
         ctx: typer.Context,
-        source: Path = typer.Argument(..., help='Path of the source file. Use "-" to read from stdin.',
-                                      exists=True, dir_okay=False, resolve_path=True, allow_dash=True),
-        destination: Path = typer.Argument(..., help='Path of the destination file inside the guest.',
-                                           exists=False, readable=False)
+        source: Annotated[Path, typer.Argument(help='Path of the source file. Use "-" to read from stdin.',
+                                               exists=True, dir_okay=False, resolve_path=True, allow_dash=True)],
+        destination: Annotated[Path, typer.Argument(help='Path of the destination file inside the guest.',
+                                                    exists=False, readable=False)]
 ):
     """Upload file to guest"""
     proxmox_api = ctx.obj['proxmox_api']
     vm = ctx.obj['vm']
 
     with typer.open_file(str(source), mode='rb') as source_stream:
         source_file = source_stream.read()
 
     with Progress(SpinnerColumn(style='bold white', finished_text='[blue bold]⠿'),
                   TextColumn('[progress.description]{task.description}')) as progress:
-        task_id = progress.add_task(description=f'[white]Uploading {source} to {destination} on {vm["name"]}...',
+        task_id = progress.add_task(description=f'[white]📤 Uploading {source} to {destination} '
+                                                f'on {vm["name"]} ({vm["vmid"]})...',
                                     total=1)
         proxmox_api.file_write(node=vm['node'], vm_id=vm['vmid'], file_path=destination, content=source_file)
         progress.update(task_id, completed=1, refresh=True,
-                        description=f'[blue]Done: Uploaded {source} to {destination} on {vm["name"]}')
+                        description=f'[blue]✅ Uploaded {source} to {destination} on {vm["name"]} ({vm["vmid"]})')
```

### Comparing `pve_cli-0.2.5/pve_cli/main.py` & `pve_cli-0.3.0/pve_cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from pathlib import Path
 from typing import Optional
 
 import typer
+from typing_extensions import Annotated
 
 from . import __version__, __metadata__
-from .guest import guest_cli
+from .guest_cmd import guest_cli
+from .nodes_cmd import nodes_cli
 from .proxmox import Proxmox
 from .proxmox.exceptions import ProxmoxConnectionError
 from .util.callbacks import config_callback, version_callback
-from .util.validators import validate_cluster
 from .util.exceptions import PVECLIError
+from .util.validators import validate_cluster
 
 HELP = f"""{__metadata__["Name"]} {__version__}
 
 {__metadata__["Summary"]}
 """
 
 cli = typer.Typer(help=HELP)
 cli.add_typer(guest_cli, name='guest', help='Guest-agent commands')
+cli.add_typer(nodes_cli, name='nodes', help='Node commands')
 
 
 @cli.callback(context_settings={'help_option_names': ['-h', '--help'], 'max_content_width': 120})
 def main(
         ctx: typer.Context,
-        _version: Optional[bool] = typer.Option(None, '--version', '-V',
-                                                callback=version_callback, is_eager=True, expose_value=False,
-                                                help='Print version and exit'),
-        _configfile: typer.FileText = typer.Option(Path(typer.get_app_dir('pve-cli')) / 'config.toml',
-                                                   '--config', '-c', encoding='utf-8',
-                                                   callback=config_callback, is_eager=True, expose_value=False,
-                                                   help='Config file path'),
-        cluster: str = typer.Option(None, '--cluster', '-C',
-                                    callback=validate_cluster,
-                                    help='Cluster from config to connect to.')
+        cluster: Annotated[str, typer.Option('--cluster', '-C', callback=validate_cluster,
+                                             help='Cluster from config to connect to.')] = '',
+        _version: Annotated[Optional[bool], typer.Option('--version', '-V', callback=version_callback, is_eager=True,
+                                                         expose_value=False, help='Print version and exit')] = None,
+        _configfile_path: Annotated[Path, typer.Option('--config', '-c', encoding='utf-8', callback=config_callback,
+                                                       is_eager=True, expose_value=False, help='Config file path')]
+        = Path(typer.get_app_dir('pve-cli')) / 'config.toml'
 ):
+    ctx.obj['cluster'] = cluster
     config = ctx.obj['config']
     cluster_config = config['clusters'][cluster]
 
     try:
         proxmox_api = Proxmox(**cluster_config)
     except ProxmoxConnectionError as exc:
         raise PVECLIError(str(exc))
```

### Comparing `pve_cli-0.2.5/pve_cli/util/callbacks.py` & `pve_cli-0.3.0/pve_cli/util/callbacks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+from pathlib import Path
+
 import toml  # with python3.11 this can be replaced by tomllib from stdlib
 import typer
 from rich import print as rprint
 
 from .validators import validate_config
 from .. import __version__
 
 
-def config_callback(ctx: typer.Context, configfile: typer.FileText):
+def config_callback(ctx: typer.Context, configfile_path: Path):
     if ctx.resilient_parsing:
         return
 
-    config = toml.loads(configfile.read())
+    with configfile_path.open('rt') as configfile:
+        config = toml.loads(configfile.read())
     validate_config(config)
 
     defaults = dict(config.pop('defaults', {}))
     ctx.default_map = ctx.default_map or {}  # preserve existing defaults
     ctx.default_map.update(defaults)
 
     ctx.ensure_object(dict)
```

### Comparing `pve_cli-0.2.5/pve_cli/util/validators.py` & `pve_cli-0.3.0/pve_cli/util/validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     cluster_config = config.get('clusters', {})
     default_cluster = config.get('defaults', {}).get('cluster', None)
     if default_cluster is not None and default_cluster not in cluster_config:
         raise InvalidConfigError(f'The configured default cluster "{default_cluster}" '
                                  f'has no configuration section in the config. (available: {", ".join(cluster_config)})')
 
     required_keys = [param.name for param in inspect.signature(Proxmox.__init__).parameters.values()
-                     if param.default == inspect.Parameter.empty and param.name != 'self']
+                     if param.default == inspect.Parameter.empty and param.name not in ['self', 'kwargs']]
 
     invalid_cluster_config = False
     err_msg = []
     for cluster_name, cluster_config in cluster_config.items():
         missing_keys = [key for key in required_keys if key not in cluster_config]
         if missing_keys:
             err_msg.append(f'  {cluster_name}: {", ".join(missing_keys)}')
```

### Comparing `pve_cli-0.2.5/pyproject.toml` & `pve_cli-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 name = "pve-cli"
-version = "0.2.5"
+version = "0.3.0"
 description = "CLI Tool to manage VMs and more on proxmox clusters"
 authors = ["Dominik Rimpf <dev@drimpf.de>"]
 readme = "README.md"
 packages = [{include = "pve_cli"}]
 
 [tool.poetry.scripts]
 pve-cli = "pve_cli.main:cli"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 proxmoxer = "^2.0.1"
-requests = "^2.28.1"
-typer = {extras = ["all"], version = "^0.7.0"}
+requests = "^2.31.0"
+typer = {extras = ["all"], version = "^0.9.0"}
 toml = "^0.10.2"
+requests-toolbelt = "^1.0.0"
+pip = "^23.1.2"
 
 [tool.poetry.group.lint.dependencies]
 bandit = {extras = ["toml"], version = "^1.7.4"}
 flake8 = "^6.0.0"
-flake8-annotations = "^2.9.1"
+flake8-annotations = "^3.0.0"
 flake8-pep585 = "^0.1.6"
 flake8-pyproject = "^1.2.2" # until flake8 gets its shit together...
 flake8-pytest = "^1.4"
 flake8-pytest-style = "^1.6.0"
 flake8-quotes = "^3.3.2"
 flake8-use-pathlib = "^0.3.0"
 mypy = "^0.991"
```

### Comparing `pve_cli-0.2.5/PKG-INFO` & `pve_cli-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pve-cli
-Version: 0.2.5
+Version: 0.3.0
 Summary: CLI Tool to manage VMs and more on proxmox clusters
 Author: Dominik Rimpf
 Author-email: dev@drimpf.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pip (>=23.1.2,<24.0.0)
 Requires-Dist: proxmoxer (>=2.0.1,<3.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # pve-cli
 
 CLI Tool to manage VMs and more on proxmox clusters
 
 ## Config
```

