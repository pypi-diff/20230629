# Comparing `tmp/openstack-image-manager-0.3.1.tar.gz` & `tmp/openstack-image-manager-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstack-image-manager-0.3.1.tar", last modified: Fri Jun 23 21:33:32 2023, max compression
+gzip compressed data, was "openstack-image-manager-0.3.2.tar", last modified: Thu Jun 29 18:10:42 2023, max compression
```

## Comparing `openstack-image-manager-0.3.1.tar` & `openstack-image-manager-0.3.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.723476 openstack-image-manager-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.clouds.yml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.711475 openstack-image-manager-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/renovate.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.715475 openstack-image-manager-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/build-container-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/mirror-images-dry-run.yml
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/mirror-images.yml
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/test-python-setup.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/update-images.yml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/validate-configuration.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.yamllint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.zuul.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-23 21:33:32.723476 openstack-image-manager-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    40597 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/clouds.yml.sample
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.715475 openstack-image-manager-0.3.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/getting_started.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.715475 openstack-image-manager-0.3.1/doc/images/
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.715475 openstack-image-manager-0.3.1/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/etc/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/almalinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/centos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/cirros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/clearlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/debian.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/fedora.yml
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/flatcar.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/gardenlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/kubernetes.yml
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/octavia.yml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/opensuse.yml
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/opnsense.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/rockylinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/talos.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/openstack_image_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/openstack_image_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47634 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/openstack_image_manager/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/openstack_image_manager/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/openstack_image_manager/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/openstack_image_manager/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/playbooks/integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/playbooks/pre-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/playbooks/pre-real-world.yml
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/playbooks/real-world.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/scripts/build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      477 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/scripts/push.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/secure.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-23 21:33:32.723476 openstack-image-manager-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/test/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/integration/fixtures/test_image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/integration/test_manage_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/unit/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.879562 openstack-image-manager-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.clouds.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.863561 openstack-image-manager-0.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.github/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.867562 openstack-image-manager-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.github/workflows/build-container-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.github/workflows/mirror-images-dry-run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.github/workflows/mirror-images.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.github/workflows/test-python-setup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.github/workflows/update-images.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.github/workflows/validate-configuration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.yamllint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/.zuul.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 18:10:42.000000 openstack-image-manager-0.3.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-29 18:10:42.000000 openstack-image-manager-0.3.2/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-29 18:10:42.879562 openstack-image-manager-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    40779 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/clouds.yml.sample
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.867562 openstack-image-manager-0.3.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/doc/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/doc/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/doc/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.867562 openstack-image-manager-0.3.2/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/doc/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/doc/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/doc/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/doc/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.867562 openstack-image-manager-0.3.2/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.871562 openstack-image-manager-0.3.2/etc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/almalinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/centos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/cirros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/clearlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/debian.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/fedora.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/flatcar.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/gardenlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/kubernetes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/octavia.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/opensuse.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/opnsense.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/rockylinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/talos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/images/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/etc/schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.875562 openstack-image-manager-0.3.2/openstack_image_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/openstack_image_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47634 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/openstack_image_manager/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/openstack_image_manager/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/openstack_image_manager/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/openstack_image_manager/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.875562 openstack-image-manager-0.3.2/openstack_image_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-29 18:10:42.000000 openstack-image-manager-0.3.2/openstack_image_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-29 18:10:42.000000 openstack-image-manager-0.3.2/openstack_image_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:10:42.000000 openstack-image-manager-0.3.2/openstack_image_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-29 18:10:42.000000 openstack-image-manager-0.3.2/openstack_image_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:10:42.000000 openstack-image-manager-0.3.2/openstack_image_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 18:10:42.000000 openstack-image-manager-0.3.2/openstack_image_manager.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 18:10:42.000000 openstack-image-manager-0.3.2/openstack_image_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-29 18:10:42.000000 openstack-image-manager-0.3.2/openstack_image_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.875562 openstack-image-manager-0.3.2/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/playbooks/integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/playbooks/pre-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/playbooks/pre-real-world.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/playbooks/real-world.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.875562 openstack-image-manager-0.3.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/scripts/build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      477 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/scripts/push.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/secure.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-29 18:10:42.879562 openstack-image-manager-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.875562 openstack-image-manager-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.875562 openstack-image-manager-0.3.2/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/test/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.879562 openstack-image-manager-0.3.2/test/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/test/integration/fixtures/test_image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/test/integration/test_manage_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:42.879562 openstack-image-manager-0.3.2/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/test/unit/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-29 18:10:30.000000 openstack-image-manager-0.3.2/tox.ini
```

### Comparing `openstack-image-manager-0.3.1/.github/workflows/build-container-image.yml` & `openstack-image-manager-0.3.2/.github/workflows/build-container-image.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/.github/workflows/mirror-images-dry-run.yml` & `openstack-image-manager-0.3.2/.github/workflows/mirror-images-dry-run.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/.github/workflows/mirror-images.yml` & `openstack-image-manager-0.3.2/.github/workflows/mirror-images.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/.github/workflows/publish.yml` & `openstack-image-manager-0.3.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/.github/workflows/run-unit-tests.yml` & `openstack-image-manager-0.3.2/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/.github/workflows/test-python-setup.yml` & `openstack-image-manager-0.3.2/.github/workflows/test-python-setup.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/.github/workflows/update-images.yml` & `openstack-image-manager-0.3.2/.github/workflows/update-images.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/.github/workflows/validate-configuration.yml` & `openstack-image-manager-0.3.2/.github/workflows/validate-configuration.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/.zuul.yaml` & `openstack-image-manager-0.3.2/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/Containerfile` & `openstack-image-manager-0.3.2/Containerfile`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/Dockerfile` & `openstack-image-manager-0.3.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/LICENSE` & `openstack-image-manager-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/PKG-INFO` & `openstack-image-manager-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-image-manager
-Version: 0.3.1
+Version: 0.3.2
 Summary: OpenStack image manager
 Home-page: https://github.com/osism/openstack-image-manager
 Author: OSISM community
 Author-email: info@osism.tech
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `openstack-image-manager-0.3.1/Pipfile.lock` & `openstack-image-manager-0.3.2/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98804012345679%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'16a697c1f3d9903ce17540a49f38f729b44037e17ad0524f4cca04d6d1bf0e6b'}}",*

 * * "'default'": "{'jsonpatch': {'hashes': {insert: [(1, "*

 * *              "'sha256:9fcd4009c41e6d12348b4a0ff2563ba56a2923a7dfee731d004e212e1ee5030c')]}}, "*

 * *              "'jsonpointer': {'hashes': {insert: [(1, "*

 * *              "'sha256:585cee82b70211fa9e6043b7bb89db6e1aa49524340dde8ad6b63206ea689d88')]}}, "*

 * *              "'openstacksdk': {'hashes': "*

 * *              "['sha256:9727ca7d213ca25ebaa7 […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "a979a09d5096c774f26ccb5c6f299ee4dccab28428a004599c5938cda1afc17b"
