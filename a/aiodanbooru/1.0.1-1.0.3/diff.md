# Comparing `tmp/aiodanbooru-1.0.1.tar.gz` & `tmp/aiodanbooru-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodanbooru-1.0.1.tar", last modified: Thu Jun 29 11:18:21 2023, max compression
+gzip compressed data, was "aiodanbooru-1.0.3.tar", last modified: Thu Jun 29 20:37:02 2023, max compression
```

## Comparing `aiodanbooru-1.0.1.tar` & `aiodanbooru-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 11:18:21.944836 aiodanbooru-1.0.1/
--rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3022 2023-06-29 11:18:21.943832 aiodanbooru-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 11:18:21.916307 aiodanbooru-1.0.1/aiodanbooru/
--rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.1/aiodanbooru/__init__.py
--rw-rw-rw-   0        0        0     1523 2023-06-29 10:39:15.000000 aiodanbooru-1.0.1/aiodanbooru/api.py
--rw-rw-rw-   0        0        0     1916 2023-06-29 10:09:01.000000 aiodanbooru-1.0.1/aiodanbooru/models.py
-drwxrwxrwx   0        0        0        0 2023-06-29 11:18:21.941313 aiodanbooru-1.0.1/aiodanbooru.egg-info/
--rw-rw-rw-   0        0        0     3022 2023-06-29 11:18:21.000000 aiodanbooru-1.0.1/aiodanbooru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-29 11:18:21.000000 aiodanbooru-1.0.1/aiodanbooru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 11:18:21.000000 aiodanbooru-1.0.1/aiodanbooru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 11:18:21.000000 aiodanbooru-1.0.1/aiodanbooru.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-29 11:18:21.000000 aiodanbooru-1.0.1/aiodanbooru.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 11:18:21.944836 aiodanbooru-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-06-29 11:14:00.000000 aiodanbooru-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 11:18:21.941313 aiodanbooru-1.0.1/tests/
--rw-rw-rw-   0        0        0     1466 2023-06-29 10:45:36.000000 aiodanbooru-1.0.1/tests/test_api.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:37:02.220804 aiodanbooru-1.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3022 2023-06-29 20:37:02.219763 aiodanbooru-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 20:37:02.212764 aiodanbooru-1.0.3/aiodanbooru/
+-rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.3/aiodanbooru/__init__.py
+-rw-rw-rw-   0        0        0     1668 2023-06-29 20:32:36.000000 aiodanbooru-1.0.3/aiodanbooru/api.py
+-rw-rw-rw-   0        0        0     3140 2023-06-29 20:34:45.000000 aiodanbooru-1.0.3/aiodanbooru/models.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:37:02.217763 aiodanbooru-1.0.3/aiodanbooru.egg-info/
+-rw-rw-rw-   0        0        0     3022 2023-06-29 20:37:02.000000 aiodanbooru-1.0.3/aiodanbooru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-29 20:37:02.000000 aiodanbooru-1.0.3/aiodanbooru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 20:37:02.000000 aiodanbooru-1.0.3/aiodanbooru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 20:37:02.000000 aiodanbooru-1.0.3/aiodanbooru.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-29 20:37:02.000000 aiodanbooru-1.0.3/aiodanbooru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 20:37:02.220804 aiodanbooru-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-06-29 20:36:41.000000 aiodanbooru-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:37:02.218763 aiodanbooru-1.0.3/tests/
+-rw-rw-rw-   0        0        0     1466 2023-06-29 20:35:36.000000 aiodanbooru-1.0.3/tests/test_api.py
```

### Comparing `aiodanbooru-1.0.1/LICENSE` & `aiodanbooru-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.1/PKG-INFO` & `aiodanbooru-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.1
+Version: 1.0.3
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.1/README.md` & `aiodanbooru-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.1/aiodanbooru/api.py` & `aiodanbooru-1.0.3/aiodanbooru/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,18 +21,24 @@
         self, session: aiohttp.ClientSession, endpoint: str, data: dict
     ) -> dict:
         url = self.base_url + endpoint
         async with session.post(url, json=data) as response:
             response.raise_for_status()
             return await response.json()
 
-    async def get_posts(self, tags: List[str], limit: int = 100) -> List[DanbooruPost]:
+    async def get_posts(
+        self, tags: List[str] = None, limit: int = None
+    ) -> List[DanbooruPost]:
         async with aiohttp.ClientSession() as session:
             endpoint = "/posts.json"
