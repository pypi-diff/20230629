# Comparing `tmp/django-airplane-1.1.0.tar.gz` & `tmp/django-airplane-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-airplane-1.1.0.tar", last modified: Thu Mar 19 13:37:49 2020, max compression
+gzip compressed data, was "django-airplane-1.1.1.tar", last modified: Thu Jun 29 20:54:26 2023, max compression
```

## Comparing `django-airplane-1.1.0.tar` & `django-airplane-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2020-03-19 13:37:49.000000 django-airplane-1.1.0/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1087 2018-10-28 15:17:06.000000 django-airplane-1.1.0/LICENSE
--rw-r--r--   0 ctrudeau   (501) staff       (20)       35 2018-10-28 15:17:06.000000 django-airplane-1.1.0/MANIFEST.in
--rw-r--r--   0 ctrudeau   (501) staff       (20)     6999 2020-03-19 13:37:49.000000 django-airplane-1.1.0/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)     4800 2020-03-19 13:34:56.000000 django-airplane-1.1.0/README.rst
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2020-03-19 13:37:49.000000 django-airplane-1.1.0/airplane/
--rw-r--r--   0 ctrudeau   (501) staff       (20)      193 2020-03-19 13:34:56.000000 django-airplane-1.1.0/airplane/__init__.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2020-03-19 13:37:49.000000 django-airplane-1.1.0/airplane/management/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-10-28 15:17:06.000000 django-airplane-1.1.0/airplane/management/__init__.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2020-03-19 13:37:49.000000 django-airplane-1.1.0/airplane/management/commands/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-10-28 15:17:06.000000 django-airplane-1.1.0/airplane/management/commands/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      409 2020-03-19 13:34:56.000000 django-airplane-1.1.0/airplane/management/commands/aircache.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      986 2020-03-19 13:34:56.000000 django-airplane-1.1.0/airplane/management/commands/airinfo.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)        8 2018-10-28 15:17:06.000000 django-airplane-1.1.0/airplane/models.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      308 2020-03-19 13:34:56.000000 django-airplane-1.1.0/airplane/pathing.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2020-03-19 13:37:49.000000 django-airplane-1.1.0/airplane/templatetags/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-10-28 15:17:06.000000 django-airplane-1.1.0/airplane/templatetags/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1273 2020-03-19 13:34:56.000000 django-airplane-1.1.0/airplane/templatetags/airplanetags.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2020-03-19 13:37:49.000000 django-airplane-1.1.0/airplane/tests/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-10-28 15:17:06.000000 django-airplane-1.1.0/airplane/tests/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     8388 2020-03-19 13:34:56.000000 django-airplane-1.1.0/airplane/tests/test_airplane.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3520 2020-03-19 13:34:56.000000 django-airplane-1.1.0/airplane/utils.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2020-03-19 13:37:49.000000 django-airplane-1.1.0/django_airplane.egg-info/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     6999 2020-03-19 13:37:49.000000 django-airplane-1.1.0/django_airplane.egg-info/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)      596 2020-03-19 13:37:49.000000 django-airplane-1.1.0/django_airplane.egg-info/SOURCES.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2020-03-19 13:37:49.000000 django-airplane-1.1.0/django_airplane.egg-info/dependency_links.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)       30 2020-03-19 13:37:49.000000 django-airplane-1.1.0/django_airplane.egg-info/requires.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        9 2020-03-19 13:37:49.000000 django-airplane-1.1.0/django_airplane.egg-info/top_level.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2020-03-19 13:37:49.000000 django-airplane-1.1.0/setup.cfg
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1469 2020-03-19 13:34:56.000000 django-airplane-1.1.0/setup.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:54:26.453204 django-airplane-1.1.1/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1087 2018-10-28 15:17:06.000000 django-airplane-1.1.1/LICENSE
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       35 2018-10-28 15:17:06.000000 django-airplane-1.1.1/MANIFEST.in
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     5854 2023-06-29 20:54:26.452886 django-airplane-1.1.1/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     4938 2023-06-29 20:19:14.000000 django-airplane-1.1.1/README.rst
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:54:26.448439 django-airplane-1.1.1/airplane/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      191 2023-06-29 20:50:13.000000 django-airplane-1.1.1/airplane/__init__.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:54:26.448744 django-airplane-1.1.1/airplane/management/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-10-28 15:17:06.000000 django-airplane-1.1.1/airplane/management/__init__.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:54:26.449544 django-airplane-1.1.1/airplane/management/commands/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-10-28 15:17:06.000000 django-airplane-1.1.1/airplane/management/commands/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      409 2020-03-19 13:34:56.000000 django-airplane-1.1.1/airplane/management/commands/aircache.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      986 2020-03-19 13:34:56.000000 django-airplane-1.1.1/airplane/management/commands/airinfo.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        8 2018-10-28 15:17:06.000000 django-airplane-1.1.1/airplane/models.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      308 2020-03-19 13:34:56.000000 django-airplane-1.1.1/airplane/pathing.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:54:26.450146 django-airplane-1.1.1/airplane/templatetags/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-10-28 15:17:06.000000 django-airplane-1.1.1/airplane/templatetags/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1273 2020-03-19 13:34:56.000000 django-airplane-1.1.1/airplane/templatetags/airplanetags.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:54:26.450704 django-airplane-1.1.1/airplane/tests/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-10-28 15:17:06.000000 django-airplane-1.1.1/airplane/tests/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     8388 2020-03-19 13:34:56.000000 django-airplane-1.1.1/airplane/tests/test_airplane.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3497 2023-06-29 19:29:44.000000 django-airplane-1.1.1/airplane/utils.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:54:26.452477 django-airplane-1.1.1/django_airplane.egg-info/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     5854 2023-06-29 20:54:26.000000 django-airplane-1.1.1/django_airplane.egg-info/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      596 2023-06-29 20:54:26.000000 django-airplane-1.1.1/django_airplane.egg-info/SOURCES.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2023-06-29 20:54:26.000000 django-airplane-1.1.1/django_airplane.egg-info/dependency_links.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       27 2023-06-29 20:54:26.000000 django-airplane-1.1.1/django_airplane.egg-info/requires.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        9 2023-06-29 20:54:26.000000 django-airplane-1.1.1/django_airplane.egg-info/top_level.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2023-06-29 20:54:26.453292 django-airplane-1.1.1/setup.cfg
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1566 2023-06-29 20:14:24.000000 django-airplane-1.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-airplane-1.1.0/LICENSE` & `django-airplane-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-airplane-1.1.0/PKG-INFO` & `django-airplane-1.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,192 +1,197 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-airplane
-Version: 1.1.0
+Version: 1.1.1
 Summary: Django app that caches CDN files for use when coding offline 
 Home-page: https://github.com/cltrudeau/django-airplane
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
-Description: django-airplane
-        ***************
-        
-        This app is to help in those situations where you can't get on the network but
-        you want to write some Django code.  Surround your static CDN references (like
-        jquery and the like) with this template tag and when you turn it on the URLs
-        will be re-written from a local copy.
-        
-        Installation
-        ============
-        
-        In your settings file, add 'airplane' to your ``settings.INSTALLED_APPS`` field:
-        
-        .. code-block:: python
-        
-            INSTALLED_APPS = (
-                ...
-                'airplane',
-            )
-        
-        Also in settings, make the following additions:
-        
-        .. code-block:: python
-        
-            import airplane
-        
-            STATICFILES_DIRS = (
-                airplane.cache_path(),
-            )
-        
-            AIRPLANE_MODE = airplane.BUILD_CACHE
-            #AIRPLANE_MODE = airplane.USE_CACHE
-            #AIRPLANE_MODE = airplane.AUTO_CACHE
-        
-        Now use the ``airplane`` tag in your templates
-        
-        .. code-block:: html
-        
-            {% load airplanetags %}
-        
-            <html>
-                <head>
-                    <link rel="stylesheet"
-                        href="{% airplane 'https://maxcdn.bootstrapcdn.com/bootstrap.min.css' %}">
-                </head>
-            </html>
-        
-        Change the ``AIRPLANE_MODE`` setting to ``airplane.USE_CACHE`` and subsequent
-        calls to the ``{% airplane %}`` tag will return a reference to the locally 
-        cached version.
-        
-        
-        Settings
-        ========
-        
-        Airplane only does something if ``DEBUG=True`` and if you have an
-        ``AIRPLANE_MODE`` value set to ``airplane.BUILD_CACHE``,
-        ``airplane.USE_CACHE``, or ``airplane.AUTO_CACHE``.  If one of these
-        conditions is not met, the tag simply returns the value passed in.
-        
-        For example, if ``DEBUG=False`` and your template contains:
-        
-        .. code-block:: html
-        
-            <link rel="stylesheet"
-                href="{% airplane 'https://maxcdn.bootstrapcdn.com/bootstrap.min.css' %}">
-        
-        
-        Then the above snippet renders as:
-        
-        .. code-block:: html
-        
-            <link rel="stylesheet"
-                href="https://maxcdn.bootstrapcdn.com/bootstrap.min.css">
-        
-        
-        When ``AIRPLANE_MODE`` is set to ``airplane.BUILD_CACHE`` any URLs passed in
-        are fetched and their contents added to a local cache.  The default local
-        cache is ``.airport_cache`` relative to the base directory of your project.
-        
-        You can change the location of the cache by setting ``AIRPLANE_CACHE``.  The
-        setting accepts either fully qualified paths or paths relative to the
-        project's base directory.
-        
-        .. code-block:: python
-        
-            # settings.py
-        
-            AIRPLANE_CACHE = /foo/bar/cache     # fully qualified
-        
-            # or
-        
-            AIRPLANE_CACHE = my_cache           # relative to settings.BASE_DIR
-        
-            # or nothing, defaults to settings.BASEDIR + '.airplane_cache'
-        
-        
-        Once you have cached all the files you are using, switch ``AIRPLANE_MODE`` to
-        ``airplane.USE_CACHE``.  All URLs are now re-written to point to the contents
-        of the local cache.
-        
-        Alternatively, you can set ``AIRPLANE_MODE`` to ``airplane.AUTO_CACHE`` and
-        the first call will cache the file and subsequent calls will use the cached
-        copy.
-        
-        Commands
-        ========
-        
-        The following django commands come with airplane.
-        
-        airinfo
-        -------
-        
-        .. code-block:: sh
-        
-            $ ./manage.py airinfo
-            Cache mode: AUTO_CACHE
-            Cache directory: /Users/foo/sample_site/.airplane_cache
-            Cache contents:
-               https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css
-        
-        
-        This command takes no arguments and displays information about the cache. The
-        current mode, the path of the directory and any items cached inside are shown.
-        
-        
-        aircache
-        --------
-        
-        .. code-block:: sh
-        
-            ./manage.py aircache https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css
-        
-        This command takes a single URL as an argument and caches the contents of the
-        URL.
-        
-        Schemaless URLs
-        ===============
-        
-        As airplane is a template tag library, it doesn't have access to the request
-        object at execution. In order to allow schemaless URLs, the code makes the
-        assumption that the schema is "https" if it is not given in the URL.
-        
-        Limitations
-        ===========
-        
-        The intent of this library is to help you when you're using the Django
-        debugging server and in a situation where you can't easily get to the network.
-        Cached files are served using the django static server code, which means you
-        are limited by what kinds of files it can serve. The static server makes
-        guesses on the mimetype of the file based on file extensions. Airplane naively
-        copies the extension of the file so the cached file has the same ending. This
-        means URLs with weird extensions or those which static serve cannot guess at
-        mimetype, will cause problems. It is not recommended to use django-airplane
-        with files that don't end in typical extensions such as ".css", ".js", ".jpg",
-        ".png" or ".gif".
-        
-        
-        Supports
-        ========
-        
-        django-airplane has been tested with:
-        
-        * Python 3.6, 3.7 and Django 2.2
-        * Python 3.6, 3.7 and Django 3.0
-        
-        Docs
-        ====
-        
-        Docs available at: http://django-airplane.readthedocs.io/en/latest/
-        
-        Source: https://github.com/cltrudeau/django-airplane
-        
 Keywords: django,cache,offline,CDN,static
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+django-airplane
+***************
+
+This app is to help in those situations where you can't get on the network but
+you want to write some Django code.  Surround your static CDN references (like
+jquery and the like) with this template tag and when you turn it on the URLs
+will be re-written from a local copy.
+
+Installation
+============
+
+In your settings file, add 'airplane' to your ``settings.INSTALLED_APPS`` field:
+
+.. code-block:: python
+
+    INSTALLED_APPS = (
+        ...
+        'airplane',
+    )
+
+Also in settings, make the following additions:
+
+.. code-block:: python
+
+    import airplane
+
+    STATICFILES_DIRS = (
+        airplane.cache_path(),
+    )
+
+    AIRPLANE_MODE = airplane.BUILD_CACHE
+    #AIRPLANE_MODE = airplane.USE_CACHE
+    #AIRPLANE_MODE = airplane.AUTO_CACHE
+
+Now use the ``airplane`` tag in your templates
+
+.. code-block:: html
+
+    {% load airplanetags %}
+
+    <html>
+        <head>
+            <link rel="stylesheet"
+                href="{% airplane 'https://maxcdn.bootstrapcdn.com/bootstrap.min.css' %}">
+        </head>
+    </html>
+
+Change the ``AIRPLANE_MODE`` setting to ``airplane.USE_CACHE`` and subsequent
+calls to the ``{% airplane %}`` tag will return a reference to the locally 
+cached version.
+
+
+Settings
+========
+
+Airplane only does something if ``DEBUG=True`` and if you have an
+``AIRPLANE_MODE`` value set to ``airplane.BUILD_CACHE``,
+``airplane.USE_CACHE``, or ``airplane.AUTO_CACHE``.  If one of these
+conditions is not met, the tag simply returns the value passed in.
+
+For example, if ``DEBUG=False`` and your template contains:
+
+.. code-block:: html
+
+    <link rel="stylesheet"
+        href="{% airplane 'https://maxcdn.bootstrapcdn.com/bootstrap.min.css' %}">
+
+
+Then the above snippet renders as:
+
+.. code-block:: html
+
+    <link rel="stylesheet"
+        href="https://maxcdn.bootstrapcdn.com/bootstrap.min.css">
+
+
+When ``AIRPLANE_MODE`` is set to ``airplane.BUILD_CACHE`` any URLs passed in
+are fetched and their contents added to a local cache.  The default local
+cache is ``.airport_cache`` relative to the base directory of your project.
+
+You can change the location of the cache by setting ``AIRPLANE_CACHE``.  The
+setting accepts either fully qualified paths or paths relative to the
+project's base directory.
+
+.. code-block:: python
+
+    # settings.py
+
+    AIRPLANE_CACHE = /foo/bar/cache     # fully qualified
+
+    # or
+
+    AIRPLANE_CACHE = my_cache           # relative to settings.BASE_DIR
+
+    # or nothing, defaults to settings.BASEDIR + '.airplane_cache'
+
+
+Once you have cached all the files you are using, switch ``AIRPLANE_MODE`` to
+``airplane.USE_CACHE``.  All URLs are now re-written to point to the contents
+of the local cache.
+
+Alternatively, you can set ``AIRPLANE_MODE`` to ``airplane.AUTO_CACHE`` and
+the first call will cache the file and subsequent calls will use the cached
+copy.
+
+Commands
+========
+
+The following django commands come with airplane.
+
+airinfo
+-------
+
+.. code-block:: sh
+
+    $ ./manage.py airinfo
+    Cache mode: AUTO_CACHE
+    Cache directory: /Users/foo/sample_site/.airplane_cache
+    Cache contents:
+       https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css
+
+
+This command takes no arguments and displays information about the cache. The
+current mode, the path of the directory and any items cached inside are shown.
+
+
+aircache
+--------
+
+.. code-block:: sh
+
+    ./manage.py aircache https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css
+
+This command takes a single URL as an argument and caches the contents of the
+URL.
+
+Schemaless URLs
+===============
+
+As airplane is a template tag library, it doesn't have access to the request
+object at execution. In order to allow schemaless URLs, the code makes the
+assumption that the schema is "https" if it is not given in the URL.
+
+Limitations
+===========
+
+The intent of this library is to help you when you're using the Django
+debugging server and in a situation where you can't easily get to the network.
+Cached files are served using the django static server code, which means you
+are limited by what kinds of files it can serve. The static server makes
+guesses on the mimetype of the file based on file extensions. Airplane naively
+copies the extension of the file so the cached file has the same ending. This
+means URLs with weird extensions or those which static serve cannot guess at
+mimetype, will cause problems. It is not recommended to use django-airplane
+with files that don't end in typical extensions such as ".css", ".js", ".jpg",
+".png" or ".gif".
+
+
+Supports
+========
+
+django-airplane has been tested with:
+
+* Python 3.8-3.11 and Django 4.1
+* Python 3.8-3.11 and Django 4.2
+
+Older versions tested against Django 2.2 and 3.2, nothing has changed since
+then that should break, but these are no longer test targets
+
+Docs
+====
+
+Docs available at: http://django-airplane.readthedocs.io/en/latest/
+
+Source: https://github.com/cltrudeau/django-airplane
```

#### html2text {}

```diff
@@ -1,18 +1,27 @@
-Metadata-Version: 1.1 Name: django-airplane Version: 1.1.0 Summary: Django app
+Metadata-Version: 2.1 Name: django-airplane Version: 1.1.1 Summary: Django app
 that caches CDN files for use when coding offline Home-page: https://
 github.com/cltrudeau/django-airplane Author: Christopher Trudeau Author-email:
