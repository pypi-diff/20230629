# Comparing `tmp/gitlabx-0.1.2-py3-none-any.whl.zip` & `tmp/gitlabx-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 8063 bytes, number of entries: 16
+Zip file size: 8074 bytes, number of entries: 16
 -rwxrwxrwx  2.0 unx        0 b- defN 23-Jun-28 23:28 gitlabx/__init__.py
 -rwxrwxrwx  2.0 unx      380 b- defN 23-Jun-29 10:14 gitlabx/abstract.py
 -rwxrwxrwx  2.0 unx      912 b- defN 23-Jun-28 23:46 gitlabx/branches.py
 -rwxrwxrwx  2.0 unx      922 b- defN 23-Jun-28 23:46 gitlabx/commits.py
 -rwxrwxrwx  2.0 unx      985 b- defN 23-Jun-28 23:46 gitlabx/deployments.py
 -rwxrwxrwx  2.0 unx      861 b- defN 23-Jun-28 23:46 gitlabx/events.py
--rwxrwxrwx  2.0 unx     1594 b- defN 23-Jun-28 23:28 gitlabx/factories.py
+-rwxrwxrwx  2.0 unx     1801 b- defN 23-Jun-29 11:12 gitlabx/factories.py
 -rwxrwxrwx  2.0 unx      903 b- defN 23-Jun-28 23:46 gitlabx/issues.py
 -rwxrwxrwx  2.0 unx      744 b- defN 23-Jun-28 23:28 gitlabx/project.py
 -rwxrwxrwx  2.0 unx      938 b- defN 23-Jun-28 23:47 gitlabx/projectLanguages.py
 -rwxrwxrwx  2.0 unx      985 b- defN 23-Jun-28 23:47 gitlabx/repositories.py
 -rwxrwxrwx  2.0 unx     1039 b- defN 23-Jun-28 23:47 gitlabx/repositoryTree.py
--rwxrwxrwx  2.0 unx     1675 b- defN 23-Jun-29 10:16 gitlabx-0.1.2.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-29 10:16 gitlabx-0.1.2.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-29 10:16 gitlabx-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1213 b- defN 23-Jun-29 10:16 gitlabx-0.1.2.dist-info/RECORD
-16 files, 13251 bytes uncompressed, 6081 bytes compressed:  54.1%
+-rwxrwxrwx  2.0 unx     1675 b- defN 23-Jun-29 11:16 gitlabx-0.1.3.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-29 11:16 gitlabx-0.1.3.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-29 11:16 gitlabx-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1213 b- defN 23-Jun-29 11:16 gitlabx-0.1.3.dist-info/RECORD
+16 files, 13458 bytes uncompressed, 6092 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: gitlabx/repositories.py
 Comment: 
 
 Filename: gitlabx/repositoryTree.py
 Comment: 
 
-Filename: gitlabx-0.1.2.dist-info/METADATA
+Filename: gitlabx-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: gitlabx-0.1.2.dist-info/WHEEL
+Filename: gitlabx-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: gitlabx-0.1.2.dist-info/top_level.txt
+Filename: gitlabx-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: gitlabx-0.1.2.dist-info/RECORD
+Filename: gitlabx-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gitlabx/factories.py

```diff
@@ -11,65 +11,72 @@
 
 class ProjectFactory(factory.Factory):
     
     class Meta:
         model = Project
         
     personal_access_token = None
+    gitlab_url = None
   
 class RepositoryTreeFactory(factory.Factory):
     
     class Meta:
         model = RepositoryTree
         
     personal_access_token = None
+    gitlab_url = None
 
 class BranchesFactory(factory.Factory):
     
     class Meta:
         model = Branches
         
     personal_access_token = None
-
+    gitlab_url = None
+    
 class CommitsFactory(factory.Factory):
     
     class Meta:
         model = Commits
         
     personal_access_token = None
-
+    gitlab_url = None
 class DeploymentsFactory(factory.Factory):
     
     class Meta:
         model = Deployments
         
     personal_access_token = None
+    gitlab_url = None
 
 class EventsFactory(factory.Factory):
     
     class Meta:
         model = Events
         
     personal_access_token = None
+    gitlab_url = None
 
 class IssuesFactory(factory.Factory):
     
     class Meta:
         model = Issues
         
     personal_access_token = None
+    gitlab_url = None
 
 class RepositoriesFactory(factory.Factory):
     
     class Meta:
         model = Repositories
         
     personal_access_token = None
-
+    gitlab_url = None
 
 
 class ProjectLanguagesFactory(factory.Factory):
     
     class Meta:
         model = ProjectLanguages
         
     personal_access_token = None
+    gitlab_url = None
```

