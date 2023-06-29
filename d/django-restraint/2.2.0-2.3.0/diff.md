# Comparing `tmp/django-restraint-2.2.0.tar.gz` & `tmp/django-restraint-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-restraint-2.2.0.tar", last modified: Thu Mar  2 14:43:02 2023, max compression
+gzip compressed data, was "django-restraint-2.3.0.tar", last modified: Thu Jun 29 18:43:46 2023, max compression
```

## Comparing `django-restraint-2.2.0.tar` & `django-restraint-2.3.0.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-02 14:43:02.000000 django-restraint-2.2.0/
--rw-rw-r--   0 jared     (1000) jared     (1000)     1075 2022-02-18 14:25:59.000000 django-restraint-2.2.0/LICENSE
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-02 14:43:02.000000 django-restraint-2.2.0/restraint/
--rw-rw-r--   0 jared     (1000) jared     (1000)      116 2023-02-28 21:28:23.000000 django-restraint-2.2.0/restraint/signals.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     7445 2023-03-01 01:43:12.000000 django-restraint-2.2.0/restraint/managers.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-02 14:43:02.000000 django-restraint-2.2.0/restraint/tests/
--rw-rw-r--   0 jared     (1000) jared     (1000)    19718 2023-03-01 01:17:28.000000 django-restraint-2.2.0/restraint/tests/core_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      779 2022-02-18 14:25:59.000000 django-restraint-2.2.0/restraint/tests/commands_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2539 2023-03-01 01:11:45.000000 django-restraint-2.2.0/restraint/tests/configuration.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2840 2022-02-21 15:25:35.000000 django-restraint-2.2.0/restraint/tests/models_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2022-02-18 14:25:59.000000 django-restraint-2.2.0/restraint/tests/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     5453 2023-02-28 21:43:11.000000 django-restraint-2.2.0/restraint/core.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      131 2022-02-18 14:25:59.000000 django-restraint-2.2.0/restraint/apps.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      199 2022-02-18 14:25:59.000000 django-restraint-2.2.0/restraint/constants.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     4787 2023-03-01 01:07:02.000000 django-restraint-2.2.0/restraint/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-02 14:43:02.000000 django-restraint-2.2.0/restraint/management/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-02 14:43:02.000000 django-restraint-2.2.0/restraint/management/commands/
--rw-rw-r--   0 jared     (1000) jared     (1000)      721 2022-02-18 14:27:54.000000 django-restraint-2.2.0/restraint/management/commands/update_restraint_db.py
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2022-02-18 14:25:59.000000 django-restraint-2.2.0/restraint/management/commands/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2022-02-18 14:25:59.000000 django-restraint-2.2.0/restraint/management/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       37 2022-02-21 15:35:38.000000 django-restraint-2.2.0/restraint/urls.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       22 2023-03-02 14:37:12.000000 django-restraint-2.2.0/restraint/version.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-02 14:43:02.000000 django-restraint-2.2.0/restraint/migrations/
--rw-r--r--   0 jared     (1000) jared     (1000)      862 2023-03-01 01:09:12.000000 django-restraint-2.2.0/restraint/migrations/0003_auto_20230301_0109.py
--rw-r--r--   0 jared     (1000) jared     (1000)      687 2022-02-21 15:43:13.000000 django-restraint-2.2.0/restraint/migrations/0002_permset_is_private.py
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2022-02-18 14:25:59.000000 django-restraint-2.2.0/restraint/migrations/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     3132 2022-02-18 14:27:54.000000 django-restraint-2.2.0/restraint/migrations/0001_initial.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      104 2022-02-18 14:25:59.000000 django-restraint-2.2.0/restraint/__init__.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-02 14:43:02.000000 django-restraint-2.2.0/django_restraint.egg-info/
--rw-rw-r--   0 jared     (1000) jared     (1000)      921 2023-03-02 14:43:01.000000 django-restraint-2.2.0/django_restraint.egg-info/SOURCES.txt
--rw-rw-r--   0 jared     (1000) jared     (1000)        1 2023-03-02 14:43:01.000000 django-restraint-2.2.0/django_restraint.egg-info/dependency_links.txt
--rw-rw-r--   0 jared     (1000) jared     (1000)        1 2022-02-28 23:59:44.000000 django-restraint-2.2.0/django_restraint.egg-info/not-zip-safe
--rw-rw-r--   0 jared     (1000) jared     (1000)       10 2023-03-02 14:43:01.000000 django-restraint-2.2.0/django_restraint.egg-info/top_level.txt
--rw-rw-r--   0 jared     (1000) jared     (1000)      828 2023-03-02 14:43:01.000000 django-restraint-2.2.0/django_restraint.egg-info/PKG-INFO
--rw-rw-r--   0 jared     (1000) jared     (1000)       40 2023-03-02 14:43:01.000000 django-restraint-2.2.0/django_restraint.egg-info/requires.txt
--rwxrwxr-x   0 jared     (1000) jared     (1000)     1742 2022-10-24 20:55:11.000000 django-restraint-2.2.0/setup.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      270 2023-03-02 14:43:02.000000 django-restraint-2.2.0/setup.cfg
--rw-rw-r--   0 jared     (1000) jared     (1000)       75 2022-02-21 16:22:17.000000 django-restraint-2.2.0/README.rst
--rw-rw-r--   0 jared     (1000) jared     (1000)       34 2022-02-18 14:25:59.000000 django-restraint-2.2.0/MANIFEST.in
--rw-rw-r--   0 jared     (1000) jared     (1000)      828 2023-03-02 14:43:02.000000 django-restraint-2.2.0/PKG-INFO
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:43:46.822097 django-restraint-2.3.0/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2023-01-09 15:26:12.000000 django-restraint-2.3.0/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       68 2023-06-29 18:42:57.000000 django-restraint-2.3.0/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)      900 2023-06-29 18:43:46.822097 django-restraint-2.3.0/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)       75 2023-06-29 18:34:34.000000 django-restraint-2.3.0/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:43:46.818096 django-restraint-2.3.0/django_restraint.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      900 2023-06-29 18:43:46.000000 django-restraint-2.3.0/django_restraint.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1011 2023-06-29 18:43:46.000000 django-restraint-2.3.0/django_restraint.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 18:43:46.000000 django-restraint-2.3.0/django_restraint.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 18:43:46.000000 django-restraint-2.3.0/django_restraint.egg-info/not-zip-safe
+-rw-rw-r--   0 wes       (1000) wes       (1000)       40 2023-06-29 18:43:46.000000 django-restraint-2.3.0/django_restraint.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       10 2023-06-29 18:43:46.000000 django-restraint-2.3.0/django_restraint.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:43:46.818096 django-restraint-2.3.0/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       31 2023-01-09 15:26:12.000000 django-restraint-2.3.0/requirements/docs.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       70 2023-06-29 18:42:57.000000 django-restraint-2.3.0/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       40 2023-06-29 18:42:57.000000 django-restraint-2.3.0/requirements/requirements.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:43:46.822097 django-restraint-2.3.0/restraint/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       50 2023-06-29 18:42:57.000000 django-restraint-2.3.0/restraint/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      131 2023-01-09 15:26:12.000000 django-restraint-2.3.0/restraint/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      199 2023-01-09 15:26:12.000000 django-restraint-2.3.0/restraint/constants.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     5453 2023-06-29 18:31:05.000000 django-restraint-2.3.0/restraint/core.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:43:46.822097 django-restraint-2.3.0/restraint/management/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:26:12.000000 django-restraint-2.3.0/restraint/management/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:43:46.822097 django-restraint-2.3.0/restraint/management/commands/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:26:12.000000 django-restraint-2.3.0/restraint/management/commands/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      721 2023-01-09 15:26:12.000000 django-restraint-2.3.0/restraint/management/commands/update_restraint_db.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7445 2023-06-29 18:31:05.000000 django-restraint-2.3.0/restraint/managers.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:43:46.822097 django-restraint-2.3.0/restraint/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3092 2023-06-29 18:42:57.000000 django-restraint-2.3.0/restraint/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      687 2023-06-29 18:31:05.000000 django-restraint-2.3.0/restraint/migrations/0002_permset_is_private.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      862 2023-06-29 18:31:05.000000 django-restraint-2.3.0/restraint/migrations/0003_auto_20230301_0109.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:26:12.000000 django-restraint-2.3.0/restraint/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4655 2023-06-29 18:42:57.000000 django-restraint-2.3.0/restraint/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      116 2023-06-29 18:31:05.000000 django-restraint-2.3.0/restraint/signals.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:43:46.822097 django-restraint-2.3.0/restraint/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:26:12.000000 django-restraint-2.3.0/restraint/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      788 2023-06-29 18:42:57.000000 django-restraint-2.3.0/restraint/tests/commands_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2539 2023-06-29 18:31:05.000000 django-restraint-2.3.0/restraint/tests/configuration.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    19708 2023-06-29 18:42:57.000000 django-restraint-2.3.0/restraint/tests/core_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2836 2023-06-29 18:42:57.000000 django-restraint-2.3.0/restraint/tests/models_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       37 2023-06-29 18:31:05.000000 django-restraint-2.3.0/restraint/urls.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-29 18:42:57.000000 django-restraint-2.3.0/restraint/version.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      270 2023-06-29 18:43:46.822097 django-restraint-2.3.0/setup.cfg
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1859 2023-06-29 18:42:57.000000 django-restraint-2.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-restraint-2.2.0/LICENSE` & `django-restraint-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-restraint-2.2.0/restraint/managers.py` & `django-restraint-2.3.0/restraint/managers.py`

 * *Files identical despite different names*

### Comparing `django-restraint-2.2.0/restraint/tests/core_tests.py` & `django-restraint-2.3.0/restraint/tests/core_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.contrib.auth.models import User
 from django.contrib.contenttypes.models import ContentType
 from django.test import SimpleTestCase, TestCase
 from django_dynamic_fixture import G