-            params = {"tags": " ".join(tags), "limit": str(limit)}
+            params = {}
+            if tags is not None:
+                params["tags"] = " ".join(tags)
+            if limit is not None:
+                params["limit"] = str(limit)
             response = await self._get(session, endpoint, params)
             posts = [DanbooruPost(**post) for post in response]
             return posts
 
     async def get_random_post(self) -> DanbooruPost:
         async with aiohttp.ClientSession() as session:
             endpoint = "/posts/random.json"
```

### Comparing `aiodanbooru-1.0.1/aiodanbooru/models.py` & `aiodanbooru-1.0.3/aiodanbooru/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,95 @@
 from typing import Optional
 
 import aiohttp
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, HttpUrl, validator
 
 
 class DanbooruPost(BaseModel):
     id: int
     uploader_id: int
     approver_id: Optional[int]
     tag_string: str
     tag_string_general: str
     tag_string_artist: str
     tag_string_copyright: str
     tag_string_character: str
     tag_string_meta: str
     rating: Optional[str]
     parent_id: Optional[int]
-    source: Optional[str]
-    md5: str
-    file_url: str
-    large_file_url: str
-    preview_file_url: str
-    file_ext: str
-    file_size: int
-    image_width: int
+    source: Optional[HttpUrl]
+    md5: Optional[str] = Field(None, description="MD5 hash of the media file")
+    file_url: Optional[HttpUrl] = Field(None, description="URL of the media file")
+    large_file_url: Optional[HttpUrl] = Field(
+        None, description="URL of the large version of the media file"
+    )
+    preview_file_url: Optional[HttpUrl] = Field(
+        None, description="URL of the preview version of the media file"
+    )
+    file_ext: Optional[str]
+    file_size: Optional[int]
+    image_width: Optional[int]
     score: int
     fav_count: int
     tag_count_general: int
     tag_count_artist: int
     tag_count_copyright: int
     tag_count_character: int
     tag_count_meta: int
     last_comment_bumped_at: Optional[str]
     last_noted_at: Optional[str]
     has_children: bool
-    image_height: int
+    image_height: Optional[int]
     created_at: str
     updated_at: str
 
+    @validator("source")
+    def validate_source(cls, source):
+        if source is not None and len(source) < 1:
+            raise ValueError("Source must have at least 1 character")
+        return source
+
     class Config:
         extra = "allow"
 
     extension: Optional[str] = Field(None, alias="file_ext")
 
     async def get_media(self, use_large: bool = True) -> bytes:
+        if not self.file_url and not self.large_file_url and self.source:
+            return await self._get_media_from_source()
         url = (
             self.large_file_url if use_large and self.large_file_url else self.file_url
         )
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as response:
                 response.raise_for_status()
                 return await response.read()
 
     @property
     def link(self):
         return f"https://danbooru.donmai.us/posts/{self.id}"
 
     @property
     def media_url(self):
-        return self.large_file_url if self.large_file_url else self.file_url
+        return (
+            self.large_file_url if self.large_file_url else self.file_url or self.source
+        )
 
     def is_video(self) -> bool:
         return self.extension in ["webm", "mp4"]
 
     def is_image(self) -> bool:
         return self.extension in ["jpg", "jpeg", "png", "gif"]
 
     @property
     def filename(self):
         return f"{self.md5}.{self.extension}"
+
+    async def _get_media_from_source(self):
+        async with aiohttp.ClientSession() as session:
+            if self.source.startswith("https://i.pximg.net"):
+                url = self.source.replace("i.pximg.net", "i.pixiv.cat")
+            else:
+                url = self.source
+            async with session.get(url) as response:
+                response.raise_for_status()
+                return await response.read()
```

### Comparing `aiodanbooru-1.0.1/aiodanbooru.egg-info/PKG-INFO` & `aiodanbooru-1.0.3/aiodanbooru.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.1
+Version: 1.0.3
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.1/setup.py` & `aiodanbooru-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiodanbooru",
-    version="1.0.1",
+    version="1.0.3",
     description="A Python library for interacting with the Danbooru API",
     author="lrdcxdes",
     author_email="lordgrief176@email.com",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "aiohttp",
         "pydantic",
```

### Comparing `aiodanbooru-1.0.1/tests/test_api.py` & `aiodanbooru-1.0.3/tests/test_api.py`

 * *Files identical despite different names*

