# Comparing `tmp/gitlabx-0.1.3-py3-none-any.whl.zip` & `tmp/gitlabx-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 8074 bytes, number of entries: 16
+Zip file size: 8218 bytes, number of entries: 16
 -rwxrwxrwx  2.0 unx        0 b- defN 23-Jun-28 23:28 gitlabx/__init__.py
 -rwxrwxrwx  2.0 unx      380 b- defN 23-Jun-29 10:14 gitlabx/abstract.py
--rwxrwxrwx  2.0 unx      912 b- defN 23-Jun-28 23:46 gitlabx/branches.py
--rwxrwxrwx  2.0 unx      922 b- defN 23-Jun-28 23:46 gitlabx/commits.py
--rwxrwxrwx  2.0 unx      985 b- defN 23-Jun-28 23:46 gitlabx/deployments.py
--rwxrwxrwx  2.0 unx      861 b- defN 23-Jun-28 23:46 gitlabx/events.py
+-rwxrwxrwx  2.0 unx      953 b- defN 23-Jun-29 11:24 gitlabx/branches.py
+-rwxrwxrwx  2.0 unx      963 b- defN 23-Jun-29 11:24 gitlabx/commits.py
+-rwxrwxrwx  2.0 unx     1026 b- defN 23-Jun-29 11:24 gitlabx/deployments.py
+-rwxrwxrwx  2.0 unx      902 b- defN 23-Jun-29 11:24 gitlabx/events.py
 -rwxrwxrwx  2.0 unx     1801 b- defN 23-Jun-29 11:12 gitlabx/factories.py
--rwxrwxrwx  2.0 unx      903 b- defN 23-Jun-28 23:46 gitlabx/issues.py
--rwxrwxrwx  2.0 unx      744 b- defN 23-Jun-28 23:28 gitlabx/project.py
--rwxrwxrwx  2.0 unx      938 b- defN 23-Jun-28 23:47 gitlabx/projectLanguages.py
--rwxrwxrwx  2.0 unx      985 b- defN 23-Jun-28 23:47 gitlabx/repositories.py
--rwxrwxrwx  2.0 unx     1039 b- defN 23-Jun-28 23:47 gitlabx/repositoryTree.py
--rwxrwxrwx  2.0 unx     1675 b- defN 23-Jun-29 11:16 gitlabx-0.1.3.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-29 11:16 gitlabx-0.1.3.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-29 11:16 gitlabx-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1213 b- defN 23-Jun-29 11:16 gitlabx-0.1.3.dist-info/RECORD
-16 files, 13458 bytes uncompressed, 6092 bytes compressed:  54.7%
+-rwxrwxrwx  2.0 unx      944 b- defN 23-Jun-29 11:24 gitlabx/issues.py
+-rwxrwxrwx  2.0 unx      785 b- defN 23-Jun-29 11:24 gitlabx/project.py
+-rwxrwxrwx  2.0 unx      979 b- defN 23-Jun-29 11:24 gitlabx/projectLanguages.py
+-rwxrwxrwx  2.0 unx     1026 b- defN 23-Jun-29 11:24 gitlabx/repositories.py
+-rwxrwxrwx  2.0 unx     1080 b- defN 23-Jun-29 11:24 gitlabx/repositoryTree.py
+-rwxrwxrwx  2.0 unx     1675 b- defN 23-Jun-29 11:29 gitlabx-0.1.4.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-29 11:29 gitlabx-0.1.4.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-29 11:29 gitlabx-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1215 b- defN 23-Jun-29 11:29 gitlabx-0.1.4.dist-info/RECORD
+16 files, 13829 bytes uncompressed, 6236 bytes compressed:  54.9%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: gitlabx/repositories.py
 Comment: 
 
 Filename: gitlabx/repositoryTree.py
 Comment: 
 
-Filename: gitlabx-0.1.3.dist-info/METADATA
+Filename: gitlabx-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: gitlabx-0.1.3.dist-info/WHEEL
+Filename: gitlabx-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: gitlabx-0.1.3.dist-info/top_level.txt
+Filename: gitlabx-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: gitlabx-0.1.3.dist-info/RECORD
+Filename: gitlabx-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gitlabx/branches.py

```diff
@@ -1,16 +1,16 @@
 import logging
 logging.basicConfig(level=logging.INFO)
 from gitlabx.abstract import AbstractGitLab
 
 # Represents a software Project
 class Branches(AbstractGitLab):
 
-	def __init__(self,personal_access_token):
-		super(Branches,self).__init__(personal_access_token=personal_access_token)
+	def __init__(self,personal_access_token, gitlab_url = None):
+		super(Branches,self).__init__(personal_access_token=personal_access_token,gitlab_url=gitlab_url)
 	
 	def get_all(self, today=False): 
 		
 		result = []
 		branch_list = []
 
 		try:
```

## gitlabx/commits.py

```diff
@@ -2,16 +2,16 @@
 logging.basicConfig(level=logging.INFO)
 from gitlabx.abstract import AbstractGitLab
 
 
 # Represents a software Project
 class Commits(AbstractGitLab):
 
-	def __init__(self,personal_access_token):
-		super(Commits,self).__init__(personal_access_token=personal_access_token)
+	def __init__(self,personal_access_token, gitlab_url = None):
+		super(Commits,self).__init__(personal_access_token=personal_access_token,gitlab_url=gitlab_url)
 	
 	def get_all(self, today=False): 
 		
 		result = []
 		commit_list = []
 
 		try:
```