-ctrudeau+pypi@arsensa.com License: MIT Description: django-airplane
-*************** This app is to help in those situations where you can't get on
-the network but you want to write some Django code. Surround your static CDN
-references (like jquery and the like) with this template tag and when you turn
-it on the URLs will be re-written from a local copy. Installation ============
-In your settings file, add 'airplane' to your ``settings.INSTALLED_APPS``
-field: .. code-block:: python INSTALLED_APPS = ( ... 'airplane', ) Also in
-settings, make the following additions: .. code-block:: python import airplane
+ctrudeau+pypi@arsensa.com License: MIT Keywords:
+django,cache,offline,CDN,static Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries ::
+Application Frameworks Classifier: Topic :: Software Development :: Libraries
+:: Python Modules License-File: LICENSE django-airplane *************** This
+app is to help in those situations where you can't get on the network but you
+want to write some Django code. Surround your static CDN references (like
+jquery and the like) with this template tag and when you turn it on the URLs
+will be re-written from a local copy. Installation ============ In your
+settings file, add 'airplane' to your ``settings.INSTALLED_APPS`` field: ..
+code-block:: python INSTALLED_APPS = ( ... 'airplane', ) Also in settings, make
+the following additions: .. code-block:: python import airplane
 STATICFILES_DIRS = ( airplane.cache_path(), ) AIRPLANE_MODE =
 airplane.BUILD_CACHE #AIRPLANE_MODE = airplane.USE_CACHE #AIRPLANE_MODE =
 airplane.AUTO_CACHE Now use the ``airplane`` tag in your templates .. code-
 block:: html {% load airplanetags %}
 Change the ``AIRPLANE_MODE`` setting to ``airplane.USE_CACHE`` and subsequent
 calls to the ``{% airplane %}`` tag will return a reference to the locally
 cached version. Settings ======== Airplane only does something if
