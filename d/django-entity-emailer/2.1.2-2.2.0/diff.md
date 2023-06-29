# Comparing `tmp/django-entity-emailer-2.1.2.tar.gz` & `tmp/django-entity-emailer-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-entity-emailer-2.1.2.tar", last modified: Wed Jun  2 17:27:12 2021, max compression
+gzip compressed data, was "django-entity-emailer-2.2.0.tar", last modified: Thu Jun 29 16:58:17 2023, max compression
```

## Comparing `django-entity-emailer-2.1.2.tar` & `django-entity-emailer-2.2.0.tar`

### file list

```diff
@@ -1,46 +1,43 @@
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/
--rw-r--r--   0 jared     (1000) jared     (1000)     1075 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/LICENSE
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/django_entity_emailer.egg-info/
--rw-r--r--   0 jared     (1000) jared     (1000)     1263 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/django_entity_emailer.egg-info/SOURCES.txt
--rw-r--r--   0 jared     (1000) jared     (1000)        1 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/django_entity_emailer.egg-info/dependency_links.txt
--rw-r--r--   0 jared     (1000) jared     (1000)       15 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/django_entity_emailer.egg-info/top_level.txt
--rw-r--r--   0 jared     (1000) jared     (1000)    13318 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/django_entity_emailer.egg-info/PKG-INFO
--rw-r--r--   0 jared     (1000) jared     (1000)      160 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/django_entity_emailer.egg-info/requires.txt
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/requirements/
--rw-rw-r--   0 jared     (1000) jared     (1000)      118 2021-06-02 16:59:34.000000 django-entity-emailer-2.1.2/requirements/requirements-testing.txt
--rw-rw-r--   0 jared     (1000) jared     (1000)      162 2021-06-02 16:59:34.000000 django-entity-emailer-2.1.2/requirements/requirements.txt
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/entity_emailer/
--rw-rw-r--   0 jared     (1000) jared     (1000)      318 2020-02-10 18:11:20.000000 django-entity-emailer-2.1.2/entity_emailer/signals.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/entity_emailer/tests/
--rw-r--r--   0 jared     (1000) jared     (1000)     3014 2019-09-26 18:33:56.000000 django-entity-emailer-2.1.2/entity_emailer/tests/test_views.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2150 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/tests/test_models.py
--rw-rw-r--   0 jared     (1000) jared     (1000)    33041 2021-06-02 17:07:46.000000 django-entity-emailer-2.1.2/entity_emailer/tests/interface_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1357 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/tests/utils_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1537 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/tests/test_management_command.py
--rw-r--r--   0 jared     (1000) jared     (1000)      382 2019-09-26 18:33:56.000000 django-entity-emailer-2.1.2/entity_emailer/tests/utils.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/tests/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     6895 2021-06-02 17:08:54.000000 django-entity-emailer-2.1.2/entity_emailer/interface.py
--rw-r--r--   0 jared     (1000) jared     (1000)      145 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/apps.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     4955 2021-06-02 16:59:34.000000 django-entity-emailer-2.1.2/entity_emailer/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/entity_emailer/management/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/entity_emailer/management/commands/
--rw-r--r--   0 jared     (1000) jared     (1000)      435 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/management/commands/add_email_medium.py
--rw-r--r--   0 jared     (1000) jared     (1000)      897 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/management/commands/entity_emailer_admin_setup.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/management/commands/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/management/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)      177 2019-09-26 18:33:56.000000 django-entity-emailer-2.1.2/entity_emailer/urls.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       22 2021-06-02 17:10:18.000000 django-entity-emailer-2.1.2/entity_emailer/version.py
--rw-r--r--   0 jared     (1000) jared     (1000)     3897 2019-09-26 18:33:56.000000 django-entity-emailer-2.1.2/entity_emailer/utils.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/entity_emailer/migrations/
--rw-rw-r--   0 jared     (1000) jared     (1000)      390 2021-06-02 16:59:34.000000 django-entity-emailer-2.1.2/entity_emailer/migrations/0004_email_num_tries.py
--rw-r--r--   0 jared     (1000) jared     (1000)      481 2019-09-26 18:33:56.000000 django-entity-emailer-2.1.2/entity_emailer/migrations/0002_auto_20170919_1653.py
--rw-r--r--   0 jared     (1000) jared     (1000)      404 2020-02-10 18:37:40.000000 django-entity-emailer-2.1.2/entity_emailer/migrations/0003_email_exception.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/migrations/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1531 2019-09-26 18:33:56.000000 django-entity-emailer-2.1.2/entity_emailer/migrations/0001_initial.py
--rw-r--r--   0 jared     (1000) jared     (1000)      112 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)      795 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/entity_emailer/views.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2104 2021-06-02 16:59:34.000000 django-entity-emailer-2.1.2/setup.py
--rw-r--r--   0 jared     (1000) jared     (1000)      203 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/setup.cfg
--rw-r--r--   0 jared     (1000) jared     (1000)    10205 2019-09-26 18:33:01.000000 django-entity-emailer-2.1.2/README.rst
--rw-r--r--   0 jared     (1000) jared     (1000)       67 2019-09-26 20:53:37.000000 django-entity-emailer-2.1.2/MANIFEST.in
--rw-rw-r--   0 jared     (1000) jared     (1000)    13318 2021-06-02 17:27:12.000000 django-entity-emailer-2.1.2/PKG-INFO
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:58:16.998297 django-entity-emailer-2.2.0/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       67 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)    11004 2023-06-29 16:58:16.998297 django-entity-emailer-2.2.0/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)    10205 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:58:16.994297 django-entity-emailer-2.2.0/django_entity_emailer.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)    11004 2023-06-29 16:58:16.000000 django-entity-emailer-2.2.0/django_entity_emailer.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1116 2023-06-29 16:58:16.000000 django-entity-emailer-2.2.0/django_entity_emailer.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 16:58:16.000000 django-entity-emailer-2.2.0/django_entity_emailer.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      127 2023-06-29 16:58:16.000000 django-entity-emailer-2.2.0/django_entity_emailer.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       15 2023-06-29 16:58:16.000000 django-entity-emailer-2.2.0/django_entity_emailer.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:58:16.998297 django-entity-emailer-2.2.0/entity_emailer/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       48 2023-06-28 21:02:36.000000 django-entity-emailer-2.2.0/entity_emailer/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      145 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6895 2023-01-25 13:27:19.000000 django-entity-emailer-2.2.0/entity_emailer/interface.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:58:16.998297 django-entity-emailer-2.2.0/entity_emailer/management/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/management/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:58:16.998297 django-entity-emailer-2.2.0/entity_emailer/management/commands/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/management/commands/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      435 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/management/commands/add_email_medium.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      897 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/management/commands/entity_emailer_admin_setup.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:58:16.998297 django-entity-emailer-2.2.0/entity_emailer/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1604 2023-06-28 21:02:36.000000 django-entity-emailer-2.2.0/entity_emailer/migrations/0001_0004_squashed.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4955 2023-01-25 13:27:19.000000 django-entity-emailer-2.2.0/entity_emailer/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      332 2023-06-28 21:02:36.000000 django-entity-emailer-2.2.0/entity_emailer/signals.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:58:16.998297 django-entity-emailer-2.2.0/entity_emailer/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    32986 2023-06-28 21:02:36.000000 django-entity-emailer-2.2.0/entity_emailer/tests/interface_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1537 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/tests/test_management_command.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2150 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/tests/test_models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2871 2023-06-28 21:02:36.000000 django-entity-emailer-2.2.0/entity_emailer/tests/test_views.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      382 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/tests/utils.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1357 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/tests/utils_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      180 2023-06-28 21:02:36.000000 django-entity-emailer-2.2.0/entity_emailer/urls.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3897 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/utils.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-28 21:08:22.000000 django-entity-emailer-2.2.0/entity_emailer/version.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      795 2021-04-06 17:21:04.000000 django-entity-emailer-2.2.0/entity_emailer/views.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:58:16.998297 django-entity-emailer-2.2.0/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       72 2023-06-28 21:02:36.000000 django-entity-emailer-2.2.0/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      129 2023-06-29 16:57:37.000000 django-entity-emailer-2.2.0/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      203 2023-06-29 16:58:16.998297 django-entity-emailer-2.2.0/setup.cfg
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2143 2023-06-28 21:09:17.000000 django-entity-emailer-2.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-entity-emailer-2.1.2/LICENSE` & `django-entity-emailer-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-entity-emailer-2.1.2/django_entity_emailer.egg-info/SOURCES.txt` & `django-entity-emailer-2.2.0/django_entity_emailer.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,18 +17,15 @@
 entity_emailer/utils.py
 entity_emailer/version.py
 entity_emailer/views.py
 entity_emailer/management/__init__.py
 entity_emailer/management/commands/__init__.py
 entity_emailer/management/commands/add_email_medium.py
 entity_emailer/management/commands/entity_emailer_admin_setup.py
