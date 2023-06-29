# Comparing `tmp/animeworld-1.6.0.tar.gz` & `tmp/animeworld-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animeworld-1.6.0.tar", last modified: Tue Jun 20 16:44:47 2023, max compression
+gzip compressed data, was "animeworld-1.6.1.tar", last modified: Thu Jun 29 10:47:58 2023, max compression
```

## Comparing `animeworld-1.6.0.tar` & `animeworld-1.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:44:47.884548 animeworld-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-20 16:44:39.000000 animeworld-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-20 16:44:47.884548 animeworld-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-20 16:44:39.000000 animeworld-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:44:47.884548 animeworld-1.6.0/animeworld/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/episodio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:44:47.884548 animeworld-1.6.0/animeworld/servers/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/servers/AnimeWorld_Server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/servers/Server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/servers/Streamtape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/servers/YouTube.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:44:47.884548 animeworld-1.6.0/animeworld.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-20 16:44:47.000000 animeworld-1.6.0/animeworld.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-20 16:44:47.000000 animeworld-1.6.0/animeworld.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:44:47.000000 animeworld-1.6.0/animeworld.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 16:44:47.000000 animeworld-1.6.0/animeworld.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 16:44:47.000000 animeworld-1.6.0/animeworld.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:44:47.884548 animeworld-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-20 16:44:39.000000 animeworld-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:47:58.234298 animeworld-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 10:47:44.000000 animeworld-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-29 10:47:58.234298 animeworld-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-29 10:47:44.000000 animeworld-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:47:58.230298 animeworld-1.6.1/animeworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/episodio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:47:58.234298 animeworld-1.6.1/animeworld/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/servers/AnimeWorld_Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/servers/Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/servers/Streamtape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/servers/YouTube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:47:58.234298 animeworld-1.6.1/animeworld.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-29 10:47:58.000000 animeworld-1.6.1/animeworld.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-29 10:47:58.000000 animeworld-1.6.1/animeworld.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:47:58.000000 animeworld-1.6.1/animeworld.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 10:47:58.000000 animeworld-1.6.1/animeworld.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 10:47:58.000000 animeworld-1.6.1/animeworld.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 10:47:58.234298 animeworld-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-29 10:47:44.000000 animeworld-1.6.1/setup.py
```

### Comparing `animeworld-1.6.0/LICENSE` & `animeworld-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.0/animeworld/exceptions.py` & `animeworld-1.6.1/animeworld/exceptions.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.0/animeworld/servers/AnimeWorld_Server.py` & `animeworld-1.6.1/animeworld/servers/AnimeWorld_Server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,81 @@
 from bs4 import BeautifulSoup
 import re
 
 from .Server import *
 from ..utility import HealthCheck
 
 class AnimeWorld_Server(Server):
