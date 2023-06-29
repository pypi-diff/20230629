# Comparing `tmp/blivet-3.7.1.tar.gz` & `tmp/blivet-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blivet-3.7.1.tar", last modified: Thu Mar 16 09:57:06 2023, max compression
+gzip compressed data, was "blivet-3.8.0.tar", last modified: Thu Jun 29 11:33:28 2023, max compression
```

## Comparing `blivet-3.7.1.tar` & `blivet-3.8.0.tar`

### file list

```diff
@@ -1,1420 +1,1422 @@
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.496378 blivet-3.7.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.415376 blivet-3.7.1/.github/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.433376 blivet-3.7.1/.github/workflows/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1700 2023-03-16 09:40:21.000000 blivet-3.7.1/.github/workflows/anaconda_tests.yml
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      474 2023-03-16 09:40:21.000000 blivet-3.7.1/.github/workflows/check.yml
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      472 2023-03-16 09:40:21.000000 blivet-3.7.1/.github/workflows/unit_tests.yml
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      384 2023-03-16 09:40:21.000000 blivet-3.7.1/.gitignore
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       90 2023-03-16 09:40:21.000000 blivet-3.7.1/.gitmodules
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      350 2023-03-16 09:40:21.000000 blivet-3.7.1/.packit.yaml
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4643 2023-03-16 09:40:21.000000 blivet-3.7.1/CONTRIBUTING
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    18092 2023-03-16 09:40:21.000000 blivet-3.7.1/COPYING
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    26530 2023-03-16 09:40:21.000000 blivet-3.7.1/COPYING.LESSER
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      160 2023-03-16 09:40:21.000000 blivet-3.7.1/MANIFEST.in
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7504 2023-03-16 09:40:21.000000 blivet-3.7.1/Makefile
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3924 2023-03-16 09:57:06.496378 blivet-3.7.1/PKG-INFO
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3289 2023-03-16 09:40:21.000000 blivet-3.7.1/README.md
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      869 2023-03-16 09:40:21.000000 blivet-3.7.1/TODO
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.435376 blivet-3.7.1/blivet/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5106 2023-03-16 09:43:56.000000 blivet-3.7.1/blivet/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    12431 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/actionlist.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11071 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/arch.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    50041 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/blivet.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9454 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/callbacks.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.436376 blivet-3.7.1/blivet/dbus/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1014 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/dbus/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1982 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/dbus/action.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10379 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/dbus/blivet.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1732 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/dbus/constants.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3154 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/dbus/device.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2451 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/dbus/format.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2971 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/dbus/manager.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4683 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/dbus/object.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    43725 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/deviceaction.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    88252 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicefactory.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.437376 blivet-3.7.1/blivet/devicelibs/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicelibs/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1429 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicelibs/btrfs.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4530 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicelibs/crypto.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3521 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicelibs/disk.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    32101 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicelibs/edd.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    12465 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicelibs/gpt.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8717 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicelibs/lvm.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1576 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicelibs/mdraid.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    24513 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicelibs/raid.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10243 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicelibs/stratis.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.438376 blivet-3.7.1/blivet/devices/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2086 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    25591 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/btrfs.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3726 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/cache.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7637 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/container.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    12651 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/device.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    26971 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/disk.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10107 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/dm.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5288 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/file.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6636 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/lib.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4458 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/loop.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10031 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/luks.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)   119532 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/lvm.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    29654 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/md.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2087 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/network.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3032 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/nfs.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3743 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/nodev.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2849 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/optical.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    40725 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/partition.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4820 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/raid.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    32913 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/storage.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9597 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devices/stratis.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    41311 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/devicetree.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6604 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/errors.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.439376 blivet-3.7.1/blivet/events/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/events/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4285 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/events/changes.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11201 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/events/handler.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11428 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/events/manager.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7798 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/fcoe.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3844 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/flags.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.440376 blivet-3.7.1/blivet/formats/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    25432 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2225 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/biosboot.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    22837 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/disklabel.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2298 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/dmraid.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    49887 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/fs.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1573 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/fslib.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    20009 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/luks.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8428 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/lvmpv.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3801 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/mdraid.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2903 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/multipath.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3619 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/prepboot.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5192 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/stratis.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7795 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/formats/swap.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2436 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/i18n.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    22061 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/iscsi.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6935 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/mounts.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2367 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/nvme.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    85044 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/partitioning.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.440376 blivet-3.7.1/blivet/populator/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       38 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/__init__.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.441376 blivet-3.7.1/blivet/populator/helpers/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2589 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2712 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/boot.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4453 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/btrfs.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2082 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/devicepopulator.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11765 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/disk.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6362 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/disklabel.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2524 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/dm.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4241 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/formatpopulator.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2590 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/loop.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7430 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/luks.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    19936 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/lvm.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8678 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/mdraid.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2566 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/multipath.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2064 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/optical.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4269 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/partition.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2869 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/populatorhelper.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7591 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/helpers/stratis.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    21471 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/populator/populator.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8267 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/safe_dbus.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7154 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/size.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.442376 blivet-3.7.1/blivet/static_data/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      188 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/static_data/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3523 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/static_data/luks_data.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4047 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/static_data/lvm_info.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2431 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/static_data/mpath_info.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5359 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/static_data/nvdimm.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10260 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/static_data/stratis_info.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2687 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/storage_log.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.443376 blivet-3.7.1/blivet/tasks/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    22386 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/availability.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1598 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/dfresize.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5413 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fsck.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3085 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fsinfo.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3202 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fslabeling.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5790 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fsminsize.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10533 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fsmkfs.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6136 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fsmount.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3723 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fsreadlabel.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6128 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fsresize.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4838 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fssize.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2961 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fssync.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1784 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fstask.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2143 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fsuuid.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3362 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fswritelabel.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1949 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/fswriteuuid.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3355 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/lukstasks.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2885 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/pvtask.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3333 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tasks/task.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3751 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/threads.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3459 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/tsort.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    34946 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/udev.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    36572 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/util.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    20888 2023-03-16 09:40:21.000000 blivet-3.7.1/blivet/zfcp.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.435376 blivet-3.7.1/blivet.egg-info/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3924 2023-03-16 09:57:05.000000 blivet-3.7.1/blivet.egg-info/PKG-INFO
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    69942 2023-03-16 09:57:06.000000 blivet-3.7.1/blivet.egg-info/SOURCES.txt
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        1 2023-03-16 09:57:05.000000 blivet-3.7.1/blivet.egg-info/dependency_links.txt
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:57:06.000000 blivet-3.7.1/blivet.egg-info/requires.txt
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        7 2023-03-16 09:57:06.000000 blivet-3.7.1/blivet.egg-info/top_level.txt
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.444376 blivet-3.7.1/dbus/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      400 2023-03-16 09:40:21.000000 blivet-3.7.1/dbus/blivet.conf
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      113 2023-03-16 09:40:21.000000 blivet-3.7.1/dbus/blivet.service
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)      364 2023-03-16 09:40:21.000000 blivet-3.7.1/dbus/blivetd
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      106 2023-03-16 09:40:21.000000 blivet-3.7.1/dbus/com.redhat.Blivet0.service
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.444376 blivet-3.7.1/doc/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5612 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/Makefile
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1023 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/_inheritance.rst
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.445376 blivet-3.7.1/doc/api/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11681 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/api/blivet.rst
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8591 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/api/devices.rst
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      423 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/api/events.rst
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7034 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/api/formats.rst
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1998 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/api.rst
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9447 2023-03-16 09:43:56.000000 blivet-3.7.1/doc/conf.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4814 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/dbus.rst
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      545 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/index.rst
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7908 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/intro.rst
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3953 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/lvmvdo.rst
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       34 2023-03-16 09:40:21.000000 blivet-3.7.1/doc/testing.rst
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.446376 blivet-3.7.1/examples/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2089 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/actions.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      825 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/dbus_client.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1560 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/factory.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      205 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/list_devices.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2174 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/lvm.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1996 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/lvm_cache.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1778 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/lvm_cachepool.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2168 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/lvm_non_linear.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1417 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/lvm_thin.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2167 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/lvm_vdo.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2884 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/partitioning.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1816 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/stratis.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      526 2023-03-16 09:40:21.000000 blivet-3.7.1/examples/uevents.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.446376 blivet-3.7.1/misc/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3050 2023-03-16 09:40:21.000000 blivet-3.7.1/misc/Vagrantfile
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5119 2023-03-16 09:40:21.000000 blivet-3.7.1/misc/install-test-dependencies.yml
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.458377 blivet-3.7.1/po/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1262 2023-03-16 09:57:03.000000 blivet-3.7.1/po/Makefile
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      944 2023-03-16 09:57:05.000000 blivet-3.7.1/po/af.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9722 2023-03-16 09:57:03.000000 blivet-3.7.1/po/af.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1059 2023-03-16 09:57:05.000000 blivet-3.7.1/po/am.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9831 2023-03-16 09:57:03.000000 blivet-3.7.1/po/am.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1169 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ar.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10348 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ar.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9162 2023-03-16 09:57:05.000000 blivet-3.7.1/po/as.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15098 2023-03-16 09:57:03.000000 blivet-3.7.1/po/as.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3660 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ast.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11161 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ast.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8312 2023-03-16 09:57:05.000000 blivet-3.7.1/po/bg.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14404 2023-03-16 09:57:03.000000 blivet-3.7.1/po/bg.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9366 2023-03-16 09:57:03.000000 blivet-3.7.1/po/blivet.pot
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5487 2023-03-16 09:57:05.000000 blivet-3.7.1/po/bn.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    13553 2023-03-16 09:57:03.000000 blivet-3.7.1/po/bn.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14554 2023-03-16 09:57:05.000000 blivet-3.7.1/po/bn_IN.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    19308 2023-03-16 09:57:03.000000 blivet-3.7.1/po/bn_IN.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      939 2023-03-16 09:57:05.000000 blivet-3.7.1/po/bs.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9798 2023-03-16 09:57:03.000000 blivet-3.7.1/po/bs.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9507 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ca.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14442 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ca.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10252 2023-03-16 09:57:05.000000 blivet-3.7.1/po/cs.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14722 2023-03-16 09:57:03.000000 blivet-3.7.1/po/cs.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      943 2023-03-16 09:57:05.000000 blivet-3.7.1/po/cy.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9775 2023-03-16 09:57:03.000000 blivet-3.7.1/po/cy.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9554 2023-03-16 09:57:05.000000 blivet-3.7.1/po/da.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14077 2023-03-16 09:57:03.000000 blivet-3.7.1/po/da.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10456 2023-03-16 09:57:05.000000 blivet-3.7.1/po/de.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15434 2023-03-16 09:57:03.000000 blivet-3.7.1/po/de.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1239 2023-03-16 09:57:05.000000 blivet-3.7.1/po/de_CH.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10347 2023-03-16 09:57:03.000000 blivet-3.7.1/po/de_CH.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1377 2023-03-16 09:57:05.000000 blivet-3.7.1/po/el.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10406 2023-03-16 09:57:03.000000 blivet-3.7.1/po/el.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3591 2023-03-16 09:57:05.000000 blivet-3.7.1/po/en_GB.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11196 2023-03-16 09:57:03.000000 blivet-3.7.1/po/en_GB.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10416 2023-03-16 09:57:05.000000 blivet-3.7.1/po/es.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15603 2023-03-16 09:57:03.000000 blivet-3.7.1/po/es.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1280 2023-03-16 09:57:05.000000 blivet-3.7.1/po/et.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9997 2023-03-16 09:57:03.000000 blivet-3.7.1/po/et.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      620 2023-03-16 09:57:05.000000 blivet-3.7.1/po/eu.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9639 2023-03-16 09:57:03.000000 blivet-3.7.1/po/eu.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7338 2023-03-16 09:57:05.000000 blivet-3.7.1/po/fa.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    13823 2023-03-16 09:57:03.000000 blivet-3.7.1/po/fa.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10323 2023-03-16 09:57:05.000000 blivet-3.7.1/po/fi.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14226 2023-03-16 09:57:03.000000 blivet-3.7.1/po/fi.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10981 2023-03-16 09:57:05.000000 blivet-3.7.1/po/fr.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15783 2023-03-16 09:57:03.000000 blivet-3.7.1/po/fr.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10674 2023-03-16 09:57:05.000000 blivet-3.7.1/po/fur.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14142 2023-03-16 09:57:03.000000 blivet-3.7.1/po/fur.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8423 2023-03-16 09:57:05.000000 blivet-3.7.1/po/gu.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14666 2023-03-16 09:57:03.000000 blivet-3.7.1/po/gu.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1216 2023-03-16 09:57:05.000000 blivet-3.7.1/po/he.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9914 2023-03-16 09:57:03.000000 blivet-3.7.1/po/he.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4840 2023-03-16 09:57:05.000000 blivet-3.7.1/po/hi.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    12552 2023-03-16 09:57:03.000000 blivet-3.7.1/po/hi.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10464 2023-03-16 09:57:05.000000 blivet-3.7.1/po/hr.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14021 2023-03-16 09:57:03.000000 blivet-3.7.1/po/hr.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10396 2023-03-16 09:57:05.000000 blivet-3.7.1/po/hu.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14920 2023-03-16 09:57:03.000000 blivet-3.7.1/po/hu.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5160 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ia.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11904 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ia.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10366 2023-03-16 09:57:05.000000 blivet-3.7.1/po/id.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14243 2023-03-16 09:57:03.000000 blivet-3.7.1/po/id.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      945 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ilo.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9726 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ilo.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1053 2023-03-16 09:57:05.000000 blivet-3.7.1/po/is.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9763 2023-03-16 09:57:03.000000 blivet-3.7.1/po/is.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9517 2023-03-16 09:57:05.000000 blivet-3.7.1/po/it.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14933 2023-03-16 09:57:03.000000 blivet-3.7.1/po/it.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11782 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ja.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    16274 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ja.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11912 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ka.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    16727 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ka.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    12917 2023-03-16 09:57:05.000000 blivet-3.7.1/po/kk.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    16397 2023-03-16 09:57:03.000000 blivet-3.7.1/po/kk.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9449 2023-03-16 09:57:05.000000 blivet-3.7.1/po/kn.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15947 2023-03-16 09:57:03.000000 blivet-3.7.1/po/kn.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10960 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ko.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14948 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ko.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1380 2023-03-16 09:57:05.000000 blivet-3.7.1/po/lv.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10006 2023-03-16 09:57:03.000000 blivet-3.7.1/po/lv.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1878 2023-03-16 09:57:05.000000 blivet-3.7.1/po/mai.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10481 2023-03-16 09:57:03.000000 blivet-3.7.1/po/mai.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      977 2023-03-16 09:57:05.000000 blivet-3.7.1/po/mk.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9971 2023-03-16 09:57:03.000000 blivet-3.7.1/po/mk.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8639 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ml.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15344 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ml.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8864 2023-03-16 09:57:05.000000 blivet-3.7.1/po/mr.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15305 2023-03-16 09:57:03.000000 blivet-3.7.1/po/mr.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      890 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ms.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9755 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ms.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9565 2023-03-16 09:57:05.000000 blivet-3.7.1/po/nb.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    13988 2023-03-16 09:57:03.000000 blivet-3.7.1/po/nb.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1210 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ne.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10132 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ne.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9877 2023-03-16 09:57:05.000000 blivet-3.7.1/po/nl.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14565 2023-03-16 09:57:03.000000 blivet-3.7.1/po/nl.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      935 2023-03-16 09:57:05.000000 blivet-3.7.1/po/nso.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9713 2023-03-16 09:57:03.000000 blivet-3.7.1/po/nso.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8185 2023-03-16 09:57:05.000000 blivet-3.7.1/po/or.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14855 2023-03-16 09:57:03.000000 blivet-3.7.1/po/or.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8387 2023-03-16 09:57:05.000000 blivet-3.7.1/po/pa.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14768 2023-03-16 09:57:03.000000 blivet-3.7.1/po/pa.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10862 2023-03-16 09:57:05.000000 blivet-3.7.1/po/pl.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15246 2023-03-16 09:57:03.000000 blivet-3.7.1/po/pl.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10257 2023-03-16 09:57:05.000000 blivet-3.7.1/po/pt.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14489 2023-03-16 09:57:03.000000 blivet-3.7.1/po/pt.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10393 2023-03-16 09:57:05.000000 blivet-3.7.1/po/pt_BR.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15638 2023-03-16 09:57:03.000000 blivet-3.7.1/po/pt_BR.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      951 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ro.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9726 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ro.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    13409 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ru.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    18138 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ru.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4859 2023-03-16 09:57:05.000000 blivet-3.7.1/po/si.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    12466 2023-03-16 09:57:03.000000 blivet-3.7.1/po/si.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10698 2023-03-16 09:57:05.000000 blivet-3.7.1/po/sk.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14702 2023-03-16 09:57:03.000000 blivet-3.7.1/po/sk.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      953 2023-03-16 09:57:05.000000 blivet-3.7.1/po/sl.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9987 2023-03-16 09:57:03.000000 blivet-3.7.1/po/sl.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1052 2023-03-16 09:57:05.000000 blivet-3.7.1/po/sq.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9767 2023-03-16 09:57:03.000000 blivet-3.7.1/po/sq.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9864 2023-03-16 09:57:05.000000 blivet-3.7.1/po/sr.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15052 2023-03-16 09:57:03.000000 blivet-3.7.1/po/sr.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3409 2023-03-16 09:57:05.000000 blivet-3.7.1/po/sr@latin.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11051 2023-03-16 09:57:03.000000 blivet-3.7.1/po/sr@latin.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10387 2023-03-16 09:57:05.000000 blivet-3.7.1/po/sv.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14443 2023-03-16 09:57:03.000000 blivet-3.7.1/po/sv.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8111 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ta.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15091 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ta.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9153 2023-03-16 09:57:05.000000 blivet-3.7.1/po/te.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15384 2023-03-16 09:57:03.000000 blivet-3.7.1/po/te.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      769 2023-03-16 09:57:05.000000 blivet-3.7.1/po/tg.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9652 2023-03-16 09:57:03.000000 blivet-3.7.1/po/tg.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1471 2023-03-16 09:57:05.000000 blivet-3.7.1/po/th.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10233 2023-03-16 09:57:03.000000 blivet-3.7.1/po/th.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10625 2023-03-16 09:57:05.000000 blivet-3.7.1/po/tr.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14535 2023-03-16 09:57:03.000000 blivet-3.7.1/po/tr.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    13478 2023-03-16 09:57:05.000000 blivet-3.7.1/po/uk.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    17502 2023-03-16 09:57:03.000000 blivet-3.7.1/po/uk.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      987 2023-03-16 09:57:05.000000 blivet-3.7.1/po/ur.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9759 2023-03-16 09:57:03.000000 blivet-3.7.1/po/ur.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     9831 2023-03-16 09:57:05.000000 blivet-3.7.1/po/zh_CN.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    13838 2023-03-16 09:57:03.000000 blivet-3.7.1/po/zh_CN.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8734 2023-03-16 09:57:05.000000 blivet-3.7.1/po/zh_TW.mo
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    13649 2023-03-16 09:57:03.000000 blivet-3.7.1/po/zh_TW.po
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)   202267 2023-03-16 09:43:56.000000 blivet-3.7.1/python-blivet.spec
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15241 2023-03-16 09:43:56.000000 blivet-3.7.1/release_notes.rst
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.459377 blivet-3.7.1/scripts/
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)     2905 2023-03-16 09:40:21.000000 blivet-3.7.1/scripts/docs-update
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)     1127 2023-03-16 09:40:21.000000 blivet-3.7.1/scripts/git-multi-merge
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)     1874 2023-03-16 09:40:21.000000 blivet-3.7.1/scripts/harvest-edd
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)    20059 2023-03-16 09:40:21.000000 blivet-3.7.1/scripts/makebumpver
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)     6641 2023-03-16 09:40:21.000000 blivet-3.7.1/scripts/makeupdates
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)     5460 2023-03-16 09:40:21.000000 blivet-3.7.1/scripts/pylintcodediff
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       38 2023-03-16 09:57:06.496378 blivet-3.7.1/setup.cfg
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3561 2023-03-16 09:43:56.000000 blivet-3.7.1/setup.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.459377 blivet-3.7.1/tests/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3395 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/README.rst
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      258 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/conftest.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.459377 blivet-3.7.1/tests/pylint/
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)     6067 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/pylint/censorship.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    12535 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/pylint/pylintrc
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)     4936 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/pylint/runpylint.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6862 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/run_tests.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1007 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/skip.yml
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.460377 blivet-3.7.1/tests/storage_tests/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      132 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/__init__.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.460377 blivet-3.7.1/tests/storage_tests/devices_test/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       82 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/devices_test/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    16011 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/devices_test/lvm_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    12789 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/devices_test/partition_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6518 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/devices_test/stratis_test.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.461377 blivet-3.7.1/tests/storage_tests/formats_test/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      128 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/formats_test/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7749 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/formats_test/fs_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6988 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/formats_test/fslabeling.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    14365 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/formats_test/fstesting.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4243 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/formats_test/fsuuid.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4279 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/formats_test/labeling_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5554 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/formats_test/loopbackedtestcase.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2760 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/formats_test/luks_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1419 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/formats_test/lvmpv_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4156 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/formats_test/uuid_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3538 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/imagebackedtestcase.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    32748 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/partitioning_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6455 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/storagetestcase.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8425 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/storage_tests/unsupported_disklabel_test.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.463377 blivet-3.7.1/tests/unit_tests/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      476 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    67699 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/action_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11603 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/blivettestcase.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     8808 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/dbus_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    49169 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicefactory_test.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.463377 blivet-3.7.1/tests/unit_tests/devicelibs_test/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      101 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5746 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/disk_test.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.464377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sda
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdb
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdc
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdd
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sde
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/vda
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.464377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/ata_port/ata7/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/ata_port/ata7/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:0/6:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:0/6:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:0/6:0:0:0/block/sr0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:1/6:0:1:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:1/6:0:1:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:1/6:0:1:0/block/sdb/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/ata_link/link7/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.0/ata_device/dev7.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.416375 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.1/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.1/ata_device/dev7.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/sda/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host9/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host9/target9:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host9/target9:0:0/9:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host9/target9:0:0/9:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host9/target9:0:0/9:0:0:0/block/sdd/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:07.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/block/vda/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/host10/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/host10/target10:0:1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/host10/target10:0:1/10:0:1:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/host10/target10:0:1/10:0:1:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/host10/target10:0:1/10:0:1:0/block/sde/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/host8/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/host8/target8:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/host8/target8:0:0/8:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/host8/target8:0:0/8:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/host8/target8:0:0/8:0:0:0/block/sdc/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.417376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.465377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        6 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       25 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       23 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        9 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.466377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       25 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       19 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        7 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.467377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       26 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        7 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.468377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        6 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       26 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        7 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.469377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        6 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       25 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       23 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        7 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.470377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        6 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       26 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        8 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.470377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sda
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sdb
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sdc
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sr0
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.470377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/scsi_host/host12/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/block/sr0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/scsi_device/12:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/ata_link/link13/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/ata_device/dev13.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/ata_device/dev13.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.470377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/ata_link/link14/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/ata_device/dev14.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.418376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/ata_device/dev14.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.471377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/scsi_host/host0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/sda/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_device/0:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/0:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/ata_link/link1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/ata_device/dev1.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.471377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/ata_link/link2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/ata_device/dev2.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.471377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/ata_link/link3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/ata_device/dev3.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.419376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.471377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/ata_link/link4/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/ata_device/dev4.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.472377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/ata_link/link5/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/ata_device/dev5.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.472377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/ata_link/link6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/ata_device/dev6.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.472377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/scsi_host/host9/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/block/sdb/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_device/9:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_disk/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_disk/9:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/ata_link/link10/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.420376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/ata_device/dev10.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.472377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/scsi_host/host10/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/block/sdc/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/scsi_device/10:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/scsi_disk/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/scsi_disk/10:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/ata_link/link11/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/ata_device/dev11.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.472377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/ata_link/link12/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/ata_device/dev12.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.473377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/ata_link/link7/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.421376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/ata_device/dev7.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.473377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/ata_link/link8/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/ata_device/dev8.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.473377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/ata_link/link9/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/ata_device/dev9.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.474377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        6 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       26 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        9 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.475377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       26 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        7 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.476377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       26 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        7 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.476377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sda
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sdb
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sdc
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sr0
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/vda
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.477377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/scsi_host/host12/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/block/sr0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.422376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/scsi_device/12:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/ata_link/link13/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/ata_device/dev13.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/ata_device/dev13.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.477377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/ata_link/link14/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/ata_device/dev14.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/ata_device/dev14.1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.477377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/scsi_host/host0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/sda/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_device/0:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/0:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/ata_link/link1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.423376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/ata_device/dev1.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.477377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/ata_link/link2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/ata_device/dev2.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.477377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/ata_link/link3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/ata_device/dev3.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.478377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/ata_link/link4/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/ata_device/dev4.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.478377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/ata_link/link5/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/ata_device/dev5.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.478377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.424376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/ata_link/link6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/ata_device/dev6.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/scsi_host/host14/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/block/sdc/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/scsi_device/14:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/scsi_disk/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/scsi_disk/14:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:07.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/block/vda/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.478377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/scsi_host/host9/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/block/sdb/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_device/9:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_disk/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_disk/9:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/ata_link/link10/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.425376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/ata_device/dev10.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.478377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/ata_link/link11/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/ata_device/dev11.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.479377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/ata_link/link12/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/ata_device/dev12.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.479377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/ata_link/link7/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/ata_device/dev7.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.479377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/ata_link/link8/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/ata_device/dev8.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.479377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.426376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/ata_link/link9/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/ata_device/dev9.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.480377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        6 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       27 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       41 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        9 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.482377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       27 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       19 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        7 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.483378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       27 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       19 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        7 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.483378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.484377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/dev/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/dev/sda
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/dev/sdb
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/block/sdb/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.484377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/ata2/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/ata2/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/block/sda/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/ata_device/dev2.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.427376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.485377 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        6 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       46 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       27 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       19 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4096 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       10 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.486378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       46 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       29 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       33 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4096 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        9 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.486378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sda
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sdb
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sdc
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      512 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sdd
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sr0
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/scsi_host/host6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/block/sdd/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/scsi_device/6:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/scsi_disk/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/scsi_disk/6:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.486378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/ata_port/ata1/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/ata_port/ata1/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/ata_port/ata1/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/scsi_host/host0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/block/sda/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/scsi_device/0:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/0:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/ata_link/link1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/dev1.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/dev1.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.428376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/dev1.0/ata_device/dev1.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.487378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/ata2/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/ata2/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/ata2/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/scsi_host/host1/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/block/sdb/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/scsi_device/1:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/scsi_disk/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/scsi_disk/1:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/ata_link/link2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/ata_device/dev2.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.487378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/ata_port/ata3/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/ata_port/ata3/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/ata_port/ata3/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/scsi_host/host2/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/block/sdc/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/scsi_device/2:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/scsi_disk/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/scsi_disk/2:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/ata_link/link3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/dev3.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/dev3.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.429376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/dev3.0/ata_device/dev3.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.487378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/ata_port/ata4/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/ata_port/ata4/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/ata_port/ata4/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/scsi_host/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/scsi_host/host3/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/3:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/3:0:0:0/block/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/3:0:0:0/block/sr0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/3:0:0:0/scsi_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/3:0:0:0/scsi_device/3:0:0:0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/ata_link/link4/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/dev4.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/dev4.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/dev4.0/ata_device/dev4.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.487378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/ata_port/ata5/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/ata_port/ata5/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/ata_port/ata5/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/ata_link/link5/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/dev5.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/dev5.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/dev5.0/ata_device/dev5.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/ata_port/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.487378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/ata_port/ata6/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/ata_port/ata6/nr_pmp_links
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        2 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/ata_port/ata6/port_no
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/ata_link/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/ata_link/link6/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/dev6.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/dev6.0/ata_device/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.430376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/dev6.0/ata_device/dev6.0/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.431376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.431376 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.489378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       46 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       29 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       33 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        9 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.490378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        6 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       46 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       27 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       19 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       10 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.491378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        6 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       46 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       27 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       19 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       10 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/version
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.492378 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        6 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/default_cylinders
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/default_heads
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/default_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       46 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/extensions
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       27 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/host_bus
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       15 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/info_flags
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       19 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/interface
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/legacy_max_cylinder
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        4 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/legacy_max_head
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        3 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/legacy_sectors_per_track
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       11 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/mbr_signature
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       74 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/raw_data
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       10 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/sectors
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        5 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/version
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    41491 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1324 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/lib.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      644 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/mdraid_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7083 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicelibs_test/raid_test.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.493378 blivet-3.7.1/tests/unit_tests/devices_test/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      372 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11726 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/device_dependencies_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    16531 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/device_methods_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3287 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/device_names_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1024 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/device_packages_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    43458 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/device_properties_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3823 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/device_size_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2442 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/disk_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    53219 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/lvm_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3856 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/md_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2184 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/network_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6542 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/partition_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4659 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devices_test/stratis_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    23110 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/devicetree_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2825 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/events_test.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.494378 blivet-3.7.1/tests/unit_tests/formats_tests/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      213 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/formats_tests/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3185 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/formats_tests/device_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7702 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/formats_tests/disklabel_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1466 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/formats_tests/init_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2001 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/formats_tests/luks_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    17899 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/formats_tests/methods_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      962 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/formats_tests/misc_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2266 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/formats_tests/selinux_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      656 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/formats_tests/swap_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3221 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/gpt_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3657 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/misc_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2471 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/parentlist_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    59785 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/populator_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    15050 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/size_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3212 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/tags_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1807 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/task_tests.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1881 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/tsort_test.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.494378 blivet-3.7.1/tests/unit_tests/udev_data/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/udev_data/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    37564 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/udev_data/raid_data.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     5451 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/udev_test.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    10179 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/unit_tests/util_test.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.494378 blivet-3.7.1/tests/vmtests/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2090 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/vmtests/README.rst
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/vmtests/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11651 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/vmtests/blivet_reset_vmtest.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6242 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/vmtests/gpt_test.py
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)     9212 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/vmtests/runvmtests.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2842 2023-03-16 09:40:21.000000 blivet-3.7.1/tests/vmtests/vmbackedtestcase.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.495378 blivet-3.7.1/translation-canary/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       52 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/.gitignore
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    26530 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/COPYING
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      296 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/Makefile
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1764 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/README.rst
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.431376 blivet-3.7.1/translation-canary/tests/
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.495378 blivet-3.7.1/translation-canary/tests/project-tests/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      264 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/tests/project-tests/project_list.txt
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)     1671 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/tests/project-tests/test_projects.sh
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.495378 blivet-3.7.1/translation-canary/tests/pylint/
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)      478 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/tests/pylint/runpylint.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.495378 blivet-3.7.1/translation-canary/tests/unittests/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3737 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/tests/unittests/test_translatable.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    11733 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/tests/unittests/test_translated.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.495378 blivet-3.7.1/translation-canary/translation_canary/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/translation_canary/__init__.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.495378 blivet-3.7.1/translation-canary/translation_canary/translatable/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2925 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/translation_canary/translatable/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1306 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/translation_canary/translatable/__main__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1424 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/translation_canary/translatable/test_comment.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1817 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/translation_canary/translatable/test_markup.py
-drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-03-16 09:57:06.496378 blivet-3.7.1/translation-canary/translation_canary/translated/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     6144 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/translation_canary/translated/__init__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1858 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/translation_canary/translated/__main__.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3126 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/translation_canary/translated/test_markup.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1702 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/translation_canary/translated/test_percentage.py
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     2043 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/translation_canary/translated/test_usability.py
--rwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)     2098 2023-03-16 09:40:21.000000 blivet-3.7.1/translation-canary/xgettext_werror.sh
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.379422 blivet-3.8.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.304422 blivet-3.8.0/.github/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.325422 blivet-3.8.0/.github/workflows/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1700 2023-06-29 11:33:16.000000 blivet-3.8.0/.github/workflows/anaconda_tests.yml
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1426 2023-06-29 11:33:16.000000 blivet-3.8.0/.github/workflows/check.yml
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      394 2023-06-29 11:33:16.000000 blivet-3.8.0/.gitignore
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       90 2023-06-29 11:33:16.000000 blivet-3.8.0/.gitmodules
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1256 2023-06-29 11:33:16.000000 blivet-3.8.0/.packit.yaml
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4643 2023-06-29 11:33:16.000000 blivet-3.8.0/CONTRIBUTING
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    18092 2023-06-29 11:33:16.000000 blivet-3.8.0/COPYING
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    26530 2023-06-29 11:33:16.000000 blivet-3.8.0/COPYING.LESSER
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)  1255003 2023-06-29 10:53:01.000000 blivet-3.8.0/ChangeLog
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      160 2023-06-29 11:33:16.000000 blivet-3.8.0/MANIFEST.in
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7503 2023-06-29 11:33:16.000000 blivet-3.8.0/Makefile
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3876 2023-06-29 11:33:28.379422 blivet-3.8.0/PKG-INFO
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3289 2023-06-29 11:33:16.000000 blivet-3.8.0/README.md
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      869 2023-06-29 11:33:16.000000 blivet-3.8.0/TODO
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.327422 blivet-3.8.0/blivet/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4964 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12559 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/actionlist.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11283 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/arch.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    50041 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/blivet.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9454 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/callbacks.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.328422 blivet-3.8.0/blivet/dbus/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1014 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/dbus/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1982 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/dbus/action.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10041 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/dbus/blivet.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1732 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/dbus/constants.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3154 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/dbus/device.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2451 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/dbus/format.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2971 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/dbus/manager.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4749 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/dbus/object.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    43725 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/deviceaction.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    88252 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicefactory.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.328422 blivet-3.8.0/blivet/devicelibs/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicelibs/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1429 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicelibs/btrfs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4838 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicelibs/crypto.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3521 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicelibs/disk.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    32101 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicelibs/edd.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12465 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicelibs/gpt.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8772 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicelibs/lvm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1576 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicelibs/mdraid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    24513 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicelibs/raid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10243 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicelibs/stratis.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.330422 blivet-3.8.0/blivet/devices/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2086 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    26509 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/btrfs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3726 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/cache.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7637 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/container.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12651 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/device.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    26971 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/disk.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10406 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/dm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5288 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/file.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6636 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/lib.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4744 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/loop.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10031 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/luks.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)   123806 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/lvm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    30571 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/md.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2087 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/network.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3032 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/nfs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3743 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/nodev.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2849 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/optical.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    40790 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/partition.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4820 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/raid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    32913 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/storage.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9597 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devices/stratis.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    41311 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/devicetree.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6730 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/errors.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.330422 blivet-3.8.0/blivet/events/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/events/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4285 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/events/changes.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11201 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/events/handler.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11428 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/events/manager.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7798 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/fcoe.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3931 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/flags.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.331422 blivet-3.8.0/blivet/formats/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    25335 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2225 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/biosboot.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    22796 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/disklabel.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2298 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/dmraid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    51034 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/fs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1699 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/fslib.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    22583 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/luks.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9223 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/lvmpv.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3930 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/mdraid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2903 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/multipath.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3619 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/prepboot.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5192 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/stratis.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8736 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/formats/swap.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2436 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/i18n.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    22494 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/iscsi.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6935 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/mounts.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2367 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/nvme.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    85044 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/partitioning.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.331422 blivet-3.8.0/blivet/populator/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       38 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/__init__.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.332422 blivet-3.8.0/blivet/populator/helpers/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2589 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2712 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/boot.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4453 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/btrfs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2082 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/devicepopulator.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11765 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/disk.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6362 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/disklabel.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2524 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/dm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4241 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/formatpopulator.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2657 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/loop.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7430 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/luks.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    19936 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/lvm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8678 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/mdraid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2566 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/multipath.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2064 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/optical.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4269 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/partition.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2869 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/populatorhelper.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7591 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/helpers/stratis.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    21471 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/populator/populator.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8267 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/safe_dbus.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7154 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/size.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.333422 blivet-3.8.0/blivet/static_data/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      188 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/static_data/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3523 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/static_data/luks_data.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4047 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/static_data/lvm_info.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2431 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/static_data/mpath_info.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5347 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/static_data/nvdimm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10260 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/static_data/stratis_info.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2687 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/storage_log.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.334422 blivet-3.8.0/blivet/tasks/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    22255 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/availability.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1598 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/dfresize.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5413 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fsck.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3085 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fsinfo.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3202 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fslabeling.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5790 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fsminsize.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10741 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fsmkfs.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6136 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fsmount.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3723 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fsreadlabel.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6128 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fsresize.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4838 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fssize.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2961 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fssync.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1784 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fstask.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2143 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fsuuid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3362 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fswritelabel.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1949 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/fswriteuuid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3695 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/lukstasks.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2885 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/pvtask.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3333 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tasks/task.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3751 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/threads.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3459 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/tsort.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    34946 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/udev.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    36755 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/util.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    20888 2023-06-29 11:33:16.000000 blivet-3.8.0/blivet/zfcp.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.327422 blivet-3.8.0/blivet.egg-info/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3876 2023-06-29 11:33:28.000000 blivet-3.8.0/blivet.egg-info/PKG-INFO
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    69998 2023-06-29 11:33:28.000000 blivet-3.8.0/blivet.egg-info/SOURCES.txt
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        1 2023-06-29 11:33:28.000000 blivet-3.8.0/blivet.egg-info/dependency_links.txt
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:28.000000 blivet-3.8.0/blivet.egg-info/requires.txt
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        7 2023-06-29 11:33:28.000000 blivet-3.8.0/blivet.egg-info/top_level.txt
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.334422 blivet-3.8.0/dbus/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      400 2023-06-29 11:33:16.000000 blivet-3.8.0/dbus/blivet.conf
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      113 2023-06-29 11:33:16.000000 blivet-3.8.0/dbus/blivet.service
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)      364 2023-06-29 11:33:16.000000 blivet-3.8.0/dbus/blivetd
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      106 2023-06-29 11:33:16.000000 blivet-3.8.0/dbus/com.redhat.Blivet0.service
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.335422 blivet-3.8.0/doc/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5612 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/Makefile
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1023 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/_inheritance.rst
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.335422 blivet-3.8.0/doc/api/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11681 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/api/blivet.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8591 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/api/devices.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      423 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/api/events.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7034 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/api/formats.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1998 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/api.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9447 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/conf.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4814 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/dbus.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      545 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/index.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7908 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/intro.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3953 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/lvmvdo.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       34 2023-06-29 11:33:16.000000 blivet-3.8.0/doc/testing.rst
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.336422 blivet-3.8.0/examples/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2089 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/actions.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      825 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/dbus_client.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1560 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/factory.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      205 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/list_devices.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2174 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/lvm.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1996 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/lvm_cache.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1778 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/lvm_cachepool.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2168 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/lvm_non_linear.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1417 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/lvm_thin.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2167 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/lvm_vdo.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2884 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/partitioning.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1816 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/stratis.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      526 2023-06-29 11:33:16.000000 blivet-3.8.0/examples/uevents.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.336422 blivet-3.8.0/misc/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3050 2023-06-29 11:33:16.000000 blivet-3.8.0/misc/Vagrantfile
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5204 2023-06-29 11:33:16.000000 blivet-3.8.0/misc/install-test-dependencies.yml
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.347422 blivet-3.8.0/po/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1262 2023-06-29 10:38:06.000000 blivet-3.8.0/po/Makefile
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      944 2023-06-29 11:33:27.000000 blivet-3.8.0/po/af.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9722 2023-06-29 10:38:06.000000 blivet-3.8.0/po/af.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1059 2023-06-29 11:33:27.000000 blivet-3.8.0/po/am.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9831 2023-06-29 10:38:06.000000 blivet-3.8.0/po/am.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1169 2023-06-29 11:33:27.000000 blivet-3.8.0/po/ar.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10348 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ar.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9162 2023-06-29 11:33:27.000000 blivet-3.8.0/po/as.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15098 2023-06-29 10:38:06.000000 blivet-3.8.0/po/as.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3660 2023-06-29 11:33:27.000000 blivet-3.8.0/po/ast.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11161 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ast.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8312 2023-06-29 11:33:27.000000 blivet-3.8.0/po/bg.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14404 2023-06-29 10:38:06.000000 blivet-3.8.0/po/bg.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9366 2023-06-29 10:38:06.000000 blivet-3.8.0/po/blivet.pot
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5487 2023-06-29 11:33:27.000000 blivet-3.8.0/po/bn.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13553 2023-06-29 10:38:06.000000 blivet-3.8.0/po/bn.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14554 2023-06-29 11:33:27.000000 blivet-3.8.0/po/bn_IN.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    19308 2023-06-29 10:38:06.000000 blivet-3.8.0/po/bn_IN.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      939 2023-06-29 11:33:27.000000 blivet-3.8.0/po/bs.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9798 2023-06-29 10:38:06.000000 blivet-3.8.0/po/bs.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9507 2023-06-29 11:33:27.000000 blivet-3.8.0/po/ca.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14442 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ca.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10594 2023-06-29 11:33:27.000000 blivet-3.8.0/po/cs.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14662 2023-06-29 10:48:27.000000 blivet-3.8.0/po/cs.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      943 2023-06-29 11:33:27.000000 blivet-3.8.0/po/cy.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9775 2023-06-29 10:38:06.000000 blivet-3.8.0/po/cy.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9554 2023-06-29 11:33:27.000000 blivet-3.8.0/po/da.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14077 2023-06-29 10:38:06.000000 blivet-3.8.0/po/da.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10456 2023-06-29 11:33:27.000000 blivet-3.8.0/po/de.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15434 2023-06-29 10:38:06.000000 blivet-3.8.0/po/de.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1239 2023-06-29 11:33:27.000000 blivet-3.8.0/po/de_CH.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10347 2023-06-29 10:38:06.000000 blivet-3.8.0/po/de_CH.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1377 2023-06-29 11:33:27.000000 blivet-3.8.0/po/el.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10406 2023-06-29 10:38:06.000000 blivet-3.8.0/po/el.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3591 2023-06-29 11:33:27.000000 blivet-3.8.0/po/en_GB.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11196 2023-06-29 10:38:06.000000 blivet-3.8.0/po/en_GB.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10416 2023-06-29 11:33:27.000000 blivet-3.8.0/po/es.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15603 2023-06-29 10:38:06.000000 blivet-3.8.0/po/es.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1280 2023-06-29 11:33:27.000000 blivet-3.8.0/po/et.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9997 2023-06-29 10:38:06.000000 blivet-3.8.0/po/et.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      620 2023-06-29 11:33:27.000000 blivet-3.8.0/po/eu.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9639 2023-06-29 10:38:06.000000 blivet-3.8.0/po/eu.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7338 2023-06-29 11:33:27.000000 blivet-3.8.0/po/fa.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13823 2023-06-29 10:38:06.000000 blivet-3.8.0/po/fa.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10323 2023-06-29 11:33:27.000000 blivet-3.8.0/po/fi.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14226 2023-06-29 10:38:06.000000 blivet-3.8.0/po/fi.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10981 2023-06-29 11:33:27.000000 blivet-3.8.0/po/fr.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15783 2023-06-29 10:38:06.000000 blivet-3.8.0/po/fr.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10674 2023-06-29 11:33:27.000000 blivet-3.8.0/po/fur.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14142 2023-06-29 10:38:06.000000 blivet-3.8.0/po/fur.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8423 2023-06-29 11:33:27.000000 blivet-3.8.0/po/gu.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14666 2023-06-29 10:38:06.000000 blivet-3.8.0/po/gu.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1216 2023-06-29 11:33:27.000000 blivet-3.8.0/po/he.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9914 2023-06-29 10:38:06.000000 blivet-3.8.0/po/he.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4840 2023-06-29 11:33:27.000000 blivet-3.8.0/po/hi.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12552 2023-06-29 10:38:06.000000 blivet-3.8.0/po/hi.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10464 2023-06-29 11:33:27.000000 blivet-3.8.0/po/hr.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14021 2023-06-29 10:38:06.000000 blivet-3.8.0/po/hr.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10051 2023-06-29 11:33:27.000000 blivet-3.8.0/po/hu.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15026 2023-06-29 10:48:27.000000 blivet-3.8.0/po/hu.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5160 2023-06-29 11:33:27.000000 blivet-3.8.0/po/ia.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11904 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ia.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10366 2023-06-29 11:33:27.000000 blivet-3.8.0/po/id.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14243 2023-06-29 10:38:06.000000 blivet-3.8.0/po/id.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      945 2023-06-29 11:33:27.000000 blivet-3.8.0/po/ilo.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9726 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ilo.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1053 2023-06-29 11:33:27.000000 blivet-3.8.0/po/is.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9763 2023-06-29 10:38:06.000000 blivet-3.8.0/po/is.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9517 2023-06-29 11:33:27.000000 blivet-3.8.0/po/it.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14933 2023-06-29 10:38:06.000000 blivet-3.8.0/po/it.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11782 2023-06-29 11:33:27.000000 blivet-3.8.0/po/ja.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    16274 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ja.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11912 2023-06-29 11:33:27.000000 blivet-3.8.0/po/ka.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    16727 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ka.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12917 2023-06-29 11:33:27.000000 blivet-3.8.0/po/kk.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    16397 2023-06-29 10:38:06.000000 blivet-3.8.0/po/kk.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9449 2023-06-29 11:33:27.000000 blivet-3.8.0/po/kn.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15947 2023-06-29 10:38:06.000000 blivet-3.8.0/po/kn.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10960 2023-06-29 11:33:27.000000 blivet-3.8.0/po/ko.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14948 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ko.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1380 2023-06-29 11:33:27.000000 blivet-3.8.0/po/lv.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10006 2023-06-29 10:38:06.000000 blivet-3.8.0/po/lv.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1878 2023-06-29 11:33:27.000000 blivet-3.8.0/po/mai.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10481 2023-06-29 10:38:06.000000 blivet-3.8.0/po/mai.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      977 2023-06-29 11:33:27.000000 blivet-3.8.0/po/mk.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9971 2023-06-29 10:38:06.000000 blivet-3.8.0/po/mk.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8639 2023-06-29 11:33:27.000000 blivet-3.8.0/po/ml.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15344 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ml.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8864 2023-06-29 11:33:27.000000 blivet-3.8.0/po/mr.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15305 2023-06-29 10:38:06.000000 blivet-3.8.0/po/mr.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      890 2023-06-29 11:33:27.000000 blivet-3.8.0/po/ms.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9755 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ms.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9565 2023-06-29 11:33:27.000000 blivet-3.8.0/po/nb.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13988 2023-06-29 10:38:06.000000 blivet-3.8.0/po/nb.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1210 2023-06-29 11:33:27.000000 blivet-3.8.0/po/ne.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10132 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ne.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10473 2023-06-29 11:33:27.000000 blivet-3.8.0/po/nl.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14532 2023-06-29 10:48:27.000000 blivet-3.8.0/po/nl.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      935 2023-06-29 11:33:27.000000 blivet-3.8.0/po/nso.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9713 2023-06-29 10:38:06.000000 blivet-3.8.0/po/nso.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8185 2023-06-29 11:33:27.000000 blivet-3.8.0/po/or.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14855 2023-06-29 10:38:06.000000 blivet-3.8.0/po/or.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8387 2023-06-29 11:33:27.000000 blivet-3.8.0/po/pa.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14768 2023-06-29 10:38:06.000000 blivet-3.8.0/po/pa.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10862 2023-06-29 11:33:28.000000 blivet-3.8.0/po/pl.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15246 2023-06-29 10:38:06.000000 blivet-3.8.0/po/pl.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10634 2023-06-29 11:33:28.000000 blivet-3.8.0/po/pt.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14452 2023-06-29 10:48:27.000000 blivet-3.8.0/po/pt.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10764 2023-06-29 11:33:28.000000 blivet-3.8.0/po/pt_BR.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15596 2023-06-29 10:48:27.000000 blivet-3.8.0/po/pt_BR.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      951 2023-06-29 11:33:28.000000 blivet-3.8.0/po/ro.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9726 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ro.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13409 2023-06-29 11:33:28.000000 blivet-3.8.0/po/ru.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    18138 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ru.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4859 2023-06-29 11:33:28.000000 blivet-3.8.0/po/si.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12466 2023-06-29 10:38:06.000000 blivet-3.8.0/po/si.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10698 2023-06-29 11:33:28.000000 blivet-3.8.0/po/sk.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14702 2023-06-29 10:38:06.000000 blivet-3.8.0/po/sk.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      953 2023-06-29 11:33:28.000000 blivet-3.8.0/po/sl.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9987 2023-06-29 10:38:06.000000 blivet-3.8.0/po/sl.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1052 2023-06-29 11:33:28.000000 blivet-3.8.0/po/sq.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9767 2023-06-29 10:38:06.000000 blivet-3.8.0/po/sq.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9864 2023-06-29 11:33:28.000000 blivet-3.8.0/po/sr.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15052 2023-06-29 10:38:06.000000 blivet-3.8.0/po/sr.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3409 2023-06-29 11:33:28.000000 blivet-3.8.0/po/sr@latin.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11051 2023-06-29 10:38:06.000000 blivet-3.8.0/po/sr@latin.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10387 2023-06-29 11:33:28.000000 blivet-3.8.0/po/sv.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14443 2023-06-29 10:38:06.000000 blivet-3.8.0/po/sv.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8111 2023-06-29 11:33:28.000000 blivet-3.8.0/po/ta.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15091 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ta.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9153 2023-06-29 11:33:28.000000 blivet-3.8.0/po/te.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15384 2023-06-29 10:38:06.000000 blivet-3.8.0/po/te.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      769 2023-06-29 11:33:28.000000 blivet-3.8.0/po/tg.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9652 2023-06-29 10:38:06.000000 blivet-3.8.0/po/tg.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1471 2023-06-29 11:33:28.000000 blivet-3.8.0/po/th.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10233 2023-06-29 10:38:06.000000 blivet-3.8.0/po/th.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10625 2023-06-29 11:33:28.000000 blivet-3.8.0/po/tr.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14535 2023-06-29 10:38:06.000000 blivet-3.8.0/po/tr.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13478 2023-06-29 11:33:28.000000 blivet-3.8.0/po/uk.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    17502 2023-06-29 10:38:06.000000 blivet-3.8.0/po/uk.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      987 2023-06-29 11:33:28.000000 blivet-3.8.0/po/ur.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9759 2023-06-29 10:38:06.000000 blivet-3.8.0/po/ur.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9831 2023-06-29 11:33:28.000000 blivet-3.8.0/po/zh_CN.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13838 2023-06-29 10:38:06.000000 blivet-3.8.0/po/zh_CN.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8734 2023-06-29 11:33:28.000000 blivet-3.8.0/po/zh_TW.mo
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    13649 2023-06-29 10:38:06.000000 blivet-3.8.0/po/zh_TW.po
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)   202081 2023-06-29 11:33:16.000000 blivet-3.8.0/python-blivet.spec
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15715 2023-06-29 11:33:16.000000 blivet-3.8.0/release_notes.rst
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.347422 blivet-3.8.0/scripts/
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)     2905 2023-06-29 11:33:16.000000 blivet-3.8.0/scripts/docs-update
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)     1127 2023-06-29 11:33:16.000000 blivet-3.8.0/scripts/git-multi-merge
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)     1874 2023-06-29 11:33:16.000000 blivet-3.8.0/scripts/harvest-edd
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)    20059 2023-06-29 11:33:16.000000 blivet-3.8.0/scripts/makebumpver
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)     6641 2023-06-29 11:33:16.000000 blivet-3.8.0/scripts/makeupdates
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)     5460 2023-06-29 11:33:16.000000 blivet-3.8.0/scripts/pylintcodediff
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       38 2023-06-29 11:33:28.379422 blivet-3.8.0/setup.cfg
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3503 2023-06-29 11:33:16.000000 blivet-3.8.0/setup.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.347422 blivet-3.8.0/tests/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3395 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/README.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      258 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/conftest.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.348422 blivet-3.8.0/tests/pylint/
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)     6067 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/pylint/censorship.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12535 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/pylint/pylintrc
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)     4936 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/pylint/runpylint.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6862 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/run_tests.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      806 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/skip.yml
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.348422 blivet-3.8.0/tests/storage_tests/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      159 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/__init__.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.348422 blivet-3.8.0/tests/storage_tests/devices_test/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       82 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/devices_test/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    16488 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/devices_test/lvm_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    12809 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/devices_test/partition_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6518 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/devices_test/stratis_test.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.349422 blivet-3.8.0/tests/storage_tests/formats_test/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      128 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/formats_test/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9318 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/formats_test/fs_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6988 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/formats_test/fslabeling.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    14365 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/formats_test/fstesting.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4243 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/formats_test/fsuuid.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4279 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/formats_test/labeling_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5554 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/formats_test/loopbackedtestcase.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4250 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/formats_test/luks_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1419 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/formats_test/lvmpv_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4156 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/formats_test/uuid_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3538 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/imagebackedtestcase.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5414 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/iscsi_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    32748 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/partitioning_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6459 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/storagetestcase.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8425 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/storage_tests/unsupported_disklabel_test.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.350422 blivet-3.8.0/tests/unit_tests/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      476 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    67699 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/action_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11603 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/blivettestcase.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     9304 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/dbus_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    49169 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicefactory_test.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.351422 blivet-3.8.0/tests/unit_tests/devicelibs_test/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      101 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5746 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/disk_test.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.351422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sda
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdb
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdc
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdd
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sde
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/vda
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.351422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/ata_port/ata7/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/ata_port/ata7/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:0/6:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:0/6:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:0/6:0:0:0/block/sr0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:1/6:0:1:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:1/6:0:1:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/host6/target6:0:1/6:0:1:0/block/sdb/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/ata_link/link7/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.0/ata_device/dev7.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.1/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:01.1/ata7/link7/dev7.1/ata_device/dev7.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.305422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/sda/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host9/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host9/target9:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host9/target9:0:0/9:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host9/target9:0:0/9:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host9/target9:0:0/9:0:0:0/block/sdd/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:07.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/block/vda/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/host10/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/host10/target10:0:1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/host10/target10:0:1/10:0:1:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/host10/target10:0:1/10:0:1:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0a.0/host10/target10:0:1/10:0:1:0/block/sde/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/host8/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/host8/target8:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/host8/target8:0:0/8:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/host8/target8:0:0/8:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/devices/pci0000:00/0000:00:0b.0/virtio3/host8/target8:0:0/8:0:0:0/block/sdc/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.306422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.352422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        6 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       25 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       23 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        9 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev80/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.354422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       25 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       19 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        7 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev81/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.354422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       26 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        7 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev82/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.355422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        6 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       26 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        7 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev83/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.356422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        6 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       25 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       23 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        7 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev84/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.356422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        6 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       26 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        8 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/sys/firmware/edd/int13_dev85/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.357422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sda
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sdb
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sdc
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sr0
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.357422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/scsi_host/host12/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/block/sr0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/scsi_device/12:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/ata_link/link13/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/ata_device/dev13.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.307422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/ata_device/dev13.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.357422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/ata_link/link14/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/ata_device/dev14.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/ata_device/dev14.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.357422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/scsi_host/host0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/sda/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_device/0:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/0:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/ata_link/link1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.308422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/ata_device/dev1.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.357422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/ata_link/link2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/ata_device/dev2.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.358422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/ata_link/link3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/ata_device/dev3.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.358422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/ata_link/link4/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/ata_device/dev4.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.358422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/ata_link/link5/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.309422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/ata_device/dev5.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.358422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/ata_link/link6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/ata_device/dev6.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.358422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/scsi_host/host9/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/block/sdb/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_device/9:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_disk/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_disk/9:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/ata_link/link10/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/ata_device/dev10.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.358422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.310422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/scsi_host/host10/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/block/sdc/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/scsi_device/10:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/scsi_disk/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/host10/target10:0:0/10:0:0:0/scsi_disk/10:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/ata_link/link11/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/ata_device/dev11.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.359422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/ata_link/link12/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/ata_device/dev12.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.359422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/ata_link/link7/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/ata_device/dev7.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.311422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.359422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/ata_link/link8/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/ata_device/dev8.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.359422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/ata_link/link9/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/ata_device/dev9.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.360422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        6 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       26 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        9 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev80/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.361422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       26 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        7 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev81/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.362422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       26 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        7 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/sys/firmware/edd/int13_dev82/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.362422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sda
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sdb
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sdc
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sr0
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/vda
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.362422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/ata_port/ata13/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/scsi_host/host12/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.312422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/block/sr0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/host12/target12:0:0/12:0:0:0/scsi_device/12:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/ata_link/link13/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.0/ata_device/dev13.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata13/link13/dev13.1/ata_device/dev13.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.362422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/ata_port/ata14/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/ata_link/link14/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.0/ata_device/dev14.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:01.1/ata14/link14/dev14.1/ata_device/dev14.1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.362422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/ata_port/ata1/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/scsi_host/host0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.313422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/block/sda/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_device/0:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/0:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/ata_link/link1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata1/link1/dev1.0/ata_device/dev1.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.363422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/ata_port/ata2/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/ata_link/link2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata2/link2/dev2.0/ata_device/dev2.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.363422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/ata_port/ata3/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/ata_link/link3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata3/link3/dev3.0/ata_device/dev3.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.363422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/ata_port/ata4/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.314422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/ata_link/link4/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata4/link4/dev4.0/ata_device/dev4.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.363422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/ata_port/ata5/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/ata_link/link5/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata5/link5/dev5.0/ata_device/dev5.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.363422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/ata_port/ata6/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/ata_link/link6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:03.0/ata6/link6/dev6.0/ata_device/dev6.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/scsi_host/host14/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/block/sdc/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/scsi_device/14:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/scsi_disk/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.315422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:06.7/usb1/1-1/1-1:1.0/host14/target14:0:0/14:0:0:0/scsi_disk/14:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:07.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:07.0/virtio1/block/vda/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.363422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/ata_port/ata10/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/scsi_host/host9/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/block/sdb/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_device/9:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_disk/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/host9/target9:0:0/9:0:0:0/scsi_disk/9:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/ata_link/link10/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata10/link10/dev10.0/ata_device/dev10.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.364422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/ata_port/ata11/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/ata_link/link11/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata11/link11/dev11.0/ata_device/dev11.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.316422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.364422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/ata_port/ata12/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/ata_link/link12/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata12/link12/dev12.0/ata_device/dev12.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.364422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/ata_port/ata7/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/ata_link/link7/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata7/link7/dev7.0/ata_device/dev7.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.364422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/ata_port/ata8/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/ata_link/link8/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata8/link8/dev8.0/ata_device/dev8.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.364422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/ata_port/ata9/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/ata_link/link9/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.317422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/devices/pci0000:00/0000:00:0c.0/ata9/link9/dev9.0/ata_device/dev9.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.365422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        6 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       27 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       41 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        9 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev80/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.366422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       27 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       19 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        7 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev81/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.367422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       27 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       19 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        7 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev82/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.368422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/sys/firmware/edd/int13_dev83/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.368422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/dev/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/dev/sda
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/dev/sdb
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/block/sdb/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.318422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.368422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/ata2/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/ata2/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/block/sda/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/ata_device/dev2.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.369422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        6 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       46 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       27 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       19 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4096 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       10 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.370422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       46 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       29 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       33 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4096 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        9 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.370422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sda
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sdb
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sdc
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      512 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sdd
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sr0
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/scsi_host/host6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/block/sdd/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/scsi_device/6:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/scsi_disk/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.319422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1d.0/usb4/4-1/4-1.2/4-1.2:1.0/host6/target6:0:0/6:0:0:0/scsi_disk/6:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.370422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/ata_port/ata1/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/ata_port/ata1/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/ata_port/ata1/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/scsi_host/host0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/block/sda/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/scsi_device/0:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/host0/target0:0:0/0:0:0:0/scsi_disk/0:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/ata_link/link1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/dev1.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/dev1.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata1/link1/dev1.0/ata_device/dev1.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.371422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/ata2/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/ata2/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/ata_port/ata2/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/scsi_host/host1/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/block/sdb/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.320422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/scsi_device/1:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/scsi_disk/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/host1/target1:0:0/1:0:0:0/scsi_disk/1:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/ata_link/link2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata2/link2/dev2.0/ata_device/dev2.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.371422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/ata_port/ata3/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/ata_port/ata3/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/ata_port/ata3/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/scsi_host/host2/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/block/sdc/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/scsi_device/2:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/scsi_disk/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/host2/target2:0:0/2:0:0:0/scsi_disk/2:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/ata_link/link3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/dev3.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/dev3.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata3/link3/dev3.0/ata_device/dev3.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.371422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/ata_port/ata4/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/ata_port/ata4/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/ata_port/ata4/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/scsi_host/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.321422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/scsi_host/host3/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/3:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/3:0:0:0/block/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/3:0:0:0/block/sr0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/3:0:0:0/scsi_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/host3/target3:0:0/3:0:0:0/scsi_device/3:0:0:0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/ata_link/link4/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/dev4.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/dev4.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata4/link4/dev4.0/ata_device/dev4.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.371422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/ata_port/ata5/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/ata_port/ata5/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/ata_port/ata5/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/ata_link/link5/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/dev5.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/dev5.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata5/link5/dev5.0/ata_device/dev5.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/ata_port/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.371422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/ata_port/ata6/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/ata_port/ata6/nr_pmp_links
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        2 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/ata_port/ata6/port_no
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/ata_link/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/ata_link/link6/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/dev6.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/dev6.0/ata_device/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/devices/pci0000:00/0000:00:1f.2/ata6/link6/dev6.0/ata_device/dev6.0/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.322422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.323422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.372422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       46 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       29 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       33 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        9 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev80/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.373422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        6 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       46 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       27 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       19 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       10 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev81/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.374422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        6 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       46 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       27 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       19 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       10 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev82/version
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.375422 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        6 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/default_cylinders
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/default_heads
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/default_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       46 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/extensions
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       27 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/host_bus
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       15 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/info_flags
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       19 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/interface
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/legacy_max_cylinder
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        4 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/legacy_max_head
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        3 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/legacy_sectors_per_track
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       11 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/mbr_signature
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       74 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/raw_data
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       10 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/sectors
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        5 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/sys/firmware/edd/int13_dev83/version
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    41491 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1324 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/lib.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      644 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/mdraid_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     7083 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicelibs_test/raid_test.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.376422 blivet-3.8.0/tests/unit_tests/devices_test/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      372 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11726 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/device_dependencies_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    16531 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/device_methods_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3287 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/device_names_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1024 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/device_packages_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    43458 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/device_properties_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3823 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/device_size_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2442 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/disk_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    54675 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/lvm_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3861 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/md_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2184 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/network_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6542 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/partition_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     4659 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devices_test/stratis_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    23110 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/devicetree_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2825 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/events_test.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.377422 blivet-3.8.0/tests/unit_tests/formats_tests/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      239 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/formats_tests/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3185 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/formats_tests/device_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     8153 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/formats_tests/disklabel_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1466 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/formats_tests/init_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5040 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/formats_tests/luks_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2348 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/formats_tests/lvmpv_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    18083 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/formats_tests/methods_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      962 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/formats_tests/misc_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2266 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/formats_tests/selinux_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      656 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/formats_tests/swap_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3221 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/gpt_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3657 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/misc_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2471 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/parentlist_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    59822 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/populator_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    15050 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/size_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3212 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/tags_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1807 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/task_tests.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1881 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/tsort_test.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.377422 blivet-3.8.0/tests/unit_tests/udev_data/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/udev_data/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    37564 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/udev_data/raid_data.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     5451 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/udev_test.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    10179 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/unit_tests/util_test.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.377422 blivet-3.8.0/tests/vmtests/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2090 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/vmtests/README.rst
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/vmtests/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11651 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/vmtests/blivet_reset_vmtest.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6242 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/vmtests/gpt_test.py
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)     9212 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/vmtests/runvmtests.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2842 2023-06-29 11:33:16.000000 blivet-3.8.0/tests/vmtests/vmbackedtestcase.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.378422 blivet-3.8.0/translation-canary/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)       52 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/.gitignore
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    26530 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/COPYING
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      296 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/Makefile
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1764 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/README.rst
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.323422 blivet-3.8.0/translation-canary/tests/
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.378422 blivet-3.8.0/translation-canary/tests/project-tests/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)      264 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/tests/project-tests/project_list.txt
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)     1671 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/tests/project-tests/test_projects.sh
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.378422 blivet-3.8.0/translation-canary/tests/pylint/
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)      478 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/tests/pylint/runpylint.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.378422 blivet-3.8.0/translation-canary/tests/unittests/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3737 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/tests/unittests/test_translatable.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)    11733 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/tests/unittests/test_translated.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.378422 blivet-3.8.0/translation-canary/translation_canary/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/translation_canary/__init__.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.378422 blivet-3.8.0/translation-canary/translation_canary/translatable/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2925 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/translation_canary/translatable/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1306 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/translation_canary/translatable/__main__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1424 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/translation_canary/translatable/test_comment.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1817 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/translation_canary/translatable/test_markup.py
+drwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)        0 2023-06-29 11:33:28.378422 blivet-3.8.0/translation-canary/translation_canary/translated/
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     6144 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/translation_canary/translated/__init__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1858 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/translation_canary/translated/__main__.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     3126 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/translation_canary/translated/test_markup.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     1702 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/translation_canary/translated/test_percentage.py
+-rw-r--r--   0 vtrefny   (1000) vtrefny   (1000)     2043 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/translation_canary/translated/test_usability.py
+-rwxr-xr-x   0 vtrefny   (1000) vtrefny   (1000)     2098 2023-06-29 11:33:16.000000 blivet-3.8.0/translation-canary/xgettext_werror.sh
```

### Comparing `blivet-3.7.1/.github/workflows/anaconda_tests.yml` & `blivet-3.8.0/.github/workflows/anaconda_tests.yml`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/CONTRIBUTING` & `blivet-3.8.0/CONTRIBUTING`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/COPYING` & `blivet-3.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/COPYING.LESSER` & `blivet-3.8.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/Makefile` & `blivet-3.8.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-PYTHON?=python3
+PYTHON=python3
 PKG_INSTALL?=dnf
 
 L10N_REPOSITORY=git@github.com:storaged-project/blivet-weblate.git
 L10N_BRANCH=master
 
 PKGNAME=blivet
 SPECFILE=python-blivet.spec