-entity_emailer/migrations/0001_initial.py
-entity_emailer/migrations/0002_auto_20170919_1653.py
-entity_emailer/migrations/0003_email_exception.py
-entity_emailer/migrations/0004_email_num_tries.py
+entity_emailer/migrations/0001_0004_squashed.py
 entity_emailer/migrations/__init__.py
 entity_emailer/tests/__init__.py
 entity_emailer/tests/interface_tests.py
 entity_emailer/tests/test_management_command.py
 entity_emailer/tests/test_models.py
 entity_emailer/tests/test_views.py
 entity_emailer/tests/utils.py
```

### Comparing `django-entity-emailer-2.1.2/django_entity_emailer.egg-info/PKG-INFO` & `django-entity-emailer-2.2.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,314 +1,293 @@
-Metadata-Version: 1.1
-Name: django-entity-emailer
-Version: 2.1.2
-Summary: Make emailing users easy and entity-based.
-Home-page: https://github.com/ambitioninc/django-entity-emailer
-Author: Erik Swanson
-Author-email: opensource@ambition.com
-License: MIT
-Description: .. image:: https://travis-ci.org/ambitioninc/django-entity-emailer.svg?branch=develop
-            :target: https://travis-ci.org/ambitioninc/django-entity-emailer
-        
-        Django Entity Emailer
-        =====================
-        
-        Do you:
-        
-        - Use `Django-Entity-Event`_?
-        - Want to have emailing as another medium for entity events?
-        - Want a record of emails sent?
-        - Want automatic assurance that you don't accidentally send hundreds
-          of emails over the course of a few minutes?
-        
-        Then use Django Entity Emailer!
-        
-        .. _`Django-Entity-Event`: https://github.com/ambitioninc/django-entity-event
-        
-        Installation
-        ------------
-        
-        This package can currently be installed by downloading and installing
-        from source:
-        
-            git clone
-            python setup.py install
-        
-        Coming soon: ``pip install``.
-        
-        
-        Setup and Configuration
-        -----------------------
-        
-        In order to use django-entity-emailer, you must be mirroring entities
-        using the `django-entity`_
-        framework.
-        Additionally, in order to send email to entities, those
-        entities must include a value for the key ``'email'`` in their
-        ``entity_meta`` field.
-        
-        .. _`django-entity`: https://github.com/ambitioninc/django-entity
-        
-        If both of those conditions are true, setup is fairly straightforward:
-        
-        1. Add ``entity_emailer`` to ``INSTALLED_APPS``.
-        
-        #. Either set a value for ``settings.ENTITY_EMAILER_FROM_EMAIL``, or be
-           sure that the ``settings.DEFAULT_FROM_EMAIL`` is set to an
-           appropriate value.
-        
-        #. Ensure that all the dependencies are installed and listed in ``INSTALLED_APPS``
-        
-           - pip: ``django-db-mutex``, INSTALLED_APPS: ``db_mutex``
-        
-           - pip: ``django-entity-subscription``, INSTALLED_APPS: ``entity_subscription``
-        
-        #. Add the scheduled email task to your ``CELERYBEAT_SCHEDULE`` (see
-           configuring celery section).
-        
-        #. Run ``python manage.py syncdb`` and ``python manage.py migrate``
-        
-        #. Ensure that a email medium is set up by running ``python manage.py
-           add_email_medium``.
-        
-        When sending an email, django-entity-emailer will first check if the
-        ``ENTITY_EMAILER_FROM_EMAIL`` exists. If it does, it will use that value
-        in the email's 'from' field, otherwise it will fall back to the value
-        set in ``DEFAULT_FROM_EMAIL``.
-        
-        Finally, django-entity-emailer is an installable medium that is used with
-        `django-entity-event`_ . This libary makes it easy for developers and
-        users to manage what sorts of notifications users recieve over various
-        mediums. However, it does require some configuration. For a simple emailer configuration,
-        see the 'Basic entity-subscription configuration' section.
-        
-        .. _`django-entity-event`: https://github.com/ambitioninc/django-entity-event
-        
-        
-        Getting ``'email'`` into ``'entity_meta'``
-        ``````````````````````````````````````````
-        
-        The requirement that entities be mirrored with an ``'email'`` field in
-        their ``entity_meta`` is not difficult.
-        
-        After installing django-entity, it is as simple as creating a model
-        inheriting from ``entity.BaseEntityModel``, with a ``get_entity_meta``
-        that returns the email along with any other data to be mirrored. A
-        simple example could be:
-        
-        .. code:: python
-        
-            from django.db import models
-            from entity import BaseEntityModel
-        
-            class Account(BaseEntityModel)
-                username = models.CharField(max_length=64)
-                email = models.CharField(max_length=254)
-        
-                def get_entity_meta(self):
-                    return {'email': self.email, 'username': self.username}
-        
-        
-        Also note that it is not necessary for every mirrored entity to
-        include an email, only those entities that will actually be sent
-        emails need to have emails mirrored in their ``entity_meta``.
-        
-        For a more complete description of how entity mirroring works, see the
-        documentation for django-entity.
-        
-        
-        Basic entity-event configuration
-        ```````````````````````````````````````
-        
-        In order to ensure that users of your site will not recieve emails
-        that they don't want to recieve, the entity-emailer application ties
-        in to the `entity-event` framework. As a developer it is up to
-        you to expose the ability for users to subscribe and unsubscribe from
-        emails. Here, we will show the basic configuration required to start
-        sending emails.
-        
-        .. _`entity-event`: https://github.com/ambitioninc/django-entity-event
-        
-        Running ``manage.py add_email_medium`` will add the medium that
-        entity-emailer relies on to send emails. We must also have a source of
-        emails, and a subscription to that combination of email and source.
-        
-        .. code:: python
-        
-            from entity_emailer import get_medium
-            from entity_event.models import Source, Subscription
-            from entity.models import Entity, EntityKind
-        
-            super_entity = Entity.objects.get_for_obj(my_group_object)
-            user_entity_kind = EntityKind.objects.get(name='myusermodel')
-        
-            email_medium = get_medium()
-            admin_source = Source.objects.create(
-                name='admin', display_name='Admin Notifications',
-                description='Important notifications for the site Admin.',
-            )
-            Subscription.objects.create(
-                source=admin_source, medium=email_medium,
-                entity=super_entity, subentity_kind=user_entity_kind
-            )
-        
-        
-        Along with this, you will need to associate the email medium with a
-        ``RenderingStyle`` object in entity event so that it can perform email
-        rendering. More about this in the next section.
-        
-        Django Entity Emailer must know the email addresses of entities and assumes that an
-        email address has been mirrored by default in the entity metadata. By default, it
-        uses the "email" metadata key, but this can be overridden by setting a
-        ``ENTITY_EMAILER_EMAIL_KEY`` in the settings.
-        
-        Django Entity Emailer also has the ability to exclude certain entities from ever
-        being emailed. In order to do this, mirror metadata that when ``None`` or ``False``
-        means that the entity should never be emailed. Then set the ``ENTITY_EMAILER_EXCLUDE_KEY``
-        setting to the key of this metadata.
-        
-        Sending an Email about an Event
-        -------------------------------
-        
-        Sending an email is as simple as saving an event to the database
-        and subscribing to the email medium after templates are defined for the
-        email. The entity emailer will go through
-        the events, send out emails to the subscribed targets, and mark the
-        events as seen so that duplicate emails are never sent.
-        
-        For example, let's say that we wish to be notified via email when a user
-        logs into a site. Assuming that the email medium and admin sources are setup
-        from our previous examples, we can make an email template (login.html) that looks like the
-        following:
-        
-        .. code:: python
-        
-            {{ user }} just logged in!
-        
-        We then set up a rendering style and a context renderer for this template so that
-        emails can be rendered:
-        
-        .. code:: python
-        
-            from entity_event.models import RenderingStyle, ContextRenderer
-        
-            style = RenderingStyle.objects.create(name='email')
-            ContextRenderer.objects.create(
-                rendering_style=style,
-                source=admin_source,
-                html_template_path='templates/login.html',
-            )
-        
-        When the context renderer is in place, the email medium will need to be updated to point
-        to the appropriate rendering style we want to use. To continue our example:
-        
-        .. code:: python
-        
-            email_medium.rendering_style = style
-            email_medium.save()
-        
-        Once we have the rendering style in place, assume an Event is created with the following context:
-        
-        .. code:: python
-        
-            {
-                'user': 'User name'
-            }
-            
-        When this happens, an email will be sent to the subscribed user that says 'User name just logged in!'.
-        
-        The subject line of this email will use the first 40 characters from the rendered email template. However,
-        if one specifies a <title> HTML tag in their template, the contents of the tag will be used as the
-        email subject.
-        
-        For more detailed information on event rendering, checkout `django-entity-event`_.
-        
-        .. _`django-entity-event`: https://github.com/ambitioninc/django-entity-event
-        
-        
-        Unsubscribing
-        -------------
-        
-        Users may want to be able to unsubscribe from certain types of
-        emails. This is easy in django-entity-emailer. Emails can be
-        unsubscribed from by individual sources, by using the
-        entity-subscription framework.
-        
-        .. code:: python
-        
-            from entity_emailer import get_medium
-            from entity_event import Source, Unsubscribe
-        
-            admin_emails = Source.objects.get(name='admin')
-            Unsubscribe.objects.create(
-                entity=entity_of_user_to_unsub,
-                source=admin_emails
-                medium=get_medium()
-            )
-        
-        This user will be excluded both from receiving emails of this type
-        that were sent to them individually, or as part of a group email.
-        
-        
-        Showing Emails in the Browser
-        -----------------------------
-        
-        Users may view emails in a browser with this application. This is accomplished by including
-        the ``entity_emailer`` urls into the Django project and providing the ``view_uid`` of the email as the url argument.
-        The url view will use the text/html templates of the email to render it as a web page.
-        
-        
-        Release Notes
-        -------------
-        
-        * 0.9.0
-        
-            * Added Django 1.8 support and dropped 1.6 support
-        
-        * 0.8.4
-        
-            * Added the abilty to override the email key in entity metadata.
-            * Added the ability to exlude entities from being emailed based on a metadata key.
-        
-        * 0.8.1
-        
-            * Added Django 1.7 support
-            * Added Python 3.4 support
-        
-        * 0.7.1
-        
-            * Squashed entity emailer migrations and removed entity subscription dependency.
-        
-        * 0.7
-        
-            * Converted entity emailer to solely be a medium for entity event.
-        
-        * 0.6
-        
-            * Added a ``recipients`` field to the ``Email`` model and removed the ``send_to`` field. This allows the user
-                to provide more than one receiver (or group of receivers) for the email.
-        
-        * 0.5
-        
-            * Added a ``context_loader`` field on the ``EmailTemplate`` model. This function allows a user to provide a function
-                path that for fetching and returning data from the stored ``Email`` context.
-            * Added a basic ``EmailView`` and urls for rendering emails through a Django view.
-        
-        * 0.4
-        
-            * Updated to use ``EntityKind`` models rather than ``ContentType`` models for specifying entity groups.
-                A schema migration to remove the old ``subentity_type`` field while adding the new ``subentity_kind``
-                field were added so that users may make appropriate data migrations. Note that it is up to the
-                user to write the appropriate data migration for converting entity types to entity kinds.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+.. image:: https://travis-ci.org/ambitioninc/django-entity-emailer.svg?branch=develop
+    :target: https://travis-ci.org/ambitioninc/django-entity-emailer
+
+Django Entity Emailer
+=====================
+
+Do you:
+
+- Use `Django-Entity-Event`_?
+- Want to have emailing as another medium for entity events?
+- Want a record of emails sent?
+- Want automatic assurance that you don't accidentally send hundreds
+  of emails over the course of a few minutes?
+
+Then use Django Entity Emailer!
+
+.. _`Django-Entity-Event`: https://github.com/ambitioninc/django-entity-event
+
+Installation
+------------
+
+This package can currently be installed by downloading and installing
+from source:
+
+    git clone
+    python setup.py install
+
+Coming soon: ``pip install``.
+
+
+Setup and Configuration
+-----------------------
+
+In order to use django-entity-emailer, you must be mirroring entities
+using the `django-entity`_
+framework.
+Additionally, in order to send email to entities, those
+entities must include a value for the key ``'email'`` in their
+``entity_meta`` field.
+
+.. _`django-entity`: https://github.com/ambitioninc/django-entity
+
+If both of those conditions are true, setup is fairly straightforward:
+
+1. Add ``entity_emailer`` to ``INSTALLED_APPS``.
+
+#. Either set a value for ``settings.ENTITY_EMAILER_FROM_EMAIL``, or be
+   sure that the ``settings.DEFAULT_FROM_EMAIL`` is set to an
+   appropriate value.
+
+#. Ensure that all the dependencies are installed and listed in ``INSTALLED_APPS``
+
+   - pip: ``django-db-mutex``, INSTALLED_APPS: ``db_mutex``
+
+   - pip: ``django-entity-subscription``, INSTALLED_APPS: ``entity_subscription``
+
+#. Add the scheduled email task to your ``CELERYBEAT_SCHEDULE`` (see
+   configuring celery section).
+
+#. Run ``python manage.py syncdb`` and ``python manage.py migrate``
+
+#. Ensure that a email medium is set up by running ``python manage.py
+   add_email_medium``.
+
+When sending an email, django-entity-emailer will first check if the
+``ENTITY_EMAILER_FROM_EMAIL`` exists. If it does, it will use that value
+in the email's 'from' field, otherwise it will fall back to the value
+set in ``DEFAULT_FROM_EMAIL``.
+
+Finally, django-entity-emailer is an installable medium that is used with
+`django-entity-event`_ . This libary makes it easy for developers and
+users to manage what sorts of notifications users recieve over various
+mediums. However, it does require some configuration. For a simple emailer configuration,
+see the 'Basic entity-subscription configuration' section.
+
+.. _`django-entity-event`: https://github.com/ambitioninc/django-entity-event
+
+
+Getting ``'email'`` into ``'entity_meta'``
+``````````````````````````````````````````
+
+The requirement that entities be mirrored with an ``'email'`` field in
+their ``entity_meta`` is not difficult.
+
+After installing django-entity, it is as simple as creating a model
+inheriting from ``entity.BaseEntityModel``, with a ``get_entity_meta``
+that returns the email along with any other data to be mirrored. A
+simple example could be:
+
+.. code:: python
+
+    from django.db import models
+    from entity import BaseEntityModel
+
+    class Account(BaseEntityModel)
+        username = models.CharField(max_length=64)
+        email = models.CharField(max_length=254)
+
+        def get_entity_meta(self):
+            return {'email': self.email, 'username': self.username}
+
+
+Also note that it is not necessary for every mirrored entity to
+include an email, only those entities that will actually be sent
+emails need to have emails mirrored in their ``entity_meta``.
+
+For a more complete description of how entity mirroring works, see the
+documentation for django-entity.
+
+
+Basic entity-event configuration
+```````````````````````````````````````
+
+In order to ensure that users of your site will not recieve emails
+that they don't want to recieve, the entity-emailer application ties
+in to the `entity-event` framework. As a developer it is up to
+you to expose the ability for users to subscribe and unsubscribe from
+emails. Here, we will show the basic configuration required to start
+sending emails.
+
+.. _`entity-event`: https://github.com/ambitioninc/django-entity-event
+
+Running ``manage.py add_email_medium`` will add the medium that
+entity-emailer relies on to send emails. We must also have a source of
+emails, and a subscription to that combination of email and source.
+
+.. code:: python
+
+    from entity_emailer import get_medium
+    from entity_event.models import Source, Subscription
+    from entity.models import Entity, EntityKind
+
+    super_entity = Entity.objects.get_for_obj(my_group_object)
+    user_entity_kind = EntityKind.objects.get(name='myusermodel')
+
+    email_medium = get_medium()
+    admin_source = Source.objects.create(
+        name='admin', display_name='Admin Notifications',
+        description='Important notifications for the site Admin.',
+    )
+    Subscription.objects.create(
+        source=admin_source, medium=email_medium,
+        entity=super_entity, subentity_kind=user_entity_kind
+    )
+
+
+Along with this, you will need to associate the email medium with a
+``RenderingStyle`` object in entity event so that it can perform email
+rendering. More about this in the next section.
+
+Django Entity Emailer must know the email addresses of entities and assumes that an
+email address has been mirrored by default in the entity metadata. By default, it
+uses the "email" metadata key, but this can be overridden by setting a
+``ENTITY_EMAILER_EMAIL_KEY`` in the settings.
+
+Django Entity Emailer also has the ability to exclude certain entities from ever
+being emailed. In order to do this, mirror metadata that when ``None`` or ``False``
+means that the entity should never be emailed. Then set the ``ENTITY_EMAILER_EXCLUDE_KEY``
+setting to the key of this metadata.
+
+Sending an Email about an Event
+-------------------------------
+
+Sending an email is as simple as saving an event to the database
+and subscribing to the email medium after templates are defined for the
+email. The entity emailer will go through
+the events, send out emails to the subscribed targets, and mark the
+events as seen so that duplicate emails are never sent.
+
+For example, let's say that we wish to be notified via email when a user
+logs into a site. Assuming that the email medium and admin sources are setup
+from our previous examples, we can make an email template (login.html) that looks like the
+following:
+
+.. code:: python
+
+    {{ user }} just logged in!
+
+We then set up a rendering style and a context renderer for this template so that
+emails can be rendered:
+
+.. code:: python
+
+    from entity_event.models import RenderingStyle, ContextRenderer
+
+    style = RenderingStyle.objects.create(name='email')
+    ContextRenderer.objects.create(
+        rendering_style=style,
+        source=admin_source,
+        html_template_path='templates/login.html',
+    )
+
+When the context renderer is in place, the email medium will need to be updated to point
+to the appropriate rendering style we want to use. To continue our example:
+
+.. code:: python
+
+    email_medium.rendering_style = style
+    email_medium.save()
+
+Once we have the rendering style in place, assume an Event is created with the following context:
+
+.. code:: python
+
+    {
+        'user': 'User name'
+    }
+    
+When this happens, an email will be sent to the subscribed user that says 'User name just logged in!'.
+
+The subject line of this email will use the first 40 characters from the rendered email template. However,
+if one specifies a <title> HTML tag in their template, the contents of the tag will be used as the
+email subject.
+
+For more detailed information on event rendering, checkout `django-entity-event`_.
+
+.. _`django-entity-event`: https://github.com/ambitioninc/django-entity-event
+
+
+Unsubscribing
+-------------
+
+Users may want to be able to unsubscribe from certain types of
+emails. This is easy in django-entity-emailer. Emails can be
+unsubscribed from by individual sources, by using the
+entity-subscription framework.
+
+.. code:: python
+
+    from entity_emailer import get_medium
+    from entity_event import Source, Unsubscribe
+
+    admin_emails = Source.objects.get(name='admin')
+    Unsubscribe.objects.create(
+        entity=entity_of_user_to_unsub,
+        source=admin_emails
+        medium=get_medium()
+    )
+
+This user will be excluded both from receiving emails of this type
+that were sent to them individually, or as part of a group email.
+
+
+Showing Emails in the Browser
+-----------------------------
+
+Users may view emails in a browser with this application. This is accomplished by including
+the ``entity_emailer`` urls into the Django project and providing the ``view_uid`` of the email as the url argument.
+The url view will use the text/html templates of the email to render it as a web page.
+
+
+Release Notes
+-------------
+
+* 0.9.0
+
+    * Added Django 1.8 support and dropped 1.6 support
+
+* 0.8.4
+
+    * Added the abilty to override the email key in entity metadata.
+    * Added the ability to exlude entities from being emailed based on a metadata key.
+
+* 0.8.1
+
+    * Added Django 1.7 support
+    * Added Python 3.4 support
+
+* 0.7.1
+
+    * Squashed entity emailer migrations and removed entity subscription dependency.
+
+* 0.7
+
+    * Converted entity emailer to solely be a medium for entity event.
+
+* 0.6
+
+    * Added a ``recipients`` field to the ``Email`` model and removed the ``send_to`` field. This allows the user
+        to provide more than one receiver (or group of receivers) for the email.
+
+* 0.5
+
+    * Added a ``context_loader`` field on the ``EmailTemplate`` model. This function allows a user to provide a function
+        path that for fetching and returning data from the stored ``Email`` context.
+    * Added a basic ``EmailView`` and urls for rendering emails through a Django view.
+
+* 0.4
+
+    * Updated to use ``EntityKind`` models rather than ``ContentType`` models for specifying entity groups.
+        A schema migration to remove the old ``subentity_type`` field while adding the new ``subentity_kind``
+        field were added so that users may make appropriate data migrations. Note that it is up to the
+        user to write the appropriate data migration for converting entity types to entity kinds.
```

### Comparing `django-entity-emailer-2.1.2/entity_emailer/tests/test_views.py` & `django-entity-emailer-2.2.0/entity_emailer/tests/test_views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from django.urls import reverse
 from django.test import TestCase
 from django_dynamic_fixture import G
 from entity.models import Entity
 from entity_event.models import Medium, RenderingStyle, ContextRenderer, Source, Event