-	@HealthCheck
-	def fileLink(self) -> str:
-		"""
-		Recupera il link diretto per il download del file dell'episodio.
-
-		```
-		return str # Link del file
-		```
-		"""
-		
-		return self.link.replace('download-file.php?id=', '')
-
-	def fileInfo(self) -> Dict[str,str]:
-		"""
-		Recupera le informazioni del file dell'episodio.
-
-		```
-		return {
-		  "content_type": str, # Tipo del file, es. video/mp4
-		  "total_bytes": int, # Byte totali del file
-		  "last_modified": datetime, # Data e ora dell'ultimo aggiornamento effettuato all'episodio sul server
-		  "server_name": str, # Nome del server
-		  "server_id": int, # ID del server
-		  "url": str # url dell'episodio
-		} 
-		```
-		"""
-
-		return self._fileInfoIn()
-
-	def download(self, title: Optional[str]=None, folder: str='', *, hook: Callable[[Dict], None]=lambda *args:None, opt: List[str]=[]) -> Optional[str]:
-		"""
-		Scarica l'episodio.
-
-		- `title`: Nome con cui verrà nominato il file scaricato.
-		- `folder`: Posizione in cui verrà spostato il file scaricato.
-		- `hook`: Funzione che viene richiamata varie volte durante il download; la funzione riceve come argomento un dizionario con le seguenti chiavi: 
-		  - `total_bytes`: Byte totali da scaricare.
-		  - `downloaded_bytes`: Byte attualmente scaricati.
-		  - `percentage`: Percentuale del progresso di download.
-		  - `speed`: Velocità di download (byte/s)
-		  - `elapsed`: Tempo trascorso dall'inizio del download.
-		  - `eta`: Tempo stimato rimanente per fine del download.
-		  - `status`: 'downloading' | 'finished' | 'aborted'
-		  - `filename`: Nome del file in download.
-		- `opt`: Lista per delle opzioni aggiuntive.
-		  - `'abort'`: Ferma forzatamente il download.
-		
-		```
-		return str # File scaricato
-		```
-		"""
-		if title is None: title = self._defTitle
-		else: title = self._sanitize(title)
-		return self._downloadIn(title,folder,hook=hook,opt=opt)
+    @HealthCheck
+    def fileLink(self) -> str:
+        """
+        Recupera il link diretto per il download del file dell'episodio.
+
+        Returns:
+          Link diretto.
+
+        Example:
+          ```py
+          return str # Link del file
+          ```
+        """
+        
+        return self.link.replace('download-file.php?id=', '')
+
+    def fileInfo(self) -> Dict[str,str]:
+        """
+        Recupera le informazioni del file dell'episodio.
+
+        Returns:
+          Informazioni file episodio.
+
+        Example:
+          ```py
+          return {
+            "content_type": str, # Tipo del file, es. video/mp4
+            "total_bytes": int, # Byte totali del file
+            "last_modified": datetime, # Data e ora dell'ultimo aggiornamento effettuato all'episodio sul server
+            "server_name": str, # Nome del server
+            "server_id": int, # ID del server
+            "url": str # url dell'episodio
+          } 
+          ```
+        """
+
+        return self._fileInfoIn()
+
+    def download(self, title: Optional[str]=None, folder: str='', *, hook: Callable[[Dict], None]=lambda *args:None, opt: List[str]=[]) -> Optional[str]:
+        """
+        Scarica l'episodio.
+
+        Args:
+          title: Nome con cui verrà nominato il file scaricato.
+          folder: Posizione in cui verrà spostato il file scaricato.
+
+        Other parameters:
+          hook: Funzione che viene richiamata varie volte durante il download; la funzione riceve come argomento un dizionario con le seguenti chiavi:\n 
+            - `total_bytes`: Byte totali da scaricare.
+            - `downloaded_bytes`: Byte attualmente scaricati.
+            - `percentage`: Percentuale del progresso di download.
+            - `speed`: Velocità di download (byte/s)
+            - `elapsed`: Tempo trascorso dall'inizio del download.
+            - `eta`: Tempo stimato rimanente per fine del download.
+            - `status`: 'downloading' | 'finished' | 'aborted'
+            - `filename`: Nome del file in download.
+
+          opt: Lista per delle opzioni aggiuntive.\n
+            - `'abort'`: Ferma forzatamente il download.
+        
+        Returns:
+          Nome del file scaricato. 
+        
+        Raises:
+          HardStoppedDownload: Il file in download è stato forzatamente interrotto.
+
+        Example:
+          ```py
+          return str # File scaricato
+          ```
+        """
+        if title is None: title = self._defTitle
+        else: title = self._sanitize(title)
+        return self._downloadIn(title,folder,hook=hook,opt=opt)
```

### Comparing `animeworld-1.6.0/animeworld/servers/Streamtape.py` & `animeworld-1.6.1/animeworld/servers/Streamtape.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,95 @@
 from bs4 import BeautifulSoup
 import re
 
 from .Server import *
 from ..utility import HealthCheck
 
 class Streamtape(Server):
