# Comparing `tmp/yt-dlp-cp-0.9.9.tar.gz` & `tmp/yt-dlp-cp-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yt-dlp-cp-0.9.9.tar", last modified: Tue Apr  4 07:25:26 2023, max compression
+gzip compressed data, was "dist\yt-dlp-cp-1.9.9.tar", last modified: Thu Jun 29 08:20:15 2023, max compression
```

## Comparing `yt-dlp-cp-0.9.9.tar` & `yt-dlp-cp-1.9.9.tar`

### file list

```diff
@@ -1,1234 +1,1234 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:26.354350 yt-dlp-cp-0.9.9/
--rw-rw-rw-   0        0        0   233121 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/Changelog.md
--rw-rw-rw-   0        0        0     1211 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/LICENSE
--rw-rw-rw-   0        0        0      219 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/MANIFEST.in
--rw-rw-rw-   0        0        0      165 2023-04-04 07:25:26.355357 yt-dlp-cp-0.9.9/PKG-INFO
--rw-rw-rw-   0        0        0   155243 2023-04-04 05:52:42.000000 yt-dlp-cp-0.9.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.308760 yt-dlp-cp-0.9.9/devscripts/
--rw-rw-rw-   0        0        0      147 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/SizeOfImage.patch
--rw-rw-rw-   0        0        0      148 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/SizeOfImage_w.patch
--rw-rw-rw-   0        0        0       78 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.309760 yt-dlp-cp-0.9.9/devscripts/__pycache__/
--rw-rw-rw-   0        0        0      135 2023-04-04 07:22:59.000000 yt-dlp-cp-0.9.9/devscripts/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     1929 2023-04-04 07:22:59.000000 yt-dlp-cp-0.9.9/devscripts/__pycache__/utils.cpython-38.pyc
--rw-rw-rw-   0        0        0      832 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/bash-completion.in
--rw-rw-rw-   0        0        0      891 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/devscripts/bash-completion.py
--rw-rw-rw-   0        0        0      942 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/changelog_override.json
--rw-rw-rw-   0        0        0     2914 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/changelog_override.schema.json
--rw-rw-rw-   0        0        0     1801 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/check-porn.py
--rw-rw-rw-   0        0        0      126 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/fish-completion.in
--rw-rw-rw-   0        0        0     1731 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/devscripts/fish-completion.py
--rw-rw-rw-   0        0        0     1191 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/devscripts/generate_aes_testdata.py
--rw-rw-rw-   0        0        0     1228 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/lazy_load_template.py
--rw-rw-rw-   0        0        0    41043 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/logo.ico
--rw-rw-rw-   0        0        0    17117 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/make_changelog.py
--rw-rw-rw-   0        0        0      763 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/make_contributing.py
--rw-rw-rw-   0        0        0     2758 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/make_issue_template.py
--rw-rw-rw-   0        0        0     4688 2023-04-04 05:52:42.000000 yt-dlp-cp-0.9.9/devscripts/make_lazy_extractors.py
--rw-rw-rw-   0        0        0     2892 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/make_readme.py
--rw-rw-rw-   0        0        0      508 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/devscripts/make_supportedsites.py
--rw-rw-rw-   0        0        0     2877 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/prepare_manpage.py
--rwxrwxrwx   0        0        0      343 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/run_tests.bat
--rw-rw-rw-   0        0        0      305 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/run_tests.sh
--rw-rw-rw-   0        0        0      987 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/devscripts/set-variant.py
--rw-rw-rw-   0        0        0     1074 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/update-formulae.py
--rw-rw-rw-   0        0        0     2061 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/devscripts/update-version.py
--rw-rw-rw-   0        0        0     1375 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/devscripts/utils.py
--rw-rw-rw-   0        0        0      864 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/devscripts/zsh-completion.in
--rw-rw-rw-   0        0        0     1437 2023-04-04 05:52:42.000000 yt-dlp-cp-0.9.9/devscripts/zsh-completion.py
--rw-rw-rw-   0        0        0      179 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/pyproject.toml
--rw-rw-rw-   0        0        0      145 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/requirements.txt
--rw-rw-rw-   0        0        0      974 2023-04-04 07:25:26.356363 yt-dlp-cp-0.9.9/setup.cfg
--rw-rw-rw-   0        0        0     4657 2023-04-04 07:25:14.000000 yt-dlp-cp-0.9.9/setup.py
--rw-rw-rw-   0        0        0    50029 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/supportedsites.md
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.341761 yt-dlp-cp-0.9.9/test/
--rw-rw-rw-   0        0        0        0 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/__init__.py
--rw-rw-rw-   0        0        0    12506 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/helper.py
--rw-rw-rw-   0        0        0     1239 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/parameters.json
--rw-rw-rw-   0        0        0   103895 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_InfoExtractor.py
--rw-rw-rw-   0        0        0    51120 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_YoutubeDL.py
--rw-rw-rw-   0        0        0     1952 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_YoutubeDLCookieJar.py
--rw-rw-rw-   0        0        0     7023 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_aes.py
--rw-rw-rw-   0        0        0     1536 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_age_restriction.py
--rw-rw-rw-   0        0        0     6245 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_all_urls.py
--rw-rw-rw-   0        0        0     1576 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_cache.py
--rw-rw-rw-   0        0        0     4759 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_compat.py
--rw-rw-rw-   0        0        0     6960 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_config.py
--rw-rw-rw-   0        0        0    13436 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_cookies.py
--rw-rw-rw-   0        0        0    11851 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_download.py
--rw-rw-rw-   0        0        0     3516 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_downloader_http.py
--rw-rw-rw-   0        0        0     1908 2023-04-04 05:52:42.000000 yt-dlp-cp-0.9.9/test/test_execution.py
--rw-rw-rw-   0        0        0     7315 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_http.py
--rw-rw-rw-   0        0        0     1042 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_iqiyi_sdk_interpreter.py
--rw-rw-rw-   0        0        0    15661 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_jsinterp.py
--rw-rw-rw-   0        0        0      746 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_netrc.py
--rw-rw-rw-   0        0        0     1813 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_overwrites.py
--rw-rw-rw-   0        0        0     2842 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_plugins.py
--rw-rw-rw-   0        0        0     2101 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_post_hooks.py
--rw-rw-rw-   0        0        0    31130 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_postprocessors.py
--rw-rw-rw-   0        0        0     3363 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/test_socks.py
--rw-rw-rw-   0        0        0    17852 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_subtitles.py
--rw-rw-rw-   0        0        0     1093 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_update.py.disabled
--rw-rw-rw-   0        0        0   113432 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_utils.py
--rw-rw-rw-   0        0        0     2791 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_verbose_output.py
--rw-rw-rw-   0        0        0     2569 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_write_annotations.py.disabled
--rw-rw-rw-   0        0        0     2817 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_youtube_lists.py
--rw-rw-rw-   0        0        0      993 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_youtube_misc.py
--rw-rw-rw-   0        0        0     9070 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/test_youtube_signature.py
--rw-rw-rw-   0        0        0     3176 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testcert.pem
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.271311 yt-dlp-cp-0.9.9/test/testdata/
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.348925 yt-dlp-cp-0.9.9/test/testdata/certificate/
--rw-rw-rw-   0        0        0      574 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/certificate/ca.crt
--rw-rw-rw-   0        0        0      227 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/certificate/ca.key
--rw-rw-rw-   0        0        0       41 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/certificate/ca.srl
--rw-rw-rw-   0        0        0      457 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/certificate/client.crt
--rw-rw-rw-   0        0        0      359 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/certificate/client.csr
--rw-rw-rw-   0        0        0      227 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/certificate/client.key
--rw-rw-rw-   0        0        0      314 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/certificate/clientencrypted.key
--rw-rw-rw-   0        0        0      771 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/certificate/clientwithencryptedkey.crt
--rw-rw-rw-   0        0        0      684 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/certificate/clientwithkey.crt
--rw-rw-rw-   0        0        0      727 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/certificate/instructions.md
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.352644 yt-dlp-cp-0.9.9/test/testdata/cookies/
--rw-rw-rw-   0        0        0      294 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/cookies/httponly_cookies.txt
--rw-rw-rw-   0        0        0      336 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/cookies/malformed_cookies.txt
--rw-rw-rw-   0        0        0      269 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/cookies/session_cookies.txt
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.354690 yt-dlp-cp-0.9.9/test/testdata/f4m/
--rw-rw-rw-   0        0        0      994 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/f4m/custom_base_url.f4m
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.357711 yt-dlp-cp-0.9.9/test/testdata/ism/
--rw-rw-rw-   0        0        0     3987 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/ism/ec-3_test.Manifest
--rw-rw-rw-   0        0        0    23179 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/ism/sintel.Manifest
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.358730 yt-dlp-cp-0.9.9/test/testdata/m3u8/
--rw-rw-rw-   0        0        0     3286 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/m3u8/bipbop_16x9.m3u8
--rw-rw-rw-   0        0        0     6291 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.362723 yt-dlp-cp-0.9.9/test/testdata/mpd/
--rw-rw-rw-   0        0        0     1715 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/mpd/float_duration.mpd
--rw-rw-rw-   0        0        0    10268 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/mpd/subtitles.mpd
--rw-rw-rw-   0        0        0     1744 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/mpd/unfragmented.mpd
--rw-rw-rw-   0        0        0    22374 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/mpd/urls_only.mpd
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.257632 yt-dlp-cp-0.9.9/test/testdata/thumbnails/
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.363726 yt-dlp-cp-0.9.9/test/testdata/thumbnails/foo %d bar/
--rw-rw-rw-   0        0        0     3928 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/thumbnails/foo %d bar/foo_%d.webp
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.363726 yt-dlp-cp-0.9.9/test/testdata/xspf/
--rw-rw-rw-   0        0        0     1385 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/testdata/xspf/foo_xspf.xspf
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.270317 yt-dlp-cp-0.9.9/test/testdata/yt_dlp_plugins/
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.366726 yt-dlp-cp-0.9.9/test/testdata/yt_dlp_plugins/extractor/
--rw-rw-rw-   0        0        0      106 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/testdata/yt_dlp_plugins/extractor/_ignore.py
--rw-rw-rw-   0        0        0      198 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/testdata/yt_dlp_plugins/extractor/ignore.py
--rw-rw-rw-   0        0        0      169 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/testdata/yt_dlp_plugins/extractor/normal.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.367661 yt-dlp-cp-0.9.9/test/testdata/yt_dlp_plugins/postprocessor/
--rw-rw-rw-   0        0        0      110 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/testdata/yt_dlp_plugins/postprocessor/normal.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.271311 yt-dlp-cp-0.9.9/test/testdata/zipped_plugins/
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.273314 yt-dlp-cp-0.9.9/test/testdata/zipped_plugins/yt_dlp_plugins/
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.368671 yt-dlp-cp-0.9.9/test/testdata/zipped_plugins/yt_dlp_plugins/extractor/
--rw-rw-rw-   0        0        0      106 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/testdata/zipped_plugins/yt_dlp_plugins/extractor/zipped.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.369661 yt-dlp-cp-0.9.9/test/testdata/zipped_plugins/yt_dlp_plugins/postprocessor/
--rw-rw-rw-   0        0        0      110 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/test/testdata/zipped_plugins/yt_dlp_plugins/postprocessor/zipped.py
--rw-rw-rw-   0        0        0     1608 2023-03-23 04:28:30.000000 yt-dlp-cp-0.9.9/test/versions.json
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.386695 yt-dlp-cp-0.9.9/yt_dlp_cp/
--rw-rw-rw-   0        0        0   199549 2023-04-04 05:54:28.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/YoutubeDL.py
--rw-rw-rw-   0        0        0    44156 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/__init__.py
--rw-rw-rw-   0        0        0      392 2023-04-04 06:43:59.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.394734 yt-dlp-cp-0.9.9/yt_dlp_cp/__pyinstaller/
--rw-rw-rw-   0        0        0       77 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      942 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/__pyinstaller/hook-yt_dlp.py
--rw-rw-rw-   0        0        0    22969 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/aes.py
--rw-rw-rw-   0        0        0     3465 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.400715 yt-dlp-cp-0.9.9/yt_dlp_cp/compat/
--rw-rw-rw-   0        0        0     2404 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/compat/__init__.py
--rw-rw-rw-   0        0        0      446 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/compat/_deprecated.py
--rw-rw-rw-   0        0        0     4011 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/compat/_legacy.py
--rw-rw-rw-   0        0        0     2660 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/compat/compat_utils.py
--rw-rw-rw-   0        0        0      690 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/compat/functools.py
--rw-rw-rw-   0        0        0      588 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/compat/imghdr.py
--rw-rw-rw-   0        0        0      889 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/compat/shutil.py
--rw-rw-rw-   0        0        0    44722 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/cookies.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.402651 yt-dlp-cp-0.9.9/yt_dlp_cp/dependencies/
--rw-rw-rw-   0        0        0     1450 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/dependencies/Cryptodome.py
--rw-rw-rw-   0        0        0     2061 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/dependencies/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.416651 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/
--rw-rw-rw-   0        0        0     4574 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/__init__.py
--rw-rw-rw-   0        0        0    19115 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/common.py
--rw-rw-rw-   0        0        0     3593 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/dash.py
--rw-rw-rw-   0        0        0    26627 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/external.py
--rw-rw-rw-   0        0        0    15759 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/f4m.py
--rw-rw-rw-   0        0        0     1370 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/fc2.py
--rw-rw-rw-   0        0        0    22680 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/fragment.py
--rw-rw-rw-   0        0        0    17396 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/hls.py
--rw-rw-rw-   0        0        0    17601 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/http.py
--rw-rw-rw-   0        0        0    11914 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/ism.py
--rw-rw-rw-   0        0        0     6371 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/mhtml.py
--rw-rw-rw-   0        0        0     1974 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/niconico.py
--rw-rw-rw-   0        0        0     9136 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/rtmp.py
--rw-rw-rw-   0        0        0     1551 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/rtsp.py
--rw-rw-rw-   0        0        0     1825 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/websocket.py
--rw-rw-rw-   0        0        0    11143 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/youtube_live_chat.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:26.343491 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/
--rw-rw-rw-   0        0        0     1395 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/__init__.py
--rw-rw-rw-   0        0        0    54810 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/_extractors.py
--rw-rw-rw-   0        0        0    13048 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/abc.py
--rw-rw-rw-   0        0        0     6481 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/abcnews.py
--rw-rw-rw-   0        0        0     4726 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/abcotvs.py
--rw-rw-rw-   0        0        0    21334 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/abematv.py
--rw-rw-rw-   0        0        0     1397 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/academicearth.py
--rw-rw-rw-   0        0        0     4542 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/acast.py
--rw-rw-rw-   0        0        0     8111 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/acfun.py
--rw-rw-rw-   0        0        0    11154 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/adn.py
--rw-rw-rw-   0        0        0     1252 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/adobeconnect.py
--rw-rw-rw-   0        0        0    54460 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/adobepass.py
--rw-rw-rw-   0        0        0    10563 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/adobetv.py
--rw-rw-rw-   0        0        0     7927 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/adultswim.py
--rw-rw-rw-   0        0        0    12422 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aenetworks.py
--rw-rw-rw-   0        0        0     1845 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aeonco.py
--rw-rw-rw-   0        0        0    22211 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/afreecatv.py
--rw-rw-rw-   0        0        0    10072 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/agora.py
--rw-rw-rw-   0        0        0     2703 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/airmozilla.py
--rw-rw-rw-   0        0        0     4181 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/airtv.py
--rw-rw-rw-   0        0        0     3016 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aitube.py
--rw-rw-rw-   0        0        0     1576 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aliexpress.py
--rw-rw-rw-   0        0        0     3447 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aljazeera.py
--rw-rw-rw-   0        0        0     4928 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/allocine.py
--rw-rw-rw-   0        0        0     2758 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/alphaporno.py
--rw-rw-rw-   0        0        0     3163 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/alsace20tv.py
--rw-rw-rw-   0        0        0     6668 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/alura.py
--rw-rw-rw-   0        0        0     3626 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/amara.py
--rw-rw-rw-   0        0        0     6759 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/amazon.py
--rw-rw-rw-   0        0        0    10904 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/amazonminitv.py
--rw-rw-rw-   0        0        0     6267 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/amcnetworks.py
--rw-rw-rw-   0        0        0     8939 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/americastestkitchen.py
--rw-rw-rw-   0        0        0     4166 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/amp.py
--rw-rw-rw-   0        0        0     4898 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/anchorfm.py
--rw-rw-rw-   0        0        0     2606 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/angel.py
--rw-rw-rw-   0        0        0     5414 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ant1newsgr.py
--rw-rw-rw-   0        0        0    27555 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/anvato.py
--rw-rw-rw-   0        0        0     5578 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aol.py
--rw-rw-rw-   0        0        0     3169 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/apa.py
--rw-rw-rw-   0        0        0     3462 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aparat.py
--rw-rw-rw-   0        0        0     1902 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/appleconnect.py
--rw-rw-rw-   0        0        0     3709 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/applepodcasts.py
--rw-rw-rw-   0        0        0    10474 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/appletrailers.py
--rw-rw-rw-   0        0        0    58664 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/archiveorg.py
--rw-rw-rw-   0        0        0     7678 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/arcpublishing.py
--rw-rw-rw-   0        0        0    28271 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ard.py
--rw-rw-rw-   0        0        0     7349 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/arkena.py
--rw-rw-rw-   0        0        0     3654 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/arnes.py
--rw-rw-rw-   0        0        0    14310 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/arte.py
--rw-rw-rw-   0        0        0     7878 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/asiancrush.py
--rw-rw-rw-   0        0        0     4241 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/atresplayer.py
--rw-rw-rw-   0        0        0     1246 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/atscaleconf.py
--rw-rw-rw-   0        0        0     1974 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/atttechchannel.py
--rw-rw-rw-   0        0        0     4299 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/atvat.py
--rw-rw-rw-   0        0        0     4018 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/audimedia.py
--rw-rw-rw-   0        0        0     2923 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/audioboom.py
--rw-rw-rw-   0        0        0     3306 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/audiodraft.py
--rw-rw-rw-   0        0        0     6328 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/audiomack.py
--rw-rw-rw-   0        0        0    11044 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/audius.py
--rw-rw-rw-   0        0        0     7317 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/awaan.py
--rw-rw-rw-   0        0        0     3184 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aws.py
--rw-rw-rw-   0        0        0     2490 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/azmedien.py
--rw-rw-rw-   0        0        0     1959 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/baidu.py
--rw-rw-rw-   0        0        0     5459 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/banbye.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bandaichannel.py
--rw-rw-rw-   0        0        0    19082 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bandcamp.py
--rw-rw-rw-   0        0        0     5458 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bannedvideo.py
--rw-rw-rw-   0        0        0    73490 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bbc.py
--rw-rw-rw-   0        0        0     4303 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/beatbump.py
--rw-rw-rw-   0        0        0     3343 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/beatport.py
--rw-rw-rw-   0        0        0     3235 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/beeg.py
--rw-rw-rw-   0        0        0     1616 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/behindkink.py
--rw-rw-rw-   0        0        0     3353 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bellmedia.py
--rw-rw-rw-   0        0        0     3171 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/berufetv.py
--rw-rw-rw-   0        0        0     2861 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bet.py
--rw-rw-rw-   0        0        0     1318 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bfi.py
--rw-rw-rw-   0        0        0     5451 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bfmtv.py
--rw-rw-rw-   0        0        0     1072 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bibeltv.py
--rw-rw-rw-   0        0        0     2313 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bigflix.py
--rw-rw-rw-   0        0        0     2021 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bigo.py
--rw-rw-rw-   0        0        0     1343 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bild.py
--rw-rw-rw-   0        0        0    52181 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bilibili.py
--rw-rw-rw-   0        0        0     3537 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/biobiochiletv.py
--rw-rw-rw-   0        0        0     4832 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/biqle.py
--rw-rw-rw-   0        0        0     9846 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bitchute.py
--rw-rw-rw-   0        0        0     1827 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bitwave.py
--rw-rw-rw-   0        0        0     2419 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/blackboardcollaborate.py
--rw-rw-rw-   0        0        0     4422 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bleacherreport.py
--rw-rw-rw-   0        0        0     4900 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/blerp.py
--rw-rw-rw-   0        0        0     1886 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/blogger.py
--rw-rw-rw-   0        0        0     3257 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bloomberg.py
--rw-rw-rw-   0        0        0     1999 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bokecc.py
--rw-rw-rw-   0        0        0     2339 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bongacams.py
--rw-rw-rw-   0        0        0     3890 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/booyah.py
--rw-rw-rw-   0        0        0     3204 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bostonglobe.py
--rw-rw-rw-   0        0        0     3779 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/box.py
--rw-rw-rw-   0        0        0     4858 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/boxcast.py
--rw-rw-rw-   0        0        0     2070 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bpb.py
--rw-rw-rw-   0        0        0    12183 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/br.py
--rw-rw-rw-   0        0        0     8252 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bravotv.py
--rw-rw-rw-   0        0        0     2944 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/breakcom.py
--rw-rw-rw-   0        0        0     1377 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/breitbart.py
--rw-rw-rw-   0        0        0    43629 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/brightcove.py
--rw-rw-rw-   0        0        0     1377 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bundesliga.py
--rw-rw-rw-   0        0        0     1986 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/businessinsider.py
--rw-rw-rw-   0        0        0     3704 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/buzzfeed.py
--rw-rw-rw-   0        0        0     4523 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/byutv.py
--rw-rw-rw-   0        0        0     2016 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/c56.py
--rw-rw-rw-   0        0        0     1155 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cableav.py
--rw-rw-rw-   0        0        0     8278 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/callin.py
--rw-rw-rw-   0        0        0     1599 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/caltrans.py
--rw-rw-rw-   0        0        0     1146 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cam4.py
--rw-rw-rw-   0        0        0     5873 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/camdemy.py
--rw-rw-rw-   0        0        0     2903 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cammodels.py
--rw-rw-rw-   0        0        0     2240 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/camsoda.py
--rw-rw-rw-   0        0        0     2546 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/camtasia.py
--rw-rw-rw-   0        0        0     3275 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/camwithher.py
--rw-rw-rw-   0        0        0     4363 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/canalalpha.py
--rw-rw-rw-   0        0        0     2283 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/canalc2.py
--rw-rw-rw-   0        0        0     4473 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/canalplus.py
--rw-rw-rw-   0        0        0    16095 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/canvas.py
--rw-rw-rw-   0        0        0     3538 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/carambatv.py
--rw-rw-rw-   0        0        0     2376 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cartoonnetwork.py
--rw-rw-rw-   0        0        0    22613 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbc.py
--rw-rw-rw-   0        0        0    12044 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbs.py
--rw-rw-rw-   0        0        0     4111 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbsinteractive.py
--rw-rw-rw-   0        0        0     4258 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbslocal.py
--rw-rw-rw-   0        0        0     7765 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbsnews.py
--rw-rw-rw-   0        0        0     4928 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbssports.py
--rw-rw-rw-   0        0        0     3959 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ccc.py
--rw-rw-rw-   0        0        0     5250 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ccma.py
--rw-rw-rw-   0        0        0     7034 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cctv.py
--rw-rw-rw-   0        0        0    14224 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cda.py
--rw-rw-rw-   0        0        0     2900 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cellebrite.py
--rw-rw-rw-   0        0        0    12005 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ceskatelevize.py
--rw-rw-rw-   0        0        0     2898 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cgtn.py
--rw-rw-rw-   0        0        0    10347 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/channel9.py
--rw-rw-rw-   0        0        0     1792 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/charlierose.py
--rw-rw-rw-   0        0        0     3922 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/chaturbate.py
--rw-rw-rw-   0        0        0     4945 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/chilloutzone.py
--rw-rw-rw-   0        0        0     8871 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/chingari.py
--rw-rw-rw-   0        0        0     2977 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/chirbit.py
--rw-rw-rw-   0        0        0     2056 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cinchcast.py
--rw-rw-rw-   0        0        0      901 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cinemax.py
--rw-rw-rw-   0        0        0     2487 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cinetecamilano.py
--rw-rw-rw-   0        0        0     6003 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ciscolive.py
--rw-rw-rw-   0        0        0     4543 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ciscowebex.py
--rw-rw-rw-   0        0        0     2407 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cjsw.py
--rw-rw-rw-   0        0        0     2532 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cliphunter.py
--rw-rw-rw-   0        0        0     2563 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/clippit.py
--rw-rw-rw-   0        0        0     1003 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cliprs.py
--rw-rw-rw-   0        0        0     1823 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/clipsyndicate.py
--rw-rw-rw-   0        0        0     3083 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/closertotruth.py
--rw-rw-rw-   0        0        0     2441 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cloudflarestream.py
--rw-rw-rw-   0        0        0     1898 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cloudy.py
--rw-rw-rw-   0        0        0     1935 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/clubic.py
--rw-rw-rw-   0        0        0     3182 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/clyp.py
--rw-rw-rw-   0        0        0     2276 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cmt.py
--rw-rw-rw-   0        0        0     2287 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cnbc.py
--rw-rw-rw-   0        0        0     9369 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cnn.py
--rw-rw-rw-   0        0        0     2196 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/comedycentral.py
--rw-rw-rw-   0        0        0   188391 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/common.py
--rw-rw-rw-   0        0        0     1306 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/commonmistakes.py
--rw-rw-rw-   0        0        0     2006 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/commonprotocols.py
--rw-rw-rw-   0        0        0     9980 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/condenast.py
--rw-rw-rw-   0        0        0     4215 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/contv.py
--rw-rw-rw-   0        0        0     6413 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/corus.py
--rw-rw-rw-   0        0        0     4695 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/coub.py
--rw-rw-rw-   0        0        0     1409 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cozytv.py
--rw-rw-rw-   0        0        0     5837 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cpac.py
--rw-rw-rw-   0        0        0     3185 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cracked.py
--rw-rw-rw-   0        0        0     9921 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/crackle.py
--rw-rw-rw-   0        0        0     2805 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/craftsy.py
--rw-rw-rw-   0        0        0     2179 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/crooksandliars.py
--rw-rw-rw-   0        0        0     4271 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/crowdbunker.py
--rw-rw-rw-   0        0        0    15216 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/crunchyroll.py
--rw-rw-rw-   0        0        0    12391 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cspan.py
--rw-rw-rw-   0        0        0     3675 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ctsnews.py
--rw-rw-rw-   0        0        0     1764 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ctv.py
--rw-rw-rw-   0        0        0     2624 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ctvnews.py
--rw-rw-rw-   0        0        0     2520 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cultureunplugged.py
--rw-rw-rw-   0        0        0     8594 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/curiositystream.py
--rw-rw-rw-   0        0        0     3937 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cwtv.py
--rw-rw-rw-   0        0        0     6438 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cybrary.py
--rw-rw-rw-   0        0        0     5960 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/daftsex.py
--rw-rw-rw-   0        0        0     3016 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dailymail.py
--rw-rw-rw-   0        0        0    16331 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dailymotion.py
--rw-rw-rw-   0        0        0     4967 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dailywire.py
--rw-rw-rw-   0        0        0     5642 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/damtomo.py
--rw-rw-rw-   0        0        0     9679 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/daum.py
--rw-rw-rw-   0        0        0     2035 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/daystar.py
--rw-rw-rw-   0        0        0     1826 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dbtv.py
--rw-rw-rw-   0        0        0     3633 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dctp.py
--rw-rw-rw-   0        0        0     5296 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/deezer.py
--rw-rw-rw-   0        0        0     1238 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/defense.py
--rw-rw-rw-   0        0        0     3098 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/democracynow.py
--rw-rw-rw-   0        0        0     8247 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/detik.py
--rw-rw-rw-   0        0        0     3271 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/deuxm.py
--rw-rw-rw-   0        0        0     2215 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dfb.py
--rw-rw-rw-   0        0        0     2107 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dhm.py
--rw-rw-rw-   0        0        0     1895 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/digg.py
--rw-rw-rw-   0        0        0     5837 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/digitalconcerthall.py
--rw-rw-rw-   0        0        0     3355 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/digiteka.py
--rw-rw-rw-   0        0        0     4958 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/discovery.py
--rw-rw-rw-   0        0        0     6174 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/discoverygo.py
--rw-rw-rw-   0        0        0     6930 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/disney.py
--rw-rw-rw-   0        0        0     5073 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dispeak.py
--rw-rw-rw-   0        0        0     3068 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dlive.py
--rw-rw-rw-   0        0        0     3119 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dotsub.py
--rw-rw-rw-   0        0        0     7417 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/douyutv.py
--rw-rw-rw-   0        0        0    39956 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dplay.py
--rw-rw-rw-   0        0        0     1935 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/drbonanza.py
--rw-rw-rw-   0        0        0     1655 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dreisat.py
--rw-rw-rw-   0        0        0     4300 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/drooble.py
--rw-rw-rw-   0        0        0     3406 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dropbox.py
--rw-rw-rw-   0        0        0     9856 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dropout.py
--rw-rw-rw-   0        0        0     3900 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/drtuber.py
--rw-rw-rw-   0        0        0    20606 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/drtv.py
--rw-rw-rw-   0        0        0     2806 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dtube.py
--rw-rw-rw-   0        0        0     8510 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/duboku.py
--rw-rw-rw-   0        0        0     2684 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dumpert.py
--rw-rw-rw-   0        0        0     7612 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dvtv.py
--rw-rw-rw-   0        0        0     4112 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dw.py
--rw-rw-rw-   0        0        0     8399 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eagleplatform.py
--rw-rw-rw-   0        0        0     1076 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ebaumsworld.py
--rw-rw-rw-   0        0        0     1308 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ebay.py
--rw-rw-rw-   0        0        0     1303 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/echomsk.py
--rw-rw-rw-   0        0        0     5070 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/egghead.py
--rw-rw-rw-   0        0        0     1513 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ehow.py
--rw-rw-rw-   0        0        0     5972 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eighttracks.py
--rw-rw-rw-   0        0        0     3717 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/einthusan.py
--rw-rw-rw-   0        0        0     3267 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eitb.py
--rw-rw-rw-   0        0        0     5007 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ellentube.py
--rw-rw-rw-   0        0        0     2649 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/elonet.py
--rw-rw-rw-   0        0        0     4399 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/elpais.py
--rw-rw-rw-   0        0        0     5413 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/embedly.py
--rw-rw-rw-   0        0        0      453 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/engadget.py
--rw-rw-rw-   0        0        0     4310 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/epicon.py
--rw-rw-rw-   0        0        0     2568 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/epoch.py
--rw-rw-rw-   0        0        0     4688 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eporner.py
--rw-rw-rw-   0        0        0     4589 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eroprofile.py
--rw-rw-rw-   0        0        0    12922 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ertgr.py
--rw-rw-rw-   0        0        0     3653 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/escapist.py
--rw-rw-rw-   0        0        0    17639 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/espn.py
--rw-rw-rw-   0        0        0     2605 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/esri.py
--rw-rw-rw-   0        0        0     6610 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/europa.py
--rw-rw-rw-   0        0        0     1299 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/europeantour.py
--rw-rw-rw-   0        0        0     5181 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eurosport.py
--rw-rw-rw-   0        0        0     3385 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/euscreen.py
--rw-rw-rw-   0        0        0     2910 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/expotv.py
--rw-rw-rw-   0        0        0     3837 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/expressen.py
--rw-rw-rw-   0        0        0      870 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/extractors.py
--rw-rw-rw-   0        0        0     1795 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/extremetube.py
--rw-rw-rw-   0        0        0     2691 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eyedotv.py
--rw-rw-rw-   0        0        0    36232 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/facebook.py
--rw-rw-rw-   0        0        0     7355 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fancode.py
--rw-rw-rw-   0        0        0     3582 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/faz.py
--rw-rw-rw-   0        0        0    11256 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fc2.py
--rw-rw-rw-   0        0        0     1717 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fczenit.py
--rw-rw-rw-   0        0        0     3926 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fifa.py
--rw-rw-rw-   0        0        0     2623 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/filmmodu.py
--rw-rw-rw-   0        0        0     6053 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/filmon.py
--rw-rw-rw-   0        0        0     1461 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/filmweb.py
--rw-rw-rw-   0        0        0     6513 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/firsttv.py
--rw-rw-rw-   0        0        0     3130 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fivetv.py
--rw-rw-rw-   0        0        0     4815 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/flickr.py
--rw-rw-rw-   0        0        0     2623 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/folketinget.py
--rw-rw-rw-   0        0        0     1871 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/footyroom.py
--rw-rw-rw-   0        0        0      962 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/formula1.py
--rw-rw-rw-   0        0        0    11807 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fourtube.py
--rw-rw-rw-   0        0        0     4988 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fourzerostudio.py
--rw-rw-rw-   0        0        0     6800 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fox.py
--rw-rw-rw-   0        0        0     1447 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fox9.py
--rw-rw-rw-   0        0        0     2123 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/foxgay.py
--rw-rw-rw-   0        0        0     6309 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/foxnews.py
--rw-rw-rw-   0        0        0     2263 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/foxsports.py
--rw-rw-rw-   0        0        0     4965 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fptplay.py
--rw-rw-rw-   0        0        0     2214 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/franceinter.py
--rw-rw-rw-   0        0        0    15517 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/francetv.py
--rw-rw-rw-   0        0        0     2581 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/freesound.py
--rw-rw-rw-   0        0        0     1045 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/freespeech.py
--rw-rw-rw-   0        0        0     5668 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/freetv.py
--rw-rw-rw-   0        0        0     8849 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/frontendmasters.py
--rw-rw-rw-   0        0        0     3205 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fujitv.py
--rw-rw-rw-   0        0        0    15291 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/funimation.py
--rw-rw-rw-   0        0        0     1691 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/funk.py
--rw-rw-rw-   0        0        0     3168 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fusion.py
--rw-rw-rw-   0        0        0     1041 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fuyintv.py
--rw-rw-rw-   0        0        0     5849 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gab.py
--rw-rw-rw-   0        0        0     4626 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gaia.py
--rw-rw-rw-   0        0        0     2111 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gameinformer.py
--rw-rw-rw-   0        0        0    25720 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gamejolt.py
--rw-rw-rw-   0        0        0     3153 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gamespot.py
--rw-rw-rw-   0        0        0     2612 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gamestar.py
--rw-rw-rw-   0        0        0     3838 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gaskrank.py
--rw-rw-rw-   0        0        0     1926 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gazeta.py
--rw-rw-rw-   0        0        0     8769 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gdcvault.py
--rw-rw-rw-   0        0        0     8720 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gedidigital.py
--rw-rw-rw-   0        0        0   122559 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/generic.py
--rw-rw-rw-   0        0        0     4722 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/genericembeds.py
--rw-rw-rw-   0        0        0     6248 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/genius.py
--rw-rw-rw-   0        0        0     8051 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gettr.py
--rw-rw-rw-   0        0        0     5254 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gfycat.py
--rw-rw-rw-   0        0        0     3049 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/giantbomb.py
--rw-rw-rw-   0        0        0     3815 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/giga.py
--rw-rw-rw-   0        0        0      656 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gigya.py
--rw-rw-rw-   0        0        0     1417 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/glide.py
--rw-rw-rw-   0        0        0    10366 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/globo.py
--rw-rw-rw-   0        0        0     8733 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/glomex.py
--rw-rw-rw-   0        0        0    14476 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/go.py
--rw-rw-rw-   0        0        0     1784 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/godtube.py
--rw-rw-rw-   0        0        0     3627 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gofile.py
--rw-rw-rw-   0        0        0     2184 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/golem.py
--rw-rw-rw-   0        0        0     2368 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/goodgame.py
--rw-rw-rw-   0        0        0    14873 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/googledrive.py
--rw-rw-rw-   0        0        0     3425 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/googlepodcasts.py
--rw-rw-rw-   0        0        0     1201 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/googlesearch.py
--rw-rw-rw-   0        0        0    15803 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/goplay.py
--rw-rw-rw-   0        0        0     3891 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gopro.py
--rw-rw-rw-   0        0        0     1533 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/goshgay.py
--rw-rw-rw-   0        0        0     2797 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gotostage.py
--rw-rw-rw-   0        0        0     1176 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gputechconf.py
--rw-rw-rw-   0        0        0     4057 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gronkh.py
--rw-rw-rw-   0        0        0     2623 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/groupon.py
--rw-rw-rw-   0        0        0     2930 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/harpodeon.py
--rw-rw-rw-   0        0        0     6206 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hbo.py
--rw-rw-rw-   0        0        0     3585 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hearthisat.py
--rw-rw-rw-   0        0        0     8639 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/heise.py
--rw-rw-rw-   0        0        0     2655 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hellporno.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/helsinki.py
--rw-rw-rw-   0        0        0     1197 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hentaistigma.py
--rw-rw-rw-   0        0        0     1415 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hgtv.py
--rw-rw-rw-   0        0        0     5064 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hidive.py
--rw-rw-rw-   0        0        0     1585 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/historicfilms.py
--rw-rw-rw-   0        0        0     7533 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hitbox.py
--rw-rw-rw-   0        0        0     2294 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hitrecord.py
--rw-rw-rw-   0        0        0     7059 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hketv.py
--rw-rw-rw-   0        0        0     2943 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hollywoodreporter.py
--rw-rw-rw-   0        0        0     4367 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/holodex.py
--rw-rw-rw-   0        0        0     2306 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hotnewhiphop.py
--rw-rw-rw-   0        0        0    15404 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hotstar.py
--rw-rw-rw-   0        0        0     1370 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/howcast.py
--rw-rw-rw-   0        0        0     3473 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/howstuffworks.py
--rw-rw-rw-   0        0        0     3935 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hrfensehen.py
--rw-rw-rw-   0        0        0     7237 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hrti.py
--rw-rw-rw-   0        0        0     3693 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hse.py
--rw-rw-rw-   0        0        0     1846 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/huajiao.py
--rw-rw-rw-   0        0        0     3387 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/huffpost.py
--rw-rw-rw-   0        0        0     5353 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hungama.py
--rw-rw-rw-   0        0        0     4996 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/huya.py
--rw-rw-rw-   0        0        0     1557 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hypem.py
--rw-rw-rw-   0        0        0     1249 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hypergryph.py
--rw-rw-rw-   0        0        0     2257 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hytale.py
--rw-rw-rw-   0        0        0     7570 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/icareus.py
--rw-rw-rw-   0        0        0     5947 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ichinanalive.py
--rw-rw-rw-   0        0        0    16931 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ign.py
--rw-rw-rw-   0        0        0     3502 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/iheart.py
--rw-rw-rw-   0        0        0     2380 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/iltalehti.py
--rw-rw-rw-   0        0        0     5780 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/imdb.py
--rw-rw-rw-   0        0        0     4942 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/imggaming.py
--rw-rw-rw-   0        0        0     5217 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/imgur.py
--rw-rw-rw-   0        0        0     3701 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ina.py
--rw-rw-rw-   0        0        0     2315 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/inc.py
--rw-rw-rw-   0        0        0     4335 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/indavideo.py
--rw-rw-rw-   0        0        0     5248 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/infoq.py
--rw-rw-rw-   0        0        0    31463 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/instagram.py
--rw-rw-rw-   0        0        0     3178 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/internazionale.py
--rw-rw-rw-   0        0        0     2319 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/internetvideoarchive.py
--rw-rw-rw-   0        0        0    10848 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/iprima.py
--rw-rw-rw-   0        0        0    31574 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/iqiyi.py
--rw-rw-rw-   0        0        0     3258 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/islamchannel.py
--rw-rw-rw-   0        0        0     2209 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/israelnationalnews.py
--rw-rw-rw-   0        0        0     5477 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/itprotv.py
--rw-rw-rw-   0        0        0    10948 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/itv.py
--rw-rw-rw-   0        0        0    10305 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ivi.py
--rw-rw-rw-   0        0        0     3205 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ivideon.py
--rw-rw-rw-   0        0        0     7062 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/iwara.py
--rw-rw-rw-   0        0        0     3509 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ixigua.py
--rw-rw-rw-   0        0        0     4172 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/izlesene.py
--rw-rw-rw-   0        0        0     4108 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jable.py
--rw-rw-rw-   0        0        0     8112 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jamendo.py
--rw-rw-rw-   0        0        0    10625 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/japandiet.py
--rw-rw-rw-   0        0        0     2018 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jeuxvideo.py
--rw-rw-rw-   0        0        0     2245 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jixie.py
--rw-rw-rw-   0        0        0     3973 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/joj.py
--rw-rw-rw-   0        0        0     3095 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jove.py
--rw-rw-rw-   0        0        0     3976 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jwplatform.py
--rw-rw-rw-   0        0        0     6052 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kakao.py
--rw-rw-rw-   0        0        0    24874 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kaltura.py
--rw-rw-rw-   0        0        0     2743 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kanal2.py
--rw-rw-rw-   0        0        0     1838 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kankanews.py
--rw-rw-rw-   0        0        0     2344 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/karaoketv.py
--rw-rw-rw-   0        0        0     3418 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/karrierevideos.py
--rw-rw-rw-   0        0        0     4665 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/keezmovies.py
--rw-rw-rw-   0        0        0     3547 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kelbyone.py
--rw-rw-rw-   0        0        0     2555 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ketnet.py
--rw-rw-rw-   0        0        0     4213 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/khanacademy.py
--rw-rw-rw-   0        0        0     5581 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kick.py
--rw-rw-rw-   0        0        0     2359 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kicker.py
--rw-rw-rw-   0        0        0     2719 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kickstarter.py
--rw-rw-rw-   0        0        0     8401 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kinja.py
--rw-rw-rw-   0        0        0     2131 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kinopoisk.py
--rw-rw-rw-   0        0        0     1123 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kommunetv.py
--rw-rw-rw-   0        0        0     1112 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kompas.py
--rw-rw-rw-   0        0        0     4530 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/konserthusetplay.py
--rw-rw-rw-   0        0        0     4799 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/koo.py
--rw-rw-rw-   0        0        0     1957 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/krasview.py
--rw-rw-rw-   0        0        0     1031 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kth.py
--rw-rw-rw-   0        0        0      981 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ku6.py
--rw-rw-rw-   0        0        0     3053 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kusi.py
--rw-rw-rw-   0        0        0    12749 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kuwo.py
--rw-rw-rw-   0        0        0     9675 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/la7.py
--rw-rw-rw-   0        0        0     9583 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/laola1tv.py
--rw-rw-rw-   0        0        0     4877 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lastfm.py
--rw-rw-rw-   0        0        0    14567 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lbry.py
--rw-rw-rw-   0        0        0     1321 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lci.py
--rw-rw-rw-   0        0        0     3024 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lcp.py
--rw-rw-rw-   0        0        0     2374 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lecture2go.py
--rw-rw-rw-   0        0        0     8440 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lecturio.py
--rw-rw-rw-   0        0        0    13357 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/leeco.py
--rw-rw-rw-   0        0        0     5523 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lefigaro.py
--rw-rw-rw-   0        0        0     6032 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lego.py
--rw-rw-rw-   0        0        0     2344 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lemonde.py
--rw-rw-rw-   0        0        0     1675 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lenta.py
--rw-rw-rw-   0        0        0     5083 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/libraryofcongress.py
--rw-rw-rw-   0        0        0     3762 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/libsyn.py
--rw-rw-rw-   0        0        0     9758 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lifenews.py
--rw-rw-rw-   0        0        0     7611 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/likee.py
--rw-rw-rw-   0        0        0    15352 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/limelight.py
--rw-rw-rw-   0        0        0     5569 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/line.py
--rw-rw-rw-   0        0        0    10180 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/linkedin.py
--rw-rw-rw-   0        0        0     9979 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/linuxacademy.py
--rw-rw-rw-   0        0        0     3195 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/liputan6.py
--rw-rw-rw-   0        0        0     4253 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/listennotes.py
--rw-rw-rw-   0        0        0     5863 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/litv.py
--rw-rw-rw-   0        0        0     1512 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/livejournal.py
--rw-rw-rw-   0        0        0    13938 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/livestream.py
--rw-rw-rw-   0        0        0     1603 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/livestreamfails.py
--rw-rw-rw-   0        0        0     6481 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lnkgo.py
--rw-rw-rw-   0        0        0     1698 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/localnews8.py
--rw-rw-rw-   0        0        0     1163 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lovehomeporn.py
--rw-rw-rw-   0        0        0     4146 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lrt.py
--rw-rw-rw-   0        0        0     1105 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lumni.py
--rw-rw-rw-   0        0        0    12776 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lynda.py
--rw-rw-rw-   0        0        0      861 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/m6.py
--rw-rw-rw-   0        0        0     3498 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/magentamusik360.py
--rw-rw-rw-   0        0        0    12360 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mailru.py
--rw-rw-rw-   0        0        0     9444 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mainstreaming.py
--rw-rw-rw-   0        0        0     4391 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/malltv.py
--rw-rw-rw-   0        0        0     2541 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mangomolo.py
--rw-rw-rw-   0        0        0     5281 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/manoto.py
--rw-rw-rw-   0        0        0     6086 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/manyvids.py
--rw-rw-rw-   0        0        0     1206 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/maoritv.py
--rw-rw-rw-   0        0        0     4587 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/markiza.py
--rw-rw-rw-   0        0        0     2643 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/massengeschmacktv.py
--rw-rw-rw-   0        0        0     1526 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/masters.py
--rw-rw-rw-   0        0        0     1751 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/matchtv.py
--rw-rw-rw-   0        0        0     7020 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mdr.py
--rw-rw-rw-   0        0        0     6192 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/medaltv.py
--rw-rw-rw-   0        0        0     4311 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediaite.py
--rw-rw-rw-   0        0        0     4434 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediaklikk.py
--rw-rw-rw-   0        0        0     4233 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/medialaan.py
--rw-rw-rw-   0        0        0    13471 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediaset.py
--rw-rw-rw-   0        0        0    17033 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediasite.py
--rw-rw-rw-   0        0        0     9681 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediastream.py
--rw-rw-rw-   0        0        0     4181 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediaworksnz.py
--rw-rw-rw-   0        0        0     2308 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/medici.py
--rw-rw-rw-   0        0        0     1650 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/megaphone.py
--rw-rw-rw-   0        0        0     6875 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/megatvcom.py
--rw-rw-rw-   0        0        0     3636 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/meipai.py
--rw-rw-rw-   0        0        0     2226 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/melonvod.py
--rw-rw-rw-   0        0        0     2636 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/meta.py
--rw-rw-rw-   0        0        0    11888 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/metacafe.py
--rw-rw-rw-   0        0        0     2656 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/metacritic.py
--rw-rw-rw-   0        0        0     2669 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mgoon.py
--rw-rw-rw-   0        0        0     5715 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mgtv.py
--rw-rw-rw-   0        0        0     1429 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/miaopai.py
--rw-rw-rw-   0        0        0     2782 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/microsoftembed.py
--rw-rw-rw-   0        0        0     5510 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/microsoftstream.py
--rw-rw-rw-   0        0        0     7495 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/microsoftvirtualacademy.py
--rw-rw-rw-   0        0        0    11842 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mildom.py
--rw-rw-rw-   0        0        0     7027 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/minds.py
--rw-rw-rw-   0        0        0     2181 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ministrygrid.py
--rw-rw-rw-   0        0        0     1856 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/minoto.py
--rw-rw-rw-   0        0        0     5149 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/miomio.py
--rw-rw-rw-   0        0        0     4998 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mirrativ.py
--rw-rw-rw-   0        0        0     4501 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mirrorcouk.py
--rw-rw-rw-   0        0        0     5295 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mit.py
--rw-rw-rw-   0        0        0     3286 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mitele.py
--rw-rw-rw-   0        0        0     3049 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mixch.py
--rw-rw-rw-   0        0        0    12517 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mixcloud.py
--rw-rw-rw-   0        0        0    15061 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mlb.py
--rw-rw-rw-   0        0        0     6810 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mlssoccer.py
--rw-rw-rw-   0        0        0     2917 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mnet.py
--rw-rw-rw-   0        0        0     3020 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mocha.py
--rw-rw-rw-   0        0        0     2837 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/moevideo.py
--rw-rw-rw-   0        0        0     2733 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mofosex.py
--rw-rw-rw-   0        0        0     2026 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mojvideo.py
--rw-rw-rw-   0        0        0     1835 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/morningstar.py
--rw-rw-rw-   0        0        0    10072 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/motherless.py
--rw-rw-rw-   0        0        0     2040 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/motorsport.py
--rw-rw-rw-   0        0        0     1880 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/movieclips.py
--rw-rw-rw-   0        0        0     3656 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/moviepilot.py
--rw-rw-rw-   0        0        0     1682 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/moview.py
--rw-rw-rw-   0        0        0     1329 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/moviezine.py
--rw-rw-rw-   0        0        0     1783 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/movingimage.py
--rw-rw-rw-   0        0        0     7647 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/msn.py
--rw-rw-rw-   0        0        0    26160 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mtv.py
--rw-rw-rw-   0        0        0     2131 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/muenchentv.py
--rw-rw-rw-   0        0        0     5155 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/murrtube.py
--rw-rw-rw-   0        0        0     2719 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/musescore.py
--rw-rw-rw-   0        0        0     7341 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/musicdex.py
--rw-rw-rw-   0        0        0     3289 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mwave.py
--rw-rw-rw-   0        0        0    10248 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mxplayer.py
--rw-rw-rw-   0        0        0     1553 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mychannels.py
--rw-rw-rw-   0        0        0     7960 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/myspace.py
--rw-rw-rw-   0        0        0     3806 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/myspass.py
--rw-rw-rw-   0        0        0     3915 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/myvi.py
--rw-rw-rw-   0        0        0     3416 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/myvideoge.py
--rw-rw-rw-   0        0        0      904 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/myvidster.py
--rw-rw-rw-   0        0        0     5523 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/n1.py
--rw-rw-rw-   0        0        0     4423 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nate.py
--rw-rw-rw-   0        0        0     3004 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nationalgeographic.py
--rw-rw-rw-   0        0        0    16318 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/naver.py
--rw-rw-rw-   0        0        0    16572 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nba.py
--rw-rw-rw-   0        0        0    33537 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nbc.py
--rw-rw-rw-   0        0        0    18703 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ndr.py
--rw-rw-rw-   0        0        0     4587 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ndtv.py
--rw-rw-rw-   0        0        0    12421 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nebula.py
--rw-rw-rw-   0        0        0     1107 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nerdcubed.py
--rw-rw-rw-   0        0        0    20131 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/neteasemusic.py
--rw-rw-rw-   0        0        0    11267 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/netverse.py
--rw-rw-rw-   0        0        0     2985 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/netzkino.py
--rw-rw-rw-   0        0        0    10185 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/newgrounds.py
--rw-rw-rw-   0        0        0     2141 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/newspicks.py
--rw-rw-rw-   0        0        0     2986 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/newstube.py
--rw-rw-rw-   0        0        0     1877 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/newsy.py
--rw-rw-rw-   0        0        0     9235 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nextmedia.py
--rw-rw-rw-   0        0        0    21718 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nexx.py
--rw-rw-rw-   0        0        0     2351 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nfb.py
--rw-rw-rw-   0        0        0     6000 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nfhsnetwork.py
--rw-rw-rw-   0        0        0    12678 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nfl.py
--rw-rw-rw-   0        0        0    13471 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nhk.py
--rw-rw-rw-   0        0        0     5035 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nhl.py
--rw-rw-rw-   0        0        0    11474 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nick.py
--rw-rw-rw-   0        0        0    37235 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/niconico.py
--rw-rw-rw-   0        0        0     5265 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ninecninemedia.py
--rw-rw-rw-   0        0        0     5326 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ninegag.py
--rw-rw-rw-   0        0        0     5420 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ninenow.py
--rw-rw-rw-   0        0        0     1882 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nintendo.py
--rw-rw-rw-   0        0        0    12954 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nitter.py
--rw-rw-rw-   0        0        0     3191 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/njpwworld.py
--rw-rw-rw-   0        0        0     2088 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nobelprize.py
--rw-rw-rw-   0        0        0     5172 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/noice.py
--rw-rw-rw-   0        0        0     1146 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nonktube.py
--rw-rw-rw-   0        0        0     2639 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/noodlemagazine.py
--rw-rw-rw-   0        0        0     3702 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/noovo.py
--rw-rw-rw-   0        0        0     2175 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/normalboots.py
--rw-rw-rw-   0        0        0     5932 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nosnl.py
--rw-rw-rw-   0        0        0     2495 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nosvideo.py
--rw-rw-rw-   0        0        0    13114 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nova.py
--rw-rw-rw-   0        0        0     3165 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/novaplay.py
--rw-rw-rw-   0        0        0     6107 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nowness.py
--rw-rw-rw-   0        0        0     3613 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/noz.py
--rw-rw-rw-   0        0        0    22896 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/npo.py
--rw-rw-rw-   0        0        0     5872 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/npr.py
--rw-rw-rw-   0        0        0    33058 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nrk.py
--rw-rw-rw-   0        0        0      958 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nrl.py
--rw-rw-rw-   0        0        0     2332 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ntvcojp.py
--rw-rw-rw-   0        0        0     3172 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ntvde.py
--rw-rw-rw-   0        0        0     5675 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ntvru.py
--rw-rw-rw-   0        0        0     4589 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nubilesporn.py
--rw-rw-rw-   0        0        0     1188 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nuevo.py
--rw-rw-rw-   0        0        0     3631 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nuvid.py
--rw-rw-rw-   0        0        0    10706 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nytimes.py
--rw-rw-rw-   0        0        0     6019 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nzherald.py
--rw-rw-rw-   0        0        0     4047 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nzonscreen.py
--rw-rw-rw-   0        0        0     1392 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nzz.py
--rw-rw-rw-   0        0        0     1487 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/odatv.py
--rw-rw-rw-   0        0        0     4367 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/odkmedia.py
--rw-rw-rw-   0        0        0    16622 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/odnoklassniki.py
--rw-rw-rw-   0        0        0     1960 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/oftv.py
--rw-rw-rw-   0        0        0     1473 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/oktoberfesttv.py
--rw-rw-rw-   0        0        0     2933 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/olympics.py
--rw-rw-rw-   0        0        0     4011 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/on24.py
--rw-rw-rw-   0        0        0     2224 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/once.py
--rw-rw-rw-   0        0        0     3424 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ondemandkorea.py
--rw-rw-rw-   0        0        0     2152 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/onefootball.py
--rw-rw-rw-   0        0        0     5247 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/onenewsnz.py
--rw-rw-rw-   0        0        0     1885 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/oneplace.py
--rw-rw-rw-   0        0        0    10104 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/onet.py
--rw-rw-rw-   0        0        0     1774 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/onionstudios.py
--rw-rw-rw-   0        0        0    10297 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ooyala.py
--rw-rw-rw-   0        0        0     8167 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/opencast.py
--rw-rw-rw-   0        0        0     8890 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/openload.py
--rw-rw-rw-   0        0        0     6139 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/openrec.py
--rw-rw-rw-   0        0        0     3197 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ora.py
--rw-rw-rw-   0        0        0    20441 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/orf.py
--rw-rw-rw-   0        0        0      963 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/outsidetv.py
--rw-rw-rw-   0        0        0     6344 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/packtpub.py
--rw-rw-rw-   0        0        0     4598 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/palcomp3.py
--rw-rw-rw-   0        0        0     4766 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pandoratv.py
--rw-rw-rw-   0        0        0    26404 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/panopto.py
--rw-rw-rw-   0        0        0     7684 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/paramountplus.py
--rw-rw-rw-   0        0        0     3892 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/parler.py
--rw-rw-rw-   0        0        0     2816 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/parlview.py
--rw-rw-rw-   0        0        0    19798 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/patreon.py
--rw-rw-rw-   0        0        0    36838 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pbs.py
--rw-rw-rw-   0        0        0     2560 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pearvideo.py
--rw-rw-rw-   0        0        0     7500 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/peekvids.py
--rw-rw-rw-   0        0        0    67249 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/peertube.py
--rw-rw-rw-   0        0        0     2226 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/peertv.py
--rw-rw-rw-   0        0        0     9062 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/peloton.py
--rw-rw-rw-   0        0        0     1112 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/people.py
--rw-rw-rw-   0        0        0     3323 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/performgroup.py
--rw-rw-rw-   0        0        0     7090 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/periscope.py
--rw-rw-rw-   0        0        0     2006 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pgatour.py
--rw-rw-rw-   0        0        0     4165 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/philharmoniedeparis.py
--rw-rw-rw-   0        0        0     5091 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/phoenix.py
--rw-rw-rw-   0        0        0     1776 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/photobucket.py
--rw-rw-rw-   0        0        0     4294 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/piapro.py
--rw-rw-rw-   0        0        0     3897 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/picarto.py
--rw-rw-rw-   0        0        0     6949 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/piksel.py
--rw-rw-rw-   0        0        0     3446 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pinkbike.py
--rw-rw-rw-   0        0        0     9843 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pinterest.py
--rw-rw-rw-   0        0        0     4870 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pixivsketch.py
--rw-rw-rw-   0        0        0     5094 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pladform.py
--rw-rw-rw-   0        0        0     3033 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/planetmarathi.py
--rw-rw-rw-   0        0        0     7622 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/platzi.py
--rw-rw-rw-   0        0        0     2597 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playfm.py
--rw-rw-rw-   0        0        0     3744 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playplustv.py
--rw-rw-rw-   0        0        0     1797 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/plays.py
--rw-rw-rw-   0        0        0     2276 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playstuff.py
--rw-rw-rw-   0        0        0     5279 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playsuisse.py
--rw-rw-rw-   0        0        0     7300 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playtvak.py
--rw-rw-rw-   0        0        0     3216 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playvid.py
--rw-rw-rw-   0        0        0     2495 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playwire.py
--rw-rw-rw-   0        0        0    18866 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pluralsight.py
--rw-rw-rw-   0        0        0     8266 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/plutotv.py
--rw-rw-rw-   0        0        0     2787 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/podbayfm.py
--rw-rw-rw-   0        0        0     3842 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/podchaser.py
--rw-rw-rw-   0        0        0     2658 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/podomatic.py
--rw-rw-rw-   0        0        0     5611 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pokemon.py
--rw-rw-rw-   0        0        0     4286 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pokergo.py
--rw-rw-rw-   0        0        0     3242 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/polsatgo.py
--rw-rw-rw-   0        0        0    21467 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/polskieradio.py
--rw-rw-rw-   0        0        0     3349 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/popcorntimes.py
--rw-rw-rw-   0        0        0     2702 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/popcorntv.py
--rw-rw-rw-   0        0        0     4142 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/porn91.py
--rw-rw-rw-   0        0        0     3889 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/porncom.py
--rw-rw-rw-   0        0        0     1779 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornez.py
--rw-rw-rw-   0        0        0     3577 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornflip.py
--rw-rw-rw-   0        0        0     4654 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornhd.py
--rw-rw-rw-   0        0        0    31978 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornhub.py
--rw-rw-rw-   0        0        0     3196 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornotube.py
--rw-rw-rw-   0        0        0     3997 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornovoisines.py
--rw-rw-rw-   0        0        0     1937 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornoxo.py
--rw-rw-rw-   0        0        0     3567 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pr0gramm.py
--rw-rw-rw-   0        0        0     2841 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/prankcast.py
--rw-rw-rw-   0        0        0     1874 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/premiershiprugby.py
--rw-rw-rw-   0        0        0     2387 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/presstv.py
--rw-rw-rw-   0        0        0     2471 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/projectveritas.py
--rw-rw-rw-   0        0        0    21989 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/prosiebensat1.py
--rw-rw-rw-   0        0        0    16493 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/prx.py
--rw-rw-rw-   0        0        0     8600 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/puhutv.py
--rw-rw-rw-   0        0        0     2292 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/puls4.py
--rw-rw-rw-   0        0        0     2789 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pyvideo.py
--rw-rw-rw-   0        0        0     1957 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/qingting.py
--rw-rw-rw-   0        0        0    13915 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/qqmusic.py
--rw-rw-rw-   0        0        0     4615 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/r7.py
--rw-rw-rw-   0        0        0     9200 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiko.py
--rw-rw-rw-   0        0        0     2432 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiobremen.py
--rw-rw-rw-   0        0        0     6406 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiocanada.py
--rw-rw-rw-   0        0        0     1774 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiode.py
--rw-rw-rw-   0        0        0     4932 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiofrance.py
--rw-rw-rw-   0        0        0     2764 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiojavan.py
--rw-rw-rw-   0        0        0     3461 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiokapital.py
--rw-rw-rw-   0        0        0     2229 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiozet.py
--rw-rw-rw-   0        0        0     7246 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radlive.py
--rw-rw-rw-   0        0        0    33133 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rai.py
--rw-rw-rw-   0        0        0     6301 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/raywenderlich.py
--rw-rw-rw-   0        0        0     3305 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rbgtum.py
--rw-rw-rw-   0        0        0     2418 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rbmaradio.py
--rw-rw-rw-   0        0        0    16592 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rcs.py
--rw-rw-rw-   0        0        0    16846 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rcti.py
--rw-rw-rw-   0        0        0     2891 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rds.py
--rw-rw-rw-   0        0        0    14938 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/redbee.py
--rw-rw-rw-   0        0        0     9485 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/redbulltv.py
--rw-rw-rw-   0        0        0    11363 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/reddit.py
--rw-rw-rw-   0        0        0     9762 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/redgifs.py
--rw-rw-rw-   0        0        0     6217 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/redtube.py
--rw-rw-rw-   0        0        0     2263 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/regiotv.py
--rw-rw-rw-   0        0        0     4165 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rentv.py
--rw-rw-rw-   0        0        0     1298 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/restudy.py
--rw-rw-rw-   0        0        0     2410 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/reuters.py
--rw-rw-rw-   0        0        0     1637 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/reverbnation.py
--rw-rw-rw-   0        0        0     4595 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rice.py
--rw-rw-rw-   0        0        0     2850 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rmcdecouverte.py
--rw-rw-rw-   0        0        0     2218 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rockstargames.py
--rw-rw-rw-   0        0        0    21546 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rokfin.py
--rw-rw-rw-   0        0        0     9066 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/roosterteeth.py
--rw-rw-rw-   0        0        0     1270 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rottentomatoes.py
--rw-rw-rw-   0        0        0     8912 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rozhlas.py
--rw-rw-rw-   0        0        0     6357 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rte.py
--rw-rw-rw-   0        0        0     7280 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtl2.py
--rw-rw-rw-   0        0        0    12416 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtlnl.py
--rw-rw-rw-   0        0        0     7841 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtnews.py
--rw-rw-rw-   0        0        0     3468 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtp.py
--rw-rw-rw-   0        0        0     2821 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtrfm.py
--rw-rw-rw-   0        0        0     9749 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rts.py
--rw-rw-rw-   0        0        0    13225 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtve.py
--rw-rw-rw-   0        0        0     2231 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtvnh.py
--rw-rw-rw-   0        0        0     3513 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtvs.py
--rw-rw-rw-   0        0        0     6294 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtvslo.py
--rw-rw-rw-   0        0        0     1571 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ruhd.py
--rw-rw-rw-   0        0        0     2278 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rule34video.py
--rw-rw-rw-   0        0        0    15562 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rumble.py
--rw-rw-rw-   0        0        0    14239 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rutube.py
--rw-rw-rw-   0        0        0     8255 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rutv.py
--rw-rw-rw-   0        0        0    11230 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ruutu.py
--rw-rw-rw-   0        0        0     7025 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ruv.py
--rw-rw-rw-   0        0        0    10081 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/safari.py
--rw-rw-rw-   0        0        0     3064 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/saitosan.py
--rw-rw-rw-   0        0        0     3914 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/samplefocus.py
--rw-rw-rw-   0        0        0     4512 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sapo.py
--rw-rw-rw-   0        0        0     1040 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/savefrom.py
--rw-rw-rw-   0        0        0     4359 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sbs.py
--rw-rw-rw-   0        0        0     2668 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/screen9.py
--rw-rw-rw-   0        0        0     4711 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/screencast.py
--rw-rw-rw-   0        0        0     1979 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/screencastify.py
--rw-rw-rw-   0        0        0     3023 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/screencastomatic.py
--rw-rw-rw-   0        0        0     5705 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/scrippsnetworks.py
--rw-rw-rw-   0        0        0     3846 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/scrolller.py
--rw-rw-rw-   0        0        0     4959 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/scte.py
--rw-rw-rw-   0        0        0     2295 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/seeker.py
--rw-rw-rw-   0        0        0     8888 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/senategov.py
--rw-rw-rw-   0        0        0     4023 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sendtonews.py
--rw-rw-rw-   0        0        0     5545 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/servus.py
--rw-rw-rw-   0        0        0     5070 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sevenplus.py
--rw-rw-rw-   0        0        0     1983 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sexu.py
--rw-rw-rw-   0        0        0     7780 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/seznamzpravy.py
--rw-rw-rw-   0        0        0     8503 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/shahid.py
--rw-rw-rw-   0        0        0     4449 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/shared.py
--rw-rw-rw-   0        0        0      243 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sharevideos.py
--rw-rw-rw-   0        0        0     4340 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/shemaroome.py
--rw-rw-rw-   0        0        0     3096 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/showroomlive.py
--rw-rw-rw-   0        0        0      744 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sibnet.py
--rw-rw-rw-   0        0        0     6196 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/simplecast.py
--rw-rw-rw-   0        0        0     4303 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sina.py
--rw-rw-rw-   0        0        0     5181 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sixplay.py
--rw-rw-rw-   0        0        0     5715 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/skeb.py
--rw-rw-rw-   0        0        0     6670 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sky.py
--rw-rw-rw-   0        0        0     9452 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/skyit.py
--rw-rw-rw-   0        0        0     1416 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/skylinewebcams.py
--rw-rw-rw-   0        0        0     5439 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/skynewsarabia.py
--rw-rw-rw-   0        0        0     1820 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/skynewsau.py
--rw-rw-rw-   0        0        0     2130 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/slideshare.py
--rw-rw-rw-   0        0        0    23251 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/slideslive.py
--rw-rw-rw-   0        0        0     2372 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/slutload.py
--rw-rw-rw-   0        0        0     2750 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/smotrim.py
--rw-rw-rw-   0        0        0     2497 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/snotr.py
--rw-rw-rw-   0        0        0     7008 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sohu.py
--rw-rw-rw-   0        0        0     9700 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sonyliv.py
--rw-rw-rw-   0        0        0    36979 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/soundcloud.py
--rw-rw-rw-   0        0        0     2427 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/soundgasm.py
--rw-rw-rw-   0        0        0     7973 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/southpark.py
--rw-rw-rw-   0        0        0     8462 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sovietscloset.py
--rw-rw-rw-   0        0        0     7388 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spankbang.py
--rw-rw-rw-   0        0        0     6447 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spankwire.py
--rw-rw-rw-   0        0        0     2378 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spiegel.py
--rw-rw-rw-   0        0        0     1707 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spike.py
--rw-rw-rw-   0        0        0     3233 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sport5.py
--rw-rw-rw-   0        0        0     3321 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sportbox.py
--rw-rw-rw-   0        0        0     6437 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sportdeutschland.py
--rw-rw-rw-   0        0        0     6508 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spotify.py
--rw-rw-rw-   0        0        0     6146 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spreaker.py
--rw-rw-rw-   0        0        0     4100 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/springboardplatform.py
--rw-rw-rw-   0        0        0     2330 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sprout.py
--rw-rw-rw-   0        0        0    10184 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/srgssr.py
--rw-rw-rw-   0        0        0     2323 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/srmediathek.py
--rw-rw-rw-   0        0        0     3574 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/stanfordoc.py
--rw-rw-rw-   0        0        0     3886 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/startrek.py
--rw-rw-rw-   0        0        0     3630 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/startv.py
--rw-rw-rw-   0        0        0     6872 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/steam.py
--rw-rw-rw-   0        0        0     5472 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/stitcher.py
--rw-rw-rw-   0        0        0     4917 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/storyfire.py
--rw-rw-rw-   0        0        0     4020 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streamable.py
--rw-rw-rw-   0        0        0     1831 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streamanity.py
--rw-rw-rw-   0        0        0     2576 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streamcloud.py
--rw-rw-rw-   0        0        0     5133 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streamcz.py
--rw-rw-rw-   0        0        0     1049 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streamff.py
--rw-rw-rw-   0        0        0     3664 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streetvoice.py
--rw-rw-rw-   0        0        0     1333 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/stretchinternet.py
--rw-rw-rw-   0        0        0     2716 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/stripchat.py
--rw-rw-rw-   0        0        0     3418 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/stv.py
--rw-rw-rw-   0        0        0     4323 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/substack.py
--rw-rw-rw-   0        0        0     2603 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sunporno.py
--rw-rw-rw-   0        0        0     3928 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sverigesradio.py
--rw-rw-rw-   0        0        0    15604 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/svt.py
--rw-rw-rw-   0        0        0     3304 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/swearnet.py
--rw-rw-rw-   0        0        0     4393 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/swrmediathek.py
--rw-rw-rw-   0        0        0     2061 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/syfy.py
--rw-rw-rw-   0        0        0     1271 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/syvdk.py
--rw-rw-rw-   0        0        0     1654 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sztvhu.py
--rw-rw-rw-   0        0        0     5900 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tagesschau.py
--rw-rw-rw-   0        0        0     1981 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tass.py
--rw-rw-rw-   0        0        0     3576 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tbs.py
--rw-rw-rw-   0        0        0     2472 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tdslifeway.py
--rw-rw-rw-   0        0        0    10734 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teachable.py
--rw-rw-rw-   0        0        0     4443 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teachertube.py
--rw-rw-rw-   0        0        0     1052 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teachingchannel.py
--rw-rw-rw-   0        0        0    10266 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teamcoco.py
--rw-rw-rw-   0        0        0     5508 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teamtreehouse.py
--rw-rw-rw-   0        0        0     2564 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/techtalks.py
--rw-rw-rw-   0        0        0    10057 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ted.py
--rw-rw-rw-   0        0        0     3333 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tele13.py
--rw-rw-rw-   0        0        0     3368 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tele5.py
--rw-rw-rw-   0        0        0     2888 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telebruxelles.py
--rw-rw-rw-   0        0        0     3208 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telecaribe.py
--rw-rw-rw-   0        0        0     6280 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telecinco.py
--rw-rw-rw-   0        0        0     3078 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telegraaf.py
--rw-rw-rw-   0        0        0     5221 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telegram.py
--rw-rw-rw-   0        0        0     2944 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telemb.py
--rw-rw-rw-   0        0        0     2425 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telemundo.py
--rw-rw-rw-   0        0        0     9224 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telequebec.py
--rw-rw-rw-   0        0        0     1749 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teletask.py
--rw-rw-rw-   0        0        0     1838 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telewebion.py
--rw-rw-rw-   0        0        0     5002 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tempo.py
--rw-rw-rw-   0        0        0    20439 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tencent.py
--rw-rw-rw-   0        0        0     7420 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tennistv.py
--rw-rw-rw-   0        0        0     4728 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tenplay.py
--rw-rw-rw-   0        0        0     1927 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/testurl.py
--rw-rw-rw-   0        0        0     3049 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tf1.py
--rw-rw-rw-   0        0        0     2033 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tfo.py
--rw-rw-rw-   0        0        0     1495 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/theholetv.py
--rw-rw-rw-   0        0        0     1790 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/theintercept.py
--rw-rw-rw-   0        0        0    17558 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/theplatform.py
--rw-rw-rw-   0        0        0     1380 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thestar.py
--rw-rw-rw-   0        0        0     1699 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thesun.py
--rw-rw-rw-   0        0        0     3669 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/theta.py
--rw-rw-rw-   0        0        0     4046 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/theweatherchannel.py
--rw-rw-rw-   0        0        0     1547 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thisamericanlife.py
--rw-rw-rw-   0        0        0     2465 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thisav.py
--rw-rw-rw-   0        0        0     2736 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thisoldhouse.py
--rw-rw-rw-   0        0        0     8843 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thisvid.py
--rw-rw-rw-   0        0        0     6375 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/threeqsdn.py
--rw-rw-rw-   0        0        0     4098 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/threespeak.py
--rw-rw-rw-   0        0        0    53946 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tiktok.py
--rw-rw-rw-   0        0        0     1905 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tinypic.py
--rw-rw-rw-   0        0        0     9781 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tmz.py
--rw-rw-rw-   0        0        0    13962 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tnaflix.py
--rw-rw-rw-   0        0        0     9040 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/toggle.py
--rw-rw-rw-   0        0        0     3486 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/toggo.py
--rw-rw-rw-   0        0        0     5774 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tokentube.py
--rw-rw-rw-   0        0        0     1919 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tonline.py
--rw-rw-rw-   0        0        0     3048 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/toongoggles.py
--rw-rw-rw-   0        0        0     3605 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/toutv.py
--rw-rw-rw-   0        0        0     2776 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/toypics.py
--rw-rw-rw-   0        0        0     2654 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/traileraddict.py
--rw-rw-rw-   0        0        0    12826 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/triller.py
--rw-rw-rw-   0        0        0     3667 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trilulilu.py
--rw-rw-rw-   0        0        0    13243 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trovo.py
--rw-rw-rw-   0        0        0     1986 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trtcocuk.py
--rw-rw-rw-   0        0        0     6484 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trueid.py
--rw-rw-rw-   0        0        0     1476 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trunews.py
--rw-rw-rw-   0        0        0     2896 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/truth.py
--rw-rw-rw-   0        0        0     2530 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trutv.py
--rw-rw-rw-   0        0        0     3082 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tube8.py
--rw-rw-rw-   0        0        0    10954 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tubetugraz.py
--rw-rw-rw-   0        0        0     6867 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tubitv.py
--rw-rw-rw-   0        0        0    16818 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tumblr.py
--rw-rw-rw-   0        0        0     9371 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tunein.py
--rw-rw-rw-   0        0        0     3210 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tunepk.py
--rw-rw-rw-   0        0        0     2398 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/turbo.py
--rw-rw-rw-   0        0        0    11312 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/turner.py
--rw-rw-rw-   0        0        0    13990 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv2.py
--rw-rw-rw-   0        0        0     3723 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv24ua.py
--rw-rw-rw-   0        0        0     6191 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv2dk.py
--rw-rw-rw-   0        0        0     4181 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv2hu.py
--rw-rw-rw-   0        0        0     4972 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv4.py
--rw-rw-rw-   0        0        0     4671 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv5mondeplus.py
--rw-rw-rw-   0        0        0     4134 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv5unis.py
--rw-rw-rw-   0        0        0     3186 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tva.py
--rw-rw-rw-   0        0        0     2406 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvanouvelles.py
--rw-rw-rw-   0        0        0     3768 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvc.py
--rw-rw-rw-   0        0        0     4983 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tver.py
--rw-rw-rw-   0        0        0     5176 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvigle.py
--rw-rw-rw-   0        0        0     3325 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tviplayer.py
--rw-rw-rw-   0        0        0     1560 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvland.py
--rw-rw-rw-   0        0        0     3908 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvn24.py
--rw-rw-rw-   0        0        0     4851 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvnet.py
--rw-rw-rw-   0        0        0     1600 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvnoe.py
--rw-rw-rw-   0        0        0    24665 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvnow.py
--rw-rw-rw-   0        0        0     5325 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvopengr.py
--rw-rw-rw-   0        0        0    23559 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvp.py
--rw-rw-rw-   0        0        0    20702 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvplay.py
--rw-rw-rw-   0        0        0     2797 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvplayer.py
--rw-rw-rw-   0        0        0     2147 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tweakers.py
--rw-rw-rw-   0        0        0     4812 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twentyfourvideo.py
--rw-rw-rw-   0        0        0     2718 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twentymin.py
--rw-rw-rw-   0        0        0     3318 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twentythreevideo.py
--rw-rw-rw-   0        0        0    12618 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twitcasting.py
--rw-rw-rw-   0        0        0    43480 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twitch.py
--rw-rw-rw-   0        0        0    59522 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twitter.py
--rw-rw-rw-   0        0        0    16085 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/txxx.py
--rw-rw-rw-   0        0        0    20020 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/udemy.py
--rw-rw-rw-   0        0        0     3676 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/udn.py
--rw-rw-rw-   0        0        0      467 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ufctv.py
--rw-rw-rw-   0        0        0     2508 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ukcolumn.py
--rw-rw-rw-   0        0        0     1493 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/uktvplay.py
--rw-rw-rw-   0        0        0     3266 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/umg.py
--rw-rw-rw-   0        0        0     2141 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/unistra.py
--rw-rw-rw-   0        0        0     1217 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/unity.py
--rw-rw-rw-   0        0        0     2573 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/unscripted.py
--rw-rw-rw-   0        0        0     5615 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/unsupported.py
--rw-rw-rw-   0        0        0     5514 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/uol.py
--rw-rw-rw-   0        0        0     3440 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/uplynk.py
--rw-rw-rw-   0        0        0     2163 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/urort.py
--rw-rw-rw-   0        0        0     7021 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/urplay.py
--rw-rw-rw-   0        0        0      819 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/usanetwork.py
--rw-rw-rw-   0        0        0     2706 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/usatoday.py
--rw-rw-rw-   0        0        0    10820 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ustream.py
--rw-rw-rw-   0        0        0     4379 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ustudio.py
--rw-rw-rw-   0        0        0     3502 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/utreon.py
--rw-rw-rw-   0        0        0     3096 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/varzesh3.py
--rw-rw-rw-   0        0        0     3295 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vbox7.py
--rw-rw-rw-   0        0        0     4209 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/veehd.py
--rw-rw-rw-   0        0        0     2812 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/veo.py
--rw-rw-rw-   0        0        0     7128 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/veoh.py
--rw-rw-rw-   0        0        0     4440 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vesti.py
--rw-rw-rw-   0        0        0    13857 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vevo.py
--rw-rw-rw-   0        0        0    11171 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vgtv.py
--rw-rw-rw-   0        0        0     1414 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vh1.py
--rw-rw-rw-   0        0        0    12365 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vice.py
--rw-rw-rw-   0        0        0     2958 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vidbit.py
--rw-rw-rw-   0        0        0     5072 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viddler.py
--rw-rw-rw-   0        0        0     6643 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videa.py
--rw-rw-rw-   0        0        0    10990 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videocampus_sachsen.py
--rw-rw-rw-   0        0        0      892 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videodetective.py
--rw-rw-rw-   0        0        0     1759 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videofyme.py
--rw-rw-rw-   0        0        0    14035 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videoken.py
--rw-rw-rw-   0        0        0    11631 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videomore.py
--rw-rw-rw-   0        0        0     3228 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videopress.py
--rw-rw-rw-   0        0        0    14059 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vidio.py
--rw-rw-rw-   0        0        0     5888 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vidlii.py
--rw-rw-rw-   0        0        0    14139 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viewlift.py
--rw-rw-rw-   0        0        0     7548 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viidea.py
--rw-rw-rw-   0        0        0    13838 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viki.py
--rw-rw-rw-   0        0        0    63610 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vimeo.py
--rw-rw-rw-   0        0        0     2220 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vimm.py
--rw-rw-rw-   0        0        0     1949 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vimple.py
--rw-rw-rw-   0        0        0     5553 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vine.py
--rw-rw-rw-   0        0        0     3123 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viqeo.py
--rw-rw-rw-   0        0        0    21769 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viu.py
--rw-rw-rw-   0        0        0    28692 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vk.py
--rw-rw-rw-   0        0        0     2199 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vocaroo.py
--rw-rw-rw-   0        0        0     2816 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vodlocker.py
--rw-rw-rw-   0        0        0     1004 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vodpl.py
--rw-rw-rw-   0        0        0     1653 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vodplatform.py
--rw-rw-rw-   0        0        0     2284 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/voicerepublic.py
--rw-rw-rw-   0        0        0     5507 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/voicy.py
--rw-rw-rw-   0        0        0     1707 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/volejtv.py
--rw-rw-rw-   0        0        0     6114 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/voot.py
--rw-rw-rw-   0        0        0    10015 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/voxmedia.py
--rw-rw-rw-   0        0        0     2963 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vrak.py
--rw-rw-rw-   0        0        0     3549 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vrt.py
--rw-rw-rw-   0        0        0    11172 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vrv.py
--rw-rw-rw-   0        0        0     2034 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vshare.py
--rw-rw-rw-   0        0        0     1901 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vtm.py
--rw-rw-rw-   0        0        0     2281 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vuclip.py
--rw-rw-rw-   0        0        0     2167 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vupload.py
--rw-rw-rw-   0        0        0    11057 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vvvvid.py
--rw-rw-rw-   0        0        0     2008 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vyborymos.py
--rw-rw-rw-   0        0        0     3516 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vzaar.py
--rw-rw-rw-   0        0        0     2851 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wakanim.py
--rw-rw-rw-   0        0        0     2802 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/walla.py
--rw-rw-rw-   0        0        0     6305 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wasdtv.py
--rw-rw-rw-   0        0        0     5939 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/washingtonpost.py
--rw-rw-rw-   0        0        0     4332 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wat.py
--rw-rw-rw-   0        0        0     5917 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/watchbox.py
--rw-rw-rw-   0        0        0     2301 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/watchindianporn.py
--rw-rw-rw-   0        0        0    14928 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wdr.py
--rw-rw-rw-   0        0        0     1628 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/webcamerapl.py
--rw-rw-rw-   0        0        0     3752 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/webcaster.py
--rw-rw-rw-   0        0        0     5611 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/webofstories.py
--rw-rw-rw-   0        0        0     4487 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/weibo.py
--rw-rw-rw-   0        0        0     1673 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/weiqitv.py
--rw-rw-rw-   0        0        0     4033 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/whowatch.py
--rw-rw-rw-   0        0        0     2376 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wikimedia.py
--rw-rw-rw-   0        0        0     2398 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/willow.py
--rw-rw-rw-   0        0        0     5614 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wimtv.py
--rw-rw-rw-   0        0        0    16231 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wistia.py
--rw-rw-rw-   0        0        0     7350 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wordpress.py
--rw-rw-rw-   0        0        0     1341 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/worldstarhiphop.py
--rw-rw-rw-   0        0        0     6286 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wppilot.py
--rw-rw-rw-   0        0        0    10017 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wrestleuniverse.py
--rw-rw-rw-   0        0        0     4778 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wsj.py
--rw-rw-rw-   0        0        0     4629 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wwe.py
--rw-rw-rw-   0        0        0     2156 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xanimu.py
--rw-rw-rw-   0        0        0     1448 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xbef.py
--rw-rw-rw-   0        0        0     2377 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xboxclips.py
--rw-rw-rw-   0        0        0     7606 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xfileshare.py
--rw-rw-rw-   0        0        0    19690 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xhamster.py
--rw-rw-rw-   0        0        0     6807 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ximalaya.py
--rw-rw-rw-   0        0        0     4048 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xinpianchang.py
--rw-rw-rw-   0        0        0     2956 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xminus.py
--rw-rw-rw-   0        0        0     2972 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xnxx.py
--rw-rw-rw-   0        0        0     3996 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xstream.py
--rw-rw-rw-   0        0        0     8107 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xtube.py
--rw-rw-rw-   0        0        0     5863 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xuite.py
--rw-rw-rw-   0        0        0     6889 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xvideos.py
--rw-rw-rw-   0        0        0     2689 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xxxymovies.py
--rw-rw-rw-   0        0        0    23347 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yahoo.py
--rw-rw-rw-   0        0        0     5201 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yandexdisk.py
--rw-rw-rw-   0        0        0    18103 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yandexmusic.py
--rw-rw-rw-   0        0        0    17877 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yandexvideo.py
--rw-rw-rw-   0        0        0     3028 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yapfiles.py
--rw-rw-rw-   0        0        0     4696 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yappy.py
--rw-rw-rw-   0        0        0     2198 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yesjapan.py
--rw-rw-rw-   0        0        0     1867 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yinyuetai.py
--rw-rw-rw-   0        0        0     6370 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yle_areena.py
--rw-rw-rw-   0        0        0     1721 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ynet.py
--rw-rw-rw-   0        0        0     3114 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/youjizz.py
--rw-rw-rw-   0        0        0    12070 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/youku.py
--rw-rw-rw-   0        0        0     7229 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/younow.py
--rw-rw-rw-   0        0        0     8268 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/youporn.py
--rw-rw-rw-   0        0        0     2086 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yourporn.py
--rw-rw-rw-   0        0        0     1397 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yourupload.py
--rw-rw-rw-   0        0        0   339334 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/youtube.py
--rw-rw-rw-   0        0        0     3938 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zapiks.py
--rw-rw-rw-   0        0        0    30272 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zattoo.py
--rw-rw-rw-   0        0        0    18883 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zdf.py
--rw-rw-rw-   0        0        0    11931 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zee5.py
--rw-rw-rw-   0        0        0     3198 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zeenews.py
--rw-rw-rw-   0        0        0     2610 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zhihu.py
--rw-rw-rw-   0        0        0    14954 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zingmp3.py
--rw-rw-rw-   0        0        0     3909 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zoom.py
--rw-rw-rw-   0        0        0     5628 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zype.py
--rw-rw-rw-   0        0        0     1957 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/flserver.py
--rw-rw-rw-   0        0        0      197 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/gunicorn.conf.py
--rw-rw-rw-   0        0        0    35050 2023-04-04 04:11:50.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/jsinterp.py
--rw-rw-rw-   0        0        0     5510 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/minicurses.py
--rw-rw-rw-   0        0        0    96161 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/options.py
--rw-rw-rw-   0        0        0     6359 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/plugins.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:26.353268 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/
--rw-rw-rw-   0        0        0     1327 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/__init__.py
--rw-rw-rw-   0        0        0     8584 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/common.py
--rw-rw-rw-   0        0        0    10652 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/embedthumbnail.py
--rw-rw-rw-   0        0        0     1649 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/exec.py
--rw-rw-rw-   0        0        0    50353 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/ffmpeg.py
--rw-rw-rw-   0        0        0     4512 2023-04-04 05:52:42.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/metadataparser.py
--rw-rw-rw-   0        0        0    18157 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/modify_chapters.py
--rw-rw-rw-   0        0        0     2109 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/movefilesafterdownload.py
--rw-rw-rw-   0        0        0     4195 2023-04-04 05:52:41.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/sponskrub.py
--rw-rw-rw-   0        0        0     4353 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/sponsorblock.py
--rw-rw-rw-   0        0        0     2544 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/xattrpp.py
--rw-rw-rw-   0        0        0     2352 2023-04-04 04:11:51.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/server1.py
--rw-rw-rw-   0        0        0     8784 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/socks.py
--rw-rw-rw-   0        0        0    16049 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/update.py
--rw-rw-rw-   0        0        0   230917 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/utils.py
--rw-rw-rw-   0        0        0      206 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/version.py
--rw-rw-rw-   0        0        0    11735 2023-04-04 04:11:52.000000 yt-dlp-cp-0.9.9/yt_dlp_cp/webvtt.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:25:25.392726 yt-dlp-cp-0.9.9/yt_dlp_cp.egg-info/
--rw-rw-rw-   0        0        0      165 2023-04-04 07:25:25.000000 yt-dlp-cp-0.9.9/yt_dlp_cp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    37696 2023-04-04 07:25:25.000000 yt-dlp-cp-0.9.9/yt_dlp_cp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 07:25:25.000000 yt-dlp-cp-0.9.9/yt_dlp_cp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-04-04 07:25:25.000000 yt-dlp-cp-0.9.9/yt_dlp_cp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      155 2023-04-04 07:25:25.000000 yt-dlp-cp-0.9.9/yt_dlp_cp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-04 07:25:25.000000 yt-dlp-cp-0.9.9/yt_dlp_cp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:15.618256 yt-dlp-cp-1.9.9/
+-rw-rw-rw-   0        0        0   233121 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/Changelog.md
+-rw-rw-rw-   0        0        0     1211 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/LICENSE
+-rw-rw-rw-   0        0        0      219 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      165 2023-06-29 08:20:15.618256 yt-dlp-cp-1.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0   155243 2023-04-04 05:52:42.000000 yt-dlp-cp-1.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.248124 yt-dlp-cp-1.9.9/devscripts/
+-rw-rw-rw-   0        0        0      147 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/SizeOfImage.patch
+-rw-rw-rw-   0        0        0      148 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/SizeOfImage_w.patch
+-rw-rw-rw-   0        0        0       78 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.249588 yt-dlp-cp-1.9.9/devscripts/__pycache__/
+-rw-rw-rw-   0        0        0      135 2023-04-04 07:22:59.000000 yt-dlp-cp-1.9.9/devscripts/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1929 2023-04-04 07:22:59.000000 yt-dlp-cp-1.9.9/devscripts/__pycache__/utils.cpython-38.pyc
+-rw-rw-rw-   0        0        0      832 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/bash-completion.in
+-rw-rw-rw-   0        0        0      891 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/devscripts/bash-completion.py
+-rw-rw-rw-   0        0        0      942 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/changelog_override.json
+-rw-rw-rw-   0        0        0     2914 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/changelog_override.schema.json
+-rw-rw-rw-   0        0        0     1801 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/check-porn.py
+-rw-rw-rw-   0        0        0      126 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/fish-completion.in
+-rw-rw-rw-   0        0        0     1731 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/devscripts/fish-completion.py
+-rw-rw-rw-   0        0        0     1191 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/devscripts/generate_aes_testdata.py
+-rw-rw-rw-   0        0        0     1228 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/lazy_load_template.py
+-rw-rw-rw-   0        0        0    41043 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/logo.ico
+-rw-rw-rw-   0        0        0    17117 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/make_changelog.py
+-rw-rw-rw-   0        0        0      763 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/make_contributing.py
+-rw-rw-rw-   0        0        0     2758 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/make_issue_template.py
+-rw-rw-rw-   0        0        0     4688 2023-04-04 05:52:42.000000 yt-dlp-cp-1.9.9/devscripts/make_lazy_extractors.py
+-rw-rw-rw-   0        0        0     2892 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/make_readme.py
+-rw-rw-rw-   0        0        0      508 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/devscripts/make_supportedsites.py
+-rw-rw-rw-   0        0        0     2877 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/prepare_manpage.py
+-rwxrwxrwx   0        0        0      343 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/run_tests.bat
+-rw-rw-rw-   0        0        0      305 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/run_tests.sh
+-rw-rw-rw-   0        0        0      987 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/devscripts/set-variant.py
+-rw-rw-rw-   0        0        0     1074 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/update-formulae.py
+-rw-rw-rw-   0        0        0     2061 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/devscripts/update-version.py
+-rw-rw-rw-   0        0        0     1375 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/devscripts/utils.py
+-rw-rw-rw-   0        0        0      864 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/devscripts/zsh-completion.in
+-rw-rw-rw-   0        0        0     1437 2023-04-04 05:52:42.000000 yt-dlp-cp-1.9.9/devscripts/zsh-completion.py
+-rw-rw-rw-   0        0        0      179 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/pyproject.toml
+-rw-rw-rw-   0        0        0      145 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/requirements.txt
+-rw-rw-rw-   0        0        0      974 2023-06-29 08:20:15.625959 yt-dlp-cp-1.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     4657 2023-06-29 07:28:38.000000 yt-dlp-cp-1.9.9/setup.py
+-rw-rw-rw-   0        0        0    50029 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/supportedsites.md
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.290275 yt-dlp-cp-1.9.9/test/
+-rw-rw-rw-   0        0        0        0 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/__init__.py
+-rw-rw-rw-   0        0        0    12506 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/helper.py
+-rw-rw-rw-   0        0        0     1239 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/parameters.json
+-rw-rw-rw-   0        0        0   103895 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_InfoExtractor.py
+-rw-rw-rw-   0        0        0    51120 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_YoutubeDL.py
+-rw-rw-rw-   0        0        0     1952 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_YoutubeDLCookieJar.py
+-rw-rw-rw-   0        0        0     7023 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_aes.py
+-rw-rw-rw-   0        0        0     1536 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_age_restriction.py
+-rw-rw-rw-   0        0        0     6245 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_all_urls.py
+-rw-rw-rw-   0        0        0     1576 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_cache.py
+-rw-rw-rw-   0        0        0     4759 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_compat.py
+-rw-rw-rw-   0        0        0     6960 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_config.py
+-rw-rw-rw-   0        0        0    13436 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_cookies.py
+-rw-rw-rw-   0        0        0    11851 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_download.py
+-rw-rw-rw-   0        0        0     3516 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_downloader_http.py
+-rw-rw-rw-   0        0        0     1908 2023-04-04 05:52:42.000000 yt-dlp-cp-1.9.9/test/test_execution.py
+-rw-rw-rw-   0        0        0     7315 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_http.py
+-rw-rw-rw-   0        0        0     1042 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_iqiyi_sdk_interpreter.py
+-rw-rw-rw-   0        0        0    15661 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_jsinterp.py
+-rw-rw-rw-   0        0        0      746 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_netrc.py
+-rw-rw-rw-   0        0        0     1813 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_overwrites.py
+-rw-rw-rw-   0        0        0     2842 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_plugins.py
+-rw-rw-rw-   0        0        0     2101 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_post_hooks.py
+-rw-rw-rw-   0        0        0    31130 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_postprocessors.py
+-rw-rw-rw-   0        0        0     3363 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/test_socks.py
+-rw-rw-rw-   0        0        0    17852 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_subtitles.py
+-rw-rw-rw-   0        0        0     1093 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_update.py.disabled
+-rw-rw-rw-   0        0        0   113432 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_utils.py
+-rw-rw-rw-   0        0        0     2791 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_verbose_output.py
+-rw-rw-rw-   0        0        0     2569 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_write_annotations.py.disabled
+-rw-rw-rw-   0        0        0     2817 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_youtube_lists.py
+-rw-rw-rw-   0        0        0      993 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_youtube_misc.py
+-rw-rw-rw-   0        0        0     9070 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/test_youtube_signature.py
+-rw-rw-rw-   0        0        0     3176 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testcert.pem
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.204113 yt-dlp-cp-1.9.9/test/testdata/
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.299176 yt-dlp-cp-1.9.9/test/testdata/certificate/
+-rw-rw-rw-   0        0        0      574 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/certificate/ca.crt
+-rw-rw-rw-   0        0        0      227 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/certificate/ca.key
+-rw-rw-rw-   0        0        0       41 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/certificate/ca.srl
+-rw-rw-rw-   0        0        0      457 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/certificate/client.crt
+-rw-rw-rw-   0        0        0      359 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/certificate/client.csr
+-rw-rw-rw-   0        0        0      227 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/certificate/client.key
+-rw-rw-rw-   0        0        0      314 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/certificate/clientencrypted.key
+-rw-rw-rw-   0        0        0      771 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/certificate/clientwithencryptedkey.crt
+-rw-rw-rw-   0        0        0      684 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/certificate/clientwithkey.crt
+-rw-rw-rw-   0        0        0      727 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/certificate/instructions.md
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.304714 yt-dlp-cp-1.9.9/test/testdata/cookies/
+-rw-rw-rw-   0        0        0      294 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/cookies/httponly_cookies.txt
+-rw-rw-rw-   0        0        0      336 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/cookies/malformed_cookies.txt
+-rw-rw-rw-   0        0        0      269 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/cookies/session_cookies.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.306084 yt-dlp-cp-1.9.9/test/testdata/f4m/
+-rw-rw-rw-   0        0        0      994 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/f4m/custom_base_url.f4m
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.307106 yt-dlp-cp-1.9.9/test/testdata/ism/
+-rw-rw-rw-   0        0        0     3987 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/ism/ec-3_test.Manifest
+-rw-rw-rw-   0        0        0    23179 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/ism/sintel.Manifest
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.309090 yt-dlp-cp-1.9.9/test/testdata/m3u8/
+-rw-rw-rw-   0        0        0     3286 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/m3u8/bipbop_16x9.m3u8
+-rw-rw-rw-   0        0        0     6291 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.312090 yt-dlp-cp-1.9.9/test/testdata/mpd/
+-rw-rw-rw-   0        0        0     1715 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/mpd/float_duration.mpd
+-rw-rw-rw-   0        0        0    10268 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/mpd/subtitles.mpd
+-rw-rw-rw-   0        0        0     1744 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/mpd/unfragmented.mpd
+-rw-rw-rw-   0        0        0    22374 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/mpd/urls_only.mpd
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.199782 yt-dlp-cp-1.9.9/test/testdata/thumbnails/
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.312090 yt-dlp-cp-1.9.9/test/testdata/thumbnails/foo %d bar/
+-rw-rw-rw-   0        0        0     3928 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/thumbnails/foo %d bar/foo_%d.webp
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.313493 yt-dlp-cp-1.9.9/test/testdata/xspf/
+-rw-rw-rw-   0        0        0     1385 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/testdata/xspf/foo_xspf.xspf
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.203102 yt-dlp-cp-1.9.9/test/testdata/yt_dlp_plugins/
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.315503 yt-dlp-cp-1.9.9/test/testdata/yt_dlp_plugins/extractor/
+-rw-rw-rw-   0        0        0      106 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/testdata/yt_dlp_plugins/extractor/_ignore.py
+-rw-rw-rw-   0        0        0      198 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/testdata/yt_dlp_plugins/extractor/ignore.py
+-rw-rw-rw-   0        0        0      169 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/testdata/yt_dlp_plugins/extractor/normal.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.316504 yt-dlp-cp-1.9.9/test/testdata/yt_dlp_plugins/postprocessor/
+-rw-rw-rw-   0        0        0      110 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/testdata/yt_dlp_plugins/postprocessor/normal.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.204113 yt-dlp-cp-1.9.9/test/testdata/zipped_plugins/
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.205445 yt-dlp-cp-1.9.9/test/testdata/zipped_plugins/yt_dlp_plugins/
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.319685 yt-dlp-cp-1.9.9/test/testdata/zipped_plugins/yt_dlp_plugins/extractor/
+-rw-rw-rw-   0        0        0      106 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/testdata/zipped_plugins/yt_dlp_plugins/extractor/zipped.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.322687 yt-dlp-cp-1.9.9/test/testdata/zipped_plugins/yt_dlp_plugins/postprocessor/
+-rw-rw-rw-   0        0        0      110 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/test/testdata/zipped_plugins/yt_dlp_plugins/postprocessor/zipped.py
+-rw-rw-rw-   0        0        0     1608 2023-03-23 04:28:30.000000 yt-dlp-cp-1.9.9/test/versions.json
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.342431 yt-dlp-cp-1.9.9/yt_dlp_cp/
+-rw-rw-rw-   0        0        0   199501 2023-06-29 07:34:36.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/YoutubeDL.py
+-rw-rw-rw-   0        0        0    44156 2023-06-29 07:25:37.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/__init__.py
+-rw-rw-rw-   0        0        0      466 2023-06-29 07:36:38.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.365261 yt-dlp-cp-1.9.9/yt_dlp_cp/__pyinstaller/
+-rw-rw-rw-   0        0        0       77 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      942 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/__pyinstaller/hook-yt_dlp.py
+-rw-rw-rw-   0        0        0    22969 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/aes.py
+-rw-rw-rw-   0        0        0     3465 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/cache.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.376801 yt-dlp-cp-1.9.9/yt_dlp_cp/compat/
+-rw-rw-rw-   0        0        0     2404 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/compat/__init__.py
+-rw-rw-rw-   0        0        0      446 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/compat/_deprecated.py
+-rw-rw-rw-   0        0        0     4011 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/compat/_legacy.py
+-rw-rw-rw-   0        0        0     2660 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/compat/compat_utils.py
+-rw-rw-rw-   0        0        0      690 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/compat/functools.py
+-rw-rw-rw-   0        0        0      588 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/compat/imghdr.py
+-rw-rw-rw-   0        0        0      889 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/compat/shutil.py
+-rw-rw-rw-   0        0        0    44722 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/cookies.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.379326 yt-dlp-cp-1.9.9/yt_dlp_cp/dependencies/
+-rw-rw-rw-   0        0        0     1450 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/dependencies/Cryptodome.py
+-rw-rw-rw-   0        0        0     2061 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/dependencies/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.396416 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/
+-rw-rw-rw-   0        0        0     4574 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/__init__.py
+-rw-rw-rw-   0        0        0    19115 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/common.py
+-rw-rw-rw-   0        0        0     3593 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/dash.py
+-rw-rw-rw-   0        0        0    26627 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/external.py
+-rw-rw-rw-   0        0        0    15759 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/f4m.py
+-rw-rw-rw-   0        0        0     1370 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/fc2.py
+-rw-rw-rw-   0        0        0    22680 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/fragment.py
+-rw-rw-rw-   0        0        0    17396 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/hls.py
+-rw-rw-rw-   0        0        0    17601 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/http.py
+-rw-rw-rw-   0        0        0    11914 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/ism.py
+-rw-rw-rw-   0        0        0     6371 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/mhtml.py
+-rw-rw-rw-   0        0        0     1974 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/niconico.py
+-rw-rw-rw-   0        0        0     9136 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/rtmp.py
+-rw-rw-rw-   0        0        0     1551 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/rtsp.py
+-rw-rw-rw-   0        0        0     1825 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/websocket.py
+-rw-rw-rw-   0        0        0    11143 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/youtube_live_chat.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:15.604730 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/
+-rw-rw-rw-   0        0        0     1395 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/__init__.py
+-rw-rw-rw-   0        0        0    54810 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/_extractors.py
+-rw-rw-rw-   0        0        0    13048 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/abc.py
+-rw-rw-rw-   0        0        0     6481 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/abcnews.py
+-rw-rw-rw-   0        0        0     4726 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/abcotvs.py
+-rw-rw-rw-   0        0        0    21334 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/abematv.py
+-rw-rw-rw-   0        0        0     1397 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/academicearth.py
+-rw-rw-rw-   0        0        0     4542 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/acast.py
+-rw-rw-rw-   0        0        0     8111 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/acfun.py
+-rw-rw-rw-   0        0        0    11154 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/adn.py
+-rw-rw-rw-   0        0        0     1252 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/adobeconnect.py
+-rw-rw-rw-   0        0        0    54460 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/adobepass.py
+-rw-rw-rw-   0        0        0    10563 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/adobetv.py
+-rw-rw-rw-   0        0        0     7927 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/adultswim.py
+-rw-rw-rw-   0        0        0    12422 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aenetworks.py
+-rw-rw-rw-   0        0        0     1845 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aeonco.py
+-rw-rw-rw-   0        0        0    22211 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/afreecatv.py
+-rw-rw-rw-   0        0        0    10072 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/agora.py
+-rw-rw-rw-   0        0        0     2703 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/airmozilla.py
+-rw-rw-rw-   0        0        0     4181 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/airtv.py
+-rw-rw-rw-   0        0        0     3016 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aitube.py
+-rw-rw-rw-   0        0        0     1576 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aliexpress.py
+-rw-rw-rw-   0        0        0     3447 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aljazeera.py
+-rw-rw-rw-   0        0        0     4928 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/allocine.py
+-rw-rw-rw-   0        0        0     2758 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/alphaporno.py
+-rw-rw-rw-   0        0        0     3163 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/alsace20tv.py
+-rw-rw-rw-   0        0        0     6668 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/alura.py
+-rw-rw-rw-   0        0        0     3626 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/amara.py
+-rw-rw-rw-   0        0        0     6759 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/amazon.py
+-rw-rw-rw-   0        0        0    10904 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/amazonminitv.py
+-rw-rw-rw-   0        0        0     6267 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/amcnetworks.py
+-rw-rw-rw-   0        0        0     8939 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/americastestkitchen.py
+-rw-rw-rw-   0        0        0     4166 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/amp.py
+-rw-rw-rw-   0        0        0     4898 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/anchorfm.py
+-rw-rw-rw-   0        0        0     2606 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/angel.py
+-rw-rw-rw-   0        0        0     5414 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ant1newsgr.py
+-rw-rw-rw-   0        0        0    27555 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/anvato.py
+-rw-rw-rw-   0        0        0     5578 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aol.py
+-rw-rw-rw-   0        0        0     3169 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/apa.py
+-rw-rw-rw-   0        0        0     3462 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aparat.py
+-rw-rw-rw-   0        0        0     1902 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/appleconnect.py
+-rw-rw-rw-   0        0        0     3709 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/applepodcasts.py
+-rw-rw-rw-   0        0        0    10474 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/appletrailers.py
+-rw-rw-rw-   0        0        0    58664 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/archiveorg.py
+-rw-rw-rw-   0        0        0     7678 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/arcpublishing.py
+-rw-rw-rw-   0        0        0    28271 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ard.py
+-rw-rw-rw-   0        0        0     7349 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/arkena.py
+-rw-rw-rw-   0        0        0     3654 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/arnes.py
+-rw-rw-rw-   0        0        0    14310 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/arte.py
+-rw-rw-rw-   0        0        0     7878 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/asiancrush.py
+-rw-rw-rw-   0        0        0     4241 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/atresplayer.py
+-rw-rw-rw-   0        0        0     1246 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/atscaleconf.py
+-rw-rw-rw-   0        0        0     1974 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/atttechchannel.py
+-rw-rw-rw-   0        0        0     4299 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/atvat.py
+-rw-rw-rw-   0        0        0     4018 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/audimedia.py
+-rw-rw-rw-   0        0        0     2923 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/audioboom.py
+-rw-rw-rw-   0        0        0     3306 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/audiodraft.py
+-rw-rw-rw-   0        0        0     6328 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/audiomack.py
+-rw-rw-rw-   0        0        0    11044 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/audius.py
+-rw-rw-rw-   0        0        0     7317 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/awaan.py
+-rw-rw-rw-   0        0        0     3184 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aws.py
+-rw-rw-rw-   0        0        0     2490 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/azmedien.py
+-rw-rw-rw-   0        0        0     1959 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/baidu.py
+-rw-rw-rw-   0        0        0     5459 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/banbye.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bandaichannel.py
+-rw-rw-rw-   0        0        0    19082 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bandcamp.py
+-rw-rw-rw-   0        0        0     5458 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bannedvideo.py
+-rw-rw-rw-   0        0        0    73490 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bbc.py
+-rw-rw-rw-   0        0        0     4303 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/beatbump.py
+-rw-rw-rw-   0        0        0     3343 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/beatport.py
+-rw-rw-rw-   0        0        0     3235 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/beeg.py
+-rw-rw-rw-   0        0        0     1616 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/behindkink.py
+-rw-rw-rw-   0        0        0     3353 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bellmedia.py
+-rw-rw-rw-   0        0        0     3171 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/berufetv.py
+-rw-rw-rw-   0        0        0     2861 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bet.py
+-rw-rw-rw-   0        0        0     1318 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bfi.py
+-rw-rw-rw-   0        0        0     5451 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bfmtv.py
+-rw-rw-rw-   0        0        0     1072 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bibeltv.py
+-rw-rw-rw-   0        0        0     2313 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bigflix.py
+-rw-rw-rw-   0        0        0     2021 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bigo.py
+-rw-rw-rw-   0        0        0     1343 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bild.py
+-rw-rw-rw-   0        0        0    52181 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bilibili.py
+-rw-rw-rw-   0        0        0     3537 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/biobiochiletv.py
+-rw-rw-rw-   0        0        0     4832 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/biqle.py
+-rw-rw-rw-   0        0        0     9846 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bitchute.py
+-rw-rw-rw-   0        0        0     1827 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bitwave.py
+-rw-rw-rw-   0        0        0     2419 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/blackboardcollaborate.py
+-rw-rw-rw-   0        0        0     4422 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bleacherreport.py
+-rw-rw-rw-   0        0        0     4900 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/blerp.py
+-rw-rw-rw-   0        0        0     1886 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/blogger.py
+-rw-rw-rw-   0        0        0     3257 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bloomberg.py
+-rw-rw-rw-   0        0        0     1999 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bokecc.py
+-rw-rw-rw-   0        0        0     2339 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bongacams.py
+-rw-rw-rw-   0        0        0     3890 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/booyah.py
+-rw-rw-rw-   0        0        0     3204 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bostonglobe.py
+-rw-rw-rw-   0        0        0     3779 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/box.py
+-rw-rw-rw-   0        0        0     4858 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/boxcast.py
+-rw-rw-rw-   0        0        0     2070 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bpb.py
+-rw-rw-rw-   0        0        0    12183 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/br.py
+-rw-rw-rw-   0        0        0     8252 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bravotv.py
+-rw-rw-rw-   0        0        0     2944 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/breakcom.py
+-rw-rw-rw-   0        0        0     1377 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/breitbart.py
+-rw-rw-rw-   0        0        0    43629 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/brightcove.py
+-rw-rw-rw-   0        0        0     1377 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bundesliga.py
+-rw-rw-rw-   0        0        0     1986 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/businessinsider.py
+-rw-rw-rw-   0        0        0     3704 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/buzzfeed.py
+-rw-rw-rw-   0        0        0     4523 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/byutv.py
+-rw-rw-rw-   0        0        0     2016 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/c56.py
+-rw-rw-rw-   0        0        0     1155 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cableav.py
+-rw-rw-rw-   0        0        0     8278 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/callin.py
+-rw-rw-rw-   0        0        0     1599 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/caltrans.py
+-rw-rw-rw-   0        0        0     1146 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cam4.py
+-rw-rw-rw-   0        0        0     5873 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/camdemy.py
+-rw-rw-rw-   0        0        0     2903 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cammodels.py
+-rw-rw-rw-   0        0        0     2240 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/camsoda.py
+-rw-rw-rw-   0        0        0     2546 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/camtasia.py
+-rw-rw-rw-   0        0        0     3275 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/camwithher.py
+-rw-rw-rw-   0        0        0     4363 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/canalalpha.py
+-rw-rw-rw-   0        0        0     2283 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/canalc2.py
+-rw-rw-rw-   0        0        0     4473 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/canalplus.py
+-rw-rw-rw-   0        0        0    16095 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/canvas.py
+-rw-rw-rw-   0        0        0     3538 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/carambatv.py
+-rw-rw-rw-   0        0        0     2376 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cartoonnetwork.py
+-rw-rw-rw-   0        0        0    22613 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbc.py
+-rw-rw-rw-   0        0        0    12044 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbs.py
+-rw-rw-rw-   0        0        0     4111 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbsinteractive.py
+-rw-rw-rw-   0        0        0     4258 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbslocal.py
+-rw-rw-rw-   0        0        0     7765 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbsnews.py
+-rw-rw-rw-   0        0        0     4928 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbssports.py
+-rw-rw-rw-   0        0        0     3959 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ccc.py
+-rw-rw-rw-   0        0        0     5250 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ccma.py
+-rw-rw-rw-   0        0        0     7034 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cctv.py
+-rw-rw-rw-   0        0        0    14224 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cda.py
+-rw-rw-rw-   0        0        0     2900 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cellebrite.py
+-rw-rw-rw-   0        0        0    12005 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ceskatelevize.py
+-rw-rw-rw-   0        0        0     2898 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cgtn.py
+-rw-rw-rw-   0        0        0    10347 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/channel9.py
+-rw-rw-rw-   0        0        0     1792 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/charlierose.py
+-rw-rw-rw-   0        0        0     3922 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/chaturbate.py
+-rw-rw-rw-   0        0        0     4945 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/chilloutzone.py
+-rw-rw-rw-   0        0        0     8871 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/chingari.py
+-rw-rw-rw-   0        0        0     2977 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/chirbit.py
+-rw-rw-rw-   0        0        0     2056 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cinchcast.py
+-rw-rw-rw-   0        0        0      901 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cinemax.py
+-rw-rw-rw-   0        0        0     2487 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cinetecamilano.py
+-rw-rw-rw-   0        0        0     6003 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ciscolive.py
+-rw-rw-rw-   0        0        0     4543 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ciscowebex.py
+-rw-rw-rw-   0        0        0     2407 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cjsw.py
+-rw-rw-rw-   0        0        0     2532 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cliphunter.py
+-rw-rw-rw-   0        0        0     2563 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/clippit.py
+-rw-rw-rw-   0        0        0     1003 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cliprs.py
+-rw-rw-rw-   0        0        0     1823 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/clipsyndicate.py
+-rw-rw-rw-   0        0        0     3083 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/closertotruth.py
+-rw-rw-rw-   0        0        0     2441 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cloudflarestream.py
+-rw-rw-rw-   0        0        0     1898 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cloudy.py
+-rw-rw-rw-   0        0        0     1935 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/clubic.py
+-rw-rw-rw-   0        0        0     3182 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/clyp.py
+-rw-rw-rw-   0        0        0     2276 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cmt.py
+-rw-rw-rw-   0        0        0     2287 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cnbc.py
+-rw-rw-rw-   0        0        0     9369 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cnn.py
+-rw-rw-rw-   0        0        0     2196 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/comedycentral.py
+-rw-rw-rw-   0        0        0   188391 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/common.py
+-rw-rw-rw-   0        0        0     1306 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/commonmistakes.py
+-rw-rw-rw-   0        0        0     2006 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/commonprotocols.py
+-rw-rw-rw-   0        0        0     9980 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/condenast.py
+-rw-rw-rw-   0        0        0     4215 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/contv.py
+-rw-rw-rw-   0        0        0     6413 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/corus.py
+-rw-rw-rw-   0        0        0     4695 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/coub.py
+-rw-rw-rw-   0        0        0     1409 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cozytv.py
+-rw-rw-rw-   0        0        0     5837 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cpac.py
+-rw-rw-rw-   0        0        0     3185 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cracked.py
+-rw-rw-rw-   0        0        0     9921 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/crackle.py
+-rw-rw-rw-   0        0        0     2805 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/craftsy.py
+-rw-rw-rw-   0        0        0     2179 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/crooksandliars.py
+-rw-rw-rw-   0        0        0     4271 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/crowdbunker.py
+-rw-rw-rw-   0        0        0    15216 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/crunchyroll.py
+-rw-rw-rw-   0        0        0    12391 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cspan.py
+-rw-rw-rw-   0        0        0     3675 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ctsnews.py
+-rw-rw-rw-   0        0        0     1764 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ctv.py
+-rw-rw-rw-   0        0        0     2624 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ctvnews.py
+-rw-rw-rw-   0        0        0     2520 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cultureunplugged.py
+-rw-rw-rw-   0        0        0     8594 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/curiositystream.py
+-rw-rw-rw-   0        0        0     3937 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cwtv.py
+-rw-rw-rw-   0        0        0     6438 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cybrary.py
+-rw-rw-rw-   0        0        0     5960 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/daftsex.py
+-rw-rw-rw-   0        0        0     3016 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dailymail.py
+-rw-rw-rw-   0        0        0    16331 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dailymotion.py
+-rw-rw-rw-   0        0        0     4967 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dailywire.py
+-rw-rw-rw-   0        0        0     5642 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/damtomo.py
+-rw-rw-rw-   0        0        0     9679 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/daum.py
+-rw-rw-rw-   0        0        0     2035 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/daystar.py
+-rw-rw-rw-   0        0        0     1826 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dbtv.py
+-rw-rw-rw-   0        0        0     3633 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dctp.py
+-rw-rw-rw-   0        0        0     5296 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/deezer.py
+-rw-rw-rw-   0        0        0     1238 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/defense.py
+-rw-rw-rw-   0        0        0     3098 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/democracynow.py
+-rw-rw-rw-   0        0        0     8247 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/detik.py
+-rw-rw-rw-   0        0        0     3271 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/deuxm.py
+-rw-rw-rw-   0        0        0     2215 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dfb.py
+-rw-rw-rw-   0        0        0     2107 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dhm.py
+-rw-rw-rw-   0        0        0     1895 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/digg.py
+-rw-rw-rw-   0        0        0     5837 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/digitalconcerthall.py
+-rw-rw-rw-   0        0        0     3355 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/digiteka.py
+-rw-rw-rw-   0        0        0     4958 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/discovery.py
+-rw-rw-rw-   0        0        0     6174 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/discoverygo.py
+-rw-rw-rw-   0        0        0     6930 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/disney.py
+-rw-rw-rw-   0        0        0     5073 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dispeak.py
+-rw-rw-rw-   0        0        0     3068 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dlive.py
+-rw-rw-rw-   0        0        0     3119 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dotsub.py
+-rw-rw-rw-   0        0        0     7417 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/douyutv.py
+-rw-rw-rw-   0        0        0    39956 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dplay.py
+-rw-rw-rw-   0        0        0     1935 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/drbonanza.py
+-rw-rw-rw-   0        0        0     1655 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dreisat.py
+-rw-rw-rw-   0        0        0     4300 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/drooble.py
+-rw-rw-rw-   0        0        0     3406 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dropbox.py
+-rw-rw-rw-   0        0        0     9856 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dropout.py
+-rw-rw-rw-   0        0        0     3900 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/drtuber.py
+-rw-rw-rw-   0        0        0    20606 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/drtv.py
+-rw-rw-rw-   0        0        0     2806 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dtube.py
+-rw-rw-rw-   0        0        0     8510 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/duboku.py
+-rw-rw-rw-   0        0        0     2684 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dumpert.py
+-rw-rw-rw-   0        0        0     7612 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dvtv.py
+-rw-rw-rw-   0        0        0     4112 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dw.py
+-rw-rw-rw-   0        0        0     8399 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eagleplatform.py
+-rw-rw-rw-   0        0        0     1076 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ebaumsworld.py
+-rw-rw-rw-   0        0        0     1308 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ebay.py
+-rw-rw-rw-   0        0        0     1303 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/echomsk.py
+-rw-rw-rw-   0        0        0     5070 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/egghead.py
+-rw-rw-rw-   0        0        0     1513 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ehow.py
+-rw-rw-rw-   0        0        0     5972 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eighttracks.py
+-rw-rw-rw-   0        0        0     3717 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/einthusan.py
+-rw-rw-rw-   0        0        0     3267 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eitb.py
+-rw-rw-rw-   0        0        0     5007 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ellentube.py
+-rw-rw-rw-   0        0        0     2649 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/elonet.py
+-rw-rw-rw-   0        0        0     4399 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/elpais.py
+-rw-rw-rw-   0        0        0     5413 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/embedly.py
+-rw-rw-rw-   0        0        0      453 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/engadget.py
+-rw-rw-rw-   0        0        0     4310 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/epicon.py
+-rw-rw-rw-   0        0        0     2568 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/epoch.py
+-rw-rw-rw-   0        0        0     4688 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eporner.py
+-rw-rw-rw-   0        0        0     4589 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eroprofile.py
+-rw-rw-rw-   0        0        0    12922 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ertgr.py
+-rw-rw-rw-   0        0        0     3653 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/escapist.py
+-rw-rw-rw-   0        0        0    17639 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/espn.py
+-rw-rw-rw-   0        0        0     2605 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/esri.py
+-rw-rw-rw-   0        0        0     6610 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/europa.py
+-rw-rw-rw-   0        0        0     1299 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/europeantour.py
+-rw-rw-rw-   0        0        0     5181 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eurosport.py
+-rw-rw-rw-   0        0        0     3385 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/euscreen.py
+-rw-rw-rw-   0        0        0     2910 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/expotv.py
+-rw-rw-rw-   0        0        0     3837 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/expressen.py
+-rw-rw-rw-   0        0        0      870 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/extractors.py
+-rw-rw-rw-   0        0        0     1795 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/extremetube.py
+-rw-rw-rw-   0        0        0     2691 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eyedotv.py
+-rw-rw-rw-   0        0        0    36232 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/facebook.py
+-rw-rw-rw-   0        0        0     7355 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fancode.py
+-rw-rw-rw-   0        0        0     3582 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/faz.py
+-rw-rw-rw-   0        0        0    11256 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fc2.py
+-rw-rw-rw-   0        0        0     1717 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fczenit.py
+-rw-rw-rw-   0        0        0     3926 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fifa.py
+-rw-rw-rw-   0        0        0     2623 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/filmmodu.py
+-rw-rw-rw-   0        0        0     6053 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/filmon.py
+-rw-rw-rw-   0        0        0     1461 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/filmweb.py
+-rw-rw-rw-   0        0        0     6513 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/firsttv.py
+-rw-rw-rw-   0        0        0     3130 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fivetv.py
+-rw-rw-rw-   0        0        0     4815 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/flickr.py
+-rw-rw-rw-   0        0        0     2623 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/folketinget.py
+-rw-rw-rw-   0        0        0     1871 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/footyroom.py
+-rw-rw-rw-   0        0        0      962 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/formula1.py
+-rw-rw-rw-   0        0        0    11807 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fourtube.py
+-rw-rw-rw-   0        0        0     4988 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fourzerostudio.py
+-rw-rw-rw-   0        0        0     6800 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fox.py
+-rw-rw-rw-   0        0        0     1447 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fox9.py
+-rw-rw-rw-   0        0        0     2123 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/foxgay.py
+-rw-rw-rw-   0        0        0     6309 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/foxnews.py
+-rw-rw-rw-   0        0        0     2263 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/foxsports.py
+-rw-rw-rw-   0        0        0     4965 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fptplay.py
+-rw-rw-rw-   0        0        0     2214 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/franceinter.py
+-rw-rw-rw-   0        0        0    15517 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/francetv.py
+-rw-rw-rw-   0        0        0     2581 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/freesound.py
+-rw-rw-rw-   0        0        0     1045 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/freespeech.py
+-rw-rw-rw-   0        0        0     5668 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/freetv.py
+-rw-rw-rw-   0        0        0     8849 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/frontendmasters.py
+-rw-rw-rw-   0        0        0     3205 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fujitv.py
+-rw-rw-rw-   0        0        0    15291 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/funimation.py
+-rw-rw-rw-   0        0        0     1691 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/funk.py
+-rw-rw-rw-   0        0        0     3168 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fusion.py
+-rw-rw-rw-   0        0        0     1041 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fuyintv.py
+-rw-rw-rw-   0        0        0     5849 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gab.py
+-rw-rw-rw-   0        0        0     4626 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gaia.py
+-rw-rw-rw-   0        0        0     2111 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gameinformer.py
+-rw-rw-rw-   0        0        0    25720 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gamejolt.py
+-rw-rw-rw-   0        0        0     3153 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gamespot.py
+-rw-rw-rw-   0        0        0     2612 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gamestar.py
+-rw-rw-rw-   0        0        0     3838 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gaskrank.py
+-rw-rw-rw-   0        0        0     1926 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gazeta.py
+-rw-rw-rw-   0        0        0     8769 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gdcvault.py
+-rw-rw-rw-   0        0        0     8720 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gedidigital.py
+-rw-rw-rw-   0        0        0   122559 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/generic.py
+-rw-rw-rw-   0        0        0     4722 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/genericembeds.py
+-rw-rw-rw-   0        0        0     6248 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/genius.py
+-rw-rw-rw-   0        0        0     8051 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gettr.py
+-rw-rw-rw-   0        0        0     5254 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gfycat.py
+-rw-rw-rw-   0        0        0     3049 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/giantbomb.py
+-rw-rw-rw-   0        0        0     3815 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/giga.py
+-rw-rw-rw-   0        0        0      656 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gigya.py
+-rw-rw-rw-   0        0        0     1417 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/glide.py
+-rw-rw-rw-   0        0        0    10366 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/globo.py
+-rw-rw-rw-   0        0        0     8733 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/glomex.py
+-rw-rw-rw-   0        0        0    14476 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/go.py
+-rw-rw-rw-   0        0        0     1784 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/godtube.py
+-rw-rw-rw-   0        0        0     3627 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gofile.py
+-rw-rw-rw-   0        0        0     2184 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/golem.py
+-rw-rw-rw-   0        0        0     2368 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/goodgame.py
+-rw-rw-rw-   0        0        0    14873 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/googledrive.py
+-rw-rw-rw-   0        0        0     3425 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/googlepodcasts.py
+-rw-rw-rw-   0        0        0     1201 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/googlesearch.py
+-rw-rw-rw-   0        0        0    15803 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/goplay.py
+-rw-rw-rw-   0        0        0     3891 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gopro.py
+-rw-rw-rw-   0        0        0     1533 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/goshgay.py
+-rw-rw-rw-   0        0        0     2797 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gotostage.py
+-rw-rw-rw-   0        0        0     1176 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gputechconf.py
+-rw-rw-rw-   0        0        0     4057 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gronkh.py
+-rw-rw-rw-   0        0        0     2623 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/groupon.py
+-rw-rw-rw-   0        0        0     2930 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/harpodeon.py
+-rw-rw-rw-   0        0        0     6206 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hbo.py
+-rw-rw-rw-   0        0        0     3585 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hearthisat.py
+-rw-rw-rw-   0        0        0     8639 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/heise.py
+-rw-rw-rw-   0        0        0     2655 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hellporno.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/helsinki.py
+-rw-rw-rw-   0        0        0     1197 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hentaistigma.py
+-rw-rw-rw-   0        0        0     1415 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hgtv.py
+-rw-rw-rw-   0        0        0     5064 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hidive.py
+-rw-rw-rw-   0        0        0     1585 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/historicfilms.py
+-rw-rw-rw-   0        0        0     7533 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hitbox.py
+-rw-rw-rw-   0        0        0     2294 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hitrecord.py
+-rw-rw-rw-   0        0        0     7059 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hketv.py
+-rw-rw-rw-   0        0        0     2943 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hollywoodreporter.py
+-rw-rw-rw-   0        0        0     4367 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/holodex.py
+-rw-rw-rw-   0        0        0     2306 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hotnewhiphop.py
+-rw-rw-rw-   0        0        0    15404 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hotstar.py
+-rw-rw-rw-   0        0        0     1370 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/howcast.py
+-rw-rw-rw-   0        0        0     3473 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/howstuffworks.py
+-rw-rw-rw-   0        0        0     3935 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hrfensehen.py
+-rw-rw-rw-   0        0        0     7237 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hrti.py
+-rw-rw-rw-   0        0        0     3693 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hse.py
+-rw-rw-rw-   0        0        0     1846 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/huajiao.py
+-rw-rw-rw-   0        0        0     3387 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/huffpost.py
+-rw-rw-rw-   0        0        0     5353 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hungama.py
+-rw-rw-rw-   0        0        0     4996 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/huya.py
+-rw-rw-rw-   0        0        0     1557 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hypem.py
+-rw-rw-rw-   0        0        0     1249 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hypergryph.py
+-rw-rw-rw-   0        0        0     2257 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hytale.py
+-rw-rw-rw-   0        0        0     7570 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/icareus.py
+-rw-rw-rw-   0        0        0     5947 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ichinanalive.py
+-rw-rw-rw-   0        0        0    16931 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ign.py
+-rw-rw-rw-   0        0        0     3502 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/iheart.py
+-rw-rw-rw-   0        0        0     2380 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/iltalehti.py
+-rw-rw-rw-   0        0        0     5780 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/imdb.py
+-rw-rw-rw-   0        0        0     4942 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/imggaming.py
+-rw-rw-rw-   0        0        0     5217 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/imgur.py
+-rw-rw-rw-   0        0        0     3701 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ina.py
+-rw-rw-rw-   0        0        0     2315 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/inc.py
+-rw-rw-rw-   0        0        0     4335 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/indavideo.py
+-rw-rw-rw-   0        0        0     5248 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/infoq.py
+-rw-rw-rw-   0        0        0    31463 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/instagram.py
+-rw-rw-rw-   0        0        0     3178 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/internazionale.py
+-rw-rw-rw-   0        0        0     2319 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/internetvideoarchive.py
+-rw-rw-rw-   0        0        0    10848 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/iprima.py
+-rw-rw-rw-   0        0        0    31574 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/iqiyi.py
+-rw-rw-rw-   0        0        0     3258 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/islamchannel.py
+-rw-rw-rw-   0        0        0     2209 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/israelnationalnews.py
+-rw-rw-rw-   0        0        0     5477 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/itprotv.py
+-rw-rw-rw-   0        0        0    10948 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/itv.py
+-rw-rw-rw-   0        0        0    10305 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ivi.py
+-rw-rw-rw-   0        0        0     3205 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ivideon.py
+-rw-rw-rw-   0        0        0     7062 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/iwara.py
+-rw-rw-rw-   0        0        0     3509 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ixigua.py
+-rw-rw-rw-   0        0        0     4172 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/izlesene.py
+-rw-rw-rw-   0        0        0     4108 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jable.py
+-rw-rw-rw-   0        0        0     8112 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jamendo.py
+-rw-rw-rw-   0        0        0    10625 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/japandiet.py
+-rw-rw-rw-   0        0        0     2018 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jeuxvideo.py
+-rw-rw-rw-   0        0        0     2245 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jixie.py
+-rw-rw-rw-   0        0        0     3973 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/joj.py
+-rw-rw-rw-   0        0        0     3095 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jove.py
+-rw-rw-rw-   0        0        0     3976 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jwplatform.py
+-rw-rw-rw-   0        0        0     6052 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kakao.py
+-rw-rw-rw-   0        0        0    24874 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kaltura.py
+-rw-rw-rw-   0        0        0     2743 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kanal2.py
+-rw-rw-rw-   0        0        0     1838 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kankanews.py
+-rw-rw-rw-   0        0        0     2344 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/karaoketv.py
+-rw-rw-rw-   0        0        0     3418 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/karrierevideos.py
+-rw-rw-rw-   0        0        0     4665 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/keezmovies.py
+-rw-rw-rw-   0        0        0     3547 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kelbyone.py
+-rw-rw-rw-   0        0        0     2555 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ketnet.py
+-rw-rw-rw-   0        0        0     4213 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/khanacademy.py
+-rw-rw-rw-   0        0        0     5581 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kick.py
+-rw-rw-rw-   0        0        0     2359 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kicker.py
+-rw-rw-rw-   0        0        0     2719 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kickstarter.py
+-rw-rw-rw-   0        0        0     8401 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kinja.py
+-rw-rw-rw-   0        0        0     2131 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kinopoisk.py
+-rw-rw-rw-   0        0        0     1123 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kommunetv.py
+-rw-rw-rw-   0        0        0     1112 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kompas.py
+-rw-rw-rw-   0        0        0     4530 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/konserthusetplay.py
+-rw-rw-rw-   0        0        0     4799 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/koo.py
+-rw-rw-rw-   0        0        0     1957 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/krasview.py
+-rw-rw-rw-   0        0        0     1031 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kth.py
+-rw-rw-rw-   0        0        0      981 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ku6.py
+-rw-rw-rw-   0        0        0     3053 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kusi.py
+-rw-rw-rw-   0        0        0    12749 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kuwo.py
+-rw-rw-rw-   0        0        0     9675 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/la7.py
+-rw-rw-rw-   0        0        0     9583 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/laola1tv.py
+-rw-rw-rw-   0        0        0     4877 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lastfm.py
+-rw-rw-rw-   0        0        0    14567 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lbry.py
+-rw-rw-rw-   0        0        0     1321 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lci.py
+-rw-rw-rw-   0        0        0     3024 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lcp.py
+-rw-rw-rw-   0        0        0     2374 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lecture2go.py
+-rw-rw-rw-   0        0        0     8440 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lecturio.py
+-rw-rw-rw-   0        0        0    13357 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/leeco.py
+-rw-rw-rw-   0        0        0     5523 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lefigaro.py
+-rw-rw-rw-   0        0        0     6032 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lego.py
+-rw-rw-rw-   0        0        0     2344 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lemonde.py
+-rw-rw-rw-   0        0        0     1675 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lenta.py
+-rw-rw-rw-   0        0        0     5083 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/libraryofcongress.py
+-rw-rw-rw-   0        0        0     3762 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/libsyn.py
+-rw-rw-rw-   0        0        0     9758 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lifenews.py
+-rw-rw-rw-   0        0        0     7611 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/likee.py
+-rw-rw-rw-   0        0        0    15352 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/limelight.py
+-rw-rw-rw-   0        0        0     5569 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/line.py
+-rw-rw-rw-   0        0        0    10180 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/linkedin.py
+-rw-rw-rw-   0        0        0     9979 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/linuxacademy.py
+-rw-rw-rw-   0        0        0     3195 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/liputan6.py
+-rw-rw-rw-   0        0        0     4253 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/listennotes.py
+-rw-rw-rw-   0        0        0     5863 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/litv.py
+-rw-rw-rw-   0        0        0     1512 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/livejournal.py
+-rw-rw-rw-   0        0        0    13938 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/livestream.py
+-rw-rw-rw-   0        0        0     1603 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/livestreamfails.py
+-rw-rw-rw-   0        0        0     6481 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lnkgo.py
+-rw-rw-rw-   0        0        0     1698 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/localnews8.py
+-rw-rw-rw-   0        0        0     1163 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lovehomeporn.py
+-rw-rw-rw-   0        0        0     4146 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lrt.py
+-rw-rw-rw-   0        0        0     1105 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lumni.py
+-rw-rw-rw-   0        0        0    12776 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lynda.py
+-rw-rw-rw-   0        0        0      861 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/m6.py
+-rw-rw-rw-   0        0        0     3498 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/magentamusik360.py
+-rw-rw-rw-   0        0        0    12360 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mailru.py
+-rw-rw-rw-   0        0        0     9444 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mainstreaming.py
+-rw-rw-rw-   0        0        0     4391 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/malltv.py
+-rw-rw-rw-   0        0        0     2541 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mangomolo.py
+-rw-rw-rw-   0        0        0     5281 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/manoto.py
+-rw-rw-rw-   0        0        0     6086 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/manyvids.py
+-rw-rw-rw-   0        0        0     1206 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/maoritv.py
+-rw-rw-rw-   0        0        0     4587 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/markiza.py
+-rw-rw-rw-   0        0        0     2643 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/massengeschmacktv.py
+-rw-rw-rw-   0        0        0     1526 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/masters.py
+-rw-rw-rw-   0        0        0     1751 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/matchtv.py
+-rw-rw-rw-   0        0        0     7020 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mdr.py
+-rw-rw-rw-   0        0        0     6192 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/medaltv.py
+-rw-rw-rw-   0        0        0     4311 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediaite.py
+-rw-rw-rw-   0        0        0     4434 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediaklikk.py
+-rw-rw-rw-   0        0        0     4233 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/medialaan.py
+-rw-rw-rw-   0        0        0    13471 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediaset.py
+-rw-rw-rw-   0        0        0    17033 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediasite.py
+-rw-rw-rw-   0        0        0     9681 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediastream.py
+-rw-rw-rw-   0        0        0     4181 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediaworksnz.py
+-rw-rw-rw-   0        0        0     2308 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/medici.py
+-rw-rw-rw-   0        0        0     1650 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/megaphone.py
+-rw-rw-rw-   0        0        0     6875 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/megatvcom.py
+-rw-rw-rw-   0        0        0     3636 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/meipai.py
+-rw-rw-rw-   0        0        0     2226 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/melonvod.py
+-rw-rw-rw-   0        0        0     2636 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/meta.py
+-rw-rw-rw-   0        0        0    11888 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/metacafe.py
+-rw-rw-rw-   0        0        0     2656 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/metacritic.py
+-rw-rw-rw-   0        0        0     2669 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mgoon.py
+-rw-rw-rw-   0        0        0     5715 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mgtv.py
+-rw-rw-rw-   0        0        0     1429 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/miaopai.py
+-rw-rw-rw-   0        0        0     2782 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/microsoftembed.py
+-rw-rw-rw-   0        0        0     5510 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/microsoftstream.py
+-rw-rw-rw-   0        0        0     7495 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/microsoftvirtualacademy.py
+-rw-rw-rw-   0        0        0    11842 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mildom.py
+-rw-rw-rw-   0        0        0     7027 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/minds.py
+-rw-rw-rw-   0        0        0     2181 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ministrygrid.py
+-rw-rw-rw-   0        0        0     1856 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/minoto.py
+-rw-rw-rw-   0        0        0     5149 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/miomio.py
+-rw-rw-rw-   0        0        0     4998 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mirrativ.py
+-rw-rw-rw-   0        0        0     4501 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mirrorcouk.py
+-rw-rw-rw-   0        0        0     5295 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mit.py
+-rw-rw-rw-   0        0        0     3286 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mitele.py
+-rw-rw-rw-   0        0        0     3049 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mixch.py
+-rw-rw-rw-   0        0        0    12517 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mixcloud.py
+-rw-rw-rw-   0        0        0    15061 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mlb.py
+-rw-rw-rw-   0        0        0     6810 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mlssoccer.py
+-rw-rw-rw-   0        0        0     2917 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mnet.py
+-rw-rw-rw-   0        0        0     3020 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mocha.py
+-rw-rw-rw-   0        0        0     2837 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/moevideo.py
+-rw-rw-rw-   0        0        0     2733 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mofosex.py
+-rw-rw-rw-   0        0        0     2026 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mojvideo.py
+-rw-rw-rw-   0        0        0     1835 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/morningstar.py
+-rw-rw-rw-   0        0        0    10072 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/motherless.py
+-rw-rw-rw-   0        0        0     2040 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/motorsport.py
+-rw-rw-rw-   0        0        0     1880 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/movieclips.py
+-rw-rw-rw-   0        0        0     3656 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/moviepilot.py
+-rw-rw-rw-   0        0        0     1682 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/moview.py
+-rw-rw-rw-   0        0        0     1329 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/moviezine.py
+-rw-rw-rw-   0        0        0     1783 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/movingimage.py
+-rw-rw-rw-   0        0        0     7647 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/msn.py
+-rw-rw-rw-   0        0        0    26160 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mtv.py
+-rw-rw-rw-   0        0        0     2131 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/muenchentv.py
+-rw-rw-rw-   0        0        0     5155 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/murrtube.py
+-rw-rw-rw-   0        0        0     2719 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/musescore.py
+-rw-rw-rw-   0        0        0     7341 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/musicdex.py
+-rw-rw-rw-   0        0        0     3289 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mwave.py
+-rw-rw-rw-   0        0        0    10248 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mxplayer.py
+-rw-rw-rw-   0        0        0     1553 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mychannels.py
+-rw-rw-rw-   0        0        0     7960 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/myspace.py
+-rw-rw-rw-   0        0        0     3806 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/myspass.py
+-rw-rw-rw-   0        0        0     3915 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/myvi.py
+-rw-rw-rw-   0        0        0     3416 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/myvideoge.py
+-rw-rw-rw-   0        0        0      904 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/myvidster.py
+-rw-rw-rw-   0        0        0     5523 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/n1.py
+-rw-rw-rw-   0        0        0     4423 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nate.py
+-rw-rw-rw-   0        0        0     3004 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nationalgeographic.py
+-rw-rw-rw-   0        0        0    16318 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/naver.py
+-rw-rw-rw-   0        0        0    16572 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nba.py
+-rw-rw-rw-   0        0        0    33537 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nbc.py
+-rw-rw-rw-   0        0        0    18703 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ndr.py
+-rw-rw-rw-   0        0        0     4587 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ndtv.py
+-rw-rw-rw-   0        0        0    12421 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nebula.py
+-rw-rw-rw-   0        0        0     1107 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nerdcubed.py
+-rw-rw-rw-   0        0        0    20131 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/neteasemusic.py
+-rw-rw-rw-   0        0        0    11267 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/netverse.py
+-rw-rw-rw-   0        0        0     2985 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/netzkino.py
+-rw-rw-rw-   0        0        0    10185 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/newgrounds.py
+-rw-rw-rw-   0        0        0     2141 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/newspicks.py
+-rw-rw-rw-   0        0        0     2986 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/newstube.py
+-rw-rw-rw-   0        0        0     1877 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/newsy.py
+-rw-rw-rw-   0        0        0     9235 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nextmedia.py
+-rw-rw-rw-   0        0        0    21718 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nexx.py
+-rw-rw-rw-   0        0        0     2351 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nfb.py
+-rw-rw-rw-   0        0        0     6000 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nfhsnetwork.py
+-rw-rw-rw-   0        0        0    12678 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nfl.py
+-rw-rw-rw-   0        0        0    13471 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nhk.py
+-rw-rw-rw-   0        0        0     5035 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nhl.py
+-rw-rw-rw-   0        0        0    11474 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nick.py
+-rw-rw-rw-   0        0        0    37235 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/niconico.py
+-rw-rw-rw-   0        0        0     5265 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ninecninemedia.py
+-rw-rw-rw-   0        0        0     5326 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ninegag.py
+-rw-rw-rw-   0        0        0     5420 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ninenow.py
+-rw-rw-rw-   0        0        0     1882 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nintendo.py
+-rw-rw-rw-   0        0        0    12954 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nitter.py
+-rw-rw-rw-   0        0        0     3191 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/njpwworld.py
+-rw-rw-rw-   0        0        0     2088 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nobelprize.py
+-rw-rw-rw-   0        0        0     5172 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/noice.py
+-rw-rw-rw-   0        0        0     1146 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nonktube.py
+-rw-rw-rw-   0        0        0     2639 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/noodlemagazine.py
+-rw-rw-rw-   0        0        0     3702 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/noovo.py
+-rw-rw-rw-   0        0        0     2175 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/normalboots.py
+-rw-rw-rw-   0        0        0     5932 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nosnl.py
+-rw-rw-rw-   0        0        0     2495 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nosvideo.py
+-rw-rw-rw-   0        0        0    13114 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nova.py
+-rw-rw-rw-   0        0        0     3165 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/novaplay.py
+-rw-rw-rw-   0        0        0     6107 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nowness.py
+-rw-rw-rw-   0        0        0     3613 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/noz.py
+-rw-rw-rw-   0        0        0    22896 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/npo.py
+-rw-rw-rw-   0        0        0     5872 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/npr.py
+-rw-rw-rw-   0        0        0    33058 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nrk.py
+-rw-rw-rw-   0        0        0      958 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nrl.py
+-rw-rw-rw-   0        0        0     2332 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ntvcojp.py
+-rw-rw-rw-   0        0        0     3172 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ntvde.py
+-rw-rw-rw-   0        0        0     5675 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ntvru.py
+-rw-rw-rw-   0        0        0     4589 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nubilesporn.py
+-rw-rw-rw-   0        0        0     1188 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nuevo.py
+-rw-rw-rw-   0        0        0     3631 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nuvid.py
+-rw-rw-rw-   0        0        0    10706 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nytimes.py
+-rw-rw-rw-   0        0        0     6019 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nzherald.py
+-rw-rw-rw-   0        0        0     4047 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nzonscreen.py
+-rw-rw-rw-   0        0        0     1392 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nzz.py
+-rw-rw-rw-   0        0        0     1487 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/odatv.py
+-rw-rw-rw-   0        0        0     4367 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/odkmedia.py
+-rw-rw-rw-   0        0        0    16622 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/odnoklassniki.py
+-rw-rw-rw-   0        0        0     1960 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/oftv.py
+-rw-rw-rw-   0        0        0     1473 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/oktoberfesttv.py
+-rw-rw-rw-   0        0        0     2933 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/olympics.py
+-rw-rw-rw-   0        0        0     4011 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/on24.py
+-rw-rw-rw-   0        0        0     2224 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/once.py
+-rw-rw-rw-   0        0        0     3424 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ondemandkorea.py
+-rw-rw-rw-   0        0        0     2152 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/onefootball.py
+-rw-rw-rw-   0        0        0     5247 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/onenewsnz.py
+-rw-rw-rw-   0        0        0     1885 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/oneplace.py
+-rw-rw-rw-   0        0        0    10104 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/onet.py
+-rw-rw-rw-   0        0        0     1774 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/onionstudios.py
+-rw-rw-rw-   0        0        0    10297 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ooyala.py
+-rw-rw-rw-   0        0        0     8167 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/opencast.py
+-rw-rw-rw-   0        0        0     8890 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/openload.py
+-rw-rw-rw-   0        0        0     6139 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/openrec.py
+-rw-rw-rw-   0        0        0     3197 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ora.py
+-rw-rw-rw-   0        0        0    20441 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/orf.py
+-rw-rw-rw-   0        0        0      963 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/outsidetv.py
+-rw-rw-rw-   0        0        0     6344 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/packtpub.py
+-rw-rw-rw-   0        0        0     4598 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/palcomp3.py
+-rw-rw-rw-   0        0        0     4766 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pandoratv.py
+-rw-rw-rw-   0        0        0    26404 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/panopto.py
+-rw-rw-rw-   0        0        0     7684 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/paramountplus.py
+-rw-rw-rw-   0        0        0     3892 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/parler.py
+-rw-rw-rw-   0        0        0     2816 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/parlview.py
+-rw-rw-rw-   0        0        0    19798 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/patreon.py
+-rw-rw-rw-   0        0        0    36838 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pbs.py
+-rw-rw-rw-   0        0        0     2560 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pearvideo.py
+-rw-rw-rw-   0        0        0     7500 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/peekvids.py
+-rw-rw-rw-   0        0        0    67249 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/peertube.py
+-rw-rw-rw-   0        0        0     2226 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/peertv.py
+-rw-rw-rw-   0        0        0     9062 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/peloton.py
+-rw-rw-rw-   0        0        0     1112 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/people.py
+-rw-rw-rw-   0        0        0     3323 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/performgroup.py
+-rw-rw-rw-   0        0        0     7090 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/periscope.py
+-rw-rw-rw-   0        0        0     2006 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pgatour.py
+-rw-rw-rw-   0        0        0     4165 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/philharmoniedeparis.py
+-rw-rw-rw-   0        0        0     5091 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/phoenix.py
+-rw-rw-rw-   0        0        0     1776 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/photobucket.py
+-rw-rw-rw-   0        0        0     4294 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/piapro.py
+-rw-rw-rw-   0        0        0     3897 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/picarto.py
+-rw-rw-rw-   0        0        0     6949 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/piksel.py
+-rw-rw-rw-   0        0        0     3446 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pinkbike.py
+-rw-rw-rw-   0        0        0     9843 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pinterest.py
+-rw-rw-rw-   0        0        0     4870 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pixivsketch.py
+-rw-rw-rw-   0        0        0     5094 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pladform.py
+-rw-rw-rw-   0        0        0     3033 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/planetmarathi.py
+-rw-rw-rw-   0        0        0     7622 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/platzi.py
+-rw-rw-rw-   0        0        0     2597 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playfm.py
+-rw-rw-rw-   0        0        0     3744 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playplustv.py
+-rw-rw-rw-   0        0        0     1797 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/plays.py
+-rw-rw-rw-   0        0        0     2276 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playstuff.py
+-rw-rw-rw-   0        0        0     5279 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playsuisse.py
+-rw-rw-rw-   0        0        0     7300 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playtvak.py
+-rw-rw-rw-   0        0        0     3216 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playvid.py
+-rw-rw-rw-   0        0        0     2495 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playwire.py
+-rw-rw-rw-   0        0        0    18866 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pluralsight.py
+-rw-rw-rw-   0        0        0     8266 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/plutotv.py
+-rw-rw-rw-   0        0        0     2787 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/podbayfm.py
+-rw-rw-rw-   0        0        0     3842 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/podchaser.py
+-rw-rw-rw-   0        0        0     2658 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/podomatic.py
+-rw-rw-rw-   0        0        0     5611 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pokemon.py
+-rw-rw-rw-   0        0        0     4286 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pokergo.py
+-rw-rw-rw-   0        0        0     3242 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/polsatgo.py
+-rw-rw-rw-   0        0        0    21467 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/polskieradio.py
+-rw-rw-rw-   0        0        0     3349 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/popcorntimes.py
+-rw-rw-rw-   0        0        0     2702 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/popcorntv.py
+-rw-rw-rw-   0        0        0     4142 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/porn91.py
+-rw-rw-rw-   0        0        0     3889 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/porncom.py
+-rw-rw-rw-   0        0        0     1779 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornez.py
+-rw-rw-rw-   0        0        0     3577 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornflip.py
+-rw-rw-rw-   0        0        0     4654 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornhd.py
+-rw-rw-rw-   0        0        0    31978 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornhub.py
+-rw-rw-rw-   0        0        0     3196 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornotube.py
+-rw-rw-rw-   0        0        0     3997 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornovoisines.py
+-rw-rw-rw-   0        0        0     1937 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornoxo.py
+-rw-rw-rw-   0        0        0     3567 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pr0gramm.py
+-rw-rw-rw-   0        0        0     2841 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/prankcast.py
+-rw-rw-rw-   0        0        0     1874 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/premiershiprugby.py
+-rw-rw-rw-   0        0        0     2387 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/presstv.py
+-rw-rw-rw-   0        0        0     2471 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/projectveritas.py
+-rw-rw-rw-   0        0        0    21989 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/prosiebensat1.py
+-rw-rw-rw-   0        0        0    16493 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/prx.py
+-rw-rw-rw-   0        0        0     8600 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/puhutv.py
+-rw-rw-rw-   0        0        0     2292 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/puls4.py
+-rw-rw-rw-   0        0        0     2789 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pyvideo.py
+-rw-rw-rw-   0        0        0     1957 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/qingting.py
+-rw-rw-rw-   0        0        0    13915 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/qqmusic.py
+-rw-rw-rw-   0        0        0     4615 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/r7.py
+-rw-rw-rw-   0        0        0     9200 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiko.py
+-rw-rw-rw-   0        0        0     2432 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiobremen.py
+-rw-rw-rw-   0        0        0     6406 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiocanada.py
+-rw-rw-rw-   0        0        0     1774 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiode.py
+-rw-rw-rw-   0        0        0     4932 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiofrance.py
+-rw-rw-rw-   0        0        0     2764 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiojavan.py
+-rw-rw-rw-   0        0        0     3461 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiokapital.py
+-rw-rw-rw-   0        0        0     2229 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiozet.py
+-rw-rw-rw-   0        0        0     7246 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radlive.py
+-rw-rw-rw-   0        0        0    33133 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rai.py
+-rw-rw-rw-   0        0        0     6301 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/raywenderlich.py
+-rw-rw-rw-   0        0        0     3305 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rbgtum.py
+-rw-rw-rw-   0        0        0     2418 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rbmaradio.py
+-rw-rw-rw-   0        0        0    16592 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rcs.py
+-rw-rw-rw-   0        0        0    16846 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rcti.py
+-rw-rw-rw-   0        0        0     2891 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rds.py
+-rw-rw-rw-   0        0        0    14938 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/redbee.py
+-rw-rw-rw-   0        0        0     9485 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/redbulltv.py
+-rw-rw-rw-   0        0        0    11363 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/reddit.py
+-rw-rw-rw-   0        0        0     9762 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/redgifs.py
+-rw-rw-rw-   0        0        0     6217 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/redtube.py
+-rw-rw-rw-   0        0        0     2263 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/regiotv.py
+-rw-rw-rw-   0        0        0     4165 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rentv.py
+-rw-rw-rw-   0        0        0     1298 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/restudy.py
+-rw-rw-rw-   0        0        0     2410 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/reuters.py
+-rw-rw-rw-   0        0        0     1637 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/reverbnation.py
+-rw-rw-rw-   0        0        0     4595 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rice.py
+-rw-rw-rw-   0        0        0     2850 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rmcdecouverte.py
+-rw-rw-rw-   0        0        0     2218 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rockstargames.py
+-rw-rw-rw-   0        0        0    21546 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rokfin.py
+-rw-rw-rw-   0        0        0     9066 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/roosterteeth.py
+-rw-rw-rw-   0        0        0     1270 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rottentomatoes.py
+-rw-rw-rw-   0        0        0     8912 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rozhlas.py
+-rw-rw-rw-   0        0        0     6357 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rte.py
+-rw-rw-rw-   0        0        0     7280 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtl2.py
+-rw-rw-rw-   0        0        0    12416 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtlnl.py
+-rw-rw-rw-   0        0        0     7841 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtnews.py
+-rw-rw-rw-   0        0        0     3468 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtp.py
+-rw-rw-rw-   0        0        0     2821 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtrfm.py
+-rw-rw-rw-   0        0        0     9749 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rts.py
+-rw-rw-rw-   0        0        0    13225 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtve.py
+-rw-rw-rw-   0        0        0     2231 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtvnh.py
+-rw-rw-rw-   0        0        0     3513 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtvs.py
+-rw-rw-rw-   0        0        0     6294 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtvslo.py
+-rw-rw-rw-   0        0        0     1571 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ruhd.py
+-rw-rw-rw-   0        0        0     2278 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rule34video.py
+-rw-rw-rw-   0        0        0    15562 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rumble.py
+-rw-rw-rw-   0        0        0    14239 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rutube.py
+-rw-rw-rw-   0        0        0     8255 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rutv.py
+-rw-rw-rw-   0        0        0    11230 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ruutu.py
+-rw-rw-rw-   0        0        0     7025 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ruv.py
+-rw-rw-rw-   0        0        0    10081 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/safari.py
+-rw-rw-rw-   0        0        0     3064 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/saitosan.py
+-rw-rw-rw-   0        0        0     3914 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/samplefocus.py
+-rw-rw-rw-   0        0        0     4512 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sapo.py
+-rw-rw-rw-   0        0        0     1040 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/savefrom.py
+-rw-rw-rw-   0        0        0     4359 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sbs.py
+-rw-rw-rw-   0        0        0     2668 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/screen9.py
+-rw-rw-rw-   0        0        0     4711 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/screencast.py
+-rw-rw-rw-   0        0        0     1979 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/screencastify.py
+-rw-rw-rw-   0        0        0     3023 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/screencastomatic.py
+-rw-rw-rw-   0        0        0     5705 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/scrippsnetworks.py
+-rw-rw-rw-   0        0        0     3846 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/scrolller.py
+-rw-rw-rw-   0        0        0     4959 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/scte.py
+-rw-rw-rw-   0        0        0     2295 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/seeker.py
+-rw-rw-rw-   0        0        0     8888 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/senategov.py
+-rw-rw-rw-   0        0        0     4023 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sendtonews.py
+-rw-rw-rw-   0        0        0     5545 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/servus.py
+-rw-rw-rw-   0        0        0     5070 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sevenplus.py
+-rw-rw-rw-   0        0        0     1983 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sexu.py
+-rw-rw-rw-   0        0        0     7780 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/seznamzpravy.py
+-rw-rw-rw-   0        0        0     8503 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/shahid.py
+-rw-rw-rw-   0        0        0     4449 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/shared.py
+-rw-rw-rw-   0        0        0      243 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sharevideos.py
+-rw-rw-rw-   0        0        0     4340 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/shemaroome.py
+-rw-rw-rw-   0        0        0     3096 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/showroomlive.py
+-rw-rw-rw-   0        0        0      744 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sibnet.py
+-rw-rw-rw-   0        0        0     6196 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/simplecast.py
+-rw-rw-rw-   0        0        0     4303 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sina.py
+-rw-rw-rw-   0        0        0     5181 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sixplay.py
+-rw-rw-rw-   0        0        0     5715 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/skeb.py
+-rw-rw-rw-   0        0        0     6670 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sky.py
+-rw-rw-rw-   0        0        0     9452 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/skyit.py
+-rw-rw-rw-   0        0        0     1416 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/skylinewebcams.py
+-rw-rw-rw-   0        0        0     5439 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/skynewsarabia.py
+-rw-rw-rw-   0        0        0     1820 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/skynewsau.py
+-rw-rw-rw-   0        0        0     2130 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/slideshare.py
+-rw-rw-rw-   0        0        0    23251 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/slideslive.py
+-rw-rw-rw-   0        0        0     2372 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/slutload.py
+-rw-rw-rw-   0        0        0     2750 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/smotrim.py
+-rw-rw-rw-   0        0        0     2497 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/snotr.py
+-rw-rw-rw-   0        0        0     7008 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sohu.py
+-rw-rw-rw-   0        0        0     9700 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sonyliv.py
+-rw-rw-rw-   0        0        0    36979 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/soundcloud.py
+-rw-rw-rw-   0        0        0     2427 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/soundgasm.py
+-rw-rw-rw-   0        0        0     7973 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/southpark.py
+-rw-rw-rw-   0        0        0     8462 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sovietscloset.py
+-rw-rw-rw-   0        0        0     7388 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spankbang.py
+-rw-rw-rw-   0        0        0     6447 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spankwire.py
+-rw-rw-rw-   0        0        0     2378 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spiegel.py
+-rw-rw-rw-   0        0        0     1707 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spike.py
+-rw-rw-rw-   0        0        0     3233 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sport5.py
+-rw-rw-rw-   0        0        0     3321 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sportbox.py
+-rw-rw-rw-   0        0        0     6437 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sportdeutschland.py
+-rw-rw-rw-   0        0        0     6508 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spotify.py
+-rw-rw-rw-   0        0        0     6146 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spreaker.py
+-rw-rw-rw-   0        0        0     4100 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/springboardplatform.py
+-rw-rw-rw-   0        0        0     2330 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sprout.py
+-rw-rw-rw-   0        0        0    10184 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/srgssr.py
+-rw-rw-rw-   0        0        0     2323 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/srmediathek.py
+-rw-rw-rw-   0        0        0     3574 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/stanfordoc.py
+-rw-rw-rw-   0        0        0     3886 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/startrek.py
+-rw-rw-rw-   0        0        0     3630 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/startv.py
+-rw-rw-rw-   0        0        0     6872 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/steam.py
+-rw-rw-rw-   0        0        0     5472 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/stitcher.py
+-rw-rw-rw-   0        0        0     4917 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/storyfire.py
+-rw-rw-rw-   0        0        0     4020 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streamable.py
+-rw-rw-rw-   0        0        0     1831 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streamanity.py
+-rw-rw-rw-   0        0        0     2576 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streamcloud.py
+-rw-rw-rw-   0        0        0     5133 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streamcz.py
+-rw-rw-rw-   0        0        0     1049 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streamff.py
+-rw-rw-rw-   0        0        0     3664 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streetvoice.py
+-rw-rw-rw-   0        0        0     1333 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/stretchinternet.py
+-rw-rw-rw-   0        0        0     2716 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/stripchat.py
+-rw-rw-rw-   0        0        0     3418 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/stv.py
+-rw-rw-rw-   0        0        0     4323 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/substack.py
+-rw-rw-rw-   0        0        0     2603 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sunporno.py
+-rw-rw-rw-   0        0        0     3928 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sverigesradio.py
+-rw-rw-rw-   0        0        0    15604 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/svt.py
+-rw-rw-rw-   0        0        0     3304 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/swearnet.py
+-rw-rw-rw-   0        0        0     4393 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/swrmediathek.py
+-rw-rw-rw-   0        0        0     2061 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/syfy.py
+-rw-rw-rw-   0        0        0     1271 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/syvdk.py
+-rw-rw-rw-   0        0        0     1654 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sztvhu.py
+-rw-rw-rw-   0        0        0     5900 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tagesschau.py
+-rw-rw-rw-   0        0        0     1981 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tass.py
+-rw-rw-rw-   0        0        0     3576 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tbs.py
+-rw-rw-rw-   0        0        0     2472 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tdslifeway.py
+-rw-rw-rw-   0        0        0    10734 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teachable.py
+-rw-rw-rw-   0        0        0     4443 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teachertube.py
+-rw-rw-rw-   0        0        0     1052 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teachingchannel.py
+-rw-rw-rw-   0        0        0    10266 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teamcoco.py
+-rw-rw-rw-   0        0        0     5508 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teamtreehouse.py
+-rw-rw-rw-   0        0        0     2564 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/techtalks.py
+-rw-rw-rw-   0        0        0    10057 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ted.py
+-rw-rw-rw-   0        0        0     3333 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tele13.py
+-rw-rw-rw-   0        0        0     3368 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tele5.py
+-rw-rw-rw-   0        0        0     2888 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telebruxelles.py
+-rw-rw-rw-   0        0        0     3208 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telecaribe.py
+-rw-rw-rw-   0        0        0     6280 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telecinco.py
+-rw-rw-rw-   0        0        0     3078 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telegraaf.py
+-rw-rw-rw-   0        0        0     5221 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telegram.py
+-rw-rw-rw-   0        0        0     2944 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telemb.py
+-rw-rw-rw-   0        0        0     2425 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telemundo.py
+-rw-rw-rw-   0        0        0     9224 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telequebec.py
+-rw-rw-rw-   0        0        0     1749 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teletask.py
+-rw-rw-rw-   0        0        0     1838 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telewebion.py
+-rw-rw-rw-   0        0        0     5002 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tempo.py
+-rw-rw-rw-   0        0        0    20439 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tencent.py
+-rw-rw-rw-   0        0        0     7420 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tennistv.py
+-rw-rw-rw-   0        0        0     4728 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tenplay.py
+-rw-rw-rw-   0        0        0     1927 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/testurl.py
+-rw-rw-rw-   0        0        0     3049 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tf1.py
+-rw-rw-rw-   0        0        0     2033 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tfo.py
+-rw-rw-rw-   0        0        0     1495 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/theholetv.py
+-rw-rw-rw-   0        0        0     1790 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/theintercept.py
+-rw-rw-rw-   0        0        0    17558 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/theplatform.py
+-rw-rw-rw-   0        0        0     1380 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thestar.py
+-rw-rw-rw-   0        0        0     1699 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thesun.py
+-rw-rw-rw-   0        0        0     3669 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/theta.py
+-rw-rw-rw-   0        0        0     4046 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/theweatherchannel.py
+-rw-rw-rw-   0        0        0     1547 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thisamericanlife.py
+-rw-rw-rw-   0        0        0     2465 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thisav.py
+-rw-rw-rw-   0        0        0     2736 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thisoldhouse.py
+-rw-rw-rw-   0        0        0     8843 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thisvid.py
+-rw-rw-rw-   0        0        0     6375 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/threeqsdn.py
+-rw-rw-rw-   0        0        0     4098 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/threespeak.py
+-rw-rw-rw-   0        0        0    53946 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tiktok.py
+-rw-rw-rw-   0        0        0     1905 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tinypic.py
+-rw-rw-rw-   0        0        0     9781 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tmz.py
+-rw-rw-rw-   0        0        0    13962 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tnaflix.py
+-rw-rw-rw-   0        0        0     9040 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/toggle.py
+-rw-rw-rw-   0        0        0     3486 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/toggo.py
+-rw-rw-rw-   0        0        0     5774 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tokentube.py
+-rw-rw-rw-   0        0        0     1919 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tonline.py
+-rw-rw-rw-   0        0        0     3048 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/toongoggles.py
+-rw-rw-rw-   0        0        0     3605 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/toutv.py
+-rw-rw-rw-   0        0        0     2776 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/toypics.py
+-rw-rw-rw-   0        0        0     2654 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/traileraddict.py
+-rw-rw-rw-   0        0        0    12826 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/triller.py
+-rw-rw-rw-   0        0        0     3667 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trilulilu.py
+-rw-rw-rw-   0        0        0    13243 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trovo.py
+-rw-rw-rw-   0        0        0     1986 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trtcocuk.py
+-rw-rw-rw-   0        0        0     6484 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trueid.py
+-rw-rw-rw-   0        0        0     1476 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trunews.py
+-rw-rw-rw-   0        0        0     2896 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/truth.py
+-rw-rw-rw-   0        0        0     2530 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trutv.py
+-rw-rw-rw-   0        0        0     3082 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tube8.py
+-rw-rw-rw-   0        0        0    10954 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tubetugraz.py
+-rw-rw-rw-   0        0        0     6867 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tubitv.py
+-rw-rw-rw-   0        0        0    16818 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tumblr.py
+-rw-rw-rw-   0        0        0     9371 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tunein.py
+-rw-rw-rw-   0        0        0     3210 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tunepk.py
+-rw-rw-rw-   0        0        0     2398 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/turbo.py
+-rw-rw-rw-   0        0        0    11312 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/turner.py
+-rw-rw-rw-   0        0        0    13990 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv2.py
+-rw-rw-rw-   0        0        0     3723 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv24ua.py
+-rw-rw-rw-   0        0        0     6191 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv2dk.py
+-rw-rw-rw-   0        0        0     4181 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv2hu.py
+-rw-rw-rw-   0        0        0     4972 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv4.py
+-rw-rw-rw-   0        0        0     4671 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv5mondeplus.py
+-rw-rw-rw-   0        0        0     4134 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv5unis.py
+-rw-rw-rw-   0        0        0     3186 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tva.py
+-rw-rw-rw-   0        0        0     2406 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvanouvelles.py
+-rw-rw-rw-   0        0        0     3768 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvc.py
+-rw-rw-rw-   0        0        0     4983 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tver.py
+-rw-rw-rw-   0        0        0     5176 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvigle.py
+-rw-rw-rw-   0        0        0     3325 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tviplayer.py
+-rw-rw-rw-   0        0        0     1560 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvland.py
+-rw-rw-rw-   0        0        0     3908 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvn24.py
+-rw-rw-rw-   0        0        0     4851 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvnet.py
+-rw-rw-rw-   0        0        0     1600 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvnoe.py
+-rw-rw-rw-   0        0        0    24665 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvnow.py
+-rw-rw-rw-   0        0        0     5325 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvopengr.py
+-rw-rw-rw-   0        0        0    23559 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvp.py
+-rw-rw-rw-   0        0        0    20702 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvplay.py
+-rw-rw-rw-   0        0        0     2797 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvplayer.py
+-rw-rw-rw-   0        0        0     2147 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tweakers.py
+-rw-rw-rw-   0        0        0     4812 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twentyfourvideo.py
+-rw-rw-rw-   0        0        0     2718 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twentymin.py
+-rw-rw-rw-   0        0        0     3318 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twentythreevideo.py
+-rw-rw-rw-   0        0        0    12618 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twitcasting.py
+-rw-rw-rw-   0        0        0    43480 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twitch.py
+-rw-rw-rw-   0        0        0    59522 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twitter.py
+-rw-rw-rw-   0        0        0    16085 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/txxx.py
+-rw-rw-rw-   0        0        0    20020 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/udemy.py
+-rw-rw-rw-   0        0        0     3676 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/udn.py
+-rw-rw-rw-   0        0        0      467 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ufctv.py
+-rw-rw-rw-   0        0        0     2508 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ukcolumn.py
+-rw-rw-rw-   0        0        0     1493 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/uktvplay.py
+-rw-rw-rw-   0        0        0     3266 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/umg.py
+-rw-rw-rw-   0        0        0     2141 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/unistra.py
+-rw-rw-rw-   0        0        0     1217 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/unity.py
+-rw-rw-rw-   0        0        0     2573 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/unscripted.py
+-rw-rw-rw-   0        0        0     5615 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/unsupported.py
+-rw-rw-rw-   0        0        0     5514 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/uol.py
+-rw-rw-rw-   0        0        0     3440 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/uplynk.py
+-rw-rw-rw-   0        0        0     2163 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/urort.py
+-rw-rw-rw-   0        0        0     7021 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/urplay.py
+-rw-rw-rw-   0        0        0      819 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/usanetwork.py
+-rw-rw-rw-   0        0        0     2706 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/usatoday.py
+-rw-rw-rw-   0        0        0    10820 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ustream.py
+-rw-rw-rw-   0        0        0     4379 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ustudio.py
+-rw-rw-rw-   0        0        0     3502 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/utreon.py
+-rw-rw-rw-   0        0        0     3096 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/varzesh3.py
+-rw-rw-rw-   0        0        0     3295 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vbox7.py
+-rw-rw-rw-   0        0        0     4209 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/veehd.py
+-rw-rw-rw-   0        0        0     2812 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/veo.py
+-rw-rw-rw-   0        0        0     7128 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/veoh.py
+-rw-rw-rw-   0        0        0     4440 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vesti.py
+-rw-rw-rw-   0        0        0    13857 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vevo.py
+-rw-rw-rw-   0        0        0    11171 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vgtv.py
+-rw-rw-rw-   0        0        0     1414 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vh1.py
+-rw-rw-rw-   0        0        0    12365 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vice.py
+-rw-rw-rw-   0        0        0     2958 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vidbit.py
+-rw-rw-rw-   0        0        0     5072 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viddler.py
+-rw-rw-rw-   0        0        0     6643 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videa.py
+-rw-rw-rw-   0        0        0    10990 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videocampus_sachsen.py
+-rw-rw-rw-   0        0        0      892 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videodetective.py
+-rw-rw-rw-   0        0        0     1759 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videofyme.py
+-rw-rw-rw-   0        0        0    14035 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videoken.py
+-rw-rw-rw-   0        0        0    11631 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videomore.py
+-rw-rw-rw-   0        0        0     3228 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videopress.py
+-rw-rw-rw-   0        0        0    14059 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vidio.py
+-rw-rw-rw-   0        0        0     5888 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vidlii.py
+-rw-rw-rw-   0        0        0    14139 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viewlift.py
+-rw-rw-rw-   0        0        0     7548 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viidea.py
+-rw-rw-rw-   0        0        0    13838 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viki.py
+-rw-rw-rw-   0        0        0    63610 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vimeo.py
+-rw-rw-rw-   0        0        0     2220 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vimm.py
+-rw-rw-rw-   0        0        0     1949 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vimple.py
+-rw-rw-rw-   0        0        0     5553 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vine.py
+-rw-rw-rw-   0        0        0     3123 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viqeo.py
+-rw-rw-rw-   0        0        0    21769 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viu.py
+-rw-rw-rw-   0        0        0    28692 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vk.py
+-rw-rw-rw-   0        0        0     2199 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vocaroo.py
+-rw-rw-rw-   0        0        0     2816 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vodlocker.py
+-rw-rw-rw-   0        0        0     1004 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vodpl.py
+-rw-rw-rw-   0        0        0     1653 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vodplatform.py
+-rw-rw-rw-   0        0        0     2284 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/voicerepublic.py
+-rw-rw-rw-   0        0        0     5507 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/voicy.py
+-rw-rw-rw-   0        0        0     1707 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/volejtv.py
+-rw-rw-rw-   0        0        0     6114 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/voot.py
+-rw-rw-rw-   0        0        0    10015 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/voxmedia.py
+-rw-rw-rw-   0        0        0     2963 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vrak.py
+-rw-rw-rw-   0        0        0     3549 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vrt.py
+-rw-rw-rw-   0        0        0    11172 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vrv.py
+-rw-rw-rw-   0        0        0     2034 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vshare.py
+-rw-rw-rw-   0        0        0     1901 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vtm.py
+-rw-rw-rw-   0        0        0     2281 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vuclip.py
+-rw-rw-rw-   0        0        0     2167 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vupload.py
+-rw-rw-rw-   0        0        0    11057 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vvvvid.py
+-rw-rw-rw-   0        0        0     2008 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vyborymos.py
+-rw-rw-rw-   0        0        0     3516 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vzaar.py
+-rw-rw-rw-   0        0        0     2851 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wakanim.py
+-rw-rw-rw-   0        0        0     2802 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/walla.py
+-rw-rw-rw-   0        0        0     6305 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wasdtv.py
+-rw-rw-rw-   0        0        0     5939 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/washingtonpost.py
+-rw-rw-rw-   0        0        0     4332 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wat.py
+-rw-rw-rw-   0        0        0     5917 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/watchbox.py
+-rw-rw-rw-   0        0        0     2301 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/watchindianporn.py
+-rw-rw-rw-   0        0        0    14928 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wdr.py
+-rw-rw-rw-   0        0        0     1628 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/webcamerapl.py
+-rw-rw-rw-   0        0        0     3752 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/webcaster.py
+-rw-rw-rw-   0        0        0     5611 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/webofstories.py
+-rw-rw-rw-   0        0        0     4487 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/weibo.py
+-rw-rw-rw-   0        0        0     1673 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/weiqitv.py
+-rw-rw-rw-   0        0        0     4033 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/whowatch.py
+-rw-rw-rw-   0        0        0     2376 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wikimedia.py
+-rw-rw-rw-   0        0        0     2398 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/willow.py
+-rw-rw-rw-   0        0        0     5614 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wimtv.py
+-rw-rw-rw-   0        0        0    16231 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wistia.py
+-rw-rw-rw-   0        0        0     7350 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wordpress.py
+-rw-rw-rw-   0        0        0     1341 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/worldstarhiphop.py
+-rw-rw-rw-   0        0        0     6286 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wppilot.py
+-rw-rw-rw-   0        0        0    10017 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wrestleuniverse.py
+-rw-rw-rw-   0        0        0     4778 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wsj.py
+-rw-rw-rw-   0        0        0     4629 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wwe.py
+-rw-rw-rw-   0        0        0     2156 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xanimu.py
+-rw-rw-rw-   0        0        0     1448 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xbef.py
+-rw-rw-rw-   0        0        0     2377 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xboxclips.py
+-rw-rw-rw-   0        0        0     7606 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xfileshare.py
+-rw-rw-rw-   0        0        0    19690 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xhamster.py
+-rw-rw-rw-   0        0        0     6807 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ximalaya.py
+-rw-rw-rw-   0        0        0     4048 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xinpianchang.py
+-rw-rw-rw-   0        0        0     2956 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xminus.py
+-rw-rw-rw-   0        0        0     2972 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xnxx.py
+-rw-rw-rw-   0        0        0     3996 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xstream.py
+-rw-rw-rw-   0        0        0     8107 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xtube.py
+-rw-rw-rw-   0        0        0     5863 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xuite.py
+-rw-rw-rw-   0        0        0     6889 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xvideos.py
+-rw-rw-rw-   0        0        0     2689 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xxxymovies.py
+-rw-rw-rw-   0        0        0    23347 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yahoo.py
+-rw-rw-rw-   0        0        0     5201 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yandexdisk.py
+-rw-rw-rw-   0        0        0    18103 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yandexmusic.py
+-rw-rw-rw-   0        0        0    17877 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yandexvideo.py
+-rw-rw-rw-   0        0        0     3028 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yapfiles.py
+-rw-rw-rw-   0        0        0     4696 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yappy.py
+-rw-rw-rw-   0        0        0     2198 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yesjapan.py
+-rw-rw-rw-   0        0        0     1867 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yinyuetai.py
+-rw-rw-rw-   0        0        0     6370 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yle_areena.py
+-rw-rw-rw-   0        0        0     1721 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ynet.py
+-rw-rw-rw-   0        0        0     3114 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/youjizz.py
+-rw-rw-rw-   0        0        0    12070 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/youku.py
+-rw-rw-rw-   0        0        0     7229 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/younow.py
+-rw-rw-rw-   0        0        0     8268 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/youporn.py
+-rw-rw-rw-   0        0        0     2086 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yourporn.py
+-rw-rw-rw-   0        0        0     1397 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yourupload.py
+-rw-rw-rw-   0        0        0   339334 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/youtube.py
+-rw-rw-rw-   0        0        0     3938 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zapiks.py
+-rw-rw-rw-   0        0        0    30272 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zattoo.py
+-rw-rw-rw-   0        0        0    18883 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zdf.py
+-rw-rw-rw-   0        0        0    11931 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zee5.py
+-rw-rw-rw-   0        0        0     3198 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zeenews.py
+-rw-rw-rw-   0        0        0     2610 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zhihu.py
+-rw-rw-rw-   0        0        0    14954 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zingmp3.py
+-rw-rw-rw-   0        0        0     3909 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zoom.py
+-rw-rw-rw-   0        0        0     5628 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zype.py
+-rw-rw-rw-   0        0        0     1957 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/flserver.py
+-rw-rw-rw-   0        0        0      197 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/gunicorn.conf.py
+-rw-rw-rw-   0        0        0    35050 2023-04-04 04:11:50.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/jsinterp.py
+-rw-rw-rw-   0        0        0     5510 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/minicurses.py
+-rw-rw-rw-   0        0        0    96161 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/options.py
+-rw-rw-rw-   0        0        0     6359 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/plugins.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:15.617253 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/
+-rw-rw-rw-   0        0        0     1327 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/__init__.py
+-rw-rw-rw-   0        0        0     8584 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/common.py
+-rw-rw-rw-   0        0        0    10652 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/embedthumbnail.py
+-rw-rw-rw-   0        0        0     1649 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/exec.py
+-rw-rw-rw-   0        0        0    50353 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/ffmpeg.py
+-rw-rw-rw-   0        0        0     4512 2023-04-04 05:52:42.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/metadataparser.py
+-rw-rw-rw-   0        0        0    18157 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/modify_chapters.py
+-rw-rw-rw-   0        0        0     2109 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/movefilesafterdownload.py
+-rw-rw-rw-   0        0        0     4195 2023-04-04 05:52:41.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/sponskrub.py
+-rw-rw-rw-   0        0        0     4353 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/sponsorblock.py
+-rw-rw-rw-   0        0        0     2544 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/xattrpp.py
+-rw-rw-rw-   0        0        0     2352 2023-04-04 04:11:51.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/server1.py
+-rw-rw-rw-   0        0        0     8784 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/socks.py
+-rw-rw-rw-   0        0        0    16049 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/update.py
+-rw-rw-rw-   0        0        0   230917 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/utils.py
+-rw-rw-rw-   0        0        0      206 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/version.py
+-rw-rw-rw-   0        0        0    11735 2023-04-04 04:11:52.000000 yt-dlp-cp-1.9.9/yt_dlp_cp/webvtt.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:14.363819 yt-dlp-cp-1.9.9/yt_dlp_cp.egg-info/
+-rw-rw-rw-   0        0        0      165 2023-06-29 08:20:13.000000 yt-dlp-cp-1.9.9/yt_dlp_cp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    37696 2023-06-29 08:20:14.000000 yt-dlp-cp-1.9.9/yt_dlp_cp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:20:13.000000 yt-dlp-cp-1.9.9/yt_dlp_cp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-06-29 08:20:13.000000 yt-dlp-cp-1.9.9/yt_dlp_cp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      155 2023-06-29 08:20:13.000000 yt-dlp-cp-1.9.9/yt_dlp_cp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-29 08:20:13.000000 yt-dlp-cp-1.9.9/yt_dlp_cp.egg-info/top_level.txt
```

### Comparing `yt-dlp-cp-0.9.9/Changelog.md` & `yt-dlp-cp-1.9.9/Changelog.md`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/LICENSE` & `yt-dlp-cp-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/README.md` & `yt-dlp-cp-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/__pycache__/utils.cpython-38.pyc` & `yt-dlp-cp-1.9.9/devscripts/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/bash-completion.in` & `yt-dlp-cp-1.9.9/devscripts/bash-completion.in`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/bash-completion.py` & `yt-dlp-cp-1.9.9/devscripts/bash-completion.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/changelog_override.json` & `yt-dlp-cp-1.9.9/devscripts/changelog_override.json`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/changelog_override.schema.json` & `yt-dlp-cp-1.9.9/devscripts/changelog_override.schema.json`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/check-porn.py` & `yt-dlp-cp-1.9.9/devscripts/check-porn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/fish-completion.py` & `yt-dlp-cp-1.9.9/devscripts/fish-completion.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/generate_aes_testdata.py` & `yt-dlp-cp-1.9.9/devscripts/generate_aes_testdata.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/lazy_load_template.py` & `yt-dlp-cp-1.9.9/devscripts/lazy_load_template.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/logo.ico` & `yt-dlp-cp-1.9.9/devscripts/logo.ico`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/make_changelog.py` & `yt-dlp-cp-1.9.9/devscripts/make_changelog.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/make_contributing.py` & `yt-dlp-cp-1.9.9/devscripts/make_contributing.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/make_issue_template.py` & `yt-dlp-cp-1.9.9/devscripts/make_issue_template.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/make_lazy_extractors.py` & `yt-dlp-cp-1.9.9/devscripts/make_lazy_extractors.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/make_readme.py` & `yt-dlp-cp-1.9.9/devscripts/make_readme.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/prepare_manpage.py` & `yt-dlp-cp-1.9.9/devscripts/prepare_manpage.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/set-variant.py` & `yt-dlp-cp-1.9.9/devscripts/set-variant.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/update-formulae.py` & `yt-dlp-cp-1.9.9/devscripts/update-formulae.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/update-version.py` & `yt-dlp-cp-1.9.9/devscripts/update-version.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/utils.py` & `yt-dlp-cp-1.9.9/devscripts/utils.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/zsh-completion.in` & `yt-dlp-cp-1.9.9/devscripts/zsh-completion.in`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/devscripts/zsh-completion.py` & `yt-dlp-cp-1.9.9/devscripts/zsh-completion.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/setup.cfg` & `yt-dlp-cp-1.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/setup.py` & `yt-dlp-cp-1.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         else:
             return freeze(**params)
     else:
         params = build_params()
 
     setup(
         name='yt-dlp-cp',
-        version='0.9.9',
+        version='1.9.9',
         maintainer='kylin99999',
         maintainer_email='kylinwork@yeah.net',
         packages=packages(),
         install_requires=REQUIREMENTS,
         python_requires='>=3.7',
         **params
     )