```

### Comparing `blivet-3.7.1/PKG-INFO` & `blivet-3.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: blivet
-Version: 3.7.1
+Version: 3.8.0
 Summary: Python module for system storage configuration
 Home-page: http://github.com/storaged-project/blivet
 Author: David Lehman
 Author-email: dlehman@redhat.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 
 Blivet is a python module for system storage configuration.
```

### Comparing `blivet-3.7.1/README.md` & `blivet-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/TODO` & `blivet-3.8.0/TODO`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/__init__.py` & `blivet-3.8.0/blivet/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # License and may only be used or replicated with the express permission of
 # Red Hat, Inc.
 #
 # Red Hat Author(s): Dave Lehman <dlehman@redhat.com>
 #                    Vratislav Podzimek <vpodzime@redhat.com>
 #
 
-__version__ = '3.7.1'
+__version__ = '3.8.0'
 
 import sys
 import importlib
 import warnings
 import syslog
 
 from . import util, arch
@@ -53,15 +53,15 @@
     # from cryptsetup and we don't want to put these into program.log
     if level <= syslog.LOG_INFO and level in LOG_LEVELS.keys():
         program_log.log(LOG_LEVELS[level], msg)
 
 
 import gi
 gi.require_version("GLib", "2.0")
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 # initialize the libblockdev library
 from gi.repository import GLib
 from gi.repository import BlockDev as blockdev
 if arch.is_s390():
     _REQUESTED_PLUGIN_NAMES = set(("lvm", "btrfs", "swap", "crypto", "loop", "mdraid", "mpath", "dm", "s390", "nvdimm"))
 else:
@@ -69,17 +69,14 @@
 
 # nvme plugin is not generally available
 if hasattr(blockdev.Plugin, "NVME"):
     _REQUESTED_PLUGIN_NAMES.add("nvme")
 
 _requested_plugins = blockdev.plugin_specs_from_names(_REQUESTED_PLUGIN_NAMES)
 try:
-    # do not check for dependencies during libblockdev initialization, do runtime
-    # checks instead
-    blockdev.switch_init_checks(False)
     succ_, avail_plugs = blockdev.try_reinit(require_plugins=_requested_plugins, reload=False, log_func=log_bd_message)
 except GLib.GError as err:
     raise RuntimeError("Failed to initialize the libblockdev library: %s" % err)
 else:
     avail_plugs = set(avail_plugs)
 
 missing_plugs = _REQUESTED_PLUGIN_NAMES - avail_plugs
```