-	@HealthCheck
-	def fileLink(self) -> str:
-		"""
-		Recupera il link diretto per il download del file dell'episodio.
-
-		```
-		return str # Link del file
-		```
-		"""
-		
-		sb_get = SES.get(self.link)
-
-		if sb_get.status_code == 200:
-			soupeddata = BeautifulSoup(sb_get.content, "html.parser")
-
-			raw_link = re.search(r"document\.getElementById\('ideoooolink'\)\.innerHTML = (\".*'\))", soupeddata.prettify()).group(1)
-
-			raw_link = raw_link.replace('"', '').replace("'", "").replace('+', '')
-
-			raw_link_part2 = re.search(r"\((.*?)\)", raw_link).group(1)[4:]
-			raw_link_part1 = re.sub(r"\(.*?\)",'', raw_link)
-
-			mp4_link = 'http:/' + (raw_link_part1 + raw_link_part2).replace(' ', '')
-
-			return mp4_link
-	
-	def fileInfo(self) -> Dict[str,str]:
-		"""
-		Recupera le informazioni del file dell'episodio.
-
-		```
-		return {
-		  "content_type": str, # Tipo del file, es. video/mp4
-		  "total_bytes": int, # Byte totali del file
-		  "last_modified": datetime, # Data e ora dell'ultimo aggiornamento effettuato all'episodio sul server
-		  "server_name": str, # Nome del server
-		  "server_id": int, # ID del server
-		  "url": str # url dell'episodio
-		} 
-		```
-		"""
-
-		return self._fileInfoIn()
-
-	def download(self, title: Optional[str]=None, folder: str='', *, hook: Callable[[Dict], None]=lambda *args:None, opt: List[str]=[]) -> Optional[str]:
-		"""
-		Scarica l'episodio.
-
-		- `title`: Nome con cui verrà nominato il file scaricato.
-		- `folder`: Posizione in cui verrà spostato il file scaricato.
-		- `hook`: Funzione che viene richiamata varie volte durante il download; la funzione riceve come argomento un dizionario con le seguenti chiavi: 
-		  - `total_bytes`: Byte totali da scaricare.
-		  - `downloaded_bytes`: Byte attualmente scaricati.
-		  - `percentage`: Percentuale del progresso di download.
-		  - `speed`: Velocità di download (byte/s)
-		  - `elapsed`: Tempo trascorso dall'inizio del download.
-		  - `eta`: Tempo stimato rimanente per fine del download.
-		  - `status`: 'downloading' | 'finished' | 'aborted'
-		  - `filename`: Nome del file in download.
-		- `opt`: Lista per delle opzioni aggiuntive.
-		  - `'abort'`: Ferma forzatamente il download.
-		
-		```
-		return str # File scaricato
-		```
-		"""
-		if title is None: title = self._defTitle
-		else: title = self._sanitize(title)
-		return self._downloadIn(title,folder,hook=hook,opt=opt)
+    @HealthCheck
+    def fileLink(self) -> str:
+        """
+        Recupera il link diretto per il download del file dell'episodio.
+
+        Returns:
+          Link diretto.
+
+        Example:
+          ```py
+          return str # Link del file
+          ```
+        """
+        
+        sb_get = SES.get(self.link)
+
+        if sb_get.status_code == 200:
+            soupeddata = BeautifulSoup(sb_get.content, "html.parser")
+
+            raw_link = re.search(r"document\.getElementById\('ideoooolink'\)\.innerHTML = (\".*'\))", soupeddata.prettify()).group(1)
+
+            raw_link = raw_link.replace('"', '').replace("'", "").replace('+', '')
+
+            raw_link_part2 = re.search(r"\((.*?)\)", raw_link).group(1)[4:]
+            raw_link_part1 = re.sub(r"\(.*?\)",'', raw_link)
+
+            mp4_link = 'http:/' + (raw_link_part1 + raw_link_part2).replace(' ', '')
+
+            return mp4_link
+    
+    def fileInfo(self) -> Dict[str,str]:
+        """
+        Recupera le informazioni del file dell'episodio.
+
+        Returns:
+          Informazioni file episodio.
+
+        Example:
+          ```py
+          return {
+            "content_type": str, # Tipo del file, es. video/mp4
+            "total_bytes": int, # Byte totali del file
+            "last_modified": datetime, # Data e ora dell'ultimo aggiornamento effettuato all'episodio sul server
+            "server_name": str, # Nome del server
+            "server_id": int, # ID del server
+            "url": str # url dell'episodio
+          } 
+          ```
+        """
+
+        return self._fileInfoIn()
+
+    def download(self, title: Optional[str]=None, folder: str='', *, hook: Callable[[Dict], None]=lambda *args:None, opt: List[str]=[]) -> Optional[str]:
+        """
+        Scarica l'episodio.
+
+        Args:
+          title: Nome con cui verrà nominato il file scaricato.
+          folder: Posizione in cui verrà spostato il file scaricato.
+
+        Other parameters:
+          hook: Funzione che viene richiamata varie volte durante il download; la funzione riceve come argomento un dizionario con le seguenti chiavi:\n 
+            - `total_bytes`: Byte totali da scaricare.
+            - `downloaded_bytes`: Byte attualmente scaricati.
+            - `percentage`: Percentuale del progresso di download.
+            - `speed`: Velocità di download (byte/s)
+            - `elapsed`: Tempo trascorso dall'inizio del download.
+            - `eta`: Tempo stimato rimanente per fine del download.
+            - `status`: 'downloading' | 'finished' | 'aborted'
+            - `filename`: Nome del file in download.
+
+          opt: Lista per delle opzioni aggiuntive.\n
+            - `'abort'`: Ferma forzatamente il download.
+        
+        Returns:
+          Nome del file scaricato. 
+
+        Raises:
+          HardStoppedDownload: Il file in download è stato forzatamente interrotto.
+          
+        Example:
+          ```py
+          return str # File scaricato
+          ```
+        """
+        if title is None: title = self._defTitle
+        else: title = self._sanitize(title)
+        return self._downloadIn(title,folder,hook=hook,opt=opt)
```

### Comparing `animeworld-1.6.0/animeworld/servers/YouTube.py` & `animeworld-1.6.1/animeworld/servers/YouTube.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 from .Server import *
 from ..utility import HealthCheck
 
 class YouTube(Server):
 	@HealthCheck
 	def fileLink(self) -> str:
 		"""
-		Recupera il link diretto per il download del file dell'episodio.
+        Recupera il link diretto per il download del file dell'episodio.
 
-		```
-		return str # Link del file
-		```
-		"""
+        Returns:
+          Link diretto.
+	
+        Example:
+          ```py
+          return str # Link del file
+          ```
+        """
 		
 		anime_id = self.link.split("/")[-1]
 		external_link = "https://www.animeworld.so/api/episode/serverPlayerAnimeWorld?id={}".format(anime_id)
 
 		sb_get = SES.get(self.link)
 		sb_get.raise_for_status()
 
@@ -27,48 +31,63 @@
 
 		yutubelink_raw = re.search(r'"(https:\/\/www\.youtube\.com\/embed\/.+)"\);', soupeddata.prettify()).group(1)
 
 		return yutubelink_raw.replace('embed/', 'watch?v=')
 
 	def fileInfo(self) -> Dict[str,str]:
 		"""
