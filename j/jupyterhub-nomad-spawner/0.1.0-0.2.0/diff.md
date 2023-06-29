# Comparing `tmp/jupyterhub-nomad-spawner-0.1.0.tar.gz` & `tmp/jupyterhub-nomad-spawner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-nomad-spawner-0.1.0.tar", max compression
+gzip compressed data, was "jupyterhub-nomad-spawner-0.2.0.tar", max compression
```

## Comparing `jupyterhub-nomad-spawner-0.1.0.tar` & `jupyterhub-nomad-spawner-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3810 2022-09-13 18:34:31.216078 jupyterhub-nomad-spawner-0.1.0/README.md
--rw-r--r--   0        0        0       22 2022-09-13 18:35:30.061573 jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/__init__.py
--rw-r--r--   0        0        0     1001 2022-09-13 18:34:31.220079 jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/consul/consul_service.py
--rw-r--r--   0        0        0     1111 2022-09-13 18:34:31.220079 jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/job_factory.py
--rw-r--r--   0        0        0      630 2022-09-13 18:34:31.220079 jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/job_options_factory.py
--rw-r--r--   0        0        0        0 2022-09-13 18:34:31.220079 jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/nomad/__init__.py
--rw-r--r--   0        0        0    61041 2022-09-13 18:34:31.220079 jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/nomad/nomad_model.py
--rw-r--r--   0        0        0     4065 2022-09-13 18:34:31.220079 jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/nomad/nomad_service.py
--rw-r--r--   0        0        0    19605 2022-09-13 18:34:31.220079 jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/spawner.py
--rw-r--r--   0        0        0     2874 2022-09-13 18:34:31.220079 jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/templates/form.html.j2
--rw-r--r--   0        0        0     1997 2022-09-13 18:34:31.220079 jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/templates/job.hcl.j2
--rw-r--r--   0        0        0     1355 2022-09-13 18:35:30.061573 jupyterhub-nomad-spawner-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5161 1970-01-01 00:00:00.000000 jupyterhub-nomad-spawner-0.1.0/setup.py
--rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 jupyterhub-nomad-spawner-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3788 2023-06-29 20:19:18.872660 jupyterhub-nomad-spawner-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-29 20:20:11.780694 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/__init__.py
+-rw-r--r--   0        0        0     1001 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/consul/consul_service.py
+-rw-r--r--   0        0        0     1715 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/job_factory.py
+-rw-r--r--   0        0        0      630 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/job_options_factory.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/nomad/__init__.py
+-rw-r--r--   0        0        0    61041 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/nomad/nomad_model.py
+-rw-r--r--   0        0        0     4780 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/nomad/nomad_service.py
+-rw-r--r--   0        0        0    20851 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/spawner.py
+-rw-r--r--   0        0        0     2874 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/templates/form.html.j2
+-rw-r--r--   0        0        0     2045 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/templates/job.hcl.j2
+-rw-r--r--   0        0        0     1435 2023-06-29 20:20:11.776694 jupyterhub-nomad-spawner-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5112 1970-01-01 00:00:00.000000 jupyterhub-nomad-spawner-0.2.0/setup.py
+-rw-r--r--   0        0        0     4442 1970-01-01 00:00:00.000000 jupyterhub-nomad-spawner-0.2.0/PKG-INFO
```

### Comparing `jupyterhub-nomad-spawner-0.1.0/README.md` & `jupyterhub-nomad-spawner-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 ## Show Case
 https://user-images.githubusercontent.com/1607547/182332760-b0f96ba2-faa8-47b6-9bd7-db93b8d31356.mp4
 
 
 TODOs:
 - Document setup
-- Extend for policies
 - Namespace support
 
 
 ## Usage
 
 ### Config
 ```python
```

### Comparing `jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/consul/consul_service.py` & `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/consul/consul_service.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/job_factory.py` & `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/job_factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,18 @@
+import os
 from enum import Enum
 from typing import Dict, List, Optional
 
