# Comparing `tmp/mongeasy-0.2.1.tar.gz` & `tmp/mongeasy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongeasy-0.2.1.tar", last modified: Thu Jun 22 13:24:46 2023, max compression
+gzip compressed data, was "mongeasy-0.2.2.tar", last modified: Thu Jun 29 07:49:42 2023, max compression
```

## Comparing `mongeasy-0.2.1.tar` & `mongeasy-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.400606 mongeasy-0.2.1/
--rw-r--r--   0 javv       (501) staff       (20)     1074 2023-06-03 04:53:57.000000 mongeasy-0.2.1/LICENSE
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.375086 mongeasy-0.2.1/Mongeasy.egg-info/
--rw-r--r--   0 javv       (501) staff       (20)    19125 2023-06-22 13:24:46.000000 mongeasy-0.2.1/Mongeasy.egg-info/PKG-INFO
--rw-r--r--   0 javv       (501) staff       (20)      990 2023-06-22 13:24:46.000000 mongeasy-0.2.1/Mongeasy.egg-info/SOURCES.txt
--rw-r--r--   0 javv       (501) staff       (20)        1 2023-06-22 13:24:46.000000 mongeasy-0.2.1/Mongeasy.egg-info/dependency_links.txt
--rw-r--r--   0 javv       (501) staff       (20)      822 2023-06-22 13:24:46.000000 mongeasy-0.2.1/Mongeasy.egg-info/requires.txt
--rw-r--r--   0 javv       (501) staff       (20)       30 2023-06-22 13:24:46.000000 mongeasy-0.2.1/Mongeasy.egg-info/top_level.txt
--rw-r--r--   0 javv       (501) staff       (20)    19125 2023-06-22 13:24:46.399958 mongeasy-0.2.1/PKG-INFO
--rw-r--r--   0 javv       (501) staff       (20)    18389 2023-06-22 10:57:41.000000 mongeasy-0.2.1/README.md
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.386446 mongeasy-0.2.1/mongeasy/
--rw-r--r--   0 javv       (501) staff       (20)      623 2023-06-22 13:22:39.000000 mongeasy-0.2.1/mongeasy/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     2692 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/base_dict.py
--rw-r--r--   0 javv       (501) staff       (20)     3557 2023-06-22 10:57:41.000000 mongeasy-0.2.1/mongeasy/connection.py
--rw-r--r--   0 javv       (501) staff       (20)     4349 2023-06-22 10:57:41.000000 mongeasy-0.2.1/mongeasy/core.py
--rw-r--r--   0 javv       (501) staff       (20)    14041 2023-06-22 10:57:41.000000 mongeasy-0.2.1/mongeasy/document.py
--rw-r--r--   0 javv       (501) staff       (20)     2696 2023-06-22 10:57:41.000000 mongeasy-0.2.1/mongeasy/dynamics.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.387584 mongeasy-0.2.1/mongeasy/examples/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/examples/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     1792 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/exceptions.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.388846 mongeasy-0.2.1/mongeasy/plugins/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/plugins/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     4101 2023-06-22 10:57:41.000000 mongeasy-0.2.1/mongeasy/plugins/registry.py
--rw-r--r--   0 javv       (501) staff       (20)     4842 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/resultlist.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.389968 mongeasy-0.2.1/mongeasy/utils/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/utils/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     1755 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/utils/utils.py
--rw-r--r--   0 javv       (501) staff       (20)       89 2023-06-03 04:53:57.000000 mongeasy-0.2.1/pyproject.toml
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.396902 mongeasy-0.2.1/sample_plugins/
--rw-r--r--   0 javv       (501) staff       (20)      786 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)      366 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/connection_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      290 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/delete_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      299 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/init_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      576 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/pydantic_validator.py
--rw-r--r--   0 javv       (501) staff       (20)      356 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/query_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      295 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/save_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      347 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/validator_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-22 13:24:46.400821 mongeasy-0.2.1/setup.cfg
--rw-r--r--   0 javv       (501) staff       (20)     1206 2023-06-22 13:23:53.000000 mongeasy-0.2.1/setup.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.399501 mongeasy-0.2.1/tests/
--rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-03 04:53:57.000000 mongeasy-0.2.1/tests/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)    13161 2023-06-22 10:57:41.000000 mongeasy-0.2.1/tests/test_mongeasy.py
--rw-r--r--   0 javv       (501) staff       (20)     2508 2023-06-22 10:57:41.000000 mongeasy-0.2.1/tests/test_plugins.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 07:49:42.292611 mongeasy-0.2.2/
+-rw-r--r--   0 javv       (501) staff       (20)     1074 2023-06-03 04:53:57.000000 mongeasy-0.2.2/LICENSE
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 07:49:42.231426 mongeasy-0.2.2/Mongeasy.egg-info/
+-rw-r--r--   0 javv       (501) staff       (20)    22372 2023-06-29 07:49:42.000000 mongeasy-0.2.2/Mongeasy.egg-info/PKG-INFO
+-rw-r--r--   0 javv       (501) staff       (20)     1018 2023-06-29 07:49:42.000000 mongeasy-0.2.2/Mongeasy.egg-info/SOURCES.txt
+-rw-r--r--   0 javv       (501) staff       (20)        1 2023-06-29 07:49:42.000000 mongeasy-0.2.2/Mongeasy.egg-info/dependency_links.txt
+-rw-r--r--   0 javv       (501) staff       (20)      822 2023-06-29 07:49:42.000000 mongeasy-0.2.2/Mongeasy.egg-info/requires.txt
+-rw-r--r--   0 javv       (501) staff       (20)       30 2023-06-29 07:49:42.000000 mongeasy-0.2.2/Mongeasy.egg-info/top_level.txt
+-rw-r--r--   0 javv       (501) staff       (20)    22372 2023-06-29 07:49:42.292182 mongeasy-0.2.2/PKG-INFO
+-rw-r--r--   0 javv       (501) staff       (20)    21636 2023-06-29 07:43:54.000000 mongeasy-0.2.2/README.md
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 07:49:42.253355 mongeasy-0.2.2/mongeasy/
+-rw-r--r--   0 javv       (501) staff       (20)      623 2023-06-22 13:22:39.000000 mongeasy-0.2.2/mongeasy/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     2692 2023-06-03 04:53:57.000000 mongeasy-0.2.2/mongeasy/base_dict.py
+-rw-r--r--   0 javv       (501) staff       (20)     3685 2023-06-26 05:55:43.000000 mongeasy-0.2.2/mongeasy/connection.py
+-rw-r--r--   0 javv       (501) staff       (20)     4349 2023-06-22 10:57:41.000000 mongeasy-0.2.2/mongeasy/core.py
+-rw-r--r--   0 javv       (501) staff       (20)    14298 2023-06-29 07:09:12.000000 mongeasy-0.2.2/mongeasy/document.py
+-rw-r--r--   0 javv       (501) staff       (20)     2696 2023-06-22 10:57:41.000000 mongeasy-0.2.2/mongeasy/dynamics.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 07:49:42.254562 mongeasy-0.2.2/mongeasy/examples/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.2/mongeasy/examples/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     1792 2023-06-03 04:53:57.000000 mongeasy-0.2.2/mongeasy/exceptions.py
+-rw-r--r--   0 javv       (501) staff       (20)     1876 2023-06-29 07:08:47.000000 mongeasy-0.2.2/mongeasy/lazy_resultlist.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 07:49:42.259223 mongeasy-0.2.2/mongeasy/plugins/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.2/mongeasy/plugins/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     4101 2023-06-22 10:57:41.000000 mongeasy-0.2.2/mongeasy/plugins/registry.py
+-rw-r--r--   0 javv       (501) staff       (20)     4842 2023-06-03 04:53:57.000000 mongeasy-0.2.2/mongeasy/resultlist.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 07:49:42.263401 mongeasy-0.2.2/mongeasy/utils/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.2/mongeasy/utils/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     1755 2023-06-03 04:53:57.000000 mongeasy-0.2.2/mongeasy/utils/utils.py
+-rw-r--r--   0 javv       (501) staff       (20)       89 2023-06-03 04:53:57.000000 mongeasy-0.2.2/pyproject.toml
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 07:49:42.287492 mongeasy-0.2.2/sample_plugins/
+-rw-r--r--   0 javv       (501) staff       (20)      786 2023-06-22 10:57:41.000000 mongeasy-0.2.2/sample_plugins/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)      366 2023-06-22 10:57:41.000000 mongeasy-0.2.2/sample_plugins/connection_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      290 2023-06-22 10:57:41.000000 mongeasy-0.2.2/sample_plugins/delete_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      299 2023-06-22 10:57:41.000000 mongeasy-0.2.2/sample_plugins/init_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      576 2023-06-22 10:57:41.000000 mongeasy-0.2.2/sample_plugins/pydantic_validator.py
+-rw-r--r--   0 javv       (501) staff       (20)      356 2023-06-22 10:57:41.000000 mongeasy-0.2.2/sample_plugins/query_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      295 2023-06-22 10:57:41.000000 mongeasy-0.2.2/sample_plugins/save_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      347 2023-06-22 10:57:41.000000 mongeasy-0.2.2/sample_plugins/validator_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-29 07:49:42.292669 mongeasy-0.2.2/setup.cfg
+-rw-r--r--   0 javv       (501) staff       (20)     1206 2023-06-29 07:44:04.000000 mongeasy-0.2.2/setup.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 07:49:42.291554 mongeasy-0.2.2/tests/
+-rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-03 04:53:57.000000 mongeasy-0.2.2/tests/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)    14505 2023-06-29 07:29:00.000000 mongeasy-0.2.2/tests/test_mongeasy.py
+-rw-r--r--   0 javv       (501) staff       (20)     2508 2023-06-22 10:57:41.000000 mongeasy-0.2.2/tests/test_plugins.py
```

### Comparing `mongeasy-0.2.1/LICENSE` & `mongeasy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/Mongeasy.egg-info/PKG-INFO` & `mongeasy-0.2.2/Mongeasy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongeasy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,39 +16,53 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mongeasy
 