### Comparing `blivet-3.7.1/blivet/actionlist.py` & `blivet-3.8.0/blivet/actionlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,19 +144,21 @@
                 continue
 
             for obsolete in self._actions[:]:
                 if action.obsoletes(obsolete):
                     log.info("removing obsolete action %d (%d)",
                              obsolete.id, action.id)
                     self._actions.remove(obsolete)
+                    _callbacks.action_removed(action=obsolete)
 
                     if obsolete.obsoletes(action) and action in self._actions:
                         log.info("removing mutually-obsolete action %d (%d)",
                                  action.id, obsolete.id)
                         self._actions.remove(action)
+                        _callbacks.action_removed(action=action)
 
     def sort(self):
         """ Sort actions based on dependencies. """
         if not self._actions:
             return
 
         edges = []
```

### Comparing `blivet-3.7.1/blivet/arch.py` & `blivet-3.8.0/blivet/arch.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,14 +345,23 @@
     :return: True if the hardware supports ARM, False otherwise.
     :rtype: boolean
 
     """
     return os.uname()[4].startswith('arm')
 
 
+def is_riscv64():
+    """
+    :return: True if the hardware supports RISCV64, False otherwise.
+    :rtype: boolean
+
+    """
+    return os.uname()[4] == 'riscv64'
+
+
 def is_loongarch(bits=None):
     """
     :return: True if the hardware supports loongarch, False otherwise.
     :rtype: boolean
     :param bits: The number of bits used to define a memory address.
     :type bits: int
 
@@ -401,14 +410,16 @@
         return os.uname()[4]
     elif is_aarch64():
         return 'aarch64'
     elif is_alpha():
         return 'alpha'
     elif is_arm():
         return 'arm'
+    elif is_riscv64():
+        return 'riscv64'
     elif is_loongarch(bits=32):
         return 'loongarch32'
     elif is_loongarch(bits=64):
         return 'loongarch64'
     else:
         return os.uname()[4]
```

### Comparing `blivet-3.7.1/blivet/blivet.py` & `blivet-3.8.0/blivet/blivet.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/callbacks.py` & `blivet-3.8.0/blivet/callbacks.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/dbus/__init__.py` & `blivet-3.8.0/blivet/dbus/__init__.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/dbus/action.py` & `blivet-3.8.0/blivet/dbus/action.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/dbus/blivet.py` & `blivet-3.8.0/blivet/dbus/blivet.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 
 class DBusBlivet(DBusObject):
     """ This class provides the main entry point to the Blivet1 service.
 
         It provides methods for controlling the blivet service and querying its
         state.
     """
+    transient = False
+
     def __init__(self, manager):
         super(DBusBlivet, self).__init__(manager)
         self._blivet = Blivet()
         self._id = ObjectID().id
         self._manager.add_object(self)
         self._set_up_callbacks()
 
@@ -137,20 +139,14 @@
         self._manager.remove_object(removed)
 
     def _action_added(self, action):
         added = DBusAction(action, self._manager)
         self._manager.add_object(added)
 
     def _action_executed(self, action):
-        if action.is_destroy:
-            if action.is_device:
-                self._device_removed(action.device, keep=False)
-            elif action.is_format:
-                self._format_removed(action.device, action.format, keep=False)
-
         self._action_removed(action)
 
     def _list_dbus_devices(self, removed=False):
         dbus_devices = (d for d in self._manager.objects if isinstance(d, DBusDevice))
         return [d for d in dbus_devices if removed or d.present]
 
     def _get_device_by_object_path(self, object_path, removed=False):
@@ -167,20 +163,17 @@
                                                 'removed.' % object_path)
 
         return dbus_device._device
 
     @dbus.service.method(dbus_interface=BLIVET_INTERFACE)
     def Reset(self):
         """ Reset the Blivet instance and populate the device tree. """
-        old_devices = self._blivet.devices[:]
-        for removed in old_devices:
-            self._device_removed(device=removed, keep=False)
-
-        for action in self._blivet.devicetree.actions:
-            self._action_removed(action)
+        for obj in self._manager.objects:
+            if obj.transient:
+                self._manager.remove_object(obj)
 
         self._blivet.reset()
 
     @dbus.service.method(dbus_interface=BLIVET_INTERFACE)
     def Exit(self):
         """ Stop the blivet service. """
         sys.exit(0)
```

### Comparing `blivet-3.7.1/blivet/dbus/constants.py` & `blivet-3.8.0/blivet/dbus/constants.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/dbus/device.py` & `blivet-3.8.0/blivet/dbus/device.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/dbus/format.py` & `blivet-3.8.0/blivet/dbus/format.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/dbus/manager.py` & `blivet-3.8.0/blivet/dbus/manager.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/dbus/object.py` & `blivet-3.8.0/blivet/dbus/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 import dbus.service
 
 from .constants import BUS_NAME
 
 
 class DBusObject(dbus.service.Object):
     """ Base class for dbus objects. """
+    transient = True  # should this be removed on Blivet.Reset ?
+
     def __init__(self, manager):
         # pylint: disable=super-init-not-called
         self._present = True
         self._init_dbus_object()
         self._manager = manager  # provides ObjectManager interface
 
     # This is here to make it easier to prevent the dbus.service.Object
```

### Comparing `blivet-3.7.1/blivet/deviceaction.py` & `blivet-3.8.0/blivet/deviceaction.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devicefactory.py` & `blivet-3.8.0/blivet/devicefactory.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from .partitioning import SameSizeSet
 from .partitioning import TotalSizeSet
 from .partitioning import do_partitioning
 from .size import Size
 from .static_data import luks_data
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import logging
 log = logging.getLogger("blivet")
 
 # policy value of >0 is a fixed size request
```

### Comparing `blivet-3.7.1/blivet/devicelibs/btrfs.py` & `blivet-3.8.0/blivet/devicelibs/btrfs.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devicelibs/crypto.py` & `blivet-3.8.0/blivet/devicelibs/crypto.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Author(s): Dave Lehman <dlehman@redhat.com>
 #            Martin Sivak <msivak@redhat.com>
 #
 
 import hashlib
+import os
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev
 
 from ..size import Size, ROUND_DOWN
 from ..tasks import availability
 from ..util import total_memory, available_memory, run_program_and_capture_output
 
@@ -128,7 +129,17 @@
         return 0
     else:
         # XXX when logical and physical block size differ, we don't want to let cryptsetup
         # decide because it will choose 4096 for disks with 4096 physical block size and
         # 512 logical block size which will make it harder to combine these in a single
         # LVM volume group if used as PVs
         return SECTOR_SIZE
+
+
+def is_fips_enabled():
+    if not os.path.exists("/proc/sys/crypto/fips_enabled"):
+        # if the file doesn't exist, we are definitely not in FIPS mode
+        return False
+
+    with open("/proc/sys/crypto/fips_enabled", "r") as f:
+        enabled = f.read()
+    return enabled.strip() == "1"
```

### Comparing `blivet-3.7.1/blivet/devicelibs/disk.py` & `blivet-3.8.0/blivet/devicelibs/disk.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devicelibs/edd.py` & `blivet-3.8.0/blivet/devicelibs/edd.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devicelibs/gpt.py` & `blivet-3.8.0/blivet/devicelibs/gpt.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devicelibs/lvm.py` & `blivet-3.8.0/blivet/devicelibs/lvm.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import os
 import re
 
 from collections import namedtuple
 import itertools
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import logging
 log = logging.getLogger("blivet")
 
 from . import raid
@@ -80,14 +80,17 @@
     except blockdev.LVMError:
         HAVE_LVMDEVICES = False
     else:
         HAVE_LVMDEVICES = True
 else:
     HAVE_LVMDEVICES = False
 
+
+LVM_DEVICES_FILE = "/etc/lvm/devices/system.devices"
+
 # list of devices that LVM is allowed to use
 # with LVM >= 2.0.13 we'll use this for the --devices option and when creating
 # the /etc/lvm/devices/system.devices file
 # with older versions of LVM we will use this for the --config based filtering
 _lvm_devices = set()
```

### Comparing `blivet-3.7.1/blivet/devicelibs/mdraid.py` & `blivet-3.8.0/blivet/devicelibs/mdraid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devicelibs/raid.py` & `blivet-3.8.0/blivet/devicelibs/raid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devicelibs/stratis.py` & `blivet-3.8.0/blivet/devicelibs/stratis.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/__init__.py` & `blivet-3.8.0/blivet/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/btrfs.py` & `blivet-3.8.0/blivet/devices/btrfs.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #
 
 import os
 import copy
 import tempfile
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 from ..devicelibs import btrfs
 from ..devicelibs import raid
 
 from .. import errors
@@ -451,18 +451,21 @@
             data_level = str(self.data_level)
         else:
             data_level = None
         if self.metadata_level:
             md_level = str(self.metadata_level)
         else:
             md_level = None
-        blockdev.btrfs.create_volume([d.path for d in self.parents],
-                                     label=self.format.label,
-                                     data_level=data_level,
-                                     md_level=md_level)
+        try:
+            blockdev.btrfs.create_volume([d.path for d in self.parents],
+                                         label=self.format.label,
+                                         data_level=data_level,
+                                         md_level=md_level)
+        except (blockdev.BtrfsError, blockdev.BlockDevNotImplementedError) as err:
+            raise errors.BTRFSError(err)
 
     def _post_create(self):
         super(BTRFSVolumeDevice, self)._post_create()
         info = udev.get_device(self.sysfs_path)
         if not info:
             log.error("failed to get updated udev info for new btrfs volume")
         else:
@@ -485,20 +488,26 @@
             device.setup(orig=True)
             DeviceFormat(device=device.path, exists=True).destroy()
 
     def _remove(self, member):
         log_method_call(self, self.name, status=self.status)
 
         with self._do_temp_mount() as mountpoint:
-            blockdev.btrfs.remove_device(mountpoint, member.path)
+            try:
+                blockdev.btrfs.remove_device(mountpoint, member.path)
+            except (blockdev.BtrfsError, blockdev.BlockDevNotImplementedError) as err:
+                raise errors.BTRFSError(err)
 
     def _add(self, member):
 
         with self._do_temp_mount() as mountpoint:
-            blockdev.btrfs.add_device(mountpoint, member.path)
+            try:
+                blockdev.btrfs.add_device(mountpoint, member.path)
+            except (blockdev.BtrfsError, blockdev.BlockDevNotImplementedError) as err:
+                raise errors.BTRFSError(err)
 
     def populate_ksdata(self, data):
         super(BTRFSVolumeDevice, self).populate_ksdata(data)
         data.dataLevel = self.data_level.name if self.data_level else None
         data.metaDataLevel = self.metadata_level.name if self.metadata_level else None
         data.devices = ["btrfs.%d" % p.id for p in self.parents]
         data.preexist = self.exists
@@ -586,29 +595,35 @@
         log_method_call(self, name=self.name, orig=orig)
         self.volume.setup(orig=orig)
 
     def _create(self):
         log_method_call(self, self.name, status=self.status)
 
         with self.volume._do_temp_mount() as mountpoint:
-            blockdev.btrfs.create_subvolume(mountpoint, self.name)
+            try:
+                blockdev.btrfs.create_subvolume(mountpoint, self.name)
+            except (blockdev.BtrfsError, blockdev.BlockDevNotImplementedError) as err:
+                raise errors.BTRFSError(err)
 
     def _post_create(self):
         super(BTRFSSubVolumeDevice, self)._post_create()
         self.format.vol_uuid = self.volume.format.vol_uuid
 
     def _destroy(self):
         log_method_call(self, self.name, status=self.status)
 
         with self.volume._do_temp_mount() as mountpoint:
             if self.volume._default_subvolume_id == self.vol_id:
                 # btrfs does not allow removal of the default subvolume
                 self.volume._set_default_subvolume_id(self.volume.vol_id)
 
-            blockdev.btrfs.delete_subvolume(mountpoint, self.name)
+            try:
+                blockdev.btrfs.delete_subvolume(mountpoint, self.name)
+            except (blockdev.BtrfsError, blockdev.BlockDevNotImplementedError) as err:
+                raise errors.BTRFSError(err)
 
     def remove_hook(self, modparent=True):
         if modparent:
             self.volume._remove_subvolume(self.name)
 
         super(BTRFSSubVolumeDevice, self).remove_hook(modparent=modparent)
 
@@ -690,12 +705,15 @@
             if isinstance(self.source, BTRFSVolumeDevice):
                 source_path = mountpoint
             else:
                 source_path = "%s/%s" % (mountpoint, self.source.name)
 
             dest_path = "%s/%s" % (mountpoint, self.name)
 
-            blockdev.btrfs.create_snapshot(source_path, dest_path, ro=self.read_only)
+            try:
+                blockdev.btrfs.create_snapshot(source_path, dest_path, ro=self.read_only)
+            except (blockdev.BtrfsError, blockdev.BlockDevNotImplementedError) as err:
+                raise errors.BTRFSError(err)
 
     def depends_on(self, dep):
         return (dep == self.source or
                 super(BTRFSSnapShotDevice, self).depends_on(dep))
```

### Comparing `blivet-3.7.1/blivet/devices/cache.py` & `blivet-3.8.0/blivet/devices/cache.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/container.py` & `blivet-3.8.0/blivet/devices/container.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/device.py` & `blivet-3.8.0/blivet/devices/device.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/disk.py` & `blivet-3.8.0/blivet/devices/disk.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # License and may only be used or replicated with the express permission of
 # Red Hat, Inc.
 #
 # Red Hat Author(s): David Lehman <dlehman@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 gi.require_version("GLib", "2.0")
 
 from gi.repository import BlockDev as blockdev
 from gi.repository import GLib
 
 import os
 from collections import namedtuple
```

### Comparing `blivet-3.7.1/blivet/devices/dm.py` & `blivet-3.8.0/blivet/devices/dm.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # License and may only be used or replicated with the express permission of
 # Red Hat, Inc.
 #
 # Red Hat Author(s): David Lehman <dlehman@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import os
 
 from .. import errors
 from .. import util
@@ -94,19 +94,14 @@
     @property
     def dict(self):
         d = super(DMDevice, self).dict
         d.update({"target": self.target, "dm_uuid": self.dm_uuid})
         return d
 
     @property
-    def fstab_spec(self):
-        """ Return the device specifier for use in /etc/fstab. """
-        return self.path
-
-    @property
     def map_name(self):
         """ This device's device-mapper map name """
         return self.name
 
     @property
     def status(self):
         try:
@@ -122,15 +117,20 @@
 
     def get_dm_node(self):
         """ Return the dm-X (eg: dm-0) device node for this device. """
         log_method_call(self, self.name, status=self.status)
         if not self.exists:
             raise errors.DeviceError("device has not been created")
 
-        return blockdev.dm.node_from_name(self.name)
+        try:
+            node = blockdev.dm.node_from_name(self.name)
+        except blockdev.DMError as e:
+            raise errors.DMError(e)
+        else:
+            return node
 
     def setup_partitions(self):
         log_method_call(self, name=self.name)
         rc = util.run_program(["kpartx", "-a", "-s", self.path])
         if rc:
             raise errors.DMError("partition activation failed for '%s'" % self.name)
         udev.settle()
@@ -140,15 +140,18 @@
         rc = util.run_program(["kpartx", "-d", "-s", self.path])
         if rc:
             raise errors.DMError("partition deactivation failed for '%s'" % self.name)
         udev.settle()
         for dev in os.listdir("/dev/mapper/"):
             prefix = self.name + "p"
             if dev.startswith(prefix) and dev[len(prefix):].isdigit():
-                blockdev.dm.remove(dev)
+                try:
+                    blockdev.dm.remove(dev)
+                except blockdev.DMError as e:
+                    raise errors.DMError(e)
 
     def _set_name(self, value):
         """ Set the device's map name. """
         if value == self._name:
             return
 
         log_method_call(self, self.name, status=self.status)
@@ -186,26 +189,34 @@
                           exists=exists, target="linear", dm_uuid=dm_uuid)
 
     def _setup(self, orig=False):
         """ Open, or set up, a device. """
         log_method_call(self, self.name, orig=orig, status=self.status,
                         controllable=self.controllable)
         parent_length = self.parents[0].current_size / LINUX_SECTOR_SIZE
-        blockdev.dm.create_linear(self.name, self.parents[0].path, parent_length,
-                                  self.dm_uuid)
+        try:
+            blockdev.dm.create_linear(self.name, self.parents[0].path, parent_length,
+                                      self.dm_uuid)
+        except blockdev.DMError as e:
+            raise errors.DMError(e)
 
     def _post_setup(self):
         StorageDevice._post_setup(self)
         self.setup_partitions()
         udev.settle()
 
     def _teardown(self, recursive=False):
         self.teardown_partitions()
         udev.settle()
-        blockdev.dm.remove(self.name)
+
+        try:
+            blockdev.dm.remove(self.name)
+        except blockdev.DMError as e:
+            raise errors.DMError(e)
+
         udev.settle()
 
     def deactivate(self, recursive=False):
         StorageDevice.teardown(self, recursive=recursive)
 
     def teardown(self, recursive=None):
         """ Close, or tear down, a device. """
```

### Comparing `blivet-3.7.1/blivet/devices/file.py` & `blivet-3.8.0/blivet/devices/file.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/lib.py` & `blivet-3.8.0/blivet/devices/lib.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/loop.py` & `blivet-3.8.0/blivet/devices/loop.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # License and may only be used or replicated with the express permission of
 # Red Hat, Inc.
 #
 # Red Hat Author(s): David Lehman <dlehman@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import os
 
 from .. import errors
 from ..storage_log import log_method_call
@@ -77,15 +77,19 @@
             # if the backing device is inactive, so are we
             return self.name
 
         if self.name.startswith("loop"):
             # if our name is loopN we must already be active
             return self.name
 
-        name = blockdev.loop.get_loop_name(self.parents[0].path)
+        try:
+            name = blockdev.loop.get_loop_name(self.parents[0].path)
+        except blockdev.LoopError as e:
+            raise errors.LoopError(e)
+
         if name.startswith("loop"):
             self.name = name
 
         return self.name
 
     @property
     def status(self):
@@ -102,24 +106,30 @@
             raise errors.DeviceError("specified file (%s) does not exist" % self.parents[0].path)
         return StorageDevice._pre_setup(self, orig=orig)
 
     def _setup(self, orig=False):
         """ Open, or set up, a device. """
         log_method_call(self, self.name, orig=orig, status=self.status,
                         controllable=self.controllable)
-        blockdev.loop.setup(self.parents[0].path)
+        try:
+            blockdev.loop.setup(self.parents[0].path)
+        except blockdev.LoopError as e:
+            raise errors.LoopError(e)
 
     def _post_setup(self):
         StorageDevice._post_setup(self)
         self.update_name()
         self.update_sysfs_path()
 
     def _teardown(self, recursive=False):
         """ Close, or tear down, a device. """
         log_method_call(self, self.name, status=self.status,
                         controllable=self.controllable)
-        blockdev.loop.teardown(self.path)
+        try:
+            blockdev.loop.teardown(self.path)
+        except blockdev.LoopError as e:
+            raise errors.LoopError(e)
 
     def _post_teardown(self, recursive=False):
         StorageDevice._post_teardown(self, recursive=recursive)
         self.name = "tmploop%d" % self.id
         self.sysfs_path = ''
```

### Comparing `blivet-3.7.1/blivet/devices/luks.py` & `blivet-3.8.0/blivet/devices/luks.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/lvm.py` & `blivet-3.8.0/blivet/devices/lvm.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,25 +27,26 @@
 import time
 from collections import namedtuple, defaultdict
 from functools import wraps
 from enum import Enum
 import six
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 # device backend modules
 from ..devicelibs import lvm
 
 from .. import errors
 from .. import util
 from ..storage_log import log_method_call
 from .. import udev
+from ..flags import flags
 from ..size import Size, KiB, MiB, ROUND_UP, ROUND_DOWN
 from ..static_data.lvm_info import lvs_info
 from ..tasks import availability
 
 import logging
 log = logging.getLogger("blivet")
 
@@ -243,21 +244,27 @@
             raise errors.DeviceError("cannot activate VG %s -- some of its PVs are missing" % self.name)
         return StorageDevice._pre_setup(self, orig=orig)
 
     def _teardown(self, recursive=None):
         """ Close, or tear down, a device. """
         log_method_call(self, self.name, status=self.status,
                         controllable=self.controllable)
-        blockdev.lvm.vgdeactivate(self.name)
+        try:
+            blockdev.lvm.vgdeactivate(self.name)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     def _create(self):
         """ Create the device. """
         log_method_call(self, self.name, status=self.status)
         pv_list = [pv.path for pv in self.parents]
-        blockdev.lvm.vgcreate(self.name, pv_list, self.pe_size)
+        try:
+            blockdev.lvm.vgcreate(self.name, pv_list, self.pe_size)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     def _post_create(self):
         self._complete = True
         super(LVMVolumeGroupDevice, self)._post_create()
         self.format.exists = True
 
     def _pre_destroy(self):
@@ -273,37 +280,49 @@
                 # add PVS to the list of LVM devices so we can wipe them.
                 lvm.lvm_devices_add(pv.path)
 
             # Don't run vgremove or vgreduce since there may be another VG with
             # the same name that we want to keep/use.
             return
 
-        blockdev.lvm.vgreduce(self.name, None)
-        blockdev.lvm.vgdeactivate(self.name)
-        blockdev.lvm.vgremove(self.name)
+        try:
+            blockdev.lvm.vgreduce(self.name, None)
+            blockdev.lvm.vgdeactivate(self.name)
+            blockdev.lvm.vgremove(self.name)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     def _remove(self, member):
         status = []
         for lv in self.lvs:
             status.append(lv.status)
             if lv.exists:
                 lv.setup()
 
         # do not run pvmove on empty PVs
         member.format.update_size_info()
         if member.format.free < member.format.current_size:
-            blockdev.lvm.pvmove(member.path)
-        blockdev.lvm.vgreduce(self.name, member.path)
+            try:
+                blockdev.lvm.pvmove(member.path)
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
+        try:
+            blockdev.lvm.vgreduce(self.name, member.path)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
         for (lv, status) in zip(self.lvs, status):
             if lv.status and not status:
                 lv.teardown()
 
     def _add(self, member):
-        blockdev.lvm.vgextend(self.name, member.path)
+        try:
+            blockdev.lvm.vgextend(self.name, member.path)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     def _add_log_vol(self, lv):
         """ Add an LV to this VG. """
         if lv in self._lvs:
             raise errors.DeviceError("lv is already part of this vg")
 
         # verify we have the space, then add it
@@ -403,15 +422,18 @@
             raise ValueError("device has not been created")
         if old_name == new_name:
             raise ValueError("device is already named '%s'" % old_name)
         if not lvm.is_lvm_name_valid(new_name):
             raise ValueError("'%s' is not a valid name for %s" % (new_name, self.type))
 
         if not dry_run:
-            blockdev.lvm.vgrename(old_name, new_name)
+            try:
+                blockdev.lvm.vgrename(old_name, new_name)
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
             for pv in self.pvs:
                 pv.format.vg_name = new_name
 
     # We can't rely on lvm to tell us about our size, free space, &c
     # since we could have modifications queued, unless the VG and all of
     # its PVs already exist.
     @property
@@ -655,15 +677,16 @@
 
     config_actions_map = {"name": "_rename",
                           "compression": "_set_compression",
                           "deduplication": "_set_deduplication"}
 
     def __init__(self, name, parents=None, size=None, uuid=None, seg_type=None,
                  fmt=None, exists=False, sysfs_path='', grow=None, maxsize=None,
-                 percent=None, cache_request=None, pvs=None, from_lvs=None):
+                 percent=None, cache_request=None, pvs=None, from_lvs=None,
+                 stripe_size=0):
 
         if not exists:
             if seg_type not in [None, "linear", "thin", "thin-pool", "cache", "vdo-pool", "vdo", "cache-pool"] + lvm.raid_seg_types:
                 raise ValueError("Invalid or unsupported segment type: %s" % seg_type)
             if seg_type and seg_type in lvm.raid_seg_types and not pvs:
                 raise errors.DeviceError("List of PVs has to be given for every non-linear LV")
             elif (not seg_type or seg_type == "linear") and pvs:
@@ -752,14 +775,23 @@
             missing = [r.name for r in
                        set(spec.pv for spec in self._pv_specs).difference(set(self.vg.parents))]
             msg = "invalid destination PV(s) %s for LV %s" % (missing, self.name)
             raise errors.DeviceError(msg)
         if self._pv_specs:
             self._assign_pv_space()
 
+        self._stripe_size = stripe_size
+        if not self.exists and self._stripe_size:
+            if self.seg_type not in lvm.raid_seg_types:
+                raise errors.DeviceError("Stripe size can be specified only for RAID volumes")
+            if self.seg_type in ("raid1", "RAID1", "1", 1, "mirror"):
+                raise errors.DeviceError("Specifying stripe size is not allowed for RAID1 or mirror")
+            if self.cache:
+                raise errors.DeviceError("Creating cached LVs with custom stripe size is not supported")
+
     def _assign_pv_space(self):
         if not self.is_raid_lv:
             # nothing to do for non-RAID (and thus non-striped) LVs here
             return
         for spec in self._pv_specs:
             spec.size = self.raid_level.get_base_member_size(self.size + self._metadata_size, len(self._pv_specs))
 
@@ -976,15 +1008,20 @@
 
     def get_dm_node(self):
         """ Return the dm-X (eg: dm-0) device node for this device. """
         log_method_call(self, self.name, status=self.status)
         if not self.exists:
             raise errors.DeviceError("device has not been created")
 
-        return blockdev.dm.node_from_name(self.map_name)
+        try:
+            node = blockdev.dm.node_from_name(self.map_name)
+        except blockdev.DMError as err:
+            raise errors.LVMError(err)
+        else:
+            return node
 
     def _get_name(self):
         """ This device's name. """
         if self.vg is not None:
             return "%s-%s" % (self.vg.name, self._name)
         else:
             return super(LVMLogicalVolumeBase, self)._get_name()
@@ -1051,15 +1088,18 @@
 
         return True
 
     def _teardown(self, recursive=None):
         """ Close, or tear down, a device. """
         log_method_call(self, self.name, status=self.status,
                         controllable=self.controllable)
-        blockdev.lvm.lvdeactivate(self.vg.name, self._name)
+        try:
+            blockdev.lvm.lvdeactivate(self.vg.name, self._name)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     def _post_teardown(self, recursive=False):
         try:
             # It's likely that teardown of a VG will fail due to other
             # LVs being active (filesystems mounted, &c), so don't let
             # it bring everything down.
             StorageDevice._post_teardown(self, recursive=recursive)
@@ -1096,15 +1136,18 @@
 
         if old_name == new_name:
             raise ValueError("device is already named '%s'" % old_name)
         if not lvm.is_lvm_name_valid(self.name):
             raise ValueError("'%s' is not a valid name for %s" % (new_name, self.type))
 
         if not dry_run:
-            blockdev.lvm.lvrename(self.vg.name, old_name, new_name)
+            try:
+                blockdev.lvm.lvrename(self.vg.name, old_name, new_name)
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
 
     @property
     def lvname(self):
         """ The LV's name (not including VG name). """
         return self._name
 
     @property
@@ -1479,15 +1522,19 @@
 
         try:
             self.teardown()
         except errors.FSError:
             pass
 
         udev.settle()