```

### Comparing `yt-dlp-cp-0.9.9/supportedsites.md` & `yt-dlp-cp-1.9.9/supportedsites.md`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/helper.py` & `yt-dlp-cp-1.9.9/test/helper.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/parameters.json` & `yt-dlp-cp-1.9.9/test/parameters.json`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_InfoExtractor.py` & `yt-dlp-cp-1.9.9/test/test_InfoExtractor.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_YoutubeDL.py` & `yt-dlp-cp-1.9.9/test/test_YoutubeDL.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_YoutubeDLCookieJar.py` & `yt-dlp-cp-1.9.9/test/test_YoutubeDLCookieJar.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_aes.py` & `yt-dlp-cp-1.9.9/test/test_aes.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_age_restriction.py` & `yt-dlp-cp-1.9.9/test/test_age_restriction.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_all_urls.py` & `yt-dlp-cp-1.9.9/test/test_all_urls.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_cache.py` & `yt-dlp-cp-1.9.9/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_compat.py` & `yt-dlp-cp-1.9.9/test/test_compat.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_config.py` & `yt-dlp-cp-1.9.9/test/test_config.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_cookies.py` & `yt-dlp-cp-1.9.9/test/test_cookies.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_download.py` & `yt-dlp-cp-1.9.9/test/test_download.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_downloader_http.py` & `yt-dlp-cp-1.9.9/test/test_downloader_http.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_execution.py` & `yt-dlp-cp-1.9.9/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_http.py` & `yt-dlp-cp-1.9.9/test/test_http.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_iqiyi_sdk_interpreter.py` & `yt-dlp-cp-1.9.9/test/test_iqiyi_sdk_interpreter.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_jsinterp.py` & `yt-dlp-cp-1.9.9/test/test_jsinterp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_netrc.py` & `yt-dlp-cp-1.9.9/test/test_netrc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_overwrites.py` & `yt-dlp-cp-1.9.9/test/test_overwrites.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_plugins.py` & `yt-dlp-cp-1.9.9/test/test_plugins.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_post_hooks.py` & `yt-dlp-cp-1.9.9/test/test_post_hooks.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_postprocessors.py` & `yt-dlp-cp-1.9.9/test/test_postprocessors.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_socks.py` & `yt-dlp-cp-1.9.9/test/test_socks.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_subtitles.py` & `yt-dlp-cp-1.9.9/test/test_subtitles.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_update.py.disabled` & `yt-dlp-cp-1.9.9/test/test_update.py.disabled`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_utils.py` & `yt-dlp-cp-1.9.9/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_verbose_output.py` & `yt-dlp-cp-1.9.9/test/test_verbose_output.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_write_annotations.py.disabled` & `yt-dlp-cp-1.9.9/test/test_write_annotations.py.disabled`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_youtube_lists.py` & `yt-dlp-cp-1.9.9/test/test_youtube_lists.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_youtube_misc.py` & `yt-dlp-cp-1.9.9/test/test_youtube_misc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/test_youtube_signature.py` & `yt-dlp-cp-1.9.9/test/test_youtube_signature.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testcert.pem` & `yt-dlp-cp-1.9.9/test/testcert.pem`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/certificate/ca.crt` & `yt-dlp-cp-1.9.9/test/testdata/certificate/ca.crt`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/certificate/clientwithencryptedkey.crt` & `yt-dlp-cp-1.9.9/test/testdata/certificate/clientwithencryptedkey.crt`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/certificate/clientwithkey.crt` & `yt-dlp-cp-1.9.9/test/testdata/certificate/clientwithkey.crt`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/certificate/instructions.md` & `yt-dlp-cp-1.9.9/test/testdata/certificate/instructions.md`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/f4m/custom_base_url.f4m` & `yt-dlp-cp-1.9.9/test/testdata/f4m/custom_base_url.f4m`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/ism/ec-3_test.Manifest` & `yt-dlp-cp-1.9.9/test/testdata/ism/ec-3_test.Manifest`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/ism/sintel.Manifest` & `yt-dlp-cp-1.9.9/test/testdata/ism/sintel.Manifest`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/m3u8/bipbop_16x9.m3u8` & `yt-dlp-cp-1.9.9/test/testdata/m3u8/bipbop_16x9.m3u8`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8` & `yt-dlp-cp-1.9.9/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/mpd/float_duration.mpd` & `yt-dlp-cp-1.9.9/test/testdata/mpd/float_duration.mpd`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/mpd/subtitles.mpd` & `yt-dlp-cp-1.9.9/test/testdata/mpd/subtitles.mpd`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/mpd/unfragmented.mpd` & `yt-dlp-cp-1.9.9/test/testdata/mpd/unfragmented.mpd`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/mpd/urls_only.mpd` & `yt-dlp-cp-1.9.9/test/testdata/mpd/urls_only.mpd`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/thumbnails/foo %d bar/foo_%d.webp` & `yt-dlp-cp-1.9.9/test/testdata/thumbnails/foo %d bar/foo_%d.webp`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/testdata/xspf/foo_xspf.xspf` & `yt-dlp-cp-1.9.9/test/testdata/xspf/foo_xspf.xspf`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/test/versions.json` & `yt-dlp-cp-1.9.9/test/versions.json`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/YoutubeDL.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/YoutubeDL.py`

 * *Files 0% similar despite different names*

```diff
@@ -1597,28 +1597,26 @@
                 if self.params.get('wait_for_video'):
                     self.report_warning(e)
                 self._wait_for_video()
             raise
         if ie_result is None:  # Finished already (backwards compatibility; listformats and friends should be moved here)
             self.report_warning(f'Extractor {ie.IE_NAME} returned nothing{bug_reports_message()}')
             return
