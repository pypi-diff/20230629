# Comparing `tmp/peek-field-app-3.4.5.tar.gz` & `tmp/peek-field-app-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-field-app-3.4.5.tar", last modified: Wed Jun 28 07:26:48 2023, max compression
+gzip compressed data, was "peek-field-app-3.4.6.tar", last modified: Thu Jun 29 10:20:37 2023, max compression
```

## Comparing `peek-field-app-3.4.5.tar` & `peek-field-app-3.4.6.tar`

### file list

```diff
@@ -1,260 +1,260 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.478082 peek-field-app-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      360 2023-06-28 07:26:48.478082 peek-field-app-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1038 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.467081 peek-field-app-3.4.5/peek_field_app/
--rw-r--r--   0 root         (0) root         (0)      487 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/.browserslistrc
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/.gitignore
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/README.md
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-28 07:26:48.000000 peek-field-app-3.4.5/peek_field_app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.468082 peek-field-app-3.4.5/peek_field_app/android/
--rw-r--r--   0 root         (0) root         (0)     1589 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.468082 peek-field-app-3.4.5/peek_field_app/android/app/
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/.npmignore
--rw-r--r--   0 root         (0) root         (0)     1523 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/build.gradle
--rw-r--r--   0 root         (0) root         (0)     1027 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/capacitor.build.gradle
--rw-r--r--   0 root         (0) root         (0)      751 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/proguard-rules.pro
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.465082 peek-field-app-3.4.5/peek_field_app/android/app/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.464082 peek-field-app-3.4.5/peek_field_app/android/app/src/androidTest/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.464082 peek-field-app-3.4.5/peek_field_app/android/app/src/androidTest/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.464082 peek-field-app-3.4.5/peek_field_app/android/app/src/androidTest/java/com/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.464082 peek-field-app-3.4.5/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/
--rw-r--r--   0 root         (0) root         (0)      757 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/ExampleInstrumentedTest.java
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/
--rw-r--r--   0 root         (0) root         (0)     2762 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/AndroidManifest.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/assets/
--rw-r--r--   0 root         (0) root         (0)      289 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/assets/capacitor.config.json
--rw-r--r--   0 root         (0) root         (0)     1344 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/assets/capacitor.plugins.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.464082 peek-field-app-3.4.5/peek_field_app/android/app/src/main/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.464082 peek-field-app-3.4.5/peek_field_app/android/app/src/main/java/com/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.464082 peek-field-app-3.4.5/peek_field_app/android/app/src/main/java/com/synerty/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/java/com/synerty/peek/
--rw-r--r--   0 root         (0) root         (0)      534 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/java/com/synerty/peek/MainActivity.java
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.465082 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable/
--rw-r--r--   0 root         (0) root         (0)     5589 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable/ic_launcher_background.xml
--rw-r--r--   0 root         (0) root         (0)     4040 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-hdpi/
--rw-r--r--   0 root         (0) root         (0)     7705 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-hdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-mdpi/
--rw-r--r--   0 root         (0) root         (0)     4040 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-mdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/
--rw-r--r--   0 root         (0) root         (0)     9251 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/
--rw-r--r--   0 root         (0) root         (0)    13984 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/
--rw-r--r--   0 root         (0) root         (0)    17683 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-hdpi/
--rw-r--r--   0 root         (0) root         (0)     7934 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-hdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-mdpi/
--rw-r--r--   0 root         (0) root         (0)     4096 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-mdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/
--rw-r--r--   0 root         (0) root         (0)     9875 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/
--rw-r--r--   0 root         (0) root         (0)    13346 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/
--rw-r--r--   0 root         (0) root         (0)    17489 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.469081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-v24/
--rw-r--r--   0 root         (0) root         (0)     1897 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-v24/ic_launcher_foreground.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.470081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/layout/
--rw-r--r--   0 root         (0) root         (0)      538 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/layout/activity_main.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.470081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/
--rw-r--r--   0 root         (0) root         (0)      265 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/ic_launcher.xml
--rw-r--r--   0 root         (0) root         (0)      265 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/ic_launcher_round.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.470081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-hdpi/
--rw-r--r--   0 root         (0) root         (0)     2786 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher.png
--rw-r--r--   0 root         (0) root         (0)     3450 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_foreground.png
--rw-r--r--   0 root         (0) root         (0)     4341 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_round.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.470081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-mdpi/
--rw-r--r--   0 root         (0) root         (0)     1869 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher.png
--rw-r--r--   0 root         (0) root         (0)     2110 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_foreground.png
--rw-r--r--   0 root         (0) root         (0)     2725 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_round.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.470081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xhdpi/
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png
--rw-r--r--   0 root         (0) root         (0)     5036 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_foreground.png
--rw-r--r--   0 root         (0) root         (0)     6593 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.470081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/
--rw-r--r--   0 root         (0) root         (0)     6644 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png
--rw-r--r--   0 root         (0) root         (0)     9793 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_foreground.png
--rw-r--r--   0 root         (0) root         (0)    10455 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.470081 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/
--rw-r--r--   0 root         (0) root         (0)     9441 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png
--rw-r--r--   0 root         (0) root         (0)    15529 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_foreground.png
--rw-r--r--   0 root         (0) root         (0)    15916 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.471082 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/values/
--rw-r--r--   0 root         (0) root         (0)      120 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/values/ic_launcher_background.xml
--rw-r--r--   0 root         (0) root         (0)      280 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/values/strings.xml
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/values/styles.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.471082 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/xml/
--rw-r--r--   0 root         (0) root         (0)      466 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/xml/config.xml
--rw-r--r--   0 root         (0) root         (0)      211 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/xml/file_paths.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.465082 peek-field-app-3.4.5/peek_field_app/android/app/src/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.465082 peek-field-app-3.4.5/peek_field_app/android/app/src/test/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.465082 peek-field-app-3.4.5/peek_field_app/android/app/src/test/java/com/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.465082 peek-field-app-3.4.5/peek_field_app/android/app/src/test/java/com/getcapacitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.471082 peek-field-app-3.4.5/peek_field_app/android/app/src/test/java/com/getcapacitor/myapp/
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/app/src/test/java/com/getcapacitor/myapp/ExampleUnitTest.java
--rw-r--r--   0 root         (0) root         (0)      622 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/build.gradle
--rw-r--r--   0 root         (0) root         (0)     1947 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/capacitor.settings.gradle
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.465082 peek-field-app-3.4.5/peek_field_app/android/gradle/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.471082 peek-field-app-3.4.5/peek_field_app/android/gradle/wrapper/
--rw-r--r--   0 root         (0) root         (0)    55616 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0 root         (0) root         (0)      233 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/gradle/wrapper/gradle-wrapper.properties
--rw-r--r--   0 root         (0) root         (0)     1072 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/gradle.properties
--rwxr-xr-x   0 root         (0) root         (0)     5856 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/gradlew
--rw-r--r--   0 root         (0) root         (0)     2842 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/gradlew.bat
--rw-r--r--   0 root         (0) root         (0)      208 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/settings.gradle
--rw-r--r--   0 root         (0) root         (0)      562 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/android/variables.gradle
--rw-r--r--   0 root         (0) root         (0)     7284 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/angular.json
--rw-r--r--   0 root         (0) root         (0)      355 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/capacitor.config.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.471082 peek-field-app-3.4.5/peek_field_app/e2e/
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/e2e/app.e2e-spec.ts
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/e2e/app.po.ts
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/e2e/tsconfig.e2e.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.471082 peek-field-app-3.4.5/peek_field_app/ios/
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.471082 peek-field-app-3.4.5/peek_field_app/ios/App/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.471082 peek-field-app-3.4.5/peek_field_app/ios/App/App/
--rw-r--r--   0 root         (0) root         (0)     3885 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/AppDelegate.swift
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.472082 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.474082 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@1x.png
--rw-r--r--   0 root         (0) root         (0)     3645 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x-1.png
--rw-r--r--   0 root         (0) root         (0)     3645 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x.png
--rw-r--r--   0 root         (0) root         (0)     7415 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@3x.png
--rw-r--r--   0 root         (0) root         (0)     2099 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@1x.png
--rw-r--r--   0 root         (0) root         (0)     6951 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x-1.png
--rw-r--r--   0 root         (0) root         (0)     6951 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x.png
--rw-r--r--   0 root         (0) root         (0)    14448 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@3x.png
--rw-r--r--   0 root         (0) root         (0)     3645 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@1x.png
--rw-r--r--   0 root         (0) root         (0)    12478 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x-1.png
--rw-r--r--   0 root         (0) root         (0)    12478 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x.png
--rw-r--r--   0 root         (0) root         (0)    26321 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@3x.png
--rw-r--r--   0 root         (0) root         (0)  1769991 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-512@2x.png
--rw-r--r--   0 root         (0) root         (0)    26321 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@2x.png
--rw-r--r--   0 root         (0) root         (0)    56548 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@3x.png
--rw-r--r--   0 root         (0) root         (0)    11435 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@1x.png
--rw-r--r--   0 root         (0) root         (0)    41291 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@2x.png
--rw-r--r--   0 root         (0) root         (0)    48964 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-83.5x83.5@2x.png
--rw-r--r--   0 root         (0) root         (0)     2889 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/Contents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.474082 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/Contents.json
--rw-r--r--   0 root         (0) root         (0)    41273 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-1.png
--rw-r--r--   0 root         (0) root         (0)    41273 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-2.png
--rw-r--r--   0 root         (0) root         (0)    41273 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.474082 peek-field-app-3.4.5/peek_field_app/ios/App/App/Base.lproj/
--rw-r--r--   0 root         (0) root         (0)     1994 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Base.lproj/LaunchScreen.storyboard
--rw-r--r--   0 root         (0) root         (0)     1019 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Base.lproj/Main.storyboard
--rw-r--r--   0 root         (0) root         (0)     2958 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/Info.plist
--rw-r--r--   0 root         (0) root         (0)      289 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/capacitor.config.json
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App/config.xml
--rw-r--r--   0 root         (0) root         (0)     2418 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App copy-Info.plist
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.471082 peek-field-app-3.4.5/peek_field_app/ios/App/App.xcodeproj/
--rw-r--r--   0 root         (0) root         (0)    17768 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App.xcodeproj/project.pbxproj
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.472082 peek-field-app-3.4.5/peek_field_app/ios/App/App.xcodeproj/project.xcworkspace/
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.465082 peek-field-app-3.4.5/peek_field_app/ios/App/App.xcodeproj/xcshareddata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.472082 peek-field-app-3.4.5/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/
--rw-r--r--   0 root         (0) root         (0)     2810 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/App.xcscheme
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.472082 peek-field-app-3.4.5/peek_field_app/ios/App/App.xcworkspace/
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.472082 peek-field-app-3.4.5/peek_field_app/ios/App/App.xcworkspace/xcshareddata/
--rw-r--r--   0 root         (0) root         (0)      238 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/App.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
--rw-r--r--   0 root         (0) root         (0)     1880 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/ios/App/Podfile
--rw-r--r--   0 root         (0) root         (0)     1341 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/karma.conf.js
--rw-r--r--   0 root         (0) root         (0)   675563 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/package-lock.json
--rw-r--r--   0 root         (0) root         (0)     3122 2023-06-28 07:26:48.000000 peek-field-app-3.4.5/peek_field_app/package.json
--rw-r--r--   0 root         (0) root         (0)      868 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/protractor.conf.js
--rw-r--r--   0 root         (0) root         (0)      279 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/proxy.conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.474082 peek-field-app-3.4.5/peek_field_app/resources/
--rw-r--r--   0 root         (0) root         (0)  1805857 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/resources/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.475082 peek-field-app-3.4.5/peek_field_app/scripts/
--rwxr-xr-x   0 root         (0) root         (0)    14824 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/scripts/build_capacitor_app.sh
--rw-r--r--   0 root         (0) root         (0)      734 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/scripts/exportOptionsPlist.plist.template
--rwxr-xr-x   0 root         (0) root         (0)     2601 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/scripts/prepare_capacitor_ios_app.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.476081 peek-field-app-3.4.5/peek_field_app/src/
--rw-r--r--   0 root         (0) root         (0)     1129 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/_components.scss
--rw-r--r--   0 root         (0) root         (0)     1343 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/_variables.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.476081 peek-field-app-3.4.5/peek_field_app/src/app/
--rw-r--r--   0 root         (0) root         (0)     2499 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/app.module.ts
--rw-r--r--   0 root         (0) root         (0)     1110 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/app.routes.ts
--rw-r--r--   0 root         (0) root         (0)      834 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/app.services.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.476081 peek-field-app-3.4.5/peek_field_app/src/app/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.476081 peek-field-app-3.4.5/peek_field_app/src/app/core/components/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.476081 peek-field-app-3.4.5/peek_field_app/src/app/core/components/app/
--rw-r--r--   0 root         (0) root         (0)      471 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/app/app.component.html
--rw-r--r--   0 root         (0) root         (0)      181 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/app/app.component.scss
--rw-r--r--   0 root         (0) root         (0)     2257 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/app/app.component.ts
--rw-r--r--   0 root         (0) root         (0)      859 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/components.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.476081 peek-field-app-3.4.5/peek_field_app/src/app/core/components/header/
--rw-r--r--   0 root         (0) root         (0)     2351 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/header/header.component.html
--rw-r--r--   0 root         (0) root         (0)     1362 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/header/header.component.scss
--rw-r--r--   0 root         (0) root         (0)     2046 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/header/header.component.ts
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/header/index.ts
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.477082 peek-field-app-3.4.5/peek_field_app/src/app/core/components/status/
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/status/index.ts
--rw-r--r--   0 root         (0) root         (0)      861 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/status/status.component.html
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/status/status.component.scss
--rw-r--r--   0 root         (0) root         (0)     1585 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/components/status/status.component.ts
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/core/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.477082 peek-field-app-3.4.5/peek_field_app/src/app/pages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.477082 peek-field-app-3.4.5/peek_field_app/src/app/pages/config/
--rw-r--r--   0 root         (0) root         (0)      946 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/config/config.page.html
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/config/config.page.scss
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/config/config.page.ts
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/config/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.477082 peek-field-app-3.4.5/peek_field_app/src/app/pages/home/
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/home/home.page.html
--rw-r--r--   0 root         (0) root         (0)     1874 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/home/home.page.scss
--rw-r--r--   0 root         (0) root         (0)     1867 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/home/home.page.ts
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/home/index.ts
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/index.ts
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/pages.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.477082 peek-field-app-3.4.5/peek_field_app/src/app/pages/unknown-route/
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/unknown-route/index.ts
--rw-r--r--   0 root         (0) root         (0)    19057 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/unknown-route/unknown-route.page.html
--rw-r--r--   0 root         (0) root         (0)      810 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/unknown-route/unknown-route.page.scss
--rw-r--r--   0 root         (0) root         (0)      513 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/pages/unknown-route/unknown-route.page.ts
--rw-r--r--   0 root         (0) root         (0)      222 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/app/plugin-root.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.478082 peek-field-app-3.4.5/peek_field_app/src/assets/
--rw-r--r--   0 root         (0) root         (0)   156480 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/assets/Poppins-Medium.ttf
--rw-r--r--   0 root         (0) root         (0)   158192 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/assets/Poppins-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   155192 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/assets/Poppins-SemiBold.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.478082 peek-field-app-3.4.5/peek_field_app/src/assets/peek_core_docdb/
--rw-r--r--   0 root         (0) root         (0)    12054 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/assets/peek_core_docdb/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.478082 peek-field-app-3.4.5/peek_field_app/src/assets/peek_core_search/
--rw-r--r--   0 root         (0) root         (0)    12730 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/assets/peek_core_search/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.478082 peek-field-app-3.4.5/peek_field_app/src/assets/peek_core_user/
--rw-r--r--   0 root         (0) root         (0)     5572 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/assets/peek_core_user/plugin_icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.478082 peek-field-app-3.4.5/peek_field_app/src/environments/
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/environments/environment.prod.ts
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/environments/environment.ts
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-28 07:26:48.000000 peek-field-app-3.4.5/peek_field_app/src/environments/peek-app-environment.ts
--rw-r--r--   0 root         (0) root         (0)    39980 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     5317 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/index.html
--rw-r--r--   0 root         (0) root         (0)      883 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/main.ts
--rw-r--r--   0 root         (0) root         (0)     2395 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/polyfills.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.478082 peek-field-app-3.4.5/peek_field_app/src/styles/
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/styles/ant-design.scss
--rw-r--r--   0 root         (0) root         (0)     7181 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/styles/shared.scss
--rw-r--r--   0 root         (0) root         (0)     2251 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/styles/styles-layout.scss
--rw-r--r--   0 root         (0) root         (0)    33037 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/styles/theme.less
--rw-r--r--   0 root         (0) root         (0)     1593 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/styles.scss
--rw-r--r--   0 root         (0) root         (0)     1090 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/test.ts
--rw-r--r--   0 root         (0) root         (0)      521 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/tsconfig.app.json
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/tsconfig.spec.json
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/src/typings.d.ts
--rw-r--r--   0 root         (0) root         (0)      414 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/tsconfig.json
--rw-r--r--   0 root         (0) root         (0)      320 2023-06-28 07:25:24.000000 peek-field-app-3.4.5/peek_field_app/tsconfig.worker.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:48.468082 peek-field-app-3.4.5/peek_field_app.egg-info/
--rw-r--r--   0 root         (0) root         (0)      360 2023-06-28 07:26:48.000000 peek-field-app-3.4.5/peek_field_app.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9983 2023-06-28 07:26:48.000000 peek-field-app-3.4.5/peek_field_app.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:48.000000 peek-field-app-3.4.5/peek_field_app.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:48.000000 peek-field-app-3.4.5/peek_field_app.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-28 07:26:48.000000 peek-field-app-3.4.5/peek_field_app.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-28 07:26:48.000000 peek-field-app-3.4.5/peek_field_app.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:26:48.478082 peek-field-app-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3087 2023-06-28 07:26:48.000000 peek-field-app-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.531434 peek-field-app-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      360 2023-06-29 10:20:37.531434 peek-field-app-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.520434 peek-field-app-3.4.6/peek_field_app/
+-rw-r--r--   0 root         (0) root         (0)      487 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/.browserslistrc
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/README.md
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-29 10:20:37.000000 peek-field-app-3.4.6/peek_field_app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.521434 peek-field-app-3.4.6/peek_field_app/android/
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.521434 peek-field-app-3.4.6/peek_field_app/android/app/
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/.npmignore
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/build.gradle
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/capacitor.build.gradle
+-rw-r--r--   0 root         (0) root         (0)      751 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/proguard-rules.pro
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.518434 peek-field-app-3.4.6/peek_field_app/android/app/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.517434 peek-field-app-3.4.6/peek_field_app/android/app/src/androidTest/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.517434 peek-field-app-3.4.6/peek_field_app/android/app/src/androidTest/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.517434 peek-field-app-3.4.6/peek_field_app/android/app/src/androidTest/java/com/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.517434 peek-field-app-3.4.6/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.521434 peek-field-app-3.4.6/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/
+-rw-r--r--   0 root         (0) root         (0)      757 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/ExampleInstrumentedTest.java
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.521434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/AndroidManifest.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.521434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/assets/
+-rw-r--r--   0 root         (0) root         (0)      289 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/assets/capacitor.config.json
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/assets/capacitor.plugins.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.517434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.517434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/java/com/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.517434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/java/com/synerty/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.521434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/java/com/synerty/peek/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/java/com/synerty/peek/MainActivity.java
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.518434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.521434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable/
+-rw-r--r--   0 root         (0) root         (0)     5589 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable/ic_launcher_background.xml
+-rw-r--r--   0 root         (0) root         (0)     4040 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-hdpi/
+-rw-r--r--   0 root         (0) root         (0)     7705 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-hdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-mdpi/
+-rw-r--r--   0 root         (0) root         (0)     4040 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-mdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/
+-rw-r--r--   0 root         (0) root         (0)     9251 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/
+-rw-r--r--   0 root         (0) root         (0)    13984 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/
+-rw-r--r--   0 root         (0) root         (0)    17683 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-hdpi/
+-rw-r--r--   0 root         (0) root         (0)     7934 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-hdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-mdpi/
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-mdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/
+-rw-r--r--   0 root         (0) root         (0)     9875 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/
+-rw-r--r--   0 root         (0) root         (0)    13346 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/
+-rw-r--r--   0 root         (0) root         (0)    17489 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-v24/
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-v24/ic_launcher_foreground.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/layout/
+-rw-r--r--   0 root         (0) root         (0)      538 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/layout/activity_main.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/ic_launcher.xml
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/ic_launcher_round.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.522434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-hdpi/
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher.png
+-rw-r--r--   0 root         (0) root         (0)     3450 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_foreground.png
+-rw-r--r--   0 root         (0) root         (0)     4341 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_round.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.523434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-mdpi/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher.png
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_foreground.png
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_round.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.523434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xhdpi/
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png
+-rw-r--r--   0 root         (0) root         (0)     5036 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_foreground.png
+-rw-r--r--   0 root         (0) root         (0)     6593 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.523434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/
+-rw-r--r--   0 root         (0) root         (0)     6644 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png
+-rw-r--r--   0 root         (0) root         (0)     9793 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_foreground.png
+-rw-r--r--   0 root         (0) root         (0)    10455 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.523434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/
+-rw-r--r--   0 root         (0) root         (0)     9441 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png
+-rw-r--r--   0 root         (0) root         (0)    15529 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_foreground.png
+-rw-r--r--   0 root         (0) root         (0)    15916 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.523434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/values/
+-rw-r--r--   0 root         (0) root         (0)      120 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/values/ic_launcher_background.xml
+-rw-r--r--   0 root         (0) root         (0)      280 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/values/strings.xml
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/values/styles.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.523434 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/xml/
+-rw-r--r--   0 root         (0) root         (0)      466 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/xml/config.xml
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/xml/file_paths.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.518434 peek-field-app-3.4.6/peek_field_app/android/app/src/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.518434 peek-field-app-3.4.6/peek_field_app/android/app/src/test/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.518434 peek-field-app-3.4.6/peek_field_app/android/app/src/test/java/com/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.518434 peek-field-app-3.4.6/peek_field_app/android/app/src/test/java/com/getcapacitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.523434 peek-field-app-3.4.6/peek_field_app/android/app/src/test/java/com/getcapacitor/myapp/
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/app/src/test/java/com/getcapacitor/myapp/ExampleUnitTest.java
+-rw-r--r--   0 root         (0) root         (0)      622 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/build.gradle
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/capacitor.settings.gradle
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.518434 peek-field-app-3.4.6/peek_field_app/android/gradle/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.524434 peek-field-app-3.4.6/peek_field_app/android/gradle/wrapper/
+-rw-r--r--   0 root         (0) root         (0)    55616 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/gradle/wrapper/gradle-wrapper.properties
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/gradle.properties
+-rwxr-xr-x   0 root         (0) root         (0)     5856 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/gradlew
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/gradlew.bat
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/settings.gradle
+-rw-r--r--   0 root         (0) root         (0)      562 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/android/variables.gradle
+-rw-r--r--   0 root         (0) root         (0)     7284 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/angular.json
+-rw-r--r--   0 root         (0) root         (0)      355 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/capacitor.config.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.524434 peek-field-app-3.4.6/peek_field_app/e2e/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/e2e/app.e2e-spec.ts
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/e2e/app.po.ts
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/e2e/tsconfig.e2e.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.524434 peek-field-app-3.4.6/peek_field_app/ios/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.524434 peek-field-app-3.4.6/peek_field_app/ios/App/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.524434 peek-field-app-3.4.6/peek_field_app/ios/App/App/
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/AppDelegate.swift
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.524434 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.526434 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@1x.png
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x-1.png
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x.png
+-rw-r--r--   0 root         (0) root         (0)     7415 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@3x.png
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@1x.png
+-rw-r--r--   0 root         (0) root         (0)     6951 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x-1.png
+-rw-r--r--   0 root         (0) root         (0)     6951 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x.png
+-rw-r--r--   0 root         (0) root         (0)    14448 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@3x.png
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@1x.png
+-rw-r--r--   0 root         (0) root         (0)    12478 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x-1.png
+-rw-r--r--   0 root         (0) root         (0)    12478 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x.png
+-rw-r--r--   0 root         (0) root         (0)    26321 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@3x.png
+-rw-r--r--   0 root         (0) root         (0)  1769991 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-512@2x.png
+-rw-r--r--   0 root         (0) root         (0)    26321 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@2x.png
+-rw-r--r--   0 root         (0) root         (0)    56548 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@3x.png
+-rw-r--r--   0 root         (0) root         (0)    11435 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@1x.png
+-rw-r--r--   0 root         (0) root         (0)    41291 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@2x.png
+-rw-r--r--   0 root         (0) root         (0)    48964 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-83.5x83.5@2x.png
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/Contents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.527434 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/Contents.json
+-rw-r--r--   0 root         (0) root         (0)    41273 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-1.png
+-rw-r--r--   0 root         (0) root         (0)    41273 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-2.png
+-rw-r--r--   0 root         (0) root         (0)    41273 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.527434 peek-field-app-3.4.6/peek_field_app/ios/App/App/Base.lproj/
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Base.lproj/LaunchScreen.storyboard
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Base.lproj/Main.storyboard
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/Info.plist
+-rw-r--r--   0 root         (0) root         (0)      289 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/capacitor.config.json
+-rw-r--r--   0 root         (0) root         (0)      385 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App/config.xml
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App copy-Info.plist
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.524434 peek-field-app-3.4.6/peek_field_app/ios/App/App.xcodeproj/
+-rw-r--r--   0 root         (0) root         (0)    17768 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App.xcodeproj/project.pbxproj
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.524434 peek-field-app-3.4.6/peek_field_app/ios/App/App.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.518434 peek-field-app-3.4.6/peek_field_app/ios/App/App.xcodeproj/xcshareddata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.524434 peek-field-app-3.4.6/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/App.xcscheme
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.524434 peek-field-app-3.4.6/peek_field_app/ios/App/App.xcworkspace/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.524434 peek-field-app-3.4.6/peek_field_app/ios/App/App.xcworkspace/xcshareddata/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/App.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/ios/App/Podfile
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/karma.conf.js
+-rw-r--r--   0 root         (0) root         (0)   675565 2023-06-29 10:19:20.000000 peek-field-app-3.4.6/peek_field_app/package-lock.json
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-06-29 10:20:37.000000 peek-field-app-3.4.6/peek_field_app/package.json
+-rw-r--r--   0 root         (0) root         (0)      868 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/protractor.conf.js
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/proxy.conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.527434 peek-field-app-3.4.6/peek_field_app/resources/
+-rw-r--r--   0 root         (0) root         (0)  1805857 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/resources/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.528434 peek-field-app-3.4.6/peek_field_app/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)    14824 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/scripts/build_capacitor_app.sh
+-rw-r--r--   0 root         (0) root         (0)      734 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/scripts/exportOptionsPlist.plist.template
+-rwxr-xr-x   0 root         (0) root         (0)     2601 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/scripts/prepare_capacitor_ios_app.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.528434 peek-field-app-3.4.6/peek_field_app/src/
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/_components.scss
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/_variables.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.528434 peek-field-app-3.4.6/peek_field_app/src/app/
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/app.module.ts
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/app.routes.ts
+-rw-r--r--   0 root         (0) root         (0)      834 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/app.services.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.529434 peek-field-app-3.4.6/peek_field_app/src/app/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.529434 peek-field-app-3.4.6/peek_field_app/src/app/core/components/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.529434 peek-field-app-3.4.6/peek_field_app/src/app/core/components/app/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/app/app.component.html
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/app/app.component.scss
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/app/app.component.ts
+-rw-r--r--   0 root         (0) root         (0)      859 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/components.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.529434 peek-field-app-3.4.6/peek_field_app/src/app/core/components/header/
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/header/header.component.html
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/header/header.component.scss
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/header/header.component.ts
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/header/index.ts
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.529434 peek-field-app-3.4.6/peek_field_app/src/app/core/components/status/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/status/index.ts
+-rw-r--r--   0 root         (0) root         (0)      861 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/status/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/status/status.component.scss
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/components/status/status.component.ts
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/core/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.529434 peek-field-app-3.4.6/peek_field_app/src/app/pages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.530434 peek-field-app-3.4.6/peek_field_app/src/app/pages/config/
+-rw-r--r--   0 root         (0) root         (0)      946 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/config/config.page.html
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/config/config.page.scss
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/config/config.page.ts
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/config/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.530434 peek-field-app-3.4.6/peek_field_app/src/app/pages/home/
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/home/home.page.html
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/home/home.page.scss
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/home/home.page.ts
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/home/index.ts
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/index.ts
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/pages.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.530434 peek-field-app-3.4.6/peek_field_app/src/app/pages/unknown-route/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/unknown-route/index.ts
+-rw-r--r--   0 root         (0) root         (0)    19057 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/unknown-route/unknown-route.page.html
+-rw-r--r--   0 root         (0) root         (0)      810 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/unknown-route/unknown-route.page.scss
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/pages/unknown-route/unknown-route.page.ts
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/app/plugin-root.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.530434 peek-field-app-3.4.6/peek_field_app/src/assets/
+-rw-r--r--   0 root         (0) root         (0)   156480 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/assets/Poppins-Medium.ttf
+-rw-r--r--   0 root         (0) root         (0)   158192 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/assets/Poppins-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)   155192 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/assets/Poppins-SemiBold.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.530434 peek-field-app-3.4.6/peek_field_app/src/assets/peek_core_docdb/
+-rw-r--r--   0 root         (0) root         (0)    12054 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/assets/peek_core_docdb/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.530434 peek-field-app-3.4.6/peek_field_app/src/assets/peek_core_search/
+-rw-r--r--   0 root         (0) root         (0)    12730 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/assets/peek_core_search/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.531434 peek-field-app-3.4.6/peek_field_app/src/assets/peek_core_user/
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/assets/peek_core_user/plugin_icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.531434 peek-field-app-3.4.6/peek_field_app/src/environments/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/environments/environment.prod.ts
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/environments/environment.ts
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-29 10:20:37.000000 peek-field-app-3.4.6/peek_field_app/src/environments/peek-app-environment.ts
+-rw-r--r--   0 root         (0) root         (0)    39980 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     5317 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/index.html
+-rw-r--r--   0 root         (0) root         (0)      883 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/main.ts
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/polyfills.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.531434 peek-field-app-3.4.6/peek_field_app/src/styles/
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/styles/ant-design.scss
+-rw-r--r--   0 root         (0) root         (0)     7181 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/styles/shared.scss
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/styles/styles-layout.scss
+-rw-r--r--   0 root         (0) root         (0)    33037 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/styles/theme.less
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/styles.scss
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/test.ts
+-rw-r--r--   0 root         (0) root         (0)      521 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/tsconfig.app.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/tsconfig.spec.json
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/src/typings.d.ts
+-rw-r--r--   0 root         (0) root         (0)      414 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/tsconfig.json
+-rw-r--r--   0 root         (0) root         (0)      320 2023-06-29 10:19:15.000000 peek-field-app-3.4.6/peek_field_app/tsconfig.worker.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:37.520434 peek-field-app-3.4.6/peek_field_app.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      360 2023-06-29 10:20:37.000000 peek-field-app-3.4.6/peek_field_app.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9983 2023-06-29 10:20:37.000000 peek-field-app-3.4.6/peek_field_app.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:37.000000 peek-field-app-3.4.6/peek_field_app.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:37.000000 peek-field-app-3.4.6/peek_field_app.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-29 10:20:37.000000 peek-field-app-3.4.6/peek_field_app.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-29 10:20:37.000000 peek-field-app-3.4.6/peek_field_app.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:20:37.531434 peek-field-app-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3087 2023-06-29 10:20:37.000000 peek-field-app-3.4.6/setup.py
```

### Comparing `peek-field-app-3.4.5/README.rst` & `peek-field-app-3.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/README.md` & `peek-field-app-3.4.6/peek_field_app/README.md`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/.gitignore` & `peek-field-app-3.4.6/peek_field_app/android/.gitignore`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/build.gradle` & `peek-field-app-3.4.6/peek_field_app/android/app/build.gradle`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/capacitor.build.gradle` & `peek-field-app-3.4.6/peek_field_app/android/app/capacitor.build.gradle`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/proguard-rules.pro` & `peek-field-app-3.4.6/peek_field_app/android/app/proguard-rules.pro`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/ExampleInstrumentedTest.java` & `peek-field-app-3.4.6/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/ExampleInstrumentedTest.java`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/AndroidManifest.xml` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/assets/capacitor.plugins.json` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/assets/capacitor.plugins.json`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/java/com/synerty/peek/MainActivity.java` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/java/com/synerty/peek/MainActivity.java`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable/ic_launcher_background.xml` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable/ic_launcher_background.xml`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable/splash.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-hdpi/splash.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-hdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-mdpi/splash.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-mdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/splash.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/splash.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/splash.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-hdpi/splash.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-hdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-mdpi/splash.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-mdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/splash.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/splash.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/splash.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/drawable-v24/ic_launcher_foreground.xml` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/drawable-v24/ic_launcher_foreground.xml`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/layout/activity_main.xml` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/layout/activity_main.xml`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_foreground.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_foreground.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_round.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_foreground.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_foreground.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_round.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_foreground.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_foreground.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_foreground.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_foreground.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_foreground.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_foreground.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/app/src/main/res/values/styles.xml` & `peek-field-app-3.4.6/peek_field_app/android/app/src/main/res/values/styles.xml`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/build.gradle` & `peek-field-app-3.4.6/peek_field_app/android/build.gradle`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/capacitor.settings.gradle` & `peek-field-app-3.4.6/peek_field_app/android/capacitor.settings.gradle`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/gradle/wrapper/gradle-wrapper.jar` & `peek-field-app-3.4.6/peek_field_app/android/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/gradle.properties` & `peek-field-app-3.4.6/peek_field_app/android/gradle.properties`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/gradlew` & `peek-field-app-3.4.6/peek_field_app/android/gradlew`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/gradlew.bat` & `peek-field-app-3.4.6/peek_field_app/android/gradlew.bat`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/android/variables.gradle` & `peek-field-app-3.4.6/peek_field_app/android/variables.gradle`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/angular.json` & `peek-field-app-3.4.6/peek_field_app/angular.json`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/AppDelegate.swift` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/AppDelegate.swift`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@1x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@1x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x-1.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x-1.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@3x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@3x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@1x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@1x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x-1.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x-1.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@3x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@3x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@1x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@1x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x-1.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x-1.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@3x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@3x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-512@2x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-512@2x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@2x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@2x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@3x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@3x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@1x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@1x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@2x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@2x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-83.5x83.5@2x.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-83.5x83.5@2x.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/Contents.json` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-1.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-1.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-2.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-2.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732.png` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Base.lproj/LaunchScreen.storyboard` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Base.lproj/LaunchScreen.storyboard`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Base.lproj/Main.storyboard` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Base.lproj/Main.storyboard`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App/Info.plist` & `peek-field-app-3.4.6/peek_field_app/ios/App/App/Info.plist`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App copy-Info.plist` & `peek-field-app-3.4.6/peek_field_app/ios/App/App copy-Info.plist`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App.xcodeproj/project.pbxproj` & `peek-field-app-3.4.6/peek_field_app/ios/App/App.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/App.xcscheme` & `peek-field-app-3.4.6/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/App.xcscheme`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/ios/App/Podfile` & `peek-field-app-3.4.6/peek_field_app/ios/App/Podfile`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/karma.conf.js` & `peek-field-app-3.4.6/peek_field_app/karma.conf.js`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/package-lock.json` & `peek-field-app-3.4.6/peek_field_app/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999851733576642%*

 * *Differences: {"'dependencies'": "{'@synerty/vortexjs': {'version': '3.3.11', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.3.11.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-IkbVN+gLBE0NJBQEjlqAAbkfvQTCp6A8vU/gLZJXsHvUzsEf7poHSt4Vf2NauWF3N1nJh2Yt20f1T/vjxdDlyw==', "*

 * *                   "'dependencies': {'tslib': {'version': '2.6.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/tslib/-/tslib-2.6.0.tgz', 'integrity': "*

 * *                 […]*

```diff
@@ -2286,25 +2286,25 @@
             },
             "resolved": "https://registry.npmjs.org/@synerty/peek-plugin-base-js/-/peek-plugin-base-js-10.7.10.tgz",
             "version": "10.7.10"
         },
         "@synerty/vortexjs": {
             "dependencies": {
                 "tslib": {
-                    "integrity": "sha512-mSxlJJwl3BMEQCUNnxXBU9jP4JBktcEGhURcPR6VQVlnP0FdDEsIaz0C35dXNGLyRfrATNofF0F5p2KPxQgB+w==",
-                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.5.3.tgz",
-                    "version": "2.5.3"
+                    "integrity": "sha512-7At1WUettjcSRHXCyYtTselblcHl9PJFFVKiCAy/bY97+BPZXSQ2wbq0P9s8tK2G7dFQfNnlJnPAiArVBVBsfA==",
+                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.6.0.tgz",
+                    "version": "2.6.0"
                 }
             },
-            "integrity": "sha512-WuMRpei1gHkT7pUGBtuIjRAl7U5KY5rkKdmgJXIBjl378wjo+pcTlkobrzAZf1mfx7OlrAMP5C9pPWOjzEhgBw==",
+            "integrity": "sha512-IkbVN+gLBE0NJBQEjlqAAbkfvQTCp6A8vU/gLZJXsHvUzsEf7poHSt4Vf2NauWF3N1nJh2Yt20f1T/vjxdDlyw==",
             "requires": {
                 "tslib": "^2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.3.9.tgz",
-            "version": "3.3.9"
+            "resolved": "https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.3.11.tgz",
+            "version": "3.3.11"
         },
         "@types/cordova": {
             "integrity": "sha512-rkiiTuf/z2wTd4RxFOb+clE7PF4AEJU0hsczbUdkHHBtkUmpWQpEddynNfJYKYtZFJKbq4F+brfekt1kx85IZA==",
             "resolved": "https://registry.npmjs.org/@types/cordova/-/cordova-0.0.34.tgz",
             "version": "0.0.34"
         },
         "@types/emscripten": {
```

### Comparing `peek-field-app-3.4.5/peek_field_app/package.json` & `peek-field-app-3.4.6/peek_field_app/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9218820861678004%*

 * *Differences: {"'dependencies'": "{'@synerty/vortexjs': '^3.3.11', 'angular-svg-icon': '^13.4.6'}",*

 * * "'scripts'": "{'start': 'ng serve --disableHostCheck --host 3.4.6.0 --port 4000 --proxy-config "*

 * *              "proxy.conf.json'}",*

 * * "'version'": "'3.4.6'"}*

```diff
@@ -25,16 +25,16 @@
         "@capacitor/filesystem": "^1.1.0",
         "@capacitor/geolocation": "^1.3.1",
         "@capacitor/ios": "^3.5.1",
         "@capacitor/local-notifications": "^1.1.0",
         "@capacitor/network": "^1.0.7",
         "@ionic/pwa-elements": "^3.1.1",
         "@synerty/peek-plugin-base-js": "^10.7.10",
-        "@synerty/vortexjs": "^3.3.9",
-        "angular-svg-icon": "^13.4.5",
+        "@synerty/vortexjs": "^3.3.11",
+        "angular-svg-icon": "^13.4.6",
         "base-64": "^1.0.0",
         "bootstrap": "^3.3.7",
         "cordova-open-native-settings": "^1.5.5",
         "cordova-plugin-nativeaudio": "^3.0.9",
         "core-js": "^3.6.5",
         "jquery": "^3.3.1",
         "json-stable-stringify": "^1.0.1",
@@ -73,12 +73,12 @@
     "private": true,
     "scripts": {
         "build": "ng build",
         "e2e": "ng e2e",
         "lint": "ng lint",
         "ng": "ng",
         "postinstall": "ngcc --properties es2015 es5 browser module main --first-only --create-ivy-entry-points",
-        "start": "ng serve --disableHostCheck --host 3.4.5.0 --port 4000 --proxy-config proxy.conf.json",
+        "start": "ng serve --disableHostCheck --host 3.4.6.0 --port 4000 --proxy-config proxy.conf.json",
         "test": "ng test"
     },
-    "version": "3.4.5"
+    "version": "3.4.6"
 }
```

### Comparing `peek-field-app-3.4.5/peek_field_app/protractor.conf.js` & `peek-field-app-3.4.6/peek_field_app/protractor.conf.js`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/resources/icon.png` & `peek-field-app-3.4.6/peek_field_app/resources/icon.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/scripts/build_capacitor_app.sh` & `peek-field-app-3.4.6/peek_field_app/scripts/build_capacitor_app.sh`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/scripts/exportOptionsPlist.plist.template` & `peek-field-app-3.4.6/peek_field_app/scripts/exportOptionsPlist.plist.template`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/scripts/prepare_capacitor_ios_app.sh` & `peek-field-app-3.4.6/peek_field_app/scripts/prepare_capacitor_ios_app.sh`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/_components.scss` & `peek-field-app-3.4.6/peek_field_app/src/_components.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/_variables.scss` & `peek-field-app-3.4.6/peek_field_app/src/_variables.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/app.module.ts` & `peek-field-app-3.4.6/peek_field_app/src/app/app.module.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/app.routes.ts` & `peek-field-app-3.4.6/peek_field_app/src/app/app.routes.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/app.services.ts` & `peek-field-app-3.4.6/peek_field_app/src/app/app.services.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/core/components/app/app.component.ts` & `peek-field-app-3.4.6/peek_field_app/src/app/core/components/app/app.component.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/core/components/components.module.ts` & `peek-field-app-3.4.6/peek_field_app/src/app/core/components/components.module.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/core/components/header/header.component.html` & `peek-field-app-3.4.6/peek_field_app/src/app/core/components/header/header.component.html`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/core/components/header/header.component.scss` & `peek-field-app-3.4.6/peek_field_app/src/app/core/components/header/header.component.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/core/components/header/header.component.ts` & `peek-field-app-3.4.6/peek_field_app/src/app/core/components/header/header.component.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/core/components/status/status.component.html` & `peek-field-app-3.4.6/peek_field_app/src/app/core/components/status/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/core/components/status/status.component.ts` & `peek-field-app-3.4.6/peek_field_app/src/app/core/components/status/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/pages/config/config.page.html` & `peek-field-app-3.4.6/peek_field_app/src/app/pages/config/config.page.html`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/pages/config/config.page.ts` & `peek-field-app-3.4.6/peek_field_app/src/app/pages/config/config.page.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/pages/home/home.page.html` & `peek-field-app-3.4.6/peek_field_app/src/app/pages/home/home.page.html`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/pages/home/home.page.scss` & `peek-field-app-3.4.6/peek_field_app/src/app/pages/home/home.page.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/pages/home/home.page.ts` & `peek-field-app-3.4.6/peek_field_app/src/app/pages/home/home.page.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/pages/pages.module.ts` & `peek-field-app-3.4.6/peek_field_app/src/app/pages/pages.module.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/pages/unknown-route/unknown-route.page.html` & `peek-field-app-3.4.6/peek_field_app/src/app/pages/unknown-route/unknown-route.page.html`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/pages/unknown-route/unknown-route.page.scss` & `peek-field-app-3.4.6/peek_field_app/src/app/pages/unknown-route/unknown-route.page.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/app/pages/unknown-route/unknown-route.page.ts` & `peek-field-app-3.4.6/peek_field_app/src/app/pages/unknown-route/unknown-route.page.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/assets/Poppins-Medium.ttf` & `peek-field-app-3.4.6/peek_field_app/src/assets/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/assets/Poppins-Regular.ttf` & `peek-field-app-3.4.6/peek_field_app/src/assets/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/assets/Poppins-SemiBold.ttf` & `peek-field-app-3.4.6/peek_field_app/src/assets/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/assets/peek_core_docdb/icon.png` & `peek-field-app-3.4.6/peek_field_app/src/assets/peek_core_docdb/icon.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/assets/peek_core_search/icon.png` & `peek-field-app-3.4.6/peek_field_app/src/assets/peek_core_search/icon.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/assets/peek_core_user/plugin_icon.png` & `peek-field-app-3.4.6/peek_field_app/src/assets/peek_core_user/plugin_icon.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/favicon.ico` & `peek-field-app-3.4.6/peek_field_app/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/index.html` & `peek-field-app-3.4.6/peek_field_app/src/index.html`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/main.ts` & `peek-field-app-3.4.6/peek_field_app/src/main.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/polyfills.ts` & `peek-field-app-3.4.6/peek_field_app/src/polyfills.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/styles/shared.scss` & `peek-field-app-3.4.6/peek_field_app/src/styles/shared.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/styles/styles-layout.scss` & `peek-field-app-3.4.6/peek_field_app/src/styles/styles-layout.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/styles/theme.less` & `peek-field-app-3.4.6/peek_field_app/src/styles/theme.less`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/styles.scss` & `peek-field-app-3.4.6/peek_field_app/src/styles.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/test.ts` & `peek-field-app-3.4.6/peek_field_app/src/test.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app/src/tsconfig.app.json` & `peek-field-app-3.4.6/peek_field_app/src/tsconfig.app.json`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/peek_field_app.egg-info/SOURCES.txt` & `peek-field-app-3.4.6/peek_field_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.4.5/setup.py` & `peek-field-app-3.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_field_app"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Field UI App."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