@@ -53,18 +62,12 @@
 means you are limited by what kinds of files it can serve. The static server
 makes guesses on the mimetype of the file based on file extensions. Airplane
 naively copies the extension of the file so the cached file has the same
 ending. This means URLs with weird extensions or those which static serve
 cannot guess at mimetype, will cause problems. It is not recommended to use
 django-airplane with files that don't end in typical extensions such as ".css",
 ".js", ".jpg", ".png" or ".gif". Supports ======== django-airplane has been
-tested with: * Python 3.6, 3.7 and Django 2.2 * Python 3.6, 3.7 and Django 3.0
-Docs ==== Docs available at: http://django-airplane.readthedocs.io/en/latest/
-Source: https://github.com/cltrudeau/django-airplane Keywords:
-django,cache,offline,CDN,static Platform: UNKNOWN Classifier: Development
-Status :: 4 - Beta Classifier: Environment :: Web Environment Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Software Development :: Libraries :: Application
-Frameworks Classifier: Topic :: Software Development :: Libraries :: Python
-Modules
+tested with: * Python 3.8-3.11 and Django 4.1 * Python 3.8-3.11 and Django 4.2
+Older versions tested against Django 2.2 and 3.2, nothing has changed since
+then that should break, but these are no longer test targets Docs ==== Docs
+available at: http://django-airplane.readthedocs.io/en/latest/ Source: https://
+github.com/cltrudeau/django-airplane
```

### Comparing `django-airplane-1.1.0/README.rst` & `django-airplane-1.1.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -157,16 +157,19 @@
 
 
 Supports
 ========
 
 django-airplane has been tested with:
 