-from mock import patch, Mock
-from mock.mock import PropertyMock
+from unittest.mock import patch, Mock
+from unittest.mock import PropertyMock
 
 from restraint import core, constants
 from restraint.models import PermSet, Perm, PermLevel, PermAccess
 import restraint.tests.configuration as test_configuration
 
 
 class TestGetRestraintConfig(SimpleTestCase):
@@ -39,15 +39,15 @@
         )
 
     def test_super_user(self):
         # Make a user that is a superuser and verify they get all proper permissions
         user = G(User, is_superuser=True)
         restraints = core.Restraint(user)
         perms = restraints.perms
-        self.assertEquals(
+        self.assertEqual(
             perms,
             {
                 'can_edit_stuff': {
                     'all_stuff': None,
                     'some_stuff': test_configuration.user_some_stuff_id_filter,
                 },
                 'can_view_stuff': {
@@ -64,29 +64,29 @@
         # Also, add an individual permission to the user and verify they get that too
         user = G(User, is_superuser=False, is_staff=False)
         pa = G(PermAccess, perm_user_id=user.id, perm_user_type=ContentType.objects.get_for_model(user))
         pa.perm_levels.add(PermLevel.objects.get(name='all_stuff'))
 
         r = core.Restraint(user)
         perms = r.perms
-        self.assertEquals(
+        self.assertEqual(
             perms,
             {
                 'can_edit_stuff': {
                     'some_stuff': test_configuration.user_some_stuff_id_filter,
                     'all_stuff': None
                 }
             }
         )
 
     def test_load_some_perms(self):
         user = G(User, is_superuser=True)
         restraints = core.Restraint(user, ['can_edit_stuff'])
         perms = restraints.perms
-        self.assertEquals(
+        self.assertEqual(
             perms,
             {
                 'can_edit_stuff': {
                     'all_stuff': None,
                     'some_stuff': test_configuration.user_some_stuff_id_filter
                 }
             }
@@ -160,76 +160,76 @@
         # super user perms
         u = G(User, is_superuser=True)
         # Make another user that they will be able to edit
         u2 = G(User)
         r = core.Restraint(u)
 
         filtered_qset = r.filter_qset(User.objects.all(), 'can_edit_stuff')
-        self.assertEquals(set(filtered_qset), set([u, u2]))
+        self.assertEqual(set(filtered_qset), set([u, u2]))
 
     def test_filter_qset_local_access(self):
         # Make a user that is not a superuser
         u = G(User, is_superuser=False)
         # Make another user that they will not be able to edit
         G(User)
         r = core.Restraint(u)
 
         filtered_qset = r.filter_qset(User.objects.all(), 'can_edit_stuff')
-        self.assertEquals(set(filtered_qset), set([u]))
+        self.assertEqual(set(filtered_qset), set([u]))
 
     def test_filter_qset_multiple_local_access(self):
         # Make a user that is staff
         u = G(User, is_superuser=False, is_staff=True)
         # Make another user that they will not be able to edit
         G(User)
         # Make another super user that they will be able to edit
         u2 = G(User, is_superuser=True)
         r = core.Restraint(u)
 
         filtered_qset = r.filter_qset(User.objects.all(), 'can_edit_stuff')
-        self.assertEquals(set(filtered_qset), set([u, u2]))
+        self.assertEqual(set(filtered_qset), set([u, u2]))
 
     def test_filter_qset_no_perms(self):
         # Make a user that is staff
         u = G(User, is_superuser=False, is_staff=True)
         # Load permissions that will not give them access to edit any accounts
         r = core.Restraint(u, ['bad_perm'])
 
         filtered_qset = r.filter_qset(User.objects.all(), 'can_edit_stuff')
-        self.assertEquals(set(filtered_qset), set([]))
+        self.assertEqual(set(filtered_qset), set([]))
 
     def test_filter_qset_restrict_subset(self):
         models = [
             G(User, first_name='foo', last_name='foofington'),
             G(User, first_name='bar', last_name='barski'),
             G(User, first_name='foo', last_name='foogeelala'),
         ]
         # Make a user that is a superuser and verify they get all of the
         # super user perms
         u = G(User, is_superuser=True)
         r = core.Restraint(u)
 
         filtered_qset = r.filter_qset(
             User.objects.all(), 'can_access_users_named_foo', restrict_kwargs={'first_name': 'foo'})
-        self.assertEquals(set(filtered_qset), set(models + [u]))
+        self.assertEqual(set(filtered_qset), set(models + [u]))
 
     def test_filter_qset_restrict_subset_no_perms(self):
         models = [
             G(User, first_name='foo', last_name='foofington'),
             G(User, first_name='bar', last_name='barski'),
             G(User, first_name='foo', last_name='foogeelala'),
         ]
         # Make a user that is a superuser and verify they get all of the
         # super user perms
         u = G(User, is_superuser=False)
         r = core.Restraint(u)
 
         filtered_qset = r.filter_qset(
             User.objects.all(), 'can_access_users_named_foo', restrict_kwargs={'first_name': 'foo'})
-        self.assertEquals(set(filtered_qset), set([models[1]] + [u]))
+        self.assertEqual(set(filtered_qset), set([models[1]] + [u]))
 
 
 class UpdateRestraintDbTest(TestCase):
     def add_custom_permission_set(self):
         # Setup a custom permission set
         custom_permission_set = PermSet.objects.create(
             name='custom',
@@ -359,45 +359,45 @@
         config['default_access']['global']['can_alter_stuff'] = [constants.BOOLEAN_LEVELS_NAME]
         config['default_access']['restricted']['can_do_stuff'] = ['all_stuff', 'this_thing']
         mock_get_restraint_config.return_value = config
 
         # update again
         core.update_restraint_db()
 
-        self.assertEquals(
+        self.assertEqual(
             set(PermSet.objects.filter(is_private=True).values_list('name', flat=True)),
             {'global', 'restricted'}
         )
-        self.assertEquals(
+        self.assertEqual(
             set(PermSet.objects.filter(is_locked=True).values_list('name', flat=True)),
             {'restricted'}
         )
-        self.assertEquals(
+        self.assertEqual(
             set(PermSet.objects.filter(is_hidden=True).values_list('name', flat=True)),
             {'restricted'}
         )
-        self.assertEquals(
+        self.assertEqual(
             set(PermSet.objects.all().values_list('name', flat=True)),
             {'global', 'restricted', 'custom'}
         )
 
-        self.assertEquals(
+        self.assertEqual(
             set(Perm.objects.values_list('name', flat=True)),
             {'can_view_stuff', 'can_edit_stuff', 'can_do_stuff', 'can_alter_stuff'}
         )
-        self.assertEquals(
+        self.assertEqual(
             set(Perm.objects.filter(is_locked=True).values_list('name', flat=True)),
             {'can_view_stuff'}
         )
-        self.assertEquals(
+        self.assertEqual(
             set(Perm.objects.filter(is_hidden=True).values_list('name', flat=True)),
             {'can_view_stuff'}
         )
 
-        self.assertEquals(
+        self.assertEqual(
             list(PermLevel.objects.order_by(
                 'perm__name',
                 'name'
             ).values_list(
                 'perm__name',
                 'name'
             )),
@@ -407,15 +407,15 @@
                 ('can_do_stuff', 'this_thing'),
                 ('can_edit_stuff', 'all_stuff'),
                 ('can_edit_stuff', 'some_stuff'),
                 ('can_view_stuff', '')
             ]
         )
 
-        self.assertEquals(
+        self.assertEqual(
             list(
                 PermAccess.objects.order_by(
                     'perm_set__name',
                     'perm_levels__perm__name',
                     'perm_levels__name'
                 ).values_list(
                     'perm_set__name',
@@ -512,44 +512,44 @@
                     'can_edit_stuff': ['all_stuff'],
                 },
             }
         }
         mock_get_restraint_config.return_value = config
         core.update_restraint_db(flush_default_access=True)
 
-        self.assertEquals(
+        self.assertEqual(
             set(PermSet.objects.filter(is_private=True).values_list('name', flat=True)),
             {'global', 'restricted'}
         )
-        self.assertEquals(
+        self.assertEqual(
             set(PermSet.objects.all().values_list('name', flat=True)),
             {'custom', 'global', 'restricted'}
         )
 
-        self.assertEquals(
+        self.assertEqual(
             set(Perm.objects.values_list('name', flat=True)),
             {'can_view_stuff', 'can_edit_stuff'}
         )
 
-        self.assertEquals(
+        self.assertEqual(
             list(PermLevel.objects.order_by(
                 'perm__name',
                 'name'
             ).values_list(
                 'perm__name',
                 'name'
             )),
             [
                 ('can_edit_stuff', 'all_stuff'),
                 ('can_edit_stuff', 'some_stuff'),
                 ('can_view_stuff', '')
             ]
         )
 
-        self.assertEquals(
+        self.assertEqual(
             list(
                 PermAccess.objects.order_by(
                     'perm_set__name',
                     'perm_levels__perm__name',
                     'perm_levels__name'
                 ).values_list(
                     'perm_set__name',
```

### Comparing `django-restraint-2.2.0/restraint/tests/commands_tests.py` & `django-restraint-2.3.0/restraint/tests/commands_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.core.management import call_command
 from django.test import SimpleTestCase
-from mock import patch
+from unittest.mock import patch
 
 
 class UpdateRestraintDbTest(SimpleTestCase):
     @patch('restraint.management.commands.update_restraint_db.update_restraint_db', spec_set=True)
     def test_wo_flush_default_access(self, mock_update_restraint_db):
         call_command('update_restraint_db')
         mock_update_restraint_db.assert_called_once_with(flush_default_access=False)
```

### Comparing `django-restraint-2.2.0/restraint/tests/configuration.py` & `django-restraint-2.3.0/restraint/tests/configuration.py`

 * *Files identical despite different names*

### Comparing `django-restraint-2.2.0/restraint/tests/models_tests.py` & `django-restraint-2.3.0/restraint/tests/models_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,43 +33,43 @@
         permission_level = G(PermLevel, perm=F(name='my_perm'), name='my_level')
         PermAccess.objects.set_default(
             permission_set_name=permission_set.name,
             permission_name='my_perm',
             levels=[permission_level.name]
         )
         pa = PermAccess.objects.get(perm_user_id=0, perm_user_type=None, perm_set=permission_set)
-        self.assertEquals(list(pa.perm_levels.all()), [permission_level])
+        self.assertEqual(list(pa.perm_levels.all()), [permission_level])
 
         # Set defaults to none
         PermAccess.objects.set_default(
             permission_set_name=permission_set.name,
             permission_name='my_perm',
         )
         pa = PermAccess.objects.get(perm_user_id=0, perm_user_type=None, perm_set=permission_set)
-        self.assertEquals(list(pa.perm_levels.all()), [])
+        self.assertEqual(list(pa.perm_levels.all()), [])
 
     def test_add_individual_access_level_exists(self):
         """
         Tests adding an individual permission to a user.
         """
         u = G(User)
         pl = G(PermLevel, perm=F(name='my_perm'), name='my_level')
 
         PermAccess.objects.add_individual_access(u, 'my_perm', 'my_level')
         PermAccess.objects.add_individual_access(u, 'my_perm', 'my_level')
 
         pa = PermAccess.objects.get(perm_user_id=u.id, perm_user_type=ContentType.objects.get_for_model(u))
-        self.assertEquals(list(pa.perm_levels.all()), [pl])
+        self.assertEqual(list(pa.perm_levels.all()), [pl])
 
     def test_remove_individual_access_level_exists(self):
         """
         Tests adding an individual permission to a user.
         """
         u = G(User)
         G(PermLevel, perm=F(name='my_perm'), name='my_level')
 
         PermAccess.objects.add_individual_access(u, 'my_perm', 'my_level')
         PermAccess.objects.add_individual_access(u, 'my_perm', 'my_level')
         PermAccess.objects.remove_individual_access(u, 'my_perm', 'my_level')
 
         pa = PermAccess.objects.get(perm_user_id=u.id, perm_user_type=ContentType.objects.get_for_model(u))
-        self.assertEquals(list(pa.perm_levels.all()), [])
+        self.assertEqual(list(pa.perm_levels.all()), [])
```

### Comparing `django-restraint-2.2.0/restraint/core.py` & `django-restraint-2.3.0/restraint/core.py`

 * *Files identical despite different names*

### Comparing `django-restraint-2.2.0/restraint/models.py` & `django-restraint-2.3.0/restraint/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 
-from six import python_2_unicode_compatible
-
 from restraint.managers import PermSetManager, PermManager, PermLevelManager, PermAccessManager
 
 
-@python_2_unicode_compatible
 class PermSet(models.Model):
     """
     This is essentially a group that has a name.
     Each PermSet will have a PermAccess associated with it that will contain the groups full permissions
     The permissions are indicated through PermAccess.perm_levels.
 
     Fields:
@@ -30,15 +27,14 @@
 
     objects = PermSetManager()
 
     def __str__(self):
         return f'{self.display_name}:{self.name}'
 
 
-@python_2_unicode_compatible
 class Perm(models.Model):
     """
     This is the actual permission name specific to what each app will add, for example competition_all.
 
     Fields:
      - Name
      - Display_name
@@ -55,15 +51,14 @@
 
     objects = PermManager()
 
     def __str__(self):
         return f'{self.display_name}:{self.name}'
 
 
-@python_2_unicode_compatible
 class PermLevel(models.Model):
     """
     Each specific Perm can have different levels of access for the same permission.
     A blank level indicates that its either a yes/no decision
     Other options might look like all, created_by, etc...
     This should be unique and handled by each app independently
```

### Comparing `django-restraint-2.2.0/restraint/management/commands/update_restraint_db.py` & `django-restraint-2.3.0/restraint/management/commands/update_restraint_db.py`

 * *Files identical despite different names*

### Comparing `django-restraint-2.2.0/restraint/migrations/0003_auto_20230301_0109.py` & `django-restraint-2.3.0/restraint/migrations/0003_auto_20230301_0109.py`

 * *Files identical despite different names*

### Comparing `django-restraint-2.2.0/restraint/migrations/0002_permset_is_private.py` & `django-restraint-2.3.0/restraint/migrations/0002_permset_is_private.py`

 * *Files identical despite different names*

### Comparing `django-restraint-2.2.0/restraint/migrations/0001_initial.py` & `django-restraint-2.3.0/restraint/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import unicode_literals
 
 from django.db import models, migrations
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
```

### Comparing `django-restraint-2.2.0/django_restraint.egg-info/PKG-INFO` & `django-restraint-2.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-restraint
-Version: 2.2.0
+Version: 2.3.0
 Summary: A dynamic object-level permission system for Django
 Home-page: https://github.com/ambitioninc/django-restraint
 Author: Wes Kendall
 Author-email: opensource@ambition.com
 License: MIT
-Description: Full documentation is available at http://django-restraint.readthedocs.org
-        
 Keywords: Django,Permission
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
+
+Full documentation is available at http://django-restraint.readthedocs.org
```

### Comparing `django-restraint-2.2.0/setup.py` & `django-restraint-2.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,45 +13,45 @@
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
 setup(
     name='django-restraint',
     version=get_version(),
     description='A dynamic object-level permission system for Django',
     long_description=open('README.rst').read(),
     url='https://github.com/ambitioninc/django-restraint',
     author='Wes Kendall',
     author_email='opensource@ambition.com',
     keywords='Django, Permission',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Framework :: Django',
-        'Framework :: Django :: 2.0',
-        'Framework :: Django :: 2.1',
-        'Framework :: Django :: 2.2',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
     license='MIT',
-    install_requires=[
-        'Django>=2.0',
-        'django-manager-utils>=1.4.0',
-    ],
-    tests_require=[
-        'psycopg2',
-        'django_dynamic_fixture',
-        'django-nose>=1.4',
-        'mock>=1.0.1',
-        'coverage>=3.7.1',
-    ],
+    install_requires=install_requires,
+    tests_require=tests_require,
     test_suite='run_tests.run',
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `django-restraint-2.2.0/PKG-INFO` & `django-restraint-2.3.0/django_restraint.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-restraint
-Version: 2.2.0
+Version: 2.3.0
 Summary: A dynamic object-level permission system for Django
 Home-page: https://github.com/ambitioninc/django-restraint
 Author: Wes Kendall
 Author-email: opensource@ambition.com
 License: MIT
-Description: Full documentation is available at http://django-restraint.readthedocs.org
-        
 Keywords: Django,Permission
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
+
+Full documentation is available at http://django-restraint.readthedocs.org
```

