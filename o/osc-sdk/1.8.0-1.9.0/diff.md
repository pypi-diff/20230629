# Comparing `tmp/osc-sdk-1.8.0.tar.gz` & `tmp/osc-sdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc-sdk-1.8.0.tar", last modified: Mon Apr 25 13:05:38 2022, max compression
+gzip compressed data, was "osc-sdk-1.9.0.tar", last modified: Tue Nov 15 08:58:10 2022, max compression
```

## Comparing `osc-sdk-1.8.0.tar` & `osc-sdk-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 13:05:38.238707 osc-sdk-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-04-25 13:05:17.000000 osc-sdk-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-04-25 13:05:38.238707 osc-sdk-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5239 2022-04-25 13:05:17.000000 osc-sdk-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 13:05:38.238707 osc-sdk-1.8.0/osc_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-04-25 13:05:17.000000 osc-sdk-1.8.0/osc_sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    24489 2022-04-25 13:05:17.000000 osc-sdk-1.8.0/osc_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-04-25 13:05:17.000000 osc-sdk-1.8.0/osc_sdk/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-04-25 13:05:17.000000 osc-sdk-1.8.0/osc_sdk/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-04-25 13:05:17.000000 osc-sdk-1.8.0/osc_sdk/test_noauth.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 13:05:38.238707 osc-sdk-1.8.0/osc_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-04-25 13:05:38.000000 osc-sdk-1.8.0/osc_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-04-25 13:05:38.000000 osc-sdk-1.8.0/osc_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 13:05:38.000000 osc-sdk-1.8.0/osc_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-04-25 13:05:38.000000 osc-sdk-1.8.0/osc_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-04-25 13:05:38.000000 osc-sdk-1.8.0/osc_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-25 13:05:38.000000 osc-sdk-1.8.0/osc_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-04-25 13:05:38.238707 osc-sdk-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-04-25 13:05:17.000000 osc-sdk-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 08:58:10.480176 osc-sdk-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-11-15 08:57:45.000000 osc-sdk-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-15 08:57:45.000000 osc-sdk-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8033 2022-11-15 08:58:10.480176 osc-sdk-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7372 2022-11-15 08:57:45.000000 osc-sdk-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 08:58:10.480176 osc-sdk-1.9.0/osc_sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-15 08:57:45.000000 osc-sdk-1.9.0/osc_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51980 2022-11-15 08:57:45.000000 osc-sdk-1.9.0/osc_sdk/osc-cli-completion.bash
+-rwxr-xr-x   0 runner    (1001) docker     (121)    25226 2022-11-15 08:57:45.000000 osc-sdk-1.9.0/osc_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2022-11-15 08:57:45.000000 osc-sdk-1.9.0/osc_sdk/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2022-11-15 08:57:45.000000 osc-sdk-1.9.0/osc_sdk/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-11-15 08:57:45.000000 osc-sdk-1.9.0/osc_sdk/test_noauth.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 08:58:10.480176 osc-sdk-1.9.0/osc_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8033 2022-11-15 08:58:10.000000 osc-sdk-1.9.0/osc_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-11-15 08:58:10.000000 osc-sdk-1.9.0/osc_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 08:58:10.000000 osc-sdk-1.9.0/osc_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-15 08:58:10.000000 osc-sdk-1.9.0/osc_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-11-15 08:58:10.000000 osc-sdk-1.9.0/osc_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-15 08:58:10.000000 osc-sdk-1.9.0/osc_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-11-15 08:58:10.480176 osc-sdk-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-11-15 08:57:45.000000 osc-sdk-1.9.0/setup.py
```

### Comparing `osc-sdk-1.8.0/LICENSE` & `osc-sdk-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osc-sdk-1.8.0/PKG-INFO` & `osc-sdk-1.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: osc-sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Outscale API SDK and CLI
 Home-page: https://github.com/outscale/osc-cli
 Author: Outscale SAS
 Author-email: contact@outscale.com
 License: BSD
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,17 +23,66 @@
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Getting Started
 
 ### Prerequisites
 