-* Python 3.6, 3.7 and Django 2.2
-* Python 3.6, 3.7 and Django 3.0
+* Python 3.8-3.11 and Django 4.1
+* Python 3.8-3.11 and Django 4.2
+
+Older versions tested against Django 2.2 and 3.2, nothing has changed since
+then that should break, but these are no longer test targets
 
 Docs
 ====
 
 Docs available at: http://django-airplane.readthedocs.io/en/latest/
 
 Source: https://github.com/cltrudeau/django-airplane
```

#### html2text {}

```diff
@@ -49,10 +49,12 @@
 means you are limited by what kinds of files it can serve. The static server
 makes guesses on the mimetype of the file based on file extensions. Airplane
 naively copies the extension of the file so the cached file has the same
 ending. This means URLs with weird extensions or those which static serve
 cannot guess at mimetype, will cause problems. It is not recommended to use
 django-airplane with files that don't end in typical extensions such as ".css",
 ".js", ".jpg", ".png" or ".gif". Supports ======== django-airplane has been
-tested with: * Python 3.6, 3.7 and Django 2.2 * Python 3.6, 3.7 and Django 3.0
-Docs ==== Docs available at: http://django-airplane.readthedocs.io/en/latest/
-Source: https://github.com/cltrudeau/django-airplane
+tested with: * Python 3.8-3.11 and Django 4.1 * Python 3.8-3.11 and Django 4.2
+Older versions tested against Django 2.2 and 3.2, nothing has changed since
+then that should break, but these are no longer test targets Docs ==== Docs
+available at: http://django-airplane.readthedocs.io/en/latest/ Source: https://
+github.com/cltrudeau/django-airplane
```

### Comparing `django-airplane-1.1.0/airplane/management/commands/airinfo.py` & `django-airplane-1.1.1/airplane/management/commands/airinfo.py`

 * *Files identical despite different names*

### Comparing `django-airplane-1.1.0/airplane/templatetags/airplanetags.py` & `django-airplane-1.1.1/airplane/templatetags/airplanetags.py`

 * *Files identical despite different names*

### Comparing `django-airplane-1.1.0/airplane/tests/test_airplane.py` & `django-airplane-1.1.1/airplane/tests/test_airplane.py`

 * *Files identical despite different names*

### Comparing `django-airplane-1.1.0/airplane/utils.py` & `django-airplane-1.1.1/airplane/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
-import json, uuid 
+import json, uuid
 import requests
 