-        blockdev.lvm.lvsnapshotmerge(self.vg.name, self.lvname)
+
+        try:
+            blockdev.lvm.lvsnapshotmerge(self.vg.name, self.lvname)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     @util.requires_property("is_snapshot_lv")
     def _update_format_from_origin(self):
         """ Update the snapshot's format to reflect the origin's.
 
             .. note::
                 This should only be called for non-existent snapshot devices.
@@ -1532,39 +1579,48 @@
         # the old snapshot cannot be setup and torn down
         pass
 
     def _create(self):
         """ Create the device. """
         if not self.is_thin_lv:
             log_method_call(self, self.name, status=self.status)
-            blockdev.lvm.lvsnapshotcreate(self.vg.name, self.origin.lvname, self._name, self.size)
+            try:
+                blockdev.lvm.lvsnapshotcreate(self.vg.name, self.origin.lvname, self._name, self.size)
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
         else:
             pool_name = None
             if not self.origin.is_thin_lv:
                 # if the origin is not a thin volume we need to tell lvm which pool
                 # to use
                 pool_name = self.pool.lvname
 
-            blockdev.lvm.thsnapshotcreate(self.vg.name, self.origin.lvname, self._name,
-                                          pool_name=pool_name)
+            try:
+                blockdev.lvm.thsnapshotcreate(self.vg.name, self.origin.lvname, self._name,
+                                              pool_name=pool_name)
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
 
     def _post_create(self):
         DMDevice._post_create(self)
         # Snapshot's format exists as soon as the snapshot has been
         # created iff the origin's format exists
         self.format.exists = self.origin.format.exists
 
     @old_snapshot_specific
     def _destroy(self):
         """ Destroy the device. """
         log_method_call(self, self.name, status=self.status)
         # old-style snapshots' status is tied to the origin's so we never
         # explicitly activate or deactivate them and we have to tell lvremove
         # that it is okay to remove the active snapshot
-        blockdev.lvm.lvremove(self.vg.name, self._name, force=True)
+        try:
+            blockdev.lvm.lvremove(self.vg.name, self._name, force=True)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     def depends_on(self, dep):
         if self.is_thin_lv:
             if self.origin == dep and not self.exists:
                 return True
             else:
                 raise NotTypeSpecific()
@@ -1731,21 +1787,27 @@
             extra = dict()
             if profile_name:
                 extra["profile"] = profile_name
             if self.chunk_size:
                 extra["chunksize"] = str(int(self.chunk_size))
             data_lv = six.next(lv for lv in self._internal_lvs if lv.int_lv_type == LVMInternalLVtype.data)
             meta_lv = six.next(lv for lv in self._internal_lvs if lv.int_lv_type == LVMInternalLVtype.meta)
-            blockdev.lvm.thpool_convert(self.vg.name, data_lv.lvname, meta_lv.lvname, self.lvname, **extra)
+            try:
+                blockdev.lvm.thpool_convert(self.vg.name, data_lv.lvname, meta_lv.lvname, self.lvname, **extra)
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
             # TODO: update the names of the internal LVs here
         else:
-            blockdev.lvm.thpoolcreate(self.vg.name, self.lvname, self.size,
-                                      md_size=self.metadata_size,
-                                      chunk_size=self.chunk_size,
-                                      profile=profile_name)
+            try:
+                blockdev.lvm.thpoolcreate(self.vg.name, self.lvname, self.size,
+                                          md_size=self.metadata_size,
+                                          chunk_size=self.chunk_size,
+                                          profile=profile_name)
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
 
     def dracut_setup_args(self):
         return set()
 
     @property
     def direct(self):
         """ Is this device directly accessible? """
@@ -1829,16 +1891,19 @@
         # free space in a VG which doesn't make sense for a ThinLV and causes a
         # bug by limitting the ThinLV's size to VG free space which is nonsense
         super(LVMLogicalVolumeBase, self)._pre_create()  # pylint: disable=bad-super-call
 
     def _create(self):
         """ Create the device. """
         log_method_call(self, self.name, status=self.status)
-        blockdev.lvm.thlvcreate(self.vg.name, self.pool.lvname, self.lvname,
-                                self.size)
+        try:
+            blockdev.lvm.thlvcreate(self.vg.name, self.pool.lvname, self.lvname,
+                                    self.size)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     def remove_hook(self, modparent=True):
         if modparent:
             self.pool._remove_log_vol(self)
 
         # pylint: disable=bad-super-call
         super(LVMLogicalVolumeBase, self).remove_hook(modparent=modparent)
@@ -1973,46 +2038,55 @@
             raise errors.DeviceError("Cannot create new VDO pool without a VDO LV.")
 
         if self.write_policy:
             write_policy = blockdev.lvm_get_vdo_write_policy_str(self.write_policy)
         else:
             write_policy = blockdev.LVMVDOWritePolicy.AUTO
 
-        blockdev.lvm.vdo_pool_create(self.vg.name, self.vdo_lv.lvname, self.lvname,
-                                     self.size, self.vdo_lv.size, self.index_memory,
-                                     self.compression, self.deduplication,
-                                     write_policy)
+        try:
+            blockdev.lvm.vdo_pool_create(self.vg.name, self.vdo_lv.lvname, self.lvname,
+                                         self.size, self.vdo_lv.size, self.index_memory,
+                                         self.compression, self.deduplication,
+                                         write_policy)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     @util.requires_property("is_vdo_pool")
     def _set_compression(self, new_compression, old_compression, dry_run):
         if not self.exists:
             raise ValueError("device has not been created")
 
         if old_compression == new_compression:
             raise ValueError("compression is already %s on this VDO pool" % ("enabled" if new_compression else "disabled"))
 
         if not dry_run:
-            if new_compression:
-                blockdev.lvm.vdo_enable_compression(self.vg.name, self.lvname)
-            else:
-                blockdev.lvm.vdo_disable_compression(self.vg.name, self.lvname)
+            try:
+                if new_compression:
+                    blockdev.lvm.vdo_enable_compression(self.vg.name, self.lvname)
+                else:
+                    blockdev.lvm.vdo_disable_compression(self.vg.name, self.lvname)
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
 
     @util.requires_property("is_vdo_pool")
     def _set_deduplication(self, new_deduplication, old_deduplication, dry_run):
         if not self.exists:
             raise ValueError("device has not been created")
 
         if old_deduplication == new_deduplication:
             raise ValueError("deduplication is already %s on this VDO pool" % ("enabled" if new_deduplication else "disabled"))
 
         if not dry_run:
-            if new_deduplication:
-                blockdev.lvm.vdo_enable_deduplication(self.vg.name, self.lvname)
-            else:
-                blockdev.lvm.vdo_disable_deduplication(self.vg.name, self.lvname)
+            try:
+                if new_deduplication:
+                    blockdev.lvm.vdo_enable_deduplication(self.vg.name, self.lvname)
+                else:
+                    blockdev.lvm.vdo_disable_deduplication(self.vg.name, self.lvname)
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
 
 
 class LVMVDOLogicalVolumeMixin(object):
 
     _external_dependencies = [availability.BLOCKDEV_LVM_PLUGIN, availability.BLOCKDEV_LVM_PLUGIN_VDO]
 
     def __init__(self):
@@ -2234,21 +2308,27 @@
         if self._from_lvs:
             extra = dict()
             if self.mode:
                 # we need the string here, it will be passed directly to he lvm command
                 extra["cachemode"] = self._cache_mode
             data_lv = six.next(lv for lv in self._internal_lvs if lv.int_lv_type == LVMInternalLVtype.data)
             meta_lv = six.next(lv for lv in self._internal_lvs if lv.int_lv_type == LVMInternalLVtype.meta)
-            blockdev.lvm.cache_pool_convert(self.vg.name, data_lv.lvname, meta_lv.lvname, self.lvname, **extra)
+            try:
+                blockdev.lvm.cache_pool_convert(self.vg.name, data_lv.lvname, meta_lv.lvname, self.lvname, **extra)
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
         else:
-            blockdev.lvm.cache_create_pool(self.vg.name, self.lvname, self.size,
-                                           self.metadata_size,
-                                           cache_mode,
-                                           0,
-                                           [spec.pv.path for spec in self._pv_specs])
+            try:
+                blockdev.lvm.cache_create_pool(self.vg.name, self.lvname, self.size,
+                                               self.metadata_size,
+                                               cache_mode,
+                                               0,
+                                               [spec.pv.path for spec in self._pv_specs])
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
         if self._attach_to:
             self._attach_to.attach_cache(self)
 
     def _post_create(self):
         if self._attach_to:
             # post_create tries to activate the LV and after attaching it no longer exists
             return
@@ -2291,15 +2371,15 @@
 
     def __init__(self, name, parents=None, size=None, uuid=None, seg_type=None,
                  fmt=None, exists=False, sysfs_path='', grow=None, maxsize=None,
                  percent=None, cache_request=None, pvs=None,
                  parent_lv=None, int_type=None, origin=None, vorigin=False,
                  metadata_size=None, chunk_size=None, profile=None, from_lvs=None,
                  compression=False, deduplication=False, index_memory=0,
-                 write_policy=None, cache_mode=None, attach_to=None):
+                 write_policy=None, cache_mode=None, attach_to=None, stripe_size=0):
         """
             :param name: the device name (generally a device node's basename)
             :type name: str
             :keyword exists: does this device exist?
             :type exists: bool
             :keyword size: the device's size
             :type size: :class:`~.size.Size`
@@ -2371,14 +2451,19 @@
             :type metadata_size: :class:`~.size.Size`
             :keyword cache_mode: mode for the cache or None for default (writethrough)
             :type cache_mode: str
             :keyword attach_to: for non-existing cache pools a logical volume the pool should
                                 be attached to when created
             :type attach_to: :class:`LVMLogicalVolumeDevice`
 
+            For RAID LVs only:
+
+            :keyword stripe_size: size of the RAID stripe
+            :type stripe_size: :class:`~.size.Size`
+
         """
 
         if isinstance(parents, (list, ParentList)):
             vg = parents[0]
         else:
             vg = parents
         if parent_lv or int_type:
@@ -2391,15 +2476,16 @@
         LVMInternalLogicalVolumeMixin.__init__(self, vg, parent_lv, int_type)
         LVMSnapshotMixin.__init__(self, origin, vorigin)
         LVMThinPoolMixin.__init__(self, metadata_size, chunk_size, profile)
         LVMThinLogicalVolumeMixin.__init__(self)
         LVMCachePoolMixin.__init__(self, metadata_size, cache_mode, attach_to)
         LVMLogicalVolumeBase.__init__(self, name, parents, size, uuid, seg_type,
                                       fmt, exists, sysfs_path, grow, maxsize,
-                                      percent, cache_request, pvs, from_lvs)
+                                      percent, cache_request, pvs, from_lvs,
+                                      stripe_size)
         LVMVDOPoolMixin.__init__(self, compression, deduplication, index_memory,
                                  write_policy)
         LVMVDOLogicalVolumeMixin.__init__(self)
 
         LVMInternalLogicalVolumeMixin._init_check(self)
         LVMSnapshotMixin._init_check(self)
         LVMThinPoolMixin._init_check(self)
@@ -2623,15 +2709,18 @@
         return super(LVMLogicalVolumeDevice, self).pool
 
     def _setup(self, orig=False):
         """ Open, or set up, a device. """
         log_method_call(self, self.name, orig=orig, status=self.status,
                         controllable=self.controllable)
         ignore_skip_activation = self.is_snapshot_lv or self.ignore_skip_activation > 0
-        blockdev.lvm.lvactivate(self.vg.name, self._name, ignore_skip=ignore_skip_activation)
+        try:
+            blockdev.lvm.lvactivate(self.vg.name, self._name, ignore_skip=ignore_skip_activation)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     @type_specific
     def _pre_create(self):
         LVMLogicalVolumeBase._pre_create(self)
 
         try:
             vg_info = blockdev.lvm.vginfo(self.vg.name)
@@ -2657,16 +2746,23 @@
         # should we use --zero for safety's sake?
         if not self.cache:
             # just a plain LV
             # TODO: specify sizes together with PVs once LVM and libblockdev support it
             pvs = [spec.pv.path for spec in self._pv_specs]
             pvs = pvs or None
 
-            blockdev.lvm.lvcreate(self.vg.name, self._name, self.size,
-                                  type=self.seg_type, pv_list=pvs)
+            extra = dict()
+            if self._stripe_size:
+                extra["stripesize"] = str(int(self._stripe_size.convert_to("KiB")))
+
+            try:
+                blockdev.lvm.lvcreate(self.vg.name, self._name, self.size,
+                                      type=self.seg_type, pv_list=pvs, **extra)
+            except blockdev.LVMError as err:
+                raise errors.LVMError(err)
         else:
             fast_pvs = [pv.path for pv in self.cache.fast_pvs]
 
             if self._pv_specs:
                 # (slow) PVs specified for this LV
                 slow_pvs = [spec.pv.path for spec in self._pv_specs]
             else:
@@ -2681,20 +2777,26 @@
             slow_pvs = util.dedup_list(slow_pvs)
 
             # VG name, LV name, data size, cache size, metadata size, mode, flags, slow PVs, fast PVs
             # XXX: we need to pass slow_pvs+fast_pvs (without duplicates) as slow PVs because parts of the
             # fast PVs may be required for allocation of the LV (it may span over the slow PVs and parts of
             # fast PVs)
             if self.cache.type == "cache":
-                mode = blockdev.lvm.cache_get_mode_from_str(self.cache.mode)
-                blockdev.lvm.cache_create_cached_lv(self.vg.name, self._name, self.size, self.cache.size, self.cache.md_size,
-                                                    mode, 0, util.dedup_list(slow_pvs + fast_pvs), fast_pvs)
+                try:
+                    mode = blockdev.lvm.cache_get_mode_from_str(self.cache.mode)
+                    blockdev.lvm.cache_create_cached_lv(self.vg.name, self._name, self.size, self.cache.size, self.cache.md_size,
+                                                        mode, 0, util.dedup_list(slow_pvs + fast_pvs), fast_pvs)
+                except blockdev.LVMError as err:
+                    raise errors.LVMError(err)
             else:
-                blockdev.lvm.writecache_create_cached_lv(self.vg.name, self._name, self.size, self.cache.size,
-                                                         util.dedup_list(slow_pvs + fast_pvs), fast_pvs)
+                try:
+                    blockdev.lvm.writecache_create_cached_lv(self.vg.name, self._name, self.size, self.cache.size,
+                                                             util.dedup_list(slow_pvs + fast_pvs), fast_pvs)
+                except blockdev.LVMError as err:
+                    raise errors.LVMError(err)
 
     @type_specific
     def _post_create(self):
         LVMLogicalVolumeBase._post_create(self)
         # update the free space info of the PVs this LV could have taken space
         # from (either specified or potentially all PVs from the VG)
         if self._pv_specs:
@@ -2706,30 +2808,38 @@
             # value when queried
             pv.format.free = None
 
     @type_specific
     def _destroy(self):
         """ Destroy the device. """
         log_method_call(self, self.name, status=self.status)
-        blockdev.lvm.lvremove(self.vg.name, self._name)
+        try:
+            blockdev.lvm.lvremove(self.vg.name, self._name)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     @type_specific
     def resize(self):
         log_method_call(self, self.name, status=self.status)
 
         # Setup VG parents (in case they are dmraid partitions for example)
         self.vg.setup_parents(orig=True)
 
-        if self.original_format.exists:
-            self.original_format.teardown()
-        if self.format.exists:
-            self.format.teardown()
+        if not flags.allow_online_fs_resize:
+            if self.original_format.exists:
+                self.original_format.teardown()
+            if self.format.exists:
+                self.format.teardown()
 
-        udev.settle()
-        blockdev.lvm.lvresize(self.vg.name, self._name, self.size)
+            udev.settle()
+
+        try:
+            blockdev.lvm.lvresize(self.vg.name, self._name, self.size)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
 
     @type_specific
     def _add_log_vol(self, lv):
         pass
 
     @type_specific
     def _remove_log_vol(self, lv):
@@ -2832,15 +2942,18 @@
     @type_specific
     def autoset_md_size(self, enforced=False):
         pass
 
     def attach_cache(self, cache_pool_lv):
         if self.is_thin_lv or self.is_snapshot_lv or self.is_internal_lv:
             raise errors.DeviceError("Cannot attach a cache pool to the '%s' LV" % self.name)
-        blockdev.lvm.cache_attach(self.vg.name, self.lvname, cache_pool_lv.lvname)
+        try:
+            blockdev.lvm.cache_attach(self.vg.name, self.lvname, cache_pool_lv.lvname)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
         self._cache = LVMCache(self, size=cache_pool_lv.size, exists=True)
 
     def attach_writecache(self, writecache_lv):
         if self.is_thin_lv or self.is_snapshot_lv or self.is_internal_lv:
             raise errors.DeviceError("Cannot attach writecache to the '%s' LV" % self.name)
         try:
             blockdev.lvm.writecache_attach(self.vg.name, self.lvname, writecache_lv.lvname)
@@ -2999,16 +3112,19 @@
         :rtype: list of LVPVSpec
 
         """
         return self._pv_specs
 
     def detach(self):
         vg_name = self._cached_lv.vg.name
-        ret = blockdev.lvm.cache_pool_name(vg_name, self._cached_lv.lvname)
-        blockdev.lvm.cache_detach(vg_name, self._cached_lv.lvname, False)
+        try:
+            ret = blockdev.lvm.cache_pool_name(vg_name, self._cached_lv.lvname)
+            blockdev.lvm.cache_detach(vg_name, self._cached_lv.lvname, False)
+        except blockdev.LVMError as err:
+            raise errors.LVMError(err)
         return ret
 
 
 class LVMWriteCache(Cache):
 
     type = "writecache"
```

### Comparing `blivet-3.7.1/blivet/devices/md.py` & `blivet-3.8.0/blivet/devices/md.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import os
 import six
 import time
 
 from six.moves import reduce
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 from ..devicelibs import mdraid, raid
 
 from .. import errors
 from ..formats import DeviceFormat
@@ -265,16 +265,19 @@
            given the total available memory for this array and raid level.
 
            :param raw_array_size: total available for this array and level
            :type raw_array_size: :class:`~.size.Size`
            :returns: estimated superblock size
            :rtype: :class:`~.size.Size`
         """
-        return blockdev.md.get_superblock_size(raw_array_size,
-                                               version=self.metadata_version)
+        try:
+            return blockdev.md.get_superblock_size(raw_array_size,
+                                                   version=self.metadata_version)
+        except blockdev.MDRaidError as err:
+            raise errors.MDRaidError(err)
 
     @property
     def size(self):
         """Returns the actual or estimated size depending on whether or
            not the array exists.
         """
         if not self.exists or not self.media_present:
@@ -510,15 +513,18 @@
         log_method_call(self, self.name, orig=orig, status=self.status,
                         controllable=self.controllable)
         disks = []
         for member in self.members:
             member.setup(orig=orig)
             disks.append(member.path)
 
-        blockdev.md.activate(self.path, members=disks, uuid=self.mdadm_format_uuid)
+        try:
+            blockdev.md.activate(self.path, members=disks, uuid=self.mdadm_format_uuid)
+        except blockdev.MDRaidError as err:
+            raise errors.MDRaidError(err)
 
     def _post_teardown(self, recursive=False):
         super(MDRaidArrayDevice, self)._post_teardown(recursive=recursive)
         # mdadm reuses minors indiscriminantly when there is no mdadm.conf, so
         # we need to clear the sysfs path now so our status method continues to
         # give valid results
         self.sysfs_path = ''
@@ -538,15 +544,18 @@
             # treat arrays whose members are disks as partitionable disks
             return
 
         # We don't really care what the array's state is. If the device
         # file exists, we want to deactivate it. mdraid has too many
         # states.
         if self.exists and os.path.exists(self.path):
-            blockdev.md.deactivate(self.path)
+            try:
+                blockdev.md.deactivate(self.path)
+            except blockdev.MDRaidError as err:
+                raise errors.MDRaidError(err)
 
         self._post_teardown(recursive=recursive)
 
     def pre_commit_fixup(self, current_fmt=False):
         """ Determine create parameters for this set """
         log_method_call(self, self.name)
         # UEFI firmware/bootloader cannot read 1.1 or 1.2 metadata arrays
@@ -557,15 +566,19 @@
         # this is critical since our status method requires a valid sysfs path
         self.exists = True  # this is needed to run update_sysfs_path
         self.update_sysfs_path()
         StorageDevice._post_create(self)
 
         # update our uuid attribute with the new array's UUID
         # XXX this won't work for containers since no UUID is reported for them
-        info = blockdev.md.detail(self.path)
+        try:
+            info = blockdev.md.detail(self.path)
+        except blockdev.MDRaidError as err:
+            raise errors.MDRaidError(err)
+
         self.uuid = info.uuid
         for member in self.members:
             member.format.md_uuid = self.uuid
 
         def remove_stale_lvm():
             """ Remove any stale LVM metadata that pre-existed in a new array's on-disk footprint. """
             log.debug("waiting 5s for activation of stale lvm on new md array %s", self.path)
@@ -579,62 +592,74 @@
             if pv_info.vg_uuid:
                 log.info("removing stale LVM metadata found on %s", self.name)
                 try:
                     blockdev.lvm.vgremove(pv_info.vg_name, extra={"--select": "vg_uuid=%s" % pv_info.vg_uuid})
                 except blockdev.LVMError as e:
                     log.error("Failed to remove stale volume group from newly-created md array %s: %s",
                               self.path, str(e))
-                    raise
+                    raise errors.MDRaidError(e)
 
             # lvm says it is a pv whether or not there is vg metadata, so wipe the pv signature
-            blockdev.lvm.pvremove(self.path)
+            try:
+                blockdev.lvm.pvremove(self.path)
+            except blockdev.LVMError as err:
+                raise errors.MDRaidError(err)
 
         remove_stale_lvm()
 
         # remove any other stale metadata before proceeding
         DeviceFormat(device=self.path, exists=True).destroy()
 
     def _create(self):
         """ Create the device. """
         log_method_call(self, self.name, status=self.status)
         disks = [disk.path for disk in self.members]
         spares = len(self.members) - self.member_devices
         level = None
         if self.level:
             level = str(self.level)
-        blockdev.md.create(self.path, level, disks, spares,
-                           version=self.metadata_version,
-                           bitmap=self.create_bitmap,
-                           chunk_size=int(self.chunk_size))
+        try:
+            blockdev.md.create(self.path, level, disks, spares,
+                               version=self.metadata_version,
+                               bitmap="internal" if self.create_bitmap else None,
+                               chunk_size=int(self.chunk_size))
+        except blockdev.MDRaidError as err:
+            raise errors.MDRaidError(err)
         udev.settle()
 
     def _remove(self, member):
         self.setup()
         # see if the device must be marked as failed before it can be removed
         fail = (self.member_status(member) == "in_sync")
-        blockdev.md.remove(self.path, member.path, fail)
+        try:
+            blockdev.md.remove(self.path, member.path, fail)
+        except blockdev.MDRaidError as err:
+            raise errors.MDRaidError(err)
 
     def _add(self, member):
         """ Add a member device to an array.
 
            :param str member: the member's path
 
-           :raises: blockdev.MDRaidError
+           :raises: :class:`~.errors.MDRaidError`
         """
         self.setup()
 
         raid_devices = None
         try:
             if not self.level.has_redundancy():
                 if self.level is not raid.Linear:
                     raid_devices = int(blockdev.md.detail(self.name).raid_devices) + 1
         except errors.RaidError:
             pass
 
-        blockdev.md.add(self.path, member.path, raid_devs=raid_devices)
+        try:
+            blockdev.md.add(self.path, member.path, raid_devs=raid_devices)
+        except blockdev.MDRaidError as err:
+            raise errors.MDRaidError(err)
 
     @property
     def format_args(self):
         format_args = []
         if self.format.type == "ext2":
             recommended_stride = self.level.get_recommended_stride(self.member_devices)
             if recommended_stride:
```

### Comparing `blivet-3.7.1/blivet/devices/network.py` & `blivet-3.8.0/blivet/devices/network.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/nfs.py` & `blivet-3.8.0/blivet/devices/nfs.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/nodev.py` & `blivet-3.8.0/blivet/devices/nodev.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/optical.py` & `blivet-3.8.0/blivet/devices/optical.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/partition.py` & `blivet-3.8.0/blivet/devices/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import os
 import parted
 import _ped
 from uuid import UUID
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 from .. import errors
 from .. import util
 from .. import arch
 from ..flags import flags
@@ -790,19 +790,20 @@
 
         return super(PartitionDevice, self).sector_size
 
     def _pre_resize(self):
         if not self.exists:
             raise errors.DeviceError("device has not been created")
 
-        # don't teardown when resizing luks
-        if self.format.type == "luks" and self.children:
-            self.children[0].format.teardown()
-        else:
-            self.teardown()
+        if not flags.allow_online_fs_resize:
+            # don't teardown when resizing luks
+            if self.format.type == "luks" and self.children:
+                self.children[0].format.teardown()
+            else:
+                self.teardown()
 
         if not self.sysfs_path:
             return
 
         self.setup_parents(orig=True)
 
     def _pre_destroy(self):
```

### Comparing `blivet-3.7.1/blivet/devices/raid.py` & `blivet-3.8.0/blivet/devices/raid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/storage.py` & `blivet-3.8.0/blivet/devices/storage.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devices/stratis.py` & `blivet-3.8.0/blivet/devices/stratis.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/devicetree.py` & `blivet-3.8.0/blivet/devicetree.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import os
 import pprint
 import re
 import six
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 from .actionlist import ActionList
 from .callbacks import callbacks
 from .errors import DeviceError, DeviceTreeError, StorageError, DuplicateUUIDError, InvalidMultideviceSelection
 from .deviceaction import ActionDestroyDevice, ActionDestroyFormat
```

### Comparing `blivet-3.7.1/blivet/errors.py` & `blivet-3.8.0/blivet/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,14 +190,25 @@
     pass
 
 
 class StratisError(StorageError):
     pass
 
 
+class LoopError(StorageError):
+    pass
+
+
+class MDRaidError(StorageError):
+    pass
+
+
+class LVMError(StorageError):
+    pass
+
 # DeviceTree
 
 
 class DeviceTreeError(StorageError):
     pass
```

### Comparing `blivet-3.7.1/blivet/events/changes.py` & `blivet-3.8.0/blivet/events/changes.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/events/handler.py` & `blivet-3.8.0/blivet/events/handler.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/events/manager.py` & `blivet-3.8.0/blivet/events/manager.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/fcoe.py` & `blivet-3.8.0/blivet/fcoe.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/flags.py` & `blivet-3.8.0/blivet/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,17 @@
         self.debug_threads = False
 
         # Assign GPT partition type UUIDs to allow partition
         # auto-discovery according to:
         # https://uapi-group.org/specifications/specs/discoverable_partitions_specification/
         self.gpt_discoverable_partitions = False
 
+        # Allow online filesystem resizes
+        self.allow_online_fs_resize = False
+
     def get_boot_cmdline(self):
         with open("/proc/cmdline") as f:
             buf = f.read().strip()
             args = shlex.split(buf)
             for arg in args:
                 (opt, _equals, val) = arg.partition("=")
                 if val:
```

### Comparing `blivet-3.7.1/blivet/formats/__init__.py` & `blivet-3.8.0/blivet/formats/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 # source code or documentation are not subject to the GNU General Public
 # License and may only be used or replicated with the express permission of
 # Red Hat, Inc.
 #
 # Red Hat Author(s): Dave Lehman <dlehman@redhat.com>
 #
 
-import gi
-gi.require_version("BlockDev", "2.0")
-
-from gi.repository import BlockDev as blockdev
-
 import os
 import importlib
 from six import add_metaclass
 
 from .. import udev
 from ..util import get_sysfs_path_by_name
 from ..util import run_program
```

### Comparing `blivet-3.7.1/blivet/formats/biosboot.py` & `blivet-3.8.0/blivet/formats/biosboot.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/formats/disklabel.py` & `blivet-3.8.0/blivet/formats/disklabel.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #
 # Red Hat Author(s): Dave Lehman <dlehman@redhat.com>
 #
 
 import gi
 import os
 
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 from gi.repository import BlockDev as blockdev
 
 from ..storage_log import log_exception_info, log_method_call
 import parted
 import _ped
 from ..errors import DiskLabelCommitError, InvalidDiskLabelError, AlignmentError, PartitioningError
 from .. import arch
@@ -219,19 +219,16 @@
         return self._parted_device
 
     @classmethod
     def get_platform_label_types(cls):
         label_types = ["msdos", "gpt"]
         if arch.is_pmac():
             label_types = ["mac"]
-        elif arch.is_aarch64():
-            label_types = ["gpt", "msdos"]
-        elif arch.is_efi() and arch.is_arm():
-            label_types = ["msdos", "gpt"]
-        elif arch.is_efi() and not arch.is_aarch64():
+        # always prefer gpt on aarch64, x86_64, and EFI plats except 32-bit ARM
+        elif arch.is_aarch64() or arch.is_x86(bits=64) or (arch.is_efi() and not arch.is_arm()):
             label_types = ["gpt", "msdos"]
         elif arch.is_s390():
             label_types += ["dasd"]
 
         return label_types
 
     @classmethod
```

### Comparing `blivet-3.7.1/blivet/formats/dmraid.py` & `blivet-3.8.0/blivet/formats/dmraid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/formats/fs.py` & `blivet-3.8.0/blivet/formats/fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 from ..storage_log import log_exception_info, log_method_call
 from .. import arch
 from ..size import Size, ROUND_UP
 from ..i18n import N_
 from .. import udev
 from ..mounts import mounts_cache
 
-from .fslib import kernel_filesystems
+from .fslib import kernel_filesystems, FSResize
 
 import logging
 log = logging.getLogger("blivet")
 
 
 AVAILABLE_FILESYSTEMS = kernel_filesystems
 
@@ -84,14 +84,17 @@
     _selinux_supported = True
     # This constant is aquired by testing some filesystems
     # and it's giving us percentage of space left after the format.
     # This number is more guess than precise number because this
     # value is already unpredictable and can change in the future...
     _metadata_size_factor = 1.0
 
+    # support for resize: grow/shrink, online/offline
+    _resize_support = 0
+
     config_actions_map = {"label": "write_label"}
 
     def __init__(self, **kwargs):
         """
             :keyword device: path to the block device node (required for
                              existing filesystems)
             :keyword mountpoint: the filesystem's planned mountpoint
@@ -432,20 +435,35 @@
             except FSError as e:
                 log.warning("Failed to write label (%s) for filesystem %s: %s", self.label, self.type, e)
         if self.uuid is not None and not self.can_set_uuid() and \
            self.can_modify_uuid():
             self.write_uuid()
 
     def _pre_resize(self):
-        # file systems need a check before being resized
-        self.do_check()
+        if self.status:
+            if flags.allow_online_fs_resize:
+                if self.target_size > self.size and not self._resize_support & FSResize.ONLINE_GROW:
+                    raise FSError("This filesystem doesn't support online growing")
+                if self.target_size < self.size and not self._resize_support & FSResize.ONLINE_SHRINK:
+                    raise FSError("This filesystem doesn't support online shrinking")
+            else:
+                raise FSError("Resizing of mounted filesystems is disabled")
+
+        if self.status:
+            # fsck tools in general don't allow checks on mounted filesystems
+            log.debug("Filesystem on %s is mounted, not checking", self.device)
+        else:
+            # file systems need a check before being resized
+            self.do_check()
+
         super(FS, self)._pre_resize()
 
     def _post_resize(self):
-        self.do_check()
+        if not self.status:
+            self.do_check()
         super(FS, self)._post_resize()
 
     def do_check(self):
         """ Run a filesystem check.
 
             :raises: FSError
         """
@@ -834,14 +852,15 @@
     _modules = ["ext2"]
     _labelfs = fslabeling.Ext2FSLabeling()
     _uuidfs = fsuuid.Ext2FSUUID()
     _packages = ["e2fsprogs"]
     _formattable = True
     _supported = True
     _resizable = True
+    _resize_support = FSResize.ONLINE_GROW | FSResize.OFFLINE_GROW | FSResize.OFFLINE_SHRINK
     _linux_native = True
     _max_size = Size("8 TiB")
     _dump = True
     _check = True
     _fsck_class = fsck.Ext2FSCK
     _info_class = fsinfo.Ext2FSInfo
     _minsize_class = fsminsize.Ext2FSMinSize
@@ -1093,14 +1112,15 @@
     _uuidfs = fsuuid.XFSUUID()
     _min_size = Size("300 MiB")
     _max_size = Size("16 EiB")
     _formattable = True
     _linux_native = True
     _supported = True
     _resizable = True
+    _resize_support = FSResize.ONLINE_GROW | FSResize.OFFLINE_GROW
     _packages = ["xfsprogs"]
     _fsck_class = fsck.XFSCK
     _info_class = fsinfo.XFSInfo
     _mkfs_class = fsmkfs.XFSMkfs
     _readlabel_class = fsreadlabel.XFSReadLabel
     _size_info_class = fssize.XFSSize
     _resize_class = fsresize.XFSResize
@@ -1243,14 +1263,15 @@
 class NTFS(FS):
 
     """ ntfs filesystem. """
     _type = "ntfs"
     _labelfs = fslabeling.NTFSLabeling()
     _uuidfs = fsuuid.NTFSUUID()
     _resizable = True
+    _resize_support = FSResize.OFFLINE_GROW | FSResize.OFFLINE_SHRINK
     _formattable = True
     _supported = True
     _min_size = Size("1 MiB")
     _max_size = Size("16 TiB")
     _packages = ["ntfsprogs"]
     _fsck_class = fsck.NTFSFSCK
     _info_class = fsinfo.NTFSInfo
@@ -1498,14 +1519,17 @@
         # the DeviceFormat parent class does a
         # self.device = kwargs["device"]
         # assignment, so we need a setter for the
         # device property, but as the device is always the
         # same, nothing actually needs to be set
         pass
 
+    def _pre_resize(self):
+        self.do_check()
+
     def do_resize(self):
         # Override superclass method to record whether mount options
         # should include an explicit size specification.
         original_size = self._size
         FS.do_resize(self)
         self._accept_default_size = self._accept_default_size and original_size == self._size
```

### Comparing `blivet-3.7.1/blivet/formats/fslib.py` & `blivet-3.8.0/blivet/formats/fslib.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,7 +32,14 @@
             fstype = fields[-1]
             kernel_filesystems.append(fstype)
             if fields[0] == "nodev":
                 nodev_filesystems.append(fstype)
 
 
 update_kernel_filesystems()
+
+
+class FSResize():
+    OFFLINE_SHRINK = 1 << 1
+    OFFLINE_GROW = 1 << 2
+    ONLINE_SHRINK = 1 << 3
+    ONLINE_GROW = 1 << 4
```

### Comparing `blivet-3.7.1/blivet/formats/luks.py` & `blivet-3.8.0/blivet/formats/luks.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # License and may only be used or replicated with the express permission of
 # Red Hat, Inc.
 #
 # Red Hat Author(s): Dave Lehman <dlehman@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import os
 
 from ..storage_log import log_method_call
 from ..errors import LUKSError, IntegrityError
@@ -258,27 +258,38 @@
             raise LUKSError("luks device not configured")
 
         return super(LUKS, self)._pre_setup(**kwargs)
 
     def _setup(self, **kwargs):
         log_method_call(self, device=self.device, map_name=self.map_name,
                         type=self.type, status=self.status)
+
+        # passphrase is preferred for open
+        if self.__passphrase:
+            context = blockdev.CryptoKeyslotContext(passphrase=self.__passphrase)
+        elif self._key_file:
+            context = blockdev.CryptoKeyslotContext(keyfile=self._key_file)
+        else:
+            raise LUKSError("Passphrase or key file must be set for LUKS setup")
+
         try:
-            blockdev.crypto.luks_open(self.device, self.map_name,
-                                      passphrase=self.__passphrase,
-                                      key_file=self._key_file)
+            blockdev.crypto.luks_open(self.device, self.map_name, context=context)
         except blockdev.CryptoError as e:
             raise LUKSError(e)
 
     def _teardown(self, **kwargs):
         """ Close, or tear down, the format. """
         log_method_call(self, device=self.device,
                         type=self.type, status=self.status)
         log.debug("unmapping %s", self.map_name)
-        blockdev.crypto.luks_close(self.map_name)
+
+        try:
+            blockdev.crypto.luks_close(self.map_name)
+        except blockdev.CryptoError as e:
+            raise LUKSError(e)
 
         udev.settle()
 
     def _pre_resize(self):
         if self.luks_version == "luks2" and not self.has_key:
             raise LUKSError("Passphrase or key needs to be set before resizing LUKS2 format.")
 
@@ -295,21 +306,23 @@
                         type=self.type, status=self.status)
         super(LUKS, self)._create(**kwargs)  # set up the event sync
 
         if not self.pbkdf_args and self.luks_version == "luks2":
             if luks_data.pbkdf_args:
                 self.pbkdf_args = luks_data.pbkdf_args
             else:
-                mem_limit = crypto.calculate_luks2_max_memory()
-                if mem_limit:
-                    self.pbkdf_args = LUKS2PBKDFArgs(max_memory_kb=int(mem_limit.convert_to(KiB)))
-                    luks_data.pbkdf_args = self.pbkdf_args
-                    log.info("PBKDF arguments for LUKS2 not specified, using defaults with memory limit %s", mem_limit)
+                # argon is not used with FIPS so we don't need to adjust the memory when in FIPS mode
+                if not crypto.is_fips_enabled():
+                    mem_limit = crypto.calculate_luks2_max_memory()
+                    if mem_limit:
+                        self.pbkdf_args = LUKS2PBKDFArgs(max_memory_kb=int(mem_limit.convert_to(KiB)))
+                        luks_data.pbkdf_args = self.pbkdf_args
+                        log.info("PBKDF arguments for LUKS2 not specified, using defaults with memory limit %s", mem_limit)
 
-        if not self.luks_sector_size:
+        if not self.luks_sector_size and self.luks_version == "luks2":
             self.luks_sector_size = crypto.get_optimal_luks_sector_size(self.device)
 
         if self.pbkdf_args:
             pbkdf = blockdev.CryptoLUKSPBKDF(type=self.pbkdf_args.type,
                                              hash=self.pbkdf_args.hash_fn,
                                              max_memory_kb=self.pbkdf_args.max_memory_kb,
                                              iterations=self.pbkdf_args.iterations,
@@ -318,26 +331,50 @@
                                              sector_size=self.luks_sector_size)
         else:
             if self.luks_sector_size:
                 extra = blockdev.CryptoLUKSExtra(sector_size=self.luks_sector_size)
             else:
                 extra = None
 
-        blockdev.crypto.luks_format(self.device,
-                                    passphrase=self.__passphrase,
-                                    key_file=self._key_file,
-                                    cipher=self.cipher,
-                                    key_size=self.key_size,
-                                    min_entropy=self.min_luks_entropy,
-                                    luks_version=crypto.LUKS_VERSIONS[self.luks_version],
-                                    extra=extra)
+        if self.__passphrase:
+            context = blockdev.CryptoKeyslotContext(passphrase=self.__passphrase)
+        elif self._key_file:
+            context = blockdev.CryptoKeyslotContext(keyfile=self._key_file)
+        else:
+            raise LUKSError("Passphrase or key file must be set for LUKS create")
+
+        try:
+            blockdev.crypto.luks_format(self.device,
+                                        context=context,
+                                        cipher=self.cipher,
+                                        key_size=self.key_size,
+                                        min_entropy=self.min_luks_entropy,
+                                        luks_version=crypto.LUKS_VERSIONS[self.luks_version],
+                                        extra=extra)
+        except blockdev.CryptoError as e:
+            raise LUKSError(e)
+
+        if self.__passphrase and self._key_file:
+            # both passphrase and keyfile are set, we need to add the keyfile too
+            ncontext = blockdev.CryptoKeyslotContext(keyfile=self._key_file)
+            try:
+                blockdev.crypto.luks_add_key(self.device, context, ncontext)
+            except blockdev.CryptoError as e:
+                raise LUKSError(e)
 
     def _post_create(self, **kwargs):
         super(LUKS, self)._post_create(**kwargs)
-        self.uuid = blockdev.crypto.luks_uuid(self.device)
+
+        try:
+            info = blockdev.crypto.luks_info(self.device)
+        except blockdev.CryptoError as e:
+            raise LUKSError("Failed to get UUID for the newly created LUKS device %s: %s" % (self.device, str(e)))
+        else:
+            self.uuid = info.uuid
+
         if not self.map_name:
             self.map_name = "luks-%s" % self.uuid
 
     @property
     def destroyable(self):
         return self._plugin.available
 
@@ -353,39 +390,64 @@
             LUKS header.
         """
         log_method_call(self, device=self.device,
                         type=self.type, status=self.status)
         if not self.exists:
             raise LUKSError("format has not been created")
 
-        blockdev.crypto.luks_add_key(self.device,
-                                     pass_=self.__passphrase,
-                                     key_file=self._key_file,
-                                     npass=passphrase)
+        # if both passphrase and keyfile are set, they both need to be valid so
+        # we can choose passphrase as default
+        if self.__passphrase:
+            context = blockdev.CryptoKeyslotContext(passphrase=self.__passphrase)
+        elif self._key_file:
+            context = blockdev.CryptoKeyslotContext(keyfile=self._key_file)
+
+        ncontext = blockdev.CryptoKeyslotContext(passphrase=passphrase)
+
+        try:
+            blockdev.crypto.luks_add_key(self.device, context, ncontext)
+        except blockdev.CryptoError as e:
+            raise LUKSError(e)
 
     def remove_passphrase(self):
         """
         Remove the saved passphrase (and possibly key file) from the LUKS
         header.
 
+        Note: If both passphrase and keyfile are set for this format, both
+              will be removed!
         """
 
         log_method_call(self, device=self.device,
                         type=self.type, status=self.status)
         if not self.exists:
             raise LUKSError("format has not been created")
 
-        blockdev.crypto.luks_remove_key(self.device,
-                                        pass_=self.__passphrase,
-                                        key_file=self._key_file)
+        def _remove_passphrase(context):
+            try:
+                blockdev.crypto.luks_remove_key(self.device, context=context)
+            except blockdev.CryptoError as e:
+                raise LUKSError(e)
+
+        if self.__passphrase:
+            context = blockdev.CryptoKeyslotContext(passphrase=self.__passphrase)
+            _remove_passphrase(context)
+        elif self._key_file:
+            context = blockdev.CryptoKeyslotContext(keyfile=self._key_file)
+            _remove_passphrase(context)
 
     def escrow(self, directory, backup_passphrase):
         log.debug("escrow: escrow_volume start for %s", self.device)
-        blockdev.crypto.escrow_device(self.device, self.__passphrase, self.escrow_cert,
-                                      directory, backup_passphrase)
+
+        try:
+            blockdev.crypto.escrow_device(self.device, self.__passphrase, self.escrow_cert,
+                                          directory, backup_passphrase)
+        except blockdev.CryptoError as e:
+            raise LUKSError(e)
+
         log.debug("escrow: escrow_volume done for %s", repr(self.device))
 
     def populate_ksdata(self, data):
         super(LUKS, self).populate_ksdata(data)
         data.luks_version = self.luks_version
 
         if self.pbkdf_args:
@@ -475,25 +537,31 @@
         super(Integrity, self)._create(**kwargs)  # set up the event sync
 
         if self.sector_size:
             extra = blockdev.CryptoIntegrityExtra(sector_size=self.sector_size)
         else:
             extra = None
 
-        blockdev.crypto.integrity_format(self.device,
-                                         self.algorithm,
-                                         extra=extra)
+        try:
+            blockdev.crypto.integrity_format(self.device,
+                                             self.algorithm,
+                                             extra=extra)
+        except blockdev.CryptoError as e:
+            raise IntegrityError(e)
 
     def _teardown(self, **kwargs):
         """ Close, or tear down, the format. """
         log_method_call(self, device=self.device,
                         type=self.type, status=self.status)
         log.debug("unmapping %s", self.map_name)
 
         # it's safe to use luks_close here, it uses crypt_deactivate which works
         # for all devices supported by cryptsetup
-        blockdev.crypto.luks_close(self.map_name)
+        try:
+            blockdev.crypto.luks_close(self.map_name)
+        except blockdev.CryptoError as e:
+            raise IntegrityError(e)
 
         udev.settle()
 
 
 register_device_format(Integrity)
```

### Comparing `blivet-3.7.1/blivet/formats/lvmpv.py` & `blivet-3.8.0/blivet/formats/lvmpv.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 # License and may only be used or replicated with the express permission of
 # Red Hat, Inc.
 #
 # Red Hat Author(s): Dave Lehman <dlehman@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import os
 
 from ..storage_log import log_method_call
 from parted import PARTITION_LVM
 from ..devicelibs import lvm
 from ..tasks import availability, pvtask
 from ..i18n import N_
 from ..size import Size
 from ..errors import PhysicalVolumeError
 from . import DeviceFormat, register_device_format
 from .. import udev
-from ..static_data.lvm_info import pvs_info
+from ..static_data.lvm_info import pvs_info, vgs_info
 
 import logging
 log = logging.getLogger("blivet")
 
 
 class LVMPhysicalVolume(DeviceFormat):
 
@@ -117,18 +117,29 @@
     def formattable(self):
         return super(LVMPhysicalVolume, self).formattable and self._plugin.available
 
     @property
     def supported(self):
         return super(LVMPhysicalVolume, self).supported and self._plugin.available
 
-    def lvmdevices_add(self):
+    def lvmdevices_add(self, force=True):
+        """ Add this PV to the LVM system devices file
+            :keyword force: whether to add the PV even if the system devices file doesn't exist and
+                            VGs are present in the system
+            :type force: bool
+        """
+
         if not lvm.HAVE_LVMDEVICES:
             raise PhysicalVolumeError("LVM devices file feature is not supported")
 
+        if not os.path.exists(lvm.LVM_DEVICES_FILE) and vgs_info.cache and not force:
+            log.debug("Not adding %s to devices file: %s doesn't exist and there are VGs present in the system",
+                      self.device, lvm.LVM_DEVICES_FILE)
+            return
+
         try:
             blockdev.lvm.devices_add(self.device)
         except blockdev.LVMError as e:
             log.debug("Failed to add PV %s to the LVM devices file: %s", self.device, str(e))
 
     def lvmdevices_remove(self):
         if not lvm.HAVE_LVMDEVICES:
@@ -146,18 +157,24 @@
 
         ea_yes = blockdev.ExtraArg.new("-y", "")
 
         if lvm.HAVE_LVMDEVICES:
             with lvm.empty_lvm_devices():
                 # with lvmdbusd we need to call the pvcreate without --devices otherwise lvmdbusd
                 # wouldn't be able to find the newly created pv and the call would fail
-                blockdev.lvm.pvcreate(self.device, data_alignment=self.data_alignment, extra=[ea_yes])
-                self.lvmdevices_add()
+                try:
+                    blockdev.lvm.pvcreate(self.device, data_alignment=self.data_alignment, extra=[ea_yes])
+                except blockdev.LVMError as e:
+                    raise PhysicalVolumeError(e)
+                self.lvmdevices_add(force=False)
         else:
-            blockdev.lvm.pvcreate(self.device, data_alignment=self.data_alignment, extra=[ea_yes])
+            try:
+                blockdev.lvm.pvcreate(self.device, data_alignment=self.data_alignment, extra=[ea_yes])
+            except blockdev.LVMError as e:
+                raise PhysicalVolumeError(e)
 
     def _destroy(self, **kwargs):
         log_method_call(self, device=self.device,
                         type=self.type, status=self.status)
         try:
             blockdev.lvm.pvremove(self.device)
         except blockdev.LVMError:
```

### Comparing `blivet-3.7.1/blivet/formats/mdraid.py` & `blivet-3.8.0/blivet/formats/mdraid.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 # License and may only be used or replicated with the express permission of
 # Red Hat, Inc.
 #
 # Red Hat Author(s): Dave Lehman <dlehman@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 from ..storage_log import log_method_call
 from parted import PARTITION_RAID
 from . import DeviceFormat, register_device_format
+from ..errors import MDMemberError
 from ..i18n import N_
 from ..tasks import availability
 
 import logging
 log = logging.getLogger("blivet")
 
 
@@ -84,15 +85,18 @@
         return super(MDRaidMember, self).formattable and self._plugin.available
 
     @property
     def supported(self):
         return super(MDRaidMember, self).supported and self._plugin.available
 
     def _destroy(self, **kwargs):
-        blockdev.md.destroy(self.device)
+        try:
+            blockdev.md.destroy(self.device)
+        except blockdev.MDRaidError as e:
+            raise MDMemberError(e)
 
     @property
     def destroyable(self):
         return self._plugin.available
 
     @property
     def status(self):
```

### Comparing `blivet-3.7.1/blivet/formats/multipath.py` & `blivet-3.8.0/blivet/formats/multipath.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/formats/prepboot.py` & `blivet-3.8.0/blivet/formats/prepboot.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/formats/stratis.py` & `blivet-3.8.0/blivet/formats/stratis.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/formats/swap.py` & `blivet-3.8.0/blivet/formats/swap.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from ..tasks import availability
 from ..tasks import fsuuid
 from . import DeviceFormat, register_device_format
 from ..size import Size
 from .. import udev
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import logging
 log = logging.getLogger("blivet")
 
 
@@ -140,15 +140,18 @@
 
             if self.label is None:
                 raise SwapSpaceError("makes no sense to write a label when accepting default label")
 
             if not self.label_format_ok(self.label):
                 raise SwapSpaceError("bad label format")
 
-            blockdev.swap.mkswap(self.device, self.label)
+            try:
+                blockdev.swap.mkswap(self.device, self.label)
+            except blockdev.SwapError as err:
+                raise SwapSpaceError("Failed to change label on %s: %s" % (self.device, str(err)))
 
     label = property(lambda s: s._get_label(), lambda s, l: s._set_label(l),
                      doc="the label for this swap space")
 
     def uuid_format_ok(self, uuid):
         """Check whether the given UUID is correct according to RFC 4122."""
         return fsuuid.FSUUID._check_rfc4122_uuid(uuid)
@@ -190,35 +193,54 @@
                     self.priority = int(arg)
                 except ValueError:
                     log.info("invalid value for swap priority: %s", arg)
 
     @property
     def status(self):
         """ Device status. """
-        return self.exists and blockdev.swap.swapstatus(self.device)
+        if not self.exists:
+            return False
+        try:
+            status = blockdev.swap.swapstatus(self.device)
+        except blockdev.SwapError as err:
+            raise SwapSpaceError("Failed to get swap status for %s: %s" % (self.device, str(err)))
+        else:
+            return status
 
     def _setup(self, **kwargs):
         log_method_call(self, device=self.device,
                         type=self.type, status=self.status)
-        blockdev.swap.swapon(self.device, priority=self.priority)
+        try:
+            blockdev.swap.swapon(self.device, priority=self.priority)
+        except blockdev.SwapError as err:
+            raise SwapSpaceError("Failed to activate swap %s: %s" % (self.device, str(err)))
 
     def _teardown(self, **kwargs):
         """ Close, or tear down, a device. """
         log_method_call(self, device=self.device,
                         type=self.type, status=self.status)
-        blockdev.swap.swapoff(self.device)
+        try:
+            blockdev.swap.swapoff(self.device)
+        except blockdev.SwapError as err:
+            raise SwapSpaceError("Failed to deactivate swap %s: %s" % (self.device, str(err)))
 
         udev.settle()
 
     def _create(self, **kwargs):
         log_method_call(self, device=self.device,
                         type=self.type, status=self.status)
         if self.uuid is None:
-            blockdev.swap.mkswap(self.device, label=self.label)
+            try:
+                blockdev.swap.mkswap(self.device, label=self.label)
+            except blockdev.SwapError as err:
+                raise SwapSpaceError(str(err))
         else:
             if not self.uuid_format_ok(self.uuid):
                 raise FSWriteUUIDError("bad UUID format for swap filesystem")
-            blockdev.swap.mkswap(self.device, label=self.label,
-                                 extra={"-U": self.uuid})
+            try:
+                blockdev.swap.mkswap(self.device, label=self.label,
+                                     extra={"-U": self.uuid})
+            except blockdev.SwapError as err:
+                raise SwapSpaceError(str(err))
 
 
 register_device_format(SwapSpace)
```

### Comparing `blivet-3.7.1/blivet/i18n.py` & `blivet-3.8.0/blivet/i18n.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/iscsi.py` & `blivet-3.8.0/blivet/iscsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 def _to_node_infos(variant):
     """Transforms an 'a(sisis)' GLib.Variant into a list of NodeInfo objects"""
     return [NodeInfo(*info) for info in variant]
 
 
 class iSCSIDependencyGuard(util.DependencyGuard):
-    error_msg = "storaged iSCSI functionality not available"
+    error_msg = "UDisks iSCSI functionality not available"
 
     def _check_avail(self):
         try:
             if not safe_dbus.check_object_available(STORAGED_SERVICE, STORAGED_MANAGER_PATH, MANAGER_IFACE):
                 return False
             # storaged is modular and we need to make sure it has the iSCSI module
             # loaded (this also autostarts storaged if it isn't running already)
@@ -208,22 +208,31 @@
         # udisks returns initiatorname as a NULL terminated bytearray
         raw_initiator = bytes(self._call_initiator_method("GetInitiatorNameRaw")[0][:-1])
         return raw_initiator.decode("utf-8", errors="replace")
 
     @initiator.setter
     @storaged_iscsi_required(critical=True, eval_mode=util.EvalMode.onetime)
     def initiator(self, val):
-        if self.initiator_set and val != self._initiator:
-            raise ValueError(_("Unable to change iSCSI initiator name once set"))
         if len(val) == 0:
             raise ValueError(_("Must provide an iSCSI initiator name"))
 
+        active = self._get_active_sessions()
+        if active:
+            raise errors.ISCSIError(_("Cannot change initiator name with an active session"))
+
         log.info("Setting up iSCSI initiator name %s", self.initiator)
         args = GLib.Variant("(sa{sv})", (val, None))
         self._call_initiator_method("SetInitiatorName", args)
+
+        if self.initiator_set and val != self._initiator:
+            log.info("Restarting iscsid after initiator name change")
+            rc = util.run_program(["systemctl", "restart", "iscsid"])
+            if rc != 0:
+                raise errors.ISCSIError(_("Failed to restart iscsid after initiator name change"))
+
         self._initiator = val
 
     def active_nodes(self, target=None):
         """Nodes logged in to"""
         if target:
             return [info.node for info in self.discovered_targets.get(target, [])
                     if info.logged_in]
@@ -260,14 +269,15 @@
         :raises :class:`~.safe_dbus.DBusCallError`: if login fails
 
         """
 
         if extra is None:
             extra = dict()
         extra["node.startup"] = GLib.Variant("s", "automatic")
+        extra["node.session.auth.chap_algs"] = GLib.Variant("s", "SHA3-256,SHA256,SHA1,MD5")
 
         args = GLib.Variant("(sisisa{sv})", node_info.conn_info + (extra,))
         self._call_initiator_method("Login", args)
 
     @storaged_iscsi_required(critical=False, eval_mode=util.EvalMode.onetime)
     def _get_active_sessions(self):
         try:
```

### Comparing `blivet-3.7.1/blivet/mounts.py` & `blivet-3.8.0/blivet/mounts.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/nvme.py` & `blivet-3.8.0/blivet/nvme.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/partitioning.py` & `blivet-3.8.0/blivet/partitioning.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #
 
 from operator import gt, lt
 from decimal import Decimal
 import functools
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 import parted
 import _ped
 
 from .errors import DeviceError, PartitioningError, AlignmentError
 from .flags import flags
 from .devices import Device, PartitionDevice, device_path_to_name
```

### Comparing `blivet-3.7.1/blivet/populator/helpers/__init__.py` & `blivet-3.8.0/blivet/populator/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/helpers/boot.py` & `blivet-3.8.0/blivet/populator/helpers/boot.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/helpers/btrfs.py` & `blivet-3.8.0/blivet/populator/helpers/btrfs.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/helpers/devicepopulator.py` & `blivet-3.8.0/blivet/populator/helpers/devicepopulator.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/helpers/disk.py` & `blivet-3.8.0/blivet/populator/helpers/disk.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # to the GNU Lesser General Public License and may only be used or
 # replicated with the express permission of Red Hat, Inc.
 #
 # Red Hat Author(s): David Lehman <dlehman@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 gi.require_version("GLib", "2.0")
 
 from gi.repository import BlockDev as blockdev
 from gi.repository import GLib
 
 from ... import udev
 from ... import util
```

### Comparing `blivet-3.7.1/blivet/populator/helpers/disklabel.py` & `blivet-3.8.0/blivet/populator/helpers/disklabel.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/helpers/dm.py` & `blivet-3.8.0/blivet/populator/helpers/dm.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/helpers/formatpopulator.py` & `blivet-3.8.0/blivet/populator/helpers/formatpopulator.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/helpers/loop.py` & `blivet-3.8.0/blivet/populator/helpers/loop.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # to the GNU Lesser General Public License and may only be used or
 # replicated with the express permission of Red Hat, Inc.
 #
 # Red Hat Author(s): David Lehman <dlehman@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 from gi.repository import BlockDev as blockdev
 
 from ... import udev
 from ...devices import FileDevice, LoopDevice
 from ...storage_log import log_method_call
 from .devicepopulator import DevicePopulator
 
@@ -35,20 +35,23 @@
     def match(cls, data):
         return udev.device_is_loop(data)
 
     def run(self):
         name = udev.device_get_name(self.data)
         log_method_call(self, name=name)
         sysfs_path = udev.device_get_sysfs_path(self.data)
-        backing_file = blockdev.loop.get_backing_file(name)
-        if backing_file is None:
+        try:
+            info = blockdev.loop.info(name)
+        except blockdev.LoopError:
             return None
-        file_device = self._devicetree.get_device_by_name(backing_file)
+        if not info.backing_file:
+            return None
+        file_device = self._devicetree.get_device_by_name(info.backing_file)
         if not file_device:
-            file_device = FileDevice(backing_file, exists=True)
+            file_device = FileDevice(info.backing_file, exists=True)
             self._devicetree._add_device(file_device)
         device = LoopDevice(name,
                             parents=[file_device],
                             sysfs_path=sysfs_path,
                             exists=True)
         if not self._devicetree._cleanup or file_device not in self._devicetree.disk_images.values():
             # don't allow manipulation of loop devices other than those
```

### Comparing `blivet-3.7.1/blivet/populator/helpers/luks.py` & `blivet-3.8.0/blivet/populator/helpers/luks.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # to the GNU Lesser General Public License and may only be used or
 # replicated with the express permission of Red Hat, Inc.
 #
 # Red Hat Author(s): David Lehman <dlehman@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 from ... import udev
 from ...devices import LUKSDevice, IntegrityDevice
 from ...errors import DeviceError, LUKSError
 from ...flags import flags
```

### Comparing `blivet-3.7.1/blivet/populator/helpers/lvm.py` & `blivet-3.8.0/blivet/populator/helpers/lvm.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # to the GNU Lesser General Public License and may only be used or
 # replicated with the express permission of Red Hat, Inc.
 #
 # Red Hat Author(s): David Lehman <dlehman@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 from ...callbacks import callbacks
 from ... import udev
 from ...devicelibs import lvm
 from ...devices.lvm import LVMVolumeGroupDevice, LVMLogicalVolumeDevice, LVMInternalLVtype
```

### Comparing `blivet-3.7.1/blivet/populator/helpers/mdraid.py` & `blivet-3.8.0/blivet/populator/helpers/mdraid.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # to the GNU Lesser General Public License and may only be used or
 # replicated with the express permission of Red Hat, Inc.
 #
 # Red Hat Author(s): David Lehman <dlehman@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import re
 
 from ... import udev
 from ...devicelibs import raid
```

### Comparing `blivet-3.7.1/blivet/populator/helpers/multipath.py` & `blivet-3.8.0/blivet/populator/helpers/multipath.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/helpers/optical.py` & `blivet-3.8.0/blivet/populator/helpers/optical.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/helpers/partition.py` & `blivet-3.8.0/blivet/populator/helpers/partition.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/helpers/populatorhelper.py` & `blivet-3.8.0/blivet/populator/helpers/populatorhelper.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/helpers/stratis.py` & `blivet-3.8.0/blivet/populator/helpers/stratis.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/populator/populator.py` & `blivet-3.8.0/blivet/populator/populator.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import os
 import pprint
 import copy
 import parted
 from six import add_metaclass
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 from ..errors import DeviceError, DeviceTreeError, NoParentsError
 from ..devices import DMLinearDevice
 from ..devices import FileDevice, LoopDevice
 from ..devices import MDRaidArrayDevice
```

### Comparing `blivet-3.7.1/blivet/safe_dbus.py` & `blivet-3.8.0/blivet/safe_dbus.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/size.py` & `blivet-3.8.0/blivet/size.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/static_data/luks_data.py` & `blivet-3.8.0/blivet/static_data/luks_data.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/static_data/lvm_info.py` & `blivet-3.8.0/blivet/static_data/lvm_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # to the GNU Lesser General Public License and may only be used or
 # replicated with the express permission of Red Hat, Inc.
 #
 # Red Hat Author(s): Jan Pokorny <japokorn@redhat.com>
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import logging
 log = logging.getLogger("blivet")
```

### Comparing `blivet-3.7.1/blivet/static_data/mpath_info.py` & `blivet-3.8.0/blivet/static_data/mpath_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # replicated with the express permission of Red Hat, Inc.
 #
 # Red Hat Author(s): Vratislav Podzimek <vpodzime@redhat.com>
 #
 
 import os
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import logging
 log = logging.getLogger("blivet")
 
 from ..tasks import availability
```

### Comparing `blivet-3.7.1/blivet/static_data/nvdimm.py` & `blivet-3.8.0/blivet/static_data/nvdimm.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 gi.require_version("GLib", "2.0")
 from gi.repository import BlockDev
 from gi.repository import GLib
 
 from .. import util
 
 import logging
@@ -30,15 +30,15 @@
 
 
 class NVDIMMDependencyGuard(util.DependencyGuard):
     error_msg = "libblockdev NVDIMM functionality not available"
 
     def _check_avail(self):
         try:
-            BlockDev.nvdimm_is_tech_avail(BlockDev.NVDIMMTech.NVDIMM_TECH_NAMESPACE,
+            BlockDev.nvdimm_is_tech_avail(BlockDev.NVDIMMTech.NAMESPACE,
                                           BlockDev.NVDIMMTechMode.RECONFIGURE |
                                           BlockDev.NVDIMMTechMode.QUERY |
                                           BlockDev.NVDIMMTechMode.ACTIVATE_DEACTIVATE)
         except GLib.GError:
             return False
         return True
```

### Comparing `blivet-3.7.1/blivet/static_data/stratis_info.py` & `blivet-3.8.0/blivet/static_data/stratis_info.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/storage_log.py` & `blivet-3.8.0/blivet/storage_log.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/availability.py` & `blivet-3.8.0/blivet/tasks/availability.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from six import add_metaclass
 
 from .. import safe_dbus
 from ..devicelibs.stratis import STRATIS_SERVICE, STRATIS_PATH
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 gi.require_version("GLib", "2.0")
 gi.require_version("Gio", "2.0")
 
 from gi.repository import BlockDev as blockdev
 from gi.repository import GLib, Gio
 
 import logging
@@ -367,15 +367,14 @@
                              blockdev.CryptoTechMode.QUERY |
                              blockdev.CryptoTechMode.ADD_KEY |
                              blockdev.CryptoTechMode.REMOVE_KEY |
                              blockdev.CryptoTechMode.RESIZE)
 BLOCKDEV_CRYPTO = BlockDevTechInfo(plugin_name="crypto",
                                    check_fn=blockdev.crypto_is_tech_avail,
                                    technologies={blockdev.CryptoTech.LUKS: BLOCKDEV_CRYPTO_ALL_MODES,
-                                                 blockdev.CryptoTech.LUKS2: BLOCKDEV_CRYPTO_ALL_MODES,
                                                  blockdev.CryptoTech.ESCROW: blockdev.CryptoTechMode.CREATE})
 BLOCKDEV_CRYPTO_TECH = BlockDevMethod(BLOCKDEV_CRYPTO)
 
 BLOCKDEV_CRYPTO_INTEGRITY = BlockDevTechInfo(plugin_name="crypto",
                                              check_fn=blockdev.crypto_is_tech_avail,
                                              technologies={blockdev.CryptoTech.INTEGRITY: (blockdev.CryptoTechMode.CREATE |
                                                                                            blockdev.CryptoTechMode.OPEN_CLOSE |
@@ -395,15 +394,15 @@
 BLOCKDEV_LOOP_ALL_MODES = (blockdev.LoopTechMode.CREATE |
                            blockdev.LoopTechMode.CREATE |
                            blockdev.LoopTechMode.DESTROY |
                            blockdev.LoopTechMode.MODIFY |
                            blockdev.LoopTechMode.QUERY)
 BLOCKDEV_LOOP = BlockDevTechInfo(plugin_name="loop",
                                  check_fn=blockdev.loop_is_tech_avail,
-                                 technologies={blockdev.LoopTech.LOOP_TECH_LOOP: BLOCKDEV_LOOP_ALL_MODES})
+                                 technologies={blockdev.LoopTech.LOOP: BLOCKDEV_LOOP_ALL_MODES})
 BLOCKDEV_LOOP_TECH = BlockDevMethod(BLOCKDEV_LOOP)
 
 # libblockdev lvm plugin required technologies and modes
 BLOCKDEV_LVM_ALL_MODES = (blockdev.LVMTechMode.CREATE |
                           blockdev.LVMTechMode.REMOVE |
                           blockdev.LVMTechMode.MODIFY |
                           blockdev.LVMTechMode.QUERY)
@@ -433,15 +432,15 @@
 # libblockdev mdraid plugin required technologies and modes
 BLOCKDEV_MD_ALL_MODES = (blockdev.MDTechMode.CREATE |
                          blockdev.MDTechMode.DELETE |
                          blockdev.MDTechMode.MODIFY |
                          blockdev.MDTechMode.QUERY)
 BLOCKDEV_MD = BlockDevTechInfo(plugin_name="mdraid",
                                check_fn=blockdev.md_is_tech_avail,
-                               technologies={blockdev.MDTech.MD_TECH_MDRAID: BLOCKDEV_MD_ALL_MODES})
+                               technologies={blockdev.MDTech.MDRAID: BLOCKDEV_MD_ALL_MODES})
 BLOCKDEV_MD_TECH = BlockDevMethod(BLOCKDEV_MD)
 
 # libblockdev mpath plugin required technologies and modes
 BLOCKDEV_MPATH_ALL_MODES = (blockdev.MpathTechMode.MODIFY |
                             blockdev.MpathTechMode.QUERY)
 BLOCKDEV_MPATH = BlockDevTechInfo(plugin_name="mpath",
                                   check_fn=blockdev.mpath_is_tech_avail,
@@ -451,15 +450,15 @@
 # libblockdev swap plugin required technologies and modes
 BLOCKDEV_SWAP_ALL_MODES = (blockdev.SwapTechMode.CREATE |
                            blockdev.SwapTechMode.ACTIVATE_DEACTIVATE |
                            blockdev.SwapTechMode.QUERY |
                            blockdev.SwapTechMode.SET_LABEL)
 BLOCKDEV_SWAP = BlockDevTechInfo(plugin_name="swap",
                                  check_fn=blockdev.swap_is_tech_avail,
-                                 technologies={blockdev.SwapTech.SWAP_TECH_SWAP: BLOCKDEV_SWAP_ALL_MODES})
+                                 technologies={blockdev.SwapTech.SWAP: BLOCKDEV_SWAP_ALL_MODES})
 BLOCKDEV_SWAP_TECH = BlockDevMethod(BLOCKDEV_SWAP)
 
 # libblockdev plugins
 # we can't just check if the plugin is loaded, we also need to make sure
 # that all technologies required by us our supported (some may be missing
 # due to missing dependencies)
 BLOCKDEV_BTRFS_PLUGIN = blockdev_plugin("libblockdev btrfs plugin", BLOCKDEV_BTRFS_TECH)
```

### Comparing `blivet-3.7.1/blivet/tasks/dfresize.py` & `blivet-3.8.0/blivet/tasks/dfresize.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fsck.py` & `blivet-3.8.0/blivet/tasks/fsck.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fsinfo.py` & `blivet-3.8.0/blivet/tasks/fsinfo.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fslabeling.py` & `blivet-3.8.0/blivet/tasks/fslabeling.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fsminsize.py` & `blivet-3.8.0/blivet/tasks/fsminsize.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fsmkfs.py` & `blivet-3.8.0/blivet/tasks/fsmkfs.py`

 * *Files 6% similar despite different names*

```diff
@@ -346,15 +346,18 @@
     ext = availability.MKFS_F2FS_APP
     label_option = "-l"
     nodiscard_option = ["-t", "nodiscard"]
     get_uuid_args = None
 
     @property
     def args(self):
-        return []
+        # Enable the extended node bitmap, this means that we can create more
+        # files and directories without running out of inodes, even if the
+        # available space for metadata is limited.
+        return ["-i"]
 
 
 class UnimplementedFSMkfs(task.UnimplementedTask, FSMkfsTask):
 
     @property
     def can_label(self):
         return False
```

### Comparing `blivet-3.7.1/blivet/tasks/fsmount.py` & `blivet-3.8.0/blivet/tasks/fsmount.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fsreadlabel.py` & `blivet-3.8.0/blivet/tasks/fsreadlabel.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fsresize.py` & `blivet-3.8.0/blivet/tasks/fsresize.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fssize.py` & `blivet-3.8.0/blivet/tasks/fssize.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fssync.py` & `blivet-3.8.0/blivet/tasks/fssync.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fstask.py` & `blivet-3.8.0/blivet/tasks/fstask.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fsuuid.py` & `blivet-3.8.0/blivet/tasks/fsuuid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fswritelabel.py` & `blivet-3.8.0/blivet/tasks/fswritelabel.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/fswriteuuid.py` & `blivet-3.8.0/blivet/tasks/fswriteuuid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tasks/lukstasks.py` & `blivet-3.8.0/blivet/tasks/lukstasks.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # source code or documentation are not subject to the GNU General Public
 # License and may only be used or replicated with the express permission of
 # Red Hat, Inc.
 #
 # Red Hat Author(s): Anne Mulhern <amulhern@redhat.com>
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 from .. import util
 
 from ..devicelibs import crypto
 from ..errors import LUKSError
@@ -83,14 +83,20 @@
         """
         self.luks = a_luks
 
     def do_task(self):  # pylint: disable=arguments-differ
         """ Resizes the LUKS format. """
         try:
             if self.luks.luks_version == "luks2":
+                if self.luks._LUKS__passphrase:
+                    context = blockdev.CryptoKeyslotContext(passphrase=self.luks._LUKS__passphrase)
+                elif self.luks._key_file:
+                    context = blockdev.CryptoKeyslotContext(keyfile=self.luks._key_file)
+                else:
+                    # context for resize can be NULL -- this means the key is already in the keyring
+                    context = None
                 blockdev.crypto.luks_resize(self.luks.map_name, self.luks.target_size.convert_to(self.unit),
-                                            passphrase=self.luks._LUKS__passphrase,
-                                            key_file=self.luks._key_file)
+                                            context=context)
             else:
                 blockdev.crypto.luks_resize(self.luks.map_name, self.luks.target_size.convert_to(self.unit))
         except blockdev.CryptoError as e:
             raise LUKSError(e)