-You will need [Python 3.5+](https://www.python.org/) or later. Earlier versions including Python 2 are not supported.
+You will need [Python 3.6+](https://www.python.org/) or later. Earlier versions including Python 2 are not supported.
 
-### Installing from package
+### Installing on Macos
+
+osc-cli is available on [brew](https://formulae.brew.sh/formula/osc-cli).
+
+### Installing on Linux
+
+osc-cli is pre-packaged for Linux as a standalone [AppImage](https://appimage.org/).
+- Download `osc-cli-x86_64.AppImage` from latest version in [releases](https://github.com/outscale/osc-cli/releases).
+- Allow file to be executed by running `chmod a+x osc-cli-x86_64.AppImage`
+- Run osc-cli: `./osc-cli-x86_64.AppImage`
+
+Optionally, you can install it for all users: `sudo mv osc-cli-x86_64.AppImage /usr/local/bin/osc-cli` and just run `osc-cli`.
+
+you can also install `osc-cli-git` on Arch Linux using AUR: (`yay -S osc-cli-git`)
+
+#### Note:
+
+if you have this error (or one similar about fuse):
+```
+fuse: failed to exec fusermount: No such file or directory
+
+Cannot mount AppImage, please check your FUSE setup.
+You might still be able to extract the contents of this AppImage
+if you run it with the --appimage-extract option.
+See https://github.com/AppImage/AppImageKit/wiki/FUSE
+for more information
+open dir error: No such file or directory
+```
+
+You can either install fuse yourself, or execute the appimage with `--appimage-extract-and-run` option
+
+Example:
+```
+./osc-cli-x86_64.AppImage --appimage-extract-and-run osc-cli api ReadImages --profile=my
+```
+
+using `appimage-extract-and-run` extract the content of the AppImage in a temporary directory and execute it,
+this operation is a **lot** slower than using fuse, and the fuse solution should be use if posible.
+
+
+### Installing on Windows
+
+osc-cli is pre-packaged for windows:
+- Download `osc-cli-x86_64.zip` from latest version in [releases](https://github.com/outscale/osc-cli/releases).
+- Extract zip archive and run `osc-cli.exe`
+
+Note that some antivirus may consider some files as a virus. Those are false positive.
+If you are worried about it, consider installing osc-cli from Python Package (see below).
+
+### Installing from Python package
 
 You can get the package from [pypi](https://pypi.org/project/osc-sdk/):
 ```
 pip3 install osc-sdk
 ```
 
 If you are using Microsoft Windows, see [how to setup osc-cli on Windows](windows-setup.md).
@@ -57,26 +105,23 @@
 
 The CLI requires a configuration file in `~/.osc/config.json` The content must be a JSON whose contents look like this:
 /!\ the old configuration path using `.osc_sdk` folder is **deprecated**. Please use the new one with `.osc`.
 ```json
 {"default":
     {"access_key": "MYACCESSKEY",
      "secret_key": "MYSECRETKEY",
-     "host": "outscale.com",
-     "https": true,
-     "method": "POST",
-     "region_name": "eu-west-2"
+     "region": "eu-west-2"
     },
   "us":
     {"access_key": "MYACCESSKEY",
      "secret_key": "MYSECRETKEY",
      "host": "outscale.com",
      "https": true,
      "method": "POST",
-     "region_name": "us-east-2"
+     "region": "us-east-2"
     }
 }
 ```
 You can add several profiles for different regions or users.
 
 Optional parameters can be applied to each profile :
 * client_certificate: if you need additional security, your pem must include your private key and your certificate
@@ -86,20 +131,38 @@
 {"default":
     {"access_key": "MYACCESSKEY",
      "secret_key": "MYSECRETKEY",
      "client_certificate" : "path_to_your_pem",
      "host": "outscale.com",
      "https": true,
      "method": "POST",
-     "region_name": "eu-west-2",
+     "region": "eu-west-2",
      "version": "2018-11-19"
     }
 }
 ```
 
+## Activate bash-completion
+
+### Activate the completion for the current bash session
+
+```
+source <(osc-cli --bash_completion)
+```
+
+### Generate the file to add it in your bach rc:
+```
+osc-cli --bash_completion > ~/.osc/cli-completion.bash
+```
+then in your bashrc add:
+
+```
+source ~/.osc/cli-completion.bash
+```
+
 ## Usage
 
 ```
 osc-cli SERVICE CALL [PROFILE] [CALL-PARAMETERS]
 ```
 or
 ```
@@ -179,9 +242,7 @@
 ```bash
 osc-cli icu ListAccessKeys --authentication-method=password --login youremail@company.com --password=Y0URpAssOrd
 ```
 ## Contributing
 OSC-CLI is an **open source software** licensed under **BSD-3-Clause.**
 
 Patches and discussions are welcome about bugs you've found or features you think are missing. If you would like to help making **osc-cli** better, take a look to [CONTRIBUTING.md](https://github.com/outscale/osc-cli/blob/master/CONTRIBUTING.md) file.
-
-
```

### Comparing `osc-sdk-1.8.0/README.md` & `osc-sdk-1.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,17 +4,66 @@
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Getting Started
 
 ### Prerequisites
 
-You will need [Python 3.5+](https://www.python.org/) or later. Earlier versions including Python 2 are not supported.
+You will need [Python 3.6+](https://www.python.org/) or later. Earlier versions including Python 2 are not supported.
 
-### Installing from package
+### Installing on Macos
+
+osc-cli is available on [brew](https://formulae.brew.sh/formula/osc-cli).
+
+### Installing on Linux
+
+osc-cli is pre-packaged for Linux as a standalone [AppImage](https://appimage.org/).
+- Download `osc-cli-x86_64.AppImage` from latest version in [releases](https://github.com/outscale/osc-cli/releases).
+- Allow file to be executed by running `chmod a+x osc-cli-x86_64.AppImage`
+- Run osc-cli: `./osc-cli-x86_64.AppImage`
+
+Optionally, you can install it for all users: `sudo mv osc-cli-x86_64.AppImage /usr/local/bin/osc-cli` and just run `osc-cli`.
+
+you can also install `osc-cli-git` on Arch Linux using AUR: (`yay -S osc-cli-git`)
+
+#### Note:
+
+if you have this error (or one similar about fuse):
+```
+fuse: failed to exec fusermount: No such file or directory
+
+Cannot mount AppImage, please check your FUSE setup.
+You might still be able to extract the contents of this AppImage
+if you run it with the --appimage-extract option.
+See https://github.com/AppImage/AppImageKit/wiki/FUSE
+for more information
+open dir error: No such file or directory
+```
+
+You can either install fuse yourself, or execute the appimage with `--appimage-extract-and-run` option
+
+Example:
+```
+./osc-cli-x86_64.AppImage --appimage-extract-and-run osc-cli api ReadImages --profile=my
+```
+
+using `appimage-extract-and-run` extract the content of the AppImage in a temporary directory and execute it,
+this operation is a **lot** slower than using fuse, and the fuse solution should be use if posible.
+
+
+### Installing on Windows
+
+osc-cli is pre-packaged for windows:
+- Download `osc-cli-x86_64.zip` from latest version in [releases](https://github.com/outscale/osc-cli/releases).
+- Extract zip archive and run `osc-cli.exe`
+
+Note that some antivirus may consider some files as a virus. Those are false positive.
+If you are worried about it, consider installing osc-cli from Python Package (see below).
+
+### Installing from Python package
 
 You can get the package from [pypi](https://pypi.org/project/osc-sdk/):
 ```
 pip3 install osc-sdk
 ```
 
 If you are using Microsoft Windows, see [how to setup osc-cli on Windows](windows-setup.md).
@@ -37,26 +86,23 @@
 
 The CLI requires a configuration file in `~/.osc/config.json` The content must be a JSON whose contents look like this:
 /!\ the old configuration path using `.osc_sdk` folder is **deprecated**. Please use the new one with `.osc`.
 ```json
 {"default":
     {"access_key": "MYACCESSKEY",
      "secret_key": "MYSECRETKEY",
-     "host": "outscale.com",
-     "https": true,
-     "method": "POST",
-     "region_name": "eu-west-2"
+     "region": "eu-west-2"
     },
   "us":
     {"access_key": "MYACCESSKEY",
      "secret_key": "MYSECRETKEY",
      "host": "outscale.com",
      "https": true,
      "method": "POST",
-     "region_name": "us-east-2"
+     "region": "us-east-2"
     }
 }
 ```
 You can add several profiles for different regions or users.
 
 Optional parameters can be applied to each profile :
 * client_certificate: if you need additional security, your pem must include your private key and your certificate
@@ -66,20 +112,38 @@
 {"default":
     {"access_key": "MYACCESSKEY",
      "secret_key": "MYSECRETKEY",
      "client_certificate" : "path_to_your_pem",
      "host": "outscale.com",
      "https": true,
      "method": "POST",
-     "region_name": "eu-west-2",
+     "region": "eu-west-2",
      "version": "2018-11-19"
     }
 }
 ```
 
+## Activate bash-completion
+
+### Activate the completion for the current bash session
+
+```
+source <(osc-cli --bash_completion)
+```
+
+### Generate the file to add it in your bach rc:
+```
+osc-cli --bash_completion > ~/.osc/cli-completion.bash
+```
+then in your bashrc add:
+
+```
+source ~/.osc/cli-completion.bash
+```
+
 ## Usage
 
 ```
 osc-cli SERVICE CALL [PROFILE] [CALL-PARAMETERS]
 ```
 or
 ```
```

### Comparing `osc-sdk-1.8.0/osc_sdk/sdk.py` & `osc-sdk-1.9.0/osc_sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import base64
 import datetime
 import hashlib
 import hmac
 import json
 import logging
+import os
 import re
+import sys
 import urllib.parse
 from dataclasses import InitVar, dataclass, field
 from pathlib import Path
 from typing import Any, Dict, List, Mapping, Optional, Set, Tuple, Union, cast
 
 import defusedxml.ElementTree as ET
 import fire
@@ -29,15 +31,15 @@
 DEFAULT_PROFILE = "default"
 DEFAULT_REGION = "eu-west-2"
 DEFAULT_VERSION = datetime.date.today().strftime("%Y-%m-%d")
 
 DEFAULT_HOST = "outscale.com"
 
 METHODS_SUPPORTED = {"GET", "POST"}
-SDK_VERSION = "1.8.0"
+SDK_VERSION = "1.9.0"
 SSL_VERIFY = True
 SUCCESS_CODES = {200, 201, 202, 203, 204}
 USER_AGENT = "osc_sdk " + SDK_VERSION
 
 logger = logging.getLogger("osc_sdk")
 
 
@@ -52,42 +54,59 @@
         "ReadNetAccessPointServices",
         "ReadProductTypes",
         "ReadPublicIpRanges",
         "ReadRegions",
         "ReadVmTypes",
         "ResetAccountPassword",
         "SendResetPasswordEmail",
+        "ReadPublicCatalog",
     },
     "icu": {
         "AuthenticateAccount",
         "ResetAccountPassword",
         "SendResetPasswordEmail",
         "ReadPublicCatalog",
         "CheckSignature",
     },
     "fcu": {
         "DescribeRegions",
         "ReadPublicIpRanges",
     },
 }
 
+dir_path = os.path.join(os.path.dirname(__file__))
+BASH_COMPLETION_PATH = os.path.abspath("{}/osc-cli-completion.bash".format(dir_path))
+
 
 class Configuration(TypedDict):
     method: str
     access_key: str
     secret_key: str
     version: str
     https: bool
     region_name: str
     ssl_verify: bool
     client_certificate: str
     endpoint: str
     host: str
 
 
+DEFAULT_CONF = cast(
+    Configuration,
+    {
+        "method": "POST",
+        "https": True,
+        "region_name": DEFAULT_REGION,
+        "ssl_verify": True,
+        "version": DEFAULT_VERSION,
+        "host": DEFAULT_HOST,
+    },
+)
+
+
 class PasswordParams(TypedDict, total=False):
     AuthenticationMethod: str
     Login: Optional[str]
     Password: Optional[str]
 
 
 class ResponseContent(Dict):
@@ -563,15 +582,18 @@
     def get_parameters(
         self, data: Union[CallParameters, List[CallParameters]], prefix: str = ""
     ) -> CallParameters:
         if not isinstance(data, dict):
             raise RuntimeError("Parameters lists are not supported")
 
         # Specific to ICU
-        if self.authentication_method == "accesskey":
+        if (
+            self.authentication_method == "accesskey"
+            or self.authentication_method == None
+        ):
             data.update({"AuthenticationMethod": "accesskey"})
 
         filters = self.get_filters(data)
         data = {k: v for k, v in data.items() if not k.startswith("Filters.")}
         return {"Action": prefix, "Filters": filters, "Version": self.version, **data}
 
     def get_filters(self, data: CallParameters) -> List[Tag]:
@@ -684,15 +706,15 @@
 
 
 def get_conf(profile: str) -> Configuration:
     # Check which conf_path is used.
     conf_path = next((path for path in CONF_PATHS if path.exists()), None)
 
     if not conf_path:
-        raise RuntimeError("No configuration file found in home folder")
+        return DEFAULT_CONF
 
     json_profiles = json.loads(conf_path.read_text())
     # convert region to region_name in json to fit Mapping
     for v in json_profiles:
         json_profile = json_profiles[v]
         if "region" in json_profile:
 
@@ -706,30 +728,32 @@
             if not "region_name" in json_profile:
                 json_profile["region_name"] = json_profile["region"]
             del json_profile["region"]
     conf = cast(Mapping[str, Configuration], json_profiles)
     try:
         return conf[profile]
     except KeyError:
-        raise RuntimeError(f"Profile {profile} not found in configuration file")
+        return DEFAULT_CONF
 
 
 def call_need_auth(service: str, call: str) -> bool:
     return call not in NO_AUTH_CALLS.get(service, set())
 
 
 def api_connect(
     service: str,
     call: str,
     profile: str = DEFAULT_PROFILE,
     login: Optional[str] = None,
     password: Optional[str] = None,
     authentication_method: Optional[str] = None,
+    bash_completion: bool = False,
     **kwargs: CallParameters,
 ):
+
     calls = {
         "api": OSCCall,
         "directlink": DirectLinkCall,
         "eim": EimCall,
         "fcu": FcuCall,
         "icu": IcuCall,
         "lbu": LbuCall,
@@ -741,13 +765,25 @@
     )
     handler.make_request(call, **kwargs)
     if handler.response:
         print(json.dumps(handler.response, indent=4))
 
 
 def main():
+    argc = len(sys.argv)
+    argv = sys.argv
+
+    if argc > 1:
+        for i in range(1, argc):
+            a = argv[i]
+            if a == "--bash_completion":
+                f = open(BASH_COMPLETION_PATH, "r")
+                print(f.read())
+                sys.exit()
+                return 0
+
     logging.basicConfig(level=logging.ERROR)
     fire.Fire(api_connect)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `osc-sdk-1.8.0/osc_sdk/test_auth.py` & `osc-sdk-1.9.0/osc_sdk/test_auth.py`

 * *Files identical despite different names*

### Comparing `osc-sdk-1.8.0/osc_sdk/test_errors.py` & `osc-sdk-1.9.0/osc_sdk/test_errors.py`

 * *Files identical despite different names*

### Comparing `osc-sdk-1.8.0/osc_sdk/test_noauth.py` & `osc-sdk-1.9.0/osc_sdk/test_noauth.py`

 * *Files identical despite different names*

### Comparing `osc-sdk-1.8.0/osc_sdk.egg-info/PKG-INFO` & `osc-sdk-1.9.0/osc_sdk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: osc-sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Outscale API SDK and CLI
 Home-page: https://github.com/outscale/osc-cli
 Author: Outscale SAS
 Author-email: contact@outscale.com
 License: BSD
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,17 +23,66 @@
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Getting Started
 
 ### Prerequisites
 
-You will need [Python 3.5+](https://www.python.org/) or later. Earlier versions including Python 2 are not supported.
+You will need [Python 3.6+](https://www.python.org/) or later. Earlier versions including Python 2 are not supported.
 
-### Installing from package
+### Installing on Macos
+
+osc-cli is available on [brew](https://formulae.brew.sh/formula/osc-cli).
+
+### Installing on Linux
+
+osc-cli is pre-packaged for Linux as a standalone [AppImage](https://appimage.org/).
+- Download `osc-cli-x86_64.AppImage` from latest version in [releases](https://github.com/outscale/osc-cli/releases).
+- Allow file to be executed by running `chmod a+x osc-cli-x86_64.AppImage`
+- Run osc-cli: `./osc-cli-x86_64.AppImage`
+
+Optionally, you can install it for all users: `sudo mv osc-cli-x86_64.AppImage /usr/local/bin/osc-cli` and just run `osc-cli`.
+
+you can also install `osc-cli-git` on Arch Linux using AUR: (`yay -S osc-cli-git`)
+
+#### Note:
+
+if you have this error (or one similar about fuse):
+```
+fuse: failed to exec fusermount: No such file or directory
+
+Cannot mount AppImage, please check your FUSE setup.
+You might still be able to extract the contents of this AppImage
+if you run it with the --appimage-extract option.
+See https://github.com/AppImage/AppImageKit/wiki/FUSE
+for more information
+open dir error: No such file or directory
+```
+
+You can either install fuse yourself, or execute the appimage with `--appimage-extract-and-run` option
+
+Example:
+```
+./osc-cli-x86_64.AppImage --appimage-extract-and-run osc-cli api ReadImages --profile=my
+```
+
+using `appimage-extract-and-run` extract the content of the AppImage in a temporary directory and execute it,
+this operation is a **lot** slower than using fuse, and the fuse solution should be use if posible.
+
+
+### Installing on Windows
+
+osc-cli is pre-packaged for windows:
+- Download `osc-cli-x86_64.zip` from latest version in [releases](https://github.com/outscale/osc-cli/releases).
+- Extract zip archive and run `osc-cli.exe`
+
+Note that some antivirus may consider some files as a virus. Those are false positive.
+If you are worried about it, consider installing osc-cli from Python Package (see below).
+
+### Installing from Python package
 
 You can get the package from [pypi](https://pypi.org/project/osc-sdk/):
 ```
 pip3 install osc-sdk
 ```
 
 If you are using Microsoft Windows, see [how to setup osc-cli on Windows](windows-setup.md).
@@ -57,26 +105,23 @@
 
 The CLI requires a configuration file in `~/.osc/config.json` The content must be a JSON whose contents look like this:
 /!\ the old configuration path using `.osc_sdk` folder is **deprecated**. Please use the new one with `.osc`.
 ```json
 {"default":
     {"access_key": "MYACCESSKEY",
      "secret_key": "MYSECRETKEY",
-     "host": "outscale.com",
-     "https": true,
-     "method": "POST",
-     "region_name": "eu-west-2"
+     "region": "eu-west-2"
     },
   "us":
     {"access_key": "MYACCESSKEY",
      "secret_key": "MYSECRETKEY",
      "host": "outscale.com",
      "https": true,
      "method": "POST",
-     "region_name": "us-east-2"
+     "region": "us-east-2"
     }
 }
 ```
 You can add several profiles for different regions or users.
 
 Optional parameters can be applied to each profile :
 * client_certificate: if you need additional security, your pem must include your private key and your certificate
@@ -86,20 +131,38 @@
 {"default":
     {"access_key": "MYACCESSKEY",
      "secret_key": "MYSECRETKEY",
      "client_certificate" : "path_to_your_pem",
      "host": "outscale.com",
      "https": true,
      "method": "POST",
-     "region_name": "eu-west-2",
+     "region": "eu-west-2",
      "version": "2018-11-19"
     }
 }
 ```
 
+## Activate bash-completion
+
+### Activate the completion for the current bash session
+
+```
+source <(osc-cli --bash_completion)
+```
+
+### Generate the file to add it in your bach rc:
+```
+osc-cli --bash_completion > ~/.osc/cli-completion.bash
+```
+then in your bashrc add:
+
+```
+source ~/.osc/cli-completion.bash
+```
+
 ## Usage
 
 ```
 osc-cli SERVICE CALL [PROFILE] [CALL-PARAMETERS]
 ```
 or
 ```
@@ -179,9 +242,7 @@
 ```bash
 osc-cli icu ListAccessKeys --authentication-method=password --login youremail@company.com --password=Y0URpAssOrd
 ```
 ## Contributing
 OSC-CLI is an **open source software** licensed under **BSD-3-Clause.**
 
 Patches and discussions are welcome about bugs you've found or features you think are missing. If you would like to help making **osc-cli** better, take a look to [CONTRIBUTING.md](https://github.com/outscale/osc-cli/blob/master/CONTRIBUTING.md) file.
-
-
```

### Comparing `osc-sdk-1.8.0/setup.py` & `osc-sdk-1.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import find_packages, setup
 
 setup(
     name="osc-sdk",
-    version="1.8.0",
+    version="1.9.0",
     packages=find_packages(),
     author="Outscale SAS",
     author_email="contact@outscale.com",
     description="Outscale API SDK and CLI",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
+    include_package_data=True,
     license="BSD",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

