# Comparing `tmp/memfault-cli-0.9.0.tar.gz` & `tmp/memfault_cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memfault-cli-0.9.0.tar", max compression
+gzip compressed data, was "memfault_cli-1.0.0.tar", max compression
```

## Comparing `memfault-cli-0.9.0.tar` & `memfault_cli-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      267 2022-07-01 18:48:24.158978 memfault-cli-0.9.0/README.md
--rw-r--r--   0        0        0       79 2022-07-01 18:48:24.158978 memfault-cli-0.9.0/memfault_cli/__init__.py
--rw-r--r--   0        0        0      465 2022-09-07 08:56:09.631200 memfault-cli-0.9.0/memfault_cli/_version.py
--rw-r--r--   0        0        0     2579 2022-09-26 12:35:31.188376 memfault-cli-0.9.0/memfault_cli/authenticator.py
--rw-r--r--   0        0        0     2773 2022-07-01 18:48:24.158978 memfault-cli-0.9.0/memfault_cli/chunk.py
--rw-r--r--   0        0        0    20132 2022-09-26 12:35:31.188376 memfault-cli-0.9.0/memfault_cli/cli.py
--rw-r--r--   0        0        0    11216 2022-09-26 12:35:31.188376 memfault-cli-0.9.0/memfault_cli/context.py
--rw-r--r--   0        0        0     2522 2022-09-07 08:56:09.631200 memfault-cli-0.9.0/memfault_cli/deploy.py
--rw-r--r--   0        0        0     2281 2022-09-26 10:55:42.178569 memfault-cli-0.9.0/memfault_cli/elf.py
--rw-r--r--   0        0        0      633 2022-07-01 18:48:24.158978 memfault-cli-0.9.0/memfault_cli/functools_ext.py
--rw-r--r--   0        0        0    22740 2022-09-26 12:35:31.188376 memfault-cli-0.9.0/memfault_cli/upload.py
--rw-r--r--   0        0        0     5712 2022-09-26 10:55:42.178569 memfault-cli-0.9.0/memfault_cli/yocto.py
--rw-r--r--   0        0        0     1677 2022-09-26 10:55:42.178569 memfault-cli-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 memfault-cli-0.9.0/setup.py
--rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 memfault-cli-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2877 2023-06-29 17:19:54.211920 memfault_cli-1.0.0/README.md
+-rw-r--r--   0        0        0       79 2022-12-06 20:53:34.385268 memfault_cli-1.0.0/memfault_cli/__init__.py
+-rw-r--r--   0        0        0      529 2023-04-27 16:08:38.128691 memfault_cli-1.0.0/memfault_cli/_version.py
+-rw-r--r--   0        0        0     2579 2023-04-28 20:34:41.371280 memfault_cli-1.0.0/memfault_cli/authenticator.py
+-rw-r--r--   0        0        0     3889 2023-04-27 16:08:38.128691 memfault_cli-1.0.0/memfault_cli/chunk.py
+-rw-r--r--   0        0        0    27792 2023-06-29 12:58:48.735971 memfault_cli-1.0.0/memfault_cli/cli.py
+-rw-r--r--   0        0        0     9759 2023-05-17 18:14:40.715182 memfault_cli-1.0.0/memfault_cli/console.py
+-rw-r--r--   0        0        0    13111 2023-06-14 15:14:13.549689 memfault_cli-1.0.0/memfault_cli/context.py
+-rw-r--r--   0        0        0     4762 2023-06-29 12:58:48.735971 memfault_cli-1.0.0/memfault_cli/deploy.py
+-rw-r--r--   0        0        0     4115 2023-04-27 16:08:38.132691 memfault_cli-1.0.0/memfault_cli/elf.py
+-rw-r--r--   0        0        0      633 2022-12-06 20:53:34.385268 memfault_cli-1.0.0/memfault_cli/functools_ext.py
+-rw-r--r--   0        0        0    25379 2023-06-29 17:19:54.211920 memfault_cli-1.0.0/memfault_cli/upload.py
+-rw-r--r--   0        0        0     7780 2023-04-28 20:34:41.371280 memfault_cli-1.0.0/memfault_cli/yocto.py
+-rw-r--r--   0        0        0     3528 2023-06-29 17:19:54.211920 memfault_cli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 memfault_cli-1.0.0/PKG-INFO
```

### Comparing `memfault-cli-0.9.0/memfault_cli/authenticator.py` & `memfault_cli-1.0.0/memfault_cli/authenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from abc import abstractmethod
 from typing import TYPE_CHECKING, List
 
 if TYPE_CHECKING:
     from .context import MemfaultCliClickContext
 
 
-LOG = logging.getLogger(__name__)
+log = logging.getLogger(__name__)
 
 
 class Authenticator:
     def __init__(self, ctx: "MemfaultCliClickContext"):
         self.ctx = ctx
 
     @staticmethod