-import six
 
 from entity_emailer.tests.utils import g_email
 
 
 class EmailViewTest(TestCase):
     def setUp(self):
         self.rendering_style = G(RenderingStyle, name='email')
@@ -26,16 +25,15 @@
         person = G(Entity, display_name='Swansonbot')
         event = G(Event, context={'entity': person.id}, source=self.source)
         email = g_email(event=event)
 
         url = reverse('entity_emailer.email', args=[email.view_uid])
         response = self.client.get(url)
         content = response.content
-        if six.PY3:  # pragma: no cover
-            content = content.decode('utf8')
+        content = content.decode('utf8')
 
         self.assertEqual(content, '<html>Hi Swansonbot</html>')
 
     def test_text_path(self):
         G(
             ContextRenderer, source=self.source, html_template_path='hi_template.txt',
             rendering_style=self.rendering_style, context_hints={
@@ -46,16 +44,15 @@
             })
         person = G(Entity, display_name='Swansonbot')
         event = G(Event, context={'entity': person.id}, source=self.source)
         email = g_email(event=event)
         url = reverse('entity_emailer.email', args=[email.view_uid])
         response = self.client.get(url)
         content = response.content
-        if six.PY3:  # pragma: no cover
-            content = content.decode('utf8')
+        content = content.decode('utf8')
         self.assertEqual(content, 'Hi Swansonbot')
 
     def test_text_and_html_path(self):
         G(
             ContextRenderer, source=self.source,
             html_template_path='hi_template.html', text_template_path='hi_template.txt',
             rendering_style=self.rendering_style, context_hints={
@@ -69,11 +66,10 @@
         event = G(Event, context={'entity': person.id}, source=self.source)
         email = g_email(context={'entity': person.id})
         email = g_email(event=event)
 
         url = reverse('entity_emailer.email', args=[email.view_uid])
         response = self.client.get(url)
         content = response.content
-        if six.PY3:  # pragma: no cover
-            content = content.decode('utf8')
+        content = content.decode('utf8')
 
         self.assertEqual(content, '<html>Hi Swansonbot</html>')
```

### Comparing `django-entity-emailer-2.1.2/entity_emailer/tests/test_models.py` & `django-entity-emailer-2.2.0/entity_emailer/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-entity-emailer-2.1.2/entity_emailer/tests/interface_tests.py` & `django-entity-emailer-2.2.0/entity_emailer/tests/interface_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,48 +10,48 @@
 from django.test.utils import override_settings
 from django_dynamic_fixture import G
 from entity.models import Entity, EntityRelationship, EntityKind
 from entity_event.models import (
     Medium, Source, Subscription, Unsubscription, Event, EventActor
 )
 from freezegun import freeze_time
-from mock import patch
+from unittest.mock import patch
 
 from entity_emailer.interface import EntityEmailerInterface
 from entity_emailer.models import Email
 from entity_emailer.tests.utils import g_email
 from entity_emailer.utils import extract_email_subject_from_html_content, create_email_message, \
     get_subscribed_email_addresses, get_from_email_address
 
 
 class ExtractEmailSubjectFromHtmlContentTest(SimpleTestCase):
     def test_blank(self):
         subject = extract_email_subject_from_html_content('')
-        self.assertEquals(subject, '')
+        self.assertEqual(subject, '')
 
     def test_with_title_block(self):
         subject = extract_email_subject_from_html_content('<html><head><title> Hello! </title></head></html>')
-        self.assertEquals(subject, 'Hello!')
+        self.assertEqual(subject, 'Hello!')
 
     def test_wo_title_block_under_40_chars_content(self):
         subject = extract_email_subject_from_html_content(' Small content ')
-        self.assertEquals(subject, 'Small content')
+        self.assertEqual(subject, 'Small content')
 
     def test_wo_title_block_under_40_chars_multiline_content(self):
         subject = extract_email_subject_from_html_content((
             ' Small content \n'
             'that spans multiple lines'
         ))
-        self.assertEquals(subject, 'Small content')
+        self.assertEqual(subject, 'Small content')
 
     def test_wo_title_block_gt_40_chars_content(self):
         subject = extract_email_subject_from_html_content((
             ' This is reallly long content that is greater than 40 chars on the first line. It should have ...'
         ))
-        self.assertEquals(subject, 'This is reallly long content that is gre...')
+        self.assertEqual(subject, 'This is reallly long content that is gre...')
 
 
 class ConvertEventsToEmailsTest(TestCase):
     def setUp(self):
         call_command('add_email_medium')
         self.email_medium = Medium.objects.get(name='email')
 
@@ -109,18 +109,18 @@
         }
         event = G(Event, source=source, context=email_context)
         G(EventActor, event=event, entity=e)
 
         EntityEmailerInterface.convert_events_to_emails()
 
         email = Email.objects.get()
-        self.assertEquals(list(email.recipients.all()), [e])
-        self.assertEquals(email.event.context, email_context)
-        self.assertEquals(email.subject, '')
-        self.assertEquals(email.scheduled, datetime(2013, 1, 2))
+        self.assertEqual(list(email.recipients.all()), [e])
+        self.assertEqual(email.event.context, email_context)
+        self.assertEqual(email.subject, '')
+        self.assertEqual(email.scheduled, datetime(2013, 1, 2))
 
     @freeze_time('2013-1-2')
     def test_basic_only_following_false_subscription_marked_seen(self):
         source = G(Source)
         e = G(Entity)
         G(Subscription, entity=e, source=source, medium=self.email_medium, only_following=False, sub_entity_kind=None)
         email_context = {
@@ -130,18 +130,18 @@
         event = G(Event, source=source, context=email_context)
         G(EventActor, event=event, entity=e)
 
         EntityEmailerInterface.convert_events_to_emails()
         EntityEmailerInterface.convert_events_to_emails()
 
         email = Email.objects.get()
-        self.assertEquals(list(email.recipients.all()), [e])
-        self.assertEquals(email.event.context, email_context)
-        self.assertEquals(email.subject, '')
-        self.assertEquals(email.scheduled, datetime(2013, 1, 2))
+        self.assertEqual(list(email.recipients.all()), [e])
+        self.assertEqual(email.event.context, email_context)
+        self.assertEqual(email.subject, '')
+        self.assertEqual(email.scheduled, datetime(2013, 1, 2))
 
     @freeze_time('2013-1-2')
     def test_basic_only_following_true_subscription(self):
         source = G(Source)
         e = G(Entity)
         se = G(Entity)
         G(EntityRelationship, sub_entity=e, super_entity=se)
@@ -156,18 +156,18 @@
         event = G(Event, source=source, context=email_context)
         G(EventActor, event=event, entity=se)
 
         EntityEmailerInterface.convert_events_to_emails()
 
         email = Email.objects.get()
         # Since the other_e entity does not follow the se entity, only the e entity receives an email
-        self.assertEquals(set(email.recipients.all()), set([e]))
-        self.assertEquals(email.event.context, email_context)
-        self.assertEquals(email.subject, '')
-        self.assertEquals(email.scheduled, datetime(2013, 1, 2))
+        self.assertEqual(set(email.recipients.all()), set([e]))
+        self.assertEqual(email.event.context, email_context)
+        self.assertEqual(email.subject, '')
+        self.assertEqual(email.scheduled, datetime(2013, 1, 2))
 
     @freeze_time('2013-1-2')
     def test_super_entity_only_following_false_subscription(self):
         source = G(Source)
         e = G(Entity)
         se = G(Entity)
         G(EntityRelationship, sub_entity=e, super_entity=se)
@@ -183,18 +183,18 @@
         G(EventActor, event=event, entity=se)
         G(EventActor, event=event, entity=other_e)
         G(EventActor, event=event, entity=e)
 
         EntityEmailerInterface.convert_events_to_emails()
 
         email = Email.objects.get()
-        self.assertEquals(set(email.recipients.all()), set([e, other_e]))
-        self.assertEquals(email.event.context, email_context)
-        self.assertEquals(email.subject, '')
-        self.assertEquals(email.scheduled, datetime(2013, 1, 2))
+        self.assertEqual(set(email.recipients.all()), set([e, other_e]))
+        self.assertEqual(email.event.context, email_context)
+        self.assertEqual(email.subject, '')
+        self.assertEqual(email.scheduled, datetime(2013, 1, 2))
 
     @freeze_time('2013-1-2')
     def test_basic_only_following_true_group_subscription(self):
         source = G(Source)
         ek = G(EntityKind)
         e = G(Entity, entity_kind=ek)
         se = G(Entity)
@@ -210,18 +210,18 @@
         event = G(Event, source=source, context=email_context)
         G(EventActor, event=event, entity=se)
 
         EntityEmailerInterface.convert_events_to_emails()
 
         email = Email.objects.get()
         # Both entities are subscribed with a group subscription and are following the super entity of the event
-        self.assertEquals(set(email.recipients.all()), set([e, other_e]))
-        self.assertEquals(email.event.context, email_context)
-        self.assertEquals(email.subject, '')
-        self.assertEquals(email.scheduled, datetime(2013, 1, 2))
+        self.assertEqual(set(email.recipients.all()), set([e, other_e]))
+        self.assertEqual(email.event.context, email_context)
+        self.assertEqual(email.subject, '')
+        self.assertEqual(email.scheduled, datetime(2013, 1, 2))
 
     @freeze_time('2013-1-2')
     def test_basic_only_following_false_group_subscription(self):
         source = G(Source)
         ek = G(EntityKind)
         e = G(Entity, entity_kind=ek)
         se = G(Entity)
@@ -237,18 +237,18 @@
         event = G(Event, source=source, context=email_context)
         G(EventActor, event=event, entity=e)
 
         EntityEmailerInterface.convert_events_to_emails()
 
         email = Email.objects.get()
         # Both entities are subscribed with a group subscription and are following the super entity of the event
-        self.assertEquals(set(email.recipients.all()), set([e, other_e]))
-        self.assertEquals(email.event.context, email_context)
-        self.assertEquals(email.subject, '')
-        self.assertEquals(email.scheduled, datetime(2013, 1, 2))
+        self.assertEqual(set(email.recipients.all()), set([e, other_e]))
+        self.assertEqual(email.event.context, email_context)
+        self.assertEqual(email.subject, '')
+        self.assertEqual(email.scheduled, datetime(2013, 1, 2))
 
     @freeze_time('2013-1-2')
     def test_basic_only_following_false_group_subscription_with_unsubscribed(self):
         source = G(Source)
         ek = G(EntityKind)
         e = G(Entity, entity_kind=ek)
         se = G(Entity)
@@ -264,18 +264,18 @@
         }
         event = G(Event, source=source, context=email_context)
         G(EventActor, event=event, entity=e)
 
         EntityEmailerInterface.convert_events_to_emails()
 
         email = Email.objects.get()
-        self.assertEquals(set(email.recipients.all()), set([other_e]))
-        self.assertEquals(email.event.context, email_context)
-        self.assertEquals(email.subject, '')
-        self.assertEquals(email.scheduled, datetime(2013, 1, 2))
+        self.assertEqual(set(email.recipients.all()), set([other_e]))
+        self.assertEqual(email.event.context, email_context)
+        self.assertEqual(email.subject, '')
+        self.assertEqual(email.scheduled, datetime(2013, 1, 2))
 
     @freeze_time('2013-1-2')
     def test_multiple_events_only_following_false(self):
         source = G(Source)
         e = G(Entity)
         other_e = G(Entity)
 
@@ -286,20 +286,20 @@
             'entity_emailer_subject': 'hi',
         }
         G(Event, source=source, context=email_context)
         G(Event, source=source, context=email_context)
 
         EntityEmailerInterface.convert_events_to_emails()
 
