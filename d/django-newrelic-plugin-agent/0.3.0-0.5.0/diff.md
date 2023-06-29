# Comparing `tmp/django-newrelic-plugin-agent-0.3.0.tar.gz` & `tmp/django-newrelic-plugin-agent-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-newrelic-plugin-agent-0.3.0.tar", last modified: Tue Mar 27 19:15:52 2018, max compression
+gzip compressed data, was "django-newrelic-plugin-agent-0.5.0.tar", last modified: Thu Jun 29 19:43:30 2023, max compression
```

## Comparing `django-newrelic-plugin-agent-0.3.0.tar` & `django-newrelic-plugin-agent-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-03-27 19:15:52.000000 django-newrelic-plugin-agent-0.3.0/
--rw-r--r--   0 root         (0) staff       (20)     2055 2018-03-27 19:15:52.000000 django-newrelic-plugin-agent-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1075 2018-03-27 17:13:33.000000 django-newrelic-plugin-agent-0.3.0/LICENSE
--rw-r--r--   0 root         (0) staff       (20)       34 2018-03-27 17:13:33.000000 django-newrelic-plugin-agent-0.3.0/MANIFEST.in
--rwxr-xr-x   0 root         (0) staff       (20)     1850 2018-03-27 18:57:26.000000 django-newrelic-plugin-agent-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-03-27 19:15:52.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-03-27 19:15:52.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/migrations/
--rw-r--r--   0 root         (0) staff       (20)        0 2018-03-27 17:13:33.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/migrations/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1442 2018-03-27 17:13:33.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/migrations/0001_initial.py
--rw-r--r--   0 root         (0) staff       (20)       22 2018-03-27 18:18:50.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/version.py
--rw-r--r--   0 root         (0) staff       (20)     5780 2018-03-27 19:03:11.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/models.py
--rw-r--r--   0 root         (0) staff       (20)     1544 2018-03-27 17:26:58.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/conf.py
--rw-r--r--   0 root         (0) staff       (20)      132 2018-03-27 17:13:33.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/constants.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-03-27 19:15:52.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/tests/
--rw-r--r--   0 root         (0) staff       (20)     1605 2018-03-27 17:13:33.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/tests/conf_tests.py
--rw-r--r--   0 root         (0) staff       (20)        0 2018-03-27 17:13:33.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/tests/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5214 2018-03-27 17:26:58.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/tests/models_tests.py
--rw-r--r--   0 root         (0) staff       (20)      124 2018-03-27 17:13:33.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      165 2018-03-27 17:13:33.000000 django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/apps.py
--rw-r--r--   0 root         (0) staff       (20)      242 2018-03-27 19:15:52.000000 django-newrelic-plugin-agent-0.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-03-27 19:15:52.000000 django-newrelic-plugin-agent-0.3.0/django_newrelic_plugin_agent.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     2055 2018-03-27 19:15:51.000000 django-newrelic-plugin-agent-0.3.0/django_newrelic_plugin_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)        1 2018-03-27 19:15:51.000000 django-newrelic-plugin-agent-0.3.0/django_newrelic_plugin_agent.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)      773 2018-03-27 19:15:51.000000 django-newrelic-plugin-agent-0.3.0/django_newrelic_plugin_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)       82 2018-03-27 19:15:51.000000 django-newrelic-plugin-agent-0.3.0/django_newrelic_plugin_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       22 2018-03-27 19:15:51.000000 django-newrelic-plugin-agent-0.3.0/django_newrelic_plugin_agent.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2018-03-27 19:15:51.000000 django-newrelic-plugin-agent-0.3.0/django_newrelic_plugin_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)     1054 2018-03-27 17:26:58.000000 django-newrelic-plugin-agent-0.3.0/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 19:43:30.066253 django-newrelic-plugin-agent-0.5.0/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2023-06-29 18:49:44.000000 django-newrelic-plugin-agent-0.5.0/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       68 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1861 2023-06-29 19:43:30.066253 django-newrelic-plugin-agent-0.5.0/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1054 2023-06-29 18:49:44.000000 django-newrelic-plugin-agent-0.5.0/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 19:43:30.066253 django-newrelic-plugin-agent-0.5.0/django_newrelic_plugin_agent.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1861 2023-06-29 19:43:30.000000 django-newrelic-plugin-agent-0.5.0/django_newrelic_plugin_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)      977 2023-06-29 19:43:30.000000 django-newrelic-plugin-agent-0.5.0/django_newrelic_plugin_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 19:43:30.000000 django-newrelic-plugin-agent-0.5.0/django_newrelic_plugin_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 19:43:29.000000 django-newrelic-plugin-agent-0.5.0/django_newrelic_plugin_agent.egg-info/not-zip-safe
+-rw-rw-r--   0 wes       (1000) wes       (1000)       43 2023-06-29 19:43:30.000000 django-newrelic-plugin-agent-0.5.0/django_newrelic_plugin_agent.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-29 19:43:30.000000 django-newrelic-plugin-agent-0.5.0/django_newrelic_plugin_agent.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 19:43:30.066253 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       48 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      165 2023-06-29 18:49:44.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1544 2023-06-29 18:49:44.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/conf.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      132 2023-06-29 18:49:44.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/constants.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 19:43:30.066253 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1398 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/migrations/0001_0002_squashed.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1368 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      394 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/migrations/0002_migrate_jsonfield.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-29 18:49:44.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     5755 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 19:43:30.066253 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-29 18:49:44.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1604 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/tests/conf_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     5223 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/tests/models_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/version.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 19:43:30.066253 django-newrelic-plugin-agent-0.5.0/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       31 2023-06-29 18:49:44.000000 django-newrelic-plugin-agent-0.5.0/requirements/docs.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       60 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       43 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      242 2023-06-29 19:43:30.066253 django-newrelic-plugin-agent-0.5.0/setup.cfg
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1871 2023-06-29 19:42:48.000000 django-newrelic-plugin-agent-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-newrelic-plugin-agent-0.3.0/PKG-INFO` & `django-newrelic-plugin-agent-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-newrelic-plugin-agent
-Version: 0.3.0
+Version: 0.5.0
 Summary: Publish arbitrary metrics to New Relic from within Django application
 Home-page: https://github.com/ambitioninc/django-newrelic-plugin-agent
 Author: Ryan Bales
 Author-email: opensource@ambition.com
 License: MIT