@@ -56,15 +56,15 @@
     - Email + User API Key
     - DEPRECATED: Organization Auth Token (passed in as password) -- --org-token should be used instead
     """
 
     def __init__(self, ctx: "MemfaultCliClickContext") -> None:
         super().__init__(ctx)
         if not self.ctx.obj.get("email") and self.ctx.password.startswith("oat_"):
-            LOG.warning(
+            log.warning(
                 "Please use --org-token instead of --password to pass organization auth token"
             )
 
     @staticmethod
     def project_key_auth() -> bool:
         return False
```

### Comparing `memfault-cli-0.9.0/memfault_cli/chunk.py` & `memfault_cli-1.0.0/memfault_cli/chunk.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+import math
+import os
 import re
 from base64 import b64decode
 from typing import List
 
 import requests
+import tqdm
+from more_itertools import chunked
 from requests import PreparedRequest
 
 from .authenticator import Authenticator
 from .context import MemfaultCliClickContext
 
 EXPORTED_CHUNKS_REGEX = re.compile(r"MC:([a-zA-z0-9+/=]+):")
 
@@ -22,18 +26,45 @@
 
     def post(self, chunk: bytes):
         request_args = self.authenticator.requests_auth_params()
         request_args["headers"]["Content-Type"] = "application/octet-stream"
         response = requests.post(self.url, data=chunk, **request_args)
         if response.status_code >= 400:
             raise Exception(
-                f"Request failed with HTTP status {response.status_code}\nResponse body:\n{response.content.decode()}"
+                f"Request failed with HTTP status {response.status_code}\nResponse"
+                f" body:\n{response.content.decode()}"
+            )
+
+    def do_batch_post(self, files: List):
+        """Issue a post with a batch of files (HTTP Multipart)"""
+        request_args = self.authenticator.requests_auth_params()
+
+        # Pick up defaults (i.e User-Agent) and merge with Memfault Auth headers
+        headers = requests.utils.default_headers()
+        headers.update(request_args["headers"])
+        del request_args["headers"]
+
+        request = PreparedRequest()
+        request.prepare(method="POST", url=self.url, files=files, headers=headers, **request_args)
+        content_type: str = request.headers["content-type"]
+        request.headers["content-type"] = content_type.replace("form-data", "mixed")
+
+        session = requests.Session()
+        response = session.send(request)
+        if response.status_code >= 400:
+            raise Exception(
+                f"Request failed with HTTP status {response.status_code}\nResponse"
+                f" body:\n{response.content.decode()}"
             )
 
     def batch_post(self, chunks: List[bytes]):
+        """
+        Post a batch of chunks to the Memfault Chunk API. Will break the request
+        into multiple Multipart requests if the chunk count is too large
+        """
         if len(chunks) == 1:
             self.post(chunks[0])
             return
 
         files = []
         for idx, chunk in enumerate(chunks):
             files.append(
@@ -46,32 +77,30 @@
                         chunk,
                         "application/octet-stream",
                         {"Content-Length": len(chunk)},
                     ),
                 )
             )
 
-        request_args = self.authenticator.requests_auth_params()
-
-        # Pick up defaults (i.e User-Agent) and merge with Memfault Auth headers
-        headers = requests.utils.default_headers()
-        headers.update(request_args["headers"])
-        del request_args["headers"]
-
-        request = PreparedRequest()
-        request.prepare(method="POST", url=self.url, files=files, headers=headers, **request_args)
-        content_type: str = request.headers["content-type"]
-        request.headers["content-type"] = content_type.replace("form-data", "mixed")
-
-        session = requests.Session()
-        response = session.send(request)
-        if response.status_code >= 400:
-            raise Exception(
-                f"Request failed with HTTP status {response.status_code}\nResponse body:\n{response.content.decode()}"
-            )
+        # by default, limit each request to 500 chunks. this is an extreme edge
+        # case but it can happen.
+        batch_size = int(os.environ.get("MEMFAULT_CLI_CHUNK_BATCH_SIZE", "500"))
+
+        if len(files) <= batch_size:
+            # do a single post if the chunk count is small enough
+            self.do_batch_post(files)
+        else:
+            # otherwise, break the request into multiple posts
+            for chunk_group in tqdm.tqdm(
+                chunked(files, batch_size),
+                total=math.ceil(len(files) / batch_size),
+                unit="batch",
+                desc=f"Uploading chunks in batches of {batch_size}",
+            ):
+                self.do_batch_post(chunk_group)
 
     @staticmethod
     def extract_exported_chunks(data: str):
         chunks = []
         for match in EXPORTED_CHUNKS_REGEX.finditer(data):
             binary_encoded_chunk = b64decode(match.group(1))
             chunks.append(binary_encoded_chunk)
```

### Comparing `memfault-cli-0.9.0/memfault_cli/cli.py` & `memfault_cli-1.0.0/memfault_cli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 import http.client
 import logging
 import os
+import pathlib
 from base64 import b64decode
-from typing import List, TextIO, Type
+from datetime import datetime, timezone
+from typing import List, Optional, Type
 
 import click
 
 from ._version import version
 from .authenticator import BasicAuthenticator, OrgTokenAuthenticator, ProjectKeyAuthenticator
 from .chunk import MemfaultChunk
+from .console import MemfaultMiniterm
 from .context import MemfaultCliClickContext
 from .deploy import Deployer
 from .upload import (
     AndroidAppSymbolsUploader,
     BugreportUploader,
     CoredumpUploader,
+    CustomDataRecordingUploader,
     ElfSymbolDirectoryUploader,
     ElfSymbolUploader,
     MarUploader,
     McuSdkElfSymbolUploader,
     ReleaseArtifactUploader,
     Uploader,
     XedUploader,
     walk_files,
 )
-from .yocto import find_elf_files_from_image_manifest
+from .yocto import (
+    BitbakeBuildEnvResult,
+    PackageDebugSplitStyle,
+    get_necessary_from_bitbake_build_env,
+    process_and_upload_yocto_symbols,
+)
+
+log = logging.getLogger(__name__)
+
 
 pass_memfault_cli_context = click.make_pass_decorator(MemfaultCliClickContext, ensure=True)
 click_argument_path = click.argument("path", type=click.Path(exists=True))
 click_option_concurrency = click.option(
     "--concurrency",
     required=False,
     default=8,
@@ -43,16 +55,16 @@
 @click.group()
 @click.option("--email", help="Account email to authenticate with")
 @click.password_option(
     "--password", prompt=False, help="Account password or user API key to authenticate with"
 )
 @click.option("--project-key", help="Memfault Project Key")
 @click.option("--org-token", help="Organization Auth Token")
-@click.option("--org", help="Organization slug")
-@click.option("--project", help="Project slug")
+@click.option("--org", help="Organization slug", callback=MemfaultCliClickContext.validate_slug_arg)
+@click.option("--project", help="Project slug", callback=MemfaultCliClickContext.validate_slug_arg)
 @click.option("--url", hidden=True)
 @click.option("--verbose", help="Log verbosely", is_flag=True)
 @click.version_option(version=version)
 @pass_memfault_cli_context
 def cli(ctx: MemfaultCliClickContext, **kwargs):
     ctx.obj.update(kwargs)
 
@@ -63,14 +75,17 @@
         requests_log = logging.getLogger("requests.packages.urllib3")
         requests_log.setLevel(logging.DEBUG)
         requests_log.propagate = True
 
         httpclient_logger = logging.getLogger("http.client")
         httpclient_logger.setLevel(logging.DEBUG)
 
+        httpclient_logger = logging.getLogger("memfault_cli")
+        httpclient_logger.setLevel(logging.DEBUG)
+
         def httpclient_log(*args) -> None:
             httpclient_logger.log(logging.DEBUG, " ".join(args))
 
         http.client.print = httpclient_log  # type: ignore[attr-defined]
         http.client.HTTPConnection.debuglevel = 1
 
 
@@ -78,15 +93,17 @@
     ctx: MemfaultCliClickContext, path: str, uploader_cls: Type[Uploader], **kwargs
 ) -> None:
     authenticator = ctx.create_authenticator(*uploader_cls.authenticator_types)
 
     uploader = uploader_cls(ctx=ctx, file_path=path, authenticator=authenticator, **kwargs)
     if not uploader.can_upload_file():
         raise click.exceptions.UsageError("Upload failed!")
-    uploader.upload()
+    did_upload = uploader.upload()
+    if not did_upload:
+        raise click.exceptions.ClickException("File(s) did not successfully upload")
 
 
 @cli.command(name="upload-coredump")
 @click.option(
     "--device-serial",
     required=False,
     help="A fallback unique identifier of a device, when one is not present in the coredump",
@@ -221,49 +238,114 @@
     """Upload a Memfault Archive File (mar) file for analysis."""
     ctx.obj.update(**kwargs)
     _do_upload_or_raise(ctx, path, MarUploader)
 
 
 @cli.command(name="upload-yocto-symbols")
 @click.option(
-    "--manifest",
-    "-m",
+    "--image",
+    "-i",
+    required=True,
+    help="""
+    The path to the root filesystem image as produced by Yocto's do_image_*.
+    The file is expected to reside in the location where Yocto produced the
+    file (tmp/deploy/images/${PACKAGE_ARCH}/images).
+
+    Supported formats: .tar, .tar.bz2, .tar.gz, .tar.xz
+    """,
+    type=click.Path(exists=True, resolve_path=True, dir_okay=False, path_type=pathlib.Path),
+)
+@click.option(
+    "--dbg-image",
+    "-d",
     required=True,
     help="""