-        self.assertEquals(Email.objects.count(), 2)
+        self.assertEqual(Email.objects.count(), 2)
         for email in Email.objects.all():
-            self.assertEquals(set(email.recipients.all()), set([e, other_e]))
-            self.assertEquals(email.event.context, email_context)
-            self.assertEquals(email.subject, '')
-            self.assertEquals(email.scheduled, datetime(2013, 1, 2))
+            self.assertEqual(set(email.recipients.all()), set([e, other_e]))
+            self.assertEqual(email.event.context, email_context)
+            self.assertEqual(email.subject, '')
+            self.assertEqual(email.scheduled, datetime(2013, 1, 2))
 
     @freeze_time('2013-1-2')
     def test_bulk_multiple_events_only_following_false(self):
         """
         Handles bulk creating events and tests the unique constraint of the duplicated subscription which would cause
         a bulk create error if it wasn't handled
         """
@@ -315,20 +315,20 @@
             'entity_emailer_subject': 'hi',
         }
         G(Event, source=source, context=email_context)
         G(Event, source=source, context=email_context)
 
         EntityEmailerInterface.bulk_convert_events_to_emails()
 
-        self.assertEquals(Email.objects.count(), 2)
+        self.assertEqual(Email.objects.count(), 2)
         for email in Email.objects.all():