-		Recupera le informazioni del file dell'episodio.
+        Recupera le informazioni del file dell'episodio.
 
-		```
-		return {
-		  "content_type": str, # Tipo del file, es. video/mp4
-		  "total_bytes": int, # Byte totali del file
-		  "last_modified": datetime, # Data e ora dell'ultimo aggiornamento effettuato all'episodio sul server
-		  "server_name": str, # Nome del server
-		  "server_id": int, # ID del server
-		  "url": str # url dell'episodio
-		} 
-		```
-		"""
+        Returns:
+          Informazioni file episodio.
+
+        Example:
+          ```py
+          return {
+            "content_type": str, # Tipo del file, es. video/mp4
+            "total_bytes": int, # Byte totali del file
+            "last_modified": datetime, # Data e ora dell'ultimo aggiornamento effettuato all'episodio sul server
+            "server_name": str, # Nome del server
+            "server_id": int, # ID del server
+            "url": str # url dell'episodio
+          } 
+          ```
+        """
 
 		return self._fileInfoEx()
 
 	def download(self, title: Optional[str]=None, folder: str='', *, hook: Callable[[Dict], None]=lambda *args:None, opt: List[str]=[]) -> Optional[str]:
 		"""
-		Scarica l'episodio.
+        Scarica l'episodio.
 
-		- `title`: Nome con cui verrà nominato il file scaricato.
-		- `folder`: Posizione in cui verrà spostato il file scaricato.
-		- `hook`: Funzione che viene richiamata varie volte durante il download; la funzione riceve come argomento un dizionario con le seguenti chiavi: 
-		  - `total_bytes`: Byte totali da scaricare.
-		  - `downloaded_bytes`: Byte attualmente scaricati.
-		  - `percentage`: Percentuale del progresso di download.
-		  - `speed`: Velocità di download (byte/s)
-		  - `elapsed`: Tempo trascorso dall'inizio del download.
-		  - `eta`: Tempo stimato rimanente per fine del download.
-		  - `status`: 'downloading' | 'finished' | 'aborted'
-		  - `filename`: Nome del file in download.
-		- `opt`: Lista per delle opzioni aggiuntive.
-		  - `'abort'`: Ferma forzatamente il download.
-		
-		```
-		return str # File scaricato
-		```
-		"""
+        Args:
+          title: Nome con cui verrà nominato il file scaricato.
+          folder: Posizione in cui verrà spostato il file scaricato.
+
+        Other parameters:
+          hook: Funzione che viene richiamata varie volte durante il download; la funzione riceve come argomento un dizionario con le seguenti chiavi:\n 
+            - `total_bytes`: Byte totali da scaricare.
+            - `downloaded_bytes`: Byte attualmente scaricati.
+            - `percentage`: Percentuale del progresso di download.
+            - `speed`: Velocità di download (byte/s)
+            - `elapsed`: Tempo trascorso dall'inizio del download.
+            - `eta`: Tempo stimato rimanente per fine del download.
+            - `status`: 'downloading' | 'finished' | 'aborted'
+            - `filename`: Nome del file in download.
+
+          opt: Lista per delle opzioni aggiuntive.\n
+            - `'abort'`: Ferma forzatamente il download.
+        
+        Returns:
+          Nome del file scaricato. 
+
+        Raises:
+          HardStoppedDownload: Il file in download è stato forzatamente interrotto.
+
+        Example:
+          ```py
+          return str # File scaricato
+          ```
+        """
 		if title is None: title = self._defTitle
 		else: title = self._sanitize(title)
 		return self._dowloadEx(title,folder,hook=hook,opt=opt)
```

### Comparing `animeworld-1.6.0/setup.py` & `animeworld-1.6.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="animeworld",
-    version="1.6.0",
+    version="1.6.1",
     author="MainKronos",
     description="AnimeWorld UNOFFICIAL API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/MainKronos/AnimeWorld-API",
+    url="https://mainkronos.github.io/AnimeWorld-API/",
     packages=setuptools.find_packages(),
-    install_requires=['httpx', 'youtube_dl', 'beautifulsoup4'],
+    install_requires=['httpx', 'httpx[http2]', 'youtube_dl', 'beautifulsoup4'],
 	license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
 		"Topic :: Utilities",
     ],
-    python_requires='>=3.6',
+    python_requires='>= 3.7',
 )
```