-    The path to the image .manifest as produced by Yocto's do_rootfs (IMAGE_MANIFEST).
-    The .manifest file is expected to reside in the location where Yocto produced the file.
-    The tool will locate the symbol files to upload in the tmp/work/ directory, based on
-    the packages that are listed in the .manifest file.
+    The path to the dbg filesystem image as produced by Yocto's
+    IMAGE_GEN_DEBUGFS option. The file is expected to reside in the location
+    where Yocto produced the file (tmp/deploy/images/${PACKAGE_ARCH}/images).
+
+    To generate it alongside the required elfutils-native, add the following to
+    your main image (note that the main image will not be affected except for
+    its build dependencies):
+
+    \b
+    DEPENDS:append = " elfutils-native"
+    IMAGE_GEN_DEBUGFS = "2"
+    IMAGE_FSTYPES_DEBUGFS = "tar.bz2"
+
+    Supported formats: .tar, .tar.bz2, .tar.gz, .tar.xz
+    """,
+    type=click.Path(exists=True, resolve_path=True, dir_okay=False, path_type=pathlib.Path),
+)
+@click.option(
+    "--eu-unstrip-path",
+    required=False,
+    help="""
+    Path to a local eu-unstrip binary from elfutils
+    (https://sourceware.org/elfutils/).
+
+    Not necessary if running after 'source oe-init-build-env'.
+
+    If you pass --eu-unstrip-path, you must also pass --package-debug-split-style.
+    """,
+    type=click.Path(exists=True, resolve_path=True, dir_okay=False, path_type=pathlib.Path),
+)
+@click.option(
+    "--package-debug-split-style",
+    type=click.Choice([style.value for style in PackageDebugSplitStyle]),
+    required=False,
+    help="""
+    Your project's PACKAGE_DEBUG_SPLIT_STYLE. In Poky, defaults to
+    'debug-with-srcpkg'.
+
+    Not necessary if running after 'source oe-init-build-env'.
+
+    If you pass --package-debug-split-style, you must also pass --eu-unstrip-path.
     """,
-    type=click.File(),
 )
 @click_option_concurrency
 @pass_memfault_cli_context
-def upload_yocto_symbols(ctx: MemfaultCliClickContext, manifest: TextIO, **kwargs):
-    """Upload symbols for a Yocto build.
+def upload_yocto_symbols(
+    ctx: MemfaultCliClickContext,
+    image: pathlib.Path,
+    dbg_image: pathlib.Path,
+    eu_unstrip_path: Optional[pathlib.Path],
+    package_debug_split_style: Optional[str],
+    **kwargs,
+):
+    """Upload symbols for a Linux Yocto build.
 
     To see a full example, take a look at the Linux SDK example project:
-    https://mflt.io/yocto-symbols-image
+    https://mflt.io/yocto-upload-symbols
 
     Example Yocto Symbol Upload:
 
         \b
         $ bitbake my-image
         $ memfault --org-token $ORG_TOKEN \\
                    --org acme-inc --project smart-sink \\
-            upload-yocto-symbols --manifest build/tmp/deploy/images/raspberrypi3/my-image-raspberrypi3.rootfs.manifest
+            upload-yocto-symbols \\
+                   --image build/tmp/deploy/images/raspberrypi3/my-image-raspberrypi3.tar.bz2 \\
+                   --dbg-image build/tmp/deploy/images/raspberrypi3/my-image-raspberrypi3-dbg.tar.bz2
     """
     ctx.obj.update(**kwargs)
 
-    ElfSymbolDirectoryUploader(
-        ctx=ctx,
-        file_path=manifest.name,  # Not used. TODO: refactor!
-        authenticator=ctx.create_authenticator(OrgTokenAuthenticator, BasicAuthenticator),
-        file_paths=find_elf_files_from_image_manifest(manifest),
-    ).upload()
+    if eu_unstrip_path and package_debug_split_style:
+        build_env = BitbakeBuildEnvResult(
+            eu_unstrip_path=eu_unstrip_path,
+            package_debug_split_style=PackageDebugSplitStyle(package_debug_split_style),
+        )
+    elif eu_unstrip_path or package_debug_split_style:
+        raise click.exceptions.UsageError(
+            "Parameters '--eu-unstrip-path' and '--package-debug-split-style' must be used together."
+        )
+    else:
+        build_env = get_necessary_from_bitbake_build_env()
+
+    process_and_upload_yocto_symbols(ctx, image, dbg_image, build_env=build_env)
 
 
 @cli.command(name="upload-mcu-symbols")
 @click.option(
     "--software-type",
     required=False,
     help="Required for MCU symbols without Build Id, see https://mflt.io/symbol-file-build-ids",
@@ -366,15 +448,25 @@
     "--version-code",
     required=False,
     help="The version code of the app. When not specified, it is read from the .apk",
 )
 @click.option(
     "--mapping-txt",
     required=False,
-    help="The path to the Proguard/R8 mapping.txt file. When not specified, the default locations are searched.",
+    help="The path to the Proguard/R8 mapping.txt file. When not specified, the gradle default locations are searched.",
+)
+@click.option(
+    "--native-libs-dir",
+    required=False,
+    help="The path to the dir containing native libs. When not specified, the gradle default locations are searched.",
+)
+@click.option(
+    "--apk-dir",
+    required=False,
+    help="The path to the apk. When not specified, the gradle default locations are searched.",
 )
 @click_option_concurrency
 @click_argument_path
 @pass_memfault_cli_context
 def upload_android_app_symbols(ctx: MemfaultCliClickContext, path: str, **kwargs):
     """Upload symbols & R8/ProGuard mapping for an Android app build.
 
@@ -415,14 +507,20 @@
 @click.option("--notes", default="", help="Optional release notes.")
 @click.option(
     "--must-pass-through",
     required=False,
     is_flag=True,
     help="When the Release is deployed to a Cohort, forces a device to update through this version even if a newer version has also been deployed to the Cohort.",
 )
+@click.option(
+    "--extra-metadata",
+    required=False,
+    multiple=True,
+    help="Extra metadata in the form of `<key>=<value>` to attach to this artifact. This metadata will be returned alongside the artifact when the release is fetched.",
+)
 @click_option_revision
 @click_argument_path
 @pass_memfault_cli_context
 def upload_ota_payload(ctx: MemfaultCliClickContext, path: str, **kwargs):
     """Upload a binary to be used for an OTA update.
 
     See https://mflt.io/34PyNGQ for details about 'hardware-version',
@@ -461,51 +559,137 @@
     ctx.obj.update(**kwargs)
     ctx.check_required_either(
         {"software_version"}, {"delta_from", "delta_to"}, mutually_exclusive=True
     )
     _do_upload_or_raise(ctx, path, ReleaseArtifactUploader)
 
 
+@cli.command(name="upload-custom-data-recording")
+@click.option(
+    "--hardware-version",
+    type=click.STRING,
+    required=True,
+    help="Required to identify the type of hardware.",
+)
+@click.option(
+    "--software-type",
+    type=click.STRING,
+    required=True,
+    help="Required to identify the system software",
+)
+@click.option(
+    "--software-version",
+    type=click.STRING,
+    required=True,
+    help="Required to identify single builds on Devices",
+)
+@click.option(
+    "--device-serial",
+    required=True,
+    type=click.STRING,
+    help="The unique identifier of a Device",
+)
+@click.option(
+    "--start-time",
+    required=False,
+    default=datetime.now(tz=timezone.utc).strftime("%Y-%m-%dT%H:%M:%S%z"),
+    type=click.DateTime(formats=("%Y-%m-%dT%H:%M:%S%z",)),
+    help="Timestamp of when the custom data recording started. The timezone needs to be specified. Defaults to the current time. Example: '2022-10-14T10:33:23Z' or '2022-10-14T10:33:23+0200'.",
+)
+@click.option(
+    "--duration-secs",
+    required=True,
+    type=click.INT,
+    help="The duration (in seconds) of the custom data recording",
+)
+@click.option(
+    "--mimetype",
+    required=True,
+    multiple=True,
+    help="(Can be given multiple times.) List of mimetypes to attach to the file.",
+)
+@click.option(
+    "--reason",
+    required=True,
+    type=click.STRING,
+    help="The reason this custom data recording was uploaded",
+)
+@click_argument_path
+@pass_memfault_cli_context
+def upload_custom_data_recording(ctx: MemfaultCliClickContext, path: str, **kwargs):
+    """Upload a custom data recording (read: any file that might help you with debugging)."""
+    ctx.obj.update(**kwargs)
+    _do_upload_or_raise(ctx, path, CustomDataRecordingUploader)
+
+
 @cli.command(name="deploy-release")
 @click.option("--release-version", type=str, required=False)
 @click.option("--delta-from", required=False)
 @click.option("--delta-to", required=False)
 @click.option("--cohort", type=str, required=True)
 @click.option(
     "--rollout-percent",
     type=int,
     show_default=True,
     default=100,
     help="The (randomly sampled) percentage of devices in the Cohort to rollout the release to.",
 )
+@click.option("--deactivate", is_flag=True, help="Deactivate the release.")
 @pass_memfault_cli_context
-def deploy_release(ctx: MemfaultCliClickContext, cohort: str, rollout_percent: int, **kwargs):
+def deploy_release(
+    ctx: MemfaultCliClickContext, cohort: str, rollout_percent: int, deactivate: bool, **kwargs
+):
     """Publish a Release to a Cohort.
 
     \b
     Example Release Deployment:
     \b
         $ memfault --org-token $ORG_TOKEN \\
                    --org acme-inc --project smart-sink \\
                    deploy-release \\
                    --release-version 1.0.0-alpha \\
                    --cohort default
+
+    \b
+    Example Delta Release Deployment:
+    \b
+        $ memfault --org-token $ORG_TOKEN \\
+                   --org acme-inc --project smart-sink \\
+                   deploy-release \\
+                   --delta-from 0.9.0 \\
+                   --delta-to 1.0.0-alpha \\
+                   --cohort default
+
+    \b
+    Example Deactivation:
+    \b
+        $ memfault --org-token $ORG_TOKEN \\
+                   --org acme-inc --project smart-sink \\
+                   deploy-release \\
+                   --release-version 1.0.0-alpha \\
+                   --cohort default \\
+                   --deactivate
     """
     ctx.obj.update(**kwargs)
 
     authenticator = ctx.create_authenticator(OrgTokenAuthenticator, BasicAuthenticator)
     ctx.check_required_either(
         {"release_version"}, {"delta_from", "delta_to"}, mutually_exclusive=True
     )
     release_version = ctx.obj.get("release_version") or (
         ctx.obj["delta_from"],
         ctx.obj["delta_to"],
     )
     deployer = Deployer(ctx=ctx, authenticator=authenticator)
-    deployer.deploy(cohort=cohort, release_version=release_version, rollout_percent=rollout_percent)
+    if deactivate:
+        deployer.deactivate(cohort=cohort, release_version=release_version)
+    else:
+        deployer.deploy(
+            cohort=cohort, release_version=release_version, rollout_percent=rollout_percent
+        )
 
 
 def _do_post_chunks_or_raise(ctx: MemfaultCliClickContext, chunks: List[bytes]):
     authenticator = ctx.create_authenticator(ProjectKeyAuthenticator)
 
     MemfaultChunk(ctx, authenticator).batch_post(chunks)
     click.echo("Success")
@@ -589,14 +773,58 @@
     # it works properly when invoked from pytest or normal cli usage.
 
     cmd = "memfault"
     os.environ[f"_{cmd.upper()}_COMPLETE"] = f"{shell}_source"
     ctx.command.main(prog_name="memfault")
 
 
+@cli.command("console")
+@click.option("--device-serial", show_default=True, default="TESTSERIAL")
+@click.option(
+    "--port",
+    help="Serial port to read data from. Omit to choose from list of detected ports",
+    default=None,
+)
+@click.option("--baudrate", help="baud rate, default: 115200", default=115200)
+@pass_memfault_cli_context
+def console(ctx: MemfaultCliClickContext, port, baudrate, **kwargs):
+    """
+    Open a serial terminal and automatically post chunks to Memfault
+    The command requires output produced by memfault_data_export_chunk.
+
+    $ memfault --project-key ${YOUR_PROJECT_KEY} console --device-serial TESTSERIAL --port /dev/tty.usbmodem1 --encoding sdk_export
+    Example Output:
+    MC:CAKnAgEDAQdqVEVTVFNFUklBTAptdGVzdC1zb2Z0d2FyZQlqMS4wLjAtdGVzdAZtdGVzdC1oYXJkd2FyZQShAaFyY2h1bmtfdGVzdF9zdWNjZXNzATHk:
+
+    Reference: https://mflt.io/chunk-api-integration
+    """
+    from serial.tools import miniterm
+
+    if port is None:
+        port = miniterm.ask_for_port()
+
+    ctx.obj.update(**kwargs)
+
+    # Build chunk-poster
+    authenticator = ctx.create_authenticator(ProjectKeyAuthenticator)
+    if not authenticator.project_key_auth():
+        click.secho(
+            "Use 'memfault --project-key=${PROJECT_KEY} console' to automatically upload chunks",
+            fg="yellow",
+        )
+        chunk_handler = None
+    else:
+        chunk_handler = MemfaultChunk(ctx, authenticator)
+
+    MemfaultMiniterm.from_port(chunk_handler=chunk_handler, port=port, baudrate=baudrate)
+
+
 def main():
     logging.basicConfig(level=logging.INFO, format="%(levelname)s: %(message)s")
-    cli(auto_envvar_prefix="MEMFAULT")
+    # optionally set terminal to infinite width for consistent click output
+    # formatting
+    terminal_width = float("inf") if os.environ.get("CI") else None
+    cli(auto_envvar_prefix="MEMFAULT", terminal_width=terminal_width)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `memfault-cli-0.9.0/memfault_cli/context.py` & `memfault_cli-1.0.0/memfault_cli/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 import json
 import logging
+import re
+from datetime import datetime, timedelta
 from typing import Any, Dict, List, Optional, Set, Type, Union
 
 import click
 
 from .authenticator import Authenticator
 
-LOG = logging.getLogger(__name__)
+log = logging.getLogger(__name__)
 
 
-class PackageInfo:  # noqa: B903 - no data classes in Python 3.6
+class PackageInfo:
     def __init__(self, name: str, version_name: str, version_code: str):
         self.name = name
         self.version_name = version_name
         self.version_code = version_code
 
 
-class FullReleaseVersion:  # noqa: B903 - no data classes in Python 3.6
+class FullReleaseVersion:
     def __init__(self, software_version: str):
         self.software_version = software_version
 
     def to_json_representable(self):
         return self.software_version
 
 
-class DeltaReleaseVersion:  # noqa: B903 - no data classes in Python 3.6
+class DeltaReleaseVersion:
     def __init__(self, delta_from: str, delta_to: str):
         self.delta_from = delta_from
         self.delta_to = delta_to
 
     def to_json_representable(self):
         return [self.delta_from, self.delta_to]
 
 
-class SoftwareInfo:  # noqa: B903 - no data classes in Python 3.6
+class SoftwareInfo:
     def __init__(
         self,
         software_type: str,
         version: Union[FullReleaseVersion, DeltaReleaseVersion],
         revision: Optional[str] = None,
     ):
         self.software_type = software_type
         self.version = version
         self.revision = revision
 
 
 CustomMetricReadingValueType = Union[int, float, str, bool, None]
 
 
-class Attribute:  # noqa: B903 - no data classes in Python 3.6
+class Attribute:
     def __init__(self, string_key: str, value: CustomMetricReadingValueType) -> None:
         self.string_key = string_key
         self.value = value
 
     @staticmethod
     def from_cli_args(key: str, cli_value: str):
         return Attribute(string_key=key, value=Attribute._convert_value(cli_value))
@@ -62,42 +64,53 @@
         if cli_value == "":
             return None
         try:
             value = json.loads(cli_value)
         except json.decoder.JSONDecodeError:
             value = cli_value
         if value is not None and not isinstance(value, (int, float, str, bool)):
-            LOG.warning(
-                "Only boolean, number, string or null types are allowed! Treating passed value as a string."
+            log.warning(
+                "Only boolean, number, string or null types are allowed! Treating passed value as a"
+                " string."
             )
             return cli_value
         return value
 
 
-class XedInfo:  # noqa: B903 - no data classes in Python 3.6
+class XedInfo:
     def __init__(self, device_serial: str, hardware_version: str):
         self.device_serial = device_serial
         self.hardware_version = hardware_version
 
 
-class CoreInfo:  # noqa: B903 - no data classes in Python 3.6
+class CoreInfo:
     def __init__(self, device_serial: str):
         self.device_serial = device_serial
 
 
-class MarInfo:  # noqa: B903 - no data classes in Python 3.6
+class DeviceTraitsInfo:
     def __init__(
         self, device_serial: str, hardware_version: str, software_type: str, software_version: str
     ):
         self.device_serial = device_serial
         self.hardware_version = hardware_version
         self.software_type = software_type
         self.software_version = software_version
 
 
+class CustomDataRecordingInfo:
+    def __init__(
+        self, start_time: datetime, duration: timedelta, mimetypes: List[str], reason: str
+    ):
+        self.start_time = start_time
+        self.duration = duration
+        self.mimetypes = mimetypes
+        self.reason = reason
+
+
 class MemfaultCliClickContext(object):
     """
     A context passed around between the memfault cli sub-commands.
 
 
     If the top level CLI has any "required" it's not possible to display
     any help info about the subcommands using "--help" without providing them.
@@ -137,15 +150,16 @@
                 passed_arg_sets.append(arg_set)
             if all(args_present):
                 valid_arg_sets.append(arg_set)
 
         if mutually_exclusive and len(passed_arg_sets) > 1:
             formatted_passed_args = [self._format_arg_set(arg_set) for arg_set in passed_arg_sets]
             raise click.exceptions.UsageError(
-                f"Parameters {' and '.join(sorted(formatted_passed_args))} may not be used together."
+                f"Parameters {' and '.join(sorted(formatted_passed_args))} may not be used"
+                " together."
             )
 
         if len(valid_arg_sets) == 0:
             formatted_required_args = [self._format_arg_set(arg_set) for arg_set in args]
             raise click.exceptions.UsageError(
                 f"Please pass either {' or '.join(sorted(formatted_required_args))}."
             )
@@ -157,14 +171,31 @@
                 self.check_required_auth_cli_args(authenticator_type=_type)
                 return _type(self)
             except click.exceptions.UsageError:
                 pass
         # Raise for the first missing option of the preferred authenticator type:
         raise self.check_required_auth_cli_args(authenticator_type=types[0])
 
+    @staticmethod
+    def validate_slug_arg(ctx, param, value) -> Optional[str]:
+        if not isinstance(value, str):
+            return value
+
+        slugified_arg = re.fullmatch(r"[a-z0-9-]+", value)
+        if not slugified_arg:
+            log.warning(
+                (
+                    "The value %r doesn't look like a slug (not to be confused with the"
+                    ' human-readable "name"). Please find your slugs at'
+                    " https://app.memfault.com/organizations/-/projects/-/settings"
+                ),
+                value,
+            )
+        return value
+
     @property
     def org(self):
         return self._find_obj_or_raise("org")
 
     @property
     def org_token(self) -> str:
         return self._find_obj_or_raise("org_token")
@@ -198,32 +229,35 @@
         delta_to = self.obj.get("delta_to")
 
         version: Union[DeltaReleaseVersion, FullReleaseVersion, None]
         if delta_from and delta_to:
             version = DeltaReleaseVersion(delta_from, delta_to)
             if delta_from == delta_to:
                 raise click.exceptions.UsageError(
-                    "Version passed to --delta-{{from-to}} must not be the same, please specify two different versions"
+                    "Version passed to --delta-{{from-to}} must not be the same, please specify two"
+                    " different versions"
                 )
         elif sw_ver:
             version = FullReleaseVersion(sw_ver)
         else:
             version = None
 
         if revision and (version is None or sw_type is None):
             raise click.exceptions.UsageError(
-                "A version ('--software-version' or '--delta-{{from,to}}') and '--software-type' must be specified when using '--revision'"
+                "A version ('--software-version' or '--delta-{{from,to}}') and '--software-type'"
+                " must be specified when using '--revision'"
             )
 
         if sw_type is None and version is None:
             return None
 
         if sw_type is None or version is None:
             raise click.exceptions.UsageError(
-                "Version ('--software-version' or '--delta-{{from,to}}') and '--software-type' must be specified together"
+                "Version ('--software-version' or '--delta-{{from,to}}') and '--software-type' must"
+                " be specified together"
             )
 
         return SoftwareInfo(
             software_type=sw_type,
             version=version,
             revision=revision,
         )
@@ -247,27 +281,38 @@
         hardware_version = self._find_obj_or_raise("hardware_version")
         return XedInfo(
             device_serial=device_serial,
             hardware_version=hardware_version,
         )
 
     @property
-    def mar_info(self) -> MarInfo:
+    def device_traits_info(self) -> DeviceTraitsInfo:
         device_serial = self._find_obj_or_raise("device_serial")
         hardware_version = self._find_obj_or_raise("hardware_version")
         software_type = self._find_obj_or_raise("software_type")
         software_version = self._find_obj_or_raise("software_version")
-        return MarInfo(
+        return DeviceTraitsInfo(
             device_serial=device_serial,
             hardware_version=hardware_version,
             software_type=software_type,
             software_version=software_version,
         )
 
     @property
+    def custom_data_recording_info(self) -> CustomDataRecordingInfo:
+        start_time = self._find_obj_or_raise("start_time")
+        duration = timedelta(seconds=self._find_obj_or_raise("duration_secs"))
+        mimetypes = self._find_obj_or_raise("mimetype")
+        reason = self._find_obj_or_raise("reason")
+
+        return CustomDataRecordingInfo(
+            start_time=start_time, duration=duration, mimetypes=mimetypes, reason=reason
+        )
+
+    @property
     def file_url(self) -> str:
         url = self.obj.get("url")
         if url is None:
             return "https://files.memfault.com"
         return url
 
     @property
@@ -327,9 +372,30 @@
         return PackageInfo(package, version_name, version_code)
 
     @property
     def android_mapping_txt(self) -> Optional[str]:
         return self.obj.get("mapping_txt")
 
     @property
+    def android_native_libs_dir(self) -> Optional[str]:
+        return self.obj.get("native_libs_dir")
+
+    @property
+    def android_apk_dir(self) -> Optional[str]:
+        return self.obj.get("apk_dir")
+
+    @property
+    def extra_info(self) -> Optional[dict]:
+        extra_metadata: List[str] | None = self.obj.get("extra_metadata")
+        if extra_metadata is None:
+            return None
+        else:
+            try:
+                return dict(s.split("=", 1) for s in extra_metadata)
+            except ValueError as error:
+                raise click.exceptions.UsageError(
+                    "--extra-metadata must be a key value pair in the form 'key=value'.",
+                ) from error
+
+    @property
     def verbose(self) -> bool:
         return self.obj.get("verbose", False)
```

### Comparing `memfault-cli-0.9.0/memfault_cli/functools_ext.py` & `memfault_cli-1.0.0/memfault_cli/functools_ext.py`

 * *Files identical despite different names*

### Comparing `memfault-cli-0.9.0/memfault_cli/upload.py` & `memfault_cli-1.0.0/memfault_cli/upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,32 +12,51 @@
 
 import click
 import requests
 from elftools.elf.elffile import ELFFile
 from mflt_build_id import BuildIdInspectorAndPatcher
 from requests import Response, Session
 from requests.adapters import HTTPAdapter
+from requests.packages.urllib3.util.retry import Retry
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
-from urllib3 import Retry
 
 from .authenticator import (
     Authenticator,
     BasicAuthenticator,
     OrgTokenAuthenticator,
     ProjectKeyAuthenticator,
 )
 from .context import DeltaReleaseVersion, MemfaultCliClickContext, PackageInfo
 from .elf import elf_has_debug_info, get_gnu_build_id, is_elf
 from .functools_ext import cached_property
 
-LOG = logging.getLogger(__name__)
+log = logging.getLogger(__name__)
 
 GNU_BUILD_ID_RE = re.compile(r"Build ID: (?P<gnu_build_id>[a-f\d]+)")
 
+UPLOAD_IS_TOO_BIG_RESPONSE = "Uploaded file is too big"
+
+
+class UploadedAlreadyExistsError(Exception):
+    pass
+
+
+class UploadIsTooLargeError(Exception):
+    pass
+
+
+class MemfaultAPIErrorResponse:
+    kind: str
+    message: str
+
+    def __init__(self, response: Response):
+        self.message = response.json()["error"]["message"]
+        self.kind = response.json()["error"]["type"]
+
 
 def hash_io_hexdigest(name, data: IO, chunksize=2**20) -> str:
     """
     A wrapper around hashlib.new() and hexdigest() which reads
     from a stream in chunks
     """
     assert data.readable()
@@ -120,20 +139,18 @@
             return f"{self._api_base_url()}/upload"
         else:
             return f"{self._projects_base_url()}/upload"
 
     @abstractmethod
     def can_upload_file(self) -> bool:
         """Test the file pointed to by `file_path`."""
-        pass
 
     @abstractmethod
     def entity_url(self) -> str:
         """The final URL to POST to during the prepared upload sequence."""
-        pass
 
     def ui_url(self) -> Optional[str]:
         """The UI URL at which results from the operation can be seen"""
         return None
 
     def _is_already_uploaded(self) -> bool:
         return False
@@ -171,36 +188,49 @@
             json_d.update(extra_request_data)
 
         response = self.session.post(
             self.entity_url(), json=json_d, **self.authenticator.requests_auth_params()
         )
         # This file had already uploaded (maybe concurrently). Gracefully ignore the error then.
         if response.status_code == 409:
-            LOG.info("%s: was already uploaded.", self.file_path)
-            return
+            log.info("%s: was already uploaded.", self.file_path)
+            raise UploadedAlreadyExistsError("%s: was already uploaded." % self.file_path)
+
+        if response.status_code == 400:
+            error = MemfaultAPIErrorResponse(response)
+            if UPLOAD_IS_TOO_BIG_RESPONSE in error.message:
+                # Need to grab the max file size from the error response, so we have to print the real message
+                raise UploadIsTooLargeError(error.message + f" ({self.file_path!r})")
 
         check_response(response)
 
     @property
     def qcomm_project(self):
         response = self.session.get(
             self._projects_base_url(base_url_override=self.ctx.api_url),
             **self.authenticator.requests_auth_params(),
         )
         check_response(response)
         return response.json()["data"].get("qcomm_enabled", False)
 
     def upload(self, *, progressbar=True) -> bool:
         if self._is_already_uploaded():
-            LOG.info("%s: skipping, already uploaded.", self.file_path)
-            return False
+            log.info("%s: skipping, already uploaded.", self.file_path)
+            return True
         upload_url, token = self._prepare_upload()
         self._put_file(upload_url, progressbar=progressbar)
-        self._post_token(token)
-        LOG.info("%s: uploaded!", self.file_path)
+        try:
+            self._post_token(token)
+            log.info("%s: uploaded!", self.file_path)
+        except UploadIsTooLargeError as e:
+            log.warning(str(e))
+            return False
+        except UploadedAlreadyExistsError:
+            pass
+
         if self.ui_url():
             click.echo(f"You can view in the UI here:\n   {self.ui_url()}")
         return True
 
     @cached_property
     def file_md5(self):
         with open(self.file_path, "rb") as f:
@@ -216,15 +246,15 @@
         ProjectKeyAuthenticator,
         OrgTokenAuthenticator,
         BasicAuthenticator,
     ]
 
     def can_upload_file(self) -> bool:
         if not is_zipfile(self.file_path):