-            self.assertEquals(set(email.recipients.all()), set([e, other_e]))
-            self.assertEquals(email.event.context, email_context)
-            self.assertEquals(email.subject, '')
-            self.assertEquals(email.scheduled, datetime(2013, 1, 2))
+            self.assertEqual(set(email.recipients.all()), set([e, other_e]))
+            self.assertEqual(email.event.context, email_context)
+            self.assertEqual(email.subject, '')
+            self.assertEqual(email.scheduled, datetime(2013, 1, 2))
 
     @freeze_time('2013-1-2')
     def test_bulk_multiple_events_only_following_true(self):
         """
         Handles bulk creating events and tests the unique constraint of the duplicated subscription which would cause
         a bulk create error if it wasn't handled
         """
@@ -346,18 +346,18 @@
         G(Event, source=source, context=email_context)
         event = G(Event, source=source, context=email_context)
         G(EventActor, event=event, entity=e)
 
         EntityEmailerInterface.bulk_convert_events_to_emails()
 
         email = Email.objects.get()
-        self.assertEquals(set(email.recipients.all()), set([e]))
-        self.assertEquals(email.event.context, email_context)
-        self.assertEquals(email.subject, '')
-        self.assertEquals(email.scheduled, datetime(2013, 1, 2))
+        self.assertEqual(set(email.recipients.all()), set([e]))
+        self.assertEqual(email.event.context, email_context)
+        self.assertEqual(email.subject, '')
+        self.assertEqual(email.scheduled, datetime(2013, 1, 2))
 
     @freeze_time('2013-1-2')
     def test_multiple_events_only_following_true(self):
         source = G(Source)
         e = G(Entity)
         other_e = G(Entity)
 