-from django.utils.http import urlquote_plus
+from urllib.parse import quote
 
 from airplane.pathing import get_cache_path
 
 # =============================================================================
 
 url_filename_map = None
 
@@ -59,27 +59,27 @@
     global url_filename_map
     read_cache_map()
 
     try:
         filename = url_filename_map[url]
     except KeyError:
         # nothing in the cache_map file, try the old filename mapping method
-        filename = urlquote_plus(url)
+        filename = quote(url)
         filename = filename.replace('%', '|')
 
     try:
         path = _create_path(filename)
         if path.exists():
             return filename
     except OSError:
         # bad characters in the filename (old filename format on Windows, for
         # example) will blow up Path, ignore to fall out to error handler
         pass
 
-    # something has gone wrong, can't find the file, return 
+    # something has gone wrong, can't find the file, return
     return None
 
 
 def cache_url(url):
     read_cache_map()
 
     # get the filename, or create a new one
```

### Comparing `django-airplane-1.1.0/django_airplane.egg-info/PKG-INFO` & `django-airplane-1.1.1/django_airplane.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,192 +1,197 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-airplane
-Version: 1.1.0
+Version: 1.1.1
 Summary: Django app that caches CDN files for use when coding offline 
 Home-page: https://github.com/cltrudeau/django-airplane
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
-Description: django-airplane
-        ***************
-        
-        This app is to help in those situations where you can't get on the network but
-        you want to write some Django code.  Surround your static CDN references (like
-        jquery and the like) with this template tag and when you turn it on the URLs
-        will be re-written from a local copy.
-        
-        Installation
-        ============
-        
-        In your settings file, add 'airplane' to your ``settings.INSTALLED_APPS`` field:
-        
-        .. code-block:: python
-        
-            INSTALLED_APPS = (
-                ...
-                'airplane',
-            )
-        
-        Also in settings, make the following additions:
-        
-        .. code-block:: python
-        
-            import airplane
-        
-            STATICFILES_DIRS = (
-                airplane.cache_path(),
-            )
-        
-            AIRPLANE_MODE = airplane.BUILD_CACHE
-            #AIRPLANE_MODE = airplane.USE_CACHE
-            #AIRPLANE_MODE = airplane.AUTO_CACHE
-        
-        Now use the ``airplane`` tag in your templates
-        
-        .. code-block:: html
-        
-            {% load airplanetags %}
-        
-            <html>
-                <head>
-                    <link rel="stylesheet"
-                        href="{% airplane 'https://maxcdn.bootstrapcdn.com/bootstrap.min.css' %}">
-                </head>
-            </html>
-        
-        Change the ``AIRPLANE_MODE`` setting to ``airplane.USE_CACHE`` and subsequent
-        calls to the ``{% airplane %}`` tag will return a reference to the locally 
-        cached version.
-        
-        
-        Settings
-        ========
-        
-        Airplane only does something if ``DEBUG=True`` and if you have an
-        ``AIRPLANE_MODE`` value set to ``airplane.BUILD_CACHE``,
-        ``airplane.USE_CACHE``, or ``airplane.AUTO_CACHE``.  If one of these
-        conditions is not met, the tag simply returns the value passed in.
-        
-        For example, if ``DEBUG=False`` and your template contains:
-        
-        .. code-block:: html
-        
-            <link rel="stylesheet"
-                href="{% airplane 'https://maxcdn.bootstrapcdn.com/bootstrap.min.css' %}">
-        
-        
-        Then the above snippet renders as:
-        
-        .. code-block:: html
-        
-            <link rel="stylesheet"
-                href="https://maxcdn.bootstrapcdn.com/bootstrap.min.css">
-        
-        
-        When ``AIRPLANE_MODE`` is set to ``airplane.BUILD_CACHE`` any URLs passed in
-        are fetched and their contents added to a local cache.  The default local
-        cache is ``.airport_cache`` relative to the base directory of your project.
-        
-        You can change the location of the cache by setting ``AIRPLANE_CACHE``.  The
-        setting accepts either fully qualified paths or paths relative to the
-        project's base directory.
-        
-        .. code-block:: python
-        
-            # settings.py
-        
-            AIRPLANE_CACHE = /foo/bar/cache     # fully qualified
-        
-            # or
-        
-            AIRPLANE_CACHE = my_cache           # relative to settings.BASE_DIR
-        
-            # or nothing, defaults to settings.BASEDIR + '.airplane_cache'
-        
-        
-        Once you have cached all the files you are using, switch ``AIRPLANE_MODE`` to
-        ``airplane.USE_CACHE``.  All URLs are now re-written to point to the contents
-        of the local cache.
-        
-        Alternatively, you can set ``AIRPLANE_MODE`` to ``airplane.AUTO_CACHE`` and
-        the first call will cache the file and subsequent calls will use the cached
-        copy.
-        
-        Commands
-        ========
-        
-        The following django commands come with airplane.
-        
-        airinfo
-        -------
-        
-        .. code-block:: sh
-        
-            $ ./manage.py airinfo
-            Cache mode: AUTO_CACHE
-            Cache directory: /Users/foo/sample_site/.airplane_cache
-            Cache contents:
-               https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css
-        
-        
-        This command takes no arguments and displays information about the cache. The
-        current mode, the path of the directory and any items cached inside are shown.
-        
-        
-        aircache
-        --------
-        
-        .. code-block:: sh
-        
-            ./manage.py aircache https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css
-        
-        This command takes a single URL as an argument and caches the contents of the
-        URL.
-        
-        Schemaless URLs
-        ===============
-        
-        As airplane is a template tag library, it doesn't have access to the request
-        object at execution. In order to allow schemaless URLs, the code makes the
-        assumption that the schema is "https" if it is not given in the URL.
-        
-        Limitations
-        ===========
-        
-        The intent of this library is to help you when you're using the Django
-        debugging server and in a situation where you can't easily get to the network.
-        Cached files are served using the django static server code, which means you
-        are limited by what kinds of files it can serve. The static server makes
-        guesses on the mimetype of the file based on file extensions. Airplane naively
-        copies the extension of the file so the cached file has the same ending. This
-        means URLs with weird extensions or those which static serve cannot guess at
-        mimetype, will cause problems. It is not recommended to use django-airplane
-        with files that don't end in typical extensions such as ".css", ".js", ".jpg",
-        ".png" or ".gif".
-        
-        
-        Supports
-        ========
-        
-        django-airplane has been tested with:
-        
-        * Python 3.6, 3.7 and Django 2.2
-        * Python 3.6, 3.7 and Django 3.0
-        
-        Docs
-        ====
-        
-        Docs available at: http://django-airplane.readthedocs.io/en/latest/
-        
-        Source: https://github.com/cltrudeau/django-airplane
-        
 Keywords: django,cache,offline,CDN,static
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+django-airplane
+***************
+
+This app is to help in those situations where you can't get on the network but
+you want to write some Django code.  Surround your static CDN references (like
+jquery and the like) with this template tag and when you turn it on the URLs
+will be re-written from a local copy.
+
+Installation
+============
+
+In your settings file, add 'airplane' to your ``settings.INSTALLED_APPS`` field:
+
+.. code-block:: python
+
+    INSTALLED_APPS = (
+        ...
+        'airplane',
+    )
+
+Also in settings, make the following additions:
+
+.. code-block:: python
+
+    import airplane
+
+    STATICFILES_DIRS = (
+        airplane.cache_path(),
+    )
+
+    AIRPLANE_MODE = airplane.BUILD_CACHE
+    #AIRPLANE_MODE = airplane.USE_CACHE
+    #AIRPLANE_MODE = airplane.AUTO_CACHE
+
+Now use the ``airplane`` tag in your templates
+
+.. code-block:: html
+
+    {% load airplanetags %}
+
+    <html>
+        <head>
+            <link rel="stylesheet"
+                href="{% airplane 'https://maxcdn.bootstrapcdn.com/bootstrap.min.css' %}">
+        </head>
+    </html>
+
+Change the ``AIRPLANE_MODE`` setting to ``airplane.USE_CACHE`` and subsequent
+calls to the ``{% airplane %}`` tag will return a reference to the locally 
+cached version.
+
+
+Settings
+========
+
+Airplane only does something if ``DEBUG=True`` and if you have an
+``AIRPLANE_MODE`` value set to ``airplane.BUILD_CACHE``,
+``airplane.USE_CACHE``, or ``airplane.AUTO_CACHE``.  If one of these
+conditions is not met, the tag simply returns the value passed in.
+
+For example, if ``DEBUG=False`` and your template contains:
+
+.. code-block:: html
+
+    <link rel="stylesheet"
+        href="{% airplane 'https://maxcdn.bootstrapcdn.com/bootstrap.min.css' %}">
+
+
+Then the above snippet renders as:
+
+.. code-block:: html
+
+    <link rel="stylesheet"
+        href="https://maxcdn.bootstrapcdn.com/bootstrap.min.css">
+
+
+When ``AIRPLANE_MODE`` is set to ``airplane.BUILD_CACHE`` any URLs passed in
+are fetched and their contents added to a local cache.  The default local
+cache is ``.airport_cache`` relative to the base directory of your project.
+
+You can change the location of the cache by setting ``AIRPLANE_CACHE``.  The
+setting accepts either fully qualified paths or paths relative to the
+project's base directory.
+
+.. code-block:: python
+
+    # settings.py
+
+    AIRPLANE_CACHE = /foo/bar/cache     # fully qualified
+
+    # or
+
+    AIRPLANE_CACHE = my_cache           # relative to settings.BASE_DIR
+
+    # or nothing, defaults to settings.BASEDIR + '.airplane_cache'
+
+
+Once you have cached all the files you are using, switch ``AIRPLANE_MODE`` to
+``airplane.USE_CACHE``.  All URLs are now re-written to point to the contents
+of the local cache.
+
+Alternatively, you can set ``AIRPLANE_MODE`` to ``airplane.AUTO_CACHE`` and
+the first call will cache the file and subsequent calls will use the cached
+copy.
+
+Commands
+========
+
+The following django commands come with airplane.
+
+airinfo
+-------
+
+.. code-block:: sh
+
+    $ ./manage.py airinfo
+    Cache mode: AUTO_CACHE
+    Cache directory: /Users/foo/sample_site/.airplane_cache
+    Cache contents:
+       https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css
+
+
+This command takes no arguments and displays information about the cache. The
+current mode, the path of the directory and any items cached inside are shown.
+
+
+aircache
+--------
+
+.. code-block:: sh
+
+    ./manage.py aircache https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css
+
+This command takes a single URL as an argument and caches the contents of the
+URL.
+
+Schemaless URLs
+===============
+
+As airplane is a template tag library, it doesn't have access to the request
+object at execution. In order to allow schemaless URLs, the code makes the
+assumption that the schema is "https" if it is not given in the URL.
+
+Limitations
+===========
+
+The intent of this library is to help you when you're using the Django
+debugging server and in a situation where you can't easily get to the network.
+Cached files are served using the django static server code, which means you
+are limited by what kinds of files it can serve. The static server makes
+guesses on the mimetype of the file based on file extensions. Airplane naively
+copies the extension of the file so the cached file has the same ending. This
+means URLs with weird extensions or those which static serve cannot guess at
+mimetype, will cause problems. It is not recommended to use django-airplane
+with files that don't end in typical extensions such as ".css", ".js", ".jpg",
+".png" or ".gif".
+
+
+Supports
+========
+
+django-airplane has been tested with:
+
+* Python 3.8-3.11 and Django 4.1
+* Python 3.8-3.11 and Django 4.2
+
+Older versions tested against Django 2.2 and 3.2, nothing has changed since
+then that should break, but these are no longer test targets
+
+Docs
+====
+
+Docs available at: http://django-airplane.readthedocs.io/en/latest/
+
+Source: https://github.com/cltrudeau/django-airplane
```

#### html2text {}

```diff
@@ -1,18 +1,27 @@
-Metadata-Version: 1.1 Name: django-airplane Version: 1.1.0 Summary: Django app
+Metadata-Version: 2.1 Name: django-airplane Version: 1.1.1 Summary: Django app
 that caches CDN files for use when coding offline Home-page: https://
 github.com/cltrudeau/django-airplane Author: Christopher Trudeau Author-email:
-ctrudeau+pypi@arsensa.com License: MIT Description: django-airplane
-*************** This app is to help in those situations where you can't get on
-the network but you want to write some Django code. Surround your static CDN
-references (like jquery and the like) with this template tag and when you turn
-it on the URLs will be re-written from a local copy. Installation ============
-In your settings file, add 'airplane' to your ``settings.INSTALLED_APPS``
-field: .. code-block:: python INSTALLED_APPS = ( ... 'airplane', ) Also in
-settings, make the following additions: .. code-block:: python import airplane
+ctrudeau+pypi@arsensa.com License: MIT Keywords:
+django,cache,offline,CDN,static Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries ::
+Application Frameworks Classifier: Topic :: Software Development :: Libraries
+:: Python Modules License-File: LICENSE django-airplane *************** This
+app is to help in those situations where you can't get on the network but you
+want to write some Django code. Surround your static CDN references (like
+jquery and the like) with this template tag and when you turn it on the URLs
+will be re-written from a local copy. Installation ============ In your
+settings file, add 'airplane' to your ``settings.INSTALLED_APPS`` field: ..
+code-block:: python INSTALLED_APPS = ( ... 'airplane', ) Also in settings, make
+the following additions: .. code-block:: python import airplane
 STATICFILES_DIRS = ( airplane.cache_path(), ) AIRPLANE_MODE =
 airplane.BUILD_CACHE #AIRPLANE_MODE = airplane.USE_CACHE #AIRPLANE_MODE =
 airplane.AUTO_CACHE Now use the ``airplane`` tag in your templates .. code-
 block:: html {% load airplanetags %}
 Change the ``AIRPLANE_MODE`` setting to ``airplane.USE_CACHE`` and subsequent
 calls to the ``{% airplane %}`` tag will return a reference to the locally
 cached version. Settings ======== Airplane only does something if