-from jinja2 import Environment, PackageLoader, select_autoescape
+from jinja2 import (
+    BaseLoader,
+    Environment,
+    FileSystemLoader,
+    PackageLoader,
+    select_autoescape,
+)
 from pydantic import BaseModel
 
 
 class VolumeType(str, Enum):
     host = "host"
     csi = "csi"
 
@@ -17,37 +24,53 @@
     volume_name: str = "notebook-data"
     destination: str = "/home/jovyan/work"
 
     class Config:
         use_enum_values = True
 
 
-class JobData(BaseModel):
+class ServiceProvider(str, Enum):
+    consul = "consul"
+    nomad = "nomad"
+
 
+class JobData(BaseModel):
     job_name: str
     username: str
     notebook_name: Optional[str] = None
 
+    service_provider: ServiceProvider
     service_name: str
     env: Dict = {}
     args: List = []
     datacenters: List[str] = []
     region: str = "global"
 
     image: str = "jupyter/base-notebook:latest"
     memory: int = 512
     cpu: int = 100
 
     volume_data: Optional[JobVolumeData]
     policies: Optional[List[str]]
 
+    class Config:
+        use_enum_values = True
 
-def create_job(job_data: JobData) -> str:
 
-    env = Environment(
-        loader=PackageLoader("jupyterhub_nomad_spawner"), autoescape=select_autoescape()
-    )
+def create_job(job_data: JobData, job_template_path: Optional[str] = None) -> str:
+    # if present, split up and use head as filesystem loader and tail as template name
+    loader: BaseLoader
+
+    if job_template_path:
+        head_tail = os.path.split(job_template_path)
+        loader = FileSystemLoader(head_tail[0])
+        template_name = head_tail[1]
+
+    else:
+        loader = PackageLoader("jupyterhub_nomad_spawner")
+        template_name = "job.hcl.j2"
+    env = Environment(loader=loader, autoescape=select_autoescape())
 
-    template = env.get_template("job.hcl.j2")
+    template = env.get_template(template_name)
     job_hcl = template.render(**job_data.dict())
 
     return job_hcl
```

### Comparing `jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/job_options_factory.py` & `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/job_options_factory.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/nomad/nomad_model.py` & `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/nomad/nomad_model.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/nomad/nomad_service.py` & `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/nomad/nomad_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,17 +25,21 @@
 
 class NomadServiceConfig(BaseModel):
     nomad_addr: AnyHttpUrl = parse_obj_as(AnyHttpUrl, "http://localhost:4646")
     nomad_token: Optional[str]
     tls_config: Optional[NomadTLSConfig] = None
 
 
+class NomadException(Exception):
+    def __init__(self, *args: object) -> None:
+        super().__init__(*args)
+
+
 @define
 class NomadService:
-
     client: AsyncClient
     log: Union[LoggerAdapter, Logger]
 
     async def create_volume(
         self,
         id: str,
         plugin_id: str,
@@ -65,39 +69,37 @@
 
         create_volume_json = request.dict(exclude_none=True, exclude_unset=True)
         result = await self.client.put(
             f"/v1/volume/csi/{id}/create",
             json=create_volume_json,
         )
         if result.is_error:
-            raise Exception(
+            raise NomadException(
                 "Error registering volume."
                 + f" status code: {result.status_code}, content: {result.text}"
             )
         self.log.info("Created volume (status code: %d)", result.status_code)
 
     async def delete_volume(self, id: str):
-
         result = await self.client.post(
             f"/v1/volume/csi/{id}/delete",
         )
         if result.is_error:
-            raise Exception(f"Error deleting volume: {result.text}")
+            raise NomadException(f"Error deleting volume: {result.text}")
 
     async def schedule_job(self, job_hcl: str) -> Tuple[str, str]:
-
         self.log.info("Parsing job: %s", job_hcl)
         job_parse_request = JobsParseRequest(JobHCL=job_hcl, Canonicalize=True)
         parsed_job = await self.client.post(
             "/v1/jobs/parse",
             json=job_parse_request.dict(exclude_none=True, exclude_unset=True),
         )
 
         if parsed_job.is_error:
-            raise Exception(f"Error parsing job: {parsed_job.text}")
+            raise NomadException(f"Error parsing job: {parsed_job.text}")
 
         parsed_job_as_dict = parsed_job.json()
         self.log.info("Got parsed job %s", parsed_job_as_dict)
         job_id = parsed_job_as_dict["ID"]
 
         register_job_as_dict = {
             "EnforceIndex": False,
@@ -107,23 +109,35 @@
             "Job": parsed_job_as_dict,
         }
         job = await self.client.post(
             "/v1/jobs",
             json=register_job_as_dict,
         )
         if job.is_error:
-            raise Exception(f"Error registering job: {job.text}")
+            raise NomadException(f"Error registering job: {job.text}")
 
         return job_id
 
     async def job_status(self, job_id) -> str:
         response = await self.client.get(f"/v1/job/{job_id}")
         if response.is_error:
-            raise Exception(f"Error getting job status: {response.text}")
+            raise NomadException(f"Error getting job status: {response.text}")
 
         job_detail = response.json()
         return job_detail.get("Status", "")
 
     async def delete_job(self, job_id: str):
         response = await self.client.delete(f"/v1/job/{job_id}")
         if response.is_error:
-            raise Exception(f"Error deleting job: {response.text}")
+            raise NomadException(f"Error deleting job: {response.text}")
+
+    async def get_service_address(self, service_name: str) -> Tuple[str, int]:
+        response = await self.client.get(f"/v1/service/{service_name}")
+        if response.is_error:
+            raise NomadException(f"Error reading service: {response.text}")
+
+        services = response.json()
+        if len(services) == 0:
+            raise NomadException(f"Service {service_name} not found")
+        if len(services) > 1:
+            raise NomadException(f"Multiple services found for {service_name}")
+        return str(services[0]["Address"]), int(services[0]["Port"])
```

### Comparing `jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/spawner.py` & `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/spawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from httpx import AsyncClient
 from jupyterhub.spawner import Spawner
 from pydantic import BaseModel
 from tenacity import retry, stop_after_attempt, wait_fixed
 from traitlets import Bool
 from traitlets import Callable as TCallable
 from traitlets import Dict as TDict
+from traitlets import Enum as TEnum
 from traitlets import Int as TInt
 from traitlets import List as TList
 from traitlets import Unicode
 from traitlets import Union as TUnion
 from traitlets import default
 
 from jupyterhub_nomad_spawner.consul.consul_service import (
@@ -310,38 +311,51 @@
         The min csi capacity in bytes
         e.g.
 
         c.NomadSpawner.csi_capacity = 13421772
         """,
     ).tag(config=True)
 
+    service_provider = TEnum(
+        values=["nomad", "consul"],
+        default_value="nomad",
+        help="""
+        The service provider to use
+        """,
+    ).tag(config=True)
+
     @property
     def csi_volume_name(self) -> str:
         if self.notebook_id:
             return f"{self.base_csi_volume_name}-{self.notebook_id}"
         raise ValueError("notebook_id is not set")
 
     @property
     def service_name(self) -> str:
         if self.notebook_id:
             return f"{self.job_name}"
         raise ValueError("notebook_id is not set")
 
-    async def start(self):
+    job_template_path = Unicode(
+        help="""
+        The path to the job template file with jinja2 placeholders
+        see templates/job.hcl.j2
+    """
+    ).tag(config=True)
 
+    async def start(self):
         nomad_service_config = build_nomad_config_from_options(self)
         nomad_httpx_client = build_nomad_httpx_client(nomad_service_config)
         nomad_service = NomadService(client=nomad_httpx_client, log=self.log)
 
         consul_service_config = build_consul_config_from_options(self)
         consul_httpx_client = build_consul_httpx_client(consul_service_config)
         consul_service = ConsulService(client=consul_httpx_client, log=self.log)
 
         try:
-
             notebook_id: str = hashlib.sha1(
                 f"{self.user.name}:{self.name}".encode("utf-8")
             ).hexdigest()[:10]
             self.notebook_id = notebook_id
             self.log.info("server name: %s", self.name)
             env = self.get_env()
             args = self.get_args()
@@ -353,34 +367,41 @@
 
             policies: TList[str] = []
             if callable(self.vault_policies):
                 policies = self.vault_policies(self)
             elif self.vault_policies:
                 policies = self.vault_policies
 
+            self.log.info("scheduling job %s", self.job_name)
             job_hcl = create_job(
-                JobData(
+                job_data=JobData(
                     job_name=self.job_name,
                     username=self.user.name,
                     notebook_name=self.name,
+                    service_provider=self.service_provider,
                     service_name=self.service_name,
                     env=env,
                     args=args,
                     image=self.user_options["image"],
                     datacenters=self.user_options["datacenters"],
                     memory=self.user_options["memory"],
                     volume_data=volume_data,
                     policies=policies,
-                )
+                ),
+                job_template_path=self.job_template_path,
             )
 
             await nomad_service.schedule_job(job_hcl)
             await self._ensure_running(nomad_service=nomad_service)
-
-            service_data = await self.service(consul_service)
+            if self.service_provider == "consul":
+                service_data = await self.address_and_port_from_consul(consul_service)
+            elif self.service_provider == "nomad":
+                service_data = await self.address_and_port_from_nomad(nomad_service)
+            else:
+                raise ValueError("Unknown service provider")
         except Exception as e:
             self.log.exception("Failed to start")
             raise e
 
         finally:
             if nomad_httpx_client is not None:
                 await nomad_httpx_client.aclose()
@@ -436,27 +457,34 @@
             elif status == "dead":
                 raise Exception(f"Job (name={self.job_name}) is dead already")
             else:
                 self.log.info("Waiting for %s...", self.job_name)
                 await asyncio.sleep(5)
 
     @retry(wait=wait_fixed(3), stop=stop_after_attempt(5))
-    async def service(self, consul_service: ConsulService):
-
+    async def address_and_port_from_consul(
+        self, consul_service: ConsulService
+    ) -> Tuple[str, int]:
         self.log.info("Getting service %s from consul", self.service_name)
         nodes = await consul_service.health_service(self.service_name)
 
         address = nodes[0]["Service"]["Address"]
         port = nodes[0]["Service"]["Port"]
 
         # address = "host.docker.internal"
         return (address, port)
 
-    async def poll(self):
+    @retry(wait=wait_fixed(3), stop=stop_after_attempt(5))
+    async def address_and_port_from_nomad(
+        self, nomad_service: NomadService
+    ) -> Tuple[str, int]:
+        self.log.info("Getting service %s from nomad", self.service_name)
+        return await nomad_service.get_service_address(self.job_name)
 
+    async def poll(self):
         nomad_httpx_client = build_nomad_httpx_client(
             build_nomad_config_from_options(self)
         )
 
         nomad_service = NomadService(client=nomad_httpx_client, log=self.log)
         try:
             status = await nomad_service.job_status(self.job_name)
@@ -472,15 +500,14 @@
             self.log.exception("Failed to poll")
             return -1
         finally:
             if nomad_httpx_client:
                 await nomad_httpx_client.aclose()
 
     async def stop(self):
-
         nomad_service_config = build_nomad_config_from_options(self)
         nomad_httpx_client = build_nomad_httpx_client(nomad_service_config)
         nomad_service = NomadService(client=nomad_httpx_client, log=self.log)
 
         try:
             await nomad_service.delete_job(self.job_name)
             self.clear_state()
@@ -582,15 +609,14 @@
         )
         if options.consul_client_key
         else None,
     )
 
 
 def build_nomad_httpx_client(config: NomadServiceConfig) -> AsyncClient:
-
     verify: Union[bool, ssl.SSLContext] = True
     cert: Optional[Tuple[str, str]] = None
     if config.tls_config:
         cert = (
             str(config.tls_config.client_cert.resolve()),
             str(config.tls_config.client_key.resolve()),
         )
@@ -608,15 +634,14 @@
         cert=cert,
         headers={"X-Nomad-Token": config.nomad_token} if config.nomad_token else None,
     )
     return client
 
 
 def build_consul_httpx_client(config: ConsulServiceConfig) -> AsyncClient:
-
     verify: Union[bool, ssl.SSLContext] = True
     cert: Optional[Tuple[str, str]] = None
     if config.tls_config:
         cert = (
             str(config.tls_config.client_cert.resolve()),
             str(config.tls_config.client_key.resolve()),
         )
```

### Comparing `jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/templates/form.html.j2` & `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/templates/form.html.j2`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.1.0/jupyterhub_nomad_spawner/templates/job.hcl.j2` & `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/templates/job.hcl.j2`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,15 @@
                 read_only   = false
             }
             {% endif %}
         }
 
         service {
             name = "{{ service_name }}"
+            provider = "{{ service_provider }}"
             port = "notebook"
              check {
                 name     = "alive"
                 type     = "tcp"
                 interval = "10s"
                 timeout  = "2s"
             }
```

### Comparing `jupyterhub-nomad-spawner-0.1.0/pyproject.toml` & `jupyterhub-nomad-spawner-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 [tool.poetry]
 name = "jupyterhub-nomad-spawner"
-version = "0.1.0"
+version = "0.2.0"
 description = "A JupyterHub Spawner that launches isolated notebooks as job"
 authors = ["Max Fröhlich <maxbruchmann@gmail.com>"]
 readme = "README.md"
+packages = [
+    { include = "jupyterhub_nomad_spawner" },
+]
+
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "~3.10"
 traitlets = "^5.1.1"
-jupyterhub = "^2.2.2"
-notebook = "^6.4.11"
+jupyterhub = "^4.0.1"
+#notebook = "^6.4.11"
 pydantic = "^1.9.0"
 tenacity = "^8.0.1"
-httpx = "^0.23.0"
-attrs = "^21.4.0"
+httpx = "^0.24.0"
+attrs = "^23.1.0"
 Jinja2 = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1"
-black = "^22.3.0"
-flake8 = "^4.0.1"
-pytest-asyncio = "^0.18.3"
+black = "^23.3.0"
+flake8 = "^6.0.0"
+pytest-asyncio = "^0.21.0"
 requests = "^2.27.1"
-datamodel-code-generator = "^0.13.0"
-poethepoet = "^0.16.2"
-mypy = "^0.961"
-respx = "^0.19.2"
+poethepoet = "^0.19.0"
+mypy = "^1.2.0"
+respx = "^0.20.1"
+datamodel-code-generator = "^0.18.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 
 [tool.poetry.plugins."jupyterhub.spawners"]
 "nomad-spawner" = "jupyterhub_nomad_spawner.spawner:NomadSpawner"
 
 [tool.poe.tasks]
-gen-nomad-model = "datamodel-codegen --url https://raw.githubusercontent.com/hashicorp/nomad-openapi/main/v1/openapi.yaml --output jupyterhub_nomad_spawner/nomad_service/nomad_model.py"
+gen-nomad-model = "datamodel-codegen --input-file-type yaml --url https://raw.githubusercontent.com/hashicorp/nomad-openapi/main/v1/openapi.yaml --output jupyterhub_nomad_spawner/nomad/nomad_model.py"
 format = "black ."
 mypy = "mypy ."
 flake8 = "flake8 ."
 check = ["format", "mypy", "flake8"]
 
 
 [tool.mypy]
@@ -48,8 +52,8 @@
     "^jupyterhub_nomad_spawner/nomad/nomad_model\\.py$",
 ]
 [tool.isort]
 profile = "black"
 
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
```

### Comparing `jupyterhub-nomad-spawner-0.1.0/setup.py` & `jupyterhub-nomad-spawner-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,38 +7,37 @@
  'jupyterhub_nomad_spawner.nomad']
 
 package_data = \
 {'': ['*'], 'jupyterhub_nomad_spawner': ['templates/*']}
 
 install_requires = \
 ['Jinja2>=3.1.2,<4.0.0',
- 'attrs>=21.4.0,<22.0.0',
- 'httpx>=0.23.0,<0.24.0',
- 'jupyterhub>=2.2.2,<3.0.0',
- 'notebook>=6.4.11,<7.0.0',
+ 'attrs>=23.1.0,<24.0.0',
+ 'httpx>=0.24.0,<0.25.0',
+ 'jupyterhub>=4.0.1,<5.0.0',
  'pydantic>=1.9.0,<2.0.0',
  'tenacity>=8.0.1,<9.0.0',
  'traitlets>=5.1.1,<6.0.0']
 
 entry_points = \
 {'jupyterhub.spawners': ['nomad-spawner = '
                          'jupyterhub_nomad_spawner.spawner:NomadSpawner']}
 
 setup_kwargs = {
     'name': 'jupyterhub-nomad-spawner',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'A JupyterHub Spawner that launches isolated notebooks as job',
-    'long_description': '# Nomad Jupyter Spawner\n\n\n> **Warning**\n> This project is currently in beta\n\nSpawns a Jupyter Notebook via Jupyterhub.\n\nUsers can select and image, resource and connect it with volumes (csi / host)\n\n```sh\npip install jupyterhub-nomad-spawner\n```\n\n## Show Case\nhttps://user-images.githubusercontent.com/1607547/182332760-b0f96ba2-faa8-47b6-9bd7-db93b8d31356.mp4\n\n\nTODOs:\n- Document setup\n- Extend for policies\n- Namespace support\n\n\n## Usage\n\n### Config\n```python\n\nimport json\nimport os\nimport socket\n\nfrom jupyterhub.auth import DummyAuthenticator\nimport tarfile\nc.JupyterHub.spawner_class = "nomad-spawner"\nc.JupyterHub.bind_url = "http://0.0.0.0:8000"\nc.JupyterHub.hub_bind_url = "http://0.0.0.0:8081"\nc.JupyterHub.hub_connect_url = f"http://{os.environ.get(\'NOMAD_IP_api\')}:{os.environ.get(\'NOMAD_HOST_PORT_api\')}"\n\nc.JupyterHub.allow_named_servers = True\nc.JupyterHub.named_server_limit_per_user = 5\n\nc.JupyterHub.authenticator_class = DummyAuthenticator\n\nc.NomadSpawner.mem_limit = "2G"\nc.NomadSpawner.datacenters = ["dc1", "dc2", "dc3"]\n\n```\n\n\n### Nomad Job\n\n\n```hcl\n\njob "jupyterhub" {\n    type = "service"\n\n    datacenters = ["dc1"]\n\n    group "jupyterhub" {\n\n        network {\n            mode = "host"\n            port "hub" {\n                to = 8000\n                static = 8000\n            }\n            port "api" {\n                to = 8081\n            }\n        }\n        task "jupyterhub" {\n            driver = "docker"\n\n            config {\n                image = "mxab/jupyterhub:1"\n                auth_soft_fail = false\n\n                args = [\n                        "jupyterhub",\n                        "-f",\n                        "/local/jupyterhub_config.py",\n                    ]\n                ports = ["hub", "api"]\n\n            }\n            template {\n                destination = "/local/nomad.env"\n                env = true\n                data = <<EOF\n\nNOMAD_ADDR=http://host.docker.internal:4646\nCONSUL_HTTP_ADDR=http://host.docker.internal:8500\n    EOF\n            }\n            template {\n                destination = "/local/jupyterhub_config.py"\n\n                data = <<EOF\nimport json\nimport os\nimport socket\n\nfrom jupyterhub.auth import DummyAuthenticator\nimport tarfile\nc.JupyterHub.spawner_class = "nomad-spawner"\nc.JupyterHub.bind_url = "http://0.0.0.0:8000"\nc.JupyterHub.hub_bind_url = "http://0.0.0.0:8081"\n\nc.JupyterHub.hub_connect_url = f"http://{os.environ.get(\'NOMAD_IP_api\')}:{os.environ.get(\'NOMAD_HOST_PORT_api\')}"\nc.JupyterHub.log_level = "DEBUG"\nc.ConfigurableHTTPProxy.debug = True\n\n\nc.JupyterHub.allow_named_servers = True\nc.JupyterHub.named_server_limit_per_user = 3\n\nc.JupyterHub.authenticator_class = DummyAuthenticator\n\nc.NomadSpawner.datacenters = ["dc1"]\n\nc.NomadSpawner.mem_limit = "2G"\n\n\nc.NomadSpawner.common_images = ["jupyter/minimal-notebook:2022-08-20"]\n\ndef csi_volume_parameters(spawner):\n    if spawner.user_options["volume_csi_plugin_id"] == "nfs":\n        return {\n            "gid" : "1000",\n            "uid" : "1000"\n        }\n    else:\n        return None\nc.NomadSpawner.csi_volume_parameters = csi_volume_parameters\n\n\ndef vault_policies(spawner):\n    return [f"my-policy-{spawner.user.name}"]\nc.NomadSpawner.vault_policies = vault_policies\n\n                EOF\n\n\n            }\n\n            resources {\n                memory = "512"\n            }\n\n        }\n\n        service {\n            name = "jupyter-hub"\n            port = "hub"\n\n            check {\n                type     = "tcp"\n                interval = "10s"\n                timeout  = "2s"\n            }\n\n        }\n        service {\n            name = "jupyter-hub-api"\n            port = "api"\n            check {\n                type     = "tcp"\n                interval = "10s"\n                timeout  = "2s"\n            }\n\n        }\n    }\n}\n\n\n```\n',
+    'long_description': '# Nomad Jupyter Spawner\n\n\n> **Warning**\n> This project is currently in beta\n\nSpawns a Jupyter Notebook via Jupyterhub.\n\nUsers can select and image, resource and connect it with volumes (csi / host)\n\n```sh\npip install jupyterhub-nomad-spawner\n```\n\n## Show Case\nhttps://user-images.githubusercontent.com/1607547/182332760-b0f96ba2-faa8-47b6-9bd7-db93b8d31356.mp4\n\n\nTODOs:\n- Document setup\n- Namespace support\n\n\n## Usage\n\n### Config\n```python\n\nimport json\nimport os\nimport socket\n\nfrom jupyterhub.auth import DummyAuthenticator\nimport tarfile\nc.JupyterHub.spawner_class = "nomad-spawner"\nc.JupyterHub.bind_url = "http://0.0.0.0:8000"\nc.JupyterHub.hub_bind_url = "http://0.0.0.0:8081"\nc.JupyterHub.hub_connect_url = f"http://{os.environ.get(\'NOMAD_IP_api\')}:{os.environ.get(\'NOMAD_HOST_PORT_api\')}"\n\nc.JupyterHub.allow_named_servers = True\nc.JupyterHub.named_server_limit_per_user = 5\n\nc.JupyterHub.authenticator_class = DummyAuthenticator\n\nc.NomadSpawner.mem_limit = "2G"\nc.NomadSpawner.datacenters = ["dc1", "dc2", "dc3"]\n\n```\n\n\n### Nomad Job\n\n\n```hcl\n\njob "jupyterhub" {\n    type = "service"\n\n    datacenters = ["dc1"]\n\n    group "jupyterhub" {\n\n        network {\n            mode = "host"\n            port "hub" {\n                to = 8000\n                static = 8000\n            }\n            port "api" {\n                to = 8081\n            }\n        }\n        task "jupyterhub" {\n            driver = "docker"\n\n            config {\n                image = "mxab/jupyterhub:1"\n                auth_soft_fail = false\n\n                args = [\n                        "jupyterhub",\n                        "-f",\n                        "/local/jupyterhub_config.py",\n                    ]\n                ports = ["hub", "api"]\n\n            }\n            template {\n                destination = "/local/nomad.env"\n                env = true\n                data = <<EOF\n\nNOMAD_ADDR=http://host.docker.internal:4646\nCONSUL_HTTP_ADDR=http://host.docker.internal:8500\n    EOF\n            }\n            template {\n                destination = "/local/jupyterhub_config.py"\n\n                data = <<EOF\nimport json\nimport os\nimport socket\n\nfrom jupyterhub.auth import DummyAuthenticator\nimport tarfile\nc.JupyterHub.spawner_class = "nomad-spawner"\nc.JupyterHub.bind_url = "http://0.0.0.0:8000"\nc.JupyterHub.hub_bind_url = "http://0.0.0.0:8081"\n\nc.JupyterHub.hub_connect_url = f"http://{os.environ.get(\'NOMAD_IP_api\')}:{os.environ.get(\'NOMAD_HOST_PORT_api\')}"\nc.JupyterHub.log_level = "DEBUG"\nc.ConfigurableHTTPProxy.debug = True\n\n\nc.JupyterHub.allow_named_servers = True\nc.JupyterHub.named_server_limit_per_user = 3\n\nc.JupyterHub.authenticator_class = DummyAuthenticator\n\nc.NomadSpawner.datacenters = ["dc1"]\n\nc.NomadSpawner.mem_limit = "2G"\n\n\nc.NomadSpawner.common_images = ["jupyter/minimal-notebook:2022-08-20"]\n\ndef csi_volume_parameters(spawner):\n    if spawner.user_options["volume_csi_plugin_id"] == "nfs":\n        return {\n            "gid" : "1000",\n            "uid" : "1000"\n        }\n    else:\n        return None\nc.NomadSpawner.csi_volume_parameters = csi_volume_parameters\n\n\ndef vault_policies(spawner):\n    return [f"my-policy-{spawner.user.name}"]\nc.NomadSpawner.vault_policies = vault_policies\n\n                EOF\n\n\n            }\n\n            resources {\n                memory = "512"\n            }\n\n        }\n\n        service {\n            name = "jupyter-hub"\n            port = "hub"\n\n            check {\n                type     = "tcp"\n                interval = "10s"\n                timeout  = "2s"\n            }\n\n        }\n        service {\n            name = "jupyter-hub-api"\n            port = "api"\n            check {\n                type     = "tcp"\n                interval = "10s"\n                timeout  = "2s"\n            }\n\n        }\n    }\n}\n\n\n```\n',
     'author': 'Max Fröhlich',
     'author_email': 'maxbruchmann@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.10,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `jupyterhub-nomad-spawner-0.1.0/PKG-INFO` & `jupyterhub-nomad-spawner-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: jupyterhub-nomad-spawner
-Version: 0.1.0
+Version: 0.2.0
 Summary: A JupyterHub Spawner that launches isolated notebooks as job
 Author: Max Fröhlich
 Author-email: maxbruchmann@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: attrs (>=21.4.0,<22.0.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: jupyterhub (>=2.2.2,<3.0.0)
-Requires-Dist: notebook (>=6.4.11,<7.0.0)
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: jupyterhub (>=4.0.1,<5.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: traitlets (>=5.1.1,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Nomad Jupyter Spawner
 
@@ -35,15 +32,14 @@
 
 ## Show Case
 https://user-images.githubusercontent.com/1607547/182332760-b0f96ba2-faa8-47b6-9bd7-db93b8d31356.mp4
 
 
 TODOs:
 - Document setup
-- Extend for policies
 - Namespace support
 
 
 ## Usage
 
 ### Config
 ```python
```