@@ -370,18 +370,18 @@
         G(Event, source=source, context=email_context)
         event = G(Event, source=source, context=email_context)
         G(EventActor, event=event, entity=e)
 
         EntityEmailerInterface.convert_events_to_emails()
 
         email = Email.objects.get()
-        self.assertEquals(set(email.recipients.all()), set([e]))
-        self.assertEquals(email.event.context, email_context)
-        self.assertEquals(email.subject, '')
-        self.assertEquals(email.scheduled, datetime(2013, 1, 2))
+        self.assertEqual(set(email.recipients.all()), set([e]))
+        self.assertEqual(email.event.context, email_context)
+        self.assertEqual(email.subject, '')
+        self.assertEqual(email.scheduled, datetime(2013, 1, 2))
 
 
 @freeze_time('2014-01-05')
 class SendUnsentScheduledEmailsTest(TestCase):
     def setUp(self):
         G(Medium, name='email')
 
@@ -527,15 +527,15 @@
         with patch(settings.EMAIL_BACKEND) as mock_connection:
             EntityEmailerInterface.send_unsent_scheduled_emails()
 
             # Assert that only one email was marked as sent
             self.assertEqual(Email.objects.filter(sent__isnull=False).count(), 1)
 
             # Assert that only one email is actually sent through backend