-        else:
-            return ie_result
         if isinstance(ie_result, list):
             # Backwards compatibility: old IE result format
             ie_result = {
                 '_type': 'compat_list',
                 'entries': ie_result,
             }
         if extra_info.get('original_url'):
             ie_result.setdefault('original_url', extra_info['original_url'])
         self.add_default_extra_info(ie_result, ie, url)
         if process:
             self._wait_for_video(ie_result)
-            return self.process_ie_result(ie_result, download, extra_info)
+            return self.process_ie_result(ie_result, False, extra_info)
         else:
             return ie_result
 
     def add_default_extra_info(self, ie_result, ie, url):
         if url is not None:
             self.add_extra_info(ie_result, {
                 'webpage_url': url,
```

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/__init__.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/__init__.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/__pyinstaller/hook-yt_dlp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/__pyinstaller/hook-yt_dlp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/aes.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/aes.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/cache.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/cache.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/compat/__init__.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/compat/_legacy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/compat/_legacy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/compat/compat_utils.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/compat/compat_utils.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/compat/functools.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/compat/functools.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/compat/imghdr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/compat/imghdr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/compat/shutil.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/compat/shutil.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/cookies.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/cookies.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/dependencies/Cryptodome.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/dependencies/Cryptodome.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/dependencies/__init__.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/__init__.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/common.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/common.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/dash.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/dash.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/external.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/external.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/f4m.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/f4m.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/fc2.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/fc2.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/fragment.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/fragment.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/hls.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/hls.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/http.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/http.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/ism.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/ism.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/mhtml.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/mhtml.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/niconico.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/niconico.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/rtmp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/rtmp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/rtsp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/rtsp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/websocket.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/websocket.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/downloader/youtube_live_chat.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/downloader/youtube_live_chat.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/__init__.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/_extractors.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/_extractors.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/abc.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/abc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/abcnews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/abcnews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/abcotvs.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/abcotvs.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/abematv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/abematv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/academicearth.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/academicearth.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/acast.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/acast.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/acfun.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/acfun.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/adn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/adn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/adobeconnect.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/adobeconnect.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/adobepass.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/adobepass.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/adobetv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/adobetv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/adultswim.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/adultswim.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aenetworks.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aenetworks.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aeonco.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aeonco.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/afreecatv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/afreecatv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/agora.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/agora.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/airmozilla.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/airmozilla.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/airtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/airtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aitube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aitube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aliexpress.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aliexpress.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aljazeera.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aljazeera.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/allocine.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/allocine.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/alphaporno.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/alphaporno.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/alsace20tv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/alsace20tv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/alura.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/alura.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/amara.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/amara.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/amazon.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/amazon.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/amazonminitv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/amazonminitv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/amcnetworks.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/amcnetworks.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/americastestkitchen.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/americastestkitchen.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/amp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/amp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/anchorfm.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/anchorfm.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/angel.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/angel.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ant1newsgr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ant1newsgr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/anvato.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/anvato.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aol.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aol.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/apa.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/apa.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aparat.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aparat.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/appleconnect.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/appleconnect.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/applepodcasts.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/applepodcasts.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/appletrailers.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/appletrailers.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/archiveorg.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/archiveorg.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/arcpublishing.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/arcpublishing.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ard.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ard.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/arkena.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/arkena.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/arnes.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/arnes.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/arte.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/arte.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/asiancrush.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/asiancrush.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/atresplayer.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/atresplayer.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/atscaleconf.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/atscaleconf.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/atttechchannel.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/atttechchannel.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/atvat.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/atvat.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/audimedia.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/audimedia.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/audioboom.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/audioboom.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/audiodraft.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/audiodraft.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/audiomack.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/audiomack.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/audius.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/audius.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/awaan.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/awaan.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/aws.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/aws.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/azmedien.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/azmedien.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/baidu.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/baidu.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/banbye.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/banbye.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bandaichannel.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bandaichannel.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bandcamp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bandcamp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bannedvideo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bannedvideo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bbc.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bbc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/beatbump.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/beatbump.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/beatport.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/beatport.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/beeg.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/beeg.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/behindkink.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/behindkink.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bellmedia.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bellmedia.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/berufetv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/berufetv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bfi.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bfi.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bfmtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bfmtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bibeltv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bibeltv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bigflix.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bigflix.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bigo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bigo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bild.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bild.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bilibili.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bilibili.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/biobiochiletv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/biobiochiletv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/biqle.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/biqle.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bitchute.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bitchute.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bitwave.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bitwave.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/blackboardcollaborate.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/blackboardcollaborate.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bleacherreport.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bleacherreport.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/blerp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/blerp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/blogger.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/blogger.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bloomberg.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bloomberg.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bokecc.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bokecc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bongacams.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bongacams.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/booyah.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/booyah.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bostonglobe.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bostonglobe.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/box.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/box.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/boxcast.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/boxcast.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bpb.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bpb.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/br.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/br.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bravotv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bravotv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/breakcom.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/breakcom.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/breitbart.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/breitbart.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/brightcove.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/brightcove.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/bundesliga.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/bundesliga.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/businessinsider.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/businessinsider.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/buzzfeed.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/buzzfeed.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/byutv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/byutv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/c56.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/c56.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cableav.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cableav.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/callin.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/callin.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/caltrans.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/caltrans.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cam4.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cam4.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/camdemy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/camdemy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cammodels.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cammodels.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/camsoda.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/camsoda.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/camtasia.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/camtasia.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/camwithher.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/camwithher.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/canalalpha.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/canalalpha.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/canalc2.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/canalc2.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/canalplus.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/canalplus.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/canvas.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/canvas.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/carambatv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/carambatv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cartoonnetwork.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cartoonnetwork.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbc.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbs.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbs.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbsinteractive.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbsinteractive.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbslocal.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbslocal.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbsnews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbsnews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cbssports.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cbssports.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ccc.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ccc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ccma.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ccma.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cctv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cctv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cda.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cda.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cellebrite.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cellebrite.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ceskatelevize.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cgtn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cgtn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/channel9.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/channel9.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/charlierose.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/charlierose.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/chaturbate.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/chaturbate.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/chilloutzone.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/chilloutzone.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/chingari.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/chingari.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/chirbit.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/chirbit.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cinchcast.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cinchcast.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cinemax.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cinemax.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cinetecamilano.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cinetecamilano.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ciscolive.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ciscolive.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ciscowebex.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ciscowebex.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cjsw.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cjsw.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cliphunter.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cliphunter.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/clippit.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/clippit.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cliprs.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cliprs.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/clipsyndicate.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/clipsyndicate.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/closertotruth.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/closertotruth.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cloudflarestream.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cloudflarestream.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cloudy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cloudy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/clubic.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/clubic.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/clyp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/clyp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cmt.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cmt.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cnbc.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cnbc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cnn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cnn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/comedycentral.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/comedycentral.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/common.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/common.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/commonmistakes.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/commonmistakes.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/commonprotocols.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/commonprotocols.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/condenast.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/condenast.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/contv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/contv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/corus.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/corus.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/coub.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/coub.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cozytv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cozytv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cpac.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cpac.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cracked.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cracked.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/crackle.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/crackle.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/craftsy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/craftsy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/crooksandliars.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/crooksandliars.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/crowdbunker.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/crowdbunker.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/crunchyroll.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/crunchyroll.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cspan.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cspan.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ctsnews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ctsnews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ctv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ctv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ctvnews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ctvnews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cultureunplugged.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cultureunplugged.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/curiositystream.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/curiositystream.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cwtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cwtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/cybrary.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/cybrary.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/daftsex.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/daftsex.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dailymail.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dailymail.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dailymotion.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dailymotion.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dailywire.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dailywire.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/damtomo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/damtomo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/daum.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/daum.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/daystar.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/daystar.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dbtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dbtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dctp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dctp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/deezer.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/deezer.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/defense.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/defense.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/democracynow.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/democracynow.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/detik.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/detik.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/deuxm.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/deuxm.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dfb.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dfb.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dhm.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dhm.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/digg.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/digg.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/digitalconcerthall.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/digitalconcerthall.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/digiteka.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/digiteka.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/discovery.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/discovery.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/discoverygo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/discoverygo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/disney.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/disney.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dispeak.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dispeak.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dlive.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dlive.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dotsub.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dotsub.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/douyutv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/douyutv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dplay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dplay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/drbonanza.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/drbonanza.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dreisat.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dreisat.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/drooble.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/drooble.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dropbox.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dropbox.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dropout.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dropout.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/drtuber.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/drtuber.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/drtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/drtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dtube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dtube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/duboku.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/duboku.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dumpert.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dumpert.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dvtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dvtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/dw.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/dw.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eagleplatform.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eagleplatform.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ebaumsworld.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ebaumsworld.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ebay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ebay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/echomsk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/echomsk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/egghead.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/egghead.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ehow.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ehow.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eighttracks.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eighttracks.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/einthusan.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/einthusan.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eitb.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eitb.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ellentube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ellentube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/elonet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/elonet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/elpais.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/elpais.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/embedly.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/embedly.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/epicon.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/epicon.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/epoch.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/epoch.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eporner.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eporner.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eroprofile.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eroprofile.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ertgr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ertgr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/escapist.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/escapist.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/espn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/espn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/esri.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/esri.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/europa.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/europa.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/europeantour.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/europeantour.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eurosport.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eurosport.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/euscreen.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/euscreen.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/expotv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/expotv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/expressen.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/expressen.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/extractors.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/extractors.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/extremetube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/extremetube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/eyedotv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/eyedotv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/facebook.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/facebook.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fancode.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fancode.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/faz.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/faz.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fc2.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fc2.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fczenit.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fczenit.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fifa.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fifa.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/filmmodu.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/filmmodu.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/filmon.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/filmon.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/filmweb.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/filmweb.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/firsttv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/firsttv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fivetv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fivetv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/flickr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/flickr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/folketinget.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/folketinget.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/footyroom.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/footyroom.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/formula1.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/formula1.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fourtube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fourtube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fourzerostudio.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fourzerostudio.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fox.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fox.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fox9.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fox9.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/foxgay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/foxgay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/foxnews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/foxnews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/foxsports.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/foxsports.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fptplay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fptplay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/franceinter.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/franceinter.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/francetv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/francetv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/freesound.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/freesound.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/freespeech.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/freespeech.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/freetv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/freetv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/frontendmasters.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/frontendmasters.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fujitv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fujitv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/funimation.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/funimation.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/funk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/funk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fusion.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fusion.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/fuyintv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/fuyintv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gab.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gab.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gaia.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gaia.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gameinformer.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gameinformer.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gamejolt.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gamejolt.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gamespot.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gamespot.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gamestar.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gamestar.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gaskrank.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gaskrank.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gazeta.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gazeta.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gdcvault.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gdcvault.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gedidigital.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gedidigital.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/generic.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/generic.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/genericembeds.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/genericembeds.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/genius.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/genius.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gettr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gettr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gfycat.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gfycat.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/giantbomb.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/giantbomb.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/giga.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/giga.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gigya.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gigya.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/glide.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/glide.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/globo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/globo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/glomex.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/glomex.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/go.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/go.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/godtube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/godtube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gofile.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gofile.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/golem.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/golem.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/goodgame.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/goodgame.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/googledrive.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/googledrive.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/googlepodcasts.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/googlepodcasts.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/googlesearch.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/googlesearch.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/goplay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/goplay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gopro.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gopro.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/goshgay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/goshgay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gotostage.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gotostage.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gputechconf.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gputechconf.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/gronkh.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/gronkh.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/groupon.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/groupon.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/harpodeon.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/harpodeon.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hbo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hbo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hearthisat.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hearthisat.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/heise.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/heise.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hellporno.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hellporno.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/helsinki.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/helsinki.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hentaistigma.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hentaistigma.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hgtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hgtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hidive.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hidive.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/historicfilms.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/historicfilms.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hitbox.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hitbox.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hitrecord.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hitrecord.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hketv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hketv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hollywoodreporter.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hollywoodreporter.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/holodex.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/holodex.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hotnewhiphop.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hotnewhiphop.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hotstar.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hotstar.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/howcast.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/howcast.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/howstuffworks.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/howstuffworks.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hrfensehen.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hrfensehen.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hrti.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hrti.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hse.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hse.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/huajiao.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/huajiao.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/huffpost.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/huffpost.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hungama.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hungama.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/huya.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/huya.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hypem.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hypem.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hypergryph.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hypergryph.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/hytale.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/hytale.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/icareus.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/icareus.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ichinanalive.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ichinanalive.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ign.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ign.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/iheart.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/iheart.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/iltalehti.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/iltalehti.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/imdb.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/imdb.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/imggaming.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/imggaming.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/imgur.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/imgur.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ina.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ina.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/inc.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/inc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/indavideo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/indavideo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/infoq.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/infoq.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/instagram.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/instagram.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/internazionale.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/internazionale.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/internetvideoarchive.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/internetvideoarchive.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/iprima.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/iprima.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/iqiyi.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/iqiyi.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/islamchannel.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/islamchannel.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/israelnationalnews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/israelnationalnews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/itprotv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/itprotv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/itv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/itv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ivi.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ivi.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ivideon.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ivideon.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/iwara.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/iwara.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ixigua.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ixigua.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/izlesene.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/izlesene.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jable.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jable.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jamendo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jamendo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/japandiet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/japandiet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jeuxvideo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jeuxvideo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jixie.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jixie.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/joj.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/joj.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jove.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jove.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/jwplatform.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/jwplatform.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kakao.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kakao.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kaltura.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kaltura.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kanal2.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kanal2.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kankanews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kankanews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/karaoketv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/karaoketv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/karrierevideos.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/karrierevideos.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/keezmovies.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/keezmovies.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kelbyone.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kelbyone.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ketnet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ketnet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/khanacademy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/khanacademy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kick.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kick.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kicker.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kicker.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kickstarter.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kickstarter.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kinja.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kinja.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kinopoisk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kinopoisk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kommunetv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kommunetv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kompas.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kompas.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/konserthusetplay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/konserthusetplay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/koo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/koo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/krasview.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/krasview.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kth.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kth.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ku6.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ku6.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kusi.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kusi.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/kuwo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/kuwo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/la7.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/la7.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/laola1tv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/laola1tv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lastfm.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lastfm.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lbry.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lbry.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lci.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lci.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lcp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lcp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lecture2go.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lecture2go.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lecturio.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lecturio.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/leeco.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/leeco.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lefigaro.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lefigaro.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lego.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lego.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lemonde.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lemonde.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lenta.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lenta.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/libraryofcongress.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/libraryofcongress.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/libsyn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/libsyn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lifenews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lifenews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/likee.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/likee.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/limelight.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/limelight.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/line.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/line.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/linkedin.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/linkedin.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/linuxacademy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/linuxacademy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/liputan6.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/liputan6.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/listennotes.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/listennotes.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/litv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/litv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/livejournal.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/livejournal.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/livestream.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/livestream.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/livestreamfails.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/livestreamfails.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lnkgo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lnkgo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/localnews8.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/localnews8.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lovehomeporn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lovehomeporn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lrt.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lrt.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lumni.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lumni.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/lynda.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/lynda.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/m6.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/m6.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/magentamusik360.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/magentamusik360.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mailru.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mailru.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mainstreaming.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mainstreaming.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/malltv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/malltv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mangomolo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mangomolo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/manoto.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/manoto.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/manyvids.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/manyvids.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/maoritv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/maoritv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/markiza.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/markiza.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/massengeschmacktv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/massengeschmacktv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/masters.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/masters.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/matchtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/matchtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mdr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mdr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/medaltv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/medaltv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediaite.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediaite.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediaklikk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediaklikk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/medialaan.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/medialaan.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediaset.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediaset.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediasite.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediasite.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediastream.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediastream.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mediaworksnz.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mediaworksnz.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/medici.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/medici.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/megaphone.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/megaphone.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/megatvcom.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/megatvcom.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/meipai.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/meipai.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/melonvod.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/melonvod.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/meta.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/meta.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/metacafe.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/metacafe.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/metacritic.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/metacritic.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mgoon.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mgoon.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mgtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mgtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/miaopai.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/miaopai.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/microsoftembed.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/microsoftembed.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/microsoftstream.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/microsoftstream.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/microsoftvirtualacademy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/microsoftvirtualacademy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mildom.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mildom.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/minds.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/minds.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ministrygrid.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ministrygrid.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/minoto.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/minoto.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/miomio.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/miomio.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mirrativ.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mirrativ.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mirrorcouk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mirrorcouk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mit.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mit.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mitele.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mitele.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mixch.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mixch.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mixcloud.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mixcloud.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mlb.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mlb.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mlssoccer.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mlssoccer.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mnet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mnet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mocha.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mocha.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/moevideo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/moevideo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mofosex.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mofosex.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mojvideo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mojvideo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/morningstar.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/morningstar.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/motherless.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/motherless.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/motorsport.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/motorsport.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/movieclips.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/movieclips.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/moviepilot.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/moviepilot.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/moview.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/moview.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/moviezine.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/moviezine.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/movingimage.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/movingimage.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/msn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/msn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/muenchentv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/muenchentv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/murrtube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/murrtube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/musescore.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/musescore.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/musicdex.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/musicdex.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mwave.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mwave.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mxplayer.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mxplayer.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/mychannels.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/mychannels.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/myspace.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/myspace.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/myspass.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/myspass.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/myvi.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/myvi.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/myvideoge.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/myvideoge.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/myvidster.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/myvidster.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/n1.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/n1.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nate.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nate.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nationalgeographic.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nationalgeographic.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/naver.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/naver.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nba.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nba.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nbc.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nbc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ndr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ndr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ndtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ndtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nebula.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nebula.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nerdcubed.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nerdcubed.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/neteasemusic.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/neteasemusic.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/netverse.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/netverse.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/netzkino.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/netzkino.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/newgrounds.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/newgrounds.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/newspicks.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/newspicks.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/newstube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/newstube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/newsy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/newsy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nextmedia.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nextmedia.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nexx.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nexx.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nfb.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nfb.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nfhsnetwork.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nfhsnetwork.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nfl.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nfl.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nhk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nhk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nhl.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nhl.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nick.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nick.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/niconico.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/niconico.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ninecninemedia.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ninecninemedia.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ninegag.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ninegag.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ninenow.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ninenow.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nintendo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nintendo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nitter.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nitter.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/njpwworld.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/njpwworld.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nobelprize.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nobelprize.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/noice.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/noice.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nonktube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nonktube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/noodlemagazine.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/noodlemagazine.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/noovo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/noovo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/normalboots.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/normalboots.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nosnl.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nosnl.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nosvideo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nosvideo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nova.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nova.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/novaplay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/novaplay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nowness.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nowness.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/noz.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/noz.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/npo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/npo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/npr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/npr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nrk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nrk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nrl.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nrl.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ntvcojp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ntvcojp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ntvde.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ntvde.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ntvru.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ntvru.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nubilesporn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nubilesporn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nuevo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nuevo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nuvid.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nuvid.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nytimes.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nytimes.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nzherald.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nzherald.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nzonscreen.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nzonscreen.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/nzz.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/nzz.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/odatv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/odatv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/odkmedia.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/odkmedia.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/odnoklassniki.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/odnoklassniki.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/oftv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/oftv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/oktoberfesttv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/oktoberfesttv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/olympics.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/olympics.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/on24.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/on24.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/once.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/once.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ondemandkorea.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ondemandkorea.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/onefootball.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/onefootball.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/onenewsnz.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/onenewsnz.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/oneplace.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/oneplace.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/onet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/onet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/onionstudios.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/onionstudios.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ooyala.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ooyala.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/opencast.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/opencast.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/openload.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/openload.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/openrec.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/openrec.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ora.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ora.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/orf.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/orf.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/outsidetv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/outsidetv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/packtpub.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/packtpub.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/palcomp3.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/palcomp3.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pandoratv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pandoratv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/panopto.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/panopto.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/paramountplus.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/paramountplus.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/parler.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/parler.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/parlview.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/parlview.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/patreon.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/patreon.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pbs.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pbs.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pearvideo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pearvideo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/peekvids.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/peekvids.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/peertube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/peertube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/peertv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/peertv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/peloton.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/peloton.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/people.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/people.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/performgroup.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/performgroup.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/periscope.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/periscope.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pgatour.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pgatour.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/philharmoniedeparis.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/philharmoniedeparis.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/phoenix.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/phoenix.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/photobucket.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/photobucket.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/piapro.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/piapro.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/picarto.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/picarto.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/piksel.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/piksel.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pinkbike.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pinkbike.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pinterest.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pinterest.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pixivsketch.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pixivsketch.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pladform.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pladform.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/planetmarathi.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/planetmarathi.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/platzi.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/platzi.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playfm.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playfm.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playplustv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playplustv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/plays.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/plays.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playstuff.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playstuff.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playsuisse.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playsuisse.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playtvak.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playtvak.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playvid.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playvid.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/playwire.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/playwire.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pluralsight.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pluralsight.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/plutotv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/plutotv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/podbayfm.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/podbayfm.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/podchaser.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/podchaser.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/podomatic.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/podomatic.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pokemon.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pokemon.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pokergo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pokergo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/polsatgo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/polsatgo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/polskieradio.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/polskieradio.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/popcorntimes.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/popcorntimes.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/popcorntv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/popcorntv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/porn91.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/porn91.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/porncom.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/porncom.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornez.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornez.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornflip.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornflip.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornhd.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornhd.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornhub.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornhub.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornotube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornotube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornovoisines.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornovoisines.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pornoxo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pornoxo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pr0gramm.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pr0gramm.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/prankcast.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/prankcast.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/premiershiprugby.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/premiershiprugby.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/presstv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/presstv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/projectveritas.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/projectveritas.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/prosiebensat1.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/prosiebensat1.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/prx.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/prx.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/puhutv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/puhutv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/puls4.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/puls4.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/pyvideo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/pyvideo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/qingting.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/qingting.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/qqmusic.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/qqmusic.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/r7.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/r7.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiko.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiko.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiobremen.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiobremen.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiocanada.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiocanada.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiode.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiode.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiofrance.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiofrance.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiojavan.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiojavan.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiokapital.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiokapital.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radiozet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radiozet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/radlive.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/radlive.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rai.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rai.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/raywenderlich.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/raywenderlich.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rbgtum.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rbgtum.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rbmaradio.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rbmaradio.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rcs.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rcs.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rcti.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rcti.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rds.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rds.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/redbee.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/redbee.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/redbulltv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/redbulltv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/reddit.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/reddit.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/redgifs.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/redgifs.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/redtube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/redtube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/regiotv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/regiotv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rentv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rentv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/restudy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/restudy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/reuters.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/reuters.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/reverbnation.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/reverbnation.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rice.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rice.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rmcdecouverte.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rmcdecouverte.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rockstargames.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rockstargames.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rokfin.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rokfin.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/roosterteeth.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/roosterteeth.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rottentomatoes.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rozhlas.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rozhlas.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rte.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rte.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtl2.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtl2.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtlnl.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtlnl.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtnews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtnews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtrfm.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtrfm.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rts.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rts.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtve.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtve.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtvnh.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtvnh.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtvs.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtvs.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rtvslo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rtvslo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ruhd.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ruhd.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rule34video.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rule34video.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rumble.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rumble.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rutube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rutube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/rutv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/rutv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ruutu.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ruutu.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ruv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ruv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/safari.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/safari.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/saitosan.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/saitosan.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/samplefocus.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/samplefocus.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sapo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sapo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/savefrom.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/savefrom.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sbs.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sbs.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/screen9.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/screen9.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/screencast.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/screencast.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/screencastify.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/screencastify.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/screencastomatic.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/screencastomatic.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/scrippsnetworks.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/scrippsnetworks.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/scrolller.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/scrolller.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/scte.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/scte.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/seeker.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/seeker.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/senategov.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/senategov.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sendtonews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sendtonews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/servus.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/servus.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sevenplus.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sevenplus.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sexu.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sexu.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/seznamzpravy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/seznamzpravy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/shahid.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/shahid.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/shared.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/shared.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/shemaroome.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/shemaroome.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/showroomlive.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/showroomlive.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sibnet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sibnet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/simplecast.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/simplecast.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sina.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sina.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sixplay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sixplay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/skeb.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/skeb.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sky.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sky.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/skyit.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/skyit.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/skylinewebcams.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/skylinewebcams.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/skynewsarabia.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/skynewsarabia.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/skynewsau.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/skynewsau.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/slideshare.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/slideshare.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/slideslive.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/slideslive.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/slutload.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/slutload.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/smotrim.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/smotrim.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/snotr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/snotr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sohu.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sohu.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sonyliv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sonyliv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/soundcloud.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/soundcloud.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/soundgasm.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/soundgasm.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/southpark.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/southpark.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sovietscloset.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sovietscloset.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spankbang.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spankbang.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spankwire.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spankwire.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spiegel.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spiegel.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spike.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spike.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sport5.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sport5.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sportbox.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sportbox.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sportdeutschland.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sportdeutschland.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spotify.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spotify.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/spreaker.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/spreaker.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/springboardplatform.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/springboardplatform.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sprout.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sprout.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/srgssr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/srgssr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/srmediathek.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/srmediathek.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/stanfordoc.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/stanfordoc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/startrek.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/startrek.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/startv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/startv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/steam.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/steam.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/stitcher.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/stitcher.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/storyfire.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/storyfire.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streamable.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streamable.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streamanity.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streamanity.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streamcloud.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streamcloud.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streamcz.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streamcz.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streamff.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streamff.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/streetvoice.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/streetvoice.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/stretchinternet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/stretchinternet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/stripchat.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/stripchat.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/stv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/stv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/substack.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/substack.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sunporno.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sunporno.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sverigesradio.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sverigesradio.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/svt.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/svt.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/swearnet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/swearnet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/swrmediathek.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/swrmediathek.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/syfy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/syfy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/syvdk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/syvdk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/sztvhu.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/sztvhu.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tagesschau.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tagesschau.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tass.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tass.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tbs.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tbs.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tdslifeway.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tdslifeway.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teachable.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teachable.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teachertube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teachertube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teachingchannel.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teachingchannel.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teamcoco.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teamcoco.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teamtreehouse.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teamtreehouse.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/techtalks.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/techtalks.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ted.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ted.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tele13.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tele13.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tele5.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tele5.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telebruxelles.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telebruxelles.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telecaribe.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telecaribe.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telecinco.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telecinco.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telegraaf.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telegraaf.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telegram.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telegram.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telemb.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telemb.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telemundo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telemundo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telequebec.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telequebec.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/teletask.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/teletask.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/telewebion.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/telewebion.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tempo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tempo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tencent.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tencent.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tennistv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tennistv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tenplay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tenplay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/testurl.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/testurl.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tf1.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tf1.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tfo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tfo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/theholetv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/theholetv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/theintercept.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/theintercept.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/theplatform.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/theplatform.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thestar.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thestar.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thesun.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thesun.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/theta.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/theta.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/theweatherchannel.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/theweatherchannel.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thisamericanlife.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thisamericanlife.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thisav.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thisav.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thisoldhouse.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thisoldhouse.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/thisvid.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/thisvid.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/threeqsdn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/threeqsdn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/threespeak.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/threespeak.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tiktok.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tiktok.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tinypic.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tinypic.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tmz.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tmz.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tnaflix.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tnaflix.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/toggle.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/toggle.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/toggo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/toggo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tokentube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tokentube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tonline.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tonline.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/toongoggles.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/toongoggles.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/toutv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/toutv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/toypics.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/toypics.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/traileraddict.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/traileraddict.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/triller.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/triller.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trilulilu.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trilulilu.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trovo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trovo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trtcocuk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trtcocuk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trueid.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trueid.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trunews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trunews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/truth.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/truth.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/trutv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/trutv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tube8.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tube8.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tubetugraz.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tubetugraz.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tubitv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tubitv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tumblr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tumblr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tunein.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tunein.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tunepk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tunepk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/turbo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/turbo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/turner.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/turner.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv2.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv2.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv24ua.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv24ua.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv2dk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv2dk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv2hu.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv2hu.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv4.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv4.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv5mondeplus.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv5mondeplus.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tv5unis.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tv5unis.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tva.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tva.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvanouvelles.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvanouvelles.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvc.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvc.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tver.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tver.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvigle.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvigle.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tviplayer.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tviplayer.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvland.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvland.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvn24.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvn24.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvnet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvnet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvnoe.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvnoe.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvnow.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvnow.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvopengr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvopengr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvplay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvplay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tvplayer.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tvplayer.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/tweakers.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/tweakers.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twentyfourvideo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twentyfourvideo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twentymin.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twentymin.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twentythreevideo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twentythreevideo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twitcasting.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twitcasting.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twitch.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twitch.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/twitter.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/twitter.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/txxx.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/txxx.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/udemy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/udemy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/udn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/udn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ukcolumn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ukcolumn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/uktvplay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/uktvplay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/umg.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/umg.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/unistra.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/unistra.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/unity.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/unity.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/unscripted.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/unscripted.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/unsupported.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/unsupported.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/uol.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/uol.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/uplynk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/uplynk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/urort.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/urort.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/urplay.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/urplay.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/usanetwork.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/usanetwork.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/usatoday.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/usatoday.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ustream.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ustream.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ustudio.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ustudio.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/utreon.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/utreon.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/varzesh3.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/varzesh3.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vbox7.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vbox7.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/veehd.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/veehd.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/veo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/veo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/veoh.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/veoh.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vesti.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vesti.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vevo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vevo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vgtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vgtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vh1.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vh1.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vice.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vice.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vidbit.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vidbit.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viddler.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viddler.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videa.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videa.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videocampus_sachsen.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videocampus_sachsen.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videodetective.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videodetective.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videofyme.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videofyme.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videoken.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videoken.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videomore.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videomore.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/videopress.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/videopress.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vidio.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vidio.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vidlii.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vidlii.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viewlift.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viewlift.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viidea.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viidea.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viki.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viki.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vimeo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vimeo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vimm.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vimm.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vimple.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vimple.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vine.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vine.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viqeo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viqeo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/viu.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/viu.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vocaroo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vocaroo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vodlocker.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vodlocker.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vodpl.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vodpl.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vodplatform.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vodplatform.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/voicerepublic.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/voicerepublic.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/voicy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/voicy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/volejtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/volejtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/voot.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/voot.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/voxmedia.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/voxmedia.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vrak.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vrak.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vrt.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vrt.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vrv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vrv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vshare.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vshare.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vtm.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vtm.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vuclip.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vuclip.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vupload.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vupload.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vvvvid.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vvvvid.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vyborymos.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vyborymos.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/vzaar.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/vzaar.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wakanim.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wakanim.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/walla.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/walla.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wasdtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wasdtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/washingtonpost.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wat.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wat.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/watchbox.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/watchbox.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/watchindianporn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/watchindianporn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wdr.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wdr.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/webcamerapl.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/webcamerapl.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/webcaster.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/webcaster.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/webofstories.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/webofstories.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/weibo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/weibo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/weiqitv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/weiqitv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/whowatch.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/whowatch.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wikimedia.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wikimedia.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/willow.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/willow.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wimtv.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wimtv.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wistia.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wistia.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wordpress.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wordpress.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/worldstarhiphop.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/worldstarhiphop.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wppilot.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wppilot.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wrestleuniverse.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wrestleuniverse.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wsj.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wsj.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/wwe.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/wwe.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xanimu.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xanimu.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xbef.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xbef.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xboxclips.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xboxclips.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xfileshare.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xfileshare.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xhamster.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xhamster.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ximalaya.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ximalaya.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xinpianchang.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xinpianchang.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xminus.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xminus.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xnxx.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xnxx.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xstream.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xstream.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xtube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xtube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xuite.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xuite.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xvideos.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xvideos.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/xxxymovies.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/xxxymovies.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yahoo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yahoo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yandexdisk.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yandexdisk.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yandexmusic.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yandexmusic.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yandexvideo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yandexvideo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yapfiles.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yapfiles.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yappy.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yappy.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yesjapan.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yesjapan.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yinyuetai.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yinyuetai.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yle_areena.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yle_areena.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/ynet.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/ynet.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/youjizz.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/youjizz.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/youku.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/youku.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/younow.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/younow.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/youporn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/youporn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yourporn.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yourporn.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/yourupload.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/yourupload.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/youtube.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/youtube.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zapiks.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zapiks.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zattoo.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zattoo.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zdf.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zdf.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zee5.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zee5.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zeenews.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zeenews.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zhihu.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zhihu.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zingmp3.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zingmp3.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zoom.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zoom.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/extractor/zype.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/extractor/zype.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/flserver.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/flserver.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/jsinterp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/jsinterp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/minicurses.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/minicurses.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/options.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/options.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/plugins.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/plugins.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/__init__.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/common.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/common.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/embedthumbnail.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/embedthumbnail.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/exec.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/exec.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/ffmpeg.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/metadataparser.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/metadataparser.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/modify_chapters.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/modify_chapters.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/movefilesafterdownload.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/movefilesafterdownload.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/sponskrub.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/sponskrub.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/sponsorblock.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/sponsorblock.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/postprocessor/xattrpp.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/postprocessor/xattrpp.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/server1.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/server1.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/socks.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/socks.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/update.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/update.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/utils.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/utils.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp/webvtt.py` & `yt-dlp-cp-1.9.9/yt_dlp_cp/webvtt.py`

 * *Files identical despite different names*

### Comparing `yt-dlp-cp-0.9.9/yt_dlp_cp.egg-info/SOURCES.txt` & `yt-dlp-cp-1.9.9/yt_dlp_cp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