```

### Comparing `blivet-3.7.1/blivet/tasks/pvtask.py` & `blivet-3.8.0/blivet/tasks/pvtask.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # source code or documentation are not subject to the GNU General Public
 # License and may only be used or replicated with the express permission of
 # Red Hat, Inc.
 #
 # Red Hat Author(s): Vojtěch Trefný <vtrefny@redhat.com>
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 from ..errors import PhysicalVolumeError
 from ..size import Size, B
 
 from . import availability
```

### Comparing `blivet-3.7.1/blivet/tasks/task.py` & `blivet-3.8.0/blivet/tasks/task.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/threads.py` & `blivet-3.8.0/blivet/threads.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/tsort.py` & `blivet-3.8.0/blivet/tsort.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/blivet/udev.py` & `blivet-3.8.0/blivet/udev.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import time
 
 from . import util
 from .size import Size
 from .flags import flags
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 global_udev = pyudev.Context()
 log = logging.getLogger("blivet")
 
 ignored_device_names = []
```

### Comparing `blivet-3.7.1/blivet/util.py` & `blivet-3.8.0/blivet/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from collections import namedtuple
 from enum import Enum
 
 from .errors import DependencyError
 from . import safe_dbus
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import six
 
 import logging
 log = logging.getLogger("blivet")