+            "sha256": "16a697c1f3d9903ce17540a49f38f729b44037e17ad0524f4cca04d6d1bf0e6b"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -286,22 +286,24 @@
                 "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.1"
         },
         "jsonpatch": {
             "hashes": [
-                "sha256:0ae28c0cd062bbd8b8ecc26d7d164fbbea9652a1a3693f3b956c1eae5145dade"
+                "sha256:0ae28c0cd062bbd8b8ecc26d7d164fbbea9652a1a3693f3b956c1eae5145dade",
+                "sha256:9fcd4009c41e6d12348b4a0ff2563ba56a2923a7dfee731d004e212e1ee5030c"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
             "version": "==1.33"
         },
         "jsonpointer": {
             "hashes": [
-                "sha256:15d51bba20eea3165644553647711d150376234112651b4f1811022aecad7d7a"
+                "sha256:15d51bba20eea3165644553647711d150376234112651b4f1811022aecad7d7a",
+                "sha256:585cee82b70211fa9e6043b7bb89db6e1aa49524340dde8ad6b63206ea689d88"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
             "version": "==2.4"
         },
         "keystoneauth1": {
             "hashes": [
                 "sha256:d2fcfdcfe347df8d92390e0806b4969289d884cd9ec3519e4c5aec53e66d0767",
@@ -391,19 +393,19 @@
                 "sha256:e76c7f351e0444721e85f975ae92718e21c1f361bda946d60a214061de1f00a1",
                 "sha256:eb4813b77d5df99903af4757ce980a98c4d702bbcb81f32a0b305a1537bdf0b1"
             ],
             "version": "==0.11.0"
         },
         "openstacksdk": {
             "hashes": [
-                "sha256:207a75e5a81e1173bf251e9976965a66ff2ff379d0a0ba55a4903dcf2b5c1974",
-                "sha256:42afb8435b137905f7733f89a6627b7604f92adea7d49b3e22826c66e6062859"
+                "sha256:9727ca7d213ca25ebaa7a04337cc7488fd7a64cfe4f640ba4006a46483c04055",
+                "sha256:fa0fd8386bf7d7549a3aceb9c4e29a8b7049a7819b8640f56b01052f8a102cca"
             ],
             "index": "pypi",
-            "version": "==1.3.0"
+            "version": "==1.3.1"
         },
         "os-service-types": {
             "hashes": [
                 "sha256:0505c72205690910077fb72b88f2a1f07533c8d39f2fe75b29583481764965d6",
                 "sha256:31800299a82239363995b91f1ebf9106ac7758542a1e4ef6dc737a5932878c6c"
             ],
             "version": "==1.7.0"
@@ -623,19 +625,19 @@
                 "sha256:5d96d986a21493606a358cae4461bd8cdf83cbf33a5aa950ae629ca3b51467ee"
             ],
             "index": "pypi",
             "version": "==0.9.0"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
-                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
+                "sha256:5d8c9dac95c27d20df12fb1d97b9793ab8b2af8a3a525e68c80e21060c161771",
+                "sha256:935ccf31549830cda708b42289d44b6f74084d616a00be651601a4f968e77c82"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.6.3"
+            "version": "==4.7.0"
         },
         "urllib3": {
             "hashes": [
                 "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
                 "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
             "markers": "python_version >= '3.7'",
```

### Comparing `openstack-image-manager-0.3.1/doc/conf.py` & `openstack-image-manager-0.3.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/doc/configuration.md` & `openstack-image-manager-0.3.2/doc/configuration.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/doc/contribute.md` & `openstack-image-manager-0.3.2/doc/contribute.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/doc/getting_started.md` & `openstack-image-manager-0.3.2/doc/getting_started.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/doc/images/logo.png` & `openstack-image-manager-0.3.2/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/doc/overview.md` & `openstack-image-manager-0.3.2/doc/overview.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/doc/quickstart.md` & `openstack-image-manager-0.3.2/doc/quickstart.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/doc/requirements.md` & `openstack-image-manager-0.3.2/doc/requirements.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/almalinux.yml` & `openstack-image-manager-0.3.2/etc/images/almalinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/centos.yml` & `openstack-image-manager-0.3.2/etc/images/centos.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/cirros.yml` & `openstack-image-manager-0.3.2/etc/images/cirros.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/clearlinux.yml` & `openstack-image-manager-0.3.2/etc/images/clearlinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/debian.yml` & `openstack-image-manager-0.3.2/etc/images/debian.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/fedora.yml` & `openstack-image-manager-0.3.2/etc/images/fedora.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/flatcar.yml` & `openstack-image-manager-0.3.2/etc/images/flatcar.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/gardenlinux.yml` & `openstack-image-manager-0.3.2/etc/images/gardenlinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/kubernetes.yml` & `openstack-image-manager-0.3.2/etc/images/kubernetes.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,35 +18,23 @@
       hw_watchdog_action: reset
       os_distro: ubuntu
       replace_frequency: never
       uuid_validity: none
       provided_until: none
     tags: []
     versions:
-      - version: '1.24.13'
-        url: https://minio.services.osism.tech/openstack-k8s-capi-images/ubuntu-2004-kube-v1.24/ubuntu-2004-kube-v1.24.13.qcow2
-        checksum: "sha256:90152f4cb814b53b9e74b16b07475830a0ea7dadaa95213ac2ad27bf68344b2a"
-        build_date: '2023-04-19'
-      - version: '1.24.14'
-        url: https://minio.services.osism.tech/openstack-k8s-capi-images/ubuntu-2204-kube-v1.24/ubuntu-2204-kube-v1.24.14.qcow2
-        checksum: "sha256:51619fbe70e41101bd653679fca0c174d6d0cbd9b242acab4388e20b737b2149"
-        build_date: '2023-05-19'
-      - version: '1.25.9'
-        url: https://minio.services.osism.tech/openstack-k8s-capi-images/ubuntu-2004-kube-v1.25/ubuntu-2004-kube-v1.25.9.qcow2
-        checksum: "sha256:5f79c55d32072b483911c69be49e2f8ca9822c9d73571a5ece6123fbda1e8b68"
-        build_date: '2023-04-19'
-      - version: '1.25.10'
-        url: https://minio.services.osism.tech/openstack-k8s-capi-images/ubuntu-2204-kube-v1.25/ubuntu-2204-kube-v1.25.10.qcow2
-        checksum: "sha256:871db0170a567d839eb9f356588ed7ded03052b699e1213b6f28ba877c3f8748"
-        build_date: '2023-05-19'
-      - version: '1.26.4'
-        url: https://minio.services.osism.tech/openstack-k8s-capi-images/ubuntu-2004-kube-v1.26/ubuntu-2004-kube-v1.26.4.qcow2
-        checksum: "sha256:114a3d038135833a6abe3320fd0c5f5304b250dbfa17523165d0f3c3e450ece9"
-        build_date: '2023-04-19'
-      - version: '1.26.5'
-        url: https://minio.services.osism.tech/openstack-k8s-capi-images/ubuntu-2204-kube-v1.26/ubuntu-2204-kube-v1.26.5.qcow2
-        checksum: "sha256:ceb2d5e3af9b659ca6ca911a392b832aeb87c226fd587ff1bb45c674900441b9"
-        build_date: '2023-05-19'
-      - version: '1.27.1'
-        url: https://minio.services.osism.tech/openstack-k8s-capi-images/ubuntu-2204-kube-v1.27/ubuntu-2204-kube-v1.27.1.qcow2
-        checksum: "sha256:a76a3bac9e5bba4d270de75b8f9e07489af9d389e8ec964e55315caa0bcb6e84"
-        build_date: '2023-05-19'
+      - version: '1.24.15'
+        url: https://minio.services.osism.tech/openstack-k8s-capi-images/ubuntu-2204-kube-v1.24/ubuntu-2204-kube-v1.24.15.qcow2
+        checksum: "sha256:12fbfead6400fae2fac20b8fae130e23afc351c44ad120deee2318b4bc7b2e59"
+        build_date: '2023-06-15'
+      - version: '1.25.11'
+        url: https://minio.services.osism.tech/openstack-k8s-capi-images/ubuntu-2204-kube-v1.25/ubuntu-2204-kube-v1.25.11.qcow2
+        checksum: "sha256:7870a6c7c1761c572c070ca7b776b39344d8d2fd0dca28718fff433e9dca1a8f"
+        build_date: '2023-06-21'
+      - version: '1.26.6'
+        url: https://minio.services.osism.tech/openstack-k8s-capi-images/ubuntu-2204-kube-v1.26/ubuntu-2204-kube-v1.26.6.qcow2
+        checksum: "sha256:0243eeee8a55ed9d9f920d4b168ec548541dc2504c996d58a20be5f6d6518409"
+        build_date: '2023-06-21'
+      - version: '1.27.3'
+        url: https://minio.services.osism.tech/openstack-k8s-capi-images/ubuntu-2204-kube-v1.27/ubuntu-2204-kube-v1.27.3.qcow2
+        checksum: "sha256:857bbb11f29faba71f9f6dc1c44ed657507e422b42f589e1d96da2711c41d5bf"
+        build_date: '2023-06-21'
```

### Comparing `openstack-image-manager-0.3.1/etc/images/octavia.yml` & `openstack-image-manager-0.3.2/etc/images/octavia.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/opensuse.yml` & `openstack-image-manager-0.3.2/etc/images/opensuse.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/opnsense.yml` & `openstack-image-manager-0.3.2/etc/images/opnsense.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/rockylinux.yml` & `openstack-image-manager-0.3.2/etc/images/rockylinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/talos.yml` & `openstack-image-manager-0.3.2/etc/images/talos.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/images/ubuntu.yml` & `openstack-image-manager-0.3.2/etc/images/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/etc/schema.yaml` & `openstack-image-manager-0.3.2/etc/schema.yaml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/openstack_image_manager/manage.py` & `openstack-image-manager-0.3.2/openstack_image_manager/manage.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/openstack_image_manager/mirror.py` & `openstack-image-manager-0.3.2/openstack_image_manager/mirror.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/openstack_image_manager/table.py` & `openstack-image-manager-0.3.2/openstack_image_manager/table.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/openstack_image_manager/update.py` & `openstack-image-manager-0.3.2/openstack_image_manager/update.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/openstack_image_manager.egg-info/PKG-INFO` & `openstack-image-manager-0.3.2/openstack_image_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-image-manager
-Version: 0.3.1
+Version: 0.3.2
 Summary: OpenStack image manager
 Home-page: https://github.com/osism/openstack-image-manager
 Author: OSISM community
 Author-email: info@osism.tech
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `openstack-image-manager-0.3.1/openstack_image_manager.egg-info/SOURCES.txt` & `openstack-image-manager-0.3.2/openstack_image_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/playbooks/real-world.yml` & `openstack-image-manager-0.3.2/playbooks/real-world.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/scripts/build.sh` & `openstack-image-manager-0.3.2/scripts/build.sh`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/setup.cfg` & `openstack-image-manager-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/test/integration/fixtures/test_image.yml` & `openstack-image-manager-0.3.2/test/integration/fixtures/test_image.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/test/integration/test_manage_api.py` & `openstack-image-manager-0.3.2/test/integration/test_manage_api.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/test/unit/test_manage.py` & `openstack-image-manager-0.3.2/test/unit/test_manage.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.1/tox.ini` & `openstack-image-manager-0.3.2/tox.ini`

 * *Files identical despite different names*