-Description: .. image:: https://travis-ci.org/ambitioninc/django-newrelic-plugin-agent.png
-           :target: https://travis-ci.org/ambitioninc/django-newrelic-plugin-agent
-        
-        .. image:: https://coveralls.io/repos/github/ambitioninc/django-newrelic-plugin-agent/badge.svg?branch=master
-            :target: https://coveralls.io/github/ambitioninc/django-newrelic-plugin-agent?branch=master
-        
-        
-        Django New Relic Plugin Agent
-        =============================
-        
-        
-        Publish arbitrary metrics to New Relic without having to build plugins with the New Relic SDK (Java, .NET)
-        
-        https://docs.newrelic.com/docs/plugins/plugin-developer-resources/developer-reference/plugin-api-specification
-        
-        
-        Installation
-        ------------
-        To install the latest release, type::
-        
-            pip install django-newrelic-plugin-agent
-        
-        To install the latest code directly from source, type::
-        
-            pip install git+git://github.com/ambitioninc/django-newrelic-plugin-agent.git
-        
-        Documentation
-        =============
-        
-        Full documentation is available at http://django-newrelic-plugin-agent.readthedocs.org
-        
-        License
-        =======
-        MIT License (see LICENSE)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django :: 1.8
-Classifier: Framework :: Django :: 1.9
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ambitioninc/django-newrelic-plugin-agent.png
+   :target: https://travis-ci.org/ambitioninc/django-newrelic-plugin-agent
+
+.. image:: https://coveralls.io/repos/github/ambitioninc/django-newrelic-plugin-agent/badge.svg?branch=master
+    :target: https://coveralls.io/github/ambitioninc/django-newrelic-plugin-agent?branch=master
+
+
+Django New Relic Plugin Agent
+=============================
+
+
+Publish arbitrary metrics to New Relic without having to build plugins with the New Relic SDK (Java, .NET)
+
+https://docs.newrelic.com/docs/plugins/plugin-developer-resources/developer-reference/plugin-api-specification
+
+
+Installation
+------------
+To install the latest release, type::
+
+    pip install django-newrelic-plugin-agent
+
+To install the latest code directly from source, type::
+
+    pip install git+git://github.com/ambitioninc/django-newrelic-plugin-agent.git
+
+Documentation
+=============
+
+Full documentation is available at http://django-newrelic-plugin-agent.readthedocs.org
+
+License
+=======
+MIT License (see LICENSE)
```

### Comparing `django-newrelic-plugin-agent-0.3.0/LICENSE` & `django-newrelic-plugin-agent-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-newrelic-plugin-agent-0.3.0/setup.py` & `django-newrelic-plugin-agent-0.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,47 +14,45 @@
     mo = re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', open(VERSION_FILE, 'rt').read(), re.M)
     if mo:
         return mo.group(1)
     else:
         raise RuntimeError('Unable to find version string in {0}.'.format(VERSION_FILE))
 
 