@@ -290,15 +290,20 @@
 
             if path == mountpoint:
                 mount_device = device
                 break
 
     if mount_device and re.match(r'/dev/loop\d+$', mount_device):
         loop_name = os.path.basename(mount_device)
-        mount_device = blockdev.loop.get_backing_file(loop_name)
+        try:
+            info = blockdev.loop.info(loop_name)
+        except blockdev.LoopError as e:
+            log.warning("failed to get loop info for %s: %s", loop_name, str(e))
+            return None
+        mount_device = info.backing_file
         log.debug("found backing file %s for loop device %s", mount_device,
                   loop_name)
 
     if mount_device:
         log.debug("%s is mounted on %s", mount_device, mountpoint)
 
     return mount_device
```

### Comparing `blivet-3.7.1/blivet/zfcp.py` & `blivet-3.8.0/blivet/zfcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import glob
 from . import udev
 from . import util
 from .i18n import _
 from .util import stringize, unicodeize
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 import logging
 log = logging.getLogger("blivet")
```

### Comparing `blivet-3.7.1/blivet.egg-info/PKG-INFO` & `blivet-3.8.0/blivet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: blivet
-Version: 3.7.1
+Version: 3.8.0
 Summary: Python module for system storage configuration
 Home-page: http://github.com/storaged-project/blivet
 Author: David Lehman
 Author-email: dlehman@redhat.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 
 Blivet is a python module for system storage configuration.
```

### Comparing `blivet-3.7.1/blivet.egg-info/SOURCES.txt` & `blivet-3.8.0/blivet.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 .gitignore
 .gitmodules
 .packit.yaml
 CONTRIBUTING
 COPYING
 COPYING.LESSER
+ChangeLog
 MANIFEST.in
 Makefile
 README.md
 TODO
 python-blivet.spec
 release_notes.rst
 setup.py
 .github/workflows/anaconda_tests.yml
 .github/workflows/check.yml
-.github/workflows/unit_tests.yml
 blivet/__init__.py
 blivet/actionlist.py
 blivet/arch.py
 blivet/blivet.py
 blivet/callbacks.py
 blivet/deviceaction.py
 blivet/devicefactory.py
@@ -334,14 +334,15 @@
 tests/run_tests.py
 tests/skip.yml
 tests/pylint/censorship.py
 tests/pylint/pylintrc
 tests/pylint/runpylint.py
 tests/storage_tests/__init__.py
 tests/storage_tests/imagebackedtestcase.py
+tests/storage_tests/iscsi_test.py
 tests/storage_tests/partitioning_test.py
 tests/storage_tests/storagetestcase.py
 tests/storage_tests/unsupported_disklabel_test.py
 tests/storage_tests/devices_test/__init__.py
 tests/storage_tests/devices_test/lvm_test.py
 tests/storage_tests/devices_test/partition_test.py
 tests/storage_tests/devices_test/stratis_test.py
@@ -929,14 +930,15 @@
 tests/unit_tests/devices_test/partition_test.py
 tests/unit_tests/devices_test/stratis_test.py
 tests/unit_tests/formats_tests/__init__.py
 tests/unit_tests/formats_tests/device_test.py
 tests/unit_tests/formats_tests/disklabel_test.py
 tests/unit_tests/formats_tests/init_test.py
 tests/unit_tests/formats_tests/luks_test.py
+tests/unit_tests/formats_tests/lvmpv_test.py
 tests/unit_tests/formats_tests/methods_test.py
 tests/unit_tests/formats_tests/misc_test.py
 tests/unit_tests/formats_tests/selinux_test.py
 tests/unit_tests/formats_tests/swap_test.py
 tests/unit_tests/udev_data/__init__.py
 tests/unit_tests/udev_data/raid_data.py
 tests/vmtests/README.rst
```

### Comparing `blivet-3.7.1/doc/Makefile` & `blivet-3.8.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/doc/_inheritance.rst` & `blivet-3.8.0/doc/_inheritance.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/doc/api/blivet.rst` & `blivet-3.8.0/doc/api/blivet.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/doc/api/devices.rst` & `blivet-3.8.0/doc/api/devices.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/doc/api/formats.rst` & `blivet-3.8.0/doc/api/formats.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/doc/api.rst` & `blivet-3.8.0/doc/api.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/doc/conf.py` & `blivet-3.8.0/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 copyright = '2013-2023, Red Hat, Inc.'     # pylint: disable=redefined-builtin
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '3.7.1'
+version = '3.8.0'
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
```

### Comparing `blivet-3.7.1/doc/dbus.rst` & `blivet-3.8.0/doc/dbus.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/doc/index.rst` & `blivet-3.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/doc/intro.rst` & `blivet-3.8.0/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/doc/lvmvdo.rst` & `blivet-3.8.0/doc/lvmvdo.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/actions.py` & `blivet-3.8.0/examples/actions.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/dbus_client.py` & `blivet-3.8.0/examples/dbus_client.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/factory.py` & `blivet-3.8.0/examples/factory.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/lvm.py` & `blivet-3.8.0/examples/lvm.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/lvm_cache.py` & `blivet-3.8.0/examples/lvm_cache.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/lvm_cachepool.py` & `blivet-3.8.0/examples/lvm_cachepool.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/lvm_non_linear.py` & `blivet-3.8.0/examples/lvm_non_linear.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/lvm_thin.py` & `blivet-3.8.0/examples/lvm_thin.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/lvm_vdo.py` & `blivet-3.8.0/examples/lvm_vdo.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/partitioning.py` & `blivet-3.8.0/examples/partitioning.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/stratis.py` & `blivet-3.8.0/examples/stratis.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/examples/uevents.py` & `blivet-3.8.0/examples/uevents.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/misc/Vagrantfile` & `blivet-3.8.0/misc/Vagrantfile`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/misc/install-test-dependencies.yml` & `blivet-3.8.0/misc/install-test-dependencies.yml`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         - python3-pyparted
         - libselinux-python3
         - python3-blockdev
         - python3-bytesize
         - python3-libvirt
         - python3-paramiko
         - targetcli
+        - iscsi-initiator-utils
     when: ansible_distribution == 'Fedora'
 
 ####### CentOS 8/9
   - name: Install basic build tools (CentOS)
     package: name=make state=present
     when: ansible_distribution == 'CentOS'
 
@@ -100,14 +101,15 @@
         - python3-pyparted
         - libselinux-python3
         - python3-blockdev
         - python3-bytesize
         - python3-libvirt
         - python3-pip
         - targetcli
+        - iscsi-initiator-utils
     when: ansible_distribution == 'CentOS' and ansible_distribution_major_version == '8'
 
   - name: Install paramiko using pip (not available in EPEL yet) (CentOS 9)
     pip: name=paramiko executable=pip3
     when: ansible_distribution == 'CentOS' and ansible_distribution_major_version == '9'
 
   - name: Install pocketlint using pip (CentOS)
@@ -154,12 +156,13 @@
         - gettext
         - python3-polib
         - python3-paramiko
         - python3-bugzilla
         - python3-libvirt
         - python3-pip
         - targetcli-fb
+        - open-iscsi
     when: ansible_distribution == 'Debian' or ansible_distribution == 'Ubuntu'
 
   - name: Install pocketlint using pip (Debian/Ubuntu)
     pip: name=pocketlint executable=pip3
     when: ansible_distribution == 'Debian' or ansible_distribution == 'Ubuntu'
```

### Comparing `blivet-3.7.1/po/Makefile` & `blivet-3.8.0/po/Makefile`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/af.mo` & `blivet-3.8.0/po/af.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/af.po` & `blivet-3.8.0/po/af.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/am.mo` & `blivet-3.8.0/po/am.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/am.po` & `blivet-3.8.0/po/am.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ar.mo` & `blivet-3.8.0/po/ar.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ar.po` & `blivet-3.8.0/po/ar.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/as.mo` & `blivet-3.8.0/po/as.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/as.po` & `blivet-3.8.0/po/as.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ast.mo` & `blivet-3.8.0/po/ast.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ast.po` & `blivet-3.8.0/po/ast.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/bg.mo` & `blivet-3.8.0/po/bg.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/bg.po` & `blivet-3.8.0/po/bg.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/blivet.pot` & `blivet-3.8.0/po/blivet.pot`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/bn.mo` & `blivet-3.8.0/po/bn.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/bn.po` & `blivet-3.8.0/po/bn.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/bn_IN.mo` & `blivet-3.8.0/po/bn_IN.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/bn_IN.po` & `blivet-3.8.0/po/bn_IN.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/bs.mo` & `blivet-3.8.0/po/bs.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/bs.po` & `blivet-3.8.0/po/bs.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ca.mo` & `blivet-3.8.0/po/ca.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ca.po` & `blivet-3.8.0/po/ca.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/cs.mo` & `blivet-3.8.0/po/cs.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2021-12-03 22:16+0000\n"
-"Last-Translator: Pavel Borecki <pavel.borecki@gmail.com>\n"
+"PO-Revision-Date: 2023-04-17 11:20+0000\n"
+"Last-Translator: Jan Kalabza <jan.kalabza@gmail.com>\n"
 "Language-Team: Czech <https://translate.fedoraproject.org/projects/blivet/"
 "blivet-master/cs/>\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
-"X-Generator: Weblate 4.9.1\n"
+"X-Generator: Weblate 4.15.2\n"
 
 msgid ""
 "All parent devices must be selected when choosing exclusive or ignored disks "
 "for a multipath or firmware RAID device."
 msgstr ""
 "Pokud jsou zvoleny výhradní nebo ignorované disky pro multipath zařízení "
 "nebo to z RAID pole hw radiče, je třeba vybrat všechna nadřazená zařízení."
@@ -42,14 +42,17 @@
 msgid ""
 "Could not correctly delete SCSI device of zFCP %(devnum)s %(wwpn)s "
 "%(fcplun)s (%(e)s)."
 msgstr ""
 "Nelze korektně smazat SCSI zařízení z zFCP %(devnum)s %(wwpn)s %(fcplun)s "
 "(%(e)s)."
 
+msgid "Could not correctly delete SCSI device of zFCP %(zfcpdev)s (%(e)s)."
+msgstr "Nelze korektně smazat SCSI zařízení ze zFCP %(zfcpdev)s (%(e)s)."
+
 msgid "Could not log in to any of the discovered nodes"
 msgstr "K žádnému nalezenému nodu se nelze přihlásit"
 
 msgid ""
 "Could not read failed attribute of LUN %(fcplun)s at WWPN %(wwpn)s on zFCP "
 "device %(devnum)s (%(e)s)."
 msgstr ""
@@ -190,14 +193,17 @@
 
 msgid "Resized filesystem on %(device)s"
 msgstr "Změna velikosti systému souborů na %(device)s"
 
 msgid "Resizing filesystem on %(device)s"
 msgstr "Změna velikosti systému souborů na %(device)s"
 
+msgid "Stratis block device"
+msgstr "Stratis blokové zařízení"
+
 msgid ""
 "This is usually caused by cloning the device image resulting in duplication "
 "of the UUID value which should be unique. In that case you can either "
 "disconnect one of the devices or reformat it."
 msgstr ""
 "Toto je obvykle způsobeno klonování obrazu zařízení, což má za následek "
 "vícero výskytů hodnoty nikde se neopakující identifikátoru (UUID), který by "
@@ -316,10 +322,13 @@
 
 msgid "software RAID"
 msgstr "softwarový RAID"
 
 msgid "unable to allocate aligned partition"
 msgstr "nelze přidělit zarovnaný oddíl"
 
+msgid "zFCP device %s cannot use auto LUN scan."
+msgstr "zFCP zařízení %s nemůže použít automatický LUN sken."
+
 msgid "zFCP device %s not found, not even in device ignore list."
 msgstr ""
 "zFCP zařízení %s nenalezeno, dokonce ani v seznamu ignorovaných zařízení."
```

### Comparing `blivet-3.7.1/po/cs.po` & `blivet-3.8.0/po/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,31 @@
 # Marcel Telka <marcel@telka.sk>, 2003-2004
 # Milan Kerslager <milan@kerslager.cz>, 2009-2010
 # Milan Kerslager <milan.kerslager@pslib.cz>, 2011
 # Zdenek <chmelarz@gmail.com>, 2015. #zanata
 # Zdenek <chmelarz@gmail.com>, 2016. #zanata
 # Zdenek <chmelarz@gmail.com>, 2018. #zanata
 # Zdenek <chmelarz@gmail.com>, 2019. #zanata
-# Pavel Borecki <pavel.borecki@gmail.com>, 2021.
+# Pavel Borecki <pavel.borecki@gmail.com>, 2021, 2023.
+# Jan Kalabza <jan.kalabza@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-09 13:31+0100\n"
-"PO-Revision-Date: 2021-12-03 22:16+0000\n"
-"Last-Translator: Pavel Borecki <pavel.borecki@gmail.com>\n"
+"PO-Revision-Date: 2023-04-17 11:20+0000\n"
+"Last-Translator: Jan Kalabza <jan.kalabza@gmail.com>\n"
 "Language-Team: Czech <https://translate.fedoraproject.org/projects/blivet/"
 "blivet-master/cs/>\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
-"X-Generator: Weblate 4.9.1\n"
+"X-Generator: Weblate 4.15.2\n"
 
 #: ../blivet/deviceaction.py:197
 #, python-format
 msgid "Executing %(action)s"
 msgstr "Provádí se %(action)s"
 
 #: ../blivet/deviceaction.py:325
@@ -349,25 +350,20 @@
 #, python-format
 msgid "Could not remove WWPN %(wwpn)s on zFCP device %(devnum)s (%(e)s)."
 msgstr "Nelze odebrat WWPN %(wwpn)s na zFCP zařízení %(devnum)s (%(e)s)."
 
 #: ../blivet/zfcp.py:418
 #, python-format
 msgid "zFCP device %s cannot use auto LUN scan."
-msgstr ""
+msgstr "zFCP zařízení %s nemůže použít automatický LUN sken."
 
 #: ../blivet/zfcp.py:432
-#, fuzzy, python-format
-#| msgid ""
-#| "Could not correctly delete SCSI device of zFCP %(devnum)s %(wwpn)s "
-#| "%(fcplun)s (%(e)s)."
+#, python-format
 msgid "Could not correctly delete SCSI device of zFCP %(zfcpdev)s (%(e)s)."
-msgstr ""
-"Nelze korektně smazat SCSI zařízení z zFCP %(devnum)s %(wwpn)s %(fcplun)s "
-"(%(e)s)."
+msgstr "Nelze korektně smazat SCSI zařízení ze zFCP %(zfcpdev)s (%(e)s)."
 
 #: ../blivet/devicelibs/lvm.py:68
 msgid "Generic"
 msgstr "Obecný"
 
 #: ../blivet/devicelibs/lvm.py:69
 msgid "Performance"
@@ -463,11 +459,9 @@
 msgstr "člen zařízení multipath"
 
 #: ../blivet/formats/prepboot.py:37
 msgid "PPC PReP Boot"
 msgstr "PPC PReP Boot"
 
 #: ../blivet/formats/stratis.py:40
-#, fuzzy
-#| msgid "create device"
 msgid "Stratis block device"
-msgstr "vytvořit zařízení"
+msgstr "Stratis blokové zařízení"
```

### Comparing `blivet-3.7.1/po/cy.mo` & `blivet-3.8.0/po/cy.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/cy.po` & `blivet-3.8.0/po/cy.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/da.mo` & `blivet-3.8.0/po/da.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/da.po` & `blivet-3.8.0/po/da.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/de.mo` & `blivet-3.8.0/po/de.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/de.po` & `blivet-3.8.0/po/de.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/de_CH.mo` & `blivet-3.8.0/po/de_CH.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/de_CH.po` & `blivet-3.8.0/po/de_CH.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/el.mo` & `blivet-3.8.0/po/el.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/el.po` & `blivet-3.8.0/po/el.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/en_GB.mo` & `blivet-3.8.0/po/en_GB.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/en_GB.po` & `blivet-3.8.0/po/en_GB.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/es.mo` & `blivet-3.8.0/po/es.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/es.po` & `blivet-3.8.0/po/es.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/et.mo` & `blivet-3.8.0/po/et.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/et.po` & `blivet-3.8.0/po/et.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/eu.mo` & `blivet-3.8.0/po/eu.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/eu.po` & `blivet-3.8.0/po/eu.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/fa.mo` & `blivet-3.8.0/po/fa.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/fa.po` & `blivet-3.8.0/po/fa.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/fi.mo` & `blivet-3.8.0/po/fi.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/fi.po` & `blivet-3.8.0/po/fi.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/fr.mo` & `blivet-3.8.0/po/fr.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/fr.po` & `blivet-3.8.0/po/fr.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/fur.mo` & `blivet-3.8.0/po/fur.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/fur.po` & `blivet-3.8.0/po/fur.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/gu.mo` & `blivet-3.8.0/po/gu.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/gu.po` & `blivet-3.8.0/po/gu.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/he.mo` & `blivet-3.8.0/po/he.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/he.po` & `blivet-3.8.0/po/he.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/hi.mo` & `blivet-3.8.0/po/hi.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/hi.po` & `blivet-3.8.0/po/hi.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/hr.mo` & `blivet-3.8.0/po/hr.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/hr.po` & `blivet-3.8.0/po/hr.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/hu.mo` & `blivet-3.8.0/po/hu.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2021-11-04 22:05+0000\n"
-"Last-Translator: Balázs Meskó <meskobalazs@mailbox.org>\n"
+"PO-Revision-Date: 2023-05-12 18:21+0000\n"
+"Last-Translator: Dankaházi (ifj.) István <dankahazi.istvan@gmail.com>\n"
 "Language-Team: Hungarian <https://translate.fedoraproject.org/projects/"
 "blivet/blivet-master/hu/>\n"
 "Language: hu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.8\n"
+"X-Generator: Weblate 4.15.2\n"
 
 msgid ""
 "All parent devices must be selected when choosing exclusive or ignored disks "
 "for a multipath or firmware RAID device."
 msgstr ""
 "A többutas vagy firmware RAID-eszköz kizárólagos vagy figyelmen kívül "
 "hagyott lemezeinek kiválasztásakor minden szülőeszközt ki kell választani."
@@ -26,41 +26,29 @@
 msgid "BIOS Boot"
 msgstr "BIOS indító"
 
 msgid "Cannot remove a member from existing %s array"
 msgstr "Nem távolítható el tag a létező %s tömbből"
 
 msgid ""
-"Could not add LUN %(fcplun)s to WWPN %(wwpn)s on zFCP device %(devnum)s "
-"(%(e)s)."
-msgstr ""
-"A(z) %(fcplun)s LUN nem adható hozzá a(z) %(wwpn)s WWPN zFCP eszközhöz: "
-"%(devnum)s (%(e)s)."
-
-msgid "Could not add WWPN %(wwpn)s to zFCP device %(devnum)s (%(e)s)."
-msgstr ""
-"Hiba: Nem lehet %(wwpn)s WWPN-t hozzáadni a zFCP eszközhöz: %(devnum)s "
-"(%(e)s)."
-
-msgid ""
 "Could not correctly delete SCSI device of zFCP %(devnum)s %(wwpn)s "
 "%(fcplun)s (%(e)s)."
 msgstr ""
 "A SCSI eszköz nem törölhető helyesen: zFCP %(devnum)s %(wwpn)s %(fcplun)s "
 "(%(e)s)."
 
 msgid "Could not log in to any of the discovered nodes"
 msgstr "Nem lehet bejelentkezni egyik felfedezett csomópontra sem"
 
 msgid ""
 "Could not read failed attribute of LUN %(fcplun)s at WWPN %(wwpn)s on zFCP "
 "device %(devnum)s (%(e)s)."
 msgstr ""
-"Nem sikerült a hibás %(fcplun)s LUN attribútum kiolvasása a(z) %(wwpn)s WWPN-"
-"en, a(z) %(devnum)s zFCP eszközön (%(e)s)."
+"%(fcplun)sNem sikerült a hibás %(fcplun)s LUN attribútum kiolvasása a(z) "
+"%(wwpn)s WWPN-en, a(z) %(devnum)s zFCP eszközön (%(e)s)."
 
 msgid ""
 "Could not remove LUN %(fcplun)s at WWPN %(wwpn)s on zFCP device %(devnum)s "
 "(%(e)s)."
 msgstr ""
 "A(z) %(fcplun)s LUN nem távolítható el a(z) %(wwpn)s WWPN-en, a(z) "
 "%(devnum)s zFCP eszközön (%(e)s)."
@@ -119,15 +107,15 @@
 msgid ""
 "For some reason we were unable to locate a disklabel on a disk that the "
 "kernel is reporting partitions on. It is unclear what the exact problem is. "
 "Please file a bug at http://bugzilla.redhat.com"
 msgstr ""
 "Valamiért nem sikerült megtalálni a lemezcímkét egy lemezen, amelyen a "
 "kernel partíciókat jelent. Nem világos, hogy mi a pontos probléma. Jelentse "
-"be a hibát a http://bugzilla.redhat.com oldalon."
+"be a hibát a http://bugzilla.redhat.com oldalon"
 
 msgid "Generic"
 msgstr "Általános"
 
 msgid "LUKS"
 msgstr "LUKS"
```

### Comparing `blivet-3.7.1/po/hu.po` & `blivet-3.8.0/po/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 # Máté Gelei <mate@geleimate.com>, 2012
 # Peter Borsa <peter.borsa@gmail.com>, 2011-2012
 # Peter Bojtos <ptr@ulx.hu>, 2011-2012
 # Zoltan Hoppár <zoltanh721@fedoraproject.org>, 2011-2013
 # Meskó Balázs <meskobalazs@gmail.com>, 2018. #zanata
 # Meskó Balázs <meskobalazs@gmail.com>, 2019. #zanata
 # Balázs Meskó <meskobalazs@mailbox.org>, 2020, 2021.
+# Dankaházi (ifj.) István <dankahazi.istvan@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-09 13:31+0100\n"
-"PO-Revision-Date: 2021-11-04 22:05+0000\n"
-"Last-Translator: Balázs Meskó <meskobalazs@mailbox.org>\n"
+"PO-Revision-Date: 2023-05-12 18:21+0000\n"
+"Last-Translator: Dankaházi (ifj.) István <dankahazi.istvan@gmail.com>\n"
 "Language-Team: Hungarian <https://translate.fedoraproject.org/projects/"
 "blivet/blivet-master/hu/>\n"
 "Language: hu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.8\n"
+"X-Generator: Weblate 4.15.2\n"
 
 #: ../blivet/deviceaction.py:197
 #, python-format
 msgid "Executing %(action)s"
 msgstr "%(action)s végrehajtása"
 
 #: ../blivet/deviceaction.py:325
@@ -118,15 +119,15 @@
 msgid ""
 "For some reason we were unable to locate a disklabel on a disk that the "
 "kernel is reporting partitions on. It is unclear what the exact problem is. "
 "Please file a bug at http://bugzilla.redhat.com"
 msgstr ""
 "Valamiért nem sikerült megtalálni a lemezcímkét egy lemezen, amelyen a "
 "kernel partíciókat jelent. Nem világos, hogy mi a pontos probléma. Jelentse "
-"be a hibát a http://bugzilla.redhat.com oldalon."
+"be a hibát a http://bugzilla.redhat.com oldalon"
 
 #: ../blivet/errors.py:237
 msgid ""
 "Either restore the disklabel to a completely working state or remove it "
 "completely.\n"
 "Hint: parted can restore it or wipefs can remove it."
 msgstr ""
@@ -281,34 +282,33 @@
 msgstr "Nem adott meg WWPN port nevet, vagy a név érvénytelen."
 
 #: ../blivet/zfcp.py:222
 msgid "You have not specified a FCP LUN or the number is invalid."
 msgstr "Nem adott meg FCP LUN számot, vagy a szám érvénytelen."
 
 #: ../blivet/zfcp.py:268
-#, python-format
+#, fuzzy, python-format
 msgid "Could not add WWPN %(wwpn)s to zFCP device %(devnum)s (%(e)s)."
 msgstr ""
-"Hiba: Nem lehet %(wwpn)s WWPN-t hozzáadni a zFCP eszközhöz: %(devnum)s "
-"(%(e)s)."
+"Nem sikerült hozzáadni a %(wwpn)s WWPN-t a %(devnum)s (%(e)s) zFCP-eszközhöz."
 
 #. newer zfcp sysfs interface with auto port scan
 #: ../blivet/zfcp.py:275
 #, python-format
 msgid "WWPN %(wwpn)s not found at zFCP device %(devnum)s."
 msgstr "%(wwpn)s WWPN nem található az zFCP eszközben: %(devnum)s."
 
 #: ../blivet/zfcp.py:291
-#, python-format
+#, fuzzy, python-format
 msgid ""
 "Could not add LUN %(fcplun)s to WWPN %(wwpn)s on zFCP device %(devnum)s "
 "(%(e)s)."
 msgstr ""
-"A(z) %(fcplun)s LUN nem adható hozzá a(z) %(wwpn)s WWPN zFCP eszközhöz: "
-"%(devnum)s (%(e)s)."
+"Nem sikerült hozzáadni a LUN %(fcplun)s-t a WWPN %(wwpn)s-hez a zFCP-"
+"eszközön %(devnum)s (%(e)s)."
 
 #: ../blivet/zfcp.py:297
 #, python-format
 msgid ""
 "LUN %(fcplun)s at WWPN %(wwpn)s on zFCP device %(devnum)s already configured."
 msgstr ""
 "A(z) %(fcplun)s LUN a(z) %(wwpn)s WWPN már be lett állítva a zFCP eszközön: "
@@ -316,16 +316,16 @@
 
 #: ../blivet/zfcp.py:310
 #, python-format
 msgid ""
 "Could not read failed attribute of LUN %(fcplun)s at WWPN %(wwpn)s on zFCP "
 "device %(devnum)s (%(e)s)."
 msgstr ""
-"Nem sikerült a hibás %(fcplun)s LUN attribútum kiolvasása a(z) %(wwpn)s WWPN-"
-"en, a(z) %(devnum)s zFCP eszközön (%(e)s)."
+"%(fcplun)sNem sikerült a hibás %(fcplun)s LUN attribútum kiolvasása a(z) "
+"%(wwpn)s WWPN-en, a(z) %(devnum)s zFCP eszközön (%(e)s)."
 
 #: ../blivet/zfcp.py:319
 #, python-format
 msgid ""
 "Failed LUN %(fcplun)s at WWPN %(wwpn)s on zFCP device %(devnum)s removed "
 "again."
 msgstr ""
```

### Comparing `blivet-3.7.1/po/ia.mo` & `blivet-3.8.0/po/ia.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ia.po` & `blivet-3.8.0/po/ia.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/id.mo` & `blivet-3.8.0/po/id.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/id.po` & `blivet-3.8.0/po/id.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ilo.mo` & `blivet-3.8.0/po/ilo.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ilo.po` & `blivet-3.8.0/po/ilo.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/is.mo` & `blivet-3.8.0/po/is.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/is.po` & `blivet-3.8.0/po/is.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/it.mo` & `blivet-3.8.0/po/it.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/it.po` & `blivet-3.8.0/po/it.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ja.mo` & `blivet-3.8.0/po/ja.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ja.po` & `blivet-3.8.0/po/ja.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ka.mo` & `blivet-3.8.0/po/ka.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ka.po` & `blivet-3.8.0/po/ka.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/kk.mo` & `blivet-3.8.0/po/kk.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/kk.po` & `blivet-3.8.0/po/kk.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/kn.mo` & `blivet-3.8.0/po/kn.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/kn.po` & `blivet-3.8.0/po/kn.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ko.mo` & `blivet-3.8.0/po/ko.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ko.po` & `blivet-3.8.0/po/ko.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/lv.mo` & `blivet-3.8.0/po/lv.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/lv.po` & `blivet-3.8.0/po/lv.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/mai.mo` & `blivet-3.8.0/po/mai.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/mai.po` & `blivet-3.8.0/po/mai.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/mk.mo` & `blivet-3.8.0/po/mk.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/mk.po` & `blivet-3.8.0/po/mk.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ml.mo` & `blivet-3.8.0/po/ml.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ml.po` & `blivet-3.8.0/po/ml.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/mr.mo` & `blivet-3.8.0/po/mr.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/mr.po` & `blivet-3.8.0/po/mr.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ms.mo` & `blivet-3.8.0/po/ms.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ms.po` & `blivet-3.8.0/po/ms.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/nb.mo` & `blivet-3.8.0/po/nb.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/nb.po` & `blivet-3.8.0/po/nb.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ne.mo` & `blivet-3.8.0/po/ne.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ne.po` & `blivet-3.8.0/po/ne.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/nl.mo` & `blivet-3.8.0/po/nl.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,29 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-10-02 15:19+0000\n"
-"Last-Translator: Vanhoorne Michael <michaeltjevanhoorne@gmail.com>\n"
+"PO-Revision-Date: 2023-06-11 13:20+0000\n"
+"Last-Translator: Geert Warrink <geert.warrink@onsnet.nu>\n"
 "Language-Team: Dutch <https://translate.fedoraproject.org/projects/blivet/"
 "blivet-master/nl/>\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1\n"
