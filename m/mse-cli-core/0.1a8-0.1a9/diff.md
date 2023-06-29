# Comparing `tmp/mse_cli_core-0.1a8.tar.gz` & `tmp/mse_cli_core-0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_cli_core-0.1a8.tar", last modified: Mon Jun 26 07:06:00 2023, max compression
+gzip compressed data, was "mse_cli_core-0.1a9.tar", last modified: Tue Jun 27 11:55:16 2023, max compression
```

## Comparing `mse_cli_core-0.1a8.tar` & `mse_cli_core-0.1a9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:06:00.401110 mse_cli_core-0.1a8/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 07:06:00.401110 mse_cli_core-0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-26 07:06:00.405110 mse_cli_core-0.1a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:06:00.393110 mse_cli_core-0.1a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:06:00.397110 mse_cli_core-0.1a8/src/mse_cli_core/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/clock_tick.py
--rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/enclave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/test_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:06:00.401110 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:06:00.401110 mse_cli_core-0.1a8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_boostrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:55:16.548452 mse_cli_core-0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-27 11:55:16.548452 mse_cli_core-0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-27 11:55:16.548452 mse_cli_core-0.1a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:55:16.544453 mse_cli_core-0.1a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:55:16.548452 mse_cli_core-0.1a9/src/mse_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/clock_tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/src/mse_cli_core/test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:55:16.548452 mse_cli_core-0.1a9/src/mse_cli_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-27 11:55:16.000000 mse_cli_core-0.1a9/src/mse_cli_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-27 11:55:16.000000 mse_cli_core-0.1a9/src/mse_cli_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:55:16.000000 mse_cli_core-0.1a9/src/mse_cli_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-27 11:55:16.000000 mse_cli_core-0.1a9/src/mse_cli_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 11:55:16.000000 mse_cli_core-0.1a9/src/mse_cli_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:55:16.000000 mse_cli_core-0.1a9/src/mse_cli_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:55:16.548452 mse_cli_core-0.1a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/tests/test_boostrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/tests/test_ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/tests/test_no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/tests/test_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-27 11:54:44.000000 mse_cli_core-0.1a9/tests/test_test_docker.py
```

### Comparing `mse_cli_core-0.1a8/PKG-INFO` & `mse_cli_core-0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_cli_core
-Version: 0.1a8
+Version: 0.1a9
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a8/setup.cfg` & `mse_cli_core-0.1a9/setup.cfg`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/setup.py` & `mse_cli_core-0.1a9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     description="Utils for MicroService Encryption Python CLIs",
     packages=find_packages("src"),
     package_dir={"": "src"},
     zip_safe=True,
     install_requires=[
         "cryptography>=41.0.1,<42.0.0",
         "docker>=6.0.1,<7.0.0",
-        "intel-sgx-ra==2.0a11",
+        "intel-sgx-ra==2.0a12",
         "pydantic>=1.10.2,<2.0.0",
         "requests>=2.31.0,<3.0.0",
         "toml>=0.10.2,<0.11.0",
     ],
     setup_requires=["wheel"],
     tests_require=["pytest>=7.2.0,<7.3.0"],
     classifiers=[
```

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core/base64.py` & `mse_cli_core-0.1a9/src/mse_cli_core/base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core/bootstrap.py` & `mse_cli_core-0.1a9/src/mse_cli_core/bootstrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core/clock_tick.py` & `mse_cli_core-0.1a9/src/mse_cli_core/clock_tick.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core/conf.py` & `mse_cli_core-0.1a9/src/mse_cli_core/conf.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core/enclave.py` & `mse_cli_core-0.1a9/src/mse_cli_core/enclave.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core/fs.py` & `mse_cli_core-0.1a9/src/mse_cli_core/fs.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core/ignore_file.py` & `mse_cli_core-0.1a9/src/mse_cli_core/ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core/no_sgx_docker.py` & `mse_cli_core-0.1a9/src/mse_cli_core/no_sgx_docker.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
 from mse_cli_core.sgx_docker import SgxDockerConfig
 
 
 class NoSgxDockerConfig(BaseModel):
     """Definition of an mse docker running on a non-sgx hardware."""
 