+def get_lines(file_path):
+    return open(file_path, 'r').read().split('\n')
+
+
+install_requires = get_lines('requirements/requirements.txt')
+tests_require = get_lines('requirements/requirements-testing.txt')
+
+
 setup(
     name='django-newrelic-plugin-agent',
     version=get_version(),
     description='Publish arbitrary metrics to New Relic from within Django application',
     long_description=open('README.rst').read(),
     url='https://github.com/ambitioninc/django-newrelic-plugin-agent',
     author='Ryan Bales',
     author_email='opensource@ambition.com',
     keywords='',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Framework :: Django :: 1.8',
-        'Framework :: Django :: 1.9'
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
     license='MIT',
-    install_requires=[
-        'django>=1.8',
-        'django-manager-utils>=0.12.0',
-        'jsonfield>=0.9.23',
-        'django-db-mutex>=0.4.0',
-    ],
-    tests_require=[
-        'freezegun>=0.2.8',
-        'psycopg2',
-        'django-nose',
-        'mock>=1.0.1',
-        'coverage>=3.7.1',
-        'django-dynamic-fixture',
-    ],
+    install_requires=install_requires,
+    tests_require=tests_require,
     test_suite='run_tests.run_tests',
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/migrations/0001_initial.py` & `django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/migrations/0001_0002_squashed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# -*- coding: utf-8 -*-
-# Generated by Django 1.9.2 on 2016-04-15 14:56
-from __future__ import unicode_literals
+# Generated by Django 3.2.19 on 2023-06-02 15:38
 
 from django.db import migrations, models
 import django.db.models.deletion
-import jsonfield.fields
 
 
 class Migration(migrations.Migration):
 
-    initial = True
+    replaces = [('newrelic_plugin_agent', '0001_initial'),
+                ('newrelic_plugin_agent', '0002_migrate_jsonfield')]
 
     dependencies = [
     ]
 
     operations = [
         migrations.CreateModel(
             name='NewRelicComponent',
@@ -25,16 +23,15 @@
             ],
         ),
         migrations.CreateModel(
             name='NewRelicMetricTimeslice',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('guid', models.CharField(max_length=256)),
-                ('values', jsonfield.fields.JSONField()),
-                ('new_relic_component', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='metric_timeslices', to='newrelic_plugin_agent.NewRelicComponent')),
+                ('values', models.JSONField()),
+                ('new_relic_component', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='metric_timeslices', to='newrelic_plugin_agent.newreliccomponent')),
             ],
-        ),
-        migrations.AlterUniqueTogether(
-            name='newrelicmetrictimeslice',
-            unique_together=set([('new_relic_component', 'guid')]),
+            options={
+                'unique_together': {('new_relic_component', 'guid')},
+            },
         ),
     ]
```

### Comparing `django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/models.py` & `django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from manager_utils import ManagerUtilsManager
 from django.db import models
-from jsonfield import JSONField
 
 
 class NewRelicComponent(models.Model):
     # A "reverse domain name" styled identifier;
     # for example, com.newrelic.mysql.
     # This is a unique identity defined in the plugin's user interface,
     # which ties the component data to the corresponding plugin user interface
@@ -135,13 +134,13 @@
     new_relic_component = models.ForeignKey(
         NewRelicComponent, related_name='metric_timeslices', on_delete=models.CASCADE)
     # Unique name of the NR metric
     # examples
     guid = models.CharField(max_length=256)
     # the metric timeslice values
     # https://docs.newrelic.com/docs/plugins/plugin-developer-resources/developer-reference/metric-data-plugin-api#timeslice
-    values = JSONField()
+    values = models.JSONField()
 
     class Meta:
         unique_together = ('new_relic_component', 'guid')
 
     objects = ManagerUtilsManager()