+"X-Generator: Weblate 4.17\n"
+
+msgid ""
+"All parent devices must be selected when choosing exclusive or ignored disks "
+"for a multipath or firmware RAID device."
+msgstr ""
+"Alle bovenliggende apparaten moeten worden geselecteerd bij het kiezen van "
+"exclusieve of genegeerde schijven voor een multipath- of firmware-RAID-"
+"apparaat."
 
 msgid "Apple Bootstrap"
 msgstr "Apple Bootstrap"
 
 msgid "BIOS Boot"
 msgstr "BIOS Boot"
 
@@ -35,14 +43,18 @@
 msgid ""
 "Could not correctly delete SCSI device of zFCP %(devnum)s %(wwpn)s "
 "%(fcplun)s (%(e)s)."
 msgstr ""
 "Kon SCSI apparaat van zFCP %(devnum)s %(wwpn)s %(fcplun)s niet correct "
 "verwijderen (%(e)s)."
 
+msgid "Could not correctly delete SCSI device of zFCP %(zfcpdev)s (%(e)s)."
+msgstr ""
+"Kon SCSI apparaat van zFCP %(zfcpdev)s niet correct verwijderen (%(e)s)."
+
 msgid "Could not log in to any of the discovered nodes"
 msgstr "Kon op geen van de ontdekte nodes inloggen"
 
 msgid ""
 "Could not read failed attribute of LUN %(fcplun)s at WWPN %(wwpn)s on zFCP "
 "device %(devnum)s (%(e)s)."
 msgstr ""
@@ -182,14 +194,17 @@
 
 msgid "Resized filesystem on %(device)s"
 msgstr "In grootte veranderd bestandssysteem op %(device)s"
 
 msgid "Resizing filesystem on %(device)s"
 msgstr "Grootte van bestandssysteem op %(device)s wordt veranderd"
 
+msgid "Stratis block device"
+msgstr "Stratis blokapparaat"
+
 msgid ""
 "This is usually caused by cloning the device image resulting in duplication "
 "of the UUID value which should be unique. In that case you can either "
 "disconnect one of the devices or reformat it."
 msgstr ""
 "Dit wordt meestal veroorzaakt door het klonen van de apparaat-image,wat "
 "resulteert in duplicatie van de UUID-waarde, die uniek moet zijn. In dat "
@@ -248,14 +263,17 @@
 
 msgid "disk %s inaccessible"
 msgstr "schijf %s is niet toegankelijk"
 
 msgid "dm-raid member device"
 msgstr "dm-raid lidapparaat"
 
+msgid "failed to add partition to disk: %s"
+msgstr "kon partitie niet toevoegen aan schijf: %s"
+
 msgid "failed to allocate aligned partition"
 msgstr "kan uitgelijnde partitie niet toekennen"
 
 msgid "iSCSI not available"
 msgstr "iSCSI niet beschikbaar"
 
 msgid "multipath member device"
```

### Comparing `blivet-3.7.1/po/nl.po` & `blivet-3.8.0/po/nl.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 # Arjan van de Ven <arjanv@redhat.com>, 2001
 # Dimitris Glezos <glezos@indifex.com>, 2011
-# Geert Warrink <geert.warrink@onsnet.nu>, 2009,2011-2012
+# Geert Warrink <geert.warrink@onsnet.nu>, 2009,2011-2012, 2023.
 # Peter van Egdom <p.van.egdom@gmail.com>, 2002
 # Richard E. van der Luit <nippur@fedoraproject.org>, 2012
 # Tino Meinen <a.t.meinen@chello.nl>, 2002-2003
-# Geert Warrink <geert.warrink@onsnet.nu>, 2015. #zanata
-# Geert Warrink <geert.warrink@onsnet.nu>, 2016. #zanata
-# Geert Warrink <geert.warrink@onsnet.nu>, 2018. #zanata
-# Geert Warrink <geert.warrink@onsnet.nu>, 2019. #zanata
-# Vanhoorne Michael <michaeltjevanhoorne@gmail.com>, 2022.
+# Geert Warrink <geert.warrink@onsnet.nu>, 2015. #zanata, 2023.
+# Geert Warrink <geert.warrink@onsnet.nu>, 2016. #zanata, 2023.
+# Geert Warrink <geert.warrink@onsnet.nu>, 2018. #zanata, 2023.
+# Geert Warrink <geert.warrink@onsnet.nu>, 2019. #zanata, 2023.
+# Vanhoorne Michael <michaeltjevanhoorne@gmail.com>, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-09 13:31+0100\n"
-"PO-Revision-Date: 2022-10-02 15:19+0000\n"
-"Last-Translator: Vanhoorne Michael <michaeltjevanhoorne@gmail.com>\n"
+"PO-Revision-Date: 2023-06-11 13:20+0000\n"
+"Last-Translator: Geert Warrink <geert.warrink@onsnet.nu>\n"
 "Language-Team: Dutch <https://translate.fedoraproject.org/projects/blivet/"
 "blivet-master/nl/>\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1\n"
+"X-Generator: Weblate 4.17\n"
 
 #: ../blivet/deviceaction.py:197
 #, python-format
 msgid "Executing %(action)s"
 msgstr "UItvoeren van %(action)s"
 
 #: ../blivet/deviceaction.py:325
@@ -143,14 +143,17 @@
 "Hint 2: Je kunt de VG UUID's krijgen met het uitvoeren van 'pvs -o +vg_uuid'."
 
 #: ../blivet/errors.py:251
 msgid ""
 "All parent devices must be selected when choosing exclusive or ignored disks "
 "for a multipath or firmware RAID device."
 msgstr ""
+"Alle bovenliggende apparaten moeten worden geselecteerd bij het kiezen van "
+"exclusieve of genegeerde schijven voor een multipath- of firmware-RAID-"
+"apparaat."
 
 #: ../blivet/fcoe.py:122
 msgid "FCoE not available"
 msgstr "FCoE niet beschikbaar"
 
 #: ../blivet/iscsi.py:216
 msgid "Unable to change iSCSI initiator name once set"
@@ -185,18 +188,17 @@
 msgstr "kan uitgelijnde partitie niet toekennen"
 
 #: ../blivet/partitioning.py:463
 msgid "requested size exceeds maximum allowed"
 msgstr "aangevraagd grootte overschrijdt het toegestane maximum"
 
 #: ../blivet/partitioning.py:475
-#, fuzzy, python-format
-#| msgid "failed to allocate aligned partition"
+#, python-format
 msgid "failed to add partition to disk: %s"
-msgstr "kan uitgelijnde partitie niet toekennen"
+msgstr "kon partitie niet toevoegen aan schijf: %s"
 
 #: ../blivet/partitioning.py:586
 #, python-format
 msgid "disk %s inaccessible"
 msgstr "schijf %s is niet toegankelijk"
 
 #: ../blivet/partitioning.py:647
@@ -353,22 +355,18 @@
 
 #: ../blivet/zfcp.py:418
 #, python-format
 msgid "zFCP device %s cannot use auto LUN scan."
 msgstr "zCFP apparaat %s kan niet automatische LUN scan."
 
 #: ../blivet/zfcp.py:432
-#, fuzzy, python-format
-#| msgid ""
-#| "Could not correctly delete SCSI device of zFCP %(devnum)s %(wwpn)s "
-#| "%(fcplun)s (%(e)s)."
+#, python-format
 msgid "Could not correctly delete SCSI device of zFCP %(zfcpdev)s (%(e)s)."
 msgstr ""
-"Kon SCSI apparaat van zFCP %(devnum)s %(wwpn)s %(fcplun)s niet correct "
-"verwijderen (%(e)s)."
+"Kon SCSI apparaat van zFCP %(zfcpdev)s niet correct verwijderen (%(e)s)."
 
 #: ../blivet/devicelibs/lvm.py:68
 msgid "Generic"
 msgstr "Generiek"
 
 #: ../blivet/devicelibs/lvm.py:69
 msgid "Performance"
@@ -461,11 +459,9 @@
 msgstr "multipad lidapparaat"
 
 #: ../blivet/formats/prepboot.py:37
 msgid "PPC PReP Boot"
 msgstr "PPC PReP Boot"
 
 #: ../blivet/formats/stratis.py:40
-#, fuzzy
-#| msgid "create device"
 msgid "Stratis block device"
-msgstr "aanmaken van apparaat"
+msgstr "Stratis blokapparaat"
```

### Comparing `blivet-3.7.1/po/nso.mo` & `blivet-3.8.0/po/nso.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/nso.po` & `blivet-3.8.0/po/nso.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/or.mo` & `blivet-3.8.0/po/or.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/or.po` & `blivet-3.8.0/po/or.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/pa.mo` & `blivet-3.8.0/po/pa.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/pa.po` & `blivet-3.8.0/po/pa.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/pl.mo` & `blivet-3.8.0/po/pl.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/pl.po` & `blivet-3.8.0/po/pl.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/pt.mo` & `blivet-3.8.0/po/pt.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-03-25 13:16+0000\n"
-"Last-Translator: Hugo Carvalho <hugokarvalho@hotmail.com>\n"
+"PO-Revision-Date: 2023-04-07 05:20+0000\n"
+"Last-Translator: Felipe Nogueira <contato.fnog@gmail.com>\n"
 "Language-Team: Portuguese <https://translate.fedoraproject.org/projects/"
 "blivet/blivet-master/pt/>\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Weblate 4.11.2\n"
+"X-Generator: Weblate 4.15.2\n"
 
 msgid ""
 "All parent devices must be selected when choosing exclusive or ignored disks "
 "for a multipath or firmware RAID device."
 msgstr ""
 "Todos os dispositivos principais devem ser selecionados ao escolher discos "
 "exclusivos ou ignorados para um dispositivo RAID multi-localização ou "
@@ -45,14 +45,19 @@
 msgid ""
 "Could not correctly delete SCSI device of zFCP %(devnum)s %(wwpn)s "
 "%(fcplun)s (%(e)s)."
 msgstr ""
 "Não foi possível remover correctamente o dispositivo SCSI do zFCP %(devnum)s "
 "%(wwpn)s %(fcplun)s (%(e)s)."
 
+msgid "Could not correctly delete SCSI device of zFCP %(zfcpdev)s (%(e)s)."
+msgstr ""
+"Não foi possível remover correctamente o dispositivo SCSI do zFCP "
+"%(zfcpdev)s (%(e)s)."
+
 msgid "Could not log in to any of the discovered nodes"
 msgstr "Não foi possível iniciar sessão em nenhum dos nós descobertos"
 
 msgid ""
 "Could not read failed attribute of LUN %(fcplun)s at WWPN %(wwpn)s on zFCP "
 "device %(devnum)s (%(e)s)."
 msgstr ""
@@ -194,14 +199,17 @@
 
 msgid "Resized filesystem on %(device)s"
 msgstr "Sistema de ficheiros redimensionado em %(device)s"
 
 msgid "Resizing filesystem on %(device)s"
 msgstr "A redimensionar sistema de ficheiros em %(device)s"
 
+msgid "Stratis block device"
+msgstr "Dispositivo em bloco Stratis"
+
 msgid ""
 "This is usually caused by cloning the device image resulting in duplication "
 "of the UUID value which should be unique. In that case you can either "
 "disconnect one of the devices or reformat it."
 msgstr ""
 "Isto ocorre normalmente ao clonar a imagem do dispositivo que resulta na "
 "duplicação do valor UUID que deve ser único. Nesse caso pode desligar um dos "
@@ -319,11 +327,14 @@
 
 msgid "software RAID"
 msgstr "RAID por software"
 
 msgid "unable to allocate aligned partition"
 msgstr "impossível alocar partição alinhada"
 
+msgid "zFCP device %s cannot use auto LUN scan."
+msgstr "O dispositivo zFCP %s não pode usar a verificação automática de LUN."
+
 msgid "zFCP device %s not found, not even in device ignore list."
 msgstr ""
 "O dispositivo zFCP %s não foi encontrado, nem mesmo na lista de dispositivos "
 "a ignorar."
```

### Comparing `blivet-3.7.1/po/pt.po` & `blivet-3.8.0/po/pt.po`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 # dcantrel <dcantrell@redhat.com>, 2011
 # Dimitris Glezos <glezos@indifex.com>, 2011
 # Miguel Sousa <migueljorgesousa@sapo.pt>, 2012
 # Ricardo Pinto <ricardo.bigote@gmail.com>, 2011
 # Rui Gouveia <rui.gouveia@gmail.com>, 2011-2012
 # Pedro Flores <pedro_flores_16@hotmail.com>, 2021.
 # Hugo Carvalho <hugokarvalho@hotmail.com>, 2022.
+# Felipe Nogueira <contato.fnog@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-09 13:31+0100\n"
-"PO-Revision-Date: 2022-03-25 13:16+0000\n"
-"Last-Translator: Hugo Carvalho <hugokarvalho@hotmail.com>\n"
+"PO-Revision-Date: 2023-04-07 05:20+0000\n"
+"Last-Translator: Felipe Nogueira <contato.fnog@gmail.com>\n"
 "Language-Team: Portuguese <https://translate.fedoraproject.org/projects/"
 "blivet/blivet-master/pt/>\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Weblate 4.11.2\n"
+"X-Generator: Weblate 4.15.2\n"
 
 #: ../blivet/deviceaction.py:197
 #, python-format
 msgid "Executing %(action)s"
 msgstr "A executar %(action)s"
 
 #: ../blivet/deviceaction.py:325
@@ -350,25 +351,22 @@
 msgstr ""
 "Não foi possível remover WWPN %(wwpn)s no dispositivo zFCP %(devnum)s "
 "(%(e)s)."
 
 #: ../blivet/zfcp.py:418
 #, python-format
 msgid "zFCP device %s cannot use auto LUN scan."
-msgstr ""
+msgstr "O dispositivo zFCP %s não pode usar a verificação automática de LUN."
 
 #: ../blivet/zfcp.py:432
-#, fuzzy, python-format
-#| msgid ""
-#| "Could not correctly delete SCSI device of zFCP %(devnum)s %(wwpn)s "
-#| "%(fcplun)s (%(e)s)."
+#, python-format
 msgid "Could not correctly delete SCSI device of zFCP %(zfcpdev)s (%(e)s)."
 msgstr ""
-"Não foi possível remover correctamente o dispositivo SCSI do zFCP %(devnum)s "
-"%(wwpn)s %(fcplun)s (%(e)s)."
+"Não foi possível remover correctamente o dispositivo SCSI do zFCP %(zfcpdev)"
+"s (%(e)s)."
 
 #: ../blivet/devicelibs/lvm.py:68
 msgid "Generic"
 msgstr "Genérico"
 
 #: ../blivet/devicelibs/lvm.py:69
 msgid "Performance"
@@ -461,11 +459,9 @@
 msgstr "dispositivo membro multicaminho"
 
 #: ../blivet/formats/prepboot.py:37
 msgid "PPC PReP Boot"
 msgstr "PPC PReP Boot"
 
 #: ../blivet/formats/stratis.py:40
-#, fuzzy
-#| msgid "create device"
 msgid "Stratis block device"
-msgstr "criar dispositivo"
+msgstr "Dispositivo em bloco Stratis"
```

### Comparing `blivet-3.7.1/po/pt_BR.mo` & `blivet-3.8.0/po/pt_BR.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-01-11 05:16+0000\n"
-"Last-Translator: Fernando Rodrigues <sigmasquadron@icloud.com>\n"
+"PO-Revision-Date: 2023-04-04 20:20+0000\n"
+"Last-Translator: Felipe Nogueira <contato.fnog@gmail.com>\n"
 "Language-Team: Portuguese (Brazil) <https://translate.fedoraproject.org/"
 "projects/blivet/blivet-master/pt_BR/>\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.10.1\n"
+"X-Generator: Weblate 4.15.2\n"
 
 msgid ""
 "All parent devices must be selected when choosing exclusive or ignored disks "
 "for a multipath or firmware RAID device."
 msgstr ""
 "Todos os dispositivos parentes devem ser selecionados ao escolher discos "
 "ignorados ou exclusivos em um dispositivo RAID de multipath ou firmware."
@@ -44,14 +44,19 @@
 msgid ""
 "Could not correctly delete SCSI device of zFCP %(devnum)s %(wwpn)s "
 "%(fcplun)s (%(e)s)."
 msgstr ""
 "Não foi possível remover corretamente o dispositivo SCSI de zFCP %(devnum)s "
 "%(wwpn)s %(fcplun)s (%(e)s)."
 
+msgid "Could not correctly delete SCSI device of zFCP %(zfcpdev)s (%(e)s)."
+msgstr ""
+"Não foi possível remover corretamente o dispositivo SCSI de zFCP %(zfcpdev)s "
+"(%(e)s)."
+
 msgid "Could not log in to any of the discovered nodes"
 msgstr "Impossível entrar em qualquer um dos nós descobertos"
 
 msgid ""
 "Could not read failed attribute of LUN %(fcplun)s at WWPN %(wwpn)s on zFCP "
 "device %(devnum)s (%(e)s)."
 msgstr ""
@@ -194,14 +199,17 @@
 
 msgid "Resized filesystem on %(device)s"
 msgstr "Redimensionando o sistema de arquivos em %(device)s"
 
 msgid "Resizing filesystem on %(device)s"
 msgstr "Redimensionando o sistema de arquivos em %(device)s"
 
+msgid "Stratis block device"
+msgstr "Dispositivo de bloco Stratis"
+
 msgid ""
 "This is usually caused by cloning the device image resulting in duplication "
 "of the UUID value which should be unique. In that case you can either "
 "disconnect one of the devices or reformat it."
 msgstr ""
 "Isso geralmente é causado pela clonagem da imagem do dispositivo resultando "
 "na duplicação do valor UUID, que deve ser único. Nesse caso, você pode "
@@ -319,11 +327,14 @@
 
 msgid "software RAID"
 msgstr "RAID por software"
 
 msgid "unable to allocate aligned partition"
 msgstr "incapaz de alocar a partição alinhada"
 
+msgid "zFCP device %s cannot use auto LUN scan."
+msgstr "O dispositivo zFCP %s não pode usar a verificação automática de LUN."
+
 msgid "zFCP device %s not found, not even in device ignore list."
 msgstr ""
 "Dispositivo zFCP %s não localizado, nem mesmo na lista de dispositivos "
 "ignorados."
```

### Comparing `blivet-3.7.1/po/pt_BR.po` & `blivet-3.8.0/po/pt_BR.po`

 * *Files 3% similar despite different names*

```diff
@@ -25,29 +25,30 @@
 # Rodrigo Padula de Oliveira <rodrigopadula@projetofedora.org>, 2005-2006
 # Marco Aurélio Krause <ouesten@me.com>, 2015. #zanata
 # Frederico Henrique Gonçalves Lima <fred@fredericolima.com.br>, 2016. #zanata
 # Frederico Henrique Gonçalves Lima <fred@fredericolima.com.br>, 2017. #zanata
 # Ludek Janda <ljanda@redhat.com>, 2018. #zanata
 # Lucas Fernandes <lucas.af88@gmail.com>, 2020.
 # Fernando Rodrigues <sigmasquadron@icloud.com>, 2022.
+# Felipe Nogueira <contato.fnog@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-09 13:31+0100\n"
-"PO-Revision-Date: 2022-01-11 05:16+0000\n"
-"Last-Translator: Fernando Rodrigues <sigmasquadron@icloud.com>\n"
+"PO-Revision-Date: 2023-04-04 20:20+0000\n"
+"Last-Translator: Felipe Nogueira <contato.fnog@gmail.com>\n"
 "Language-Team: Portuguese (Brazil) <https://translate.fedoraproject.org/"
 "projects/blivet/blivet-master/pt_BR/>\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.10.1\n"
+"X-Generator: Weblate 4.15.2\n"
 
 #: ../blivet/deviceaction.py:197
 #, python-format
 msgid "Executing %(action)s"
 msgstr "Executando %(action)s"
 
 #: ../blivet/deviceaction.py:325
@@ -370,25 +371,22 @@
 msgstr ""
 "Não foi possível remover o WWPN %(wwpn)s no dispositivo zFCP %(devnum)s "
 "(%(e)s)."
 
 #: ../blivet/zfcp.py:418
 #, python-format
 msgid "zFCP device %s cannot use auto LUN scan."
-msgstr ""
+msgstr "O dispositivo zFCP %s não pode usar a verificação automática de LUN."
 
 #: ../blivet/zfcp.py:432
-#, fuzzy, python-format
-#| msgid ""
-#| "Could not correctly delete SCSI device of zFCP %(devnum)s %(wwpn)s "
-#| "%(fcplun)s (%(e)s)."
+#, python-format
 msgid "Could not correctly delete SCSI device of zFCP %(zfcpdev)s (%(e)s)."
 msgstr ""
-"Não foi possível remover corretamente o dispositivo SCSI de zFCP %(devnum)s "
-"%(wwpn)s %(fcplun)s (%(e)s)."
+"Não foi possível remover corretamente o dispositivo SCSI de zFCP %(zfcpdev)s "
+"(%(e)s)."
 
 #: ../blivet/devicelibs/lvm.py:68
 msgid "Generic"
 msgstr "Genérico"
 
 #: ../blivet/devicelibs/lvm.py:69
 msgid "Performance"
@@ -480,11 +478,9 @@
 msgstr "dispositivo membro de multipath"
 
 #: ../blivet/formats/prepboot.py:37
 msgid "PPC PReP Boot"
 msgstr "Inicialização PPC PReP"
 
 #: ../blivet/formats/stratis.py:40
-#, fuzzy
-#| msgid "create device"
 msgid "Stratis block device"
-msgstr "criar dispositivo"
+msgstr "Dispositivo de bloco Stratis"
```

### Comparing `blivet-3.7.1/po/ro.mo` & `blivet-3.8.0/po/ro.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ro.po` & `blivet-3.8.0/po/ro.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ru.mo` & `blivet-3.8.0/po/ru.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ru.po` & `blivet-3.8.0/po/ru.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/si.mo` & `blivet-3.8.0/po/si.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/si.po` & `blivet-3.8.0/po/si.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sk.mo` & `blivet-3.8.0/po/sk.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sk.po` & `blivet-3.8.0/po/sk.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sl.mo` & `blivet-3.8.0/po/sl.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sl.po` & `blivet-3.8.0/po/sl.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sq.mo` & `blivet-3.8.0/po/sq.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sq.po` & `blivet-3.8.0/po/sq.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sr.mo` & `blivet-3.8.0/po/sr.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sr.po` & `blivet-3.8.0/po/sr.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sr@latin.mo` & `blivet-3.8.0/po/sr@latin.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sr@latin.po` & `blivet-3.8.0/po/sr@latin.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sv.mo` & `blivet-3.8.0/po/sv.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/sv.po` & `blivet-3.8.0/po/sv.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ta.mo` & `blivet-3.8.0/po/ta.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ta.po` & `blivet-3.8.0/po/ta.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/te.mo` & `blivet-3.8.0/po/te.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/te.po` & `blivet-3.8.0/po/te.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/tg.mo` & `blivet-3.8.0/po/tg.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/tg.po` & `blivet-3.8.0/po/tg.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/th.mo` & `blivet-3.8.0/po/th.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/th.po` & `blivet-3.8.0/po/th.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/tr.mo` & `blivet-3.8.0/po/tr.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/tr.po` & `blivet-3.8.0/po/tr.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/uk.mo` & `blivet-3.8.0/po/uk.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/uk.po` & `blivet-3.8.0/po/uk.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ur.mo` & `blivet-3.8.0/po/ur.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/ur.po` & `blivet-3.8.0/po/ur.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/zh_CN.mo` & `blivet-3.8.0/po/zh_CN.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/zh_CN.po` & `blivet-3.8.0/po/zh_CN.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/zh_TW.mo` & `blivet-3.8.0/po/zh_TW.mo`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/po/zh_TW.po` & `blivet-3.8.0/po/zh_TW.po`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/python-blivet.spec` & `blivet-3.8.0/python-blivet.spec`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,11 @@
-%define is_rhel 0%{?rhel} != 0
-
-# python3 is not available on RHEL <=7
-%if %{is_rhel} && 0%{?rhel} <= 7
-# disable python3 by default
-%bcond_with python3
-%else
-%bcond_without python3
-%endif
-
-# python2 is not available on RHEL > 7 and not needed on Fedora > 28
-%if 0%{?rhel} > 7 || 0%{?fedora} > 28
-# disable python2 by default
-%bcond_with python2
-%else
-%bcond_without python2
-%endif
-
 Summary:  A python module for system storage configuration
 Name: python-blivet
 Url: https://storageapis.wordpress.com/projects/blivet
-Version: 3.7.1
+Version: 3.8.0
 
 #%%global prerelease .b2
 # prerelease, if defined, should be something like .a1, .b1, .b2.dev1, or .c2
 Release: 1%{?prerelease}%{?dist}
 Epoch: 1
 License: LGPL-2.1-or-later
 %global realname blivet
@@ -32,15 +14,15 @@
 Source1: http://github.com/storaged-project/blivet/archive/%{realname}-%{realversion}-tests.tar.gz
 
 # Versions of required components (done so we make sure the buildrequires
 # match the requires versions of things).
 %global partedver 1.8.1
 %global pypartedver 3.10.4
 %global utillinuxver 2.15.1
-%global libblockdevver 2.24
+%global libblockdevver 3.0
 %global libbytesizever 0.3
 %global pyudevver 0.18
 
 BuildArch: noarch
 
 %description
 The python-blivet package is a python module for examining and modifying
@@ -55,15 +37,14 @@
 Conflicts: python-blivet < 1:2.0.0
 Conflicts: python3-blivet < 1:2.0.0
 
 %description -n %{realname}-data
 The %{realname}-data package provides data files required by the %{realname}
 python module.
 
-%if %{with python3}
 %package -n python3-%{realname}
 Summary: A python3 package for examining and modifying storage configuration.
 
 %{?python_provide:%python_provide python3-%{realname}}
 
 BuildRequires: gettext
 BuildRequires: python3-devel
@@ -94,108 +75,80 @@
 Requires: lsof
 Requires: python3-gobject-base
 Requires: systemd-udev
 Requires: %{realname}-data = %{epoch}:%{version}-%{release}
 
 Obsoletes: blivet-data < 1:2.0.0
 
-%if %{without python2}
-Obsoletes: python2-blivet < 1:2.0.2-2
-Obsoletes: python-blivet < 1:2.0.2-2
-%else
-Obsoletes: python-blivet < 1:2.0.0
-%endif
-
 %description -n python3-%{realname}
 The python3-%{realname} is a python3 package for examining and modifying storage
 configuration.
-%endif
-
-%if %{with python2}
-%package -n python2-%{realname}
-Summary: A python2 package for examining and modifying storage configuration.
-
-%{?python_provide:%python_provide python2-%{realname}}
-
-BuildRequires: gettext
-BuildRequires: python2-devel
-BuildRequires: python2-setuptools
-
-Requires: python2
-Requires: python2-six
-Requires: python2-pyudev >= %{pyudevver}
-Requires: parted >= %{partedver}
-Requires: python2-pyparted >= %{pypartedver}
-Requires: python2-libselinux
-Requires: python2-blockdev >= %{libblockdevver}
-Recommends: libblockdev-btrfs >= %{libblockdevver}
-Recommends: libblockdev-crypto >= %{libblockdevver}
-Recommends: libblockdev-dm >= %{libblockdevver}
-Recommends: libblockdev-fs >= %{libblockdevver}
-Recommends: libblockdev-kbd >= %{libblockdevver}
-Recommends: libblockdev-loop >= %{libblockdevver}
-Recommends: libblockdev-lvm >= %{libblockdevver}
-Recommends: libblockdev-mdraid >= %{libblockdevver}
-Recommends: libblockdev-mpath >= %{libblockdevver}
-Recommends: libblockdev-nvdimm >= %{libblockdevver}
-Recommends: libblockdev-part >= %{libblockdevver}
-Recommends: libblockdev-swap >= %{libblockdevver}
-Recommends: libblockdev-s390 >= %{libblockdevver}
-Requires: python2-bytesize >= %{libbytesizever}
-Requires: util-linux >= %{utillinuxver}
-Requires: lsof
-Requires: python2-hawkey
-Requires: %{realname}-data = %{epoch}:%{version}-%{release}
-
-Requires: systemd-udev
-Requires: python2-gobject-base
-
-Obsoletes: blivet-data < 1:2.0.0
-Obsoletes: python-blivet < 1:2.0.0
-
-%description -n python2-%{realname}
-The python2-%{realname} is a python2 package for examining and modifying storage
-configuration.
-%endif
 
 %prep
 %autosetup -n %{realname}-%{realversion} -N
 %autosetup -n %{realname}-%{realversion} -b1 -p1
 
 %build
-%{?with_python2:make PYTHON=%{__python2}}
-%{?with_python3:make PYTHON=%{__python3}}
+make
 
 %install
-%{?with_python2:make PYTHON=%{__python2} DESTDIR=%{buildroot} install}
-%{?with_python3:make PYTHON=%{__python3} DESTDIR=%{buildroot} install}
+make DESTDIR=%{buildroot} install
 
 %find_lang %{realname}
 
 %files -n %{realname}-data -f %{realname}.lang
 %{_sysconfdir}/dbus-1/system.d/*
 %{_datadir}/dbus-1/system-services/*
 %{_libexecdir}/*
 %{_unitdir}/*
 
-%if %{with python2}
-%files -n python2-%{realname}
-%license COPYING
-%doc README.md ChangeLog examples
-%{python2_sitelib}/*
-%endif
-
-%if %{with python3}
 %files -n python3-%{realname}
 %license COPYING
 %doc README.md ChangeLog examples
 %{python3_sitelib}/*
-%endif
 
 %changelog
+* Thu Jun 29 2023 Vojtech Trefny <vtrefny@redhat.com> - 3.8.0-1
+- Revert "Makefile cleanup" (blivet-ci)
+- Require libblockdev 3.0 when importing from GI (vtrefny)
+- spec: Bump required version of libblockdev to 3.0 (vtrefny)
+- md: Adapt libblockdev 3.0 mdraid bitmap arg changes (tbzatek)
+- spec: Bump release to 99 to be always ahead of Fedora in nightly (vtrefny)
+- ci: Run GH actions tests in a Fedora container (vtrefny)
+- Add new LUKS tests for add/remove key and key file usage (vtrefny)
+- Adjust to the new libblockdev 3.0 crypto API (vtrefny)
+- Adjust to libblockdev 3.0 API changes (vtrefny)
+- blivet: Enable the extended node bitmap for F2FS (akoskovich)
+- Remove all state-dependent objects when resetting Blivet DBus object. (dlehman)
+- Run callbacks when pruning actions. (dlehman)
+- Always prefer GPT disk labels on x86_64 (and clean up the logic) (awilliam)
+- Do not add new PVs to the LVM devices file if it doesn't exist and VGs are present (vtrefny)
+- Add RISCV64 architecture helper [is_riscv64()] for arch module. (48907457+nirousseau)
+- iscsi: Extend allowed CHAP auth algorithms (tbzatek)
+- Fix checking FIPS mode when /proc/sys/crypto/fips_enabled doesn't exist (vtrefny)
+- Fix creating LUKS1 on disks with mixed sector size (#2188785) (vtrefny)
+- Do not set memory limit for LUKS2 when running in FIPS mode (vtrefny)
+- Revert "tests: Skip test_lvcreate_type on CentOS/RHEL 9" (vtrefny)
+- DBus: remove extra callback invocations (dlehman)
+- Add a test case for filesystem online resize (vtrefny)
+- Add support for filesystem online resize (vtrefny)
+- iscsi: Use UDisks instead of storaged in the availability message (vtrefny)
+- tests: Fix skipping iSCSI tests if UDisks iSCSI isn't available (vtrefny)
+- Add ChangeLog to .gitignore (vtrefny)
+- Makefile cleanup (vtrefny)
+- ci: Use Packit for daily builds in Copr (vtrefny)
+- Avoid raising libblockdev exceptions from our code (vtrefny)
+- ci: Fix Packit configuration (vtrefny)
+- Add support for specifying stripe size for RAID LVs (vtrefny)
+- tests: Use blivet-specific prefix for targetcli backing files (vtrefny)
+- Add a basic test case for the iscsi module (vtrefny)
+- Allow changing iSCSI initiator name after setting it (vtrefny)
+- Prefer UUID for fstab spec for DM devices too (vtrefny)
+- Remove support for Python 2 from spec and Makefile (vtrefny)
+
 * Thu Mar 16 2023 Vojtech Trefny <vtrefny@redhat.com> - 3.7.1-1
 - Fix the get_mount_device function (vponcova)
 - Prefer using UUID for the kickstart --onpart argument (vtrefny)
 - Fix setting kickstart data (vtrefny)
 - pylint: Remove the "EXCEPTIONS" section from pylintrc (vtrefny)
 - Add "microsoft" to list of recognized VM environments (vtrefny)
 - ci: Add action to run unit tests in GH actions (vtrefny)
```

### Comparing `blivet-3.7.1/release_notes.rst` & `blivet-3.8.0/release_notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+3.8.0
+======
+* `Filesystem online resize support`_
+* `Libblockdev 3.0`_
+
+Filesystem online resize support
+---------------------------------
+Filesystem that support online shrink and/or grow can now be resized when
+mounted. The default behaviour is still to try to unmount the filesystem
+first. This can be controlled with the `flags.allow_online_fs_resize` flag.
+
+Libblockdev 3.0
+----------------
+Latest major release of the libblockdev library is now required for blivet.
+
 3.7.0
 ======
 * `NVMe and NVMe over Fabrics support`_
 * `Discoverable partition IDs support`_
 * `DMRAID support removed`_
 * `Removed`_
