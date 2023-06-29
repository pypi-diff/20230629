# Comparing `tmp/cruiz-1.4.0a1.tar.gz` & `tmp/cruiz-1.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cruiz-1.4.0a1.tar", last modified: Sun Jun 18 19:35:41 2023, max compression
+gzip compressed data, was "cruiz-1.4.0a2.tar", last modified: Thu Jun 29 07:29:31 2023, max compression
```

## Comparing `cruiz-1.4.0a1.tar` & `cruiz-1.4.0a2.tar`

### file list

```diff
@@ -1,232 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.214604 cruiz-1.4.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-18 19:35:41.214604 cruiz-1.4.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.170604 cruiz-1.4.0a1/cruiz/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz/RELEASE_VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1828 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.174605 cruiz-1.4.0a1/cruiz/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      303 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/conanconf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1677 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/conanenv.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6322 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/conaninvocation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25506 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/guardedlisttoflush.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2401 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/logdetails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4289 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/messagereplyprocessor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5721 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/metarequestconaninvocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/dumpobjecttypes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3769 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.174605 cruiz-1.4.0a1/cruiz/interop/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13930 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/commandparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/commonparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/packagebinaryparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/packageidparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/packagenode.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/packagerevisionsparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/reciperevisionsparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/searchrecipesparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.174605 cruiz-1.4.0a1/cruiz/load_recipe/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/loadrecipewizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.178604 cruiz-1.4.0a1/cruiz/load_recipe/pages/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/pages/initialprofilepage.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/pages/intropage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/pages/localcachepage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/pages/packageversionpage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28384 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.178604 cruiz-1.4.0a1/cruiz/manage_local_cache/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34261 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/managelocalcachesdialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.178604 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addenvironmentdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2425 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2570 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addremotedialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/configpathorurl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3695 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/installconfigdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/keyvaluetable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7891 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/movelocalcachedialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7052 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/newlocalcachewizard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1683 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/progressdialogs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4933 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/remotestable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2062 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/runconancommanddialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.182604 cruiz-1.4.0a1/cruiz/model/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/model/conanpackagetypeflags.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/model/graphaslistmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.182604 cruiz-1.4.0a1/cruiz/pyside6/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/pyside6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.182604 cruiz-1.4.0a1/cruiz/recipe/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/dependencyview.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1206 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/expressioneditordialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1586 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/findtextdialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.182604 cruiz-1.4.0a1/cruiz/recipe/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/logs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6110 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/logs/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2234 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/recipe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58859 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/recipewidget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.182604 cruiz-1.4.0a1/cruiz/recipe/toolbars/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/toolbars/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6096 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/toolbars/behaviour.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9887 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/toolbars/buildfeatures.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30694 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/toolbars/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.186604 cruiz-1.4.0a1/cruiz/remote_browser/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.186604 cruiz-1.4.0a1/cruiz/remote_browser/pages/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/packagebinarypage.py
--rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/packageidpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/packagereferencepage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/packagerevisionpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/reciperevisionpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/remotebrowser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resourcegeneration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.194604 cruiz-1.4.0a1/cruiz/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/001-rubbish.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/002-null.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/003-chemistry.svg
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/004-share.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/005-box.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/006-toolbox.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/007-book.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/008-cloud-computing.svg
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/009-import.svg
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/010-draw.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/012-hammer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/013-pencil.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/014-code.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/Cmake.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/about_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/cruise.png
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/cruizres.qrc
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/find_text_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    53573 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/license-cruise.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    96863 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/license.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/load_recipe_wizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_add_environment.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_add_profile_directory.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_add_remote.ui
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_install_config.ui
--rw-r--r--   0 runner    (1001) docker     (123)    26699 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_manage.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_move.ui
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_new_wizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_remove_environment.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_run_command_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/preferences.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_cmake_features_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_compilercache_features_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_cpucores_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_local_workflow_expression_editor.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_profile_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)    33767 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)    28688 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/remote_browser.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/remote_browser_fileview.ui
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/revealonfilesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.194604 cruiz-1.4.0a1/cruiz/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/ensuredefaultlocalcache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.202604 cruiz-1.4.0a1/cruiz/settings/managers/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10185 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/basesettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4871 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/cleansettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1728 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/cmakepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3244 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/compilercachepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2499 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/conanpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2309 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/fontpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/generalpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1890 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/graphvizpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3903 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/localcachepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14295 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/namedlocalcache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/ninjapreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3681 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/recentconanconfigs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3590 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/recentconanremotes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/recentrecipes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18314 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/recipe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/restoredefaults.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7928 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/shortcuts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/valueclasses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4187 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/writermixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.202604 cruiz-1.4.0a1/cruiz/settings/models/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/models/recentconanconfigmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/models/recentconanremotesmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2727 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/models/recipesmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    53761 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/preferencesdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14331 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/updatesettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5848 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/svggraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.202604 cruiz-1.4.0a1/cruiz/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/widgets/aboutcruizdialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/widgets/debugging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1387 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/widgets/shortcutlineedit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2050 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/widgets/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.214604 cruiz-1.4.0a1/cruiz/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/arbitrary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/build.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2148 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/cmakebuildtool.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/configinstall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/create.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/deletecmakecache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      325 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/endmessagethread.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/exportpackage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/imports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/install.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4826 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/lockcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15302 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/meta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      968 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/package.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1704 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/packagebinary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1339 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/packagedetails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/packagerevisions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/reciperevisions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2169 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/remotesearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      696 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/removeallpackages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      506 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/removelocks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      967 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/removepackage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/source.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1092 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/testpackage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.214604 cruiz-1.4.0a1/cruiz/workers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/colorarma_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/conanapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/formatoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/message.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7679 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/monkeypatch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1588 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/qtlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/text2html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.170604 cruiz-1.4.0a1/cruiz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 19:35:41.214604 cruiz-1.4.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.092252 cruiz-1.4.0a2/cruiz/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz/RELEASE_VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1828 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.092252 cruiz-1.4.0a2/cruiz/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/conanconf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/conanenv.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6322 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/conaninvocation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25565 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/guardedlisttoflush.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2401 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/logdetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4189 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/messagereplyprocessor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5555 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/metarequestconaninvocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/dumpobjecttypes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3770 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/commandparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/commonparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/packagebinaryparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/packageidparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/packagenode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/packagerevisionsparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/reciperevisionsparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/searchrecipesparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/load_recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/loadrecipewizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/load_recipe/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/pages/initialprofilepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/pages/intropage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/pages/localcachepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/pages/packageversionpage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28296 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/manage_local_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36004 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/managelocalcachesdialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addenvironmentdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2425 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2570 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addremotedialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/configpathorurl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3712 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/installconfigdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/keyvaluetable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8370 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/movelocalcachedialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7548 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/newlocalcachewizard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1683 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/progressdialogs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4933 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/remotestable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2239 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/runconancommanddialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/model/conanpackagetypeflags.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/model/graphaslistmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/pyside6/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/pyside6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.100252 cruiz-1.4.0a2/cruiz/recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/dependencyview.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1206 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/expressioneditordialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1586 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/findtextdialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.100252 cruiz-1.4.0a2/cruiz/recipe/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/logs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6022 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/logs/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2234 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/recipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59849 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/recipewidget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.100252 cruiz-1.4.0a2/cruiz/recipe/toolbars/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/toolbars/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6621 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/toolbars/behaviour.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9887 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/toolbars/buildfeatures.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32749 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/toolbars/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.100252 cruiz-1.4.0a2/cruiz/remote_browser/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.100252 cruiz-1.4.0a2/cruiz/remote_browser/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/packagebinarypage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/packageidpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/packagereferencepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/packagerevisionpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/reciperevisionpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/remotebrowser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resourcegeneration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.104252 cruiz-1.4.0a2/cruiz/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/001-rubbish.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/002-null.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/003-chemistry.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/004-share.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/005-box.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/006-toolbox.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/007-book.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/008-cloud-computing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/009-import.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/010-draw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/012-hammer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/013-pencil.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/014-code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/Cmake.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/about_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/cruise.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/cruizres.qrc
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/find_text_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    53573 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/license-cruise.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    96863 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/license.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/load_recipe_wizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_add_environment.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_add_profile_directory.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_add_remote.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_install_config.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    27112 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_manage.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_move.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_new_wizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_remove_environment.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_run_command_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    41069 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/preferences.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_cmake_features_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_compilercache_features_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_cpucores_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_local_workflow_expression_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_profile_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    33767 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    28688 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/remote_browser.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/remote_browser_fileview.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/revealonfilesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.104252 cruiz-1.4.0a2/cruiz/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/ensuredefaultlocalcache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/settings/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10185 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/basesettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4871 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/cleansettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1728 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/cmakepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3244 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/compilercachepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2499 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/conanpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2309 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/fontpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/generalpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1890 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/graphvizpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3903 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/localcachepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14295 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/namedlocalcache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/ninjapreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3681 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/recentconanconfigs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3590 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/recentconanremotes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/recentrecipes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18314 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/recipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/restoredefaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7928 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/shortcuts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/valueclasses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4187 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/writermixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/settings/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/models/recentconanconfigmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/models/recentconanremotesmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2727 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/models/recipesmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54673 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/preferencesdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14331 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/updatesettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5848 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/svggraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/widgets/aboutcruizdialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/widgets/debugging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1387 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/widgets/shortcutlineedit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2050 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/widgets/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/workers/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/workers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/colorarma_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/formatoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/qtlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/text2html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.092252 cruiz-1.4.0a2/cruiz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/setup.py
```

### Comparing `cruiz-1.4.0a1/LICENSE` & `cruiz-1.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/PKG-INFO` & `cruiz-1.4.0a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cruiz
-Version: 1.4.0a1
+Version: 1.4.0a2
 Summary: Conan recipe user interface
 Home-page: https://github.com/markfinal/cruiz
 Author: Mark Final
 Author-email: markfinal@hotmail.com
 Project-URL: Documentation, https://cruiz.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/markfinal/cruiz
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,24 +34,29 @@
 See the documentation at [Read The Docs](https://cruiz.readthedocs.io/).
 
 ## Prerequisites
 
 - Intel x86_64 platforms:
   - Windows 10+
   - Linux (CentOS 7.5+/Ubuntu 18+)
-  - macOS (10.13+)
+  - macOS (11.0+)
 - Apple Silicon platforms:
   - macOS (11.0+)
 - Python 3.7-3.11
-- Conan 1.17.1+, but not 2.x (these are the versions tested)
+- Conan 1.x (from 1.17.1 onwards) and 2.x (from 2.0.7 onwards)
 
 All other Python dependencies are installed when the package is installed.
 
 In order to use the dependency graph visualisation, an additional installation of GraphViz is required from https://graphviz.org/download/. Assign the installed location to the preferences.
 
+## Conan versions
+Cruiz does _not_ depend directly on the Conan package in its UI. Instead, it uses child processes to run Conan APIs, which _are_ dependent on the Conan version installed.
+
+Cruiz does _not_ support multiple Conan versions simultaneously in the same process. Instead, the UI dynamically changes by detecting the Conan version installed at startup. You will therefore see a slightly different UI depending on which Conan you have. Note the Conan version detected is shown on the status bar in the bottom right corner of the UI.
+
 ## Getting started
 If you have cloned this repository, you will need:
 
 1. A Python 3 environment. Make a virtual env if necessary. `python3 -m venv <folder to be the env>`
     - Activate the virtual env with either:
         - `source <folder to be the env>/bin/activate` (Linux/macOSX)
         - `<folder to be the env>\Scripts\activate.bat` (Windows cmd)
```

### Comparing `cruiz-1.4.0a1/README.md` & `cruiz-1.4.0a2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,24 +11,29 @@
 See the documentation at [Read The Docs](https://cruiz.readthedocs.io/).
 
 ## Prerequisites
 
 - Intel x86_64 platforms:
   - Windows 10+
   - Linux (CentOS 7.5+/Ubuntu 18+)
-  - macOS (10.13+)
+  - macOS (11.0+)
 - Apple Silicon platforms:
   - macOS (11.0+)
 - Python 3.7-3.11
-- Conan 1.17.1+, but not 2.x (these are the versions tested)
+- Conan 1.x (from 1.17.1 onwards) and 2.x (from 2.0.7 onwards)
 
 All other Python dependencies are installed when the package is installed.
 
 In order to use the dependency graph visualisation, an additional installation of GraphViz is required from https://graphviz.org/download/. Assign the installed location to the preferences.
 
+## Conan versions
+Cruiz does _not_ depend directly on the Conan package in its UI. Instead, it uses child processes to run Conan APIs, which _are_ dependent on the Conan version installed.
+
+Cruiz does _not_ support multiple Conan versions simultaneously in the same process. Instead, the UI dynamically changes by detecting the Conan version installed at startup. You will therefore see a slightly different UI depending on which Conan you have. Note the Conan version detected is shown on the status bar in the bottom right corner of the UI.
+
 ## Getting started
 If you have cloned this repository, you will need:
 
 1. A Python 3 environment. Make a virtual env if necessary. `python3 -m venv <folder to be the env>`
     - Activate the virtual env with either:
         - `source <folder to be the env>/bin/activate` (Linux/macOSX)
         - `<folder to be the env>\Scripts\activate.bat` (Windows cmd)
```

### Comparing `cruiz-1.4.0a1/cruiz/application.py` & `cruiz-1.4.0a2/cruiz/application.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/commands/conanenv.py` & `cruiz-1.4.0a2/cruiz/commands/conanenv.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """
 Get environment for Conan
 """
 
 import logging
 import typing
 
+import cruiz.globals
+
 from cruiz.settings.managers.conanpreferences import ConanSettingsReader
 from cruiz.settings.managers.generalpreferences import GeneralSettingsReader
 from cruiz.settings.managers.namedlocalcache import NamedLocalCacheSettingsReader
 
 
 logger = logging.getLogger(__name__)
 
@@ -26,22 +28,28 @@
     """
     with NamedLocalCacheSettingsReader(cache_name) as settings:
         home_dir = settings.home_dir.resolve()
         short_home_dir = settings.short_home_dir.resolve()
         added_environment = settings.environment_added.resolve()
         removed_environment = settings.environment_removed.resolve()
     env: typing.Dict[str, str] = {}
-    if home_dir:
-        env["CONAN_USER_HOME"] = home_dir
-    if short_home_dir:
-        env["CONAN_USER_HOME_SHORT"] = short_home_dir
+    if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+        if home_dir:
+            env["CONAN_USER_HOME"] = home_dir
+        if short_home_dir:
+            env["CONAN_USER_HOME_SHORT"] = short_home_dir
+    else:
+        if home_dir:
+            env["CONAN_HOME"] = home_dir
+        # short home no longer needed
     with GeneralSettingsReader() as settings:
         use_dark_mode = settings.use_dark_mode.resolve()
     env["CONAN_COLOR_DARK"] = "0" if use_dark_mode else "1"
-    with ConanSettingsReader() as settings:
-        log_level = settings.log_level.resolve()
-    env["CONAN_LOGGING_LEVEL"] = log_level
-    env["CONAN_NON_INTERACTIVE"] = "1"
+    if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+        with ConanSettingsReader() as settings:
+            log_level = settings.log_level.resolve()
+            env["CONAN_LOGGING_LEVEL"] = log_level
+        env["CONAN_NON_INTERACTIVE"] = "1"
     # custom environment variables - this is where cruiz behaviour might vary
     # from Conan on the command line
     env.update(added_environment)
     return (env, removed_environment)
```

### Comparing `cruiz-1.4.0a1/cruiz/commands/conaninvocation.py` & `cruiz-1.4.0a2/cruiz/commands/conaninvocation.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/commands/context.py` & `cruiz-1.4.0a2/cruiz/commands/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,46 +9,26 @@
 import pathlib
 import typing
 
 from qtpy import QtCore, QtWidgets
 
 from cruiz.exceptions import RecipeInspectionError
 
-import cruiz.interop.dependencygraph
 from cruiz.interop.packagenode import PackageNode
 from cruiz.interop.pod import ConanRemote, ConanHook
 from cruiz.interop.commandparameters import CommandParameters
 from cruiz.interop.searchrecipesparameters import SearchRecipesParameters
 from cruiz.interop.reciperevisionsparameters import RecipeRevisionsParameters
 from cruiz.interop.packageidparameters import PackageIdParameters
 from cruiz.interop.packagerevisionsparameters import PackageRevisionsParameters
 from cruiz.interop.packagebinaryparameters import PackageBinaryParameters
 from cruiz.recipe.logs.command import CommandListWidgetItem
 from cruiz.settings.managers.namedlocalcache import NamedLocalCacheSettingsReader
 
-import cruiz.workers.create
-import cruiz.workers.imports
-import cruiz.workers.install
-import cruiz.workers.source
-import cruiz.workers.build
-import cruiz.workers.package
-import cruiz.workers.exportpackage
-import cruiz.workers.testpackage
-import cruiz.workers.cmakebuildtool
-import cruiz.workers.deletecmakecache
-import cruiz.workers.removepackage
-import cruiz.workers.removeallpackages
-import cruiz.workers.removelocks
-import cruiz.workers.configinstall
-import cruiz.workers.remotesearch
-import cruiz.workers.reciperevisions
-import cruiz.workers.packagedetails
-import cruiz.workers.packagerevisions
-import cruiz.workers.packagebinary
-import cruiz.workers.arbitrary
+import cruiz.workers.api as workers_api
 
 from cruiz.recipe.logs.command import RecipeCommandHistoryWidget
 from cruiz.constants import DEFAULT_CACHE_NAME
 
 from .conaninvocation import ConanInvocation
 from .metarequestconaninvocation import MetaRequestConanInvocation
 from .conanenv import get_conan_env
@@ -110,21 +90,21 @@
             self._meta_invocation.close()
             self._meta_invocation.deleteLater()
             del self._meta_invocation
         except AttributeError:
             # don't double close this
             pass
 
-    def change_cache(self, cache_name: str) -> None:
+    def change_cache(self, cache_name: str, force: bool = False) -> None:
         """
         Change the local cache used by this context.
         """
         # don't even try to check for a name no-op if the cache has already been closed
         if hasattr(self, "_meta_invocation"):
-            if cache_name == self.cache_name:
+            if cache_name == self.cache_name and not force:
                 return
             assert not self.is_busy
             self.close()
         self._configure_to_local_cache(cache_name)
 
     def _configure_to_local_cache(self, cache_name: str) -> None:
         self.cache_name = cache_name
@@ -286,27 +266,27 @@
         self,
         continuation: typing.Optional[typing.Callable[[typing.Any, typing.Any], None]],
     ) -> None:
         """
         Run 'conan remove [-f] *'
         """
         params = CommandParameters(
-            "removeallpackages", cruiz.workers.removeallpackages.invoke
+            "removeallpackages", workers_api.removeallpackages.invoke
         )
         params.force = True
         self._start_invocation(params, None, continuation)
 
     def remove_local_cache_locks(
         self,
         continuation: typing.Optional[typing.Callable[[typing.Any, typing.Any], None]],
     ) -> None:
         """
         Run 'conan remove --locks' to remove all lock files from the local cache
         """
-        params = CommandParameters("removelocks", cruiz.workers.removelocks.invoke)
+        params = CommandParameters("removelocks", workers_api.removelocks.invoke)
         self._start_invocation(params, None, continuation)
 
     def install_config(
         self,
         params: CommandParameters,
         continuation: typing.Optional[
             typing.Callable[[typing.Any, typing.Any], None]
@@ -475,23 +455,24 @@
         )
 
     def get_list_of_profiles(self) -> typing.List[typing.Tuple[pathlib.Path, str]]:
         """
         Return a list of all profiles in this context.
         """
         profile_paths: typing.List[typing.Tuple[pathlib.Path, str]] = []
+        # TODO: Conan2 candidate: api.profiles.list() for the local-cache based profiles
         profiles_dir = QtCore.QDir(str(self.profiles_dir()))
         for profile in profiles_dir.entryList(  # type: ignore
             filters=QtCore.QDir.Files
         ):
             # local cache profiles are listed relative
             path = pathlib.Path(profiles_dir.filePath(profile))
             text = path.read_text()
             profile_paths.append((pathlib.Path(path.name), text))
-        assert profile_paths
+        # in Conan 2, there can be no profiles at this point
         with NamedLocalCacheSettingsReader(self.cache_name) as settings:
             extra_profile_dirs = settings.extra_profile_directories.resolve()
         for _, extra_profile_dir in extra_profile_dirs.items():
             profiles_dir = QtCore.QDir(extra_profile_dir)
             for profile in profiles_dir.entryList(  # type: ignore
                 filters=QtCore.QDir.Files
             ):
@@ -690,14 +671,28 @@
     def is_busy(self) -> bool:
         """
         Is the context busy running any Conan commands?
         Explicitly or via its meta commands
         """
         return bool(self._invocations) or self._meta_invocation.active
 
+    def create_default_profile(self) -> None:
+        """
+        Create the default profile in the local cache by detecting the environment.
+        This will overwrite any existing default profile.
+        """
+        _, exception = self._meta_invocation.request_data("create_default_profile")
+        if exception:
+            if self.parent():
+                self.parent().record_exception(exception)
+            else:
+                raise Exception(
+                    "Creating the default profile for the local cache failed"
+                ) from exception
+
 
 @contextmanager
 def managed_conan_context(
     cache_name: str, log_details: LogDetails
 ) -> typing.Generator[ConanContext, None, None]:
     """
     Context manager for uses where all API calls on the ConanContext are guaranteed
```

### Comparing `cruiz-1.4.0a1/cruiz/commands/guardedlisttoflush.py` & `cruiz-1.4.0a2/cruiz/commands/guardedlisttoflush.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/commands/logdetails.py` & `cruiz-1.4.0a2/cruiz/commands/logdetails.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/commands/messagereplyprocessor.py` & `cruiz-1.4.0a2/cruiz/commands/messagereplyprocessor.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,16 +12,24 @@
 import sys
 import typing
 
 from qtpy import QtCore
 
 from cruiz.dumpobjecttypes import dump_object_types
 
-import cruiz.workers.endmessagethread
-import cruiz.workers.utils.message
+import cruiz.workers.api as workers_api
+from cruiz.interop.message import (
+    Message,
+    End,
+    Stdout,
+    Stderr,
+    Success,
+    Failure,
+    ConanLogMessage,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class MessageReplyProcessor(QtCore.QObject):
     """
     Process replies across a multiprocessing Queue in a background thread.
@@ -36,28 +44,28 @@
     critical_failure = QtCore.Signal(str)
 
     def __del__(self) -> None:
         logger.debug("-=%d", id(self))
 
     def __init__(
         self,
-        queue: multiprocessing.Queue[cruiz.workers.utils.message.Message],
+        queue: multiprocessing.Queue[Message],
     ):
         logger.debug("+=%d", id(self))
         super().__init__()
         self._mp_context = multiprocessing.get_context("spawn")
         self._queue = queue
 
     def stop(self) -> None:
         """
         Stop the background thread.
         """
         # start a process to shut down the thread
         shutdown_process = self._mp_context.Process(
-            target=cruiz.workers.endmessagethread.invoke, args=(self._queue,)
+            target=workers_api.endmessagethread.invoke, args=(self._queue,)
         )
         shutdown_process.start()
         shutdown_process.join()
         shutdown_process.close()
 
     def __check_for_conan_leakage(self, entry: typing.Any = None) -> bool:
         if "conans" not in sys.modules:
@@ -86,25 +94,25 @@
             logger.debug("(%d) wait for queue entry...", id(self))
             try:
                 if not self.__check_for_conan_leakage(None):
                     break
                 entry = self._queue.get()
                 if not self.__check_for_conan_leakage(entry):
                     break
-                if isinstance(entry, cruiz.workers.utils.message.End):
+                if isinstance(entry, End):
                     break
-                if isinstance(entry, cruiz.workers.utils.message.Stdout):
+                if isinstance(entry, Stdout):
                     self.stdout_message.emit(entry.message())
-                elif isinstance(entry, cruiz.workers.utils.message.Stderr):
+                elif isinstance(entry, Stderr):
                     self.stderr_message.emit(entry.message())
-                elif isinstance(entry, cruiz.workers.utils.message.ConanLogMessage):
+                elif isinstance(entry, ConanLogMessage):
                     self.conan_log_message.emit(entry.message())
-                elif isinstance(entry, cruiz.workers.utils.message.Success):
+                elif isinstance(entry, Success):
                     self.completed.emit(entry.payload(), None)
-                elif isinstance(entry, cruiz.workers.utils.message.Failure):
+                elif isinstance(entry, Failure):
                     # TODO: temporary, at least always record the exception
                     # in the error log
                     self.stderr_message.emit(str(entry.exception()))
                     self.completed.emit(None, entry.exception())
                 else:
                     logger.error("Unknown message type: '%s'", entry)
             except EOFError as exception:
```

### Comparing `cruiz-1.4.0a1/cruiz/commands/metarequestconaninvocation.py` & `cruiz-1.4.0a2/cruiz/commands/metarequestconaninvocation.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,16 +11,22 @@
 import sys
 import typing
 import urllib.parse
 
 from qtpy import QtCore
 
 from cruiz.interop.commandparameters import CommandParameters
-import cruiz.workers.utils.message
-import cruiz.workers.meta
+from cruiz.interop.message import (
+    Success,
+    Failure,
+    Stdout,
+    Stderr,
+    ConanLogMessage,
+)
+import cruiz.workers.api as workers_api
 from cruiz.dumpobjecttypes import dump_object_types
 
 from .conanenv import get_conan_env
 from .logdetails import LogDetails
 
 
 logger = logging.getLogger(__name__)
@@ -44,15 +50,15 @@
         logger.debug("+=%d", id(self))
         super().__init__(parent)
         self._log_details = log_details
         self._mp_context = multiprocessing.get_context("spawn")
         self._request_queue = self._mp_context.JoinableQueue()
         self._reply_queue = self._mp_context.Queue()
         self.active = False
-        params = CommandParameters("meta", cruiz.workers.meta.invoke)
+        params = CommandParameters("meta", workers_api.meta.invoke)
         added_environment, removed_environment = get_conan_env(cache_name)
         params.added_environment.update(added_environment)
         params.removed_environment.extend(removed_environment)
         self._invoke_conan_process(params)
 
     def close(self) -> None:
         """
@@ -112,40 +118,40 @@
         logger.debug("* Requesting %s", meta_request)
         self._request_queue.put(meta_request)
         self.active = True
         logger.debug("* Requested %s waiting for reply", meta_request)
         # the requested task is done when there is a success or a failure
         self._request_queue.join()
         response: typing.Union[
-            cruiz.workers.utils.message.Success,
-            cruiz.workers.utils.message.Failure,
+            Success,
+            Failure,
             None,
         ] = None
         while True:
             MetaRequestConanInvocation.__check_for_conan_leakage(None)
             reply = self._reply_queue.get()
             MetaRequestConanInvocation.__check_for_conan_leakage(reply)
-            if isinstance(reply, cruiz.workers.utils.message.Stdout):
+            if isinstance(reply, Stdout):
                 logger.debug("* Got stdout message: '%s", reply.message())
                 self._log_details.stdout(reply.message())
-            elif isinstance(reply, cruiz.workers.utils.message.Stderr):
+            elif isinstance(reply, Stderr):
                 logger.debug("* Got stderr message: '%s", reply.message())
                 self._log_details.stderr(reply.message())
-            elif isinstance(reply, cruiz.workers.utils.message.ConanLogMessage):
+            elif isinstance(reply, ConanLogMessage):
                 logger.debug("* Got Conan log message: '%s", reply.message())
                 self._log_details.conan_log(reply.message())
-            elif isinstance(reply, cruiz.workers.utils.message.Success):
+            elif isinstance(reply, Success):
                 logger.debug("* Requested %s got reply '%s'", meta_request, reply)
                 response = reply
                 break
-            elif isinstance(reply, cruiz.workers.utils.message.Failure):
+            elif isinstance(reply, Failure):
                 logger.debug("* Got failure message: '%s'", str(reply.exception()))
                 response = reply
                 break
         assert self._reply_queue.empty()
         self.active = False
         if response is not None:
-            if isinstance(reply, cruiz.workers.utils.message.Success):
+            if isinstance(reply, Success):
                 return (response.payload(), None)  # type: ignore
-            if isinstance(reply, cruiz.workers.utils.message.Failure):
+            if isinstance(reply, Failure):
                 return (None, response.exception())  # type: ignore
         raise RuntimeError("No success message")
```

### Comparing `cruiz-1.4.0a1/cruiz/constants.py` & `cruiz-1.4.0a2/cruiz/constants.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/dumpobjecttypes.py` & `cruiz-1.4.0a2/cruiz/dumpobjecttypes.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/entrypoint.py` & `cruiz-1.4.0a2/cruiz/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,26 @@
 import sys
 
 from qtpy import QtCore, QtWidgets
 
 from cruiz.resourcegeneration import generate_resources
 
 
+CONAN_SPEC = importlib.util.find_spec("conans")
+if CONAN_SPEC is None:
+    QtWidgets.QApplication()
+    QtWidgets.QMessageBox.critical(
+        None,  # type: ignore
+        "Conan unavailable",
+        "Unable to locate the conan Python package in the current environment.\n"
+        "Use pip install conan[==version].",
+    )
+    sys.exit(-1)
+
+
 logging.basicConfig(
     level=os.getenv("LOGLEVEL", "WARNING"),
     filename=os.getenv("LOGFILE", None),
 )
 
 
 logger = logging.getLogger(__name__)
@@ -31,25 +43,14 @@
 
 from cruiz.application import Application  # noqa: E402
 from cruiz.mainwindow import MainWindow  # noqa: E402
 from cruiz.settings.updatesettings import (  # noqa: E402
     update_settings_to_current_version,
 )
 
-CONAN_SPEC = importlib.util.find_spec("conans")
-if CONAN_SPEC is None:
-    QtWidgets.QApplication()
-    QtWidgets.QMessageBox.critical(
-        None,  # type: ignore
-        "Conan unavailable",
-        "Unable to locate the conan Python package in the current environment.\n"
-        "Use pip install conan[==version].",
-    )
-    sys.exit(-1)
-
 
 def _are_resources_out_of_date() -> bool:
     current_dir = pathlib.Path(__file__).parent
     resources_dir = current_dir / "resources"
     if not resources_dir.exists():
         return False
     generated_files = [
```

### Comparing `cruiz-1.4.0a1/cruiz/environ.py` & `cruiz-1.4.0a2/cruiz/environ.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/exceptions.py` & `cruiz-1.4.0a2/cruiz/exceptions.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/interop/commandparameters.py` & `cruiz-1.4.0a2/cruiz/interop/commandparameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 Conan command parameters
 """
 
 from io import StringIO
 import pathlib
 import typing
 
+import cruiz.globals
+
 from cruiz.constants import BuildFeatureConstants
 
 from .commonparameters import CommonParameters
 
 
 # TODO: should a recipe be in here? it is quite a heavyweight Context object though
 class CommandParameters(CommonParameters):
@@ -36,66 +38,115 @@
         self._profile: typing.Optional[str] = None
         self._common_subdir: typing.Optional[pathlib.PurePosixPath] = None
         self._install_folder: typing.Optional[pathlib.PurePosixPath] = None
         self._imports_folder: typing.Optional[pathlib.PurePosixPath] = None
         self._source_folder: typing.Optional[pathlib.PurePosixPath] = None
         self._build_folder: typing.Optional[pathlib.PurePosixPath] = None
         self._package_folder: typing.Optional[pathlib.PurePosixPath] = None
-        self._test_folder: typing.Optional[pathlib.PurePosixPath] = None
+        self._test_build_folder: typing.Optional[pathlib.PurePosixPath] = None
         self._name: typing.Optional[str] = None
         self._version: typing.Optional[
             str
         ] = None  # TODO: these are aliased with the recipe, so should we store it?
         self._user: typing.Optional[str] = None
         self._channel: typing.Optional[str] = None
         self._options: typing.Dict[str, str] = {}
         self._force: typing.Optional[bool] = None
         self._package_reference: typing.Optional[str] = None
         self._args: typing.List[str] = []
         self._named_args: typing.Dict[str, str] = {}
         self._time_commands: typing.Optional[bool] = None
+        self._v2_omit_test_folder: typing.Optional[bool] = None
+        self._v2_needs_reference: typing.Optional[bool] = None
 
-    def __str__(self) -> str:
-        components = ["conan"]
-        components.append(self.verb)
-        if self._install_folder:
-            components.extend(["-if", str(self._install_folder)])
-        if self._imports_folder:
-            components.extend(["-imf", str(self._imports_folder)])
-        if self._source_folder:
-            components.extend(["-sf", str(self._source_folder)])
-        if self._build_folder:
-            components.extend(["-bf", str(self._build_folder)])
-        if self._package_folder:
-            components.extend(["-pf", str(self._package_folder)])
-        if self._test_folder:
-            components.extend(["-tbf", str(self._test_folder)])
+    def to_args(self) -> typing.List[str]:
+        """
+        Get the argument list corresponding to these command parameters.
+        """
+        components = [self.verb]
         if self._profile:
             components.extend(
                 [
                     "-pr",
                     self._profile,
                 ]
             )
-        for key, value in self._options.items():
-            components.extend(
-                [
-                    "-o",
-                    f"{key}={value}",
-                ]
-            )
-        if self._force:
-            components.append("-f")
         if self._args:
+            # e.g. things like update
             components.extend(self._args)
-        # no named args
-        if self._recipe_path:
-            components.append(str(self._recipe_path))
-        if self._package_reference:
-            components.append(self._package_reference)
+        if cruiz.globals.CONAN_MAJOR_VERSION == 2:
+            for key, value in self._options.items():
+                key_split = key.split(":")
+                name = key_split[0]
+                option_name = key_split[1]
+                components.extend(
+                    [
+                        "-o",
+                        f"{name}/*:{option_name}={value}",
+                    ]
+                )
+            if not self._v2_needs_reference:
+                if self._name:
+                    components.extend(["--name", self._name])
+                if self._version:
+                    components.extend(["--version", self._version])
+                if self._user:
+                    components.extend(["--user", self._user])
+                if self._channel:
+                    components.extend(["--channel", self._channel])
+            if self.v2_omit_test_folder:
+                components.extend(["-tf", ""])
+            if self._force:
+                components.append("-c")
+            # no named args
+            if self._recipe_path:
+                components.append(str(self._recipe_path))
+            if self._v2_needs_reference and self._package_reference:
+                components.append(self._package_reference)
+        elif cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            if self._install_folder:
+                components.extend(["-if", str(self._install_folder)])
+            if self._imports_folder:
+                components.extend(["-imf", str(self._imports_folder)])
+            if self._source_folder:
+                components.extend(["-sf", str(self._source_folder)])
+            if self._build_folder:
+                components.extend(["-bf", str(self._build_folder)])
+            if self._package_folder:
+                components.extend(["-pf", str(self._package_folder)])
+            if self._test_build_folder:
+                components.extend(["-tbf", str(self._test_build_folder)])
+            for key, value in self._options.items():
+                components.extend(
+                    [
+                        "-o",
+                        f"{key}={value}",
+                    ]
+                )
+            if self._force:
+                components.append("-f")
+            # no named args
+            if self._recipe_path:
+                components.append(str(self._recipe_path))
+            if self._package_reference:
+                components.append(self._package_reference)
+        return components
+
+    def __str__(self) -> str:
+        components = ["conan"]
+        for comp in self.to_args():
+            if comp:
+                if "*" in comp:
+                    # dealing with options of the form <name>*:<opt>=<value>
+                    components.append(f'"{comp}"')
+                else:
+                    components.append(comp)
+            else:
+                # dealing with empty strings
+                components.append('""')
         command = " ".join(components)
         return command
 
     @property
     def cmd_expression(self) -> StringIO:
         """
         Get the expression valid in a CMD batch shell for this command
@@ -278,25 +329,25 @@
         return self._package_folder
 
     @package_folder.setter
     def package_folder(self, value: typing.Optional[pathlib.PurePosixPath]) -> None:
         self._package_folder = value
 
     @property
-    def test_folder(self) -> typing.Optional[pathlib.PurePosixPath]:
+    def test_build_folder(self) -> typing.Optional[pathlib.PurePosixPath]:
         """
         Get the test build folder to use in the command against this recipe.
         -tbf/--test-build-folder switch
         May be None to omit
         """
-        return self._test_folder
+        return self._test_build_folder
 
-    @test_folder.setter
-    def test_folder(self, value: typing.Optional[pathlib.PurePosixPath]) -> None:
-        self._test_folder = value
+    @test_build_folder.setter
+    def test_build_folder(self, value: typing.Optional[pathlib.PurePosixPath]) -> None:
+        self._test_build_folder = value
 
     @property
     def name(self) -> typing.Optional[str]:
         """
         Get the package name.
         May be None.
         """
@@ -421,7 +472,31 @@
         self._time_commands = value
 
     def set_build_feature(self, feature: BuildFeatureConstants, value: str) -> None:
         """
         Set an optional build feature
         """
         self.added_environment[str(feature)] = value
+
+    @property
+    def v2_omit_test_folder(self) -> typing.Optional[bool]:
+        """
+        Whether to omit to the test folder parameter
+        Conan v2+
+        """
+        return self._v2_omit_test_folder
+
+    @v2_omit_test_folder.setter
+    def v2_omit_test_folder(self, value: typing.Optional[bool]) -> None:
+        self._v2_omit_test_folder = value
+
+    @property
+    def v2_need_reference(self) -> typing.Optional[bool]:
+        """
+        Whether a package reference is actually needed.
+        Conan v2+
+        """
+        return self._v2_needs_reference
+
+    @v2_need_reference.setter
+    def v2_need_reference(self, value: typing.Optional[bool]) -> None:
+        self._v2_needs_reference = value
```

### Comparing `cruiz-1.4.0a1/cruiz/interop/dependencygraph.py` & `cruiz-1.4.0a2/cruiz/interop/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/interop/packagenode.py` & `cruiz-1.4.0a2/cruiz/interop/packagenode.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/interop/pod.py` & `cruiz-1.4.0a2/cruiz/interop/pod.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/interop/reciperevisionsparameters.py` & `cruiz-1.4.0a2/cruiz/interop/reciperevisionsparameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,12 +13,12 @@
     """
     Representation of all the arguments to get recipe revisions
 
     Attributes are dynamically added from the keyword-args passed in.
     """
 
     def __init__(self, **args: typing.Any) -> None:
-        import cruiz.workers.reciperevisions
+        import cruiz.workers.api as workers_api
 
-        super().__init__(cruiz.workers.reciperevisions.invoke)
+        super().__init__(workers_api.reciperevisions.invoke)
         for k, v in args.items():
             self.__setattr__(k, v)
```

### Comparing `cruiz-1.4.0a1/cruiz/interop/searchrecipesparameters.py` & `cruiz-1.4.0a2/cruiz/interop/searchrecipesparameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,12 +13,12 @@
     """
     Representation of all the arguments to search for a recipe
 
     Attributes are dynamically added from the keyword-args passed in.
     """
 
     def __init__(self, **args: typing.Any) -> None:
-        import cruiz.workers.remotesearch
+        import cruiz.workers.api as workers_api
 
-        super().__init__(cruiz.workers.remotesearch.invoke)
+        super().__init__(workers_api.remotesearch.invoke)
         for k, v in args.items():
             self.__setattr__(k, v)
```

### Comparing `cruiz-1.4.0a1/cruiz/load_recipe/loadrecipewizard.py` & `cruiz-1.4.0a2/cruiz/load_recipe/loadrecipewizard.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/load_recipe/pages/initialprofilepage.py` & `cruiz-1.4.0a2/cruiz/load_recipe/pages/initialprofilepage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/load_recipe/pages/localcachepage.py` & `cruiz-1.4.0a2/cruiz/load_recipe/pages/localcachepage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/load_recipe/pages/packageversionpage.py` & `cruiz-1.4.0a2/cruiz/load_recipe/pages/packageversionpage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/mainwindow.py` & `cruiz-1.4.0a2/cruiz/mainwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os
 import pathlib
 import platform
 import subprocess
 import time
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE6
+from qtpy import QtCore, QtGui, QtWidgets
 import psutil
 
 from cruiz.exceptions import (
     InconsistentSettingsError,
     RecipeAlreadyOpenError,
     RecipeDoesNotExistError,
     RecipeInspectionError,
@@ -55,19 +55,14 @@
 
 import cruiz.config
 
 import cruiz.globals
 
 logger = logging.getLogger(__name__)
 
-if PYSIDE6:
-    QAction = QtGui.QAction
-else:
-    QAction = QtWidgets.QAction
-
 
 class MainWindow(QtWidgets.QMainWindow):
     """
     The main window of the application
     """
 
     # pylint: disable=too-many-instance-attributes, too-many-locals
```

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/managelocalcachesdialog.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/managelocalcachesdialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 #!/usr/bin/env python3
 
 """
 Dialog for managing local caches
 """
 
+import dataclasses
 from enum import IntEnum
 import os
 import pathlib
 import platform
 import shutil
 import stat
 import typing
 
 from qtpy import QtCore, QtGui, QtWidgets
+
+import cruiz.globals
+
 from cruiz.commands.logdetails import LogDetails
 
 from cruiz.interop.pod import ConanHook
 from cruiz.settings.managers.namedlocalcache import (
     NamedLocalCacheSettings,
     NamedLocalCacheSettingsReader,
     NamedLocalCacheSettingsWriter,
@@ -92,14 +96,16 @@
         self._ui.conan_user_home_short.setReadOnly(True)
         open_short_user_home_action = QtGui.QAction(dir_icon, "", self)
         open_short_user_home_action.triggered.connect(self._open_conan_user_home_short)
         self._ui.conan_user_home_short.addAction(
             open_short_user_home_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
+        # profiles
+        self._ui.profilesCreateDefault.clicked.connect(self._profiles_create_default)
         # extra profiles
         self._ui.profilesTableButtons.button(QtWidgets.QDialogButtonBox.Open).setText(
             "+"
         )
         self._ui.profilesTableButtons.button(
             QtWidgets.QDialogButtonBox.Open
         ).clicked.connect(self._profiles_add)
@@ -110,18 +116,22 @@
             QtWidgets.QDialogButtonBox.Close
         ).clicked.connect(self._profiles_remove)
         self._ui.profilesTableButtons.button(
             QtWidgets.QDialogButtonBox.Close
         ).setEnabled(False)
         self._ui.profilesTable.itemSelectionChanged.connect(self._profiles_selection)
         # config
-        self._ui.configPrintRunCommands.toggled.connect(
-            self._config_toggle_printruncommands
-        )
-        self._ui.configRevisions.toggled.connect(self._config_toggle_revisions)
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            self._ui.configPrintRunCommands.toggled.connect(
+                self._config_toggle_printruncommands
+            )
+            self._ui.configRevisions.toggled.connect(self._config_toggle_revisions)
+        else:
+            self._ui.configPrintRunCommands.hide()
+            self._ui.configRevisions.hide()
         # environments
         # - adding
         self._ui.envTableButtons.button(QtWidgets.QDialogButtonBox.Open).setText("+")
         self._ui.envTableButtons.button(
             QtWidgets.QDialogButtonBox.Open
         ).clicked.connect(self._env_add_plus)
         self._ui.envTableButtons.button(QtWidgets.QDialogButtonBox.Close).setText("-")
@@ -168,17 +178,21 @@
         self._ui.remotesTable.remote_enabled.connect(self._remote_enabled)
         # hooks
         self._ui.hooksTable.itemChanged.connect(self._hooks_item_changed)
         # operations
         self._ui.operations_installConfigButton.clicked.connect(
             self._operations_install_config
         )
-        self._ui.operations_removeLocksButton.clicked.connect(
-            self._operations_remove_locks
-        )
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            self._ui.operations_removeLocksButton.clicked.connect(
+                self._operations_remove_locks
+            )
+        else:
+            # does not appear to be an equivalent operation in Conan 2
+            self._ui.operations_removeLocksButton.hide()
         self._ui.operations_removeAllPackagesButton.clicked.connect(
             self._operations_remove_all_packages
         )
         self._ui.moveCacheButton.clicked.connect(self._operations_move_cache)
         self._ui.deleteCacheButton.clicked.connect(self._operations_delete_cache)
         self._ui.runConanCommandButton.clicked.connect(self._operations_run_command)
         # log
@@ -292,28 +306,32 @@
             self._context.get_list_of_profiles()
         ):
             self._ui.profilesList.addItem(str(profile_path))
             item = self._ui.profilesList.item(i)
             item.setData(QtCore.Qt.ToolTipRole, profile_text)  # type: ignore[arg-type]
 
     def _update_cache_config(self) -> None:
-        with BlockSignals(self._ui.configPrintRunCommands) as blocked_widget:
-            blocked_widget.setCheckState(
-                QtCore.Qt.Checked
-                if self._context.get_boolean_config(
-                    ConanConfigBoolean.PRINT_RUN_COMMANDS, False
+        if self._ui.configPrintRunCommands.isVisible():
+            with BlockSignals(self._ui.configPrintRunCommands) as blocked_widget:
+                blocked_widget.setCheckState(
+                    QtCore.Qt.Checked
+                    if self._context.get_boolean_config(
+                        ConanConfigBoolean.PRINT_RUN_COMMANDS, False
+                    )
+                    else QtCore.Qt.Unchecked
+                )
+        if self._ui.configRevisions.isVisible():
+            with BlockSignals(self._ui.configRevisions) as blocked_widget:
+                blocked_widget.setCheckState(
+                    QtCore.Qt.Checked
+                    if self._context.get_boolean_config(
+                        ConanConfigBoolean.REVISIONS, False
+                    )
+                    else QtCore.Qt.Unchecked
                 )
-                else QtCore.Qt.Unchecked
-            )
-        with BlockSignals(self._ui.configRevisions) as blocked_widget:
-            blocked_widget.setCheckState(
-                QtCore.Qt.Checked
-                if self._context.get_boolean_config(ConanConfigBoolean.REVISIONS, False)
-                else QtCore.Qt.Unchecked
-            )
 
     def _update_cache_environment(
         self, env_added: typing.Dict[str, str], env_removed: typing.List[str]
     ) -> None:
         self._ui.envTable.setRowCount(0)
         for key, value in env_added.items():
             self._ui.envTable.add_key_value_pair(key, value)
@@ -327,14 +345,19 @@
         for remote in self._context.get_remotes_list():
             self._ui.remotesTable.add_remote(remote)
 
     def _update_cache_hooks(self) -> None:
         self._ui.hooksTable.setRowCount(0)
         hooks = self._context.get_hooks_list()
         self._ui.hooksTable.setRowCount(len(hooks))
+        if cruiz.globals.CONAN_MAJOR_VERSION > 1:
+            # in Conan 2, hooks are enabled when they are are present in the cache
+            self._ui.hooksTable.setColumnHidden(
+                ManageLocalCachesDialog._HooksTableColumnIndex.ENABLED, True
+            )
         for i, hook in enumerate(hooks):
             enabled_item = QtWidgets.QTableWidgetItem()
             enabled_item.setFlags(
                 QtCore.Qt.ItemIsEnabled  # type: ignore
                 | QtCore.Qt.ItemIsSelectable
                 | QtCore.Qt.ItemIsUserCheckable
             )
@@ -352,15 +375,16 @@
                     enabled_item,
                 )
                 blocked_widget.setItem(
                     i, ManageLocalCachesDialog._HooksTableColumnIndex.PATH, name_item
                 )
 
     def _update_cache_details(self, cache_name: str) -> None:
-        self._context.change_cache(cache_name)
+        force_change = self._context.cache_name == cache_name
+        self._context.change_cache(cache_name, force=force_change)
         with NamedLocalCacheSettingsReader(cache_name) as settings:
             home_dir = settings.home_dir.resolve()
             short_home_dir = settings.short_home_dir.resolve()
             env_added = settings.environment_added.resolve()
             env_removed = settings.environment_removed.resolve()
             extra_profile_dirs = settings.extra_profile_directories.resolve()
             recipe_uuids = settings.recipe_uuids
@@ -486,38 +510,43 @@
                 self._modifications["Remotes"] = {}
             if "Reordered" not in self._modifications["Remotes"]:
                 self._modifications["Remotes"]["Reordered"] = True
         self._modified.emit()
 
     def _remote_enabled(self, name: str, state: QtCore.Qt.CheckState) -> None:
         remotes = self._context.get_remotes_list()
-        try:
-            remote = next(item for item in remotes if item.name == name)
-            if remote.enabled == bool(state):
-                self._modifications["Remotes"]["Toggled"].remove(name)
-                if not self._modifications["Remotes"]["Toggled"]:
-                    del self._modifications["Remotes"]["Toggled"]
-                if not self._modifications["Remotes"]:
-                    del self._modifications["Remotes"]
-            else:
-                if "Remotes" not in self._modifications:
-                    self._modifications["Remotes"] = {}
-                if "Toggled" not in self._modifications["Remotes"]:
-                    self._modifications["Remotes"]["Toggled"] = []
-                self._modifications["Remotes"]["Toggled"].append(name)
-        except StopIteration:
-            assert "Remotes" in self._modifications
-            assert "Add" in self._modifications["Remotes"]
-            remote = next(
-                item
-                for item in self._modifications["Remotes"]["Add"]
-                if item.name == name
+        added_remotes = self._modifications.get("Remotes", {}).get("Add", [])
+        remote_iterator = (
+            item for item in remotes + added_remotes if item.name == name
+        )
+        remote = next(remote_iterator, None)
+        assert remote is not None
+
+        if name in self._modifications.get("Remotes", {}).get("Toggled", []):
+            self._modifications["Remotes"]["Toggled"].remove(name)
+            if not self._modifications["Remotes"]["Toggled"]:
+                del self._modifications["Remotes"]["Toggled"]
+            if not self._modifications["Remotes"]:
+                del self._modifications["Remotes"]
+        else:
+            if "Remotes" not in self._modifications:
+                self._modifications["Remotes"] = {}
+            if "Toggled" not in self._modifications:
+                self._modifications["Remotes"]["Toggled"] = []
+            self._modifications["Remotes"]["Toggled"].append(name)
+
+        if remote in added_remotes:
+            self._modifications["Remotes"]["Add"].remove(remote)
+            self._modifications["Remotes"]["Add"].append(
+                dataclasses.replace(remote, enabled=state == QtCore.Qt.Checked)
             )
-            # this was simply to check that the modifications contained the remote
-            # toggled since the table holds the truth, not the modifications
+
+        # check that the remote was uniquely named
+        remote = next(remote_iterator, None)
+        assert remote is None
         self._modified.emit()
 
     def _hooks_item_changed(self, item: QtWidgets.QTableWidgetItem) -> None:
         if item.column() == ManageLocalCachesDialog._HooksTableColumnIndex.ENABLED:
             path_item = self._ui.hooksTable.item(
                 item.row(), ManageLocalCachesDialog._HooksTableColumnIndex.PATH
             )
@@ -591,19 +620,25 @@
             self,
             "Local cache deletion",
             f"Are you sure you want to delete the local cache {cache_name}?",
         )
         if result == QtWidgets.QMessageBox.StandardButton.No:
             return
         with NamedLocalCacheSettingsReader(cache_name) as settings:
-            home_dir = pathlib.Path(settings.home_dir.resolve())
-            short_home_dir = pathlib.Path(settings.short_home_dir.resolve())
+            home_dir_raw = settings.home_dir.resolve()
+            short_home_dir_raw = settings.short_home_dir.resolve()
 
-        assert home_dir  # because it's non-default
-        conan_home_dir = home_dir / ".conan"
+        assert home_dir_raw  # because it's non-default
+        home_dir = pathlib.Path(home_dir_raw)
+        short_home_dir = (
+            pathlib.Path(short_home_dir_raw) if short_home_dir_raw else None
+        )
+        conan_home_dir = home_dir
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            conan_home_dir /= ".conan"
         # since this is destructive, check again
         result = QtWidgets.QMessageBox.question(
             self,
             "Local cache deletion",
             f"Please confirm you want to delete the directories {conan_home_dir} and "
             f"{short_home_dir}?"
             if short_home_dir
@@ -620,14 +655,21 @@
         )
         self._ui.local_cache_names.setCurrentIndex(0)  # default
         self.cache_changed.emit(cache_name)
 
     def _operations_run_command(self) -> None:
         RunConanCommandDialog(self._context.cache_name, self).exec_()
 
+    def _profiles_create_default(self) -> None:
+        self._context.create_default_profile()
+        # reload all profiles into the UI
+        with NamedLocalCacheSettingsReader(self._context.cache_name) as settings:
+            extra_profile_dirs = settings.extra_profile_directories.resolve()
+        self._update_cache_profiles(extra_profile_dirs)
+
     def _profiles_add(self) -> None:
         dialog = AddExtraProfileDirectoryDialog(self)
         if dialog.exec_() == QtWidgets.QDialog.Accepted:
             extra = dialog.extra
             self._ui.profilesTable.add_key_value_pair(extra.name, extra.directory)
             if "Profiles" not in self._modifications:
                 self._modifications["Profiles"] = {}
```

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/__init__.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addenvironmentdialog.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addenvironmentdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addremotedialog.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addremotedialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/configpathorurl.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/configpathorurl.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/installconfigdialog.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/installconfigdialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from cruiz.pyside6.local_cache_install_config import Ui_InstallConfigDialog
 
 from cruiz.settings.managers.recentconanconfigs import (
     RecentConanConfigSettingsReader,
     RecentConanConfigSettings,
     RecentConanConfigSettingsWriter,
 )
-import cruiz.workers
+import cruiz.workers.api as workers_api
 
 
 class InstallConfigDialog(QtWidgets.QDialog):
     """
     Dialog for installing a new Conan config onto the local cache.
     """
 
@@ -55,15 +55,15 @@
         self._ui.pathOrUrl.setText(path)
 
     def _path_updated(self, path: str) -> None:
         self._ui.installButton.setEnabled(bool(path))
 
     def _install(self) -> None:
         self._ui.progressBar.setMaximum(0)
-        params = CommandParameters("install_config", cruiz.workers.configinstall.invoke)
+        params = CommandParameters("install_config", workers_api.configinstall.invoke)
         named_args = params.named_arguments
         named_args["pathOrUrl"] = self._ui.pathOrUrl.text().strip()
         if self._ui.gitBranch.text():
             named_args["gitBranch"] = self._ui.gitBranch.text().strip()
         if self._ui.sourceFolder.text():
             named_args["sourceFolder"] = self._ui.sourceFolder.text().strip()
         if self._ui.targetFolder.text():
```

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/keyvaluetable.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/keyvaluetable.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/movelocalcachedialog.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/movelocalcachedialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import pathlib
 import platform
 import shutil
 import typing
 
 from qtpy import QtCore, QtGui, QtWidgets
 
+import cruiz.globals
+
 from cruiz.commands.context import ConanContext
 
 from cruiz.settings.managers.namedlocalcache import (
     NamedLocalCacheSettings,
     NamedLocalCacheSettingsReader,
     NamedLocalCacheSettingsWriter,
 )
@@ -47,16 +49,21 @@
         self._ui.newUserHome.addAction(
             home_dir_browse_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         self._ui.newUserHome.textChanged.connect(self._new_path_changed)
         self._ui.newUserHomeShort.textChanged.connect(self._new_path_changed)
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Ok).setEnabled(False)
-        if platform.system() == "Windows":
-            pass
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            if platform.system() == "Windows":
+                pass
+            else:
+                self._ui.userHomeShortLabel.hide()
+                self._ui.currentUserHomeShort.hide()
+                self._ui.newUserHomeShort.hide()
         else:
             self._ui.userHomeShortLabel.hide()
             self._ui.currentUserHomeShort.hide()
             self._ui.newUserHomeShort.hide()
 
     def _home_dir_browse(self) -> None:
         dir_found = QtWidgets.QFileDialog.getExistingDirectory(
@@ -90,15 +97,15 @@
                 self,
                 "Conan local cache home directory",
                 f"The selected home directory '{new_home_dir}' is unchanged. "
                 "Please choose another.",
             )
             return
         qdir = QtCore.QDir(new_home_dir)
-        if qdir.exists():
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1 and qdir.exists():
             QtWidgets.QMessageBox.critical(
                 self,
                 "Conan local cache home directory",
                 f"The selected home directory '{new_home_dir}' already exists. "
                 "Please choose another.",
             )
             return
@@ -153,17 +160,20 @@
         assert old_home_dir  # since it's non-default
         # update settings
         settings.home_dir = new_home_dir  # type: ignore
         settings.short_home_dir = new_short_home_dir  # type: ignore
         NamedLocalCacheSettingsWriter(self._context.cache_name).sync(settings)
         # pylint: disable=broad-except
         try:
-            # move <old>/.conan to <new>/.conan
-            old_conan_dir = pathlib.Path(old_home_dir) / ".conan"
-            new_conan_dir = pathlib.Path(new_home_dir) / ".conan"
+            old_conan_dir = pathlib.Path(old_home_dir)
+            new_conan_dir = pathlib.Path(new_home_dir)
+            if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+                # move <old>/.conan to <new>/.conan
+                old_conan_dir /= ".conan"
+                new_conan_dir /= ".conan"
             shutil.move(str(old_conan_dir), str(new_conan_dir))
         except Exception as exception:
             QtWidgets.QMessageBox.critical(
                 self,
                 "Conan move local cache",
                 f"Failed to move the local cache home dir because: {exception}.",
             )
@@ -188,10 +198,11 @@
                     shutil.move(new_home_dir, str(old_conan_dir))
                     settings.home_dir = old_home_dir  # type: ignore
                     settings.short_home_dir = old_short_home_dir  # type: ignore
                     NamedLocalCacheSettingsWriter(self._context.cache_name).sync(
                         settings
                     )
                     return
-        qdir = QtCore.QDir(old_home_dir)
-        if qdir.isEmpty():
-            qdir.removeRecursively()
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            qdir = QtCore.QDir(old_home_dir)
+            if qdir.isEmpty():
+                qdir.removeRecursively()
```

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/newlocalcachewizard.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/newlocalcachewizard.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 """
 
 import platform
 import typing
 
 from qtpy import QtGui, QtWidgets
 
+import cruiz.globals
+
 from cruiz.commands.context import ConanContext
 from cruiz.interop.commandparameters import CommandParameters
 from cruiz.commands.logdetails import LogDetails
 from cruiz.settings.managers.localcachepreferences import LocalCacheSettingsReader
 from cruiz.settings.managers.namedlocalcache import NamedLocalCacheCreator
 from cruiz.widgets.util import search_for_dir_options
 from cruiz.constants import DEFAULT_CACHE_NAME
 
-import cruiz.workers
+import cruiz.workers.api as workers_api
 
 from cruiz.pyside6.local_cache_new_wizard import Ui_NewLocalCacheWizard
 
 
 class NewLocalCacheWizard(QtWidgets.QWizard):
     """
     Wizard for creating new local caches
@@ -58,17 +60,26 @@
         self._ui.configBranch.setText(new_config_branch or "<default branch>")
         self._ui.queryConfigInstall.setChecked(bool(new_config_url))
         self._ui.queryConfigInstall.setEnabled(bool(new_config_url))
         self._ui.createCache.clicked.connect(self._create_cache)
         self._ui.createProgress.setMinimum(0)
         self._ui.createProgress.setMaximum(1)
         self._ui.createProgress.setValue(0)
-        if platform.system() == "Windows":
-            pass
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            if platform.system() == "Windows":
+                pass
+            else:
+                self._ui.userHomeShortExplanation.hide()
+                self._ui.userHomeShortLabel.hide()
+                self._ui.userHomeShort.hide()
         else:
+            # Conan2 behaviour is different - there is no implicit .conan2 folder
+            self._ui.userHomeExplanation.setText(
+                "Each local cache resides entirely in the specified directory."
+            )
             self._ui.userHomeShortExplanation.hide()
             self._ui.userHomeShortLabel.hide()
             self._ui.userHomeShort.hide()
         self.currentIdChanged.connect(self._changed_page)
 
     def done(self, result: int) -> None:
         self._context.close()
@@ -133,15 +144,15 @@
         if self._ui.queryConfigInstall.isChecked():
             with LocalCacheSettingsReader() as settings:
                 config_install = settings.new_configuration_install.resolve()
                 git_branch = settings.new_configuration_git_branch.resolve()
             if config_install:
                 self._context.change_cache(name)
                 params = CommandParameters(
-                    "install_config", cruiz.workers.configinstall.invoke
+                    "install_config", workers_api.configinstall.invoke
                 )
                 named_args = params.named_arguments
                 named_args["pathOrUrl"] = config_install
                 if git_branch:
                     named_args["gitBranch"] = git_branch
                 self._context.install_config(
                     params, self._perform_new_cache_config_install_complete
```

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/progressdialogs.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/progressdialogs.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/remotestable.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/remotestable.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/runconancommanddialog.py` & `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/runconancommanddialog.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 Dialog for running a Conan command in a local cache.
 """
 
 import typing
 
 from qtpy import QtCore, QtWidgets
 
+import cruiz.globals
+
 from cruiz.commands.context import ConanContext, LogDetails
 from cruiz.interop.commandparameters import CommandParameters
 
 from cruiz.pyside6.local_cache_run_command_dialog import Ui_RunConanCommandDialog
 
-import cruiz.workers.arbitrary
+import cruiz.workers.api as workers_api
 
 
 class RunConanCommandDialog(QtWidgets.QDialog):
     """
     Dialog for adding an environment key-value pair to the local cache.
     """
 
@@ -37,21 +39,25 @@
         super().done(result)
 
     def _on_arguments_changed(self, text: str) -> None:
         self._ui.run.setEnabled(bool(text))
 
     def _on_run(self) -> None:
         args = self._ui.arguments.text().split()
-        params = CommandParameters(args[0], cruiz.workers.arbitrary.invoke)
+        params = CommandParameters(args[0], workers_api.arbitrary.invoke)
         params.arguments.extend(args[1:])
         self._ui.arguments.setEnabled(False)
         self._ui.run.setEnabled(False)
         self._context.run_any_command(params, self._on_run_complete)
 
     def _on_run_complete(self, payload: typing.Any, exception: typing.Any) -> None:
-        # payload is always None
         self._ui.arguments.setEnabled(True)
         self._ui.run.setEnabled(True)
-        if exception:
-            self._log_details.stderr("<font color='red'>Failed</font><br>")
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            # payload is always None
+            pass
         else:
-            self._log_details.stdout("<font color='green'>Succeeded</font><br>")
+            self._log_details.stdout(payload)
+            if exception:
+                self._log_details.stderr("<font color='red'>Failed</font><br>")
+            else:
+                self._log_details.stdout("<font color='green'>Succeeded</font><br>")
```

### Comparing `cruiz-1.4.0a1/cruiz/model/graphaslistmodel.py` & `cruiz-1.4.0a2/cruiz/model/graphaslistmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/recipe/dependencyview.py` & `cruiz-1.4.0a2/cruiz/recipe/dependencyview.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/recipe/expressioneditordialog.py` & `cruiz-1.4.0a2/cruiz/recipe/expressioneditordialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/recipe/findtextdialog.py` & `cruiz-1.4.0a2/cruiz/recipe/findtextdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/recipe/logs/command.py` & `cruiz-1.4.0a2/cruiz/recipe/logs/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,18 @@
 Recipe command log window
 """
 
 import pathlib
 import stat
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE6
+from qtpy import QtCore, QtGui, QtWidgets
 
 from cruiz.interop.commandparameters import CommandParameters
 
-if PYSIDE6:
-    QAction = QtGui.QAction
-else:
-    QAction = QtWidgets.QAction
-
 
 class CommandListWidgetItem(QtWidgets.QListWidgetItem):
     """
     QListWidgetItem representing a Conan command
     """
 
     def __init__(
```

### Comparing `cruiz-1.4.0a1/cruiz/recipe/recipe.py` & `cruiz-1.4.0a2/cruiz/recipe/recipe.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/recipe/recipewidget.py` & `cruiz-1.4.0a2/cruiz/recipe/recipewidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     RecipeSettingsReader,
     RecipeSettingsWriter,
 )
 from cruiz.settings.managers.namedlocalcache import NamedLocalCacheSettingsReader
 from cruiz.settings.managers.fontpreferences import FontSettingsReader, FontUsage
 from cruiz.widgets.util import BlockSignals, clear_widgets_from_layout
 from cruiz.revealonfilesystem import reveal_on_filesystem
-import cruiz.workers.lockcreate
+import cruiz.workers.api as workers_api
 from cruiz.model.graphaslistmodel import DependenciesListModel, DependenciesTreeModel
 from cruiz.manage_local_cache import ManageLocalCachesDialog
 import cruiz.revealonfilesystem
 import cruiz.globals
 from cruiz.exceptions import RecipeInspectionError
 
 from .recipe import Recipe
@@ -268,14 +268,17 @@
         )
         # tabify the docks on the right hand side
         self.tabifyDockWidget(
             self._ui.conanLocalWorkflowDock, self._ui.conanConfigureDock
         )
         # tabify the docks on the bottom side
         self.tabifyDockWidget(self._ui.conanLogDock, self._ui.conanCommandsDock)
+        if cruiz.globals.CONAN_MAJOR_VERSION > 1:
+            self._ui.conanLogDock.hide()
+            self._ui.conanLocalWorkflowDock.hide()
 
         # dependency dock
         self._ui.dependentsTabs.setTabVisible(1, False)  # tree disabled
         self._ui.dependentsLog.hide()
         self._ui.dependentsLog.customContextMenuRequested.connect(
             self._dependents_log_context_menu
         )
@@ -316,14 +319,17 @@
         self._ui.dependenciesPackageList.customContextMenuRequested.connect(
             self._dependency_list_context_menu
         )
         self._ui.behaviourToolbar.profile_changed.connect(
             self._generate_dependency_graph_from_profile_change
         )
 
+        if cruiz.globals.CONAN_MAJOR_VERSION > 1:
+            self._ui.buildFeaturesToolbar.hide()
+
         # associate with local caches
         self.log_details = LogDetails(
             self._ui.outputPane,
             self._ui.errorPane,
             self.combined_output_and_error_logs,
             use_batching,
             self._ui.conanLog,
@@ -380,15 +386,21 @@
         return self.recipe.context.inspect_recipe(
             self.recipe.path, propagate_errors=True
         )
 
     def _get_options_from_recipe(
         self, attrs: typing.Dict[str, str]
     ) -> typing.List[typing.Tuple[str, typing.List[typing.Any], typing.Any]]:
-        options = attrs.get("options")
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            # this lists the possible values for the option
+            options = attrs.get("options")
+        else:
+            # don't use the 'options' key, as that has been assigned the value
+            # options_definitions is where the possible values are
+            options = attrs.get("options_definitions")
         if not options:
             return []
         default_options = attrs["default_options"]
         if isinstance(default_options, (tuple, list)):
             as_dict = {}
             for entry in default_options:
                 key, value = entry.split("=")
@@ -397,15 +409,22 @@
         assert isinstance(
             default_options, dict
         ), "Expected default_options to be a dict"
         values: typing.List[typing.Tuple[str, typing.List[typing.Any], typing.Any]] = []
         assert isinstance(options, dict)
         for key, value in options.items():
             if default_options:
-                default_value = default_options[key]
+                if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+                    default_value = default_options[key]
+                else:
+                    # when the recipe is serialised,
+                    # default_options come through as typed (e.g. bool)
+                    # while option_definitions are all strings, so in order to compare
+                    # let's do everything as strings
+                    default_value = str(default_options[key])
                 if isinstance(value, list) and default_value not in value:
                     if isinstance(value[0], bool):
                         default_value = _strtobool(default_value)
                         assert default_value in value, (
                             f"Cannot find default value '{default_value}' in possible "
                             f"values {value}"
                         )
@@ -1036,15 +1055,15 @@
     ) -> None:
         # reset views
         self._ui.configurePackageId.setText("Calculating...")
         # https://stackoverflow.com/questions/46630185/qt-remove-model-from-view
         self._ui.dependenciesPackageList.setModel(None)  # type: ignore[arg-type]
         self._ui.dependencyView.clear()
         # calculate lock file
-        params = CommandParameters("lock create", cruiz.workers.lockcreate.invoke)
+        params = CommandParameters("lock create", workers_api.lockcreate.invoke)
         params.recipe_path = self.recipe.path
         params.name = recipe_attributes.get("name")
         params.version = self.recipe.version
         params.user = self.recipe.user
         params.channel = self.recipe.channel
         with RecipeSettingsReader.from_recipe(self.recipe) as settings:
             params.profile = settings.profile.resolve()
```

### Comparing `cruiz-1.4.0a1/cruiz/recipe/toolbars/behaviour.py` & `cruiz-1.4.0a2/cruiz/recipe/toolbars/behaviour.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 """
 
 import os
 import pathlib
 
 from qtpy import QtCore, QtWidgets
 
+import cruiz.globals
+
 from cruiz.pyside6.recipe_profile_frame import Ui_profileFrame
 from cruiz.pyside6.recipe_cpucores_frame import Ui_cpuCoresFrame
 
 from cruiz.widgets.util import BlockSignals
 
 from cruiz.settings.managers.recipe import (
     RecipeSettings,
@@ -43,21 +45,26 @@
         with NamedLocalCacheSettingsReader(cache_name) as settings:
             home_dir = settings.home_dir.resolve()
         # using normcase for Windows path compares
         home_dir = os.path.normcase(home_dir) if home_dir else str(pathlib.Path.home())
         profile_dirs = "\n  ".join(
             [str(os.path.normcase(p)) for p in self._recipe.context.all_profile_dirs()]
         )
-        parameterised_profile_dirs = profile_dirs.replace(home_dir, "<CONAN_USER_HOME>")
+        local_cache_envvar = (
+            "<CONAN_USER_HOME>"
+            if cruiz.globals.CONAN_MAJOR_VERSION == 1
+            else "<CONAN_HOME>"
+        )
+        parameterised_profile_dirs = profile_dirs.replace(home_dir, local_cache_envvar)
         tooltip = (
             "Profiles listed here are from the following directories:\n\n"
             f"{profile_dirs}\n\n"
             "which can be read as this parameterisation\n\n"
             f"{parameterised_profile_dirs}\n\n"
-            "where <CONAN_USER_HOME> is the base directory "
+            f"where {local_cache_envvar} is the base directory "
             "for this recipe's associated local cache, called "
             f"'{cache_name}'"
         )
         self._ui.profileCombo.setToolTip(tooltip)
         self._ui.profileLabel.setToolTip(tooltip)
 
     def refresh_content(self, recipe: Recipe) -> None:
@@ -72,25 +79,28 @@
             for profile_path, _ in profile_list:
                 blocked_widget.addItem(str(profile_path))
 
             index = blocked_widget.findText(current_profile)
             if index >= 0:
                 blocked_widget.setCurrentIndex(index)
             else:
-                # this means that the profile in settings cannot be found in the
-                # local cache profiles
-                blocked_widget.setCurrentIndex(0)
-                # sync this choice back to the settings
-                updated_profile_settings = RecipeSettings()
-                updated_profile_settings.profile = str(
-                    profile_list[0][0]
-                )  # type: ignore
-                RecipeSettingsWriter().from_recipe(recipe).sync(
-                    updated_profile_settings
-                )
+                if profile_list:
+                    # this means that the profile in settings cannot be found in the
+                    # local cache profiles
+                    blocked_widget.setCurrentIndex(0)
+                    # sync that the first profile in the list is now current
+                    updated_profile_settings = RecipeSettings()
+                    updated_profile_settings.profile = str(
+                        profile_list[0][0]
+                    )  # type: ignore
+                    RecipeSettingsWriter().from_recipe(recipe).sync(
+                        updated_profile_settings
+                    )
+                else:
+                    blocked_widget.setCurrentIndex(-1)
         self._refresh_tooltip()
 
     def _changed_profile(self, text: str) -> None:
         recipe = self._recipe
         settings = RecipeSettings.from_recipe(recipe)
         settings.profile = text  # type: ignore
         # note: has to be from recipe, as the profile setter needs
@@ -135,32 +145,35 @@
         RecipeSettingsWriter.from_recipe(recipe).sync(settings)
         self.refresh_content(recipe)
 
 
 class RecipeBehaviourToolbar(QtWidgets.QToolBar):
     """
     QToolBar representing tne behaviour of a recipe, profile and cpu cores
+    CPU cores not available in Conan 2 at this time
     """
 
     profile_changed = QtCore.Signal(str)
 
     def __init__(self, parent: QtWidgets.QWidget) -> None:
         super().__init__(parent)
         self._profile = _ProfileFrame(self)
-        self._cpu_cores = _CPUCoresFrame(self)
         self.addWidget(self._profile)
-        self.addSeparator()
-        self.addWidget(self._cpu_cores)
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            self._cpu_cores = _CPUCoresFrame(self)
+            self.addSeparator()
+            self.addWidget(self._cpu_cores)
 
     @property
     def _recipe(self) -> Recipe:
         recipe_widget = self.parent()
         recipe = recipe_widget.recipe
         return recipe
 
     def refresh_content(self) -> None:
         """
         Refresh the content of the toolbar.
         """
         recipe = self._recipe
         self._profile.refresh_content(recipe)
-        self._cpu_cores.refresh_content(recipe)
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            self._cpu_cores.refresh_content(recipe)
```

### Comparing `cruiz-1.4.0a1/cruiz/recipe/toolbars/buildfeatures.py` & `cruiz-1.4.0a2/cruiz/recipe/toolbars/buildfeatures.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/recipe/toolbars/command.py` & `cruiz-1.4.0a2/cruiz/recipe/toolbars/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,36 +4,35 @@
 Recipe command toolbar
 """
 
 from io import StringIO
 import os
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE6
+from qtpy import QtCore, QtGui, QtWidgets
+
+import cruiz.globals
+
 from cruiz.settings.managers.generalpreferences import GeneralSettingsReader
 
 from cruiz.settings.managers.recipe import RecipeSettings, RecipeSettingsReader
 from cruiz.settings.managers.shortcuts import ShortcutSettingsReader
 from cruiz.settings.managers.compilercachepreferences import CompilerCacheSettingsReader
 
-import cruiz.workers.install
+import cruiz.workers.api as workers_api
 
 from cruiz.interop.commandparameters import CommandParameters
 
 from cruiz.constants import BuildFeatureConstants, CompilerCacheTypes
 from cruiz.environ import EnvironSaver
 
 from cruiz.exceptions import RecipeInspectionError
 
-if PYSIDE6:
-    QAction = QtGui.QAction
-    QActionGroup = QtGui.QActionGroup
-else:
-    QAction = QtWidgets.QAction
-    QActionGroup = QtWidgets.QActionGroup
+
+IS_CONAN_V1 = cruiz.globals.CONAN_MAJOR_VERSION == 1
 
 
 class RecipeCommandToolbar(QtWidgets.QToolBar):
     """
     QToolBar representing the recipe commands
     """
 
@@ -41,50 +40,61 @@
     command_ended = QtCore.Signal()
 
     def __init__(self, parent: QtWidgets.QWidget) -> None:
         super().__init__(parent)
         recipe_ui = parent._ui
         self.command_started.connect(self._command_started)
         self.command_ended.connect(self._command_ended)
-        self._idle_group = QActionGroup(self)
+        self._idle_group = QtGui.QActionGroup(self)
         self._idle_group.setEnabled(True)
-        self._cancel_command_group = QActionGroup(self)
+        self._cancel_command_group = QtGui.QActionGroup(self)
         self._cancel_command_group.setEnabled(False)
         self._add_toolbutton(
             [recipe_ui.actionCreateCommand, recipe_ui.actionCreateUpdateCommand]
         )
         self.addSeparator()
         self._add_toolbutton(
             [recipe_ui.actionInstallCommand, recipe_ui.actionInstallUpdateCommand]
         )
-        self._add_toolbutton([recipe_ui.actionImportsCommand])
+        if IS_CONAN_V1:
+            self._add_toolbutton([recipe_ui.actionImportsCommand])
+        else:
+            recipe_ui.actionImportsCommand.setVisible(False)
         self._add_toolbutton([recipe_ui.actionSourceCommand])
         self._add_toolbutton([recipe_ui.actionBuildCommand])
-        self._add_toolbutton([recipe_ui.actionPackageCommand])
+        if IS_CONAN_V1:
+            self._add_toolbutton([recipe_ui.actionPackageCommand])
+        else:
+            recipe_ui.actionPackageCommand.setVisible(False)
         self._add_toolbutton([recipe_ui.actionExportPackageCommand])
         self._add_toolbutton([recipe_ui.actionTestCommand])
         self.addSeparator()
         self._add_toolbutton([recipe_ui.actionCancelCommand], for_cancel_group=True)
         self.addSeparator()
         self._add_toolbutton([recipe_ui.actionRemovePackageCommand])
         self.addSeparator()
-        self._add_toolbutton(
-            [
-                recipe_ui.actionCMakeBuildToolCommand,
-                recipe_ui.actionCMakeBuildToolVerboseCommand,
-                recipe_ui.actionCMakeRemoveCacheCommand,
-            ]
-        )
+        if IS_CONAN_V1:
+            self._add_toolbutton(
+                [
+                    recipe_ui.actionCMakeBuildToolCommand,
+                    recipe_ui.actionCMakeBuildToolVerboseCommand,
+                    recipe_ui.actionCMakeRemoveCacheCommand,
+                ]
+            )
+        else:
+            recipe_ui.actionCMakeBuildToolCommand.setEnabled(False)
+            recipe_ui.actionCMakeBuildToolVerboseCommand.setEnabled(False)
+            recipe_ui.actionCMakeRemoveCacheCommand.setEnabled(False)
 
     @property
     def _recipe_widget(self) -> QtCore.QObject:
         return self.parent()
 
     def _add_toolbutton(
-        self, actions: typing.List[QAction], for_cancel_group: bool = False
+        self, actions: typing.List[QtGui.QAction], for_cancel_group: bool = False
     ) -> None:
         assert actions
         button = QtWidgets.QToolButton()
         button.addActions(actions)
         button.setDefaultAction(actions[0])
         self.addWidget(button)
         if for_cancel_group:
@@ -96,40 +106,45 @@
 
     def configure_actions(self) -> None:
         """
         Configure the QActions in the toolbar
         """
 
         def _configure(
-            action: QAction, trigger_slot: typing.Callable[[], None]
+            action: QtGui.QAction, trigger_slot: typing.Callable[[], None]
         ) -> None:
             action.setShortcutVisibleInContextMenu(True)
             action.setShortcutContext(QtCore.Qt.WindowShortcut)
             action.triggered.connect(trigger_slot)
 
         # shortcuts themselves are set elsewhere, as they can be dynamic
         # through the lifetime of the application
         recipe_ui = self.parent()._ui
         _configure(recipe_ui.actionCreateCommand, self._conan_create)
         _configure(recipe_ui.actionCreateUpdateCommand, self._conan_create_update)
         _configure(recipe_ui.actionInstallCommand, self._conan_install)
         _configure(recipe_ui.actionInstallUpdateCommand, self._conan_install_update)
-        _configure(recipe_ui.actionImportsCommand, self._conan_imports)
+        if IS_CONAN_V1:
+            _configure(recipe_ui.actionImportsCommand, self._conan_imports)
         _configure(recipe_ui.actionSourceCommand, self._conan_source)
         _configure(recipe_ui.actionBuildCommand, self._conan_build)
-        _configure(recipe_ui.actionPackageCommand, self._conan_package)
+        if IS_CONAN_V1:
+            _configure(recipe_ui.actionPackageCommand, self._conan_package)
         _configure(recipe_ui.actionExportPackageCommand, self._conan_export_package)
         _configure(recipe_ui.actionTestCommand, self._conan_test)
-        _configure(recipe_ui.actionRemovePackageCommand, self._conan_remove)
         _configure(recipe_ui.actionCancelCommand, self._cancel_command)
-        _configure(recipe_ui.actionCMakeBuildToolCommand, self._cmake_build)
-        _configure(
-            recipe_ui.actionCMakeBuildToolVerboseCommand, self._cmake_build_verbose
-        )
-        _configure(recipe_ui.actionCMakeRemoveCacheCommand, self._cmake_remove_cache)
+        _configure(recipe_ui.actionRemovePackageCommand, self._conan_remove)
+        if IS_CONAN_V1:
+            _configure(recipe_ui.actionCMakeBuildToolCommand, self._cmake_build)
+            _configure(
+                recipe_ui.actionCMakeBuildToolVerboseCommand, self._cmake_build_verbose
+            )
+            _configure(
+                recipe_ui.actionCMakeRemoveCacheCommand, self._cmake_remove_cache
+            )
 
     def disable_all_actions(self) -> None:
         """
         Disable everything in the case of recipe loading errors
         """
         self._idle_group.setEnabled(False)
         self._cancel_command_group.setEnabled(False)
@@ -139,30 +154,33 @@
     ) -> None:
         """
         Refresh all command action shortcuts and tooltips
         """
         with ShortcutSettingsReader() as settings:
             conan_create = settings.conan_create.resolve()
             conan_create_updates = settings.conan_create_updates.resolve()
-            conan_imports = settings.conan_imports.resolve()
             conan_install = settings.conan_install.resolve()
             conan_install_updates = settings.conan_install_updates.resolve()
+            if IS_CONAN_V1:
+                conan_imports = settings.conan_imports.resolve()
             conan_source = settings.conan_source.resolve()
             conan_build = settings.conan_build.resolve()
-            conan_package = settings.conan_package.resolve()
+            if IS_CONAN_V1:
+                conan_package = settings.conan_package.resolve()
             conan_exportpkg = settings.conan_export_package.resolve()
             conan_test = settings.conan_test_package.resolve()
-            conan_remove = settings.conan_remove_package.resolve()
             cancel = settings.cancel.resolve()
-            cmake_build_tool = settings.cmake_build_tool.resolve()
-            cmake_build_tool_verbose = settings.cmake_build_tool_verbose.resolve()
-            remove_cmakecache = settings.delete_cmake_cache.resolve()
+            conan_remove = settings.conan_remove_package.resolve()
+            if IS_CONAN_V1:
+                cmake_build_tool = settings.cmake_build_tool.resolve()
+                cmake_build_tool_verbose = settings.cmake_build_tool_verbose.resolve()
+                remove_cmakecache = settings.delete_cmake_cache.resolve()
 
         def _configure(
-            action: QAction, shortcut: str, params: CommandParameters
+            action: QtGui.QAction, shortcut: str, params: CommandParameters
         ) -> None:
             action.setShortcut(QtGui.QKeySequence(shortcut))
             action.setToolTip(self._generate_command_tooltip(params))
 
         recipe_ui = self.parent()._ui
         _configure(
             recipe_ui.actionCreateCommand,
@@ -180,63 +198,68 @@
             self._make_conan_install_params(recipe_attributes, None),
         )
         _configure(
             recipe_ui.actionInstallUpdateCommand,
             conan_install_updates,
             self._make_conan_install_params(recipe_attributes, ["-u"]),
         )
-        _configure(
-            recipe_ui.actionImportsCommand,
-            conan_imports,
-            self._make_conan_imports_params(recipe_attributes),
-        )
+        if IS_CONAN_V1:
+            _configure(
+                recipe_ui.actionImportsCommand,
+                conan_imports,
+                self._make_conan_imports_params(recipe_attributes),
+            )
         _configure(
             recipe_ui.actionSourceCommand,
             conan_source,
             self._make_conan_source_params(recipe_attributes),
         )
         _configure(
             recipe_ui.actionBuildCommand,
             conan_build,
             self._make_conan_build_params(recipe_attributes),
         )
-        _configure(
-            recipe_ui.actionPackageCommand,
-            conan_package,
-            self._make_conan_package_params(recipe_attributes),
-        )
+        if IS_CONAN_V1:
+            _configure(
+                recipe_ui.actionPackageCommand,
+                conan_package,
+                self._make_conan_package_params(recipe_attributes),
+            )
         _configure(
             recipe_ui.actionExportPackageCommand,
             conan_exportpkg,
             self._make_conan_export_package_params(recipe_attributes),
         )
         _configure(
             recipe_ui.actionTestCommand,
             conan_test,
             self._make_conan_test_package_params(recipe_attributes),
         )
+        recipe_ui.actionCancelCommand.setShortcut(QtGui.QKeySequence(cancel))
+        recipe_ui.actionCancelCommand.setToolTip("Cancel the currently running command")
         _configure(
             recipe_ui.actionRemovePackageCommand,
             conan_remove,
             self._make_conan_remove_package_params(recipe_attributes),
         )
-        recipe_ui.actionCancelCommand.setShortcut(QtGui.QKeySequence(cancel))
-        recipe_ui.actionCancelCommand.setToolTip("Cancel the currently running command")
-        recipe_ui.actionCMakeBuildToolCommand.setShortcut(
-            QtGui.QKeySequence(cmake_build_tool)
-        )
-        recipe_ui.actionCMakeBuildToolCommand.setToolTip("CMake build")
-        recipe_ui.actionCMakeBuildToolVerboseCommand.setShortcut(
-            QtGui.QKeySequence(cmake_build_tool_verbose)
-        )
-        recipe_ui.actionCMakeBuildToolVerboseCommand.setToolTip("CMake verbose build")
-        recipe_ui.actionCMakeRemoveCacheCommand.setShortcut(
-            QtGui.QKeySequence(remove_cmakecache)
-        )
-        recipe_ui.actionCMakeRemoveCacheCommand.setToolTip("Remove CMake cache")
+        if IS_CONAN_V1:
+            recipe_ui.actionCMakeBuildToolCommand.setShortcut(
+                QtGui.QKeySequence(cmake_build_tool)
+            )
+            recipe_ui.actionCMakeBuildToolCommand.setToolTip("CMake build")
+            recipe_ui.actionCMakeBuildToolVerboseCommand.setShortcut(
+                QtGui.QKeySequence(cmake_build_tool_verbose)
+            )
+            recipe_ui.actionCMakeBuildToolVerboseCommand.setToolTip(
+                "CMake verbose build"
+            )
+            recipe_ui.actionCMakeRemoveCacheCommand.setShortcut(
+                QtGui.QKeySequence(remove_cmakecache)
+            )
+            recipe_ui.actionCMakeRemoveCacheCommand.setToolTip("Remove CMake cache")
 
     def _command_started(self) -> None:
         self._idle_group.setEnabled(False)
         self._cancel_command_group.setEnabled(True)
 
     def _command_ended(self) -> None:
         self._idle_group.setEnabled(True)
@@ -327,19 +350,21 @@
         with_profile: bool = False,
         with_install_folder: bool = False,
         with_imports_folder: bool = False,
         with_source_folder: bool = False,
         fudge_source_folder: bool = False,
         with_build_folder: bool = False,
         with_package_folder: bool = False,
-        with_test_folder: bool = False,
+        with_test_build_folder: bool = False,
         with_explicit_name: bool = False,
         with_force: bool = False,
         with_exclusive_package_folder: bool = False,
         with_options: bool = False,
+        v2_omit_test_folder: bool = False,
+        v2_need_reference: bool = False,
     ) -> CommandParameters:
         recipe_widget = self._recipe_widget
         recipe = recipe_widget.recipe
         params = CommandParameters(verb, worker)
         if with_recipe_path:
             params.recipe_path = recipe.path
         if with_explicit_name:
@@ -347,21 +372,24 @@
         if with_pkgref:
             params.version = recipe.version or recipe_attributes["version"]
             params.user = recipe.user
             params.channel = recipe.channel
             params.make_package_reference()  # only needed for the exported string
         if with_force:
             params.force = True
+        if cruiz.globals.CONAN_MAJOR_VERSION > 1:
+            params.v2_need_reference = v2_need_reference
         self._append_general_prefs(params)
         with RecipeSettingsReader.from_recipe(recipe) as settings:
-            num_cores = settings.num_cpu_cores
-            if num_cores.value is not None:
-                params.added_environment.update(
-                    {"CONAN_CPU_COUNT": str(num_cores.value)}
-                )
+            if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+                num_cores = settings.num_cpu_cores
+                if num_cores.value is not None:
+                    params.added_environment.update(
+                        {"CONAN_CPU_COUNT": str(num_cores.value)}
+                    )
             if with_options:
                 for key, value in settings.options.resolve().items():
                     assert recipe_attributes["name"]
                     params.add_option(
                         recipe_attributes["name"], key, value
                     )  # TODO: is this the most efficient algorithm?
             self._append_build_features(params, settings)
@@ -404,27 +432,31 @@
                 params.source_folder = recipe_widget.resolve_expression(source_folder)
             if with_build_folder:
                 build_folder = settings.local_workflow_build_folder.resolve()
                 params.build_folder = recipe_widget.resolve_expression(build_folder)
             if with_package_folder:
                 package_folder = settings.local_workflow_package_folder.resolve()
                 params.package_folder = recipe_widget.resolve_expression(package_folder)
-            if with_test_folder:
+            if with_test_build_folder:
                 test_folder = settings.local_workflow_test_folder.resolve()
-                params.test_folder = recipe_widget.resolve_expression(test_folder)
+                params.test_build_folder = recipe_widget.resolve_expression(test_folder)
+            if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+                pass
+            else:
+                params.v2_omit_test_folder = v2_omit_test_folder
         return params
 
     def _make_conan_create_params(
         self,
         recipe_attributes: typing.Dict[str, typing.Optional[str]],
         args: typing.Optional[typing.List[str]],
     ) -> CommandParameters:
         params = self._make_common_params(
             "create",
-            cruiz.workers.create.invoke,
+            workers_api.create.invoke,
             recipe_attributes,
             with_pkgref=True,
             with_profile=True,
             with_options=True,
         )
         if args:
             params.arguments.extend(args)
@@ -433,15 +465,15 @@
     def _make_conan_install_params(
         self,
         recipe_attributes: typing.Dict[str, typing.Optional[str]],
         args: typing.Optional[typing.List[str]],
     ) -> CommandParameters:
         params = self._make_common_params(
             "install",
-            cruiz.workers.install.invoke,
+            workers_api.install.invoke,
             recipe_attributes,
             with_pkgref=True,
             with_cwd=True,
             with_profile=True,
             with_install_folder=True,
             with_options=True,
         )
@@ -450,114 +482,143 @@
         return params
 
     def _make_conan_imports_params(
         self, recipe_attributes: typing.Dict[str, typing.Optional[str]]
     ) -> CommandParameters:
         return self._make_common_params(
             "imports",
-            cruiz.workers.imports.invoke,
+            workers_api.imports.invoke,
             recipe_attributes,
             with_cwd=True,
             with_install_folder=True,
             with_imports_folder=True,
         )
 
     def _make_conan_source_params(
         self, recipe_attributes: typing.Dict[str, typing.Optional[str]]
     ) -> CommandParameters:
+        named_args = {}
+        if IS_CONAN_V1:
+            pass
+        else:
+            named_args["with_pkgref"] = True
         return self._make_common_params(
             "source",
-            cruiz.workers.source.invoke,
+            workers_api.source.invoke,
             recipe_attributes,
             with_cwd=True,
             with_install_folder=True,
             with_source_folder=True,
+            **named_args,
         )
 
     def _make_conan_build_params(
         self, recipe_attributes: typing.Dict[str, typing.Optional[str]]
     ) -> CommandParameters:
+        named_args = {}
+        if IS_CONAN_V1:
+            pass
+        else:
+            named_args["with_pkgref"] = True
         return self._make_common_params(
             "build",
-            cruiz.workers.build.invoke,
+            workers_api.build.invoke,
             recipe_attributes,
             with_cwd=True,
             with_install_folder=True,
             with_source_folder=True,
             fudge_source_folder=True,
             with_build_folder=True,
             with_package_folder=True,
+            **named_args,
         )
 
     def _make_conan_package_params(
         self, recipe_attributes: typing.Dict[str, typing.Optional[str]]
     ) -> CommandParameters:
         return self._make_common_params(
             "package",
-            cruiz.workers.package.invoke,
+            workers_api.package.invoke,
             recipe_attributes,
             with_cwd=True,
             with_install_folder=True,
             with_source_folder=True,
             fudge_source_folder=True,
             with_build_folder=True,
             with_package_folder=True,
         )
 
     def _make_conan_export_package_params(
         self, recipe_attributes: typing.Dict[str, typing.Optional[str]]
     ) -> CommandParameters:
+        named_args = {}
+        if IS_CONAN_V1:
+            named_args["with_force"] = True
+        else:
+            named_args["v2_omit_test_folder"] = True
         return self._make_common_params(
             "export-pkg",
-            cruiz.workers.exportpackage.invoke,
+            workers_api.exportpackage.invoke,
             recipe_attributes,
             with_cwd=True,
             with_pkgref=True,
             with_install_folder=True,
             with_source_folder=True,
             fudge_source_folder=True,
             with_build_folder=True,
             with_package_folder=True,
             with_exclusive_package_folder=True,
             with_explicit_name=True,
-            with_force=True,
             with_options=True,
+            **named_args,
         )
 
     def _make_conan_test_package_params(
         self, recipe_attributes: typing.Dict[str, typing.Optional[str]]
     ) -> CommandParameters:
+        named_args = {}
+        if IS_CONAN_V1:
+            pass
+        else:
+            named_args["v2_need_reference"] = True
         params = self._make_common_params(
             "test",
-            cruiz.workers.testpackage.invoke,
+            workers_api.testpackage.invoke,
             recipe_attributes,
             with_recipe_path=False,
             with_cwd=True,
             with_profile=True,
-            with_test_folder=True,
+            with_test_build_folder=True,
             with_explicit_name=True,
             with_pkgref=True,
             with_options=True,
+            **named_args,
         )
         recipe_widget = self._recipe_widget
         recipe = recipe_widget.recipe
         params.recipe_path = recipe.path.parent / "test_package"
         return params
 
     def _make_conan_remove_package_params(
         self, recipe_attributes: typing.Dict[str, typing.Optional[str]]
     ) -> CommandParameters:
+        named_args = {}
+        if IS_CONAN_V1:
+            pass
+        else:
+            named_args["v2_need_reference"] = True
         return self._make_common_params(
             "remove",
-            cruiz.workers.removepackage.invoke,
+            workers_api.removepackage.invoke,
             recipe_attributes,
             with_explicit_name=True,
             with_pkgref=True,
             with_force=True,
             with_recipe_path=False,
+            **named_args,
         )
 
     def _conan_create_common(
         self, args: typing.Optional[typing.List[str]] = None
     ) -> None:
         # note that this is done early, to force a focus change in any
         # configuration windows, forcing serialising changes before commands kick off
@@ -690,15 +751,15 @@
     def _cmake_build_common(
         self, args: typing.Optional[typing.List[str]] = None
     ) -> None:
         # TODO review
         recipe_widget = self._recipe_widget
         recipe = recipe_widget.recipe
         params = CommandParameters(
-            "cmakebuild", cruiz.workers.cmakebuildtool.invoke
+            "cmakebuild", workers_api.cmakebuildtool.invoke
         )  # TODO: verb is wrong
         with RecipeSettingsReader.from_recipe(recipe) as settings:
             num_cores = settings.num_cpu_cores
             if num_cores.value is not None:
                 params.added_environment.update(
                     {"CONAN_CPU_COUNT": str(num_cores.value)}
                 )
@@ -725,15 +786,15 @@
         self._cmake_build_common(args=["verbose"])
 
     def _cmake_remove_cache(self) -> None:
         # TODO: review
         recipe_widget = self._recipe_widget
         recipe = recipe_widget.recipe
         params = CommandParameters(
-            "cmakeremovecache", cruiz.workers.deletecmakecache.invoke
+            "cmakeremovecache", workers_api.deletecmakecache.invoke
         )  # TODO: verb is wrong
         with RecipeSettingsReader.from_recipe(recipe) as settings:
             workflow_cwd = settings.local_workflow_cwd.resolve()
             common_subdir = settings.local_workflow_common_subdir.resolve()
             params.cwd = recipe_widget.get_working_dir(workflow_cwd, common_subdir)
             layout_build_subdir = (
                 recipe_widget._dependency_graph.root.layout_build_subdir
```

### Comparing `cruiz-1.4.0a1/cruiz/remote_browser/pages/packagebinarypage.py` & `cruiz-1.4.0a2/cruiz/remote_browser/pages/packagebinarypage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/remote_browser/pages/packageidpage.py` & `cruiz-1.4.0a2/cruiz/remote_browser/pages/packageidpage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/remote_browser/pages/packagereferencepage.py` & `cruiz-1.4.0a2/cruiz/remote_browser/pages/packagereferencepage.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 Remote browser page
 """
 
 import typing
 
 from qtpy import QtCore, QtGui
 
+import cruiz.globals
+
 from cruiz.commands.context import ConanConfigBoolean
 
 from cruiz.interop.searchrecipesparameters import SearchRecipesParameters
 
 from cruiz.settings.managers.namedlocalcache import AllNamedLocalCacheSettingsReader
 
 from cruiz.widgets.util import BlockSignals
@@ -98,15 +100,17 @@
         self._ui.search_pattern.inputRejected.connect(self._pattern_incorrect)
         self._ui.search_pattern.returnPressed.connect(self._search)
 
         self._ui.package_references.doubleClicked.connect(self._on_pkgref_dclicked)
 
         self._ui.pkgref_cancel.clicked.connect(self.on_cancel)
 
+    def showEvent(self, event: QtGui.QShowEvent) -> None:
         self.refresh_local_cache_names()
+        super().showEvent(event)
 
     def refresh_local_cache_names(self) -> None:
         """
         Refresh the UI for current local cache names.
         """
         with BlockSignals(self._ui.local_cache_name) as blocked_widget:
             blocked_widget.clear()
@@ -131,18 +135,22 @@
         self._context.change_cache(text)
         with BlockSignals(self._ui.remote) as blocked_widget:
             blocked_widget.clear()
             for remote in self._context.get_remotes_list():
                 blocked_widget.addItem(remote.name)
             blocked_widget.setCurrentIndex(-1)
         self._ui.remote.setCurrentIndex(0)
-        self._revs_enabled = self._context.get_boolean_config(
-            ConanConfigBoolean.REVISIONS, False
-        )
-        self._ui.revisions.setChecked(self._revs_enabled)
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            self._revs_enabled = self._context.get_boolean_config(
+                ConanConfigBoolean.REVISIONS, False
+            )
+            self._ui.revisions.setChecked(self._revs_enabled)
+        else:
+            self._revs_enabled = True
+            self._ui.revisions.hide()
 
     def _on_remote_change(self, text: str) -> None:
         # pylint: disable=unused-argument
         self._model.clear()
 
     def _pattern_incorrect(self) -> None:
         with BlockSignals(self._ui.search_pattern) as blocked_widget:
```

### Comparing `cruiz-1.4.0a1/cruiz/remote_browser/pages/packagerevisionpage.py` & `cruiz-1.4.0a2/cruiz/remote_browser/pages/packagerevisionpage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/remote_browser/pages/page.py` & `cruiz-1.4.0a2/cruiz/remote_browser/pages/page.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/remote_browser/pages/reciperevisionpage.py` & `cruiz-1.4.0a2/cruiz/remote_browser/pages/reciperevisionpage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/remote_browser/remotebrowser.py` & `cruiz-1.4.0a2/cruiz/remote_browser/remotebrowser.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resourcegeneration.py` & `cruiz-1.4.0a2/cruiz/resourcegeneration.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/001-rubbish.svg` & `cruiz-1.4.0a2/cruiz/resources/001-rubbish.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/002-null.svg` & `cruiz-1.4.0a2/cruiz/resources/002-null.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/003-chemistry.svg` & `cruiz-1.4.0a2/cruiz/resources/003-chemistry.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/004-share.svg` & `cruiz-1.4.0a2/cruiz/resources/004-share.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/005-box.svg` & `cruiz-1.4.0a2/cruiz/resources/005-box.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/006-toolbox.svg` & `cruiz-1.4.0a2/cruiz/resources/006-toolbox.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/007-book.svg` & `cruiz-1.4.0a2/cruiz/resources/007-book.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/008-cloud-computing.svg` & `cruiz-1.4.0a2/cruiz/resources/008-cloud-computing.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/009-import.svg` & `cruiz-1.4.0a2/cruiz/resources/009-import.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/010-draw.svg` & `cruiz-1.4.0a2/cruiz/resources/010-draw.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/012-hammer.svg` & `cruiz-1.4.0a2/cruiz/resources/012-hammer.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/013-pencil.svg` & `cruiz-1.4.0a2/cruiz/resources/013-pencil.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/014-code.svg` & `cruiz-1.4.0a2/cruiz/resources/014-code.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/Cmake.svg` & `cruiz-1.4.0a2/cruiz/resources/Cmake.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/about_dialog.ui` & `cruiz-1.4.0a2/cruiz/resources/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/cruise.png` & `cruiz-1.4.0a2/cruiz/resources/cruise.png`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/cruizres.qrc` & `cruiz-1.4.0a2/cruiz/resources/cruizres.qrc`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/find_text_dialog.ui` & `cruiz-1.4.0a2/cruiz/resources/find_text_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/license-cruise.pdf` & `cruiz-1.4.0a2/cruiz/resources/license-cruise.pdf`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/license.pdf` & `cruiz-1.4.0a2/cruiz/resources/license.pdf`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/load_recipe_wizard.ui` & `cruiz-1.4.0a2/cruiz/resources/load_recipe_wizard.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/local_cache_add_environment.ui` & `cruiz-1.4.0a2/cruiz/resources/local_cache_add_environment.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/local_cache_add_profile_directory.ui` & `cruiz-1.4.0a2/cruiz/resources/local_cache_add_profile_directory.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/local_cache_add_remote.ui` & `cruiz-1.4.0a2/cruiz/resources/local_cache_add_remote.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/local_cache_install_config.ui` & `cruiz-1.4.0a2/cruiz/resources/local_cache_install_config.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/local_cache_manage.ui` & `cruiz-1.4.0a2/cruiz/resources/local_cache_manage.ui`

 * *Files 2% similar despite different names*

#### Comparing `cruiz-1.4.0a1/cruiz/resources/local_cache_manage.ui` & `cruiz-1.4.0a2/cruiz/resources/local_cache_manage.ui`

```diff
@@ -3,15 +3,15 @@
   <class>ManageLocalCaches</class>
   <widget class="QDialog" name="ManageLocalCaches">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>561</width>
-        <height>639</height>
+        <height>643</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Manage Local Caches</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
@@ -86,25 +86,25 @@
                     <layout class="QGridLayout" name="locationsLayout">
                       <item row="1" column="0">
                         <widget class="QLabel" name="loc_conan_user_home_short_label">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
-                            <string>CONAN_USER_HOME_SHORT</string>
+                            <string>Cache short home</string>
                           </property>
                         </widget>
                       </item>
                       <item row="0" column="0">
                         <widget class="QLabel" name="label_5">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
-                            <string>CONAN_USER_HOME</string>
+                            <string>Cache home</string>
                           </property>
                         </widget>
                       </item>
                       <item row="0" column="1">
                         <widget class="QLineEdit" name="conan_user_home"/>
                       </item>
                       <item row="1" column="1">
@@ -158,19 +158,30 @@
                             <property name="rightMargin">
                               <number>2</number>
                             </property>
                             <property name="bottomMargin">
                               <number>2</number>
                             </property>
                             <item>
-                              <widget class="QListWidget" name="profilesList">
-                                <property name="sizeAdjustPolicy">
-                                  <enum>QAbstractScrollArea::AdjustToContents</enum>
-                                </property>
-                              </widget>
+                              <layout class="QHBoxLayout" name="horizontalLayout_7">
+                                <item>
+                                  <widget class="QListWidget" name="profilesList">
+                                    <property name="sizeAdjustPolicy">
+                                      <enum>QAbstractScrollArea::AdjustToContents</enum>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
+                                  <widget class="QPushButton" name="profilesCreateDefault">
+                                    <property name="text">
+                                      <string>Create Default</string>
+                                    </property>
+                                  </widget>
+                                </item>
+                              </layout>
                             </item>
                           </layout>
                         </widget>
                       </item>
                       <item>
                         <widget class="QGroupBox" name="groupBox">
                           <property name="title">
```

### Comparing `cruiz-1.4.0a1/cruiz/resources/local_cache_move.ui` & `cruiz-1.4.0a2/cruiz/resources/local_cache_move.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/local_cache_new_wizard.ui` & `cruiz-1.4.0a2/cruiz/resources/local_cache_new_wizard.ui`

 * *Files 1% similar despite different names*

#### Comparing `cruiz-1.4.0a1/cruiz/resources/local_cache_new_wizard.ui` & `cruiz-1.4.0a2/cruiz/resources/local_cache_new_wizard.ui`

```diff
@@ -103,15 +103,15 @@
           </widget>
         </item>
       </layout>
     </widget>
     <widget class="NewLocalCacheLocationPage" name="locationsPage">
       <layout class="QVBoxLayout" name="verticalLayout_2">
         <item>
-          <widget class="QLabel" name="label_5">
+          <widget class="QLabel" name="userHomeExplanation">
             <property name="text">
               <string>Each local cache exists in a .conan folder in the specified directory.</string>
             </property>
             <property name="textFormat">
               <enum>Qt::MarkdownText</enum>
             </property>
             <property name="wordWrap">
@@ -120,15 +120,15 @@
           </widget>
         </item>
         <item>
           <layout class="QGridLayout" name="gridLayout_2">
             <item row="0" column="0">
               <widget class="QLabel" name="label_6">
                 <property name="text">
-                  <string>CONAN_USER_HOME</string>
+                  <string>Cache home</string>
                 </property>
               </widget>
             </item>
             <item row="0" column="1">
               <widget class="QLineEdit" name="userHome"/>
             </item>
           </layout>
@@ -147,15 +147,15 @@
           </widget>
         </item>
         <item>
           <layout class="QGridLayout" name="gridLayout_3">
             <item row="0" column="0">
               <widget class="QLabel" name="userHomeShortLabel">
                 <property name="text">
-                  <string>CONAN_USER_HOME_SHORT</string>
+                  <string>Cache short home</string>
                 </property>
               </widget>
             </item>
             <item row="0" column="1">
               <widget class="QLineEdit" name="userHomeShort"/>
             </item>
           </layout>
```

### Comparing `cruiz-1.4.0a1/cruiz/resources/local_cache_remove_environment.ui` & `cruiz-1.4.0a2/cruiz/resources/local_cache_remove_environment.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/local_cache_run_command_dialog.ui` & `cruiz-1.4.0a2/cruiz/resources/local_cache_run_command_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/preferences.ui` & `cruiz-1.4.0a2/cruiz/resources/preferences.ui`

 * *Files 2% similar despite different names*

#### Comparing `cruiz-1.4.0a1/cruiz/resources/preferences.ui` & `cruiz-1.4.0a2/cruiz/resources/preferences.ui`

```diff
@@ -172,15 +172,15 @@
             </layout>
           </widget>
           <widget class="QWidget" name="prefs_fonts">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>432</width>
+                <width>639</width>
                 <height>233</height>
               </rect>
             </property>
             <attribute name="label">
               <string>Fonts</string>
             </attribute>
             <layout class="QVBoxLayout" name="verticalLayout_2">
@@ -298,16 +298,16 @@
             </layout>
           </widget>
           <widget class="QWidget" name="prefs_conan">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>343</width>
-                <height>172</height>
+                <width>654</width>
+                <height>232</height>
               </rect>
             </property>
             <attribute name="label">
               <string>Conan</string>
             </attribute>
             <layout class="QVBoxLayout" name="verticalLayout_3">
               <item>
@@ -408,16 +408,16 @@
             </layout>
           </widget>
           <widget class="QWidget" name="prefs_localcache">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>297</width>
-                <height>203</height>
+                <width>654</width>
+                <height>232</height>
               </rect>
             </property>
             <attribute name="label">
               <string>Local cache</string>
             </attribute>
             <layout class="QVBoxLayout" name="verticalLayout_4">
               <item>
@@ -491,16 +491,16 @@
             </layout>
           </widget>
           <widget class="QWidget" name="prefs_graphviz">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>305</width>
-                <height>79</height>
+                <width>654</width>
+                <height>232</height>
               </rect>
             </property>
             <attribute name="label">
               <string>GraphViz</string>
             </attribute>
             <layout class="QGridLayout" name="gridLayout_8">
               <item row="2" column="1">
@@ -539,16 +539,16 @@
             </layout>
           </widget>
           <widget class="QWidget" name="prefs_cmake">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>175</width>
-                <height>86</height>
+                <width>654</width>
+                <height>232</height>
               </rect>
             </property>
             <attribute name="label">
               <string>CMake</string>
             </attribute>
             <layout class="QGridLayout" name="gridLayout_9">
               <item row="0" column="0">
@@ -600,15 +600,15 @@
             </layout>
           </widget>
           <widget class="QWidget" name="prefs_compilercache">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>405</width>
+                <width>639</width>
                 <height>384</height>
               </rect>
             </property>
             <attribute name="label">
               <string>Compiler cache</string>
             </attribute>
             <layout class="QVBoxLayout" name="verticalLayout_5">
@@ -750,15 +750,15 @@
               </item>
             </layout>
           </widget>
           <widget class="QWidget" name="prefs_shortcuts">
             <property name="geometry">
               <rect>
                 <x>0</x>
-                <y>0</y>
+                <y>-287</y>
                 <width>639</width>
                 <height>519</height>
               </rect>
             </property>
             <attribute name="label">
               <string>Shortcuts</string>
             </attribute>
@@ -826,15 +826,15 @@
                 <widget class="QLabel" name="label_22">
                   <property name="text">
                     <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/exportpackage.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan export-pkg&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                   </property>
                 </widget>
               </item>
               <item row="12" column="0">
-                <widget class="QLabel" name="label_26">
+                <widget class="QLabel" name="prefs_shortcuts_cmakebuildtool_label">
                   <property name="text">
                     <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/cmakebuildtool.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; CMake Build Tool&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                   </property>
                 </widget>
               </item>
               <item row="4" column="0">
                 <widget class="QLabel" name="label_5">
@@ -850,15 +850,15 @@
                 <widget class="QLabel" name="label_6">
                   <property name="text">
                     <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/source.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan source&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                   </property>
                 </widget>
               </item>
               <item row="13" column="0">
-                <widget class="QLabel" name="label_27">
+                <widget class="QLabel" name="prefs_shortcuts_cmakebuildtoolverbose_label">
                   <property name="text">
                     <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/cmakebuildtoolverbose.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; CMake Build Tool (verbose)&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                   </property>
                 </widget>
               </item>
               <item row="9" column="2">
                 <widget class="ShortcutLineEdit" name="prefs_shortcuts_test_edit"/>
@@ -876,29 +876,29 @@
                   </property>
                 </widget>
               </item>
               <item row="11" column="2">
                 <widget class="ShortcutLineEdit" name="prefs_shortcuts_cancel_edit"/>
               </item>
               <item row="7" column="0">
-                <widget class="QLabel" name="label_21">
+                <widget class="QLabel" name="prefs_shortcuts_package_label">
                   <property name="text">
                     <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/package.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan package&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                   </property>
                 </widget>
               </item>
               <item row="2" column="0">
-                <widget class="QLabel" name="label_3">
+                <widget class="QLabel" name="prefs_shortcuts_imports_label">
                   <property name="text">
                     <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/imports.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan imports&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                   </property>
                 </widget>
               </item>
               <item row="14" column="0">
-                <widget class="QLabel" name="label_28">
+                <widget class="QLabel" name="prefs_shortcuts_deletecmakecache_label">
                   <property name="text">
                     <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/removecmakecache.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; Delete CMakeCache&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                   </property>
                 </widget>
               </item>
               <item row="8" column="2">
                 <widget class="ShortcutLineEdit" name="prefs_shortcuts_exportpackage_edit"/>
@@ -938,16 +938,16 @@
             </layout>
           </widget>
           <widget class="QWidget" name="prefs_recipes">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>98</width>
-                <height>105</height>
+                <width>654</width>
+                <height>232</height>
               </rect>
             </property>
             <attribute name="label">
               <string>Recipes</string>
             </attribute>
             <layout class="QVBoxLayout" name="verticalLayout_7">
               <item>
@@ -994,16 +994,16 @@
             </layout>
           </widget>
           <widget class="QWidget" name="prefs_recentconfigs">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>98</width>
-                <height>105</height>
+                <width>654</width>
+                <height>232</height>
               </rect>
             </property>
             <attribute name="label">
               <string>Recent configs</string>
             </attribute>
             <layout class="QVBoxLayout" name="verticalLayout_8">
               <item>
@@ -1041,16 +1041,16 @@
             </layout>
           </widget>
           <widget class="QWidget" name="prefs_recentremotes">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>98</width>
-                <height>105</height>
+                <width>654</width>
+                <height>232</height>
               </rect>
             </property>
             <attribute name="label">
               <string>Recent remotes</string>
             </attribute>
             <layout class="QVBoxLayout" name="verticalLayout_9">
               <item>
```

### Comparing `cruiz-1.4.0a1/cruiz/resources/recipe_cmake_features_frame.ui` & `cruiz-1.4.0a2/cruiz/resources/recipe_cmake_features_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui` & `cruiz-1.4.0a2/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/recipe_compilercache_features_frame.ui` & `cruiz-1.4.0a2/cruiz/resources/recipe_compilercache_features_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/recipe_cpucores_frame.ui` & `cruiz-1.4.0a2/cruiz/resources/recipe_cpucores_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/recipe_local_workflow_expression_editor.ui` & `cruiz-1.4.0a2/cruiz/resources/recipe_local_workflow_expression_editor.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/recipe_profile_frame.ui` & `cruiz-1.4.0a2/cruiz/resources/recipe_profile_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/recipe_window.ui` & `cruiz-1.4.0a2/cruiz/resources/recipe_window.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/remote_browser.ui` & `cruiz-1.4.0a2/cruiz/resources/remote_browser.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/resources/remote_browser_fileview.ui` & `cruiz-1.4.0a2/cruiz/resources/remote_browser_fileview.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/revealonfilesystem.py` & `cruiz-1.4.0a2/cruiz/revealonfilesystem.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/ensuredefaultlocalcache.py` & `cruiz-1.4.0a2/cruiz/settings/ensuredefaultlocalcache.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/__init__.py` & `cruiz-1.4.0a2/cruiz/settings/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/basesettings.py` & `cruiz-1.4.0a2/cruiz/settings/managers/basesettings.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/cleansettings.py` & `cruiz-1.4.0a2/cruiz/settings/managers/cleansettings.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/cmakepreferences.py` & `cruiz-1.4.0a2/cruiz/settings/managers/cmakepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/compilercachepreferences.py` & `cruiz-1.4.0a2/cruiz/settings/managers/compilercachepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/conanpreferences.py` & `cruiz-1.4.0a2/cruiz/settings/managers/conanpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/fontpreferences.py` & `cruiz-1.4.0a2/cruiz/settings/managers/fontpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/generalpreferences.py` & `cruiz-1.4.0a2/cruiz/settings/managers/generalpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/graphvizpreferences.py` & `cruiz-1.4.0a2/cruiz/settings/managers/graphvizpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/localcachepreferences.py` & `cruiz-1.4.0a2/cruiz/settings/managers/localcachepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/namedlocalcache.py` & `cruiz-1.4.0a2/cruiz/settings/managers/namedlocalcache.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/ninjapreferences.py` & `cruiz-1.4.0a2/cruiz/settings/managers/ninjapreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/recentconanconfigs.py` & `cruiz-1.4.0a2/cruiz/settings/managers/recentconanconfigs.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/recentconanremotes.py` & `cruiz-1.4.0a2/cruiz/settings/managers/recentconanremotes.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/recentrecipes.py` & `cruiz-1.4.0a2/cruiz/settings/managers/recentrecipes.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/recipe.py` & `cruiz-1.4.0a2/cruiz/settings/managers/recipe.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/shortcuts.py` & `cruiz-1.4.0a2/cruiz/settings/managers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/valueclasses.py` & `cruiz-1.4.0a2/cruiz/settings/managers/valueclasses.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/managers/writermixin.py` & `cruiz-1.4.0a2/cruiz/settings/managers/writermixin.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/models/recentconanconfigmodel.py` & `cruiz-1.4.0a2/cruiz/settings/models/recentconanconfigmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/models/recentconanremotesmodel.py` & `cruiz-1.4.0a2/cruiz/settings/models/recentconanremotesmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/models/recipesmodel.py` & `cruiz-1.4.0a2/cruiz/settings/models/recipesmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/settings/preferencesdialog.py` & `cruiz-1.4.0a2/cruiz/settings/preferencesdialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 import json
 import pathlib
 import typing
 
 from qtpy import QtCore, QtGui, QtWidgets
 
+import cruiz.globals
+
 from cruiz.settings.managers.namedlocalcache import NamedLocalCacheSettingsReader
 
 from cruiz.pyside6.preferences import Ui_PreferencesDialog
 
 from cruiz.settings.managers.generalpreferences import (
     GeneralSettings,
     GeneralSettingsReader,
@@ -366,53 +368,69 @@
         )
 
     def _setup_shortcuts_toolbox(self) -> None:
         self._prefs_shortcuts = ShortcutSettings()
         self._ui.prefs_shortcuts_create_edit.textChanged.connect(
             self._shortcuts_change_create
         )
-        self._ui.prefs_shortcuts_imports_edit.textChanged.connect(
-            self._shortcuts_change_imports
-        )
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            self._ui.prefs_shortcuts_imports_edit.textChanged.connect(
+                self._shortcuts_change_imports
+            )
+        else:
+            self._ui.prefs_shortcuts_imports_label.hide()
+            self._ui.prefs_shortcuts_imports_edit.hide()
         self._ui.prefs_shortcuts_install_edit.textChanged.connect(
             self._shortcuts_change_install
         )
         self._ui.prefs_shortcuts_installupdates_edit.textChanged.connect(
             self._shortcuts_change_installupdates
         )
         self._ui.prefs_shortcuts_source_edit.textChanged.connect(
             self._shortcuts_change_source
         )
         self._ui.prefs_shortcuts_build_edit.textChanged.connect(
             self._shortcuts_change_build
         )
-        self._ui.prefs_shortcuts_package_edit.textChanged.connect(
-            self._shortcuts_change_package
-        )
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            self._ui.prefs_shortcuts_package_edit.textChanged.connect(
+                self._shortcuts_change_package
+            )
+        else:
+            self._ui.prefs_shortcuts_package_label.hide()
+            self._ui.prefs_shortcuts_package_edit.hide()
         self._ui.prefs_shortcuts_exportpackage_edit.textChanged.connect(
             self._shortcuts_change_exportpkg
         )
         self._ui.prefs_shortcuts_test_edit.textChanged.connect(
             self._shortcuts_change_test
         )
         self._ui.prefs_shortcuts_remove_edit.textChanged.connect(
             self._shortcuts_change_remove
         )
         self._ui.prefs_shortcuts_cancel_edit.textChanged.connect(
             self._shortcuts_change_cancel
         )
-        self._ui.prefs_shortcuts_cmakebuildtool_edit.textChanged.connect(
-            self._shortcuts_change_cmakebuildtool
-        )
-        self._ui.prefs_shortcuts_cmakebuildtoolverbose_edit.textChanged.connect(
-            self._shortcuts_change_cmakebuildtoolverbose
-        )
-        self._ui.prefs_shortcuts_deletecmakecache_edit.textChanged.connect(
-            self._shortcuts_change_deletecmakecache
-        )
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            self._ui.prefs_shortcuts_cmakebuildtool_edit.textChanged.connect(
+                self._shortcuts_change_cmakebuildtool
+            )
+            self._ui.prefs_shortcuts_cmakebuildtoolverbose_edit.textChanged.connect(
+                self._shortcuts_change_cmakebuildtoolverbose
+            )
+            self._ui.prefs_shortcuts_deletecmakecache_edit.textChanged.connect(
+                self._shortcuts_change_deletecmakecache
+            )
+        else:
+            self._ui.prefs_shortcuts_cmakebuildtool_label.hide()
+            self._ui.prefs_shortcuts_cmakebuildtool_edit.hide()
+            self._ui.prefs_shortcuts_cmakebuildtoolverbose_label.hide()
+            self._ui.prefs_shortcuts_cmakebuildtoolverbose_edit.hide()
+            self._ui.prefs_shortcuts_deletecmakecache_label.hide()
+            self._ui.prefs_shortcuts_deletecmakecache_edit.hide()
 
     def _setup_recipes_toolbox(self) -> None:
         self._prefs_recipes_model = RecipesModel()
         self._ui.prefs_recipes_table.setModel(self._prefs_recipes_model)
         self._ui.prefs_recipes_table.horizontalHeader().setSectionResizeMode(
             0, QtWidgets.QHeaderView.ResizeToContents
         )
```

### Comparing `cruiz-1.4.0a1/cruiz/settings/updatesettings.py` & `cruiz-1.4.0a2/cruiz/settings/updatesettings.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/svggraph.py` & `cruiz-1.4.0a2/cruiz/svggraph.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/version.py` & `cruiz-1.4.0a2/cruiz/version.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/widgets/aboutcruizdialog.py` & `cruiz-1.4.0a2/cruiz/widgets/aboutcruizdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/widgets/debugging.py` & `cruiz-1.4.0a2/cruiz/widgets/debugging.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/widgets/shortcutlineedit.py` & `cruiz-1.4.0a2/cruiz/widgets/shortcutlineedit.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/widgets/util.py` & `cruiz-1.4.0a2/cruiz/widgets/util.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/workers/utils/colorarma_conversion.py` & `cruiz-1.4.0a2/cruiz/workers/utils/colorarma_conversion.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/workers/utils/env.py` & `cruiz-1.4.0a2/cruiz/workers/utils/env.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/workers/utils/message.py` & `cruiz-1.4.0a2/cruiz/interop/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 """
-Conan worker message
+Conan interop message
 """
 
 import typing
 
 
 # pylint: disable=too-few-public-methods
 class Message:
```

### Comparing `cruiz-1.4.0a1/cruiz/workers/utils/qtlogger.py` & `cruiz-1.4.0a2/cruiz/workers/utils/qtlogger.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import logging
 import multiprocessing
 import typing
 
 import conans.util.log
 
-import cruiz.workers.utils.message
+from cruiz.interop.message import Message, ConanLogMessage
 
 
 class _Singleton(type):
     """
     Base class for all singletons
     """
 
@@ -37,24 +37,21 @@
 
     def __init__(self) -> None:
         super().__init__()
         formatter = conans.util.log.MultiLineFormatter(
             "%(levelname)-6s:%(filename)-15s[%(lineno)d]: %(message)s [%(asctime)s]"
         )
         self.setFormatter(formatter)
-        self._queue: typing.Optional[
-            multiprocessing.Queue[cruiz.workers.utils.message.Message]
-        ] = None
+        self._queue: typing.Optional[multiprocessing.Queue[Message]] = None
 
     def set_queue(
-        self, queue: multiprocessing.Queue[cruiz.workers.utils.message.Message]
+        self,
+        queue: multiprocessing.Queue[Message],
     ) -> None:
         """
         Set the multiprocessing queue to send messages with.
         """
         self._queue = queue
 
     def emit(self, record: typing.Any) -> None:
         assert self._queue
-        self._queue.put(
-            cruiz.workers.utils.message.ConanLogMessage(self.format(record))
-        )
+        self._queue.put(ConanLogMessage(self.format(record)))
```

### Comparing `cruiz-1.4.0a1/cruiz/workers/utils/stream.py` & `cruiz-1.4.0a2/cruiz/workers/utils/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import multiprocessing
 import six
 import typing
 
 from .colorarma_conversion import convert_from_colorama_to_html
 
-from cruiz.workers.utils.message import Message
+from cruiz.interop.message import Message
 
 
 if False:
     import io
 
     # Conan 1.30.0+ changed the assumptions on the base-class of streams used in their
     # runner output to be based from six, so this Python 3 implementation is no longer
```

### Comparing `cruiz-1.4.0a1/cruiz/workers/utils/text2html.py` & `cruiz-1.4.0a2/cruiz/workers/utils/text2html.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a1/cruiz/workers/utils/worker.py` & `cruiz-1.4.0a2/cruiz/workers/utils/worker.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 from cruiz.interop.commandparameters import CommandParameters
 from cruiz.interop.commonparameters import CommonParameters
 from cruiz.interop.searchrecipesparameters import SearchRecipesParameters
 from cruiz.interop.reciperevisionsparameters import RecipeRevisionsParameters
 from cruiz.interop.packagerevisionsparameters import PackageRevisionsParameters
 from cruiz.interop.packageidparameters import PackageIdParameters
 from cruiz.interop.packagebinaryparameters import PackageBinaryParameters
+from cruiz.interop.message import Message, Failure, Stdout
 
-from .env import set_env, clear_conan_env
-from .message import Message, Failure, Stdout
-from .text2html import text_to_html
+from cruiz.workers.utils.env import set_env, clear_conan_env
+from cruiz.workers.utils.text2html import text_to_html
 
 
 class Worker:
     """
     Non-Conan specific worker context manager
     """
 
@@ -108,56 +108,7 @@
                     f"{datetime.timedelta(seconds=elapsed_time / 1000)}"
                 )
             )
             self._queue.put(Stdout("-" * 64))
         self._queue.close()
         self._queue.join_thread()
         return True  # suppress further exception propogation
-
-
-# pylint: disable=too-few-public-methods
-class ConanWorker(Worker):
-    """
-    Conan specific context manager
-    """
-
-    def __enter__(self) -> typing.Any:
-        super().__enter__()
-        # import here because it can use the environment variables set in the
-        # super class
-        # pylint: disable=import-outside-toplevel
-        from .conanapi import instance
-
-        api = instance(self._queue, self._params)
-        return api
-
-
-def replace_conan_version_struct_with_string(
-    result: typing.Dict[typing.Any, typing.Any]
-) -> None:
-    """
-    Results have ConanVersion structs, but these cannot be passed over the
-    process divide so just convert them to strings
-    """
-    if "installed" not in result:
-        return
-    for installed in result["installed"]:
-        recipe = installed["recipe"]
-        recipe["version"] = str(recipe["version"])
-        for package in installed["packages"]:
-            try:
-                cpp_info = package["cpp_info"]
-            except KeyError:
-                # no cpp_info, so abort further processing
-                continue
-            cpp_info["version"] = str(cpp_info["version"])
-            with contextlib.suppress(KeyError):
-                # ignore 'components' not being in cpp_info
-                for component_key in cpp_info["components"]:
-                    component = cpp_info["components"][component_key]
-                    component["version"] = str(component["version"])
-            with contextlib.suppress(KeyError):
-                # ignore 'build_modules' not being in cpp_info
-                build_modules: typing.Dict[str, str] = {}
-                for key, value in cpp_info["build_modules"].items():
-                    build_modules[key] = value
-                cpp_info["build_modules"] = build_modules
```

### Comparing `cruiz-1.4.0a1/cruiz.egg-info/PKG-INFO` & `cruiz-1.4.0a2/cruiz.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cruiz
-Version: 1.4.0a1
+Version: 1.4.0a2
 Summary: Conan recipe user interface
 Home-page: https://github.com/markfinal/cruiz
 Author: Mark Final
 Author-email: markfinal@hotmail.com
 Project-URL: Documentation, https://cruiz.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/markfinal/cruiz
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,24 +34,29 @@
 See the documentation at [Read The Docs](https://cruiz.readthedocs.io/).
 
 ## Prerequisites
 
 - Intel x86_64 platforms:
   - Windows 10+
   - Linux (CentOS 7.5+/Ubuntu 18+)
-  - macOS (10.13+)
+  - macOS (11.0+)
 - Apple Silicon platforms:
   - macOS (11.0+)
 - Python 3.7-3.11
-- Conan 1.17.1+, but not 2.x (these are the versions tested)
+- Conan 1.x (from 1.17.1 onwards) and 2.x (from 2.0.7 onwards)
 
 All other Python dependencies are installed when the package is installed.
 
 In order to use the dependency graph visualisation, an additional installation of GraphViz is required from https://graphviz.org/download/. Assign the installed location to the preferences.
 
+## Conan versions
+Cruiz does _not_ depend directly on the Conan package in its UI. Instead, it uses child processes to run Conan APIs, which _are_ dependent on the Conan version installed.
+
+Cruiz does _not_ support multiple Conan versions simultaneously in the same process. Instead, the UI dynamically changes by detecting the Conan version installed at startup. You will therefore see a slightly different UI depending on which Conan you have. Note the Conan version detected is shown on the status bar in the bottom right corner of the UI.
+
 ## Getting started
 If you have cloned this repository, you will need:
 
 1. A Python 3 environment. Make a virtual env if necessary. `python3 -m venv <folder to be the env>`
     - Activate the virtual env with either:
         - `source <folder to be the env>/bin/activate` (Linux/macOSX)
         - `<folder to be the env>\Scripts\activate.bat` (Windows cmd)
```

### Comparing `cruiz-1.4.0a1/cruiz.egg-info/SOURCES.txt` & `cruiz-1.4.0a2/cruiz.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 cruiz/commands/logdetails.py
 cruiz/commands/messagereplyprocessor.py
 cruiz/commands/metarequestconaninvocation.py
 cruiz/interop/__init__.py
 cruiz/interop/commandparameters.py
 cruiz/interop/commonparameters.py
 cruiz/interop/dependencygraph.py
+cruiz/interop/message.py
 cruiz/interop/packagebinaryparameters.py
 cruiz/interop/packageidparameters.py
 cruiz/interop/packagenode.py
 cruiz/interop/packagerevisionsparameters.py
 cruiz/interop/pod.py
 cruiz/interop/reciperevisionsparameters.py
 cruiz/interop/searchrecipesparameters.py
@@ -167,41 +168,16 @@
 cruiz/settings/models/recipesmodel.py
 cruiz/widgets/__init__.py
 cruiz/widgets/aboutcruizdialog.py
 cruiz/widgets/debugging.py
 cruiz/widgets/shortcutlineedit.py
 cruiz/widgets/util.py
 cruiz/workers/__init__.py
-cruiz/workers/arbitrary.py
-cruiz/workers/build.py
-cruiz/workers/cmakebuildtool.py
-cruiz/workers/configinstall.py
-cruiz/workers/create.py
-cruiz/workers/deletecmakecache.py
-cruiz/workers/endmessagethread.py
-cruiz/workers/exportpackage.py
-cruiz/workers/imports.py
-cruiz/workers/install.py
-cruiz/workers/lockcreate.py
-cruiz/workers/meta.py
-cruiz/workers/package.py
-cruiz/workers/packagebinary.py
-cruiz/workers/packagedetails.py
-cruiz/workers/packagerevisions.py
-cruiz/workers/reciperevisions.py
-cruiz/workers/remotesearch.py
-cruiz/workers/removeallpackages.py
-cruiz/workers/removelocks.py
-cruiz/workers/removepackage.py
-cruiz/workers/source.py
-cruiz/workers/testpackage.py
+cruiz/workers/api/__init__.py
 cruiz/workers/utils/__init__.py
 cruiz/workers/utils/colorarma_conversion.py
-cruiz/workers/utils/conanapi.py
 cruiz/workers/utils/env.py
 cruiz/workers/utils/formatoptions.py
-cruiz/workers/utils/message.py
-cruiz/workers/utils/monkeypatch.py
 cruiz/workers/utils/qtlogger.py
 cruiz/workers/utils/stream.py
 cruiz/workers/utils/text2html.py
 cruiz/workers/utils/worker.py
```

### Comparing `cruiz-1.4.0a1/setup.py` & `cruiz-1.4.0a2/setup.py`

 * *Files identical despite different names*