## Comparing `gitlabx-0.1.2.dist-info/METADATA` & `gitlabx-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabx
-Version: 0.1.2
+Version: 0.1.3
 Summary: Uma Lib para buscar dados do Gitlab
 Home-page: https://gitlab.com/immigrant-data-driven-development/libs/application/gitlab
 Author: Carlos Henrique Maulaz de Freitas
 Author-email: carlosmaulaz@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `gitlabx-0.1.2.dist-info/RECORD` & `gitlabx-0.1.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 gitlabx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gitlabx/abstract.py,sha256=mc5cmcD-klDfmHwo0HSl8itgsAiHx9nla1d5FQFjmcQ,380
 gitlabx/branches.py,sha256=Eexe2Ef8JtGNf3Bh_jJcskvFb2vzI4E28ARG54NcGnU,912
 gitlabx/commits.py,sha256=T74pE1bJK1vSmoLcRbsLePJGKU9M3RyUaH3FiFdyOW4,922
 gitlabx/deployments.py,sha256=J-xD6dZA958KGqIuY7sDhWdihtAgH9hj75l9x8JZDB4,985
 gitlabx/events.py,sha256=iciXrcb2lZTgJlN8IuTFiDxUMWeNmQ7r1w26pHCCymo,861
-gitlabx/factories.py,sha256=a4BRvL27l1DgyrbKtW6ysUVh6PaC7RXqW4PQZf0PzYU,1594
+gitlabx/factories.py,sha256=nFQIQg6VSTiEUOZb2_52OwRqJqyD5jEGHWCTTXWKUbM,1801
 gitlabx/issues.py,sha256=Zkygd30INnJ7ohNKGPLIbORO2c7syACgl2QeLIaN2nU,903
 gitlabx/project.py,sha256=Dlmr7NbMZFsGqjbYc0bk_6v87UBju07wJD32sco-PA4,744
 gitlabx/projectLanguages.py,sha256=d3za4BOfBvC4Dg_laz1lV2fzy_m21uJoLZiDuYYDY64,938
 gitlabx/repositories.py,sha256=qHAxIH61ouC1qhJnuou1V7hyGgZhIiJxhlrCy6r3I_s,985
 gitlabx/repositoryTree.py,sha256=-XEiboSxun8_Yed2kq1lSIOYtjBlGVqRX79Cr3BPzA8,1039
-gitlabx-0.1.2.dist-info/METADATA,sha256=sgmzmxyjnlAf_UdvjicZUsrrknZWTU8eGiAA-IKNzME,1675
-gitlabx-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gitlabx-0.1.2.dist-info/top_level.txt,sha256=EkmcO7CZ14bNE_fgl8kFTFfgu1K7yvMO481rj0zu6ns,8
-gitlabx-0.1.2.dist-info/RECORD,,
+gitlabx-0.1.3.dist-info/METADATA,sha256=ofGbE9m6DCpSQrSbgxM6H3JP5sFpbjx9L28ukqmHnLc,1675
+gitlabx-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gitlabx-0.1.3.dist-info/top_level.txt,sha256=EkmcO7CZ14bNE_fgl8kFTFfgu1K7yvMO481rj0zu6ns,8
+gitlabx-0.1.3.dist-info/RECORD,,
```