-Mongeasy is a easy to use library to be used for simple access to a MongoDB database, without any need for schemas or validation. Just store the data as it is used in your application.
+Mongeasy is a powerful yet easy-to-use Python library for interacting with MongoDB databases. Embracing the dynamic nature of Python and MongoDB, Mongeasy eliminates the need for rigid schemas and validation layers. This means you can store and handle data in its natural form, just as it is used in your application, enhancing code readability and efficiency.
+
+However, Mongeasy's flexibility doesn't mean it compromises on control. With its built-in plugin system, you can hook into the lifecycle of a document and the database connection, enabling advanced features like data validation, logging, and more as per your application's requirements.
+
+Whether you're developing a small personal project or a large-scale production application, Mongeasy helps you focus more on your application logic, and less on managing your database. Experience the freedom of schema-less design with the power of customization, all bundled in a single, user-friendly package.
 
 ## Installation
 Mongoeasy is available on PyPI and can be installed using pip:
 
 ```bash
 pip install mongeasy
 ```
 
 ## Documentation
 The documentation can be found at [https://mongeasy.readthedocs.io](https://mongeasy.readthedocs.io)
 
-## What's new in version 0.2.0?
-### New plugin system
-Mongeasy now has a plugin system that allows you to hook into the lifecycle of a document and the database connection. This allows you to do things like validation, logging, and more.
+## What's new in version 0.2.2?
+### Support for lazy queries
+The find method now supports a lazy flag (defeault set to False) which when set to True, returns a lazy query object instead of a result list. This is useful when you want to iterate over a large number of documents without loading them all into memory at once.
+
+```python
+from mongeasy import create_document_class
+
+User = create_document_class('User', 'users')
 
-See documentation for this feature below.
+# Find all documents in the 'users' collection
+users = User.all(lazy=True)
 
-### Breaking changes
+# Find all documents with age 25
+users = User.find({'age': 25}, lazy=True)
+```
+
+### Breaking changes (0.2.0)
 The class method `delete` has been renamed to `delete_many` as the name conflicted with the instance method `delete`.
 
 --------------------
 
 ## Connection
-Connection to the database is handled automtically for you if you have the conenction information in a configfile or set as environment variables.
+Connection to the database is handled automatically for you if you have the connection information in a configfile or set as environment variables.
 
 ### Connection using configfile
 Create a file called `mongeasy_config.yml` and place it in your project root folder.
 
 The contents of the file should be:
 
 ```bash
@@ -61,148 +75,143 @@
 You can, as an alternative method, define your connection information using environment variables. Just set these two:
 
 ```bash
 MONGOEASY_CONNECTION_STRING=mongodb://localhost:27017/
 MONGOEASY_DATABASE_NAME=mydatabase
 ```
 
-## Create a document class
-To use Mongeasy you will create a document class that can be used with the collection of choice. To do this you will use the `create_document_class` factory function like this:
+Absolutely, here's a revised version of your examples section:
 
-```python
-from mongeasy import create_document_class
+---
 
+## Create a Document Class
 
-User = create_document_class('User', 'users')
-
-```
+In Mongeasy, you interact with your MongoDB collections through document classes. A document class is a Python class that represents a MongoDB collection and provides methods for interacting with that collection.
 
-The first argument is the name the class will get and the second argument is the name of the collection to use. If the collection does not exist it will be created when you use the class to store documents.
-
-You will not need to assign the returned value to a class variable as in the example above, as the generated class is injected into the current namespace:
+You can create a document class using the `create_document_class` factory function. The first argument is the name you want to give to the class (which should be the singular form of the collection name), and the second argument is the name of the MongoDB collection that the class will interact with.
 
 ```python
 from mongeasy import create_document_class
 
+User = create_document_class('User', 'users')
+```
 
-create_document_class('User', 'users')
+After running this code, `User` becomes a new class that you can use to interact with the 'users' collection in your MongoDB database.
 
-# The class User exist from this point in the code
+## Create and Store a Document
 
-```
-
-## Create a store a document
-You can create a documnet by using the generated class. You can either use keyword arguments or pass a dict.
+Once you have a document class, you can use it to create new documents in your MongoDB collection. You can create a document using keyword arguments or by passing a dictionary. After creating a document, you can save it to your MongoDB collection using the `save` method.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
 # Create a document using keyword arguments
 user1 = User(name='Alice', age=25)
 user1.save()
 
-# Create a document using a dict
+# Create a document using a dictionary
 user2 = User({'name': 'Bob', 'age': 30})
 user2.save()
-
 ```
 
-## Find documents
-You can find documents using the `find` method on the generated class. This method will return a list of documents.
+In this example, `user1` and `user2` are instances of the `User` document class. When you call the `save` method on these instances, Mongeasy automatically inserts them into the 'users' collection in your MongoDB database.
+
+## Find Documents
+
+You can retrieve documents from your MongoDB collection using the `find` method on your document class. This method returns a `ResultList` object that contains the found documents.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
-# Find all documents
+# Find all documents in the 'users' collection
 users = User.all()
 
 # Find all documents with age 25
 users = User.find({'age': 25})
-
 ```
-### Find one document
-You can find one document using the `find` method on the generated class.
 
-Find will return a ResultList object that can be used to get the first, or last, document in the list. If no document is found None is returned.
+In the first `find` example, Mongeasy returns all documents in the 'users' collection. In the second example, Mongeasy only returns documents where the 'age' field is 25.
+
+Find also has a lazy flag (defeault set to False) which when set to True, returns a lazy query object instead of a result list. This is useful when you want to iterate over a large number of documents without loading them all into memory at once.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
-# Find one document with age 25
-user = User.find({'age': 25}).first()
+# Find all documents in the 'users' collection
+users = User.all(lazy=True)
 
-if user is None:
-    print('No user found')
+# Find all documents with age 25
 
+users = User.find({'age': 25}, lazy=True)
 ```
 
-## Update a document
-You can update a document just by changing the attributes and then calling the `save` method.
+## Update a Document
+
+You can update a document by changing its attributes and then calling the `save` method. Mongeasy automatically updates the corresponding document in your MongoDB collection.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
 # Find one document with age 25
 user = User.find({'age': 25}).first()
 
-if user is None:
-    print('No user found')
-else:
+if user is not None:
     # Update the age of the user
     user.age = 26
     user.save()
 ```
 
-## Delete a document
-You can delete a document by calling the `delete` method on the document.
+In this example, Mongeasy first retrieves the document where the 'age' field is 25. Then, it changes the 'age' field of the document to 26 and saves the document back to the MongoDB collection.
+
+## Delete a Document
+
+You can remove a document from your MongoDB collection by calling the `delete` method on an instance of your document class.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
 # Find one document with age 25
 user = User.find({'age': 25}).first()
 
-if user is None:
-    print('No user found')
-else:
-    # Delete the user
+if user is not None:
     user.delete()
 ```
 
-You can also delete all documents in a collection by calling the `delete` method on the generated class.
+In this example, Mongeasy first retrieves the document where the 'age' field is 25. Then, it deletes that document from the 'users' collection in your MongoDB database.
+
+
+You can also delete all documents in a collection by calling the `delete_many` class method on the generated class.
 
 ```python
 from mongeasy import create_document_class
 
 
 User = create_document_class('User', 'users')
 
 
 # Delete using a filter
-User.delete({'age': 25})
+User.delete_many({'age': 25})
 
 # Delete all documents in the collection
-User.delete()
+User.delete_many()
 ```
 
+The `delete_many`method is useful when you want to delete multiple documents at once. The first call above deletes all users with age 25, and the second call deletes all users in the collection. 
+
+---
 ## Indexes
 You can create indexes on the collection by using the `create_index` method on the generated class.
 
 ```python
 from mongeasy import create_document_class
 
 
@@ -301,15 +310,15 @@
 except ValueError as e:
     print(e)
 ```
 
 This approach makes it easier to write, read, and manage your database queries in Python, providing a more user-friendly interface for MongoDB.
 
 ## ResultList
-All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
+All queries that can return more than one document will return a `ResultList` object, if not the lazy flag has been set. This object can be used to get the first or last document in the list, or None if no document is found.
 
 
 ```python
 from mongeasy import create_document_class
 
 
 User = create_document_class('User', 'users')
@@ -329,14 +338,33 @@
 * `last_or_none` - Get the last document in the list or None if no document is found, same as last
 * `map` - Apply a given function to each element in the list and return a new ResultList containing the results
 * `filter` - Filter the list using a given function and return a new ResultList containing the results
 * `reduce` - Apply a given function to each element in the list and return a single value
 * `group_by` - Group the list by a given key and return a dict with the results grouped by the key
 * `random` - Get a random document from the list or None if no document is found
 
+
+If lazy loading is enabled a LazyResultList. LazyResultList is a lazy version of Result list. It will cache the result of the query and only load the documents when they are accessed. This can be useful if you want to load the documents later or if you want to use the list in a for loop.
+
+Methods in the LazyResultList are
+* `first` - Get the first document in the list 
+* `next` - Get the next document in the list 
+
+Note that LazyResultList uses the PyMongo cursor generator. If you want to access the cursor directly you can use the `raw_query` method on the Document class.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find one document with age 25
+users = User.raw_query({'age': 25})
+```
+
 ## Mongeasy Plugin System
 
 The Mongeasy library provides a robust and flexible platform for interacting with MongoDB databases. To further enhance its utility and versatility, Mongeasy offers a plugin system. This system allows developers to customize and extend the library's functionality according to their specific needs.
 
 The motivation behind the plugin system is to provide a mechanism for developers to introduce new behaviors or modify existing ones without having to alter the core library code. By doing so, it promotes a modular approach where additional features or modifications can be encapsulated within individual plugins. This system fosters a more maintainable codebase, as plugins can be added, removed, or updated independently, without impacting the overall stability or functionality of the library.
 
 The plugin system can be particularly beneficial in scenarios where customized behaviors or additional features are required. These might include logging operations, implementing custom data validation or transformation rules, handling errors in specific ways, or integrating with other systems or libraries.
@@ -452,16 +480,16 @@
 plugins:
   - your_plugin_name.YourPluginClass
 ```
 
 As always, when developing a plugin, remember to respect the privacy and security of the user's data.
 
 ## Planned features
-* Enable lazy-loading of query results and support for query chaining
-* Implement a schema plugin system to allow for validation and type checking of documents
+* ~~Enable lazy-loading of query results and support for query chaining~~
+* ~~Implement a schema plugin system to allow for validation and type checking of documents~~
 * Add support for transactions using resource management
 * Implement logging and profiling to aid with debugging and performance tuning
 * Enable asynchronous I/O support for improved scalability
 * Implement caching with customizable caching strategies
 * Add support for background tasks using a task queue
 * Implement a paginator utility to allow for pagination of query results
 * Support for MongoDB Atlas search
```

### Comparing `mongeasy-0.2.1/Mongeasy.egg-info/SOURCES.txt` & `mongeasy-0.2.2/Mongeasy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 mongeasy/__init__.py
 mongeasy/base_dict.py
 mongeasy/connection.py
 mongeasy/core.py
 mongeasy/document.py
 mongeasy/dynamics.py
 mongeasy/exceptions.py
+mongeasy/lazy_resultlist.py
 mongeasy/resultlist.py
 mongeasy.egg-info/PKG-INFO
 mongeasy.egg-info/SOURCES.txt
 mongeasy.egg-info/dependency_links.txt
 mongeasy.egg-info/requires.txt
 mongeasy.egg-info/top_level.txt
 mongeasy/examples/__init__.py
```

### Comparing `mongeasy-0.2.1/Mongeasy.egg-info/requires.txt` & `mongeasy-0.2.2/Mongeasy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/PKG-INFO` & `mongeasy-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongeasy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,39 +16,53 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mongeasy
 
-Mongeasy is a easy to use library to be used for simple access to a MongoDB database, without any need for schemas or validation. Just store the data as it is used in your application.
+Mongeasy is a powerful yet easy-to-use Python library for interacting with MongoDB databases. Embracing the dynamic nature of Python and MongoDB, Mongeasy eliminates the need for rigid schemas and validation layers. This means you can store and handle data in its natural form, just as it is used in your application, enhancing code readability and efficiency.
+
+However, Mongeasy's flexibility doesn't mean it compromises on control. With its built-in plugin system, you can hook into the lifecycle of a document and the database connection, enabling advanced features like data validation, logging, and more as per your application's requirements.
+
+Whether you're developing a small personal project or a large-scale production application, Mongeasy helps you focus more on your application logic, and less on managing your database. Experience the freedom of schema-less design with the power of customization, all bundled in a single, user-friendly package.
 
 ## Installation
 Mongoeasy is available on PyPI and can be installed using pip:
 
 ```bash
 pip install mongeasy
 ```
 
 ## Documentation
 The documentation can be found at [https://mongeasy.readthedocs.io](https://mongeasy.readthedocs.io)
 
-## What's new in version 0.2.0?
-### New plugin system
-Mongeasy now has a plugin system that allows you to hook into the lifecycle of a document and the database connection. This allows you to do things like validation, logging, and more.
+## What's new in version 0.2.2?
+### Support for lazy queries
+The find method now supports a lazy flag (defeault set to False) which when set to True, returns a lazy query object instead of a result list. This is useful when you want to iterate over a large number of documents without loading them all into memory at once.
+
+```python
+from mongeasy import create_document_class
+
+User = create_document_class('User', 'users')
 
-See documentation for this feature below.
+# Find all documents in the 'users' collection
+users = User.all(lazy=True)
 
-### Breaking changes
+# Find all documents with age 25
+users = User.find({'age': 25}, lazy=True)
+```
+
+### Breaking changes (0.2.0)
 The class method `delete` has been renamed to `delete_many` as the name conflicted with the instance method `delete`.
 
 --------------------
 
 ## Connection
-Connection to the database is handled automtically for you if you have the conenction information in a configfile or set as environment variables.
+Connection to the database is handled automatically for you if you have the connection information in a configfile or set as environment variables.
 
 ### Connection using configfile
 Create a file called `mongeasy_config.yml` and place it in your project root folder.
 
 The contents of the file should be:
 
 ```bash
@@ -61,148 +75,143 @@
 You can, as an alternative method, define your connection information using environment variables. Just set these two:
 
 ```bash
 MONGOEASY_CONNECTION_STRING=mongodb://localhost:27017/
 MONGOEASY_DATABASE_NAME=mydatabase
 ```
 
-## Create a document class
-To use Mongeasy you will create a document class that can be used with the collection of choice. To do this you will use the `create_document_class` factory function like this:
+Absolutely, here's a revised version of your examples section:
 
-```python
-from mongeasy import create_document_class
+---
 
+## Create a Document Class
 
-User = create_document_class('User', 'users')
-
-```
+In Mongeasy, you interact with your MongoDB collections through document classes. A document class is a Python class that represents a MongoDB collection and provides methods for interacting with that collection.
 
-The first argument is the name the class will get and the second argument is the name of the collection to use. If the collection does not exist it will be created when you use the class to store documents.
-
-You will not need to assign the returned value to a class variable as in the example above, as the generated class is injected into the current namespace:
+You can create a document class using the `create_document_class` factory function. The first argument is the name you want to give to the class (which should be the singular form of the collection name), and the second argument is the name of the MongoDB collection that the class will interact with.
 
 ```python
 from mongeasy import create_document_class
 
+User = create_document_class('User', 'users')
+```
 
-create_document_class('User', 'users')
+After running this code, `User` becomes a new class that you can use to interact with the 'users' collection in your MongoDB database.
 
-# The class User exist from this point in the code
+## Create and Store a Document
 
-```
-
-## Create a store a document
-You can create a documnet by using the generated class. You can either use keyword arguments or pass a dict.
+Once you have a document class, you can use it to create new documents in your MongoDB collection. You can create a document using keyword arguments or by passing a dictionary. After creating a document, you can save it to your MongoDB collection using the `save` method.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
 # Create a document using keyword arguments
 user1 = User(name='Alice', age=25)
 user1.save()
 
-# Create a document using a dict
+# Create a document using a dictionary
 user2 = User({'name': 'Bob', 'age': 30})
 user2.save()
-
 ```
 
-## Find documents
-You can find documents using the `find` method on the generated class. This method will return a list of documents.
+In this example, `user1` and `user2` are instances of the `User` document class. When you call the `save` method on these instances, Mongeasy automatically inserts them into the 'users' collection in your MongoDB database.
+
+## Find Documents
+
+You can retrieve documents from your MongoDB collection using the `find` method on your document class. This method returns a `ResultList` object that contains the found documents.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
-# Find all documents
+# Find all documents in the 'users' collection
 users = User.all()
 
 # Find all documents with age 25
 users = User.find({'age': 25})
-
 ```
-### Find one document
-You can find one document using the `find` method on the generated class.
 
-Find will return a ResultList object that can be used to get the first, or last, document in the list. If no document is found None is returned.
+In the first `find` example, Mongeasy returns all documents in the 'users' collection. In the second example, Mongeasy only returns documents where the 'age' field is 25.
+
+Find also has a lazy flag (defeault set to False) which when set to True, returns a lazy query object instead of a result list. This is useful when you want to iterate over a large number of documents without loading them all into memory at once.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
-# Find one document with age 25
-user = User.find({'age': 25}).first()
+# Find all documents in the 'users' collection
+users = User.all(lazy=True)
 
-if user is None:
-    print('No user found')
+# Find all documents with age 25
 
+users = User.find({'age': 25}, lazy=True)
 ```
 
-## Update a document
-You can update a document just by changing the attributes and then calling the `save` method.
+## Update a Document
+
+You can update a document by changing its attributes and then calling the `save` method. Mongeasy automatically updates the corresponding document in your MongoDB collection.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
 # Find one document with age 25
 user = User.find({'age': 25}).first()
 
-if user is None:
-    print('No user found')
-else:
+if user is not None:
     # Update the age of the user
     user.age = 26
     user.save()
 ```
 
-## Delete a document
-You can delete a document by calling the `delete` method on the document.
+In this example, Mongeasy first retrieves the document where the 'age' field is 25. Then, it changes the 'age' field of the document to 26 and saves the document back to the MongoDB collection.
+
+## Delete a Document
+
+You can remove a document from your MongoDB collection by calling the `delete` method on an instance of your document class.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
 # Find one document with age 25
 user = User.find({'age': 25}).first()
 
-if user is None:
-    print('No user found')
-else:
-    # Delete the user
+if user is not None:
     user.delete()
 ```
 
-You can also delete all documents in a collection by calling the `delete` method on the generated class.
+In this example, Mongeasy first retrieves the document where the 'age' field is 25. Then, it deletes that document from the 'users' collection in your MongoDB database.
+
+
+You can also delete all documents in a collection by calling the `delete_many` class method on the generated class.
 
 ```python
 from mongeasy import create_document_class
 
 
 User = create_document_class('User', 'users')
 
 
 # Delete using a filter
-User.delete({'age': 25})
+User.delete_many({'age': 25})
 
 # Delete all documents in the collection
-User.delete()
+User.delete_many()
 ```
 
+The `delete_many`method is useful when you want to delete multiple documents at once. The first call above deletes all users with age 25, and the second call deletes all users in the collection. 
+
+---
 ## Indexes
 You can create indexes on the collection by using the `create_index` method on the generated class.
 
 ```python
 from mongeasy import create_document_class
 
 
@@ -301,15 +310,15 @@
 except ValueError as e:
     print(e)
 ```
 
 This approach makes it easier to write, read, and manage your database queries in Python, providing a more user-friendly interface for MongoDB.
 
 ## ResultList
-All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
+All queries that can return more than one document will return a `ResultList` object, if not the lazy flag has been set. This object can be used to get the first or last document in the list, or None if no document is found.
 
 
 ```python
 from mongeasy import create_document_class
 
 
 User = create_document_class('User', 'users')
@@ -329,14 +338,33 @@
 * `last_or_none` - Get the last document in the list or None if no document is found, same as last
 * `map` - Apply a given function to each element in the list and return a new ResultList containing the results
 * `filter` - Filter the list using a given function and return a new ResultList containing the results
 * `reduce` - Apply a given function to each element in the list and return a single value
 * `group_by` - Group the list by a given key and return a dict with the results grouped by the key
 * `random` - Get a random document from the list or None if no document is found
 
+
+If lazy loading is enabled a LazyResultList. LazyResultList is a lazy version of Result list. It will cache the result of the query and only load the documents when they are accessed. This can be useful if you want to load the documents later or if you want to use the list in a for loop.
+
+Methods in the LazyResultList are
+* `first` - Get the first document in the list 
+* `next` - Get the next document in the list 
+
+Note that LazyResultList uses the PyMongo cursor generator. If you want to access the cursor directly you can use the `raw_query` method on the Document class.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find one document with age 25
+users = User.raw_query({'age': 25})
+```
+
 ## Mongeasy Plugin System
 
 The Mongeasy library provides a robust and flexible platform for interacting with MongoDB databases. To further enhance its utility and versatility, Mongeasy offers a plugin system. This system allows developers to customize and extend the library's functionality according to their specific needs.
 
 The motivation behind the plugin system is to provide a mechanism for developers to introduce new behaviors or modify existing ones without having to alter the core library code. By doing so, it promotes a modular approach where additional features or modifications can be encapsulated within individual plugins. This system fosters a more maintainable codebase, as plugins can be added, removed, or updated independently, without impacting the overall stability or functionality of the library.
 
 The plugin system can be particularly beneficial in scenarios where customized behaviors or additional features are required. These might include logging operations, implementing custom data validation or transformation rules, handling errors in specific ways, or integrating with other systems or libraries.
@@ -452,16 +480,16 @@
 plugins:
   - your_plugin_name.YourPluginClass
 ```
 
 As always, when developing a plugin, remember to respect the privacy and security of the user's data.
 
 ## Planned features
-* Enable lazy-loading of query results and support for query chaining
-* Implement a schema plugin system to allow for validation and type checking of documents
+* ~~Enable lazy-loading of query results and support for query chaining~~
+* ~~Implement a schema plugin system to allow for validation and type checking of documents~~
 * Add support for transactions using resource management
 * Implement logging and profiling to aid with debugging and performance tuning
 * Enable asynchronous I/O support for improved scalability
 * Implement caching with customizable caching strategies
 * Add support for background tasks using a task queue
 * Implement a paginator utility to allow for pagination of query results
 * Support for MongoDB Atlas search
```

### Comparing `mongeasy-0.2.1/README.md` & `mongeasy-0.2.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 # Mongeasy
 
-Mongeasy is a easy to use library to be used for simple access to a MongoDB database, without any need for schemas or validation. Just store the data as it is used in your application.
+Mongeasy is a powerful yet easy-to-use Python library for interacting with MongoDB databases. Embracing the dynamic nature of Python and MongoDB, Mongeasy eliminates the need for rigid schemas and validation layers. This means you can store and handle data in its natural form, just as it is used in your application, enhancing code readability and efficiency.
+
+However, Mongeasy's flexibility doesn't mean it compromises on control. With its built-in plugin system, you can hook into the lifecycle of a document and the database connection, enabling advanced features like data validation, logging, and more as per your application's requirements.
+
+Whether you're developing a small personal project or a large-scale production application, Mongeasy helps you focus more on your application logic, and less on managing your database. Experience the freedom of schema-less design with the power of customization, all bundled in a single, user-friendly package.
 
 ## Installation
 Mongoeasy is available on PyPI and can be installed using pip:
 
 ```bash
 pip install mongeasy
 ```
 
 ## Documentation
 The documentation can be found at [https://mongeasy.readthedocs.io](https://mongeasy.readthedocs.io)
 
-## What's new in version 0.2.0?
-### New plugin system
-Mongeasy now has a plugin system that allows you to hook into the lifecycle of a document and the database connection. This allows you to do things like validation, logging, and more.
+## What's new in version 0.2.2?
+### Support for lazy queries
+The find method now supports a lazy flag (defeault set to False) which when set to True, returns a lazy query object instead of a result list. This is useful when you want to iterate over a large number of documents without loading them all into memory at once.
+
+```python
+from mongeasy import create_document_class
+
+User = create_document_class('User', 'users')
 
-See documentation for this feature below.
+# Find all documents in the 'users' collection
+users = User.all(lazy=True)
 
-### Breaking changes
+# Find all documents with age 25
+users = User.find({'age': 25}, lazy=True)
+```
+
+### Breaking changes (0.2.0)
 The class method `delete` has been renamed to `delete_many` as the name conflicted with the instance method `delete`.
 
 --------------------
 
 ## Connection
-Connection to the database is handled automtically for you if you have the conenction information in a configfile or set as environment variables.
+Connection to the database is handled automatically for you if you have the connection information in a configfile or set as environment variables.
 
 ### Connection using configfile
 Create a file called `mongeasy_config.yml` and place it in your project root folder.
 
 The contents of the file should be:
 
 ```bash
@@ -41,148 +55,143 @@
 You can, as an alternative method, define your connection information using environment variables. Just set these two:
 
 ```bash
 MONGOEASY_CONNECTION_STRING=mongodb://localhost:27017/
 MONGOEASY_DATABASE_NAME=mydatabase
 ```
 
-## Create a document class
-To use Mongeasy you will create a document class that can be used with the collection of choice. To do this you will use the `create_document_class` factory function like this:
+Absolutely, here's a revised version of your examples section:
 
-```python
-from mongeasy import create_document_class
+---
 
+## Create a Document Class
 
-User = create_document_class('User', 'users')
-
-```
+In Mongeasy, you interact with your MongoDB collections through document classes. A document class is a Python class that represents a MongoDB collection and provides methods for interacting with that collection.
 
-The first argument is the name the class will get and the second argument is the name of the collection to use. If the collection does not exist it will be created when you use the class to store documents.
-
-You will not need to assign the returned value to a class variable as in the example above, as the generated class is injected into the current namespace:
+You can create a document class using the `create_document_class` factory function. The first argument is the name you want to give to the class (which should be the singular form of the collection name), and the second argument is the name of the MongoDB collection that the class will interact with.
 
 ```python
 from mongeasy import create_document_class
 
+User = create_document_class('User', 'users')
+```
 
-create_document_class('User', 'users')
+After running this code, `User` becomes a new class that you can use to interact with the 'users' collection in your MongoDB database.
 
-# The class User exist from this point in the code
+## Create and Store a Document
 
-```
-
-## Create a store a document
-You can create a documnet by using the generated class. You can either use keyword arguments or pass a dict.
+Once you have a document class, you can use it to create new documents in your MongoDB collection. You can create a document using keyword arguments or by passing a dictionary. After creating a document, you can save it to your MongoDB collection using the `save` method.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
 # Create a document using keyword arguments
 user1 = User(name='Alice', age=25)
 user1.save()
 
-# Create a document using a dict
+# Create a document using a dictionary
 user2 = User({'name': 'Bob', 'age': 30})
 user2.save()
-
 ```
 
-## Find documents
-You can find documents using the `find` method on the generated class. This method will return a list of documents.
+In this example, `user1` and `user2` are instances of the `User` document class. When you call the `save` method on these instances, Mongeasy automatically inserts them into the 'users' collection in your MongoDB database.
+
+## Find Documents
+
+You can retrieve documents from your MongoDB collection using the `find` method on your document class. This method returns a `ResultList` object that contains the found documents.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
-# Find all documents
+# Find all documents in the 'users' collection
 users = User.all()
 
 # Find all documents with age 25
 users = User.find({'age': 25})
-
 ```
-### Find one document
-You can find one document using the `find` method on the generated class.
 
-Find will return a ResultList object that can be used to get the first, or last, document in the list. If no document is found None is returned.
+In the first `find` example, Mongeasy returns all documents in the 'users' collection. In the second example, Mongeasy only returns documents where the 'age' field is 25.
+
+Find also has a lazy flag (defeault set to False) which when set to True, returns a lazy query object instead of a result list. This is useful when you want to iterate over a large number of documents without loading them all into memory at once.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
-# Find one document with age 25
-user = User.find({'age': 25}).first()
+# Find all documents in the 'users' collection
+users = User.all(lazy=True)
 
-if user is None:
-    print('No user found')
+# Find all documents with age 25
 
+users = User.find({'age': 25}, lazy=True)
 ```
 
-## Update a document
-You can update a document just by changing the attributes and then calling the `save` method.
+## Update a Document
+
+You can update a document by changing its attributes and then calling the `save` method. Mongeasy automatically updates the corresponding document in your MongoDB collection.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
 # Find one document with age 25
 user = User.find({'age': 25}).first()
 
-if user is None:
-    print('No user found')
-else:
+if user is not None:
     # Update the age of the user
     user.age = 26
     user.save()
 ```
 
-## Delete a document
-You can delete a document by calling the `delete` method on the document.
+In this example, Mongeasy first retrieves the document where the 'age' field is 25. Then, it changes the 'age' field of the document to 26 and saves the document back to the MongoDB collection.
+
+## Delete a Document
+
+You can remove a document from your MongoDB collection by calling the `delete` method on an instance of your document class.
 
 ```python
 from mongeasy import create_document_class
 
-
 User = create_document_class('User', 'users')
 
 # Find one document with age 25
 user = User.find({'age': 25}).first()
 
-if user is None:
-    print('No user found')
-else:
-    # Delete the user
+if user is not None:
     user.delete()
 ```
 
-You can also delete all documents in a collection by calling the `delete` method on the generated class.
+In this example, Mongeasy first retrieves the document where the 'age' field is 25. Then, it deletes that document from the 'users' collection in your MongoDB database.
+
+
+You can also delete all documents in a collection by calling the `delete_many` class method on the generated class.
 
 ```python
 from mongeasy import create_document_class
 
 
 User = create_document_class('User', 'users')
 
 
 # Delete using a filter
-User.delete({'age': 25})
+User.delete_many({'age': 25})
 
 # Delete all documents in the collection
-User.delete()
+User.delete_many()
 ```
 
+The `delete_many`method is useful when you want to delete multiple documents at once. The first call above deletes all users with age 25, and the second call deletes all users in the collection. 
+
+---
 ## Indexes
 You can create indexes on the collection by using the `create_index` method on the generated class.
 
 ```python
 from mongeasy import create_document_class
 
 
@@ -281,15 +290,15 @@
 except ValueError as e:
     print(e)
 ```
 
 This approach makes it easier to write, read, and manage your database queries in Python, providing a more user-friendly interface for MongoDB.
 
 ## ResultList
-All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
+All queries that can return more than one document will return a `ResultList` object, if not the lazy flag has been set. This object can be used to get the first or last document in the list, or None if no document is found.
 
 
 ```python
 from mongeasy import create_document_class
 
 
 User = create_document_class('User', 'users')
@@ -309,14 +318,33 @@
 * `last_or_none` - Get the last document in the list or None if no document is found, same as last
 * `map` - Apply a given function to each element in the list and return a new ResultList containing the results
 * `filter` - Filter the list using a given function and return a new ResultList containing the results
 * `reduce` - Apply a given function to each element in the list and return a single value
 * `group_by` - Group the list by a given key and return a dict with the results grouped by the key
 * `random` - Get a random document from the list or None if no document is found
 
+
+If lazy loading is enabled a LazyResultList. LazyResultList is a lazy version of Result list. It will cache the result of the query and only load the documents when they are accessed. This can be useful if you want to load the documents later or if you want to use the list in a for loop.
+
+Methods in the LazyResultList are
+* `first` - Get the first document in the list 
+* `next` - Get the next document in the list 
+
+Note that LazyResultList uses the PyMongo cursor generator. If you want to access the cursor directly you can use the `raw_query` method on the Document class.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find one document with age 25
+users = User.raw_query({'age': 25})
+```
+
 ## Mongeasy Plugin System
 
 The Mongeasy library provides a robust and flexible platform for interacting with MongoDB databases. To further enhance its utility and versatility, Mongeasy offers a plugin system. This system allows developers to customize and extend the library's functionality according to their specific needs.
 
 The motivation behind the plugin system is to provide a mechanism for developers to introduce new behaviors or modify existing ones without having to alter the core library code. By doing so, it promotes a modular approach where additional features or modifications can be encapsulated within individual plugins. This system fosters a more maintainable codebase, as plugins can be added, removed, or updated independently, without impacting the overall stability or functionality of the library.
 
 The plugin system can be particularly beneficial in scenarios where customized behaviors or additional features are required. These might include logging operations, implementing custom data validation or transformation rules, handling errors in specific ways, or integrating with other systems or libraries.
@@ -432,16 +460,16 @@
 plugins:
   - your_plugin_name.YourPluginClass
 ```
 
 As always, when developing a plugin, remember to respect the privacy and security of the user's data.
 
 ## Planned features
-* Enable lazy-loading of query results and support for query chaining
-* Implement a schema plugin system to allow for validation and type checking of documents
+* ~~Enable lazy-loading of query results and support for query chaining~~
+* ~~Implement a schema plugin system to allow for validation and type checking of documents~~
 * Add support for transactions using resource management
 * Implement logging and profiling to aid with debugging and performance tuning
 * Enable asynchronous I/O support for improved scalability
 * Implement caching with customizable caching strategies
 * Add support for background tasks using a task queue
 * Implement a paginator utility to allow for pagination of query results
 * Support for MongoDB Atlas search
```

### Comparing `mongeasy-0.2.1/mongeasy/__init__.py` & `mongeasy-0.2.2/mongeasy/__init__.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/mongeasy/base_dict.py` & `mongeasy-0.2.2/mongeasy/base_dict.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/mongeasy/connection.py` & `mongeasy-0.2.2/mongeasy/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,22 +50,26 @@
         config_path = os.path.join(os.getcwd(), 'mongeasy_config.yml')
 
         # Check if the configuration file exists
         if os.path.exists(config_path):
             # Read the configuration from the file
             with open(config_path, 'r') as f:
                 config = yaml.safe_load(f)
+                if config is None:
+                    config = {}
                 db_config = config.get('db_config', {})
 
-            if self.uri is None:
-                self.uri = db_config.get('uri', None)
-            if self.database is None:
-                self.database = db_config.get('database', None)
-            if self.connection_options is None:
-                self.connection_options = db_config.get('connection_options', None)
+            if db_config != {}:
+    
+                if self.uri is None:
+                    self.uri = db_config.get('uri', None)
+                if self.database is None:
+                    self.database = db_config.get('database', None)
+                if self.connection_options is None:
+                    self.connection_options = db_config.get('connection_options', None)
 
             # Handle plugins
             from mongeasy import registry
             plugins_paths = config.get('plugins', [])
             for plugin_path in plugins_paths:
                 plugin = import_string(plugin_path)()
                 registry.register_plugin(plugin)
```

### Comparing `mongeasy-0.2.1/mongeasy/core.py` & `mongeasy-0.2.2/mongeasy/core.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/mongeasy/document.py` & `mongeasy-0.2.2/mongeasy/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import json
 import bson
 from mongeasy.exceptions import MongeasyDBCollectionError, MongeasyFieldError, MongeasyDBDocumentError, MongeasyIndexException
 from mongeasy.plugins.registry import Hook, plugin_dispatcher
 from mongeasy.base_dict import BaseDict
 from mongeasy.core import Query
 from mongeasy.resultlist import ResultList
+from mongeasy.lazy_resultlist import LazyResultList
 import pymongo
 
 
 class Document(BaseDict):
     """
     This class acts as the base class for collection classes. Each instance of the subclasses
     will represent a single document
@@ -288,30 +289,36 @@
                 Document.logger.exception(f"Error inserting item: {item}. Exception: {e}")
 
     @classmethod
     @plugin_dispatcher([
         {'hook': Hook.BEFORE_QUERY_DOCUMENT, 'when': 'pre'},
         {'hook': Hook.AFTER_QUERY_DOCUMENT, 'when': 'post'},
         ])
-    def find(cls, *args, **kwargs):
+    def find(cls, *args, lazy=False, **kwargs):
         """
         Find a document that matches the keywords
         :param arg: positional arguments
+        :param lazy: Whether to use lazy loading. Default is False.
         :param kwargs: keyword arguments or dict to match
-        :return: ResultList
+        :return: ResultList or LazyResultList
         """
         # Handle positional arguments
         if len(args) == 1 and isinstance(args[0], dict):
             as_dict = copy(args[0])
         if len(args) == 1 and isinstance(args[0], Query):
             as_dict = args[0].to_mongo_query()
         elif len(args) == 0:
             as_dict = copy(kwargs)
 
-        return ResultList(cls(item) for item in cls.collection.find(as_dict))
+        cursor = cls.collection.find(as_dict)
+        if lazy:
+            return LazyResultList(cursor, cls)
+        else:
+            return ResultList(cls(item) for item in cursor)
+
 
     @classmethod
     def find_in(cls, field:str, values:list) -> ResultList:
         """
         Find a document that matches the keywords
         :param field: str, the field to search in
         :param values: list, the values to search for
```

### Comparing `mongeasy-0.2.1/mongeasy/dynamics.py` & `mongeasy-0.2.2/mongeasy/dynamics.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/mongeasy/exceptions.py` & `mongeasy-0.2.2/mongeasy/exceptions.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/mongeasy/plugins/registry.py` & `mongeasy-0.2.2/mongeasy/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/mongeasy/resultlist.py` & `mongeasy-0.2.2/mongeasy/resultlist.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/mongeasy/utils/utils.py` & `mongeasy-0.2.2/mongeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/sample_plugins/__init__.py` & `mongeasy-0.2.2/sample_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/sample_plugins/pydantic_validator.py` & `mongeasy-0.2.2/sample_plugins/pydantic_validator.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.1/setup.py` & `mongeasy-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     readme = f.read()
 
 with open("LICENSE", encoding="utf8") as f:
     license = f.read()
 
 setup(
     name="mongeasy",
-    version="0.2.1",
+    version="0.2.2",
     author="Joakim Wassberg",
     author_email="joakim.wassberg@arthead.se",
     description="Easy to use wrapper around pymongo for easy access to MongoDB.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/artheadsweden/mongeasy",
     license="MIT",
```

### Comparing `mongeasy-0.2.1/tests/test_mongeasy.py` & `mongeasy-0.2.2/tests/test_mongeasy.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import os
 os.environ['MONGOEASY_CONNECTION_STRING'] = 'mongodb://localhost:27017'
 os.environ['MONGOEASY_DATABASE_NAME'] = 'mongeasy_pytest'
 from pymongo import MongoClient
 import pytest
 from mongeasy import create_document_class
 from mongeasy.exceptions import MongeasyDBDocumentError
+from mongeasy.resultlist import ResultList
+from mongeasy.lazy_resultlist import LazyResultList
 
 
 @pytest.fixture(scope='function')
 def clean_mongo():
     # Connect to MongoDB
     client = MongoClient('mongodb://localhost:27017')
     db = client['mongeasy_pytest']
@@ -354,8 +356,44 @@
         q.to_mongo_query()
     assert "Invalid query string" in str(excinfo.value)
 
 def test_unmatched_parentheses():
     with pytest.raises(ValueError) as excinfo:
         q = Query("(age > 25 and (name == 'John'")  # Unmatched parentheses
         q.to_mongo_query()
-    assert "Invalid query string" in str(excinfo.value)
+    assert "Invalid query string" in str(excinfo.value)
+
+
+####################
+# Test Lazyness    #
+####################
+
+def test_lazy_result_list(clean_mongo):
+    client = MongoClient('mongodb://localhost:27017')
+    db = client['mongeasy_pytest']
+    collection = db['users']
+    documents = [{'name': f'user{i}', 'age': i} for i in range(10)]
+    collection.insert_many(documents)
+    User = create_document_class('User', 'users')
+    cursor = collection.find({})
+    lazy_result_list = LazyResultList(cursor, User)
+
+    # Test that we can iterate over the LazyResultList
+    for i, document in enumerate(lazy_result_list):
+        assert document['name'] == f'user{i}'
+        assert document['age'] == i
+
+ 
+def test_lazy_result_list_with_query(clean_mongo):
+    client = MongoClient('mongodb://localhost:27017')
+    db = client['mongeasy_pytest']
+    collection = db['users']
+    documents = [{'name': f'user{i}', 'age': i} for i in range(10)]
+    collection.insert_many(documents)
+    User = create_document_class('User', 'users')
+    q = Query('age > 5')
+    lazy_result_list = User.find(q, lazy=True)
+
+    # Test that we can iterate over the LazyResultList
+    for i, document in enumerate(lazy_result_list):
+        assert document['name'] == f'user{i+6}'
+        assert document['age'] == i+6
```

### Comparing `mongeasy-0.2.1/tests/test_plugins.py` & `mongeasy-0.2.2/tests/test_plugins.py`

 * *Files identical despite different names*