```

### Comparing `django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/conf.py` & `django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/conf.py`

 * *Files identical despite different names*

### Comparing `django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/tests/conf_tests.py` & `django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/tests/conf_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         Verifies that settings are initialized with defaults
         """
         from newrelic_plugin_agent.conf import settings, DEFAULTS
         self.assertEqual(settings.TIMESLICE_LOCK_RETRY_DELAY_MS, DEFAULTS['TIMESLICE_LOCK_RETRY_DELAY_MS'])
         self.assertEqual(settings.NEWRELIC_BASE_URL, DEFAULTS['NEWRELIC_BASE_URL'])
         self.assertEqual(settings.NEWRELIC_LICENSE_KEY, DEFAULTS['NEWRELIC_LICENSE_KEY'])
         with self.assertRaises(AttributeError):
-            assert(settings.FOO)
+            assert settings.FOO
 
     @override_settings(
         NEWRELIC_PLUGIN_AGENT={'TIMESLICE_LOCK_RETRY_DELAY_MS': 500})
     def test_user_settings(self):
         """
         Verifies that user settings are applied correctly
         """
```

### Comparing `django-newrelic-plugin-agent-0.3.0/newrelic_plugin_agent/tests/models_tests.py` & `django-newrelic-plugin-agent-0.5.0/newrelic_plugin_agent/tests/models_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.test import TestCase
 from django_dynamic_fixture import G
-from mock import patch
+from unittest.mock import patch
 from manager_utils import ManagerUtilsManager
 
 from newrelic_plugin_agent.models import NewRelicMetricTimeslice, NewRelicComponent
 
 
 class NewRelicComponentTest(TestCase):
```

### Comparing `django-newrelic-plugin-agent-0.3.0/django_newrelic_plugin_agent.egg-info/PKG-INFO` & `django-newrelic-plugin-agent-0.5.0/django_newrelic_plugin_agent.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-newrelic-plugin-agent
-Version: 0.3.0
+Version: 0.5.0
 Summary: Publish arbitrary metrics to New Relic from within Django application
 Home-page: https://github.com/ambitioninc/django-newrelic-plugin-agent
 Author: Ryan Bales
 Author-email: opensource@ambition.com
 License: MIT
-Description: .. image:: https://travis-ci.org/ambitioninc/django-newrelic-plugin-agent.png
-           :target: https://travis-ci.org/ambitioninc/django-newrelic-plugin-agent
-        
-        .. image:: https://coveralls.io/repos/github/ambitioninc/django-newrelic-plugin-agent/badge.svg?branch=master
-            :target: https://coveralls.io/github/ambitioninc/django-newrelic-plugin-agent?branch=master
-        
-        
-        Django New Relic Plugin Agent
-        =============================
-        
-        
-        Publish arbitrary metrics to New Relic without having to build plugins with the New Relic SDK (Java, .NET)
-        
-        https://docs.newrelic.com/docs/plugins/plugin-developer-resources/developer-reference/plugin-api-specification
-        
-        
-        Installation
-        ------------
-        To install the latest release, type::
-        
-            pip install django-newrelic-plugin-agent
-        
-        To install the latest code directly from source, type::
-        
-            pip install git+git://github.com/ambitioninc/django-newrelic-plugin-agent.git
-        
-        Documentation
-        =============
-        
-        Full documentation is available at http://django-newrelic-plugin-agent.readthedocs.org
-        
-        License
-        =======
-        MIT License (see LICENSE)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django :: 1.8
-Classifier: Framework :: Django :: 1.9
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ambitioninc/django-newrelic-plugin-agent.png
+   :target: https://travis-ci.org/ambitioninc/django-newrelic-plugin-agent
+
+.. image:: https://coveralls.io/repos/github/ambitioninc/django-newrelic-plugin-agent/badge.svg?branch=master
+    :target: https://coveralls.io/github/ambitioninc/django-newrelic-plugin-agent?branch=master
+
+
+Django New Relic Plugin Agent
+=============================
+
+
+Publish arbitrary metrics to New Relic without having to build plugins with the New Relic SDK (Java, .NET)
+
+https://docs.newrelic.com/docs/plugins/plugin-developer-resources/developer-reference/plugin-api-specification
+
+
+Installation
+------------
+To install the latest release, type::
+
+    pip install django-newrelic-plugin-agent
+
+To install the latest code directly from source, type::
+
+    pip install git+git://github.com/ambitioninc/django-newrelic-plugin-agent.git
+
+Documentation
+=============
+
+Full documentation is available at http://django-newrelic-plugin-agent.readthedocs.org
+
+License
+=======
+MIT License (see LICENSE)
```

### Comparing `django-newrelic-plugin-agent-0.3.0/django_newrelic_plugin_agent.egg-info/SOURCES.txt` & `django-newrelic-plugin-agent-0.5.0/django_newrelic_plugin_agent.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,12 +11,17 @@
 django_newrelic_plugin_agent.egg-info/top_level.txt
 newrelic_plugin_agent/__init__.py
 newrelic_plugin_agent/apps.py
 newrelic_plugin_agent/conf.py
 newrelic_plugin_agent/constants.py
 newrelic_plugin_agent/models.py
 newrelic_plugin_agent/version.py
+newrelic_plugin_agent/migrations/0001_0002_squashed.py
 newrelic_plugin_agent/migrations/0001_initial.py
+newrelic_plugin_agent/migrations/0002_migrate_jsonfield.py
 newrelic_plugin_agent/migrations/__init__.py
 newrelic_plugin_agent/tests/__init__.py
 newrelic_plugin_agent/tests/conf_tests.py
-newrelic_plugin_agent/tests/models_tests.py
+newrelic_plugin_agent/tests/models_tests.py
+requirements/docs.txt
+requirements/requirements-testing.txt
+requirements/requirements.txt
```

### Comparing `django-newrelic-plugin-agent-0.3.0/README.rst` & `django-newrelic-plugin-agent-0.5.0/README.rst`

 * *Files identical despite different names*