```

### Comparing `blivet-3.7.1/scripts/docs-update` & `blivet-3.8.0/scripts/docs-update`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/scripts/git-multi-merge` & `blivet-3.8.0/scripts/git-multi-merge`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/scripts/harvest-edd` & `blivet-3.8.0/scripts/harvest-edd`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/scripts/makebumpver` & `blivet-3.8.0/scripts/makebumpver`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/scripts/makeupdates` & `blivet-3.8.0/scripts/makeupdates`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/scripts/pylintcodediff` & `blivet-3.8.0/scripts/pylintcodediff`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/setup.py` & `blivet-3.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,24 +81,23 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(name='blivet',
-      version='3.7.1',
+      version='3.8.0',
       cmdclass={"sdist": blivet_sdist},
       description='Python module for system storage configuration',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author='David Lehman', author_email='dlehman@redhat.com',
       url='http://github.com/storaged-project/blivet',
       data_files=data_files,
       packages=['blivet', 'blivet.dbus', 'blivet.devices', 'blivet.devicelibs', 'blivet.events', 'blivet.formats', 'blivet.populator', 'blivet.static_data', 'blivet.tasks', 'blivet.populator.helpers'],
       install_requires=['pyudev', 'six'],
       classifiers=["Development Status :: 5 - Production/Stable",
                    "Intended Audience :: Developers",
                    "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
-                   "Programming Language :: Python :: 2",
                    "Programming Language :: Python :: 3",
                    "Operating System :: POSIX :: Linux"]
      )
```

### Comparing `blivet-3.7.1/tests/README.rst` & `blivet-3.8.0/tests/README.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/pylint/censorship.py` & `blivet-3.8.0/tests/pylint/censorship.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/pylint/pylintrc` & `blivet-3.8.0/tests/pylint/pylintrc`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/pylint/runpylint.py` & `blivet-3.8.0/tests/pylint/runpylint.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/run_tests.py` & `blivet-3.8.0/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/skip.yml` & `blivet-3.8.0/tests/skip.yml`

 * *Files 7% similar despite different names*

```diff
@@ -19,13 +19,7 @@
 # - multiple combinations of reasons are supported.
 # - 'reason' and at least one of 'distro', 'version' and 'arch' is required
 # - 'test' (ID of the test case) can be specified as a regular expression
 #   for example 'kbd_test.KbdBcacheTestCase.*' to skip all kbd tests
 # - all "skips" can specified as a list, for example 'version: [10, 11]'
 
 ---
-
-- test: storage_tests.devices_test.lvm_test.LVMTestCase.test_lvm_raid
-  skip_on:
-    - distro: "centos"
-      version: "9"
-      reason: "Creating RAID 1 LV on CentOS/RHEL 9 causes a system deadlock"
```

### Comparing `blivet-3.7.1/tests/storage_tests/devices_test/lvm_test.py` & `blivet-3.8.0/tests/storage_tests/devices_test/lvm_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import shutil
+import subprocess
 
 from ..storagetestcase import StorageTestCase
 
 import blivet
 
 
 class LVMTestCase(StorageTestCase):
@@ -134,15 +135,15 @@
         self.assertEqual(thinlv.pool, pool)
 
         snap = self.storage.devicetree.get_device_by_name("%s-blivetTestThinLV_snapshot" % self.vgname)
         self.assertIsNotNone(snap)
         self.assertTrue(snap.is_snapshot_lv)
         self.assertEqual(snap.origin, thinlv)
 
-    def _test_lvm_raid(self, seg_type, raid_level):
+    def _test_lvm_raid(self, seg_type, raid_level, stripe_size=0):
         disk1 = self.storage.devicetree.get_device_by_path(self.vdevs[0])
         self.assertIsNotNone(disk1)
         self.storage.initialize_disk(disk1)
 
         disk2 = self.storage.devicetree.get_device_by_path(self.vdevs[1])
         self.assertIsNotNone(disk2)
         self.storage.initialize_disk(disk2)
@@ -158,29 +159,36 @@
         blivet.partitioning.do_partitioning(self.storage)
 
         vg = self.storage.new_vg(name=self.vgname, parents=[pv1, pv2])
         self.storage.create_device(vg)
 
         raidlv = self.storage.new_lv(fmt_type="ext4", size=blivet.size.Size("50 MiB"),
                                      parents=[vg], name="blivetTestRAIDLV",
-                                     seg_type=seg_type, pvs=[pv1, pv2])
+                                     seg_type=seg_type, pvs=[pv1, pv2], stripe_size=stripe_size)
         self.storage.create_device(raidlv)
 
         self.storage.do_it()
         self.storage.reset()
 
         raidlv = self.storage.devicetree.get_device_by_name("%s-blivetTestRAIDLV" % self.vgname)
         self.assertIsNotNone(raidlv)
         self.assertTrue(raidlv.is_raid_lv)
         self.assertEqual(raidlv.raid_level, raid_level)
         self.assertEqual(raidlv.seg_type, seg_type)
 
+        if stripe_size:
+            out = subprocess.check_output(["lvs", "-o", "stripe_size", "--noheadings", "--nosuffix", "--units=b", raidlv.vg.name + "/" + raidlv.lvname])
+            self.assertEqual(out.decode().strip(), str(int(stripe_size.convert_to())))
+
     def test_lvm_raid_raid0(self):
         self._test_lvm_raid("raid0", blivet.devicelibs.raid.RAID0)
 
+    def test_lvm_raid_raid0_stripe_size(self):
+        self._test_lvm_raid("raid0", blivet.devicelibs.raid.RAID0, stripe_size=blivet.size.Size("1 MiB"))
+
     def test_lvm_raid_striped(self):
         self._test_lvm_raid("striped", blivet.devicelibs.raid.Striped)
 
     def test_lvm_raid_raid1(self):
         self._test_lvm_raid("raid1", blivet.devicelibs.raid.RAID1)
 
     def test_lvm_raid_mirror(self):
```

### Comparing `blivet-3.7.1/tests/storage_tests/devices_test/partition_test.py` & `blivet-3.8.0/tests/storage_tests/devices_test/partition_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             self.assertEqual(device.size, orig_size)
             parted_size = Size(device.parted_partition.getLength(unit='B'))
             self.assertEqual(parted_size, device.target_size)
 
     def test_min_max_size_alignment(self):
         with sparsetmpfile("minsizetest", Size("10 MiB")) as disk_file:
             disk = DiskFile(disk_file)
-            disk.format = get_format("disklabel", device=disk.path)
+            disk.format = get_format("disklabel", device=disk.path, label_type="msdos")
             grain_size = Size(disk.format.alignment.grainSize)
             sector_size = Size(disk.format.parted_device.sectorSize)
             start = int(grain_size)
             end = start + int(Size("6 MiB") / sector_size)
             disk.format.add_partition(start, end)
             partition = disk.format.parted_disk.getPartitionBySector(start)
             self.assertNotEqual(partition, None)
```

### Comparing `blivet-3.7.1/tests/storage_tests/devices_test/stratis_test.py` & `blivet-3.8.0/tests/storage_tests/devices_test/stratis_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/storage_tests/formats_test/fs_test.py` & `blivet-3.8.0/tests/storage_tests/formats_test/fs_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import tempfile
 import unittest
 
 import parted
 
 import blivet.formats.fs as fs
 from blivet.size import Size, ROUND_DOWN
-from blivet.errors import DeviceFormatError
+from blivet.errors import DeviceFormatError, FSError
 from blivet.formats import get_format
 from blivet.devices import PartitionDevice, DiskDevice
+from blivet.flags import flags
 
 from .loopbackedtestcase import LoopBackedTestCase
 
 from . import fstesting
 
 
 class Ext2FSTestCase(fstesting.FSAsRoot):
@@ -22,14 +23,54 @@
 class Ext3FSTestCase(Ext2FSTestCase):
     _fs_class = fs.Ext3FS
 
 
 class Ext4FSTestCase(Ext3FSTestCase):
     _fs_class = fs.Ext4FS
 
+    def test_online_resize(self):
+        an_fs = self._fs_class()
+        if not an_fs.formattable:
+            self.skipTest("can not create filesystem %s" % an_fs.name)
+        an_fs.device = self.loop_devices[0]
+        self.assertIsNone(an_fs.create())
+        an_fs.update_size_info()
+
+        if not self.can_resize(an_fs):
+            self.skipTest("filesystem is not resizable")
+
+        # shrink offline first (ext doesn't support online shrinking)
+        TARGET_SIZE = Size("64 MiB")
+        an_fs.target_size = TARGET_SIZE
+        self.assertEqual(an_fs.target_size, TARGET_SIZE)
+        self.assertNotEqual(an_fs._size, TARGET_SIZE)
+        self.assertIsNone(an_fs.do_resize())
+
+        with tempfile.TemporaryDirectory() as mountpoint:
+            an_fs.mount(mountpoint=mountpoint)
+
+            # grow back when mounted
+            TARGET_SIZE = Size("100 MiB")
+            an_fs.target_size = TARGET_SIZE
+            self.assertEqual(an_fs.target_size, TARGET_SIZE)
+            self.assertNotEqual(an_fs._size, TARGET_SIZE)
+
+            # should fail, online resize disabled by default
+            with self.assertRaisesRegex(FSError, "Resizing of mounted filesystems is disabled"):
+                an_fs.do_resize()
+
+            # enable online resize
+            flags.allow_online_fs_resize = True
+            an_fs.do_resize()
+            flags.allow_online_fs_resize = False
+            self._test_sizes(an_fs)
+            self.assertEqual(an_fs.system_mountpoint, mountpoint)
+
+            an_fs.unmount()
+
 
 class FATFSTestCase(fstesting.FSAsRoot):
     _fs_class = fs.FATFS
 
 
 class EFIFSTestCase(FATFSTestCase):
     _fs_class = fs.EFIFS
```

### Comparing `blivet-3.7.1/tests/storage_tests/formats_test/fslabeling.py` & `blivet-3.8.0/tests/storage_tests/formats_test/fslabeling.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/storage_tests/formats_test/fstesting.py` & `blivet-3.8.0/tests/storage_tests/formats_test/fstesting.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/storage_tests/formats_test/fsuuid.py` & `blivet-3.8.0/tests/storage_tests/formats_test/fsuuid.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/storage_tests/formats_test/labeling_test.py` & `blivet-3.8.0/tests/storage_tests/formats_test/labeling_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/storage_tests/formats_test/loopbackedtestcase.py` & `blivet-3.8.0/tests/storage_tests/formats_test/loopbackedtestcase.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/storage_tests/formats_test/lvmpv_test.py` & `blivet-3.8.0/tests/storage_tests/formats_test/lvmpv_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/storage_tests/formats_test/uuid_test.py` & `blivet-3.8.0/tests/storage_tests/formats_test/uuid_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/storage_tests/imagebackedtestcase.py` & `blivet-3.8.0/tests/storage_tests/imagebackedtestcase.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/storage_tests/partitioning_test.py` & `blivet-3.8.0/tests/storage_tests/partitioning_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/storage_tests/storagetestcase.py` & `blivet-3.8.0/tests/storage_tests/storagetestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 def create_sparse_tempfile(name, size):
     """ Create a temporary sparse file.
 
         :param str name: suffix for filename
         :param size: the file size (in bytes)
         :returns: the path to the newly created file
     """
-    (fd, path) = tempfile.mkstemp(prefix="bd.", suffix="-%s" % name)
+    (fd, path) = tempfile.mkstemp(prefix="blivet.", suffix="-%s" % name)
     os.close(fd)
     create_sparse_file(path, size)
     return path
 
 
 def create_sparse_file(path, size):
     """ Create a sparse file.
```

### Comparing `blivet-3.7.1/tests/storage_tests/unsupported_disklabel_test.py` & `blivet-3.8.0/tests/storage_tests/unsupported_disklabel_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/action_test.py` & `blivet-3.8.0/tests/unit_tests/action_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/blivettestcase.py` & `blivet-3.8.0/tests/unit_tests/blivettestcase.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/dbus_test.py` & `blivet-3.8.0/tests/unit_tests/dbus_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import random
 
 try:
-    from unittest.mock import patch, Mock
+    from unittest.mock import patch, Mock, call
 except ImportError:
-    from mock import patch, Mock
+    from mock import patch, Mock, call
 
 from unittest import TestCase
 
 import dbus
 
 from blivet.dbus.action import DBusAction
 from blivet.dbus.blivet import DBusBlivet
@@ -19,14 +19,15 @@
 from blivet.dbus.constants import DEVICE_OBJECT_PATH_BASE, DEVICE_REMOVED_OBJECT_PATH_BASE
 from blivet.dbus.constants import FORMAT_OBJECT_PATH_BASE, FORMAT_REMOVED_OBJECT_PATH_BASE
 
 
 def mock_dbus_device(obj_id):
     obj = Mock(name="DBusDevice [%d]" % obj_id,
                id=obj_id,
+               transient=True,
                object_path="%s/%d" % (DEVICE_OBJECT_PATH_BASE, obj_id),
                _device=Mock(name="StorageDevice %d" % obj_id))
     return obj
 
 
 class DBusBlivetTestCase(TestCase):
     @patch.object(DBusObject, "_init_dbus_object")
@@ -56,16 +57,23 @@
             self.assertEqual(self.dbus_object.Get(BLIVET_INTERFACE, 'Devices'), object_paths)
 
     def test_Reset(self):
         """ Verify that Reset calls the underlying Blivet's reset method. """
         self.dbus_object._blivet.reset_mock()
         self.dbus_object._blivet.devices = []
         self.dbus_object._blivet.devicetree.actions = []
+        device_ids = [1, 11, 20, 101]
+        dbus_devices = [mock_dbus_device(i) for i in device_ids]
+        self.dbus_object._manager.objects = [self.dbus_object]
+        self.dbus_object._manager.objects.extend(dbus_devices)
         self.dbus_object.Reset()
         self.dbus_object._blivet.reset.assert_called_once_with()
+        self.dbus_object._manager.remove_object.assert_has_calls([call(d) for d in dbus_devices])
+        self.assertNotIn(call(self.dbus_object),
+                         self.dbus_object._manager.remove_object.mock_calls)
         self.dbus_object._blivet.reset_mock()
 
     def test_RemoveDevice(self):
         self.dbus_object._blivet.reset_mock()
         dbus_device = mock_dbus_device(23)
         with patch.object(self.dbus_object._manager, "get_object_by_path", return_value=dbus_device):
             with patch("blivet.dbus.blivet.isinstance", return_value=True):
```

### Comparing `blivet-3.7.1/tests/unit_tests/devicefactory_test.py` & `blivet-3.8.0/tests/unit_tests/devicefactory_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/disk_test.py` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/disk_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sda` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sda`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdb` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdb`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdc` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdc`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdd` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sdd`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sde` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/sde`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/vda` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/absurd_virt/dev/vda`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sda` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sda`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sdb` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sdb`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sdc` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/bad_sata_virt/dev/sdc`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sda` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sda`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sdb` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sdb`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sdc` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/sdc`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/vda` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/mostly_fixed_virt/dev/vda`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/dev/sda` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/dev/sda`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/dev/sdb` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/dev/sdb`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/raw_data` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev80/raw_data`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/raw_data` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/sata_usb/sys/firmware/edd/int13_dev81/raw_data`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sdc` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sdc`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sdd` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_data/strawberry_mountain/dev/sdd`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/edd_test.py` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/edd_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/lib.py` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/lib.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/mdraid_test.py` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/mdraid_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicelibs_test/raid_test.py` & `blivet-3.8.0/tests/unit_tests/devicelibs_test/raid_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/device_dependencies_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/device_dependencies_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from mock import patch, PropertyMock
 
 import unittest
 import os
 import six
 import blivet
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 from gi.repository import BlockDev as blockdev
 
 from blivet.errors import DependencyError
 
 from blivet.deviceaction import ActionCreateDevice
 from blivet.deviceaction import ActionDestroyDevice
 from blivet.deviceaction import ActionResizeDevice
```

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/device_methods_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/device_methods_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/device_names_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/device_names_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/device_packages_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/device_packages_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/device_properties_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/device_properties_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import six
 import unittest
 
 import gi
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 
 from gi.repository import BlockDev as blockdev
 
 try:
     from unittest.mock import patch, Mock
 except ImportError:
     from mock import patch, Mock
```

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/device_size_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/device_size_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/disk_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/disk_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/lvm_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/lvm_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,14 +359,41 @@
                                     exists=False, cache_request=cache_req,
                                     pvs=[pv_spec, pv_spec2])
         self.assertEqual(lv.seg_type, "linear")
         # 1024 MiB (free) - 256 MiB (LV part) - 504 MiB (cache shrank for pmspare space)
         self.assertEqual(pv.format.free, Size("264 MiB"))
         self.assertEqual(pv2.format.free, Size("256 MiB"))
 
+    def test_lvm_logical_volume_raid_stripe_size(self):
+        pv = StorageDevice("pv1", fmt=blivet.formats.get_format("lvmpv"),
+                           size=Size("1025 MiB"))
+        pv2 = StorageDevice("pv2", fmt=blivet.formats.get_format("lvmpv"),
+                            size=Size("513 MiB"))
+        vg = LVMVolumeGroupDevice("testvg", parents=[pv, pv2])
+
+        with self.assertRaises(blivet.errors.DeviceError):
+            # non-raid LV
+            lv = LVMLogicalVolumeDevice("testlv", parents=[vg], size=Size("1 GiB"),
+                                        fmt=blivet.formats.get_format("xfs"),
+                                        exists=False, stripe_size=Size("1 MiB"))
+
+        with self.assertRaises(blivet.errors.DeviceError):
+            # raid1 LV
+            lv = LVMLogicalVolumeDevice("testlv", parents=[vg], size=Size("1 GiB"),
+                                        fmt=blivet.formats.get_format("xfs"),
+                                        exists=False, seg_type="raid1", pvs=[pv, pv2],
+                                        stripe_size=Size("1 MiB"))
+
+        lv = LVMLogicalVolumeDevice("testlv", parents=[vg], size=Size("1 GiB"),
+                                    fmt=blivet.formats.get_format("xfs"),
+                                    exists=False, seg_type="raid0", pvs=[pv, pv2],
+                                    stripe_size=Size("1 MiB"))
+
+        self.assertEqual(lv._stripe_size, Size("1 MiB"))
+
     @patch("blivet.formats.fs.Ext4FS.resizable", return_value=True)
     def test_target_size(self, *args):  # pylint: disable=unused-argument
         pv = StorageDevice("pv1", fmt=blivet.formats.get_format("lvmpv"),
                            size=Size("1 GiB"))
         vg = LVMVolumeGroupDevice("testvg", parents=[pv])
         orig_size = Size("800 MiB")
         lv = LVMLogicalVolumeDevice("testlv", parents=[vg], size=orig_size,
```

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/md_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/md_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,27 +34,27 @@
 
         # no chunk_size specified and RAID0 -- default value
         self.assertEqual(raid_array.chunk_size, mdraid.MD_CHUNK_SIZE)
 
         with patch("blivet.devices.md.blockdev.md.create") as md_create:
             raid_array._create()
             md_create.assert_called_with("/dev/md/raid", "raid0", ["/dev/member1", "/dev/member2"],
-                                         0, version="default", bitmap=False,
+                                         0, version="default", bitmap=None,
                                          chunk_size=mdraid.MD_CHUNK_SIZE)
 
         raid_array = MDRaidArrayDevice(name="raid", level="raid1", member_devices=2,
                                        total_devices=2, parents=[member1, member2])
 
         # no chunk_size specified and RAID1 -- no chunk size set (0)
         self.assertEqual(raid_array.chunk_size, Size(0))
 
         with patch("blivet.devices.md.blockdev.md.create") as md_create:
             raid_array._create()
             md_create.assert_called_with("/dev/md/raid", "raid1", ["/dev/member1", "/dev/member2"],
-                                         0, version="default", bitmap=True,
+                                         0, version="default", bitmap="internal",
                                          chunk_size=0)
 
     def test_chunk_size2(self):
 
         member1 = StorageDevice("member1", fmt=blivet.formats.get_format("mdmember"),
                                 size=Size("1 GiB"))
         member2 = StorageDevice("member2", fmt=blivet.formats.get_format("mdmember"),
```

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/network_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/network_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/partition_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/partition_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devices_test/stratis_test.py` & `blivet-3.8.0/tests/unit_tests/devices_test/stratis_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/devicetree_test.py` & `blivet-3.8.0/tests/unit_tests/devicetree_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/events_test.py` & `blivet-3.8.0/tests/unit_tests/events_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/formats_tests/device_test.py` & `blivet-3.8.0/tests/unit_tests/formats_tests/device_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/formats_tests/disklabel_test.py` & `blivet-3.8.0/tests/unit_tests/formats_tests/disklabel_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         disklabel_class = blivet.formats.disklabel.DiskLabel
 
         arch.is_s390.return_value = False
         arch.is_efi.return_value = False
         arch.is_aarch64.return_value = False
         arch.is_arm.return_value = False
         arch.is_pmac.return_value = False
+        arch.is_x86.return_value = False
 
         self.assertEqual(disklabel_class.get_platform_label_types(), ["msdos", "gpt"])
 
         arch.is_pmac.return_value = True
         self.assertEqual(disklabel_class.get_platform_label_types(), ["mac"])
         arch.is_pmac.return_value = False
 
@@ -92,14 +93,22 @@
         arch.is_arm.return_value = False
         arch.is_efi.return_value = False
 
         arch.is_arm.return_value = True
         self.assertEqual(disklabel_class.get_platform_label_types(), ["msdos", "gpt"])
         arch.is_arm.return_value = False
 
+        # this simulates x86_64
+        arch.is_x86.return_value = True
+        self.assertEqual(disklabel_class.get_platform_label_types(), ["gpt", "msdos"])
+        arch.is_efi.return_value = True
+        self.assertEqual(disklabel_class.get_platform_label_types(), ["gpt", "msdos"])
+        arch.is_x86.return_value = False
+        arch.is_efi.return_value = False
+
         arch.is_s390.return_value = True
         self.assertEqual(disklabel_class.get_platform_label_types(), ["msdos", "gpt", "dasd"])
         arch.is_s390.return_value = False
 
     def test_label_type_size_check(self):
         dl = blivet.formats.disklabel.DiskLabel()
         dl._parted_disk = mock.Mock()
@@ -134,14 +143,15 @@
         dl._device = "labeltypefakedev"
 
         arch.is_s390.return_value = False
         arch.is_efi.return_value = False
         arch.is_aarch64.return_value = False
         arch.is_arm.return_value = False
         arch.is_pmac.return_value = False
+        arch.is_x86.return_value = False
 
         with mock.patch.object(dl, '_label_type_size_check') as size_check:
             # size check passes for first type ("msdos")
             size_check.return_value = True
             self.assertEqual(dl._get_best_label_type(), "msdos")
 
             # size checks all fail -> label type is None
```

### Comparing `blivet-3.7.1/tests/unit_tests/formats_tests/init_test.py` & `blivet-3.8.0/tests/unit_tests/formats_tests/init_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/formats_tests/methods_test.py` & `blivet-3.8.0/tests/unit_tests/formats_tests/methods_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,19 +362,22 @@
         super(LUKSMethodsTestCase, self).set_patches()
         self.patchers["configured"] = patch.object(self.format_class, "configured", new=PropertyMock(return_value=True))
         self.patchers["has_key"] = patch.object(self.format_class, "has_key", new=PropertyMock(return_value=True))
         self.patchers["blockdev"] = patch("blivet.formats.luks.blockdev")
 
     def _test_create_backend(self):
         self.format.exists = False
+        self.format.passphrase = "passphrase"
         with patch("blivet.devicelibs.crypto.get_optimal_luks_sector_size", return_value=512):
-            self.format.create()
+            with patch("blivet.devicelibs.crypto.is_fips_enabled", return_value=False):
+                self.format.create()
         self.assertTrue(self.patches["blockdev"].crypto.luks_format.called)  # pylint: disable=no-member
 
     def _test_setup_backend(self):
+        self.format.passphrase = "passphrase"
         self.format.setup()
         self.assertTrue(self.patches["blockdev"].crypto.luks_open.called)
 
     def _test_teardown_backend(self):
         self.format.teardown()
         self.assertTrue(self.patches["blockdev"].crypto.luks_close.called)
```

### Comparing `blivet-3.7.1/tests/unit_tests/formats_tests/misc_test.py` & `blivet-3.8.0/tests/unit_tests/formats_tests/misc_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/formats_tests/selinux_test.py` & `blivet-3.8.0/tests/unit_tests/formats_tests/selinux_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/formats_tests/swap_test.py` & `blivet-3.8.0/tests/unit_tests/formats_tests/swap_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/gpt_test.py` & `blivet-3.8.0/tests/unit_tests/gpt_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/misc_test.py` & `blivet-3.8.0/tests/unit_tests/misc_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/parentlist_test.py` & `blivet-3.8.0/tests/unit_tests/parentlist_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/populator_test.py` & `blivet-3.8.0/tests/unit_tests/populator_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 except ImportError:
     from mock import call, patch, sentinel, Mock, PropertyMock
 
 import gi
 import six
 import unittest
 
-gi.require_version("BlockDev", "2.0")
+gi.require_version("BlockDev", "3.0")
 from gi.repository import BlockDev as blockdev
 
 from blivet.devices import DiskDevice, DMDevice, FileDevice, LoopDevice
 from blivet.devices import MDRaidArrayDevice, MultipathDevice, OpticalDevice
 from blivet.devices import PartitionDevice, StorageDevice, NVDIMMNamespaceDevice
 from blivet.devices import NVMeNamespaceDevice, NVMeFabricsNamespaceDevice
 from blivet.devicelibs import lvm
@@ -128,71 +128,71 @@
 
     def test_match(self, *args):
         """Test matching of loop device populator."""
         # LoopDevicePopulator.match just runs the check if device is loop
         # The backing file check is now performed in the "run" method.
         # Test intentionally left empty
 
-    @patch("blivet.populator.helpers.loop.blockdev.loop.get_backing_file")
+    @patch("blivet.populator.helpers.loop.blockdev.loop.info")
     @patch("blivet.udev.device_get_name")
     @patch("blivet.udev.device_is_dm", return_value=False)
     @patch("blivet.udev.device_is_dm_luks", return_value=False)
     @patch("blivet.udev.device_is_dm_integrity", return_value=False)
     @patch("blivet.udev.device_is_dm_lvm", return_value=False)
     @patch("blivet.udev.device_is_dm_mpath", return_value=False)
     @patch("blivet.udev.device_is_md", return_value=False)
     @patch("blivet.udev.device_is_loop", return_value=True)
     def test_get_helper(self, *args):
         """Test get_device_helper for loop devices."""
         device_is_loop = args[0]
-        get_backing_file = args[7]
+        loop_info = args[7]
         data = {'SYS_PATH': 'dummy'}
-        get_backing_file.return_value = True
+        loop_info.return_value = Mock(baking_file="foobar")
         self.assertEqual(get_device_helper(data), self.helper_class)
 
-        get_backing_file.return_value = False
+        loop_info.return_value = Mock(baking_file=None)
         self.assertEqual(get_device_helper(data), self.helper_class)
-        get_backing_file.return_value = True
+        loop_info.return_value = Mock(baking_file="foobar")
 
         # verify that setting one of the required True return values to False prevents success
         device_is_loop.return_value = False
         self.assertNotEqual(get_device_helper(data), self.helper_class)
         device_is_loop.return_value = True
 
         # You can't be assured that setting any of the False return values to True will trigger
         # a failure because the ordering is not complete, meaning any of several device helpers
         # could be the first helper class checked.
 
     @patch.object(DeviceTree, "get_device_by_name")
     @patch.object(FileDevice, "status", return_value=True)
     @patch.object(LoopDevice, "status", return_value=True)
-    @patch("blivet.populator.helpers.loop.blockdev.loop.get_backing_file")
+    @patch("blivet.populator.helpers.loop.blockdev.loop.info")
     @patch("blivet.udev.device_get_name")
     @patch("blivet.udev.device_get_sysfs_path", return_value=sentinel.sysfs_path)
     def test_run(self, *args):
         """Test loop device populator."""
         device_get_name = args[1]
-        get_backing_file = args[2]
+        loop_info = args[2]
 
         devicetree = DeviceTree()
         data = Mock()
 
         # Add backing file and loop device.
         devicetree.get_device_by_name.return_value = None
         device_name = "loop3"
         device_get_name.return_value = device_name
         backing_file = "/some/file"
 
-        get_backing_file.return_value = None
+        loop_info.return_value = Mock(backing_file=None)
         helper = self.helper_class(devicetree, data)
         device = helper.run()
 
         self.assertIsNone(device)
 
-        get_backing_file.return_value = backing_file
+        loop_info.return_value = Mock(backing_file=backing_file)
 
         device = helper.run()
 
         self.assertIsInstance(device, LoopDevice)
         self.assertTrue(device in devicetree.devices)
         self.assertTrue(device.exists)
         self.assertEqual(device.name, device_name)
@@ -387,15 +387,15 @@
         device_is_partition.return_value = False
         self.assertNotEqual(get_device_helper(data), self.helper_class)
         device_is_partition.return_value = True
 
         # verify that setting one of the required False return values to True prevents success
         # as of now, loop is always checked before partition
         device_is_loop.return_value = True
-        with patch("blivet.populator.helpers.loop.blockdev.loop.get_backing_file", return_value=True):
+        with patch("blivet.populator.helpers.loop.blockdev.loop.info", return_value=Mock(backing_file="foobar")):
             self.assertNotEqual(get_device_helper(data), self.helper_class)
 
         device_is_loop.return_value = False
 
     @patch.object(DiskDevice, "partitioned")
     @patch.object(DiskLabel, "parted_disk")
     @patch.object(DiskLabel, "parted_device")
```

### Comparing `blivet-3.7.1/tests/unit_tests/size_test.py` & `blivet-3.8.0/tests/unit_tests/size_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/tags_test.py` & `blivet-3.8.0/tests/unit_tests/tags_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/task_tests.py` & `blivet-3.8.0/tests/unit_tests/task_tests.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/tsort_test.py` & `blivet-3.8.0/tests/unit_tests/tsort_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/udev_data/raid_data.py` & `blivet-3.8.0/tests/unit_tests/udev_data/raid_data.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/udev_test.py` & `blivet-3.8.0/tests/unit_tests/udev_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/unit_tests/util_test.py` & `blivet-3.8.0/tests/unit_tests/util_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/vmtests/README.rst` & `blivet-3.8.0/tests/vmtests/README.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/vmtests/blivet_reset_vmtest.py` & `blivet-3.8.0/tests/vmtests/blivet_reset_vmtest.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/vmtests/gpt_test.py` & `blivet-3.8.0/tests/vmtests/gpt_test.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/vmtests/runvmtests.py` & `blivet-3.8.0/tests/vmtests/runvmtests.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/tests/vmtests/vmbackedtestcase.py` & `blivet-3.8.0/tests/vmtests/vmbackedtestcase.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/COPYING` & `blivet-3.8.0/translation-canary/COPYING`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/README.rst` & `blivet-3.8.0/translation-canary/README.rst`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/tests/project-tests/test_projects.sh` & `blivet-3.8.0/translation-canary/tests/project-tests/test_projects.sh`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/tests/unittests/test_translatable.py` & `blivet-3.8.0/translation-canary/tests/unittests/test_translatable.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/tests/unittests/test_translated.py` & `blivet-3.8.0/translation-canary/tests/unittests/test_translated.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/translation_canary/translatable/__init__.py` & `blivet-3.8.0/translation-canary/translation_canary/translatable/__init__.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/translation_canary/translatable/__main__.py` & `blivet-3.8.0/translation-canary/translation_canary/translatable/__main__.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/translation_canary/translatable/test_comment.py` & `blivet-3.8.0/translation-canary/translation_canary/translatable/test_comment.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/translation_canary/translatable/test_markup.py` & `blivet-3.8.0/translation-canary/translation_canary/translatable/test_markup.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/translation_canary/translated/__init__.py` & `blivet-3.8.0/translation-canary/translation_canary/translated/__init__.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/translation_canary/translated/__main__.py` & `blivet-3.8.0/translation-canary/translation_canary/translated/__main__.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/translation_canary/translated/test_markup.py` & `blivet-3.8.0/translation-canary/translation_canary/translated/test_markup.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/translation_canary/translated/test_percentage.py` & `blivet-3.8.0/translation-canary/translation_canary/translated/test_percentage.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/translation_canary/translated/test_usability.py` & `blivet-3.8.0/translation-canary/translation_canary/translated/test_usability.py`

 * *Files identical despite different names*

### Comparing `blivet-3.7.1/translation-canary/xgettext_werror.sh` & `blivet-3.8.0/translation-canary/xgettext_werror.sh`

 * *Files identical despite different names*