-            LOG.error("%s is not a valid zip file!", self.file_path)
+            log.error("%s is not a valid zip file!", self.file_path)
             return False
         return True
 
     def entity_url(self) -> str:
         if self.authenticator.project_key_auth():
             return f"{self._api_base_url()}/upload/bugreport"
         else:
@@ -238,15 +268,15 @@
         BasicAuthenticator,
     ]
 
     def can_upload_file(self) -> bool:
         with open(self.file_path, "rb") as f:
             hdr = f.read(4).decode("ascii", errors="ignore")
             if hdr != "CORE":
-                LOG.error("%s is not a Memfault Coredump", self.file_path)
+                log.error("%s is not a Memfault Coredump", self.file_path)
                 return False
 
         return True
 
     def entity_url(self) -> str:
         if self.authenticator.project_key_auth():
             return f"{self._api_base_url()}/upload/coredump"
@@ -293,69 +323,104 @@
         ProjectKeyAuthenticator,
         OrgTokenAuthenticator,
         BasicAuthenticator,
     ]
 
     def can_upload_file(self) -> bool:
         if not is_zipfile(self.file_path):
-            LOG.error("%s is not a valid zip file!", self.file_path)
+            log.error("%s is not a valid zip file!", self.file_path)
             return False
         return True
 
     def entity_url(self) -> str:
         if self.authenticator.project_key_auth():
             return f"{self._api_base_url()}/upload/mar"
         else:
             return f"{self._projects_base_url()}/mar"
 
     def post_token_extra_request_data(self) -> Optional[Dict]:
-        info = self.ctx.mar_info
+        info = self.ctx.device_traits_info
         return {
             "device_serial": info.device_serial,
             "hardware_version": info.hardware_version,
             "software_type": info.software_type,
             "software_version": info.software_version,
         }
 
 
+class CustomDataRecordingUploader(Uploader):
+    authenticator_types = [
+        ProjectKeyAuthenticator,
+        OrgTokenAuthenticator,
+        BasicAuthenticator,
+    ]
+
+    def can_upload_file(self) -> bool:
+        return True
+
+    def entity_url(self) -> str:
+        if self.authenticator.project_key_auth():
+            return f"{self._api_base_url()}/upload/custom-data-recording"
+        else:
+            return f"{self._projects_base_url()}/custom-data-recording"
+
+    def post_token_extra_request_data(self) -> Optional[Dict]:
+        device_traits = self.ctx.device_traits_info
+        info = self.ctx.custom_data_recording_info
+        return {
+            "start_time": info.start_time.isoformat(),
+            "duration_secs": int(info.duration.total_seconds()),
+            "mimetypes": info.mimetypes,
+            "reason": info.reason,
+            "device": {
+                "device_serial": device_traits.device_serial,
+                "hardware_version": device_traits.hardware_version,
+                "software_type": device_traits.software_type,
+                "software_version": device_traits.software_version,
+            },
+        }
+
+
 class ElfSymbolUploader(Uploader):
     authenticator_types = [
         OrgTokenAuthenticator,
         BasicAuthenticator,
     ]
 