## gitlabx/deployments.py

```diff
@@ -1,16 +1,16 @@
 import logging
 logging.basicConfig(level=logging.INFO)
 from gitlabx.abstract import AbstractGitLab
 
 # Represents a software Project
 class Deployments(AbstractGitLab):
 
-	def __init__(self,personal_access_token):
-		super(Deployments,self).__init__(personal_access_token=personal_access_token)
+	def __init__(self,personal_access_token, gitlab_url = None):
+		super(Deployments,self).__init__(personal_access_token=personal_access_token,gitlab_url=gitlab_url)
 	
 	def get_all(self, today=False): 
 		
 		result = []
 		deployment_list = []
 
 		try:
```

## gitlabx/events.py

```diff
@@ -1,16 +1,16 @@
 import logging
 logging.basicConfig(level=logging.INFO)
 from gitlabx.abstract import AbstractGitLab
 
 # Represents a software Project
 class Events(AbstractGitLab):
 
-	def __init__(self,personal_access_token):
-		super(Events,self).__init__(personal_access_token=personal_access_token)
+	def __init__(self,personal_access_token, gitlab_url = None):
+		super(Events,self).__init__(personal_access_token=personal_access_token,gitlab_url=gitlab_url)
 	
 	def get_all(self, today=False): 
 		
 		result = []
 		event_list = []
 
 		try:
```

## gitlabx/issues.py

```diff
@@ -1,16 +1,16 @@
 import logging
 logging.basicConfig(level=logging.INFO)
 from gitlabx.abstract import AbstractGitLab
 
 # Represents a software Project
 class Issues(AbstractGitLab):
 
-	def __init__(self,personal_access_token):
-		super(Issues,self).__init__(personal_access_token=personal_access_token)
+	def __init__(self,personal_access_token, gitlab_url = None):
+		super(Issues,self).__init__(personal_access_token=personal_access_token,gitlab_url=gitlab_url)
 	
 	def get_all(self, today=False): 
 		
 		result = []
 		issue_list = []
 
 		try:
```

## gitlabx/project.py

```diff
@@ -1,16 +1,16 @@
 import logging
 logging.basicConfig(level=logging.INFO)
 from gitlabx.abstract import AbstractGitLab
 
 # Represents a software Project
 class Project(AbstractGitLab):
 
-	def __init__(self,personal_access_token):
-		super(Project,self).__init__(personal_access_token=personal_access_token)
+	def __init__(self,personal_access_token, gitlab_url = None):
+		super(Project,self).__init__(personal_access_token=personal_access_token,gitlab_url=gitlab_url)
 	
 	def get_all(self, today=False): 
 		
 		result = []
 		projects = []
 
 		try:
```

## gitlabx/projectLanguages.py

```diff
@@ -2,16 +2,16 @@
 logging.basicConfig(level=logging.INFO)
 from gitlabx.abstract import AbstractGitLab
 import json
 
 # Represents a software Project
 class ProjectLanguages(AbstractGitLab):
 
-	def __init__(self,personal_access_token):
-		super(ProjectLanguages,self).__init__(personal_access_token=personal_access_token)
+	def __init__(self,personal_access_token, gitlab_url = None):
+		super(ProjectLanguages,self).__init__(personal_access_token=personal_access_token,gitlab_url=gitlab_url)
 	
 	def get_all(self, today=False): 
 		
 		result = []
 		languages = []
 
 		try:
```

## gitlabx/repositories.py

```diff
@@ -1,16 +1,16 @@
 import logging
 logging.basicConfig(level=logging.INFO)
 from gitlabx.abstract import AbstractGitLab
 
 # Represents a software Project
 class Repositories(AbstractGitLab):
 
-	def __init__(self,personal_access_token):
-		super(Repositories,self).__init__(personal_access_token=personal_access_token)
+	def __init__(self,personal_access_token, gitlab_url = None):
+		super(Repositories,self).__init__(personal_access_token=personal_access_token,gitlab_url=gitlab_url)
 	
 	def get_all(self, today=False): 
 		
 		result = []
 		repository_list = []
 
 		try:
```

## gitlabx/repositoryTree.py

```diff
@@ -1,16 +1,16 @@
 import logging
 logging.basicConfig(level=logging.INFO)
 from gitlabx.abstract import AbstractGitLab
 
 # Represents a software Project
 class RepositoryTree(AbstractGitLab):
 
-	def __init__(self,personal_access_token):
-		super(RepositoryTree,self).__init__(personal_access_token=personal_access_token)
+	def __init__(self,personal_access_token, gitlab_url = None):
+		super(RepositoryTree,self).__init__(personal_access_token=personal_access_token,gitlab_url=gitlab_url)
 	
 	def get_all(self, today=False):
 		
 		projects = []
 		project_repository_tree = []
 
 		try:
```

## Comparing `gitlabx-0.1.3.dist-info/METADATA` & `gitlabx-0.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabx
-Version: 0.1.3
+Version: 0.1.4
 Summary: Uma Lib para buscar dados do Gitlab
 Home-page: https://gitlab.com/immigrant-data-driven-development/libs/application/gitlab
 Author: Carlos Henrique Maulaz de Freitas
 Author-email: carlosmaulaz@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