-            self.assertEquals(1, mock_connection.call_count)
+            self.assertEqual(1, mock_connection.call_count)
             # Assert that one email raised an exception and that the tries count was updated
             exception_email = Email.objects.get(exception__isnull=False, num_tries=1)
             self.assertIsNotNone(exception_email)
             self.assertTrue('Exception: test' in exception_email.exception)
 
     def test_send_unsent_emails_is_durable(self):
         """
@@ -554,15 +554,15 @@
         # Create test emails to send
         g_email(context={}, scheduled=datetime.min)
         failed_email = g_email(context={}, scheduled=datetime.min)
         mock_get_subscribed_addresses.return_value = ['test1@example.com']
         mock_render.return_value = ('foo', 'bar',)
 
         # Verify baseline, namely that both emails are not marked as sent and that neither has an exception saved
-        self.assertEquals(2, Email.objects.filter(sent__isnull=True).count())
+        self.assertEqual(2, Email.objects.filter(sent__isnull=True).count())
 
         class TestEmailSendMessageException(Exception):
             @property
             def to_dict(self):
                 return {'message': str(self)}
 
         with patch(settings.EMAIL_BACKEND) as mock_connection:
@@ -571,50 +571,50 @@
                 None,
                 TestEmailSendMessageException('test'),
             ]
 
             EntityEmailerInterface.send_unsent_scheduled_emails()
 
         # Verify that only one email is marked as sent
-        self.assertEquals(1, Email.objects.filter(sent__isnull=False).count())
+        self.assertEqual(1, Email.objects.filter(sent__isnull=False).count())
         # Verify that the failed email was saved with the exception
         actual_failed_email = Email.objects.get(exception__isnull=False, num_tries=1)
-        self.assertEquals(failed_email.id, actual_failed_email.id)
-        self.assertEquals(
+        self.assertEqual(failed_email.id, actual_failed_email.id)
+        self.assertEqual(
             'test: {}'.format(json.dumps({'message': 'test'})),
             actual_failed_email.exception
         )
 
         # Verify that a subsequent attempt to send unscheduled emails will retry the failed email
         with patch(settings.EMAIL_BACKEND) as mock_connection:
             # Mock side effect for sending email
             mock_connection.return_value.__enter__.return_value.send_messages.side_effect = (
                 TestEmailSendMessageException('test')
             )
 
             EntityEmailerInterface.send_unsent_scheduled_emails()
 
             # Verify only called once, with the failed email
-            self.assertEquals(1, mock_connection.return_value.__enter__.return_value.send_messages.call_count)
+            self.assertEqual(1, mock_connection.return_value.__enter__.return_value.send_messages.call_count)
 
         # Verify num tries updated
         actual_failed_email = Email.objects.get(exception__isnull=False, num_tries=2)
-        self.assertEquals(failed_email.id, actual_failed_email.id)
+        self.assertEqual(failed_email.id, actual_failed_email.id)
 
         # Verify that a subsequent attempt to send unscheduled emails will find no emails to send
         with patch(settings.EMAIL_BACKEND) as mock_connection:
 
             EntityEmailerInterface.send_unsent_scheduled_emails()
 
             # Verify only called once, with the failed email
-            self.assertEquals(0, mock_connection.return_value.__enter__.return_value.send_messages.call_count)
+            self.assertEqual(0, mock_connection.return_value.__enter__.return_value.send_messages.call_count)
 
         # Verify num tries not updated
         actual_failed_email = Email.objects.get(exception__isnull=False, num_tries=2)
-        self.assertEquals(failed_email.id, actual_failed_email.id)
+        self.assertEqual(failed_email.id, actual_failed_email.id)
 
     @override_settings(DISABLE_DURABILITY_CHECKING=True, ENTITY_EMAILER_MAX_SEND_MESSAGE_TRIES=2)
     @patch.object(Event, 'render', spec_set=True)
     @patch('entity_emailer.interface.get_subscribed_email_addresses')
     def test_send_exception_with_to_dict_method(self, mock_get_subscribed_addresses, mock_render):
         """
         Verifies that when a single email raises an exception from within the backend, the batch is still