-    gnu_build_id: str = ""
+    gnu_build_id: Optional[str] = ""
 
     def can_upload_file(self) -> bool:
         if os.path.islink(self.file_path) and not os.path.exists(self.file_path):
             return False
 
         with open(self.file_path, "rb") as f:
             if not is_elf(f):
-                LOG.info("%s: Not an ELF file", self.file_path)
+                log.info("%s: Not an ELF file", self.file_path)
                 return False
 
             elf = ELFFile(f)
             gnu_build_id, has_debug_info = get_gnu_build_id(elf), elf_has_debug_info(elf)
             if not gnu_build_id:
-                LOG.info(
+                log.info(
                     "%s: looks like an ELF but does not contain a GNU Build ID", self.file_path
                 )
                 return False
 
         self.gnu_build_id = gnu_build_id
         if not has_debug_info:
-            LOG.info("%s: looks like an ELF but it has no .debug_info", self.file_path)
+            log.info("%s: looks like an ELF but it has no .debug_info", self.file_path)
             return False
-        LOG.info(
+        log.info(
             "%s: ELF file with .debug_info and GNU Build ID: %s", self.file_path, self.gnu_build_id
         )
         return True
 
     def _is_already_uploaded(self) -> bool:
+        if not self.gnu_build_id:
+            return False
         response = self.session.head(
             f"{self._projects_base_url()}/symbols-by-gnu-build-id/{self.gnu_build_id}",
             **self.authenticator.requests_auth_params(),
         )
         try:
             check_response(response)
         except Exception:
@@ -364,50 +429,51 @@
             raise
         return True
 
     def entity_url(self) -> str:
         return f"{self._projects_base_url()}/symbols"
 
 
-class McuSdkElfSymbolUploader(Uploader):
+class McuSdkElfSymbolUploader(ElfSymbolUploader, Uploader):
     authenticator_types = [
         OrgTokenAuthenticator,
         BasicAuthenticator,
     ]
 
     def can_upload_file(self) -> bool:
         with open(self.file_path, "rb") as file:
             if file.read(4) != b"\x7FELF":
-                LOG.info("%s: Not an ELF file", self.file_path)
+                log.info("%s: Not an ELF file", self.file_path)
                 return False
             file.seek(0)
 
             inspector = BuildIdInspectorAndPatcher(file)
             if not elf_has_debug_info(inspector.elf):
-                LOG.info("%s: looks like an ELF but it has no .debug_info", self.file_path)
+                log.info("%s: looks like an ELF but it has no .debug_info", self.file_path)
                 return False
 
-            mcu_build_id_type, mcu_build_id, mcu_build_id_short_len = inspector.get_build_info()
+            (
+                mcu_build_id_type,
+                self.gnu_build_id,
+                mcu_build_id_short_len,
+            ) = inspector.get_build_info()
 
             # NB: QC symbol files have different arg requirements depending on the subsystem the
             # ELF is associated with so we offload to the Memfault backend.
-            if not self.ctx.software_info and mcu_build_id is None and not self.qcomm_project:
-                LOG.error(
+            if not self.ctx.software_info and self.gnu_build_id is None and not self.qcomm_project:
+                log.error(
                     "%s: Build Id missing. Specify --software-version and --software-type options "
                     "or add a Build Id (see https://mflt.io/symbol-file-build-ids)",
                     self.file_path,
                 )
                 return False
 
-        LOG.info("%s: ELF file with .debug_info. Build Id: %s", self.file_path, mcu_build_id)
+        log.info("%s: ELF file with .debug_info. Build Id: %s", self.file_path, self.gnu_build_id)
         return True
 
-    def _is_already_uploaded(self) -> bool:
-        return False
-
     def entity_url(self) -> str:
         return f"{self._projects_base_url()}/symbols"
 
     def ui_url(self) -> Optional[str]:
         if not self.ctx.software_info or (
             # Unreachable with our CLI, but for safety:
             isinstance(self.ctx.software_info.version, DeltaReleaseVersion)
@@ -485,14 +551,15 @@
                 "version": info.version.to_json_representable(),
                 "software_type": info.software_type,
                 **({"revision": info.revision} if info.revision else {}),
             },
             "must_pass_through": self.ctx.must_pass_through,
             "hardware_version": self.ctx.hardware_version,
             "notes": self.ctx.notes,
+            **(dict(extra_info=self.ctx.extra_info) if self.ctx.extra_info else {}),
         }
 
 
 def walk_files(toplevel: str) -> Iterable[str]:
     for root, _dirs, files in os.walk(toplevel):
         for file in files:
             yield os.path.join(root, file)
@@ -524,15 +591,15 @@
             uploader = self.uploader_cls(
                 ctx=self.ctx, file_path=file_path, authenticator=self.authenticator
             )
             if uploader.can_upload_file():
                 queued_uploaders.append(uploader)
                 did_upload |= True
             else:
-                LOG.info("%s: skipping...", file_path)
+                log.info("%s: skipping...", file_path)
 
         def do_upload(uploader: Uploader):
             uploader.upload(progressbar=False)
 
         # If we find that we have more implementations that need to do parallel uploads,
         # We should generalize this logic into a class or have a function called `get_uploaders`
         # that the calling client can then parallelize by calling `.upload()` on each.
@@ -592,23 +659,25 @@
     authenticator_types = [
         OrgTokenAuthenticator,
         BasicAuthenticator,
     ]
 
     def can_upload_file(self) -> bool:
         if not os.path.isdir(self.file_path):
-            LOG.error(
+            log.error(
                 '%s is not a directory. Please specify the Android app\'s root "build" path instead!',
                 self.file_path,
             )
             return False
         return True
 
     def _find_apk_path(self) -> str:
-        apk_dir = os.path.join(self.file_path, "outputs", "apk", self.ctx.build_variant)
+        apk_dir = self.ctx.android_apk_dir
+        if apk_dir is None:
+            apk_dir = os.path.join(self.file_path, "outputs", "apk", self.ctx.build_variant)
         if not os.path.isdir(apk_dir):
             raise click.exceptions.FileError(
                 apk_dir, hint='Please pass the Android app\'s root "build" path!'
             )
         apk_glob = os.path.join(apk_dir, "*.apk")
         apks = glob(apk_glob)
         if not apks:
@@ -635,15 +704,15 @@
                 ),
                 subdirs,
             )
         )
         for path in paths_to_check:
             if os.path.isfile(path):
                 return path