@@ -53,18 +62,12 @@
 means you are limited by what kinds of files it can serve. The static server
 makes guesses on the mimetype of the file based on file extensions. Airplane
 naively copies the extension of the file so the cached file has the same
 ending. This means URLs with weird extensions or those which static serve
 cannot guess at mimetype, will cause problems. It is not recommended to use
 django-airplane with files that don't end in typical extensions such as ".css",
 ".js", ".jpg", ".png" or ".gif". Supports ======== django-airplane has been
-tested with: * Python 3.6, 3.7 and Django 2.2 * Python 3.6, 3.7 and Django 3.0
-Docs ==== Docs available at: http://django-airplane.readthedocs.io/en/latest/
-Source: https://github.com/cltrudeau/django-airplane Keywords:
-django,cache,offline,CDN,static Platform: UNKNOWN Classifier: Development
-Status :: 4 - Beta Classifier: Environment :: Web Environment Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Software Development :: Libraries :: Application
-Frameworks Classifier: Topic :: Software Development :: Libraries :: Python
-Modules
+tested with: * Python 3.8-3.11 and Django 4.1 * Python 3.8-3.11 and Django 4.2
+Older versions tested against Django 2.2 and 3.2, nothing has changed since
+then that should break, but these are no longer test targets Docs ==== Docs
+available at: http://django-airplane.readthedocs.io/en/latest/ Source: https://
+github.com/cltrudeau/django-airplane
```

### Comparing `django-airplane-1.1.0/django_airplane.egg-info/SOURCES.txt` & `django-airplane-1.1.1/django_airplane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-airplane-1.1.0/setup.py` & `django-airplane-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,23 +17,25 @@
     include_package_data=True,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     keywords='django,cache,offline,CDN,static',
     test_suite="load_tests.get_suite",
     install_requires=[
-        'Django>=2.2.10',
+        'Django>=4.1',
         'requests>=2.23',
     ],
     tests_require=[
         'context_temp>=0.11.1',
         'django-awl>=0.24.0',
         'waelstow>=0.10.2',
     ]
```