@@ -623,15 +623,15 @@
         # Create test emails to send
         g_email(context={}, scheduled=datetime.min)
         failed_email = g_email(context={}, scheduled=datetime.min)
         mock_get_subscribed_addresses.return_value = ['test1@example.com']
         mock_render.return_value = ('foo', 'bar',)
 
         # Verify baseline, namely that both emails are not marked as sent and that neither has an exception saved
-        self.assertEquals(2, Email.objects.filter(sent__isnull=True).count())
+        self.assertEqual(2, Email.objects.filter(sent__isnull=True).count())
 
         class TestEmailSendMessageException(Exception):
             def to_dict(self):
                 return {'message': str(self)}
 
         with patch(settings.EMAIL_BACKEND) as mock_connection:
             # Mock side effects for sending emails
@@ -639,19 +639,19 @@
                 None,
                 TestEmailSendMessageException('test'),
             ]
 
             EntityEmailerInterface.send_unsent_scheduled_emails()
 
         # Verify that only one email is marked as sent
-        self.assertEquals(1, Email.objects.filter(sent__isnull=False).count())
+        self.assertEqual(1, Email.objects.filter(sent__isnull=False).count())
         # Verify that the failed email was saved with the exception
         actual_failed_email = Email.objects.get(exception__isnull=False, num_tries=1)
-        self.assertEquals(failed_email.id, actual_failed_email.id)
-        self.assertEquals(
+        self.assertEqual(failed_email.id, actual_failed_email.id)
+        self.assertEqual(
             'test: {}'.format(json.dumps({'message': 'test'})),
             actual_failed_email.exception
         )
 
 
 class CreateEmailObjectTest(TestCase):
     def test_no_html(self):
```

### Comparing `django-entity-emailer-2.1.2/entity_emailer/tests/utils_tests.py` & `django-entity-emailer-2.2.0/entity_emailer/tests/utils_tests.py`

 * *Files identical despite different names*

### Comparing `django-entity-emailer-2.1.2/entity_emailer/tests/test_management_command.py` & `django-entity-emailer-2.2.0/entity_emailer/tests/test_management_command.py`

 * *Files identical despite different names*

### Comparing `django-entity-emailer-2.1.2/entity_emailer/interface.py` & `django-entity-emailer-2.2.0/entity_emailer/interface.py`

 * *Files identical despite different names*

### Comparing `django-entity-emailer-2.1.2/entity_emailer/models.py` & `django-entity-emailer-2.2.0/entity_emailer/models.py`

 * *Files identical despite different names*

### Comparing `django-entity-emailer-2.1.2/entity_emailer/management/commands/entity_emailer_admin_setup.py` & `django-entity-emailer-2.2.0/entity_emailer/management/commands/entity_emailer_admin_setup.py`

 * *Files identical despite different names*

### Comparing `django-entity-emailer-2.1.2/entity_emailer/utils.py` & `django-entity-emailer-2.2.0/entity_emailer/utils.py`

 * *Files identical despite different names*

### Comparing `django-entity-emailer-2.1.2/entity_emailer/migrations/0001_initial.py` & `django-entity-emailer-2.2.0/entity_emailer/migrations/0001_0004_squashed.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals
+# Generated by Django 3.2.19 on 2023-06-01 13:10
 
-from django.db import models, migrations
-import django.db.models.deletion
 import datetime
+from django.db import migrations, models
+import django.db.models.deletion
 import uuid
 
 
-if hasattr(models, 'UUIDField'):
-    uuid_field = ('view_uid', models.UUIDField(default=uuid.uuid4, editable=False))
-else:
-    import uuidfield.fields
-    uuid_field = ('view_uid', uuidfield.fields.UUIDField(editable=False, unique=True, max_length=32, blank=True)),
-
-
 class Migration(migrations.Migration):
+    replaces = [('entity_emailer', '0001_initial'),
+                ('entity_emailer', '0002_auto_20170919_1653'),
+                ('entity_emailer', '0003_email_exception'),
+                ('entity_emailer', '0004_email_num_tries')]
 
     dependencies = [
         ('entity_event', '0001_initial'),
         ('entity', '0001_initial'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='Email',
             fields=[
-                ('id', models.AutoField(primary_key=True, verbose_name='ID', auto_created=True, serialize=False)),
-                uuid_field,
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('view_uid', models.UUIDField(default=uuid.uuid4, editable=False)),
                 ('subject', models.CharField(max_length=256)),
                 ('from_address', models.CharField(default='', max_length=256)),
-                ('uid', models.CharField(null=True, default=None, unique=True, max_length=100)),
-                ('scheduled', models.DateTimeField(null=True, default=datetime.datetime.utcnow)),
-                ('sent', models.DateTimeField(null=True, default=None)),
-                ('event', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.Event')),
+                ('uid', models.CharField(default=None, max_length=100, null=True, unique=True)),
+                ('scheduled', models.DateTimeField(default=datetime.datetime.utcnow, null=True)),
+                ('sent', models.DateTimeField(default=None, null=True)),
+                ('event', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.event')),
                 ('recipients', models.ManyToManyField(to='entity.Entity')),
+                ('exception', models.TextField(default=None, null=True)),
+                ('num_tries', models.IntegerField(default=0)),
             ],
-            options={
-            },
-            bases=(models.Model,),
         ),
     ]
```

### Comparing `django-entity-emailer-2.1.2/entity_emailer/views.py` & `django-entity-emailer-2.2.0/entity_emailer/views.py`

 * *Files identical despite different names*

### Comparing `django-entity-emailer-2.1.2/setup.py` & `django-entity-emailer-2.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,36 +30,38 @@
     requirements = [r.strip() for r in requirements if r.strip()]
 
     return [
         r for r in requirements
         if not r.startswith('#') and not r.startswith('-')
     ]
 
+
 setup(
     name='django-entity-emailer',
     version=get_version(),
     description='Make emailing users easy and entity-based.',
     long_description=open('README.rst').read(),
     url='https://github.com/ambitioninc/django-entity-emailer',
     author='Erik Swanson',
     author_email='opensource@ambition.com',
     keywords='',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
     license='MIT',
     install_requires=get_requirements('requirements.txt'),
     tests_require=get_requirements('requirements-testing.txt'),
     test_suite='run_tests.run',
     include_package_data=True,
 )
```

### Comparing `django-entity-emailer-2.1.2/README.rst` & `django-entity-emailer-2.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: django-entity-emailer
+Version: 2.2.0
+Summary: Make emailing users easy and entity-based.
+Home-page: https://github.com/ambitioninc/django-entity-emailer
+Author: Erik Swanson
+Author-email: opensource@ambition.com
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
+
 .. image:: https://travis-ci.org/ambitioninc/django-entity-emailer.svg?branch=develop
     :target: https://travis-ci.org/ambitioninc/django-entity-emailer
 
 Django Entity Emailer
 =====================
 
 Do you:
```