-        LOG.info("No mapping.txt found in default locations, assuming ProGuard/R8 is disabled...")
+        log.info("No mapping.txt found in default locations, assuming ProGuard/R8 is disabled...")
         return None
 
     def _upload_mapping_txt(self) -> bool:
         mapping_txt_path = self._find_mapping_txt()
         if not mapping_txt_path:
             return False
         package_info = self.ctx.android_package_info
@@ -654,25 +723,28 @@
             file_path=mapping_txt_path,
             package_info=package_info,
             authenticator=self.authenticator,
         )
         return pg_uploader.upload()
 
     def _upload_ndk_symbols(self) -> bool:
-        # TODO: add support for legacy ndkBuild?
-        cmake_path_out = os.path.join(
-            self.file_path, "intermediates", "cmake", self.ctx.build_variant
-        )
-        if not os.path.isdir(cmake_path_out):
+        native_libs_dir = self.ctx.android_native_libs_dir
+        if native_libs_dir is None:
+            native_libs_dir = os.path.join(
+                self.file_path, "intermediates", "cmake", self.ctx.build_variant
+            )
+        if not os.path.isdir(native_libs_dir):
+            log.info("No native libs found in %s, assuming none were built...", native_libs_dir)
             return False
+        native_libs_dir = str(native_libs_dir)
         sym_dir_uploader = ElfSymbolDirectoryUploader(
             ctx=self.ctx,
-            file_path=cmake_path_out,
+            file_path=native_libs_dir,
             authenticator=self.authenticator,
-            file_paths=walk_files(cmake_path_out),
+            file_paths=walk_files(native_libs_dir),
         )
         return sym_dir_uploader.upload()
 
     def upload(self, *, progressbar=True) -> bool:
         did_upload = self._upload_mapping_txt() or self._upload_ndk_symbols()
         if not did_upload:
             raise click.exceptions.UsageError("No files uploaded!")
```