-    host: str
+    subject_alternative_name: str
     expiration_date: Optional[int]
     size: int
     app_id: UUID
     application: str
 
     app_mountpoint: ClassVar[str] = "/opt/input"
     entrypoint: ClassVar[str] = "mse-run"
 
     def cmd(self) -> List[str]:
         """Serialize the docker command args."""
         command = [
             "--size",
             f"{self.size}M",
             "--san",
-            str(self.host),
+            str(self.subject_alternative_name),
             "--id",
             str(self.app_id),
             "--application",
             self.application,
             "--dry-run",
         ]
 
@@ -50,13 +50,13 @@
             }
         }
 
     @staticmethod
     def from_sgx(docker_config: SgxDockerConfig):
         """Load from a SgxDockerConfig object."""
         return NoSgxDockerConfig(
-            host=docker_config.host,
+            subject_alternative_name=docker_config.subject_alternative_name,
             expiration_date=docker_config.expiration_date,
             size=docker_config.size,
             app_id=docker_config.app_id,
             application=docker_config.application,
         )
```

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core/sgx_docker.py` & `mse_cli_core-0.1a9/src/mse_cli_core/sgx_docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 class SgxDockerConfig(BaseModel):
     """Definition of an mse docker running on a SGX hardware."""
 
     size: int
     host: str
     port: int
     app_id: UUID
+    subject_alternative_name: str
     expiration_date: int
     app_dir: Path
     application: str
     healthcheck: str
     signer_key: Path
 
     signer_key_mountpoint: ClassVar[str] = "/root/.config/gramine/enclave-key.pem"
@@ -27,26 +28,26 @@
 
     def cmd(self) -> List[str]:
         """Serialize the docker command args."""
         return [
             "--size",
             f"{self.size}M",
             "--san",
-            str(self.host),
+            str(self.subject_alternative_name),
             "--id",
             str(self.app_id),
             "--application",
             self.application,
             "--expiration",
             str(self.expiration_date),
         ]
 
     def ports(self) -> Dict[str, Tuple[str, str]]:
         """Define the docker ports."""
-        return {"443/tcp": ("127.0.0.1", str(self.port))}
+        return {"443/tcp": (self.host, str(self.port))}
 
     def labels(self) -> Dict[str, str]:
         """Define the docker labels."""
         return {
             SgxDockerConfig.docker_label: "1",
             "healthcheck_endpoint": self.healthcheck,
         }
@@ -110,15 +111,16 @@
                 continue
 
             dataMap[key] = cmd[i + 1]
             i += 2
 
         return SgxDockerConfig(
             size=int(dataMap["size"][:-1]),
-            host=dataMap["san"],
+            host=port["443/tcp"][0]["HostIp"],
+            subject_alternative_name=dataMap["san"],
             app_id=UUID(dataMap["id"]),
             expiration_date=int(dataMap["expiration"]),
             app_dir=Path(app["Source"]),
             application=dataMap["application"],
             port=int(port["443/tcp"][0]["HostPort"]),
             healthcheck=docker_labels["healthcheck_endpoint"],
             signer_key=Path(signer_key["Source"]),
```

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core/spinner.py` & `mse_cli_core-0.1a9/src/mse_cli_core/spinner.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core/test_docker.py` & `mse_cli_core-0.1a9/src/mse_cli_core/test_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core.egg-info/PKG-INFO` & `mse_cli_core-0.1a9/src/mse_cli_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-cli-core
-Version: 0.1a8
+Version: 0.1a9
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a8/src/mse_cli_core.egg-info/SOURCES.txt` & `mse_cli_core-0.1a9/src/mse_cli_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/tests/test_base64.py` & `mse_cli_core-0.1a9/tests/test_base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/tests/test_boostrap.py` & `mse_cli_core-0.1a9/tests/test_boostrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/tests/test_conf.py` & `mse_cli_core-0.1a9/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/tests/test_ignore_file.py` & `mse_cli_core-0.1a9/tests/test_ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a8/tests/test_no_sgx_docker.py` & `mse_cli_core-0.1a9/tests/test_no_sgx_docker.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 from mse_cli_core.no_sgx_docker import NoSgxDockerConfig
 from mse_cli_core.sgx_docker import SgxDockerConfig
 
 
 def test_from_sgx():
     """Test the `from_sgx` method."""
     ref_conf = NoSgxDockerConfig(
-        host="localhost",
+        subject_alternative_name="localhost",
         expiration_date=1714058115,
         size=4096,
         app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
         application="app:app",
     )
 
     conf = NoSgxDockerConfig.from_sgx(
         SgxDockerConfig(
             size=4096,
             host="localhost",
             port=7788,
+            subject_alternative_name="localhost",
             app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
             expiration_date=1714058115,
             app_dir="/home/cosmian/workspace/sgx_operator/",
             application="app:app",
             healthcheck="/health",
             signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
         )
@@ -32,15 +33,15 @@
 
     assert conf == ref_conf
 
 
 def test_volumes():
     """Test `volumes` function."""
     ref_conf = NoSgxDockerConfig(
-        host="localhost",
+        subject_alternative_name="localhost",
         expiration_date=1714058115,
         size=4096,
         app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
         application="app:app",
     )
 
     assert ref_conf.volumes(Path("/tmp/")) == {
@@ -50,15 +51,15 @@
         }
     }
 
 
 def test_cmd():
     """Test `cmd` function."""
     ref_conf = NoSgxDockerConfig(
-        host="localhost",
+        subject_alternative_name="localhost",
         expiration_date=1714058115,
         size=4096,
         app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
         application="app:app",
     )
 
     assert ref_conf.cmd() == [
@@ -72,15 +73,15 @@
         "app:app",
         "--dry-run",
         "--expiration",
         "1714058115",
     ]
 
     ref_conf = NoSgxDockerConfig(
-        host="localhost",
+        subject_alternative_name="localhost",
         size=4096,
         app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
         application="app:app",
     )
 
     assert ref_conf.cmd() == [
         "--size",
```

### Comparing `mse_cli_core-0.1a8/tests/test_sgx_docker.py` & `mse_cli_core-0.1a9/tests/test_sgx_docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 from mse_cli_core.sgx_docker import SgxDockerConfig
 
 
 def test_load():
     """Test `load` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
-        host="myapp.fr",
+        host="0.0.0.0",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
+        subject_alternative_name="myapp.fr",
         expiration_date=1714639412,
         app_dir="/home/cosmian/workspace/sgx_operator/",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
 
     conf = SgxDockerConfig.load(
         docker_labels={"healthcheck_endpoint": "/health", "mse-home": "1"},
         docker_attrs={
             "HostConfig": {
                 "PortBindings": {
-                    "443/tcp": [{"HostIp": "127.0.0.1", "HostPort": "7788"}]
+                    "443/tcp": [{"HostIp": "0.0.0.0", "HostPort": "7788"}]
                 },
             },
             "Config": {
                 "Cmd": [
                     "--size",
                     "4096M",
                     "--san",
@@ -72,34 +73,36 @@
     assert conf == ref_conf
 
 
 def test_labels():
     """Test `labels` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
-        host="myapp.fr",
+        host="0.0.0.0",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
+        subject_alternative_name="myapp.fr",
         expiration_date=1714639412,
         app_dir="/home/cosmian/workspace/sgx_operator/",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
 
     assert ref_conf.labels() == {"mse-home": "1", "healthcheck_endpoint": "/health"}
 
 
 def test_devices():
     """Test `devices` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
-        host="myapp.fr",
+        host="0.0.0.0",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
+        subject_alternative_name="myapp.fr",
         expiration_date=1714639412,
         app_dir="/home/cosmian/workspace/sgx_operator/",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
 
@@ -111,34 +114,36 @@
     ]
 
 
 def test_ports():
     """Test `ports` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
-        host="myapp.fr",
+        host="0.0.0.0",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
+        subject_alternative_name="myapp.fr",
         expiration_date=1714639412,
         app_dir="/home/cosmian/workspace/sgx_operator/code.tar",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
 
-    assert ref_conf.ports() == {"443/tcp": ("127.0.0.1", "7788")}
+    assert ref_conf.ports() == {"443/tcp": ("0.0.0.0", "7788")}
 
 
 def test_volumes():
     """Test `volumes` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
-        host="myapp.fr",
+        host="0.0.0.0",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
+        subject_alternative_name="myapp.fr",
         expiration_date=1714639412,
         app_dir="/home/cosmian/workspace/sgx_operator/",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
 
@@ -158,17 +163,18 @@
     }
 
 
 def test_cmd():
     """Test `cmd` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
-        host="myapp.fr",
+        host="0.0.0.0",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
+        subject_alternative_name="myapp.fr",
         expiration_date=1714639412,
         app_dir="/home/cosmian/workspace/sgx_operator/",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
```

### Comparing `mse_cli_core-0.1a8/tests/test_test_docker.py` & `mse_cli_core-0.1a9/tests/test_test_docker.py`

 * *Files identical despite different names*

