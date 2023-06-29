# Comparing `tmp/translators-5.7.7.tar.gz` & `tmp/translators-5.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translators-5.7.7.tar", last modified: Thu Jun 29 14:32:34 2023, max compression
+gzip compressed data, was "translators-5.7.8.tar", last modified: Thu Jun 29 18:50:09 2023, max compression
```

## Comparing `translators-5.7.7.tar` & `translators-5.7.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:34.475466 translators-5.7.7/
--rw-rw-rw-   0        0        0    35821 2023-06-29 09:26:06.000000 translators-5.7.7/LICENSE
--rw-rw-rw-   0        0        0      113 2023-05-15 23:01:25.000000 translators-5.7.7/MANIFEST.in
--rw-rw-rw-   0        0        0    67914 2023-06-29 14:32:34.475466 translators-5.7.7/PKG-INFO
--rw-rw-rw-   0        0        0    66420 2023-06-29 14:23:17.000000 translators-5.7.7/README.md
--rw-rw-rw-   0        0        0    66378 2023-06-29 14:23:17.000000 translators-5.7.7/README_history.md
--rw-rw-rw-   0        0        0     8719 2023-06-29 13:48:32.000000 translators-5.7.7/change_log.txt
--rw-rw-rw-   0        0        0      138 2022-10-21 20:53:52.000000 translators-5.7.7/pyproject.toml
--rw-rw-rw-   0        0        0       54 2023-03-09 23:10:40.000000 translators-5.7.7/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 14:32:34.476483 translators-5.7.7/setup.cfg
--rw-rw-rw-   0        0        0     2669 2023-06-29 14:32:21.000000 translators-5.7.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:34.467043 translators-5.7.7/translators/
--rw-rw-rw-   0        0        0      162 2023-06-29 13:36:57.000000 translators-5.7.7/translators/__init__.py
--rw-rw-rw-   0        0        0   275186 2023-06-29 13:48:32.000000 translators-5.7.7/translators/server.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:34.474466 translators-5.7.7/translators.egg-info/
--rw-rw-rw-   0        0        0    67914 2023-06-29 14:32:34.000000 translators-5.7.7/translators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-06-29 14:32:34.000000 translators-5.7.7/translators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:32:34.000000 translators-5.7.7/translators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-29 14:32:34.000000 translators-5.7.7/translators.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      127 2023-06-29 14:32:34.000000 translators-5.7.7/translators.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-29 14:32:34.000000 translators-5.7.7/translators.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 18:50:09.594185 translators-5.7.8/
+-rw-rw-rw-   0        0        0    35821 2023-06-29 09:26:06.000000 translators-5.7.8/LICENSE
+-rw-rw-rw-   0        0        0      113 2023-05-15 23:01:25.000000 translators-5.7.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    68063 2023-06-29 18:50:09.594185 translators-5.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0    66569 2023-06-29 18:41:04.000000 translators-5.7.8/README.md
+-rw-rw-rw-   0        0        0    66527 2023-06-29 18:46:25.000000 translators-5.7.8/README_history.md
+-rw-rw-rw-   0        0        0     8792 2023-06-29 18:49:58.000000 translators-5.7.8/change_log.txt
+-rw-rw-rw-   0        0        0      138 2022-10-21 20:53:52.000000 translators-5.7.8/pyproject.toml
+-rw-rw-rw-   0        0        0       54 2023-03-09 23:10:40.000000 translators-5.7.8/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 18:50:09.595181 translators-5.7.8/setup.cfg
+-rw-rw-rw-   0        0        0     2669 2023-06-29 14:32:21.000000 translators-5.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:50:09.585116 translators-5.7.8/translators/
+-rw-rw-rw-   0        0        0      162 2023-06-29 18:46:25.000000 translators-5.7.8/translators/__init__.py
+-rw-rw-rw-   0        0        0   275965 2023-06-29 18:42:49.000000 translators-5.7.8/translators/server.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:50:09.593186 translators-5.7.8/translators.egg-info/
+-rw-rw-rw-   0        0        0    68063 2023-06-29 18:50:09.000000 translators-5.7.8/translators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-06-29 18:50:09.000000 translators-5.7.8/translators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 18:50:09.000000 translators-5.7.8/translators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-29 18:50:09.000000 translators-5.7.8/translators.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      127 2023-06-29 18:50:09.000000 translators-5.7.8/translators.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-29 18:50:09.000000 translators-5.7.8/translators.egg-info/top_level.txt
```

### Comparing `translators-5.7.7/LICENSE` & `translators-5.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `translators-5.7.7/PKG-INFO` & `translators-5.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translators
-Version: 5.7.7
+Version: 5.7.8
 Summary: Translators is a library which aims to bring free, multiple, enjoyable translation to individuals and students in Python.
 Home-page: https://github.com/uliontse/translators
 Author: UlionTse
 Author-email: uliontse@outlook.com
 License: GPLv3
 Project-URL: Source, https://github.com/UlionTse/translators
 Project-URL: Changelog, https://github.com/UlionTse/translators/blob/master/change_log.txt
@@ -24,37 +24,37 @@
 Provides-Extra: pypi
 License-File: LICENSE
 
 <p align="center">
   <img src="https://github.com/UlionTse/translators/blob/master/docs/translators_logo.png" width="500"/>
 </p>
 <p align="center">
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/translators.svg"></a>
-  <a href="https://anaconda.org/conda-forge/translators"><img alt="Conda - Version" src="https://img.shields.io/conda/vn/conda-forge/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Python" src="https://img.shields.io/pypi/pyversions/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Status" src="https://img.shields.io/pypi/status/translators.svg"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/translators.svg?color=blue"></a>
+  <a href="https://anaconda.org/conda-forge/translators"><img alt="Conda - Version" src="https://img.shields.io/conda/vn/conda-forge/translators.svg?color=blue"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/translators.svg?color=brightgreen"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Python" src="https://img.shields.io/pypi/pyversions/translators.svg?color=blue"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Status" src="https://img.shields.io/pypi/status/translators.svg?color=brightgreen"></a>
   <a href="https://pypi.org/project/translators"><img alt="PyPI - Wheel" src="https://img.shields.io/badge/wheel-yes-brightgreen.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="Downloads" src="https://pepy.tech/badge/translators"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Downloads" src="https://static.pepy.tech/personalized-badge/translators?left_text=downloads&left_color=gray&right_color=blue"></a>
 </p>
 
 * * *
 
 **Translators** is a library which aims to bring **free, multiple, enjoyable** translation to individuals and students in Python. 
 
 <details>
 <summary>Supported Translation Services</summary>
 
 | ID  | Translator                                                                        | Number of Supported Languages | Advantage                                                                                   | Service                                                                                                           | Status                          |
 | --- | --------------------------------------------------------------------------------- | ----------------------------- | ------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ------------------------------- |
-| 1   | [Niutrans](https://niutrans.com/trans)                                            | 302                           | support the most languages in the world                                                     | [Northeastern University](http://english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China            | /                               |
-| 2   | [Alibaba](https://translate.alibaba.com)                                          | 221                           | support most languages, support professional field                                          | [Alibaba](https://damo.alibaba.com/about?lang=en), China                                                          | stable                          |
-| 3   | [Baidu](https://fanyi.baidu.com)                                                  | 201                           | support most languages, support professional field, support classical Chinese               | [Baidu](https://ir.baidu.com/company-overview), China                                                             | stable                          |
-| 4   | [Iciba](https://www.iciba.com/fy)                                                 | 187                           | support the most languages in the world                                                     | [Kingsoft](https://www.wps.com/about-us/) / [Xiaomi](https://www.mi.com/us/about/), China                         | stable                          |
-| 5   | [MyMemory](https://mymemory.translated.net)                                       | 151                           | support the most languages in the world, good at Creole English, Creole French              | [Translated](https://translatedlabs.com/welcome), Italy                                                           | stable                          |
+| 1   | [MyMemory](https://mymemory.translated.net)                                       | 330                           | support the most languages in the world                                                     | [Translated](https://translatedlabs.com/welcome), Italy                                                           | stable                          |
+| 2   | [Niutrans](https://niutrans.com/trans)                                            | 302                           | support the most languages in the world                                                     | [Northeastern University](http://english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China            | /                               |
+| 3   | [Alibaba](https://translate.alibaba.com)                                          | 221                           | support most languages, support professional field                                          | [Alibaba](https://damo.alibaba.com/about?lang=en), China                                                          | stable                          |
+| 4   | [Baidu](https://fanyi.baidu.com)                                                  | 201                           | support most languages, support professional field, support classical Chinese               | [Baidu](https://ir.baidu.com/company-overview), China                                                             | stable                          |
+| 5   | [Iciba](https://www.iciba.com/fy)                                                 | 187                           | support the most languages in the world                                                     | [Kingsoft](https://www.wps.com/about-us/) / [Xiaomi](https://www.mi.com/us/about/), China                         | stable                          |
 | 6   | [Iflytek](https://fanyi.xfyun.cn/console/trans/text)                              | 140                           | support the most languages in the world                                                     | [Iflytek](https://www.iflytek.com/en/about-us.html), China                                                        | /                               |
 | 7   | [Google](https://translate.google.com)                                            | 134                           | support more languages in the world                                                         | [Google](https://about.google/), America                                                                          | stable(offline in China inland) |
 | 8   | [VolcEngine](https://translate.volcengine.com)                                    | 122                           | support more languages in the world, support professional field                             | [ByteDance](https://www.bytedance.com/en/), China                                                                 | /                               |
 | 9   | [Lingvanex](https://lingvanex.com/demo)                                           | 112                           | support translation of different regions but the same language                              | [Lingvanex](https://lingvanex.com/about-us/), Cyprus                                                              | stable                          |
 | 10  | [Bing](https://www.bing.com/Translator)                                           | 110                           | support more languages in the world                                                         | [Microsoft](https://www.microsoft.com/en-us/about), America                                                       | stable                          |
 | 11  | [Yandex](https://translate.yandex.com)                                            | 102                           | support more languages in the world, support word to emoji                                  | [Yandex](https://yandex.com/company/), Russia                                                                     | /                               |
 | 12  | [Itranslate](https://itranslate.com/webapp)                                       | 101                           | support translation of different regions but the same language, such as en-US, en-UK, en-AU | [Itranslate](https://itranslate.com/about), Austria                                                               | stable                          |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: translators Version: 5.7.7 Summary: Translators is
+Metadata-Version: 2.1 Name: translators Version: 5.7.8 Summary: Translators is
 a library which aims to bring free, multiple, enjoyable translation to
 individuals and students in Python. Home-page: https://github.com/uliontse/
 translators Author: UlionTse Author-email: uliontse@outlook.com License: GPLv3
 Project-URL: Source, https://github.com/UlionTse/translators Project-URL:
 Changelog, https://github.com/UlionTse/translators/blob/master/change_log.txt
 Project-URL: Documentation, https://github.com/UlionTse/translators/blob/
 master/README.md Keywords:
@@ -13,99 +13,98 @@
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Provides-Extra: pypi License-File: LICENSE
 [https://github.com/UlionTse/translators/blob/master/docs/translators_logo.png]
   [PyPI_-_Version] [Conda_-_Version] [PyPI_-_License] [PyPI_-_Python] [PyPI_-
-                      Status] [PyPI_-_Wheel] [Downloads]
+                   Status] [PyPI_-_Wheel] [PyPI_-_Downloads]
 * * * **Translators** is a library which aims to bring **free, multiple,
 enjoyable** translation to individuals and students in Python.  Supported
 Translation Services | ID | Translator | Number of Supported Languages |
 Advantage | Service | Status | | --- | ----------------------------------------
 ----------------------------------------- | ----------------------------- | ---
 -------------------------------------------------------------------------------
 --------- | -------------------------------------------------------------------
 ---------------------------------------------- | ------------------------------
-- | | 1 | [Niutrans](https://niutrans.com/trans) | 302 | support the most
-languages in the world | [Northeastern University](http://english.neu.edu.cn/
-) / [Niutrans](https://github.com/NiuTrans), China | / | | 2 | [Alibaba](https:
-//translate.alibaba.com) | 221 | support most languages, support professional
-field | [Alibaba](https://damo.alibaba.com/about?lang=en), China | stable | | 3
-| [Baidu](https://fanyi.baidu.com) | 201 | support most languages, support
-professional field, support classical Chinese | [Baidu](https://ir.baidu.com/
-company-overview), China | stable | | 4 | [Iciba](https://www.iciba.com/fy) |
-187 | support the most languages in the world | [Kingsoft](https://www.wps.com/
-about-us/) / [Xiaomi](https://www.mi.com/us/about/), China | stable | | 5 |
-[MyMemory](https://mymemory.translated.net) | 151 | support the most languages
-in the world, good at Creole English, Creole French | [Translated](https://
-translatedlabs.com/welcome), Italy | stable | | 6 | [Iflytek](https://
-fanyi.xfyun.cn/console/trans/text) | 140 | support the most languages in the
-world | [Iflytek](https://www.iflytek.com/en/about-us.html), China | / | | 7 |
-[Google](https://translate.google.com) | 134 | support more languages in the
-world | [Google](https://about.google/), America | stable(offline in China
-inland) | | 8 | [VolcEngine](https://translate.volcengine.com) | 122 | support
-more languages in the world, support professional field | [ByteDance](https://
-www.bytedance.com/en/), China | / | | 9 | [Lingvanex](https://lingvanex.com/
-demo) | 112 | support translation of different regions but the same language |
-[Lingvanex](https://lingvanex.com/about-us/), Cyprus | stable | | 10 | [Bing]
-(https://www.bing.com/Translator) | 110 | support more languages in the world |
-[Microsoft](https://www.microsoft.com/en-us/about), America | stable | | 11 |
-[Yandex](https://translate.yandex.com) | 102 | support more languages in the
-world, support word to emoji | [Yandex](https://yandex.com/company/), Russia |
-/ | | 12 | [Itranslate](https://itranslate.com/webapp) | 101 | support
-translation of different regions but the same language, such as en-US, en-UK,
-en-AU | [Itranslate](https://itranslate.com/about), Austria | stable | | 13 |
-[Sogou](https://fanyi.sogou.com/text) | 61 | support more languages in the
-world | [Tencent](https://www.tencent.com/en-us/about.html), China | stable | |
-14 | [ModernMt](https://www.modernmt.com/translate) | 56 | open-source, support
-more languages in the world | [Modernmt](https://github.com/modernmt) /
-[Translated](https://translatedlabs.com/welcome), Italy | stable | | 15 |
-[SysTran](https://www.systran.net/translate/) | 52 | support more languages in
-the world | [SysTran](https://www.systran.net/about/), France | stable | | 16 |
-[Apertium](https://www.apertium.org/) | 45 | open-source | [Apertium](https://
-github.com/apertium), Spain | stable | | 17 | [Reverso](https://
-www.reverso.net/text-translation) | 42 | popular on Mac and Iphone | [Reverso]
-(https://www.corporate-translation.reverso.com/about-us), France | stable | |
-18 | [CloudYi](https://www.cloudtranslation.com/#/translate) | 28 | support
-main languages | [Xiamen University](http://nlp.xmu.edu.cn/) /
-[CloudTranslation](https://www.cloudtranslation.com/#/about), China | stable |
-| 19 | [Deepl](https://www.deepl.com/translator) | 27 | high quality to
-translate but response slowly | [Deepl](https://jobs.deepl.com/l/en), Germany |
-stable | | 20 | [QQTranSmart](https://transmart.qq.com) | 22 | support main
-languages | [Tencent](https://www.tencent.com/en-us/about.html), China | stable
-| | 21 | [TranslateCom](https://www.translate.com/machine-translation) | 21 |
-good at English translation | [TranslateCom](https://www.translate.com/about-
-us), America | stable | | 22 | [Tilde](https://translate.tilde.com/) | 21 |
-good at lv, de, fr translation | [Tilde](https://tilde.com/about), Latvia | / |
-| 23 | [QQFanyi](https://fanyi.qq.com) | 17 | support main languages |
-[Tencent](https://www.tencent.com/en-us/about.html), China | stable | | 24 |
-[Argos](https://translate.argosopentech.com) | 17 | open-source | [Argos]
-(https://github.com/argosopentech) / [Libre](https://github.com/
-LibreTranslate), America | stable | | 25 | [TranslateMe](https://
-translateme.network/) | 16 | good at English translation | [TranslateMe](https:
-//translateme.network/our-team/) / [Neosus](https://neosus.net/about/),
-Lithuania | / | | 26 | [Youdao](https://ai.youdao.com/product-fanyi-text.s) |
-15 | support main languages, high quality | [Netease](https://ir.netease.com/
-company-overview/corporate-profile), China | stable | | 27 | [Papago](https://
-papago.naver.com) | 15 | good at Korean translation | [Naver](https://
-www.navercorp.com/en/naver/company), South Korea | stable | | 28 | [Marai]
-(https://miraitranslate.com/trial/) | 15 | good at Japanese translation |
-[MaraiTranslate](https://miraitranslate.com/en/company/), Japan | / | | 29 |
-[Iflyrec](https://fanyi.iflyrec.com) | 12 | good at Chinese translation |
-[Iflytek](https://www.iflytek.com/en/about-us.html), China | stable | | 30 |
-[Yeekit](https://www.yeekit.com/site/translate) | 10 | support main languages |
-[CTC](https://www.ctpc.com.cn/cms/enAboutUs.htm), China | / | | 31 |
-[LanguageWire](https://www.languagewire.com/en/technology/languagewire-
-translate) | 8 | good at English translation | [LanguageWire](https://
-www.languagewire.com/about-us), Denmark | stable | | 32 | [Caiyun](https://
-fanyi.caiyunapp.com) | 7 | high quality to translate but response slowly,
-support professional field | [ColorfulClouds](http://caiyunapp.com/jobs/),
-China | stable | | 33 | [Elia](https://elia.eus/translator) | 6 | good at
-Basque translation | [Elhuyar](https://www.elhuyar.eus/eu/nor-gara), Spain |
+- | | 1 | [MyMemory](https://mymemory.translated.net) | 330 | support the most
+languages in the world | [Translated](https://translatedlabs.com/welcome),
+Italy | stable | | 2 | [Niutrans](https://niutrans.com/trans) | 302 | support
+the most languages in the world | [Northeastern University](http://
+english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China | / | | 3
+| [Alibaba](https://translate.alibaba.com) | 221 | support most languages,
+support professional field | [Alibaba](https://damo.alibaba.com/about?lang=en),
+China | stable | | 4 | [Baidu](https://fanyi.baidu.com) | 201 | support most
+languages, support professional field, support classical Chinese | [Baidu]
+(https://ir.baidu.com/company-overview), China | stable | | 5 | [Iciba](https:/
+/www.iciba.com/fy) | 187 | support the most languages in the world | [Kingsoft]
+(https://www.wps.com/about-us/) / [Xiaomi](https://www.mi.com/us/about/), China
+| stable | | 6 | [Iflytek](https://fanyi.xfyun.cn/console/trans/text) | 140 |
+support the most languages in the world | [Iflytek](https://www.iflytek.com/en/
+about-us.html), China | / | | 7 | [Google](https://translate.google.com) | 134
+| support more languages in the world | [Google](https://about.google/),
+America | stable(offline in China inland) | | 8 | [VolcEngine](https://
+translate.volcengine.com) | 122 | support more languages in the world, support
+professional field | [ByteDance](https://www.bytedance.com/en/), China | / | |
+9 | [Lingvanex](https://lingvanex.com/demo) | 112 | support translation of
+different regions but the same language | [Lingvanex](https://lingvanex.com/
+about-us/), Cyprus | stable | | 10 | [Bing](https://www.bing.com/Translator) |
+110 | support more languages in the world | [Microsoft](https://
+www.microsoft.com/en-us/about), America | stable | | 11 | [Yandex](https://
+translate.yandex.com) | 102 | support more languages in the world, support word
+to emoji | [Yandex](https://yandex.com/company/), Russia | / | | 12 |
+[Itranslate](https://itranslate.com/webapp) | 101 | support translation of
+different regions but the same language, such as en-US, en-UK, en-AU |
+[Itranslate](https://itranslate.com/about), Austria | stable | | 13 | [Sogou]
+(https://fanyi.sogou.com/text) | 61 | support more languages in the world |
+[Tencent](https://www.tencent.com/en-us/about.html), China | stable | | 14 |
+[ModernMt](https://www.modernmt.com/translate) | 56 | open-source, support more
+languages in the world | [Modernmt](https://github.com/modernmt) / [Translated]
+(https://translatedlabs.com/welcome), Italy | stable | | 15 | [SysTran](https:/
+/www.systran.net/translate/) | 52 | support more languages in the world |
+[SysTran](https://www.systran.net/about/), France | stable | | 16 | [Apertium]
+(https://www.apertium.org/) | 45 | open-source | [Apertium](https://github.com/
+apertium), Spain | stable | | 17 | [Reverso](https://www.reverso.net/text-
+translation) | 42 | popular on Mac and Iphone | [Reverso](https://
+www.corporate-translation.reverso.com/about-us), France | stable | | 18 |
+[CloudYi](https://www.cloudtranslation.com/#/translate) | 28 | support main
+languages | [Xiamen University](http://nlp.xmu.edu.cn/) / [CloudTranslation]
+(https://www.cloudtranslation.com/#/about), China | stable | | 19 | [Deepl]
+(https://www.deepl.com/translator) | 27 | high quality to translate but
+response slowly | [Deepl](https://jobs.deepl.com/l/en), Germany | stable | | 20
+| [QQTranSmart](https://transmart.qq.com) | 22 | support main languages |
+[Tencent](https://www.tencent.com/en-us/about.html), China | stable | | 21 |
+[TranslateCom](https://www.translate.com/machine-translation) | 21 | good at
+English translation | [TranslateCom](https://www.translate.com/about-us),
+America | stable | | 22 | [Tilde](https://translate.tilde.com/) | 21 | good at
+lv, de, fr translation | [Tilde](https://tilde.com/about), Latvia | / | | 23 |
+[QQFanyi](https://fanyi.qq.com) | 17 | support main languages | [Tencent]
+(https://www.tencent.com/en-us/about.html), China | stable | | 24 | [Argos]
+(https://translate.argosopentech.com) | 17 | open-source | [Argos](https://
+github.com/argosopentech) / [Libre](https://github.com/LibreTranslate), America
+| stable | | 25 | [TranslateMe](https://translateme.network/) | 16 | good at
+English translation | [TranslateMe](https://translateme.network/our-team/) /
+[Neosus](https://neosus.net/about/), Lithuania | / | | 26 | [Youdao](https://
+ai.youdao.com/product-fanyi-text.s) | 15 | support main languages, high quality
+| [Netease](https://ir.netease.com/company-overview/corporate-profile), China |
+stable | | 27 | [Papago](https://papago.naver.com) | 15 | good at Korean
+translation | [Naver](https://www.navercorp.com/en/naver/company), South Korea
+| stable | | 28 | [Marai](https://miraitranslate.com/trial/) | 15 | good at
+Japanese translation | [MaraiTranslate](https://miraitranslate.com/en/company/
+), Japan | / | | 29 | [Iflyrec](https://fanyi.iflyrec.com) | 12 | good at
+Chinese translation | [Iflytek](https://www.iflytek.com/en/about-us.html),
+China | stable | | 30 | [Yeekit](https://www.yeekit.com/site/translate) | 10 |
+support main languages | [CTC](https://www.ctpc.com.cn/cms/enAboutUs.htm),
+China | / | | 31 | [LanguageWire](https://www.languagewire.com/en/technology/
+languagewire-translate) | 8 | good at English translation | [LanguageWire]
+(https://www.languagewire.com/about-us), Denmark | stable | | 32 | [Caiyun]
+(https://fanyi.caiyunapp.com) | 7 | high quality to translate but response
+slowly, support professional field | [ColorfulClouds](http://caiyunapp.com/
+jobs/), China | stable | | 33 | [Elia](https://elia.eus/translator) | 6 | good
+at Basque translation | [Elhuyar](https://www.elhuyar.eus/eu/nor-gara), Spain |
 stable | | 34 | [Judic](https://judic.io/en/translate) | 4 | good at European
 translation | [CrossLang](https://crosslang.com/about-us/), Belgium | stable |
 | 35 | [Mglip](http://fy.mglip.com/pc) | 3 | good at Mongolia translation |
 [Inner Mongolia University](https://www.imu.edu.cn/yw/Home.htm), China | stable
 | | 36 | [Utibet](http://mt.utibet.edu.cn/mt) | 2 | good at Tibet translation |
 [Tibet University](http://www.utibet.edu.cn/), China | stable |   Installation
 ```sh # PYPI pip install --upgrade translators # Conda conda install -c conda-
```

### Comparing `translators-5.7.7/README.md` & `translators-5.7.8/README_history.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 <p align="center">
   <img src="https://github.com/UlionTse/translators/blob/master/docs/translators_logo.png" width="500"/>
 </p>
 <p align="center">
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/translators.svg"></a>
-  <a href="https://anaconda.org/conda-forge/translators"><img alt="Conda - Version" src="https://img.shields.io/conda/vn/conda-forge/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Python" src="https://img.shields.io/pypi/pyversions/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Status" src="https://img.shields.io/pypi/status/translators.svg"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/translators.svg?color=blue"></a>
+  <a href="https://anaconda.org/conda-forge/translators"><img alt="Conda - Version" src="https://img.shields.io/conda/vn/conda-forge/translators.svg?color=blue"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/translators.svg?color=brightgreen"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Python" src="https://img.shields.io/pypi/pyversions/translators.svg?color=blue"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Status" src="https://img.shields.io/pypi/status/translators.svg?color=brightgreen"></a>
   <a href="https://pypi.org/project/translators"><img alt="PyPI - Wheel" src="https://img.shields.io/badge/wheel-yes-brightgreen.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="Downloads" src="https://pepy.tech/badge/translators"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Downloads" src="https://static.pepy.tech/personalized-badge/translators?left_text=downloads&left_color=gray&right_color=blue"></a>
 </p>
 
 * * *
 
 **Translators** is a library which aims to bring **free, multiple, enjoyable** translation to individuals and students in Python. 
 
-<details>
-<summary>Supported Translation Services</summary>
+- [Supported Translation Services](#supported-translation-services)
+- [Installation](#installation)
+- [Getting Started](#getting-started)
+- [Supported Languages](#supported-languages)
+- [Debug Tips](#debug-tips)
+- [License](#license)
+
+## Supported Translation Services
 
 | ID  | Translator                                                                        | Number of Supported Languages | Advantage                                                                                   | Service                                                                                                           | Status                          |
 | --- | --------------------------------------------------------------------------------- | ----------------------------- | ------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ------------------------------- |
-| 1   | [Niutrans](https://niutrans.com/trans)                                            | 302                           | support the most languages in the world                                                     | [Northeastern University](http://english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China            | /                               |
-| 2   | [Alibaba](https://translate.alibaba.com)                                          | 221                           | support most languages, support professional field                                          | [Alibaba](https://damo.alibaba.com/about?lang=en), China                                                          | stable                          |
-| 3   | [Baidu](https://fanyi.baidu.com)                                                  | 201                           | support most languages, support professional field, support classical Chinese               | [Baidu](https://ir.baidu.com/company-overview), China                                                             | stable                          |
-| 4   | [Iciba](https://www.iciba.com/fy)                                                 | 187                           | support the most languages in the world                                                     | [Kingsoft](https://www.wps.com/about-us/) / [Xiaomi](https://www.mi.com/us/about/), China                         | stable                          |
-| 5   | [MyMemory](https://mymemory.translated.net)                                       | 151                           | support the most languages in the world, good at Creole English, Creole French              | [Translated](https://translatedlabs.com/welcome), Italy                                                           | stable                          |
+| 1   | [MyMemory](https://mymemory.translated.net)                                       | 330                           | support the most languages in the world                                                     | [Translated](https://translatedlabs.com/welcome), Italy                                                           | stable                          |
+| 2   | [Niutrans](https://niutrans.com/trans)                                            | 302                           | support the most languages in the world                                                     | [Northeastern University](http://english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China            | /                               |
+| 3   | [Alibaba](https://translate.alibaba.com)                                          | 221                           | support most languages, support professional field                                          | [Alibaba](https://damo.alibaba.com/about?lang=en), China                                                          | stable                          |
+| 4   | [Baidu](https://fanyi.baidu.com)                                                  | 201                           | support most languages, support professional field, support classical Chinese               | [Baidu](https://ir.baidu.com/company-overview), China                                                             | stable                          |
+| 5   | [Iciba](https://www.iciba.com/fy)                                                 | 187                           | support the most languages in the world                                                     | [Kingsoft](https://www.wps.com/about-us/) / [Xiaomi](https://www.mi.com/us/about/), China                         | stable                          |
 | 6   | [Iflytek](https://fanyi.xfyun.cn/console/trans/text)                              | 140                           | support the most languages in the world                                                     | [Iflytek](https://www.iflytek.com/en/about-us.html), China                                                        | /                               |
 | 7   | [Google](https://translate.google.com)                                            | 134                           | support more languages in the world                                                         | [Google](https://about.google/), America                                                                          | stable(offline in China inland) |
 | 8   | [VolcEngine](https://translate.volcengine.com)                                    | 122                           | support more languages in the world, support professional field                             | [ByteDance](https://www.bytedance.com/en/), China                                                                 | /                               |
 | 9   | [Lingvanex](https://lingvanex.com/demo)                                           | 112                           | support translation of different regions but the same language                              | [Lingvanex](https://lingvanex.com/about-us/), Cyprus                                                              | stable                          |
 | 10  | [Bing](https://www.bing.com/Translator)                                           | 110                           | support more languages in the world                                                         | [Microsoft](https://www.microsoft.com/en-us/about), America                                                       | stable                          |
 | 11  | [Yandex](https://translate.yandex.com)                                            | 102                           | support more languages in the world, support word to emoji                                  | [Yandex](https://yandex.com/company/), Russia                                                                     | /                               |
 | 12  | [Itranslate](https://itranslate.com/webapp)                                       | 101                           | support translation of different regions but the same language, such as en-US, en-UK, en-AU | [Itranslate](https://itranslate.com/about), Austria                                                               | stable                          |
@@ -53,36 +59,30 @@
 | 31  | [LanguageWire](https://www.languagewire.com/en/technology/languagewire-translate) | 8                             | good at English translation                                                                 | [LanguageWire](https://www.languagewire.com/about-us), Denmark                                                    | stable                          |
 | 32  | [Caiyun](https://fanyi.caiyunapp.com)                                             | 7                             | high quality to translate but response slowly, support professional field                   | [ColorfulClouds](http://caiyunapp.com/jobs/), China                                                               | stable                          |
 | 33  | [Elia](https://elia.eus/translator)                                               | 6                             | good at Basque translation                                                                  | [Elhuyar](https://www.elhuyar.eus/eu/nor-gara), Spain                                                             | stable                          |
 | 34  | [Judic](https://judic.io/en/translate)                                            | 4                             | good at European translation                                                                | [CrossLang](https://crosslang.com/about-us/), Belgium                                                             | stable                          |
 | 35  | [Mglip](http://fy.mglip.com/pc)                                                   | 3                             | good at Mongolia translation                                                                | [Inner Mongolia University](https://www.imu.edu.cn/yw/Home.htm), China                                            | stable                          |
 | 36  | [Utibet](http://mt.utibet.edu.cn/mt)                                              | 2                             | good at Tibet translation                                                                   | [Tibet University](http://www.utibet.edu.cn/), China                                                              | stable                          |
 
-</details>
-
-<details>
-<summary>Installation</summary>
+## Installation
 
 ```sh
 # PYPI
 pip install --upgrade translators
 
 # Conda
 conda install -c conda-forge translators
 
 # Source
 git clone https://github.com/UlionTse/translators.git
 cd translators
 python setup.py install
 ```
 
-</details>
-
-<details>
-<summary>Getting Started</summary>
+## Getting Started
 
 ```python
 import translators as ts
 
 q_text = '季姬寂，集鸡，鸡即棘鸡。棘鸡饥叽，季姬及箕稷济鸡。'
 q_html = '''<!DOCTYPE html><html><head><title>《季姬击鸡记》</title></head><body><p>还有另一篇文章《施氏食狮史》。</p></body></html>'''
 
@@ -122,18 +122,15 @@
             :param if_print_warning: bool, default True.
             :param lingvanex_mode: str, default 'B2C', choose from ("B2C", "B2B").
             :param myMemory_mode: str, default "web", choose from ("web", "api").
     :return: str or dict
 """
 ```
 
-</details>
-
-<details>
-<summary>Supported Languages</summary>
+## Supported Languages
 
 | Language             | Language of Translator | [Google](https://translate.google.com) | [Yandex](https://translate.yandex.com) | [Bing](https://www.bing.com/Translator) | [Baidu](https://fanyi.baidu.com) | [Alibaba](https://translate.alibaba.com) | [Tencent](https://fanyi.qq.com) | [Youdao](https://fanyi.youdao.com) | [Sogou](https://fanyi.sogou.com) | [Deepl](https://www.deepl.com/translator) | [Caiyun](https://fanyi.caiyunapp.com) | [Argos](https://translate.argosopentech.com) | others... |
 | -------------------- | ---------------------- | -------------------------------------- | -------------------------------------- | --------------------------------------- | -------------------------------- | ---------------------------------------- | ------------------------------- | ---------------------------------- | -------------------------------- | ----------------------------------------- | ------------------------------------- | -------------------------------------------- | --------- |
 | english              | en                     | Y                                      | Y                                      | Y                                       | Y                                | Y                                        | Y                               | Y                                  | Y                                | Y                                         | Y                                     | Y                                            | ...       |
 | chinese              | zh                     | Y                                      | Y                                      | Y                                       | Y                                | Y                                        | Y                               | Y                                  | Y                                | Y                                         | Y                                     | Y                                            |           |
 | arabic               | ar                     | Y                                      | Y                                      | Y                                       | Y(ara)                           | Y                                        | Y                               | Y                                  | Y                                |                                           |                                       | Y                                            |           |
 | russian              | ru                     | Y                                      | Y                                      | Y                                       | Y                                | Y                                        | Y                               | Y                                  | Y                                | Y                                         | Y                                     | Y                                            |           |
@@ -201,16 +198,15 @@
 | chuvash              | cv                     |                                        | Y                                      |                                         |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 | esperanto            | eo                     | Y                                      | Y                                      |                                         |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 | basque               | eu                     | Y                                      | Y                                      |                                         |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 | irish                | ga                     | Y                                      | Y                                      | Y                                       |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 | emoji                | emj                    |                                        | Y                                      |                                         |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 | ...                  | ...                    |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 
-<details>
-<summary>About Chinese Language</summary>
+### About Chinese Language
 
 | Language      | Language of Translator | [Google](https://translate.google.com) | [Yandex](https://translate.yandex.com) | [Bing](https://www.bing.com/Translator) | [Baidu](https://fanyi.baidu.com) | [Alibaba](https://translate.alibaba.com) | [Tencent](https://fanyi.qq.com) | [Youdao](https://fanyi.youdao.com) | [Sogou](https://fanyi.sogou.com) | [Iciba](https://www.iciba.com/fy) | [Iflytek](https://fanyi.xfyun.cn/console/trans/text) | [Caiyun](https://fanyi.caiyunapp.com) | [Deepl](https://www.deepl.com/translator) | [Argos](https://translate.argosopentech.com) | [Itranslate](https://itranslate.com/webapp) | [Reverso](https://www.reverso.net/text-translation) | [TranslateCom](https://www.translate.com/machine-translation) | [Papago](https://papago.naver.com) | [Utibet](http://mt.utibet.edu.cn/mt) |
 | ------------- | ---------------------- | -------------------------------------- | -------------------------------------- | --------------------------------------- | -------------------------------- | ---------------------------------------- | ------------------------------- | ---------------------------------- | -------------------------------- | --------------------------------- | ---------------------------------------------------- | ------------------------------------- | ----------------------------------------- | -------------------------------------------- | ------------------------------------------- | --------------------------------------------------- | ------------------------------------------------------------- | ---------------------------------- | ------------------------------------ |
 | Chinese(简体)   | zh-CHS                 | Y(zh-CN)                               | Y(zh)                                  | Y(zh-Hans)                              | Y(zh)                            | Y(zh)                                    | Y(zh)                           | Y                                  | Y                                | Y(zh)                             | Y(zh)                                                | Y(zh)                                 | Y(zh)                                     | Y(zh)                                        | Y(zh-CN)                                    | Y(zh/chi)                                           | ...                                                           | Y(zh-CN)                           | Y(zh)                                |
 | Chinese(繁体)   | zh-CHT                 | Y(zh-TW)                               |                                        | Y(zh-Hant)                              | Y(cht)                           | Y(zh-TW)                                 |                                 |                                    | Y                                | Y(cnt)                            |                                                      |                                       |                                           |                                              | Y(zh-TW)                                    |                                                     |                                                               | Y(zh-TW)                           |                                      |
 | Chinese(文言文)  | wyw                    |                                        |                                        |                                         | Y                                |                                          |                                 |                                    |                                  |                                   |                                                      |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    |                                      |
 | Chinese(粤语)   | yue                    |                                        |                                        | Y                                       | Y                                |                                          |                                 |                                    | Y                                | Y                                 | Y                                                    |                                       |                                           |                                              | Y(zh-HK)                                    |                                                     |                                                               |                                    |                                      |
@@ -218,19 +214,15 @@
 | Chinese(维吾尔语) | uy                     |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  | Y                                 |                                                      |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    |                                      |
 | Chinese(藏语)   | ti                     |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  | Y                                 |                                                      |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    | Y                                    |
 | Chinese(白苗文)  | mww                    |                                        |                                        | Y                                       |                                  |                                          |                                 |                                    | Y                                | Y                                 |                                                      |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    |                                      |
 | Chinese(彝语)   | ii                     |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  |                                   | Y                                                    |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    |                                      |
 | Chinese(苗语)   | hmn                    |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  |                                   |                                                      |                                       |                                           |                                              | Y                                           |                                                     |                                                               |                                    |                                      |
 | Chinese(壮语)   | zyb                    |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  |                                   |                                                      |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    |                                      |
 
-</details>
-</details>
-
-<details>
-<summary>Debug Tips</summary>
+## Debug Tips
 
 ### Linux Runtime Environment
 
 1. To support javascript runtime environment, you should [download and install Node.js](https://nodejs.org/en/download/).
 2. baidu() doesn't work on Linux without desktop.
 
 ### HttpError 4xx
@@ -241,15 +233,10 @@
 4. [Issue me](https://github.com/UlionTse/translators/issues), thanks.
 
 ### NetworkError or ProxyError
 
 1. Check whether the network is connected correctly.
 2. Check the proxy are enabled on your computer. If it is enabled, try turning it off or otherwise. 
 
-</details>
-
-<details>
-<summary>License</summary>
+## License
 
 [GPLv3 License](https://github.com/uliontse/translators/blob/master/LICENSE)
-
-</details>
```

#### html2text {}

```diff
@@ -1,103 +1,106 @@
 [https://github.com/UlionTse/translators/blob/master/docs/translators_logo.png]
   [PyPI_-_Version] [Conda_-_Version] [PyPI_-_License] [PyPI_-_Python] [PyPI_-
-                      Status] [PyPI_-_Wheel] [Downloads]
+                   Status] [PyPI_-_Wheel] [PyPI_-_Downloads]
 * * * **Translators** is a library which aims to bring **free, multiple,
-enjoyable** translation to individuals and students in Python.  Supported
-Translation Services | ID | Translator | Number of Supported Languages |
-Advantage | Service | Status | | --- | ----------------------------------------
------------------------------------------ | ----------------------------- | ---
--------------------------------------------------------------------------------
---------- | -------------------------------------------------------------------
----------------------------------------------- | ------------------------------
-- | | 1 | [Niutrans](https://niutrans.com/trans) | 302 | support the most
-languages in the world | [Northeastern University](http://english.neu.edu.cn/
-) / [Niutrans](https://github.com/NiuTrans), China | / | | 2 | [Alibaba](https:
-//translate.alibaba.com) | 221 | support most languages, support professional
-field | [Alibaba](https://damo.alibaba.com/about?lang=en), China | stable | | 3
+enjoyable** translation to individuals and students in Python. - [Supported
+Translation Services](#supported-translation-services) - [Installation]
+(#installation) - [Getting Started](#getting-started) - [Supported Languages]
+(#supported-languages) - [Debug Tips](#debug-tips) - [License](#license) ##
+Supported Translation Services | ID | Translator | Number of Supported
+Languages | Advantage | Service | Status | | --- | ----------------------------
+----------------------------------------------------- | -----------------------
+------ | ----------------------------------------------------------------------
+--------------------- | -------------------------------------------------------
+---------------------------------------------------------- | ------------------
+------------- | | 1 | [MyMemory](https://mymemory.translated.net) | 330 |
+support the most languages in the world | [Translated](https://
+translatedlabs.com/welcome), Italy | stable | | 2 | [Niutrans](https://
+niutrans.com/trans) | 302 | support the most languages in the world |
+[Northeastern University](http://english.neu.edu.cn/) / [Niutrans](https://
+github.com/NiuTrans), China | / | | 3 | [Alibaba](https://
+translate.alibaba.com) | 221 | support most languages, support professional
+field | [Alibaba](https://damo.alibaba.com/about?lang=en), China | stable | | 4
 | [Baidu](https://fanyi.baidu.com) | 201 | support most languages, support
 professional field, support classical Chinese | [Baidu](https://ir.baidu.com/
-company-overview), China | stable | | 4 | [Iciba](https://www.iciba.com/fy) |
+company-overview), China | stable | | 5 | [Iciba](https://www.iciba.com/fy) |
 187 | support the most languages in the world | [Kingsoft](https://www.wps.com/
-about-us/) / [Xiaomi](https://www.mi.com/us/about/), China | stable | | 5 |
-[MyMemory](https://mymemory.translated.net) | 151 | support the most languages
-in the world, good at Creole English, Creole French | [Translated](https://
-translatedlabs.com/welcome), Italy | stable | | 6 | [Iflytek](https://
-fanyi.xfyun.cn/console/trans/text) | 140 | support the most languages in the
-world | [Iflytek](https://www.iflytek.com/en/about-us.html), China | / | | 7 |
-[Google](https://translate.google.com) | 134 | support more languages in the
-world | [Google](https://about.google/), America | stable(offline in China
-inland) | | 8 | [VolcEngine](https://translate.volcengine.com) | 122 | support
-more languages in the world, support professional field | [ByteDance](https://
-www.bytedance.com/en/), China | / | | 9 | [Lingvanex](https://lingvanex.com/
-demo) | 112 | support translation of different regions but the same language |
-[Lingvanex](https://lingvanex.com/about-us/), Cyprus | stable | | 10 | [Bing]
-(https://www.bing.com/Translator) | 110 | support more languages in the world |
-[Microsoft](https://www.microsoft.com/en-us/about), America | stable | | 11 |
-[Yandex](https://translate.yandex.com) | 102 | support more languages in the
-world, support word to emoji | [Yandex](https://yandex.com/company/), Russia |
-/ | | 12 | [Itranslate](https://itranslate.com/webapp) | 101 | support
-translation of different regions but the same language, such as en-US, en-UK,
-en-AU | [Itranslate](https://itranslate.com/about), Austria | stable | | 13 |
-[Sogou](https://fanyi.sogou.com/text) | 61 | support more languages in the
-world | [Tencent](https://www.tencent.com/en-us/about.html), China | stable | |
-14 | [ModernMt](https://www.modernmt.com/translate) | 56 | open-source, support
-more languages in the world | [Modernmt](https://github.com/modernmt) /
-[Translated](https://translatedlabs.com/welcome), Italy | stable | | 15 |
-[SysTran](https://www.systran.net/translate/) | 52 | support more languages in
-the world | [SysTran](https://www.systran.net/about/), France | stable | | 16 |
-[Apertium](https://www.apertium.org/) | 45 | open-source | [Apertium](https://
-github.com/apertium), Spain | stable | | 17 | [Reverso](https://
-www.reverso.net/text-translation) | 42 | popular on Mac and Iphone | [Reverso]
-(https://www.corporate-translation.reverso.com/about-us), France | stable | |
-18 | [CloudYi](https://www.cloudtranslation.com/#/translate) | 28 | support
-main languages | [Xiamen University](http://nlp.xmu.edu.cn/) /
-[CloudTranslation](https://www.cloudtranslation.com/#/about), China | stable |
-| 19 | [Deepl](https://www.deepl.com/translator) | 27 | high quality to
-translate but response slowly | [Deepl](https://jobs.deepl.com/l/en), Germany |
-stable | | 20 | [QQTranSmart](https://transmart.qq.com) | 22 | support main
-languages | [Tencent](https://www.tencent.com/en-us/about.html), China | stable
-| | 21 | [TranslateCom](https://www.translate.com/machine-translation) | 21 |
-good at English translation | [TranslateCom](https://www.translate.com/about-
-us), America | stable | | 22 | [Tilde](https://translate.tilde.com/) | 21 |
-good at lv, de, fr translation | [Tilde](https://tilde.com/about), Latvia | / |
-| 23 | [QQFanyi](https://fanyi.qq.com) | 17 | support main languages |
-[Tencent](https://www.tencent.com/en-us/about.html), China | stable | | 24 |
-[Argos](https://translate.argosopentech.com) | 17 | open-source | [Argos]
-(https://github.com/argosopentech) / [Libre](https://github.com/
-LibreTranslate), America | stable | | 25 | [TranslateMe](https://
-translateme.network/) | 16 | good at English translation | [TranslateMe](https:
-//translateme.network/our-team/) / [Neosus](https://neosus.net/about/),
-Lithuania | / | | 26 | [Youdao](https://ai.youdao.com/product-fanyi-text.s) |
-15 | support main languages, high quality | [Netease](https://ir.netease.com/
-company-overview/corporate-profile), China | stable | | 27 | [Papago](https://
-papago.naver.com) | 15 | good at Korean translation | [Naver](https://
-www.navercorp.com/en/naver/company), South Korea | stable | | 28 | [Marai]
-(https://miraitranslate.com/trial/) | 15 | good at Japanese translation |
-[MaraiTranslate](https://miraitranslate.com/en/company/), Japan | / | | 29 |
-[Iflyrec](https://fanyi.iflyrec.com) | 12 | good at Chinese translation |
-[Iflytek](https://www.iflytek.com/en/about-us.html), China | stable | | 30 |
-[Yeekit](https://www.yeekit.com/site/translate) | 10 | support main languages |
-[CTC](https://www.ctpc.com.cn/cms/enAboutUs.htm), China | / | | 31 |
-[LanguageWire](https://www.languagewire.com/en/technology/languagewire-
-translate) | 8 | good at English translation | [LanguageWire](https://
-www.languagewire.com/about-us), Denmark | stable | | 32 | [Caiyun](https://
-fanyi.caiyunapp.com) | 7 | high quality to translate but response slowly,
-support professional field | [ColorfulClouds](http://caiyunapp.com/jobs/),
-China | stable | | 33 | [Elia](https://elia.eus/translator) | 6 | good at
-Basque translation | [Elhuyar](https://www.elhuyar.eus/eu/nor-gara), Spain |
+about-us/) / [Xiaomi](https://www.mi.com/us/about/), China | stable | | 6 |
+[Iflytek](https://fanyi.xfyun.cn/console/trans/text) | 140 | support the most
+languages in the world | [Iflytek](https://www.iflytek.com/en/about-us.html),
+China | / | | 7 | [Google](https://translate.google.com) | 134 | support more
+languages in the world | [Google](https://about.google/), America | stable
+(offline in China inland) | | 8 | [VolcEngine](https://
+translate.volcengine.com) | 122 | support more languages in the world, support
+professional field | [ByteDance](https://www.bytedance.com/en/), China | / | |
+9 | [Lingvanex](https://lingvanex.com/demo) | 112 | support translation of
+different regions but the same language | [Lingvanex](https://lingvanex.com/
+about-us/), Cyprus | stable | | 10 | [Bing](https://www.bing.com/Translator) |
+110 | support more languages in the world | [Microsoft](https://
+www.microsoft.com/en-us/about), America | stable | | 11 | [Yandex](https://
+translate.yandex.com) | 102 | support more languages in the world, support word
+to emoji | [Yandex](https://yandex.com/company/), Russia | / | | 12 |
+[Itranslate](https://itranslate.com/webapp) | 101 | support translation of
+different regions but the same language, such as en-US, en-UK, en-AU |
+[Itranslate](https://itranslate.com/about), Austria | stable | | 13 | [Sogou]
+(https://fanyi.sogou.com/text) | 61 | support more languages in the world |
+[Tencent](https://www.tencent.com/en-us/about.html), China | stable | | 14 |
+[ModernMt](https://www.modernmt.com/translate) | 56 | open-source, support more
+languages in the world | [Modernmt](https://github.com/modernmt) / [Translated]
+(https://translatedlabs.com/welcome), Italy | stable | | 15 | [SysTran](https:/
+/www.systran.net/translate/) | 52 | support more languages in the world |
+[SysTran](https://www.systran.net/about/), France | stable | | 16 | [Apertium]
+(https://www.apertium.org/) | 45 | open-source | [Apertium](https://github.com/
+apertium), Spain | stable | | 17 | [Reverso](https://www.reverso.net/text-
+translation) | 42 | popular on Mac and Iphone | [Reverso](https://
+www.corporate-translation.reverso.com/about-us), France | stable | | 18 |
+[CloudYi](https://www.cloudtranslation.com/#/translate) | 28 | support main
+languages | [Xiamen University](http://nlp.xmu.edu.cn/) / [CloudTranslation]
+(https://www.cloudtranslation.com/#/about), China | stable | | 19 | [Deepl]
+(https://www.deepl.com/translator) | 27 | high quality to translate but
+response slowly | [Deepl](https://jobs.deepl.com/l/en), Germany | stable | | 20
+| [QQTranSmart](https://transmart.qq.com) | 22 | support main languages |
+[Tencent](https://www.tencent.com/en-us/about.html), China | stable | | 21 |
+[TranslateCom](https://www.translate.com/machine-translation) | 21 | good at
+English translation | [TranslateCom](https://www.translate.com/about-us),
+America | stable | | 22 | [Tilde](https://translate.tilde.com/) | 21 | good at
+lv, de, fr translation | [Tilde](https://tilde.com/about), Latvia | / | | 23 |
+[QQFanyi](https://fanyi.qq.com) | 17 | support main languages | [Tencent]
+(https://www.tencent.com/en-us/about.html), China | stable | | 24 | [Argos]
+(https://translate.argosopentech.com) | 17 | open-source | [Argos](https://
+github.com/argosopentech) / [Libre](https://github.com/LibreTranslate), America
+| stable | | 25 | [TranslateMe](https://translateme.network/) | 16 | good at
+English translation | [TranslateMe](https://translateme.network/our-team/) /
+[Neosus](https://neosus.net/about/), Lithuania | / | | 26 | [Youdao](https://
+ai.youdao.com/product-fanyi-text.s) | 15 | support main languages, high quality
+| [Netease](https://ir.netease.com/company-overview/corporate-profile), China |
+stable | | 27 | [Papago](https://papago.naver.com) | 15 | good at Korean
+translation | [Naver](https://www.navercorp.com/en/naver/company), South Korea
+| stable | | 28 | [Marai](https://miraitranslate.com/trial/) | 15 | good at
+Japanese translation | [MaraiTranslate](https://miraitranslate.com/en/company/
+), Japan | / | | 29 | [Iflyrec](https://fanyi.iflyrec.com) | 12 | good at
+Chinese translation | [Iflytek](https://www.iflytek.com/en/about-us.html),
+China | stable | | 30 | [Yeekit](https://www.yeekit.com/site/translate) | 10 |
+support main languages | [CTC](https://www.ctpc.com.cn/cms/enAboutUs.htm),
+China | / | | 31 | [LanguageWire](https://www.languagewire.com/en/technology/
+languagewire-translate) | 8 | good at English translation | [LanguageWire]
+(https://www.languagewire.com/about-us), Denmark | stable | | 32 | [Caiyun]
+(https://fanyi.caiyunapp.com) | 7 | high quality to translate but response
+slowly, support professional field | [ColorfulClouds](http://caiyunapp.com/
+jobs/), China | stable | | 33 | [Elia](https://elia.eus/translator) | 6 | good
+at Basque translation | [Elhuyar](https://www.elhuyar.eus/eu/nor-gara), Spain |
 stable | | 34 | [Judic](https://judic.io/en/translate) | 4 | good at European
 translation | [CrossLang](https://crosslang.com/about-us/), Belgium | stable |
 | 35 | [Mglip](http://fy.mglip.com/pc) | 3 | good at Mongolia translation |
 [Inner Mongolia University](https://www.imu.edu.cn/yw/Home.htm), China | stable
 | | 36 | [Utibet](http://mt.utibet.edu.cn/mt) | 2 | good at Tibet translation |
-[Tibet University](http://www.utibet.edu.cn/), China | stable |   Installation
+[Tibet University](http://www.utibet.edu.cn/), China | stable | ## Installation
 ```sh # PYPI pip install --upgrade translators # Conda conda install -c conda-
 forge translators # Source git clone https://github.com/UlionTse/
-translators.git cd translators python setup.py install ```   Getting Started
+translators.git cd translators python setup.py install ``` ## Getting Started
 ```python import translators as ts q_text =
 'å­£å§¬å¯ï¼éé¸¡ï¼é¸¡å³æ£é¸¡ãæ£é¸¡é¥¥å½ï¼å­£å§¬åç®ç¨·æµé¸¡ã'
 q_html = '''
 è¿æå¦ä¸ç¯æç« ãæ½æ°é£ç®å²ãã
 ''' ### usage _ = ts.preaccelerate_and_speedtest() # Optional. Caching sessions
 in advance, which can help improve access speed. print(ts.translators_pool)
 print(ts.translate_text(q_text)) print(ts.translate_html(q_html,
@@ -117,15 +120,15 @@
 default None. Support google(), argos(), yandex() only. :param
 if_check_reset_host_url: bool, default True. Support google(), yandex() only. :
 param if_ignore_empty_query: bool, default False. :param limit_of_length: int,
 default 20000. :param if_ignore_limit_of_length: bool, default False. :param
 if_show_time_stat: bool, default False. :param show_time_stat_precision: int,
 default 2. :param if_print_warning: bool, default True. :param lingvanex_mode:
 str, default 'B2C', choose from ("B2C", "B2B"). :param myMemory_mode: str,
-default "web", choose from ("web", "api"). :return: str or dict """ ```
+default "web", choose from ("web", "api"). :return: str or dict """ ``` ##
 Supported Languages | Language | Language of Translator | [Google](https://
 translate.google.com) | [Yandex](https://translate.yandex.com) | [Bing](https:/
 /www.bing.com/Translator) | [Baidu](https://fanyi.baidu.com) | [Alibaba](https:
 //translate.alibaba.com) | [Tencent](https://fanyi.qq.com) | [Youdao](https://
 fanyi.youdao.com) | [Sogou](https://fanyi.sogou.com) | [Deepl](https://
 www.deepl.com/translator) | [Caiyun](https://fanyi.caiyunapp.com) | [Argos]
 (https://translate.argosopentech.com) | others... | | -------------------- | --
@@ -179,19 +182,19 @@
 | | | | | | | | | | | telugu | te | Y | Y | Y | | | | | | | | | | | punjabi |
 pa | Y | Y | Y | | | | | | | | | | | amharic | am | Y | Y | | | | | | | | | | |
 | azerbaijani | az | Y | Y | | | | | | | | | | | | bashkir | ba | | Y | | | | |
 | | | | | | | belarusian | be | Y | Y | | | | | | | | | | | | cebuano | ceb | Y
 | Y | | | | | | | | | | | | chuvash | cv | | Y | | | | | | | | | | | |
 esperanto | eo | Y | Y | | | | | | | | | | | | basque | eu | Y | Y | | | | | |
 | | | | | | irish | ga | Y | Y | Y | | | | | | | | | | | emoji | emj | | Y | |
-| | | | | | | | | | ... | ... | | | | | | | | | | | | |  About Chinese Language
-| Language | Language of Translator | [Google](https://translate.google.com) |
-[Yandex](https://translate.yandex.com) | [Bing](https://www.bing.com/
-Translator) | [Baidu](https://fanyi.baidu.com) | [Alibaba](https://
-translate.alibaba.com) | [Tencent](https://fanyi.qq.com) | [Youdao](https://
+| | | | | | | | | | ... | ... | | | | | | | | | | | | | ### About Chinese
+Language | Language | Language of Translator | [Google](https://
+translate.google.com) | [Yandex](https://translate.yandex.com) | [Bing](https:/
+/www.bing.com/Translator) | [Baidu](https://fanyi.baidu.com) | [Alibaba](https:
+//translate.alibaba.com) | [Tencent](https://fanyi.qq.com) | [Youdao](https://
 fanyi.youdao.com) | [Sogou](https://fanyi.sogou.com) | [Iciba](https://
 www.iciba.com/fy) | [Iflytek](https://fanyi.xfyun.cn/console/trans/text) |
 [Caiyun](https://fanyi.caiyunapp.com) | [Deepl](https://www.deepl.com/
 translator) | [Argos](https://translate.argosopentech.com) | [Itranslate]
 (https://itranslate.com/webapp) | [Reverso](https://www.reverso.net/text-
 translation) | [TranslateCom](https://www.translate.com/machine-translation) |
 [Papago](https://papago.naver.com) | [Utibet](http://mt.utibet.edu.cn/mt) | | -
@@ -213,19 +216,19 @@
 | | | | Chinese(ç²¤è¯­) | yue | | | Y | Y | | | | Y | Y | Y | | | | Y(zh-HK) |
 | | | | | Chinese(åèè¯­) | mn | N[å¤è] | N[å¤è] | | | | | | | | Y
 [åè] | | | | N[å¤è] | | | | | | Chinese(ç»´å¾å°è¯­) | uy | | | | | | |
 | | Y | | | | | | | | | | | Chinese(èè¯­) | ti | | | | | | | | | Y | | | | |
 | | | | Y | | Chinese(ç½èæ) | mww | | | Y | | | | | Y | Y | | | | | | | |
 | | | Chinese(å½è¯­) | ii | | | | | | | | | | Y | | | | | | | | | | Chinese
 (èè¯­) | hmn | | | | | | | | | | | | | | Y | | | | | | Chinese(å£®è¯­) | zyb
-| | | | | | | | | | | | | | | | | | |    Debug Tips ### Linux Runtime
+| | | | | | | | | | | | | | | | | | | ## Debug Tips ### Linux Runtime
 Environment 1. To support javascript runtime environment, you should [download
 and install Node.js](https://nodejs.org/en/download/). 2. baidu() doesn't work
 on Linux without desktop. ### HttpError 4xx 1. Check whether you made high
 frequency requests, especially httperror 429. 2. Check whether this service is
 provided in your region. 3. Detail to solve [HttpError](https://
 developer.mozilla.org/en-US/docs/Web/HTTP/Status) itself. 4. [Issue me](https:/
 /github.com/UlionTse/translators/issues), thanks. ### NetworkError or
 ProxyError 1. Check whether the network is connected correctly. 2. Check the
 proxy are enabled on your computer. If it is enabled, try turning it off or
-otherwise.   License [GPLv3 License](https://github.com/uliontse/translators/
+otherwise. ## License [GPLv3 License](https://github.com/uliontse/translators/
 blob/master/LICENSE)
```

### Comparing `translators-5.7.7/README_history.md` & `translators-5.7.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 <p align="center">
   <img src="https://github.com/UlionTse/translators/blob/master/docs/translators_logo.png" width="500"/>
 </p>
 <p align="center">
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/translators.svg"></a>
-  <a href="https://anaconda.org/conda-forge/translators"><img alt="Conda - Version" src="https://img.shields.io/conda/vn/conda-forge/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Python" src="https://img.shields.io/pypi/pyversions/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Status" src="https://img.shields.io/pypi/status/translators.svg"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/translators.svg?color=blue"></a>
+  <a href="https://anaconda.org/conda-forge/translators"><img alt="Conda - Version" src="https://img.shields.io/conda/vn/conda-forge/translators.svg?color=blue"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/translators.svg?color=brightgreen"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Python" src="https://img.shields.io/pypi/pyversions/translators.svg?color=blue"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Status" src="https://img.shields.io/pypi/status/translators.svg?color=brightgreen"></a>
   <a href="https://pypi.org/project/translators"><img alt="PyPI - Wheel" src="https://img.shields.io/badge/wheel-yes-brightgreen.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="Downloads" src="https://pepy.tech/badge/translators"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Downloads" src="https://static.pepy.tech/personalized-badge/translators?left_text=downloads&left_color=gray&right_color=blue"></a>
 </p>
 
 * * *
 
 **Translators** is a library which aims to bring **free, multiple, enjoyable** translation to individuals and students in Python. 
 
-- [Supported Translation Services](#supported-translation-services)
-- [Installation](#installation)
-- [Getting Started](#getting-started)
-- [Supported Languages](#supported-languages)
-- [Debug Tips](#debug-tips)
-- [License](#license)
-
-## Supported Translation Services
+<details>
+<summary>Supported Translation Services</summary>
 
 | ID  | Translator                                                                        | Number of Supported Languages | Advantage                                                                                   | Service                                                                                                           | Status                          |
 | --- | --------------------------------------------------------------------------------- | ----------------------------- | ------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ------------------------------- |
-| 1   | [Niutrans](https://niutrans.com/trans)                                            | 302                           | support the most languages in the world                                                     | [Northeastern University](http://english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China            | /                               |
-| 2   | [Alibaba](https://translate.alibaba.com)                                          | 221                           | support most languages, support professional field                                          | [Alibaba](https://damo.alibaba.com/about?lang=en), China                                                          | stable                          |
-| 3   | [Baidu](https://fanyi.baidu.com)                                                  | 201                           | support most languages, support professional field, support classical Chinese               | [Baidu](https://ir.baidu.com/company-overview), China                                                             | stable                          |
-| 4   | [Iciba](https://www.iciba.com/fy)                                                 | 187                           | support the most languages in the world                                                     | [Kingsoft](https://www.wps.com/about-us/) / [Xiaomi](https://www.mi.com/us/about/), China                         | stable                          |
-| 5   | [MyMemory](https://mymemory.translated.net)                                       | 151                           | support the most languages in the world, good at Creole English, Creole French              | [Translated](https://translatedlabs.com/welcome), Italy                                                           | stable                          |
+| 1   | [MyMemory](https://mymemory.translated.net)                                       | 330                           | support the most languages in the world                                                     | [Translated](https://translatedlabs.com/welcome), Italy                                                           | stable                          |
+| 2   | [Niutrans](https://niutrans.com/trans)                                            | 302                           | support the most languages in the world                                                     | [Northeastern University](http://english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China            | /                               |
+| 3   | [Alibaba](https://translate.alibaba.com)                                          | 221                           | support most languages, support professional field                                          | [Alibaba](https://damo.alibaba.com/about?lang=en), China                                                          | stable                          |
+| 4   | [Baidu](https://fanyi.baidu.com)                                                  | 201                           | support most languages, support professional field, support classical Chinese               | [Baidu](https://ir.baidu.com/company-overview), China                                                             | stable                          |
+| 5   | [Iciba](https://www.iciba.com/fy)                                                 | 187                           | support the most languages in the world                                                     | [Kingsoft](https://www.wps.com/about-us/) / [Xiaomi](https://www.mi.com/us/about/), China                         | stable                          |
 | 6   | [Iflytek](https://fanyi.xfyun.cn/console/trans/text)                              | 140                           | support the most languages in the world                                                     | [Iflytek](https://www.iflytek.com/en/about-us.html), China                                                        | /                               |
 | 7   | [Google](https://translate.google.com)                                            | 134                           | support more languages in the world                                                         | [Google](https://about.google/), America                                                                          | stable(offline in China inland) |
 | 8   | [VolcEngine](https://translate.volcengine.com)                                    | 122                           | support more languages in the world, support professional field                             | [ByteDance](https://www.bytedance.com/en/), China                                                                 | /                               |
 | 9   | [Lingvanex](https://lingvanex.com/demo)                                           | 112                           | support translation of different regions but the same language                              | [Lingvanex](https://lingvanex.com/about-us/), Cyprus                                                              | stable                          |
 | 10  | [Bing](https://www.bing.com/Translator)                                           | 110                           | support more languages in the world                                                         | [Microsoft](https://www.microsoft.com/en-us/about), America                                                       | stable                          |
 | 11  | [Yandex](https://translate.yandex.com)                                            | 102                           | support more languages in the world, support word to emoji                                  | [Yandex](https://yandex.com/company/), Russia                                                                     | /                               |
 | 12  | [Itranslate](https://itranslate.com/webapp)                                       | 101                           | support translation of different regions but the same language, such as en-US, en-UK, en-AU | [Itranslate](https://itranslate.com/about), Austria                                                               | stable                          |
@@ -59,30 +53,36 @@
 | 31  | [LanguageWire](https://www.languagewire.com/en/technology/languagewire-translate) | 8                             | good at English translation                                                                 | [LanguageWire](https://www.languagewire.com/about-us), Denmark                                                    | stable                          |
 | 32  | [Caiyun](https://fanyi.caiyunapp.com)                                             | 7                             | high quality to translate but response slowly, support professional field                   | [ColorfulClouds](http://caiyunapp.com/jobs/), China                                                               | stable                          |
 | 33  | [Elia](https://elia.eus/translator)                                               | 6                             | good at Basque translation                                                                  | [Elhuyar](https://www.elhuyar.eus/eu/nor-gara), Spain                                                             | stable                          |
 | 34  | [Judic](https://judic.io/en/translate)                                            | 4                             | good at European translation                                                                | [CrossLang](https://crosslang.com/about-us/), Belgium                                                             | stable                          |
 | 35  | [Mglip](http://fy.mglip.com/pc)                                                   | 3                             | good at Mongolia translation                                                                | [Inner Mongolia University](https://www.imu.edu.cn/yw/Home.htm), China                                            | stable                          |
 | 36  | [Utibet](http://mt.utibet.edu.cn/mt)                                              | 2                             | good at Tibet translation                                                                   | [Tibet University](http://www.utibet.edu.cn/), China                                                              | stable                          |
 
-## Installation
+</details>
+
+<details>
+<summary>Installation</summary>
 
 ```sh
 # PYPI
 pip install --upgrade translators
 
 # Conda
 conda install -c conda-forge translators
 
 # Source
 git clone https://github.com/UlionTse/translators.git
 cd translators
 python setup.py install
 ```
 
-## Getting Started
+</details>
+
+<details>
+<summary>Getting Started</summary>
 
 ```python
 import translators as ts
 
 q_text = '季姬寂，集鸡，鸡即棘鸡。棘鸡饥叽，季姬及箕稷济鸡。'
 q_html = '''<!DOCTYPE html><html><head><title>《季姬击鸡记》</title></head><body><p>还有另一篇文章《施氏食狮史》。</p></body></html>'''
 
@@ -122,15 +122,18 @@
             :param if_print_warning: bool, default True.
             :param lingvanex_mode: str, default 'B2C', choose from ("B2C", "B2B").
             :param myMemory_mode: str, default "web", choose from ("web", "api").
     :return: str or dict
 """
 ```
 
-## Supported Languages
+</details>
+
+<details>
+<summary>Supported Languages</summary>
 
 | Language             | Language of Translator | [Google](https://translate.google.com) | [Yandex](https://translate.yandex.com) | [Bing](https://www.bing.com/Translator) | [Baidu](https://fanyi.baidu.com) | [Alibaba](https://translate.alibaba.com) | [Tencent](https://fanyi.qq.com) | [Youdao](https://fanyi.youdao.com) | [Sogou](https://fanyi.sogou.com) | [Deepl](https://www.deepl.com/translator) | [Caiyun](https://fanyi.caiyunapp.com) | [Argos](https://translate.argosopentech.com) | others... |
 | -------------------- | ---------------------- | -------------------------------------- | -------------------------------------- | --------------------------------------- | -------------------------------- | ---------------------------------------- | ------------------------------- | ---------------------------------- | -------------------------------- | ----------------------------------------- | ------------------------------------- | -------------------------------------------- | --------- |
 | english              | en                     | Y                                      | Y                                      | Y                                       | Y                                | Y                                        | Y                               | Y                                  | Y                                | Y                                         | Y                                     | Y                                            | ...       |
 | chinese              | zh                     | Y                                      | Y                                      | Y                                       | Y                                | Y                                        | Y                               | Y                                  | Y                                | Y                                         | Y                                     | Y                                            |           |
 | arabic               | ar                     | Y                                      | Y                                      | Y                                       | Y(ara)                           | Y                                        | Y                               | Y                                  | Y                                |                                           |                                       | Y                                            |           |
 | russian              | ru                     | Y                                      | Y                                      | Y                                       | Y                                | Y                                        | Y                               | Y                                  | Y                                | Y                                         | Y                                     | Y                                            |           |
@@ -198,15 +201,16 @@
 | chuvash              | cv                     |                                        | Y                                      |                                         |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 | esperanto            | eo                     | Y                                      | Y                                      |                                         |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 | basque               | eu                     | Y                                      | Y                                      |                                         |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 | irish                | ga                     | Y                                      | Y                                      | Y                                       |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 | emoji                | emj                    |                                        | Y                                      |                                         |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 | ...                  | ...                    |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  |                                           |                                       |                                              |           |
 
-### About Chinese Language
+<details>
+<summary>About Chinese Language</summary>
 
 | Language      | Language of Translator | [Google](https://translate.google.com) | [Yandex](https://translate.yandex.com) | [Bing](https://www.bing.com/Translator) | [Baidu](https://fanyi.baidu.com) | [Alibaba](https://translate.alibaba.com) | [Tencent](https://fanyi.qq.com) | [Youdao](https://fanyi.youdao.com) | [Sogou](https://fanyi.sogou.com) | [Iciba](https://www.iciba.com/fy) | [Iflytek](https://fanyi.xfyun.cn/console/trans/text) | [Caiyun](https://fanyi.caiyunapp.com) | [Deepl](https://www.deepl.com/translator) | [Argos](https://translate.argosopentech.com) | [Itranslate](https://itranslate.com/webapp) | [Reverso](https://www.reverso.net/text-translation) | [TranslateCom](https://www.translate.com/machine-translation) | [Papago](https://papago.naver.com) | [Utibet](http://mt.utibet.edu.cn/mt) |
 | ------------- | ---------------------- | -------------------------------------- | -------------------------------------- | --------------------------------------- | -------------------------------- | ---------------------------------------- | ------------------------------- | ---------------------------------- | -------------------------------- | --------------------------------- | ---------------------------------------------------- | ------------------------------------- | ----------------------------------------- | -------------------------------------------- | ------------------------------------------- | --------------------------------------------------- | ------------------------------------------------------------- | ---------------------------------- | ------------------------------------ |
 | Chinese(简体)   | zh-CHS                 | Y(zh-CN)                               | Y(zh)                                  | Y(zh-Hans)                              | Y(zh)                            | Y(zh)                                    | Y(zh)                           | Y                                  | Y                                | Y(zh)                             | Y(zh)                                                | Y(zh)                                 | Y(zh)                                     | Y(zh)                                        | Y(zh-CN)                                    | Y(zh/chi)                                           | ...                                                           | Y(zh-CN)                           | Y(zh)                                |
 | Chinese(繁体)   | zh-CHT                 | Y(zh-TW)                               |                                        | Y(zh-Hant)                              | Y(cht)                           | Y(zh-TW)                                 |                                 |                                    | Y                                | Y(cnt)                            |                                                      |                                       |                                           |                                              | Y(zh-TW)                                    |                                                     |                                                               | Y(zh-TW)                           |                                      |
 | Chinese(文言文)  | wyw                    |                                        |                                        |                                         | Y                                |                                          |                                 |                                    |                                  |                                   |                                                      |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    |                                      |
 | Chinese(粤语)   | yue                    |                                        |                                        | Y                                       | Y                                |                                          |                                 |                                    | Y                                | Y                                 | Y                                                    |                                       |                                           |                                              | Y(zh-HK)                                    |                                                     |                                                               |                                    |                                      |
@@ -214,15 +218,19 @@
 | Chinese(维吾尔语) | uy                     |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  | Y                                 |                                                      |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    |                                      |
 | Chinese(藏语)   | ti                     |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  | Y                                 |                                                      |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    | Y                                    |
 | Chinese(白苗文)  | mww                    |                                        |                                        | Y                                       |                                  |                                          |                                 |                                    | Y                                | Y                                 |                                                      |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    |                                      |
 | Chinese(彝语)   | ii                     |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  |                                   | Y                                                    |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    |                                      |
 | Chinese(苗语)   | hmn                    |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  |                                   |                                                      |                                       |                                           |                                              | Y                                           |                                                     |                                                               |                                    |                                      |
 | Chinese(壮语)   | zyb                    |                                        |                                        |                                         |                                  |                                          |                                 |                                    |                                  |                                   |                                                      |                                       |                                           |                                              |                                             |                                                     |                                                               |                                    |                                      |
 
-## Debug Tips
+</details>
+</details>
+
+<details>
+<summary>Debug Tips</summary>
 
 ### Linux Runtime Environment
 
 1. To support javascript runtime environment, you should [download and install Node.js](https://nodejs.org/en/download/).
 2. baidu() doesn't work on Linux without desktop.
 
 ### HttpError 4xx
@@ -233,10 +241,15 @@
 4. [Issue me](https://github.com/UlionTse/translators/issues), thanks.
 
 ### NetworkError or ProxyError
 
 1. Check whether the network is connected correctly.
 2. Check the proxy are enabled on your computer. If it is enabled, try turning it off or otherwise. 
 
-## License
+</details>
+
+<details>
+<summary>License</summary>
 
 [GPLv3 License](https://github.com/uliontse/translators/blob/master/LICENSE)
+
+</details>
```

#### html2text {}

```diff
@@ -1,39 +1,35 @@
 [https://github.com/UlionTse/translators/blob/master/docs/translators_logo.png]
   [PyPI_-_Version] [Conda_-_Version] [PyPI_-_License] [PyPI_-_Python] [PyPI_-
-                      Status] [PyPI_-_Wheel] [Downloads]
+                   Status] [PyPI_-_Wheel] [PyPI_-_Downloads]
 * * * **Translators** is a library which aims to bring **free, multiple,
-enjoyable** translation to individuals and students in Python. - [Supported
-Translation Services](#supported-translation-services) - [Installation]
-(#installation) - [Getting Started](#getting-started) - [Supported Languages]
-(#supported-languages) - [Debug Tips](#debug-tips) - [License](#license) ##
-Supported Translation Services | ID | Translator | Number of Supported
-Languages | Advantage | Service | Status | | --- | ----------------------------
------------------------------------------------------ | -----------------------
------- | ----------------------------------------------------------------------
---------------------- | -------------------------------------------------------
----------------------------------------------------------- | ------------------
-------------- | | 1 | [Niutrans](https://niutrans.com/trans) | 302 | support
+enjoyable** translation to individuals and students in Python.  Supported
+Translation Services | ID | Translator | Number of Supported Languages |
+Advantage | Service | Status | | --- | ----------------------------------------
+----------------------------------------- | ----------------------------- | ---
+-------------------------------------------------------------------------------
+--------- | -------------------------------------------------------------------
+---------------------------------------------- | ------------------------------
+- | | 1 | [MyMemory](https://mymemory.translated.net) | 330 | support the most
+languages in the world | [Translated](https://translatedlabs.com/welcome),
+Italy | stable | | 2 | [Niutrans](https://niutrans.com/trans) | 302 | support
 the most languages in the world | [Northeastern University](http://
-english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China | / | | 2
+english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China | / | | 3
 | [Alibaba](https://translate.alibaba.com) | 221 | support most languages,
 support professional field | [Alibaba](https://damo.alibaba.com/about?lang=en),
-China | stable | | 3 | [Baidu](https://fanyi.baidu.com) | 201 | support most
+China | stable | | 4 | [Baidu](https://fanyi.baidu.com) | 201 | support most
 languages, support professional field, support classical Chinese | [Baidu]
-(https://ir.baidu.com/company-overview), China | stable | | 4 | [Iciba](https:/
+(https://ir.baidu.com/company-overview), China | stable | | 5 | [Iciba](https:/
 /www.iciba.com/fy) | 187 | support the most languages in the world | [Kingsoft]
 (https://www.wps.com/about-us/) / [Xiaomi](https://www.mi.com/us/about/), China
-| stable | | 5 | [MyMemory](https://mymemory.translated.net) | 151 | support
-the most languages in the world, good at Creole English, Creole French |
-[Translated](https://translatedlabs.com/welcome), Italy | stable | | 6 |
-[Iflytek](https://fanyi.xfyun.cn/console/trans/text) | 140 | support the most
-languages in the world | [Iflytek](https://www.iflytek.com/en/about-us.html),
-China | / | | 7 | [Google](https://translate.google.com) | 134 | support more
-languages in the world | [Google](https://about.google/), America | stable
-(offline in China inland) | | 8 | [VolcEngine](https://
+| stable | | 6 | [Iflytek](https://fanyi.xfyun.cn/console/trans/text) | 140 |
+support the most languages in the world | [Iflytek](https://www.iflytek.com/en/
+about-us.html), China | / | | 7 | [Google](https://translate.google.com) | 134
+| support more languages in the world | [Google](https://about.google/),
+America | stable(offline in China inland) | | 8 | [VolcEngine](https://
 translate.volcengine.com) | 122 | support more languages in the world, support
 professional field | [ByteDance](https://www.bytedance.com/en/), China | / | |
 9 | [Lingvanex](https://lingvanex.com/demo) | 112 | support translation of
 different regions but the same language | [Lingvanex](https://lingvanex.com/
 about-us/), Cyprus | stable | | 10 | [Bing](https://www.bing.com/Translator) |
 110 | support more languages in the world | [Microsoft](https://
 www.microsoft.com/en-us/about), America | stable | | 11 | [Yandex](https://
@@ -89,18 +85,18 @@
 jobs/), China | stable | | 33 | [Elia](https://elia.eus/translator) | 6 | good
 at Basque translation | [Elhuyar](https://www.elhuyar.eus/eu/nor-gara), Spain |
 stable | | 34 | [Judic](https://judic.io/en/translate) | 4 | good at European
 translation | [CrossLang](https://crosslang.com/about-us/), Belgium | stable |
 | 35 | [Mglip](http://fy.mglip.com/pc) | 3 | good at Mongolia translation |
 [Inner Mongolia University](https://www.imu.edu.cn/yw/Home.htm), China | stable
 | | 36 | [Utibet](http://mt.utibet.edu.cn/mt) | 2 | good at Tibet translation |
-[Tibet University](http://www.utibet.edu.cn/), China | stable | ## Installation
+[Tibet University](http://www.utibet.edu.cn/), China | stable |   Installation
 ```sh # PYPI pip install --upgrade translators # Conda conda install -c conda-
 forge translators # Source git clone https://github.com/UlionTse/
-translators.git cd translators python setup.py install ``` ## Getting Started
+translators.git cd translators python setup.py install ```   Getting Started
 ```python import translators as ts q_text =
 'å­£å§¬å¯ï¼éé¸¡ï¼é¸¡å³æ£é¸¡ãæ£é¸¡é¥¥å½ï¼å­£å§¬åç®ç¨·æµé¸¡ã'
 q_html = '''
 è¿æå¦ä¸ç¯æç« ãæ½æ°é£ç®å²ãã
 ''' ### usage _ = ts.preaccelerate_and_speedtest() # Optional. Caching sessions
 in advance, which can help improve access speed. print(ts.translators_pool)
 print(ts.translate_text(q_text)) print(ts.translate_html(q_html,
@@ -120,15 +116,15 @@
 default None. Support google(), argos(), yandex() only. :param
 if_check_reset_host_url: bool, default True. Support google(), yandex() only. :
 param if_ignore_empty_query: bool, default False. :param limit_of_length: int,
 default 20000. :param if_ignore_limit_of_length: bool, default False. :param
 if_show_time_stat: bool, default False. :param show_time_stat_precision: int,
 default 2. :param if_print_warning: bool, default True. :param lingvanex_mode:
 str, default 'B2C', choose from ("B2C", "B2B"). :param myMemory_mode: str,
-default "web", choose from ("web", "api"). :return: str or dict """ ``` ##
+default "web", choose from ("web", "api"). :return: str or dict """ ```
 Supported Languages | Language | Language of Translator | [Google](https://
 translate.google.com) | [Yandex](https://translate.yandex.com) | [Bing](https:/
 /www.bing.com/Translator) | [Baidu](https://fanyi.baidu.com) | [Alibaba](https:
 //translate.alibaba.com) | [Tencent](https://fanyi.qq.com) | [Youdao](https://
 fanyi.youdao.com) | [Sogou](https://fanyi.sogou.com) | [Deepl](https://
 www.deepl.com/translator) | [Caiyun](https://fanyi.caiyunapp.com) | [Argos]
 (https://translate.argosopentech.com) | others... | | -------------------- | --
@@ -182,19 +178,19 @@
 | | | | | | | | | | | telugu | te | Y | Y | Y | | | | | | | | | | | punjabi |
 pa | Y | Y | Y | | | | | | | | | | | amharic | am | Y | Y | | | | | | | | | | |
 | azerbaijani | az | Y | Y | | | | | | | | | | | | bashkir | ba | | Y | | | | |
 | | | | | | | belarusian | be | Y | Y | | | | | | | | | | | | cebuano | ceb | Y
 | Y | | | | | | | | | | | | chuvash | cv | | Y | | | | | | | | | | | |
 esperanto | eo | Y | Y | | | | | | | | | | | | basque | eu | Y | Y | | | | | |
 | | | | | | irish | ga | Y | Y | Y | | | | | | | | | | | emoji | emj | | Y | |
-| | | | | | | | | | ... | ... | | | | | | | | | | | | | ### About Chinese
-Language | Language | Language of Translator | [Google](https://
-translate.google.com) | [Yandex](https://translate.yandex.com) | [Bing](https:/
-/www.bing.com/Translator) | [Baidu](https://fanyi.baidu.com) | [Alibaba](https:
-//translate.alibaba.com) | [Tencent](https://fanyi.qq.com) | [Youdao](https://
+| | | | | | | | | | ... | ... | | | | | | | | | | | | |  About Chinese Language
+| Language | Language of Translator | [Google](https://translate.google.com) |
+[Yandex](https://translate.yandex.com) | [Bing](https://www.bing.com/
+Translator) | [Baidu](https://fanyi.baidu.com) | [Alibaba](https://
+translate.alibaba.com) | [Tencent](https://fanyi.qq.com) | [Youdao](https://
 fanyi.youdao.com) | [Sogou](https://fanyi.sogou.com) | [Iciba](https://
 www.iciba.com/fy) | [Iflytek](https://fanyi.xfyun.cn/console/trans/text) |
 [Caiyun](https://fanyi.caiyunapp.com) | [Deepl](https://www.deepl.com/
 translator) | [Argos](https://translate.argosopentech.com) | [Itranslate]
 (https://itranslate.com/webapp) | [Reverso](https://www.reverso.net/text-
 translation) | [TranslateCom](https://www.translate.com/machine-translation) |
 [Papago](https://papago.naver.com) | [Utibet](http://mt.utibet.edu.cn/mt) | | -
@@ -216,19 +212,19 @@
 | | | | Chinese(ç²¤è¯­) | yue | | | Y | Y | | | | Y | Y | Y | | | | Y(zh-HK) |
 | | | | | Chinese(åèè¯­) | mn | N[å¤è] | N[å¤è] | | | | | | | | Y
 [åè] | | | | N[å¤è] | | | | | | Chinese(ç»´å¾å°è¯­) | uy | | | | | | |
 | | Y | | | | | | | | | | | Chinese(èè¯­) | ti | | | | | | | | | Y | | | | |
 | | | | Y | | Chinese(ç½èæ) | mww | | | Y | | | | | Y | Y | | | | | | | |
 | | | Chinese(å½è¯­) | ii | | | | | | | | | | Y | | | | | | | | | | Chinese
 (èè¯­) | hmn | | | | | | | | | | | | | | Y | | | | | | Chinese(å£®è¯­) | zyb
-| | | | | | | | | | | | | | | | | | | ## Debug Tips ### Linux Runtime
+| | | | | | | | | | | | | | | | | | |    Debug Tips ### Linux Runtime
 Environment 1. To support javascript runtime environment, you should [download
 and install Node.js](https://nodejs.org/en/download/). 2. baidu() doesn't work
 on Linux without desktop. ### HttpError 4xx 1. Check whether you made high
 frequency requests, especially httperror 429. 2. Check whether this service is
 provided in your region. 3. Detail to solve [HttpError](https://
 developer.mozilla.org/en-US/docs/Web/HTTP/Status) itself. 4. [Issue me](https:/
 /github.com/UlionTse/translators/issues), thanks. ### NetworkError or
 ProxyError 1. Check whether the network is connected correctly. 2. Check the
 proxy are enabled on your computer. If it is enabled, try turning it off or
-otherwise. ## License [GPLv3 License](https://github.com/uliontse/translators/
+otherwise.   License [GPLv3 License](https://github.com/uliontse/translators/
 blob/master/LICENSE)
```

### Comparing `translators-5.7.7/change_log.txt` & `translators-5.7.8/change_log.txt`

 * *Files 2% similar despite different names*

```diff
@@ -395,7 +395,11 @@
 
 5.7.7
 update license.
 update email.
 stronger parameter type.
 stronger sysTran().
 check translateMe(), server is bad now.
+
+5.7.8
+stronger myMemory() and add languages.  #132
+update readme.md
```

### Comparing `translators-5.7.7/setup.py` & `translators-5.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `translators-5.7.7/translators/server.py` & `translators-5.7.8/translators/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -12244,4957 +12244,5005 @@
 0002fd30: 6f72 792e 7472 616e 736c 6174 6564 2e6e  ory.translated.n
 0002fd40: 6574 2f61 7069 2f61 6a61 7866 6574 6368  et/api/ajaxfetch
 0002fd50: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
 0002fd60: 6170 695f 6170 695f 7572 6c20 3d20 2768  api_api_url = 'h
 0002fd70: 7474 7073 3a2f 2f61 7069 2e6d 796d 656d  ttps://api.mymem
 0002fd80: 6f72 792e 7472 616e 736c 6174 6564 2e6e  ory.translated.n
 0002fd90: 6574 2f67 6574 270d 0a20 2020 2020 2020  et/get'..       
-0002fda0: 2073 656c 662e 686f 7374 5f68 6561 6465   self.host_heade
-0002fdb0: 7273 203d 2073 656c 662e 6765 745f 6865  rs = self.get_he
-0002fdc0: 6164 6572 7328 7365 6c66 2e68 6f73 745f  aders(self.host_
-0002fdd0: 7572 6c2c 2069 665f 6170 693d 4661 6c73  url, if_api=Fals
-0002fde0: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
-0002fdf0: 2e73 6573 7369 6f6e 203d 204e 6f6e 650d  .session = None.
-0002fe00: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-0002fe10: 6e67 7561 6765 5f6d 6170 203d 204e 6f6e  nguage_map = Non
-0002fe20: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-0002fe30: 7175 6572 795f 636f 756e 7420 3d20 300d  query_count = 0.
-0002fe40: 0a20 2020 2020 2020 2073 656c 662e 6f75  .        self.ou
-0002fe50: 7470 7574 5f7a 6820 3d20 277a 682d 434e  tput_zh = 'zh-CN
-0002fe60: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
-0002fe70: 696e 7075 745f 6c69 6d69 7420 3d20 696e  input_limit = in
-0002fe80: 7428 3565 3229 0d0a 2020 2020 2020 2020  t(5e2)..        
-0002fe90: 7365 6c66 2e64 6566 6175 6c74 5f66 726f  self.default_fro
-0002fea0: 6d5f 6c61 6e67 7561 6765 203d 2073 656c  m_language = sel
-0002feb0: 662e 6f75 7470 7574 5f7a 680d 0a0d 0a20  f.output_zh.... 
-0002fec0: 2020 2040 5473 652e 6465 6275 675f 6c61     @Tse.debug_la
-0002fed0: 6e67 7561 6765 5f6d 6170 0d0a 2020 2020  nguage_map..    
-0002fee0: 6465 6620 6765 745f 6c61 6e67 7561 6765  def get_language
-0002fef0: 5f6d 6170 2873 656c 662c 2068 6f73 745f  _map(self, host_
-0002ff00: 6874 6d6c 3a20 7374 722c 202a 2a6b 7761  html: str, **kwa
-0002ff10: 7267 733a 204c 616e 674d 6170 4b77 6172  rgs: LangMapKwar
-0002ff20: 6773 5479 7065 2920 2d3e 2064 6963 743a  gsType) -> dict:
-0002ff30: 0d0a 2020 2020 2020 2020 6574 203d 206c  ..        et = l
-0002ff40: 786d 6c2e 6574 7265 652e 4854 4d4c 2868  xml.etree.HTML(h
-0002ff50: 6f73 745f 6874 6d6c 290d 0a20 2020 2020  ost_html)..     
-0002ff60: 2020 206c 616e 675f 6c69 7374 203d 2065     lang_list = e
-0002ff70: 742e 7870 6174 6828 272f 2f2a 5b40 6964  t.xpath('//*[@id
-0002ff80: 3d22 7365 6c65 6374 5f73 6f75 7263 655f  ="select_source_
-0002ff90: 6d6d 225d 2f6f 7074 696f 6e2f 4076 616c  mm"]/option/@val
-0002ffa0: 7565 2729 5b32 3a5d 0d0a 2020 2020 2020  ue')[2:]..      
-0002ffb0: 2020 6c61 6e67 5f6c 6973 7420 3d20 736f    lang_list = so
-0002ffc0: 7274 6564 286c 6973 7428 7365 7428 6c61  rted(list(set(la
-0002ffd0: 6e67 5f6c 6973 7429 2929 0d0a 2020 2020  ng_list)))..    
-0002ffe0: 2020 2020 7265 7475 726e 207b 7d2e 6672      return {}.fr
-0002fff0: 6f6d 6b65 7973 286c 616e 675f 6c69 7374  omkeys(lang_list
-00030000: 2c20 6c61 6e67 5f6c 6973 7429 0d0a 0d0a  , lang_list)....
-00030010: 2020 2020 4054 7365 2e74 696d 655f 7374      @Tse.time_st
-00030020: 6174 0d0a 2020 2020 4054 7365 2e63 6865  at..    @Tse.che
-00030030: 636b 5f71 7565 7279 0d0a 2020 2020 6465  ck_query..    de
-00030040: 6620 6d79 4d65 6d6f 7279 5f61 7069 2873  f myMemory_api(s
-00030050: 656c 662c 2071 7565 7279 5f74 6578 743a  elf, query_text:
-00030060: 2073 7472 2c20 6672 6f6d 5f6c 616e 6775   str, from_langu
-00030070: 6167 653a 2073 7472 203d 2027 6175 746f  age: str = 'auto
-00030080: 272c 2074 6f5f 6c61 6e67 7561 6765 3a20  ', to_language: 
-00030090: 7374 7220 3d20 2765 6e27 2c20 2a2a 6b77  str = 'en', **kw
-000300a0: 6172 6773 3a20 4170 694b 7761 7267 7354  args: ApiKwargsT
-000300b0: 7970 6529 202d 3e20 556e 696f 6e5b 7374  ype) -> Union[st
-000300c0: 722c 2064 6963 745d 3a0d 0a20 2020 2020  r, dict]:..     
-000300d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000300e0: 6874 7470 733a 2f2f 6d79 6d65 6d6f 7279  https://mymemory
-000300f0: 2e74 7261 6e73 6c61 7465 642e 6e65 740d  .translated.net.
-00030100: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00030110: 7175 6572 795f 7465 7874 3a20 7374 722c  query_text: str,
-00030120: 206d 7573 742e 0d0a 2020 2020 2020 2020   must...        
-00030130: 3a70 6172 616d 2066 726f 6d5f 6c61 6e67  :param from_lang
-00030140: 7561 6765 3a20 7374 722c 2064 6566 6175  uage: str, defau
-00030150: 6c74 2027 6175 746f 272e 0d0a 2020 2020  lt 'auto'...    
-00030160: 2020 2020 3a70 6172 616d 2074 6f5f 6c61      :param to_la
-00030170: 6e67 7561 6765 3a20 7374 722c 2064 6566  nguage: str, def
-00030180: 6175 6c74 2027 656e 272e 0d0a 2020 2020  ault 'en'...    
-00030190: 2020 2020 3a70 6172 616d 202a 2a6b 7761      :param **kwa
-000301a0: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-000301b0: 2020 2020 2020 3a70 6172 616d 2074 696d        :param tim
-000301c0: 656f 7574 3a20 666c 6f61 742c 2064 6566  eout: float, def
-000301d0: 6175 6c74 204e 6f6e 652e 0d0a 2020 2020  ault None...    
-000301e0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-000301f0: 616d 2070 726f 7869 6573 3a20 6469 6374  am proxies: dict
-00030200: 2c20 6465 6661 756c 7420 4e6f 6e65 2e0d  , default None..
-00030210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00030220: 203a 7061 7261 6d20 736c 6565 705f 7365   :param sleep_se
-00030230: 636f 6e64 733a 2066 6c6f 6174 2c20 6465  conds: float, de
-00030240: 6661 756c 7420 302e 0d0a 2020 2020 2020  fault 0...      
-00030250: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00030260: 2069 735f 6465 7461 696c 5f72 6573 756c   is_detail_resul
-00030270: 743a 2062 6f6f 6c2c 2064 6566 6175 6c74  t: bool, default
-00030280: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
-00030290: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-000302a0: 6966 5f69 676e 6f72 655f 6c69 6d69 745f  if_ignore_limit_
-000302b0: 6f66 5f6c 656e 6774 683a 2062 6f6f 6c2c  of_length: bool,
-000302c0: 2064 6566 6175 6c74 2046 616c 7365 2e0d   default False..
-000302d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000302e0: 203a 7061 7261 6d20 6c69 6d69 745f 6f66   :param limit_of
-000302f0: 5f6c 656e 6774 683a 2069 6e74 2c20 6465  _length: int, de
-00030300: 6661 756c 7420 3230 3030 302e 0d0a 2020  fault 20000...  
-00030310: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-00030320: 6172 616d 2069 665f 6967 6e6f 7265 5f65  aram if_ignore_e
-00030330: 6d70 7479 5f71 7565 7279 3a20 626f 6f6c  mpty_query: bool
-00030340: 2c20 6465 6661 756c 7420 4661 6c73 652e  , default False.
-00030350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00030360: 2020 3a70 6172 616d 2075 7064 6174 655f    :param update_
-00030370: 7365 7373 696f 6e5f 6166 7465 725f 6672  session_after_fr
-00030380: 6571 3a20 696e 742c 2064 6566 6175 6c74  eq: int, default
-00030390: 2031 3030 302e 0d0a 2020 2020 2020 2020   1000...        
-000303a0: 2020 2020 2020 2020 3a70 6172 616d 2075          :param u
-000303b0: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
-000303c0: 7465 725f 7365 636f 6e64 733a 2066 6c6f  ter_seconds: flo
-000303d0: 6174 2c20 6465 6661 756c 7420 3135 3030  at, default 1500
-000303e0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000303f0: 2020 203a 7061 7261 6d20 6966 5f73 686f     :param if_sho
-00030400: 775f 7469 6d65 5f73 7461 743a 2062 6f6f  w_time_stat: boo
-00030410: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-00030420: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00030430: 2020 203a 7061 7261 6d20 7368 6f77 5f74     :param show_t
-00030440: 696d 655f 7374 6174 5f70 7265 6369 7369  ime_stat_precisi
-00030450: 6f6e 3a20 696e 742c 2064 6566 6175 6c74  on: int, default
-00030460: 2032 2e0d 0a20 2020 2020 2020 2020 2020   2...           
-00030470: 2020 2020 203a 7061 7261 6d20 6966 5f70       :param if_p
-00030480: 7269 6e74 5f77 6172 6e69 6e67 3a20 626f  rint_warning: bo
-00030490: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
-000304a0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000304b0: 2020 203a 7061 7261 6d20 6d79 4d65 6d6f     :param myMemo
-000304c0: 7279 5f6d 6f64 653a 2073 7472 2c20 6465  ry_mode: str, de
-000304d0: 6661 756c 7420 2277 6562 222c 2063 686f  fault "web", cho
-000304e0: 6f73 6520 6672 6f6d 2028 2277 6562 222c  ose from ("web",
-000304f0: 2022 6170 6922 292e 0d0a 2020 2020 2020   "api")...      
-00030500: 2020 3a72 6574 7572 6e3a 2073 7472 206f    :return: str o
-00030510: 7220 6469 6374 0d0a 2020 2020 2020 2020  r dict..        
-00030520: 2222 220d 0a0d 0a20 2020 2020 2020 206d  """....        m
-00030530: 6f64 6520 3d20 6b77 6172 6773 2e67 6574  ode = kwargs.get
-00030540: 2827 6d79 4d65 6d6f 7279 5f6d 6f64 6527  ('myMemory_mode'
-00030550: 2c20 2777 6562 2729 0d0a 2020 2020 2020  , 'web')..      
-00030560: 2020 7469 6d65 6f75 7420 3d20 6b77 6172    timeout = kwar
-00030570: 6773 2e67 6574 2827 7469 6d65 6f75 7427  gs.get('timeout'
-00030580: 2c20 4e6f 6e65 290d 0a20 2020 2020 2020  , None)..       
-00030590: 2070 726f 7869 6573 203d 206b 7761 7267   proxies = kwarg
-000305a0: 732e 6765 7428 2770 726f 7869 6573 272c  s.get('proxies',
-000305b0: 204e 6f6e 6529 0d0a 2020 2020 2020 2020   None)..        
-000305c0: 736c 6565 705f 7365 636f 6e64 7320 3d20  sleep_seconds = 
-000305d0: 6b77 6172 6773 2e67 6574 2827 736c 6565  kwargs.get('slee
-000305e0: 705f 7365 636f 6e64 7327 2c20 3029 0d0a  p_seconds', 0)..
-000305f0: 2020 2020 2020 2020 6966 5f70 7269 6e74          if_print
-00030600: 5f77 6172 6e69 6e67 203d 206b 7761 7267  _warning = kwarg
-00030610: 732e 6765 7428 2769 665f 7072 696e 745f  s.get('if_print_
-00030620: 7761 726e 696e 6727 2c20 5472 7565 290d  warning', True).
-00030630: 0a20 2020 2020 2020 2069 735f 6465 7461  .        is_deta
-00030640: 696c 5f72 6573 756c 7420 3d20 6b77 6172  il_result = kwar
-00030650: 6773 2e67 6574 2827 6973 5f64 6574 6169  gs.get('is_detai
-00030660: 6c5f 7265 7375 6c74 272c 2046 616c 7365  l_result', False
-00030670: 290d 0a20 2020 2020 2020 2075 7064 6174  )..        updat
-00030680: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
-00030690: 6672 6571 203d 206b 7761 7267 732e 6765  freq = kwargs.ge
-000306a0: 7428 2775 7064 6174 655f 7365 7373 696f  t('update_sessio
-000306b0: 6e5f 6166 7465 725f 6672 6571 272c 2073  n_after_freq', s
-000306c0: 656c 662e 6465 6661 756c 745f 7365 7373  elf.default_sess
-000306d0: 696f 6e5f 6672 6571 290d 0a20 2020 2020  ion_freq)..     
-000306e0: 2020 2075 7064 6174 655f 7365 7373 696f     update_sessio
-000306f0: 6e5f 6166 7465 725f 7365 636f 6e64 7320  n_after_seconds 
-00030700: 3d20 6b77 6172 6773 2e67 6574 2827 7570  = kwargs.get('up
-00030710: 6461 7465 5f73 6573 7369 6f6e 5f61 6674  date_session_aft
-00030720: 6572 5f73 6563 6f6e 6473 272c 2073 656c  er_seconds', sel
-00030730: 662e 6465 6661 756c 745f 7365 7373 696f  f.default_sessio
-00030740: 6e5f 7365 636f 6e64 7329 0d0a 2020 2020  n_seconds)..    
-00030750: 2020 2020 7365 6c66 2e63 6865 636b 5f69      self.check_i
-00030760: 6e70 7574 5f6c 696d 6974 2871 7565 7279  nput_limit(query
-00030770: 5f74 6578 742c 2073 656c 662e 696e 7075  _text, self.inpu
-00030780: 745f 6c69 6d69 7429 0d0a 0d0a 2020 2020  t_limit)....    
-00030790: 2020 2020 6e6f 745f 7570 6461 7465 5f63      not_update_c
-000307a0: 6f6e 645f 6672 6571 203d 2031 2069 6620  ond_freq = 1 if 
-000307b0: 7365 6c66 2e71 7565 7279 5f63 6f75 6e74  self.query_count
-000307c0: 203c 2075 7064 6174 655f 7365 7373 696f   < update_sessio
-000307d0: 6e5f 6166 7465 725f 6672 6571 2065 6c73  n_after_freq els
-000307e0: 6520 300d 0a20 2020 2020 2020 206e 6f74  e 0..        not
-000307f0: 5f75 7064 6174 655f 636f 6e64 5f74 696d  _update_cond_tim
-00030800: 6520 3d20 3120 6966 2074 696d 652e 7469  e = 1 if time.ti
-00030810: 6d65 2829 202d 2073 656c 662e 6265 6769  me() - self.begi
-00030820: 6e5f 7469 6d65 203c 2075 7064 6174 655f  n_time < update_
-00030830: 7365 7373 696f 6e5f 6166 7465 725f 7365  session_after_se
-00030840: 636f 6e64 7320 656c 7365 2030 0d0a 2020  conds else 0..  
-00030850: 2020 2020 2020 6966 206e 6f74 2028 7365        if not (se
-00030860: 6c66 2e73 6573 7369 6f6e 2061 6e64 2073  lf.session and s
-00030870: 656c 662e 6c61 6e67 7561 6765 5f6d 6170  elf.language_map
-00030880: 2061 6e64 206e 6f74 5f75 7064 6174 655f   and not_update_
-00030890: 636f 6e64 5f66 7265 7120 616e 6420 6e6f  cond_freq and no
-000308a0: 745f 7570 6461 7465 5f63 6f6e 645f 7469  t_update_cond_ti
-000308b0: 6d65 293a 0d0a 2020 2020 2020 2020 2020  me):..          
-000308c0: 2020 7365 6c66 2e73 6573 7369 6f6e 203d    self.session =
-000308d0: 2072 6571 7565 7374 732e 5365 7373 696f   requests.Sessio
-000308e0: 6e28 290d 0a20 2020 2020 2020 2020 2020  n()..           
-000308f0: 2068 6f73 745f 6874 6d6c 203d 2073 656c   host_html = sel
-00030900: 662e 7365 7373 696f 6e2e 6765 7428 7365  f.session.get(se
-00030910: 6c66 2e68 6f73 745f 7572 6c2c 2068 6561  lf.host_url, hea
-00030920: 6465 7273 3d73 656c 662e 686f 7374 5f68  ders=self.host_h
-00030930: 6561 6465 7273 2c20 7469 6d65 6f75 743d  eaders, timeout=
-00030940: 7469 6d65 6f75 742c 2070 726f 7869 6573  timeout, proxies
-00030950: 3d70 726f 7869 6573 292e 7465 7874 0d0a  =proxies).text..
-00030960: 2020 2020 2020 2020 2020 2020 6465 6275              debu
-00030970: 675f 6c61 6e67 5f6b 7761 7267 7320 3d20  g_lang_kwargs = 
-00030980: 7365 6c66 2e64 6562 7567 5f6c 616e 675f  self.debug_lang_
-00030990: 6b77 6172 6773 2866 726f 6d5f 6c61 6e67  kwargs(from_lang
-000309a0: 7561 6765 2c20 746f 5f6c 616e 6775 6167  uage, to_languag
-000309b0: 652c 2073 656c 662e 6465 6661 756c 745f  e, self.default_
-000309c0: 6672 6f6d 5f6c 616e 6775 6167 652c 2069  from_language, i
-000309d0: 665f 7072 696e 745f 7761 726e 696e 6729  f_print_warning)
-000309e0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000309f0: 6c66 2e6c 616e 6775 6167 655f 6d61 7020  lf.language_map 
-00030a00: 3d20 7365 6c66 2e67 6574 5f6c 616e 6775  = self.get_langu
-00030a10: 6167 655f 6d61 7028 686f 7374 5f68 746d  age_map(host_htm
-00030a20: 6c2c 202a 2a64 6562 7567 5f6c 616e 675f  l, **debug_lang_
-00030a30: 6b77 6172 6773 290d 0a0d 0a20 2020 2020  kwargs)....     
-00030a40: 2020 2069 6620 6672 6f6d 5f6c 616e 6775     if from_langu
-00030a50: 6167 6520 3d3d 2027 6175 746f 273a 0d0a  age == 'auto':..
-00030a60: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
-00030a70: 5f6c 616e 6775 6167 6520 3d20 7365 6c66  _language = self
-00030a80: 2e77 6172 6e69 6e67 5f61 7574 6f5f 6c61  .warning_auto_la
-00030a90: 6e67 2827 6d79 4d65 6d6f 7279 272c 2073  ng('myMemory', s
-00030aa0: 656c 662e 6465 6661 756c 745f 6672 6f6d  elf.default_from
-00030ab0: 5f6c 616e 6775 6167 652c 2069 665f 7072  _language, if_pr
-00030ac0: 696e 745f 7761 726e 696e 6729 0d0a 2020  int_warning)..  
-00030ad0: 2020 2020 2020 6672 6f6d 5f6c 616e 6775        from_langu
-00030ae0: 6167 652c 2074 6f5f 6c61 6e67 7561 6765  age, to_language
-00030af0: 203d 2073 656c 662e 6368 6563 6b5f 6c61   = self.check_la
-00030b00: 6e67 7561 6765 2866 726f 6d5f 6c61 6e67  nguage(from_lang
-00030b10: 7561 6765 2c20 746f 5f6c 616e 6775 6167  uage, to_languag
-00030b20: 652c 2073 656c 662e 6c61 6e67 7561 6765  e, self.language
-00030b30: 5f6d 6170 2c20 6f75 7470 7574 5f7a 683d  _map, output_zh=
-00030b40: 7365 6c66 2e6f 7574 7075 745f 7a68 2c0d  self.output_zh,.
-00030b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00030b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030b80: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00030b90: 5f65 6e5f 7472 616e 736c 6174 6f72 3d27  _en_translator='
-00030ba0: 6d79 4d65 6d6f 7279 272c 206f 7574 7075  myMemory', outpu
-00030bb0: 745f 656e 3d27 656e 2d47 4227 290d 0a0d  t_en='en-GB')...
-00030bc0: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-00030bd0: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-00030be0: 2027 7127 3a20 7175 6572 795f 7465 7874   'q': query_text
-00030bf0: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00030c00: 6c61 6e67 7061 6972 273a 2066 277b 6672  langpair': f'{fr
-00030c10: 6f6d 5f6c 616e 6775 6167 657d 7c7b 746f  om_language}|{to
-00030c20: 5f6c 616e 6775 6167 657d 270d 0a20 2020  _language}'..   
-00030c30: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00030c40: 7061 7261 6d73 203d 2070 6172 616d 7320  params = params 
-00030c50: 6966 206d 6f64 6520 3d3d 2027 6170 6927  if mode == 'api'
-00030c60: 2065 6c73 6520 7b2a 2a70 6172 616d 732c   else {**params,
-00030c70: 202a 2a7b 276d 746f 6e6c 7927 3a20 317d   **{'mtonly': 1}
-00030c80: 7d0d 0a20 2020 2020 2020 2061 7069 5f75  }..        api_u
-00030c90: 726c 203d 2073 656c 662e 6170 695f 6170  rl = self.api_ap
-00030ca0: 695f 7572 6c20 6966 206d 6f64 6520 3d3d  i_url if mode ==
-00030cb0: 2027 6170 6927 2065 6c73 6520 7365 6c66   'api' else self
-00030cc0: 2e61 7069 5f77 6562 5f75 726c 0d0a 0d0a  .api_web_url....
-00030cd0: 2020 2020 2020 2020 7220 3d20 7365 6c66          r = self
-00030ce0: 2e73 6573 7369 6f6e 2e67 6574 2861 7069  .session.get(api
-00030cf0: 5f75 726c 2c20 7061 7261 6d73 3d70 6172  _url, params=par
-00030d00: 616d 732c 2068 6561 6465 7273 3d73 656c  ams, headers=sel
-00030d10: 662e 686f 7374 5f68 6561 6465 7273 2c20  f.host_headers, 
-00030d20: 7469 6d65 6f75 743d 7469 6d65 6f75 742c  timeout=timeout,
-00030d30: 2070 726f 7869 6573 3d70 726f 7869 6573   proxies=proxies
-00030d40: 290d 0a20 2020 2020 2020 2072 2e72 6169  )..        r.rai
-00030d50: 7365 5f66 6f72 5f73 7461 7475 7328 290d  se_for_status().
-00030d60: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00030d70: 722e 6a73 6f6e 2829 0d0a 2020 2020 2020  r.json()..      
-00030d80: 2020 7469 6d65 2e73 6c65 6570 2873 6c65    time.sleep(sle
-00030d90: 6570 5f73 6563 6f6e 6473 290d 0a20 2020  ep_seconds)..   
-00030da0: 2020 2020 2073 656c 662e 7175 6572 795f       self.query_
-00030db0: 636f 756e 7420 2b3d 2031 0d0a 2020 2020  count += 1..    
-00030dc0: 2020 2020 7265 7475 726e 2064 6174 6120      return data 
-00030dd0: 6966 2069 735f 6465 7461 696c 5f72 6573  if is_detail_res
-00030de0: 756c 7420 656c 7365 2064 6174 615b 2772  ult else data['r
-00030df0: 6573 706f 6e73 6544 6174 6127 5d5b 2774  esponseData']['t
-00030e00: 7261 6e73 6c61 7465 6454 6578 7427 5d0d  ranslatedText'].
-00030e10: 0a0d 0a0d 0a63 6c61 7373 204d 6972 6169  .....class Mirai
-00030e20: 2854 7365 293a 0d0a 2020 2020 6465 6620  (Tse):..    def 
-00030e30: 5f5f 696e 6974 5f5f 2873 656c 6629 3a0d  __init__(self):.
-00030e40: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00030e50: 2e5f 5f69 6e69 745f 5f28 290d 0a20 2020  .__init__()..   
-00030e60: 2020 2020 2073 656c 662e 686f 6d65 5f75       self.home_u
-00030e70: 726c 203d 2027 6874 7470 733a 2f2f 6d69  rl = 'https://mi
-00030e80: 7261 6974 7261 6e73 6c61 7465 2e63 6f6d  raitranslate.com
-00030e90: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
-00030ea0: 686f 7374 5f75 726c 203d 2027 6874 7470  host_url = 'http
-00030eb0: 733a 2f2f 6d69 7261 6974 7261 6e73 6c61  s://miraitransla
-00030ec0: 7465 2e63 6f6d 2f74 7269 616c 2f27 0d0a  te.com/trial/'..
-00030ed0: 2020 2020 2020 2020 7365 6c66 2e61 7069          self.api
-00030ee0: 5f75 726c 203d 2027 6874 7470 733a 2f2f  _url = 'https://
-00030ef0: 7472 6961 6c2e 6d69 7261 6974 7261 6e73  trial.miraitrans
-00030f00: 6c61 7465 2e63 6f6d 2f74 7269 616c 2f61  late.com/trial/a
-00030f10: 7069 2f74 7261 6e73 6c61 7465 2e70 6870  pi/translate.php
-00030f20: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
-00030f30: 6c61 6e67 5f75 726c 203d 204e 6f6e 650d  lang_url = None.
-00030f40: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00030f50: 6e67 5f75 726c 5f70 6174 7465 726e 203d  ng_url_pattern =
-00030f60: 2027 6d61 696e 2d65 7332 3031 352e 282e   'main-es2015.(.
-00030f70: 2a3f 292e 6a73 270d 0a20 2020 2020 2020  *?).js'..       
-00030f80: 2073 656c 662e 6465 7465 6374 5f6c 616e   self.detect_lan
-00030f90: 675f 7572 6c20 3d20 2768 7474 7073 3a2f  g_url = 'https:/
-00030fa0: 2f74 7269 616c 2e6d 6972 6169 7472 616e  /trial.miraitran
-00030fb0: 736c 6174 652e 636f 6d2f 7472 6961 6c2f  slate.com/trial/
-00030fc0: 6170 692f 6465 7465 6374 5f6c 616e 672e  api/detect_lang.
-00030fd0: 7068 7027 0d0a 2020 2020 2020 2020 7365  php'..        se
-00030fe0: 6c66 2e74 7261 6365 5f75 726c 203d 2027  lf.trace_url = '
-00030ff0: 6874 7470 733a 2f2f 7472 6961 6c2e 6d69  https://trial.mi
-00031000: 7261 6974 7261 6e73 6c61 7465 2e63 6f6d  raitranslate.com
-00031010: 2f74 7269 616c 2f61 7069 2f74 7261 6365  /trial/api/trace
-00031020: 2e70 6870 270d 0a20 2020 2020 2020 2073  .php'..        s
-00031030: 656c 662e 686f 7374 5f68 6561 6465 7273  elf.host_headers
-00031040: 203d 2073 656c 662e 6765 745f 6865 6164   = self.get_head
-00031050: 6572 7328 7365 6c66 2e68 6f6d 655f 7572  ers(self.home_ur
-00031060: 6c2c 2069 665f 6170 693d 4661 6c73 6529  l, if_api=False)
-00031070: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00031080: 7069 5f6a 736f 6e5f 6865 6164 6572 7320  pi_json_headers 
-00031090: 3d20 7365 6c66 2e67 6574 5f68 6561 6465  = self.get_heade
-000310a0: 7273 2873 656c 662e 686f 6d65 5f75 726c  rs(self.home_url
-000310b0: 2c20 6966 5f61 7069 3d54 7275 652c 2069  , if_api=True, i
-000310c0: 665f 6a73 6f6e 5f66 6f72 5f61 7069 3d54  f_json_for_api=T
-000310d0: 7275 6529 0d0a 2020 2020 2020 2020 7365  rue)..        se
-000310e0: 6c66 2e61 7069 5f74 6578 745f 6865 6164  lf.api_text_head
-000310f0: 6572 7320 3d20 7365 6c66 2e67 6574 5f68  ers = self.get_h
-00031100: 6561 6465 7273 2873 656c 662e 686f 6d65  eaders(self.home
-00031110: 5f75 726c 2c20 6966 5f61 7069 3d54 7275  _url, if_api=Tru
-00031120: 652c 2069 665f 616a 6178 5f66 6f72 5f61  e, if_ajax_for_a
-00031130: 7069 3d46 616c 7365 290d 0a20 2020 2020  pi=False)..     
-00031140: 2020 2073 656c 662e 7365 7373 696f 6e20     self.session 
-00031150: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-00031160: 7365 6c66 2e6c 616e 6775 6167 655f 6d61  self.language_ma
-00031170: 7020 3d20 4e6f 6e65 0d0a 2020 2020 2020  p = None..      
-00031180: 2020 7365 6c66 2e74 7261 6e5f 6b65 7920    self.tran_key 
-00031190: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-000311a0: 7365 6c66 2e74 7261 6e73 5f69 6420 3d20  self.trans_id = 
-000311b0: 7374 7228 7575 6964 2e75 7569 6434 2829  str(uuid.uuid4()
-000311c0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000311d0: 7573 6572 5f69 6420 3d20 7374 7228 7575  user_id = str(uu
-000311e0: 6964 2e75 7569 6434 2829 290d 0a20 2020  id.uuid4())..   
-000311f0: 2020 2020 2073 656c 662e 6c61 6e67 5f7a       self.lang_z
-00031200: 685f 6d61 7020 3d20 7b27 7a68 2d43 4e27  h_map = {'zh-CN'
-00031210: 3a20 277a 6827 2c20 277a 682d 5457 273a  : 'zh', 'zh-TW':
-00031220: 2027 7a74 277d 0d0a 2020 2020 2020 2020   'zt'}..        
-00031230: 7365 6c66 2e71 7565 7279 5f63 6f75 6e74  self.query_count
-00031240: 203d 2030 0d0a 2020 2020 2020 2020 7365   = 0..        se
-00031250: 6c66 2e6f 7574 7075 745f 7a68 203d 2027  lf.output_zh = '
-00031260: 7a68 270d 0a20 2020 2020 2020 2073 656c  zh'..        sel
-00031270: 662e 696e 7075 745f 6c69 6d69 7420 3d20  f.input_limit = 
-00031280: 696e 7428 3265 3329 0d0a 2020 2020 2020  int(2e3)..      
-00031290: 2020 7365 6c66 2e64 6566 6175 6c74 5f66    self.default_f
-000312a0: 726f 6d5f 6c61 6e67 7561 6765 203d 2073  rom_language = s
-000312b0: 656c 662e 6f75 7470 7574 5f7a 680d 0a0d  elf.output_zh...
-000312c0: 0a20 2020 2040 5473 652e 6465 6275 675f  .    @Tse.debug_
-000312d0: 6c61 6e67 7561 6765 5f6d 6170 0d0a 2020  language_map..  
-000312e0: 2020 6465 6620 6765 745f 6c61 6e67 7561    def get_langua
-000312f0: 6765 5f6d 6170 2873 656c 662c 206c 616e  ge_map(self, lan
-00031300: 675f 7572 6c3a 2073 7472 2c20 7373 3a20  g_url: str, ss: 
-00031310: 5365 7373 696f 6e54 7970 652c 2068 6561  SessionType, hea
-00031320: 6465 7273 3a20 6469 6374 2c20 7469 6d65  ders: dict, time
-00031330: 6f75 743a 204f 7074 696f 6e61 6c5b 666c  out: Optional[fl
-00031340: 6f61 745d 2c20 7072 6f78 6965 733a 204f  oat], proxies: O
-00031350: 7074 696f 6e61 6c5b 6469 6374 5d2c 202a  ptional[dict], *
-00031360: 2a6b 7761 7267 733a 204c 616e 674d 6170  *kwargs: LangMap
-00031370: 4b77 6172 6773 5479 7065 2920 2d3e 2064  KwargsType) -> d
-00031380: 6963 743a 0d0a 2020 2020 2020 2020 6a73  ict:..        js
-00031390: 5f68 746d 6c20 3d20 7373 2e67 6574 286c  _html = ss.get(l
-000313a0: 616e 675f 7572 6c2c 2068 6561 6465 7273  ang_url, headers
-000313b0: 3d68 6561 6465 7273 2c20 7469 6d65 6f75  =headers, timeou
-000313c0: 743d 7469 6d65 6f75 742c 2070 726f 7869  t=timeout, proxi
-000313d0: 6573 3d70 726f 7869 6573 292e 7465 7874  es=proxies).text
-000313e0: 0d0a 2020 2020 2020 2020 6c61 6e67 5f70  ..        lang_p
-000313f0: 6169 7273 203d 2072 652e 636f 6d70 696c  airs = re.compil
-00031400: 6528 2722 2f74 7269 616c 2f28 5c5c 777b  e('"/trial/(\\w{
-00031410: 327d 292f 285c 5c77 7b32 7d29 2227 292e  2})/(\\w{2})"').
-00031420: 6669 6e64 616c 6c28 6a73 5f68 746d 6c29  findall(js_html)
-00031430: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00031440: 207b 665f 6c61 6e67 3a20 5b76 2066 6f72   {f_lang: [v for
-00031450: 206b 2c20 7620 696e 206c 616e 675f 7061   k, v in lang_pa
-00031460: 6972 7320 6966 206b 203d 3d20 665f 6c61  irs if k == f_la
-00031470: 6e67 5d20 666f 7220 665f 6c61 6e67 2c20  ng] for f_lang, 
-00031480: 745f 6c61 6e67 2069 6e20 6c61 6e67 5f70  t_lang in lang_p
-00031490: 6169 7273 7d0d 0a0d 0a20 2020 2040 5473  airs}....    @Ts
-000314a0: 652e 756e 6365 7274 6966 6965 640d 0a20  e.uncertified.. 
-000314b0: 2020 2040 5473 652e 7469 6d65 5f73 7461     @Tse.time_sta
-000314c0: 740d 0a20 2020 2040 5473 652e 6368 6563  t..    @Tse.chec
-000314d0: 6b5f 7175 6572 790d 0a20 2020 2064 6566  k_query..    def
-000314e0: 206d 6972 6169 5f61 7069 2873 656c 662c   mirai_api(self,
-000314f0: 2071 7565 7279 5f74 6578 743a 2073 7472   query_text: str
-00031500: 2c20 6672 6f6d 5f6c 616e 6775 6167 653a  , from_language:
-00031510: 2073 7472 203d 2027 6175 746f 272c 2074   str = 'auto', t
-00031520: 6f5f 6c61 6e67 7561 6765 3a20 7374 7220  o_language: str 
-00031530: 3d20 276a 6127 2c20 2a2a 6b77 6172 6773  = 'ja', **kwargs
-00031540: 3a20 4170 694b 7761 7267 7354 7970 6529  : ApiKwargsType)
-00031550: 202d 3e20 556e 696f 6e5b 7374 722c 2064   -> Union[str, d
-00031560: 6963 745d 3a0d 0a20 2020 2020 2020 2022  ict]:..        "
-00031570: 2222 0d0a 2020 2020 2020 2020 6874 7470  ""..        http
-00031580: 733a 2f2f 6d69 7261 6974 7261 6e73 6c61  s://miraitransla
-00031590: 7465 2e63 6f6d 2f65 6e2f 7472 6961 6c2f  te.com/en/trial/
-000315a0: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000315b0: 2071 7565 7279 5f74 6578 743a 2073 7472   query_text: str
-000315c0: 2c20 6d75 7374 2e0d 0a20 2020 2020 2020  , must...       
-000315d0: 203a 7061 7261 6d20 6672 6f6d 5f6c 616e   :param from_lan
-000315e0: 6775 6167 653a 2073 7472 2c20 6465 6661  guage: str, defa
-000315f0: 756c 7420 2761 7574 6f27 2e0d 0a20 2020  ult 'auto'...   
-00031600: 2020 2020 203a 7061 7261 6d20 746f 5f6c       :param to_l
-00031610: 616e 6775 6167 653a 2073 7472 2c20 6465  anguage: str, de
-00031620: 6661 756c 7420 276a 6127 2e0d 0a20 2020  fault 'ja'...   
-00031630: 2020 2020 203a 7061 7261 6d20 2a2a 6b77       :param **kw
-00031640: 6172 6773 3a0d 0a20 2020 2020 2020 2020  args:..         
-00031650: 2020 2020 2020 203a 7061 7261 6d20 7469         :param ti
-00031660: 6d65 6f75 743a 2066 6c6f 6174 2c20 6465  meout: float, de
-00031670: 6661 756c 7420 4e6f 6e65 2e0d 0a20 2020  fault None...   
-00031680: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-00031690: 7261 6d20 7072 6f78 6965 733a 2064 6963  ram proxies: dic
-000316a0: 742c 2064 6566 6175 6c74 204e 6f6e 652e  t, default None.
-000316b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000316c0: 2020 3a70 6172 616d 2073 6c65 6570 5f73    :param sleep_s
-000316d0: 6563 6f6e 6473 3a20 666c 6f61 742c 2064  econds: float, d
-000316e0: 6566 6175 6c74 2030 2e0d 0a20 2020 2020  efault 0...     
-000316f0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00031700: 6d20 6973 5f64 6574 6169 6c5f 7265 7375  m is_detail_resu
-00031710: 6c74 3a20 626f 6f6c 2c20 6465 6661 756c  lt: bool, defaul
-00031720: 7420 4661 6c73 652e 0d0a 2020 2020 2020  t False...      
-00031730: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00031740: 2069 665f 6967 6e6f 7265 5f6c 696d 6974   if_ignore_limit
-00031750: 5f6f 665f 6c65 6e67 7468 3a20 626f 6f6c  _of_length: bool
-00031760: 2c20 6465 6661 756c 7420 4661 6c73 652e  , default False.
-00031770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00031780: 2020 3a70 6172 616d 206c 696d 6974 5f6f    :param limit_o
-00031790: 665f 6c65 6e67 7468 3a20 696e 742c 2064  f_length: int, d
-000317a0: 6566 6175 6c74 2032 3030 3030 2e0d 0a20  efault 20000... 
-000317b0: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-000317c0: 7061 7261 6d20 6966 5f69 676e 6f72 655f  param if_ignore_
-000317d0: 656d 7074 795f 7175 6572 793a 2062 6f6f  empty_query: boo
-000317e0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-000317f0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00031800: 2020 203a 7061 7261 6d20 7570 6461 7465     :param update
-00031810: 5f73 6573 7369 6f6e 5f61 6674 6572 5f66  _session_after_f
-00031820: 7265 713a 2069 6e74 2c20 6465 6661 756c  req: int, defaul
-00031830: 7420 3130 3030 2e0d 0a20 2020 2020 2020  t 1000...       
-00031840: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00031850: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
-00031860: 6674 6572 5f73 6563 6f6e 6473 3a20 666c  fter_seconds: fl
-00031870: 6f61 742c 2064 6566 6175 6c74 2031 3530  oat, default 150
-00031880: 302e 0d0a 2020 2020 2020 2020 2020 2020  0...            
-00031890: 2020 2020 3a70 6172 616d 2069 665f 7368      :param if_sh
-000318a0: 6f77 5f74 696d 655f 7374 6174 3a20 626f  ow_time_stat: bo
-000318b0: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-000318c0: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
-000318d0: 2020 2020 3a70 6172 616d 2073 686f 775f      :param show_
-000318e0: 7469 6d65 5f73 7461 745f 7072 6563 6973  time_stat_precis
-000318f0: 696f 6e3a 2069 6e74 2c20 6465 6661 756c  ion: int, defaul
-00031900: 7420 322e 0d0a 2020 2020 2020 2020 2020  t 2...          
-00031910: 2020 2020 2020 3a70 6172 616d 2069 665f        :param if_
-00031920: 7072 696e 745f 7761 726e 696e 673a 2062  print_warning: b
-00031930: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
-00031940: 652e 0d0a 2020 2020 2020 2020 3a72 6574  e...        :ret
-00031950: 7572 6e3a 2073 7472 206f 7220 6469 6374  urn: str or dict
-00031960: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
-00031970: 0a20 2020 2020 2020 2074 696d 656f 7574  .        timeout
-00031980: 203d 206b 7761 7267 732e 6765 7428 2774   = kwargs.get('t
-00031990: 696d 656f 7574 272c 204e 6f6e 6529 0d0a  imeout', None)..
-000319a0: 2020 2020 2020 2020 7072 6f78 6965 7320          proxies 
-000319b0: 3d20 6b77 6172 6773 2e67 6574 2827 7072  = kwargs.get('pr
-000319c0: 6f78 6965 7327 2c20 4e6f 6e65 290d 0a20  oxies', None).. 
-000319d0: 2020 2020 2020 2073 6c65 6570 5f73 6563         sleep_sec
-000319e0: 6f6e 6473 203d 206b 7761 7267 732e 6765  onds = kwargs.ge
-000319f0: 7428 2773 6c65 6570 5f73 6563 6f6e 6473  t('sleep_seconds
-00031a00: 272c 2030 290d 0a20 2020 2020 2020 2069  ', 0)..        i
-00031a10: 665f 7072 696e 745f 7761 726e 696e 6720  f_print_warning 
-00031a20: 3d20 6b77 6172 6773 2e67 6574 2827 6966  = kwargs.get('if
-00031a30: 5f70 7269 6e74 5f77 6172 6e69 6e67 272c  _print_warning',
-00031a40: 2054 7275 6529 0d0a 2020 2020 2020 2020   True)..        
-00031a50: 6973 5f64 6574 6169 6c5f 7265 7375 6c74  is_detail_result
-00031a60: 203d 206b 7761 7267 732e 6765 7428 2769   = kwargs.get('i
-00031a70: 735f 6465 7461 696c 5f72 6573 756c 7427  s_detail_result'
-00031a80: 2c20 4661 6c73 6529 0d0a 2020 2020 2020  , False)..      
-00031a90: 2020 7570 6461 7465 5f73 6573 7369 6f6e    update_session
-00031aa0: 5f61 6674 6572 5f66 7265 7120 3d20 6b77  _after_freq = kw
-00031ab0: 6172 6773 2e67 6574 2827 7570 6461 7465  args.get('update
-00031ac0: 5f73 6573 7369 6f6e 5f61 6674 6572 5f66  _session_after_f
-00031ad0: 7265 7127 2c20 7365 6c66 2e64 6566 6175  req', self.defau
-00031ae0: 6c74 5f73 6573 7369 6f6e 5f66 7265 7129  lt_session_freq)
-00031af0: 0d0a 2020 2020 2020 2020 7570 6461 7465  ..        update
-00031b00: 5f73 6573 7369 6f6e 5f61 6674 6572 5f73  _session_after_s
-00031b10: 6563 6f6e 6473 203d 206b 7761 7267 732e  econds = kwargs.
-00031b20: 6765 7428 2775 7064 6174 655f 7365 7373  get('update_sess
-00031b30: 696f 6e5f 6166 7465 725f 7365 636f 6e64  ion_after_second
-00031b40: 7327 2c20 7365 6c66 2e64 6566 6175 6c74  s', self.default
-00031b50: 5f73 6573 7369 6f6e 5f73 6563 6f6e 6473  _session_seconds
-00031b60: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00031b70: 6368 6563 6b5f 696e 7075 745f 6c69 6d69  check_input_limi
-00031b80: 7428 7175 6572 795f 7465 7874 2c20 7365  t(query_text, se
-00031b90: 6c66 2e69 6e70 7574 5f6c 696d 6974 290d  lf.input_limit).
-00031ba0: 0a0d 0a20 2020 2020 2020 206e 6f74 5f75  ...        not_u
-00031bb0: 7064 6174 655f 636f 6e64 5f66 7265 7120  pdate_cond_freq 
-00031bc0: 3d20 3120 6966 2073 656c 662e 7175 6572  = 1 if self.quer
-00031bd0: 795f 636f 756e 7420 3c20 7570 6461 7465  y_count < update
-00031be0: 5f73 6573 7369 6f6e 5f61 6674 6572 5f66  _session_after_f
-00031bf0: 7265 7120 656c 7365 2030 0d0a 2020 2020  req else 0..    
-00031c00: 2020 2020 6e6f 745f 7570 6461 7465 5f63      not_update_c
-00031c10: 6f6e 645f 7469 6d65 203d 2031 2069 6620  ond_time = 1 if 
-00031c20: 7469 6d65 2e74 696d 6528 2920 2d20 7365  time.time() - se
-00031c30: 6c66 2e62 6567 696e 5f74 696d 6520 3c20  lf.begin_time < 
-00031c40: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
-00031c50: 6674 6572 5f73 6563 6f6e 6473 2065 6c73  fter_seconds els
-00031c60: 6520 300d 0a20 2020 2020 2020 2069 6620  e 0..        if 
-00031c70: 6e6f 7420 2873 656c 662e 7365 7373 696f  not (self.sessio
-00031c80: 6e20 616e 6420 7365 6c66 2e6c 616e 6775  n and self.langu
-00031c90: 6167 655f 6d61 7020 616e 6420 6e6f 745f  age_map and not_
-00031ca0: 7570 6461 7465 5f63 6f6e 645f 6672 6571  update_cond_freq
-00031cb0: 2061 6e64 206e 6f74 5f75 7064 6174 655f   and not_update_
-00031cc0: 636f 6e64 5f74 696d 6520 616e 6420 7365  cond_time and se
-00031cd0: 6c66 2e74 7261 6e5f 6b65 7929 3a0d 0a20  lf.tran_key):.. 
-00031ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00031cf0: 7365 7373 696f 6e20 3d20 7265 7175 6573  session = reques
-00031d00: 7473 2e53 6573 7369 6f6e 2829 0d0a 2020  ts.Session()..  
-00031d10: 2020 2020 2020 2020 2020 2320 5f20 3d20            # _ = 
-00031d20: 7365 6c66 2e73 6573 7369 6f6e 2e67 6574  self.session.get
-00031d30: 2873 656c 662e 686f 6d65 5f75 726c 2c20  (self.home_url, 
-00031d40: 6865 6164 6572 733d 7365 6c66 2e68 6f73  headers=self.hos
-00031d50: 745f 6865 6164 6572 732c 2074 696d 656f  t_headers, timeo
-00031d60: 7574 3d74 696d 656f 7574 2c20 7072 6f78  ut=timeout, prox
-00031d70: 6965 733d 7072 6f78 6965 7329 0d0a 2020  ies=proxies)..  
-00031d80: 2020 2020 2020 2020 2020 686f 7374 5f68            host_h
-00031d90: 746d 6c20 3d20 7365 6c66 2e73 6573 7369  tml = self.sessi
-00031da0: 6f6e 2e67 6574 2873 656c 662e 686f 7374  on.get(self.host
-00031db0: 5f75 726c 2c20 6865 6164 6572 733d 7365  _url, headers=se
-00031dc0: 6c66 2e68 6f73 745f 6865 6164 6572 732c  lf.host_headers,
-00031dd0: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
-00031de0: 2c20 7072 6f78 6965 733d 7072 6f78 6965  , proxies=proxie
-00031df0: 7329 2e74 6578 740d 0a20 2020 2020 2020  s).text..       
-00031e00: 2020 2020 2073 656c 662e 7472 616e 5f6b       self.tran_k
-00031e10: 6579 203d 2072 652e 636f 6d70 696c 6528  ey = re.compile(
-00031e20: 2776 6172 2074 7261 6e20 3d20 2228 2e2a  'var tran = "(.*
-00031e30: 3f29 223b 2729 2e73 6561 7263 6828 686f  ?)";').search(ho
-00031e40: 7374 5f68 746d 6c29 2e67 726f 7570 2831  st_html).group(1
-00031e50: 290d 0a20 2020 2020 2020 2020 2020 206c  )..            l
-00031e60: 616e 675f 7572 6c5f 7061 7274 203d 2072  ang_url_part = r
-00031e70: 652e 636f 6d70 696c 6528 7365 6c66 2e6c  e.compile(self.l
-00031e80: 616e 675f 7572 6c5f 7061 7474 6572 6e29  ang_url_pattern)
-00031e90: 2e73 6561 7263 6828 686f 7374 5f68 746d  .search(host_htm
-00031ea0: 6c29 2e67 726f 7570 2829 0d0a 2020 2020  l).group()..    
-00031eb0: 2020 2020 2020 2020 7365 6c66 2e6c 616e          self.lan
-00031ec0: 675f 7572 6c20 3d20 6627 6874 7470 733a  g_url = f'https:
-00031ed0: 2f2f 6d69 7261 6974 7261 6e73 6c61 7465  //miraitranslate
-00031ee0: 2e63 6f6d 2f74 7269 616c 2f69 6e6d 742f  .com/trial/inmt/
-00031ef0: 7b6c 616e 675f 7572 6c5f 7061 7274 7d27  {lang_url_part}'
-00031f00: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
-00031f10: 6275 675f 6c61 6e67 5f6b 7761 7267 7320  bug_lang_kwargs 
-00031f20: 3d20 7365 6c66 2e64 6562 7567 5f6c 616e  = self.debug_lan
-00031f30: 675f 6b77 6172 6773 2866 726f 6d5f 6c61  g_kwargs(from_la
-00031f40: 6e67 7561 6765 2c20 746f 5f6c 616e 6775  nguage, to_langu
-00031f50: 6167 652c 2073 656c 662e 6465 6661 756c  age, self.defaul
-00031f60: 745f 6672 6f6d 5f6c 616e 6775 6167 652c  t_from_language,
-00031f70: 2069 665f 7072 696e 745f 7761 726e 696e   if_print_warnin
-00031f80: 6729 0d0a 2020 2020 2020 2020 2020 2020  g)..            
-00031f90: 7365 6c66 2e6c 616e 6775 6167 655f 6d61  self.language_ma
-00031fa0: 7020 3d20 7365 6c66 2e67 6574 5f6c 616e  p = self.get_lan
-00031fb0: 6775 6167 655f 6d61 7028 7365 6c66 2e6c  guage_map(self.l
-00031fc0: 616e 675f 7572 6c2c 2073 656c 662e 7365  ang_url, self.se
-00031fd0: 7373 696f 6e2c 2073 656c 662e 6170 695f  ssion, self.api_
-00031fe0: 6a73 6f6e 5f68 6561 6465 7273 2c20 7469  json_headers, ti
-00031ff0: 6d65 6f75 742c 2070 726f 7869 6573 2c20  meout, proxies, 
-00032000: 2a2a 6465 6275 675f 6c61 6e67 5f6b 7761  **debug_lang_kwa
-00032010: 7267 7329 0d0a 0d0a 2020 2020 2020 2020  rgs)....        
-00032020: 6966 2066 726f 6d5f 6c61 6e67 7561 6765  if from_language
-00032030: 203d 3d20 2761 7574 6f27 3a0d 0a20 2020   == 'auto':..   
-00032040: 2020 2020 2020 2020 2072 203d 2073 656c           r = sel
-00032050: 662e 7365 7373 696f 6e2e 706f 7374 2873  f.session.post(s
-00032060: 656c 662e 6465 7465 6374 5f6c 616e 675f  elf.detect_lang_
-00032070: 7572 6c2c 2068 6561 6465 7273 3d73 656c  url, headers=sel
-00032080: 662e 6170 695f 6a73 6f6e 5f68 6561 6465  f.api_json_heade
-00032090: 7273 2c20 6a73 6f6e 3d7b 2774 6578 7427  rs, json={'text'
-000320a0: 3a20 7175 6572 795f 7465 7874 7d2c 2074  : query_text}, t
-000320b0: 696d 656f 7574 3d74 696d 656f 7574 2c20  imeout=timeout, 
-000320c0: 7072 6f78 6965 733d 7072 6f78 6965 7329  proxies=proxies)
-000320d0: 0d0a 2020 2020 2020 2020 2020 2020 6672  ..            fr
-000320e0: 6f6d 5f6c 616e 6775 6167 6520 3d20 722e  om_language = r.
-000320f0: 6a73 6f6e 2829 5b27 6c61 6e67 7561 6765  json()['language
-00032100: 275d 0d0a 2020 2020 2020 2020 2020 2020  ']..            
-00032110: 6672 6f6d 5f6c 616e 6775 6167 6520 3d20  from_language = 
-00032120: 7365 6c66 2e6c 616e 675f 7a68 5f6d 6170  self.lang_zh_map
-00032130: 5b66 726f 6d5f 6c61 6e67 7561 6765 5d20  [from_language] 
-00032140: 6966 2027 7a68 2720 696e 2066 726f 6d5f  if 'zh' in from_
-00032150: 6c61 6e67 7561 6765 2065 6c73 6520 6672  language else fr
-00032160: 6f6d 5f6c 616e 6775 6167 650d 0a20 2020  om_language..   
-00032170: 2020 2020 2066 726f 6d5f 6c61 6e67 7561       from_langua
-00032180: 6765 2c20 746f 5f6c 616e 6775 6167 6520  ge, to_language 
-00032190: 3d20 7365 6c66 2e63 6865 636b 5f6c 616e  = self.check_lan
-000321a0: 6775 6167 6528 6672 6f6d 5f6c 616e 6775  guage(from_langu
-000321b0: 6167 652c 2074 6f5f 6c61 6e67 7561 6765  age, to_language
-000321c0: 2c20 7365 6c66 2e6c 616e 6775 6167 655f  , self.language_
-000321d0: 6d61 702c 206f 7574 7075 745f 7a68 3d73  map, output_zh=s
-000321e0: 656c 662e 6f75 7470 7574 5f7a 6829 0d0a  elf.output_zh)..
-000321f0: 0d0a 2020 2020 2020 2020 7472 6163 655f  ..        trace_
-00032200: 6461 7461 203d 207b 0d0a 2020 2020 2020  data = {..      
-00032210: 2020 2020 2020 276f 7065 7261 7469 6f6e        'operation
-00032220: 5479 7065 273a 2027 534c 4127 2c0d 0a20  Type': 'SLA',.. 
-00032230: 2020 2020 2020 2020 2020 2027 6c61 6e67             'lang
-00032240: 273a 2066 726f 6d5f 6c61 6e67 7561 6765  ': from_language
-00032250: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00032260: 736f 7572 6365 273a 2071 7565 7279 5f74  source': query_t
-00032270: 6578 742c 0d0a 2020 2020 2020 2020 2020  ext,..          
-00032280: 2020 2775 7365 7249 6427 3a20 7365 6c66    'userId': self
-00032290: 2e75 7365 725f 6964 2c0d 0a20 2020 2020  .user_id,..     
-000322a0: 2020 2020 2020 2027 7472 616e 7349 6427         'transId'
-000322b0: 3a20 7365 6c66 2e74 7261 6e73 5f69 642c  : self.trans_id,
-000322c0: 0d0a 2020 2020 2020 2020 2020 2020 2775  ..            'u
-000322d0: 6e69 7175 6549 6427 3a20 7365 6c66 2e74  niqueId': self.t
-000322e0: 7261 6e5f 6b65 792c 0d0a 2020 2020 2020  ran_key,..      
-000322f0: 2020 2020 2020 2764 6174 6527 3a20 6627        'date': f'
-00032300: 7b64 6174 6574 696d 652e 6461 7465 7469  {datetime.dateti
-00032310: 6d65 2e75 7463 6e6f 7728 292e 6973 6f66  me.utcnow().isof
-00032320: 6f72 6d61 7428 295b 3a2d 335d 7d5a 272c  ormat()[:-3]}Z',
-00032330: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
-00032340: 2020 2020 205f 203d 2073 656c 662e 7365       _ = self.se
-00032350: 7373 696f 6e2e 706f 7374 2873 656c 662e  ssion.post(self.
-00032360: 7472 6163 655f 7572 6c2c 206a 736f 6e3d  trace_url, json=
-00032370: 7472 6163 655f 6461 7461 2c20 6865 6164  trace_data, head
-00032380: 6572 733d 7365 6c66 2e61 7069 5f74 6578  ers=self.api_tex
-00032390: 745f 6865 6164 6572 732c 2074 696d 656f  t_headers, timeo
-000323a0: 7574 3d74 696d 656f 7574 2c20 7072 6f78  ut=timeout, prox
-000323b0: 6965 733d 7072 6f78 6965 7329 0d0a 0d0a  ies=proxies)....
-000323c0: 2020 2020 2020 2020 7061 796c 6f61 6420          payload 
-000323d0: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-000323e0: 2027 696e 7075 7427 3a20 7175 6572 795f   'input': query_
-000323f0: 7465 7874 2c0d 0a20 2020 2020 2020 2020  text,..         
-00032400: 2020 2027 736f 7572 6365 273a 2066 726f     'source': fro
-00032410: 6d5f 6c61 6e67 7561 6765 2c0d 0a20 2020  m_language,..   
-00032420: 2020 2020 2020 2020 2027 7461 7267 6574           'target
-00032430: 273a 2074 6f5f 6c61 6e67 7561 6765 2c0d  ': to_language,.
-00032440: 0a20 2020 2020 2020 2020 2020 2027 7472  .            'tr
-00032450: 616e 273a 2073 656c 662e 7472 616e 5f6b  an': self.tran_k
-00032460: 6579 2c0d 0a20 2020 2020 2020 2020 2020  ey,..           
-00032470: 2027 6164 6170 7450 6872 6173 6573 273a   'adaptPhrases':
-00032480: 205b 5d2c 0d0a 2020 2020 2020 2020 2020   [],..          
-00032490: 2020 2766 696c 7465 725f 7072 6f66 696c    'filter_profil
-000324a0: 6527 3a20 276e 6d74 272c 0d0a 2020 2020  e': 'nmt',..    
-000324b0: 2020 2020 2020 2020 2770 726f 6669 6c65          'profile
-000324c0: 273a 2027 696e 6d74 272c 0d0a 2020 2020  ': 'inmt',..    
-000324d0: 2020 2020 2020 2020 2775 7365 5072 6566          'usePref
-000324e0: 6978 273a 2027 6661 6c73 6527 2c0d 0a20  ix': 'false',.. 
-000324f0: 2020 2020 2020 2020 2020 2027 7a74 273a             'zt':
-00032500: 2027 7472 7565 2720 6966 2027 7a74 2720   'true' if 'zt' 
-00032510: 696e 2028 6672 6f6d 5f6c 616e 6775 6167  in (from_languag
-00032520: 652c 2074 6f5f 6c61 6e67 7561 6765 2920  e, to_language) 
-00032530: 656c 7365 2027 6661 6c73 6527 2c0d 0a20  else 'false',.. 
-00032540: 2020 2020 2020 2020 2020 2027 496e 6d74             'Inmt
-00032550: 5461 7267 6574 273a 2027 272c 0d0a 2020  Target': '',..  
-00032560: 2020 2020 2020 2020 2020 2749 6e6d 7454            'InmtT
-00032570: 7261 6e73 6c61 7465 5479 7065 273a 2027  ranslateType': '
-00032580: 6769 7374 696e 6727 2c0d 0a20 2020 2020  gisting',..     
-00032590: 2020 207d 0d0a 2020 2020 2020 2020 7220     }..        r 
-000325a0: 3d20 7365 6c66 2e73 6573 7369 6f6e 2e70  = self.session.p
-000325b0: 6f73 7428 7365 6c66 2e61 7069 5f75 726c  ost(self.api_url
-000325c0: 2c20 6461 7461 3d70 6179 6c6f 6164 2c20  , data=payload, 
-000325d0: 6865 6164 6572 733d 7365 6c66 2e61 7069  headers=self.api
-000325e0: 5f74 6578 745f 6865 6164 6572 732c 2074  _text_headers, t
-000325f0: 696d 656f 7574 3d74 696d 656f 7574 2c20  imeout=timeout, 
-00032600: 7072 6f78 6965 733d 7072 6f78 6965 7329  proxies=proxies)
-00032610: 0d0a 2020 2020 2020 2020 722e 7261 6973  ..        r.rais
-00032620: 655f 666f 725f 7374 6174 7573 2829 0d0a  e_for_status()..
-00032630: 2020 2020 2020 2020 6461 7461 203d 2072          data = r
-00032640: 2e6a 736f 6e28 290d 0a20 2020 2020 2020  .json()..       
-00032650: 2074 696d 652e 736c 6565 7028 736c 6565   time.sleep(slee
-00032660: 705f 7365 636f 6e64 7329 0d0a 2020 2020  p_seconds)..    
-00032670: 2020 2020 7365 6c66 2e71 7565 7279 5f63      self.query_c
-00032680: 6f75 6e74 202b 3d20 310d 0a20 2020 2020  ount += 1..     
-00032690: 2020 2072 6574 7572 6e20 6461 7461 2069     return data i
-000326a0: 6620 6973 5f64 6574 6169 6c5f 7265 7375  f is_detail_resu
-000326b0: 6c74 2065 6c73 6520 6461 7461 5b27 6f75  lt else data['ou
-000326c0: 7075 7473 275d 5b30 5d5b 276f 7574 7075  puts'][0]['outpu
-000326d0: 7427 5d5b 305d 5b27 7472 616e 736c 6174  t'][0]['translat
-000326e0: 696f 6e27 5d0d 0a0d 0a0d 0a63 6c61 7373  ion']......class
-000326f0: 2041 7065 7274 6975 6d28 5473 6529 3a0d   Apertium(Tse):.
-00032700: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00032710: 5f28 7365 6c66 293a 0d0a 2020 2020 2020  _(self):..      
-00032720: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-00032730: 5f5f 2829 0d0a 2020 2020 2020 2020 7365  __()..        se
-00032740: 6c66 2e68 6f73 745f 7572 6c20 3d20 2768  lf.host_url = 'h
-00032750: 7474 7073 3a2f 2f77 7777 2e61 7065 7274  ttps://www.apert
-00032760: 6975 6d2e 6f72 672f 270d 0a20 2020 2020  ium.org/'..     
-00032770: 2020 2073 656c 662e 6170 695f 7572 6c20     self.api_url 
-00032780: 3d20 2768 7474 7073 3a2f 2f61 7065 7274  = 'https://apert
-00032790: 6975 6d2e 6f72 672f 6170 792f 7472 616e  ium.org/apy/tran
-000327a0: 736c 6174 6527 0d0a 2020 2020 2020 2020  slate'..        
-000327b0: 7365 6c66 2e67 6574 5f6c 616e 675f 7572  self.get_lang_ur
-000327c0: 6c20 3d20 2768 7474 7073 3a2f 2f77 7777  l = 'https://www
-000327d0: 2e61 7065 7274 6975 6d2e 6f72 672f 696e  .apertium.org/in
-000327e0: 6465 782e 6a73 270d 0a20 2020 2020 2020  dex.js'..       
-000327f0: 2073 656c 662e 6465 7465 6374 5f6c 616e   self.detect_lan
-00032800: 675f 7572 6c20 3d20 2768 7474 7073 3a2f  g_url = 'https:/
-00032810: 2f61 7065 7274 6975 6d2e 6f72 672f 6170  /apertium.org/ap
-00032820: 792f 6964 656e 7469 6679 4c61 6e67 270d  y/identifyLang'.
-00032830: 0a20 2020 2020 2020 2073 656c 662e 686f  .        self.ho
-00032840: 7374 5f68 6561 6465 7273 203d 2073 656c  st_headers = sel
-00032850: 662e 6765 745f 6865 6164 6572 7328 7365  f.get_headers(se
-00032860: 6c66 2e68 6f73 745f 7572 6c2c 2069 665f  lf.host_url, if_
-00032870: 6170 693d 4661 6c73 652c 2069 665f 7265  api=False, if_re
-00032880: 6665 7265 725f 666f 725f 686f 7374 3d54  ferer_for_host=T
-00032890: 7275 6529 0d0a 2020 2020 2020 2020 7365  rue)..        se
-000328a0: 6c66 2e61 7069 5f68 6561 6465 7273 203d  lf.api_headers =
-000328b0: 2073 656c 662e 6765 745f 6865 6164 6572   self.get_header
-000328c0: 7328 7365 6c66 2e68 6f73 745f 7572 6c2c  s(self.host_url,
-000328d0: 2069 665f 6170 693d 5472 7565 290d 0a20   if_api=True).. 
-000328e0: 2020 2020 2020 2073 656c 662e 7365 7373         self.sess
-000328f0: 696f 6e20 3d20 4e6f 6e65 0d0a 2020 2020  ion = None..    
-00032900: 2020 2020 7365 6c66 2e6c 616e 6775 6167      self.languag
-00032910: 655f 6d61 7020 3d20 4e6f 6e65 0d0a 2020  e_map = None..  
-00032920: 2020 2020 2020 7365 6c66 2e71 7565 7279        self.query
-00032930: 5f63 6f75 6e74 203d 2030 0d0a 2020 2020  _count = 0..    
-00032940: 2020 2020 7365 6c66 2e6f 7574 7075 745f      self.output_
-00032950: 7a68 203d 204e 6f6e 6520 2023 2075 6e73  zh = None  # uns
-00032960: 7570 706f 7274 6564 0d0a 2020 2020 2020  upported..      
-00032970: 2020 7365 6c66 2e6f 7574 7075 745f 656e    self.output_en
-00032980: 203d 2027 656e 6727 0d0a 2020 2020 2020   = 'eng'..      
-00032990: 2020 7365 6c66 2e69 6e70 7574 5f6c 696d    self.input_lim
-000329a0: 6974 203d 2069 6e74 2831 6534 2920 2023  it = int(1e4)  #
-000329b0: 2061 6c6d 6f73 7420 6e6f 206c 696d 6974   almost no limit
-000329c0: 2e0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-000329d0: 6465 6661 756c 745f 6672 6f6d 5f6c 616e  default_from_lan
-000329e0: 6775 6167 6520 3d20 2773 7061 270d 0a0d  guage = 'spa'...
-000329f0: 0a20 2020 2040 5473 652e 6465 6275 675f  .    @Tse.debug_
-00032a00: 6c61 6e67 7561 6765 5f6d 6170 0d0a 2020  language_map..  
-00032a10: 2020 6465 6620 6765 745f 6c61 6e67 7561    def get_langua
-00032a20: 6765 5f6d 6170 2873 656c 662c 206c 616e  ge_map(self, lan
-00032a30: 675f 7572 6c3a 2073 7472 2c20 7373 3a20  g_url: str, ss: 
-00032a40: 5365 7373 696f 6e54 7970 652c 2068 6561  SessionType, hea
-00032a50: 6465 7273 3a20 6469 6374 2c20 7469 6d65  ders: dict, time
-00032a60: 6f75 743a 204f 7074 696f 6e61 6c5b 666c  out: Optional[fl
-00032a70: 6f61 745d 2c20 7072 6f78 6965 733a 204f  oat], proxies: O
-00032a80: 7074 696f 6e61 6c5b 6469 6374 5d2c 202a  ptional[dict], *
-00032a90: 2a6b 7761 7267 733a 204c 616e 674d 6170  *kwargs: LangMap
-00032aa0: 4b77 6172 6773 5479 7065 2920 2d3e 2064  KwargsType) -> d
-00032ab0: 6963 743a 0d0a 2020 2020 2020 2020 6a73  ict:..        js
-00032ac0: 5f68 746d 6c20 3d20 7373 2e67 6574 286c  _html = ss.get(l
-00032ad0: 616e 675f 7572 6c2c 2068 6561 6465 7273  ang_url, headers
-00032ae0: 3d68 6561 6465 7273 2c20 7469 6d65 6f75  =headers, timeou
-00032af0: 743d 7469 6d65 6f75 742c 2070 726f 7869  t=timeout, proxi
-00032b00: 6573 3d70 726f 7869 6573 292e 7465 7874  es=proxies).text
-00032b10: 0d0a 2020 2020 2020 2020 6c61 6e67 5f70  ..        lang_p
-00032b20: 6169 7273 203d 2072 652e 636f 6d70 696c  airs = re.compil
-00032b30: 6528 277b 736f 7572 6365 4c61 6e67 7561  e('{sourceLangua
-00032b40: 6765 3a22 282e 2a3f 2922 2c74 6172 6765  ge:"(.*?)",targe
-00032b50: 744c 616e 6775 6167 653a 2228 2e2a 3f29  tLanguage:"(.*?)
-00032b60: 227d 2729 2e66 696e 6461 6c6c 286a 735f  "}').findall(js_
-00032b70: 6874 6d6c 290d 0a20 2020 2020 2020 2072  html)..        r
-00032b80: 6574 7572 6e20 7b66 5f6c 616e 673a 205b  eturn {f_lang: [
-00032b90: 7620 666f 7220 6b2c 2076 2069 6e20 6c61  v for k, v in la
-00032ba0: 6e67 5f70 6169 7273 2069 6620 6b20 3d3d  ng_pairs if k ==
-00032bb0: 2066 5f6c 616e 675d 2066 6f72 2066 5f6c   f_lang] for f_l
-00032bc0: 616e 672c 2074 5f6c 616e 6720 696e 206c  ang, t_lang in l
-00032bd0: 616e 675f 7061 6972 737d 0d0a 0d0a 2020  ang_pairs}....  
-00032be0: 2020 4054 7365 2e74 696d 655f 7374 6174    @Tse.time_stat
-00032bf0: 0d0a 2020 2020 4054 7365 2e63 6865 636b  ..    @Tse.check
-00032c00: 5f71 7565 7279 0d0a 2020 2020 6465 6620  _query..    def 
-00032c10: 6170 6572 7469 756d 5f61 7069 2873 656c  apertium_api(sel
-00032c20: 662c 2071 7565 7279 5f74 6578 743a 2073  f, query_text: s
-00032c30: 7472 2c20 6672 6f6d 5f6c 616e 6775 6167  tr, from_languag
-00032c40: 653a 2073 7472 203d 2027 6175 746f 272c  e: str = 'auto',
-00032c50: 2074 6f5f 6c61 6e67 7561 6765 3a20 7374   to_language: st
-00032c60: 7220 3d20 2765 6e27 2c20 2a2a 6b77 6172  r = 'en', **kwar
-00032c70: 6773 3a20 4170 694b 7761 7267 7354 7970  gs: ApiKwargsTyp
-00032c80: 6529 202d 3e20 556e 696f 6e5b 7374 722c  e) -> Union[str,
-00032c90: 2064 6963 745d 3a0d 0a20 2020 2020 2020   dict]:..       
-00032ca0: 2022 2222 0d0a 2020 2020 2020 2020 6874   """..        ht
-00032cb0: 7470 733a 2f2f 7777 772e 6170 6572 7469  tps://www.aperti
-00032cc0: 756d 2e6f 7267 2f0d 0a20 2020 2020 2020  um.org/..       
-00032cd0: 203a 7061 7261 6d20 7175 6572 795f 7465   :param query_te
-00032ce0: 7874 3a20 7374 722c 206d 7573 742e 0d0a  xt: str, must...
-00032cf0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-00032d00: 726f 6d5f 6c61 6e67 7561 6765 3a20 7374  rom_language: st
-00032d10: 722c 2064 6566 6175 6c74 2027 6175 746f  r, default 'auto
-00032d20: 272e 0d0a 2020 2020 2020 2020 3a70 6172  '...        :par
-00032d30: 616d 2074 6f5f 6c61 6e67 7561 6765 3a20  am to_language: 
-00032d40: 7374 722c 2064 6566 6175 6c74 2027 656e  str, default 'en
-00032d50: 272e 0d0a 2020 2020 2020 2020 3a70 6172  '...        :par
-00032d60: 616d 202a 2a6b 7761 7267 733a 0d0a 2020  am **kwargs:..  
-00032d70: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-00032d80: 6172 616d 2074 696d 656f 7574 3a20 666c  aram timeout: fl
-00032d90: 6f61 742c 2064 6566 6175 6c74 204e 6f6e  oat, default Non
-00032da0: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
-00032db0: 2020 2020 3a70 6172 616d 2070 726f 7869      :param proxi
-00032dc0: 6573 3a20 6469 6374 2c20 6465 6661 756c  es: dict, defaul
-00032dd0: 7420 4e6f 6e65 2e0d 0a20 2020 2020 2020  t None...       
-00032de0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00032df0: 736c 6565 705f 7365 636f 6e64 733a 2066  sleep_seconds: f
-00032e00: 6c6f 6174 2c20 6465 6661 756c 7420 302e  loat, default 0.
-00032e10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00032e20: 2020 3a70 6172 616d 2069 735f 6465 7461    :param is_deta
-00032e30: 696c 5f72 6573 756c 743a 2062 6f6f 6c2c  il_result: bool,
-00032e40: 2064 6566 6175 6c74 2046 616c 7365 2e0d   default False..
-00032e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00032e60: 203a 7061 7261 6d20 6966 5f69 676e 6f72   :param if_ignor
-00032e70: 655f 6c69 6d69 745f 6f66 5f6c 656e 6774  e_limit_of_lengt
-00032e80: 683a 2062 6f6f 6c2c 2064 6566 6175 6c74  h: bool, default
-00032e90: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
-00032ea0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00032eb0: 6c69 6d69 745f 6f66 5f6c 656e 6774 683a  limit_of_length:
-00032ec0: 2069 6e74 2c20 6465 6661 756c 7420 3230   int, default 20
-00032ed0: 3030 302e 0d0a 2020 2020 2020 2020 2020  000...          
-00032ee0: 2020 2020 2020 3a70 6172 616d 2069 665f        :param if_
-00032ef0: 6967 6e6f 7265 5f65 6d70 7479 5f71 7565  ignore_empty_que
-00032f00: 7279 3a20 626f 6f6c 2c20 6465 6661 756c  ry: bool, defaul
-00032f10: 7420 4661 6c73 652e 0d0a 2020 2020 2020  t False...      
-00032f20: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00032f30: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
-00032f40: 6166 7465 725f 6672 6571 3a20 696e 742c  after_freq: int,
-00032f50: 2064 6566 6175 6c74 2031 3030 302e 0d0a   default 1000...
-00032f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032f70: 3a70 6172 616d 2075 7064 6174 655f 7365  :param update_se
-00032f80: 7373 696f 6e5f 6166 7465 725f 7365 636f  ssion_after_seco
-00032f90: 6e64 733a 2066 6c6f 6174 2c20 6465 6661  nds: float, defa
-00032fa0: 756c 7420 3135 3030 2e0d 0a20 2020 2020  ult 1500...     
-00032fb0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00032fc0: 6d20 6966 5f73 686f 775f 7469 6d65 5f73  m if_show_time_s
-00032fd0: 7461 743a 2062 6f6f 6c2c 2064 6566 6175  tat: bool, defau
-00032fe0: 6c74 2046 616c 7365 2e0d 0a20 2020 2020  lt False...     
-00032ff0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00033000: 6d20 7368 6f77 5f74 696d 655f 7374 6174  m show_time_stat
-00033010: 5f70 7265 6369 7369 6f6e 3a20 696e 742c  _precision: int,
-00033020: 2064 6566 6175 6c74 2032 2e0d 0a20 2020   default 2...   
-00033030: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-00033040: 7261 6d20 6966 5f70 7269 6e74 5f77 6172  ram if_print_war
-00033050: 6e69 6e67 3a20 626f 6f6c 2c20 6465 6661  ning: bool, defa
-00033060: 756c 7420 5472 7565 2e0d 0a20 2020 2020  ult True...     
-00033070: 2020 203a 7265 7475 726e 3a20 7374 7220     :return: str 
-00033080: 6f72 2064 6963 740d 0a20 2020 2020 2020  or dict..       
-00033090: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-000330a0: 7469 6d65 6f75 7420 3d20 6b77 6172 6773  timeout = kwargs
-000330b0: 2e67 6574 2827 7469 6d65 6f75 7427 2c20  .get('timeout', 
-000330c0: 4e6f 6e65 290d 0a20 2020 2020 2020 2070  None)..        p
-000330d0: 726f 7869 6573 203d 206b 7761 7267 732e  roxies = kwargs.
-000330e0: 6765 7428 2770 726f 7869 6573 272c 204e  get('proxies', N
-000330f0: 6f6e 6529 0d0a 2020 2020 2020 2020 736c  one)..        sl
-00033100: 6565 705f 7365 636f 6e64 7320 3d20 6b77  eep_seconds = kw
-00033110: 6172 6773 2e67 6574 2827 736c 6565 705f  args.get('sleep_
-00033120: 7365 636f 6e64 7327 2c20 3029 0d0a 2020  seconds', 0)..  
-00033130: 2020 2020 2020 6966 5f70 7269 6e74 5f77        if_print_w
-00033140: 6172 6e69 6e67 203d 206b 7761 7267 732e  arning = kwargs.
-00033150: 6765 7428 2769 665f 7072 696e 745f 7761  get('if_print_wa
-00033160: 726e 696e 6727 2c20 5472 7565 290d 0a20  rning', True).. 
-00033170: 2020 2020 2020 2069 735f 6465 7461 696c         is_detail
-00033180: 5f72 6573 756c 7420 3d20 6b77 6172 6773  _result = kwargs
-00033190: 2e67 6574 2827 6973 5f64 6574 6169 6c5f  .get('is_detail_
-000331a0: 7265 7375 6c74 272c 2046 616c 7365 290d  result', False).
-000331b0: 0a20 2020 2020 2020 2075 7064 6174 655f  .        update_
-000331c0: 7365 7373 696f 6e5f 6166 7465 725f 6672  session_after_fr
-000331d0: 6571 203d 206b 7761 7267 732e 6765 7428  eq = kwargs.get(
-000331e0: 2775 7064 6174 655f 7365 7373 696f 6e5f  'update_session_
-000331f0: 6166 7465 725f 6672 6571 272c 2073 656c  after_freq', sel
-00033200: 662e 6465 6661 756c 745f 7365 7373 696f  f.default_sessio
-00033210: 6e5f 6672 6571 290d 0a20 2020 2020 2020  n_freq)..       
-00033220: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
-00033230: 6166 7465 725f 7365 636f 6e64 7320 3d20  after_seconds = 
-00033240: 6b77 6172 6773 2e67 6574 2827 7570 6461  kwargs.get('upda
-00033250: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
-00033260: 5f73 6563 6f6e 6473 272c 2073 656c 662e  _seconds', self.
-00033270: 6465 6661 756c 745f 7365 7373 696f 6e5f  default_session_
-00033280: 7365 636f 6e64 7329 0d0a 2020 2020 2020  seconds)..      
-00033290: 2020 7365 6c66 2e63 6865 636b 5f69 6e70    self.check_inp
-000332a0: 7574 5f6c 696d 6974 2871 7565 7279 5f74  ut_limit(query_t
-000332b0: 6578 742c 2073 656c 662e 696e 7075 745f  ext, self.input_
-000332c0: 6c69 6d69 7429 0d0a 0d0a 2020 2020 2020  limit)....      
-000332d0: 2020 6e6f 745f 7570 6461 7465 5f63 6f6e    not_update_con
-000332e0: 645f 6672 6571 203d 2031 2069 6620 7365  d_freq = 1 if se
-000332f0: 6c66 2e71 7565 7279 5f63 6f75 6e74 203c  lf.query_count <
-00033300: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
-00033310: 6166 7465 725f 6672 6571 2065 6c73 6520  after_freq else 
-00033320: 300d 0a20 2020 2020 2020 206e 6f74 5f75  0..        not_u
-00033330: 7064 6174 655f 636f 6e64 5f74 696d 6520  pdate_cond_time 
-00033340: 3d20 3120 6966 2074 696d 652e 7469 6d65  = 1 if time.time
-00033350: 2829 202d 2073 656c 662e 6265 6769 6e5f  () - self.begin_
-00033360: 7469 6d65 203c 2075 7064 6174 655f 7365  time < update_se
-00033370: 7373 696f 6e5f 6166 7465 725f 7365 636f  ssion_after_seco
-00033380: 6e64 7320 656c 7365 2030 0d0a 2020 2020  nds else 0..    
-00033390: 2020 2020 6966 206e 6f74 2028 7365 6c66      if not (self
-000333a0: 2e73 6573 7369 6f6e 2061 6e64 2073 656c  .session and sel
-000333b0: 662e 6c61 6e67 7561 6765 5f6d 6170 2061  f.language_map a
-000333c0: 6e64 206e 6f74 5f75 7064 6174 655f 636f  nd not_update_co
-000333d0: 6e64 5f66 7265 7120 616e 6420 6e6f 745f  nd_freq and not_
-000333e0: 7570 6461 7465 5f63 6f6e 645f 7469 6d65  update_cond_time
-000333f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00033400: 7365 6c66 2e73 6573 7369 6f6e 203d 2072  self.session = r
-00033410: 6571 7565 7374 732e 5365 7373 696f 6e28  equests.Session(
-00033420: 290d 0a20 2020 2020 2020 2020 2020 205f  )..            _
-00033430: 203d 2073 656c 662e 7365 7373 696f 6e2e   = self.session.
-00033440: 6765 7428 7365 6c66 2e68 6f73 745f 7572  get(self.host_ur
-00033450: 6c2c 2068 6561 6465 7273 3d73 656c 662e  l, headers=self.
-00033460: 686f 7374 5f68 6561 6465 7273 2c20 7469  host_headers, ti
-00033470: 6d65 6f75 743d 7469 6d65 6f75 742c 2070  meout=timeout, p
-00033480: 726f 7869 6573 3d70 726f 7869 6573 290d  roxies=proxies).
-00033490: 0a20 2020 2020 2020 2020 2020 2064 6562  .            deb
-000334a0: 7567 5f6c 616e 675f 6b77 6172 6773 203d  ug_lang_kwargs =
-000334b0: 2073 656c 662e 6465 6275 675f 6c61 6e67   self.debug_lang
-000334c0: 5f6b 7761 7267 7328 6672 6f6d 5f6c 616e  _kwargs(from_lan
-000334d0: 6775 6167 652c 2074 6f5f 6c61 6e67 7561  guage, to_langua
-000334e0: 6765 2c20 7365 6c66 2e64 6566 6175 6c74  ge, self.default
-000334f0: 5f66 726f 6d5f 6c61 6e67 7561 6765 2c20  _from_language, 
-00033500: 6966 5f70 7269 6e74 5f77 6172 6e69 6e67  if_print_warning
-00033510: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00033520: 656c 662e 6c61 6e67 7561 6765 5f6d 6170  elf.language_map
-00033530: 203d 2073 656c 662e 6765 745f 6c61 6e67   = self.get_lang
-00033540: 7561 6765 5f6d 6170 2873 656c 662e 6765  uage_map(self.ge
-00033550: 745f 6c61 6e67 5f75 726c 2c20 7365 6c66  t_lang_url, self
-00033560: 2e73 6573 7369 6f6e 2c20 7365 6c66 2e68  .session, self.h
-00033570: 6f73 745f 6865 6164 6572 732c 2074 696d  ost_headers, tim
-00033580: 656f 7574 2c20 7072 6f78 6965 732c 202a  eout, proxies, *
-00033590: 2a64 6562 7567 5f6c 616e 675f 6b77 6172  *debug_lang_kwar
-000335a0: 6773 290d 0a0d 0a20 2020 2020 2020 2069  gs)....        i
-000335b0: 6620 6672 6f6d 5f6c 616e 6775 6167 6520  f from_language 
-000335c0: 3d3d 2027 6175 746f 273a 0d0a 2020 2020  == 'auto':..    
-000335d0: 2020 2020 2020 2020 7061 796c 6f61 6420          payload 
-000335e0: 3d20 7572 6c6c 6962 2e70 6172 7365 2e75  = urllib.parse.u
-000335f0: 726c 656e 636f 6465 287b 2771 273a 2071  rlencode({'q': q
-00033600: 7565 7279 5f74 6578 747d 290d 0a20 2020  uery_text})..   
-00033610: 2020 2020 2020 2020 206c 616e 6773 203d           langs =
-00033620: 2073 656c 662e 7365 7373 696f 6e2e 706f   self.session.po
-00033630: 7374 2873 656c 662e 6465 7465 6374 5f6c  st(self.detect_l
-00033640: 616e 675f 7572 6c2c 2064 6174 613d 7061  ang_url, data=pa
-00033650: 796c 6f61 642c 2068 6561 6465 7273 3d73  yload, headers=s
-00033660: 656c 662e 6170 695f 6865 6164 6572 732c  elf.api_headers,
-00033670: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
-00033680: 2c20 7072 6f78 6965 733d 7072 6f78 6965  , proxies=proxie
-00033690: 7329 2e6a 736f 6e28 290d 0a20 2020 2020  s).json()..     
-000336a0: 2020 2020 2020 2066 726f 6d5f 6c61 6e67         from_lang
-000336b0: 7561 6765 203d 2073 6f72 7465 6428 6c61  uage = sorted(la
-000336c0: 6e67 732c 206b 6579 3d6c 616d 6264 6120  ngs, key=lambda 
-000336d0: 6b3a 206c 616e 6773 5b6b 5d2c 2072 6576  k: langs[k], rev
-000336e0: 6572 7365 3d54 7275 6529 5b30 5d0d 0a20  erse=True)[0].. 
-000336f0: 2020 2020 2020 2066 726f 6d5f 6c61 6e67         from_lang
-00033700: 7561 6765 2c20 746f 5f6c 616e 6775 6167  uage, to_languag
-00033710: 6520 3d20 7365 6c66 2e63 6865 636b 5f6c  e = self.check_l
-00033720: 616e 6775 6167 6528 6672 6f6d 5f6c 616e  anguage(from_lan
-00033730: 6775 6167 652c 2074 6f5f 6c61 6e67 7561  guage, to_langua
-00033740: 6765 2c20 7365 6c66 2e6c 616e 6775 6167  ge, self.languag
-00033750: 655f 6d61 702c 0d0a 2020 2020 2020 2020  e_map,..        
-00033760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033790: 206f 7574 7075 745f 656e 5f74 7261 6e73   output_en_trans
-000337a0: 6c61 746f 723d 2761 7065 7274 6975 6d27  lator='apertium'
-000337b0: 2c20 6f75 7470 7574 5f65 6e3d 7365 6c66  , output_en=self
-000337c0: 2e6f 7574 7075 745f 656e 290d 0a0d 0a20  .output_en).... 
-000337d0: 2020 2020 2020 2070 6179 6c6f 6164 203d         payload =
-000337e0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-000337f0: 2771 273a 2071 7565 7279 5f74 6578 742c  'q': query_text,
-00033800: 0d0a 2020 2020 2020 2020 2020 2020 276c  ..            'l
-00033810: 616e 6770 6169 7227 3a20 6627 7b66 726f  angpair': f'{fro
-00033820: 6d5f 6c61 6e67 7561 6765 7d7c 7b74 6f5f  m_language}|{to_
-00033830: 6c61 6e67 7561 6765 7d27 2c0d 0a20 2020  language}',..   
-00033840: 2020 2020 2020 2020 2027 7072 6566 7327           'prefs'
-00033850: 3a20 2727 2c0d 0a20 2020 2020 2020 2020  : '',..         
-00033860: 2020 2027 6d61 726b 556e 6b6e 6f77 6e27     'markUnknown'
-00033870: 3a20 276e 6f27 2c0d 0a20 2020 2020 2020  : 'no',..       
-00033880: 207d 0d0a 2020 2020 2020 2020 7061 796c   }..        payl
-00033890: 6f61 6420 3d20 7572 6c6c 6962 2e70 6172  oad = urllib.par
-000338a0: 7365 2e75 726c 656e 636f 6465 2870 6179  se.urlencode(pay
-000338b0: 6c6f 6164 290d 0a20 2020 2020 2020 2072  load)..        r
-000338c0: 203d 2073 656c 662e 7365 7373 696f 6e2e   = self.session.
-000338d0: 706f 7374 2873 656c 662e 6170 695f 7572  post(self.api_ur
-000338e0: 6c2c 2064 6174 613d 7061 796c 6f61 642c  l, data=payload,
-000338f0: 2068 6561 6465 7273 3d73 656c 662e 6170   headers=self.ap
-00033900: 695f 6865 6164 6572 732c 2074 696d 656f  i_headers, timeo
-00033910: 7574 3d74 696d 656f 7574 2c20 7072 6f78  ut=timeout, prox
-00033920: 6965 733d 7072 6f78 6965 7329 0d0a 2020  ies=proxies)..  
-00033930: 2020 2020 2020 722e 7261 6973 655f 666f        r.raise_fo
-00033940: 725f 7374 6174 7573 2829 0d0a 2020 2020  r_status()..    
-00033950: 2020 2020 6461 7461 203d 2072 2e6a 736f      data = r.jso
-00033960: 6e28 290d 0a20 2020 2020 2020 2074 696d  n()..        tim
-00033970: 652e 736c 6565 7028 736c 6565 705f 7365  e.sleep(sleep_se
-00033980: 636f 6e64 7329 0d0a 2020 2020 2020 2020  conds)..        
-00033990: 7365 6c66 2e71 7565 7279 5f63 6f75 6e74  self.query_count
-000339a0: 202b 3d20 310d 0a20 2020 2020 2020 2072   += 1..        r
-000339b0: 6574 7572 6e20 6461 7461 2069 6620 6973  eturn data if is
-000339c0: 5f64 6574 6169 6c5f 7265 7375 6c74 2065  _detail_result e
-000339d0: 6c73 6520 6461 7461 5b27 7265 7370 6f6e  lse data['respon
-000339e0: 7365 4461 7461 275d 5b27 7472 616e 736c  seData']['transl
-000339f0: 6174 6564 5465 7874 275d 0d0a 0d0a 0d0a  atedText']......
-00033a00: 636c 6173 7320 5469 6c64 6528 5473 6529  class Tilde(Tse)
-00033a10: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
-00033a20: 745f 5f28 7365 6c66 293a 0d0a 2020 2020  t__(self):..    
-00033a30: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00033a40: 6974 5f5f 2829 0d0a 2020 2020 2020 2020  it__()..        
-00033a50: 7365 6c66 2e68 6f73 745f 7572 6c20 3d20  self.host_url = 
-00033a60: 2768 7474 7073 3a2f 2f74 7261 6e73 6c61  'https://transla
-00033a70: 7465 2e74 696c 6465 2e63 6f6d 2f27 0d0a  te.tilde.com/'..
-00033a80: 2020 2020 2020 2020 7365 6c66 2e61 7069          self.api
-00033a90: 5f75 726c 203d 2027 6874 7470 733a 2f2f  _url = 'https://
-00033aa0: 6c65 7473 6d74 2e65 752f 7773 2f73 6572  letsmt.eu/ws/ser
-00033ab0: 7669 6365 2e73 7663 2f6a 736f 6e2f 5472  vice.svc/json/Tr
-00033ac0: 616e 736c 6174 6545 7827 0d0a 2020 2020  anslateEx'..    
-00033ad0: 2020 2020 7365 6c66 2e67 6574 5f63 6f6e      self.get_con
-00033ae0: 6669 675f 7572 6c20 3d20 2768 7474 7073  fig_url = 'https
-00033af0: 3a2f 2f74 7261 6e73 6c61 7465 2e74 696c  ://translate.til
-00033b00: 6465 2e63 6f6d 2f61 7373 6574 732f 636f  de.com/assets/co
-00033b10: 6e66 6967 2e6c 6f63 616c 2e6a 736f 6e27  nfig.local.json'
-00033b20: 2020 2320 3f76 6572 7369 6f6e 3d34 3638    # ?version=468
-00033b30: 3532 0d0a 2020 2020 2020 2020 7365 6c66  52..        self
-00033b40: 2e73 7562 7363 7269 6265 5f75 726c 203d  .subscribe_url =
-00033b50: 2027 6874 7470 733a 2f2f 7472 616e 736c   'https://transl
-00033b60: 6174 652e 7469 6c64 652e 636f 6d2f 6173  ate.tilde.com/as
-00033b70: 7365 7473 2f73 7562 7363 7269 7074 696f  sets/subscriptio
-00033b80: 6e73 2d63 6f6e 6669 672e 6c6f 6361 6c2e  ns-config.local.
-00033b90: 6a73 6f6e 270d 0a20 2020 2020 2020 2073  json'..        s
-00033ba0: 656c 662e 706c 6175 7369 626c 655f 7572  elf.plausible_ur
-00033bb0: 6c20 3d20 2768 7474 7073 3a2f 2f70 6c61  l = 'https://pla
-00033bc0: 7573 6962 6c65 2e69 6f2f 6170 692f 6576  usible.io/api/ev
-00033bd0: 656e 7427 0d0a 2020 2020 2020 2020 7365  ent'..        se
-00033be0: 6c66 2e61 7574 685f 7572 6c20 3d20 2768  lf.auth_url = 'h
-00033bf0: 7474 7073 3a2f 2f61 7574 682e 7469 6c64  ttps://auth.tild
-00033c00: 652e 636f 6d2f 6175 7468 2f72 6561 6c6d  e.com/auth/realm
-00033c10: 732f 5469 6c64 652f 7072 6f74 6f63 6f6c  s/Tilde/protocol
-00033c20: 2f6f 7065 6e69 642d 636f 6e6e 6563 742f  /openid-connect/
-00033c30: 6c6f 6769 6e2d 7374 6174 7573 2d69 6672  login-status-ifr
-00033c40: 616d 652e 6874 6d6c 2f69 6e69 7427 0d0a  ame.html/init'..
-00033c50: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
-00033c60: 6563 685f 7572 6c20 3d20 2768 7474 7073  ech_url = 'https
-00033c70: 3a2f 2f76 612e 7469 6c64 652e 636f 6d2f  ://va.tilde.com/
-00033c80: 646c 2f64 6972 6563 746c 696e 652f 6148  dl/directline/aH
-00033c90: 5230 6344 6f76 4c33 4279 6232 5272 4f48  R0cDovL3Byb2RrOH
-00033ca0: 4e69 6233 5230 6157 786b 5a54 513d 2f74  Nib3R0aWxkZTQ=/t
-00033cb0: 6f6b 656e 732f 7370 6565 6368 270d 0a20  okens/speech'.. 
-00033cc0: 2020 2020 2020 2073 656c 662e 686f 7374         self.host
-00033cd0: 5f68 6561 6465 7273 203d 2073 656c 662e  _headers = self.
-00033ce0: 6765 745f 6865 6164 6572 7328 7365 6c66  get_headers(self
-00033cf0: 2e68 6f73 745f 7572 6c2c 2069 665f 6170  .host_url, if_ap
-00033d00: 693d 4661 6c73 652c 2069 665f 7265 6665  i=False, if_refe
-00033d10: 7265 725f 666f 725f 686f 7374 3d54 7275  rer_for_host=Tru
-00033d20: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
-00033d30: 2e61 7069 5f68 6561 6465 7273 203d 2073  .api_headers = s
-00033d40: 656c 662e 6765 745f 6865 6164 6572 7328  elf.get_headers(
-00033d50: 7365 6c66 2e68 6f73 745f 7572 6c2c 2069  self.host_url, i
-00033d60: 665f 6170 693d 5472 7565 2c20 6966 5f6a  f_api=True, if_j
-00033d70: 736f 6e5f 666f 725f 6170 693d 5472 7565  son_for_api=True
-00033d80: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00033d90: 7365 7373 696f 6e20 3d20 4e6f 6e65 0d0a  session = None..
-00033da0: 2020 2020 2020 2020 7365 6c66 2e6c 616e          self.lan
-00033db0: 6775 6167 655f 6d61 7020 3d20 4e6f 6e65  guage_map = None
-00033dc0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00033dd0: 616e 6770 6169 725f 6964 7320 3d20 4e6f  angpair_ids = No
-00033de0: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
-00033df0: 2e63 6f6e 6669 675f 6461 7461 203d 204e  .config_data = N
-00033e00: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
-00033e10: 662e 7379 735f 6461 7461 203d 204e 6f6e  f.sys_data = Non
-00033e20: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00033e30: 7175 6572 795f 636f 756e 7420 3d20 300d  query_count = 0.
-00033e40: 0a20 2020 2020 2020 2073 656c 662e 6f75  .        self.ou
-00033e50: 7470 7574 5f7a 6820 3d20 4e6f 6e65 2020  tput_zh = None  
-00033e60: 2320 756e 7375 7070 6f72 7465 640d 0a20  # unsupported.. 
-00033e70: 2020 2020 2020 2073 656c 662e 6f75 7470         self.outp
-00033e80: 7574 5f65 6e20 3d20 2765 6e67 270d 0a20  ut_en = 'eng'.. 
-00033e90: 2020 2020 2020 2073 656c 662e 696e 7075         self.inpu
-00033ea0: 745f 6c69 6d69 7420 3d20 696e 7428 3565  t_limit = int(5e
-00033eb0: 3329 2020 2320 756e 6b6e 6f77 6e0d 0a20  3)  # unknown.. 
-00033ec0: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
-00033ed0: 756c 745f 6672 6f6d 5f6c 616e 6775 6167  ult_from_languag
-00033ee0: 6520 3d20 276c 7627 2020 2320 2766 7227  e = 'lv'  # 'fr'
-00033ef0: 0d0a 0d0a 2020 2020 4054 7365 2e64 6562  ....    @Tse.deb
-00033f00: 7567 5f6c 616e 6775 6167 655f 6d61 700d  ug_language_map.
-00033f10: 0a20 2020 2064 6566 2067 6574 5f6c 616e  .    def get_lan
-00033f20: 6775 6167 655f 6d61 7028 7365 6c66 2c20  guage_map(self, 
-00033f30: 7379 735f 6461 7461 3a20 6469 6374 2c20  sys_data: dict, 
-00033f40: 2a2a 6b77 6172 6773 3a20 4c61 6e67 4d61  **kwargs: LangMa
-00033f50: 704b 7761 7267 7354 7970 6529 202d 3e20  pKwargsType) -> 
-00033f60: 6469 6374 3a0d 0a20 2020 2020 2020 206c  dict:..        l
-00033f70: 616e 675f 7061 6972 7320 3d20 5b5b 6974  ang_pairs = [[it
-00033f80: 656d 5b27 536f 7572 6365 4c61 6e67 7561  em['SourceLangua
-00033f90: 6765 275d 5b27 436f 6465 275d 2c20 6974  ge']['Code'], it
-00033fa0: 656d 5b27 5461 7267 6574 4c61 6e67 7561  em['TargetLangua
-00033fb0: 6765 275d 5b27 436f 6465 275d 5d20 666f  ge']['Code']] fo
-00033fc0: 7220 6974 656d 2069 6e20 7379 735f 6461  r item in sys_da
-00033fd0: 7461 5b27 5379 7374 656d 275d 2069 6620  ta['System'] if 
-00033fe0: 2747 656e 6572 616c 2720 696e 2069 7465  'General' in ite
-00033ff0: 6d5b 2744 6f6d 6169 6e27 5d5d 0d0a 2020  m['Domain']]..  
-00034000: 2020 2020 2020 7265 7475 726e 207b 665f        return {f_
-00034010: 6c61 6e67 3a20 5b76 2066 6f72 206b 2c20  lang: [v for k, 
-00034020: 7620 696e 206c 616e 675f 7061 6972 7320  v in lang_pairs 
-00034030: 6966 206b 203d 3d20 665f 6c61 6e67 5d20  if k == f_lang] 
-00034040: 666f 7220 665f 6c61 6e67 2c20 745f 6c61  for f_lang, t_la
-00034050: 6e67 2069 6e20 6c61 6e67 5f70 6169 7273  ng in lang_pairs
-00034060: 7d0d 0a0d 0a20 2020 2064 6566 2067 6574  }....    def get
-00034070: 5f6c 616e 6770 6169 725f 6964 7328 7365  _langpair_ids(se
-00034080: 6c66 2c20 7379 735f 6461 7461 3a20 6469  lf, sys_data: di
-00034090: 6374 2920 2d3e 2064 6963 743a 0d0a 2020  ct) -> dict:..  
-000340a0: 2020 2020 2020 7265 7475 726e 207b 6622        return {f"
-000340b0: 7b69 7465 6d5b 2753 6f75 7263 654c 616e  {item['SourceLan
-000340c0: 6775 6167 6527 5d5b 2743 6f64 6527 5d7d  guage']['Code']}
-000340d0: 2d7b 6974 656d 5b27 5461 7267 6574 4c61  -{item['TargetLa
-000340e0: 6e67 7561 6765 275d 5b27 436f 6465 275d  nguage']['Code']
-000340f0: 7d22 3a20 6974 656d 5b27 4944 275d 2066  }": item['ID'] f
-00034100: 6f72 2069 7465 6d20 696e 2073 7973 5f64  or item in sys_d
-00034110: 6174 615b 2753 7973 7465 6d27 5d20 6966  ata['System'] if
-00034120: 2027 4765 6e65 7261 6c27 2069 6e20 6974   'General' in it
-00034130: 656d 5b27 446f 6d61 696e 275d 7d0d 0a0d  em['Domain']}...
-00034140: 0a20 2020 2040 5473 652e 756e 6365 7274  .    @Tse.uncert
-00034150: 6966 6965 640d 0a20 2020 2040 5473 652e  ified..    @Tse.
-00034160: 7469 6d65 5f73 7461 740d 0a20 2020 2040  time_stat..    @
-00034170: 5473 652e 6368 6563 6b5f 7175 6572 790d  Tse.check_query.
-00034180: 0a20 2020 2064 6566 2074 696c 6465 5f61  .    def tilde_a
-00034190: 7069 2873 656c 662c 2071 7565 7279 5f74  pi(self, query_t
-000341a0: 6578 743a 2073 7472 2c20 6672 6f6d 5f6c  ext: str, from_l
-000341b0: 616e 6775 6167 653a 2073 7472 203d 2027  anguage: str = '
-000341c0: 6175 746f 272c 2074 6f5f 6c61 6e67 7561  auto', to_langua
-000341d0: 6765 3a20 7374 7220 3d20 2765 6e27 2c20  ge: str = 'en', 
-000341e0: 2a2a 6b77 6172 6773 3a20 4170 694b 7761  **kwargs: ApiKwa
-000341f0: 7267 7354 7970 6529 202d 3e20 556e 696f  rgsType) -> Unio
-00034200: 6e5b 7374 722c 2064 6963 745d 3a0d 0a20  n[str, dict]:.. 
-00034210: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00034220: 2020 2020 6874 7470 733a 2f2f 7472 616e      https://tran
-00034230: 736c 6174 652e 7469 6c64 652e 636f 6d2f  slate.tilde.com/
-00034240: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00034250: 2071 7565 7279 5f74 6578 743a 2073 7472   query_text: str
-00034260: 2c20 6d75 7374 2e0d 0a20 2020 2020 2020  , must...       
-00034270: 203a 7061 7261 6d20 6672 6f6d 5f6c 616e   :param from_lan
-00034280: 6775 6167 653a 2073 7472 2c20 6465 6661  guage: str, defa
-00034290: 756c 7420 2761 7574 6f27 2e0d 0a20 2020  ult 'auto'...   
-000342a0: 2020 2020 203a 7061 7261 6d20 746f 5f6c       :param to_l
-000342b0: 616e 6775 6167 653a 2073 7472 2c20 6465  anguage: str, de
-000342c0: 6661 756c 7420 2765 6e27 2e0d 0a20 2020  fault 'en'...   
-000342d0: 2020 2020 203a 7061 7261 6d20 2a2a 6b77       :param **kw
-000342e0: 6172 6773 3a0d 0a20 2020 2020 2020 2020  args:..         
-000342f0: 2020 2020 2020 203a 7061 7261 6d20 7469         :param ti
-00034300: 6d65 6f75 743a 2066 6c6f 6174 2c20 6465  meout: float, de
-00034310: 6661 756c 7420 4e6f 6e65 2e0d 0a20 2020  fault None...   
-00034320: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-00034330: 7261 6d20 7072 6f78 6965 733a 2064 6963  ram proxies: dic
-00034340: 742c 2064 6566 6175 6c74 204e 6f6e 652e  t, default None.
-00034350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00034360: 2020 3a70 6172 616d 2073 6c65 6570 5f73    :param sleep_s
-00034370: 6563 6f6e 6473 3a20 666c 6f61 742c 2064  econds: float, d
-00034380: 6566 6175 6c74 2030 2e0d 0a20 2020 2020  efault 0...     
-00034390: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-000343a0: 6d20 6973 5f64 6574 6169 6c5f 7265 7375  m is_detail_resu
-000343b0: 6c74 3a20 626f 6f6c 2c20 6465 6661 756c  lt: bool, defaul
-000343c0: 7420 4661 6c73 652e 0d0a 2020 2020 2020  t False...      
-000343d0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-000343e0: 2069 665f 6967 6e6f 7265 5f6c 696d 6974   if_ignore_limit
-000343f0: 5f6f 665f 6c65 6e67 7468 3a20 626f 6f6c  _of_length: bool
-00034400: 2c20 6465 6661 756c 7420 4661 6c73 652e  , default False.
-00034410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00034420: 2020 3a70 6172 616d 206c 696d 6974 5f6f    :param limit_o
-00034430: 665f 6c65 6e67 7468 3a20 696e 742c 2064  f_length: int, d
-00034440: 6566 6175 6c74 2032 3030 3030 2e0d 0a20  efault 20000... 
-00034450: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-00034460: 7061 7261 6d20 6966 5f69 676e 6f72 655f  param if_ignore_
-00034470: 656d 7074 795f 7175 6572 793a 2062 6f6f  empty_query: boo
-00034480: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-00034490: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000344a0: 2020 203a 7061 7261 6d20 7570 6461 7465     :param update
-000344b0: 5f73 6573 7369 6f6e 5f61 6674 6572 5f66  _session_after_f
-000344c0: 7265 713a 2069 6e74 2c20 6465 6661 756c  req: int, defaul
-000344d0: 7420 3130 3030 2e0d 0a20 2020 2020 2020  t 1000...       
-000344e0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-000344f0: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
-00034500: 6674 6572 5f73 6563 6f6e 6473 3a20 666c  fter_seconds: fl
-00034510: 6f61 742c 2064 6566 6175 6c74 2031 3530  oat, default 150
-00034520: 302e 0d0a 2020 2020 2020 2020 2020 2020  0...            
-00034530: 2020 2020 3a70 6172 616d 2069 665f 7368      :param if_sh
-00034540: 6f77 5f74 696d 655f 7374 6174 3a20 626f  ow_time_stat: bo
-00034550: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-00034560: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
-00034570: 2020 2020 3a70 6172 616d 2073 686f 775f      :param show_
-00034580: 7469 6d65 5f73 7461 745f 7072 6563 6973  time_stat_precis
-00034590: 696f 6e3a 2069 6e74 2c20 6465 6661 756c  ion: int, defaul
-000345a0: 7420 322e 0d0a 2020 2020 2020 2020 2020  t 2...          
-000345b0: 2020 2020 2020 3a70 6172 616d 2069 665f        :param if_
-000345c0: 7072 696e 745f 7761 726e 696e 673a 2062  print_warning: b
-000345d0: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
-000345e0: 652e 0d0a 2020 2020 2020 2020 3a72 6574  e...        :ret
-000345f0: 7572 6e3a 2073 7472 206f 7220 6469 6374  urn: str or dict
-00034600: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
-00034610: 0a20 2020 2020 2020 2074 696d 656f 7574  .        timeout
-00034620: 203d 206b 7761 7267 732e 6765 7428 2774   = kwargs.get('t
-00034630: 696d 656f 7574 272c 204e 6f6e 6529 0d0a  imeout', None)..
-00034640: 2020 2020 2020 2020 7072 6f78 6965 7320          proxies 
-00034650: 3d20 6b77 6172 6773 2e67 6574 2827 7072  = kwargs.get('pr
-00034660: 6f78 6965 7327 2c20 4e6f 6e65 290d 0a20  oxies', None).. 
-00034670: 2020 2020 2020 2073 6c65 6570 5f73 6563         sleep_sec
-00034680: 6f6e 6473 203d 206b 7761 7267 732e 6765  onds = kwargs.ge
-00034690: 7428 2773 6c65 6570 5f73 6563 6f6e 6473  t('sleep_seconds
-000346a0: 272c 2030 290d 0a20 2020 2020 2020 2069  ', 0)..        i
-000346b0: 665f 7072 696e 745f 7761 726e 696e 6720  f_print_warning 
-000346c0: 3d20 6b77 6172 6773 2e67 6574 2827 6966  = kwargs.get('if
-000346d0: 5f70 7269 6e74 5f77 6172 6e69 6e67 272c  _print_warning',
-000346e0: 2054 7275 6529 0d0a 2020 2020 2020 2020   True)..        
-000346f0: 6973 5f64 6574 6169 6c5f 7265 7375 6c74  is_detail_result
-00034700: 203d 206b 7761 7267 732e 6765 7428 2769   = kwargs.get('i
-00034710: 735f 6465 7461 696c 5f72 6573 756c 7427  s_detail_result'
-00034720: 2c20 4661 6c73 6529 0d0a 2020 2020 2020  , False)..      
-00034730: 2020 7570 6461 7465 5f73 6573 7369 6f6e    update_session
-00034740: 5f61 6674 6572 5f66 7265 7120 3d20 6b77  _after_freq = kw
-00034750: 6172 6773 2e67 6574 2827 7570 6461 7465  args.get('update
-00034760: 5f73 6573 7369 6f6e 5f61 6674 6572 5f66  _session_after_f
-00034770: 7265 7127 2c20 7365 6c66 2e64 6566 6175  req', self.defau
-00034780: 6c74 5f73 6573 7369 6f6e 5f66 7265 7129  lt_session_freq)
-00034790: 0d0a 2020 2020 2020 2020 7570 6461 7465  ..        update
-000347a0: 5f73 6573 7369 6f6e 5f61 6674 6572 5f73  _session_after_s
-000347b0: 6563 6f6e 6473 203d 206b 7761 7267 732e  econds = kwargs.
-000347c0: 6765 7428 2775 7064 6174 655f 7365 7373  get('update_sess
-000347d0: 696f 6e5f 6166 7465 725f 7365 636f 6e64  ion_after_second
-000347e0: 7327 2c20 7365 6c66 2e64 6566 6175 6c74  s', self.default
-000347f0: 5f73 6573 7369 6f6e 5f73 6563 6f6e 6473  _session_seconds
-00034800: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00034810: 6368 6563 6b5f 696e 7075 745f 6c69 6d69  check_input_limi
-00034820: 7428 7175 6572 795f 7465 7874 2c20 7365  t(query_text, se
-00034830: 6c66 2e69 6e70 7574 5f6c 696d 6974 290d  lf.input_limit).
-00034840: 0a0d 0a20 2020 2020 2020 206e 6f74 5f75  ...        not_u
-00034850: 7064 6174 655f 636f 6e64 5f66 7265 7120  pdate_cond_freq 
-00034860: 3d20 3120 6966 2073 656c 662e 7175 6572  = 1 if self.quer
-00034870: 795f 636f 756e 7420 3c20 7570 6461 7465  y_count < update
-00034880: 5f73 6573 7369 6f6e 5f61 6674 6572 5f66  _session_after_f
-00034890: 7265 7120 656c 7365 2030 0d0a 2020 2020  req else 0..    
-000348a0: 2020 2020 6e6f 745f 7570 6461 7465 5f63      not_update_c
-000348b0: 6f6e 645f 7469 6d65 203d 2031 2069 6620  ond_time = 1 if 
-000348c0: 7469 6d65 2e74 696d 6528 2920 2d20 7365  time.time() - se
-000348d0: 6c66 2e62 6567 696e 5f74 696d 6520 3c20  lf.begin_time < 
-000348e0: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
-000348f0: 6674 6572 5f73 6563 6f6e 6473 2065 6c73  fter_seconds els
-00034900: 6520 300d 0a20 2020 2020 2020 2069 6620  e 0..        if 
-00034910: 6e6f 7420 2873 656c 662e 7365 7373 696f  not (self.sessio
-00034920: 6e20 616e 6420 7365 6c66 2e6c 616e 6775  n and self.langu
-00034930: 6167 655f 6d61 7020 616e 6420 6e6f 745f  age_map and not_
-00034940: 7570 6461 7465 5f63 6f6e 645f 6672 6571  update_cond_freq
-00034950: 2061 6e64 206e 6f74 5f75 7064 6174 655f   and not_update_
-00034960: 636f 6e64 5f74 696d 6529 3a0d 0a20 2020  cond_time):..   
-00034970: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00034980: 7373 696f 6e20 3d20 7265 7175 6573 7473  ssion = requests
-00034990: 2e53 6573 7369 6f6e 2829 0d0a 2020 2020  .Session()..    
-000349a0: 2020 2020 2020 2020 5f20 3d20 7365 6c66          _ = self
-000349b0: 2e73 6573 7369 6f6e 2e67 6574 2873 656c  .session.get(sel
-000349c0: 662e 686f 7374 5f75 726c 2c20 6865 6164  f.host_url, head
-000349d0: 6572 733d 7365 6c66 2e68 6f73 745f 6865  ers=self.host_he
-000349e0: 6164 6572 732c 2074 696d 656f 7574 3d74  aders, timeout=t
-000349f0: 696d 656f 7574 2c20 7072 6f78 6965 733d  imeout, proxies=
-00034a00: 7072 6f78 6965 7329 0d0a 2020 2020 2020  proxies)..      
-00034a10: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
-00034a20: 675f 6461 7461 203d 2073 656c 662e 7365  g_data = self.se
-00034a30: 7373 696f 6e2e 6765 7428 7365 6c66 2e67  ssion.get(self.g
-00034a40: 6574 5f63 6f6e 6669 675f 7572 6c2c 2068  et_config_url, h
-00034a50: 6561 6465 7273 3d73 656c 662e 686f 7374  eaders=self.host
-00034a60: 5f68 6561 6465 7273 2c20 7469 6d65 6f75  _headers, timeou
-00034a70: 743d 7469 6d65 6f75 742c 2070 726f 7869  t=timeout, proxi
-00034a80: 6573 3d70 726f 7869 6573 292e 6a73 6f6e  es=proxies).json
-00034a90: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00034aa0: 7365 6c66 2e61 7069 5f68 6561 6465 7273  self.api_headers
-00034ab0: 2e75 7064 6174 6528 7b27 636c 6965 6e74  .update({'client
-00034ac0: 2d69 6427 3a20 7365 6c66 2e63 6f6e 6669  -id': self.confi
-00034ad0: 675f 6461 7461 5b27 6d74 275d 5b27 6170  g_data['mt']['ap
-00034ae0: 6927 5d5b 2763 6c69 656e 7449 6427 5d7d  i']['clientId']}
-00034af0: 2920 2023 206d 7573 7420 6c6f 7765 7220  )  # must lower 
-00034b00: 6b65 7977 6f72 640d 0a0d 0a20 2020 2020  keyword....     
-00034b10: 2020 2020 2020 2073 7973 5f75 726c 203d         sys_url =
-00034b20: 2073 656c 662e 636f 6e66 6967 5f64 6174   self.config_dat
-00034b30: 615b 276d 7427 5d5b 2761 7069 275d 5b27  a['mt']['api']['
-00034b40: 7379 7374 656d 4c69 7374 5572 6c27 5d0d  systemListUrl'].
-00034b50: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-00034b60: 616d 7320 3d20 7b27 6170 7049 4427 3a20  ams = {'appID': 
-00034b70: 7365 6c66 2e63 6f6e 6669 675f 6461 7461  self.config_data
-00034b80: 5b27 6d74 275d 5b27 6170 6927 5d5b 2761  ['mt']['api']['a
-00034b90: 7070 4944 275d 2c20 2775 694c 616e 6775  ppID'], 'uiLangu
-00034ba0: 6167 6549 4427 3a20 7365 6c66 2e63 6f6e  ageID': self.con
-00034bb0: 6669 675f 6461 7461 5b27 6d74 275d 5b27  fig_data['mt']['
-00034bc0: 6170 6927 5d5b 2775 694c 616e 6775 6167  api']['uiLanguag
-00034bd0: 6549 4427 5d7d 0d0a 2020 2020 2020 2020  eID']}..        
-00034be0: 2020 2020 7365 6c66 2e73 7973 5f64 6174      self.sys_dat
-00034bf0: 6120 3d20 7365 6c66 2e73 6573 7369 6f6e  a = self.session
-00034c00: 2e67 6574 2873 7973 5f75 726c 2c20 7061  .get(sys_url, pa
-00034c10: 7261 6d73 3d70 6172 616d 732c 2068 6561  rams=params, hea
-00034c20: 6465 7273 3d73 656c 662e 6170 695f 6865  ders=self.api_he
-00034c30: 6164 6572 732c 2074 696d 656f 7574 3d74  aders, timeout=t
-00034c40: 696d 656f 7574 2c20 7072 6f78 6965 733d  imeout, proxies=
-00034c50: 7072 6f78 6965 7329 2e6a 736f 6e28 2920  proxies).json() 
-00034c60: 2023 2074 6573 740d 0a20 2020 2020 2020   # test..       
-00034c70: 2020 2020 2073 656c 662e 6c61 6e67 7061       self.langpa
-00034c80: 6972 5f69 6473 203d 2073 656c 662e 6765  ir_ids = self.ge
-00034c90: 745f 6c61 6e67 7061 6972 5f69 6473 2873  t_langpair_ids(s
-00034ca0: 656c 662e 7379 735f 6461 7461 290d 0a20  elf.sys_data).. 
-00034cb0: 2020 2020 2020 2020 2020 2064 6562 7567             debug
-00034cc0: 5f6c 616e 675f 6b77 6172 6773 203d 2073  _lang_kwargs = s
-00034cd0: 656c 662e 6465 6275 675f 6c61 6e67 5f6b  elf.debug_lang_k
-00034ce0: 7761 7267 7328 6672 6f6d 5f6c 616e 6775  wargs(from_langu
-00034cf0: 6167 652c 2074 6f5f 6c61 6e67 7561 6765  age, to_language
-00034d00: 2c20 7365 6c66 2e64 6566 6175 6c74 5f66  , self.default_f
-00034d10: 726f 6d5f 6c61 6e67 7561 6765 2c20 6966  rom_language, if
-00034d20: 5f70 7269 6e74 5f77 6172 6e69 6e67 290d  _print_warning).
-00034d30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00034d40: 662e 6c61 6e67 7561 6765 5f6d 6170 203d  f.language_map =
-00034d50: 2073 656c 662e 6765 745f 6c61 6e67 7561   self.get_langua
-00034d60: 6765 5f6d 6170 2873 656c 662e 7379 735f  ge_map(self.sys_
-00034d70: 6461 7461 2c20 2a2a 6465 6275 675f 6c61  data, **debug_la
-00034d80: 6e67 5f6b 7761 7267 7329 0d0a 0d0a 2020  ng_kwargs)....  
-00034d90: 2020 2020 2020 6966 2066 726f 6d5f 6c61        if from_la
-00034da0: 6e67 7561 6765 203d 3d20 2761 7574 6f27  nguage == 'auto'
-00034db0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00034dc0: 726f 6d5f 6c61 6e67 7561 6765 203d 2073  rom_language = s
-00034dd0: 656c 662e 7761 726e 696e 675f 6175 746f  elf.warning_auto
-00034de0: 5f6c 616e 6728 2774 696c 6465 272c 2073  _lang('tilde', s
-00034df0: 656c 662e 6465 6661 756c 745f 6672 6f6d  elf.default_from
-00034e00: 5f6c 616e 6775 6167 652c 2069 665f 7072  _language, if_pr
-00034e10: 696e 745f 7761 726e 696e 6729 0d0a 2020  int_warning)..  
-00034e20: 2020 2020 2020 6672 6f6d 5f6c 616e 6775        from_langu
-00034e30: 6167 652c 2074 6f5f 6c61 6e67 7561 6765  age, to_language
-00034e40: 203d 2073 656c 662e 6368 6563 6b5f 6c61   = self.check_la
-00034e50: 6e67 7561 6765 2866 726f 6d5f 6c61 6e67  nguage(from_lang
-00034e60: 7561 6765 2c20 746f 5f6c 616e 6775 6167  uage, to_languag
-00034e70: 652c 2073 656c 662e 6c61 6e67 7561 6765  e, self.language
-00034e80: 5f6d 6170 290d 0a0d 0a20 2020 2020 2020  _map)....       
-00034e90: 2070 6179 6c6f 6164 203d 207b 0d0a 2020   payload = {..  
-00034ea0: 2020 2020 2020 2020 2020 2774 6578 7427            'text'
-00034eb0: 3a20 7175 6572 795f 7465 7874 2c0d 0a20  : query_text,.. 
-00034ec0: 2020 2020 2020 2020 2020 2027 6170 7049             'appI
-00034ed0: 4427 3a20 7365 6c66 2e63 6f6e 6669 675f  D': self.config_
-00034ee0: 6461 7461 5b27 6d74 275d 5b27 6170 6927  data['mt']['api'
-00034ef0: 5d5b 2761 7070 4944 275d 2c0d 0a20 2020  ]['appID'],..   
-00034f00: 2020 2020 2020 2020 2027 7379 7374 656d           'system
-00034f10: 4944 273a 2073 656c 662e 6c61 6e67 7061  ID': self.langpa
-00034f20: 6972 5f69 6473 5b66 277b 6672 6f6d 5f6c  ir_ids[f'{from_l
-00034f30: 616e 6775 6167 657d 2d7b 746f 5f6c 616e  anguage}-{to_lan
-00034f40: 6775 6167 657d 275d 2c0d 0a20 2020 2020  guage}'],..     
-00034f50: 2020 2020 2020 2027 6f70 7469 6f6e 7327         'options'
-00034f60: 3a20 2777 6964 6765 743d 7465 7874 2c61  : 'widget=text,a
-00034f70: 6c69 676e 6d65 6e74 2c6d 6172 6b53 656e  lignment,markSen
-00034f80: 7465 6e63 6573 272c 0d0a 2020 2020 2020  tences',..      
-00034f90: 2020 7d0d 0a20 2020 2020 2020 2072 203d    }..        r =
-00034fa0: 2073 656c 662e 7365 7373 696f 6e2e 706f   self.session.po
-00034fb0: 7374 2873 656c 662e 6170 695f 7572 6c2c  st(self.api_url,
-00034fc0: 206a 736f 6e3d 7061 796c 6f61 642c 2068   json=payload, h
-00034fd0: 6561 6465 7273 3d73 656c 662e 6170 695f  eaders=self.api_
-00034fe0: 6865 6164 6572 732c 2074 696d 656f 7574  headers, timeout
-00034ff0: 3d74 696d 656f 7574 2c20 7072 6f78 6965  =timeout, proxie
-00035000: 733d 7072 6f78 6965 7329 0d0a 2020 2020  s=proxies)..    
-00035010: 2020 2020 722e 7261 6973 655f 666f 725f      r.raise_for_
-00035020: 7374 6174 7573 2829 0d0a 2020 2020 2020  status()..      
-00035030: 2020 6461 7461 203d 2072 2e6a 736f 6e28    data = r.json(
-00035040: 290d 0a20 2020 2020 2020 2074 696d 652e  )..        time.
-00035050: 736c 6565 7028 736c 6565 705f 7365 636f  sleep(sleep_seco
-00035060: 6e64 7329 0d0a 2020 2020 2020 2020 7365  nds)..        se
-00035070: 6c66 2e71 7565 7279 5f63 6f75 6e74 202b  lf.query_count +
-00035080: 3d20 310d 0a20 2020 2020 2020 2072 6574  = 1..        ret
-00035090: 7572 6e20 6461 7461 2069 6620 6973 5f64  urn data if is_d
-000350a0: 6574 6169 6c5f 7265 7375 6c74 2065 6c73  etail_result els
-000350b0: 6520 6461 7461 5b27 7472 616e 736c 6174  e data['translat
-000350c0: 696f 6e27 5d0d 0a0d 0a0d 0a63 6c61 7373  ion']......class
-000350d0: 2043 6c6f 7564 5969 2854 7365 293a 0d0a   CloudYi(Tse):..
-000350e0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000350f0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00035100: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
-00035110: 5f28 290d 0a20 2020 2020 2020 2073 656c  _()..        sel
-00035120: 662e 686f 6d65 5f75 726c 203d 2027 6874  f.home_url = 'ht
-00035130: 7470 733a 2f2f 7777 772e 636c 6f75 6474  tps://www.cloudt
-00035140: 7261 6e73 6c61 7469 6f6e 2e63 6f6d 270d  ranslation.com'.
-00035150: 0a20 2020 2020 2020 2073 656c 662e 686f  .        self.ho
-00035160: 7374 5f75 726c 203d 2027 6874 7470 733a  st_url = 'https:
-00035170: 2f2f 7777 772e 636c 6f75 6474 7261 6e73  //www.cloudtrans
-00035180: 6c61 7469 6f6e 2e63 6f6d 2f23 2f74 7261  lation.com/#/tra
-00035190: 6e73 6c61 7465 270d 0a20 2020 2020 2020  nslate'..       
-000351a0: 2073 656c 662e 6170 695f 7572 6c20 3d20   self.api_url = 
-000351b0: 2768 7474 7073 3a2f 2f77 7777 2e63 6c6f  'https://www.clo
-000351c0: 7564 7472 616e 736c 6174 696f 6e2e 636f  udtranslation.co
-000351d0: 6d2f 6f66 6669 6369 616c 2d77 6562 7369  m/official-websi
-000351e0: 7465 2f76 312f 7472 616e 734f 6e65 5372  te/v1/transOneSr
-000351f0: 6354 6578 7427 0d0a 2020 2020 2020 2020  cText'..        
-00035200: 7365 6c66 2e67 6574 5f6c 616e 675f 7572  self.get_lang_ur
-00035210: 6c20 3d20 2768 7474 7073 3a2f 2f6f 6e6c  l = 'https://onl
-00035220: 696e 652e 636c 6f75 6474 7261 6e73 6c61  ine.cloudtransla
-00035230: 7469 6f6e 2e63 6f6d 2f61 7069 2f76 312e  tion.com/api/v1.
-00035240: 302f 7369 7465 2f67 6574 5f61 6c6c 5f6c  0/site/get_all_l
-00035250: 616e 6775 6167 655f 616e 645f 646f 6d61  anguage_and_doma
-00035260: 696e 270d 0a20 2020 2020 2020 2073 656c  in'..        sel
-00035270: 662e 6465 7465 6374 5f6c 616e 675f 7572  f.detect_lang_ur
-00035280: 6c20 3d20 2768 7474 7073 3a2f 2f6f 6e6c  l = 'https://onl
-00035290: 696e 652e 636c 6f75 6474 7261 6e73 6c61  ine.cloudtransla
-000352a0: 7469 6f6e 2e63 6f6d 2f61 7069 2f76 312e  tion.com/api/v1.
-000352b0: 302f 7265 7175 6573 745f 7472 616e 736c  0/request_transl
-000352c0: 6174 652f 6c61 6e67 6964 270d 0a20 2020  ate/langid'..   
-000352d0: 2020 2020 2073 656c 662e 6765 745f 636f       self.get_co
-000352e0: 6f6b 6965 5f75 726c 203d 2027 6874 7470  okie_url = 'http
-000352f0: 733a 2f2f 6f6e 6c69 6e65 2e63 6c6f 7564  s://online.cloud
-00035300: 7472 616e 736c 6174 696f 6e2e 636f 6d2f  translation.com/
-00035310: 6170 692f 7631 2e30 2f73 6974 652f 7369  api/v1.0/site/si
-00035320: 7465 735f 6c61 6e67 7561 6765 5f6c 6973  tes_language_lis
-00035330: 7427 0d0a 2020 2020 2020 2020 7365 6c66  t'..        self
-00035340: 2e68 6f73 745f 6865 6164 6572 7320 3d20  .host_headers = 
-00035350: 7365 6c66 2e67 6574 5f68 6561 6465 7273  self.get_headers
-00035360: 2873 656c 662e 686f 6d65 5f75 726c 2c20  (self.home_url, 
-00035370: 6966 5f61 7069 3d46 616c 7365 2c20 6966  if_api=False, if
-00035380: 5f72 6566 6572 6572 5f66 6f72 5f68 6f73  _referer_for_hos
-00035390: 743d 5472 7565 290d 0a20 2020 2020 2020  t=True)..       
-000353a0: 2073 656c 662e 6170 695f 6865 6164 6572   self.api_header
-000353b0: 7320 3d20 7365 6c66 2e67 6574 5f68 6561  s = self.get_hea
-000353c0: 6465 7273 2873 656c 662e 686f 6d65 5f75  ders(self.home_u
-000353d0: 726c 2c20 6966 5f61 7069 3d54 7275 652c  rl, if_api=True,
-000353e0: 2069 665f 6a73 6f6e 5f66 6f72 5f61 7069   if_json_for_api
-000353f0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-00035400: 7365 6c66 2e73 6573 7369 6f6e 203d 204e  self.session = N
-00035410: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
-00035420: 662e 6c61 6e67 7561 6765 5f6d 6170 203d  f.language_map =
-00035430: 204e 6f6e 650d 0a20 2020 2020 2020 2073   None..        s
-00035440: 656c 662e 6c61 6e67 7061 6972 5f64 6f6d  elf.langpair_dom
-00035450: 6169 6e20 3d20 4e6f 6e65 0d0a 2020 2020  ain = None..    
-00035460: 2020 2020 7365 6c66 2e70 726f 6665 7373      self.profess
-00035470: 696f 6e61 6c5f 6669 656c 6420 3d20 4e6f  ional_field = No
-00035480: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
-00035490: 2e71 7565 7279 5f63 6f75 6e74 203d 2030  .query_count = 0
-000354a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
-000354b0: 7574 7075 745f 7a68 203d 2027 7a68 2d63  utput_zh = 'zh-c
-000354c0: 6e27 0d0a 2020 2020 2020 2020 7365 6c66  n'..        self
-000354d0: 2e6f 7574 7075 745f 656e 203d 2027 656e  .output_en = 'en
-000354e0: 2d75 7327 0d0a 2020 2020 2020 2020 7365  -us'..        se
-000354f0: 6c66 2e6f 7574 7075 745f 6175 746f 203d  lf.output_auto =
-00035500: 2027 616c 6c27 0d0a 2020 2020 2020 2020   'all'..        
-00035510: 7365 6c66 2e69 6e70 7574 5f6c 696d 6974  self.input_limit
-00035520: 203d 2069 6e74 2835 6533 290d 0a20 2020   = int(5e3)..   
-00035530: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
-00035540: 745f 6672 6f6d 5f6c 616e 6775 6167 6520  t_from_language 
-00035550: 3d20 7365 6c66 2e6f 7574 7075 745f 7a68  = self.output_zh
-00035560: 0d0a 0d0a 2020 2020 4054 7365 2e64 6562  ....    @Tse.deb
-00035570: 7567 5f6c 616e 6775 6167 655f 6d61 700d  ug_language_map.
-00035580: 0a20 2020 2064 6566 2067 6574 5f6c 616e  .    def get_lan
-00035590: 6775 6167 655f 6d61 7028 7365 6c66 2c20  guage_map(self, 
-000355a0: 645f 6c61 6e67 5f6d 6170 3a20 6469 6374  d_lang_map: dict
-000355b0: 2c20 2a2a 6b77 6172 6773 3a20 4c61 6e67  , **kwargs: Lang
-000355c0: 4d61 704b 7761 7267 7354 7970 6529 202d  MapKwargsType) -
-000355d0: 3e20 6469 6374 3a0d 0a20 2020 2020 2020  > dict:..       
-000355e0: 2072 6574 7572 6e20 7b6b 3a20 5b69 745b   return {k: [it[
-000355f0: 276c 616e 6775 6167 655f 636f 6465 275d  'language_code']
-00035600: 2066 6f72 2069 7420 696e 2069 7465 6d5d   for it in item]
-00035610: 2066 6f72 206b 2c20 6974 656d 2069 6e20   for k, item in 
-00035620: 645f 6c61 6e67 5f6d 6170 5b27 6461 7461  d_lang_map['data
-00035630: 275d 5b27 7372 635f 746f 5f74 6774 275d  ']['src_to_tgt']
-00035640: 2e69 7465 6d73 2829 7d0d 0a0d 0a20 2020  .items()}....   
-00035650: 2064 6566 2067 6574 5f6c 616e 6770 6169   def get_langpai
-00035660: 725f 646f 6d61 696e 2873 656c 662c 2064  r_domain(self, d
-00035670: 5f6c 616e 675f 6d61 703a 2064 6963 7429  _lang_map: dict)
-00035680: 202d 3e20 6469 6374 3a0d 0a20 2020 2020   -> dict:..     
-00035690: 2020 2072 6574 7572 6e20 7b6b 3a20 5b69     return {k: [i
-000356a0: 745b 2764 6f6d 6169 6e5f 636f 6465 275d  t['domain_code']
-000356b0: 2066 6f72 2069 7420 696e 2069 7465 6d5d   for it in item]
-000356c0: 2066 6f72 206b 2c20 6974 656d 2069 6e20   for k, item in 
-000356d0: 645f 6c61 6e67 5f6d 6170 5b27 6461 7461  d_lang_map['data
-000356e0: 275d 5b27 6c61 6e67 7561 6765 5f70 6169  ']['language_pai
-000356f0: 725f 746f 5f64 6f6d 6169 6e27 5d2e 6974  r_to_domain'].it
-00035700: 656d 7328 297d 0d0a 0d0a 2020 2020 6465  ems()}....    de
-00035710: 6620 6765 745f 7072 6f66 6573 7369 6f6e  f get_profession
-00035720: 616c 5f66 6965 6c64 5f6c 6973 7428 7365  al_field_list(se
-00035730: 6c66 2c20 645f 6c61 6e67 5f6d 6170 3a20  lf, d_lang_map: 
-00035740: 6469 6374 2920 2d3e 2073 6574 3a0d 0a20  dict) -> set:.. 
-00035750: 2020 2020 2020 2072 6574 7572 6e20 7b69         return {i
-00035760: 745b 2764 6f6d 6169 6e5f 636f 6465 275d  t['domain_code']
-00035770: 2066 6f72 205f 2c20 6974 656d 2069 6e20   for _, item in 
-00035780: 645f 6c61 6e67 5f6d 6170 5b27 6461 7461  d_lang_map['data
-00035790: 275d 5b27 6c61 6e67 7561 6765 5f70 6169  ']['language_pai
-000357a0: 725f 746f 5f64 6f6d 6169 6e27 5d2e 6974  r_to_domain'].it
-000357b0: 656d 7328 2920 666f 7220 6974 2069 6e20  ems() for it in 
-000357c0: 6974 656d 7d0d 0a0d 0a20 2020 2040 5473  item}....    @Ts
-000357d0: 652e 7469 6d65 5f73 7461 740d 0a20 2020  e.time_stat..   
-000357e0: 2040 5473 652e 6368 6563 6b5f 7175 6572   @Tse.check_quer
-000357f0: 790d 0a20 2020 2064 6566 2063 6c6f 7564  y..    def cloud
-00035800: 5969 5f61 7069 2873 656c 662c 2071 7565  Yi_api(self, que
-00035810: 7279 5f74 6578 743a 2073 7472 2c20 6672  ry_text: str, fr
-00035820: 6f6d 5f6c 616e 6775 6167 653a 2073 7472  om_language: str
-00035830: 203d 2027 6175 746f 272c 2074 6f5f 6c61   = 'auto', to_la
-00035840: 6e67 7561 6765 3a20 7374 7220 3d20 2765  nguage: str = 'e
-00035850: 6e27 2c20 2a2a 6b77 6172 6773 3a20 4170  n', **kwargs: Ap
-00035860: 694b 7761 7267 7354 7970 6529 202d 3e20  iKwargsType) -> 
-00035870: 556e 696f 6e5b 7374 722c 2064 6963 745d  Union[str, dict]
-00035880: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00035890: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-000358a0: 7777 772e 636c 6f75 6474 7261 6e73 6c61  www.cloudtransla
-000358b0: 7469 6f6e 2e63 6f6d 2f23 2f74 7261 6e73  tion.com/#/trans
-000358c0: 6c61 7465 0d0a 2020 2020 2020 2020 3a70  late..        :p
-000358d0: 6172 616d 2071 7565 7279 5f74 6578 743a  aram query_text:
-000358e0: 2073 7472 2c20 6d75 7374 2e0d 0a20 2020   str, must...   
-000358f0: 2020 2020 203a 7061 7261 6d20 6672 6f6d       :param from
-00035900: 5f6c 616e 6775 6167 653a 2073 7472 2c20  _language: str, 
-00035910: 6465 6661 756c 7420 2761 7574 6f27 2e0d  default 'auto'..
-00035920: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00035930: 746f 5f6c 616e 6775 6167 653a 2073 7472  to_language: str
-00035940: 2c20 6465 6661 756c 7420 2765 6e27 2e0d  , default 'en'..
-00035950: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00035960: 2a2a 6b77 6172 6773 3a0d 0a20 2020 2020  **kwargs:..     
-00035970: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00035980: 6d20 7469 6d65 6f75 743a 2066 6c6f 6174  m timeout: float
-00035990: 2c20 6465 6661 756c 7420 4e6f 6e65 2e0d  , default None..
-000359a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000359b0: 203a 7061 7261 6d20 7072 6f78 6965 733a   :param proxies:
-000359c0: 2064 6963 742c 2064 6566 6175 6c74 204e   dict, default N
-000359d0: 6f6e 652e 0d0a 2020 2020 2020 2020 2020  one...          
-000359e0: 2020 2020 2020 3a70 6172 616d 2073 6c65        :param sle
-000359f0: 6570 5f73 6563 6f6e 6473 3a20 666c 6f61  ep_seconds: floa
-00035a00: 742c 2064 6566 6175 6c74 2030 2e0d 0a20  t, default 0... 
-00035a10: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-00035a20: 7061 7261 6d20 6973 5f64 6574 6169 6c5f  param is_detail_
-00035a30: 7265 7375 6c74 3a20 626f 6f6c 2c20 6465  result: bool, de
-00035a40: 6661 756c 7420 4661 6c73 652e 0d0a 2020  fault False...  
-00035a50: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-00035a60: 6172 616d 2069 665f 6967 6e6f 7265 5f6c  aram if_ignore_l
-00035a70: 696d 6974 5f6f 665f 6c65 6e67 7468 3a20  imit_of_length: 
-00035a80: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-00035a90: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
-00035aa0: 2020 2020 2020 3a70 6172 616d 206c 696d        :param lim
-00035ab0: 6974 5f6f 665f 6c65 6e67 7468 3a20 696e  it_of_length: in
-00035ac0: 742c 2064 6566 6175 6c74 2032 3030 3030  t, default 20000
-00035ad0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00035ae0: 2020 203a 7061 7261 6d20 6966 5f69 676e     :param if_ign
-00035af0: 6f72 655f 656d 7074 795f 7175 6572 793a  ore_empty_query:
-00035b00: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
-00035b10: 616c 7365 2e0d 0a20 2020 2020 2020 2020  alse...         
-00035b20: 2020 2020 2020 203a 7061 7261 6d20 7570         :param up
-00035b30: 6461 7465 5f73 6573 7369 6f6e 5f61 6674  date_session_aft
-00035b40: 6572 5f66 7265 713a 2069 6e74 2c20 6465  er_freq: int, de
-00035b50: 6661 756c 7420 3130 3030 2e0d 0a20 2020  fault 1000...   
-00035b60: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-00035b70: 7261 6d20 7570 6461 7465 5f73 6573 7369  ram update_sessi
-00035b80: 6f6e 5f61 6674 6572 5f73 6563 6f6e 6473  on_after_seconds
-00035b90: 3a20 666c 6f61 742c 2064 6566 6175 6c74  : float, default
-00035ba0: 2031 3530 302e 0d0a 2020 2020 2020 2020   1500...        
-00035bb0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-00035bc0: 665f 7368 6f77 5f74 696d 655f 7374 6174  f_show_time_stat
-00035bd0: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00035be0: 4661 6c73 652e 0d0a 2020 2020 2020 2020  False...        
-00035bf0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-00035c00: 686f 775f 7469 6d65 5f73 7461 745f 7072  how_time_stat_pr
-00035c10: 6563 6973 696f 6e3a 2069 6e74 2c20 6465  ecision: int, de
-00035c20: 6661 756c 7420 322e 0d0a 2020 2020 2020  fault 2...      
-00035c30: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00035c40: 2069 665f 7072 696e 745f 7761 726e 696e   if_print_warnin
-00035c50: 673a 2062 6f6f 6c2c 2064 6566 6175 6c74  g: bool, default
-00035c60: 2054 7275 652e 0d0a 2020 2020 2020 2020   True...        
-00035c70: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-00035c80: 726f 6665 7373 696f 6e61 6c5f 6669 656c  rofessional_fiel
-00035c90: 643a 2073 7472 2c20 6465 6661 756c 7420  d: str, default 
-00035ca0: 2767 656e 6572 616c 272e 0d0a 2020 2020  'general'...    
-00035cb0: 2020 2020 3a72 6574 7572 6e3a 2073 7472      :return: str
-00035cc0: 206f 7220 6469 6374 0d0a 2020 2020 2020   or dict..      
-00035cd0: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
-00035ce0: 2075 7365 5f64 6f6d 6169 6e20 3d20 6b77   use_domain = kw
-00035cf0: 6172 6773 2e67 6574 2827 7072 6f66 6573  args.get('profes
-00035d00: 7369 6f6e 616c 5f66 6965 6c64 272c 2027  sional_field', '
-00035d10: 6765 6e65 7261 6c27 290d 0a20 2020 2020  general')..     
-00035d20: 2020 2074 696d 656f 7574 203d 206b 7761     timeout = kwa
-00035d30: 7267 732e 6765 7428 2774 696d 656f 7574  rgs.get('timeout
-00035d40: 272c 204e 6f6e 6529 0d0a 2020 2020 2020  ', None)..      
-00035d50: 2020 7072 6f78 6965 7320 3d20 6b77 6172    proxies = kwar
-00035d60: 6773 2e67 6574 2827 7072 6f78 6965 7327  gs.get('proxies'
-00035d70: 2c20 4e6f 6e65 290d 0a20 2020 2020 2020  , None)..       
-00035d80: 2073 6c65 6570 5f73 6563 6f6e 6473 203d   sleep_seconds =
-00035d90: 206b 7761 7267 732e 6765 7428 2773 6c65   kwargs.get('sle
-00035da0: 6570 5f73 6563 6f6e 6473 272c 2030 290d  ep_seconds', 0).
-00035db0: 0a20 2020 2020 2020 2069 665f 7072 696e  .        if_prin
-00035dc0: 745f 7761 726e 696e 6720 3d20 6b77 6172  t_warning = kwar
-00035dd0: 6773 2e67 6574 2827 6966 5f70 7269 6e74  gs.get('if_print
-00035de0: 5f77 6172 6e69 6e67 272c 2054 7275 6529  _warning', True)
-00035df0: 0d0a 2020 2020 2020 2020 6973 5f64 6574  ..        is_det
-00035e00: 6169 6c5f 7265 7375 6c74 203d 206b 7761  ail_result = kwa
-00035e10: 7267 732e 6765 7428 2769 735f 6465 7461  rgs.get('is_deta
-00035e20: 696c 5f72 6573 756c 7427 2c20 4661 6c73  il_result', Fals
-00035e30: 6529 0d0a 2020 2020 2020 2020 7570 6461  e)..        upda
-00035e40: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
-00035e50: 5f66 7265 7120 3d20 6b77 6172 6773 2e67  _freq = kwargs.g
-00035e60: 6574 2827 7570 6461 7465 5f73 6573 7369  et('update_sessi
-00035e70: 6f6e 5f61 6674 6572 5f66 7265 7127 2c20  on_after_freq', 
-00035e80: 7365 6c66 2e64 6566 6175 6c74 5f73 6573  self.default_ses
-00035e90: 7369 6f6e 5f66 7265 7129 0d0a 2020 2020  sion_freq)..    
-00035ea0: 2020 2020 7570 6461 7465 5f73 6573 7369      update_sessi
-00035eb0: 6f6e 5f61 6674 6572 5f73 6563 6f6e 6473  on_after_seconds
-00035ec0: 203d 206b 7761 7267 732e 6765 7428 2775   = kwargs.get('u
-00035ed0: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
-00035ee0: 7465 725f 7365 636f 6e64 7327 2c20 7365  ter_seconds', se
-00035ef0: 6c66 2e64 6566 6175 6c74 5f73 6573 7369  lf.default_sessi
-00035f00: 6f6e 5f73 6563 6f6e 6473 290d 0a20 2020  on_seconds)..   
-00035f10: 2020 2020 2073 656c 662e 6368 6563 6b5f       self.check_
-00035f20: 696e 7075 745f 6c69 6d69 7428 7175 6572  input_limit(quer
-00035f30: 795f 7465 7874 2c20 7365 6c66 2e69 6e70  y_text, self.inp
-00035f40: 7574 5f6c 696d 6974 290d 0a0d 0a20 2020  ut_limit)....   
-00035f50: 2020 2020 206e 6f74 5f75 7064 6174 655f       not_update_
-00035f60: 636f 6e64 5f66 7265 7120 3d20 3120 6966  cond_freq = 1 if
-00035f70: 2073 656c 662e 7175 6572 795f 636f 756e   self.query_coun
-00035f80: 7420 3c20 7570 6461 7465 5f73 6573 7369  t < update_sessi
-00035f90: 6f6e 5f61 6674 6572 5f66 7265 7120 656c  on_after_freq el
-00035fa0: 7365 2030 0d0a 2020 2020 2020 2020 6e6f  se 0..        no
-00035fb0: 745f 7570 6461 7465 5f63 6f6e 645f 7469  t_update_cond_ti
-00035fc0: 6d65 203d 2031 2069 6620 7469 6d65 2e74  me = 1 if time.t
-00035fd0: 696d 6528 2920 2d20 7365 6c66 2e62 6567  ime() - self.beg
-00035fe0: 696e 5f74 696d 6520 3c20 7570 6461 7465  in_time < update
-00035ff0: 5f73 6573 7369 6f6e 5f61 6674 6572 5f73  _session_after_s
-00036000: 6563 6f6e 6473 2065 6c73 6520 300d 0a20  econds else 0.. 
-00036010: 2020 2020 2020 2069 6620 6e6f 7420 2873         if not (s
-00036020: 656c 662e 7365 7373 696f 6e20 616e 6420  elf.session and 
-00036030: 7365 6c66 2e6c 616e 6775 6167 655f 6d61  self.language_ma
-00036040: 7020 616e 6420 6e6f 745f 7570 6461 7465  p and not_update
-00036050: 5f63 6f6e 645f 6672 6571 2061 6e64 206e  _cond_freq and n
-00036060: 6f74 5f75 7064 6174 655f 636f 6e64 5f74  ot_update_cond_t
-00036070: 696d 6529 3a0d 0a20 2020 2020 2020 2020  ime):..         
-00036080: 2020 2073 656c 662e 7365 7373 696f 6e20     self.session 
-00036090: 3d20 7265 7175 6573 7473 2e53 6573 7369  = requests.Sessi
-000360a0: 6f6e 2829 0d0a 2020 2020 2020 2020 2020  on()..          
-000360b0: 2020 5f20 3d20 7365 6c66 2e73 6573 7369    _ = self.sessi
-000360c0: 6f6e 2e67 6574 2873 656c 662e 686f 7374  on.get(self.host
-000360d0: 5f75 726c 2c20 6865 6164 6572 733d 7365  _url, headers=se
-000360e0: 6c66 2e68 6f73 745f 6865 6164 6572 732c  lf.host_headers,
-000360f0: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
-00036100: 2c20 7072 6f78 6965 733d 7072 6f78 6965  , proxies=proxie
-00036110: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00036120: 5f20 3d20 7365 6c66 2e73 6573 7369 6f6e  _ = self.session
-00036130: 2e67 6574 2873 656c 662e 6765 745f 636f  .get(self.get_co
-00036140: 6f6b 6965 5f75 726c 2c20 6865 6164 6572  okie_url, header
-00036150: 733d 7365 6c66 2e61 7069 5f68 6561 6465  s=self.api_heade
-00036160: 7273 2c20 7469 6d65 6f75 743d 7469 6d65  rs, timeout=time
-00036170: 6f75 742c 2070 726f 7869 6573 3d70 726f  out, proxies=pro
-00036180: 7869 6573 290d 0a20 2020 2020 2020 2020  xies)..         
-00036190: 2020 2064 5f6c 616e 675f 6d61 7020 3d20     d_lang_map = 
-000361a0: 7365 6c66 2e73 6573 7369 6f6e 2e67 6574  self.session.get
-000361b0: 2873 656c 662e 6765 745f 6c61 6e67 5f75  (self.get_lang_u
-000361c0: 726c 2c20 6865 6164 6572 733d 7365 6c66  rl, headers=self
-000361d0: 2e61 7069 5f68 6561 6465 7273 2c20 7469  .api_headers, ti
-000361e0: 6d65 6f75 743d 7469 6d65 6f75 742c 2070  meout=timeout, p
-000361f0: 726f 7869 6573 3d70 726f 7869 6573 292e  roxies=proxies).
-00036200: 6a73 6f6e 2829 0d0a 2020 2020 2020 2020  json()..        
-00036210: 2020 2020 6465 6275 675f 6c61 6e67 5f6b      debug_lang_k
-00036220: 7761 7267 7320 3d20 7365 6c66 2e64 6562  wargs = self.deb
-00036230: 7567 5f6c 616e 675f 6b77 6172 6773 2866  ug_lang_kwargs(f
-00036240: 726f 6d5f 6c61 6e67 7561 6765 2c20 746f  rom_language, to
-00036250: 5f6c 616e 6775 6167 652c 2073 656c 662e  _language, self.
-00036260: 6465 6661 756c 745f 6672 6f6d 5f6c 616e  default_from_lan
-00036270: 6775 6167 652c 2069 665f 7072 696e 745f  guage, if_print_
-00036280: 7761 726e 696e 6729 0d0a 2020 2020 2020  warning)..      
-00036290: 2020 2020 2020 7365 6c66 2e6c 616e 6775        self.langu
-000362a0: 6167 655f 6d61 7020 3d20 7365 6c66 2e67  age_map = self.g
-000362b0: 6574 5f6c 616e 6775 6167 655f 6d61 7028  et_language_map(
-000362c0: 645f 6c61 6e67 5f6d 6170 2c20 2a2a 6465  d_lang_map, **de
-000362d0: 6275 675f 6c61 6e67 5f6b 7761 7267 7329  bug_lang_kwargs)
-000362e0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000362f0: 6c66 2e6c 616e 6770 6169 725f 646f 6d61  lf.langpair_doma
-00036300: 696e 203d 2073 656c 662e 6765 745f 6c61  in = self.get_la
-00036310: 6e67 7061 6972 5f64 6f6d 6169 6e28 645f  ngpair_domain(d_
-00036320: 6c61 6e67 5f6d 6170 290d 0a20 2020 2020  lang_map)..     
-00036330: 2020 2020 2020 2073 656c 662e 7072 6f66         self.prof
-00036340: 6573 7369 6f6e 616c 5f66 6965 6c64 203d  essional_field =
-00036350: 2073 656c 662e 6765 745f 7072 6f66 6573   self.get_profes
-00036360: 7369 6f6e 616c 5f66 6965 6c64 5f6c 6973  sional_field_lis
-00036370: 7428 645f 6c61 6e67 5f6d 6170 290d 0a0d  t(d_lang_map)...
-00036380: 0a20 2020 2020 2020 2069 6620 6672 6f6d  .        if from
-00036390: 5f6c 616e 6775 6167 6520 3d3d 2027 6175  _language == 'au
-000363a0: 746f 273a 0d0a 2020 2020 2020 2020 2020  to':..          
-000363b0: 2020 7061 796c 6f61 6420 3d20 7b27 7465    payload = {'te
-000363c0: 7874 273a 2071 7565 7279 5f74 6578 747d  xt': query_text}
-000363d0: 0d0a 2020 2020 2020 2020 2020 2020 7220  ..            r 
-000363e0: 3d20 7365 6c66 2e73 6573 7369 6f6e 2e70  = self.session.p
-000363f0: 6f73 7428 7365 6c66 2e64 6574 6563 745f  ost(self.detect_
-00036400: 6c61 6e67 5f75 726c 2c20 6a73 6f6e 3d70  lang_url, json=p
-00036410: 6179 6c6f 6164 2c20 6865 6164 6572 733d  ayload, headers=
-00036420: 7365 6c66 2e61 7069 5f68 6561 6465 7273  self.api_headers
-00036430: 2c20 7469 6d65 6f75 743d 7469 6d65 6f75  , timeout=timeou
-00036440: 742c 2070 726f 7869 6573 3d70 726f 7869  t, proxies=proxi
-00036450: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
-00036460: 2066 726f 6d5f 6c61 6e67 7561 6765 203d   from_language =
-00036470: 2072 2e6a 736f 6e28 295b 2764 6174 6127   r.json()['data'
-00036480: 5d5b 276c 616e 6775 6167 6527 5d0d 0a20  ]['language'].. 
-00036490: 2020 2020 2020 2066 726f 6d5f 6c61 6e67         from_lang
-000364a0: 7561 6765 2c20 746f 5f6c 616e 6775 6167  uage, to_languag
-000364b0: 6520 3d20 6672 6f6d 5f6c 616e 6775 6167  e = from_languag
-000364c0: 652e 6c6f 7765 7228 292c 2074 6f5f 6c61  e.lower(), to_la
-000364d0: 6e67 7561 6765 2e6c 6f77 6572 2829 2020  nguage.lower()  
-000364e0: 2320 6d75 7374 206c 6f77 6572 0d0a 2020  # must lower..  
-000364f0: 2020 2020 2020 6672 6f6d 5f6c 616e 6775        from_langu
-00036500: 6167 652c 2074 6f5f 6c61 6e67 7561 6765  age, to_language
-00036510: 203d 2073 656c 662e 6368 6563 6b5f 6c61   = self.check_la
-00036520: 6e67 7561 6765 2866 726f 6d5f 6c61 6e67  nguage(from_lang
-00036530: 7561 6765 2c20 746f 5f6c 616e 6775 6167  uage, to_languag
-00036540: 652c 2073 656c 662e 6c61 6e67 7561 6765  e, self.language
-00036550: 5f6d 6170 2c20 6f75 7470 7574 5f7a 683d  _map, output_zh=
-00036560: 7365 6c66 2e6f 7574 7075 745f 7a68 2c0d  self.output_zh,.
-00036570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00036580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000365a0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-000365b0: 5f65 6e5f 7472 616e 736c 6174 6f72 3d27  _en_translator='
-000365c0: 636c 6f75 6459 6927 2c20 6f75 7470 7574  cloudYi', output
-000365d0: 5f65 6e3d 7365 6c66 2e6f 7574 7075 745f  _en=self.output_
-000365e0: 656e 290d 0a0d 0a20 2020 2020 2020 2064  en)....        d
-000365f0: 6f6d 6169 6e73 203d 2073 656c 662e 6c61  omains = self.la
-00036600: 6e67 7061 6972 5f64 6f6d 6169 6e2e 6765  ngpair_domain.ge
-00036610: 7428 6627 7b66 726f 6d5f 6c61 6e67 7561  t(f'{from_langua
-00036620: 6765 7d5f 7b74 6f5f 6c61 6e67 7561 6765  ge}_{to_language
-00036630: 7d27 290d 0a20 2020 2020 2020 2069 6620  }')..        if 
-00036640: 6e6f 7420 646f 6d61 696e 733a 0d0a 2020  not domains:..  
-00036650: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00036660: 5472 616e 736c 6174 6f72 4572 726f 720d  TranslatorError.
-00036670: 0a20 2020 2020 2020 2069 6620 7573 655f  .        if use_
-00036680: 646f 6d61 696e 206e 6f74 2069 6e20 646f  domain not in do
-00036690: 6d61 696e 733a 0d0a 2020 2020 2020 2020  mains:..        
-000366a0: 2020 2020 7573 655f 646f 6d61 696e 203d      use_domain =
-000366b0: 2064 6f6d 6169 6e73 5b30 5d0d 0a0d 0a20   domains[0].... 
-000366c0: 2020 2020 2020 2070 6179 6c6f 6164 203d         payload =
-000366d0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-000366e0: 2774 6578 7427 3a20 7175 6572 795f 7465  'text': query_te
-000366f0: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
-00036700: 2027 646f 6d61 696e 273a 2075 7365 5f64   'domain': use_d
-00036710: 6f6d 6169 6e2c 0d0a 2020 2020 2020 2020  omain,..        
-00036720: 2020 2020 2773 7263 4c61 6e67 436f 6465      'srcLangCode
-00036730: 273a 2066 726f 6d5f 6c61 6e67 7561 6765  ': from_language
-00036740: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00036750: 7467 744c 616e 6743 6f64 6527 3a20 746f  tgtLangCode': to
-00036760: 5f6c 616e 6775 6167 652c 0d0a 2020 2020  _language,..    
-00036770: 2020 2020 7d0d 0a20 2020 2020 2020 2072      }..        r
-00036780: 203d 2073 656c 662e 7365 7373 696f 6e2e   = self.session.
-00036790: 706f 7374 2873 656c 662e 6170 695f 7572  post(self.api_ur
-000367a0: 6c2c 206a 736f 6e3d 7061 796c 6f61 642c  l, json=payload,
-000367b0: 2068 6561 6465 7273 3d73 656c 662e 6170   headers=self.ap
-000367c0: 695f 6865 6164 6572 732c 2074 696d 656f  i_headers, timeo
-000367d0: 7574 3d74 696d 656f 7574 2c20 7072 6f78  ut=timeout, prox
-000367e0: 6965 733d 7072 6f78 6965 7329 0d0a 2020  ies=proxies)..  
-000367f0: 2020 2020 2020 722e 7261 6973 655f 666f        r.raise_fo
-00036800: 725f 7374 6174 7573 2829 0d0a 2020 2020  r_status()..    
-00036810: 2020 2020 6461 7461 203d 2072 2e6a 736f      data = r.jso
-00036820: 6e28 290d 0a20 2020 2020 2020 2074 696d  n()..        tim
-00036830: 652e 736c 6565 7028 736c 6565 705f 7365  e.sleep(sleep_se
-00036840: 636f 6e64 7329 0d0a 2020 2020 2020 2020  conds)..        
-00036850: 7365 6c66 2e71 7565 7279 5f63 6f75 6e74  self.query_count
-00036860: 202b 3d20 310d 0a20 2020 2020 2020 2072   += 1..        r
-00036870: 6574 7572 6e20 6461 7461 2069 6620 6973  eturn data if is
-00036880: 5f64 6574 6169 6c5f 7265 7375 6c74 2065  _detail_result e
-00036890: 6c73 6520 6461 7461 5b27 6461 7461 275d  lse data['data']
-000368a0: 5b27 7472 616e 736c 6174 696f 6e27 5d0d  ['translation'].
-000368b0: 0a0d 0a0d 0a63 6c61 7373 2053 7973 5472  .....class SysTr
-000368c0: 616e 2854 7365 293a 0d0a 2020 2020 6465  an(Tse):..    de
-000368d0: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
-000368e0: 3a0d 0a20 2020 2020 2020 2073 7570 6572  :..        super
-000368f0: 2829 2e5f 5f69 6e69 745f 5f28 290d 0a20  ().__init__().. 
-00036900: 2020 2020 2020 2073 656c 662e 686f 6d65         self.home
-00036910: 5f75 726c 203d 2027 6874 7470 733a 2f2f  _url = 'https://
-00036920: 7777 772e 7379 7374 7261 6e2e 6e65 7427  www.systran.net'
-00036930: 0d0a 2020 2020 2020 2020 7365 6c66 2e68  ..        self.h
-00036940: 6f73 745f 7572 6c20 3d20 2768 7474 7073  ost_url = 'https
-00036950: 3a2f 2f77 7777 2e73 7973 7472 616e 2e6e  ://www.systran.n
-00036960: 6574 2f74 7261 6e73 6c61 7465 2f27 0d0a  et/translate/'..
-00036970: 2020 2020 2020 2020 7365 6c66 2e61 7069          self.api
-00036980: 5f75 726c 203d 2027 6874 7470 733a 2f2f  _url = 'https://
-00036990: 6170 692d 7472 616e 736c 6174 652e 7379  api-translate.sy
-000369a0: 7374 7261 6e2e 6e65 742f 7472 616e 736c  stran.net/transl
-000369b0: 6174 696f 6e2f 7465 7874 2f74 7261 6e73  ation/text/trans
-000369c0: 6c61 7465 270d 0a20 2020 2020 2020 2073  late'..        s
-000369d0: 656c 662e 6765 745f 6c61 6e67 5f75 726c  elf.get_lang_url
-000369e0: 203d 2027 6874 7470 733a 2f2f 6170 692d   = 'https://api-
-000369f0: 7472 616e 736c 6174 652e 7379 7374 7261  translate.systra
-00036a00: 6e2e 6e65 742f 7472 616e 736c 6174 696f  n.net/translatio
-00036a10: 6e2f 7375 7070 6f72 7465 644c 616e 6775  n/supportedLangu
-00036a20: 6167 6573 270d 0a20 2020 2020 2020 2073  ages'..        s
-00036a30: 656c 662e 6765 745f 746f 6b65 6e5f 7572  elf.get_token_ur
-00036a40: 6c20 3d20 2768 7474 7073 3a2f 2f74 7261  l = 'https://tra
-00036a50: 6e73 6c61 7465 2e73 7973 7472 616e 2e6e  nslate.systran.n
-00036a60: 6574 2f6f 6964 632f 746f 6b65 6e27 0d0a  et/oidc/token'..
-00036a70: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
-00036a80: 5f63 6c69 656e 745f 7572 6c20 3d20 2768  _client_url = 'h
-00036a90: 7474 7073 3a2f 2f77 7777 2e73 7973 7472  ttps://www.systr
-00036aa0: 616e 2e6e 6574 2f77 702d 636f 6e74 656e  an.net/wp-conten
-00036ab0: 742f 7468 656d 6573 2f73 7973 7472 616e  t/themes/systran
-00036ac0: 2f74 7261 6e73 6c61 746f 722f 6a73 2f74  /translator/js/t
-00036ad0: 7261 6e73 6c61 7465 426f 782e 6275 6e64  ranslateBox.bund
-00036ae0: 6c65 2e6a 7327 0d0a 2020 2020 2020 2020  le.js'..        
-00036af0: 7365 6c66 2e68 6f73 745f 6865 6164 6572  self.host_header
-00036b00: 7320 3d20 7365 6c66 2e67 6574 5f68 6561  s = self.get_hea
-00036b10: 6465 7273 2873 656c 662e 686f 6d65 5f75  ders(self.home_u
-00036b20: 726c 2c20 6966 5f61 7069 3d46 616c 7365  rl, if_api=False
-00036b30: 2c20 6966 5f72 6566 6572 6572 5f66 6f72  , if_referer_for
-00036b40: 5f68 6f73 743d 5472 7565 290d 0a20 2020  _host=True)..   
-00036b50: 2020 2020 2073 656c 662e 6170 695f 616a       self.api_aj
-00036b60: 6178 5f68 6561 6465 7273 203d 2073 656c  ax_headers = sel
-00036b70: 662e 6765 745f 6865 6164 6572 7328 7365  f.get_headers(se
-00036b80: 6c66 2e68 6f6d 655f 7572 6c2c 2069 665f  lf.home_url, if_
-00036b90: 6170 693d 5472 7565 2c20 6966 5f61 6a61  api=True, if_aja
-00036ba0: 785f 666f 725f 6170 693d 5472 7565 290d  x_for_api=True).
-00036bb0: 0a20 2020 2020 2020 2073 656c 662e 6170  .        self.ap
-00036bc0: 695f 6a73 6f6e 5f68 6561 6465 7273 203d  i_json_headers =
-00036bd0: 2073 656c 662e 6765 745f 6865 6164 6572   self.get_header
-00036be0: 7328 7365 6c66 2e68 6f6d 655f 7572 6c2c  s(self.home_url,
-00036bf0: 2069 665f 6170 693d 5472 7565 2c20 6966   if_api=True, if
-00036c00: 5f6a 736f 6e5f 666f 725f 6170 693d 5472  _json_for_api=Tr
-00036c10: 7565 290d 0a20 2020 2020 2020 2073 656c  ue)..        sel
-00036c20: 662e 7365 7373 696f 6e20 3d20 4e6f 6e65  f.session = None
-00036c30: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00036c40: 616e 6775 6167 655f 6d61 7020 3d20 4e6f  anguage_map = No
-00036c50: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
-00036c60: 2e70 726f 6665 7373 696f 6e61 6c5f 6669  .professional_fi
-00036c70: 656c 6420 3d20 4e6f 6e65 0d0a 2020 2020  eld = None..    
-00036c80: 2020 2020 7365 6c66 2e6c 616e 6770 6169      self.langpai
-00036c90: 725f 646f 6d61 696e 203d 204e 6f6e 650d  r_domain = None.
-00036ca0: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
-00036cb0: 6965 6e74 5f64 6174 6120 3d20 4e6f 6e65  ient_data = None
-00036cc0: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-00036cd0: 6f6b 656e 5f64 6174 6120 3d20 4e6f 6e65  oken_data = None
-00036ce0: 0d0a 2020 2020 2020 2020 7365 6c66 2e71  ..        self.q
-00036cf0: 7565 7279 5f63 6f75 6e74 203d 2030 0d0a  uery_count = 0..
-00036d00: 2020 2020 2020 2020 7365 6c66 2e6f 7574          self.out
-00036d10: 7075 745f 7a68 203d 2027 7a68 270d 0a20  put_zh = 'zh'.. 
-00036d20: 2020 2020 2020 2073 656c 662e 696e 7075         self.inpu
-00036d30: 745f 6c69 6d69 7420 3d20 696e 7428 3565  t_limit = int(5e
-00036d40: 3329 0d0a 2020 2020 2020 2020 7365 6c66  3)..        self
-00036d50: 2e64 6566 6175 6c74 5f66 726f 6d5f 6c61  .default_from_la
-00036d60: 6e67 7561 6765 203d 2073 656c 662e 6f75  nguage = self.ou
-00036d70: 7470 7574 5f7a 680d 0a0d 0a20 2020 2040  tput_zh....    @
-00036d80: 5473 652e 6465 6275 675f 6c61 6e67 7561  Tse.debug_langua
-00036d90: 6765 5f6d 6170 0d0a 2020 2020 6465 6620  ge_map..    def 
-00036da0: 6765 745f 6c61 6e67 7561 6765 5f6d 6170  get_language_map
-00036db0: 2873 656c 662c 2064 5f6c 616e 675f 6d61  (self, d_lang_ma
-00036dc0: 703a 2064 6963 742c 202a 2a6b 7761 7267  p: dict, **kwarg
-00036dd0: 733a 204c 616e 674d 6170 4b77 6172 6773  s: LangMapKwargs
-00036de0: 5479 7065 2920 2d3e 2064 6963 743a 0d0a  Type) -> dict:..
-00036df0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-00036e00: 6969 5b27 736f 7572 6365 275d 3a20 5b6a  ii['source']: [j
-00036e10: 6a5b 2774 6172 6765 7427 5d20 666f 7220  j['target'] for 
-00036e20: 6a6a 2069 6e20 645f 6c61 6e67 5f6d 6170  jj in d_lang_map
-00036e30: 5b27 6c61 6e67 7561 6765 5061 6972 7327  ['languagePairs'
-00036e40: 5d20 6966 206a 6a5b 2773 6f75 7263 6527  ] if jj['source'
-00036e50: 5d20 3d3d 2069 695b 2773 6f75 7263 6527  ] == ii['source'
-00036e60: 5d5d 2066 6f72 2069 6920 696e 2064 5f6c  ]] for ii in d_l
-00036e70: 616e 675f 6d61 705b 276c 616e 6775 6167  ang_map['languag
-00036e80: 6550 6169 7273 275d 7d0d 0a0d 0a20 2020  ePairs']}....   
-00036e90: 2064 6566 2067 6574 5f70 726f 6665 7373   def get_profess
-00036ea0: 696f 6e61 6c5f 6669 656c 645f 6c69 7374  ional_field_list
-00036eb0: 2873 656c 662c 2064 5f6c 616e 675f 6d61  (self, d_lang_ma
-00036ec0: 703a 2064 6963 7429 202d 3e20 7365 743a  p: dict) -> set:
-00036ed0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00036ee0: 207b 6974 5b27 7365 6c65 6374 6f72 7327   {it['selectors'
-00036ef0: 5d5b 2764 6f6d 6169 6e27 5d20 666f 7220  ]['domain'] for 
-00036f00: 6974 656d 2069 6e20 645f 6c61 6e67 5f6d  item in d_lang_m
-00036f10: 6170 5b27 6c61 6e67 7561 6765 5061 6972  ap['languagePair
-00036f20: 7327 5d20 666f 7220 6974 2069 6e20 6974  s'] for it in it
-00036f30: 656d 5b27 7072 6f66 696c 6573 275d 7d0d  em['profiles']}.
-00036f40: 0a0d 0a20 2020 2064 6566 2067 6574 5f6c  ...    def get_l
-00036f50: 616e 6770 6169 725f 646f 6d61 696e 2873  angpair_domain(s
-00036f60: 656c 662c 2064 5f6c 616e 675f 6d61 703a  elf, d_lang_map:
-00036f70: 2064 6963 7429 202d 3e20 6469 6374 3a0d   dict) -> dict:.
-00036f80: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00036f90: 7b0d 0a20 2020 2020 2020 2020 2020 2066  {..            f
-00036fa0: 277b 6974 656d 5b22 736f 7572 6365 225d  '{item["source"]
-00036fb0: 7d5f 5f7b 6974 656d 5b22 7461 7267 6574  }__{item["target
-00036fc0: 225d 7d5f 5f7b 6974 5b22 7365 6c65 6374  "]}__{it["select
-00036fd0: 6f72 7322 5d5b 2264 6f6d 6169 6e22 5d7d  ors"]["domain"]}
-00036fe0: 273a 207b 0d0a 2020 2020 2020 2020 2020  ': {..          
-00036ff0: 2020 2020 2020 2764 6f6d 6169 6e27 3a20        'domain': 
-00037000: 6974 5b22 7365 6c65 6374 6f72 7322 5d5b  it["selectors"][
-00037010: 2264 6f6d 6169 6e22 5d2c 0d0a 2020 2020  "domain"],..    
-00037020: 2020 2020 2020 2020 2020 2020 276f 776e              'own
-00037030: 6572 273a 2069 745b 2773 656c 6563 746f  er': it['selecto
-00037040: 7273 275d 5b27 6f77 6e65 7227 5d2c 0d0a  rs']['owner'],..
-00037050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00037060: 2773 697a 6527 3a20 6974 5b27 7365 6c65  'size': it['sele
-00037070: 6374 6f72 7327 5d5b 2773 697a 6527 5d2c  ctors']['size'],
-00037080: 0d0a 2020 2020 2020 2020 2020 2020 7d20  ..            } 
-00037090: 666f 7220 6974 656d 2069 6e20 645f 6c61  for item in d_la
-000370a0: 6e67 5f6d 6170 5b27 6c61 6e67 7561 6765  ng_map['language
-000370b0: 5061 6972 7327 5d20 666f 7220 6974 2069  Pairs'] for it i
-000370c0: 6e20 6974 656d 5b27 7072 6f66 696c 6573  n item['profiles
-000370d0: 275d 0d0a 2020 2020 2020 2020 7d0d 0a20  ']..        }.. 
-000370e0: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-000370f0: 7461 0d0a 0d0a 2020 2020 6465 6620 6765  ta....    def ge
-00037100: 745f 636c 6965 6e74 5f64 6174 6128 7365  t_client_data(se
-00037110: 6c66 2c20 636c 6965 6e74 5f75 726c 3a20  lf, client_url: 
-00037120: 7374 722c 2073 733a 2053 6573 7369 6f6e  str, ss: Session
-00037130: 5479 7065 2c20 6865 6164 6572 733a 2064  Type, headers: d
-00037140: 6963 742c 2074 696d 656f 7574 3a20 666c  ict, timeout: fl
-00037150: 6f61 742c 2070 726f 7869 6573 3a20 6469  oat, proxies: di
-00037160: 6374 2920 2d3e 2064 6963 743a 0d0a 2020  ct) -> dict:..  
-00037170: 2020 2020 2020 6a73 5f68 746d 6c20 3d20        js_html = 
-00037180: 7373 2e67 6574 2863 6c69 656e 745f 7572  ss.get(client_ur
-00037190: 6c2c 2068 6561 6465 7273 3d68 6561 6465  l, headers=heade
-000371a0: 7273 2c20 7469 6d65 6f75 743d 7469 6d65  rs, timeout=time
-000371b0: 6f75 742c 2070 726f 7869 6573 3d70 726f  out, proxies=pro
-000371c0: 7869 6573 292e 7465 7874 0d0a 2020 2020  xies).text..    
-000371d0: 2020 2020 7365 6172 6368 5f67 726f 7570      search_group
-000371e0: 7320 3d20 7265 2e63 6f6d 7069 6c65 2827  s = re.compile('
-000371f0: 2268 7474 7073 3a2f 2f74 7261 6e73 6c61  "https://transla
-00037200: 7465 2e73 7973 7472 616e 2e6e 6574 2f6f  te.systran.net/o
-00037210: 6964 6322 2c5c 5c77 3d22 282e 2a3f 2922  idc",\\w="(.*?)"
-00037220: 2c5c 5c77 3d22 282e 2a3f 2922 3b27 292e  ,\\w="(.*?)";').
-00037230: 7365 6172 6368 286a 735f 6874 6d6c 2920  search(js_html) 
-00037240: 2023 205c 5c77 7b31 7d20 3d3d 205c 5c77   # \\w{1} == \\w
-00037250: 0d0a 2020 2020 2020 2020 636c 6965 6e74  ..        client
-00037260: 5f64 6174 6120 3d20 7b0d 0a20 2020 2020  _data = {..     
-00037270: 2020 2020 2020 2027 6772 616e 745f 7479         'grant_ty
-00037280: 7065 273a 2027 636c 6965 6e74 5f63 7265  pe': 'client_cre
-00037290: 6465 6e74 6961 6c73 272c 0d0a 2020 2020  dentials',..    
-000372a0: 2020 2020 2020 2020 2763 6c69 656e 745f          'client_
-000372b0: 6964 273a 2073 6561 7263 685f 6772 6f75  id': search_grou
-000372c0: 7073 2e67 726f 7570 2831 292c 0d0a 2020  ps.group(1),..  
-000372d0: 2020 2020 2020 2020 2020 2763 6c69 656e            'clien
-000372e0: 745f 7365 6372 6574 273a 2073 6561 7263  t_secret': searc
-000372f0: 685f 6772 6f75 7073 2e67 726f 7570 2832  h_groups.group(2
-00037300: 292c 0d0a 2020 2020 2020 2020 7d0d 0a20  ),..        }.. 
-00037310: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
-00037320: 6965 6e74 5f64 6174 610d 0a0d 0a20 2020  ient_data....   
-00037330: 2040 5473 652e 7469 6d65 5f73 7461 740d   @Tse.time_stat.
-00037340: 0a20 2020 2040 5473 652e 6368 6563 6b5f  .    @Tse.check_
-00037350: 7175 6572 790d 0a20 2020 2064 6566 2073  query..    def s
-00037360: 7973 5472 616e 5f61 7069 2873 656c 662c  ysTran_api(self,
-00037370: 2071 7565 7279 5f74 6578 743a 2073 7472   query_text: str
-00037380: 2c20 6672 6f6d 5f6c 616e 6775 6167 653a  , from_language:
-00037390: 2073 7472 203d 2027 6175 746f 272c 2074   str = 'auto', t
-000373a0: 6f5f 6c61 6e67 7561 6765 3a20 7374 7220  o_language: str 
-000373b0: 3d20 2765 6e27 2c20 2a2a 6b77 6172 6773  = 'en', **kwargs
-000373c0: 3a20 4170 694b 7761 7267 7354 7970 6529  : ApiKwargsType)
-000373d0: 202d 3e20 556e 696f 6e5b 7374 722c 2064   -> Union[str, d
-000373e0: 6963 745d 3a0d 0a20 2020 2020 2020 2022  ict]:..        "
-000373f0: 2222 0d0a 2020 2020 2020 2020 6874 7470  ""..        http
-00037400: 733a 2f2f 7777 772e 7379 7374 7261 6e2e  s://www.systran.
-00037410: 6e65 742f 7472 616e 736c 6174 652f 0d0a  net/translate/..
-00037420: 2020 2020 2020 2020 3a70 6172 616d 2071          :param q
-00037430: 7565 7279 5f74 6578 743a 2073 7472 2c20  uery_text: str, 
-00037440: 6d75 7374 2e0d 0a20 2020 2020 2020 203a  must...        :
-00037450: 7061 7261 6d20 6672 6f6d 5f6c 616e 6775  param from_langu
-00037460: 6167 653a 2073 7472 2c20 6465 6661 756c  age: str, defaul
-00037470: 7420 2761 7574 6f27 2e0d 0a20 2020 2020  t 'auto'...     
-00037480: 2020 203a 7061 7261 6d20 746f 5f6c 616e     :param to_lan
-00037490: 6775 6167 653a 2073 7472 2c20 6465 6661  guage: str, defa
-000374a0: 756c 7420 2765 6e27 2e0d 0a20 2020 2020  ult 'en'...     
-000374b0: 2020 203a 7061 7261 6d20 2a2a 6b77 6172     :param **kwar
-000374c0: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
-000374d0: 2020 2020 203a 7061 7261 6d20 7469 6d65       :param time
-000374e0: 6f75 743a 2066 6c6f 6174 2c20 6465 6661  out: float, defa
-000374f0: 756c 7420 4e6f 6e65 2e0d 0a20 2020 2020  ult None...     
-00037500: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00037510: 6d20 7072 6f78 6965 733a 2064 6963 742c  m proxies: dict,
-00037520: 2064 6566 6175 6c74 204e 6f6e 652e 0d0a   default None...
-00037530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00037540: 3a70 6172 616d 2073 6c65 6570 5f73 6563  :param sleep_sec
-00037550: 6f6e 6473 3a20 666c 6f61 742c 2064 6566  onds: float, def
-00037560: 6175 6c74 2030 2e0d 0a20 2020 2020 2020  ault 0...       
-00037570: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00037580: 6973 5f64 6574 6169 6c5f 7265 7375 6c74  is_detail_result
-00037590: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-000375a0: 4661 6c73 652e 0d0a 2020 2020 2020 2020  False...        
-000375b0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-000375c0: 665f 6967 6e6f 7265 5f6c 696d 6974 5f6f  f_ignore_limit_o
-000375d0: 665f 6c65 6e67 7468 3a20 626f 6f6c 2c20  f_length: bool, 
-000375e0: 6465 6661 756c 7420 4661 6c73 652e 0d0a  default False...
-000375f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00037600: 3a70 6172 616d 206c 696d 6974 5f6f 665f  :param limit_of_
-00037610: 6c65 6e67 7468 3a20 696e 742c 2064 6566  length: int, def
-00037620: 6175 6c74 2032 3030 3030 2e0d 0a20 2020  ault 20000...   
-00037630: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-00037640: 7261 6d20 6966 5f69 676e 6f72 655f 656d  ram if_ignore_em
-00037650: 7074 795f 7175 6572 793a 2062 6f6f 6c2c  pty_query: bool,
-00037660: 2064 6566 6175 6c74 2046 616c 7365 2e0d   default False..
-00037670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00037680: 203a 7061 7261 6d20 7570 6461 7465 5f73   :param update_s
-00037690: 6573 7369 6f6e 5f61 6674 6572 5f66 7265  ession_after_fre
-000376a0: 713a 2069 6e74 2c20 6465 6661 756c 7420  q: int, default 
-000376b0: 3130 3030 2e0d 0a20 2020 2020 2020 2020  1000...         
-000376c0: 2020 2020 2020 203a 7061 7261 6d20 7570         :param up
-000376d0: 6461 7465 5f73 6573 7369 6f6e 5f61 6674  date_session_aft
-000376e0: 6572 5f73 6563 6f6e 6473 3a20 666c 6f61  er_seconds: floa
-000376f0: 742c 2064 6566 6175 6c74 2031 3530 302e  t, default 1500.
-00037700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00037710: 2020 3a70 6172 616d 2069 665f 7368 6f77    :param if_show
-00037720: 5f74 696d 655f 7374 6174 3a20 626f 6f6c  _time_stat: bool
-00037730: 2c20 6465 6661 756c 7420 4661 6c73 652e  , default False.
-00037740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00037750: 2020 3a70 6172 616d 2073 686f 775f 7469    :param show_ti
-00037760: 6d65 5f73 7461 745f 7072 6563 6973 696f  me_stat_precisio
-00037770: 6e3a 2069 6e74 2c20 6465 6661 756c 7420  n: int, default 
-00037780: 322e 0d0a 2020 2020 2020 2020 2020 2020  2...            
-00037790: 2020 2020 3a70 6172 616d 2069 665f 7072      :param if_pr
-000377a0: 696e 745f 7761 726e 696e 673a 2062 6f6f  int_warning: boo
-000377b0: 6c2c 2064 6566 6175 6c74 2054 7275 652e  l, default True.
-000377c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000377d0: 2020 3a70 6172 616d 2070 726f 6665 7373    :param profess
-000377e0: 696f 6e61 6c5f 6669 656c 643a 2073 7472  ional_field: str
-000377f0: 2c20 6465 6661 756c 7420 4e6f 6e65 2e0d  , default None..
-00037800: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00037810: 3a20 7374 7220 6f72 2064 6963 740d 0a20  : str or dict.. 
-00037820: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
-00037830: 2020 2020 2020 7573 655f 646f 6d61 696e        use_domain
-00037840: 203d 206b 7761 7267 732e 6765 7428 2770   = kwargs.get('p
-00037850: 726f 6665 7373 696f 6e61 6c5f 6669 656c  rofessional_fiel
-00037860: 6427 2c20 2747 656e 6572 6963 2729 0d0a  d', 'Generic')..
-00037870: 2020 2020 2020 2020 7469 6d65 6f75 7420          timeout 
-00037880: 3d20 6b77 6172 6773 2e67 6574 2827 7469  = kwargs.get('ti
-00037890: 6d65 6f75 7427 2c20 4e6f 6e65 290d 0a20  meout', None).. 
-000378a0: 2020 2020 2020 2070 726f 7869 6573 203d         proxies =
-000378b0: 206b 7761 7267 732e 6765 7428 2770 726f   kwargs.get('pro
-000378c0: 7869 6573 272c 204e 6f6e 6529 0d0a 2020  xies', None)..  
-000378d0: 2020 2020 2020 736c 6565 705f 7365 636f        sleep_seco
-000378e0: 6e64 7320 3d20 6b77 6172 6773 2e67 6574  nds = kwargs.get
-000378f0: 2827 736c 6565 705f 7365 636f 6e64 7327  ('sleep_seconds'
-00037900: 2c20 3029 0d0a 2020 2020 2020 2020 6966  , 0)..        if
-00037910: 5f70 7269 6e74 5f77 6172 6e69 6e67 203d  _print_warning =
-00037920: 206b 7761 7267 732e 6765 7428 2769 665f   kwargs.get('if_
-00037930: 7072 696e 745f 7761 726e 696e 6727 2c20  print_warning', 
-00037940: 5472 7565 290d 0a20 2020 2020 2020 2069  True)..        i
-00037950: 735f 6465 7461 696c 5f72 6573 756c 7420  s_detail_result 
-00037960: 3d20 6b77 6172 6773 2e67 6574 2827 6973  = kwargs.get('is
-00037970: 5f64 6574 6169 6c5f 7265 7375 6c74 272c  _detail_result',
-00037980: 2046 616c 7365 290d 0a20 2020 2020 2020   False)..       
-00037990: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
-000379a0: 6166 7465 725f 6672 6571 203d 206b 7761  after_freq = kwa
-000379b0: 7267 732e 6765 7428 2775 7064 6174 655f  rgs.get('update_
-000379c0: 7365 7373 696f 6e5f 6166 7465 725f 6672  session_after_fr
-000379d0: 6571 272c 2073 656c 662e 6465 6661 756c  eq', self.defaul
-000379e0: 745f 7365 7373 696f 6e5f 6672 6571 290d  t_session_freq).
-000379f0: 0a20 2020 2020 2020 2075 7064 6174 655f  .        update_
-00037a00: 7365 7373 696f 6e5f 6166 7465 725f 7365  session_after_se
-00037a10: 636f 6e64 7320 3d20 6b77 6172 6773 2e67  conds = kwargs.g
-00037a20: 6574 2827 7570 6461 7465 5f73 6573 7369  et('update_sessi
-00037a30: 6f6e 5f61 6674 6572 5f73 6563 6f6e 6473  on_after_seconds
-00037a40: 272c 2073 656c 662e 6465 6661 756c 745f  ', self.default_
-00037a50: 7365 7373 696f 6e5f 7365 636f 6e64 7329  session_seconds)
-00037a60: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-00037a70: 6865 636b 5f69 6e70 7574 5f6c 696d 6974  heck_input_limit
-00037a80: 2871 7565 7279 5f74 6578 742c 2073 656c  (query_text, sel
-00037a90: 662e 696e 7075 745f 6c69 6d69 7429 0d0a  f.input_limit)..
-00037aa0: 0d0a 2020 2020 2020 2020 6e6f 745f 7570  ..        not_up
-00037ab0: 6461 7465 5f63 6f6e 645f 6672 6571 203d  date_cond_freq =
-00037ac0: 2031 2069 6620 7365 6c66 2e71 7565 7279   1 if self.query
-00037ad0: 5f63 6f75 6e74 203c 2075 7064 6174 655f  _count < update_
-00037ae0: 7365 7373 696f 6e5f 6166 7465 725f 6672  session_after_fr
-00037af0: 6571 2065 6c73 6520 300d 0a20 2020 2020  eq else 0..     
-00037b00: 2020 206e 6f74 5f75 7064 6174 655f 636f     not_update_co
-00037b10: 6e64 5f74 696d 6520 3d20 3120 6966 2074  nd_time = 1 if t
-00037b20: 696d 652e 7469 6d65 2829 202d 2073 656c  ime.time() - sel
-00037b30: 662e 6265 6769 6e5f 7469 6d65 203c 2075  f.begin_time < u
-00037b40: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
-00037b50: 7465 725f 7365 636f 6e64 7320 656c 7365  ter_seconds else
-00037b60: 2030 0d0a 2020 2020 2020 2020 6966 206e   0..        if n
-00037b70: 6f74 2028 7365 6c66 2e73 6573 7369 6f6e  ot (self.session
-00037b80: 2061 6e64 2073 656c 662e 6c61 6e67 7561   and self.langua
-00037b90: 6765 5f6d 6170 2061 6e64 206e 6f74 5f75  ge_map and not_u
-00037ba0: 7064 6174 655f 636f 6e64 5f66 7265 7120  pdate_cond_freq 
-00037bb0: 616e 6420 6e6f 745f 7570 6461 7465 5f63  and not_update_c
-00037bc0: 6f6e 645f 7469 6d65 293a 0d0a 2020 2020  ond_time):..    
-00037bd0: 2020 2020 2020 2020 7365 6c66 2e73 6573          self.ses
-00037be0: 7369 6f6e 203d 2072 6571 7565 7374 732e  sion = requests.
-00037bf0: 5365 7373 696f 6e28 290d 0a20 2020 2020  Session()..     
-00037c00: 2020 2020 2020 205f 203d 2073 656c 662e         _ = self.
-00037c10: 7365 7373 696f 6e2e 6765 7428 7365 6c66  session.get(self
-00037c20: 2e68 6f73 745f 7572 6c2c 2068 6561 6465  .host_url, heade
-00037c30: 7273 3d73 656c 662e 686f 7374 5f68 6561  rs=self.host_hea
-00037c40: 6465 7273 2c20 7469 6d65 6f75 743d 7469  ders, timeout=ti
-00037c50: 6d65 6f75 742c 2070 726f 7869 6573 3d70  meout, proxies=p
-00037c60: 726f 7869 6573 290d 0a20 2020 2020 2020  roxies)..       
-00037c70: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-00037c80: 5f64 6174 6120 3d20 7365 6c66 2e67 6574  _data = self.get
-00037c90: 5f63 6c69 656e 745f 6461 7461 2873 656c  _client_data(sel
-00037ca0: 662e 6765 745f 636c 6965 6e74 5f75 726c  f.get_client_url
-00037cb0: 2c20 7365 6c66 2e73 6573 7369 6f6e 2c20  , self.session, 
-00037cc0: 7365 6c66 2e68 6f73 745f 6865 6164 6572  self.host_header
-00037cd0: 732c 2074 696d 656f 7574 2c20 7072 6f78  s, timeout, prox
-00037ce0: 6965 7329 0d0a 2020 2020 2020 2020 2020  ies)..          
-00037cf0: 2020 7061 796c 6f61 6420 3d20 7572 6c6c    payload = urll
-00037d00: 6962 2e70 6172 7365 2e75 726c 656e 636f  ib.parse.urlenco
-00037d10: 6465 2873 656c 662e 636c 6965 6e74 5f64  de(self.client_d
-00037d20: 6174 6129 0d0a 2020 2020 2020 2020 2020  ata)..          
-00037d30: 2020 7365 6c66 2e74 6f6b 656e 5f64 6174    self.token_dat
-00037d40: 6120 3d20 7365 6c66 2e73 6573 7369 6f6e  a = self.session
-00037d50: 2e70 6f73 7428 7365 6c66 2e67 6574 5f74  .post(self.get_t
-00037d60: 6f6b 656e 5f75 726c 2c20 6461 7461 3d70  oken_url, data=p
-00037d70: 6179 6c6f 6164 2c20 6865 6164 6572 733d  ayload, headers=
-00037d80: 7365 6c66 2e61 7069 5f61 6a61 785f 6865  self.api_ajax_he
-00037d90: 6164 6572 732c 2074 696d 656f 7574 3d74  aders, timeout=t
-00037da0: 696d 656f 7574 2c20 7072 6f78 6965 733d  imeout, proxies=
-00037db0: 7072 6f78 6965 7329 2e6a 736f 6e28 290d  proxies).json().
-00037dc0: 0a0d 0a20 2020 2020 2020 2020 2020 2068  ...            h
-00037dd0: 6561 6465 725f 7061 7261 6d73 203d 207b  eader_params = {
-00037de0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00037df0: 2020 2761 7574 686f 7269 7a61 7469 6f6e    'authorization
-00037e00: 273a 2066 277b 7365 6c66 2e74 6f6b 656e  ': f'{self.token
-00037e10: 5f64 6174 615b 2274 6f6b 656e 5f74 7970  _data["token_typ
-00037e20: 6522 5d7d 207b 7365 6c66 2e74 6f6b 656e  e"]} {self.token
-00037e30: 5f64 6174 615b 2261 6363 6573 735f 746f  _data["access_to
-00037e40: 6b65 6e22 5d7d 272c 0d0a 2020 2020 2020  ken"]}',..      
-00037e50: 2020 2020 2020 2020 2020 2778 2d75 7365            'x-use
-00037e60: 722d 6167 656e 7427 3a20 2746 696c 6520  r-agent': 'File 
-00037e70: 5472 616e 736c 6174 6520 426f 7820 506f  Translate Box Po
-00037e80: 7274 6162 6c65 272c 0d0a 2020 2020 2020  rtable',..      
-00037e90: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-00037ea0: 2020 2020 2073 656c 662e 6170 695f 6a73       self.api_js
-00037eb0: 6f6e 5f68 6561 6465 7273 2e75 7064 6174  on_headers.updat
-00037ec0: 6528 6865 6164 6572 5f70 6172 616d 7329  e(header_params)
-00037ed0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00037ee0: 645f 6c61 6e67 5f6d 6170 203d 2073 656c  d_lang_map = sel
-00037ef0: 662e 7365 7373 696f 6e2e 6765 7428 7365  f.session.get(se
-00037f00: 6c66 2e67 6574 5f6c 616e 675f 7572 6c2c  lf.get_lang_url,
-00037f10: 2068 6561 6465 7273 3d73 656c 662e 6170   headers=self.ap
-00037f20: 695f 6a73 6f6e 5f68 6561 6465 7273 2c20  i_json_headers, 
-00037f30: 7469 6d65 6f75 743d 7469 6d65 6f75 742c  timeout=timeout,
-00037f40: 2070 726f 7869 6573 3d70 726f 7869 6573   proxies=proxies
-00037f50: 292e 6a73 6f6e 2829 0d0a 2020 2020 2020  ).json()..      
-00037f60: 2020 2020 2020 6465 6275 675f 6c61 6e67        debug_lang
-00037f70: 5f6b 7761 7267 7320 3d20 7365 6c66 2e64  _kwargs = self.d
-00037f80: 6562 7567 5f6c 616e 675f 6b77 6172 6773  ebug_lang_kwargs
-00037f90: 2866 726f 6d5f 6c61 6e67 7561 6765 2c20  (from_language, 
-00037fa0: 746f 5f6c 616e 6775 6167 652c 2073 656c  to_language, sel
-00037fb0: 662e 6465 6661 756c 745f 6672 6f6d 5f6c  f.default_from_l
-00037fc0: 616e 6775 6167 652c 2069 665f 7072 696e  anguage, if_prin
-00037fd0: 745f 7761 726e 696e 6729 0d0a 2020 2020  t_warning)..    
-00037fe0: 2020 2020 2020 2020 7365 6c66 2e6c 616e          self.lan
-00037ff0: 6775 6167 655f 6d61 7020 3d20 7365 6c66  guage_map = self
-00038000: 2e67 6574 5f6c 616e 6775 6167 655f 6d61  .get_language_ma
-00038010: 7028 645f 6c61 6e67 5f6d 6170 2c20 2a2a  p(d_lang_map, **
-00038020: 6465 6275 675f 6c61 6e67 5f6b 7761 7267  debug_lang_kwarg
-00038030: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00038040: 7365 6c66 2e70 726f 6665 7373 696f 6e61  self.professiona
-00038050: 6c5f 6669 656c 6420 3d20 7365 6c66 2e67  l_field = self.g
-00038060: 6574 5f70 726f 6665 7373 696f 6e61 6c5f  et_professional_
-00038070: 6669 656c 645f 6c69 7374 2864 5f6c 616e  field_list(d_lan
-00038080: 675f 6d61 7029 0d0a 2020 2020 2020 2020  g_map)..        
-00038090: 2020 2020 7365 6c66 2e6c 616e 6770 6169      self.langpai
-000380a0: 725f 646f 6d61 696e 203d 2073 656c 662e  r_domain = self.
-000380b0: 6765 745f 6c61 6e67 7061 6972 5f64 6f6d  get_langpair_dom
-000380c0: 6169 6e28 645f 6c61 6e67 5f6d 6170 290d  ain(d_lang_map).
-000380d0: 0a0d 0a20 2020 2020 2020 2066 726f 6d5f  ...        from_
-000380e0: 6c61 6e67 7561 6765 2c20 746f 5f6c 616e  language, to_lan
-000380f0: 6775 6167 6520 3d20 7365 6c66 2e63 6865  guage = self.che
-00038100: 636b 5f6c 616e 6775 6167 6528 6672 6f6d  ck_language(from
-00038110: 5f6c 616e 6775 6167 652c 2074 6f5f 6c61  _language, to_la
-00038120: 6e67 7561 6765 2c20 7365 6c66 2e6c 616e  nguage, self.lan
-00038130: 6775 6167 655f 6d61 702c 206f 7574 7075  guage_map, outpu
-00038140: 745f 7a68 3d73 656c 662e 6f75 7470 7574  t_zh=self.output
-00038150: 5f7a 6829 0d0a 2020 2020 2020 2020 6966  _zh)..        if
-00038160: 2066 726f 6d5f 6c61 6e67 7561 6765 203d   from_language =
-00038170: 3d20 2761 7574 6f27 3a0d 0a20 2020 2020  = 'auto':..     
-00038180: 2020 2020 2020 2066 726f 6d5f 6c61 6e67         from_lang
-00038190: 7561 6765 203d 2073 656c 662e 7761 726e  uage = self.warn
-000381a0: 696e 675f 6175 746f 5f6c 616e 6728 2773  ing_auto_lang('s
-000381b0: 7973 5472 616e 272c 2073 656c 662e 6465  ysTran', self.de
-000381c0: 6661 756c 745f 6672 6f6d 5f6c 616e 6775  fault_from_langu
-000381d0: 6167 652c 2069 665f 7072 696e 745f 7761  age, if_print_wa
-000381e0: 726e 696e 6729 0d0a 0d0a 2020 2020 2020  rning)....      
-000381f0: 2020 7061 796c 6f61 6420 3d20 7b0d 0a20    payload = {.. 
-00038200: 2020 2020 2020 2020 2020 2027 7461 7267             'targ
-00038210: 6574 273a 2074 6f5f 6c61 6e67 7561 6765  et': to_language
-00038220: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00038230: 736f 7572 6365 273a 2066 726f 6d5f 6c61  source': from_la
-00038240: 6e67 7561 6765 2069 6620 6672 6f6d 5f6c  nguage if from_l
-00038250: 616e 6775 6167 6520 213d 2027 6175 746f  anguage != 'auto
-00038260: 2720 656c 7365 204e 6f6e 652c 0d0a 2020  ' else None,..  
-00038270: 2020 2020 2020 2020 2020 2769 6e70 7574            'input
-00038280: 7327 3a20 5b70 6172 6167 7261 7068 2066  s': [paragraph f
-00038290: 6f72 2070 6172 6167 7261 7068 2069 6e20  or paragraph in 
-000382a0: 7175 6572 795f 7465 7874 2e73 706c 6974  query_text.split
-000382b0: 2827 5c6e 2729 2069 6620 7061 7261 6772  ('\n') if paragr
-000382c0: 6170 682e 7374 7269 7028 295d 2c0d 0a20  aph.strip()],.. 
-000382d0: 2020 2020 2020 2020 2020 2027 666f 726d             'form
-000382e0: 6174 273a 2027 7465 7874 2f70 6c61 696e  at': 'text/plain
-000382f0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00038300: 2761 7574 6f64 6574 6563 7469 6f6e 4d6f  'autodetectionMo
-00038310: 6465 273a 2027 7369 6e67 6c65 272c 0d0a  de': 'single',..
-00038320: 2020 2020 2020 2020 2020 2020 2777 6974              'wit
-00038330: 6849 6e66 6f27 3a20 2774 7275 6527 2c0d  hInfo': 'true',.
-00038340: 0a20 2020 2020 2020 2020 2020 2027 7769  .            'wi
-00038350: 7468 416e 6e6f 7461 7469 6f6e 7327 3a20  thAnnotations': 
-00038360: 2774 7275 6527 2c0d 0a20 2020 2020 2020  'true',..       
-00038370: 2020 2020 2027 7072 6f66 696c 6549 6427       'profileId'
-00038380: 3a20 4e6f 6e65 2c0d 0a20 2020 2020 2020  : None,..       
-00038390: 2020 2020 2027 646f 6d61 696e 273a 204e       'domain': N
-000383a0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-000383b0: 2020 276f 776e 6572 273a 204e 6f6e 652c    'owner': None,
-000383c0: 0d0a 2020 2020 2020 2020 2020 2020 2773  ..            's
-000383d0: 697a 6527 3a20 4e6f 6e65 2c0d 0a20 2020  ize': None,..   
-000383e0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-000383f0: 6966 2075 7365 5f64 6f6d 6169 6e20 616e  if use_domain an
-00038400: 6420 6672 6f6d 5f6c 616e 6775 6167 6520  d from_language 
-00038410: 213d 2027 6175 746f 273a 0d0a 2020 2020  != 'auto':..    
-00038420: 2020 2020 2020 2020 646f 6d61 696e 5f70          domain_p
-00038430: 6179 6c6f 6164 203d 2073 656c 662e 6c61  ayload = self.la
-00038440: 6e67 7061 6972 5f64 6f6d 6169 6e2e 6765  ngpair_domain.ge
-00038450: 7428 6627 7b66 726f 6d5f 6c61 6e67 7561  t(f'{from_langua
-00038460: 6765 7d5f 5f7b 746f 5f6c 616e 6775 6167  ge}__{to_languag
-00038470: 657d 5f5f 7b75 7365 5f64 6f6d 6169 6e7d  e}__{use_domain}
-00038480: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00038490: 6966 206e 6f74 2064 6f6d 6169 6e5f 7061  if not domain_pa
-000384a0: 796c 6f61 643a 0d0a 2020 2020 2020 2020  yload:..        
-000384b0: 2020 2020 2020 2020 7261 6973 6520 5472          raise Tr
-000384c0: 616e 736c 6174 6f72 4572 726f 720d 0a20  anslatorError.. 
-000384d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000384e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000384f0: 2020 7061 796c 6f61 642e 7570 6461 7465    payload.update
-00038500: 2864 6f6d 6169 6e5f 7061 796c 6f61 6429  (domain_payload)
-00038510: 0d0a 0d0a 2020 2020 2020 2020 7220 3d20  ....        r = 
-00038520: 7365 6c66 2e73 6573 7369 6f6e 2e70 6f73  self.session.pos
-00038530: 7428 7365 6c66 2e61 7069 5f75 726c 2c20  t(self.api_url, 
-00038540: 6a73 6f6e 3d70 6179 6c6f 6164 2c20 6865  json=payload, he
-00038550: 6164 6572 733d 7365 6c66 2e61 7069 5f6a  aders=self.api_j
-00038560: 736f 6e5f 6865 6164 6572 732c 2074 696d  son_headers, tim
-00038570: 656f 7574 3d74 696d 656f 7574 2c20 7072  eout=timeout, pr
-00038580: 6f78 6965 733d 7072 6f78 6965 7329 0d0a  oxies=proxies)..
-00038590: 2020 2020 2020 2020 722e 7261 6973 655f          r.raise_
-000385a0: 666f 725f 7374 6174 7573 2829 0d0a 2020  for_status()..  
-000385b0: 2020 2020 2020 6461 7461 203d 2072 2e6a        data = r.j
-000385c0: 736f 6e28 290d 0a20 2020 2020 2020 2074  son()..        t
-000385d0: 696d 652e 736c 6565 7028 736c 6565 705f  ime.sleep(sleep_
-000385e0: 7365 636f 6e64 7329 0d0a 2020 2020 2020  seconds)..      
-000385f0: 2020 7365 6c66 2e71 7565 7279 5f63 6f75    self.query_cou
-00038600: 6e74 202b 3d20 310d 0a20 2020 2020 2020  nt += 1..       
-00038610: 2072 6574 7572 6e20 6461 7461 2069 6620   return data if 
-00038620: 6973 5f64 6574 6169 6c5f 7265 7375 6c74  is_detail_result
-00038630: 2065 6c73 6520 275c 6e27 2e6a 6f69 6e28   else '\n'.join(
-00038640: 2720 272e 6a6f 696e 2869 745b 2761 6c74  ' '.join(it['alt
-00038650: 5f74 7261 6e73 6573 275d 5b30 5d5b 2774  _transes'][0]['t
-00038660: 6172 6765 7427 5d5b 2774 6578 7427 5d20  arget']['text'] 
-00038670: 666f 7220 6974 2069 6e20 6974 656d 5b27  for it in item['
-00038680: 6f75 7470 7574 275d 5b27 646f 6375 6d65  output']['docume
-00038690: 6e74 7327 5d5b 305d 5b27 7472 616e 735f  nts'][0]['trans_
-000386a0: 756e 6974 7327 5d5b 305d 5b27 7365 6e74  units'][0]['sent
-000386b0: 656e 6365 7327 5d29 2066 6f72 2069 7465  ences']) for ite
-000386c0: 6d20 696e 2064 6174 615b 276f 7574 7075  m in data['outpu
-000386d0: 7473 275d 290d 0a0d 0a0d 0a63 6c61 7373  ts'])......class
-000386e0: 2054 7261 6e73 6c61 7465 4d65 2854 7365   TranslateMe(Tse
-000386f0: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-00038700: 6974 5f5f 2873 656c 6629 3a0d 0a20 2020  it__(self):..   
-00038710: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00038720: 6e69 745f 5f28 290d 0a20 2020 2020 2020  nit__()..       
-00038730: 2073 656c 662e 686f 7374 5f75 726c 203d   self.host_url =
-00038740: 2027 6874 7470 733a 2f2f 7472 616e 736c   'https://transl
-00038750: 6174 656d 652e 6e65 7477 6f72 6b2f 270d  ateme.network/'.
-00038760: 0a20 2020 2020 2020 2073 656c 662e 6170  .        self.ap
-00038770: 695f 7572 6c20 3d20 2768 7474 7073 3a2f  i_url = 'https:/
-00038780: 2f74 7261 6e73 6c61 7465 6d65 2e6e 6574  /translateme.net
-00038790: 776f 726b 2f77 702d 6164 6d69 6e2f 6164  work/wp-admin/ad
-000387a0: 6d69 6e2d 616a 6178 2e70 6870 270d 0a20  min-ajax.php'.. 
-000387b0: 2020 2020 2020 2073 656c 662e 686f 7374         self.host
-000387c0: 5f68 6561 6465 7273 203d 2073 656c 662e  _headers = self.
-000387d0: 6765 745f 6865 6164 6572 7328 7365 6c66  get_headers(self
-000387e0: 2e68 6f73 745f 7572 6c2c 2069 665f 6170  .host_url, if_ap
-000387f0: 693d 4661 6c73 652c 2069 665f 7265 6665  i=False, if_refe
-00038800: 7265 725f 666f 725f 686f 7374 3d54 7275  rer_for_host=Tru
-00038810: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
-00038820: 2e61 7069 5f68 6561 6465 7273 203d 2073  .api_headers = s
-00038830: 656c 662e 6765 745f 6865 6164 6572 7328  elf.get_headers(
-00038840: 7365 6c66 2e68 6f73 745f 7572 6c2c 2069  self.host_url, i
-00038850: 665f 6170 693d 5472 7565 2c20 6966 5f61  f_api=True, if_a
-00038860: 6a61 785f 666f 725f 6170 693d 5472 7565  jax_for_api=True
-00038870: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00038880: 7365 7373 696f 6e20 3d20 4e6f 6e65 0d0a  session = None..
-00038890: 2020 2020 2020 2020 7365 6c66 2e6c 616e          self.lan
-000388a0: 6775 6167 655f 6d61 7020 3d20 4e6f 6e65  guage_map = None
-000388b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e71  ..        self.q
-000388c0: 7565 7279 5f63 6f75 6e74 203d 2030 0d0a  uery_count = 0..
-000388d0: 2020 2020 2020 2020 7365 6c66 2e6f 7574          self.out
-000388e0: 7075 745f 7a68 203d 2027 4368 696e 6573  put_zh = 'Chines
-000388f0: 6527 0d0a 2020 2020 2020 2020 7365 6c66  e'..        self
-00038900: 2e6f 7574 7075 745f 656e 203d 2027 456e  .output_en = 'En
-00038910: 676c 6973 6827 0d0a 2020 2020 2020 2020  glish'..        
-00038920: 7365 6c66 2e69 6e70 7574 5f6c 696d 6974  self.input_limit
-00038930: 203d 2069 6e74 2831 6532 290d 0a20 2020   = int(1e2)..   
-00038940: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
-00038950: 745f 6672 6f6d 5f6c 616e 6775 6167 6520  t_from_language 
-00038960: 3d20 7365 6c66 2e6f 7574 7075 745f 7a68  = self.output_zh
-00038970: 0d0a 0d0a 2020 2020 4054 7365 2e64 6562  ....    @Tse.deb
-00038980: 7567 5f6c 616e 6775 6167 655f 6d61 700d  ug_language_map.
-00038990: 0a20 2020 2064 6566 2067 6574 5f6c 616e  .    def get_lan
-000389a0: 6775 6167 655f 6d61 7028 7365 6c66 2c20  guage_map(self, 
-000389b0: 686f 7374 5f68 746d 6c3a 2073 7472 2c20  host_html: str, 
-000389c0: 2a2a 6b77 6172 6773 3a20 4c61 6e67 4d61  **kwargs: LangMa
-000389d0: 704b 7761 7267 7354 7970 6529 202d 3e20  pKwargsType) -> 
-000389e0: 6469 6374 3a0d 0a20 2020 2020 2020 206c  dict:..        l
-000389f0: 616e 675f 6c69 7374 203d 2072 652e 636f  ang_list = re.co
-00038a00: 6d70 696c 6528 2764 6174 612d 6c61 6e67  mpile('data-lang
-00038a10: 3d22 282e 2a3f 2922 2729 2e66 696e 6461  ="(.*?)"').finda
-00038a20: 6c6c 2868 6f73 745f 6874 6d6c 290d 0a20  ll(host_html).. 
-00038a30: 2020 2020 2020 2069 6620 6e6f 7420 6c61         if not la
-00038a40: 6e67 5f6c 6973 743a 0d0a 2020 2020 2020  ng_list:..      
-00038a50: 2020 2020 2020 7261 6973 6520 5472 616e        raise Tran
-00038a60: 736c 6174 6f72 4572 726f 720d 0a0d 0a20  slatorError.... 
-00038a70: 2020 2020 2020 206c 616e 675f 6c69 7374         lang_list
-00038a80: 203d 2073 6f72 7465 6428 6c69 7374 2873   = sorted(list(s
-00038a90: 6574 286c 616e 675f 6c69 7374 2929 290d  et(lang_list))).
-00038aa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00038ab0: 7b7d 2e66 726f 6d6b 6579 7328 6c61 6e67  {}.fromkeys(lang
-00038ac0: 5f6c 6973 742c 206c 616e 675f 6c69 7374  _list, lang_list
-00038ad0: 290d 0a0d 0a20 2020 2023 2040 5473 652e  )....    # @Tse.
-00038ae0: 756e 6365 7274 6966 6965 640d 0a20 2020  uncertified..   
-00038af0: 2023 2040 5473 652e 7469 6d65 5f73 7461   # @Tse.time_sta
-00038b00: 740d 0a20 2020 2023 2040 5473 652e 6368  t..    # @Tse.ch
-00038b10: 6563 6b5f 7175 6572 790d 0a20 2020 2064  eck_query..    d
-00038b20: 6566 205f 7472 616e 736c 6174 654d 655f  ef _translateMe_
-00038b30: 6170 6928 7365 6c66 2c20 7175 6572 795f  api(self, query_
-00038b40: 7465 7874 3a20 7374 722c 2066 726f 6d5f  text: str, from_
-00038b50: 6c61 6e67 7561 6765 3a20 7374 7220 3d20  language: str = 
-00038b60: 2761 7574 6f27 2c20 746f 5f6c 616e 6775  'auto', to_langu
-00038b70: 6167 653a 2073 7472 203d 2027 656e 272c  age: str = 'en',
-00038b80: 202a 2a6b 7761 7267 733a 2041 7069 4b77   **kwargs: ApiKw
-00038b90: 6172 6773 5479 7065 2920 2d3e 2055 6e69  argsType) -> Uni
-00038ba0: 6f6e 5b73 7472 2c20 6469 6374 5d3a 0d0a  on[str, dict]:..
-00038bb0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00038bc0: 2020 2020 2068 7474 7073 3a2f 2f74 7261       https://tra
-00038bd0: 6e73 6c61 7465 6d65 2e6e 6574 776f 726b  nslateme.network
-00038be0: 2f0d 0a20 2020 2020 2020 203a 7061 7261  /..        :para
-00038bf0: 6d20 7175 6572 795f 7465 7874 3a20 7374  m query_text: st
-00038c00: 722c 206d 7573 742e 0d0a 2020 2020 2020  r, must...      
-00038c10: 2020 3a70 6172 616d 2066 726f 6d5f 6c61    :param from_la
-00038c20: 6e67 7561 6765 3a20 7374 722c 2064 6566  nguage: str, def
-00038c30: 6175 6c74 2027 6175 746f 272e 0d0a 2020  ault 'auto'...  
-00038c40: 2020 2020 2020 3a70 6172 616d 2074 6f5f        :param to_
-00038c50: 6c61 6e67 7561 6765 3a20 7374 722c 2064  language: str, d
-00038c60: 6566 6175 6c74 2027 656e 272e 0d0a 2020  efault 'en'...  
-00038c70: 2020 2020 2020 3a70 6172 616d 202a 2a6b        :param **k
-00038c80: 7761 7267 733a 0d0a 2020 2020 2020 2020  wargs:..        
-00038c90: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
-00038ca0: 696d 656f 7574 3a20 666c 6f61 742c 2064  imeout: float, d
-00038cb0: 6566 6175 6c74 204e 6f6e 652e 0d0a 2020  efault None...  
-00038cc0: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-00038cd0: 6172 616d 2070 726f 7869 6573 3a20 6469  aram proxies: di
-00038ce0: 6374 2c20 6465 6661 756c 7420 4e6f 6e65  ct, default None
-00038cf0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00038d00: 2020 203a 7061 7261 6d20 736c 6565 705f     :param sleep_
-00038d10: 7365 636f 6e64 733a 2066 6c6f 6174 2c20  seconds: float, 
-00038d20: 6465 6661 756c 7420 302e 0d0a 2020 2020  default 0...    
-00038d30: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-00038d40: 616d 2069 735f 6465 7461 696c 5f72 6573  am is_detail_res
-00038d50: 756c 743a 2062 6f6f 6c2c 2064 6566 6175  ult: bool, defau
-00038d60: 6c74 2046 616c 7365 2e0d 0a20 2020 2020  lt False...     
-00038d70: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00038d80: 6d20 6966 5f69 676e 6f72 655f 6c69 6d69  m if_ignore_limi
-00038d90: 745f 6f66 5f6c 656e 6774 683a 2062 6f6f  t_of_length: boo
-00038da0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-00038db0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00038dc0: 2020 203a 7061 7261 6d20 6c69 6d69 745f     :param limit_
-00038dd0: 6f66 5f6c 656e 6774 683a 2069 6e74 2c20  of_length: int, 
-00038de0: 6465 6661 756c 7420 3230 3030 302e 0d0a  default 20000...
-00038df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00038e00: 3a70 6172 616d 2069 665f 6967 6e6f 7265  :param if_ignore
-00038e10: 5f65 6d70 7479 5f71 7565 7279 3a20 626f  _empty_query: bo
-00038e20: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-00038e30: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
-00038e40: 2020 2020 3a70 6172 616d 2075 7064 6174      :param updat
-00038e50: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
-00038e60: 6672 6571 3a20 696e 742c 2064 6566 6175  freq: int, defau
-00038e70: 6c74 2031 3030 302e 0d0a 2020 2020 2020  lt 1000...      
-00038e80: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00038e90: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
-00038ea0: 6166 7465 725f 7365 636f 6e64 733a 2066  after_seconds: f
-00038eb0: 6c6f 6174 2c20 6465 6661 756c 7420 3135  loat, default 15
-00038ec0: 3030 2e0d 0a20 2020 2020 2020 2020 2020  00...           
-00038ed0: 2020 2020 203a 7061 7261 6d20 6966 5f73       :param if_s
-00038ee0: 686f 775f 7469 6d65 5f73 7461 743a 2062  how_time_stat: b
-00038ef0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
-00038f00: 7365 2e0d 0a20 2020 2020 2020 2020 2020  se...           
-00038f10: 2020 2020 203a 7061 7261 6d20 7368 6f77       :param show
-00038f20: 5f74 696d 655f 7374 6174 5f70 7265 6369  _time_stat_preci
-00038f30: 7369 6f6e 3a20 696e 742c 2064 6566 6175  sion: int, defau
-00038f40: 6c74 2032 2e0d 0a20 2020 2020 2020 2020  lt 2...         
-00038f50: 2020 2020 2020 203a 7061 7261 6d20 6966         :param if
-00038f60: 5f70 7269 6e74 5f77 6172 6e69 6e67 3a20  _print_warning: 
-00038f70: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
-00038f80: 7565 2e0d 0a20 2020 2020 2020 203a 7265  ue...        :re
-00038f90: 7475 726e 3a20 7374 7220 6f72 2064 6963  turn: str or dic
-00038fa0: 740d 0a20 2020 2020 2020 2022 2222 0d0a  t..        """..
-00038fb0: 0d0a 2020 2020 2020 2020 7469 6d65 6f75  ..        timeou
-00038fc0: 7420 3d20 6b77 6172 6773 2e67 6574 2827  t = kwargs.get('
-00038fd0: 7469 6d65 6f75 7427 2c20 4e6f 6e65 290d  timeout', None).
-00038fe0: 0a20 2020 2020 2020 2070 726f 7869 6573  .        proxies
-00038ff0: 203d 206b 7761 7267 732e 6765 7428 2770   = kwargs.get('p
-00039000: 726f 7869 6573 272c 204e 6f6e 6529 0d0a  roxies', None)..
-00039010: 2020 2020 2020 2020 736c 6565 705f 7365          sleep_se
-00039020: 636f 6e64 7320 3d20 6b77 6172 6773 2e67  conds = kwargs.g
-00039030: 6574 2827 736c 6565 705f 7365 636f 6e64  et('sleep_second
-00039040: 7327 2c20 3029 0d0a 2020 2020 2020 2020  s', 0)..        
-00039050: 6966 5f70 7269 6e74 5f77 6172 6e69 6e67  if_print_warning
-00039060: 203d 206b 7761 7267 732e 6765 7428 2769   = kwargs.get('i
-00039070: 665f 7072 696e 745f 7761 726e 696e 6727  f_print_warning'
-00039080: 2c20 5472 7565 290d 0a20 2020 2020 2020  , True)..       
-00039090: 2069 735f 6465 7461 696c 5f72 6573 756c   is_detail_resul
-000390a0: 7420 3d20 6b77 6172 6773 2e67 6574 2827  t = kwargs.get('
-000390b0: 6973 5f64 6574 6169 6c5f 7265 7375 6c74  is_detail_result
-000390c0: 272c 2046 616c 7365 290d 0a20 2020 2020  ', False)..     
-000390d0: 2020 2075 7064 6174 655f 7365 7373 696f     update_sessio
-000390e0: 6e5f 6166 7465 725f 6672 6571 203d 206b  n_after_freq = k
-000390f0: 7761 7267 732e 6765 7428 2775 7064 6174  wargs.get('updat
-00039100: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
-00039110: 6672 6571 272c 2073 656c 662e 6465 6661  freq', self.defa
-00039120: 756c 745f 7365 7373 696f 6e5f 6672 6571  ult_session_freq
-00039130: 290d 0a20 2020 2020 2020 2075 7064 6174  )..        updat
-00039140: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
-00039150: 7365 636f 6e64 7320 3d20 6b77 6172 6773  seconds = kwargs
-00039160: 2e67 6574 2827 7570 6461 7465 5f73 6573  .get('update_ses
-00039170: 7369 6f6e 5f61 6674 6572 5f73 6563 6f6e  sion_after_secon
-00039180: 6473 272c 2073 656c 662e 6465 6661 756c  ds', self.defaul
-00039190: 745f 7365 7373 696f 6e5f 7365 636f 6e64  t_session_second
-000391a0: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
-000391b0: 2e63 6865 636b 5f69 6e70 7574 5f6c 696d  .check_input_lim
-000391c0: 6974 2871 7565 7279 5f74 6578 742c 2073  it(query_text, s
-000391d0: 656c 662e 696e 7075 745f 6c69 6d69 7429  elf.input_limit)
-000391e0: 0d0a 0d0a 2020 2020 2020 2020 6e6f 745f  ....        not_
-000391f0: 7570 6461 7465 5f63 6f6e 645f 6672 6571  update_cond_freq
-00039200: 203d 2031 2069 6620 7365 6c66 2e71 7565   = 1 if self.que
-00039210: 7279 5f63 6f75 6e74 203c 2075 7064 6174  ry_count < updat
-00039220: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
-00039230: 6672 6571 2065 6c73 6520 300d 0a20 2020  freq else 0..   
-00039240: 2020 2020 206e 6f74 5f75 7064 6174 655f       not_update_
-00039250: 636f 6e64 5f74 696d 6520 3d20 3120 6966  cond_time = 1 if
-00039260: 2074 696d 652e 7469 6d65 2829 202d 2073   time.time() - s
-00039270: 656c 662e 6265 6769 6e5f 7469 6d65 203c  elf.begin_time <
-00039280: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
-00039290: 6166 7465 725f 7365 636f 6e64 7320 656c  after_seconds el
-000392a0: 7365 2030 0d0a 2020 2020 2020 2020 6966  se 0..        if
-000392b0: 206e 6f74 2028 7365 6c66 2e73 6573 7369   not (self.sessi
-000392c0: 6f6e 2061 6e64 2073 656c 662e 6c61 6e67  on and self.lang
-000392d0: 7561 6765 5f6d 6170 2061 6e64 206e 6f74  uage_map and not
-000392e0: 5f75 7064 6174 655f 636f 6e64 5f66 7265  _update_cond_fre
-000392f0: 7120 616e 6420 6e6f 745f 7570 6461 7465  q and not_update
-00039300: 5f63 6f6e 645f 7469 6d65 293a 0d0a 2020  _cond_time):..  
-00039310: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00039320: 6573 7369 6f6e 203d 2072 6571 7565 7374  ession = request
-00039330: 732e 5365 7373 696f 6e28 290d 0a20 2020  s.Session()..   
-00039340: 2020 2020 2020 2020 2068 6f73 745f 6874           host_ht
-00039350: 6d6c 203d 2073 656c 662e 7365 7373 696f  ml = self.sessio
-00039360: 6e2e 6765 7428 7365 6c66 2e68 6f73 745f  n.get(self.host_
-00039370: 7572 6c2c 2068 6561 6465 7273 3d73 656c  url, headers=sel
-00039380: 662e 686f 7374 5f68 6561 6465 7273 2c20  f.host_headers, 
-00039390: 7469 6d65 6f75 743d 7469 6d65 6f75 742c  timeout=timeout,
-000393a0: 2070 726f 7869 6573 3d70 726f 7869 6573   proxies=proxies
-000393b0: 292e 7465 7874 0d0a 2020 2020 2020 2020  ).text..        
-000393c0: 2020 2020 6465 6275 675f 6c61 6e67 5f6b      debug_lang_k
-000393d0: 7761 7267 7320 3d20 7365 6c66 2e64 6562  wargs = self.deb
-000393e0: 7567 5f6c 616e 675f 6b77 6172 6773 2866  ug_lang_kwargs(f
-000393f0: 726f 6d5f 6c61 6e67 7561 6765 2c20 746f  rom_language, to
-00039400: 5f6c 616e 6775 6167 652c 2073 656c 662e  _language, self.
-00039410: 6465 6661 756c 745f 6672 6f6d 5f6c 616e  default_from_lan
-00039420: 6775 6167 652c 2069 665f 7072 696e 745f  guage, if_print_
-00039430: 7761 726e 696e 6729 0d0a 2020 2020 2020  warning)..      
-00039440: 2020 2020 2020 7365 6c66 2e6c 616e 6775        self.langu
-00039450: 6167 655f 6d61 7020 3d20 7365 6c66 2e67  age_map = self.g
-00039460: 6574 5f6c 616e 6775 6167 655f 6d61 7028  et_language_map(
-00039470: 686f 7374 5f68 746d 6c2c 202a 2a64 6562  host_html, **deb
-00039480: 7567 5f6c 616e 675f 6b77 6172 6773 290d  ug_lang_kwargs).
-00039490: 0a0d 0a20 2020 2020 2020 2069 6620 6672  ...        if fr
-000394a0: 6f6d 5f6c 616e 6775 6167 6520 3d3d 2027  om_language == '
-000394b0: 6175 746f 273a 0d0a 2020 2020 2020 2020  auto':..        
-000394c0: 2020 2020 6672 6f6d 5f6c 616e 6775 6167      from_languag
-000394d0: 6520 3d20 7365 6c66 2e77 6172 6e69 6e67  e = self.warning
-000394e0: 5f61 7574 6f5f 6c61 6e67 2827 7472 616e  _auto_lang('tran
-000394f0: 736c 6174 654d 6527 2c20 7365 6c66 2e64  slateMe', self.d
-00039500: 6566 6175 6c74 5f66 726f 6d5f 6c61 6e67  efault_from_lang
-00039510: 7561 6765 2c20 6966 5f70 7269 6e74 5f77  uage, if_print_w
-00039520: 6172 6e69 6e67 290d 0a20 2020 2020 2020  arning)..       
-00039530: 2066 726f 6d5f 6c61 6e67 7561 6765 2c20   from_language, 
-00039540: 746f 5f6c 616e 6775 6167 6520 3d20 7365  to_language = se
-00039550: 6c66 2e63 6865 636b 5f6c 616e 6775 6167  lf.check_languag
-00039560: 6528 6672 6f6d 5f6c 616e 6775 6167 652c  e(from_language,
-00039570: 2074 6f5f 6c61 6e67 7561 6765 2c20 7365   to_language, se
-00039580: 6c66 2e6c 616e 6775 6167 655f 6d61 702c  lf.language_map,
-00039590: 206f 7574 7075 745f 7a68 3d73 656c 662e   output_zh=self.
-000395a0: 6f75 7470 7574 5f7a 682c 0d0a 2020 2020  output_zh,..    
-000395b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000395c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000395d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000395e0: 2020 2020 206f 7574 7075 745f 656e 5f74       output_en_t
-000395f0: 7261 6e73 6c61 746f 723d 2774 7261 6e73  ranslator='trans
-00039600: 6c61 7465 4d65 272c 206f 7574 7075 745f  lateMe', output_
-00039610: 656e 3d73 656c 662e 6f75 7470 7574 5f65  en=self.output_e
-00039620: 6e29 0d0a 2020 2020 2020 2020 6966 2073  n)..        if s
-00039630: 656c 662e 6f75 7470 7574 5f65 6e20 6e6f  elf.output_en no
-00039640: 7420 696e 2028 6672 6f6d 5f6c 616e 6775  t in (from_langu
-00039650: 6167 652c 2074 6f5f 6c61 6e67 7561 6765  age, to_language
-00039660: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00039670: 7261 6973 6520 5472 616e 736c 6174 6f72  raise Translator
-00039680: 4572 726f 7228 274d 7573 7420 7573 6520  Error('Must use 
-00039690: 456e 676c 6973 6820 6173 2061 6e20 696e  English as an in
-000396a0: 7465 726d 6564 6961 7465 2074 7261 6e73  termediate trans
-000396b0: 6c61 7469 6f6e 2e27 290d 0a0d 0a20 2020  lation.')....   
-000396c0: 2020 2020 2064 6174 615f 6c69 7374 203d       data_list =
-000396d0: 205b 5d0d 0a20 2020 2020 2020 2070 6172   []..        par
-000396e0: 6167 7261 7068 7320 3d20 5b70 6172 6167  agraphs = [parag
-000396f0: 7261 7068 2066 6f72 2070 6172 6167 7261  raph for paragra
-00039700: 7068 2069 6e20 7175 6572 795f 7465 7874  ph in query_text
-00039710: 2e73 706c 6974 2827 5c6e 2729 2069 6620  .split('\n') if 
-00039720: 7061 7261 6772 6170 682e 7374 7269 7028  paragraph.strip(
-00039730: 295d 0d0a 2020 2020 2020 2020 666f 7220  )]..        for 
-00039740: 7061 7261 6772 6170 6820 696e 2070 6172  paragraph in par
-00039750: 6167 7261 7068 733a 0d0a 2020 2020 2020  agraphs:..      
-00039760: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
-00039770: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00039780: 2020 2027 7465 7874 273a 2070 6172 6167     'text': parag
-00039790: 7261 7068 2c0d 0a20 2020 2020 2020 2020  raph,..         
-000397a0: 2020 2020 2020 2027 6c61 6e67 5f66 726f         'lang_fro
-000397b0: 6d27 3a20 6672 6f6d 5f6c 616e 6775 6167  m': from_languag
-000397c0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000397d0: 2020 2020 276c 616e 675f 746f 273a 2074      'lang_to': t
-000397e0: 6f5f 6c61 6e67 7561 6765 2c0d 0a20 2020  o_language,..   
-000397f0: 2020 2020 2020 2020 2020 2020 2027 6163               'ac
-00039800: 7469 6f6e 273a 2027 746d 5f6d 795f 6163  tion': 'tm_my_ac
-00039810: 7469 6f6e 272c 0d0a 2020 2020 2020 2020  tion',..        
-00039820: 2020 2020 2020 2020 2774 7970 6527 3a20          'type': 
-00039830: 2763 6f6e 7665 7274 270d 0a20 2020 2020  'convert'..     
-00039840: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-00039850: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
-00039860: 7572 6c6c 6962 2e70 6172 7365 2e75 726c  urllib.parse.url
-00039870: 656e 636f 6465 2870 6179 6c6f 6164 290d  encode(payload).
-00039880: 0a20 2020 2020 2020 2020 2020 2072 203d  .            r =
-00039890: 2073 656c 662e 7365 7373 696f 6e2e 706f   self.session.po
-000398a0: 7374 2873 656c 662e 6170 695f 7572 6c2c  st(self.api_url,
-000398b0: 2064 6174 613d 7061 796c 6f61 642c 2068   data=payload, h
-000398c0: 6561 6465 7273 3d73 656c 662e 6170 695f  eaders=self.api_
-000398d0: 6865 6164 6572 732c 2074 696d 656f 7574  headers, timeout
-000398e0: 3d74 696d 656f 7574 2c20 7072 6f78 6965  =timeout, proxie
-000398f0: 733d 7072 6f78 6965 7329 0d0a 2020 2020  s=proxies)..    
-00039900: 2020 2020 2020 2020 722e 7261 6973 655f          r.raise_
-00039910: 666f 725f 7374 6174 7573 2829 0d0a 2020  for_status()..  
-00039920: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00039930: 2072 2e6a 736f 6e28 290d 0a20 2020 2020   r.json()..     
-00039940: 2020 2020 2020 2064 6174 615f 6c69 7374         data_list
-00039950: 2e61 7070 656e 6428 6461 7461 290d 0a20  .append(data).. 
-00039960: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-00039970: 7028 736c 6565 705f 7365 636f 6e64 7329  p(sleep_seconds)
-00039980: 0d0a 2020 2020 2020 2020 7365 6c66 2e71  ..        self.q
-00039990: 7565 7279 5f63 6f75 6e74 202b 3d20 310d  uery_count += 1.
-000399a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000399b0: 7b27 6461 7461 273a 2064 6174 615f 6c69  {'data': data_li
-000399c0: 7374 7d20 6966 2069 735f 6465 7461 696c  st} if is_detail
-000399d0: 5f72 6573 756c 7420 656c 7365 2027 5c6e  _result else '\n
-000399e0: 272e 6a6f 696e 285b 6974 656d 5b27 746f  '.join([item['to
-000399f0: 275d 2066 6f72 2069 7465 6d20 696e 2064  '] for item in d
-00039a00: 6174 615f 6c69 7374 5d29 0d0a 0d0a 2020  ata_list])....  
-00039a10: 2020 4054 7365 2e75 6e63 6572 7469 6669    @Tse.uncertifi
-00039a20: 6564 0d0a 2020 2020 4054 7365 2e74 696d  ed..    @Tse.tim
-00039a30: 655f 7374 6174 0d0a 2020 2020 4054 7365  e_stat..    @Tse
-00039a40: 2e63 6865 636b 5f71 7565 7279 0d0a 2020  .check_query..  
-00039a50: 2020 6465 6620 7472 616e 736c 6174 654d    def translateM
-00039a60: 655f 6170 6928 7365 6c66 2c20 7175 6572  e_api(self, quer
-00039a70: 795f 7465 7874 3a20 7374 722c 2066 726f  y_text: str, fro
-00039a80: 6d5f 6c61 6e67 7561 6765 3a20 7374 7220  m_language: str 
-00039a90: 3d20 2761 7574 6f27 2c20 746f 5f6c 616e  = 'auto', to_lan
-00039aa0: 6775 6167 653a 2073 7472 203d 2027 656e  guage: str = 'en
-00039ab0: 272c 202a 2a6b 7761 7267 733a 2041 7069  ', **kwargs: Api
-00039ac0: 4b77 6172 6773 5479 7065 2920 2d3e 2055  KwargsType) -> U
-00039ad0: 6e69 6f6e 5b73 7472 2c20 6469 6374 5d3a  nion[str, dict]:
-00039ae0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00039af0: 2020 2020 2020 2068 7474 7073 3a2f 2f74         https://t
-00039b00: 7261 6e73 6c61 7465 6d65 2e6e 6574 776f  ranslateme.netwo
-00039b10: 726b 2f0d 0a20 2020 2020 2020 203a 7061  rk/..        :pa
-00039b20: 7261 6d20 7175 6572 795f 7465 7874 3a20  ram query_text: 
-00039b30: 7374 722c 206d 7573 742e 0d0a 2020 2020  str, must...    
-00039b40: 2020 2020 3a70 6172 616d 2066 726f 6d5f      :param from_
-00039b50: 6c61 6e67 7561 6765 3a20 7374 722c 2064  language: str, d
-00039b60: 6566 6175 6c74 2027 6175 746f 272e 0d0a  efault 'auto'...
-00039b70: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
-00039b80: 6f5f 6c61 6e67 7561 6765 3a20 7374 722c  o_language: str,
-00039b90: 2064 6566 6175 6c74 2027 656e 272e 0d0a   default 'en'...
-00039ba0: 2020 2020 2020 2020 3a70 6172 616d 202a          :param *
-00039bb0: 2a6b 7761 7267 733a 0d0a 2020 2020 2020  *kwargs:..      
-00039bc0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00039bd0: 2074 696d 656f 7574 3a20 666c 6f61 742c   timeout: float,
-00039be0: 2064 6566 6175 6c74 204e 6f6e 652e 0d0a   default None...
-00039bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039c00: 3a70 6172 616d 2070 726f 7869 6573 3a20  :param proxies: 
-00039c10: 6469 6374 2c20 6465 6661 756c 7420 4e6f  dict, default No
-00039c20: 6e65 2e0d 0a20 2020 2020 2020 2020 2020  ne...           
-00039c30: 2020 2020 203a 7061 7261 6d20 736c 6565       :param slee
-00039c40: 705f 7365 636f 6e64 733a 2066 6c6f 6174  p_seconds: float
-00039c50: 2c20 6465 6661 756c 7420 302e 0d0a 2020  , default 0...  
-00039c60: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-00039c70: 6172 616d 2069 735f 6465 7461 696c 5f72  aram is_detail_r
-00039c80: 6573 756c 743a 2062 6f6f 6c2c 2064 6566  esult: bool, def
-00039c90: 6175 6c74 2046 616c 7365 2e0d 0a20 2020  ault False...   
-00039ca0: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-00039cb0: 7261 6d20 6966 5f69 676e 6f72 655f 6c69  ram if_ignore_li
-00039cc0: 6d69 745f 6f66 5f6c 656e 6774 683a 2062  mit_of_length: b
-00039cd0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
-00039ce0: 7365 2e0d 0a20 2020 2020 2020 2020 2020  se...           
-00039cf0: 2020 2020 203a 7061 7261 6d20 6c69 6d69       :param limi
-00039d00: 745f 6f66 5f6c 656e 6774 683a 2069 6e74  t_of_length: int
-00039d10: 2c20 6465 6661 756c 7420 3230 3030 302e  , default 20000.
-00039d20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00039d30: 2020 3a70 6172 616d 2069 665f 6967 6e6f    :param if_igno
-00039d40: 7265 5f65 6d70 7479 5f71 7565 7279 3a20  re_empty_query: 
-00039d50: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-00039d60: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
-00039d70: 2020 2020 2020 3a70 6172 616d 2075 7064        :param upd
-00039d80: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
-00039d90: 725f 6672 6571 3a20 696e 742c 2064 6566  r_freq: int, def
-00039da0: 6175 6c74 2031 3030 302e 0d0a 2020 2020  ault 1000...    
-00039db0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-00039dc0: 616d 2075 7064 6174 655f 7365 7373 696f  am update_sessio
-00039dd0: 6e5f 6166 7465 725f 7365 636f 6e64 733a  n_after_seconds:
-00039de0: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
-00039df0: 3135 3030 2e0d 0a20 2020 2020 2020 2020  1500...         
-00039e00: 2020 2020 2020 203a 7061 7261 6d20 6966         :param if
-00039e10: 5f73 686f 775f 7469 6d65 5f73 7461 743a  _show_time_stat:
-00039e20: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
-00039e30: 616c 7365 2e0d 0a20 2020 2020 2020 2020  alse...         
-00039e40: 2020 2020 2020 203a 7061 7261 6d20 7368         :param sh
-00039e50: 6f77 5f74 696d 655f 7374 6174 5f70 7265  ow_time_stat_pre
-00039e60: 6369 7369 6f6e 3a20 696e 742c 2064 6566  cision: int, def
-00039e70: 6175 6c74 2032 2e0d 0a20 2020 2020 2020  ault 2...       
-00039e80: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00039e90: 6966 5f70 7269 6e74 5f77 6172 6e69 6e67  if_print_warning
-00039ea0: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00039eb0: 5472 7565 2e0d 0a20 2020 2020 2020 203a  True...        :
-00039ec0: 7265 7475 726e 3a20 7374 7220 6f72 2064  return: str or d
-00039ed0: 6963 740d 0a20 2020 2020 2020 2022 2222  ict..        """
-00039ee0: 0d0a 0d0a 2020 2020 2020 2020 7469 6d65  ....        time
-00039ef0: 6f75 7420 3d20 6b77 6172 6773 2e67 6574  out = kwargs.get
-00039f00: 2827 7469 6d65 6f75 7427 2c20 4e6f 6e65  ('timeout', None
-00039f10: 290d 0a20 2020 2020 2020 2070 726f 7869  )..        proxi
-00039f20: 6573 203d 206b 7761 7267 732e 6765 7428  es = kwargs.get(
-00039f30: 2770 726f 7869 6573 272c 204e 6f6e 6529  'proxies', None)
-00039f40: 0d0a 2020 2020 2020 2020 736c 6565 705f  ..        sleep_
-00039f50: 7365 636f 6e64 7320 3d20 6b77 6172 6773  seconds = kwargs
-00039f60: 2e67 6574 2827 736c 6565 705f 7365 636f  .get('sleep_seco
-00039f70: 6e64 7327 2c20 3029 0d0a 2020 2020 2020  nds', 0)..      
-00039f80: 2020 6966 5f70 7269 6e74 5f77 6172 6e69    if_print_warni
-00039f90: 6e67 203d 206b 7761 7267 732e 6765 7428  ng = kwargs.get(
-00039fa0: 2769 665f 7072 696e 745f 7761 726e 696e  'if_print_warnin
-00039fb0: 6727 2c20 5472 7565 290d 0a20 2020 2020  g', True)..     
-00039fc0: 2020 2069 735f 6465 7461 696c 5f72 6573     is_detail_res
-00039fd0: 756c 7420 3d20 6b77 6172 6773 2e67 6574  ult = kwargs.get
-00039fe0: 2827 6973 5f64 6574 6169 6c5f 7265 7375  ('is_detail_resu
-00039ff0: 6c74 272c 2046 616c 7365 290d 0a20 2020  lt', False)..   
-0003a000: 2020 2020 2075 7064 6174 655f 7365 7373       update_sess
-0003a010: 696f 6e5f 6166 7465 725f 6672 6571 203d  ion_after_freq =
-0003a020: 206b 7761 7267 732e 6765 7428 2775 7064   kwargs.get('upd
-0003a030: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
-0003a040: 725f 6672 6571 272c 2073 656c 662e 6465  r_freq', self.de
-0003a050: 6661 756c 745f 7365 7373 696f 6e5f 6672  fault_session_fr
-0003a060: 6571 290d 0a20 2020 2020 2020 2075 7064  eq)..        upd
-0003a070: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
-0003a080: 725f 7365 636f 6e64 7320 3d20 6b77 6172  r_seconds = kwar
-0003a090: 6773 2e67 6574 2827 7570 6461 7465 5f73  gs.get('update_s
-0003a0a0: 6573 7369 6f6e 5f61 6674 6572 5f73 6563  ession_after_sec
-0003a0b0: 6f6e 6473 272c 2073 656c 662e 6465 6661  onds', self.defa
-0003a0c0: 756c 745f 7365 7373 696f 6e5f 7365 636f  ult_session_seco
-0003a0d0: 6e64 7329 0d0a 2020 2020 2020 2020 7365  nds)..        se
-0003a0e0: 6c66 2e63 6865 636b 5f69 6e70 7574 5f6c  lf.check_input_l
-0003a0f0: 696d 6974 2871 7565 7279 5f74 6578 742c  imit(query_text,
-0003a100: 2073 656c 662e 696e 7075 745f 6c69 6d69   self.input_limi
-0003a110: 7429 0d0a 0d0a 2020 2020 2020 2020 6e6f  t)....        no
-0003a120: 745f 7570 6461 7465 5f63 6f6e 645f 6672  t_update_cond_fr
-0003a130: 6571 203d 2031 2069 6620 7365 6c66 2e71  eq = 1 if self.q
-0003a140: 7565 7279 5f63 6f75 6e74 203c 2075 7064  uery_count < upd
-0003a150: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
-0003a160: 725f 6672 6571 2065 6c73 6520 300d 0a20  r_freq else 0.. 
-0003a170: 2020 2020 2020 206e 6f74 5f75 7064 6174         not_updat
-0003a180: 655f 636f 6e64 5f74 696d 6520 3d20 3120  e_cond_time = 1 
-0003a190: 6966 2074 696d 652e 7469 6d65 2829 202d  if time.time() -
-0003a1a0: 2073 656c 662e 6265 6769 6e5f 7469 6d65   self.begin_time
-0003a1b0: 203c 2075 7064 6174 655f 7365 7373 696f   < update_sessio
-0003a1c0: 6e5f 6166 7465 725f 7365 636f 6e64 7320  n_after_seconds 
-0003a1d0: 656c 7365 2030 0d0a 2020 2020 2020 2020  else 0..        
-0003a1e0: 6966 206e 6f74 2028 7365 6c66 2e73 6573  if not (self.ses
-0003a1f0: 7369 6f6e 2061 6e64 2073 656c 662e 6c61  sion and self.la
-0003a200: 6e67 7561 6765 5f6d 6170 2061 6e64 206e  nguage_map and n
-0003a210: 6f74 5f75 7064 6174 655f 636f 6e64 5f66  ot_update_cond_f
-0003a220: 7265 7120 616e 6420 6e6f 745f 7570 6461  req and not_upda
-0003a230: 7465 5f63 6f6e 645f 7469 6d65 293a 0d0a  te_cond_time):..
-0003a240: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0003a250: 2e73 6573 7369 6f6e 203d 2072 6571 7565  .session = reque
-0003a260: 7374 732e 5365 7373 696f 6e28 290d 0a20  sts.Session().. 
-0003a270: 2020 2020 2020 2020 2020 2068 6f73 745f             host_
-0003a280: 6874 6d6c 203d 2073 656c 662e 7365 7373  html = self.sess
-0003a290: 696f 6e2e 6765 7428 7365 6c66 2e68 6f73  ion.get(self.hos
-0003a2a0: 745f 7572 6c2c 2068 6561 6465 7273 3d73  t_url, headers=s
-0003a2b0: 656c 662e 686f 7374 5f68 6561 6465 7273  elf.host_headers
-0003a2c0: 2c20 7469 6d65 6f75 743d 7469 6d65 6f75  , timeout=timeou
-0003a2d0: 742c 2070 726f 7869 6573 3d70 726f 7869  t, proxies=proxi
-0003a2e0: 6573 292e 7465 7874 0d0a 2020 2020 2020  es).text..      
-0003a2f0: 2020 2020 2020 6465 6275 675f 6c61 6e67        debug_lang
-0003a300: 5f6b 7761 7267 7320 3d20 7365 6c66 2e64  _kwargs = self.d
-0003a310: 6562 7567 5f6c 616e 675f 6b77 6172 6773  ebug_lang_kwargs
-0003a320: 2866 726f 6d5f 6c61 6e67 7561 6765 2c20  (from_language, 
-0003a330: 746f 5f6c 616e 6775 6167 652c 2073 656c  to_language, sel
-0003a340: 662e 6465 6661 756c 745f 6672 6f6d 5f6c  f.default_from_l
-0003a350: 616e 6775 6167 652c 2069 665f 7072 696e  anguage, if_prin
-0003a360: 745f 7761 726e 696e 6729 0d0a 2020 2020  t_warning)..    
-0003a370: 2020 2020 2020 2020 7365 6c66 2e6c 616e          self.lan
-0003a380: 6775 6167 655f 6d61 7020 3d20 7365 6c66  guage_map = self
-0003a390: 2e67 6574 5f6c 616e 6775 6167 655f 6d61  .get_language_ma
-0003a3a0: 7028 686f 7374 5f68 746d 6c2c 202a 2a64  p(host_html, **d
-0003a3b0: 6562 7567 5f6c 616e 675f 6b77 6172 6773  ebug_lang_kwargs
-0003a3c0: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
-0003a3d0: 6672 6f6d 5f6c 616e 6775 6167 6520 3d3d  from_language ==
-0003a3e0: 2027 6175 746f 273a 0d0a 2020 2020 2020   'auto':..      
-0003a3f0: 2020 2020 2020 6672 6f6d 5f6c 616e 6775        from_langu
-0003a400: 6167 6520 3d20 7365 6c66 2e77 6172 6e69  age = self.warni
-0003a410: 6e67 5f61 7574 6f5f 6c61 6e67 2827 7472  ng_auto_lang('tr
-0003a420: 616e 736c 6174 654d 6527 2c20 7365 6c66  anslateMe', self
-0003a430: 2e64 6566 6175 6c74 5f66 726f 6d5f 6c61  .default_from_la
-0003a440: 6e67 7561 6765 2c20 6966 5f70 7269 6e74  nguage, if_print
-0003a450: 5f77 6172 6e69 6e67 290d 0a20 2020 2020  _warning)..     
-0003a460: 2020 2066 726f 6d5f 6c61 6e67 7561 6765     from_language
-0003a470: 2c20 746f 5f6c 616e 6775 6167 6520 3d20  , to_language = 
-0003a480: 7365 6c66 2e63 6865 636b 5f6c 616e 6775  self.check_langu
-0003a490: 6167 6528 6672 6f6d 5f6c 616e 6775 6167  age(from_languag
-0003a4a0: 652c 2074 6f5f 6c61 6e67 7561 6765 2c20  e, to_language, 
-0003a4b0: 7365 6c66 2e6c 616e 6775 6167 655f 6d61  self.language_ma
-0003a4c0: 702c 206f 7574 7075 745f 7a68 3d73 656c  p, output_zh=sel
-0003a4d0: 662e 6f75 7470 7574 5f7a 682c 0d0a 2020  f.output_zh,..  
-0003a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003a510: 2020 2020 2020 206f 7574 7075 745f 656e         output_en
-0003a520: 5f74 7261 6e73 6c61 746f 723d 2774 7261  _translator='tra
-0003a530: 6e73 6c61 7465 4d65 272c 206f 7574 7075  nslateMe', outpu
-0003a540: 745f 656e 3d73 656c 662e 6f75 7470 7574  t_en=self.output
-0003a550: 5f65 6e29 0d0a 0d0a 2020 2020 2020 2020  _en)....        
-0003a560: 6966 2073 656c 662e 6f75 7470 7574 5f65  if self.output_e
-0003a570: 6e20 696e 2028 6672 6f6d 5f6c 616e 6775  n in (from_langu
-0003a580: 6167 652c 2074 6f5f 6c61 6e67 7561 6765  age, to_language
-0003a590: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0003a5a0: 7265 7475 726e 2073 656c 662e 5f74 7261  return self._tra
-0003a5b0: 6e73 6c61 7465 4d65 5f61 7069 2871 7565  nslateMe_api(que
-0003a5c0: 7279 5f74 6578 742c 2066 726f 6d5f 6c61  ry_text, from_la
-0003a5d0: 6e67 7561 6765 2c20 746f 5f6c 616e 6775  nguage, to_langu
-0003a5e0: 6167 652c 202a 2a6b 7761 7267 7329 0d0a  age, **kwargs)..
-0003a5f0: 0d0a 2020 2020 2020 2020 746d 705f 6b77  ..        tmp_kw
-0003a600: 6172 6773 203d 206b 7761 7267 732e 636f  args = kwargs.co
-0003a610: 7079 2829 0d0a 2020 2020 2020 2020 746d  py()..        tm
-0003a620: 705f 6b77 6172 6773 2e75 7064 6174 6528  p_kwargs.update(
-0003a630: 7b27 6973 5f64 6574 6169 6c5f 7265 7375  {'is_detail_resu
-0003a640: 6c74 273a 2046 616c 7365 2c20 2769 665f  lt': False, 'if_
-0003a650: 7368 6f77 5f74 696d 655f 7374 6174 273a  show_time_stat':
-0003a660: 2046 616c 7365 7d29 0d0a 2020 2020 2020   False})..      
-0003a670: 2020 6e65 7874 5f71 7565 7279 5f74 6578    next_query_tex
-0003a680: 7420 3d20 7365 6c66 2e5f 7472 616e 736c  t = self._transl
-0003a690: 6174 654d 655f 6170 6928 7175 6572 795f  ateMe_api(query_
-0003a6a0: 7465 7874 2c20 6672 6f6d 5f6c 616e 6775  text, from_langu
-0003a6b0: 6167 652c 2073 656c 662e 6f75 7470 7574  age, self.output
-0003a6c0: 5f65 6e2c 202a 2a74 6d70 5f6b 7761 7267  _en, **tmp_kwarg
-0003a6d0: 7329 0d0a 2020 2020 2020 2020 7265 7475  s)..        retu
-0003a6e0: 726e 2073 656c 662e 5f74 7261 6e73 6c61  rn self._transla
-0003a6f0: 7465 4d65 5f61 7069 286e 6578 745f 7175  teMe_api(next_qu
-0003a700: 6572 795f 7465 7874 2c20 7365 6c66 2e6f  ery_text, self.o
-0003a710: 7574 7075 745f 656e 2c20 746f 5f6c 616e  utput_en, to_lan
-0003a720: 6775 6167 652c 202a 2a6b 7761 7267 7329  guage, **kwargs)
-0003a730: 0d0a 0d0a 0d0a 636c 6173 7320 456c 6961  ......class Elia
-0003a740: 2854 7365 293a 0d0a 2020 2020 6465 6620  (Tse):..    def 
-0003a750: 5f5f 696e 6974 5f5f 2873 656c 6629 3a0d  __init__(self):.
-0003a760: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-0003a770: 2e5f 5f69 6e69 745f 5f28 290d 0a20 2020  .__init__()..   
-0003a780: 2020 2020 2073 656c 662e 686f 7374 5f75       self.host_u
-0003a790: 726c 203d 2027 6874 7470 733a 2f2f 656c  rl = 'https://el
-0003a7a0: 6961 2e65 7573 2f74 7261 6e73 6c61 746f  ia.eus/translato
-0003a7b0: 7227 0d0a 2020 2020 2020 2020 7365 6c66  r'..        self
-0003a7c0: 2e61 7069 5f75 726c 203d 2027 6874 7470  .api_url = 'http
-0003a7d0: 733a 2f2f 656c 6961 2e65 7573 2f61 6a61  s://elia.eus/aja
-0003a7e0: 782f 7472 616e 736c 6174 655f 7374 7269  x/translate_stri
-0003a7f0: 6e67 270d 0a20 2020 2020 2020 2073 656c  ng'..        sel
-0003a800: 662e 6465 7465 6374 5f6c 616e 675f 7572  f.detect_lang_ur
-0003a810: 6c20 3d20 2768 7474 7073 3a2f 2f65 6c69  l = 'https://eli
-0003a820: 612e 6575 732f 616a 6178 2f6c 616e 6775  a.eus/ajax/langu
-0003a830: 6167 655f 6465 7465 6374 696f 6e27 0d0a  age_detection'..
-0003a840: 2020 2020 2020 2020 7365 6c66 2e68 6f73          self.hos
-0003a850: 745f 6865 6164 6572 7320 3d20 7365 6c66  t_headers = self
-0003a860: 2e67 6574 5f68 6561 6465 7273 2873 656c  .get_headers(sel
-0003a870: 662e 686f 7374 5f75 726c 2c20 6966 5f61  f.host_url, if_a
-0003a880: 7069 3d46 616c 7365 2c20 6966 5f72 6566  pi=False, if_ref
-0003a890: 6572 6572 5f66 6f72 5f68 6f73 743d 5472  erer_for_host=Tr
-0003a8a0: 7565 290d 0a20 2020 2020 2020 2073 656c  ue)..        sel
-0003a8b0: 662e 6170 695f 6865 6164 6572 7320 3d20  f.api_headers = 
-0003a8c0: 7365 6c66 2e67 6574 5f68 6561 6465 7273  self.get_headers
-0003a8d0: 2873 656c 662e 686f 7374 5f75 726c 2c20  (self.host_url, 
-0003a8e0: 6966 5f61 7069 3d54 7275 652c 2069 665f  if_api=True, if_
-0003a8f0: 616a 6178 5f66 6f72 5f61 7069 3d54 7275  ajax_for_api=Tru
-0003a900: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
-0003a910: 2e73 6573 7369 6f6e 203d 204e 6f6e 650d  .session = None.
-0003a920: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-0003a930: 6e67 7561 6765 5f6d 6170 203d 204e 6f6e  nguage_map = Non
-0003a940: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-0003a950: 7072 6f66 6573 7369 6f6e 616c 5f66 6965  professional_fie
-0003a960: 6c64 203d 204e 6f6e 650d 0a20 2020 2020  ld = None..     
-0003a970: 2020 2073 656c 662e 6c61 6e67 7061 6972     self.langpair
-0003a980: 5f64 6f6d 6169 6e20 3d20 4e6f 6e65 0d0a  _domain = None..
-0003a990: 2020 2020 2020 2020 7365 6c66 2e74 6f6b          self.tok
-0003a9a0: 656e 203d 204e 6f6e 650d 0a20 2020 2020  en = None..     
-0003a9b0: 2020 2073 656c 662e 7175 6572 795f 636f     self.query_co
-0003a9c0: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
-0003a9d0: 2073 656c 662e 6f75 7470 7574 5f7a 6820   self.output_zh 
-0003a9e0: 3d20 4e6f 6e65 2020 2320 756e 7375 7070  = None  # unsupp
-0003a9f0: 6f72 7465 640d 0a20 2020 2020 2020 2073  orted..        s
-0003aa00: 656c 662e 696e 7075 745f 6c69 6d69 7420  elf.input_limit 
-0003aa10: 3d20 696e 7428 3165 3229 0d0a 2020 2020  = int(1e2)..    
-0003aa20: 2020 2020 7365 6c66 2e64 6566 6175 6c74      self.default
-0003aa30: 5f66 726f 6d5f 6c61 6e67 7561 6765 203d  _from_language =
-0003aa40: 2027 6672 270d 0a0d 0a20 2020 2040 5473   'fr'....    @Ts
-0003aa50: 652e 6465 6275 675f 6c61 6e67 7561 6765  e.debug_language
-0003aa60: 5f6d 6170 0d0a 2020 2020 6465 6620 6765  _map..    def ge
-0003aa70: 745f 6c61 6e67 7561 6765 5f6d 6170 2873  t_language_map(s
-0003aa80: 656c 662c 2064 643a 2064 6963 742c 202a  elf, dd: dict, *
-0003aa90: 2a6b 7761 7267 733a 204c 616e 674d 6170  *kwargs: LangMap
-0003aaa0: 4b77 6172 6773 5479 7065 2920 2d3e 2064  KwargsType) -> d
-0003aab0: 6963 743a 0d0a 2020 2020 2020 2020 7265  ict:..        re
-0003aac0: 7475 726e 207b 6969 5b27 736f 7572 6365  turn {ii['source
-0003aad0: 5f6c 616e 6775 6167 6527 5d5b 2763 6f64  _language']['cod
-0003aae0: 6527 5d3a 205b 6a6a 5b27 7461 7267 6574  e']: [jj['target
-0003aaf0: 5f6c 616e 6775 6167 6527 5d5b 2763 6f64  _language']['cod
-0003ab00: 6527 5d20 666f 7220 6a6a 2069 6e20 6464  e'] for jj in dd
-0003ab10: 5b27 6c61 6e67 7561 6765 5f70 6169 7273  ['language_pairs
-0003ab20: 275d 2069 6620 6a6a 5b27 736f 7572 6365  '] if jj['source
-0003ab30: 5f6c 616e 6775 6167 6527 5d5b 2763 6f64  _language']['cod
-0003ab40: 6527 5d20 3d3d 2069 695b 2773 6f75 7263  e'] == ii['sourc
-0003ab50: 655f 6c61 6e67 7561 6765 275d 5b27 636f  e_language']['co
-0003ab60: 6465 275d 5d20 666f 7220 6969 2069 6e20  de']] for ii in 
-0003ab70: 6464 5b27 6c61 6e67 7561 6765 5f70 6169  dd['language_pai
-0003ab80: 7273 275d 7d0d 0a0d 0a20 2020 2064 6566  rs']}....    def
-0003ab90: 2067 6574 5f70 726f 6665 7373 696f 6e61   get_professiona
-0003aba0: 6c5f 6669 656c 645f 6c69 7374 2873 656c  l_field_list(sel
-0003abb0: 662c 2064 643a 2064 6963 7429 202d 3e20  f, dd: dict) -> 
-0003abc0: 7365 743a 0d0a 2020 2020 2020 2020 7265  set:..        re
-0003abd0: 7475 726e 207b 6974 5b27 7472 616e 736c  turn {it['transl
-0003abe0: 6174 696f 6e5f 6d6f 6465 6c27 5d5b 2763  ation_model']['c
-0003abf0: 6f64 6527 5d20 666f 7220 6974 2069 6e20  ode'] for it in 
-0003ac00: 6464 5b27 6c61 6e67 7561 6765 5f70 6169  dd['language_pai
-0003ac10: 7273 275d 7d0d 0a0d 0a20 2020 2064 6566  rs']}....    def
-0003ac20: 2067 6574 5f6c 616e 6770 6169 725f 646f   get_langpair_do
-0003ac30: 6d61 696e 2873 656c 662c 2064 643a 2064  main(self, dd: d
-0003ac40: 6963 7429 202d 3e20 6469 6374 3a0d 0a20  ict) -> dict:.. 
-0003ac50: 2020 2020 2020 2064 6174 6120 3d20 7b0d         data = {.
-0003ac60: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
-0003ac70: 6974 656d 5b22 736f 7572 6365 5f6c 616e  item["source_lan
-0003ac80: 6775 6167 6522 5d5b 2263 6f64 6522 5d7d  guage"]["code"]}
-0003ac90: 5f5f 7b69 7465 6d5b 2274 6172 6765 745f  __{item["target_
-0003aca0: 6c61 6e67 7561 6765 225d 5b22 636f 6465  language"]["code
-0003acb0: 225d 7d5f 5f7b 6974 656d 5b22 7472 616e  "]}__{item["tran
-0003acc0: 736c 6174 696f 6e5f 6d6f 6465 6c22 5d5b  slation_model"][
-0003acd0: 2263 6f64 6522 5d7d 273a 207b 0d0a 2020  "code"]}': {..  
-0003ace0: 2020 2020 2020 2020 2020 2020 2020 2774                't
-0003acf0: 7261 6e73 6c61 7469 6f6e 5f65 6e67 696e  ranslation_engin
-0003ad00: 6527 3a20 6974 656d 5b22 656e 6769 6e65  e': item["engine
-0003ad10: 225d 5b22 706b 225d 2c0d 0a20 2020 2020  "]["pk"],..     
-0003ad20: 2020 2020 2020 207d 2066 6f72 2069 7465         } for ite
-0003ad30: 6d20 696e 2064 645b 276c 616e 6775 6167  m in dd['languag
-0003ad40: 655f 7061 6972 7327 5d0d 0a20 2020 2020  e_pairs']..     
-0003ad50: 2020 207d 0d0a 2020 2020 2020 2020 7265     }..        re
-0003ad60: 7475 726e 2064 6174 610d 0a0d 0a20 2020  turn data....   
-0003ad70: 2040 5473 652e 7469 6d65 5f73 7461 740d   @Tse.time_stat.
-0003ad80: 0a20 2020 2040 5473 652e 6368 6563 6b5f  .    @Tse.check_
-0003ad90: 7175 6572 790d 0a20 2020 2064 6566 2065  query..    def e
-0003ada0: 6c69 615f 6170 6928 7365 6c66 2c20 7175  lia_api(self, qu
-0003adb0: 6572 795f 7465 7874 3a20 7374 722c 2066  ery_text: str, f
-0003adc0: 726f 6d5f 6c61 6e67 7561 6765 3a20 7374  rom_language: st
-0003add0: 7220 3d20 2761 7574 6f27 2c20 746f 5f6c  r = 'auto', to_l
-0003ade0: 616e 6775 6167 653a 2073 7472 203d 2027  anguage: str = '
-0003adf0: 656e 272c 202a 2a6b 7761 7267 733a 2041  en', **kwargs: A
-0003ae00: 7069 4b77 6172 6773 5479 7065 2920 2d3e  piKwargsType) ->
-0003ae10: 2055 6e69 6f6e 5b73 7472 2c20 6469 6374   Union[str, dict
-0003ae20: 5d3a 0d0a 2020 2020 2020 2020 2222 220d  ]:..        """.
-0003ae30: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
-0003ae40: 2f65 6c69 612e 6575 732f 7472 616e 736c  /elia.eus/transl
-0003ae50: 6174 6f72 0d0a 2020 2020 2020 2020 3a70  ator..        :p
-0003ae60: 6172 616d 2071 7565 7279 5f74 6578 743a  aram query_text:
-0003ae70: 2073 7472 2c20 6d75 7374 2e0d 0a20 2020   str, must...   
-0003ae80: 2020 2020 203a 7061 7261 6d20 6672 6f6d       :param from
-0003ae90: 5f6c 616e 6775 6167 653a 2073 7472 2c20  _language: str, 
-0003aea0: 6465 6661 756c 7420 2761 7574 6f27 2e0d  default 'auto'..
-0003aeb0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0003aec0: 746f 5f6c 616e 6775 6167 653a 2073 7472  to_language: str
-0003aed0: 2c20 6465 6661 756c 7420 2765 6e27 2e0d  , default 'en'..
-0003aee0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0003aef0: 2a2a 6b77 6172 6773 3a0d 0a20 2020 2020  **kwargs:..     
-0003af00: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-0003af10: 6d20 7469 6d65 6f75 743a 2066 6c6f 6174  m timeout: float
-0003af20: 2c20 6465 6661 756c 7420 4e6f 6e65 2e0d  , default None..
-0003af30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003af40: 203a 7061 7261 6d20 7072 6f78 6965 733a   :param proxies:
-0003af50: 2064 6963 742c 2064 6566 6175 6c74 204e   dict, default N
-0003af60: 6f6e 652e 0d0a 2020 2020 2020 2020 2020  one...          
-0003af70: 2020 2020 2020 3a70 6172 616d 2073 6c65        :param sle
-0003af80: 6570 5f73 6563 6f6e 6473 3a20 666c 6f61  ep_seconds: floa
-0003af90: 742c 2064 6566 6175 6c74 2030 2e0d 0a20  t, default 0... 
-0003afa0: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-0003afb0: 7061 7261 6d20 6973 5f64 6574 6169 6c5f  param is_detail_
-0003afc0: 7265 7375 6c74 3a20 626f 6f6c 2c20 6465  result: bool, de
-0003afd0: 6661 756c 7420 4661 6c73 652e 0d0a 2020  fault False...  
-0003afe0: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-0003aff0: 6172 616d 2069 665f 6967 6e6f 7265 5f6c  aram if_ignore_l
-0003b000: 696d 6974 5f6f 665f 6c65 6e67 7468 3a20  imit_of_length: 
-0003b010: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-0003b020: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
-0003b030: 2020 2020 2020 3a70 6172 616d 206c 696d        :param lim
-0003b040: 6974 5f6f 665f 6c65 6e67 7468 3a20 696e  it_of_length: in
-0003b050: 742c 2064 6566 6175 6c74 2032 3030 3030  t, default 20000
-0003b060: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0003b070: 2020 203a 7061 7261 6d20 6966 5f69 676e     :param if_ign
-0003b080: 6f72 655f 656d 7074 795f 7175 6572 793a  ore_empty_query:
-0003b090: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
-0003b0a0: 616c 7365 2e0d 0a20 2020 2020 2020 2020  alse...         
-0003b0b0: 2020 2020 2020 203a 7061 7261 6d20 7570         :param up
-0003b0c0: 6461 7465 5f73 6573 7369 6f6e 5f61 6674  date_session_aft
-0003b0d0: 6572 5f66 7265 713a 2069 6e74 2c20 6465  er_freq: int, de
-0003b0e0: 6661 756c 7420 3130 3030 2e0d 0a20 2020  fault 1000...   
-0003b0f0: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-0003b100: 7261 6d20 7570 6461 7465 5f73 6573 7369  ram update_sessi
-0003b110: 6f6e 5f61 6674 6572 5f73 6563 6f6e 6473  on_after_seconds
-0003b120: 3a20 666c 6f61 742c 2064 6566 6175 6c74  : float, default
-0003b130: 2031 3530 302e 0d0a 2020 2020 2020 2020   1500...        
-0003b140: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-0003b150: 665f 7368 6f77 5f74 696d 655f 7374 6174  f_show_time_stat
-0003b160: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-0003b170: 4661 6c73 652e 0d0a 2020 2020 2020 2020  False...        
-0003b180: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-0003b190: 686f 775f 7469 6d65 5f73 7461 745f 7072  how_time_stat_pr
-0003b1a0: 6563 6973 696f 6e3a 2069 6e74 2c20 6465  ecision: int, de
-0003b1b0: 6661 756c 7420 322e 0d0a 2020 2020 2020  fault 2...      
-0003b1c0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-0003b1d0: 2069 665f 7072 696e 745f 7761 726e 696e   if_print_warnin
-0003b1e0: 673a 2062 6f6f 6c2c 2064 6566 6175 6c74  g: bool, default
-0003b1f0: 2054 7275 652e 0d0a 2020 2020 2020 2020   True...        
-0003b200: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-0003b210: 726f 6665 7373 696f 6e61 6c5f 6669 656c  rofessional_fiel
-0003b220: 643a 2073 7472 2c20 6465 6661 756c 7420  d: str, default 
-0003b230: 2767 656e 6572 616c 272e 2043 686f 6f73  'general'. Choos
-0003b240: 6520 6672 6f6d 2028 2767 656e 6572 616c  e from ('general
-0003b250: 272c 2027 6164 6d69 6e27 292e 0d0a 2020  ', 'admin')...  
-0003b260: 2020 2020 2020 3a72 6574 7572 6e3a 2073        :return: s
-0003b270: 7472 206f 7220 6469 6374 0d0a 2020 2020  tr or dict..    
-0003b280: 2020 2020 2222 220d 0a0d 0a20 2020 2020      """....     
-0003b290: 2020 2075 7365 5f64 6f6d 6169 6e20 3d20     use_domain = 
-0003b2a0: 6b77 6172 6773 2e67 6574 2827 7072 6f66  kwargs.get('prof
-0003b2b0: 6573 7369 6f6e 616c 5f66 6965 6c64 272c  essional_field',
-0003b2c0: 2027 6765 6e65 7261 6c27 290d 0a20 2020   'general')..   
-0003b2d0: 2020 2020 2074 696d 656f 7574 203d 206b       timeout = k
-0003b2e0: 7761 7267 732e 6765 7428 2774 696d 656f  wargs.get('timeo
-0003b2f0: 7574 272c 204e 6f6e 6529 0d0a 2020 2020  ut', None)..    
-0003b300: 2020 2020 7072 6f78 6965 7320 3d20 6b77      proxies = kw
-0003b310: 6172 6773 2e67 6574 2827 7072 6f78 6965  args.get('proxie
-0003b320: 7327 2c20 4e6f 6e65 290d 0a20 2020 2020  s', None)..     
-0003b330: 2020 2073 6c65 6570 5f73 6563 6f6e 6473     sleep_seconds
-0003b340: 203d 206b 7761 7267 732e 6765 7428 2773   = kwargs.get('s
-0003b350: 6c65 6570 5f73 6563 6f6e 6473 272c 2030  leep_seconds', 0
-0003b360: 290d 0a20 2020 2020 2020 2069 665f 7072  )..        if_pr
-0003b370: 696e 745f 7761 726e 696e 6720 3d20 6b77  int_warning = kw
-0003b380: 6172 6773 2e67 6574 2827 6966 5f70 7269  args.get('if_pri
-0003b390: 6e74 5f77 6172 6e69 6e67 272c 2054 7275  nt_warning', Tru
-0003b3a0: 6529 0d0a 2020 2020 2020 2020 6973 5f64  e)..        is_d
-0003b3b0: 6574 6169 6c5f 7265 7375 6c74 203d 206b  etail_result = k
-0003b3c0: 7761 7267 732e 6765 7428 2769 735f 6465  wargs.get('is_de
-0003b3d0: 7461 696c 5f72 6573 756c 7427 2c20 4661  tail_result', Fa
-0003b3e0: 6c73 6529 0d0a 2020 2020 2020 2020 7570  lse)..        up
-0003b3f0: 6461 7465 5f73 6573 7369 6f6e 5f61 6674  date_session_aft
-0003b400: 6572 5f66 7265 7120 3d20 6b77 6172 6773  er_freq = kwargs
-0003b410: 2e67 6574 2827 7570 6461 7465 5f73 6573  .get('update_ses
-0003b420: 7369 6f6e 5f61 6674 6572 5f66 7265 7127  sion_after_freq'
-0003b430: 2c20 7365 6c66 2e64 6566 6175 6c74 5f73  , self.default_s
-0003b440: 6573 7369 6f6e 5f66 7265 7129 0d0a 2020  ession_freq)..  
-0003b450: 2020 2020 2020 7570 6461 7465 5f73 6573        update_ses
-0003b460: 7369 6f6e 5f61 6674 6572 5f73 6563 6f6e  sion_after_secon
-0003b470: 6473 203d 206b 7761 7267 732e 6765 7428  ds = kwargs.get(
-0003b480: 2775 7064 6174 655f 7365 7373 696f 6e5f  'update_session_
-0003b490: 6166 7465 725f 7365 636f 6e64 7327 2c20  after_seconds', 
-0003b4a0: 7365 6c66 2e64 6566 6175 6c74 5f73 6573  self.default_ses
-0003b4b0: 7369 6f6e 5f73 6563 6f6e 6473 290d 0a20  sion_seconds).. 
-0003b4c0: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
-0003b4d0: 6b5f 696e 7075 745f 6c69 6d69 7428 7175  k_input_limit(qu
-0003b4e0: 6572 795f 7465 7874 2c20 7365 6c66 2e69  ery_text, self.i
-0003b4f0: 6e70 7574 5f6c 696d 6974 290d 0a0d 0a20  nput_limit).... 
-0003b500: 2020 2020 2020 206e 6f74 5f75 7064 6174         not_updat
-0003b510: 655f 636f 6e64 5f66 7265 7120 3d20 3120  e_cond_freq = 1 
-0003b520: 6966 2073 656c 662e 7175 6572 795f 636f  if self.query_co
-0003b530: 756e 7420 3c20 7570 6461 7465 5f73 6573  unt < update_ses
-0003b540: 7369 6f6e 5f61 6674 6572 5f66 7265 7120  sion_after_freq 
-0003b550: 656c 7365 2030 0d0a 2020 2020 2020 2020  else 0..        
-0003b560: 6e6f 745f 7570 6461 7465 5f63 6f6e 645f  not_update_cond_
-0003b570: 7469 6d65 203d 2031 2069 6620 7469 6d65  time = 1 if time
-0003b580: 2e74 696d 6528 2920 2d20 7365 6c66 2e62  .time() - self.b
-0003b590: 6567 696e 5f74 696d 6520 3c20 7570 6461  egin_time < upda
-0003b5a0: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
-0003b5b0: 5f73 6563 6f6e 6473 2065 6c73 6520 300d  _seconds else 0.
-0003b5c0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0003b5d0: 2873 656c 662e 7365 7373 696f 6e20 616e  (self.session an
-0003b5e0: 6420 7365 6c66 2e6c 616e 6775 6167 655f  d self.language_
-0003b5f0: 6d61 7020 616e 6420 6e6f 745f 7570 6461  map and not_upda
-0003b600: 7465 5f63 6f6e 645f 6672 6571 2061 6e64  te_cond_freq and
-0003b610: 206e 6f74 5f75 7064 6174 655f 636f 6e64   not_update_cond
-0003b620: 5f74 696d 6529 3a0d 0a20 2020 2020 2020  _time):..       
-0003b630: 2020 2020 2073 656c 662e 7365 7373 696f       self.sessio
-0003b640: 6e20 3d20 7265 7175 6573 7473 2e53 6573  n = requests.Ses
-0003b650: 7369 6f6e 2829 0d0a 2020 2020 2020 2020  sion()..        
-0003b660: 2020 2020 686f 7374 5f68 746d 6c20 3d20      host_html = 
-0003b670: 7365 6c66 2e73 6573 7369 6f6e 2e67 6574  self.session.get
-0003b680: 2873 656c 662e 686f 7374 5f75 726c 2c20  (self.host_url, 
-0003b690: 6865 6164 6572 733d 7365 6c66 2e68 6f73  headers=self.hos
-0003b6a0: 745f 6865 6164 6572 732c 2074 696d 656f  t_headers, timeo
-0003b6b0: 7574 3d74 696d 656f 7574 2c20 7072 6f78  ut=timeout, prox
-0003b6c0: 6965 733d 7072 6f78 6965 7329 2e74 6578  ies=proxies).tex
-0003b6d0: 740d 0a20 2020 2020 2020 2020 2020 2073  t..            s
-0003b6e0: 656c 662e 746f 6b65 6e20 3d20 7265 2e63  elf.token = re.c
-0003b6f0: 6f6d 7069 6c65 2827 2263 7372 666d 6964  ompile('"csrfmid
-0003b700: 646c 6577 6172 6574 6f6b 656e 223a 2022  dlewaretoken": "
-0003b710: 282e 2a3f 2922 2729 2e73 6561 7263 6828  (.*?)"').search(
-0003b720: 686f 7374 5f68 746d 6c29 2e67 726f 7570  host_html).group
-0003b730: 2831 290d 0a20 2020 2020 2020 2020 2020  (1)..           
-0003b740: 2064 5f6c 616e 675f 7374 7220 3d20 7265   d_lang_str = re
-0003b750: 2e63 6f6d 7069 6c65 2827 7661 7220 6c61  .compile('var la
-0003b760: 6e67 7561 6765 5061 6972 7320 3d20 4a53  nguagePairs = JS
-0003b770: 4f4e 2e70 6172 7365 5c5c 2828 2e2a 3f29  ON.parse\\((.*?)
-0003b780: 5c5c 293b 2729 2e73 6561 7263 6828 686f  \\);').search(ho
-0003b790: 7374 5f68 746d 6c29 2e67 726f 7570 2829  st_html).group()
-0003b7a0: 0d0a 2020 2020 2020 2020 2020 2020 645f  ..            d_
-0003b7b0: 6c61 6e67 5f6d 6170 203d 206a 736f 6e2e  lang_map = json.
-0003b7c0: 6c6f 6164 7328 645f 6c61 6e67 5f73 7472  loads(d_lang_str
-0003b7d0: 5b34 333a 2d34 5d2e 7265 706c 6163 6528  [43:-4].replace(
-0003b7e0: 2726 7175 6f74 3b27 2c20 2722 2729 290d  '&quot;', '"')).
-0003b7f0: 0a20 2020 2020 2020 2020 2020 2064 6562  .            deb
-0003b800: 7567 5f6c 616e 675f 6b77 6172 6773 203d  ug_lang_kwargs =
-0003b810: 2073 656c 662e 6465 6275 675f 6c61 6e67   self.debug_lang
-0003b820: 5f6b 7761 7267 7328 6672 6f6d 5f6c 616e  _kwargs(from_lan
-0003b830: 6775 6167 652c 2074 6f5f 6c61 6e67 7561  guage, to_langua
-0003b840: 6765 2c20 7365 6c66 2e64 6566 6175 6c74  ge, self.default
-0003b850: 5f66 726f 6d5f 6c61 6e67 7561 6765 2c20  _from_language, 
-0003b860: 6966 5f70 7269 6e74 5f77 6172 6e69 6e67  if_print_warning
-0003b870: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0003b880: 656c 662e 6c61 6e67 7561 6765 5f6d 6170  elf.language_map
-0003b890: 203d 2073 656c 662e 6765 745f 6c61 6e67   = self.get_lang
-0003b8a0: 7561 6765 5f6d 6170 2864 5f6c 616e 675f  uage_map(d_lang_
-0003b8b0: 6d61 702c 202a 2a64 6562 7567 5f6c 616e  map, **debug_lan
-0003b8c0: 675f 6b77 6172 6773 290d 0a20 2020 2020  g_kwargs)..     
-0003b8d0: 2020 2020 2020 2073 656c 662e 7072 6f66         self.prof
-0003b8e0: 6573 7369 6f6e 616c 5f66 6965 6c64 203d  essional_field =
-0003b8f0: 2073 656c 662e 6765 745f 7072 6f66 6573   self.get_profes
-0003b900: 7369 6f6e 616c 5f66 6965 6c64 5f6c 6973  sional_field_lis
-0003b910: 7428 645f 6c61 6e67 5f6d 6170 290d 0a20  t(d_lang_map).. 
-0003b920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0003b930: 6c61 6e67 7061 6972 5f64 6f6d 6169 6e20  langpair_domain 
-0003b940: 3d20 7365 6c66 2e67 6574 5f6c 616e 6770  = self.get_langp
-0003b950: 6169 725f 646f 6d61 696e 2864 5f6c 616e  air_domain(d_lan
-0003b960: 675f 6d61 7029 0d0a 0d0a 2020 2020 2020  g_map)....      
-0003b970: 2020 6966 2066 726f 6d5f 6c61 6e67 7561    if from_langua
-0003b980: 6765 203d 3d20 2761 7574 6f27 3a0d 0a20  ge == 'auto':.. 
-0003b990: 2020 2020 2020 2020 2020 2070 6179 6c6f             paylo
-0003b9a0: 6164 203d 207b 0d0a 2020 2020 2020 2020  ad = {..        
-0003b9b0: 2020 2020 2020 2020 2774 6578 7427 3a20          'text': 
-0003b9c0: 7175 6572 795f 7465 7874 2c0d 0a20 2020  query_text,..   
-0003b9d0: 2020 2020 2020 2020 2020 2020 2027 6373               'cs
-0003b9e0: 7266 6d69 6464 6c65 7761 7265 746f 6b65  rfmiddlewaretoke
-0003b9f0: 6e27 3a20 7365 6c66 2e74 6f6b 656e 2c0d  n': self.token,.
-0003ba00: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
-0003ba10: 2020 2020 2020 2020 2020 2020 7061 796c              payl
-0003ba20: 6f61 6420 3d20 7572 6c6c 6962 2e70 6172  oad = urllib.par
-0003ba30: 7365 2e75 726c 656e 636f 6465 2870 6179  se.urlencode(pay
-0003ba40: 6c6f 6164 290d 0a20 2020 2020 2020 2020  load)..         
-0003ba50: 2020 2072 203d 2073 656c 662e 7365 7373     r = self.sess
-0003ba60: 696f 6e2e 706f 7374 2873 656c 662e 6465  ion.post(self.de
-0003ba70: 7465 6374 5f6c 616e 675f 7572 6c2c 2064  tect_lang_url, d
-0003ba80: 6174 613d 7061 796c 6f61 642c 2068 6561  ata=payload, hea
-0003ba90: 6465 7273 3d73 656c 662e 6170 695f 6865  ders=self.api_he
-0003baa0: 6164 6572 732c 2074 696d 656f 7574 3d74  aders, timeout=t
-0003bab0: 696d 656f 7574 2c20 7072 6f78 6965 733d  imeout, proxies=
-0003bac0: 7072 6f78 6965 7329 0d0a 2020 2020 2020  proxies)..      
-0003bad0: 2020 2020 2020 6672 6f6d 5f6c 616e 6775        from_langu
-0003bae0: 6167 6520 3d20 722e 6a73 6f6e 2829 5b27  age = r.json()['
-0003baf0: 6c61 6e67 5f69 6427 5d0d 0a20 2020 2020  lang_id']..     
-0003bb00: 2020 2066 726f 6d5f 6c61 6e67 7561 6765     from_language
-0003bb10: 2c20 746f 5f6c 616e 6775 6167 6520 3d20  , to_language = 
-0003bb20: 7365 6c66 2e63 6865 636b 5f6c 616e 6775  self.check_langu
-0003bb30: 6167 6528 6672 6f6d 5f6c 616e 6775 6167  age(from_languag
-0003bb40: 652c 2074 6f5f 6c61 6e67 7561 6765 2c20  e, to_language, 
-0003bb50: 7365 6c66 2e6c 616e 6775 6167 655f 6d61  self.language_ma
-0003bb60: 7029 0d0a 0d0a 2020 2020 2020 2020 7061  p)....        pa
-0003bb70: 796c 6f61 6420 3d20 7b0d 0a20 2020 2020  yload = {..     
-0003bb80: 2020 2020 2020 2027 696e 7075 745f 7465         'input_te
-0003bb90: 7874 273a 2071 7565 7279 5f74 6578 742c  xt': query_text,
-0003bba0: 0d0a 2020 2020 2020 2020 2020 2020 2773  ..            's
-0003bbb0: 6f75 7263 655f 6c61 6e67 7561 6765 273a  ource_language':
-0003bbc0: 2066 726f 6d5f 6c61 6e67 7561 6765 2c0d   from_language,.
-0003bbd0: 0a20 2020 2020 2020 2020 2020 2027 7461  .            'ta
-0003bbe0: 7267 6574 5f6c 616e 6775 6167 6527 3a20  rget_language': 
-0003bbf0: 746f 5f6c 616e 6775 6167 652c 0d0a 2020  to_language,..  
-0003bc00: 2020 2020 2020 2020 2020 2774 7261 6e73            'trans
-0003bc10: 6c61 7469 6f6e 5f6d 6f64 656c 273a 2075  lation_model': u
-0003bc20: 7365 5f64 6f6d 6169 6e2c 0d0a 2020 2020  se_domain,..    
-0003bc30: 2020 2020 2020 2020 2774 7261 6e73 6c61          'transla
-0003bc40: 7469 6f6e 5f65 6e67 696e 6527 3a20 312c  tion_engine': 1,
-0003bc50: 0d0a 2020 2020 2020 2020 2020 2020 2763  ..            'c
-0003bc60: 7372 666d 6964 646c 6577 6172 6574 6f6b  srfmiddlewaretok
-0003bc70: 656e 273a 2073 656c 662e 746f 6b65 6e2c  en': self.token,
-0003bc80: 0d0a 2020 2020 2020 2020 7d0d 0a0d 0a20  ..        }.... 
-0003bc90: 2020 2020 2020 2064 6f6d 6169 6e5f 7061         domain_pa
-0003bca0: 796c 6f61 6420 3d20 7365 6c66 2e6c 616e  yload = self.lan
-0003bcb0: 6770 6169 725f 646f 6d61 696e 2e67 6574  gpair_domain.get
-0003bcc0: 2866 277b 6672 6f6d 5f6c 616e 6775 6167  (f'{from_languag
-0003bcd0: 657d 5f5f 7b74 6f5f 6c61 6e67 7561 6765  e}__{to_language
-0003bce0: 7d5f 5f7b 7573 655f 646f 6d61 696e 7d27  }__{use_domain}'
-0003bcf0: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-0003bd00: 7420 646f 6d61 696e 5f70 6179 6c6f 6164  t domain_payload
-0003bd10: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0003bd20: 6169 7365 2054 7261 6e73 6c61 746f 7245  aise TranslatorE
-0003bd30: 7272 6f72 0d0a 2020 2020 2020 2020 656c  rror..        el
-0003bd40: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0003bd50: 2070 6179 6c6f 6164 2e75 7064 6174 6528   payload.update(
-0003bd60: 646f 6d61 696e 5f70 6179 6c6f 6164 290d  domain_payload).
-0003bd70: 0a0d 0a20 2020 2020 2020 2070 6179 6c6f  ...        paylo
-0003bd80: 6164 203d 2075 726c 6c69 622e 7061 7273  ad = urllib.pars
-0003bd90: 652e 7572 6c65 6e63 6f64 6528 7061 796c  e.urlencode(payl
-0003bda0: 6f61 6429 0d0a 2020 2020 2020 2020 7220  oad)..        r 
-0003bdb0: 3d20 7365 6c66 2e73 6573 7369 6f6e 2e70  = self.session.p
-0003bdc0: 6f73 7428 7365 6c66 2e61 7069 5f75 726c  ost(self.api_url
-0003bdd0: 2c20 6461 7461 3d70 6179 6c6f 6164 2c20  , data=payload, 
-0003bde0: 6865 6164 6572 733d 7365 6c66 2e61 7069  headers=self.api
-0003bdf0: 5f68 6561 6465 7273 2c20 7469 6d65 6f75  _headers, timeou
-0003be00: 743d 7469 6d65 6f75 742c 2070 726f 7869  t=timeout, proxi
-0003be10: 6573 3d70 726f 7869 6573 290d 0a20 2020  es=proxies)..   
-0003be20: 2020 2020 2072 2e72 6169 7365 5f66 6f72       r.raise_for
-0003be30: 5f73 7461 7475 7328 290d 0a20 2020 2020  _status()..     
-0003be40: 2020 2064 6174 6120 3d20 722e 6a73 6f6e     data = r.json
-0003be50: 2829 0d0a 2020 2020 2020 2020 7469 6d65  ()..        time
-0003be60: 2e73 6c65 6570 2873 6c65 6570 5f73 6563  .sleep(sleep_sec
-0003be70: 6f6e 6473 290d 0a20 2020 2020 2020 2073  onds)..        s
-0003be80: 656c 662e 7175 6572 795f 636f 756e 7420  elf.query_count 
-0003be90: 2b3d 2031 0d0a 2020 2020 2020 2020 7265  += 1..        re
-0003bea0: 7475 726e 2064 6174 6120 6966 2069 735f  turn data if is_
-0003beb0: 6465 7461 696c 5f72 6573 756c 7420 656c  detail_result el
-0003bec0: 7365 2064 6174 615b 2774 7261 6e73 6c61  se data['transla
-0003bed0: 7465 645f 7465 7874 275d 2e72 6570 6c61  ted_text'].repla
-0003bee0: 6365 2827 3c2f 6469 763e 272c 2027 5c6e  ce('</div>', '\n
-0003bef0: 2729 2e72 6570 6c61 6365 2827 3c64 6976  ').replace('<div
-0003bf00: 3e27 2c20 2727 292e 7265 706c 6163 6528  >', '').replace(
-0003bf10: 273c 7370 616e 3e27 2c20 2727 292e 7265  '<span>', '').re
-0003bf20: 706c 6163 6528 273c 2f73 7061 6e3e 272c  place('</span>',
-0003bf30: 2027 2729 0d0a 0d0a 0d0a 636c 6173 7320   '')......class 
-0003bf40: 4c61 6e67 7561 6765 5769 7265 2854 7365  LanguageWire(Tse
-0003bf50: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-0003bf60: 6974 5f5f 2873 656c 6629 3a0d 0a20 2020  it__(self):..   
-0003bf70: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-0003bf80: 6e69 745f 5f28 290d 0a20 2020 2020 2020  nit__()..       
-0003bf90: 2073 656c 662e 686f 6d65 5f75 726c 203d   self.home_url =
-0003bfa0: 2027 6874 7470 733a 2f2f 6a77 742e 6c61   'https://jwt.la
-0003bfb0: 6e67 7561 6765 7769 7265 2e63 6f6d 270d  nguagewire.com'.
-0003bfc0: 0a20 2020 2020 2020 2073 656c 662e 686f  .        self.ho
-0003bfd0: 7374 5f75 726c 203d 2027 6874 7470 733a  st_url = 'https:
-0003bfe0: 2f2f 7777 772e 6c61 6e67 7561 6765 7769  //www.languagewi
-0003bff0: 7265 2e63 6f6d 2f65 6e2f 7465 6368 6e6f  re.com/en/techno
-0003c000: 6c6f 6779 2f6c 616e 6775 6167 6577 6972  logy/languagewir
-0003c010: 652d 7472 616e 736c 6174 6527 0d0a 2020  e-translate'..  
-0003c020: 2020 2020 2020 7365 6c66 2e61 7069 5f75        self.api_u
-0003c030: 726c 203d 2027 6874 7470 733a 2f2f 6c77  rl = 'https://lw
-0003c040: 742e 6c61 6e67 7561 6765 7769 7265 2e63  t.languagewire.c
-0003c050: 6f6d 2f66 2f61 7069 2f76 312f 7472 616e  om/f/api/v1/tran
-0003c060: 736c 6174 696f 6e73 2f74 6578 7427 0d0a  slations/text'..
-0003c070: 2020 2020 2020 2020 7365 6c66 2e6c 616e          self.lan
-0003c080: 675f 7572 6c20 3d20 2768 7474 7073 3a2f  g_url = 'https:/
-0003c090: 2f6c 7774 2e6c 616e 6775 6167 6577 6972  /lwt.languagewir
-0003c0a0: 652e 636f 6d2f 662f 6170 692f 7631 2f6c  e.com/f/api/v1/l
-0003c0b0: 616e 6775 6167 652d 7061 6972 733f 696e  anguage-pairs?in
-0003c0c0: 636c 7564 6556 6172 6961 6e74 733d 7472  cludeVariants=tr
-0003c0d0: 7565 270d 0a20 2020 2020 2020 2073 656c  ue'..        sel
-0003c0e0: 662e 636f 6f6b 6965 5f75 726c 203d 2027  f.cookie_url = '
-0003c0f0: 6874 7470 733a 2f2f 6c77 742e 6c61 6e67  https://lwt.lang
-0003c100: 7561 6765 7769 7265 2e63 6f6d 2f66 2f61  uagewire.com/f/a
-0003c110: 7069 2f76 312f 6175 7468 2f63 6f6f 6b69  pi/v1/auth/cooki
-0003c120: 6527 0d0a 2020 2020 2020 2020 7365 6c66  e'..        self
-0003c130: 2e6c 7774 5f6a 735f 7572 6c20 3d20 2768  .lwt_js_url = 'h
-0003c140: 7474 7073 3a2f 2f6c 7774 2e6c 616e 6775  ttps://lwt.langu
-0003c150: 6167 6577 6972 652e 636f 6d2f 656e 2f6d  agewire.com/en/m
-0003c160: 6169 6e2e 3666 3230 3239 3562 3130 3462  ain.6f20295b104b
-0003c170: 6335 3261 2e6a 7327 0d0a 2020 2020 2020  c52a.js'..      
-0003c180: 2020 7365 6c66 2e68 6f73 745f 6865 6164    self.host_head
-0003c190: 6572 7320 3d20 7365 6c66 2e67 6574 5f68  ers = self.get_h
-0003c1a0: 6561 6465 7273 2873 656c 662e 686f 6d65  eaders(self.home
-0003c1b0: 5f75 726c 2c20 6966 5f61 7069 3d46 616c  _url, if_api=Fal
-0003c1c0: 7365 2c20 6966 5f72 6566 6572 6572 5f66  se, if_referer_f
-0003c1d0: 6f72 5f68 6f73 743d 5472 7565 290d 0a20  or_host=True).. 
-0003c1e0: 2020 2020 2020 2073 656c 662e 6170 695f         self.api_
-0003c1f0: 6865 6164 6572 7320 3d20 7365 6c66 2e67  headers = self.g
-0003c200: 6574 5f68 6561 6465 7273 2873 656c 662e  et_headers(self.
-0003c210: 686f 6d65 5f75 726c 2c20 6966 5f61 7069  home_url, if_api
-0003c220: 3d54 7275 652c 2069 665f 6a73 6f6e 5f66  =True, if_json_f
-0003c230: 6f72 5f61 7069 3d54 7275 6529 0d0a 2020  or_api=True)..  
-0003c240: 2020 2020 2020 7365 6c66 2e73 6573 7369        self.sessi
-0003c250: 6f6e 203d 204e 6f6e 650d 0a20 2020 2020  on = None..     
-0003c260: 2020 2073 656c 662e 6c61 6e67 7561 6765     self.language
-0003c270: 5f6d 6170 203d 204e 6f6e 650d 0a20 2020  _map = None..   
-0003c280: 2020 2020 2073 656c 662e 6c77 745f 6461       self.lwt_da
-0003c290: 7461 203d 204e 6f6e 650d 0a20 2020 2020  ta = None..     
-0003c2a0: 2020 2073 656c 662e 7175 6572 795f 636f     self.query_co
-0003c2b0: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
-0003c2c0: 2073 656c 662e 6f75 7470 7574 5f7a 6820   self.output_zh 
-0003c2d0: 3d20 4e6f 6e65 2020 2320 756e 7375 7070  = None  # unsupp
-0003c2e0: 6f72 7465 640d 0a20 2020 2020 2020 2073  orted..        s
-0003c2f0: 656c 662e 696e 7075 745f 6c69 6d69 7420  elf.input_limit 
-0003c300: 3d20 696e 7428 3565 3329 0d0a 2020 2020  = int(5e3)..    
-0003c310: 2020 2020 7365 6c66 2e64 6566 6175 6c74      self.default
-0003c320: 5f66 726f 6d5f 6c61 6e67 7561 6765 203d  _from_language =
-0003c330: 2027 6672 270d 0a20 2020 2020 2020 2073   'fr'..        s
-0003c340: 656c 662e 6465 6661 756c 745f 656e 5f74  elf.default_en_t
-0003c350: 6f5f 6c61 6e67 7561 6765 203d 2027 656e  o_language = 'en
-0003c360: 2d55 5327 0d0a 0d0a 2020 2020 4054 7365  -US'....    @Tse
-0003c370: 2e64 6562 7567 5f6c 616e 6775 6167 655f  .debug_language_
-0003c380: 6d61 700d 0a20 2020 2064 6566 2067 6574  map..    def get
-0003c390: 5f6c 616e 6775 6167 655f 6d61 7028 7365  _language_map(se
-0003c3a0: 6c66 2c20 6c61 6e67 5f75 726c 3a20 7374  lf, lang_url: st
-0003c3b0: 722c 2073 733a 2053 6573 7369 6f6e 5479  r, ss: SessionTy
-0003c3c0: 7065 2c20 6865 6164 6572 733a 2064 6963  pe, headers: dic
-0003c3d0: 742c 2074 696d 656f 7574 3a20 4f70 7469  t, timeout: Opti
-0003c3e0: 6f6e 616c 5b66 6c6f 6174 5d2c 2070 726f  onal[float], pro
-0003c3f0: 7869 6573 3a20 4f70 7469 6f6e 616c 5b64  xies: Optional[d
-0003c400: 6963 745d 2c20 2a2a 6b77 6172 6773 3a20  ict], **kwargs: 
-0003c410: 4c61 6e67 4d61 704b 7761 7267 7354 7970  LangMapKwargsTyp
-0003c420: 6529 202d 3e20 6469 6374 3a0d 0a20 2020  e) -> dict:..   
-0003c430: 2020 2020 2064 5f6c 616e 675f 6d61 7020       d_lang_map 
-0003c440: 3d20 7373 2e67 6574 286c 616e 675f 7572  = ss.get(lang_ur
-0003c450: 6c2c 2068 6561 6465 7273 3d68 6561 6465  l, headers=heade
-0003c460: 7273 2c20 7469 6d65 6f75 743d 7469 6d65  rs, timeout=time
-0003c470: 6f75 742c 2070 726f 7869 6573 3d70 726f  out, proxies=pro
-0003c480: 7869 6573 292e 6a73 6f6e 2829 0d0a 2020  xies).json()..  
-0003c490: 2020 2020 2020 7265 7475 726e 207b 6969        return {ii
-0003c4a0: 5b27 736f 7572 6365 4c61 6e67 7561 6765  ['sourceLanguage
-0003c4b0: 275d 5b27 6d6d 7443 6f64 6527 5d3a 205b  ']['mmtCode']: [
-0003c4c0: 6a6a 5b27 7461 7267 6574 4c61 6e67 7561  jj['targetLangua
-0003c4d0: 6765 275d 5b27 6d6d 7443 6f64 6527 5d20  ge']['mmtCode'] 
-0003c4e0: 666f 7220 6a6a 2069 6e20 645f 6c61 6e67  for jj in d_lang
-0003c4f0: 5f6d 6170 2069 6620 6a6a 5b27 736f 7572  _map if jj['sour
-0003c500: 6365 4c61 6e67 7561 6765 275d 5b27 6d6d  ceLanguage']['mm
-0003c510: 7443 6f64 6527 5d20 3d3d 2069 695b 2773  tCode'] == ii['s
-0003c520: 6f75 7263 654c 616e 6775 6167 6527 5d5b  ourceLanguage'][
-0003c530: 276d 6d74 436f 6465 275d 5d20 666f 7220  'mmtCode']] for 
-0003c540: 6969 2069 6e20 645f 6c61 6e67 5f6d 6170  ii in d_lang_map
-0003c550: 7d0d 0a0d 0a20 2020 2023 2064 6566 2067  }....    # def g
-0003c560: 6574 5f6c 7774 5f64 6174 6128 7365 6c66  et_lwt_data(self
-0003c570: 2c20 6c77 745f 6a73 5f75 726c 3a20 7374  , lwt_js_url: st
-0003c580: 722c 2073 733a 2053 6573 7369 6f6e 5479  r, ss: SessionTy
-0003c590: 7065 2c20 6865 6164 6572 733a 2064 6963  pe, headers: dic
-0003c5a0: 742c 2074 696d 656f 7574 3a20 666c 6f61  t, timeout: floa
-0003c5b0: 742c 2070 726f 7869 6573 3a20 6469 6374  t, proxies: dict
-0003c5c0: 2920 2d3e 2064 6963 743a 0d0a 2020 2020  ) -> dict:..    
-0003c5d0: 2320 2020 2020 6a73 5f68 746d 6c20 3d20  #     js_html = 
-0003c5e0: 7373 2e67 6574 286c 7774 5f6a 735f 7572  ss.get(lwt_js_ur
-0003c5f0: 6c2c 2068 6561 6465 7273 3d68 6561 6465  l, headers=heade
-0003c600: 7273 2c20 7469 6d65 6f75 743d 7469 6d65  rs, timeout=time
-0003c610: 6f75 742c 2070 726f 7869 6573 3d70 726f  out, proxies=pro
-0003c620: 7869 6573 292e 7465 7874 0d0a 2020 2020  xies).text..    
-0003c630: 2320 2020 2020 6c77 745f 6461 7461 203d  #     lwt_data =
-0003c640: 207b 0d0a 2020 2020 2320 2020 2020 2020   {..    #       
-0003c650: 2020 2778 2d6c 7774 2d61 7070 6c69 6361    'x-lwt-applica
-0003c660: 7469 6f6e 2d69 6427 3a20 7265 2e63 6f6d  tion-id': re.com
-0003c670: 7069 6c65 2827 2258 2d4c 5754 2d41 7070  pile('"X-LWT-App
-0003c680: 6c69 6361 7469 6f6e 2d49 4422 3a22 282e  lication-ID":"(.
-0003c690: 2a3f 2922 2729 2e73 6561 7263 6828 6a73  *?)"').search(js
-0003c6a0: 5f68 746d 6c29 2e67 726f 7570 2831 292c  _html).group(1),
-0003c6b0: 0d0a 2020 2020 2320 2020 2020 2020 2020  ..    #         
-0003c6c0: 2778 2d6c 7774 2d62 7569 6c64 2d69 6427  'x-lwt-build-id'
-0003c6d0: 3a20 7265 2e63 6f6d 7069 6c65 2827 2258  : re.compile('"X
-0003c6e0: 2d4c 5754 2d42 7569 6c64 2d49 4422 3a22  -LWT-Build-ID":"
-0003c6f0: 282e 2a3f 2922 2729 2e73 6561 7263 6828  (.*?)"').search(
-0003c700: 6a73 5f68 746d 6c29 2e67 726f 7570 2831  js_html).group(1
-0003c710: 292c 0d0a 2020 2020 2320 2020 2020 7d0d  ),..    #     }.
-0003c720: 0a20 2020 2023 2020 2020 2072 6574 7572  .    #     retur
-0003c730: 6e20 6c77 745f 6461 7461 0d0a 0d0a 2020  n lwt_data....  
-0003c740: 2020 6465 6620 6765 745f 6c77 745f 6461    def get_lwt_da
-0003c750: 7461 2873 656c 6629 202d 3e20 6469 6374  ta(self) -> dict
-0003c760: 3a0d 0a20 2020 2020 2020 206c 7774 5f64  :..        lwt_d
-0003c770: 6174 6120 3d20 7b0d 0a20 2020 2020 2020  ata = {..       
-0003c780: 2020 2020 2027 782d 6c77 742d 6170 706c       'x-lwt-appl
-0003c790: 6963 6174 696f 6e2d 6964 273a 2027 4c57  ication-id': 'LW
-0003c7a0: 545f 5745 4227 2c0d 0a20 2020 2020 2020  T_WEB',..       
-0003c7b0: 2020 2020 2027 782d 6c77 742d 6275 696c       'x-lwt-buil
-0003c7c0: 642d 6964 273a 2027 3334 3637 3735 272c  d-id': '346775',
-0003c7d0: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
-0003c7e0: 2020 2020 2072 6574 7572 6e20 6c77 745f       return lwt_
-0003c7f0: 6461 7461 0d0a 0d0a 2020 2020 4054 7365  data....    @Tse
-0003c800: 2e74 696d 655f 7374 6174 0d0a 2020 2020  .time_stat..    
-0003c810: 4054 7365 2e63 6865 636b 5f71 7565 7279  @Tse.check_query
-0003c820: 0d0a 2020 2020 6465 6620 6c61 6e67 7561  ..    def langua
-0003c830: 6765 5769 7265 5f61 7069 2873 656c 662c  geWire_api(self,
-0003c840: 2071 7565 7279 5f74 6578 743a 2073 7472   query_text: str
-0003c850: 2c20 6672 6f6d 5f6c 616e 6775 6167 653a  , from_language:
-0003c860: 2073 7472 203d 2027 6175 746f 272c 2074   str = 'auto', t
-0003c870: 6f5f 6c61 6e67 7561 6765 3a20 7374 7220  o_language: str 
-0003c880: 3d20 2765 6e27 2c20 2a2a 6b77 6172 6773  = 'en', **kwargs
-0003c890: 3a20 4170 694b 7761 7267 7354 7970 6529  : ApiKwargsType)
-0003c8a0: 202d 3e20 556e 696f 6e5b 7374 722c 2064   -> Union[str, d
-0003c8b0: 6963 745d 3a0d 0a20 2020 2020 2020 2022  ict]:..        "
-0003c8c0: 2222 0d0a 2020 2020 2020 2020 6874 7470  ""..        http
-0003c8d0: 733a 2f2f 7777 772e 6c61 6e67 7561 6765  s://www.language
-0003c8e0: 7769 7265 2e63 6f6d 2f65 6e2f 7465 6368  wire.com/en/tech
-0003c8f0: 6e6f 6c6f 6779 2f6c 616e 6775 6167 6577  nology/languagew
-0003c900: 6972 652d 7472 616e 736c 6174 650d 0a20  ire-translate.. 
-0003c910: 2020 2020 2020 203a 7061 7261 6d20 7175         :param qu
-0003c920: 6572 795f 7465 7874 3a20 7374 722c 206d  ery_text: str, m
-0003c930: 7573 742e 0d0a 2020 2020 2020 2020 3a70  ust...        :p
-0003c940: 6172 616d 2066 726f 6d5f 6c61 6e67 7561  aram from_langua
-0003c950: 6765 3a20 7374 722c 2064 6566 6175 6c74  ge: str, default
-0003c960: 2027 6175 746f 272e 0d0a 2020 2020 2020   'auto'...      
-0003c970: 2020 3a70 6172 616d 2074 6f5f 6c61 6e67    :param to_lang
-0003c980: 7561 6765 3a20 7374 722c 2064 6566 6175  uage: str, defau
-0003c990: 6c74 2027 656e 272e 0d0a 2020 2020 2020  lt 'en'...      
-0003c9a0: 2020 3a70 6172 616d 202a 2a6b 7761 7267    :param **kwarg
-0003c9b0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-0003c9c0: 2020 2020 3a70 6172 616d 2074 696d 656f      :param timeo
-0003c9d0: 7574 3a20 666c 6f61 742c 2064 6566 6175  ut: float, defau
-0003c9e0: 6c74 204e 6f6e 652e 0d0a 2020 2020 2020  lt None...      
-0003c9f0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-0003ca00: 2070 726f 7869 6573 3a20 6469 6374 2c20   proxies: dict, 
-0003ca10: 6465 6661 756c 7420 4e6f 6e65 2e0d 0a20  default None... 
-0003ca20: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-0003ca30: 7061 7261 6d20 736c 6565 705f 7365 636f  param sleep_seco
-0003ca40: 6e64 733a 2066 6c6f 6174 2c20 6465 6661  nds: float, defa
-0003ca50: 756c 7420 302e 0d0a 2020 2020 2020 2020  ult 0...        
-0003ca60: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-0003ca70: 735f 6465 7461 696c 5f72 6573 756c 743a  s_detail_result:
-0003ca80: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
-0003ca90: 616c 7365 2e0d 0a20 2020 2020 2020 2020  alse...         
-0003caa0: 2020 2020 2020 203a 7061 7261 6d20 6966         :param if
-0003cab0: 5f69 676e 6f72 655f 6c69 6d69 745f 6f66  _ignore_limit_of
-0003cac0: 5f6c 656e 6774 683a 2062 6f6f 6c2c 2064  _length: bool, d
-0003cad0: 6566 6175 6c74 2046 616c 7365 2e0d 0a20  efault False... 
-0003cae0: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-0003caf0: 7061 7261 6d20 6c69 6d69 745f 6f66 5f6c  param limit_of_l
-0003cb00: 656e 6774 683a 2069 6e74 2c20 6465 6661  ength: int, defa
-0003cb10: 756c 7420 3230 3030 302e 0d0a 2020 2020  ult 20000...    
-0003cb20: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-0003cb30: 616d 2069 665f 6967 6e6f 7265 5f65 6d70  am if_ignore_emp
-0003cb40: 7479 5f71 7565 7279 3a20 626f 6f6c 2c20  ty_query: bool, 
-0003cb50: 6465 6661 756c 7420 4661 6c73 652e 0d0a  default False...
-0003cb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003cb70: 3a70 6172 616d 2075 7064 6174 655f 7365  :param update_se
-0003cb80: 7373 696f 6e5f 6166 7465 725f 6672 6571  ssion_after_freq
-0003cb90: 3a20 696e 742c 2064 6566 6175 6c74 2031  : int, default 1
-0003cba0: 3030 302e 0d0a 2020 2020 2020 2020 2020  000...          
-0003cbb0: 2020 2020 2020 3a70 6172 616d 2075 7064        :param upd
-0003cbc0: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
-0003cbd0: 725f 7365 636f 6e64 733a 2066 6c6f 6174  r_seconds: float
-0003cbe0: 2c20 6465 6661 756c 7420 3135 3030 2e0d  , default 1500..
-0003cbf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003cc00: 203a 7061 7261 6d20 6966 5f73 686f 775f   :param if_show_
-0003cc10: 7469 6d65 5f73 7461 743a 2062 6f6f 6c2c  time_stat: bool,
-0003cc20: 2064 6566 6175 6c74 2046 616c 7365 2e0d   default False..
-0003cc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003cc40: 203a 7061 7261 6d20 7368 6f77 5f74 696d   :param show_tim
-0003cc50: 655f 7374 6174 5f70 7265 6369 7369 6f6e  e_stat_precision
-0003cc60: 3a20 696e 742c 2064 6566 6175 6c74 2032  : int, default 2
-0003cc70: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0003cc80: 2020 203a 7061 7261 6d20 6966 5f70 7269     :param if_pri
-0003cc90: 6e74 5f77 6172 6e69 6e67 3a20 626f 6f6c  nt_warning: bool
-0003cca0: 2c20 6465 6661 756c 7420 5472 7565 2e0d  , default True..
-0003ccb0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-0003ccc0: 3a20 7374 7220 6f72 2064 6963 740d 0a20  : str or dict.. 
-0003ccd0: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
-0003cce0: 2020 2020 2020 7469 6d65 6f75 7420 3d20        timeout = 
-0003ccf0: 6b77 6172 6773 2e67 6574 2827 7469 6d65  kwargs.get('time
-0003cd00: 6f75 7427 2c20 4e6f 6e65 290d 0a20 2020  out', None)..   
-0003cd10: 2020 2020 2070 726f 7869 6573 203d 206b       proxies = k
-0003cd20: 7761 7267 732e 6765 7428 2770 726f 7869  wargs.get('proxi
-0003cd30: 6573 272c 204e 6f6e 6529 0d0a 2020 2020  es', None)..    
-0003cd40: 2020 2020 736c 6565 705f 7365 636f 6e64      sleep_second
-0003cd50: 7320 3d20 6b77 6172 6773 2e67 6574 2827  s = kwargs.get('
-0003cd60: 736c 6565 705f 7365 636f 6e64 7327 2c20  sleep_seconds', 
-0003cd70: 3029 0d0a 2020 2020 2020 2020 6966 5f70  0)..        if_p
-0003cd80: 7269 6e74 5f77 6172 6e69 6e67 203d 206b  rint_warning = k
-0003cd90: 7761 7267 732e 6765 7428 2769 665f 7072  wargs.get('if_pr
-0003cda0: 696e 745f 7761 726e 696e 6727 2c20 5472  int_warning', Tr
-0003cdb0: 7565 290d 0a20 2020 2020 2020 2069 735f  ue)..        is_
-0003cdc0: 6465 7461 696c 5f72 6573 756c 7420 3d20  detail_result = 
-0003cdd0: 6b77 6172 6773 2e67 6574 2827 6973 5f64  kwargs.get('is_d
-0003cde0: 6574 6169 6c5f 7265 7375 6c74 272c 2046  etail_result', F
-0003cdf0: 616c 7365 290d 0a20 2020 2020 2020 2075  alse)..        u
-0003ce00: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
-0003ce10: 7465 725f 6672 6571 203d 206b 7761 7267  ter_freq = kwarg
-0003ce20: 732e 6765 7428 2775 7064 6174 655f 7365  s.get('update_se
-0003ce30: 7373 696f 6e5f 6166 7465 725f 6672 6571  ssion_after_freq
-0003ce40: 272c 2073 656c 662e 6465 6661 756c 745f  ', self.default_
-0003ce50: 7365 7373 696f 6e5f 6672 6571 290d 0a20  session_freq).. 
-0003ce60: 2020 2020 2020 2075 7064 6174 655f 7365         update_se
-0003ce70: 7373 696f 6e5f 6166 7465 725f 7365 636f  ssion_after_seco
-0003ce80: 6e64 7320 3d20 6b77 6172 6773 2e67 6574  nds = kwargs.get
-0003ce90: 2827 7570 6461 7465 5f73 6573 7369 6f6e  ('update_session
-0003cea0: 5f61 6674 6572 5f73 6563 6f6e 6473 272c  _after_seconds',
-0003ceb0: 2073 656c 662e 6465 6661 756c 745f 7365   self.default_se
-0003cec0: 7373 696f 6e5f 7365 636f 6e64 7329 0d0a  ssion_seconds)..
-0003ced0: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
-0003cee0: 636b 5f69 6e70 7574 5f6c 696d 6974 2871  ck_input_limit(q
-0003cef0: 7565 7279 5f74 6578 742c 2073 656c 662e  uery_text, self.
-0003cf00: 696e 7075 745f 6c69 6d69 7429 0d0a 0d0a  input_limit)....
-0003cf10: 2020 2020 2020 2020 6e6f 745f 7570 6461          not_upda
-0003cf20: 7465 5f63 6f6e 645f 6672 6571 203d 2031  te_cond_freq = 1
-0003cf30: 2069 6620 7365 6c66 2e71 7565 7279 5f63   if self.query_c
-0003cf40: 6f75 6e74 203c 2075 7064 6174 655f 7365  ount < update_se
-0003cf50: 7373 696f 6e5f 6166 7465 725f 6672 6571  ssion_after_freq
-0003cf60: 2065 6c73 6520 300d 0a20 2020 2020 2020   else 0..       
-0003cf70: 206e 6f74 5f75 7064 6174 655f 636f 6e64   not_update_cond
-0003cf80: 5f74 696d 6520 3d20 3120 6966 2074 696d  _time = 1 if tim
-0003cf90: 652e 7469 6d65 2829 202d 2073 656c 662e  e.time() - self.
-0003cfa0: 6265 6769 6e5f 7469 6d65 203c 2075 7064  begin_time < upd
-0003cfb0: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
-0003cfc0: 725f 7365 636f 6e64 7320 656c 7365 2030  r_seconds else 0
-0003cfd0: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-0003cfe0: 2028 7365 6c66 2e73 6573 7369 6f6e 2061   (self.session a
-0003cff0: 6e64 2073 656c 662e 6c61 6e67 7561 6765  nd self.language
-0003d000: 5f6d 6170 2061 6e64 206e 6f74 5f75 7064  _map and not_upd
-0003d010: 6174 655f 636f 6e64 5f66 7265 7120 616e  ate_cond_freq an
-0003d020: 6420 6e6f 745f 7570 6461 7465 5f63 6f6e  d not_update_con
-0003d030: 645f 7469 6d65 293a 0d0a 2020 2020 2020  d_time):..      
-0003d040: 2020 2020 2020 7365 6c66 2e73 6573 7369        self.sessi
-0003d050: 6f6e 203d 2072 6571 7565 7374 732e 5365  on = requests.Se
-0003d060: 7373 696f 6e28 290d 0a20 2020 2020 2020  ssion()..       
-0003d070: 2020 2020 205f 203d 2073 656c 662e 7365       _ = self.se
-0003d080: 7373 696f 6e2e 6765 7428 7365 6c66 2e68  ssion.get(self.h
-0003d090: 6f73 745f 7572 6c2c 2068 6561 6465 7273  ost_url, headers
-0003d0a0: 3d73 656c 662e 686f 7374 5f68 6561 6465  =self.host_heade
-0003d0b0: 7273 2c20 7469 6d65 6f75 743d 7469 6d65  rs, timeout=time
-0003d0c0: 6f75 742c 2070 726f 7869 6573 3d70 726f  out, proxies=pro
-0003d0d0: 7869 6573 290d 0a20 2020 2020 2020 2020  xies)..         
-0003d0e0: 2020 2073 656c 662e 6c77 745f 6461 7461     self.lwt_data
-0003d0f0: 203d 2073 656c 662e 6765 745f 6c77 745f   = self.get_lwt_
-0003d100: 6461 7461 2829 0d0a 2020 2020 2020 2020  data()..        
-0003d110: 2020 2020 7365 6c66 2e61 7069 5f68 6561      self.api_hea
-0003d120: 6465 7273 2e75 7064 6174 6528 7365 6c66  ders.update(self
-0003d130: 2e6c 7774 5f64 6174 6129 0d0a 0d0a 2020  .lwt_data)....  
-0003d140: 2020 2020 2020 2020 2020 5f20 3d20 7365            _ = se
-0003d150: 6c66 2e73 6573 7369 6f6e 2e70 6f73 7428  lf.session.post(
-0003d160: 7365 6c66 2e63 6f6f 6b69 655f 7572 6c2c  self.cookie_url,
-0003d170: 2068 6561 6465 7273 3d73 656c 662e 6170   headers=self.ap
-0003d180: 695f 6865 6164 6572 732c 2074 696d 656f  i_headers, timeo
-0003d190: 7574 3d74 696d 656f 7574 2c20 7072 6f78  ut=timeout, prox
-0003d1a0: 6965 733d 7072 6f78 6965 7329 0d0a 2020  ies=proxies)..  
-0003d1b0: 2020 2020 2020 2020 2020 6465 6275 675f            debug_
-0003d1c0: 6c61 6e67 5f6b 7761 7267 7320 3d20 7365  lang_kwargs = se
-0003d1d0: 6c66 2e64 6562 7567 5f6c 616e 675f 6b77  lf.debug_lang_kw
-0003d1e0: 6172 6773 2866 726f 6d5f 6c61 6e67 7561  args(from_langua
-0003d1f0: 6765 2c20 746f 5f6c 616e 6775 6167 652c  ge, to_language,
-0003d200: 2073 656c 662e 6465 6661 756c 745f 6672   self.default_fr
-0003d210: 6f6d 5f6c 616e 6775 6167 652c 2069 665f  om_language, if_
-0003d220: 7072 696e 745f 7761 726e 696e 6729 0d0a  print_warning)..
-0003d230: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0003d240: 2e6c 616e 6775 6167 655f 6d61 7020 3d20  .language_map = 
-0003d250: 7365 6c66 2e67 6574 5f6c 616e 6775 6167  self.get_languag
-0003d260: 655f 6d61 7028 7365 6c66 2e6c 616e 675f  e_map(self.lang_
-0003d270: 7572 6c2c 2073 656c 662e 7365 7373 696f  url, self.sessio
-0003d280: 6e2c 2073 656c 662e 6170 695f 6865 6164  n, self.api_head
-0003d290: 6572 732c 2074 696d 656f 7574 2c20 7072  ers, timeout, pr
-0003d2a0: 6f78 6965 732c 202a 2a64 6562 7567 5f6c  oxies, **debug_l
-0003d2b0: 616e 675f 6b77 6172 6773 290d 0a0d 0a20  ang_kwargs).... 
-0003d2c0: 2020 2020 2020 2069 6620 6672 6f6d 5f6c         if from_l
-0003d2d0: 616e 6775 6167 6520 3d3d 2027 6175 746f  anguage == 'auto
-0003d2e0: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
-0003d2f0: 6672 6f6d 5f6c 616e 6775 6167 6520 3d20  from_language = 
-0003d300: 7365 6c66 2e77 6172 6e69 6e67 5f61 7574  self.warning_aut
-0003d310: 6f5f 6c61 6e67 2827 6c61 6e67 7561 6765  o_lang('language
-0003d320: 5769 7265 272c 2073 656c 662e 6465 6661  Wire', self.defa
-0003d330: 756c 745f 6672 6f6d 5f6c 616e 6775 6167  ult_from_languag
-0003d340: 652c 2069 665f 7072 696e 745f 7761 726e  e, if_print_warn
-0003d350: 696e 6729 0d0a 2020 2020 2020 2020 746f  ing)..        to
-0003d360: 5f6c 616e 6775 6167 6520 3d20 7365 6c66  _language = self
-0003d370: 2e64 6566 6175 6c74 5f65 6e5f 746f 5f6c  .default_en_to_l
-0003d380: 616e 6775 6167 6520 6966 2074 6f5f 6c61  anguage if to_la
-0003d390: 6e67 7561 6765 203d 3d20 2765 6e27 2065  nguage == 'en' e
-0003d3a0: 6c73 6520 746f 5f6c 616e 6775 6167 650d  lse to_language.
-0003d3b0: 0a20 2020 2020 2020 2066 726f 6d5f 6c61  .        from_la
-0003d3c0: 6e67 7561 6765 2c20 746f 5f6c 616e 6775  nguage, to_langu
-0003d3d0: 6167 6520 3d20 7365 6c66 2e63 6865 636b  age = self.check
-0003d3e0: 5f6c 616e 6775 6167 6528 6672 6f6d 5f6c  _language(from_l
-0003d3f0: 616e 6775 6167 652c 2074 6f5f 6c61 6e67  anguage, to_lang
-0003d400: 7561 6765 2c20 7365 6c66 2e6c 616e 6775  uage, self.langu
-0003d410: 6167 655f 6d61 702c 2069 665f 6368 6563  age_map, if_chec
-0003d420: 6b5f 6c61 6e67 5f72 6576 6572 7365 3d46  k_lang_reverse=F
-0003d430: 616c 7365 290d 0a0d 0a20 2020 2020 2020  alse)....       
-0003d440: 2070 6179 6c6f 6164 203d 207b 0d0a 2020   payload = {..  
-0003d450: 2020 2020 2020 2020 2020 2773 6f75 7263            'sourc
-0003d460: 6554 6578 7427 3a20 7175 6572 795f 7465  eText': query_te
-0003d470: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
-0003d480: 2027 736f 7572 6365 4c61 6e67 7561 6765   'sourceLanguage
-0003d490: 273a 2066 726f 6d5f 6c61 6e67 7561 6765  ': from_language
-0003d4a0: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-0003d4b0: 7461 7267 6574 4c61 6e67 7561 6765 273a  targetLanguage':
-0003d4c0: 2074 6f5f 6c61 6e67 7561 6765 2c0d 0a20   to_language,.. 
-0003d4d0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-0003d4e0: 2020 7220 3d20 7365 6c66 2e73 6573 7369    r = self.sessi
-0003d4f0: 6f6e 2e70 6f73 7428 7365 6c66 2e61 7069  on.post(self.api
-0003d500: 5f75 726c 2c20 6a73 6f6e 3d70 6179 6c6f  _url, json=paylo
-0003d510: 6164 2c20 6865 6164 6572 733d 7365 6c66  ad, headers=self
-0003d520: 2e61 7069 5f68 6561 6465 7273 2c20 7469  .api_headers, ti
-0003d530: 6d65 6f75 743d 7469 6d65 6f75 742c 2070  meout=timeout, p
-0003d540: 726f 7869 6573 3d70 726f 7869 6573 290d  roxies=proxies).
-0003d550: 0a20 2020 2020 2020 2072 2e72 6169 7365  .        r.raise
-0003d560: 5f66 6f72 5f73 7461 7475 7328 290d 0a20  _for_status().. 
-0003d570: 2020 2020 2020 2064 6174 6120 3d20 722e         data = r.
-0003d580: 6a73 6f6e 2829 0d0a 2020 2020 2020 2020  json()..        
-0003d590: 7469 6d65 2e73 6c65 6570 2873 6c65 6570  time.sleep(sleep
-0003d5a0: 5f73 6563 6f6e 6473 290d 0a20 2020 2020  _seconds)..     
-0003d5b0: 2020 2073 656c 662e 7175 6572 795f 636f     self.query_co
-0003d5c0: 756e 7420 2b3d 2031 0d0a 2020 2020 2020  unt += 1..      
-0003d5d0: 2020 7265 7475 726e 2064 6174 6120 6966    return data if
-0003d5e0: 2069 735f 6465 7461 696c 5f72 6573 756c   is_detail_resul
-0003d5f0: 7420 656c 7365 2064 6174 615b 2774 7261  t else data['tra
-0003d600: 6e73 6c61 7469 6f6e 275d 0d0a 0d0a 0d0a  nslation']......
-0003d610: 636c 6173 7320 4a75 6469 6328 5473 6529  class Judic(Tse)
-0003d620: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
-0003d630: 745f 5f28 7365 6c66 293a 0d0a 2020 2020  t__(self):..    
-0003d640: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-0003d650: 6974 5f5f 2829 0d0a 2020 2020 2020 2020  it__()..        
-0003d660: 7365 6c66 2e68 6f6d 655f 7572 6c20 3d20  self.home_url = 
-0003d670: 2768 7474 7073 3a2f 2f6a 7564 6963 2e69  'https://judic.i
-0003d680: 6f27 0d0a 2020 2020 2020 2020 7365 6c66  o'..        self
-0003d690: 2e68 6f73 745f 7572 6c20 3d20 2768 7474  .host_url = 'htt
-0003d6a0: 7073 3a2f 2f6a 7564 6963 2e69 6f2f 656e  ps://judic.io/en
-0003d6b0: 2f74 7261 6e73 6c61 7465 270d 0a20 2020  /translate'..   
-0003d6c0: 2020 2020 2073 656c 662e 6170 695f 7572       self.api_ur
-0003d6d0: 6c20 3d20 2768 7474 7073 3a2f 2f6a 7564  l = 'https://jud
-0003d6e0: 6963 2e69 6f2f 7472 616e 736c 6174 652f  ic.io/translate/
-0003d6f0: 7465 7874 270d 0a20 2020 2020 2020 2073  text'..        s
-0003d700: 656c 662e 686f 7374 5f68 6561 6465 7273  elf.host_headers
-0003d710: 203d 2073 656c 662e 6765 745f 6865 6164   = self.get_head
-0003d720: 6572 7328 7365 6c66 2e68 6f6d 655f 7572  ers(self.home_ur
-0003d730: 6c2c 2069 665f 6170 693d 4661 6c73 652c  l, if_api=False,
-0003d740: 2069 665f 7265 6665 7265 725f 666f 725f   if_referer_for_
-0003d750: 686f 7374 3d54 7275 6529 0d0a 2020 2020  host=True)..    
-0003d760: 2020 2020 7365 6c66 2e61 7069 5f68 6561      self.api_hea
-0003d770: 6465 7273 203d 2073 656c 662e 6765 745f  ders = self.get_
-0003d780: 6865 6164 6572 7328 7365 6c66 2e68 6f6d  headers(self.hom
-0003d790: 655f 7572 6c2c 2069 665f 6170 693d 5472  e_url, if_api=Tr
-0003d7a0: 7565 2c20 6966 5f6a 736f 6e5f 666f 725f  ue, if_json_for_
-0003d7b0: 6170 693d 5472 7565 290d 0a20 2020 2020  api=True)..     
-0003d7c0: 2020 2073 656c 662e 7365 7373 696f 6e20     self.session 
-0003d7d0: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-0003d7e0: 7365 6c66 2e6c 616e 675f 6c69 7374 203d  self.lang_list =
-0003d7f0: 205b 2765 6e27 2c20 2764 6527 2c20 2766   ['en', 'de', 'f
-0003d800: 7227 2c20 276e 6c27 5d0d 0a20 2020 2020  r', 'nl']..     
-0003d810: 2020 2073 656c 662e 6c61 6e67 7561 6765     self.language
-0003d820: 5f6d 6170 203d 204e 6f6e 650d 0a20 2020  _map = None..   
-0003d830: 2020 2020 2073 656c 662e 7175 6572 795f       self.query_
-0003d840: 636f 756e 7420 3d20 300d 0a20 2020 2020  count = 0..     
-0003d850: 2020 2073 656c 662e 6f75 7470 7574 5f7a     self.output_z
-0003d860: 6820 3d20 4e6f 6e65 2020 2320 756e 7375  h = None  # unsu
-0003d870: 7070 6f72 7465 640d 0a20 2020 2020 2020  pported..       
-0003d880: 2073 656c 662e 696e 7075 745f 6c69 6d69   self.input_limi
-0003d890: 7420 3d20 696e 7428 3165 3329 0d0a 2020  t = int(1e3)..  
-0003d8a0: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
-0003d8b0: 6c74 5f66 726f 6d5f 6c61 6e67 7561 6765  lt_from_language
-0003d8c0: 203d 2027 6e6c 270d 0a0d 0a20 2020 2040   = 'nl'....    @
-0003d8d0: 5473 652e 6465 6275 675f 6c61 6e67 7561  Tse.debug_langua
-0003d8e0: 6765 5f6d 6170 0d0a 2020 2020 6465 6620  ge_map..    def 
-0003d8f0: 6765 745f 6c61 6e67 7561 6765 5f6d 6170  get_language_map
-0003d900: 2873 656c 662c 206c 616e 675f 6c69 7374  (self, lang_list
-0003d910: 3a20 4c69 7374 5b73 7472 5d2c 202a 2a6b  : List[str], **k
-0003d920: 7761 7267 733a 204c 616e 674d 6170 4b77  wargs: LangMapKw
-0003d930: 6172 6773 5479 7065 2920 2d3e 2064 6963  argsType) -> dic
-0003d940: 743a 0d0a 2020 2020 2020 2020 7265 7475  t:..        retu
-0003d950: 726e 207b 7d2e 6672 6f6d 6b65 7973 286c  rn {}.fromkeys(l
-0003d960: 616e 675f 6c69 7374 2c20 6c61 6e67 5f6c  ang_list, lang_l
-0003d970: 6973 7429 0d0a 0d0a 2020 2020 4054 7365  ist)....    @Tse
-0003d980: 2e74 696d 655f 7374 6174 0d0a 2020 2020  .time_stat..    
-0003d990: 4054 7365 2e63 6865 636b 5f71 7565 7279  @Tse.check_query
-0003d9a0: 0d0a 2020 2020 6465 6620 6a75 6469 635f  ..    def judic_
-0003d9b0: 6170 6928 7365 6c66 2c20 7175 6572 795f  api(self, query_
-0003d9c0: 7465 7874 3a20 7374 722c 2066 726f 6d5f  text: str, from_
-0003d9d0: 6c61 6e67 7561 6765 3a20 7374 7220 3d20  language: str = 
-0003d9e0: 2761 7574 6f27 2c20 746f 5f6c 616e 6775  'auto', to_langu
-0003d9f0: 6167 653a 2073 7472 203d 2027 656e 272c  age: str = 'en',
-0003da00: 202a 2a6b 7761 7267 733a 2041 7069 4b77   **kwargs: ApiKw
-0003da10: 6172 6773 5479 7065 2920 2d3e 2055 6e69  argsType) -> Uni
-0003da20: 6f6e 5b73 7472 2c20 6469 6374 5d3a 0d0a  on[str, dict]:..
-0003da30: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0003da40: 2020 2020 2068 7474 7073 3a2f 2f6a 7564       https://jud
-0003da50: 6963 2e69 6f2f 656e 2f74 7261 6e73 6c61  ic.io/en/transla
-0003da60: 7465 0d0a 2020 2020 2020 2020 3a70 6172  te..        :par
-0003da70: 616d 2071 7565 7279 5f74 6578 743a 2073  am query_text: s
-0003da80: 7472 2c20 6d75 7374 2e0d 0a20 2020 2020  tr, must...     
-0003da90: 2020 203a 7061 7261 6d20 6672 6f6d 5f6c     :param from_l
-0003daa0: 616e 6775 6167 653a 2073 7472 2c20 6465  anguage: str, de
-0003dab0: 6661 756c 7420 2761 7574 6f27 2e0d 0a20  fault 'auto'... 
-0003dac0: 2020 2020 2020 203a 7061 7261 6d20 746f         :param to
-0003dad0: 5f6c 616e 6775 6167 653a 2073 7472 2c20  _language: str, 
-0003dae0: 6465 6661 756c 7420 2765 6e27 2e0d 0a20  default 'en'... 
-0003daf0: 2020 2020 2020 203a 7061 7261 6d20 2a2a         :param **
-0003db00: 6b77 6172 6773 3a0d 0a20 2020 2020 2020  kwargs:..       
-0003db10: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-0003db20: 7469 6d65 6f75 743a 2066 6c6f 6174 2c20  timeout: float, 
-0003db30: 6465 6661 756c 7420 4e6f 6e65 2e0d 0a20  default None... 
-0003db40: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-0003db50: 7061 7261 6d20 7072 6f78 6965 733a 2064  param proxies: d
-0003db60: 6963 742c 2064 6566 6175 6c74 204e 6f6e  ict, default Non
-0003db70: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
-0003db80: 2020 2020 3a70 6172 616d 2073 6c65 6570      :param sleep
-0003db90: 5f73 6563 6f6e 6473 3a20 666c 6f61 742c  _seconds: float,
-0003dba0: 2064 6566 6175 6c74 2030 2e0d 0a20 2020   default 0...   
-0003dbb0: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-0003dbc0: 7261 6d20 6973 5f64 6574 6169 6c5f 7265  ram is_detail_re
-0003dbd0: 7375 6c74 3a20 626f 6f6c 2c20 6465 6661  sult: bool, defa
-0003dbe0: 756c 7420 4661 6c73 652e 0d0a 2020 2020  ult False...    
-0003dbf0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-0003dc00: 616d 2069 665f 6967 6e6f 7265 5f6c 696d  am if_ignore_lim
-0003dc10: 6974 5f6f 665f 6c65 6e67 7468 3a20 626f  it_of_length: bo
-0003dc20: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-0003dc30: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
-0003dc40: 2020 2020 3a70 6172 616d 206c 696d 6974      :param limit
-0003dc50: 5f6f 665f 6c65 6e67 7468 3a20 696e 742c  _of_length: int,
-0003dc60: 2064 6566 6175 6c74 2032 3030 3030 2e0d   default 20000..
-0003dc70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003dc80: 203a 7061 7261 6d20 6966 5f69 676e 6f72   :param if_ignor
-0003dc90: 655f 656d 7074 795f 7175 6572 793a 2062  e_empty_query: b
-0003dca0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
-0003dcb0: 7365 2e0d 0a20 2020 2020 2020 2020 2020  se...           
-0003dcc0: 2020 2020 203a 7061 7261 6d20 7570 6461       :param upda
-0003dcd0: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
-0003dce0: 5f66 7265 713a 2069 6e74 2c20 6465 6661  _freq: int, defa
-0003dcf0: 756c 7420 3130 3030 2e0d 0a20 2020 2020  ult 1000...     
-0003dd00: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-0003dd10: 6d20 7570 6461 7465 5f73 6573 7369 6f6e  m update_session
-0003dd20: 5f61 6674 6572 5f73 6563 6f6e 6473 3a20  _after_seconds: 
-0003dd30: 666c 6f61 742c 2064 6566 6175 6c74 2031  float, default 1
-0003dd40: 3530 302e 0d0a 2020 2020 2020 2020 2020  500...          
-0003dd50: 2020 2020 2020 3a70 6172 616d 2069 665f        :param if_
-0003dd60: 7368 6f77 5f74 696d 655f 7374 6174 3a20  show_time_stat: 
-0003dd70: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-0003dd80: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
-0003dd90: 2020 2020 2020 3a70 6172 616d 2073 686f        :param sho
-0003dda0: 775f 7469 6d65 5f73 7461 745f 7072 6563  w_time_stat_prec
-0003ddb0: 6973 696f 6e3a 2069 6e74 2c20 6465 6661  ision: int, defa
-0003ddc0: 756c 7420 322e 0d0a 2020 2020 2020 2020  ult 2...        
-0003ddd0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-0003dde0: 665f 7072 696e 745f 7761 726e 696e 673a  f_print_warning:
-0003ddf0: 2062 6f6f 6c2c 2064 6566 6175 6c74 2054   bool, default T
-0003de00: 7275 652e 0d0a 2020 2020 2020 2020 3a72  rue...        :r
-0003de10: 6574 7572 6e3a 2073 7472 206f 7220 6469  eturn: str or di
-0003de20: 6374 0d0a 2020 2020 2020 2020 2222 220d  ct..        """.
-0003de30: 0a0d 0a20 2020 2020 2020 2074 696d 656f  ...        timeo
-0003de40: 7574 203d 206b 7761 7267 732e 6765 7428  ut = kwargs.get(
-0003de50: 2774 696d 656f 7574 272c 204e 6f6e 6529  'timeout', None)
-0003de60: 0d0a 2020 2020 2020 2020 7072 6f78 6965  ..        proxie
-0003de70: 7320 3d20 6b77 6172 6773 2e67 6574 2827  s = kwargs.get('
-0003de80: 7072 6f78 6965 7327 2c20 4e6f 6e65 290d  proxies', None).
-0003de90: 0a20 2020 2020 2020 2073 6c65 6570 5f73  .        sleep_s
-0003dea0: 6563 6f6e 6473 203d 206b 7761 7267 732e  econds = kwargs.
-0003deb0: 6765 7428 2773 6c65 6570 5f73 6563 6f6e  get('sleep_secon
-0003dec0: 6473 272c 2030 290d 0a20 2020 2020 2020  ds', 0)..       
-0003ded0: 2069 665f 7072 696e 745f 7761 726e 696e   if_print_warnin
-0003dee0: 6720 3d20 6b77 6172 6773 2e67 6574 2827  g = kwargs.get('
-0003def0: 6966 5f70 7269 6e74 5f77 6172 6e69 6e67  if_print_warning
-0003df00: 272c 2054 7275 6529 0d0a 2020 2020 2020  ', True)..      
-0003df10: 2020 6973 5f64 6574 6169 6c5f 7265 7375    is_detail_resu
-0003df20: 6c74 203d 206b 7761 7267 732e 6765 7428  lt = kwargs.get(
-0003df30: 2769 735f 6465 7461 696c 5f72 6573 756c  'is_detail_resul
-0003df40: 7427 2c20 4661 6c73 6529 0d0a 2020 2020  t', False)..    
-0003df50: 2020 2020 7570 6461 7465 5f73 6573 7369      update_sessi
-0003df60: 6f6e 5f61 6674 6572 5f66 7265 7120 3d20  on_after_freq = 
-0003df70: 6b77 6172 6773 2e67 6574 2827 7570 6461  kwargs.get('upda
-0003df80: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
-0003df90: 5f66 7265 7127 2c20 7365 6c66 2e64 6566  _freq', self.def
-0003dfa0: 6175 6c74 5f73 6573 7369 6f6e 5f66 7265  ault_session_fre
-0003dfb0: 7129 0d0a 2020 2020 2020 2020 7570 6461  q)..        upda
-0003dfc0: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
-0003dfd0: 5f73 6563 6f6e 6473 203d 206b 7761 7267  _seconds = kwarg
-0003dfe0: 732e 6765 7428 2775 7064 6174 655f 7365  s.get('update_se
-0003dff0: 7373 696f 6e5f 6166 7465 725f 7365 636f  ssion_after_seco
-0003e000: 6e64 7327 2c20 7365 6c66 2e64 6566 6175  nds', self.defau
-0003e010: 6c74 5f73 6573 7369 6f6e 5f73 6563 6f6e  lt_session_secon
-0003e020: 6473 290d 0a20 2020 2020 2020 2073 656c  ds)..        sel
-0003e030: 662e 6368 6563 6b5f 696e 7075 745f 6c69  f.check_input_li
-0003e040: 6d69 7428 7175 6572 795f 7465 7874 2c20  mit(query_text, 
-0003e050: 7365 6c66 2e69 6e70 7574 5f6c 696d 6974  self.input_limit
-0003e060: 290d 0a0d 0a20 2020 2020 2020 206e 6f74  )....        not
-0003e070: 5f75 7064 6174 655f 636f 6e64 5f66 7265  _update_cond_fre
-0003e080: 7120 3d20 3120 6966 2073 656c 662e 7175  q = 1 if self.qu
-0003e090: 6572 795f 636f 756e 7420 3c20 7570 6461  ery_count < upda
-0003e0a0: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
-0003e0b0: 5f66 7265 7120 656c 7365 2030 0d0a 2020  _freq else 0..  
-0003e0c0: 2020 2020 2020 6e6f 745f 7570 6461 7465        not_update
-0003e0d0: 5f63 6f6e 645f 7469 6d65 203d 2031 2069  _cond_time = 1 i
-0003e0e0: 6620 7469 6d65 2e74 696d 6528 2920 2d20  f time.time() - 
-0003e0f0: 7365 6c66 2e62 6567 696e 5f74 696d 6520  self.begin_time 
-0003e100: 3c20 7570 6461 7465 5f73 6573 7369 6f6e  < update_session
-0003e110: 5f61 6674 6572 5f73 6563 6f6e 6473 2065  _after_seconds e
-0003e120: 6c73 6520 300d 0a20 2020 2020 2020 2069  lse 0..        i
-0003e130: 6620 6e6f 7420 2873 656c 662e 7365 7373  f not (self.sess
-0003e140: 696f 6e20 616e 6420 7365 6c66 2e6c 616e  ion and self.lan
-0003e150: 6775 6167 655f 6d61 7020 616e 6420 6e6f  guage_map and no
-0003e160: 745f 7570 6461 7465 5f63 6f6e 645f 6672  t_update_cond_fr
-0003e170: 6571 2061 6e64 206e 6f74 5f75 7064 6174  eq and not_updat
-0003e180: 655f 636f 6e64 5f74 696d 6529 3a0d 0a20  e_cond_time):.. 
-0003e190: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0003e1a0: 7365 7373 696f 6e20 3d20 7265 7175 6573  session = reques
-0003e1b0: 7473 2e53 6573 7369 6f6e 2829 0d0a 2020  ts.Session()..  
-0003e1c0: 2020 2020 2020 2020 2020 5f20 3d20 7365            _ = se
-0003e1d0: 6c66 2e73 6573 7369 6f6e 2e67 6574 2873  lf.session.get(s
-0003e1e0: 656c 662e 686f 7374 5f75 726c 2c20 6865  elf.host_url, he
-0003e1f0: 6164 6572 733d 7365 6c66 2e68 6f73 745f  aders=self.host_
-0003e200: 6865 6164 6572 732c 2074 696d 656f 7574  headers, timeout
-0003e210: 3d74 696d 656f 7574 2c20 7072 6f78 6965  =timeout, proxie
-0003e220: 733d 7072 6f78 6965 7329 0d0a 2020 2020  s=proxies)..    
-0003e230: 2020 2020 2020 2020 6465 6275 675f 6c61          debug_la
-0003e240: 6e67 5f6b 7761 7267 7320 3d20 7365 6c66  ng_kwargs = self
-0003e250: 2e64 6562 7567 5f6c 616e 675f 6b77 6172  .debug_lang_kwar
-0003e260: 6773 2866 726f 6d5f 6c61 6e67 7561 6765  gs(from_language
-0003e270: 2c20 746f 5f6c 616e 6775 6167 652c 2073  , to_language, s
-0003e280: 656c 662e 6465 6661 756c 745f 6672 6f6d  elf.default_from
-0003e290: 5f6c 616e 6775 6167 652c 2069 665f 7072  _language, if_pr
-0003e2a0: 696e 745f 7761 726e 696e 6729 0d0a 2020  int_warning)..  
-0003e2b0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-0003e2c0: 616e 6775 6167 655f 6d61 7020 3d20 7365  anguage_map = se
-0003e2d0: 6c66 2e67 6574 5f6c 616e 6775 6167 655f  lf.get_language_
-0003e2e0: 6d61 7028 7365 6c66 2e6c 616e 675f 6c69  map(self.lang_li
-0003e2f0: 7374 2c20 2a2a 6465 6275 675f 6c61 6e67  st, **debug_lang
-0003e300: 5f6b 7761 7267 7329 0d0a 0d0a 2020 2020  _kwargs)....    
-0003e310: 2020 2020 6966 2066 726f 6d5f 6c61 6e67      if from_lang
-0003e320: 7561 6765 203d 3d20 2761 7574 6f27 3a0d  uage == 'auto':.
-0003e330: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-0003e340: 6d5f 6c61 6e67 7561 6765 203d 2073 656c  m_language = sel
-0003e350: 662e 7761 726e 696e 675f 6175 746f 5f6c  f.warning_auto_l
-0003e360: 616e 6728 276a 7564 6963 272c 2073 656c  ang('judic', sel
-0003e370: 662e 6465 6661 756c 745f 6672 6f6d 5f6c  f.default_from_l
-0003e380: 616e 6775 6167 652c 2069 665f 7072 696e  anguage, if_prin
-0003e390: 745f 7761 726e 696e 6729 0d0a 2020 2020  t_warning)..    
-0003e3a0: 2020 2020 6672 6f6d 5f6c 616e 6775 6167      from_languag
-0003e3b0: 652c 2074 6f5f 6c61 6e67 7561 6765 203d  e, to_language =
-0003e3c0: 2073 656c 662e 6368 6563 6b5f 6c61 6e67   self.check_lang
-0003e3d0: 7561 6765 2866 726f 6d5f 6c61 6e67 7561  uage(from_langua
-0003e3e0: 6765 2c20 746f 5f6c 616e 6775 6167 652c  ge, to_language,
-0003e3f0: 2073 656c 662e 6c61 6e67 7561 6765 5f6d   self.language_m
-0003e400: 6170 290d 0a0d 0a20 2020 2020 2020 2070  ap)....        p
-0003e410: 6179 6c6f 6164 203d 207b 0d0a 2020 2020  ayload = {..    
-0003e420: 2020 2020 2020 2020 2773 6f75 7263 6554          'sourceT
-0003e430: 6578 7427 3a20 7175 6572 795f 7465 7874  ext': query_text
-0003e440: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-0003e450: 696e 7075 744c 616e 6727 3a20 6672 6f6d  inputLang': from
-0003e460: 5f6c 616e 6775 6167 652c 0d0a 2020 2020  _language,..    
-0003e470: 2020 2020 2020 2020 276f 7574 7075 744c          'outputL
-0003e480: 616e 6727 3a20 746f 5f6c 616e 6775 6167  ang': to_languag
-0003e490: 650d 0a20 2020 2020 2020 207d 0d0a 2020  e..        }..  
-0003e4a0: 2020 2020 2020 7220 3d20 7365 6c66 2e73        r = self.s
-0003e4b0: 6573 7369 6f6e 2e70 6f73 7428 7365 6c66  ession.post(self
-0003e4c0: 2e61 7069 5f75 726c 2c20 6a73 6f6e 3d70  .api_url, json=p
-0003e4d0: 6179 6c6f 6164 2c20 6865 6164 6572 733d  ayload, headers=
-0003e4e0: 7365 6c66 2e61 7069 5f68 6561 6465 7273  self.api_headers
-0003e4f0: 2c20 7469 6d65 6f75 743d 7469 6d65 6f75  , timeout=timeou
-0003e500: 742c 2070 726f 7869 6573 3d70 726f 7869  t, proxies=proxi
-0003e510: 6573 290d 0a20 2020 2020 2020 2072 2e72  es)..        r.r
-0003e520: 6169 7365 5f66 6f72 5f73 7461 7475 7328  aise_for_status(
-0003e530: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
-0003e540: 3d20 722e 6a73 6f6e 2829 0d0a 2020 2020  = r.json()..    
-0003e550: 2020 2020 7469 6d65 2e73 6c65 6570 2873      time.sleep(s
-0003e560: 6c65 6570 5f73 6563 6f6e 6473 290d 0a20  leep_seconds).. 
-0003e570: 2020 2020 2020 2073 656c 662e 7175 6572         self.quer
-0003e580: 795f 636f 756e 7420 2b3d 2031 0d0a 2020  y_count += 1..  
-0003e590: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
-0003e5a0: 6120 6966 2069 735f 6465 7461 696c 5f72  a if is_detail_r
-0003e5b0: 6573 756c 7420 656c 7365 2064 6174 615b  esult else data[
-0003e5c0: 2774 7261 6e73 6c61 7469 6f6e 275d 0d0a  'translation']..
-0003e5d0: 0d0a 0d0a 636c 6173 7320 5965 656b 6974  ....class Yeekit
-0003e5e0: 2854 7365 293a 0d0a 2020 2020 6465 6620  (Tse):..    def 
-0003e5f0: 5f5f 696e 6974 5f5f 2873 656c 6629 3a0d  __init__(self):.
-0003e600: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-0003e610: 2e5f 5f69 6e69 745f 5f28 290d 0a20 2020  .__init__()..   
-0003e620: 2020 2020 2073 656c 662e 686f 6d65 5f75       self.home_u
-0003e630: 726c 203d 2027 6874 7470 733a 2f2f 7777  rl = 'https://ww
-0003e640: 772e 7965 656b 6974 2e63 6f6d 270d 0a20  w.yeekit.com'.. 
-0003e650: 2020 2020 2020 2073 656c 662e 686f 7374         self.host
-0003e660: 5f75 726c 203d 2027 6874 7470 733a 2f2f  _url = 'https://
-0003e670: 7777 772e 7965 656b 6974 2e63 6f6d 2f73  www.yeekit.com/s
-0003e680: 6974 652f 7472 616e 736c 6174 6527 0d0a  ite/translate'..
-0003e690: 2020 2020 2020 2020 7365 6c66 2e61 7069          self.api
-0003e6a0: 5f75 726c 203d 2027 6874 7470 733a 2f2f  _url = 'https://
-0003e6b0: 7777 772e 7965 656b 6974 2e63 6f6d 2f73  www.yeekit.com/s
-0003e6c0: 6974 652f 646f 7472 616e 736c 6174 6527  ite/dotranslate'
-0003e6d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-0003e6e0: 616e 675f 7572 6c20 3d20 2768 7474 7073  ang_url = 'https
-0003e6f0: 3a2f 2f77 7777 2e79 6565 6b69 742e 636f  ://www.yeekit.co
-0003e700: 6d2f 6a73 2f74 7261 6e73 6c61 7465 2e6a  m/js/translate.j
-0003e710: 7327 0d0a 2020 2020 2020 2020 7365 6c66  s'..        self
-0003e720: 2e68 6f73 745f 6865 6164 6572 7320 3d20  .host_headers = 
-0003e730: 7365 6c66 2e67 6574 5f68 6561 6465 7273  self.get_headers
-0003e740: 2873 656c 662e 686f 6d65 5f75 726c 2c20  (self.home_url, 
-0003e750: 6966 5f61 7069 3d46 616c 7365 2c20 6966  if_api=False, if
-0003e760: 5f72 6566 6572 6572 5f66 6f72 5f68 6f73  _referer_for_hos
-0003e770: 743d 5472 7565 290d 0a20 2020 2020 2020  t=True)..       
-0003e780: 2073 656c 662e 6170 695f 6865 6164 6572   self.api_header
-0003e790: 7320 3d20 7365 6c66 2e67 6574 5f68 6561  s = self.get_hea
-0003e7a0: 6465 7273 2873 656c 662e 686f 6d65 5f75  ders(self.home_u
-0003e7b0: 726c 2c20 6966 5f61 7069 3d54 7275 652c  rl, if_api=True,
-0003e7c0: 2069 665f 616a 6178 5f66 6f72 5f61 7069   if_ajax_for_api
-0003e7d0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-0003e7e0: 7365 6c66 2e73 6573 7369 6f6e 203d 204e  self.session = N
-0003e7f0: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
-0003e800: 662e 6c61 6e67 5f6c 6973 7420 3d20 5b27  f.lang_list = ['
-0003e810: 7a68 272c 2027 656e 272c 2027 6172 272c  zh', 'en', 'ar',
-0003e820: 2027 6465 272c 2027 7275 272c 2027 6672   'de', 'ru', 'fr
-0003e830: 272c 2027 637a 272c 2027 7074 272c 2027  ', 'cz', 'pt', '
-0003e840: 6a70 272c 2027 6573 275d 0d0a 2020 2020  jp', 'es']..    
-0003e850: 2020 2020 7365 6c66 2e6c 616e 6775 6167      self.languag
-0003e860: 655f 6d61 7020 3d20 4e6f 6e65 0d0a 2020  e_map = None..  
-0003e870: 2020 2020 2020 7365 6c66 2e71 7565 7279        self.query
-0003e880: 5f63 6f75 6e74 203d 2030 0d0a 2020 2020  _count = 0..    
-0003e890: 2020 2020 7365 6c66 2e6f 7574 7075 745f      self.output_
-0003e8a0: 7a68 203d 2027 7a68 270d 0a20 2020 2020  zh = 'zh'..     
-0003e8b0: 2020 2073 656c 662e 696e 7075 745f 6c69     self.input_li
-0003e8c0: 6d69 7420 3d20 696e 7428 3165 3329 0d0a  mit = int(1e3)..
-0003e8d0: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
-0003e8e0: 6175 6c74 5f66 726f 6d5f 6c61 6e67 7561  ault_from_langua
-0003e8f0: 6765 203d 2073 656c 662e 6f75 7470 7574  ge = self.output
-0003e900: 5f7a 680d 0a0d 0a20 2020 2040 5473 652e  _zh....    @Tse.
-0003e910: 6465 6275 675f 6c61 6e67 7561 6765 5f6d  debug_language_m
-0003e920: 6170 0d0a 2020 2020 6465 6620 6765 745f  ap..    def get_
-0003e930: 6c61 6e67 7561 6765 5f6d 6170 2873 656c  language_map(sel
-0003e940: 662c 206c 616e 675f 6c69 7374 3a20 4c69  f, lang_list: Li
-0003e950: 7374 5b73 7472 5d2c 202a 2a6b 7761 7267  st[str], **kwarg
-0003e960: 733a 204c 616e 674d 6170 4b77 6172 6773  s: LangMapKwargs
-0003e970: 5479 7065 2920 2d3e 2064 6963 743a 0d0a  Type) -> dict:..
-0003e980: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-0003e990: 7d2e 6672 6f6d 6b65 7973 286c 616e 675f  }.fromkeys(lang_
-0003e9a0: 6c69 7374 2c20 6c61 6e67 5f6c 6973 7429  list, lang_list)
-0003e9b0: 0d0a 0d0a 2020 2020 4054 7365 2e75 6e63  ....    @Tse.unc
-0003e9c0: 6572 7469 6669 6564 2020 2320 6e6f 7420  ertified  # not 
-0003e9d0: 636f 6465 2c20 6275 7420 7365 7276 6572  code, but server
-0003e9e0: 2e0d 0a20 2020 2040 5473 652e 7469 6d65  ...    @Tse.time
-0003e9f0: 5f73 7461 740d 0a20 2020 2040 5473 652e  _stat..    @Tse.
-0003ea00: 6368 6563 6b5f 7175 6572 790d 0a20 2020  check_query..   
-0003ea10: 2064 6566 2079 6565 6b69 745f 6170 6928   def yeekit_api(
-0003ea20: 7365 6c66 2c20 7175 6572 795f 7465 7874  self, query_text
-0003ea30: 3a20 7374 722c 2066 726f 6d5f 6c61 6e67  : str, from_lang
-0003ea40: 7561 6765 3a20 7374 7220 3d20 2761 7574  uage: str = 'aut
-0003ea50: 6f27 2c20 746f 5f6c 616e 6775 6167 653a  o', to_language:
-0003ea60: 2073 7472 203d 2027 656e 272c 202a 2a6b   str = 'en', **k
-0003ea70: 7761 7267 733a 2041 7069 4b77 6172 6773  wargs: ApiKwargs
-0003ea80: 5479 7065 2920 2d3e 2055 6e69 6f6e 5b73  Type) -> Union[s
-0003ea90: 7472 2c20 6469 6374 5d3a 0d0a 2020 2020  tr, dict]:..    
-0003eaa0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-0003eab0: 2068 7474 7073 3a2f 2f77 7777 2e79 6565   https://www.yee
-0003eac0: 6b69 742e 636f 6d2f 7369 7465 2f74 7261  kit.com/site/tra
-0003ead0: 6e73 6c61 7465 0d0a 2020 2020 2020 2020  nslate..        
-0003eae0: 3a70 6172 616d 2071 7565 7279 5f74 6578  :param query_tex
-0003eaf0: 743a 2073 7472 2c20 6d75 7374 2e0d 0a20  t: str, must... 
-0003eb00: 2020 2020 2020 203a 7061 7261 6d20 6672         :param fr
-0003eb10: 6f6d 5f6c 616e 6775 6167 653a 2073 7472  om_language: str
-0003eb20: 2c20 6465 6661 756c 7420 2761 7574 6f27  , default 'auto'
-0003eb30: 2e0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-0003eb40: 6d20 746f 5f6c 616e 6775 6167 653a 2073  m to_language: s
-0003eb50: 7472 2c20 6465 6661 756c 7420 2765 6e27  tr, default 'en'
-0003eb60: 2e0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-0003eb70: 6d20 2a2a 6b77 6172 6773 3a0d 0a20 2020  m **kwargs:..   
-0003eb80: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-0003eb90: 7261 6d20 7469 6d65 6f75 743a 2066 6c6f  ram timeout: flo
-0003eba0: 6174 2c20 6465 6661 756c 7420 4e6f 6e65  at, default None
-0003ebb0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0003ebc0: 2020 203a 7061 7261 6d20 7072 6f78 6965     :param proxie
-0003ebd0: 733a 2064 6963 742c 2064 6566 6175 6c74  s: dict, default
-0003ebe0: 204e 6f6e 652e 0d0a 2020 2020 2020 2020   None...        
-0003ebf0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-0003ec00: 6c65 6570 5f73 6563 6f6e 6473 3a20 666c  leep_seconds: fl
-0003ec10: 6f61 742c 2064 6566 6175 6c74 2030 2e0d  oat, default 0..
-0003ec20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003ec30: 203a 7061 7261 6d20 6973 5f64 6574 6169   :param is_detai
-0003ec40: 6c5f 7265 7375 6c74 3a20 626f 6f6c 2c20  l_result: bool, 
-0003ec50: 6465 6661 756c 7420 4661 6c73 652e 0d0a  default False...
-0003ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003ec70: 3a70 6172 616d 2069 665f 6967 6e6f 7265  :param if_ignore
-0003ec80: 5f6c 696d 6974 5f6f 665f 6c65 6e67 7468  _limit_of_length
-0003ec90: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-0003eca0: 4661 6c73 652e 0d0a 2020 2020 2020 2020  False...        
-0003ecb0: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
-0003ecc0: 696d 6974 5f6f 665f 6c65 6e67 7468 3a20  imit_of_length: 
-0003ecd0: 696e 742c 2064 6566 6175 6c74 2032 3030  int, default 200
-0003ece0: 3030 2e0d 0a20 2020 2020 2020 2020 2020  00...           
-0003ecf0: 2020 2020 203a 7061 7261 6d20 6966 5f69       :param if_i
-0003ed00: 676e 6f72 655f 656d 7074 795f 7175 6572  gnore_empty_quer
-0003ed10: 793a 2062 6f6f 6c2c 2064 6566 6175 6c74  y: bool, default
-0003ed20: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
-0003ed30: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-0003ed40: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
-0003ed50: 6674 6572 5f66 7265 713a 2069 6e74 2c20  fter_freq: int, 
-0003ed60: 6465 6661 756c 7420 3130 3030 2e0d 0a20  default 1000... 
-0003ed70: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-0003ed80: 7061 7261 6d20 7570 6461 7465 5f73 6573  param update_ses
-0003ed90: 7369 6f6e 5f61 6674 6572 5f73 6563 6f6e  sion_after_secon
-0003eda0: 6473 3a20 666c 6f61 742c 2064 6566 6175  ds: float, defau
-0003edb0: 6c74 2031 3530 302e 0d0a 2020 2020 2020  lt 1500...      
-0003edc0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-0003edd0: 2069 665f 7368 6f77 5f74 696d 655f 7374   if_show_time_st
-0003ede0: 6174 3a20 626f 6f6c 2c20 6465 6661 756c  at: bool, defaul
-0003edf0: 7420 4661 6c73 652e 0d0a 2020 2020 2020  t False...      
-0003ee00: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-0003ee10: 2073 686f 775f 7469 6d65 5f73 7461 745f   show_time_stat_
-0003ee20: 7072 6563 6973 696f 6e3a 2069 6e74 2c20  precision: int, 
-0003ee30: 6465 6661 756c 7420 322e 0d0a 2020 2020  default 2...    
-0003ee40: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-0003ee50: 616d 2069 665f 7072 696e 745f 7761 726e  am if_print_warn
-0003ee60: 696e 673a 2062 6f6f 6c2c 2064 6566 6175  ing: bool, defau
-0003ee70: 6c74 2054 7275 652e 0d0a 2020 2020 2020  lt True...      
-0003ee80: 2020 3a72 6574 7572 6e3a 2073 7472 206f    :return: str o
-0003ee90: 7220 6469 6374 0d0a 2020 2020 2020 2020  r dict..        
-0003eea0: 2222 220d 0a0d 0a20 2020 2020 2020 2074  """....        t
-0003eeb0: 696d 656f 7574 203d 206b 7761 7267 732e  imeout = kwargs.
-0003eec0: 6765 7428 2774 696d 656f 7574 272c 204e  get('timeout', N
-0003eed0: 6f6e 6529 0d0a 2020 2020 2020 2020 7072  one)..        pr
-0003eee0: 6f78 6965 7320 3d20 6b77 6172 6773 2e67  oxies = kwargs.g
-0003eef0: 6574 2827 7072 6f78 6965 7327 2c20 4e6f  et('proxies', No
-0003ef00: 6e65 290d 0a20 2020 2020 2020 2073 6c65  ne)..        sle
-0003ef10: 6570 5f73 6563 6f6e 6473 203d 206b 7761  ep_seconds = kwa
-0003ef20: 7267 732e 6765 7428 2773 6c65 6570 5f73  rgs.get('sleep_s
-0003ef30: 6563 6f6e 6473 272c 2030 290d 0a20 2020  econds', 0)..   
-0003ef40: 2020 2020 2069 665f 7072 696e 745f 7761       if_print_wa
-0003ef50: 726e 696e 6720 3d20 6b77 6172 6773 2e67  rning = kwargs.g
-0003ef60: 6574 2827 6966 5f70 7269 6e74 5f77 6172  et('if_print_war
-0003ef70: 6e69 6e67 272c 2054 7275 6529 0d0a 2020  ning', True)..  
-0003ef80: 2020 2020 2020 6973 5f64 6574 6169 6c5f        is_detail_
-0003ef90: 7265 7375 6c74 203d 206b 7761 7267 732e  result = kwargs.
-0003efa0: 6765 7428 2769 735f 6465 7461 696c 5f72  get('is_detail_r
-0003efb0: 6573 756c 7427 2c20 4661 6c73 6529 0d0a  esult', False)..
-0003efc0: 2020 2020 2020 2020 7570 6461 7465 5f73          update_s
-0003efd0: 6573 7369 6f6e 5f61 6674 6572 5f66 7265  ession_after_fre
-0003efe0: 7120 3d20 6b77 6172 6773 2e67 6574 2827  q = kwargs.get('
-0003eff0: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
-0003f000: 6674 6572 5f66 7265 7127 2c20 7365 6c66  fter_freq', self
-0003f010: 2e64 6566 6175 6c74 5f73 6573 7369 6f6e  .default_session
-0003f020: 5f66 7265 7129 0d0a 2020 2020 2020 2020  _freq)..        
-0003f030: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
-0003f040: 6674 6572 5f73 6563 6f6e 6473 203d 206b  fter_seconds = k
-0003f050: 7761 7267 732e 6765 7428 2775 7064 6174  wargs.get('updat
-0003f060: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
-0003f070: 7365 636f 6e64 7327 2c20 7365 6c66 2e64  seconds', self.d
-0003f080: 6566 6175 6c74 5f73 6573 7369 6f6e 5f73  efault_session_s
-0003f090: 6563 6f6e 6473 290d 0a20 2020 2020 2020  econds)..       
-0003f0a0: 2073 656c 662e 6368 6563 6b5f 696e 7075   self.check_inpu
-0003f0b0: 745f 6c69 6d69 7428 7175 6572 795f 7465  t_limit(query_te
-0003f0c0: 7874 2c20 7365 6c66 2e69 6e70 7574 5f6c  xt, self.input_l
-0003f0d0: 696d 6974 290d 0a0d 0a20 2020 2020 2020  imit)....       
-0003f0e0: 206e 6f74 5f75 7064 6174 655f 636f 6e64   not_update_cond
-0003f0f0: 5f66 7265 7120 3d20 3120 6966 2073 656c  _freq = 1 if sel
-0003f100: 662e 7175 6572 795f 636f 756e 7420 3c20  f.query_count < 
-0003f110: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
-0003f120: 6674 6572 5f66 7265 7120 656c 7365 2030  fter_freq else 0
-0003f130: 0d0a 2020 2020 2020 2020 6e6f 745f 7570  ..        not_up
-0003f140: 6461 7465 5f63 6f6e 645f 7469 6d65 203d  date_cond_time =
-0003f150: 2031 2069 6620 7469 6d65 2e74 696d 6528   1 if time.time(
-0003f160: 2920 2d20 7365 6c66 2e62 6567 696e 5f74  ) - self.begin_t
-0003f170: 696d 6520 3c20 7570 6461 7465 5f73 6573  ime < update_ses
-0003f180: 7369 6f6e 5f61 6674 6572 5f73 6563 6f6e  sion_after_secon
-0003f190: 6473 2065 6c73 6520 300d 0a20 2020 2020  ds else 0..     
-0003f1a0: 2020 2069 6620 6e6f 7420 2873 656c 662e     if not (self.
-0003f1b0: 7365 7373 696f 6e20 616e 6420 7365 6c66  session and self
-0003f1c0: 2e6c 616e 6775 6167 655f 6d61 7020 616e  .language_map an
-0003f1d0: 6420 6e6f 745f 7570 6461 7465 5f63 6f6e  d not_update_con
-0003f1e0: 645f 6672 6571 2061 6e64 206e 6f74 5f75  d_freq and not_u
-0003f1f0: 7064 6174 655f 636f 6e64 5f74 696d 6529  pdate_cond_time)
-0003f200: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-0003f210: 656c 662e 7365 7373 696f 6e20 3d20 7265  elf.session = re
-0003f220: 7175 6573 7473 2e53 6573 7369 6f6e 2829  quests.Session()
-0003f230: 0d0a 2020 2020 2020 2020 2020 2020 5f20  ..            _ 
-0003f240: 3d20 7365 6c66 2e73 6573 7369 6f6e 2e67  = self.session.g
-0003f250: 6574 2873 656c 662e 686f 7374 5f75 726c  et(self.host_url
-0003f260: 2c20 6865 6164 6572 733d 7365 6c66 2e68  , headers=self.h
-0003f270: 6f73 745f 6865 6164 6572 732c 2074 696d  ost_headers, tim
-0003f280: 656f 7574 3d74 696d 656f 7574 2c20 7072  eout=timeout, pr
-0003f290: 6f78 6965 733d 7072 6f78 6965 7329 0d0a  oxies=proxies)..
-0003f2a0: 2020 2020 2020 2020 2020 2020 6465 6275              debu
-0003f2b0: 675f 6c61 6e67 5f6b 7761 7267 7320 3d20  g_lang_kwargs = 
-0003f2c0: 7365 6c66 2e64 6562 7567 5f6c 616e 675f  self.debug_lang_
-0003f2d0: 6b77 6172 6773 2866 726f 6d5f 6c61 6e67  kwargs(from_lang
-0003f2e0: 7561 6765 2c20 746f 5f6c 616e 6775 6167  uage, to_languag
-0003f2f0: 652c 2073 656c 662e 6465 6661 756c 745f  e, self.default_
-0003f300: 6672 6f6d 5f6c 616e 6775 6167 652c 2069  from_language, i
-0003f310: 665f 7072 696e 745f 7761 726e 696e 6729  f_print_warning)
-0003f320: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0003f330: 6c66 2e6c 616e 6775 6167 655f 6d61 7020  lf.language_map 
-0003f340: 3d20 7365 6c66 2e67 6574 5f6c 616e 6775  = self.get_langu
-0003f350: 6167 655f 6d61 7028 7365 6c66 2e6c 616e  age_map(self.lan
-0003f360: 675f 6c69 7374 2c20 2a2a 6465 6275 675f  g_list, **debug_
-0003f370: 6c61 6e67 5f6b 7761 7267 7329 0d0a 0d0a  lang_kwargs)....
-0003f380: 2020 2020 2020 2020 6966 2066 726f 6d5f          if from_
-0003f390: 6c61 6e67 7561 6765 203d 3d20 2761 7574  language == 'aut
-0003f3a0: 6f27 3a0d 0a20 2020 2020 2020 2020 2020  o':..           
-0003f3b0: 2066 726f 6d5f 6c61 6e67 7561 6765 203d   from_language =
-0003f3c0: 2073 656c 662e 7761 726e 696e 675f 6175   self.warning_au
-0003f3d0: 746f 5f6c 616e 6728 2779 6565 6b69 7427  to_lang('yeekit'
-0003f3e0: 2c20 7365 6c66 2e64 6566 6175 6c74 5f66  , self.default_f
-0003f3f0: 726f 6d5f 6c61 6e67 7561 6765 2c20 6966  rom_language, if
-0003f400: 5f70 7269 6e74 5f77 6172 6e69 6e67 290d  _print_warning).
-0003f410: 0a20 2020 2020 2020 2066 726f 6d5f 6c61  .        from_la
-0003f420: 6e67 7561 6765 2c20 746f 5f6c 616e 6775  nguage, to_langu
-0003f430: 6167 6520 3d20 7365 6c66 2e63 6865 636b  age = self.check
-0003f440: 5f6c 616e 6775 6167 6528 6672 6f6d 5f6c  _language(from_l
-0003f450: 616e 6775 6167 652c 2074 6f5f 6c61 6e67  anguage, to_lang
-0003f460: 7561 6765 2c20 7365 6c66 2e6c 616e 6775  uage, self.langu
-0003f470: 6167 655f 6d61 7029 0d0a 0d0a 2020 2020  age_map)....    
-0003f480: 2020 2020 7061 796c 6f61 6420 3d20 7b0d      payload = {.
-0003f490: 0a20 2020 2020 2020 2020 2020 2027 636f  .            'co
-0003f4a0: 6e74 656e 745b 5d27 3a20 7175 6572 795f  ntent[]': query_
-0003f4b0: 7465 7874 2c0d 0a20 2020 2020 2020 2020  text,..         
-0003f4c0: 2020 2027 736f 7572 6365 4c61 6e67 273a     'sourceLang':
-0003f4d0: 2066 276e 7b66 726f 6d5f 6c61 6e67 7561   f'n{from_langua
-0003f4e0: 6765 7d27 2c0d 0a20 2020 2020 2020 2020  ge}',..         
-0003f4f0: 2020 2027 7461 7267 6574 4c61 6e67 273a     'targetLang':
-0003f500: 2066 276e 7b74 6f5f 6c61 6e67 7561 6765   f'n{to_language
-0003f510: 7d27 2c0d 0a20 2020 2020 2020 207d 0d0a  }',..        }..
-0003f520: 2020 2020 2020 2020 7061 796c 6f61 6420          payload 
-0003f530: 3d20 7572 6c6c 6962 2e70 6172 7365 2e75  = urllib.parse.u
-0003f540: 726c 656e 636f 6465 2870 6179 6c6f 6164  rlencode(payload
-0003f550: 290d 0a20 2020 2020 2020 2072 203d 2073  )..        r = s
-0003f560: 656c 662e 7365 7373 696f 6e2e 706f 7374  elf.session.post
-0003f570: 2873 656c 662e 6170 695f 7572 6c2c 2064  (self.api_url, d
-0003f580: 6174 613d 7061 796c 6f61 642c 2068 6561  ata=payload, hea
-0003f590: 6465 7273 3d73 656c 662e 6170 695f 6865  ders=self.api_he
-0003f5a0: 6164 6572 732c 2074 696d 656f 7574 3d74  aders, timeout=t
-0003f5b0: 696d 656f 7574 2c20 7072 6f78 6965 733d  imeout, proxies=
-0003f5c0: 7072 6f78 6965 7329 0d0a 2020 2020 2020  proxies)..      
-0003f5d0: 2020 722e 7261 6973 655f 666f 725f 7374    r.raise_for_st
-0003f5e0: 6174 7573 2829 0d0a 2020 2020 2020 2020  atus()..        
-0003f5f0: 6461 7461 203d 2072 2e6a 736f 6e28 290d  data = r.json().
-0003f600: 0a20 2020 2020 2020 2074 696d 652e 736c  .        time.sl
-0003f610: 6565 7028 736c 6565 705f 7365 636f 6e64  eep(sleep_second
-0003f620: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
-0003f630: 2e71 7565 7279 5f63 6f75 6e74 202b 3d20  .query_count += 
-0003f640: 310d 0a20 2020 2020 2020 2072 6574 7572  1..        retur
-0003f650: 6e20 6461 7461 2069 6620 6973 5f64 6574  n data if is_det
-0003f660: 6169 6c5f 7265 7375 6c74 2065 6c73 6520  ail_result else 
-0003f670: 275c 6e27 2e6a 6f69 6e28 2720 272e 6a6f  '\n'.join(' '.jo
-0003f680: 696e 2870 2920 666f 7220 7020 696e 206a  in(p) for p in j
-0003f690: 736f 6e2e 6c6f 6164 7328 6461 7461 5b30  son.loads(data[0
-0003f6a0: 5d29 5b27 7472 616e 736c 6174 696f 6e27  ])['translation'
-0003f6b0: 5d5b 305d 5b27 7472 616e 736c 6174 6564  ][0]['translated
-0003f6c0: 275d 5b30 5d5b 2774 7261 6e73 6c61 7469  '][0]['translati
-0003f6d0: 6f6e 206c 6973 7427 5d29 0d0a 0d0a 0d0a  on list'])......
-0003f6e0: 636c 6173 7320 5472 616e 736c 6174 6f72  class Translator
-0003f6f0: 7353 6572 7665 723a 0d0a 2020 2020 6465  sServer:..    de
-0003f700: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
-0003f710: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-0003f720: 6370 755f 636e 7420 3d20 6f73 2e63 7075  cpu_cnt = os.cpu
-0003f730: 5f63 6f75 6e74 2829 0d0a 2020 2020 2020  _count()..      
-0003f740: 2020 7365 6c66 2e73 6572 7665 725f 7265    self.server_re
-0003f750: 6769 6f6e 203d 2047 7565 7374 5365 7665  gion = GuestSeve
-0003f760: 7252 6567 696f 6e28 292e 6765 745f 7365  rRegion().get_se
-0003f770: 7276 6572 5f72 6567 696f 6e0d 0a20 2020  rver_region..   
-0003f780: 2020 2020 2073 656c 662e 5f61 6c69 6261       self._aliba
-0003f790: 6261 203d 2041 6c69 6261 6261 5632 2829  ba = AlibabaV2()
-0003f7a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-0003f7b0: 6c69 6261 6261 203d 2073 656c 662e 5f61  libaba = self._a
-0003f7c0: 6c69 6261 6261 2e61 6c69 6261 6261 5f61  libaba.alibaba_a
-0003f7d0: 7069 0d0a 2020 2020 2020 2020 7365 6c66  pi..        self
-0003f7e0: 2e5f 6170 6572 7469 756d 203d 2041 7065  ._apertium = Ape
-0003f7f0: 7274 6975 6d28 290d 0a20 2020 2020 2020  rtium()..       
-0003f800: 2073 656c 662e 6170 6572 7469 756d 203d   self.apertium =
-0003f810: 2073 656c 662e 5f61 7065 7274 6975 6d2e   self._apertium.
-0003f820: 6170 6572 7469 756d 5f61 7069 0d0a 2020  apertium_api..  
-0003f830: 2020 2020 2020 7365 6c66 2e5f 6172 676f        self._argo
-0003f840: 7320 3d20 4172 676f 7328 290d 0a20 2020  s = Argos()..   
-0003f850: 2020 2020 2073 656c 662e 6172 676f 7320       self.argos 
-0003f860: 3d20 7365 6c66 2e5f 6172 676f 732e 6172  = self._argos.ar
-0003f870: 676f 735f 6170 690d 0a20 2020 2020 2020  gos_api..       
-0003f880: 2073 656c 662e 5f62 6169 6475 203d 2042   self._baidu = B
-0003f890: 6169 6475 5631 2829 2020 2320 5632 0d0a  aiduV1()  # V2..
-0003f8a0: 2020 2020 2020 2020 7365 6c66 2e62 6169          self.bai
-0003f8b0: 6475 203d 2073 656c 662e 5f62 6169 6475  du = self._baidu
-0003f8c0: 2e62 6169 6475 5f61 7069 0d0a 2020 2020  .baidu_api..    
-0003f8d0: 2020 2020 7365 6c66 2e5f 6269 6e67 203d      self._bing =
-0003f8e0: 2042 696e 6728 7365 7276 6572 5f72 6567   Bing(server_reg
-0003f8f0: 696f 6e3d 7365 6c66 2e73 6572 7665 725f  ion=self.server_
-0003f900: 7265 6769 6f6e 290d 0a20 2020 2020 2020  region)..       
-0003f910: 2073 656c 662e 6269 6e67 203d 2073 656c   self.bing = sel
-0003f920: 662e 5f62 696e 672e 6269 6e67 5f61 7069  f._bing.bing_api
-0003f930: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-0003f940: 6361 6979 756e 203d 2043 6169 7975 6e28  caiyun = Caiyun(
-0003f950: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0003f960: 6361 6979 756e 203d 2073 656c 662e 5f63  caiyun = self._c
-0003f970: 6169 7975 6e2e 6361 6979 756e 5f61 7069  aiyun.caiyun_api
-0003f980: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-0003f990: 636c 6f75 6459 6920 3d20 436c 6f75 6459  cloudYi = CloudY
-0003f9a0: 6928 290d 0a20 2020 2020 2020 2073 656c  i()..        sel
-0003f9b0: 662e 636c 6f75 6459 6920 3d20 7365 6c66  f.cloudYi = self
-0003f9c0: 2e5f 636c 6f75 6459 692e 636c 6f75 6459  ._cloudYi.cloudY
-0003f9d0: 695f 6170 690d 0a20 2020 2020 2020 2073  i_api..        s
-0003f9e0: 656c 662e 5f64 6565 706c 203d 2044 6565  elf._deepl = Dee
-0003f9f0: 706c 2829 0d0a 2020 2020 2020 2020 7365  pl()..        se
-0003fa00: 6c66 2e64 6565 706c 203d 2073 656c 662e  lf.deepl = self.
-0003fa10: 5f64 6565 706c 2e64 6565 706c 5f61 7069  _deepl.deepl_api
-0003fa20: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-0003fa30: 656c 6961 203d 2045 6c69 6128 290d 0a20  elia = Elia().. 
-0003fa40: 2020 2020 2020 2073 656c 662e 656c 6961         self.elia
-0003fa50: 203d 2073 656c 662e 5f65 6c69 612e 656c   = self._elia.el
-0003fa60: 6961 5f61 7069 0d0a 2020 2020 2020 2020  ia_api..        
-0003fa70: 7365 6c66 2e5f 676f 6f67 6c65 203d 2047  self._google = G
-0003fa80: 6f6f 676c 6556 3228 7365 7276 6572 5f72  oogleV2(server_r
-0003fa90: 6567 696f 6e3d 7365 6c66 2e73 6572 7665  egion=self.serve
-0003faa0: 725f 7265 6769 6f6e 290d 0a20 2020 2020  r_region)..     
-0003fab0: 2020 2073 656c 662e 676f 6f67 6c65 203d     self.google =
-0003fac0: 2073 656c 662e 5f67 6f6f 676c 652e 676f   self._google.go
-0003fad0: 6f67 6c65 5f61 7069 0d0a 2020 2020 2020  ogle_api..      
-0003fae0: 2020 7365 6c66 2e5f 6963 6962 6120 3d20    self._iciba = 
-0003faf0: 4963 6962 6128 290d 0a20 2020 2020 2020  Iciba()..       
-0003fb00: 2073 656c 662e 6963 6962 6120 3d20 7365   self.iciba = se
-0003fb10: 6c66 2e5f 6963 6962 612e 6963 6962 615f  lf._iciba.iciba_
-0003fb20: 6170 690d 0a20 2020 2020 2020 2073 656c  api..        sel
-0003fb30: 662e 5f69 666c 7974 656b 203d 2049 666c  f._iflytek = Ifl
-0003fb40: 7974 656b 5632 2829 0d0a 2020 2020 2020  ytekV2()..      
-0003fb50: 2020 7365 6c66 2e69 666c 7974 656b 203d    self.iflytek =
-0003fb60: 2073 656c 662e 5f69 666c 7974 656b 2e69   self._iflytek.i
-0003fb70: 666c 7974 656b 5f61 7069 0d0a 2020 2020  flytek_api..    
-0003fb80: 2020 2020 7365 6c66 2e5f 6966 6c79 7265      self._iflyre
-0003fb90: 6320 3d20 4966 6c79 7265 6328 290d 0a20  c = Iflyrec().. 
-0003fba0: 2020 2020 2020 2073 656c 662e 6966 6c79         self.ifly
-0003fbb0: 7265 6320 3d20 7365 6c66 2e5f 6966 6c79  rec = self._ifly
-0003fbc0: 7265 632e 6966 6c79 7265 635f 6170 690d  rec.iflyrec_api.
-0003fbd0: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
-0003fbe0: 7472 616e 736c 6174 6520 3d20 4974 7261  translate = Itra
-0003fbf0: 6e73 6c61 7465 2829 0d0a 2020 2020 2020  nslate()..      
-0003fc00: 2020 7365 6c66 2e69 7472 616e 736c 6174    self.itranslat
-0003fc10: 6520 3d20 7365 6c66 2e5f 6974 7261 6e73  e = self._itrans
-0003fc20: 6c61 7465 2e69 7472 616e 736c 6174 655f  late.itranslate_
-0003fc30: 6170 690d 0a20 2020 2020 2020 2073 656c  api..        sel
-0003fc40: 662e 5f6a 7564 6963 203d 204a 7564 6963  f._judic = Judic
-0003fc50: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-0003fc60: 2e6a 7564 6963 203d 2073 656c 662e 5f6a  .judic = self._j
-0003fc70: 7564 6963 2e6a 7564 6963 5f61 7069 0d0a  udic.judic_api..
-0003fc80: 2020 2020 2020 2020 7365 6c66 2e5f 6c61          self._la
-0003fc90: 6e67 7561 6765 5769 7265 203d 204c 616e  nguageWire = Lan
-0003fca0: 6775 6167 6557 6972 6528 290d 0a20 2020  guageWire()..   
-0003fcb0: 2020 2020 2073 656c 662e 6c61 6e67 7561       self.langua
-0003fcc0: 6765 5769 7265 203d 2073 656c 662e 5f6c  geWire = self._l
-0003fcd0: 616e 6775 6167 6557 6972 652e 6c61 6e67  anguageWire.lang
-0003fce0: 7561 6765 5769 7265 5f61 7069 0d0a 2020  uageWire_api..  
-0003fcf0: 2020 2020 2020 7365 6c66 2e5f 6c69 6e67        self._ling
-0003fd00: 7661 6e65 7820 3d20 4c69 6e67 7661 6e65  vanex = Lingvane
-0003fd10: 7828 290d 0a20 2020 2020 2020 2073 656c  x()..        sel
-0003fd20: 662e 6c69 6e67 7661 6e65 7820 3d20 7365  f.lingvanex = se
-0003fd30: 6c66 2e5f 6c69 6e67 7661 6e65 782e 6c69  lf._lingvanex.li
-0003fd40: 6e67 7661 6e65 785f 6170 690d 0a20 2020  ngvanex_api..   
-0003fd50: 2020 2020 2073 656c 662e 5f6e 6975 7472       self._niutr
-0003fd60: 616e 7320 3d20 4e69 7574 7261 6e73 2829  ans = Niutrans()
-0003fd70: 0d0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-0003fd80: 6975 7472 616e 7320 3d20 7365 6c66 2e5f  iutrans = self._
-0003fd90: 6e69 7574 7261 6e73 2e6e 6975 7472 616e  niutrans.niutran
-0003fda0: 735f 6170 690d 0a20 2020 2020 2020 2073  s_api..        s
-0003fdb0: 656c 662e 5f6d 676c 6970 203d 204d 676c  elf._mglip = Mgl
-0003fdc0: 6970 2829 0d0a 2020 2020 2020 2020 7365  ip()..        se
-0003fdd0: 6c66 2e6d 676c 6970 203d 2073 656c 662e  lf.mglip = self.
-0003fde0: 5f6d 676c 6970 2e6d 676c 6970 5f61 7069  _mglip.mglip_api
-0003fdf0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-0003fe00: 6d69 7261 6920 3d20 4d69 7261 6928 290d  mirai = Mirai().
-0003fe10: 0a20 2020 2020 2020 2073 656c 662e 6d69  .        self.mi
-0003fe20: 7261 6920 3d20 7365 6c66 2e5f 6d69 7261  rai = self._mira
-0003fe30: 692e 6d69 7261 695f 6170 690d 0a20 2020  i.mirai_api..   
-0003fe40: 2020 2020 2073 656c 662e 5f6d 6f64 6572       self._moder
-0003fe50: 6e4d 7420 3d20 4d6f 6465 726e 4d74 2829  nMt = ModernMt()
-0003fe60: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-0003fe70: 6f64 6572 6e4d 7420 3d20 7365 6c66 2e5f  odernMt = self._
-0003fe80: 6d6f 6465 726e 4d74 2e6d 6f64 6572 6e4d  modernMt.modernM
-0003fe90: 745f 6170 690d 0a20 2020 2020 2020 2073  t_api..        s
-0003fea0: 656c 662e 5f6d 794d 656d 6f72 7920 3d20  elf._myMemory = 
-0003feb0: 4d79 4d65 6d6f 7279 2829 0d0a 2020 2020  MyMemory()..    
-0003fec0: 2020 2020 7365 6c66 2e6d 794d 656d 6f72      self.myMemor
-0003fed0: 7920 3d20 7365 6c66 2e5f 6d79 4d65 6d6f  y = self._myMemo
-0003fee0: 7279 2e6d 794d 656d 6f72 795f 6170 690d  ry.myMemory_api.
-0003fef0: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
-0003ff00: 6170 6167 6f20 3d20 5061 7061 676f 2829  apago = Papago()
-0003ff10: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-0003ff20: 6170 6167 6f20 3d20 7365 6c66 2e5f 7061  apago = self._pa
-0003ff30: 7061 676f 2e70 6170 6167 6f5f 6170 690d  pago.papago_api.
-0003ff40: 0a20 2020 2020 2020 2073 656c 662e 5f71  .        self._q
-0003ff50: 7146 616e 7969 203d 2051 5146 616e 7969  qFanyi = QQFanyi
-0003ff60: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-0003ff70: 2e71 7146 616e 7969 203d 2073 656c 662e  .qqFanyi = self.
-0003ff80: 5f71 7146 616e 7969 2e71 7146 616e 7969  _qqFanyi.qqFanyi
-0003ff90: 5f61 7069 0d0a 2020 2020 2020 2020 7365  _api..        se
-0003ffa0: 6c66 2e5f 7171 5472 616e 536d 6172 7420  lf._qqTranSmart 
-0003ffb0: 3d20 5151 5472 616e 536d 6172 7428 290d  = QQTranSmart().
-0003ffc0: 0a20 2020 2020 2020 2073 656c 662e 7171  .        self.qq
-0003ffd0: 5472 616e 536d 6172 7420 3d20 7365 6c66  TranSmart = self
-0003ffe0: 2e5f 7171 5472 616e 536d 6172 742e 7171  ._qqTranSmart.qq
-0003fff0: 5472 616e 536d 6172 745f 6170 690d 0a20  TranSmart_api.. 
-00040000: 2020 2020 2020 2073 656c 662e 5f72 6576         self._rev
-00040010: 6572 736f 203d 2052 6576 6572 736f 2829  erso = Reverso()
-00040020: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-00040030: 6576 6572 736f 203d 2073 656c 662e 5f72  everso = self._r
-00040040: 6576 6572 736f 2e72 6576 6572 736f 5f61  everso.reverso_a
-00040050: 7069 0d0a 2020 2020 2020 2020 7365 6c66  pi..        self
-00040060: 2e5f 736f 676f 7520 3d20 536f 676f 7528  ._sogou = Sogou(
-00040070: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00040080: 736f 676f 7520 3d20 7365 6c66 2e5f 736f  sogou = self._so
-00040090: 676f 752e 736f 676f 755f 6170 690d 0a20  gou.sogou_api.. 
-000400a0: 2020 2020 2020 2073 656c 662e 5f73 7973         self._sys
-000400b0: 5472 616e 203d 2053 7973 5472 616e 2829  Tran = SysTran()
-000400c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-000400d0: 7973 5472 616e 203d 2073 656c 662e 5f73  ysTran = self._s
-000400e0: 7973 5472 616e 2e73 7973 5472 616e 5f61  ysTran.sysTran_a
-000400f0: 7069 0d0a 2020 2020 2020 2020 7365 6c66  pi..        self
-00040100: 2e5f 7469 6c64 6520 3d20 5469 6c64 6528  ._tilde = Tilde(
-00040110: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00040120: 7469 6c64 6520 3d20 7365 6c66 2e5f 7469  tilde = self._ti
-00040130: 6c64 652e 7469 6c64 655f 6170 690d 0a20  lde.tilde_api.. 
-00040140: 2020 2020 2020 2073 656c 662e 5f74 7261         self._tra
-00040150: 6e73 6c61 7465 436f 6d20 3d20 5472 616e  nslateCom = Tran
-00040160: 736c 6174 6543 6f6d 2829 0d0a 2020 2020  slateCom()..    
-00040170: 2020 2020 7365 6c66 2e74 7261 6e73 6c61      self.transla
-00040180: 7465 436f 6d20 3d20 7365 6c66 2e5f 7472  teCom = self._tr
-00040190: 616e 736c 6174 6543 6f6d 2e74 7261 6e73  anslateCom.trans
-000401a0: 6c61 7465 436f 6d5f 6170 690d 0a20 2020  lateCom_api..   
-000401b0: 2020 2020 2073 656c 662e 5f74 7261 6e73       self._trans
-000401c0: 6c61 7465 4d65 203d 2054 7261 6e73 6c61  lateMe = Transla
-000401d0: 7465 4d65 2829 0d0a 2020 2020 2020 2020  teMe()..        
-000401e0: 7365 6c66 2e74 7261 6e73 6c61 7465 4d65  self.translateMe
-000401f0: 203d 2073 656c 662e 5f74 7261 6e73 6c61   = self._transla
-00040200: 7465 4d65 2e74 7261 6e73 6c61 7465 4d65  teMe.translateMe
-00040210: 5f61 7069 0d0a 2020 2020 2020 2020 7365  _api..        se
-00040220: 6c66 2e5f 7574 6962 6574 203d 2055 7469  lf._utibet = Uti
-00040230: 6265 7428 290d 0a20 2020 2020 2020 2073  bet()..        s
-00040240: 656c 662e 7574 6962 6574 203d 2073 656c  elf.utibet = sel
-00040250: 662e 5f75 7469 6265 742e 7574 6962 6574  f._utibet.utibet
-00040260: 5f61 7069 0d0a 2020 2020 2020 2020 7365  _api..        se
-00040270: 6c66 2e5f 766f 6c63 456e 6769 6e65 203d  lf._volcEngine =
-00040280: 2056 6f6c 6345 6e67 696e 6528 290d 0a20   VolcEngine().. 
-00040290: 2020 2020 2020 2073 656c 662e 766f 6c63         self.volc
-000402a0: 456e 6769 6e65 203d 2073 656c 662e 5f76  Engine = self._v
-000402b0: 6f6c 6345 6e67 696e 652e 766f 6c63 456e  olcEngine.volcEn
-000402c0: 6769 6e65 5f61 7069 0d0a 2020 2020 2020  gine_api..      
-000402d0: 2020 7365 6c66 2e5f 7961 6e64 6578 203d    self._yandex =
-000402e0: 2059 616e 6465 7828 290d 0a20 2020 2020   Yandex()..     
-000402f0: 2020 2073 656c 662e 7961 6e64 6578 203d     self.yandex =
-00040300: 2073 656c 662e 5f79 616e 6465 782e 7961   self._yandex.ya
-00040310: 6e64 6578 5f61 7069 0d0a 2020 2020 2020  ndex_api..      
-00040320: 2020 7365 6c66 2e5f 7965 656b 6974 203d    self._yeekit =
-00040330: 2059 6565 6b69 7428 290d 0a20 2020 2020   Yeekit()..     
-00040340: 2020 2073 656c 662e 7965 656b 6974 203d     self.yeekit =
-00040350: 2073 656c 662e 5f79 6565 6b69 742e 7965   self._yeekit.ye
-00040360: 656b 6974 5f61 7069 0d0a 2020 2020 2020  ekit_api..      
-00040370: 2020 7365 6c66 2e5f 796f 7564 616f 203d    self._youdao =
-00040380: 2059 6f75 6461 6f56 3328 290d 0a20 2020   YoudaoV3()..   
-00040390: 2020 2020 2073 656c 662e 796f 7564 616f       self.youdao
-000403a0: 203d 2073 656c 662e 5f79 6f75 6461 6f2e   = self._youdao.
-000403b0: 796f 7564 616f 5f61 7069 0d0a 2020 2020  youdao_api..    
-000403c0: 2020 2020 7365 6c66 2e74 7261 6e73 6c61      self.transla
-000403d0: 746f 7273 5f64 6963 7420 3d20 7b0d 0a20  tors_dict = {.. 
-000403e0: 2020 2020 2020 2020 2020 2027 616c 6962             'alib
-000403f0: 6162 6127 3a20 7365 6c66 2e61 6c69 6261  aba': self.aliba
-00040400: 6261 2c20 2761 7065 7274 6975 6d27 3a20  ba, 'apertium': 
-00040410: 7365 6c66 2e61 7065 7274 6975 6d2c 2027  self.apertium, '
-00040420: 6172 676f 7327 3a20 7365 6c66 2e61 7267  argos': self.arg
-00040430: 6f73 2c20 2762 6169 6475 273a 2073 656c  os, 'baidu': sel
-00040440: 662e 6261 6964 752c 2027 6269 6e67 273a  f.baidu, 'bing':
-00040450: 2073 656c 662e 6269 6e67 2c0d 0a20 2020   self.bing,..   
-00040460: 2020 2020 2020 2020 2027 6361 6979 756e           'caiyun
-00040470: 273a 2073 656c 662e 6361 6979 756e 2c20  ': self.caiyun, 
-00040480: 2763 6c6f 7564 5969 273a 2073 656c 662e  'cloudYi': self.
-00040490: 636c 6f75 6459 692c 2027 6465 6570 6c27  cloudYi, 'deepl'
-000404a0: 3a20 7365 6c66 2e64 6565 706c 2c20 2765  : self.deepl, 'e
-000404b0: 6c69 6127 3a20 7365 6c66 2e65 6c69 612c  lia': self.elia,
-000404c0: 2027 676f 6f67 6c65 273a 2073 656c 662e   'google': self.
-000404d0: 676f 6f67 6c65 2c0d 0a20 2020 2020 2020  google,..       
-000404e0: 2020 2020 2027 6963 6962 6127 3a20 7365       'iciba': se
-000404f0: 6c66 2e69 6369 6261 2c20 2769 666c 7974  lf.iciba, 'iflyt
-00040500: 656b 273a 2073 656c 662e 6966 6c79 7465  ek': self.iflyte
-00040510: 6b2c 2027 6966 6c79 7265 6327 3a20 7365  k, 'iflyrec': se
-00040520: 6c66 2e69 666c 7972 6563 2c20 2769 7472  lf.iflyrec, 'itr
-00040530: 616e 736c 6174 6527 3a20 7365 6c66 2e69  anslate': self.i
-00040540: 7472 616e 736c 6174 652c 2027 6a75 6469  translate, 'judi
-00040550: 6327 3a20 7365 6c66 2e6a 7564 6963 2c0d  c': self.judic,.
-00040560: 0a20 2020 2020 2020 2020 2020 2027 6c61  .            'la
-00040570: 6e67 7561 6765 5769 7265 273a 2073 656c  nguageWire': sel
-00040580: 662e 6c61 6e67 7561 6765 5769 7265 2c20  f.languageWire, 
-00040590: 276c 696e 6776 616e 6578 273a 2073 656c  'lingvanex': sel
-000405a0: 662e 6c69 6e67 7661 6e65 782c 2027 6e69  f.lingvanex, 'ni
-000405b0: 7574 7261 6e73 273a 2073 656c 662e 6e69  utrans': self.ni
-000405c0: 7574 7261 6e73 2c20 276d 676c 6970 273a  utrans, 'mglip':
-000405d0: 2073 656c 662e 6d67 6c69 702c 2027 6d6f   self.mglip, 'mo
-000405e0: 6465 726e 4d74 273a 2073 656c 662e 6d6f  dernMt': self.mo
-000405f0: 6465 726e 4d74 2c0d 0a20 2020 2020 2020  dernMt,..       
-00040600: 2020 2020 2027 6d79 4d65 6d6f 7279 273a       'myMemory':
-00040610: 2073 656c 662e 6d79 4d65 6d6f 7279 2c20   self.myMemory, 
-00040620: 2770 6170 6167 6f27 3a20 7365 6c66 2e70  'papago': self.p
-00040630: 6170 6167 6f2c 2027 7171 4661 6e79 6927  apago, 'qqFanyi'
-00040640: 3a20 7365 6c66 2e71 7146 616e 7969 2c20  : self.qqFanyi, 
-00040650: 2771 7154 7261 6e53 6d61 7274 273a 2073  'qqTranSmart': s
-00040660: 656c 662e 7171 5472 616e 536d 6172 742c  elf.qqTranSmart,
-00040670: 2027 7265 7665 7273 6f27 3a20 7365 6c66   'reverso': self
-00040680: 2e72 6576 6572 736f 2c0d 0a20 2020 2020  .reverso,..     
-00040690: 2020 2020 2020 2027 736f 676f 7527 3a20         'sogou': 
-000406a0: 7365 6c66 2e73 6f67 6f75 2c20 2773 7973  self.sogou, 'sys
-000406b0: 5472 616e 273a 2073 656c 662e 7379 7354  Tran': self.sysT
-000406c0: 7261 6e2c 2027 7469 6c64 6527 3a20 7365  ran, 'tilde': se
-000406d0: 6c66 2e74 696c 6465 2c20 2774 7261 6e73  lf.tilde, 'trans
-000406e0: 6c61 7465 436f 6d27 3a20 7365 6c66 2e74  lateCom': self.t
-000406f0: 7261 6e73 6c61 7465 436f 6d2c 2027 7472  ranslateCom, 'tr
-00040700: 616e 736c 6174 654d 6527 3a20 7365 6c66  anslateMe': self
-00040710: 2e74 7261 6e73 6c61 7465 4d65 2c0d 0a20  .translateMe,.. 
-00040720: 2020 2020 2020 2020 2020 2027 7574 6962             'utib
-00040730: 6574 273a 2073 656c 662e 7574 6962 6574  et': self.utibet
-00040740: 2c20 2776 6f6c 6345 6e67 696e 6527 3a20  , 'volcEngine': 
-00040750: 7365 6c66 2e76 6f6c 6345 6e67 696e 652c  self.volcEngine,
-00040760: 2027 7961 6e64 6578 273a 2073 656c 662e   'yandex': self.
-00040770: 7961 6e64 6578 2c20 2779 6565 6b69 7427  yandex, 'yeekit'
-00040780: 3a20 7365 6c66 2e79 6565 6b69 742c 2027  : self.yeekit, '
-00040790: 796f 7564 616f 273a 2073 656c 662e 796f  youdao': self.yo
-000407a0: 7564 616f 2c0d 0a20 2020 2020 2020 207d  udao,..        }
-000407b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-000407c0: 7261 6e73 6c61 746f 7273 5f70 6f6f 6c20  ranslators_pool 
-000407d0: 3d20 6c69 7374 2873 656c 662e 7472 616e  = list(self.tran
-000407e0: 736c 6174 6f72 735f 6469 6374 2e6b 6579  slators_dict.key
-000407f0: 7328 2929 0d0a 2020 2020 2020 2020 7365  s())..        se
-00040800: 6c66 2e6e 6f74 5f65 6e5f 6c61 6e67 7320  lf.not_en_langs 
-00040810: 3d20 7b27 7574 6962 6574 273a 2027 7469  = {'utibet': 'ti
-00040820: 272c 2027 6d67 6c69 7027 3a20 276d 6f6e  ', 'mglip': 'mon
-00040830: 277d 0d0a 2020 2020 2020 2020 7365 6c66  '}..        self
-00040840: 2e6e 6f74 5f7a 685f 6c61 6e67 7320 3d20  .not_zh_langs = 
-00040850: 7b27 6c61 6e67 7561 6765 5769 7265 273a  {'languageWire':
-00040860: 2027 6672 272c 2027 7469 6c64 6527 3a20   'fr', 'tilde': 
-00040870: 2766 7227 2c20 2765 6c69 6127 3a20 2766  'fr', 'elia': 'f
-00040880: 7227 2c20 2761 7065 7274 6975 6d27 3a20  r', 'apertium': 
-00040890: 2773 7061 277d 0d0a 2020 2020 2020 2020  'spa'}..        
-000408a0: 7365 6c66 2e70 7265 5f61 6363 656c 6572  self.pre_acceler
-000408b0: 6174 696f 6e5f 6c61 6265 6c20 3d20 300d  ation_label = 0.
-000408c0: 0a20 2020 2020 2020 2073 656c 662e 6578  .        self.ex
-000408d0: 616d 706c 655f 7175 6572 795f 7465 7874  ample_query_text
-000408e0: 203d 2027 e4bd a0e5 a5bd e380 825c 6ee6   = '.........\n.
-000408f0: aca2 e8bf 8ee4 bda0 efbc 8127 0d0a 2020  ...........'..  
-00040900: 2020 2020 2020 7365 6c66 2e73 7563 6365        self.succe
-00040910: 7373 5f74 7261 6e73 6c61 746f 7273 5f70  ss_translators_p
-00040920: 6f6f 6c20 3d20 5b5d 0d0a 2020 2020 2020  ool = []..      
-00040930: 2020 7365 6c66 2e66 6169 6c75 7265 5f74    self.failure_t
-00040940: 7261 6e73 6c61 746f 7273 5f70 6f6f 6c20  ranslators_pool 
-00040950: 3d20 5b5d 0d0a 0d0a 2020 2020 6465 6620  = []....    def 
-00040960: 7472 616e 736c 6174 655f 7465 7874 2873  translate_text(s
-00040970: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
-00040980: 2020 2020 2020 2020 2020 2020 2071 7565               que
-00040990: 7279 5f74 6578 743a 2073 7472 2c0d 0a20  ry_text: str,.. 
-000409a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000409b0: 2020 2020 2020 7472 616e 736c 6174 6f72        translator
-000409c0: 3a20 7374 7220 3d20 2762 696e 6727 2c0d  : str = 'bing',.
-000409d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000409e0: 2020 2020 2020 2020 6672 6f6d 5f6c 616e          from_lan
-000409f0: 6775 6167 653a 2073 7472 203d 2027 6175  guage: str = 'au
-00040a00: 746f 272c 0d0a 2020 2020 2020 2020 2020  to',..          
-00040a10: 2020 2020 2020 2020 2020 2020 2074 6f5f               to_
-00040a20: 6c61 6e67 7561 6765 3a20 7374 7220 3d20  language: str = 
-00040a30: 2765 6e27 2c0d 0a20 2020 2020 2020 2020  'en',..         
-00040a40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00040a50: 5f75 7365 5f70 7265 6163 6365 6c65 7261  _use_preaccelera
-00040a60: 7469 6f6e 3a20 626f 6f6c 203d 2046 616c  tion: bool = Fal
-00040a70: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-00040a80: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
-00040a90: 6172 6773 3a20 4170 694b 7761 7267 7354  args: ApiKwargsT
-00040aa0: 7970 652c 0d0a 2020 2020 2020 2020 2020  ype,..          
-00040ab0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-00040ac0: 3e20 556e 696f 6e5b 7374 722c 2064 6963  > Union[str, dic
-00040ad0: 745d 3a0d 0a20 2020 2020 2020 2022 2222  t]:..        """
-00040ae0: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00040af0: 2071 7565 7279 5f74 6578 743a 2073 7472   query_text: str
-00040b00: 2c20 6d75 7374 2e0d 0a20 2020 2020 2020  , must...       
-00040b10: 203a 7061 7261 6d20 7472 616e 736c 6174   :param translat
-00040b20: 6f72 3a20 7374 722c 2064 6566 6175 6c74  or: str, default
-00040b30: 2027 6269 6e67 272e 0d0a 2020 2020 2020   'bing'...      
-00040b40: 2020 3a70 6172 616d 2066 726f 6d5f 6c61    :param from_la
-00040b50: 6e67 7561 6765 3a20 7374 722c 2064 6566  nguage: str, def
-00040b60: 6175 6c74 2027 6175 746f 272e 0d0a 2020  ault 'auto'...  
-00040b70: 2020 2020 2020 3a70 6172 616d 2074 6f5f        :param to_
-00040b80: 6c61 6e67 7561 6765 3a20 7374 722c 2064  language: str, d
-00040b90: 6566 6175 6c74 2027 656e 272e 0d0a 2020  efault 'en'...  
-00040ba0: 2020 2020 2020 3a70 6172 616d 2069 665f        :param if_
-00040bb0: 7573 655f 7072 6561 6363 656c 6572 6174  use_preaccelerat
-00040bc0: 696f 6e3a 2062 6f6f 6c2c 2064 6566 6175  ion: bool, defau
-00040bd0: 6c74 2046 616c 7365 2e0d 0a20 2020 2020  lt False...     
-00040be0: 2020 203a 7061 7261 6d20 2a2a 6b77 6172     :param **kwar
-00040bf0: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
-00040c00: 2020 2020 203a 7061 7261 6d20 6973 5f64       :param is_d
-00040c10: 6574 6169 6c5f 7265 7375 6c74 3a20 626f  etail_result: bo
-00040c20: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-00040c30: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
-00040c40: 2020 2020 3a70 6172 616d 2070 726f 6665      :param profe
-00040c50: 7373 696f 6e61 6c5f 6669 656c 643a 2073  ssional_field: s
-00040c60: 7472 2c20 7375 7070 6f72 7420 616c 6962  tr, support alib
-00040c70: 6162 6128 292c 2062 6169 6475 2829 2c20  aba(), baidu(), 
-00040c80: 6361 6979 756e 2829 2c20 636c 6f75 6459  caiyun(), cloudY
-00040c90: 6928 292c 2065 6c69 6128 292c 2073 7973  i(), elia(), sys
-00040ca0: 5472 616e 2829 2c20 796f 7564 616f 2829  Tran(), youdao()
-00040cb0: 2c20 766f 6c63 456e 6769 6e65 2829 206f  , volcEngine() o
-00040cc0: 6e6c 792e 0d0a 2020 2020 2020 2020 2020  nly...          
-00040cd0: 2020 2020 2020 3a70 6172 616d 2074 696d        :param tim
-00040ce0: 656f 7574 3a20 666c 6f61 742c 2064 6566  eout: float, def
-00040cf0: 6175 6c74 204e 6f6e 652e 0d0a 2020 2020  ault None...    
-00040d00: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-00040d10: 616d 2070 726f 7869 6573 3a20 6469 6374  am proxies: dict
-00040d20: 2c20 6465 6661 756c 7420 4e6f 6e65 2e0d  , default None..
-00040d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00040d40: 203a 7061 7261 6d20 736c 6565 705f 7365   :param sleep_se
-00040d50: 636f 6e64 733a 2066 6c6f 6174 2c20 6465  conds: float, de
-00040d60: 6661 756c 7420 302e 0d0a 2020 2020 2020  fault 0...      
-00040d70: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00040d80: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
-00040d90: 6166 7465 725f 6672 6571 3a20 696e 742c  after_freq: int,
-00040da0: 2064 6566 6175 6c74 2031 3030 302e 0d0a   default 1000...
-00040db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00040dc0: 3a70 6172 616d 2075 7064 6174 655f 7365  :param update_se
-00040dd0: 7373 696f 6e5f 6166 7465 725f 7365 636f  ssion_after_seco
-00040de0: 6e64 733a 2066 6c6f 6174 2c20 6465 6661  nds: float, defa
-00040df0: 756c 7420 3135 3030 2e0d 0a20 2020 2020  ult 1500...     
-00040e00: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00040e10: 6d20 6966 5f75 7365 5f63 6e5f 686f 7374  m if_use_cn_host
-00040e20: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00040e30: 4661 6c73 652e 2053 7570 706f 7274 2067  False. Support g
-00040e40: 6f6f 676c 6528 292c 2062 696e 6728 2920  oogle(), bing() 
-00040e50: 6f6e 6c79 2e0d 0a20 2020 2020 2020 2020  only...         
-00040e60: 2020 2020 2020 203a 7061 7261 6d20 7265         :param re
-00040e70: 7365 745f 686f 7374 5f75 726c 3a20 7374  set_host_url: st
-00040e80: 722c 2064 6566 6175 6c74 204e 6f6e 652e  r, default None.
-00040e90: 2053 7570 706f 7274 2067 6f6f 676c 6528   Support google(
-00040ea0: 292c 2061 7267 6f73 2829 2c20 7961 6e64  ), argos(), yand
-00040eb0: 6578 2829 206f 6e6c 792e 0d0a 2020 2020  ex() only...    
-00040ec0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-00040ed0: 616d 2069 665f 6368 6563 6b5f 7265 7365  am if_check_rese
-00040ee0: 745f 686f 7374 5f75 726c 3a20 626f 6f6c  t_host_url: bool
-00040ef0: 2c20 6465 6661 756c 7420 5472 7565 2e20  , default True. 
-00040f00: 5375 7070 6f72 7420 676f 6f67 6c65 2829  Support google()
-00040f10: 2c20 7961 6e64 6578 2829 206f 6e6c 792e  , yandex() only.
-00040f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00040f30: 2020 3a70 6172 616d 2069 665f 6967 6e6f    :param if_igno
-00040f40: 7265 5f65 6d70 7479 5f71 7565 7279 3a20  re_empty_query: 
-00040f50: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-00040f60: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
-00040f70: 2020 2020 2020 3a70 6172 616d 2069 665f        :param if_
-00040f80: 6967 6e6f 7265 5f6c 696d 6974 5f6f 665f  ignore_limit_of_
-00040f90: 6c65 6e67 7468 3a20 626f 6f6c 2c20 6465  length: bool, de
-00040fa0: 6661 756c 7420 4661 6c73 652e 0d0a 2020  fault False...  
-00040fb0: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-00040fc0: 6172 616d 206c 696d 6974 5f6f 665f 6c65  aram limit_of_le
-00040fd0: 6e67 7468 3a20 696e 742c 2064 6566 6175  ngth: int, defau
-00040fe0: 6c74 2032 3030 3030 2e0d 0a20 2020 2020  lt 20000...     
-00040ff0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00041000: 6d20 6966 5f73 686f 775f 7469 6d65 5f73  m if_show_time_s
-00041010: 7461 743a 2062 6f6f 6c2c 2064 6566 6175  tat: bool, defau
-00041020: 6c74 2046 616c 7365 2e0d 0a20 2020 2020  lt False...     
-00041030: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00041040: 6d20 7368 6f77 5f74 696d 655f 7374 6174  m show_time_stat
-00041050: 5f70 7265 6369 7369 6f6e 3a20 696e 742c  _precision: int,
-00041060: 2064 6566 6175 6c74 2032 2e0d 0a20 2020   default 2...   
-00041070: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-00041080: 7261 6d20 6966 5f70 7269 6e74 5f77 6172  ram if_print_war
-00041090: 6e69 6e67 3a20 626f 6f6c 2c20 6465 6661  ning: bool, defa
-000410a0: 756c 7420 5472 7565 2e0d 0a20 2020 2020  ult True...     
-000410b0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-000410c0: 6d20 6c69 6e67 7661 6e65 785f 6d6f 6465  m lingvanex_mode
-000410d0: 6c3a 2073 7472 2c20 6465 6661 756c 7420  l: str, default 
-000410e0: 2742 3243 272c 2063 686f 6f73 6520 6672  'B2C', choose fr
-000410f0: 6f6d 2028 2242 3243 222c 2022 4232 4222  om ("B2C", "B2B"
-00041100: 292e 0d0a 2020 2020 2020 2020 2020 2020  )...            
-00041110: 2020 2020 3a70 6172 616d 206d 794d 656d      :param myMem
-00041120: 6f72 795f 6d6f 6465 3a20 7374 722c 2064  ory_mode: str, d
-00041130: 6566 6175 6c74 2022 7765 6222 2c20 6368  efault "web", ch
-00041140: 6f6f 7365 2066 726f 6d20 2822 7765 6222  oose from ("web"
-00041150: 2c20 2261 7069 2229 2e0d 0a20 2020 2020  , "api")...     
-00041160: 2020 203a 7265 7475 726e 3a20 7374 7220     :return: str 
-00041170: 6f72 2064 6963 740d 0a20 2020 2020 2020  or dict..       
-00041180: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-00041190: 6966 2074 7261 6e73 6c61 746f 7220 6e6f  if translator no
-000411a0: 7420 696e 2073 656c 662e 7472 616e 736c  t in self.transl
-000411b0: 6174 6f72 735f 706f 6f6c 3a0d 0a20 2020  ators_pool:..   
-000411c0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-000411d0: 7261 6e73 6c61 746f 7245 7272 6f72 0d0a  ranslatorError..
-000411e0: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-000411f0: 2073 656c 662e 7072 655f 6163 6365 6c65   self.pre_accele
-00041200: 7261 7469 6f6e 5f6c 6162 656c 2061 6e64  ration_label and
-00041210: 2069 665f 7573 655f 7072 6561 6363 656c   if_use_preaccel
-00041220: 6572 6174 696f 6e3a 0d0a 2020 2020 2020  eration:..      
-00041230: 2020 2020 2020 5f20 3d20 7365 6c66 2e70        _ = self.p
-00041240: 7265 6163 6365 6c65 7261 7465 2829 0d0a  reaccelerate()..
-00041250: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00041260: 2073 656c 662e 7472 616e 736c 6174 6f72   self.translator
-00041270: 735f 6469 6374 5b74 7261 6e73 6c61 746f  s_dict[translato
-00041280: 725d 2871 7565 7279 5f74 6578 743d 7175  r](query_text=qu
-00041290: 6572 795f 7465 7874 2c20 6672 6f6d 5f6c  ery_text, from_l
-000412a0: 616e 6775 6167 653d 6672 6f6d 5f6c 616e  anguage=from_lan
-000412b0: 6775 6167 652c 2074 6f5f 6c61 6e67 7561  guage, to_langua
-000412c0: 6765 3d74 6f5f 6c61 6e67 7561 6765 2c20  ge=to_language, 
-000412d0: 2a2a 6b77 6172 6773 290d 0a0d 0a20 2020  **kwargs)....   
-000412e0: 2064 6566 2074 7261 6e73 6c61 7465 5f68   def translate_h
-000412f0: 746d 6c28 7365 6c66 2c0d 0a20 2020 2020  tml(self,..     
-00041300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00041310: 2020 6874 6d6c 5f74 6578 743a 2073 7472    html_text: str
-00041320: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00041330: 2020 2020 2020 2020 2020 7472 616e 736c            transl
-00041340: 6174 6f72 3a20 7374 7220 3d20 2762 696e  ator: str = 'bin
-00041350: 6727 2c0d 0a20 2020 2020 2020 2020 2020  g',..           
-00041360: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
-00041370: 5f6c 616e 6775 6167 653a 2073 7472 203d  _language: str =
-00041380: 2027 6175 746f 272c 0d0a 2020 2020 2020   'auto',..      
-00041390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000413a0: 2074 6f5f 6c61 6e67 7561 6765 3a20 7374   to_language: st
-000413b0: 7220 3d20 2765 6e27 2c0d 0a20 2020 2020  r = 'en',..     
-000413c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000413d0: 2020 6e5f 6a6f 6273 3a20 696e 7420 3d20    n_jobs: int = 
-000413e0: 2d31 2c0d 0a20 2020 2020 2020 2020 2020  -1,..           
-000413f0: 2020 2020 2020 2020 2020 2020 6966 5f75              if_u
-00041400: 7365 5f70 7265 6163 6365 6c65 7261 7469  se_preaccelerati
-00041410: 6f6e 3a20 626f 6f6c 203d 2046 616c 7365  on: bool = False
-00041420: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00041430: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-00041440: 6773 3a20 4170 694b 7761 7267 7354 7970  gs: ApiKwargsTyp
-00041450: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00041460: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-00041470: 7374 723a 0d0a 2020 2020 2020 2020 2222  str:..        ""
-00041480: 220d 0a20 2020 2020 2020 2054 7261 6e73  "..        Trans
-00041490: 6c61 7465 2074 6865 2064 6973 706c 6179  late the display
-000414a0: 6564 2063 6f6e 7465 6e74 206f 6620 6874  ed content of ht
-000414b0: 6d6c 2077 6974 686f 7574 2063 6861 6e67  ml without chang
-000414c0: 696e 6720 7468 6520 6874 6d6c 2073 7472  ing the html str
-000414d0: 7563 7475 7265 2e0d 0a20 2020 2020 2020  ucture...       
-000414e0: 203a 7061 7261 6d20 6874 6d6c 5f74 6578   :param html_tex
-000414f0: 743a 2073 7472 2c20 6d75 7374 2e0d 0a20  t: str, must... 
-00041500: 2020 2020 2020 203a 7061 7261 6d20 7472         :param tr
-00041510: 616e 736c 6174 6f72 3a20 7374 722c 2064  anslator: str, d
-00041520: 6566 6175 6c74 2027 6269 6e67 272e 0d0a  efault 'bing'...
-00041530: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-00041540: 726f 6d5f 6c61 6e67 7561 6765 3a20 7374  rom_language: st
-00041550: 722c 2064 6566 6175 6c74 2027 6175 746f  r, default 'auto
-00041560: 272e 0d0a 2020 2020 2020 2020 3a70 6172  '...        :par
-00041570: 616d 2074 6f5f 6c61 6e67 7561 6765 3a20  am to_language: 
-00041580: 7374 722c 2064 6566 6175 6c74 2027 656e  str, default 'en
-00041590: 272e 0d0a 2020 2020 2020 2020 3a70 6172  '...        :par
-000415a0: 616d 206e 5f6a 6f62 733a 2069 6e74 2c20  am n_jobs: int, 
-000415b0: 6465 6661 756c 7420 2d31 2c20 6d65 616e  default -1, mean
-000415c0: 7320 6f73 2e63 7075 5f63 6e74 2829 2e0d  s os.cpu_cnt()..
-000415d0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000415e0: 6966 5f75 7365 5f70 7265 6163 6365 6c65  if_use_preaccele
-000415f0: 7261 7469 6f6e 3a20 626f 6f6c 2c20 6465  ration: bool, de
-00041600: 6661 756c 7420 4661 6c73 652e 0d0a 2020  fault False...  
-00041610: 2020 2020 2020 3a70 6172 616d 202a 2a6b        :param **k
-00041620: 7761 7267 733a 0d0a 2020 2020 2020 2020  wargs:..        
-00041630: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-00041640: 735f 6465 7461 696c 5f72 6573 756c 743a  s_detail_result:
-00041650: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
-00041660: 616c 7365 2e0d 0a20 2020 2020 2020 2020  alse...         
-00041670: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
-00041680: 6f66 6573 7369 6f6e 616c 5f66 6965 6c64  ofessional_field
-00041690: 3a20 7374 722c 2073 7570 706f 7274 2061  : str, support a
-000416a0: 6c69 6261 6261 2829 2c20 6261 6964 7528  libaba(), baidu(
-000416b0: 292c 2063 6169 7975 6e28 292c 2063 6c6f  ), caiyun(), clo
-000416c0: 7564 5969 2829 2c20 656c 6961 2829 2c20  udYi(), elia(), 
-000416d0: 7379 7354 7261 6e28 292c 2079 6f75 6461  sysTran(), youda
-000416e0: 6f28 292c 2076 6f6c 6345 6e67 696e 6528  o(), volcEngine(
-000416f0: 2920 6f6e 6c79 2e0d 0a20 2020 2020 2020  ) only...       
-00041700: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00041710: 7469 6d65 6f75 743a 2066 6c6f 6174 2c20  timeout: float, 
-00041720: 6465 6661 756c 7420 4e6f 6e65 2e0d 0a20  default None... 
-00041730: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-00041740: 7061 7261 6d20 7072 6f78 6965 733a 2064  param proxies: d
-00041750: 6963 742c 2064 6566 6175 6c74 204e 6f6e  ict, default Non
-00041760: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
-00041770: 2020 2020 3a70 6172 616d 2073 6c65 6570      :param sleep
-00041780: 5f73 6563 6f6e 6473 3a20 666c 6f61 742c  _seconds: float,
-00041790: 2064 6566 6175 6c74 2030 2e0d 0a20 2020   default 0...   
-000417a0: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-000417b0: 7261 6d20 7570 6461 7465 5f73 6573 7369  ram update_sessi
-000417c0: 6f6e 5f61 6674 6572 5f66 7265 713a 2069  on_after_freq: i
-000417d0: 6e74 2c20 6465 6661 756c 7420 3130 3030  nt, default 1000
-000417e0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000417f0: 2020 203a 7061 7261 6d20 7570 6461 7465     :param update
-00041800: 5f73 6573 7369 6f6e 5f61 6674 6572 5f73  _session_after_s
-00041810: 6563 6f6e 6473 3a20 666c 6f61 742c 2064  econds: float, d
-00041820: 6566 6175 6c74 2031 3530 302e 0d0a 2020  efault 1500...  
-00041830: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-00041840: 6172 616d 2069 665f 7573 655f 636e 5f68  aram if_use_cn_h
-00041850: 6f73 743a 2062 6f6f 6c2c 2064 6566 6175  ost: bool, defau
-00041860: 6c74 2046 616c 7365 2e20 5375 7070 6f72  lt False. Suppor
-00041870: 7420 676f 6f67 6c65 2829 2c20 6269 6e67  t google(), bing
-00041880: 2829 206f 6e6c 792e 0d0a 2020 2020 2020  () only...      
-00041890: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-000418a0: 2072 6573 6574 5f68 6f73 745f 7572 6c3a   reset_host_url:
-000418b0: 2073 7472 2c20 6465 6661 756c 7420 4e6f   str, default No
-000418c0: 6e65 2e20 5375 7070 6f72 7420 676f 6f67  ne. Support goog
-000418d0: 6c65 2829 2c20 6172 676f 7328 292c 2079  le(), argos(), y
-000418e0: 616e 6465 7828 2920 6f6e 6c79 2e0d 0a20  andex() only... 
-000418f0: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-00041900: 7061 7261 6d20 6966 5f63 6865 636b 5f72  param if_check_r
-00041910: 6573 6574 5f68 6f73 745f 7572 6c3a 2062  eset_host_url: b
-00041920: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
-00041930: 652e 2053 7570 706f 7274 2067 6f6f 676c  e. Support googl
-00041940: 6528 292c 2079 616e 6465 7828 2920 6f6e  e(), yandex() on
-00041950: 6c79 2e0d 0a20 2020 2020 2020 2020 2020  ly...           
-00041960: 2020 2020 203a 7061 7261 6d20 6966 5f69       :param if_i
-00041970: 676e 6f72 655f 656d 7074 795f 7175 6572  gnore_empty_quer
-00041980: 793a 2062 6f6f 6c2c 2064 6566 6175 6c74  y: bool, default
-00041990: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
-000419a0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-000419b0: 6966 5f69 676e 6f72 655f 6c69 6d69 745f  if_ignore_limit_
-000419c0: 6f66 5f6c 656e 6774 683a 2062 6f6f 6c2c  of_length: bool,
-000419d0: 2064 6566 6175 6c74 2046 616c 7365 2e0d   default False..
-000419e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000419f0: 203a 7061 7261 6d20 6c69 6d69 745f 6f66   :param limit_of
-00041a00: 5f6c 656e 6774 683a 2069 6e74 2c20 6465  _length: int, de
-00041a10: 6661 756c 7420 3230 3030 302e 0d0a 2020  fault 20000...  
-00041a20: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-00041a30: 6172 616d 2069 665f 7368 6f77 5f74 696d  aram if_show_tim
-00041a40: 655f 7374 6174 3a20 626f 6f6c 2c20 6465  e_stat: bool, de
-00041a50: 6661 756c 7420 4661 6c73 652e 0d0a 2020  fault False...  
-00041a60: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-00041a70: 6172 616d 2073 686f 775f 7469 6d65 5f73  aram show_time_s
-00041a80: 7461 745f 7072 6563 6973 696f 6e3a 2069  tat_precision: i
-00041a90: 6e74 2c20 6465 6661 756c 7420 322e 0d0a  nt, default 2...
-00041aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00041ab0: 3a70 6172 616d 2069 665f 7072 696e 745f  :param if_print_
-00041ac0: 7761 726e 696e 673a 2062 6f6f 6c2c 2064  warning: bool, d
-00041ad0: 6566 6175 6c74 2054 7275 652e 0d0a 2020  efault True...  
-00041ae0: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-00041af0: 6172 616d 206c 696e 6776 616e 6578 5f6d  aram lingvanex_m
-00041b00: 6f64 656c 3a20 7374 722c 2064 6566 6175  odel: str, defau
-00041b10: 6c74 2027 4232 4327 2c20 6368 6f6f 7365  lt 'B2C', choose
-00041b20: 2066 726f 6d20 2822 4232 4322 2c20 2242   from ("B2C", "B
-00041b30: 3242 2229 2e0d 0a20 2020 2020 2020 2020  2B")...         
-00041b40: 2020 2020 2020 203a 7061 7261 6d20 6d79         :param my
-00041b50: 4d65 6d6f 7279 5f6d 6f64 653a 2073 7472  Memory_mode: str
-00041b60: 2c20 6465 6661 756c 7420 2277 6562 222c  , default "web",
-00041b70: 2063 686f 6f73 6520 6672 6f6d 2028 2277   choose from ("w
-00041b80: 6562 222c 2022 6170 6922 292e 0d0a 2020  eb", "api")...  
-00041b90: 2020 2020 2020 3a72 6574 7572 6e3a 2073        :return: s
-00041ba0: 7472 0d0a 2020 2020 2020 2020 2222 220d  tr..        """.
-00041bb0: 0a0d 0a20 2020 2020 2020 2069 6620 7472  ...        if tr
-00041bc0: 616e 736c 6174 6f72 206e 6f74 2069 6e20  anslator not in 
-00041bd0: 7365 6c66 2e74 7261 6e73 6c61 746f 7273  self.translators
-00041be0: 5f70 6f6f 6c20 6f72 206b 7761 7267 732e  _pool or kwargs.
-00041bf0: 6765 7428 2769 735f 6465 7461 696c 5f72  get('is_detail_r
-00041c00: 6573 756c 7427 2c20 4661 6c73 6529 206f  esult', False) o
-00041c10: 7220 6e5f 6a6f 6273 203e 2073 656c 662e  r n_jobs > self.
-00041c20: 6370 755f 636e 743a 0d0a 2020 2020 2020  cpu_cnt:..      
-00041c30: 2020 2020 2020 7261 6973 6520 5472 616e        raise Tran
-00041c40: 736c 6174 6f72 4572 726f 720d 0a0d 0a20  slatorError.... 
-00041c50: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00041c60: 6c66 2e70 7265 5f61 6363 656c 6572 6174  lf.pre_accelerat
-00041c70: 696f 6e5f 6c61 6265 6c20 616e 6420 6966  ion_label and if
-00041c80: 5f75 7365 5f70 7265 6163 6365 6c65 7261  _use_preaccelera
-00041c90: 7469 6f6e 3a0d 0a20 2020 2020 2020 2020  tion:..         
-00041ca0: 2020 205f 203d 2073 656c 662e 7072 6561     _ = self.prea
-00041cb0: 6363 656c 6572 6174 6528 290d 0a0d 0a20  ccelerate().... 
-00041cc0: 2020 2020 2020 2064 6566 205f 7472 616e         def _tran
-00041cd0: 736c 6174 655f 7465 7874 2873 656e 7465  slate_text(sente
-00041ce0: 6e63 653a 2073 7472 2920 2d3e 2054 7570  nce: str) -> Tup
-00041cf0: 6c65 5b73 7472 2c20 7374 725d 3a0d 0a20  le[str, str]:.. 
-00041d00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00041d10: 6e20 7365 6e74 656e 6365 2c20 7365 6c66  n sentence, self
-00041d20: 2e74 7261 6e73 6c61 746f 7273 5f64 6963  .translators_dic
-00041d30: 745b 7472 616e 736c 6174 6f72 5d28 7175  t[translator](qu
-00041d40: 6572 795f 7465 7874 3d73 656e 7465 6e63  ery_text=sentenc
-00041d50: 652c 2066 726f 6d5f 6c61 6e67 7561 6765  e, from_language
-00041d60: 3d66 726f 6d5f 6c61 6e67 7561 6765 2c20  =from_language, 
-00041d70: 746f 5f6c 616e 6775 6167 653d 746f 5f6c  to_language=to_l
-00041d80: 616e 6775 6167 652c 202a 2a6b 7761 7267  anguage, **kwarg
-00041d90: 7329 0d0a 0d0a 2020 2020 2020 2020 7061  s)....        pa
-00041da0: 7474 6572 6e20 3d20 7265 2e63 6f6d 7069  ttern = re.compi
-00041db0: 6c65 2822 283f 3a5e 7c28 3f3c 3d3e 2929  le("(?:^|(?<=>))
-00041dc0: 285b 5c5c 735c 5c53 5d2a 3f29 283f 3a28  ([\\s\\S]*?)(?:(
-00041dd0: 3f3d 3c29 7c24 2922 2920 2023 2054 4f44  ?=<)|$)")  # TOD
-00041de0: 4f3a 203c 636f 6465 3e3c 2f63 6f64 653e  O: <code></code>
-00041df0: 203c 6469 7620 636c 6173 733d 2263 6f64   <div class="cod
-00041e00: 6574 6578 7420 6e6f 7472 616e 736c 6174  etext notranslat
-00041e10: 6522 3e0d 0a20 2020 2020 2020 2073 656e  e">..        sen
-00041e20: 7465 6e63 655f 6c69 7374 203d 206c 6973  tence_list = lis
-00041e30: 7428 7365 7428 7061 7474 6572 6e2e 6669  t(set(pattern.fi
-00041e40: 6e64 616c 6c28 6874 6d6c 5f74 6578 7429  ndall(html_text)
-00041e50: 2929 0d0a 0d0a 2020 2020 2020 2020 6e5f  ))....        n_
-00041e60: 6a6f 6273 203d 2073 656c 662e 6370 755f  jobs = self.cpu_
-00041e70: 636e 7420 6966 206e 5f6a 6f62 7320 3c3d  cnt if n_jobs <=
-00041e80: 2030 2065 6c73 6520 6e5f 6a6f 6273 0d0a   0 else n_jobs..
-00041e90: 2020 2020 2020 2020 7769 7468 2070 6174          with pat
-00041ea0: 686f 732e 6d75 6c74 6970 726f 6365 7373  hos.multiprocess
-00041eb0: 696e 672e 5072 6f63 6573 7350 6f6f 6c28  ing.ProcessPool(
-00041ec0: 6e5f 6a6f 6273 2920 6173 2070 6f6f 6c3a  n_jobs) as pool:
-00041ed0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00041ee0: 7375 6c74 5f6c 6973 7420 3d20 706f 6f6c  sult_list = pool
-00041ef0: 2e6d 6170 285f 7472 616e 736c 6174 655f  .map(_translate_
-00041f00: 7465 7874 2c20 7365 6e74 656e 6365 5f6c  text, sentence_l
-00041f10: 6973 7429 0d0a 0d0a 2020 2020 2020 2020  ist)....        
-00041f20: 7265 7375 6c74 5f64 6963 7420 3d20 7b74  result_dict = {t
-00041f30: 6578 743a 2074 735f 7465 7874 2066 6f72  ext: ts_text for
-00041f40: 2074 6578 742c 2074 735f 7465 7874 2069   text, ts_text i
-00041f50: 6e20 7265 7375 6c74 5f6c 6973 747d 0d0a  n result_list}..
-00041f60: 2020 2020 2020 2020 5f67 6574 5f72 6573          _get_res
-00041f70: 756c 745f 6675 6e63 203d 206c 616d 6264  ult_func = lambd
-00041f80: 6120 6b3a 2072 6573 756c 745f 6469 6374  a k: result_dict
-00041f90: 2e67 6574 286b 2e67 726f 7570 2831 292c  .get(k.group(1),
-00041fa0: 2027 2729 0d0a 2020 2020 2020 2020 7265   '')..        re
-00041fb0: 7475 726e 2070 6174 7465 726e 2e73 7562  turn pattern.sub
-00041fc0: 2872 6570 6c3d 5f67 6574 5f72 6573 756c  (repl=_get_resul
-00041fd0: 745f 6675 6e63 2c20 7374 7269 6e67 3d68  t_func, string=h
-00041fe0: 746d 6c5f 7465 7874 290d 0a0d 0a20 2020  tml_text)....   
-00041ff0: 2064 6566 205f 7465 7374 5f74 7261 6e73   def _test_trans
-00042000: 6c61 7465 2873 656c 662c 205f 7473 3a20  late(self, _ts: 
-00042010: 7374 722c 2074 696d 656f 7574 3a20 4f70  str, timeout: Op
-00042020: 7469 6f6e 616c 5b66 6c6f 6174 5d20 3d20  tional[float] = 
-00042030: 4e6f 6e65 2c20 6966 5f73 686f 775f 7469  None, if_show_ti
-00042040: 6d65 5f73 7461 743a 2062 6f6f 6c20 3d20  me_stat: bool = 
-00042050: 4661 6c73 6529 202d 3e20 7374 723a 0d0a  False) -> str:..
-00042060: 2020 2020 2020 2020 6672 6f6d 5f6c 616e          from_lan
-00042070: 6775 6167 6520 3d20 7365 6c66 2e6e 6f74  guage = self.not
-00042080: 5f7a 685f 6c61 6e67 735b 5f74 735d 2069  _zh_langs[_ts] i
-00042090: 6620 5f74 7320 696e 2073 656c 662e 6e6f  f _ts in self.no
-000420a0: 745f 7a68 5f6c 616e 6773 2065 6c73 6520  t_zh_langs else 
-000420b0: 2761 7574 6f27 0d0a 2020 2020 2020 2020  'auto'..        
-000420c0: 746f 5f6c 616e 6775 6167 6520 3d20 7365  to_language = se
-000420d0: 6c66 2e6e 6f74 5f65 6e5f 6c61 6e67 735b  lf.not_en_langs[
-000420e0: 5f74 735d 2069 6620 5f74 7320 696e 2073  _ts] if _ts in s
-000420f0: 656c 662e 6e6f 745f 656e 5f6c 616e 6773  elf.not_en_langs
-00042100: 2065 6c73 6520 2765 6e27 0d0a 2020 2020   else 'en'..    
-00042110: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-00042120: 662e 7472 616e 736c 6174 6f72 735f 6469  f.translators_di
-00042130: 6374 5b5f 7473 5d28 0d0a 2020 2020 2020  ct[_ts](..      
-00042140: 2020 2020 2020 7175 6572 795f 7465 7874        query_text
-00042150: 3d73 656c 662e 6578 616d 706c 655f 7175  =self.example_qu
-00042160: 6572 795f 7465 7874 2c0d 0a20 2020 2020  ery_text,..     
-00042170: 2020 2020 2020 2074 7261 6e73 6c61 746f         translato
-00042180: 723d 5f74 732c 0d0a 2020 2020 2020 2020  r=_ts,..        
-00042190: 2020 2020 6672 6f6d 5f6c 616e 6775 6167      from_languag
-000421a0: 653d 6672 6f6d 5f6c 616e 6775 6167 652c  e=from_language,
-000421b0: 0d0a 2020 2020 2020 2020 2020 2020 746f  ..            to
-000421c0: 5f6c 616e 6775 6167 653d 746f 5f6c 616e  _language=to_lan
-000421d0: 6775 6167 652c 0d0a 2020 2020 2020 2020  guage,..        
-000421e0: 2020 2020 6966 5f70 7269 6e74 5f77 6172      if_print_war
-000421f0: 6e69 6e67 3d46 616c 7365 2c0d 0a20 2020  ning=False,..   
-00042200: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-00042210: 3d74 696d 656f 7574 2c0d 0a20 2020 2020  =timeout,..     
-00042220: 2020 2020 2020 2069 665f 7368 6f77 5f74         if_show_t
-00042230: 696d 655f 7374 6174 3d69 665f 7368 6f77  ime_stat=if_show
-00042240: 5f74 696d 655f 7374 6174 0d0a 2020 2020  _time_stat..    
-00042250: 2020 2020 290d 0a20 2020 2020 2020 2072      )..        r
-00042260: 6574 7572 6e20 7265 7375 6c74 0d0a 0d0a  eturn result....
-00042270: 2020 2020 6465 6620 7072 6561 6363 656c      def preaccel
-00042280: 6572 6174 6528 7365 6c66 2c20 7469 6d65  erate(self, time
-00042290: 6f75 743a 204f 7074 696f 6e61 6c5b 666c  out: Optional[fl
-000422a0: 6f61 745d 203d 204e 6f6e 652c 2069 665f  oat] = None, if_
-000422b0: 7368 6f77 5f74 696d 655f 7374 6174 3a20  show_time_stat: 
-000422c0: 626f 6f6c 203d 2054 7275 652c 202a 2a6b  bool = True, **k
-000422d0: 7761 7267 733a 2073 7472 2920 2d3e 2064  wargs: str) -> d
-000422e0: 6963 743a 0d0a 2020 2020 2020 2020 6966  ict:..        if
-000422f0: 2073 656c 662e 7072 655f 6163 6365 6c65   self.pre_accele
-00042300: 7261 7469 6f6e 5f6c 6162 656c 203e 2030  ration_label > 0
-00042310: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00042320: 6169 7365 2054 7261 6e73 6c61 746f 7245  aise TranslatorE
-00042330: 7272 6f72 2827 5072 6561 6363 656c 6572  rror('Preacceler
-00042340: 6174 696f 6e20 6361 6e20 6f6e 6c79 2062  ation can only b
-00042350: 6520 7065 7266 6f72 6d65 6420 6f6e 6365  e performed once
-00042360: 2e27 290d 0a0d 0a20 2020 2020 2020 2073  .')....        s
-00042370: 656c 662e 6578 616d 706c 655f 7175 6572  elf.example_quer
-00042380: 795f 7465 7874 203d 206b 7761 7267 732e  y_text = kwargs.
-00042390: 6765 7428 2765 7861 6d70 6c65 5f71 7565  get('example_que
-000423a0: 7279 5f74 6578 7427 2c20 7365 6c66 2e65  ry_text', self.e
-000423b0: 7861 6d70 6c65 5f71 7565 7279 5f74 6578  xample_query_tex
-000423c0: 7429 0d0a 0d0a 2020 2020 2020 2020 7379  t)....        sy
-000423d0: 732e 7374 6465 7272 2e77 7269 7465 2827  s.stderr.write('
-000423e0: 5072 6561 6363 656c 6572 6174 696f 6e2d  Preacceleration-
-000423f0: 5072 6f63 6573 7320 7769 6c6c 2074 616b  Process will tak
-00042400: 6520 6120 6665 7720 6d69 6e75 7465 732e  e a few minutes.
-00042410: 5c6e 2729 0d0a 2020 2020 2020 2020 7379  \n')..        sy
-00042420: 732e 7374 6465 7272 2e77 7269 7465 2827  s.stderr.write('
-00042430: 5469 7073 3a20 5468 6520 736d 616c 6c65  Tips: The smalle
-00042440: 7220 6074 696d 656f 7574 6020 7661 6c75  r `timeout` valu
-00042450: 652c 2074 6865 2066 6577 6572 2074 7261  e, the fewer tra
-00042460: 6e73 6c61 746f 7273 2070 6173 7320 7468  nslators pass th
-00042470: 6520 7465 7374 2027 0d0a 2020 2020 2020  e test '..      
-00042480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00042490: 2020 2027 616e 6420 7468 6520 6c65 7373     'and the less
-000424a0: 2074 696d 6520 6974 2074 616b 6573 2074   time it takes t
-000424b0: 6f20 7072 6561 6363 656c 6572 6174 652e  o preaccelerate.
-000424c0: 2048 6f77 6576 6572 2c20 7468 6520 736c   However, the sl
-000424d0: 6f77 2073 7065 6564 206f 6620 270d 0a20  ow speed of '.. 
-000424e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000424f0: 2020 2020 2020 2020 2770 7265 6163 6365          'preacce
-00042500: 6c65 7261 7469 6f6e 2064 6f65 7320 6e6f  leration does no
-00042510: 7420 6d65 616e 2074 6865 2073 6c6f 7720  t mean the slow 
-00042520: 7370 6565 6420 6f66 206c 6174 6572 2074  speed of later t
-00042530: 7261 6e73 6c61 7469 6f6e 2e5c 6e5c 6e27  ranslation.\n\n'
-00042540: 290d 0a0d 0a20 2020 2020 2020 2066 6f72  )....        for
-00042550: 2069 2069 6e20 7471 646d 2e74 7164 6d28   i in tqdm.tqdm(
-00042560: 7261 6e67 6528 6c65 6e28 7365 6c66 2e74  range(len(self.t
-00042570: 7261 6e73 6c61 746f 7273 5f70 6f6f 6c29  ranslators_pool)
-00042580: 292c 2064 6573 633d 2750 7265 6163 6365  ), desc='Preacce
-00042590: 6c65 7261 7469 6f6e 2050 726f 6365 7373  leration Process
-000425a0: 272c 206e 636f 6c73 3d38 3029 3a0d 0a20  ', ncols=80):.. 
-000425b0: 2020 2020 2020 2020 2020 205f 7473 203d             _ts =
-000425c0: 2073 656c 662e 7472 616e 736c 6174 6f72   self.translator
-000425d0: 735f 706f 6f6c 5b69 5d0d 0a20 2020 2020  s_pool[i]..     
-000425e0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-000425f0: 2020 2020 2020 2020 2020 2020 205f 203d               _ =
-00042600: 2073 656c 662e 5f74 6573 745f 7472 616e   self._test_tran
-00042610: 736c 6174 6528 5f74 732c 2074 696d 656f  slate(_ts, timeo
-00042620: 7574 2c20 6966 5f73 686f 775f 7469 6d65  ut, if_show_time
-00042630: 5f73 7461 7429 0d0a 2020 2020 2020 2020  _stat)..        
-00042640: 2020 2020 2020 2020 7365 6c66 2e73 7563          self.suc
-00042650: 6365 7373 5f74 7261 6e73 6c61 746f 7273  cess_translators
-00042660: 5f70 6f6f 6c2e 6170 7065 6e64 285f 7473  _pool.append(_ts
-00042670: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00042680: 7863 6570 743a 0d0a 2020 2020 2020 2020  xcept:..        
-00042690: 2020 2020 2020 2020 7365 6c66 2e66 6169          self.fai
-000426a0: 6c75 7265 5f74 7261 6e73 6c61 746f 7273  lure_translators
-000426b0: 5f70 6f6f 6c2e 6170 7065 6e64 285f 7473  _pool.append(_ts
-000426c0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000426d0: 2073 656c 662e 7072 655f 6163 6365 6c65   self.pre_accele
-000426e0: 7261 7469 6f6e 5f6c 6162 656c 202b 3d20  ration_label += 
-000426f0: 310d 0a20 2020 2020 2020 2072 6574 7572  1..        retur
-00042700: 6e20 7b27 7375 6363 6573 7327 3a20 7365  n {'success': se
-00042710: 6c66 2e73 7563 6365 7373 5f74 7261 6e73  lf.success_trans
-00042720: 6c61 746f 7273 5f70 6f6f 6c2c 2027 6661  lators_pool, 'fa
-00042730: 696c 7572 6527 3a20 7365 6c66 2e66 6169  ilure': self.fai
-00042740: 6c75 7265 5f74 7261 6e73 6c61 746f 7273  lure_translators
-00042750: 5f70 6f6f 6c7d 0d0a 0d0a 2020 2020 6465  _pool}....    de
-00042760: 6620 7370 6565 6474 6573 7428 7365 6c66  f speedtest(self
-00042770: 2c20 2a2a 6b77 6172 6773 3a20 4c69 7374  , **kwargs: List
-00042780: 5b73 7472 5d29 202d 3e20 4e6f 6e65 3a0d  [str]) -> None:.
-00042790: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000427a0: 2e70 7265 5f61 6363 656c 6572 6174 696f  .pre_acceleratio
-000427b0: 6e5f 6c61 6265 6c20 3c20 313a 0d0a 2020  n_label < 1:..  
-000427c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000427d0: 5472 616e 736c 6174 6f72 4572 726f 7228  TranslatorError(
-000427e0: 2750 7265 6163 6365 6c65 7261 7469 6f6e  'Preacceleration
-000427f0: 2066 6972 7374 2e27 290d 0a0d 0a20 2020   first.')....   
-00042800: 2020 2020 2074 6573 745f 7472 616e 736c       test_transl
-00042810: 6174 6f72 735f 706f 6f6c 203d 206b 7761  ators_pool = kwa
-00042820: 7267 732e 6765 7428 2774 6573 745f 7472  rgs.get('test_tr
-00042830: 616e 736c 6174 6f72 735f 706f 6f6c 272c  anslators_pool',
-00042840: 2073 656c 662e 7375 6363 6573 735f 7472   self.success_tr
-00042850: 616e 736c 6174 6f72 735f 706f 6f6c 290d  anslators_pool).
-00042860: 0a0d 0a20 2020 2020 2020 2073 7973 2e73  ...        sys.s
-00042870: 7464 6572 722e 7772 6974 6528 2753 7065  tderr.write('Spe
-00042880: 6564 5465 7374 2d50 726f 6365 7373 2077  edTest-Process w
-00042890: 696c 6c20 7461 6b65 2061 2066 6577 2073  ill take a few s
-000428a0: 6563 6f6e 6473 2e5c 6e5c 6e27 290d 0a20  econds.\n\n').. 
-000428b0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000428c0: 7471 646d 2e74 7164 6d28 7261 6e67 6528  tqdm.tqdm(range(
-000428d0: 6c65 6e28 7465 7374 5f74 7261 6e73 6c61  len(test_transla
-000428e0: 746f 7273 5f70 6f6f 6c29 292c 2064 6573  tors_pool)), des
-000428f0: 633d 2753 7065 6564 5465 7374 2050 726f  c='SpeedTest Pro
-00042900: 6365 7373 272c 206e 636f 6c73 3d38 3029  cess', ncols=80)
-00042910: 3a0d 0a20 2020 2020 2020 2020 2020 205f  :..            _
-00042920: 7473 203d 2074 6573 745f 7472 616e 736c  ts = test_transl
-00042930: 6174 6f72 735f 706f 6f6c 5b69 5d0d 0a20  ators_pool[i].. 
-00042940: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00042950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00042960: 205f 203d 2073 656c 662e 5f74 6573 745f   _ = self._test_
-00042970: 7472 616e 736c 6174 6528 5f74 732c 2074  translate(_ts, t
-00042980: 696d 656f 7574 3d4e 6f6e 652c 2069 665f  imeout=None, if_
-00042990: 7368 6f77 5f74 696d 655f 7374 6174 3d54  show_time_stat=T
-000429a0: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
-000429b0: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
-000429c0: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
-000429d0: 0a20 2020 2020 2020 2072 6574 7572 6e0d  .        return.
-000429e0: 0a0d 0a20 2020 2064 6566 2070 7265 6163  ...    def preac
-000429f0: 6365 6c65 7261 7465 5f61 6e64 5f73 7065  celerate_and_spe
-00042a00: 6564 7465 7374 2873 656c 662c 2074 696d  edtest(self, tim
-00042a10: 656f 7574 3a20 4f70 7469 6f6e 616c 5b66  eout: Optional[f
-00042a20: 6c6f 6174 5d20 3d20 4e6f 6e65 2c20 2a2a  loat] = None, **
-00042a30: 6b77 6172 6773 3a20 7374 7229 202d 3e20  kwargs: str) -> 
-00042a40: 6469 6374 3a0d 0a20 2020 2020 2020 2072  dict:..        r
-00042a50: 6573 756c 7420 3d20 7365 6c66 2e70 7265  esult = self.pre
-00042a60: 6163 6365 6c65 7261 7465 2874 696d 656f  accelerate(timeo
-00042a70: 7574 3d74 696d 656f 7574 2c20 2a2a 6b77  ut=timeout, **kw
-00042a80: 6172 6773 290d 0a20 2020 2020 2020 2073  args)..        s
-00042a90: 7973 2e73 7464 6572 722e 7772 6974 6528  ys.stderr.write(
-00042aa0: 275c 6e5c 6e27 290d 0a20 2020 2020 2020  '\n\n')..       
-00042ab0: 2073 656c 662e 7370 6565 6474 6573 7428   self.speedtest(
-00042ac0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00042ad0: 6e20 7265 7375 6c74 0d0a 0d0a 0d0a 7473  n result......ts
-00042ae0: 7320 3d20 5472 616e 736c 6174 6f72 7353  s = TranslatorsS
-00042af0: 6572 7665 7228 290d 0a0d 0a5f 616c 6962  erver()...._alib
-00042b00: 6162 6120 3d20 7473 732e 5f61 6c69 6261  aba = tss._aliba
-00042b10: 6261 0d0a 616c 6962 6162 6120 3d20 7473  ba..alibaba = ts
-00042b20: 732e 616c 6962 6162 610d 0a5f 6170 6572  s.alibaba.._aper
-00042b30: 7469 756d 203d 2074 7373 2e5f 6170 6572  tium = tss._aper
-00042b40: 7469 756d 0d0a 6170 6572 7469 756d 203d  tium..apertium =
-00042b50: 2074 7373 2e61 7065 7274 6975 6d0d 0a5f   tss.apertium.._
-00042b60: 6172 676f 7320 3d20 7473 732e 5f61 7267  argos = tss._arg
-00042b70: 6f73 0d0a 6172 676f 7320 3d20 7473 732e  os..argos = tss.
-00042b80: 6172 676f 730d 0a5f 6261 6964 7520 3d20  argos.._baidu = 
-00042b90: 7473 732e 5f62 6169 6475 0d0a 6261 6964  tss._baidu..baid
-00042ba0: 7520 3d20 7473 732e 6261 6964 750d 0a5f  u = tss.baidu.._
-00042bb0: 6269 6e67 203d 2074 7373 2e5f 6269 6e67  bing = tss._bing
-00042bc0: 0d0a 6269 6e67 203d 2074 7373 2e62 696e  ..bing = tss.bin
-00042bd0: 670d 0a5f 6361 6979 756e 203d 2074 7373  g.._caiyun = tss
-00042be0: 2e5f 6361 6979 756e 0d0a 6361 6979 756e  ._caiyun..caiyun
-00042bf0: 203d 2074 7373 2e63 6169 7975 6e0d 0a5f   = tss.caiyun.._
-00042c00: 636c 6f75 6459 6920 3d20 7473 732e 5f63  cloudYi = tss._c
-00042c10: 6c6f 7564 5969 0d0a 636c 6f75 6459 6920  loudYi..cloudYi 
-00042c20: 3d20 7473 732e 636c 6f75 6459 690d 0a5f  = tss.cloudYi.._
-00042c30: 6465 6570 6c20 3d20 7473 732e 5f64 6565  deepl = tss._dee
-00042c40: 706c 0d0a 6465 6570 6c20 3d20 7473 732e  pl..deepl = tss.
-00042c50: 6465 6570 6c0d 0a5f 656c 6961 203d 2074  deepl.._elia = t
-00042c60: 7373 2e5f 656c 6961 0d0a 656c 6961 203d  ss._elia..elia =
-00042c70: 2074 7373 2e65 6c69 610d 0a5f 676f 6f67   tss.elia.._goog
-00042c80: 6c65 203d 2074 7373 2e5f 676f 6f67 6c65  le = tss._google
-00042c90: 0d0a 676f 6f67 6c65 203d 2074 7373 2e67  ..google = tss.g
-00042ca0: 6f6f 676c 650d 0a5f 6963 6962 6120 3d20  oogle.._iciba = 
-00042cb0: 7473 732e 5f69 6369 6261 0d0a 6963 6962  tss._iciba..icib
-00042cc0: 6120 3d20 7473 732e 6963 6962 610d 0a5f  a = tss.iciba.._
-00042cd0: 6966 6c79 7465 6b20 3d20 7473 732e 5f69  iflytek = tss._i
-00042ce0: 666c 7974 656b 0d0a 6966 6c79 7465 6b20  flytek..iflytek 
-00042cf0: 3d20 7473 732e 6966 6c79 7465 6b0d 0a5f  = tss.iflytek.._
-00042d00: 6966 6c79 7265 6320 3d20 7473 732e 5f69  iflyrec = tss._i
-00042d10: 666c 7972 6563 0d0a 6966 6c79 7265 6320  flyrec..iflyrec 
-00042d20: 3d20 7473 732e 6966 6c79 7265 630d 0a5f  = tss.iflyrec.._
-00042d30: 6974 7261 6e73 6c61 7465 203d 2074 7373  itranslate = tss
-00042d40: 2e5f 6974 7261 6e73 6c61 7465 0d0a 6974  ._itranslate..it
-00042d50: 7261 6e73 6c61 7465 203d 2074 7373 2e69  ranslate = tss.i
-00042d60: 7472 616e 736c 6174 650d 0a5f 6a75 6469  translate.._judi
-00042d70: 6320 3d20 7473 732e 5f6a 7564 6963 0d0a  c = tss._judic..
-00042d80: 6a75 6469 6320 3d20 7473 732e 6a75 6469  judic = tss.judi
-00042d90: 630d 0a5f 6c61 6e67 7561 6765 5769 7265  c.._languageWire
-00042da0: 203d 2074 7373 2e5f 6c61 6e67 7561 6765   = tss._language
-00042db0: 5769 7265 0d0a 6c61 6e67 7561 6765 5769  Wire..languageWi
-00042dc0: 7265 203d 2074 7373 2e6c 616e 6775 6167  re = tss.languag
-00042dd0: 6557 6972 650d 0a5f 6c69 6e67 7661 6e65  eWire.._lingvane
-00042de0: 7820 3d20 7473 732e 5f6c 696e 6776 616e  x = tss._lingvan
-00042df0: 6578 0d0a 6c69 6e67 7661 6e65 7820 3d20  ex..lingvanex = 
-00042e00: 7473 732e 6c69 6e67 7661 6e65 780d 0a5f  tss.lingvanex.._
-00042e10: 6e69 7574 7261 6e73 203d 2074 7373 2e5f  niutrans = tss._
-00042e20: 6e69 7574 7261 6e73 0d0a 6e69 7574 7261  niutrans..niutra
-00042e30: 6e73 203d 2074 7373 2e6e 6975 7472 616e  ns = tss.niutran
-00042e40: 730d 0a5f 6d67 6c69 7020 3d20 7473 732e  s.._mglip = tss.
-00042e50: 5f6d 676c 6970 0d0a 6d67 6c69 7020 3d20  _mglip..mglip = 
-00042e60: 7473 732e 6d67 6c69 700d 0a5f 6d69 7261  tss.mglip.._mira
-00042e70: 6920 3d20 7473 732e 5f6d 6972 6169 0d0a  i = tss._mirai..
-00042e80: 6d69 7261 6920 3d20 7473 732e 6d69 7261  mirai = tss.mira
-00042e90: 690d 0a5f 6d6f 6465 726e 4d74 203d 2074  i.._modernMt = t
-00042ea0: 7373 2e5f 6d6f 6465 726e 4d74 0d0a 6d6f  ss._modernMt..mo
-00042eb0: 6465 726e 4d74 203d 2074 7373 2e6d 6f64  dernMt = tss.mod
-00042ec0: 6572 6e4d 740d 0a5f 6d79 4d65 6d6f 7279  ernMt.._myMemory
-00042ed0: 203d 2074 7373 2e5f 6d79 4d65 6d6f 7279   = tss._myMemory
-00042ee0: 0d0a 6d79 4d65 6d6f 7279 203d 2074 7373  ..myMemory = tss
-00042ef0: 2e6d 794d 656d 6f72 790d 0a5f 7061 7061  .myMemory.._papa
-00042f00: 676f 203d 2074 7373 2e5f 7061 7061 676f  go = tss._papago
-00042f10: 0d0a 7061 7061 676f 203d 2074 7373 2e70  ..papago = tss.p
-00042f20: 6170 6167 6f0d 0a5f 7171 4661 6e79 6920  apago.._qqFanyi 
-00042f30: 3d20 7473 732e 5f71 7146 616e 7969 0d0a  = tss._qqFanyi..
-00042f40: 7171 4661 6e79 6920 3d20 7473 732e 7171  qqFanyi = tss.qq
-00042f50: 4661 6e79 690d 0a5f 7171 5472 616e 536d  Fanyi.._qqTranSm
-00042f60: 6172 7420 3d20 7473 732e 5f71 7154 7261  art = tss._qqTra
-00042f70: 6e53 6d61 7274 0d0a 7171 5472 616e 536d  nSmart..qqTranSm
-00042f80: 6172 7420 3d20 7473 732e 7171 5472 616e  art = tss.qqTran
-00042f90: 536d 6172 740d 0a5f 7265 7665 7273 6f20  Smart.._reverso 
-00042fa0: 3d20 7473 732e 5f72 6576 6572 736f 0d0a  = tss._reverso..
-00042fb0: 7265 7665 7273 6f20 3d20 7473 732e 7265  reverso = tss.re
-00042fc0: 7665 7273 6f0d 0a5f 736f 676f 7520 3d20  verso.._sogou = 
-00042fd0: 7473 732e 5f73 6f67 6f75 0d0a 736f 676f  tss._sogou..sogo
-00042fe0: 7520 3d20 7473 732e 736f 676f 750d 0a5f  u = tss.sogou.._
-00042ff0: 7379 7354 7261 6e20 3d20 7473 732e 5f73  sysTran = tss._s
-00043000: 7973 5472 616e 0d0a 7379 7354 7261 6e20  ysTran..sysTran 
-00043010: 3d20 7473 732e 7379 7354 7261 6e0d 0a5f  = tss.sysTran.._
-00043020: 7469 6c64 6520 3d20 7473 732e 5f74 696c  tilde = tss._til
-00043030: 6465 0d0a 7469 6c64 6520 3d20 7473 732e  de..tilde = tss.
-00043040: 7469 6c64 650d 0a5f 7472 616e 736c 6174  tilde.._translat
-00043050: 6543 6f6d 203d 2074 7373 2e5f 7472 616e  eCom = tss._tran
-00043060: 736c 6174 6543 6f6d 0d0a 7472 616e 736c  slateCom..transl
-00043070: 6174 6543 6f6d 203d 2074 7373 2e74 7261  ateCom = tss.tra
-00043080: 6e73 6c61 7465 436f 6d0d 0a5f 7472 616e  nslateCom.._tran
-00043090: 736c 6174 654d 6520 3d20 7473 732e 5f74  slateMe = tss._t
-000430a0: 7261 6e73 6c61 7465 4d65 0d0a 7472 616e  ranslateMe..tran
-000430b0: 736c 6174 654d 6520 3d20 7473 732e 7472  slateMe = tss.tr
-000430c0: 616e 736c 6174 654d 650d 0a5f 7574 6962  anslateMe.._utib
-000430d0: 6574 203d 2074 7373 2e5f 7574 6962 6574  et = tss._utibet
-000430e0: 0d0a 7574 6962 6574 203d 2074 7373 2e75  ..utibet = tss.u
-000430f0: 7469 6265 740d 0a5f 766f 6c63 456e 6769  tibet.._volcEngi
-00043100: 6e65 203d 2074 7373 2e5f 766f 6c63 456e  ne = tss._volcEn
-00043110: 6769 6e65 0d0a 766f 6c63 456e 6769 6e65  gine..volcEngine
-00043120: 203d 2074 7373 2e76 6f6c 6345 6e67 696e   = tss.volcEngin
-00043130: 650d 0a5f 7961 6e64 6578 203d 2074 7373  e.._yandex = tss
-00043140: 2e5f 7961 6e64 6578 0d0a 7961 6e64 6578  ._yandex..yandex
-00043150: 203d 2074 7373 2e79 616e 6465 780d 0a5f   = tss.yandex.._
-00043160: 7965 656b 6974 203d 2074 7373 2e5f 7965  yeekit = tss._ye
-00043170: 656b 6974 0d0a 7965 656b 6974 203d 2074  ekit..yeekit = t
-00043180: 7373 2e79 6565 6b69 740d 0a5f 796f 7564  ss.yeekit.._youd
-00043190: 616f 203d 2074 7373 2e5f 796f 7564 616f  ao = tss._youdao
-000431a0: 0d0a 796f 7564 616f 203d 2074 7373 2e79  ..youdao = tss.y
-000431b0: 6f75 6461 6f0d 0a0d 0a74 7261 6e73 6c61  oudao....transla
-000431c0: 7465 5f74 6578 7420 3d20 7473 732e 7472  te_text = tss.tr
-000431d0: 616e 736c 6174 655f 7465 7874 0d0a 7472  anslate_text..tr
-000431e0: 616e 736c 6174 655f 6874 6d6c 203d 2074  anslate_html = t
-000431f0: 7373 2e74 7261 6e73 6c61 7465 5f68 746d  ss.translate_htm
-00043200: 6c0d 0a74 7261 6e73 6c61 746f 7273 5f70  l..translators_p
-00043210: 6f6f 6c20 3d20 7473 732e 7472 616e 736c  ool = tss.transl
-00043220: 6174 6f72 735f 706f 6f6c 0d0a 0d0a 7072  ators_pool....pr
-00043230: 6561 6363 656c 6572 6174 6520 3d20 7473  eaccelerate = ts
-00043240: 732e 7072 6561 6363 656c 6572 6174 650d  s.preaccelerate.
-00043250: 0a73 7065 6564 7465 7374 203d 2074 7373  .speedtest = tss
-00043260: 2e73 7065 6564 7465 7374 0d0a 7072 6561  .speedtest..prea
-00043270: 6363 656c 6572 6174 655f 616e 645f 7370  ccelerate_and_sp
-00043280: 6565 6474 6573 7420 3d20 7473 732e 7072  eedtest = tss.pr
-00043290: 6561 6363 656c 6572 6174 655f 616e 645f  eaccelerate_and_
-000432a0: 7370 6565 6474 6573 740d 0a23 2073 7973  speedtest..# sys
-000432b0: 2e73 7464 6572 722e 7772 6974 6528 6627  .stderr.write(f'
-000432c0: 5375 7070 6f72 7420 7472 616e 736c 6174  Support translat
-000432d0: 6f72 7320 7b74 7261 6e73 6c61 746f 7273  ors {translators
-000432e0: 5f70 6f6f 6c7d 206f 6e6c 792e 5c6e 2729  _pool} only.\n')
-000432f0: 0d0a                                     ..
+0002fda0: 2073 656c 662e 6765 745f 6d61 7465 6361   self.get_mateca
+0002fdb0: 745f 6c61 6e67 7561 6765 5f75 726c 203d  t_language_url =
+0002fdc0: 2027 6874 7470 733a 2f2f 7777 772e 6d61   'https://www.ma
+0002fdd0: 7465 6361 742e 636f 6d2f 6170 692f 7632  tecat.com/api/v2
+0002fde0: 2f6c 616e 6775 6167 6573 270d 0a20 2020  /languages'..   
+0002fdf0: 2020 2020 2073 656c 662e 686f 7374 5f68       self.host_h
+0002fe00: 6561 6465 7273 203d 2073 656c 662e 6765  eaders = self.ge
+0002fe10: 745f 6865 6164 6572 7328 7365 6c66 2e68  t_headers(self.h
+0002fe20: 6f73 745f 7572 6c2c 2069 665f 6170 693d  ost_url, if_api=
+0002fe30: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+0002fe40: 7365 6c66 2e73 6573 7369 6f6e 203d 204e  self.session = N
+0002fe50: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
+0002fe60: 662e 6c61 6e67 7561 6765 5f6d 6170 203d  f.language_map =
+0002fe70: 204e 6f6e 650d 0a20 2020 2020 2020 2073   None..        s
+0002fe80: 656c 662e 6d79 4d65 6d6f 7279 5f6c 616e  elf.myMemory_lan
+0002fe90: 6775 6167 655f 6c69 7374 203d 204e 6f6e  guage_list = Non
+0002fea0: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+0002feb0: 6d61 7465 4361 745f 6c61 6e67 7561 6765  mateCat_language
+0002fec0: 5f6c 6973 7420 3d20 4e6f 6e65 0d0a 2020  _list = None..  
+0002fed0: 2020 2020 2020 7365 6c66 2e71 7565 7279        self.query
+0002fee0: 5f63 6f75 6e74 203d 2030 0d0a 2020 2020  _count = 0..    
+0002fef0: 2020 2020 7365 6c66 2e6f 7574 7075 745f      self.output_
+0002ff00: 7a68 203d 2027 7a68 2d43 4e27 0d0a 2020  zh = 'zh-CN'..  
+0002ff10: 2020 2020 2020 7365 6c66 2e69 6e70 7574        self.input
+0002ff20: 5f6c 696d 6974 203d 2069 6e74 2835 6532  _limit = int(5e2
+0002ff30: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0002ff40: 6465 6661 756c 745f 6672 6f6d 5f6c 616e  default_from_lan
+0002ff50: 6775 6167 6520 3d20 7365 6c66 2e6f 7574  guage = self.out
+0002ff60: 7075 745f 7a68 0d0a 0d0a 2020 2020 4054  put_zh....    @T
+0002ff70: 7365 2e64 6562 7567 5f6c 616e 6775 6167  se.debug_languag
+0002ff80: 655f 6d61 700d 0a20 2020 2064 6566 2067  e_map..    def g
+0002ff90: 6574 5f6c 616e 6775 6167 655f 6d61 7028  et_language_map(
+0002ffa0: 7365 6c66 2c20 6d79 4d65 6d6f 7279 5f68  self, myMemory_h
+0002ffb0: 6f73 745f 6874 6d6c 3a20 7374 722c 206d  ost_html: str, m
+0002ffc0: 6174 6563 6174 5f6c 616e 675f 7572 6c3a  atecat_lang_url:
+0002ffd0: 2073 7472 2c20 7373 3a20 5365 7373 696f   str, ss: Sessio
+0002ffe0: 6e54 7970 652c 2068 6561 6465 7273 3a20  nType, headers: 
+0002fff0: 6469 6374 2c0d 0a20 2020 2020 2020 2020  dict,..         
+00030000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030010: 7469 6d65 6f75 743a 204f 7074 696f 6e61  timeout: Optiona
+00030020: 6c5b 666c 6f61 745d 2c20 7072 6f78 6965  l[float], proxie
+00030030: 733a 204f 7074 696f 6e61 6c5b 6469 6374  s: Optional[dict
+00030040: 5d2c 202a 2a6b 7761 7267 733a 204c 616e  ], **kwargs: Lan
+00030050: 674d 6170 4b77 6172 6773 5479 7065 2920  gMapKwargsType) 
+00030060: 2d3e 2064 6963 743a 0d0a 2020 2020 2020  -> dict:..      
+00030070: 2020 6574 203d 206c 786d 6c2e 6574 7265    et = lxml.etre
+00030080: 652e 4854 4d4c 286d 794d 656d 6f72 795f  e.HTML(myMemory_
+00030090: 686f 7374 5f68 746d 6c29 0d0a 2020 2020  host_html)..    
+000300a0: 2020 2020 6c61 6e67 5f6c 6973 7420 3d20      lang_list = 
+000300b0: 6574 2e78 7061 7468 2827 2f2f 2a5b 4069  et.xpath('//*[@i
+000300c0: 643d 2273 656c 6563 745f 736f 7572 6365  d="select_source
+000300d0: 5f6d 6d22 5d2f 6f70 7469 6f6e 2f40 7661  _mm"]/option/@va
+000300e0: 6c75 6527 295b 323a 5d0d 0a20 2020 2020  lue')[2:]..     
+000300f0: 2020 2073 656c 662e 6d79 4d65 6d6f 7279     self.myMemory
+00030100: 5f6c 616e 6775 6167 655f 6c69 7374 203d  _language_list =
+00030110: 2073 6f72 7465 6428 6c69 7374 2873 6574   sorted(list(set
+00030120: 286c 616e 675f 6c69 7374 2929 290d 0a0d  (lang_list)))...
+00030130: 0a20 2020 2020 2020 206c 616e 675f 645f  .        lang_d_
+00030140: 6c69 7374 203d 2073 732e 6765 7428 6d61  list = ss.get(ma
+00030150: 7465 6361 745f 6c61 6e67 5f75 726c 2c20  tecat_lang_url, 
+00030160: 6865 6164 6572 733d 6865 6164 6572 732c  headers=headers,
+00030170: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
+00030180: 2c20 7072 6f78 6965 733d 7072 6f78 6965  , proxies=proxie
+00030190: 7329 2e6a 736f 6e28 290d 0a20 2020 2020  s).json()..     
+000301a0: 2020 2073 656c 662e 6d61 7465 4361 745f     self.mateCat_
+000301b0: 6c61 6e67 7561 6765 5f6c 6973 7420 3d20  language_list = 
+000301c0: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
+000301d0: 5b69 7465 6d5b 2763 6f64 6527 5d20 666f  [item['code'] fo
+000301e0: 7220 6974 656d 2069 6e20 6c61 6e67 5f64  r item in lang_d
+000301f0: 5f6c 6973 745d 2929 290d 0a0d 0a20 2020  _list])))....   
+00030200: 2020 2020 206c 616e 675f 6c69 7374 203d       lang_list =
+00030210: 2073 6f72 7465 6428 6c69 7374 2873 6574   sorted(list(set
+00030220: 2873 656c 662e 6d79 4d65 6d6f 7279 5f6c  (self.myMemory_l
+00030230: 616e 6775 6167 655f 6c69 7374 202b 2073  anguage_list + s
+00030240: 656c 662e 6d61 7465 4361 745f 6c61 6e67  elf.mateCat_lang
+00030250: 7561 6765 5f6c 6973 7429 2929 0d0a 2020  uage_list)))..  
+00030260: 2020 2020 2020 7265 7475 726e 207b 7d2e        return {}.
+00030270: 6672 6f6d 6b65 7973 286c 616e 675f 6c69  fromkeys(lang_li
+00030280: 7374 2c20 6c61 6e67 5f6c 6973 7429 0d0a  st, lang_list)..
+00030290: 0d0a 2020 2020 4054 7365 2e74 696d 655f  ..    @Tse.time_
+000302a0: 7374 6174 0d0a 2020 2020 4054 7365 2e63  stat..    @Tse.c
+000302b0: 6865 636b 5f71 7565 7279 0d0a 2020 2020  heck_query..    
+000302c0: 6465 6620 6d79 4d65 6d6f 7279 5f61 7069  def myMemory_api
+000302d0: 2873 656c 662c 2071 7565 7279 5f74 6578  (self, query_tex
+000302e0: 743a 2073 7472 2c20 6672 6f6d 5f6c 616e  t: str, from_lan
+000302f0: 6775 6167 653a 2073 7472 203d 2027 6175  guage: str = 'au
+00030300: 746f 272c 2074 6f5f 6c61 6e67 7561 6765  to', to_language
+00030310: 3a20 7374 7220 3d20 2765 6e27 2c20 2a2a  : str = 'en', **
+00030320: 6b77 6172 6773 3a20 4170 694b 7761 7267  kwargs: ApiKwarg
+00030330: 7354 7970 6529 202d 3e20 556e 696f 6e5b  sType) -> Union[
+00030340: 7374 722c 2064 6963 745d 3a0d 0a20 2020  str, dict]:..   
+00030350: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00030360: 2020 6874 7470 733a 2f2f 6d79 6d65 6d6f    https://mymemo
+00030370: 7279 2e74 7261 6e73 6c61 7465 642e 6e65  ry.translated.ne
+00030380: 740d 0a20 2020 2020 2020 203a 7061 7261  t..        :para
+00030390: 6d20 7175 6572 795f 7465 7874 3a20 7374  m query_text: st
+000303a0: 722c 206d 7573 742e 0d0a 2020 2020 2020  r, must...      
+000303b0: 2020 3a70 6172 616d 2066 726f 6d5f 6c61    :param from_la
+000303c0: 6e67 7561 6765 3a20 7374 722c 2064 6566  nguage: str, def
+000303d0: 6175 6c74 2027 6175 746f 272e 0d0a 2020  ault 'auto'...  
+000303e0: 2020 2020 2020 3a70 6172 616d 2074 6f5f        :param to_
+000303f0: 6c61 6e67 7561 6765 3a20 7374 722c 2064  language: str, d
+00030400: 6566 6175 6c74 2027 656e 272e 0d0a 2020  efault 'en'...  
+00030410: 2020 2020 2020 3a70 6172 616d 202a 2a6b        :param **k
+00030420: 7761 7267 733a 0d0a 2020 2020 2020 2020  wargs:..        
+00030430: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
+00030440: 696d 656f 7574 3a20 666c 6f61 742c 2064  imeout: float, d
+00030450: 6566 6175 6c74 204e 6f6e 652e 0d0a 2020  efault None...  
+00030460: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+00030470: 6172 616d 2070 726f 7869 6573 3a20 6469  aram proxies: di
+00030480: 6374 2c20 6465 6661 756c 7420 4e6f 6e65  ct, default None
+00030490: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000304a0: 2020 203a 7061 7261 6d20 736c 6565 705f     :param sleep_
+000304b0: 7365 636f 6e64 733a 2066 6c6f 6174 2c20  seconds: float, 
+000304c0: 6465 6661 756c 7420 302e 0d0a 2020 2020  default 0...    
+000304d0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+000304e0: 616d 2069 735f 6465 7461 696c 5f72 6573  am is_detail_res
+000304f0: 756c 743a 2062 6f6f 6c2c 2064 6566 6175  ult: bool, defau
+00030500: 6c74 2046 616c 7365 2e0d 0a20 2020 2020  lt False...     
+00030510: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00030520: 6d20 6966 5f69 676e 6f72 655f 6c69 6d69  m if_ignore_limi
+00030530: 745f 6f66 5f6c 656e 6774 683a 2062 6f6f  t_of_length: boo
+00030540: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+00030550: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00030560: 2020 203a 7061 7261 6d20 6c69 6d69 745f     :param limit_
+00030570: 6f66 5f6c 656e 6774 683a 2069 6e74 2c20  of_length: int, 
+00030580: 6465 6661 756c 7420 3230 3030 302e 0d0a  default 20000...
+00030590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000305a0: 3a70 6172 616d 2069 665f 6967 6e6f 7265  :param if_ignore
+000305b0: 5f65 6d70 7479 5f71 7565 7279 3a20 626f  _empty_query: bo
+000305c0: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
+000305d0: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
+000305e0: 2020 2020 3a70 6172 616d 2075 7064 6174      :param updat
+000305f0: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
+00030600: 6672 6571 3a20 696e 742c 2064 6566 6175  freq: int, defau
+00030610: 6c74 2031 3030 302e 0d0a 2020 2020 2020  lt 1000...      
+00030620: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+00030630: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
+00030640: 6166 7465 725f 7365 636f 6e64 733a 2066  after_seconds: f
+00030650: 6c6f 6174 2c20 6465 6661 756c 7420 3135  loat, default 15
+00030660: 3030 2e0d 0a20 2020 2020 2020 2020 2020  00...           
+00030670: 2020 2020 203a 7061 7261 6d20 6966 5f73       :param if_s
+00030680: 686f 775f 7469 6d65 5f73 7461 743a 2062  how_time_stat: b
+00030690: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+000306a0: 7365 2e0d 0a20 2020 2020 2020 2020 2020  se...           
+000306b0: 2020 2020 203a 7061 7261 6d20 7368 6f77       :param show
+000306c0: 5f74 696d 655f 7374 6174 5f70 7265 6369  _time_stat_preci
+000306d0: 7369 6f6e 3a20 696e 742c 2064 6566 6175  sion: int, defau
+000306e0: 6c74 2032 2e0d 0a20 2020 2020 2020 2020  lt 2...         
+000306f0: 2020 2020 2020 203a 7061 7261 6d20 6966         :param if
+00030700: 5f70 7269 6e74 5f77 6172 6e69 6e67 3a20  _print_warning: 
+00030710: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
+00030720: 7565 2e0d 0a20 2020 2020 2020 2020 2020  ue...           
+00030730: 2020 2020 203a 7061 7261 6d20 6d79 4d65       :param myMe
+00030740: 6d6f 7279 5f6d 6f64 653a 2073 7472 2c20  mory_mode: str, 
+00030750: 6465 6661 756c 7420 2277 6562 222c 2063  default "web", c
+00030760: 686f 6f73 6520 6672 6f6d 2028 2277 6562  hoose from ("web
+00030770: 222c 2022 6170 6922 292e 0d0a 2020 2020  ", "api")...    
+00030780: 2020 2020 3a72 6574 7572 6e3a 2073 7472      :return: str
+00030790: 206f 7220 6469 6374 0d0a 2020 2020 2020   or dict..      
+000307a0: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
+000307b0: 206d 6f64 6520 3d20 6b77 6172 6773 2e67   mode = kwargs.g
+000307c0: 6574 2827 6d79 4d65 6d6f 7279 5f6d 6f64  et('myMemory_mod
+000307d0: 6527 2c20 2777 6562 2729 0d0a 2020 2020  e', 'web')..    
+000307e0: 2020 2020 7469 6d65 6f75 7420 3d20 6b77      timeout = kw
+000307f0: 6172 6773 2e67 6574 2827 7469 6d65 6f75  args.get('timeou
+00030800: 7427 2c20 4e6f 6e65 290d 0a20 2020 2020  t', None)..     
+00030810: 2020 2070 726f 7869 6573 203d 206b 7761     proxies = kwa
+00030820: 7267 732e 6765 7428 2770 726f 7869 6573  rgs.get('proxies
+00030830: 272c 204e 6f6e 6529 0d0a 2020 2020 2020  ', None)..      
+00030840: 2020 736c 6565 705f 7365 636f 6e64 7320    sleep_seconds 
+00030850: 3d20 6b77 6172 6773 2e67 6574 2827 736c  = kwargs.get('sl
+00030860: 6565 705f 7365 636f 6e64 7327 2c20 3029  eep_seconds', 0)
+00030870: 0d0a 2020 2020 2020 2020 6966 5f70 7269  ..        if_pri
+00030880: 6e74 5f77 6172 6e69 6e67 203d 206b 7761  nt_warning = kwa
+00030890: 7267 732e 6765 7428 2769 665f 7072 696e  rgs.get('if_prin
+000308a0: 745f 7761 726e 696e 6727 2c20 5472 7565  t_warning', True
+000308b0: 290d 0a20 2020 2020 2020 2069 735f 6465  )..        is_de
+000308c0: 7461 696c 5f72 6573 756c 7420 3d20 6b77  tail_result = kw
+000308d0: 6172 6773 2e67 6574 2827 6973 5f64 6574  args.get('is_det
+000308e0: 6169 6c5f 7265 7375 6c74 272c 2046 616c  ail_result', Fal
+000308f0: 7365 290d 0a20 2020 2020 2020 2075 7064  se)..        upd
+00030900: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
+00030910: 725f 6672 6571 203d 206b 7761 7267 732e  r_freq = kwargs.
+00030920: 6765 7428 2775 7064 6174 655f 7365 7373  get('update_sess
+00030930: 696f 6e5f 6166 7465 725f 6672 6571 272c  ion_after_freq',
+00030940: 2073 656c 662e 6465 6661 756c 745f 7365   self.default_se
+00030950: 7373 696f 6e5f 6672 6571 290d 0a20 2020  ssion_freq)..   
+00030960: 2020 2020 2075 7064 6174 655f 7365 7373       update_sess
+00030970: 696f 6e5f 6166 7465 725f 7365 636f 6e64  ion_after_second
+00030980: 7320 3d20 6b77 6172 6773 2e67 6574 2827  s = kwargs.get('
+00030990: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
+000309a0: 6674 6572 5f73 6563 6f6e 6473 272c 2073  fter_seconds', s
+000309b0: 656c 662e 6465 6661 756c 745f 7365 7373  elf.default_sess
+000309c0: 696f 6e5f 7365 636f 6e64 7329 0d0a 2020  ion_seconds)..  
+000309d0: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
+000309e0: 5f69 6e70 7574 5f6c 696d 6974 2871 7565  _input_limit(que
+000309f0: 7279 5f74 6578 742c 2073 656c 662e 696e  ry_text, self.in
+00030a00: 7075 745f 6c69 6d69 7429 0d0a 0d0a 2020  put_limit)....  
+00030a10: 2020 2020 2020 6e6f 745f 7570 6461 7465        not_update
+00030a20: 5f63 6f6e 645f 6672 6571 203d 2031 2069  _cond_freq = 1 i
+00030a30: 6620 7365 6c66 2e71 7565 7279 5f63 6f75  f self.query_cou
+00030a40: 6e74 203c 2075 7064 6174 655f 7365 7373  nt < update_sess
+00030a50: 696f 6e5f 6166 7465 725f 6672 6571 2065  ion_after_freq e
+00030a60: 6c73 6520 300d 0a20 2020 2020 2020 206e  lse 0..        n
+00030a70: 6f74 5f75 7064 6174 655f 636f 6e64 5f74  ot_update_cond_t
+00030a80: 696d 6520 3d20 3120 6966 2074 696d 652e  ime = 1 if time.
+00030a90: 7469 6d65 2829 202d 2073 656c 662e 6265  time() - self.be
+00030aa0: 6769 6e5f 7469 6d65 203c 2075 7064 6174  gin_time < updat
+00030ab0: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
+00030ac0: 7365 636f 6e64 7320 656c 7365 2030 0d0a  seconds else 0..
+00030ad0: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
+00030ae0: 7365 6c66 2e73 6573 7369 6f6e 2061 6e64  self.session and
+00030af0: 2073 656c 662e 6c61 6e67 7561 6765 5f6d   self.language_m
+00030b00: 6170 2061 6e64 206e 6f74 5f75 7064 6174  ap and not_updat
+00030b10: 655f 636f 6e64 5f66 7265 7120 616e 6420  e_cond_freq and 
+00030b20: 6e6f 745f 7570 6461 7465 5f63 6f6e 645f  not_update_cond_
+00030b30: 7469 6d65 293a 0d0a 2020 2020 2020 2020  time):..        
+00030b40: 2020 2020 7365 6c66 2e73 6573 7369 6f6e      self.session
+00030b50: 203d 2072 6571 7565 7374 732e 5365 7373   = requests.Sess
+00030b60: 696f 6e28 290d 0a20 2020 2020 2020 2020  ion()..         
+00030b70: 2020 2068 6f73 745f 6874 6d6c 203d 2073     host_html = s
+00030b80: 656c 662e 7365 7373 696f 6e2e 6765 7428  elf.session.get(
+00030b90: 7365 6c66 2e68 6f73 745f 7572 6c2c 2068  self.host_url, h
+00030ba0: 6561 6465 7273 3d73 656c 662e 686f 7374  eaders=self.host
+00030bb0: 5f68 6561 6465 7273 2c20 7469 6d65 6f75  _headers, timeou
+00030bc0: 743d 7469 6d65 6f75 742c 2070 726f 7869  t=timeout, proxi
+00030bd0: 6573 3d70 726f 7869 6573 292e 7465 7874  es=proxies).text
+00030be0: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+00030bf0: 6275 675f 6c61 6e67 5f6b 7761 7267 7320  bug_lang_kwargs 
+00030c00: 3d20 7365 6c66 2e64 6562 7567 5f6c 616e  = self.debug_lan
+00030c10: 675f 6b77 6172 6773 2866 726f 6d5f 6c61  g_kwargs(from_la
+00030c20: 6e67 7561 6765 2c20 746f 5f6c 616e 6775  nguage, to_langu
+00030c30: 6167 652c 2073 656c 662e 6465 6661 756c  age, self.defaul
+00030c40: 745f 6672 6f6d 5f6c 616e 6775 6167 652c  t_from_language,
+00030c50: 2069 665f 7072 696e 745f 7761 726e 696e   if_print_warnin
+00030c60: 6729 0d0a 2020 2020 2020 2020 2020 2020  g)..            
+00030c70: 7365 6c66 2e6c 616e 6775 6167 655f 6d61  self.language_ma
+00030c80: 7020 3d20 7365 6c66 2e67 6574 5f6c 616e  p = self.get_lan
+00030c90: 6775 6167 655f 6d61 7028 686f 7374 5f68  guage_map(host_h
+00030ca0: 746d 6c2c 2073 656c 662e 6765 745f 6d61  tml, self.get_ma
+00030cb0: 7465 6361 745f 6c61 6e67 7561 6765 5f75  tecat_language_u
+00030cc0: 726c 2c20 7365 6c66 2e73 6573 7369 6f6e  rl, self.session
+00030cd0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00030ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030d00: 2020 2020 2020 2020 2073 656c 662e 686f           self.ho
+00030d10: 7374 5f68 6561 6465 7273 2c20 7469 6d65  st_headers, time
+00030d20: 6f75 742c 2070 726f 7869 6573 2c20 2a2a  out, proxies, **
+00030d30: 6465 6275 675f 6c61 6e67 5f6b 7761 7267  debug_lang_kwarg
+00030d40: 7329 0d0a 0d0a 2020 2020 2020 2020 6966  s)....        if
+00030d50: 2066 726f 6d5f 6c61 6e67 7561 6765 203d   from_language =
+00030d60: 3d20 2761 7574 6f27 3a0d 0a20 2020 2020  = 'auto':..     
+00030d70: 2020 2020 2020 2066 726f 6d5f 6c61 6e67         from_lang
+00030d80: 7561 6765 203d 2073 656c 662e 7761 726e  uage = self.warn
+00030d90: 696e 675f 6175 746f 5f6c 616e 6728 276d  ing_auto_lang('m
+00030da0: 794d 656d 6f72 7927 2c20 7365 6c66 2e64  yMemory', self.d
+00030db0: 6566 6175 6c74 5f66 726f 6d5f 6c61 6e67  efault_from_lang
+00030dc0: 7561 6765 2c20 6966 5f70 7269 6e74 5f77  uage, if_print_w
+00030dd0: 6172 6e69 6e67 290d 0a20 2020 2020 2020  arning)..       
+00030de0: 2066 726f 6d5f 6c61 6e67 7561 6765 2c20   from_language, 
+00030df0: 746f 5f6c 616e 6775 6167 6520 3d20 7365  to_language = se
+00030e00: 6c66 2e63 6865 636b 5f6c 616e 6775 6167  lf.check_languag
+00030e10: 6528 6672 6f6d 5f6c 616e 6775 6167 652c  e(from_language,
+00030e20: 2074 6f5f 6c61 6e67 7561 6765 2c20 7365   to_language, se
+00030e30: 6c66 2e6c 616e 6775 6167 655f 6d61 702c  lf.language_map,
+00030e40: 206f 7574 7075 745f 7a68 3d73 656c 662e   output_zh=self.
+00030e50: 6f75 7470 7574 5f7a 682c 0d0a 2020 2020  output_zh,..    
+00030e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030e90: 2020 2020 206f 7574 7075 745f 656e 5f74       output_en_t
+00030ea0: 7261 6e73 6c61 746f 723d 276d 794d 656d  ranslator='myMem
+00030eb0: 6f72 7927 2c20 6f75 7470 7574 5f65 6e3d  ory', output_en=
+00030ec0: 2765 6e2d 4742 2729 0d0a 0d0a 2020 2020  'en-GB')....    
+00030ed0: 2020 2020 7061 7261 6d73 203d 207b 0d0a      params = {..
+00030ee0: 2020 2020 2020 2020 2020 2020 2771 273a              'q':
+00030ef0: 2071 7565 7279 5f74 6578 742c 0d0a 2020   query_text,..  
+00030f00: 2020 2020 2020 2020 2020 276c 616e 6770            'langp
+00030f10: 6169 7227 3a20 6627 7b66 726f 6d5f 6c61  air': f'{from_la
+00030f20: 6e67 7561 6765 7d7c 7b74 6f5f 6c61 6e67  nguage}|{to_lang
+00030f30: 7561 6765 7d27 0d0a 2020 2020 2020 2020  uage}'..        
+00030f40: 7d0d 0a20 2020 2020 2020 2070 6172 616d  }..        param
+00030f50: 7320 3d20 7061 7261 6d73 2069 6620 6d6f  s = params if mo
+00030f60: 6465 203d 3d20 2761 7069 2720 656c 7365  de == 'api' else
+00030f70: 207b 2a2a 7061 7261 6d73 2c20 2a2a 7b27   {**params, **{'
+00030f80: 6d74 6f6e 6c79 273a 2031 7d7d 0d0a 2020  mtonly': 1}}..  
+00030f90: 2020 2020 2020 6170 695f 7572 6c20 3d20        api_url = 
+00030fa0: 7365 6c66 2e61 7069 5f61 7069 5f75 726c  self.api_api_url
+00030fb0: 2069 6620 6d6f 6465 203d 3d20 2761 7069   if mode == 'api
+00030fc0: 2720 656c 7365 2073 656c 662e 6170 695f  ' else self.api_
+00030fd0: 7765 625f 7572 6c0d 0a0d 0a20 2020 2020  web_url....     
+00030fe0: 2020 2072 203d 2073 656c 662e 7365 7373     r = self.sess
+00030ff0: 696f 6e2e 6765 7428 6170 695f 7572 6c2c  ion.get(api_url,
+00031000: 2070 6172 616d 733d 7061 7261 6d73 2c20   params=params, 
+00031010: 6865 6164 6572 733d 7365 6c66 2e68 6f73  headers=self.hos
+00031020: 745f 6865 6164 6572 732c 2074 696d 656f  t_headers, timeo
+00031030: 7574 3d74 696d 656f 7574 2c20 7072 6f78  ut=timeout, prox
+00031040: 6965 733d 7072 6f78 6965 7329 0d0a 2020  ies=proxies)..  
+00031050: 2020 2020 2020 722e 7261 6973 655f 666f        r.raise_fo
+00031060: 725f 7374 6174 7573 2829 0d0a 2020 2020  r_status()..    
+00031070: 2020 2020 6461 7461 203d 2072 2e6a 736f      data = r.jso
+00031080: 6e28 290d 0a20 2020 2020 2020 2074 696d  n()..        tim
+00031090: 652e 736c 6565 7028 736c 6565 705f 7365  e.sleep(sleep_se
+000310a0: 636f 6e64 7329 0d0a 2020 2020 2020 2020  conds)..        
+000310b0: 7365 6c66 2e71 7565 7279 5f63 6f75 6e74  self.query_count
+000310c0: 202b 3d20 310d 0a20 2020 2020 2020 2072   += 1..        r
+000310d0: 6574 7572 6e20 6461 7461 2069 6620 6973  eturn data if is
+000310e0: 5f64 6574 6169 6c5f 7265 7375 6c74 2065  _detail_result e
+000310f0: 6c73 6520 6461 7461 5b27 7265 7370 6f6e  lse data['respon
+00031100: 7365 4461 7461 275d 5b27 7472 616e 736c  seData']['transl
+00031110: 6174 6564 5465 7874 275d 0d0a 0d0a 0d0a  atedText']......
+00031120: 636c 6173 7320 4d69 7261 6928 5473 6529  class Mirai(Tse)
+00031130: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
+00031140: 745f 5f28 7365 6c66 293a 0d0a 2020 2020  t__(self):..    
+00031150: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+00031160: 6974 5f5f 2829 0d0a 2020 2020 2020 2020  it__()..        
+00031170: 7365 6c66 2e68 6f6d 655f 7572 6c20 3d20  self.home_url = 
+00031180: 2768 7474 7073 3a2f 2f6d 6972 6169 7472  'https://miraitr
+00031190: 616e 736c 6174 652e 636f 6d27 0d0a 2020  anslate.com'..  
+000311a0: 2020 2020 2020 7365 6c66 2e68 6f73 745f        self.host_
+000311b0: 7572 6c20 3d20 2768 7474 7073 3a2f 2f6d  url = 'https://m
+000311c0: 6972 6169 7472 616e 736c 6174 652e 636f  iraitranslate.co
+000311d0: 6d2f 7472 6961 6c2f 270d 0a20 2020 2020  m/trial/'..     
+000311e0: 2020 2073 656c 662e 6170 695f 7572 6c20     self.api_url 
+000311f0: 3d20 2768 7474 7073 3a2f 2f74 7269 616c  = 'https://trial
+00031200: 2e6d 6972 6169 7472 616e 736c 6174 652e  .miraitranslate.
+00031210: 636f 6d2f 7472 6961 6c2f 6170 692f 7472  com/trial/api/tr
+00031220: 616e 736c 6174 652e 7068 7027 0d0a 2020  anslate.php'..  
+00031230: 2020 2020 2020 7365 6c66 2e6c 616e 675f        self.lang_
+00031240: 7572 6c20 3d20 4e6f 6e65 0d0a 2020 2020  url = None..    
+00031250: 2020 2020 7365 6c66 2e6c 616e 675f 7572      self.lang_ur
+00031260: 6c5f 7061 7474 6572 6e20 3d20 276d 6169  l_pattern = 'mai
+00031270: 6e2d 6573 3230 3135 2e28 2e2a 3f29 2e6a  n-es2015.(.*?).j
+00031280: 7327 0d0a 2020 2020 2020 2020 7365 6c66  s'..        self
+00031290: 2e64 6574 6563 745f 6c61 6e67 5f75 726c  .detect_lang_url
+000312a0: 203d 2027 6874 7470 733a 2f2f 7472 6961   = 'https://tria
+000312b0: 6c2e 6d69 7261 6974 7261 6e73 6c61 7465  l.miraitranslate
+000312c0: 2e63 6f6d 2f74 7269 616c 2f61 7069 2f64  .com/trial/api/d
+000312d0: 6574 6563 745f 6c61 6e67 2e70 6870 270d  etect_lang.php'.
+000312e0: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
+000312f0: 6163 655f 7572 6c20 3d20 2768 7474 7073  ace_url = 'https
+00031300: 3a2f 2f74 7269 616c 2e6d 6972 6169 7472  ://trial.miraitr
+00031310: 616e 736c 6174 652e 636f 6d2f 7472 6961  anslate.com/tria
+00031320: 6c2f 6170 692f 7472 6163 652e 7068 7027  l/api/trace.php'
+00031330: 0d0a 2020 2020 2020 2020 7365 6c66 2e68  ..        self.h
+00031340: 6f73 745f 6865 6164 6572 7320 3d20 7365  ost_headers = se
+00031350: 6c66 2e67 6574 5f68 6561 6465 7273 2873  lf.get_headers(s
+00031360: 656c 662e 686f 6d65 5f75 726c 2c20 6966  elf.home_url, if
+00031370: 5f61 7069 3d46 616c 7365 290d 0a20 2020  _api=False)..   
+00031380: 2020 2020 2073 656c 662e 6170 695f 6a73       self.api_js
+00031390: 6f6e 5f68 6561 6465 7273 203d 2073 656c  on_headers = sel
+000313a0: 662e 6765 745f 6865 6164 6572 7328 7365  f.get_headers(se
+000313b0: 6c66 2e68 6f6d 655f 7572 6c2c 2069 665f  lf.home_url, if_
+000313c0: 6170 693d 5472 7565 2c20 6966 5f6a 736f  api=True, if_jso
+000313d0: 6e5f 666f 725f 6170 693d 5472 7565 290d  n_for_api=True).
+000313e0: 0a20 2020 2020 2020 2073 656c 662e 6170  .        self.ap
+000313f0: 695f 7465 7874 5f68 6561 6465 7273 203d  i_text_headers =
+00031400: 2073 656c 662e 6765 745f 6865 6164 6572   self.get_header
+00031410: 7328 7365 6c66 2e68 6f6d 655f 7572 6c2c  s(self.home_url,
+00031420: 2069 665f 6170 693d 5472 7565 2c20 6966   if_api=True, if
+00031430: 5f61 6a61 785f 666f 725f 6170 693d 4661  _ajax_for_api=Fa
+00031440: 6c73 6529 0d0a 2020 2020 2020 2020 7365  lse)..        se
+00031450: 6c66 2e73 6573 7369 6f6e 203d 204e 6f6e  lf.session = Non
+00031460: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+00031470: 6c61 6e67 7561 6765 5f6d 6170 203d 204e  language_map = N
+00031480: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
+00031490: 662e 7472 616e 5f6b 6579 203d 204e 6f6e  f.tran_key = Non
+000314a0: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+000314b0: 7472 616e 735f 6964 203d 2073 7472 2875  trans_id = str(u
+000314c0: 7569 642e 7575 6964 3428 2929 0d0a 2020  uid.uuid4())..  
+000314d0: 2020 2020 2020 7365 6c66 2e75 7365 725f        self.user_
+000314e0: 6964 203d 2073 7472 2875 7569 642e 7575  id = str(uuid.uu
+000314f0: 6964 3428 2929 0d0a 2020 2020 2020 2020  id4())..        
+00031500: 7365 6c66 2e6c 616e 675f 7a68 5f6d 6170  self.lang_zh_map
+00031510: 203d 207b 277a 682d 434e 273a 2027 7a68   = {'zh-CN': 'zh
+00031520: 272c 2027 7a68 2d54 5727 3a20 277a 7427  ', 'zh-TW': 'zt'
+00031530: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
+00031540: 7175 6572 795f 636f 756e 7420 3d20 300d  query_count = 0.
+00031550: 0a20 2020 2020 2020 2073 656c 662e 6f75  .        self.ou
+00031560: 7470 7574 5f7a 6820 3d20 277a 6827 0d0a  tput_zh = 'zh'..
+00031570: 2020 2020 2020 2020 7365 6c66 2e69 6e70          self.inp
+00031580: 7574 5f6c 696d 6974 203d 2069 6e74 2832  ut_limit = int(2
+00031590: 6533 290d 0a20 2020 2020 2020 2073 656c  e3)..        sel
+000315a0: 662e 6465 6661 756c 745f 6672 6f6d 5f6c  f.default_from_l
+000315b0: 616e 6775 6167 6520 3d20 7365 6c66 2e6f  anguage = self.o
+000315c0: 7574 7075 745f 7a68 0d0a 0d0a 2020 2020  utput_zh....    
+000315d0: 4054 7365 2e64 6562 7567 5f6c 616e 6775  @Tse.debug_langu
+000315e0: 6167 655f 6d61 700d 0a20 2020 2064 6566  age_map..    def
+000315f0: 2067 6574 5f6c 616e 6775 6167 655f 6d61   get_language_ma
+00031600: 7028 7365 6c66 2c20 6c61 6e67 5f75 726c  p(self, lang_url
+00031610: 3a20 7374 722c 2073 733a 2053 6573 7369  : str, ss: Sessi
+00031620: 6f6e 5479 7065 2c20 6865 6164 6572 733a  onType, headers:
+00031630: 2064 6963 742c 2074 696d 656f 7574 3a20   dict, timeout: 
+00031640: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d2c  Optional[float],
+00031650: 2070 726f 7869 6573 3a20 4f70 7469 6f6e   proxies: Option
+00031660: 616c 5b64 6963 745d 2c20 2a2a 6b77 6172  al[dict], **kwar
+00031670: 6773 3a20 4c61 6e67 4d61 704b 7761 7267  gs: LangMapKwarg
+00031680: 7354 7970 6529 202d 3e20 6469 6374 3a0d  sType) -> dict:.
+00031690: 0a20 2020 2020 2020 206a 735f 6874 6d6c  .        js_html
+000316a0: 203d 2073 732e 6765 7428 6c61 6e67 5f75   = ss.get(lang_u
+000316b0: 726c 2c20 6865 6164 6572 733d 6865 6164  rl, headers=head
+000316c0: 6572 732c 2074 696d 656f 7574 3d74 696d  ers, timeout=tim
+000316d0: 656f 7574 2c20 7072 6f78 6965 733d 7072  eout, proxies=pr
+000316e0: 6f78 6965 7329 2e74 6578 740d 0a20 2020  oxies).text..   
+000316f0: 2020 2020 206c 616e 675f 7061 6972 7320       lang_pairs 
+00031700: 3d20 7265 2e63 6f6d 7069 6c65 2827 222f  = re.compile('"/
+00031710: 7472 6961 6c2f 285c 5c77 7b32 7d29 2f28  trial/(\\w{2})/(
+00031720: 5c5c 777b 327d 2922 2729 2e66 696e 6461  \\w{2})"').finda
+00031730: 6c6c 286a 735f 6874 6d6c 290d 0a20 2020  ll(js_html)..   
+00031740: 2020 2020 2072 6574 7572 6e20 7b66 5f6c       return {f_l
+00031750: 616e 673a 205b 7620 666f 7220 6b2c 2076  ang: [v for k, v
+00031760: 2069 6e20 6c61 6e67 5f70 6169 7273 2069   in lang_pairs i
+00031770: 6620 6b20 3d3d 2066 5f6c 616e 675d 2066  f k == f_lang] f
+00031780: 6f72 2066 5f6c 616e 672c 2074 5f6c 616e  or f_lang, t_lan
+00031790: 6720 696e 206c 616e 675f 7061 6972 737d  g in lang_pairs}
+000317a0: 0d0a 0d0a 2020 2020 4054 7365 2e75 6e63  ....    @Tse.unc
+000317b0: 6572 7469 6669 6564 0d0a 2020 2020 4054  ertified..    @T
+000317c0: 7365 2e74 696d 655f 7374 6174 0d0a 2020  se.time_stat..  
+000317d0: 2020 4054 7365 2e63 6865 636b 5f71 7565    @Tse.check_que
+000317e0: 7279 0d0a 2020 2020 6465 6620 6d69 7261  ry..    def mira
+000317f0: 695f 6170 6928 7365 6c66 2c20 7175 6572  i_api(self, quer
+00031800: 795f 7465 7874 3a20 7374 722c 2066 726f  y_text: str, fro
+00031810: 6d5f 6c61 6e67 7561 6765 3a20 7374 7220  m_language: str 
+00031820: 3d20 2761 7574 6f27 2c20 746f 5f6c 616e  = 'auto', to_lan
+00031830: 6775 6167 653a 2073 7472 203d 2027 6a61  guage: str = 'ja
+00031840: 272c 202a 2a6b 7761 7267 733a 2041 7069  ', **kwargs: Api
+00031850: 4b77 6172 6773 5479 7065 2920 2d3e 2055  KwargsType) -> U
+00031860: 6e69 6f6e 5b73 7472 2c20 6469 6374 5d3a  nion[str, dict]:
+00031870: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00031880: 2020 2020 2020 2068 7474 7073 3a2f 2f6d         https://m
+00031890: 6972 6169 7472 616e 736c 6174 652e 636f  iraitranslate.co
+000318a0: 6d2f 656e 2f74 7269 616c 2f0d 0a20 2020  m/en/trial/..   
+000318b0: 2020 2020 203a 7061 7261 6d20 7175 6572       :param quer
+000318c0: 795f 7465 7874 3a20 7374 722c 206d 7573  y_text: str, mus
+000318d0: 742e 0d0a 2020 2020 2020 2020 3a70 6172  t...        :par
+000318e0: 616d 2066 726f 6d5f 6c61 6e67 7561 6765  am from_language
+000318f0: 3a20 7374 722c 2064 6566 6175 6c74 2027  : str, default '
+00031900: 6175 746f 272e 0d0a 2020 2020 2020 2020  auto'...        
+00031910: 3a70 6172 616d 2074 6f5f 6c61 6e67 7561  :param to_langua
+00031920: 6765 3a20 7374 722c 2064 6566 6175 6c74  ge: str, default
+00031930: 2027 6a61 272e 0d0a 2020 2020 2020 2020   'ja'...        
+00031940: 3a70 6172 616d 202a 2a6b 7761 7267 733a  :param **kwargs:
+00031950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00031960: 2020 3a70 6172 616d 2074 696d 656f 7574    :param timeout
+00031970: 3a20 666c 6f61 742c 2064 6566 6175 6c74  : float, default
+00031980: 204e 6f6e 652e 0d0a 2020 2020 2020 2020   None...        
+00031990: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+000319a0: 726f 7869 6573 3a20 6469 6374 2c20 6465  roxies: dict, de
+000319b0: 6661 756c 7420 4e6f 6e65 2e0d 0a20 2020  fault None...   
+000319c0: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+000319d0: 7261 6d20 736c 6565 705f 7365 636f 6e64  ram sleep_second
+000319e0: 733a 2066 6c6f 6174 2c20 6465 6661 756c  s: float, defaul
+000319f0: 7420 302e 0d0a 2020 2020 2020 2020 2020  t 0...          
+00031a00: 2020 2020 2020 3a70 6172 616d 2069 735f        :param is_
+00031a10: 6465 7461 696c 5f72 6573 756c 743a 2062  detail_result: b
+00031a20: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+00031a30: 7365 2e0d 0a20 2020 2020 2020 2020 2020  se...           
+00031a40: 2020 2020 203a 7061 7261 6d20 6966 5f69       :param if_i
+00031a50: 676e 6f72 655f 6c69 6d69 745f 6f66 5f6c  gnore_limit_of_l
+00031a60: 656e 6774 683a 2062 6f6f 6c2c 2064 6566  ength: bool, def
+00031a70: 6175 6c74 2046 616c 7365 2e0d 0a20 2020  ault False...   
+00031a80: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+00031a90: 7261 6d20 6c69 6d69 745f 6f66 5f6c 656e  ram limit_of_len
+00031aa0: 6774 683a 2069 6e74 2c20 6465 6661 756c  gth: int, defaul
+00031ab0: 7420 3230 3030 302e 0d0a 2020 2020 2020  t 20000...      
+00031ac0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+00031ad0: 2069 665f 6967 6e6f 7265 5f65 6d70 7479   if_ignore_empty
+00031ae0: 5f71 7565 7279 3a20 626f 6f6c 2c20 6465  _query: bool, de
+00031af0: 6661 756c 7420 4661 6c73 652e 0d0a 2020  fault False...  
+00031b00: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+00031b10: 6172 616d 2075 7064 6174 655f 7365 7373  aram update_sess
+00031b20: 696f 6e5f 6166 7465 725f 6672 6571 3a20  ion_after_freq: 
+00031b30: 696e 742c 2064 6566 6175 6c74 2031 3030  int, default 100
+00031b40: 302e 0d0a 2020 2020 2020 2020 2020 2020  0...            
+00031b50: 2020 2020 3a70 6172 616d 2075 7064 6174      :param updat
+00031b60: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
+00031b70: 7365 636f 6e64 733a 2066 6c6f 6174 2c20  seconds: float, 
+00031b80: 6465 6661 756c 7420 3135 3030 2e0d 0a20  default 1500... 
+00031b90: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+00031ba0: 7061 7261 6d20 6966 5f73 686f 775f 7469  param if_show_ti
+00031bb0: 6d65 5f73 7461 743a 2062 6f6f 6c2c 2064  me_stat: bool, d
+00031bc0: 6566 6175 6c74 2046 616c 7365 2e0d 0a20  efault False... 
+00031bd0: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+00031be0: 7061 7261 6d20 7368 6f77 5f74 696d 655f  param show_time_
+00031bf0: 7374 6174 5f70 7265 6369 7369 6f6e 3a20  stat_precision: 
+00031c00: 696e 742c 2064 6566 6175 6c74 2032 2e0d  int, default 2..
+00031c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00031c20: 203a 7061 7261 6d20 6966 5f70 7269 6e74   :param if_print
+00031c30: 5f77 6172 6e69 6e67 3a20 626f 6f6c 2c20  _warning: bool, 
+00031c40: 6465 6661 756c 7420 5472 7565 2e0d 0a20  default True... 
+00031c50: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00031c60: 7374 7220 6f72 2064 6963 740d 0a20 2020  str or dict..   
+00031c70: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
+00031c80: 2020 2020 7469 6d65 6f75 7420 3d20 6b77      timeout = kw
+00031c90: 6172 6773 2e67 6574 2827 7469 6d65 6f75  args.get('timeou
+00031ca0: 7427 2c20 4e6f 6e65 290d 0a20 2020 2020  t', None)..     
+00031cb0: 2020 2070 726f 7869 6573 203d 206b 7761     proxies = kwa
+00031cc0: 7267 732e 6765 7428 2770 726f 7869 6573  rgs.get('proxies
+00031cd0: 272c 204e 6f6e 6529 0d0a 2020 2020 2020  ', None)..      
+00031ce0: 2020 736c 6565 705f 7365 636f 6e64 7320    sleep_seconds 
+00031cf0: 3d20 6b77 6172 6773 2e67 6574 2827 736c  = kwargs.get('sl
+00031d00: 6565 705f 7365 636f 6e64 7327 2c20 3029  eep_seconds', 0)
+00031d10: 0d0a 2020 2020 2020 2020 6966 5f70 7269  ..        if_pri
+00031d20: 6e74 5f77 6172 6e69 6e67 203d 206b 7761  nt_warning = kwa
+00031d30: 7267 732e 6765 7428 2769 665f 7072 696e  rgs.get('if_prin
+00031d40: 745f 7761 726e 696e 6727 2c20 5472 7565  t_warning', True
+00031d50: 290d 0a20 2020 2020 2020 2069 735f 6465  )..        is_de
+00031d60: 7461 696c 5f72 6573 756c 7420 3d20 6b77  tail_result = kw
+00031d70: 6172 6773 2e67 6574 2827 6973 5f64 6574  args.get('is_det
+00031d80: 6169 6c5f 7265 7375 6c74 272c 2046 616c  ail_result', Fal
+00031d90: 7365 290d 0a20 2020 2020 2020 2075 7064  se)..        upd
+00031da0: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
+00031db0: 725f 6672 6571 203d 206b 7761 7267 732e  r_freq = kwargs.
+00031dc0: 6765 7428 2775 7064 6174 655f 7365 7373  get('update_sess
+00031dd0: 696f 6e5f 6166 7465 725f 6672 6571 272c  ion_after_freq',
+00031de0: 2073 656c 662e 6465 6661 756c 745f 7365   self.default_se
+00031df0: 7373 696f 6e5f 6672 6571 290d 0a20 2020  ssion_freq)..   
+00031e00: 2020 2020 2075 7064 6174 655f 7365 7373       update_sess
+00031e10: 696f 6e5f 6166 7465 725f 7365 636f 6e64  ion_after_second
+00031e20: 7320 3d20 6b77 6172 6773 2e67 6574 2827  s = kwargs.get('
+00031e30: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
+00031e40: 6674 6572 5f73 6563 6f6e 6473 272c 2073  fter_seconds', s
+00031e50: 656c 662e 6465 6661 756c 745f 7365 7373  elf.default_sess
+00031e60: 696f 6e5f 7365 636f 6e64 7329 0d0a 2020  ion_seconds)..  
+00031e70: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
+00031e80: 5f69 6e70 7574 5f6c 696d 6974 2871 7565  _input_limit(que
+00031e90: 7279 5f74 6578 742c 2073 656c 662e 696e  ry_text, self.in
+00031ea0: 7075 745f 6c69 6d69 7429 0d0a 0d0a 2020  put_limit)....  
+00031eb0: 2020 2020 2020 6e6f 745f 7570 6461 7465        not_update
+00031ec0: 5f63 6f6e 645f 6672 6571 203d 2031 2069  _cond_freq = 1 i
+00031ed0: 6620 7365 6c66 2e71 7565 7279 5f63 6f75  f self.query_cou
+00031ee0: 6e74 203c 2075 7064 6174 655f 7365 7373  nt < update_sess
+00031ef0: 696f 6e5f 6166 7465 725f 6672 6571 2065  ion_after_freq e
+00031f00: 6c73 6520 300d 0a20 2020 2020 2020 206e  lse 0..        n
+00031f10: 6f74 5f75 7064 6174 655f 636f 6e64 5f74  ot_update_cond_t
+00031f20: 696d 6520 3d20 3120 6966 2074 696d 652e  ime = 1 if time.
+00031f30: 7469 6d65 2829 202d 2073 656c 662e 6265  time() - self.be
+00031f40: 6769 6e5f 7469 6d65 203c 2075 7064 6174  gin_time < updat
+00031f50: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
+00031f60: 7365 636f 6e64 7320 656c 7365 2030 0d0a  seconds else 0..
+00031f70: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
+00031f80: 7365 6c66 2e73 6573 7369 6f6e 2061 6e64  self.session and
+00031f90: 2073 656c 662e 6c61 6e67 7561 6765 5f6d   self.language_m
+00031fa0: 6170 2061 6e64 206e 6f74 5f75 7064 6174  ap and not_updat
+00031fb0: 655f 636f 6e64 5f66 7265 7120 616e 6420  e_cond_freq and 
+00031fc0: 6e6f 745f 7570 6461 7465 5f63 6f6e 645f  not_update_cond_
+00031fd0: 7469 6d65 2061 6e64 2073 656c 662e 7472  time and self.tr
+00031fe0: 616e 5f6b 6579 293a 0d0a 2020 2020 2020  an_key):..      
+00031ff0: 2020 2020 2020 7365 6c66 2e73 6573 7369        self.sessi
+00032000: 6f6e 203d 2072 6571 7565 7374 732e 5365  on = requests.Se
+00032010: 7373 696f 6e28 290d 0a20 2020 2020 2020  ssion()..       
+00032020: 2020 2020 2023 205f 203d 2073 656c 662e       # _ = self.
+00032030: 7365 7373 696f 6e2e 6765 7428 7365 6c66  session.get(self
+00032040: 2e68 6f6d 655f 7572 6c2c 2068 6561 6465  .home_url, heade
+00032050: 7273 3d73 656c 662e 686f 7374 5f68 6561  rs=self.host_hea
+00032060: 6465 7273 2c20 7469 6d65 6f75 743d 7469  ders, timeout=ti
+00032070: 6d65 6f75 742c 2070 726f 7869 6573 3d70  meout, proxies=p
+00032080: 726f 7869 6573 290d 0a20 2020 2020 2020  roxies)..       
+00032090: 2020 2020 2068 6f73 745f 6874 6d6c 203d       host_html =
+000320a0: 2073 656c 662e 7365 7373 696f 6e2e 6765   self.session.ge
+000320b0: 7428 7365 6c66 2e68 6f73 745f 7572 6c2c  t(self.host_url,
+000320c0: 2068 6561 6465 7273 3d73 656c 662e 686f   headers=self.ho
+000320d0: 7374 5f68 6561 6465 7273 2c20 7469 6d65  st_headers, time
+000320e0: 6f75 743d 7469 6d65 6f75 742c 2070 726f  out=timeout, pro
+000320f0: 7869 6573 3d70 726f 7869 6573 292e 7465  xies=proxies).te
+00032100: 7874 0d0a 2020 2020 2020 2020 2020 2020  xt..            
+00032110: 7365 6c66 2e74 7261 6e5f 6b65 7920 3d20  self.tran_key = 
+00032120: 7265 2e63 6f6d 7069 6c65 2827 7661 7220  re.compile('var 
+00032130: 7472 616e 203d 2022 282e 2a3f 2922 3b27  tran = "(.*?)";'
+00032140: 292e 7365 6172 6368 2868 6f73 745f 6874  ).search(host_ht
+00032150: 6d6c 292e 6772 6f75 7028 3129 0d0a 2020  ml).group(1)..  
+00032160: 2020 2020 2020 2020 2020 6c61 6e67 5f75            lang_u
+00032170: 726c 5f70 6172 7420 3d20 7265 2e63 6f6d  rl_part = re.com
+00032180: 7069 6c65 2873 656c 662e 6c61 6e67 5f75  pile(self.lang_u
+00032190: 726c 5f70 6174 7465 726e 292e 7365 6172  rl_pattern).sear
+000321a0: 6368 2868 6f73 745f 6874 6d6c 292e 6772  ch(host_html).gr
+000321b0: 6f75 7028 290d 0a20 2020 2020 2020 2020  oup()..         
+000321c0: 2020 2073 656c 662e 6c61 6e67 5f75 726c     self.lang_url
+000321d0: 203d 2066 2768 7474 7073 3a2f 2f6d 6972   = f'https://mir
+000321e0: 6169 7472 616e 736c 6174 652e 636f 6d2f  aitranslate.com/
+000321f0: 7472 6961 6c2f 696e 6d74 2f7b 6c61 6e67  trial/inmt/{lang
+00032200: 5f75 726c 5f70 6172 747d 270d 0a20 2020  _url_part}'..   
+00032210: 2020 2020 2020 2020 2064 6562 7567 5f6c           debug_l
+00032220: 616e 675f 6b77 6172 6773 203d 2073 656c  ang_kwargs = sel
+00032230: 662e 6465 6275 675f 6c61 6e67 5f6b 7761  f.debug_lang_kwa
+00032240: 7267 7328 6672 6f6d 5f6c 616e 6775 6167  rgs(from_languag
+00032250: 652c 2074 6f5f 6c61 6e67 7561 6765 2c20  e, to_language, 
+00032260: 7365 6c66 2e64 6566 6175 6c74 5f66 726f  self.default_fro
+00032270: 6d5f 6c61 6e67 7561 6765 2c20 6966 5f70  m_language, if_p
+00032280: 7269 6e74 5f77 6172 6e69 6e67 290d 0a20  rint_warning).. 
+00032290: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000322a0: 6c61 6e67 7561 6765 5f6d 6170 203d 2073  language_map = s
+000322b0: 656c 662e 6765 745f 6c61 6e67 7561 6765  elf.get_language
+000322c0: 5f6d 6170 2873 656c 662e 6c61 6e67 5f75  _map(self.lang_u
+000322d0: 726c 2c20 7365 6c66 2e73 6573 7369 6f6e  rl, self.session
+000322e0: 2c20 7365 6c66 2e61 7069 5f6a 736f 6e5f  , self.api_json_
+000322f0: 6865 6164 6572 732c 2074 696d 656f 7574  headers, timeout
+00032300: 2c20 7072 6f78 6965 732c 202a 2a64 6562  , proxies, **deb
+00032310: 7567 5f6c 616e 675f 6b77 6172 6773 290d  ug_lang_kwargs).
+00032320: 0a0d 0a20 2020 2020 2020 2069 6620 6672  ...        if fr
+00032330: 6f6d 5f6c 616e 6775 6167 6520 3d3d 2027  om_language == '
+00032340: 6175 746f 273a 0d0a 2020 2020 2020 2020  auto':..        
+00032350: 2020 2020 7220 3d20 7365 6c66 2e73 6573      r = self.ses
+00032360: 7369 6f6e 2e70 6f73 7428 7365 6c66 2e64  sion.post(self.d
+00032370: 6574 6563 745f 6c61 6e67 5f75 726c 2c20  etect_lang_url, 
+00032380: 6865 6164 6572 733d 7365 6c66 2e61 7069  headers=self.api
+00032390: 5f6a 736f 6e5f 6865 6164 6572 732c 206a  _json_headers, j
+000323a0: 736f 6e3d 7b27 7465 7874 273a 2071 7565  son={'text': que
+000323b0: 7279 5f74 6578 747d 2c20 7469 6d65 6f75  ry_text}, timeou
+000323c0: 743d 7469 6d65 6f75 742c 2070 726f 7869  t=timeout, proxi
+000323d0: 6573 3d70 726f 7869 6573 290d 0a20 2020  es=proxies)..   
+000323e0: 2020 2020 2020 2020 2066 726f 6d5f 6c61           from_la
+000323f0: 6e67 7561 6765 203d 2072 2e6a 736f 6e28  nguage = r.json(
+00032400: 295b 276c 616e 6775 6167 6527 5d0d 0a20  )['language'].. 
+00032410: 2020 2020 2020 2020 2020 2066 726f 6d5f             from_
+00032420: 6c61 6e67 7561 6765 203d 2073 656c 662e  language = self.
+00032430: 6c61 6e67 5f7a 685f 6d61 705b 6672 6f6d  lang_zh_map[from
+00032440: 5f6c 616e 6775 6167 655d 2069 6620 277a  _language] if 'z
+00032450: 6827 2069 6e20 6672 6f6d 5f6c 616e 6775  h' in from_langu
+00032460: 6167 6520 656c 7365 2066 726f 6d5f 6c61  age else from_la
+00032470: 6e67 7561 6765 0d0a 2020 2020 2020 2020  nguage..        
+00032480: 6672 6f6d 5f6c 616e 6775 6167 652c 2074  from_language, t
+00032490: 6f5f 6c61 6e67 7561 6765 203d 2073 656c  o_language = sel
+000324a0: 662e 6368 6563 6b5f 6c61 6e67 7561 6765  f.check_language
+000324b0: 2866 726f 6d5f 6c61 6e67 7561 6765 2c20  (from_language, 
+000324c0: 746f 5f6c 616e 6775 6167 652c 2073 656c  to_language, sel
+000324d0: 662e 6c61 6e67 7561 6765 5f6d 6170 2c20  f.language_map, 
+000324e0: 6f75 7470 7574 5f7a 683d 7365 6c66 2e6f  output_zh=self.o
+000324f0: 7574 7075 745f 7a68 290d 0a0d 0a20 2020  utput_zh)....   
+00032500: 2020 2020 2074 7261 6365 5f64 6174 6120       trace_data 
+00032510: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
+00032520: 2027 6f70 6572 6174 696f 6e54 7970 6527   'operationType'
+00032530: 3a20 2753 4c41 272c 0d0a 2020 2020 2020  : 'SLA',..      
+00032540: 2020 2020 2020 276c 616e 6727 3a20 6672        'lang': fr
+00032550: 6f6d 5f6c 616e 6775 6167 652c 0d0a 2020  om_language,..  
+00032560: 2020 2020 2020 2020 2020 2773 6f75 7263            'sourc
+00032570: 6527 3a20 7175 6572 795f 7465 7874 2c0d  e': query_text,.
+00032580: 0a20 2020 2020 2020 2020 2020 2027 7573  .            'us
+00032590: 6572 4964 273a 2073 656c 662e 7573 6572  erId': self.user
+000325a0: 5f69 642c 0d0a 2020 2020 2020 2020 2020  _id,..          
+000325b0: 2020 2774 7261 6e73 4964 273a 2073 656c    'transId': sel
+000325c0: 662e 7472 616e 735f 6964 2c0d 0a20 2020  f.trans_id,..   
+000325d0: 2020 2020 2020 2020 2027 756e 6971 7565           'unique
+000325e0: 4964 273a 2073 656c 662e 7472 616e 5f6b  Id': self.tran_k
+000325f0: 6579 2c0d 0a20 2020 2020 2020 2020 2020  ey,..           
+00032600: 2027 6461 7465 273a 2066 277b 6461 7465   'date': f'{date
+00032610: 7469 6d65 2e64 6174 6574 696d 652e 7574  time.datetime.ut
+00032620: 636e 6f77 2829 2e69 736f 666f 726d 6174  cnow().isoformat
+00032630: 2829 5b3a 2d33 5d7d 5a27 2c0d 0a20 2020  ()[:-3]}Z',..   
+00032640: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+00032650: 5f20 3d20 7365 6c66 2e73 6573 7369 6f6e  _ = self.session
+00032660: 2e70 6f73 7428 7365 6c66 2e74 7261 6365  .post(self.trace
+00032670: 5f75 726c 2c20 6a73 6f6e 3d74 7261 6365  _url, json=trace
+00032680: 5f64 6174 612c 2068 6561 6465 7273 3d73  _data, headers=s
+00032690: 656c 662e 6170 695f 7465 7874 5f68 6561  elf.api_text_hea
+000326a0: 6465 7273 2c20 7469 6d65 6f75 743d 7469  ders, timeout=ti
+000326b0: 6d65 6f75 742c 2070 726f 7869 6573 3d70  meout, proxies=p
+000326c0: 726f 7869 6573 290d 0a0d 0a20 2020 2020  roxies)....     
+000326d0: 2020 2070 6179 6c6f 6164 203d 207b 0d0a     payload = {..
+000326e0: 2020 2020 2020 2020 2020 2020 2769 6e70              'inp
+000326f0: 7574 273a 2071 7565 7279 5f74 6578 742c  ut': query_text,
+00032700: 0d0a 2020 2020 2020 2020 2020 2020 2773  ..            's
+00032710: 6f75 7263 6527 3a20 6672 6f6d 5f6c 616e  ource': from_lan
+00032720: 6775 6167 652c 0d0a 2020 2020 2020 2020  guage,..        
+00032730: 2020 2020 2774 6172 6765 7427 3a20 746f      'target': to
+00032740: 5f6c 616e 6775 6167 652c 0d0a 2020 2020  _language,..    
+00032750: 2020 2020 2020 2020 2774 7261 6e27 3a20          'tran': 
+00032760: 7365 6c66 2e74 7261 6e5f 6b65 792c 0d0a  self.tran_key,..
+00032770: 2020 2020 2020 2020 2020 2020 2761 6461              'ada
+00032780: 7074 5068 7261 7365 7327 3a20 5b5d 2c0d  ptPhrases': [],.
+00032790: 0a20 2020 2020 2020 2020 2020 2027 6669  .            'fi
+000327a0: 6c74 6572 5f70 726f 6669 6c65 273a 2027  lter_profile': '
+000327b0: 6e6d 7427 2c0d 0a20 2020 2020 2020 2020  nmt',..         
+000327c0: 2020 2027 7072 6f66 696c 6527 3a20 2769     'profile': 'i
+000327d0: 6e6d 7427 2c0d 0a20 2020 2020 2020 2020  nmt',..         
+000327e0: 2020 2027 7573 6550 7265 6669 7827 3a20     'usePrefix': 
+000327f0: 2766 616c 7365 272c 0d0a 2020 2020 2020  'false',..      
+00032800: 2020 2020 2020 277a 7427 3a20 2774 7275        'zt': 'tru
+00032810: 6527 2069 6620 277a 7427 2069 6e20 2866  e' if 'zt' in (f
+00032820: 726f 6d5f 6c61 6e67 7561 6765 2c20 746f  rom_language, to
+00032830: 5f6c 616e 6775 6167 6529 2065 6c73 6520  _language) else 
+00032840: 2766 616c 7365 272c 0d0a 2020 2020 2020  'false',..      
+00032850: 2020 2020 2020 2749 6e6d 7454 6172 6765        'InmtTarge
+00032860: 7427 3a20 2727 2c0d 0a20 2020 2020 2020  t': '',..       
+00032870: 2020 2020 2027 496e 6d74 5472 616e 736c       'InmtTransl
+00032880: 6174 6554 7970 6527 3a20 2767 6973 7469  ateType': 'gisti
+00032890: 6e67 272c 0d0a 2020 2020 2020 2020 7d0d  ng',..        }.
+000328a0: 0a20 2020 2020 2020 2072 203d 2073 656c  .        r = sel
+000328b0: 662e 7365 7373 696f 6e2e 706f 7374 2873  f.session.post(s
+000328c0: 656c 662e 6170 695f 7572 6c2c 2064 6174  elf.api_url, dat
+000328d0: 613d 7061 796c 6f61 642c 2068 6561 6465  a=payload, heade
+000328e0: 7273 3d73 656c 662e 6170 695f 7465 7874  rs=self.api_text
+000328f0: 5f68 6561 6465 7273 2c20 7469 6d65 6f75  _headers, timeou
+00032900: 743d 7469 6d65 6f75 742c 2070 726f 7869  t=timeout, proxi
+00032910: 6573 3d70 726f 7869 6573 290d 0a20 2020  es=proxies)..   
+00032920: 2020 2020 2072 2e72 6169 7365 5f66 6f72       r.raise_for
+00032930: 5f73 7461 7475 7328 290d 0a20 2020 2020  _status()..     
+00032940: 2020 2064 6174 6120 3d20 722e 6a73 6f6e     data = r.json
+00032950: 2829 0d0a 2020 2020 2020 2020 7469 6d65  ()..        time
+00032960: 2e73 6c65 6570 2873 6c65 6570 5f73 6563  .sleep(sleep_sec
+00032970: 6f6e 6473 290d 0a20 2020 2020 2020 2073  onds)..        s
+00032980: 656c 662e 7175 6572 795f 636f 756e 7420  elf.query_count 
+00032990: 2b3d 2031 0d0a 2020 2020 2020 2020 7265  += 1..        re
+000329a0: 7475 726e 2064 6174 6120 6966 2069 735f  turn data if is_
+000329b0: 6465 7461 696c 5f72 6573 756c 7420 656c  detail_result el
+000329c0: 7365 2064 6174 615b 276f 7570 7574 7327  se data['ouputs'
+000329d0: 5d5b 305d 5b27 6f75 7470 7574 275d 5b30  ][0]['output'][0
+000329e0: 5d5b 2774 7261 6e73 6c61 7469 6f6e 275d  ]['translation']
+000329f0: 0d0a 0d0a 0d0a 636c 6173 7320 4170 6572  ......class Aper
+00032a00: 7469 756d 2854 7365 293a 0d0a 2020 2020  tium(Tse):..    
+00032a10: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00032a20: 6629 3a0d 0a20 2020 2020 2020 2073 7570  f):..        sup
+00032a30: 6572 2829 2e5f 5f69 6e69 745f 5f28 290d  er().__init__().
+00032a40: 0a20 2020 2020 2020 2073 656c 662e 686f  .        self.ho
+00032a50: 7374 5f75 726c 203d 2027 6874 7470 733a  st_url = 'https:
+00032a60: 2f2f 7777 772e 6170 6572 7469 756d 2e6f  //www.apertium.o
+00032a70: 7267 2f27 0d0a 2020 2020 2020 2020 7365  rg/'..        se
+00032a80: 6c66 2e61 7069 5f75 726c 203d 2027 6874  lf.api_url = 'ht
+00032a90: 7470 733a 2f2f 6170 6572 7469 756d 2e6f  tps://apertium.o
+00032aa0: 7267 2f61 7079 2f74 7261 6e73 6c61 7465  rg/apy/translate
+00032ab0: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+00032ac0: 6765 745f 6c61 6e67 5f75 726c 203d 2027  get_lang_url = '
+00032ad0: 6874 7470 733a 2f2f 7777 772e 6170 6572  https://www.aper
+00032ae0: 7469 756d 2e6f 7267 2f69 6e64 6578 2e6a  tium.org/index.j
+00032af0: 7327 0d0a 2020 2020 2020 2020 7365 6c66  s'..        self
+00032b00: 2e64 6574 6563 745f 6c61 6e67 5f75 726c  .detect_lang_url
+00032b10: 203d 2027 6874 7470 733a 2f2f 6170 6572   = 'https://aper
+00032b20: 7469 756d 2e6f 7267 2f61 7079 2f69 6465  tium.org/apy/ide
+00032b30: 6e74 6966 794c 616e 6727 0d0a 2020 2020  ntifyLang'..    
+00032b40: 2020 2020 7365 6c66 2e68 6f73 745f 6865      self.host_he
+00032b50: 6164 6572 7320 3d20 7365 6c66 2e67 6574  aders = self.get
+00032b60: 5f68 6561 6465 7273 2873 656c 662e 686f  _headers(self.ho
+00032b70: 7374 5f75 726c 2c20 6966 5f61 7069 3d46  st_url, if_api=F
+00032b80: 616c 7365 2c20 6966 5f72 6566 6572 6572  alse, if_referer
+00032b90: 5f66 6f72 5f68 6f73 743d 5472 7565 290d  _for_host=True).
+00032ba0: 0a20 2020 2020 2020 2073 656c 662e 6170  .        self.ap
+00032bb0: 695f 6865 6164 6572 7320 3d20 7365 6c66  i_headers = self
+00032bc0: 2e67 6574 5f68 6561 6465 7273 2873 656c  .get_headers(sel
+00032bd0: 662e 686f 7374 5f75 726c 2c20 6966 5f61  f.host_url, if_a
+00032be0: 7069 3d54 7275 6529 0d0a 2020 2020 2020  pi=True)..      
+00032bf0: 2020 7365 6c66 2e73 6573 7369 6f6e 203d    self.session =
+00032c00: 204e 6f6e 650d 0a20 2020 2020 2020 2073   None..        s
+00032c10: 656c 662e 6c61 6e67 7561 6765 5f6d 6170  elf.language_map
+00032c20: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
+00032c30: 2073 656c 662e 7175 6572 795f 636f 756e   self.query_coun
+00032c40: 7420 3d20 300d 0a20 2020 2020 2020 2073  t = 0..        s
+00032c50: 656c 662e 6f75 7470 7574 5f7a 6820 3d20  elf.output_zh = 
+00032c60: 4e6f 6e65 2020 2320 756e 7375 7070 6f72  None  # unsuppor
+00032c70: 7465 640d 0a20 2020 2020 2020 2073 656c  ted..        sel
+00032c80: 662e 6f75 7470 7574 5f65 6e20 3d20 2765  f.output_en = 'e
+00032c90: 6e67 270d 0a20 2020 2020 2020 2073 656c  ng'..        sel
+00032ca0: 662e 696e 7075 745f 6c69 6d69 7420 3d20  f.input_limit = 
+00032cb0: 696e 7428 3165 3429 2020 2320 616c 6d6f  int(1e4)  # almo
+00032cc0: 7374 206e 6f20 6c69 6d69 742e 0d0a 2020  st no limit...  
+00032cd0: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
+00032ce0: 6c74 5f66 726f 6d5f 6c61 6e67 7561 6765  lt_from_language
+00032cf0: 203d 2027 7370 6127 0d0a 0d0a 2020 2020   = 'spa'....    
+00032d00: 4054 7365 2e64 6562 7567 5f6c 616e 6775  @Tse.debug_langu
+00032d10: 6167 655f 6d61 700d 0a20 2020 2064 6566  age_map..    def
+00032d20: 2067 6574 5f6c 616e 6775 6167 655f 6d61   get_language_ma
+00032d30: 7028 7365 6c66 2c20 6c61 6e67 5f75 726c  p(self, lang_url
+00032d40: 3a20 7374 722c 2073 733a 2053 6573 7369  : str, ss: Sessi
+00032d50: 6f6e 5479 7065 2c20 6865 6164 6572 733a  onType, headers:
+00032d60: 2064 6963 742c 2074 696d 656f 7574 3a20   dict, timeout: 
+00032d70: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d2c  Optional[float],
+00032d80: 2070 726f 7869 6573 3a20 4f70 7469 6f6e   proxies: Option
+00032d90: 616c 5b64 6963 745d 2c20 2a2a 6b77 6172  al[dict], **kwar
+00032da0: 6773 3a20 4c61 6e67 4d61 704b 7761 7267  gs: LangMapKwarg
+00032db0: 7354 7970 6529 202d 3e20 6469 6374 3a0d  sType) -> dict:.
+00032dc0: 0a20 2020 2020 2020 206a 735f 6874 6d6c  .        js_html
+00032dd0: 203d 2073 732e 6765 7428 6c61 6e67 5f75   = ss.get(lang_u
+00032de0: 726c 2c20 6865 6164 6572 733d 6865 6164  rl, headers=head
+00032df0: 6572 732c 2074 696d 656f 7574 3d74 696d  ers, timeout=tim
+00032e00: 656f 7574 2c20 7072 6f78 6965 733d 7072  eout, proxies=pr
+00032e10: 6f78 6965 7329 2e74 6578 740d 0a20 2020  oxies).text..   
+00032e20: 2020 2020 206c 616e 675f 7061 6972 7320       lang_pairs 
+00032e30: 3d20 7265 2e63 6f6d 7069 6c65 2827 7b73  = re.compile('{s
+00032e40: 6f75 7263 654c 616e 6775 6167 653a 2228  ourceLanguage:"(
+00032e50: 2e2a 3f29 222c 7461 7267 6574 4c61 6e67  .*?)",targetLang
+00032e60: 7561 6765 3a22 282e 2a3f 2922 7d27 292e  uage:"(.*?)"}').
+00032e70: 6669 6e64 616c 6c28 6a73 5f68 746d 6c29  findall(js_html)
+00032e80: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00032e90: 207b 665f 6c61 6e67 3a20 5b76 2066 6f72   {f_lang: [v for
+00032ea0: 206b 2c20 7620 696e 206c 616e 675f 7061   k, v in lang_pa
+00032eb0: 6972 7320 6966 206b 203d 3d20 665f 6c61  irs if k == f_la
+00032ec0: 6e67 5d20 666f 7220 665f 6c61 6e67 2c20  ng] for f_lang, 
+00032ed0: 745f 6c61 6e67 2069 6e20 6c61 6e67 5f70  t_lang in lang_p
+00032ee0: 6169 7273 7d0d 0a0d 0a20 2020 2040 5473  airs}....    @Ts
+00032ef0: 652e 7469 6d65 5f73 7461 740d 0a20 2020  e.time_stat..   
+00032f00: 2040 5473 652e 6368 6563 6b5f 7175 6572   @Tse.check_quer
+00032f10: 790d 0a20 2020 2064 6566 2061 7065 7274  y..    def apert
+00032f20: 6975 6d5f 6170 6928 7365 6c66 2c20 7175  ium_api(self, qu
+00032f30: 6572 795f 7465 7874 3a20 7374 722c 2066  ery_text: str, f
+00032f40: 726f 6d5f 6c61 6e67 7561 6765 3a20 7374  rom_language: st
+00032f50: 7220 3d20 2761 7574 6f27 2c20 746f 5f6c  r = 'auto', to_l
+00032f60: 616e 6775 6167 653a 2073 7472 203d 2027  anguage: str = '
+00032f70: 656e 272c 202a 2a6b 7761 7267 733a 2041  en', **kwargs: A
+00032f80: 7069 4b77 6172 6773 5479 7065 2920 2d3e  piKwargsType) ->
+00032f90: 2055 6e69 6f6e 5b73 7472 2c20 6469 6374   Union[str, dict
+00032fa0: 5d3a 0d0a 2020 2020 2020 2020 2222 220d  ]:..        """.
+00032fb0: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
+00032fc0: 2f77 7777 2e61 7065 7274 6975 6d2e 6f72  /www.apertium.or
+00032fd0: 672f 0d0a 2020 2020 2020 2020 3a70 6172  g/..        :par
+00032fe0: 616d 2071 7565 7279 5f74 6578 743a 2073  am query_text: s
+00032ff0: 7472 2c20 6d75 7374 2e0d 0a20 2020 2020  tr, must...     
+00033000: 2020 203a 7061 7261 6d20 6672 6f6d 5f6c     :param from_l
+00033010: 616e 6775 6167 653a 2073 7472 2c20 6465  anguage: str, de
+00033020: 6661 756c 7420 2761 7574 6f27 2e0d 0a20  fault 'auto'... 
+00033030: 2020 2020 2020 203a 7061 7261 6d20 746f         :param to
+00033040: 5f6c 616e 6775 6167 653a 2073 7472 2c20  _language: str, 
+00033050: 6465 6661 756c 7420 2765 6e27 2e0d 0a20  default 'en'... 
+00033060: 2020 2020 2020 203a 7061 7261 6d20 2a2a         :param **
+00033070: 6b77 6172 6773 3a0d 0a20 2020 2020 2020  kwargs:..       
+00033080: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00033090: 7469 6d65 6f75 743a 2066 6c6f 6174 2c20  timeout: float, 
+000330a0: 6465 6661 756c 7420 4e6f 6e65 2e0d 0a20  default None... 
+000330b0: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+000330c0: 7061 7261 6d20 7072 6f78 6965 733a 2064  param proxies: d
+000330d0: 6963 742c 2064 6566 6175 6c74 204e 6f6e  ict, default Non
+000330e0: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
+000330f0: 2020 2020 3a70 6172 616d 2073 6c65 6570      :param sleep
+00033100: 5f73 6563 6f6e 6473 3a20 666c 6f61 742c  _seconds: float,
+00033110: 2064 6566 6175 6c74 2030 2e0d 0a20 2020   default 0...   
+00033120: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+00033130: 7261 6d20 6973 5f64 6574 6169 6c5f 7265  ram is_detail_re
+00033140: 7375 6c74 3a20 626f 6f6c 2c20 6465 6661  sult: bool, defa
+00033150: 756c 7420 4661 6c73 652e 0d0a 2020 2020  ult False...    
+00033160: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00033170: 616d 2069 665f 6967 6e6f 7265 5f6c 696d  am if_ignore_lim
+00033180: 6974 5f6f 665f 6c65 6e67 7468 3a20 626f  it_of_length: bo
+00033190: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
+000331a0: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
+000331b0: 2020 2020 3a70 6172 616d 206c 696d 6974      :param limit
+000331c0: 5f6f 665f 6c65 6e67 7468 3a20 696e 742c  _of_length: int,
+000331d0: 2064 6566 6175 6c74 2032 3030 3030 2e0d   default 20000..
+000331e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000331f0: 203a 7061 7261 6d20 6966 5f69 676e 6f72   :param if_ignor
+00033200: 655f 656d 7074 795f 7175 6572 793a 2062  e_empty_query: b
+00033210: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+00033220: 7365 2e0d 0a20 2020 2020 2020 2020 2020  se...           
+00033230: 2020 2020 203a 7061 7261 6d20 7570 6461       :param upda
+00033240: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
+00033250: 5f66 7265 713a 2069 6e74 2c20 6465 6661  _freq: int, defa
+00033260: 756c 7420 3130 3030 2e0d 0a20 2020 2020  ult 1000...     
+00033270: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00033280: 6d20 7570 6461 7465 5f73 6573 7369 6f6e  m update_session
+00033290: 5f61 6674 6572 5f73 6563 6f6e 6473 3a20  _after_seconds: 
+000332a0: 666c 6f61 742c 2064 6566 6175 6c74 2031  float, default 1
+000332b0: 3530 302e 0d0a 2020 2020 2020 2020 2020  500...          
+000332c0: 2020 2020 2020 3a70 6172 616d 2069 665f        :param if_
+000332d0: 7368 6f77 5f74 696d 655f 7374 6174 3a20  show_time_stat: 
+000332e0: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+000332f0: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
+00033300: 2020 2020 2020 3a70 6172 616d 2073 686f        :param sho
+00033310: 775f 7469 6d65 5f73 7461 745f 7072 6563  w_time_stat_prec
+00033320: 6973 696f 6e3a 2069 6e74 2c20 6465 6661  ision: int, defa
+00033330: 756c 7420 322e 0d0a 2020 2020 2020 2020  ult 2...        
+00033340: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+00033350: 665f 7072 696e 745f 7761 726e 696e 673a  f_print_warning:
+00033360: 2062 6f6f 6c2c 2064 6566 6175 6c74 2054   bool, default T
+00033370: 7275 652e 0d0a 2020 2020 2020 2020 3a72  rue...        :r
+00033380: 6574 7572 6e3a 2073 7472 206f 7220 6469  eturn: str or di
+00033390: 6374 0d0a 2020 2020 2020 2020 2222 220d  ct..        """.
+000333a0: 0a0d 0a20 2020 2020 2020 2074 696d 656f  ...        timeo
+000333b0: 7574 203d 206b 7761 7267 732e 6765 7428  ut = kwargs.get(
+000333c0: 2774 696d 656f 7574 272c 204e 6f6e 6529  'timeout', None)
+000333d0: 0d0a 2020 2020 2020 2020 7072 6f78 6965  ..        proxie
+000333e0: 7320 3d20 6b77 6172 6773 2e67 6574 2827  s = kwargs.get('
+000333f0: 7072 6f78 6965 7327 2c20 4e6f 6e65 290d  proxies', None).
+00033400: 0a20 2020 2020 2020 2073 6c65 6570 5f73  .        sleep_s
+00033410: 6563 6f6e 6473 203d 206b 7761 7267 732e  econds = kwargs.
+00033420: 6765 7428 2773 6c65 6570 5f73 6563 6f6e  get('sleep_secon
+00033430: 6473 272c 2030 290d 0a20 2020 2020 2020  ds', 0)..       
+00033440: 2069 665f 7072 696e 745f 7761 726e 696e   if_print_warnin
+00033450: 6720 3d20 6b77 6172 6773 2e67 6574 2827  g = kwargs.get('
+00033460: 6966 5f70 7269 6e74 5f77 6172 6e69 6e67  if_print_warning
+00033470: 272c 2054 7275 6529 0d0a 2020 2020 2020  ', True)..      
+00033480: 2020 6973 5f64 6574 6169 6c5f 7265 7375    is_detail_resu
+00033490: 6c74 203d 206b 7761 7267 732e 6765 7428  lt = kwargs.get(
+000334a0: 2769 735f 6465 7461 696c 5f72 6573 756c  'is_detail_resul
+000334b0: 7427 2c20 4661 6c73 6529 0d0a 2020 2020  t', False)..    
+000334c0: 2020 2020 7570 6461 7465 5f73 6573 7369      update_sessi
+000334d0: 6f6e 5f61 6674 6572 5f66 7265 7120 3d20  on_after_freq = 
+000334e0: 6b77 6172 6773 2e67 6574 2827 7570 6461  kwargs.get('upda
+000334f0: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
+00033500: 5f66 7265 7127 2c20 7365 6c66 2e64 6566  _freq', self.def
+00033510: 6175 6c74 5f73 6573 7369 6f6e 5f66 7265  ault_session_fre
+00033520: 7129 0d0a 2020 2020 2020 2020 7570 6461  q)..        upda
+00033530: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
+00033540: 5f73 6563 6f6e 6473 203d 206b 7761 7267  _seconds = kwarg
+00033550: 732e 6765 7428 2775 7064 6174 655f 7365  s.get('update_se
+00033560: 7373 696f 6e5f 6166 7465 725f 7365 636f  ssion_after_seco
+00033570: 6e64 7327 2c20 7365 6c66 2e64 6566 6175  nds', self.defau
+00033580: 6c74 5f73 6573 7369 6f6e 5f73 6563 6f6e  lt_session_secon
+00033590: 6473 290d 0a20 2020 2020 2020 2073 656c  ds)..        sel
+000335a0: 662e 6368 6563 6b5f 696e 7075 745f 6c69  f.check_input_li
+000335b0: 6d69 7428 7175 6572 795f 7465 7874 2c20  mit(query_text, 
+000335c0: 7365 6c66 2e69 6e70 7574 5f6c 696d 6974  self.input_limit
+000335d0: 290d 0a0d 0a20 2020 2020 2020 206e 6f74  )....        not
+000335e0: 5f75 7064 6174 655f 636f 6e64 5f66 7265  _update_cond_fre
+000335f0: 7120 3d20 3120 6966 2073 656c 662e 7175  q = 1 if self.qu
+00033600: 6572 795f 636f 756e 7420 3c20 7570 6461  ery_count < upda
+00033610: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
+00033620: 5f66 7265 7120 656c 7365 2030 0d0a 2020  _freq else 0..  
+00033630: 2020 2020 2020 6e6f 745f 7570 6461 7465        not_update
+00033640: 5f63 6f6e 645f 7469 6d65 203d 2031 2069  _cond_time = 1 i
+00033650: 6620 7469 6d65 2e74 696d 6528 2920 2d20  f time.time() - 
+00033660: 7365 6c66 2e62 6567 696e 5f74 696d 6520  self.begin_time 
+00033670: 3c20 7570 6461 7465 5f73 6573 7369 6f6e  < update_session
+00033680: 5f61 6674 6572 5f73 6563 6f6e 6473 2065  _after_seconds e
+00033690: 6c73 6520 300d 0a20 2020 2020 2020 2069  lse 0..        i
+000336a0: 6620 6e6f 7420 2873 656c 662e 7365 7373  f not (self.sess
+000336b0: 696f 6e20 616e 6420 7365 6c66 2e6c 616e  ion and self.lan
+000336c0: 6775 6167 655f 6d61 7020 616e 6420 6e6f  guage_map and no
+000336d0: 745f 7570 6461 7465 5f63 6f6e 645f 6672  t_update_cond_fr
+000336e0: 6571 2061 6e64 206e 6f74 5f75 7064 6174  eq and not_updat
+000336f0: 655f 636f 6e64 5f74 696d 6529 3a0d 0a20  e_cond_time):.. 
+00033700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00033710: 7365 7373 696f 6e20 3d20 7265 7175 6573  session = reques
+00033720: 7473 2e53 6573 7369 6f6e 2829 0d0a 2020  ts.Session()..  
+00033730: 2020 2020 2020 2020 2020 5f20 3d20 7365            _ = se
+00033740: 6c66 2e73 6573 7369 6f6e 2e67 6574 2873  lf.session.get(s
+00033750: 656c 662e 686f 7374 5f75 726c 2c20 6865  elf.host_url, he
+00033760: 6164 6572 733d 7365 6c66 2e68 6f73 745f  aders=self.host_
+00033770: 6865 6164 6572 732c 2074 696d 656f 7574  headers, timeout
+00033780: 3d74 696d 656f 7574 2c20 7072 6f78 6965  =timeout, proxie
+00033790: 733d 7072 6f78 6965 7329 0d0a 2020 2020  s=proxies)..    
+000337a0: 2020 2020 2020 2020 6465 6275 675f 6c61          debug_la
+000337b0: 6e67 5f6b 7761 7267 7320 3d20 7365 6c66  ng_kwargs = self
+000337c0: 2e64 6562 7567 5f6c 616e 675f 6b77 6172  .debug_lang_kwar
+000337d0: 6773 2866 726f 6d5f 6c61 6e67 7561 6765  gs(from_language
+000337e0: 2c20 746f 5f6c 616e 6775 6167 652c 2073  , to_language, s
+000337f0: 656c 662e 6465 6661 756c 745f 6672 6f6d  elf.default_from
+00033800: 5f6c 616e 6775 6167 652c 2069 665f 7072  _language, if_pr
+00033810: 696e 745f 7761 726e 696e 6729 0d0a 2020  int_warning)..  
+00033820: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00033830: 616e 6775 6167 655f 6d61 7020 3d20 7365  anguage_map = se
+00033840: 6c66 2e67 6574 5f6c 616e 6775 6167 655f  lf.get_language_
+00033850: 6d61 7028 7365 6c66 2e67 6574 5f6c 616e  map(self.get_lan
+00033860: 675f 7572 6c2c 2073 656c 662e 7365 7373  g_url, self.sess
+00033870: 696f 6e2c 2073 656c 662e 686f 7374 5f68  ion, self.host_h
+00033880: 6561 6465 7273 2c20 7469 6d65 6f75 742c  eaders, timeout,
+00033890: 2070 726f 7869 6573 2c20 2a2a 6465 6275   proxies, **debu
+000338a0: 675f 6c61 6e67 5f6b 7761 7267 7329 0d0a  g_lang_kwargs)..
+000338b0: 0d0a 2020 2020 2020 2020 6966 2066 726f  ..        if fro
+000338c0: 6d5f 6c61 6e67 7561 6765 203d 3d20 2761  m_language == 'a
+000338d0: 7574 6f27 3a0d 0a20 2020 2020 2020 2020  uto':..         
+000338e0: 2020 2070 6179 6c6f 6164 203d 2075 726c     payload = url
+000338f0: 6c69 622e 7061 7273 652e 7572 6c65 6e63  lib.parse.urlenc
+00033900: 6f64 6528 7b27 7127 3a20 7175 6572 795f  ode({'q': query_
+00033910: 7465 7874 7d29 0d0a 2020 2020 2020 2020  text})..        
+00033920: 2020 2020 6c61 6e67 7320 3d20 7365 6c66      langs = self
+00033930: 2e73 6573 7369 6f6e 2e70 6f73 7428 7365  .session.post(se
+00033940: 6c66 2e64 6574 6563 745f 6c61 6e67 5f75  lf.detect_lang_u
+00033950: 726c 2c20 6461 7461 3d70 6179 6c6f 6164  rl, data=payload
+00033960: 2c20 6865 6164 6572 733d 7365 6c66 2e61  , headers=self.a
+00033970: 7069 5f68 6561 6465 7273 2c20 7469 6d65  pi_headers, time
+00033980: 6f75 743d 7469 6d65 6f75 742c 2070 726f  out=timeout, pro
+00033990: 7869 6573 3d70 726f 7869 6573 292e 6a73  xies=proxies).js
+000339a0: 6f6e 2829 0d0a 2020 2020 2020 2020 2020  on()..          
+000339b0: 2020 6672 6f6d 5f6c 616e 6775 6167 6520    from_language 
+000339c0: 3d20 736f 7274 6564 286c 616e 6773 2c20  = sorted(langs, 
+000339d0: 6b65 793d 6c61 6d62 6461 206b 3a20 6c61  key=lambda k: la
+000339e0: 6e67 735b 6b5d 2c20 7265 7665 7273 653d  ngs[k], reverse=
+000339f0: 5472 7565 295b 305d 0d0a 2020 2020 2020  True)[0]..      
+00033a00: 2020 6672 6f6d 5f6c 616e 6775 6167 652c    from_language,
+00033a10: 2074 6f5f 6c61 6e67 7561 6765 203d 2073   to_language = s
+00033a20: 656c 662e 6368 6563 6b5f 6c61 6e67 7561  elf.check_langua
+00033a30: 6765 2866 726f 6d5f 6c61 6e67 7561 6765  ge(from_language
+00033a40: 2c20 746f 5f6c 616e 6775 6167 652c 2073  , to_language, s
+00033a50: 656c 662e 6c61 6e67 7561 6765 5f6d 6170  elf.language_map
+00033a60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00033a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033a90: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00033aa0: 7574 5f65 6e5f 7472 616e 736c 6174 6f72  ut_en_translator
+00033ab0: 3d27 6170 6572 7469 756d 272c 206f 7574  ='apertium', out
+00033ac0: 7075 745f 656e 3d73 656c 662e 6f75 7470  put_en=self.outp
+00033ad0: 7574 5f65 6e29 0d0a 0d0a 2020 2020 2020  ut_en)....      
+00033ae0: 2020 7061 796c 6f61 6420 3d20 7b0d 0a20    payload = {.. 
+00033af0: 2020 2020 2020 2020 2020 2027 7127 3a20             'q': 
+00033b00: 7175 6572 795f 7465 7874 2c0d 0a20 2020  query_text,..   
+00033b10: 2020 2020 2020 2020 2027 6c61 6e67 7061           'langpa
+00033b20: 6972 273a 2066 277b 6672 6f6d 5f6c 616e  ir': f'{from_lan
+00033b30: 6775 6167 657d 7c7b 746f 5f6c 616e 6775  guage}|{to_langu
+00033b40: 6167 657d 272c 0d0a 2020 2020 2020 2020  age}',..        
+00033b50: 2020 2020 2770 7265 6673 273a 2027 272c      'prefs': '',
+00033b60: 0d0a 2020 2020 2020 2020 2020 2020 276d  ..            'm
+00033b70: 6172 6b55 6e6b 6e6f 776e 273a 2027 6e6f  arkUnknown': 'no
+00033b80: 272c 0d0a 2020 2020 2020 2020 7d0d 0a20  ',..        }.. 
+00033b90: 2020 2020 2020 2070 6179 6c6f 6164 203d         payload =
+00033ba0: 2075 726c 6c69 622e 7061 7273 652e 7572   urllib.parse.ur
+00033bb0: 6c65 6e63 6f64 6528 7061 796c 6f61 6429  lencode(payload)
+00033bc0: 0d0a 2020 2020 2020 2020 7220 3d20 7365  ..        r = se
+00033bd0: 6c66 2e73 6573 7369 6f6e 2e70 6f73 7428  lf.session.post(
+00033be0: 7365 6c66 2e61 7069 5f75 726c 2c20 6461  self.api_url, da
+00033bf0: 7461 3d70 6179 6c6f 6164 2c20 6865 6164  ta=payload, head
+00033c00: 6572 733d 7365 6c66 2e61 7069 5f68 6561  ers=self.api_hea
+00033c10: 6465 7273 2c20 7469 6d65 6f75 743d 7469  ders, timeout=ti
+00033c20: 6d65 6f75 742c 2070 726f 7869 6573 3d70  meout, proxies=p
+00033c30: 726f 7869 6573 290d 0a20 2020 2020 2020  roxies)..       
+00033c40: 2072 2e72 6169 7365 5f66 6f72 5f73 7461   r.raise_for_sta
+00033c50: 7475 7328 290d 0a20 2020 2020 2020 2064  tus()..        d
+00033c60: 6174 6120 3d20 722e 6a73 6f6e 2829 0d0a  ata = r.json()..
+00033c70: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
+00033c80: 6570 2873 6c65 6570 5f73 6563 6f6e 6473  ep(sleep_seconds
+00033c90: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00033ca0: 7175 6572 795f 636f 756e 7420 2b3d 2031  query_count += 1
+00033cb0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00033cc0: 2064 6174 6120 6966 2069 735f 6465 7461   data if is_deta
+00033cd0: 696c 5f72 6573 756c 7420 656c 7365 2064  il_result else d
+00033ce0: 6174 615b 2772 6573 706f 6e73 6544 6174  ata['responseDat
+00033cf0: 6127 5d5b 2774 7261 6e73 6c61 7465 6454  a']['translatedT
+00033d00: 6578 7427 5d0d 0a0d 0a0d 0a63 6c61 7373  ext']......class
+00033d10: 2054 696c 6465 2854 7365 293a 0d0a 2020   Tilde(Tse):..  
+00033d20: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00033d30: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
+00033d40: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+00033d50: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00033d60: 686f 7374 5f75 726c 203d 2027 6874 7470  host_url = 'http
+00033d70: 733a 2f2f 7472 616e 736c 6174 652e 7469  s://translate.ti
+00033d80: 6c64 652e 636f 6d2f 270d 0a20 2020 2020  lde.com/'..     
+00033d90: 2020 2073 656c 662e 6170 695f 7572 6c20     self.api_url 
+00033da0: 3d20 2768 7474 7073 3a2f 2f6c 6574 736d  = 'https://letsm
+00033db0: 742e 6575 2f77 732f 7365 7276 6963 652e  t.eu/ws/service.
+00033dc0: 7376 632f 6a73 6f6e 2f54 7261 6e73 6c61  svc/json/Transla
+00033dd0: 7465 4578 270d 0a20 2020 2020 2020 2073  teEx'..        s
+00033de0: 656c 662e 6765 745f 636f 6e66 6967 5f75  elf.get_config_u
+00033df0: 726c 203d 2027 6874 7470 733a 2f2f 7472  rl = 'https://tr
+00033e00: 616e 736c 6174 652e 7469 6c64 652e 636f  anslate.tilde.co
+00033e10: 6d2f 6173 7365 7473 2f63 6f6e 6669 672e  m/assets/config.
+00033e20: 6c6f 6361 6c2e 6a73 6f6e 2720 2023 203f  local.json'  # ?
+00033e30: 7665 7273 696f 6e3d 3436 3835 320d 0a20  version=46852.. 
+00033e40: 2020 2020 2020 2073 656c 662e 7375 6273         self.subs
+00033e50: 6372 6962 655f 7572 6c20 3d20 2768 7474  cribe_url = 'htt
+00033e60: 7073 3a2f 2f74 7261 6e73 6c61 7465 2e74  ps://translate.t
+00033e70: 696c 6465 2e63 6f6d 2f61 7373 6574 732f  ilde.com/assets/
+00033e80: 7375 6273 6372 6970 7469 6f6e 732d 636f  subscriptions-co
+00033e90: 6e66 6967 2e6c 6f63 616c 2e6a 736f 6e27  nfig.local.json'
+00033ea0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00033eb0: 6c61 7573 6962 6c65 5f75 726c 203d 2027  lausible_url = '
+00033ec0: 6874 7470 733a 2f2f 706c 6175 7369 626c  https://plausibl
+00033ed0: 652e 696f 2f61 7069 2f65 7665 6e74 270d  e.io/api/event'.
+00033ee0: 0a20 2020 2020 2020 2073 656c 662e 6175  .        self.au
+00033ef0: 7468 5f75 726c 203d 2027 6874 7470 733a  th_url = 'https:
+00033f00: 2f2f 6175 7468 2e74 696c 6465 2e63 6f6d  //auth.tilde.com
+00033f10: 2f61 7574 682f 7265 616c 6d73 2f54 696c  /auth/realms/Til
+00033f20: 6465 2f70 726f 746f 636f 6c2f 6f70 656e  de/protocol/open
+00033f30: 6964 2d63 6f6e 6e65 6374 2f6c 6f67 696e  id-connect/login
+00033f40: 2d73 7461 7475 732d 6966 7261 6d65 2e68  -status-iframe.h
+00033f50: 746d 6c2f 696e 6974 270d 0a20 2020 2020  tml/init'..     
+00033f60: 2020 2073 656c 662e 7370 6565 6368 5f75     self.speech_u
+00033f70: 726c 203d 2027 6874 7470 733a 2f2f 7661  rl = 'https://va
+00033f80: 2e74 696c 6465 2e63 6f6d 2f64 6c2f 6469  .tilde.com/dl/di
+00033f90: 7265 6374 6c69 6e65 2f61 4852 3063 446f  rectline/aHR0cDo
+00033fa0: 764c 3342 7962 3252 724f 484e 6962 3352  vL3Byb2RrOHNib3R
+00033fb0: 3061 5778 6b5a 5451 3d2f 746f 6b65 6e73  0aWxkZTQ=/tokens
+00033fc0: 2f73 7065 6563 6827 0d0a 2020 2020 2020  /speech'..      
+00033fd0: 2020 7365 6c66 2e68 6f73 745f 6865 6164    self.host_head
+00033fe0: 6572 7320 3d20 7365 6c66 2e67 6574 5f68  ers = self.get_h
+00033ff0: 6561 6465 7273 2873 656c 662e 686f 7374  eaders(self.host
+00034000: 5f75 726c 2c20 6966 5f61 7069 3d46 616c  _url, if_api=Fal
+00034010: 7365 2c20 6966 5f72 6566 6572 6572 5f66  se, if_referer_f
+00034020: 6f72 5f68 6f73 743d 5472 7565 290d 0a20  or_host=True).. 
+00034030: 2020 2020 2020 2073 656c 662e 6170 695f         self.api_
+00034040: 6865 6164 6572 7320 3d20 7365 6c66 2e67  headers = self.g
+00034050: 6574 5f68 6561 6465 7273 2873 656c 662e  et_headers(self.
+00034060: 686f 7374 5f75 726c 2c20 6966 5f61 7069  host_url, if_api
+00034070: 3d54 7275 652c 2069 665f 6a73 6f6e 5f66  =True, if_json_f
+00034080: 6f72 5f61 7069 3d54 7275 6529 0d0a 2020  or_api=True)..  
+00034090: 2020 2020 2020 7365 6c66 2e73 6573 7369        self.sessi
+000340a0: 6f6e 203d 204e 6f6e 650d 0a20 2020 2020  on = None..     
+000340b0: 2020 2073 656c 662e 6c61 6e67 7561 6765     self.language
+000340c0: 5f6d 6170 203d 204e 6f6e 650d 0a20 2020  _map = None..   
+000340d0: 2020 2020 2073 656c 662e 6c61 6e67 7061       self.langpa
+000340e0: 6972 5f69 6473 203d 204e 6f6e 650d 0a20  ir_ids = None.. 
+000340f0: 2020 2020 2020 2073 656c 662e 636f 6e66         self.conf
+00034100: 6967 5f64 6174 6120 3d20 4e6f 6e65 0d0a  ig_data = None..
+00034110: 2020 2020 2020 2020 7365 6c66 2e73 7973          self.sys
+00034120: 5f64 6174 6120 3d20 4e6f 6e65 0d0a 2020  _data = None..  
+00034130: 2020 2020 2020 7365 6c66 2e71 7565 7279        self.query
+00034140: 5f63 6f75 6e74 203d 2030 0d0a 2020 2020  _count = 0..    
+00034150: 2020 2020 7365 6c66 2e6f 7574 7075 745f      self.output_
+00034160: 7a68 203d 204e 6f6e 6520 2023 2075 6e73  zh = None  # uns
+00034170: 7570 706f 7274 6564 0d0a 2020 2020 2020  upported..      
+00034180: 2020 7365 6c66 2e6f 7574 7075 745f 656e    self.output_en
+00034190: 203d 2027 656e 6727 0d0a 2020 2020 2020   = 'eng'..      
+000341a0: 2020 7365 6c66 2e69 6e70 7574 5f6c 696d    self.input_lim
+000341b0: 6974 203d 2069 6e74 2835 6533 2920 2023  it = int(5e3)  #
+000341c0: 2075 6e6b 6e6f 776e 0d0a 2020 2020 2020   unknown..      
+000341d0: 2020 7365 6c66 2e64 6566 6175 6c74 5f66    self.default_f
+000341e0: 726f 6d5f 6c61 6e67 7561 6765 203d 2027  rom_language = '
+000341f0: 6c76 2720 2023 2027 6672 270d 0a0d 0a20  lv'  # 'fr'.... 
+00034200: 2020 2040 5473 652e 6465 6275 675f 6c61     @Tse.debug_la
+00034210: 6e67 7561 6765 5f6d 6170 0d0a 2020 2020  nguage_map..    
+00034220: 6465 6620 6765 745f 6c61 6e67 7561 6765  def get_language
+00034230: 5f6d 6170 2873 656c 662c 2073 7973 5f64  _map(self, sys_d
+00034240: 6174 613a 2064 6963 742c 202a 2a6b 7761  ata: dict, **kwa
+00034250: 7267 733a 204c 616e 674d 6170 4b77 6172  rgs: LangMapKwar
+00034260: 6773 5479 7065 2920 2d3e 2064 6963 743a  gsType) -> dict:
+00034270: 0d0a 2020 2020 2020 2020 6c61 6e67 5f70  ..        lang_p
+00034280: 6169 7273 203d 205b 5b69 7465 6d5b 2753  airs = [[item['S
+00034290: 6f75 7263 654c 616e 6775 6167 6527 5d5b  ourceLanguage'][
+000342a0: 2743 6f64 6527 5d2c 2069 7465 6d5b 2754  'Code'], item['T
+000342b0: 6172 6765 744c 616e 6775 6167 6527 5d5b  argetLanguage'][
+000342c0: 2743 6f64 6527 5d5d 2066 6f72 2069 7465  'Code']] for ite
+000342d0: 6d20 696e 2073 7973 5f64 6174 615b 2753  m in sys_data['S
+000342e0: 7973 7465 6d27 5d20 6966 2027 4765 6e65  ystem'] if 'Gene
+000342f0: 7261 6c27 2069 6e20 6974 656d 5b27 446f  ral' in item['Do
+00034300: 6d61 696e 275d 5d0d 0a20 2020 2020 2020  main']]..       
+00034310: 2072 6574 7572 6e20 7b66 5f6c 616e 673a   return {f_lang:
+00034320: 205b 7620 666f 7220 6b2c 2076 2069 6e20   [v for k, v in 
+00034330: 6c61 6e67 5f70 6169 7273 2069 6620 6b20  lang_pairs if k 
+00034340: 3d3d 2066 5f6c 616e 675d 2066 6f72 2066  == f_lang] for f
+00034350: 5f6c 616e 672c 2074 5f6c 616e 6720 696e  _lang, t_lang in
+00034360: 206c 616e 675f 7061 6972 737d 0d0a 0d0a   lang_pairs}....
+00034370: 2020 2020 6465 6620 6765 745f 6c61 6e67      def get_lang
+00034380: 7061 6972 5f69 6473 2873 656c 662c 2073  pair_ids(self, s
+00034390: 7973 5f64 6174 613a 2064 6963 7429 202d  ys_data: dict) -
+000343a0: 3e20 6469 6374 3a0d 0a20 2020 2020 2020  > dict:..       
+000343b0: 2072 6574 7572 6e20 7b66 227b 6974 656d   return {f"{item
+000343c0: 5b27 536f 7572 6365 4c61 6e67 7561 6765  ['SourceLanguage
+000343d0: 275d 5b27 436f 6465 275d 7d2d 7b69 7465  ']['Code']}-{ite
+000343e0: 6d5b 2754 6172 6765 744c 616e 6775 6167  m['TargetLanguag
+000343f0: 6527 5d5b 2743 6f64 6527 5d7d 223a 2069  e']['Code']}": i
+00034400: 7465 6d5b 2749 4427 5d20 666f 7220 6974  tem['ID'] for it
+00034410: 656d 2069 6e20 7379 735f 6461 7461 5b27  em in sys_data['
+00034420: 5379 7374 656d 275d 2069 6620 2747 656e  System'] if 'Gen
+00034430: 6572 616c 2720 696e 2069 7465 6d5b 2744  eral' in item['D
+00034440: 6f6d 6169 6e27 5d7d 0d0a 0d0a 2020 2020  omain']}....    
+00034450: 4054 7365 2e75 6e63 6572 7469 6669 6564  @Tse.uncertified
+00034460: 0d0a 2020 2020 4054 7365 2e74 696d 655f  ..    @Tse.time_
+00034470: 7374 6174 0d0a 2020 2020 4054 7365 2e63  stat..    @Tse.c
+00034480: 6865 636b 5f71 7565 7279 0d0a 2020 2020  heck_query..    
+00034490: 6465 6620 7469 6c64 655f 6170 6928 7365  def tilde_api(se
+000344a0: 6c66 2c20 7175 6572 795f 7465 7874 3a20  lf, query_text: 
+000344b0: 7374 722c 2066 726f 6d5f 6c61 6e67 7561  str, from_langua
+000344c0: 6765 3a20 7374 7220 3d20 2761 7574 6f27  ge: str = 'auto'
+000344d0: 2c20 746f 5f6c 616e 6775 6167 653a 2073  , to_language: s
+000344e0: 7472 203d 2027 656e 272c 202a 2a6b 7761  tr = 'en', **kwa
+000344f0: 7267 733a 2041 7069 4b77 6172 6773 5479  rgs: ApiKwargsTy
+00034500: 7065 2920 2d3e 2055 6e69 6f6e 5b73 7472  pe) -> Union[str
+00034510: 2c20 6469 6374 5d3a 0d0a 2020 2020 2020  , dict]:..      
+00034520: 2020 2222 220d 0a20 2020 2020 2020 2068    """..        h
+00034530: 7474 7073 3a2f 2f74 7261 6e73 6c61 7465  ttps://translate
+00034540: 2e74 696c 6465 2e63 6f6d 2f0d 0a20 2020  .tilde.com/..   
+00034550: 2020 2020 203a 7061 7261 6d20 7175 6572       :param quer
+00034560: 795f 7465 7874 3a20 7374 722c 206d 7573  y_text: str, mus
+00034570: 742e 0d0a 2020 2020 2020 2020 3a70 6172  t...        :par
+00034580: 616d 2066 726f 6d5f 6c61 6e67 7561 6765  am from_language
+00034590: 3a20 7374 722c 2064 6566 6175 6c74 2027  : str, default '
+000345a0: 6175 746f 272e 0d0a 2020 2020 2020 2020  auto'...        
+000345b0: 3a70 6172 616d 2074 6f5f 6c61 6e67 7561  :param to_langua
+000345c0: 6765 3a20 7374 722c 2064 6566 6175 6c74  ge: str, default
+000345d0: 2027 656e 272e 0d0a 2020 2020 2020 2020   'en'...        
+000345e0: 3a70 6172 616d 202a 2a6b 7761 7267 733a  :param **kwargs:
+000345f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00034600: 2020 3a70 6172 616d 2074 696d 656f 7574    :param timeout
+00034610: 3a20 666c 6f61 742c 2064 6566 6175 6c74  : float, default
+00034620: 204e 6f6e 652e 0d0a 2020 2020 2020 2020   None...        
+00034630: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+00034640: 726f 7869 6573 3a20 6469 6374 2c20 6465  roxies: dict, de
+00034650: 6661 756c 7420 4e6f 6e65 2e0d 0a20 2020  fault None...   
+00034660: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+00034670: 7261 6d20 736c 6565 705f 7365 636f 6e64  ram sleep_second
+00034680: 733a 2066 6c6f 6174 2c20 6465 6661 756c  s: float, defaul
+00034690: 7420 302e 0d0a 2020 2020 2020 2020 2020  t 0...          
+000346a0: 2020 2020 2020 3a70 6172 616d 2069 735f        :param is_
+000346b0: 6465 7461 696c 5f72 6573 756c 743a 2062  detail_result: b
+000346c0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+000346d0: 7365 2e0d 0a20 2020 2020 2020 2020 2020  se...           
+000346e0: 2020 2020 203a 7061 7261 6d20 6966 5f69       :param if_i
+000346f0: 676e 6f72 655f 6c69 6d69 745f 6f66 5f6c  gnore_limit_of_l
+00034700: 656e 6774 683a 2062 6f6f 6c2c 2064 6566  ength: bool, def
+00034710: 6175 6c74 2046 616c 7365 2e0d 0a20 2020  ault False...   
+00034720: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+00034730: 7261 6d20 6c69 6d69 745f 6f66 5f6c 656e  ram limit_of_len
+00034740: 6774 683a 2069 6e74 2c20 6465 6661 756c  gth: int, defaul
+00034750: 7420 3230 3030 302e 0d0a 2020 2020 2020  t 20000...      
+00034760: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+00034770: 2069 665f 6967 6e6f 7265 5f65 6d70 7479   if_ignore_empty
+00034780: 5f71 7565 7279 3a20 626f 6f6c 2c20 6465  _query: bool, de
+00034790: 6661 756c 7420 4661 6c73 652e 0d0a 2020  fault False...  
+000347a0: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+000347b0: 6172 616d 2075 7064 6174 655f 7365 7373  aram update_sess
+000347c0: 696f 6e5f 6166 7465 725f 6672 6571 3a20  ion_after_freq: 
+000347d0: 696e 742c 2064 6566 6175 6c74 2031 3030  int, default 100
+000347e0: 302e 0d0a 2020 2020 2020 2020 2020 2020  0...            
+000347f0: 2020 2020 3a70 6172 616d 2075 7064 6174      :param updat
+00034800: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
+00034810: 7365 636f 6e64 733a 2066 6c6f 6174 2c20  seconds: float, 
+00034820: 6465 6661 756c 7420 3135 3030 2e0d 0a20  default 1500... 
+00034830: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+00034840: 7061 7261 6d20 6966 5f73 686f 775f 7469  param if_show_ti
+00034850: 6d65 5f73 7461 743a 2062 6f6f 6c2c 2064  me_stat: bool, d
+00034860: 6566 6175 6c74 2046 616c 7365 2e0d 0a20  efault False... 
+00034870: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+00034880: 7061 7261 6d20 7368 6f77 5f74 696d 655f  param show_time_
+00034890: 7374 6174 5f70 7265 6369 7369 6f6e 3a20  stat_precision: 
+000348a0: 696e 742c 2064 6566 6175 6c74 2032 2e0d  int, default 2..
+000348b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000348c0: 203a 7061 7261 6d20 6966 5f70 7269 6e74   :param if_print
+000348d0: 5f77 6172 6e69 6e67 3a20 626f 6f6c 2c20  _warning: bool, 
+000348e0: 6465 6661 756c 7420 5472 7565 2e0d 0a20  default True... 
+000348f0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00034900: 7374 7220 6f72 2064 6963 740d 0a20 2020  str or dict..   
+00034910: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
+00034920: 2020 2020 7469 6d65 6f75 7420 3d20 6b77      timeout = kw
+00034930: 6172 6773 2e67 6574 2827 7469 6d65 6f75  args.get('timeou
+00034940: 7427 2c20 4e6f 6e65 290d 0a20 2020 2020  t', None)..     
+00034950: 2020 2070 726f 7869 6573 203d 206b 7761     proxies = kwa
+00034960: 7267 732e 6765 7428 2770 726f 7869 6573  rgs.get('proxies
+00034970: 272c 204e 6f6e 6529 0d0a 2020 2020 2020  ', None)..      
+00034980: 2020 736c 6565 705f 7365 636f 6e64 7320    sleep_seconds 
+00034990: 3d20 6b77 6172 6773 2e67 6574 2827 736c  = kwargs.get('sl
+000349a0: 6565 705f 7365 636f 6e64 7327 2c20 3029  eep_seconds', 0)
+000349b0: 0d0a 2020 2020 2020 2020 6966 5f70 7269  ..        if_pri
+000349c0: 6e74 5f77 6172 6e69 6e67 203d 206b 7761  nt_warning = kwa
+000349d0: 7267 732e 6765 7428 2769 665f 7072 696e  rgs.get('if_prin
+000349e0: 745f 7761 726e 696e 6727 2c20 5472 7565  t_warning', True
+000349f0: 290d 0a20 2020 2020 2020 2069 735f 6465  )..        is_de
+00034a00: 7461 696c 5f72 6573 756c 7420 3d20 6b77  tail_result = kw
+00034a10: 6172 6773 2e67 6574 2827 6973 5f64 6574  args.get('is_det
+00034a20: 6169 6c5f 7265 7375 6c74 272c 2046 616c  ail_result', Fal
+00034a30: 7365 290d 0a20 2020 2020 2020 2075 7064  se)..        upd
+00034a40: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
+00034a50: 725f 6672 6571 203d 206b 7761 7267 732e  r_freq = kwargs.
+00034a60: 6765 7428 2775 7064 6174 655f 7365 7373  get('update_sess
+00034a70: 696f 6e5f 6166 7465 725f 6672 6571 272c  ion_after_freq',
+00034a80: 2073 656c 662e 6465 6661 756c 745f 7365   self.default_se
+00034a90: 7373 696f 6e5f 6672 6571 290d 0a20 2020  ssion_freq)..   
+00034aa0: 2020 2020 2075 7064 6174 655f 7365 7373       update_sess
+00034ab0: 696f 6e5f 6166 7465 725f 7365 636f 6e64  ion_after_second
+00034ac0: 7320 3d20 6b77 6172 6773 2e67 6574 2827  s = kwargs.get('
+00034ad0: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
+00034ae0: 6674 6572 5f73 6563 6f6e 6473 272c 2073  fter_seconds', s
+00034af0: 656c 662e 6465 6661 756c 745f 7365 7373  elf.default_sess
+00034b00: 696f 6e5f 7365 636f 6e64 7329 0d0a 2020  ion_seconds)..  
+00034b10: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
+00034b20: 5f69 6e70 7574 5f6c 696d 6974 2871 7565  _input_limit(que
+00034b30: 7279 5f74 6578 742c 2073 656c 662e 696e  ry_text, self.in
+00034b40: 7075 745f 6c69 6d69 7429 0d0a 0d0a 2020  put_limit)....  
+00034b50: 2020 2020 2020 6e6f 745f 7570 6461 7465        not_update
+00034b60: 5f63 6f6e 645f 6672 6571 203d 2031 2069  _cond_freq = 1 i
+00034b70: 6620 7365 6c66 2e71 7565 7279 5f63 6f75  f self.query_cou
+00034b80: 6e74 203c 2075 7064 6174 655f 7365 7373  nt < update_sess
+00034b90: 696f 6e5f 6166 7465 725f 6672 6571 2065  ion_after_freq e
+00034ba0: 6c73 6520 300d 0a20 2020 2020 2020 206e  lse 0..        n
+00034bb0: 6f74 5f75 7064 6174 655f 636f 6e64 5f74  ot_update_cond_t
+00034bc0: 696d 6520 3d20 3120 6966 2074 696d 652e  ime = 1 if time.
+00034bd0: 7469 6d65 2829 202d 2073 656c 662e 6265  time() - self.be
+00034be0: 6769 6e5f 7469 6d65 203c 2075 7064 6174  gin_time < updat
+00034bf0: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
+00034c00: 7365 636f 6e64 7320 656c 7365 2030 0d0a  seconds else 0..
+00034c10: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
+00034c20: 7365 6c66 2e73 6573 7369 6f6e 2061 6e64  self.session and
+00034c30: 2073 656c 662e 6c61 6e67 7561 6765 5f6d   self.language_m
+00034c40: 6170 2061 6e64 206e 6f74 5f75 7064 6174  ap and not_updat
+00034c50: 655f 636f 6e64 5f66 7265 7120 616e 6420  e_cond_freq and 
+00034c60: 6e6f 745f 7570 6461 7465 5f63 6f6e 645f  not_update_cond_
+00034c70: 7469 6d65 293a 0d0a 2020 2020 2020 2020  time):..        
+00034c80: 2020 2020 7365 6c66 2e73 6573 7369 6f6e      self.session
+00034c90: 203d 2072 6571 7565 7374 732e 5365 7373   = requests.Sess
+00034ca0: 696f 6e28 290d 0a20 2020 2020 2020 2020  ion()..         
+00034cb0: 2020 205f 203d 2073 656c 662e 7365 7373     _ = self.sess
+00034cc0: 696f 6e2e 6765 7428 7365 6c66 2e68 6f73  ion.get(self.hos
+00034cd0: 745f 7572 6c2c 2068 6561 6465 7273 3d73  t_url, headers=s
+00034ce0: 656c 662e 686f 7374 5f68 6561 6465 7273  elf.host_headers
+00034cf0: 2c20 7469 6d65 6f75 743d 7469 6d65 6f75  , timeout=timeou
+00034d00: 742c 2070 726f 7869 6573 3d70 726f 7869  t, proxies=proxi
+00034d10: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+00034d20: 2073 656c 662e 636f 6e66 6967 5f64 6174   self.config_dat
+00034d30: 6120 3d20 7365 6c66 2e73 6573 7369 6f6e  a = self.session
+00034d40: 2e67 6574 2873 656c 662e 6765 745f 636f  .get(self.get_co
+00034d50: 6e66 6967 5f75 726c 2c20 6865 6164 6572  nfig_url, header
+00034d60: 733d 7365 6c66 2e68 6f73 745f 6865 6164  s=self.host_head
+00034d70: 6572 732c 2074 696d 656f 7574 3d74 696d  ers, timeout=tim
+00034d80: 656f 7574 2c20 7072 6f78 6965 733d 7072  eout, proxies=pr
+00034d90: 6f78 6965 7329 2e6a 736f 6e28 290d 0a20  oxies).json().. 
+00034da0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00034db0: 6170 695f 6865 6164 6572 732e 7570 6461  api_headers.upda
+00034dc0: 7465 287b 2763 6c69 656e 742d 6964 273a  te({'client-id':
+00034dd0: 2073 656c 662e 636f 6e66 6967 5f64 6174   self.config_dat
+00034de0: 615b 276d 7427 5d5b 2761 7069 275d 5b27  a['mt']['api']['
+00034df0: 636c 6965 6e74 4964 275d 7d29 2020 2320  clientId']})  # 
+00034e00: 6d75 7374 206c 6f77 6572 206b 6579 776f  must lower keywo
+00034e10: 7264 0d0a 0d0a 2020 2020 2020 2020 2020  rd....          
+00034e20: 2020 7379 735f 7572 6c20 3d20 7365 6c66    sys_url = self
+00034e30: 2e63 6f6e 6669 675f 6461 7461 5b27 6d74  .config_data['mt
+00034e40: 275d 5b27 6170 6927 5d5b 2773 7973 7465  ']['api']['syste
+00034e50: 6d4c 6973 7455 726c 275d 0d0a 2020 2020  mListUrl']..    
+00034e60: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+00034e70: 207b 2761 7070 4944 273a 2073 656c 662e   {'appID': self.
+00034e80: 636f 6e66 6967 5f64 6174 615b 276d 7427  config_data['mt'
+00034e90: 5d5b 2761 7069 275d 5b27 6170 7049 4427  ]['api']['appID'
+00034ea0: 5d2c 2027 7569 4c61 6e67 7561 6765 4944  ], 'uiLanguageID
+00034eb0: 273a 2073 656c 662e 636f 6e66 6967 5f64  ': self.config_d
+00034ec0: 6174 615b 276d 7427 5d5b 2761 7069 275d  ata['mt']['api']
+00034ed0: 5b27 7569 4c61 6e67 7561 6765 4944 275d  ['uiLanguageID']
+00034ee0: 7d0d 0a20 2020 2020 2020 2020 2020 2073  }..            s
+00034ef0: 656c 662e 7379 735f 6461 7461 203d 2073  elf.sys_data = s
+00034f00: 656c 662e 7365 7373 696f 6e2e 6765 7428  elf.session.get(
+00034f10: 7379 735f 7572 6c2c 2070 6172 616d 733d  sys_url, params=
+00034f20: 7061 7261 6d73 2c20 6865 6164 6572 733d  params, headers=
+00034f30: 7365 6c66 2e61 7069 5f68 6561 6465 7273  self.api_headers
+00034f40: 2c20 7469 6d65 6f75 743d 7469 6d65 6f75  , timeout=timeou
+00034f50: 742c 2070 726f 7869 6573 3d70 726f 7869  t, proxies=proxi
+00034f60: 6573 292e 6a73 6f6e 2829 2020 2320 7465  es).json()  # te
+00034f70: 7374 0d0a 2020 2020 2020 2020 2020 2020  st..            
+00034f80: 7365 6c66 2e6c 616e 6770 6169 725f 6964  self.langpair_id
+00034f90: 7320 3d20 7365 6c66 2e67 6574 5f6c 616e  s = self.get_lan
+00034fa0: 6770 6169 725f 6964 7328 7365 6c66 2e73  gpair_ids(self.s
+00034fb0: 7973 5f64 6174 6129 0d0a 2020 2020 2020  ys_data)..      
+00034fc0: 2020 2020 2020 6465 6275 675f 6c61 6e67        debug_lang
+00034fd0: 5f6b 7761 7267 7320 3d20 7365 6c66 2e64  _kwargs = self.d
+00034fe0: 6562 7567 5f6c 616e 675f 6b77 6172 6773  ebug_lang_kwargs
+00034ff0: 2866 726f 6d5f 6c61 6e67 7561 6765 2c20  (from_language, 
+00035000: 746f 5f6c 616e 6775 6167 652c 2073 656c  to_language, sel
+00035010: 662e 6465 6661 756c 745f 6672 6f6d 5f6c  f.default_from_l
+00035020: 616e 6775 6167 652c 2069 665f 7072 696e  anguage, if_prin
+00035030: 745f 7761 726e 696e 6729 0d0a 2020 2020  t_warning)..    
+00035040: 2020 2020 2020 2020 7365 6c66 2e6c 616e          self.lan
+00035050: 6775 6167 655f 6d61 7020 3d20 7365 6c66  guage_map = self
+00035060: 2e67 6574 5f6c 616e 6775 6167 655f 6d61  .get_language_ma
+00035070: 7028 7365 6c66 2e73 7973 5f64 6174 612c  p(self.sys_data,
+00035080: 202a 2a64 6562 7567 5f6c 616e 675f 6b77   **debug_lang_kw
+00035090: 6172 6773 290d 0a0d 0a20 2020 2020 2020  args)....       
+000350a0: 2069 6620 6672 6f6d 5f6c 616e 6775 6167   if from_languag
+000350b0: 6520 3d3d 2027 6175 746f 273a 0d0a 2020  e == 'auto':..  
+000350c0: 2020 2020 2020 2020 2020 6672 6f6d 5f6c            from_l
+000350d0: 616e 6775 6167 6520 3d20 7365 6c66 2e77  anguage = self.w
+000350e0: 6172 6e69 6e67 5f61 7574 6f5f 6c61 6e67  arning_auto_lang
+000350f0: 2827 7469 6c64 6527 2c20 7365 6c66 2e64  ('tilde', self.d
+00035100: 6566 6175 6c74 5f66 726f 6d5f 6c61 6e67  efault_from_lang
+00035110: 7561 6765 2c20 6966 5f70 7269 6e74 5f77  uage, if_print_w
+00035120: 6172 6e69 6e67 290d 0a20 2020 2020 2020  arning)..       
+00035130: 2066 726f 6d5f 6c61 6e67 7561 6765 2c20   from_language, 
+00035140: 746f 5f6c 616e 6775 6167 6520 3d20 7365  to_language = se
+00035150: 6c66 2e63 6865 636b 5f6c 616e 6775 6167  lf.check_languag
+00035160: 6528 6672 6f6d 5f6c 616e 6775 6167 652c  e(from_language,
+00035170: 2074 6f5f 6c61 6e67 7561 6765 2c20 7365   to_language, se
+00035180: 6c66 2e6c 616e 6775 6167 655f 6d61 7029  lf.language_map)
+00035190: 0d0a 0d0a 2020 2020 2020 2020 7061 796c  ....        payl
+000351a0: 6f61 6420 3d20 7b0d 0a20 2020 2020 2020  oad = {..       
+000351b0: 2020 2020 2027 7465 7874 273a 2071 7565       'text': que
+000351c0: 7279 5f74 6578 742c 0d0a 2020 2020 2020  ry_text,..      
+000351d0: 2020 2020 2020 2761 7070 4944 273a 2073        'appID': s
+000351e0: 656c 662e 636f 6e66 6967 5f64 6174 615b  elf.config_data[
+000351f0: 276d 7427 5d5b 2761 7069 275d 5b27 6170  'mt']['api']['ap
+00035200: 7049 4427 5d2c 0d0a 2020 2020 2020 2020  pID'],..        
+00035210: 2020 2020 2773 7973 7465 6d49 4427 3a20      'systemID': 
+00035220: 7365 6c66 2e6c 616e 6770 6169 725f 6964  self.langpair_id
+00035230: 735b 6627 7b66 726f 6d5f 6c61 6e67 7561  s[f'{from_langua
+00035240: 6765 7d2d 7b74 6f5f 6c61 6e67 7561 6765  ge}-{to_language
+00035250: 7d27 5d2c 0d0a 2020 2020 2020 2020 2020  }'],..          
+00035260: 2020 276f 7074 696f 6e73 273a 2027 7769    'options': 'wi
+00035270: 6467 6574 3d74 6578 742c 616c 6967 6e6d  dget=text,alignm
+00035280: 656e 742c 6d61 726b 5365 6e74 656e 6365  ent,markSentence
+00035290: 7327 2c0d 0a20 2020 2020 2020 207d 0d0a  s',..        }..
+000352a0: 2020 2020 2020 2020 7220 3d20 7365 6c66          r = self
+000352b0: 2e73 6573 7369 6f6e 2e70 6f73 7428 7365  .session.post(se
+000352c0: 6c66 2e61 7069 5f75 726c 2c20 6a73 6f6e  lf.api_url, json
+000352d0: 3d70 6179 6c6f 6164 2c20 6865 6164 6572  =payload, header
+000352e0: 733d 7365 6c66 2e61 7069 5f68 6561 6465  s=self.api_heade
+000352f0: 7273 2c20 7469 6d65 6f75 743d 7469 6d65  rs, timeout=time
+00035300: 6f75 742c 2070 726f 7869 6573 3d70 726f  out, proxies=pro
+00035310: 7869 6573 290d 0a20 2020 2020 2020 2072  xies)..        r
+00035320: 2e72 6169 7365 5f66 6f72 5f73 7461 7475  .raise_for_statu
+00035330: 7328 290d 0a20 2020 2020 2020 2064 6174  s()..        dat
+00035340: 6120 3d20 722e 6a73 6f6e 2829 0d0a 2020  a = r.json()..  
+00035350: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+00035360: 2873 6c65 6570 5f73 6563 6f6e 6473 290d  (sleep_seconds).
+00035370: 0a20 2020 2020 2020 2073 656c 662e 7175  .        self.qu
+00035380: 6572 795f 636f 756e 7420 2b3d 2031 0d0a  ery_count += 1..
+00035390: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+000353a0: 6174 6120 6966 2069 735f 6465 7461 696c  ata if is_detail
+000353b0: 5f72 6573 756c 7420 656c 7365 2064 6174  _result else dat
+000353c0: 615b 2774 7261 6e73 6c61 7469 6f6e 275d  a['translation']
+000353d0: 0d0a 0d0a 0d0a 636c 6173 7320 436c 6f75  ......class Clou
+000353e0: 6459 6928 5473 6529 3a0d 0a20 2020 2064  dYi(Tse):..    d
+000353f0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00035400: 293a 0d0a 2020 2020 2020 2020 7375 7065  ):..        supe
+00035410: 7228 292e 5f5f 696e 6974 5f5f 2829 0d0a  r().__init__()..
+00035420: 2020 2020 2020 2020 7365 6c66 2e68 6f6d          self.hom
+00035430: 655f 7572 6c20 3d20 2768 7474 7073 3a2f  e_url = 'https:/
+00035440: 2f77 7777 2e63 6c6f 7564 7472 616e 736c  /www.cloudtransl
+00035450: 6174 696f 6e2e 636f 6d27 0d0a 2020 2020  ation.com'..    
+00035460: 2020 2020 7365 6c66 2e68 6f73 745f 7572      self.host_ur
+00035470: 6c20 3d20 2768 7474 7073 3a2f 2f77 7777  l = 'https://www
+00035480: 2e63 6c6f 7564 7472 616e 736c 6174 696f  .cloudtranslatio
+00035490: 6e2e 636f 6d2f 232f 7472 616e 736c 6174  n.com/#/translat
+000354a0: 6527 0d0a 2020 2020 2020 2020 7365 6c66  e'..        self
+000354b0: 2e61 7069 5f75 726c 203d 2027 6874 7470  .api_url = 'http
+000354c0: 733a 2f2f 7777 772e 636c 6f75 6474 7261  s://www.cloudtra
+000354d0: 6e73 6c61 7469 6f6e 2e63 6f6d 2f6f 6666  nslation.com/off
+000354e0: 6963 6961 6c2d 7765 6273 6974 652f 7631  icial-website/v1
+000354f0: 2f74 7261 6e73 4f6e 6553 7263 5465 7874  /transOneSrcText
+00035500: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+00035510: 6765 745f 6c61 6e67 5f75 726c 203d 2027  get_lang_url = '
+00035520: 6874 7470 733a 2f2f 6f6e 6c69 6e65 2e63  https://online.c
+00035530: 6c6f 7564 7472 616e 736c 6174 696f 6e2e  loudtranslation.
+00035540: 636f 6d2f 6170 692f 7631 2e30 2f73 6974  com/api/v1.0/sit
+00035550: 652f 6765 745f 616c 6c5f 6c61 6e67 7561  e/get_all_langua
+00035560: 6765 5f61 6e64 5f64 6f6d 6169 6e27 0d0a  ge_and_domain'..
+00035570: 2020 2020 2020 2020 7365 6c66 2e64 6574          self.det
+00035580: 6563 745f 6c61 6e67 5f75 726c 203d 2027  ect_lang_url = '
+00035590: 6874 7470 733a 2f2f 6f6e 6c69 6e65 2e63  https://online.c
+000355a0: 6c6f 7564 7472 616e 736c 6174 696f 6e2e  loudtranslation.
+000355b0: 636f 6d2f 6170 692f 7631 2e30 2f72 6571  com/api/v1.0/req
+000355c0: 7565 7374 5f74 7261 6e73 6c61 7465 2f6c  uest_translate/l
+000355d0: 616e 6769 6427 0d0a 2020 2020 2020 2020  angid'..        
+000355e0: 7365 6c66 2e67 6574 5f63 6f6f 6b69 655f  self.get_cookie_
+000355f0: 7572 6c20 3d20 2768 7474 7073 3a2f 2f6f  url = 'https://o
+00035600: 6e6c 696e 652e 636c 6f75 6474 7261 6e73  nline.cloudtrans
+00035610: 6c61 7469 6f6e 2e63 6f6d 2f61 7069 2f76  lation.com/api/v
+00035620: 312e 302f 7369 7465 2f73 6974 6573 5f6c  1.0/site/sites_l
+00035630: 616e 6775 6167 655f 6c69 7374 270d 0a20  anguage_list'.. 
+00035640: 2020 2020 2020 2073 656c 662e 686f 7374         self.host
+00035650: 5f68 6561 6465 7273 203d 2073 656c 662e  _headers = self.
+00035660: 6765 745f 6865 6164 6572 7328 7365 6c66  get_headers(self
+00035670: 2e68 6f6d 655f 7572 6c2c 2069 665f 6170  .home_url, if_ap
+00035680: 693d 4661 6c73 652c 2069 665f 7265 6665  i=False, if_refe
+00035690: 7265 725f 666f 725f 686f 7374 3d54 7275  rer_for_host=Tru
+000356a0: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
+000356b0: 2e61 7069 5f68 6561 6465 7273 203d 2073  .api_headers = s
+000356c0: 656c 662e 6765 745f 6865 6164 6572 7328  elf.get_headers(
+000356d0: 7365 6c66 2e68 6f6d 655f 7572 6c2c 2069  self.home_url, i
+000356e0: 665f 6170 693d 5472 7565 2c20 6966 5f6a  f_api=True, if_j
+000356f0: 736f 6e5f 666f 725f 6170 693d 5472 7565  son_for_api=True
+00035700: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00035710: 7365 7373 696f 6e20 3d20 4e6f 6e65 0d0a  session = None..
+00035720: 2020 2020 2020 2020 7365 6c66 2e6c 616e          self.lan
+00035730: 6775 6167 655f 6d61 7020 3d20 4e6f 6e65  guage_map = None
+00035740: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00035750: 616e 6770 6169 725f 646f 6d61 696e 203d  angpair_domain =
+00035760: 204e 6f6e 650d 0a20 2020 2020 2020 2073   None..        s
+00035770: 656c 662e 7072 6f66 6573 7369 6f6e 616c  elf.professional
+00035780: 5f66 6965 6c64 203d 204e 6f6e 650d 0a20  _field = None.. 
+00035790: 2020 2020 2020 2073 656c 662e 7175 6572         self.quer
+000357a0: 795f 636f 756e 7420 3d20 300d 0a20 2020  y_count = 0..   
+000357b0: 2020 2020 2073 656c 662e 6f75 7470 7574       self.output
+000357c0: 5f7a 6820 3d20 277a 682d 636e 270d 0a20  _zh = 'zh-cn'.. 
+000357d0: 2020 2020 2020 2073 656c 662e 6f75 7470         self.outp
+000357e0: 7574 5f65 6e20 3d20 2765 6e2d 7573 270d  ut_en = 'en-us'.
+000357f0: 0a20 2020 2020 2020 2073 656c 662e 6f75  .        self.ou
+00035800: 7470 7574 5f61 7574 6f20 3d20 2761 6c6c  tput_auto = 'all
+00035810: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+00035820: 696e 7075 745f 6c69 6d69 7420 3d20 696e  input_limit = in
+00035830: 7428 3565 3329 0d0a 2020 2020 2020 2020  t(5e3)..        
+00035840: 7365 6c66 2e64 6566 6175 6c74 5f66 726f  self.default_fro
+00035850: 6d5f 6c61 6e67 7561 6765 203d 2073 656c  m_language = sel
+00035860: 662e 6f75 7470 7574 5f7a 680d 0a0d 0a20  f.output_zh.... 
+00035870: 2020 2040 5473 652e 6465 6275 675f 6c61     @Tse.debug_la
+00035880: 6e67 7561 6765 5f6d 6170 0d0a 2020 2020  nguage_map..    
+00035890: 6465 6620 6765 745f 6c61 6e67 7561 6765  def get_language
+000358a0: 5f6d 6170 2873 656c 662c 2064 5f6c 616e  _map(self, d_lan
+000358b0: 675f 6d61 703a 2064 6963 742c 202a 2a6b  g_map: dict, **k
+000358c0: 7761 7267 733a 204c 616e 674d 6170 4b77  wargs: LangMapKw
+000358d0: 6172 6773 5479 7065 2920 2d3e 2064 6963  argsType) -> dic
+000358e0: 743a 0d0a 2020 2020 2020 2020 7265 7475  t:..        retu
+000358f0: 726e 207b 6b3a 205b 6974 5b27 6c61 6e67  rn {k: [it['lang
+00035900: 7561 6765 5f63 6f64 6527 5d20 666f 7220  uage_code'] for 
+00035910: 6974 2069 6e20 6974 656d 5d20 666f 7220  it in item] for 
+00035920: 6b2c 2069 7465 6d20 696e 2064 5f6c 616e  k, item in d_lan
+00035930: 675f 6d61 705b 2764 6174 6127 5d5b 2773  g_map['data']['s
+00035940: 7263 5f74 6f5f 7467 7427 5d2e 6974 656d  rc_to_tgt'].item
+00035950: 7328 297d 0d0a 0d0a 2020 2020 6465 6620  s()}....    def 
+00035960: 6765 745f 6c61 6e67 7061 6972 5f64 6f6d  get_langpair_dom
+00035970: 6169 6e28 7365 6c66 2c20 645f 6c61 6e67  ain(self, d_lang
+00035980: 5f6d 6170 3a20 6469 6374 2920 2d3e 2064  _map: dict) -> d
+00035990: 6963 743a 0d0a 2020 2020 2020 2020 7265  ict:..        re
+000359a0: 7475 726e 207b 6b3a 205b 6974 5b27 646f  turn {k: [it['do
+000359b0: 6d61 696e 5f63 6f64 6527 5d20 666f 7220  main_code'] for 
+000359c0: 6974 2069 6e20 6974 656d 5d20 666f 7220  it in item] for 
+000359d0: 6b2c 2069 7465 6d20 696e 2064 5f6c 616e  k, item in d_lan
+000359e0: 675f 6d61 705b 2764 6174 6127 5d5b 276c  g_map['data']['l
+000359f0: 616e 6775 6167 655f 7061 6972 5f74 6f5f  anguage_pair_to_
+00035a00: 646f 6d61 696e 275d 2e69 7465 6d73 2829  domain'].items()
+00035a10: 7d0d 0a0d 0a20 2020 2064 6566 2067 6574  }....    def get
+00035a20: 5f70 726f 6665 7373 696f 6e61 6c5f 6669  _professional_fi
+00035a30: 656c 645f 6c69 7374 2873 656c 662c 2064  eld_list(self, d
+00035a40: 5f6c 616e 675f 6d61 703a 2064 6963 7429  _lang_map: dict)
+00035a50: 202d 3e20 7365 743a 0d0a 2020 2020 2020   -> set:..      
+00035a60: 2020 7265 7475 726e 207b 6974 5b27 646f    return {it['do
+00035a70: 6d61 696e 5f63 6f64 6527 5d20 666f 7220  main_code'] for 
+00035a80: 5f2c 2069 7465 6d20 696e 2064 5f6c 616e  _, item in d_lan
+00035a90: 675f 6d61 705b 2764 6174 6127 5d5b 276c  g_map['data']['l
+00035aa0: 616e 6775 6167 655f 7061 6972 5f74 6f5f  anguage_pair_to_
+00035ab0: 646f 6d61 696e 275d 2e69 7465 6d73 2829  domain'].items()
+00035ac0: 2066 6f72 2069 7420 696e 2069 7465 6d7d   for it in item}
+00035ad0: 0d0a 0d0a 2020 2020 4054 7365 2e74 696d  ....    @Tse.tim
+00035ae0: 655f 7374 6174 0d0a 2020 2020 4054 7365  e_stat..    @Tse
+00035af0: 2e63 6865 636b 5f71 7565 7279 0d0a 2020  .check_query..  
+00035b00: 2020 6465 6620 636c 6f75 6459 695f 6170    def cloudYi_ap
+00035b10: 6928 7365 6c66 2c20 7175 6572 795f 7465  i(self, query_te
+00035b20: 7874 3a20 7374 722c 2066 726f 6d5f 6c61  xt: str, from_la
+00035b30: 6e67 7561 6765 3a20 7374 7220 3d20 2761  nguage: str = 'a
+00035b40: 7574 6f27 2c20 746f 5f6c 616e 6775 6167  uto', to_languag
+00035b50: 653a 2073 7472 203d 2027 656e 272c 202a  e: str = 'en', *
+00035b60: 2a6b 7761 7267 733a 2041 7069 4b77 6172  *kwargs: ApiKwar
+00035b70: 6773 5479 7065 2920 2d3e 2055 6e69 6f6e  gsType) -> Union
+00035b80: 5b73 7472 2c20 6469 6374 5d3a 0d0a 2020  [str, dict]:..  
+00035b90: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00035ba0: 2020 2068 7474 7073 3a2f 2f77 7777 2e63     https://www.c
+00035bb0: 6c6f 7564 7472 616e 736c 6174 696f 6e2e  loudtranslation.
+00035bc0: 636f 6d2f 232f 7472 616e 736c 6174 650d  com/#/translate.
+00035bd0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00035be0: 7175 6572 795f 7465 7874 3a20 7374 722c  query_text: str,
+00035bf0: 206d 7573 742e 0d0a 2020 2020 2020 2020   must...        
+00035c00: 3a70 6172 616d 2066 726f 6d5f 6c61 6e67  :param from_lang
+00035c10: 7561 6765 3a20 7374 722c 2064 6566 6175  uage: str, defau
+00035c20: 6c74 2027 6175 746f 272e 0d0a 2020 2020  lt 'auto'...    
+00035c30: 2020 2020 3a70 6172 616d 2074 6f5f 6c61      :param to_la
+00035c40: 6e67 7561 6765 3a20 7374 722c 2064 6566  nguage: str, def
+00035c50: 6175 6c74 2027 656e 272e 0d0a 2020 2020  ault 'en'...    
+00035c60: 2020 2020 3a70 6172 616d 202a 2a6b 7761      :param **kwa
+00035c70: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+00035c80: 2020 2020 2020 3a70 6172 616d 2074 696d        :param tim
+00035c90: 656f 7574 3a20 666c 6f61 742c 2064 6566  eout: float, def
+00035ca0: 6175 6c74 204e 6f6e 652e 0d0a 2020 2020  ault None...    
+00035cb0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00035cc0: 616d 2070 726f 7869 6573 3a20 6469 6374  am proxies: dict
+00035cd0: 2c20 6465 6661 756c 7420 4e6f 6e65 2e0d  , default None..
+00035ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00035cf0: 203a 7061 7261 6d20 736c 6565 705f 7365   :param sleep_se
+00035d00: 636f 6e64 733a 2066 6c6f 6174 2c20 6465  conds: float, de
+00035d10: 6661 756c 7420 302e 0d0a 2020 2020 2020  fault 0...      
+00035d20: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+00035d30: 2069 735f 6465 7461 696c 5f72 6573 756c   is_detail_resul
+00035d40: 743a 2062 6f6f 6c2c 2064 6566 6175 6c74  t: bool, default
+00035d50: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
+00035d60: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00035d70: 6966 5f69 676e 6f72 655f 6c69 6d69 745f  if_ignore_limit_
+00035d80: 6f66 5f6c 656e 6774 683a 2062 6f6f 6c2c  of_length: bool,
+00035d90: 2064 6566 6175 6c74 2046 616c 7365 2e0d   default False..
+00035da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00035db0: 203a 7061 7261 6d20 6c69 6d69 745f 6f66   :param limit_of
+00035dc0: 5f6c 656e 6774 683a 2069 6e74 2c20 6465  _length: int, de
+00035dd0: 6661 756c 7420 3230 3030 302e 0d0a 2020  fault 20000...  
+00035de0: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+00035df0: 6172 616d 2069 665f 6967 6e6f 7265 5f65  aram if_ignore_e
+00035e00: 6d70 7479 5f71 7565 7279 3a20 626f 6f6c  mpty_query: bool
+00035e10: 2c20 6465 6661 756c 7420 4661 6c73 652e  , default False.
+00035e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00035e30: 2020 3a70 6172 616d 2075 7064 6174 655f    :param update_
+00035e40: 7365 7373 696f 6e5f 6166 7465 725f 6672  session_after_fr
+00035e50: 6571 3a20 696e 742c 2064 6566 6175 6c74  eq: int, default
+00035e60: 2031 3030 302e 0d0a 2020 2020 2020 2020   1000...        
+00035e70: 2020 2020 2020 2020 3a70 6172 616d 2075          :param u
+00035e80: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
+00035e90: 7465 725f 7365 636f 6e64 733a 2066 6c6f  ter_seconds: flo
+00035ea0: 6174 2c20 6465 6661 756c 7420 3135 3030  at, default 1500
+00035eb0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00035ec0: 2020 203a 7061 7261 6d20 6966 5f73 686f     :param if_sho
+00035ed0: 775f 7469 6d65 5f73 7461 743a 2062 6f6f  w_time_stat: boo
+00035ee0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+00035ef0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00035f00: 2020 203a 7061 7261 6d20 7368 6f77 5f74     :param show_t
+00035f10: 696d 655f 7374 6174 5f70 7265 6369 7369  ime_stat_precisi
+00035f20: 6f6e 3a20 696e 742c 2064 6566 6175 6c74  on: int, default
+00035f30: 2032 2e0d 0a20 2020 2020 2020 2020 2020   2...           
+00035f40: 2020 2020 203a 7061 7261 6d20 6966 5f70       :param if_p
+00035f50: 7269 6e74 5f77 6172 6e69 6e67 3a20 626f  rint_warning: bo
+00035f60: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+00035f70: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00035f80: 2020 203a 7061 7261 6d20 7072 6f66 6573     :param profes
+00035f90: 7369 6f6e 616c 5f66 6965 6c64 3a20 7374  sional_field: st
+00035fa0: 722c 2064 6566 6175 6c74 2027 6765 6e65  r, default 'gene
+00035fb0: 7261 6c27 2e0d 0a20 2020 2020 2020 203a  ral'...        :
+00035fc0: 7265 7475 726e 3a20 7374 7220 6f72 2064  return: str or d
+00035fd0: 6963 740d 0a20 2020 2020 2020 2022 2222  ict..        """
+00035fe0: 0d0a 0d0a 2020 2020 2020 2020 7573 655f  ....        use_
+00035ff0: 646f 6d61 696e 203d 206b 7761 7267 732e  domain = kwargs.
+00036000: 6765 7428 2770 726f 6665 7373 696f 6e61  get('professiona
+00036010: 6c5f 6669 656c 6427 2c20 2767 656e 6572  l_field', 'gener
+00036020: 616c 2729 0d0a 2020 2020 2020 2020 7469  al')..        ti
+00036030: 6d65 6f75 7420 3d20 6b77 6172 6773 2e67  meout = kwargs.g
+00036040: 6574 2827 7469 6d65 6f75 7427 2c20 4e6f  et('timeout', No
+00036050: 6e65 290d 0a20 2020 2020 2020 2070 726f  ne)..        pro
+00036060: 7869 6573 203d 206b 7761 7267 732e 6765  xies = kwargs.ge
+00036070: 7428 2770 726f 7869 6573 272c 204e 6f6e  t('proxies', Non
+00036080: 6529 0d0a 2020 2020 2020 2020 736c 6565  e)..        slee
+00036090: 705f 7365 636f 6e64 7320 3d20 6b77 6172  p_seconds = kwar
+000360a0: 6773 2e67 6574 2827 736c 6565 705f 7365  gs.get('sleep_se
+000360b0: 636f 6e64 7327 2c20 3029 0d0a 2020 2020  conds', 0)..    
+000360c0: 2020 2020 6966 5f70 7269 6e74 5f77 6172      if_print_war
+000360d0: 6e69 6e67 203d 206b 7761 7267 732e 6765  ning = kwargs.ge
+000360e0: 7428 2769 665f 7072 696e 745f 7761 726e  t('if_print_warn
+000360f0: 696e 6727 2c20 5472 7565 290d 0a20 2020  ing', True)..   
+00036100: 2020 2020 2069 735f 6465 7461 696c 5f72       is_detail_r
+00036110: 6573 756c 7420 3d20 6b77 6172 6773 2e67  esult = kwargs.g
+00036120: 6574 2827 6973 5f64 6574 6169 6c5f 7265  et('is_detail_re
+00036130: 7375 6c74 272c 2046 616c 7365 290d 0a20  sult', False).. 
+00036140: 2020 2020 2020 2075 7064 6174 655f 7365         update_se
+00036150: 7373 696f 6e5f 6166 7465 725f 6672 6571  ssion_after_freq
+00036160: 203d 206b 7761 7267 732e 6765 7428 2775   = kwargs.get('u
+00036170: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
+00036180: 7465 725f 6672 6571 272c 2073 656c 662e  ter_freq', self.
+00036190: 6465 6661 756c 745f 7365 7373 696f 6e5f  default_session_
+000361a0: 6672 6571 290d 0a20 2020 2020 2020 2075  freq)..        u
+000361b0: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
+000361c0: 7465 725f 7365 636f 6e64 7320 3d20 6b77  ter_seconds = kw
+000361d0: 6172 6773 2e67 6574 2827 7570 6461 7465  args.get('update
+000361e0: 5f73 6573 7369 6f6e 5f61 6674 6572 5f73  _session_after_s
+000361f0: 6563 6f6e 6473 272c 2073 656c 662e 6465  econds', self.de
+00036200: 6661 756c 745f 7365 7373 696f 6e5f 7365  fault_session_se
+00036210: 636f 6e64 7329 0d0a 2020 2020 2020 2020  conds)..        
+00036220: 7365 6c66 2e63 6865 636b 5f69 6e70 7574  self.check_input
+00036230: 5f6c 696d 6974 2871 7565 7279 5f74 6578  _limit(query_tex
+00036240: 742c 2073 656c 662e 696e 7075 745f 6c69  t, self.input_li
+00036250: 6d69 7429 0d0a 0d0a 2020 2020 2020 2020  mit)....        
+00036260: 6e6f 745f 7570 6461 7465 5f63 6f6e 645f  not_update_cond_
+00036270: 6672 6571 203d 2031 2069 6620 7365 6c66  freq = 1 if self
+00036280: 2e71 7565 7279 5f63 6f75 6e74 203c 2075  .query_count < u
+00036290: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
+000362a0: 7465 725f 6672 6571 2065 6c73 6520 300d  ter_freq else 0.
+000362b0: 0a20 2020 2020 2020 206e 6f74 5f75 7064  .        not_upd
+000362c0: 6174 655f 636f 6e64 5f74 696d 6520 3d20  ate_cond_time = 
+000362d0: 3120 6966 2074 696d 652e 7469 6d65 2829  1 if time.time()
+000362e0: 202d 2073 656c 662e 6265 6769 6e5f 7469   - self.begin_ti
+000362f0: 6d65 203c 2075 7064 6174 655f 7365 7373  me < update_sess
+00036300: 696f 6e5f 6166 7465 725f 7365 636f 6e64  ion_after_second
+00036310: 7320 656c 7365 2030 0d0a 2020 2020 2020  s else 0..      
+00036320: 2020 6966 206e 6f74 2028 7365 6c66 2e73    if not (self.s
+00036330: 6573 7369 6f6e 2061 6e64 2073 656c 662e  ession and self.
+00036340: 6c61 6e67 7561 6765 5f6d 6170 2061 6e64  language_map and
+00036350: 206e 6f74 5f75 7064 6174 655f 636f 6e64   not_update_cond
+00036360: 5f66 7265 7120 616e 6420 6e6f 745f 7570  _freq and not_up
+00036370: 6461 7465 5f63 6f6e 645f 7469 6d65 293a  date_cond_time):
+00036380: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00036390: 6c66 2e73 6573 7369 6f6e 203d 2072 6571  lf.session = req
+000363a0: 7565 7374 732e 5365 7373 696f 6e28 290d  uests.Session().
+000363b0: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
+000363c0: 2073 656c 662e 7365 7373 696f 6e2e 6765   self.session.ge
+000363d0: 7428 7365 6c66 2e68 6f73 745f 7572 6c2c  t(self.host_url,
+000363e0: 2068 6561 6465 7273 3d73 656c 662e 686f   headers=self.ho
+000363f0: 7374 5f68 6561 6465 7273 2c20 7469 6d65  st_headers, time
+00036400: 6f75 743d 7469 6d65 6f75 742c 2070 726f  out=timeout, pro
+00036410: 7869 6573 3d70 726f 7869 6573 290d 0a20  xies=proxies).. 
+00036420: 2020 2020 2020 2020 2020 205f 203d 2073             _ = s
+00036430: 656c 662e 7365 7373 696f 6e2e 6765 7428  elf.session.get(
+00036440: 7365 6c66 2e67 6574 5f63 6f6f 6b69 655f  self.get_cookie_
+00036450: 7572 6c2c 2068 6561 6465 7273 3d73 656c  url, headers=sel
+00036460: 662e 6170 695f 6865 6164 6572 732c 2074  f.api_headers, t
+00036470: 696d 656f 7574 3d74 696d 656f 7574 2c20  imeout=timeout, 
+00036480: 7072 6f78 6965 733d 7072 6f78 6965 7329  proxies=proxies)
+00036490: 0d0a 2020 2020 2020 2020 2020 2020 645f  ..            d_
+000364a0: 6c61 6e67 5f6d 6170 203d 2073 656c 662e  lang_map = self.
+000364b0: 7365 7373 696f 6e2e 6765 7428 7365 6c66  session.get(self
+000364c0: 2e67 6574 5f6c 616e 675f 7572 6c2c 2068  .get_lang_url, h
+000364d0: 6561 6465 7273 3d73 656c 662e 6170 695f  eaders=self.api_
+000364e0: 6865 6164 6572 732c 2074 696d 656f 7574  headers, timeout
+000364f0: 3d74 696d 656f 7574 2c20 7072 6f78 6965  =timeout, proxie
+00036500: 733d 7072 6f78 6965 7329 2e6a 736f 6e28  s=proxies).json(
+00036510: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
+00036520: 6562 7567 5f6c 616e 675f 6b77 6172 6773  ebug_lang_kwargs
+00036530: 203d 2073 656c 662e 6465 6275 675f 6c61   = self.debug_la
+00036540: 6e67 5f6b 7761 7267 7328 6672 6f6d 5f6c  ng_kwargs(from_l
+00036550: 616e 6775 6167 652c 2074 6f5f 6c61 6e67  anguage, to_lang
+00036560: 7561 6765 2c20 7365 6c66 2e64 6566 6175  uage, self.defau
+00036570: 6c74 5f66 726f 6d5f 6c61 6e67 7561 6765  lt_from_language
+00036580: 2c20 6966 5f70 7269 6e74 5f77 6172 6e69  , if_print_warni
+00036590: 6e67 290d 0a20 2020 2020 2020 2020 2020  ng)..           
+000365a0: 2073 656c 662e 6c61 6e67 7561 6765 5f6d   self.language_m
+000365b0: 6170 203d 2073 656c 662e 6765 745f 6c61  ap = self.get_la
+000365c0: 6e67 7561 6765 5f6d 6170 2864 5f6c 616e  nguage_map(d_lan
+000365d0: 675f 6d61 702c 202a 2a64 6562 7567 5f6c  g_map, **debug_l
+000365e0: 616e 675f 6b77 6172 6773 290d 0a20 2020  ang_kwargs)..   
+000365f0: 2020 2020 2020 2020 2073 656c 662e 6c61           self.la
+00036600: 6e67 7061 6972 5f64 6f6d 6169 6e20 3d20  ngpair_domain = 
+00036610: 7365 6c66 2e67 6574 5f6c 616e 6770 6169  self.get_langpai
+00036620: 725f 646f 6d61 696e 2864 5f6c 616e 675f  r_domain(d_lang_
+00036630: 6d61 7029 0d0a 2020 2020 2020 2020 2020  map)..          
+00036640: 2020 7365 6c66 2e70 726f 6665 7373 696f    self.professio
+00036650: 6e61 6c5f 6669 656c 6420 3d20 7365 6c66  nal_field = self
+00036660: 2e67 6574 5f70 726f 6665 7373 696f 6e61  .get_professiona
+00036670: 6c5f 6669 656c 645f 6c69 7374 2864 5f6c  l_field_list(d_l
+00036680: 616e 675f 6d61 7029 0d0a 0d0a 2020 2020  ang_map)....    
+00036690: 2020 2020 6966 2066 726f 6d5f 6c61 6e67      if from_lang
+000366a0: 7561 6765 203d 3d20 2761 7574 6f27 3a0d  uage == 'auto':.
+000366b0: 0a20 2020 2020 2020 2020 2020 2070 6179  .            pay
+000366c0: 6c6f 6164 203d 207b 2774 6578 7427 3a20  load = {'text': 
+000366d0: 7175 6572 795f 7465 7874 7d0d 0a20 2020  query_text}..   
+000366e0: 2020 2020 2020 2020 2072 203d 2073 656c           r = sel
+000366f0: 662e 7365 7373 696f 6e2e 706f 7374 2873  f.session.post(s
+00036700: 656c 662e 6465 7465 6374 5f6c 616e 675f  elf.detect_lang_
+00036710: 7572 6c2c 206a 736f 6e3d 7061 796c 6f61  url, json=payloa
+00036720: 642c 2068 6561 6465 7273 3d73 656c 662e  d, headers=self.
+00036730: 6170 695f 6865 6164 6572 732c 2074 696d  api_headers, tim
+00036740: 656f 7574 3d74 696d 656f 7574 2c20 7072  eout=timeout, pr
+00036750: 6f78 6965 733d 7072 6f78 6965 7329 0d0a  oxies=proxies)..
+00036760: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
+00036770: 5f6c 616e 6775 6167 6520 3d20 722e 6a73  _language = r.js
+00036780: 6f6e 2829 5b27 6461 7461 275d 5b27 6c61  on()['data']['la
+00036790: 6e67 7561 6765 275d 0d0a 2020 2020 2020  nguage']..      
+000367a0: 2020 6672 6f6d 5f6c 616e 6775 6167 652c    from_language,
+000367b0: 2074 6f5f 6c61 6e67 7561 6765 203d 2066   to_language = f
+000367c0: 726f 6d5f 6c61 6e67 7561 6765 2e6c 6f77  rom_language.low
+000367d0: 6572 2829 2c20 746f 5f6c 616e 6775 6167  er(), to_languag
+000367e0: 652e 6c6f 7765 7228 2920 2023 206d 7573  e.lower()  # mus
+000367f0: 7420 6c6f 7765 720d 0a20 2020 2020 2020  t lower..       
+00036800: 2066 726f 6d5f 6c61 6e67 7561 6765 2c20   from_language, 
+00036810: 746f 5f6c 616e 6775 6167 6520 3d20 7365  to_language = se
+00036820: 6c66 2e63 6865 636b 5f6c 616e 6775 6167  lf.check_languag
+00036830: 6528 6672 6f6d 5f6c 616e 6775 6167 652c  e(from_language,
+00036840: 2074 6f5f 6c61 6e67 7561 6765 2c20 7365   to_language, se
+00036850: 6c66 2e6c 616e 6775 6167 655f 6d61 702c  lf.language_map,
+00036860: 206f 7574 7075 745f 7a68 3d73 656c 662e   output_zh=self.
+00036870: 6f75 7470 7574 5f7a 682c 0d0a 2020 2020  output_zh,..    
+00036880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00036890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000368a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000368b0: 2020 2020 206f 7574 7075 745f 656e 5f74       output_en_t
+000368c0: 7261 6e73 6c61 746f 723d 2763 6c6f 7564  ranslator='cloud
+000368d0: 5969 272c 206f 7574 7075 745f 656e 3d73  Yi', output_en=s
+000368e0: 656c 662e 6f75 7470 7574 5f65 6e29 0d0a  elf.output_en)..
+000368f0: 0d0a 2020 2020 2020 2020 646f 6d61 696e  ..        domain
+00036900: 7320 3d20 7365 6c66 2e6c 616e 6770 6169  s = self.langpai
+00036910: 725f 646f 6d61 696e 2e67 6574 2866 277b  r_domain.get(f'{
+00036920: 6672 6f6d 5f6c 616e 6775 6167 657d 5f7b  from_language}_{
+00036930: 746f 5f6c 616e 6775 6167 657d 2729 0d0a  to_language}')..
+00036940: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
+00036950: 6f6d 6169 6e73 3a0d 0a20 2020 2020 2020  omains:..       
+00036960: 2020 2020 2072 6169 7365 2054 7261 6e73       raise Trans
+00036970: 6c61 746f 7245 7272 6f72 0d0a 2020 2020  latorError..    
+00036980: 2020 2020 6966 2075 7365 5f64 6f6d 6169      if use_domai
+00036990: 6e20 6e6f 7420 696e 2064 6f6d 6169 6e73  n not in domains
+000369a0: 3a0d 0a20 2020 2020 2020 2020 2020 2075  :..            u
+000369b0: 7365 5f64 6f6d 6169 6e20 3d20 646f 6d61  se_domain = doma
+000369c0: 696e 735b 305d 0d0a 0d0a 2020 2020 2020  ins[0]....      
+000369d0: 2020 7061 796c 6f61 6420 3d20 7b0d 0a20    payload = {.. 
+000369e0: 2020 2020 2020 2020 2020 2027 7465 7874             'text
+000369f0: 273a 2071 7565 7279 5f74 6578 742c 0d0a  ': query_text,..
+00036a00: 2020 2020 2020 2020 2020 2020 2764 6f6d              'dom
+00036a10: 6169 6e27 3a20 7573 655f 646f 6d61 696e  ain': use_domain
+00036a20: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
+00036a30: 7372 634c 616e 6743 6f64 6527 3a20 6672  srcLangCode': fr
+00036a40: 6f6d 5f6c 616e 6775 6167 652c 0d0a 2020  om_language,..  
+00036a50: 2020 2020 2020 2020 2020 2774 6774 4c61            'tgtLa
+00036a60: 6e67 436f 6465 273a 2074 6f5f 6c61 6e67  ngCode': to_lang
+00036a70: 7561 6765 2c0d 0a20 2020 2020 2020 207d  uage,..        }
+00036a80: 0d0a 2020 2020 2020 2020 7220 3d20 7365  ..        r = se
+00036a90: 6c66 2e73 6573 7369 6f6e 2e70 6f73 7428  lf.session.post(
+00036aa0: 7365 6c66 2e61 7069 5f75 726c 2c20 6a73  self.api_url, js
+00036ab0: 6f6e 3d70 6179 6c6f 6164 2c20 6865 6164  on=payload, head
+00036ac0: 6572 733d 7365 6c66 2e61 7069 5f68 6561  ers=self.api_hea
+00036ad0: 6465 7273 2c20 7469 6d65 6f75 743d 7469  ders, timeout=ti
+00036ae0: 6d65 6f75 742c 2070 726f 7869 6573 3d70  meout, proxies=p
+00036af0: 726f 7869 6573 290d 0a20 2020 2020 2020  roxies)..       
+00036b00: 2072 2e72 6169 7365 5f66 6f72 5f73 7461   r.raise_for_sta
+00036b10: 7475 7328 290d 0a20 2020 2020 2020 2064  tus()..        d
+00036b20: 6174 6120 3d20 722e 6a73 6f6e 2829 0d0a  ata = r.json()..
+00036b30: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
+00036b40: 6570 2873 6c65 6570 5f73 6563 6f6e 6473  ep(sleep_seconds
+00036b50: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00036b60: 7175 6572 795f 636f 756e 7420 2b3d 2031  query_count += 1
+00036b70: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00036b80: 2064 6174 6120 6966 2069 735f 6465 7461   data if is_deta
+00036b90: 696c 5f72 6573 756c 7420 656c 7365 2064  il_result else d
+00036ba0: 6174 615b 2764 6174 6127 5d5b 2774 7261  ata['data']['tra
+00036bb0: 6e73 6c61 7469 6f6e 275d 0d0a 0d0a 0d0a  nslation']......
+00036bc0: 636c 6173 7320 5379 7354 7261 6e28 5473  class SysTran(Ts
+00036bd0: 6529 3a0d 0a20 2020 2064 6566 205f 5f69  e):..    def __i
+00036be0: 6e69 745f 5f28 7365 6c66 293a 0d0a 2020  nit__(self):..  
+00036bf0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+00036c00: 696e 6974 5f5f 2829 0d0a 2020 2020 2020  init__()..      
+00036c10: 2020 7365 6c66 2e68 6f6d 655f 7572 6c20    self.home_url 
+00036c20: 3d20 2768 7474 7073 3a2f 2f77 7777 2e73  = 'https://www.s
+00036c30: 7973 7472 616e 2e6e 6574 270d 0a20 2020  ystran.net'..   
+00036c40: 2020 2020 2073 656c 662e 686f 7374 5f75       self.host_u
+00036c50: 726c 203d 2027 6874 7470 733a 2f2f 7777  rl = 'https://ww
+00036c60: 772e 7379 7374 7261 6e2e 6e65 742f 7472  w.systran.net/tr
+00036c70: 616e 736c 6174 652f 270d 0a20 2020 2020  anslate/'..     
+00036c80: 2020 2073 656c 662e 6170 695f 7572 6c20     self.api_url 
+00036c90: 3d20 2768 7474 7073 3a2f 2f61 7069 2d74  = 'https://api-t
+00036ca0: 7261 6e73 6c61 7465 2e73 7973 7472 616e  ranslate.systran
+00036cb0: 2e6e 6574 2f74 7261 6e73 6c61 7469 6f6e  .net/translation
+00036cc0: 2f74 6578 742f 7472 616e 736c 6174 6527  /text/translate'
+00036cd0: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
+00036ce0: 6574 5f6c 616e 675f 7572 6c20 3d20 2768  et_lang_url = 'h
+00036cf0: 7474 7073 3a2f 2f61 7069 2d74 7261 6e73  ttps://api-trans
+00036d00: 6c61 7465 2e73 7973 7472 616e 2e6e 6574  late.systran.net
+00036d10: 2f74 7261 6e73 6c61 7469 6f6e 2f73 7570  /translation/sup
+00036d20: 706f 7274 6564 4c61 6e67 7561 6765 7327  portedLanguages'
+00036d30: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
+00036d40: 6574 5f74 6f6b 656e 5f75 726c 203d 2027  et_token_url = '
+00036d50: 6874 7470 733a 2f2f 7472 616e 736c 6174  https://translat
+00036d60: 652e 7379 7374 7261 6e2e 6e65 742f 6f69  e.systran.net/oi
+00036d70: 6463 2f74 6f6b 656e 270d 0a20 2020 2020  dc/token'..     
+00036d80: 2020 2073 656c 662e 6765 745f 636c 6965     self.get_clie
+00036d90: 6e74 5f75 726c 203d 2027 6874 7470 733a  nt_url = 'https:
+00036da0: 2f2f 7777 772e 7379 7374 7261 6e2e 6e65  //www.systran.ne
+00036db0: 742f 7770 2d63 6f6e 7465 6e74 2f74 6865  t/wp-content/the
+00036dc0: 6d65 732f 7379 7374 7261 6e2f 7472 616e  mes/systran/tran
+00036dd0: 736c 6174 6f72 2f6a 732f 7472 616e 736c  slator/js/transl
+00036de0: 6174 6542 6f78 2e62 756e 646c 652e 6a73  ateBox.bundle.js
+00036df0: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+00036e00: 686f 7374 5f68 6561 6465 7273 203d 2073  host_headers = s
+00036e10: 656c 662e 6765 745f 6865 6164 6572 7328  elf.get_headers(
+00036e20: 7365 6c66 2e68 6f6d 655f 7572 6c2c 2069  self.home_url, i
+00036e30: 665f 6170 693d 4661 6c73 652c 2069 665f  f_api=False, if_
+00036e40: 7265 6665 7265 725f 666f 725f 686f 7374  referer_for_host
+00036e50: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00036e60: 7365 6c66 2e61 7069 5f61 6a61 785f 6865  self.api_ajax_he
+00036e70: 6164 6572 7320 3d20 7365 6c66 2e67 6574  aders = self.get
+00036e80: 5f68 6561 6465 7273 2873 656c 662e 686f  _headers(self.ho
+00036e90: 6d65 5f75 726c 2c20 6966 5f61 7069 3d54  me_url, if_api=T
+00036ea0: 7275 652c 2069 665f 616a 6178 5f66 6f72  rue, if_ajax_for
+00036eb0: 5f61 7069 3d54 7275 6529 0d0a 2020 2020  _api=True)..    
+00036ec0: 2020 2020 7365 6c66 2e61 7069 5f6a 736f      self.api_jso
+00036ed0: 6e5f 6865 6164 6572 7320 3d20 7365 6c66  n_headers = self
+00036ee0: 2e67 6574 5f68 6561 6465 7273 2873 656c  .get_headers(sel
+00036ef0: 662e 686f 6d65 5f75 726c 2c20 6966 5f61  f.home_url, if_a
+00036f00: 7069 3d54 7275 652c 2069 665f 6a73 6f6e  pi=True, if_json
+00036f10: 5f66 6f72 5f61 7069 3d54 7275 6529 0d0a  _for_api=True)..
+00036f20: 2020 2020 2020 2020 7365 6c66 2e73 6573          self.ses
+00036f30: 7369 6f6e 203d 204e 6f6e 650d 0a20 2020  sion = None..   
+00036f40: 2020 2020 2073 656c 662e 6c61 6e67 7561       self.langua
+00036f50: 6765 5f6d 6170 203d 204e 6f6e 650d 0a20  ge_map = None.. 
+00036f60: 2020 2020 2020 2073 656c 662e 7072 6f66         self.prof
+00036f70: 6573 7369 6f6e 616c 5f66 6965 6c64 203d  essional_field =
+00036f80: 204e 6f6e 650d 0a20 2020 2020 2020 2073   None..        s
+00036f90: 656c 662e 6c61 6e67 7061 6972 5f64 6f6d  elf.langpair_dom
+00036fa0: 6169 6e20 3d20 4e6f 6e65 0d0a 2020 2020  ain = None..    
+00036fb0: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
+00036fc0: 6461 7461 203d 204e 6f6e 650d 0a20 2020  data = None..   
+00036fd0: 2020 2020 2073 656c 662e 746f 6b65 6e5f       self.token_
+00036fe0: 6461 7461 203d 204e 6f6e 650d 0a20 2020  data = None..   
+00036ff0: 2020 2020 2073 656c 662e 7175 6572 795f       self.query_
+00037000: 636f 756e 7420 3d20 300d 0a20 2020 2020  count = 0..     
+00037010: 2020 2073 656c 662e 6f75 7470 7574 5f7a     self.output_z
+00037020: 6820 3d20 277a 6827 0d0a 2020 2020 2020  h = 'zh'..      
+00037030: 2020 7365 6c66 2e69 6e70 7574 5f6c 696d    self.input_lim
+00037040: 6974 203d 2069 6e74 2835 6533 290d 0a20  it = int(5e3).. 
+00037050: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
+00037060: 756c 745f 6672 6f6d 5f6c 616e 6775 6167  ult_from_languag
+00037070: 6520 3d20 7365 6c66 2e6f 7574 7075 745f  e = self.output_
+00037080: 7a68 0d0a 0d0a 2020 2020 4054 7365 2e64  zh....    @Tse.d
+00037090: 6562 7567 5f6c 616e 6775 6167 655f 6d61  ebug_language_ma
+000370a0: 700d 0a20 2020 2064 6566 2067 6574 5f6c  p..    def get_l
+000370b0: 616e 6775 6167 655f 6d61 7028 7365 6c66  anguage_map(self
+000370c0: 2c20 645f 6c61 6e67 5f6d 6170 3a20 6469  , d_lang_map: di
+000370d0: 6374 2c20 2a2a 6b77 6172 6773 3a20 4c61  ct, **kwargs: La
+000370e0: 6e67 4d61 704b 7761 7267 7354 7970 6529  ngMapKwargsType)
+000370f0: 202d 3e20 6469 6374 3a0d 0a20 2020 2020   -> dict:..     
+00037100: 2020 2072 6574 7572 6e20 7b69 695b 2773     return {ii['s
+00037110: 6f75 7263 6527 5d3a 205b 6a6a 5b27 7461  ource']: [jj['ta
+00037120: 7267 6574 275d 2066 6f72 206a 6a20 696e  rget'] for jj in
+00037130: 2064 5f6c 616e 675f 6d61 705b 276c 616e   d_lang_map['lan
+00037140: 6775 6167 6550 6169 7273 275d 2069 6620  guagePairs'] if 
+00037150: 6a6a 5b27 736f 7572 6365 275d 203d 3d20  jj['source'] == 
+00037160: 6969 5b27 736f 7572 6365 275d 5d20 666f  ii['source']] fo
+00037170: 7220 6969 2069 6e20 645f 6c61 6e67 5f6d  r ii in d_lang_m
+00037180: 6170 5b27 6c61 6e67 7561 6765 5061 6972  ap['languagePair
+00037190: 7327 5d7d 0d0a 0d0a 2020 2020 6465 6620  s']}....    def 
+000371a0: 6765 745f 7072 6f66 6573 7369 6f6e 616c  get_professional
+000371b0: 5f66 6965 6c64 5f6c 6973 7428 7365 6c66  _field_list(self
+000371c0: 2c20 645f 6c61 6e67 5f6d 6170 3a20 6469  , d_lang_map: di
+000371d0: 6374 2920 2d3e 2073 6574 3a0d 0a20 2020  ct) -> set:..   
+000371e0: 2020 2020 2072 6574 7572 6e20 7b69 745b       return {it[
+000371f0: 2773 656c 6563 746f 7273 275d 5b27 646f  'selectors']['do
+00037200: 6d61 696e 275d 2066 6f72 2069 7465 6d20  main'] for item 
+00037210: 696e 2064 5f6c 616e 675f 6d61 705b 276c  in d_lang_map['l
+00037220: 616e 6775 6167 6550 6169 7273 275d 2066  anguagePairs'] f
+00037230: 6f72 2069 7420 696e 2069 7465 6d5b 2770  or it in item['p
+00037240: 726f 6669 6c65 7327 5d7d 0d0a 0d0a 2020  rofiles']}....  
+00037250: 2020 6465 6620 6765 745f 6c61 6e67 7061    def get_langpa
+00037260: 6972 5f64 6f6d 6169 6e28 7365 6c66 2c20  ir_domain(self, 
+00037270: 645f 6c61 6e67 5f6d 6170 3a20 6469 6374  d_lang_map: dict
+00037280: 2920 2d3e 2064 6963 743a 0d0a 2020 2020  ) -> dict:..    
+00037290: 2020 2020 6461 7461 203d 207b 0d0a 2020      data = {..  
+000372a0: 2020 2020 2020 2020 2020 6627 7b69 7465            f'{ite
+000372b0: 6d5b 2273 6f75 7263 6522 5d7d 5f5f 7b69  m["source"]}__{i
+000372c0: 7465 6d5b 2274 6172 6765 7422 5d7d 5f5f  tem["target"]}__
+000372d0: 7b69 745b 2273 656c 6563 746f 7273 225d  {it["selectors"]
+000372e0: 5b22 646f 6d61 696e 225d 7d27 3a20 7b0d  ["domain"]}': {.
+000372f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00037300: 2027 646f 6d61 696e 273a 2069 745b 2273   'domain': it["s
+00037310: 656c 6563 746f 7273 225d 5b22 646f 6d61  electors"]["doma
+00037320: 696e 225d 2c0d 0a20 2020 2020 2020 2020  in"],..         
+00037330: 2020 2020 2020 2027 6f77 6e65 7227 3a20         'owner': 
+00037340: 6974 5b27 7365 6c65 6374 6f72 7327 5d5b  it['selectors'][
+00037350: 276f 776e 6572 275d 2c0d 0a20 2020 2020  'owner'],..     
+00037360: 2020 2020 2020 2020 2020 2027 7369 7a65             'size
+00037370: 273a 2069 745b 2773 656c 6563 746f 7273  ': it['selectors
+00037380: 275d 5b27 7369 7a65 275d 2c0d 0a20 2020  ']['size'],..   
+00037390: 2020 2020 2020 2020 207d 2066 6f72 2069           } for i
+000373a0: 7465 6d20 696e 2064 5f6c 616e 675f 6d61  tem in d_lang_ma
+000373b0: 705b 276c 616e 6775 6167 6550 6169 7273  p['languagePairs
+000373c0: 275d 2066 6f72 2069 7420 696e 2069 7465  '] for it in ite
+000373d0: 6d5b 2770 726f 6669 6c65 7327 5d0d 0a20  m['profiles'].. 
+000373e0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+000373f0: 2020 7265 7475 726e 2064 6174 610d 0a0d    return data...
+00037400: 0a20 2020 2064 6566 2067 6574 5f63 6c69  .    def get_cli
+00037410: 656e 745f 6461 7461 2873 656c 662c 2063  ent_data(self, c
+00037420: 6c69 656e 745f 7572 6c3a 2073 7472 2c20  lient_url: str, 
+00037430: 7373 3a20 5365 7373 696f 6e54 7970 652c  ss: SessionType,
+00037440: 2068 6561 6465 7273 3a20 6469 6374 2c20   headers: dict, 
+00037450: 7469 6d65 6f75 743a 2066 6c6f 6174 2c20  timeout: float, 
+00037460: 7072 6f78 6965 733a 2064 6963 7429 202d  proxies: dict) -
+00037470: 3e20 6469 6374 3a0d 0a20 2020 2020 2020  > dict:..       
+00037480: 206a 735f 6874 6d6c 203d 2073 732e 6765   js_html = ss.ge
+00037490: 7428 636c 6965 6e74 5f75 726c 2c20 6865  t(client_url, he
+000374a0: 6164 6572 733d 6865 6164 6572 732c 2074  aders=headers, t
+000374b0: 696d 656f 7574 3d74 696d 656f 7574 2c20  imeout=timeout, 
+000374c0: 7072 6f78 6965 733d 7072 6f78 6965 7329  proxies=proxies)
+000374d0: 2e74 6578 740d 0a20 2020 2020 2020 2073  .text..        s
+000374e0: 6561 7263 685f 6772 6f75 7073 203d 2072  earch_groups = r
+000374f0: 652e 636f 6d70 696c 6528 2722 6874 7470  e.compile('"http
+00037500: 733a 2f2f 7472 616e 736c 6174 652e 7379  s://translate.sy
+00037510: 7374 7261 6e2e 6e65 742f 6f69 6463 222c  stran.net/oidc",
+00037520: 5c5c 773d 2228 2e2a 3f29 222c 5c5c 773d  \\w="(.*?)",\\w=
+00037530: 2228 2e2a 3f29 223b 2729 2e73 6561 7263  "(.*?)";').searc
+00037540: 6828 6a73 5f68 746d 6c29 2020 2320 5c5c  h(js_html)  # \\
+00037550: 777b 317d 203d 3d20 5c5c 770d 0a20 2020  w{1} == \\w..   
+00037560: 2020 2020 2063 6c69 656e 745f 6461 7461       client_data
+00037570: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
+00037580: 2020 2767 7261 6e74 5f74 7970 6527 3a20    'grant_type': 
+00037590: 2763 6c69 656e 745f 6372 6564 656e 7469  'client_credenti
+000375a0: 616c 7327 2c0d 0a20 2020 2020 2020 2020  als',..         
+000375b0: 2020 2027 636c 6965 6e74 5f69 6427 3a20     'client_id': 
+000375c0: 7365 6172 6368 5f67 726f 7570 732e 6772  search_groups.gr
+000375d0: 6f75 7028 3129 2c0d 0a20 2020 2020 2020  oup(1),..       
+000375e0: 2020 2020 2027 636c 6965 6e74 5f73 6563       'client_sec
+000375f0: 7265 7427 3a20 7365 6172 6368 5f67 726f  ret': search_gro
+00037600: 7570 732e 6772 6f75 7028 3229 2c0d 0a20  ups.group(2),.. 
+00037610: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00037620: 2020 7265 7475 726e 2063 6c69 656e 745f    return client_
+00037630: 6461 7461 0d0a 0d0a 2020 2020 4054 7365  data....    @Tse
+00037640: 2e74 696d 655f 7374 6174 0d0a 2020 2020  .time_stat..    
+00037650: 4054 7365 2e63 6865 636b 5f71 7565 7279  @Tse.check_query
+00037660: 0d0a 2020 2020 6465 6620 7379 7354 7261  ..    def sysTra
+00037670: 6e5f 6170 6928 7365 6c66 2c20 7175 6572  n_api(self, quer
+00037680: 795f 7465 7874 3a20 7374 722c 2066 726f  y_text: str, fro
+00037690: 6d5f 6c61 6e67 7561 6765 3a20 7374 7220  m_language: str 
+000376a0: 3d20 2761 7574 6f27 2c20 746f 5f6c 616e  = 'auto', to_lan
+000376b0: 6775 6167 653a 2073 7472 203d 2027 656e  guage: str = 'en
+000376c0: 272c 202a 2a6b 7761 7267 733a 2041 7069  ', **kwargs: Api
+000376d0: 4b77 6172 6773 5479 7065 2920 2d3e 2055  KwargsType) -> U
+000376e0: 6e69 6f6e 5b73 7472 2c20 6469 6374 5d3a  nion[str, dict]:
+000376f0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00037700: 2020 2020 2020 2068 7474 7073 3a2f 2f77         https://w
+00037710: 7777 2e73 7973 7472 616e 2e6e 6574 2f74  ww.systran.net/t
+00037720: 7261 6e73 6c61 7465 2f0d 0a20 2020 2020  ranslate/..     
+00037730: 2020 203a 7061 7261 6d20 7175 6572 795f     :param query_
+00037740: 7465 7874 3a20 7374 722c 206d 7573 742e  text: str, must.
+00037750: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00037760: 2066 726f 6d5f 6c61 6e67 7561 6765 3a20   from_language: 
+00037770: 7374 722c 2064 6566 6175 6c74 2027 6175  str, default 'au
+00037780: 746f 272e 0d0a 2020 2020 2020 2020 3a70  to'...        :p
+00037790: 6172 616d 2074 6f5f 6c61 6e67 7561 6765  aram to_language
+000377a0: 3a20 7374 722c 2064 6566 6175 6c74 2027  : str, default '
+000377b0: 656e 272e 0d0a 2020 2020 2020 2020 3a70  en'...        :p
+000377c0: 6172 616d 202a 2a6b 7761 7267 733a 0d0a  aram **kwargs:..
+000377d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000377e0: 3a70 6172 616d 2074 696d 656f 7574 3a20  :param timeout: 
+000377f0: 666c 6f61 742c 2064 6566 6175 6c74 204e  float, default N
+00037800: 6f6e 652e 0d0a 2020 2020 2020 2020 2020  one...          
+00037810: 2020 2020 2020 3a70 6172 616d 2070 726f        :param pro
+00037820: 7869 6573 3a20 6469 6374 2c20 6465 6661  xies: dict, defa
+00037830: 756c 7420 4e6f 6e65 2e0d 0a20 2020 2020  ult None...     
+00037840: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00037850: 6d20 736c 6565 705f 7365 636f 6e64 733a  m sleep_seconds:
+00037860: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
+00037870: 302e 0d0a 2020 2020 2020 2020 2020 2020  0...            
+00037880: 2020 2020 3a70 6172 616d 2069 735f 6465      :param is_de
+00037890: 7461 696c 5f72 6573 756c 743a 2062 6f6f  tail_result: boo
+000378a0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+000378b0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000378c0: 2020 203a 7061 7261 6d20 6966 5f69 676e     :param if_ign
+000378d0: 6f72 655f 6c69 6d69 745f 6f66 5f6c 656e  ore_limit_of_len
+000378e0: 6774 683a 2062 6f6f 6c2c 2064 6566 6175  gth: bool, defau
+000378f0: 6c74 2046 616c 7365 2e0d 0a20 2020 2020  lt False...     
+00037900: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00037910: 6d20 6c69 6d69 745f 6f66 5f6c 656e 6774  m limit_of_lengt
+00037920: 683a 2069 6e74 2c20 6465 6661 756c 7420  h: int, default 
+00037930: 3230 3030 302e 0d0a 2020 2020 2020 2020  20000...        
+00037940: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+00037950: 665f 6967 6e6f 7265 5f65 6d70 7479 5f71  f_ignore_empty_q
+00037960: 7565 7279 3a20 626f 6f6c 2c20 6465 6661  uery: bool, defa
+00037970: 756c 7420 4661 6c73 652e 0d0a 2020 2020  ult False...    
+00037980: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00037990: 616d 2075 7064 6174 655f 7365 7373 696f  am update_sessio
+000379a0: 6e5f 6166 7465 725f 6672 6571 3a20 696e  n_after_freq: in
+000379b0: 742c 2064 6566 6175 6c74 2031 3030 302e  t, default 1000.
+000379c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000379d0: 2020 3a70 6172 616d 2075 7064 6174 655f    :param update_
+000379e0: 7365 7373 696f 6e5f 6166 7465 725f 7365  session_after_se
+000379f0: 636f 6e64 733a 2066 6c6f 6174 2c20 6465  conds: float, de
+00037a00: 6661 756c 7420 3135 3030 2e0d 0a20 2020  fault 1500...   
+00037a10: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+00037a20: 7261 6d20 6966 5f73 686f 775f 7469 6d65  ram if_show_time
+00037a30: 5f73 7461 743a 2062 6f6f 6c2c 2064 6566  _stat: bool, def
+00037a40: 6175 6c74 2046 616c 7365 2e0d 0a20 2020  ault False...   
+00037a50: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+00037a60: 7261 6d20 7368 6f77 5f74 696d 655f 7374  ram show_time_st
+00037a70: 6174 5f70 7265 6369 7369 6f6e 3a20 696e  at_precision: in
+00037a80: 742c 2064 6566 6175 6c74 2032 2e0d 0a20  t, default 2... 
+00037a90: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+00037aa0: 7061 7261 6d20 6966 5f70 7269 6e74 5f77  param if_print_w
+00037ab0: 6172 6e69 6e67 3a20 626f 6f6c 2c20 6465  arning: bool, de
+00037ac0: 6661 756c 7420 5472 7565 2e0d 0a20 2020  fault True...   
+00037ad0: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+00037ae0: 7261 6d20 7072 6f66 6573 7369 6f6e 616c  ram professional
+00037af0: 5f66 6965 6c64 3a20 7374 722c 2064 6566  _field: str, def
+00037b00: 6175 6c74 204e 6f6e 652e 0d0a 2020 2020  ault None...    
+00037b10: 2020 2020 3a72 6574 7572 6e3a 2073 7472      :return: str
+00037b20: 206f 7220 6469 6374 0d0a 2020 2020 2020   or dict..      
+00037b30: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
+00037b40: 2075 7365 5f64 6f6d 6169 6e20 3d20 6b77   use_domain = kw
+00037b50: 6172 6773 2e67 6574 2827 7072 6f66 6573  args.get('profes
+00037b60: 7369 6f6e 616c 5f66 6965 6c64 272c 2027  sional_field', '
+00037b70: 4765 6e65 7269 6327 290d 0a20 2020 2020  Generic')..     
+00037b80: 2020 2074 696d 656f 7574 203d 206b 7761     timeout = kwa
+00037b90: 7267 732e 6765 7428 2774 696d 656f 7574  rgs.get('timeout
+00037ba0: 272c 204e 6f6e 6529 0d0a 2020 2020 2020  ', None)..      
+00037bb0: 2020 7072 6f78 6965 7320 3d20 6b77 6172    proxies = kwar
+00037bc0: 6773 2e67 6574 2827 7072 6f78 6965 7327  gs.get('proxies'
+00037bd0: 2c20 4e6f 6e65 290d 0a20 2020 2020 2020  , None)..       
+00037be0: 2073 6c65 6570 5f73 6563 6f6e 6473 203d   sleep_seconds =
+00037bf0: 206b 7761 7267 732e 6765 7428 2773 6c65   kwargs.get('sle
+00037c00: 6570 5f73 6563 6f6e 6473 272c 2030 290d  ep_seconds', 0).
+00037c10: 0a20 2020 2020 2020 2069 665f 7072 696e  .        if_prin
+00037c20: 745f 7761 726e 696e 6720 3d20 6b77 6172  t_warning = kwar
+00037c30: 6773 2e67 6574 2827 6966 5f70 7269 6e74  gs.get('if_print
+00037c40: 5f77 6172 6e69 6e67 272c 2054 7275 6529  _warning', True)
+00037c50: 0d0a 2020 2020 2020 2020 6973 5f64 6574  ..        is_det
+00037c60: 6169 6c5f 7265 7375 6c74 203d 206b 7761  ail_result = kwa
+00037c70: 7267 732e 6765 7428 2769 735f 6465 7461  rgs.get('is_deta
+00037c80: 696c 5f72 6573 756c 7427 2c20 4661 6c73  il_result', Fals
+00037c90: 6529 0d0a 2020 2020 2020 2020 7570 6461  e)..        upda
+00037ca0: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
+00037cb0: 5f66 7265 7120 3d20 6b77 6172 6773 2e67  _freq = kwargs.g
+00037cc0: 6574 2827 7570 6461 7465 5f73 6573 7369  et('update_sessi
+00037cd0: 6f6e 5f61 6674 6572 5f66 7265 7127 2c20  on_after_freq', 
+00037ce0: 7365 6c66 2e64 6566 6175 6c74 5f73 6573  self.default_ses
+00037cf0: 7369 6f6e 5f66 7265 7129 0d0a 2020 2020  sion_freq)..    
+00037d00: 2020 2020 7570 6461 7465 5f73 6573 7369      update_sessi
+00037d10: 6f6e 5f61 6674 6572 5f73 6563 6f6e 6473  on_after_seconds
+00037d20: 203d 206b 7761 7267 732e 6765 7428 2775   = kwargs.get('u
+00037d30: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
+00037d40: 7465 725f 7365 636f 6e64 7327 2c20 7365  ter_seconds', se
+00037d50: 6c66 2e64 6566 6175 6c74 5f73 6573 7369  lf.default_sessi
+00037d60: 6f6e 5f73 6563 6f6e 6473 290d 0a20 2020  on_seconds)..   
+00037d70: 2020 2020 2073 656c 662e 6368 6563 6b5f       self.check_
+00037d80: 696e 7075 745f 6c69 6d69 7428 7175 6572  input_limit(quer
+00037d90: 795f 7465 7874 2c20 7365 6c66 2e69 6e70  y_text, self.inp
+00037da0: 7574 5f6c 696d 6974 290d 0a0d 0a20 2020  ut_limit)....   
+00037db0: 2020 2020 206e 6f74 5f75 7064 6174 655f       not_update_
+00037dc0: 636f 6e64 5f66 7265 7120 3d20 3120 6966  cond_freq = 1 if
+00037dd0: 2073 656c 662e 7175 6572 795f 636f 756e   self.query_coun
+00037de0: 7420 3c20 7570 6461 7465 5f73 6573 7369  t < update_sessi
+00037df0: 6f6e 5f61 6674 6572 5f66 7265 7120 656c  on_after_freq el
+00037e00: 7365 2030 0d0a 2020 2020 2020 2020 6e6f  se 0..        no
+00037e10: 745f 7570 6461 7465 5f63 6f6e 645f 7469  t_update_cond_ti
+00037e20: 6d65 203d 2031 2069 6620 7469 6d65 2e74  me = 1 if time.t
+00037e30: 696d 6528 2920 2d20 7365 6c66 2e62 6567  ime() - self.beg
+00037e40: 696e 5f74 696d 6520 3c20 7570 6461 7465  in_time < update
+00037e50: 5f73 6573 7369 6f6e 5f61 6674 6572 5f73  _session_after_s
+00037e60: 6563 6f6e 6473 2065 6c73 6520 300d 0a20  econds else 0.. 
+00037e70: 2020 2020 2020 2069 6620 6e6f 7420 2873         if not (s
+00037e80: 656c 662e 7365 7373 696f 6e20 616e 6420  elf.session and 
+00037e90: 7365 6c66 2e6c 616e 6775 6167 655f 6d61  self.language_ma
+00037ea0: 7020 616e 6420 6e6f 745f 7570 6461 7465  p and not_update
+00037eb0: 5f63 6f6e 645f 6672 6571 2061 6e64 206e  _cond_freq and n
+00037ec0: 6f74 5f75 7064 6174 655f 636f 6e64 5f74  ot_update_cond_t
+00037ed0: 696d 6529 3a0d 0a20 2020 2020 2020 2020  ime):..         
+00037ee0: 2020 2073 656c 662e 7365 7373 696f 6e20     self.session 
+00037ef0: 3d20 7265 7175 6573 7473 2e53 6573 7369  = requests.Sessi
+00037f00: 6f6e 2829 0d0a 2020 2020 2020 2020 2020  on()..          
+00037f10: 2020 5f20 3d20 7365 6c66 2e73 6573 7369    _ = self.sessi
+00037f20: 6f6e 2e67 6574 2873 656c 662e 686f 7374  on.get(self.host
+00037f30: 5f75 726c 2c20 6865 6164 6572 733d 7365  _url, headers=se
+00037f40: 6c66 2e68 6f73 745f 6865 6164 6572 732c  lf.host_headers,
+00037f50: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
+00037f60: 2c20 7072 6f78 6965 733d 7072 6f78 6965  , proxies=proxie
+00037f70: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+00037f80: 7365 6c66 2e63 6c69 656e 745f 6461 7461  self.client_data
+00037f90: 203d 2073 656c 662e 6765 745f 636c 6965   = self.get_clie
+00037fa0: 6e74 5f64 6174 6128 7365 6c66 2e67 6574  nt_data(self.get
+00037fb0: 5f63 6c69 656e 745f 7572 6c2c 2073 656c  _client_url, sel
+00037fc0: 662e 7365 7373 696f 6e2c 2073 656c 662e  f.session, self.
+00037fd0: 686f 7374 5f68 6561 6465 7273 2c20 7469  host_headers, ti
+00037fe0: 6d65 6f75 742c 2070 726f 7869 6573 290d  meout, proxies).
+00037ff0: 0a20 2020 2020 2020 2020 2020 2070 6179  .            pay
+00038000: 6c6f 6164 203d 2075 726c 6c69 622e 7061  load = urllib.pa
+00038010: 7273 652e 7572 6c65 6e63 6f64 6528 7365  rse.urlencode(se
+00038020: 6c66 2e63 6c69 656e 745f 6461 7461 290d  lf.client_data).
+00038030: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00038040: 662e 746f 6b65 6e5f 6461 7461 203d 2073  f.token_data = s
+00038050: 656c 662e 7365 7373 696f 6e2e 706f 7374  elf.session.post
+00038060: 2873 656c 662e 6765 745f 746f 6b65 6e5f  (self.get_token_
+00038070: 7572 6c2c 2064 6174 613d 7061 796c 6f61  url, data=payloa
+00038080: 642c 2068 6561 6465 7273 3d73 656c 662e  d, headers=self.
+00038090: 6170 695f 616a 6178 5f68 6561 6465 7273  api_ajax_headers
+000380a0: 2c20 7469 6d65 6f75 743d 7469 6d65 6f75  , timeout=timeou
+000380b0: 742c 2070 726f 7869 6573 3d70 726f 7869  t, proxies=proxi
+000380c0: 6573 292e 6a73 6f6e 2829 0d0a 0d0a 2020  es).json()....  
+000380d0: 2020 2020 2020 2020 2020 6865 6164 6572            header
+000380e0: 5f70 6172 616d 7320 3d20 7b0d 0a20 2020  _params = {..   
+000380f0: 2020 2020 2020 2020 2020 2020 2027 6175               'au
+00038100: 7468 6f72 697a 6174 696f 6e27 3a20 6627  thorization': f'
+00038110: 7b73 656c 662e 746f 6b65 6e5f 6461 7461  {self.token_data
+00038120: 5b22 746f 6b65 6e5f 7479 7065 225d 7d20  ["token_type"]} 
+00038130: 7b73 656c 662e 746f 6b65 6e5f 6461 7461  {self.token_data
+00038140: 5b22 6163 6365 7373 5f74 6f6b 656e 225d  ["access_token"]
+00038150: 7d27 2c0d 0a20 2020 2020 2020 2020 2020  }',..           
+00038160: 2020 2020 2027 782d 7573 6572 2d61 6765       'x-user-age
+00038170: 6e74 273a 2027 4669 6c65 2054 7261 6e73  nt': 'File Trans
+00038180: 6c61 7465 2042 6f78 2050 6f72 7461 626c  late Box Portabl
+00038190: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
+000381a0: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
+000381b0: 7365 6c66 2e61 7069 5f6a 736f 6e5f 6865  self.api_json_he
+000381c0: 6164 6572 732e 7570 6461 7465 2868 6561  aders.update(hea
+000381d0: 6465 725f 7061 7261 6d73 290d 0a0d 0a20  der_params).... 
+000381e0: 2020 2020 2020 2020 2020 2064 5f6c 616e             d_lan
+000381f0: 675f 6d61 7020 3d20 7365 6c66 2e73 6573  g_map = self.ses
+00038200: 7369 6f6e 2e67 6574 2873 656c 662e 6765  sion.get(self.ge
+00038210: 745f 6c61 6e67 5f75 726c 2c20 6865 6164  t_lang_url, head
+00038220: 6572 733d 7365 6c66 2e61 7069 5f6a 736f  ers=self.api_jso
+00038230: 6e5f 6865 6164 6572 732c 2074 696d 656f  n_headers, timeo
+00038240: 7574 3d74 696d 656f 7574 2c20 7072 6f78  ut=timeout, prox
+00038250: 6965 733d 7072 6f78 6965 7329 2e6a 736f  ies=proxies).jso
+00038260: 6e28 290d 0a20 2020 2020 2020 2020 2020  n()..           
+00038270: 2064 6562 7567 5f6c 616e 675f 6b77 6172   debug_lang_kwar
+00038280: 6773 203d 2073 656c 662e 6465 6275 675f  gs = self.debug_
+00038290: 6c61 6e67 5f6b 7761 7267 7328 6672 6f6d  lang_kwargs(from
+000382a0: 5f6c 616e 6775 6167 652c 2074 6f5f 6c61  _language, to_la
+000382b0: 6e67 7561 6765 2c20 7365 6c66 2e64 6566  nguage, self.def
+000382c0: 6175 6c74 5f66 726f 6d5f 6c61 6e67 7561  ault_from_langua
+000382d0: 6765 2c20 6966 5f70 7269 6e74 5f77 6172  ge, if_print_war
+000382e0: 6e69 6e67 290d 0a20 2020 2020 2020 2020  ning)..         
+000382f0: 2020 2073 656c 662e 6c61 6e67 7561 6765     self.language
+00038300: 5f6d 6170 203d 2073 656c 662e 6765 745f  _map = self.get_
+00038310: 6c61 6e67 7561 6765 5f6d 6170 2864 5f6c  language_map(d_l
+00038320: 616e 675f 6d61 702c 202a 2a64 6562 7567  ang_map, **debug
+00038330: 5f6c 616e 675f 6b77 6172 6773 290d 0a20  _lang_kwargs).. 
+00038340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00038350: 7072 6f66 6573 7369 6f6e 616c 5f66 6965  professional_fie
+00038360: 6c64 203d 2073 656c 662e 6765 745f 7072  ld = self.get_pr
+00038370: 6f66 6573 7369 6f6e 616c 5f66 6965 6c64  ofessional_field
+00038380: 5f6c 6973 7428 645f 6c61 6e67 5f6d 6170  _list(d_lang_map
+00038390: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+000383a0: 656c 662e 6c61 6e67 7061 6972 5f64 6f6d  elf.langpair_dom
+000383b0: 6169 6e20 3d20 7365 6c66 2e67 6574 5f6c  ain = self.get_l
+000383c0: 616e 6770 6169 725f 646f 6d61 696e 2864  angpair_domain(d
+000383d0: 5f6c 616e 675f 6d61 7029 0d0a 0d0a 2020  _lang_map)....  
+000383e0: 2020 2020 2020 6672 6f6d 5f6c 616e 6775        from_langu
+000383f0: 6167 652c 2074 6f5f 6c61 6e67 7561 6765  age, to_language
+00038400: 203d 2073 656c 662e 6368 6563 6b5f 6c61   = self.check_la
+00038410: 6e67 7561 6765 2866 726f 6d5f 6c61 6e67  nguage(from_lang
+00038420: 7561 6765 2c20 746f 5f6c 616e 6775 6167  uage, to_languag
+00038430: 652c 2073 656c 662e 6c61 6e67 7561 6765  e, self.language
+00038440: 5f6d 6170 2c20 6f75 7470 7574 5f7a 683d  _map, output_zh=
+00038450: 7365 6c66 2e6f 7574 7075 745f 7a68 290d  self.output_zh).
+00038460: 0a20 2020 2020 2020 2069 6620 6672 6f6d  .        if from
+00038470: 5f6c 616e 6775 6167 6520 3d3d 2027 6175  _language == 'au
+00038480: 746f 273a 0d0a 2020 2020 2020 2020 2020  to':..          
+00038490: 2020 6672 6f6d 5f6c 616e 6775 6167 6520    from_language 
+000384a0: 3d20 7365 6c66 2e77 6172 6e69 6e67 5f61  = self.warning_a
+000384b0: 7574 6f5f 6c61 6e67 2827 7379 7354 7261  uto_lang('sysTra
+000384c0: 6e27 2c20 7365 6c66 2e64 6566 6175 6c74  n', self.default
+000384d0: 5f66 726f 6d5f 6c61 6e67 7561 6765 2c20  _from_language, 
+000384e0: 6966 5f70 7269 6e74 5f77 6172 6e69 6e67  if_print_warning
+000384f0: 290d 0a0d 0a20 2020 2020 2020 2070 6179  )....        pay
+00038500: 6c6f 6164 203d 207b 0d0a 2020 2020 2020  load = {..      
+00038510: 2020 2020 2020 2774 6172 6765 7427 3a20        'target': 
+00038520: 746f 5f6c 616e 6775 6167 652c 0d0a 2020  to_language,..  
+00038530: 2020 2020 2020 2020 2020 2773 6f75 7263            'sourc
+00038540: 6527 3a20 6672 6f6d 5f6c 616e 6775 6167  e': from_languag
+00038550: 6520 6966 2066 726f 6d5f 6c61 6e67 7561  e if from_langua
+00038560: 6765 2021 3d20 2761 7574 6f27 2065 6c73  ge != 'auto' els
+00038570: 6520 4e6f 6e65 2c0d 0a20 2020 2020 2020  e None,..       
+00038580: 2020 2020 2027 696e 7075 7473 273a 205b       'inputs': [
+00038590: 7061 7261 6772 6170 6820 666f 7220 7061  paragraph for pa
+000385a0: 7261 6772 6170 6820 696e 2071 7565 7279  ragraph in query
+000385b0: 5f74 6578 742e 7370 6c69 7428 275c 6e27  _text.split('\n'
+000385c0: 2920 6966 2070 6172 6167 7261 7068 2e73  ) if paragraph.s
+000385d0: 7472 6970 2829 5d2c 0d0a 2020 2020 2020  trip()],..      
+000385e0: 2020 2020 2020 2766 6f72 6d61 7427 3a20        'format': 
+000385f0: 2774 6578 742f 706c 6169 6e27 2c0d 0a20  'text/plain',.. 
+00038600: 2020 2020 2020 2020 2020 2027 6175 746f             'auto
+00038610: 6465 7465 6374 696f 6e4d 6f64 6527 3a20  detectionMode': 
+00038620: 2773 696e 676c 6527 2c0d 0a20 2020 2020  'single',..     
+00038630: 2020 2020 2020 2027 7769 7468 496e 666f         'withInfo
+00038640: 273a 2027 7472 7565 272c 0d0a 2020 2020  ': 'true',..    
+00038650: 2020 2020 2020 2020 2777 6974 6841 6e6e          'withAnn
+00038660: 6f74 6174 696f 6e73 273a 2027 7472 7565  otations': 'true
+00038670: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00038680: 2770 726f 6669 6c65 4964 273a 204e 6f6e  'profileId': Non
+00038690: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000386a0: 2764 6f6d 6169 6e27 3a20 4e6f 6e65 2c0d  'domain': None,.
+000386b0: 0a20 2020 2020 2020 2020 2020 2027 6f77  .            'ow
+000386c0: 6e65 7227 3a20 4e6f 6e65 2c0d 0a20 2020  ner': None,..   
+000386d0: 2020 2020 2020 2020 2027 7369 7a65 273a           'size':
+000386e0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+000386f0: 7d0d 0a20 2020 2020 2020 2069 6620 7573  }..        if us
+00038700: 655f 646f 6d61 696e 2061 6e64 2066 726f  e_domain and fro
+00038710: 6d5f 6c61 6e67 7561 6765 2021 3d20 2761  m_language != 'a
+00038720: 7574 6f27 3a0d 0a20 2020 2020 2020 2020  uto':..         
+00038730: 2020 2064 6f6d 6169 6e5f 7061 796c 6f61     domain_payloa
+00038740: 6420 3d20 7365 6c66 2e6c 616e 6770 6169  d = self.langpai
+00038750: 725f 646f 6d61 696e 2e67 6574 2866 277b  r_domain.get(f'{
+00038760: 6672 6f6d 5f6c 616e 6775 6167 657d 5f5f  from_language}__
+00038770: 7b74 6f5f 6c61 6e67 7561 6765 7d5f 5f7b  {to_language}__{
+00038780: 7573 655f 646f 6d61 696e 7d27 290d 0a20  use_domain}').. 
+00038790: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+000387a0: 7420 646f 6d61 696e 5f70 6179 6c6f 6164  t domain_payload
+000387b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000387c0: 2020 2072 6169 7365 2054 7261 6e73 6c61     raise Transla
+000387d0: 746f 7245 7272 6f72 0d0a 2020 2020 2020  torError..      
+000387e0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000387f0: 2020 2020 2020 2020 2020 2020 2070 6179               pay
+00038800: 6c6f 6164 2e75 7064 6174 6528 646f 6d61  load.update(doma
+00038810: 696e 5f70 6179 6c6f 6164 290d 0a0d 0a20  in_payload).... 
+00038820: 2020 2020 2020 2072 203d 2073 656c 662e         r = self.
+00038830: 7365 7373 696f 6e2e 706f 7374 2873 656c  session.post(sel
+00038840: 662e 6170 695f 7572 6c2c 206a 736f 6e3d  f.api_url, json=
+00038850: 7061 796c 6f61 642c 2068 6561 6465 7273  payload, headers
+00038860: 3d73 656c 662e 6170 695f 6a73 6f6e 5f68  =self.api_json_h
+00038870: 6561 6465 7273 2c20 7469 6d65 6f75 743d  eaders, timeout=
+00038880: 7469 6d65 6f75 742c 2070 726f 7869 6573  timeout, proxies
+00038890: 3d70 726f 7869 6573 290d 0a20 2020 2020  =proxies)..     
+000388a0: 2020 2072 2e72 6169 7365 5f66 6f72 5f73     r.raise_for_s
+000388b0: 7461 7475 7328 290d 0a20 2020 2020 2020  tatus()..       
+000388c0: 2064 6174 6120 3d20 722e 6a73 6f6e 2829   data = r.json()
+000388d0: 0d0a 2020 2020 2020 2020 7469 6d65 2e73  ..        time.s
+000388e0: 6c65 6570 2873 6c65 6570 5f73 6563 6f6e  leep(sleep_secon
+000388f0: 6473 290d 0a20 2020 2020 2020 2073 656c  ds)..        sel
+00038900: 662e 7175 6572 795f 636f 756e 7420 2b3d  f.query_count +=
+00038910: 2031 0d0a 2020 2020 2020 2020 7265 7475   1..        retu
+00038920: 726e 2064 6174 6120 6966 2069 735f 6465  rn data if is_de
+00038930: 7461 696c 5f72 6573 756c 7420 656c 7365  tail_result else
+00038940: 2027 5c6e 272e 6a6f 696e 2827 2027 2e6a   '\n'.join(' '.j
+00038950: 6f69 6e28 6974 5b27 616c 745f 7472 616e  oin(it['alt_tran
+00038960: 7365 7327 5d5b 305d 5b27 7461 7267 6574  ses'][0]['target
+00038970: 275d 5b27 7465 7874 275d 2066 6f72 2069  ']['text'] for i
+00038980: 7420 696e 2069 7465 6d5b 276f 7574 7075  t in item['outpu
+00038990: 7427 5d5b 2764 6f63 756d 656e 7473 275d  t']['documents']
+000389a0: 5b30 5d5b 2774 7261 6e73 5f75 6e69 7473  [0]['trans_units
+000389b0: 275d 5b30 5d5b 2773 656e 7465 6e63 6573  '][0]['sentences
+000389c0: 275d 2920 666f 7220 6974 656d 2069 6e20  ']) for item in 
+000389d0: 6461 7461 5b27 6f75 7470 7574 7327 5d29  data['outputs'])
+000389e0: 0d0a 0d0a 0d0a 636c 6173 7320 5472 616e  ......class Tran
+000389f0: 736c 6174 654d 6528 5473 6529 3a0d 0a20  slateMe(Tse):.. 
+00038a00: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00038a10: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00038a20: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00038a30: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+00038a40: 2e68 6f73 745f 7572 6c20 3d20 2768 7474  .host_url = 'htt
+00038a50: 7073 3a2f 2f74 7261 6e73 6c61 7465 6d65  ps://translateme
+00038a60: 2e6e 6574 776f 726b 2f27 0d0a 2020 2020  .network/'..    
+00038a70: 2020 2020 7365 6c66 2e61 7069 5f75 726c      self.api_url
+00038a80: 203d 2027 6874 7470 733a 2f2f 7472 616e   = 'https://tran
+00038a90: 736c 6174 656d 652e 6e65 7477 6f72 6b2f  slateme.network/
+00038aa0: 7770 2d61 646d 696e 2f61 646d 696e 2d61  wp-admin/admin-a
+00038ab0: 6a61 782e 7068 7027 0d0a 2020 2020 2020  jax.php'..      
+00038ac0: 2020 7365 6c66 2e68 6f73 745f 6865 6164    self.host_head
+00038ad0: 6572 7320 3d20 7365 6c66 2e67 6574 5f68  ers = self.get_h
+00038ae0: 6561 6465 7273 2873 656c 662e 686f 7374  eaders(self.host
+00038af0: 5f75 726c 2c20 6966 5f61 7069 3d46 616c  _url, if_api=Fal
+00038b00: 7365 2c20 6966 5f72 6566 6572 6572 5f66  se, if_referer_f
+00038b10: 6f72 5f68 6f73 743d 5472 7565 290d 0a20  or_host=True).. 
+00038b20: 2020 2020 2020 2073 656c 662e 6170 695f         self.api_
+00038b30: 6865 6164 6572 7320 3d20 7365 6c66 2e67  headers = self.g
+00038b40: 6574 5f68 6561 6465 7273 2873 656c 662e  et_headers(self.
+00038b50: 686f 7374 5f75 726c 2c20 6966 5f61 7069  host_url, if_api
+00038b60: 3d54 7275 652c 2069 665f 616a 6178 5f66  =True, if_ajax_f
+00038b70: 6f72 5f61 7069 3d54 7275 6529 0d0a 2020  or_api=True)..  
+00038b80: 2020 2020 2020 7365 6c66 2e73 6573 7369        self.sessi
+00038b90: 6f6e 203d 204e 6f6e 650d 0a20 2020 2020  on = None..     
+00038ba0: 2020 2073 656c 662e 6c61 6e67 7561 6765     self.language
+00038bb0: 5f6d 6170 203d 204e 6f6e 650d 0a20 2020  _map = None..   
+00038bc0: 2020 2020 2073 656c 662e 7175 6572 795f       self.query_
+00038bd0: 636f 756e 7420 3d20 300d 0a20 2020 2020  count = 0..     
+00038be0: 2020 2073 656c 662e 6f75 7470 7574 5f7a     self.output_z
+00038bf0: 6820 3d20 2743 6869 6e65 7365 270d 0a20  h = 'Chinese'.. 
+00038c00: 2020 2020 2020 2073 656c 662e 6f75 7470         self.outp
+00038c10: 7574 5f65 6e20 3d20 2745 6e67 6c69 7368  ut_en = 'English
+00038c20: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+00038c30: 696e 7075 745f 6c69 6d69 7420 3d20 696e  input_limit = in
+00038c40: 7428 3165 3229 0d0a 2020 2020 2020 2020  t(1e2)..        
+00038c50: 7365 6c66 2e64 6566 6175 6c74 5f66 726f  self.default_fro
+00038c60: 6d5f 6c61 6e67 7561 6765 203d 2073 656c  m_language = sel
+00038c70: 662e 6f75 7470 7574 5f7a 680d 0a0d 0a20  f.output_zh.... 
+00038c80: 2020 2040 5473 652e 6465 6275 675f 6c61     @Tse.debug_la
+00038c90: 6e67 7561 6765 5f6d 6170 0d0a 2020 2020  nguage_map..    
+00038ca0: 6465 6620 6765 745f 6c61 6e67 7561 6765  def get_language
+00038cb0: 5f6d 6170 2873 656c 662c 2068 6f73 745f  _map(self, host_
+00038cc0: 6874 6d6c 3a20 7374 722c 202a 2a6b 7761  html: str, **kwa
+00038cd0: 7267 733a 204c 616e 674d 6170 4b77 6172  rgs: LangMapKwar
+00038ce0: 6773 5479 7065 2920 2d3e 2064 6963 743a  gsType) -> dict:
+00038cf0: 0d0a 2020 2020 2020 2020 6c61 6e67 5f6c  ..        lang_l
+00038d00: 6973 7420 3d20 7265 2e63 6f6d 7069 6c65  ist = re.compile
+00038d10: 2827 6461 7461 2d6c 616e 673d 2228 2e2a  ('data-lang="(.*
+00038d20: 3f29 2227 292e 6669 6e64 616c 6c28 686f  ?)"').findall(ho
+00038d30: 7374 5f68 746d 6c29 0d0a 2020 2020 2020  st_html)..      
+00038d40: 2020 6966 206e 6f74 206c 616e 675f 6c69    if not lang_li
+00038d50: 7374 3a0d 0a20 2020 2020 2020 2020 2020  st:..           
+00038d60: 2072 6169 7365 2054 7261 6e73 6c61 746f   raise Translato
+00038d70: 7245 7272 6f72 0d0a 0d0a 2020 2020 2020  rError....      
+00038d80: 2020 6c61 6e67 5f6c 6973 7420 3d20 736f    lang_list = so
+00038d90: 7274 6564 286c 6973 7428 7365 7428 6c61  rted(list(set(la
+00038da0: 6e67 5f6c 6973 7429 2929 0d0a 2020 2020  ng_list)))..    
+00038db0: 2020 2020 7265 7475 726e 207b 7d2e 6672      return {}.fr
+00038dc0: 6f6d 6b65 7973 286c 616e 675f 6c69 7374  omkeys(lang_list
+00038dd0: 2c20 6c61 6e67 5f6c 6973 7429 0d0a 0d0a  , lang_list)....
+00038de0: 2020 2020 2320 4054 7365 2e75 6e63 6572      # @Tse.uncer
+00038df0: 7469 6669 6564 0d0a 2020 2020 2320 4054  tified..    # @T
+00038e00: 7365 2e74 696d 655f 7374 6174 0d0a 2020  se.time_stat..  
+00038e10: 2020 2320 4054 7365 2e63 6865 636b 5f71    # @Tse.check_q
+00038e20: 7565 7279 0d0a 2020 2020 6465 6620 5f74  uery..    def _t
+00038e30: 7261 6e73 6c61 7465 4d65 5f61 7069 2873  ranslateMe_api(s
+00038e40: 656c 662c 2071 7565 7279 5f74 6578 743a  elf, query_text:
+00038e50: 2073 7472 2c20 6672 6f6d 5f6c 616e 6775   str, from_langu
+00038e60: 6167 653a 2073 7472 203d 2027 6175 746f  age: str = 'auto
+00038e70: 272c 2074 6f5f 6c61 6e67 7561 6765 3a20  ', to_language: 
+00038e80: 7374 7220 3d20 2765 6e27 2c20 2a2a 6b77  str = 'en', **kw
+00038e90: 6172 6773 3a20 4170 694b 7761 7267 7354  args: ApiKwargsT
+00038ea0: 7970 6529 202d 3e20 556e 696f 6e5b 7374  ype) -> Union[st
+00038eb0: 722c 2064 6963 745d 3a0d 0a20 2020 2020  r, dict]:..     
+00038ec0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00038ed0: 6874 7470 733a 2f2f 7472 616e 736c 6174  https://translat
+00038ee0: 656d 652e 6e65 7477 6f72 6b2f 0d0a 2020  eme.network/..  
+00038ef0: 2020 2020 2020 3a70 6172 616d 2071 7565        :param que
+00038f00: 7279 5f74 6578 743a 2073 7472 2c20 6d75  ry_text: str, mu
+00038f10: 7374 2e0d 0a20 2020 2020 2020 203a 7061  st...        :pa
+00038f20: 7261 6d20 6672 6f6d 5f6c 616e 6775 6167  ram from_languag
+00038f30: 653a 2073 7472 2c20 6465 6661 756c 7420  e: str, default 
+00038f40: 2761 7574 6f27 2e0d 0a20 2020 2020 2020  'auto'...       
+00038f50: 203a 7061 7261 6d20 746f 5f6c 616e 6775   :param to_langu
+00038f60: 6167 653a 2073 7472 2c20 6465 6661 756c  age: str, defaul
+00038f70: 7420 2765 6e27 2e0d 0a20 2020 2020 2020  t 'en'...       
+00038f80: 203a 7061 7261 6d20 2a2a 6b77 6172 6773   :param **kwargs
+00038f90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00038fa0: 2020 203a 7061 7261 6d20 7469 6d65 6f75     :param timeou
+00038fb0: 743a 2066 6c6f 6174 2c20 6465 6661 756c  t: float, defaul
+00038fc0: 7420 4e6f 6e65 2e0d 0a20 2020 2020 2020  t None...       
+00038fd0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00038fe0: 7072 6f78 6965 733a 2064 6963 742c 2064  proxies: dict, d
+00038ff0: 6566 6175 6c74 204e 6f6e 652e 0d0a 2020  efault None...  
+00039000: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+00039010: 6172 616d 2073 6c65 6570 5f73 6563 6f6e  aram sleep_secon
+00039020: 6473 3a20 666c 6f61 742c 2064 6566 6175  ds: float, defau
+00039030: 6c74 2030 2e0d 0a20 2020 2020 2020 2020  lt 0...         
+00039040: 2020 2020 2020 203a 7061 7261 6d20 6973         :param is
+00039050: 5f64 6574 6169 6c5f 7265 7375 6c74 3a20  _detail_result: 
+00039060: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+00039070: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
+00039080: 2020 2020 2020 3a70 6172 616d 2069 665f        :param if_
+00039090: 6967 6e6f 7265 5f6c 696d 6974 5f6f 665f  ignore_limit_of_
+000390a0: 6c65 6e67 7468 3a20 626f 6f6c 2c20 6465  length: bool, de
+000390b0: 6661 756c 7420 4661 6c73 652e 0d0a 2020  fault False...  
+000390c0: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+000390d0: 6172 616d 206c 696d 6974 5f6f 665f 6c65  aram limit_of_le
+000390e0: 6e67 7468 3a20 696e 742c 2064 6566 6175  ngth: int, defau
+000390f0: 6c74 2032 3030 3030 2e0d 0a20 2020 2020  lt 20000...     
+00039100: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00039110: 6d20 6966 5f69 676e 6f72 655f 656d 7074  m if_ignore_empt
+00039120: 795f 7175 6572 793a 2062 6f6f 6c2c 2064  y_query: bool, d
+00039130: 6566 6175 6c74 2046 616c 7365 2e0d 0a20  efault False... 
+00039140: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+00039150: 7061 7261 6d20 7570 6461 7465 5f73 6573  param update_ses
+00039160: 7369 6f6e 5f61 6674 6572 5f66 7265 713a  sion_after_freq:
+00039170: 2069 6e74 2c20 6465 6661 756c 7420 3130   int, default 10
+00039180: 3030 2e0d 0a20 2020 2020 2020 2020 2020  00...           
+00039190: 2020 2020 203a 7061 7261 6d20 7570 6461       :param upda
+000391a0: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
+000391b0: 5f73 6563 6f6e 6473 3a20 666c 6f61 742c  _seconds: float,
+000391c0: 2064 6566 6175 6c74 2031 3530 302e 0d0a   default 1500...
+000391d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000391e0: 3a70 6172 616d 2069 665f 7368 6f77 5f74  :param if_show_t
+000391f0: 696d 655f 7374 6174 3a20 626f 6f6c 2c20  ime_stat: bool, 
+00039200: 6465 6661 756c 7420 4661 6c73 652e 0d0a  default False...
+00039210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039220: 3a70 6172 616d 2073 686f 775f 7469 6d65  :param show_time
+00039230: 5f73 7461 745f 7072 6563 6973 696f 6e3a  _stat_precision:
+00039240: 2069 6e74 2c20 6465 6661 756c 7420 322e   int, default 2.
+00039250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00039260: 2020 3a70 6172 616d 2069 665f 7072 696e    :param if_prin
+00039270: 745f 7761 726e 696e 673a 2062 6f6f 6c2c  t_warning: bool,
+00039280: 2064 6566 6175 6c74 2054 7275 652e 0d0a   default True...
+00039290: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+000392a0: 2073 7472 206f 7220 6469 6374 0d0a 2020   str or dict..  
+000392b0: 2020 2020 2020 2222 220d 0a0d 0a20 2020        """....   
+000392c0: 2020 2020 2074 696d 656f 7574 203d 206b       timeout = k
+000392d0: 7761 7267 732e 6765 7428 2774 696d 656f  wargs.get('timeo
+000392e0: 7574 272c 204e 6f6e 6529 0d0a 2020 2020  ut', None)..    
+000392f0: 2020 2020 7072 6f78 6965 7320 3d20 6b77      proxies = kw
+00039300: 6172 6773 2e67 6574 2827 7072 6f78 6965  args.get('proxie
+00039310: 7327 2c20 4e6f 6e65 290d 0a20 2020 2020  s', None)..     
+00039320: 2020 2073 6c65 6570 5f73 6563 6f6e 6473     sleep_seconds
+00039330: 203d 206b 7761 7267 732e 6765 7428 2773   = kwargs.get('s
+00039340: 6c65 6570 5f73 6563 6f6e 6473 272c 2030  leep_seconds', 0
+00039350: 290d 0a20 2020 2020 2020 2069 665f 7072  )..        if_pr
+00039360: 696e 745f 7761 726e 696e 6720 3d20 6b77  int_warning = kw
+00039370: 6172 6773 2e67 6574 2827 6966 5f70 7269  args.get('if_pri
+00039380: 6e74 5f77 6172 6e69 6e67 272c 2054 7275  nt_warning', Tru
+00039390: 6529 0d0a 2020 2020 2020 2020 6973 5f64  e)..        is_d
+000393a0: 6574 6169 6c5f 7265 7375 6c74 203d 206b  etail_result = k
+000393b0: 7761 7267 732e 6765 7428 2769 735f 6465  wargs.get('is_de
+000393c0: 7461 696c 5f72 6573 756c 7427 2c20 4661  tail_result', Fa
+000393d0: 6c73 6529 0d0a 2020 2020 2020 2020 7570  lse)..        up
+000393e0: 6461 7465 5f73 6573 7369 6f6e 5f61 6674  date_session_aft
+000393f0: 6572 5f66 7265 7120 3d20 6b77 6172 6773  er_freq = kwargs
+00039400: 2e67 6574 2827 7570 6461 7465 5f73 6573  .get('update_ses
+00039410: 7369 6f6e 5f61 6674 6572 5f66 7265 7127  sion_after_freq'
+00039420: 2c20 7365 6c66 2e64 6566 6175 6c74 5f73  , self.default_s
+00039430: 6573 7369 6f6e 5f66 7265 7129 0d0a 2020  ession_freq)..  
+00039440: 2020 2020 2020 7570 6461 7465 5f73 6573        update_ses
+00039450: 7369 6f6e 5f61 6674 6572 5f73 6563 6f6e  sion_after_secon
+00039460: 6473 203d 206b 7761 7267 732e 6765 7428  ds = kwargs.get(
+00039470: 2775 7064 6174 655f 7365 7373 696f 6e5f  'update_session_
+00039480: 6166 7465 725f 7365 636f 6e64 7327 2c20  after_seconds', 
+00039490: 7365 6c66 2e64 6566 6175 6c74 5f73 6573  self.default_ses
+000394a0: 7369 6f6e 5f73 6563 6f6e 6473 290d 0a20  sion_seconds).. 
+000394b0: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+000394c0: 6b5f 696e 7075 745f 6c69 6d69 7428 7175  k_input_limit(qu
+000394d0: 6572 795f 7465 7874 2c20 7365 6c66 2e69  ery_text, self.i
+000394e0: 6e70 7574 5f6c 696d 6974 290d 0a0d 0a20  nput_limit).... 
+000394f0: 2020 2020 2020 206e 6f74 5f75 7064 6174         not_updat
+00039500: 655f 636f 6e64 5f66 7265 7120 3d20 3120  e_cond_freq = 1 
+00039510: 6966 2073 656c 662e 7175 6572 795f 636f  if self.query_co
+00039520: 756e 7420 3c20 7570 6461 7465 5f73 6573  unt < update_ses
+00039530: 7369 6f6e 5f61 6674 6572 5f66 7265 7120  sion_after_freq 
+00039540: 656c 7365 2030 0d0a 2020 2020 2020 2020  else 0..        
+00039550: 6e6f 745f 7570 6461 7465 5f63 6f6e 645f  not_update_cond_
+00039560: 7469 6d65 203d 2031 2069 6620 7469 6d65  time = 1 if time
+00039570: 2e74 696d 6528 2920 2d20 7365 6c66 2e62  .time() - self.b
+00039580: 6567 696e 5f74 696d 6520 3c20 7570 6461  egin_time < upda
+00039590: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
+000395a0: 5f73 6563 6f6e 6473 2065 6c73 6520 300d  _seconds else 0.
+000395b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000395c0: 2873 656c 662e 7365 7373 696f 6e20 616e  (self.session an
+000395d0: 6420 7365 6c66 2e6c 616e 6775 6167 655f  d self.language_
+000395e0: 6d61 7020 616e 6420 6e6f 745f 7570 6461  map and not_upda
+000395f0: 7465 5f63 6f6e 645f 6672 6571 2061 6e64  te_cond_freq and
+00039600: 206e 6f74 5f75 7064 6174 655f 636f 6e64   not_update_cond
+00039610: 5f74 696d 6529 3a0d 0a20 2020 2020 2020  _time):..       
+00039620: 2020 2020 2073 656c 662e 7365 7373 696f       self.sessio
+00039630: 6e20 3d20 7265 7175 6573 7473 2e53 6573  n = requests.Ses
+00039640: 7369 6f6e 2829 0d0a 2020 2020 2020 2020  sion()..        
+00039650: 2020 2020 686f 7374 5f68 746d 6c20 3d20      host_html = 
+00039660: 7365 6c66 2e73 6573 7369 6f6e 2e67 6574  self.session.get
+00039670: 2873 656c 662e 686f 7374 5f75 726c 2c20  (self.host_url, 
+00039680: 6865 6164 6572 733d 7365 6c66 2e68 6f73  headers=self.hos
+00039690: 745f 6865 6164 6572 732c 2074 696d 656f  t_headers, timeo
+000396a0: 7574 3d74 696d 656f 7574 2c20 7072 6f78  ut=timeout, prox
+000396b0: 6965 733d 7072 6f78 6965 7329 2e74 6578  ies=proxies).tex
+000396c0: 740d 0a20 2020 2020 2020 2020 2020 2064  t..            d
+000396d0: 6562 7567 5f6c 616e 675f 6b77 6172 6773  ebug_lang_kwargs
+000396e0: 203d 2073 656c 662e 6465 6275 675f 6c61   = self.debug_la
+000396f0: 6e67 5f6b 7761 7267 7328 6672 6f6d 5f6c  ng_kwargs(from_l
+00039700: 616e 6775 6167 652c 2074 6f5f 6c61 6e67  anguage, to_lang
+00039710: 7561 6765 2c20 7365 6c66 2e64 6566 6175  uage, self.defau
+00039720: 6c74 5f66 726f 6d5f 6c61 6e67 7561 6765  lt_from_language
+00039730: 2c20 6966 5f70 7269 6e74 5f77 6172 6e69  , if_print_warni
+00039740: 6e67 290d 0a20 2020 2020 2020 2020 2020  ng)..           
+00039750: 2073 656c 662e 6c61 6e67 7561 6765 5f6d   self.language_m
+00039760: 6170 203d 2073 656c 662e 6765 745f 6c61  ap = self.get_la
+00039770: 6e67 7561 6765 5f6d 6170 2868 6f73 745f  nguage_map(host_
+00039780: 6874 6d6c 2c20 2a2a 6465 6275 675f 6c61  html, **debug_la
+00039790: 6e67 5f6b 7761 7267 7329 0d0a 0d0a 2020  ng_kwargs)....  
+000397a0: 2020 2020 2020 6966 2066 726f 6d5f 6c61        if from_la
+000397b0: 6e67 7561 6765 203d 3d20 2761 7574 6f27  nguage == 'auto'
+000397c0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+000397d0: 726f 6d5f 6c61 6e67 7561 6765 203d 2073  rom_language = s
+000397e0: 656c 662e 7761 726e 696e 675f 6175 746f  elf.warning_auto
+000397f0: 5f6c 616e 6728 2774 7261 6e73 6c61 7465  _lang('translate
+00039800: 4d65 272c 2073 656c 662e 6465 6661 756c  Me', self.defaul
+00039810: 745f 6672 6f6d 5f6c 616e 6775 6167 652c  t_from_language,
+00039820: 2069 665f 7072 696e 745f 7761 726e 696e   if_print_warnin
+00039830: 6729 0d0a 2020 2020 2020 2020 6672 6f6d  g)..        from
+00039840: 5f6c 616e 6775 6167 652c 2074 6f5f 6c61  _language, to_la
+00039850: 6e67 7561 6765 203d 2073 656c 662e 6368  nguage = self.ch
+00039860: 6563 6b5f 6c61 6e67 7561 6765 2866 726f  eck_language(fro
+00039870: 6d5f 6c61 6e67 7561 6765 2c20 746f 5f6c  m_language, to_l
+00039880: 616e 6775 6167 652c 2073 656c 662e 6c61  anguage, self.la
+00039890: 6e67 7561 6765 5f6d 6170 2c20 6f75 7470  nguage_map, outp
+000398a0: 7574 5f7a 683d 7365 6c66 2e6f 7574 7075  ut_zh=self.outpu
+000398b0: 745f 7a68 2c0d 0a20 2020 2020 2020 2020  t_zh,..         
+000398c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000398d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000398e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000398f0: 6f75 7470 7574 5f65 6e5f 7472 616e 736c  output_en_transl
+00039900: 6174 6f72 3d27 7472 616e 736c 6174 654d  ator='translateM
+00039910: 6527 2c20 6f75 7470 7574 5f65 6e3d 7365  e', output_en=se
+00039920: 6c66 2e6f 7574 7075 745f 656e 290d 0a20  lf.output_en).. 
+00039930: 2020 2020 2020 2069 6620 7365 6c66 2e6f         if self.o
+00039940: 7574 7075 745f 656e 206e 6f74 2069 6e20  utput_en not in 
+00039950: 2866 726f 6d5f 6c61 6e67 7561 6765 2c20  (from_language, 
+00039960: 746f 5f6c 616e 6775 6167 6529 3a0d 0a20  to_language):.. 
+00039970: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00039980: 2054 7261 6e73 6c61 746f 7245 7272 6f72   TranslatorError
+00039990: 2827 4d75 7374 2075 7365 2045 6e67 6c69  ('Must use Engli
+000399a0: 7368 2061 7320 616e 2069 6e74 6572 6d65  sh as an interme
+000399b0: 6469 6174 6520 7472 616e 736c 6174 696f  diate translatio
+000399c0: 6e2e 2729 0d0a 0d0a 2020 2020 2020 2020  n.')....        
+000399d0: 6461 7461 5f6c 6973 7420 3d20 5b5d 0d0a  data_list = []..
+000399e0: 2020 2020 2020 2020 7061 7261 6772 6170          paragrap
+000399f0: 6873 203d 205b 7061 7261 6772 6170 6820  hs = [paragraph 
+00039a00: 666f 7220 7061 7261 6772 6170 6820 696e  for paragraph in
+00039a10: 2071 7565 7279 5f74 6578 742e 7370 6c69   query_text.spli
+00039a20: 7428 275c 6e27 2920 6966 2070 6172 6167  t('\n') if parag
+00039a30: 7261 7068 2e73 7472 6970 2829 5d0d 0a20  raph.strip()].. 
+00039a40: 2020 2020 2020 2066 6f72 2070 6172 6167         for parag
+00039a50: 7261 7068 2069 6e20 7061 7261 6772 6170  raph in paragrap
+00039a60: 6873 3a0d 0a20 2020 2020 2020 2020 2020  hs:..           
+00039a70: 2070 6179 6c6f 6164 203d 207b 0d0a 2020   payload = {..  
+00039a80: 2020 2020 2020 2020 2020 2020 2020 2774                't
+00039a90: 6578 7427 3a20 7061 7261 6772 6170 682c  ext': paragraph,
+00039aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00039ab0: 2020 276c 616e 675f 6672 6f6d 273a 2066    'lang_from': f
+00039ac0: 726f 6d5f 6c61 6e67 7561 6765 2c0d 0a20  rom_language,.. 
+00039ad0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00039ae0: 6c61 6e67 5f74 6f27 3a20 746f 5f6c 616e  lang_to': to_lan
+00039af0: 6775 6167 652c 0d0a 2020 2020 2020 2020  guage,..        
+00039b00: 2020 2020 2020 2020 2761 6374 696f 6e27          'action'
+00039b10: 3a20 2774 6d5f 6d79 5f61 6374 696f 6e27  : 'tm_my_action'
+00039b20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00039b30: 2020 2027 7479 7065 273a 2027 636f 6e76     'type': 'conv
+00039b40: 6572 7427 0d0a 2020 2020 2020 2020 2020  ert'..          
+00039b50: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
+00039b60: 2070 6179 6c6f 6164 203d 2075 726c 6c69   payload = urlli
+00039b70: 622e 7061 7273 652e 7572 6c65 6e63 6f64  b.parse.urlencod
+00039b80: 6528 7061 796c 6f61 6429 0d0a 2020 2020  e(payload)..    
+00039b90: 2020 2020 2020 2020 7220 3d20 7365 6c66          r = self
+00039ba0: 2e73 6573 7369 6f6e 2e70 6f73 7428 7365  .session.post(se
+00039bb0: 6c66 2e61 7069 5f75 726c 2c20 6461 7461  lf.api_url, data
+00039bc0: 3d70 6179 6c6f 6164 2c20 6865 6164 6572  =payload, header
+00039bd0: 733d 7365 6c66 2e61 7069 5f68 6561 6465  s=self.api_heade
+00039be0: 7273 2c20 7469 6d65 6f75 743d 7469 6d65  rs, timeout=time
+00039bf0: 6f75 742c 2070 726f 7869 6573 3d70 726f  out, proxies=pro
+00039c00: 7869 6573 290d 0a20 2020 2020 2020 2020  xies)..         
+00039c10: 2020 2072 2e72 6169 7365 5f66 6f72 5f73     r.raise_for_s
+00039c20: 7461 7475 7328 290d 0a20 2020 2020 2020  tatus()..       
+00039c30: 2020 2020 2064 6174 6120 3d20 722e 6a73       data = r.js
+00039c40: 6f6e 2829 0d0a 2020 2020 2020 2020 2020  on()..          
+00039c50: 2020 6461 7461 5f6c 6973 742e 6170 7065    data_list.appe
+00039c60: 6e64 2864 6174 6129 0d0a 2020 2020 2020  nd(data)..      
+00039c70: 2020 7469 6d65 2e73 6c65 6570 2873 6c65    time.sleep(sle
+00039c80: 6570 5f73 6563 6f6e 6473 290d 0a20 2020  ep_seconds)..   
+00039c90: 2020 2020 2073 656c 662e 7175 6572 795f       self.query_
+00039ca0: 636f 756e 7420 2b3d 2031 0d0a 2020 2020  count += 1..    
+00039cb0: 2020 2020 7265 7475 726e 207b 2764 6174      return {'dat
+00039cc0: 6127 3a20 6461 7461 5f6c 6973 747d 2069  a': data_list} i
+00039cd0: 6620 6973 5f64 6574 6169 6c5f 7265 7375  f is_detail_resu
+00039ce0: 6c74 2065 6c73 6520 275c 6e27 2e6a 6f69  lt else '\n'.joi
+00039cf0: 6e28 5b69 7465 6d5b 2774 6f27 5d20 666f  n([item['to'] fo
+00039d00: 7220 6974 656d 2069 6e20 6461 7461 5f6c  r item in data_l
+00039d10: 6973 745d 290d 0a0d 0a20 2020 2040 5473  ist])....    @Ts
+00039d20: 652e 756e 6365 7274 6966 6965 640d 0a20  e.uncertified.. 
+00039d30: 2020 2040 5473 652e 7469 6d65 5f73 7461     @Tse.time_sta
+00039d40: 740d 0a20 2020 2040 5473 652e 6368 6563  t..    @Tse.chec
+00039d50: 6b5f 7175 6572 790d 0a20 2020 2064 6566  k_query..    def
+00039d60: 2074 7261 6e73 6c61 7465 4d65 5f61 7069   translateMe_api
+00039d70: 2873 656c 662c 2071 7565 7279 5f74 6578  (self, query_tex
+00039d80: 743a 2073 7472 2c20 6672 6f6d 5f6c 616e  t: str, from_lan
+00039d90: 6775 6167 653a 2073 7472 203d 2027 6175  guage: str = 'au
+00039da0: 746f 272c 2074 6f5f 6c61 6e67 7561 6765  to', to_language
+00039db0: 3a20 7374 7220 3d20 2765 6e27 2c20 2a2a  : str = 'en', **
+00039dc0: 6b77 6172 6773 3a20 4170 694b 7761 7267  kwargs: ApiKwarg
+00039dd0: 7354 7970 6529 202d 3e20 556e 696f 6e5b  sType) -> Union[
+00039de0: 7374 722c 2064 6963 745d 3a0d 0a20 2020  str, dict]:..   
+00039df0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00039e00: 2020 6874 7470 733a 2f2f 7472 616e 736c    https://transl
+00039e10: 6174 656d 652e 6e65 7477 6f72 6b2f 0d0a  ateme.network/..
+00039e20: 2020 2020 2020 2020 3a70 6172 616d 2071          :param q
+00039e30: 7565 7279 5f74 6578 743a 2073 7472 2c20  uery_text: str, 
+00039e40: 6d75 7374 2e0d 0a20 2020 2020 2020 203a  must...        :
+00039e50: 7061 7261 6d20 6672 6f6d 5f6c 616e 6775  param from_langu
+00039e60: 6167 653a 2073 7472 2c20 6465 6661 756c  age: str, defaul
+00039e70: 7420 2761 7574 6f27 2e0d 0a20 2020 2020  t 'auto'...     
+00039e80: 2020 203a 7061 7261 6d20 746f 5f6c 616e     :param to_lan
+00039e90: 6775 6167 653a 2073 7472 2c20 6465 6661  guage: str, defa
+00039ea0: 756c 7420 2765 6e27 2e0d 0a20 2020 2020  ult 'en'...     
+00039eb0: 2020 203a 7061 7261 6d20 2a2a 6b77 6172     :param **kwar
+00039ec0: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
+00039ed0: 2020 2020 203a 7061 7261 6d20 7469 6d65       :param time
+00039ee0: 6f75 743a 2066 6c6f 6174 2c20 6465 6661  out: float, defa
+00039ef0: 756c 7420 4e6f 6e65 2e0d 0a20 2020 2020  ult None...     
+00039f00: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00039f10: 6d20 7072 6f78 6965 733a 2064 6963 742c  m proxies: dict,
+00039f20: 2064 6566 6175 6c74 204e 6f6e 652e 0d0a   default None...
+00039f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039f40: 3a70 6172 616d 2073 6c65 6570 5f73 6563  :param sleep_sec
+00039f50: 6f6e 6473 3a20 666c 6f61 742c 2064 6566  onds: float, def
+00039f60: 6175 6c74 2030 2e0d 0a20 2020 2020 2020  ault 0...       
+00039f70: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00039f80: 6973 5f64 6574 6169 6c5f 7265 7375 6c74  is_detail_result
+00039f90: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+00039fa0: 4661 6c73 652e 0d0a 2020 2020 2020 2020  False...        
+00039fb0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+00039fc0: 665f 6967 6e6f 7265 5f6c 696d 6974 5f6f  f_ignore_limit_o
+00039fd0: 665f 6c65 6e67 7468 3a20 626f 6f6c 2c20  f_length: bool, 
+00039fe0: 6465 6661 756c 7420 4661 6c73 652e 0d0a  default False...
+00039ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003a000: 3a70 6172 616d 206c 696d 6974 5f6f 665f  :param limit_of_
+0003a010: 6c65 6e67 7468 3a20 696e 742c 2064 6566  length: int, def
+0003a020: 6175 6c74 2032 3030 3030 2e0d 0a20 2020  ault 20000...   
+0003a030: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+0003a040: 7261 6d20 6966 5f69 676e 6f72 655f 656d  ram if_ignore_em
+0003a050: 7074 795f 7175 6572 793a 2062 6f6f 6c2c  pty_query: bool,
+0003a060: 2064 6566 6175 6c74 2046 616c 7365 2e0d   default False..
+0003a070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003a080: 203a 7061 7261 6d20 7570 6461 7465 5f73   :param update_s
+0003a090: 6573 7369 6f6e 5f61 6674 6572 5f66 7265  ession_after_fre
+0003a0a0: 713a 2069 6e74 2c20 6465 6661 756c 7420  q: int, default 
+0003a0b0: 3130 3030 2e0d 0a20 2020 2020 2020 2020  1000...         
+0003a0c0: 2020 2020 2020 203a 7061 7261 6d20 7570         :param up
+0003a0d0: 6461 7465 5f73 6573 7369 6f6e 5f61 6674  date_session_aft
+0003a0e0: 6572 5f73 6563 6f6e 6473 3a20 666c 6f61  er_seconds: floa
+0003a0f0: 742c 2064 6566 6175 6c74 2031 3530 302e  t, default 1500.
+0003a100: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0003a110: 2020 3a70 6172 616d 2069 665f 7368 6f77    :param if_show
+0003a120: 5f74 696d 655f 7374 6174 3a20 626f 6f6c  _time_stat: bool
+0003a130: 2c20 6465 6661 756c 7420 4661 6c73 652e  , default False.
+0003a140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0003a150: 2020 3a70 6172 616d 2073 686f 775f 7469    :param show_ti
+0003a160: 6d65 5f73 7461 745f 7072 6563 6973 696f  me_stat_precisio
+0003a170: 6e3a 2069 6e74 2c20 6465 6661 756c 7420  n: int, default 
+0003a180: 322e 0d0a 2020 2020 2020 2020 2020 2020  2...            
+0003a190: 2020 2020 3a70 6172 616d 2069 665f 7072      :param if_pr
+0003a1a0: 696e 745f 7761 726e 696e 673a 2062 6f6f  int_warning: boo
+0003a1b0: 6c2c 2064 6566 6175 6c74 2054 7275 652e  l, default True.
+0003a1c0: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+0003a1d0: 6e3a 2073 7472 206f 7220 6469 6374 0d0a  n: str or dict..
+0003a1e0: 2020 2020 2020 2020 2222 220d 0a0d 0a20          """.... 
+0003a1f0: 2020 2020 2020 2074 696d 656f 7574 203d         timeout =
+0003a200: 206b 7761 7267 732e 6765 7428 2774 696d   kwargs.get('tim
+0003a210: 656f 7574 272c 204e 6f6e 6529 0d0a 2020  eout', None)..  
+0003a220: 2020 2020 2020 7072 6f78 6965 7320 3d20        proxies = 
+0003a230: 6b77 6172 6773 2e67 6574 2827 7072 6f78  kwargs.get('prox
+0003a240: 6965 7327 2c20 4e6f 6e65 290d 0a20 2020  ies', None)..   
+0003a250: 2020 2020 2073 6c65 6570 5f73 6563 6f6e       sleep_secon
+0003a260: 6473 203d 206b 7761 7267 732e 6765 7428  ds = kwargs.get(
+0003a270: 2773 6c65 6570 5f73 6563 6f6e 6473 272c  'sleep_seconds',
+0003a280: 2030 290d 0a20 2020 2020 2020 2069 665f   0)..        if_
+0003a290: 7072 696e 745f 7761 726e 696e 6720 3d20  print_warning = 
+0003a2a0: 6b77 6172 6773 2e67 6574 2827 6966 5f70  kwargs.get('if_p
+0003a2b0: 7269 6e74 5f77 6172 6e69 6e67 272c 2054  rint_warning', T
+0003a2c0: 7275 6529 0d0a 2020 2020 2020 2020 6973  rue)..        is
+0003a2d0: 5f64 6574 6169 6c5f 7265 7375 6c74 203d  _detail_result =
+0003a2e0: 206b 7761 7267 732e 6765 7428 2769 735f   kwargs.get('is_
+0003a2f0: 6465 7461 696c 5f72 6573 756c 7427 2c20  detail_result', 
+0003a300: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+0003a310: 7570 6461 7465 5f73 6573 7369 6f6e 5f61  update_session_a
+0003a320: 6674 6572 5f66 7265 7120 3d20 6b77 6172  fter_freq = kwar
+0003a330: 6773 2e67 6574 2827 7570 6461 7465 5f73  gs.get('update_s
+0003a340: 6573 7369 6f6e 5f61 6674 6572 5f66 7265  ession_after_fre
+0003a350: 7127 2c20 7365 6c66 2e64 6566 6175 6c74  q', self.default
+0003a360: 5f73 6573 7369 6f6e 5f66 7265 7129 0d0a  _session_freq)..
+0003a370: 2020 2020 2020 2020 7570 6461 7465 5f73          update_s
+0003a380: 6573 7369 6f6e 5f61 6674 6572 5f73 6563  ession_after_sec
+0003a390: 6f6e 6473 203d 206b 7761 7267 732e 6765  onds = kwargs.ge
+0003a3a0: 7428 2775 7064 6174 655f 7365 7373 696f  t('update_sessio
+0003a3b0: 6e5f 6166 7465 725f 7365 636f 6e64 7327  n_after_seconds'
+0003a3c0: 2c20 7365 6c66 2e64 6566 6175 6c74 5f73  , self.default_s
+0003a3d0: 6573 7369 6f6e 5f73 6563 6f6e 6473 290d  ession_seconds).
+0003a3e0: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
+0003a3f0: 6563 6b5f 696e 7075 745f 6c69 6d69 7428  eck_input_limit(
+0003a400: 7175 6572 795f 7465 7874 2c20 7365 6c66  query_text, self
+0003a410: 2e69 6e70 7574 5f6c 696d 6974 290d 0a0d  .input_limit)...
+0003a420: 0a20 2020 2020 2020 206e 6f74 5f75 7064  .        not_upd
+0003a430: 6174 655f 636f 6e64 5f66 7265 7120 3d20  ate_cond_freq = 
+0003a440: 3120 6966 2073 656c 662e 7175 6572 795f  1 if self.query_
+0003a450: 636f 756e 7420 3c20 7570 6461 7465 5f73  count < update_s
+0003a460: 6573 7369 6f6e 5f61 6674 6572 5f66 7265  ession_after_fre
+0003a470: 7120 656c 7365 2030 0d0a 2020 2020 2020  q else 0..      
+0003a480: 2020 6e6f 745f 7570 6461 7465 5f63 6f6e    not_update_con
+0003a490: 645f 7469 6d65 203d 2031 2069 6620 7469  d_time = 1 if ti
+0003a4a0: 6d65 2e74 696d 6528 2920 2d20 7365 6c66  me.time() - self
+0003a4b0: 2e62 6567 696e 5f74 696d 6520 3c20 7570  .begin_time < up
+0003a4c0: 6461 7465 5f73 6573 7369 6f6e 5f61 6674  date_session_aft
+0003a4d0: 6572 5f73 6563 6f6e 6473 2065 6c73 6520  er_seconds else 
+0003a4e0: 300d 0a20 2020 2020 2020 2069 6620 6e6f  0..        if no
+0003a4f0: 7420 2873 656c 662e 7365 7373 696f 6e20  t (self.session 
+0003a500: 616e 6420 7365 6c66 2e6c 616e 6775 6167  and self.languag
+0003a510: 655f 6d61 7020 616e 6420 6e6f 745f 7570  e_map and not_up
+0003a520: 6461 7465 5f63 6f6e 645f 6672 6571 2061  date_cond_freq a
+0003a530: 6e64 206e 6f74 5f75 7064 6174 655f 636f  nd not_update_co
+0003a540: 6e64 5f74 696d 6529 3a0d 0a20 2020 2020  nd_time):..     
+0003a550: 2020 2020 2020 2073 656c 662e 7365 7373         self.sess
+0003a560: 696f 6e20 3d20 7265 7175 6573 7473 2e53  ion = requests.S
+0003a570: 6573 7369 6f6e 2829 0d0a 2020 2020 2020  ession()..      
+0003a580: 2020 2020 2020 686f 7374 5f68 746d 6c20        host_html 
+0003a590: 3d20 7365 6c66 2e73 6573 7369 6f6e 2e67  = self.session.g
+0003a5a0: 6574 2873 656c 662e 686f 7374 5f75 726c  et(self.host_url
+0003a5b0: 2c20 6865 6164 6572 733d 7365 6c66 2e68  , headers=self.h
+0003a5c0: 6f73 745f 6865 6164 6572 732c 2074 696d  ost_headers, tim
+0003a5d0: 656f 7574 3d74 696d 656f 7574 2c20 7072  eout=timeout, pr
+0003a5e0: 6f78 6965 733d 7072 6f78 6965 7329 2e74  oxies=proxies).t
+0003a5f0: 6578 740d 0a20 2020 2020 2020 2020 2020  ext..           
+0003a600: 2064 6562 7567 5f6c 616e 675f 6b77 6172   debug_lang_kwar
+0003a610: 6773 203d 2073 656c 662e 6465 6275 675f  gs = self.debug_
+0003a620: 6c61 6e67 5f6b 7761 7267 7328 6672 6f6d  lang_kwargs(from
+0003a630: 5f6c 616e 6775 6167 652c 2074 6f5f 6c61  _language, to_la
+0003a640: 6e67 7561 6765 2c20 7365 6c66 2e64 6566  nguage, self.def
+0003a650: 6175 6c74 5f66 726f 6d5f 6c61 6e67 7561  ault_from_langua
+0003a660: 6765 2c20 6966 5f70 7269 6e74 5f77 6172  ge, if_print_war
+0003a670: 6e69 6e67 290d 0a20 2020 2020 2020 2020  ning)..         
+0003a680: 2020 2073 656c 662e 6c61 6e67 7561 6765     self.language
+0003a690: 5f6d 6170 203d 2073 656c 662e 6765 745f  _map = self.get_
+0003a6a0: 6c61 6e67 7561 6765 5f6d 6170 2868 6f73  language_map(hos
+0003a6b0: 745f 6874 6d6c 2c20 2a2a 6465 6275 675f  t_html, **debug_
+0003a6c0: 6c61 6e67 5f6b 7761 7267 7329 0d0a 0d0a  lang_kwargs)....
+0003a6d0: 2020 2020 2020 2020 6966 2066 726f 6d5f          if from_
+0003a6e0: 6c61 6e67 7561 6765 203d 3d20 2761 7574  language == 'aut
+0003a6f0: 6f27 3a0d 0a20 2020 2020 2020 2020 2020  o':..           
+0003a700: 2066 726f 6d5f 6c61 6e67 7561 6765 203d   from_language =
+0003a710: 2073 656c 662e 7761 726e 696e 675f 6175   self.warning_au
+0003a720: 746f 5f6c 616e 6728 2774 7261 6e73 6c61  to_lang('transla
+0003a730: 7465 4d65 272c 2073 656c 662e 6465 6661  teMe', self.defa
+0003a740: 756c 745f 6672 6f6d 5f6c 616e 6775 6167  ult_from_languag
+0003a750: 652c 2069 665f 7072 696e 745f 7761 726e  e, if_print_warn
+0003a760: 696e 6729 0d0a 2020 2020 2020 2020 6672  ing)..        fr
+0003a770: 6f6d 5f6c 616e 6775 6167 652c 2074 6f5f  om_language, to_
+0003a780: 6c61 6e67 7561 6765 203d 2073 656c 662e  language = self.
+0003a790: 6368 6563 6b5f 6c61 6e67 7561 6765 2866  check_language(f
+0003a7a0: 726f 6d5f 6c61 6e67 7561 6765 2c20 746f  rom_language, to
+0003a7b0: 5f6c 616e 6775 6167 652c 2073 656c 662e  _language, self.
+0003a7c0: 6c61 6e67 7561 6765 5f6d 6170 2c20 6f75  language_map, ou
+0003a7d0: 7470 7574 5f7a 683d 7365 6c66 2e6f 7574  tput_zh=self.out
+0003a7e0: 7075 745f 7a68 2c0d 0a20 2020 2020 2020  put_zh,..       
+0003a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003a820: 2020 6f75 7470 7574 5f65 6e5f 7472 616e    output_en_tran
+0003a830: 736c 6174 6f72 3d27 7472 616e 736c 6174  slator='translat
+0003a840: 654d 6527 2c20 6f75 7470 7574 5f65 6e3d  eMe', output_en=
+0003a850: 7365 6c66 2e6f 7574 7075 745f 656e 290d  self.output_en).
+0003a860: 0a0d 0a20 2020 2020 2020 2069 6620 7365  ...        if se
+0003a870: 6c66 2e6f 7574 7075 745f 656e 2069 6e20  lf.output_en in 
+0003a880: 2866 726f 6d5f 6c61 6e67 7561 6765 2c20  (from_language, 
+0003a890: 746f 5f6c 616e 6775 6167 6529 3a0d 0a20  to_language):.. 
+0003a8a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0003a8b0: 6e20 7365 6c66 2e5f 7472 616e 736c 6174  n self._translat
+0003a8c0: 654d 655f 6170 6928 7175 6572 795f 7465  eMe_api(query_te
+0003a8d0: 7874 2c20 6672 6f6d 5f6c 616e 6775 6167  xt, from_languag
+0003a8e0: 652c 2074 6f5f 6c61 6e67 7561 6765 2c20  e, to_language, 
+0003a8f0: 2a2a 6b77 6172 6773 290d 0a0d 0a20 2020  **kwargs)....   
+0003a900: 2020 2020 2074 6d70 5f6b 7761 7267 7320       tmp_kwargs 
+0003a910: 3d20 6b77 6172 6773 2e63 6f70 7928 290d  = kwargs.copy().
+0003a920: 0a20 2020 2020 2020 2074 6d70 5f6b 7761  .        tmp_kwa
+0003a930: 7267 732e 7570 6461 7465 287b 2769 735f  rgs.update({'is_
+0003a940: 6465 7461 696c 5f72 6573 756c 7427 3a20  detail_result': 
+0003a950: 4661 6c73 652c 2027 6966 5f73 686f 775f  False, 'if_show_
+0003a960: 7469 6d65 5f73 7461 7427 3a20 4661 6c73  time_stat': Fals
+0003a970: 657d 290d 0a20 2020 2020 2020 206e 6578  e})..        nex
+0003a980: 745f 7175 6572 795f 7465 7874 203d 2073  t_query_text = s
+0003a990: 656c 662e 5f74 7261 6e73 6c61 7465 4d65  elf._translateMe
+0003a9a0: 5f61 7069 2871 7565 7279 5f74 6578 742c  _api(query_text,
+0003a9b0: 2066 726f 6d5f 6c61 6e67 7561 6765 2c20   from_language, 
+0003a9c0: 7365 6c66 2e6f 7574 7075 745f 656e 2c20  self.output_en, 
+0003a9d0: 2a2a 746d 705f 6b77 6172 6773 290d 0a20  **tmp_kwargs).. 
+0003a9e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0003a9f0: 6c66 2e5f 7472 616e 736c 6174 654d 655f  lf._translateMe_
+0003aa00: 6170 6928 6e65 7874 5f71 7565 7279 5f74  api(next_query_t
+0003aa10: 6578 742c 2073 656c 662e 6f75 7470 7574  ext, self.output
+0003aa20: 5f65 6e2c 2074 6f5f 6c61 6e67 7561 6765  _en, to_language
+0003aa30: 2c20 2a2a 6b77 6172 6773 290d 0a0d 0a0d  , **kwargs).....
+0003aa40: 0a63 6c61 7373 2045 6c69 6128 5473 6529  .class Elia(Tse)
+0003aa50: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
+0003aa60: 745f 5f28 7365 6c66 293a 0d0a 2020 2020  t__(self):..    
+0003aa70: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+0003aa80: 6974 5f5f 2829 0d0a 2020 2020 2020 2020  it__()..        
+0003aa90: 7365 6c66 2e68 6f73 745f 7572 6c20 3d20  self.host_url = 
+0003aaa0: 2768 7474 7073 3a2f 2f65 6c69 612e 6575  'https://elia.eu
+0003aab0: 732f 7472 616e 736c 6174 6f72 270d 0a20  s/translator'.. 
+0003aac0: 2020 2020 2020 2073 656c 662e 6170 695f         self.api_
+0003aad0: 7572 6c20 3d20 2768 7474 7073 3a2f 2f65  url = 'https://e
+0003aae0: 6c69 612e 6575 732f 616a 6178 2f74 7261  lia.eus/ajax/tra
+0003aaf0: 6e73 6c61 7465 5f73 7472 696e 6727 0d0a  nslate_string'..
+0003ab00: 2020 2020 2020 2020 7365 6c66 2e64 6574          self.det
+0003ab10: 6563 745f 6c61 6e67 5f75 726c 203d 2027  ect_lang_url = '
+0003ab20: 6874 7470 733a 2f2f 656c 6961 2e65 7573  https://elia.eus
+0003ab30: 2f61 6a61 782f 6c61 6e67 7561 6765 5f64  /ajax/language_d
+0003ab40: 6574 6563 7469 6f6e 270d 0a20 2020 2020  etection'..     
+0003ab50: 2020 2073 656c 662e 686f 7374 5f68 6561     self.host_hea
+0003ab60: 6465 7273 203d 2073 656c 662e 6765 745f  ders = self.get_
+0003ab70: 6865 6164 6572 7328 7365 6c66 2e68 6f73  headers(self.hos
+0003ab80: 745f 7572 6c2c 2069 665f 6170 693d 4661  t_url, if_api=Fa
+0003ab90: 6c73 652c 2069 665f 7265 6665 7265 725f  lse, if_referer_
+0003aba0: 666f 725f 686f 7374 3d54 7275 6529 0d0a  for_host=True)..
+0003abb0: 2020 2020 2020 2020 7365 6c66 2e61 7069          self.api
+0003abc0: 5f68 6561 6465 7273 203d 2073 656c 662e  _headers = self.
+0003abd0: 6765 745f 6865 6164 6572 7328 7365 6c66  get_headers(self
+0003abe0: 2e68 6f73 745f 7572 6c2c 2069 665f 6170  .host_url, if_ap
+0003abf0: 693d 5472 7565 2c20 6966 5f61 6a61 785f  i=True, if_ajax_
+0003ac00: 666f 725f 6170 693d 5472 7565 290d 0a20  for_api=True).. 
+0003ac10: 2020 2020 2020 2073 656c 662e 7365 7373         self.sess
+0003ac20: 696f 6e20 3d20 4e6f 6e65 0d0a 2020 2020  ion = None..    
+0003ac30: 2020 2020 7365 6c66 2e6c 616e 6775 6167      self.languag
+0003ac40: 655f 6d61 7020 3d20 4e6f 6e65 0d0a 2020  e_map = None..  
+0003ac50: 2020 2020 2020 7365 6c66 2e70 726f 6665        self.profe
+0003ac60: 7373 696f 6e61 6c5f 6669 656c 6420 3d20  ssional_field = 
+0003ac70: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
+0003ac80: 6c66 2e6c 616e 6770 6169 725f 646f 6d61  lf.langpair_doma
+0003ac90: 696e 203d 204e 6f6e 650d 0a20 2020 2020  in = None..     
+0003aca0: 2020 2073 656c 662e 746f 6b65 6e20 3d20     self.token = 
+0003acb0: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
+0003acc0: 6c66 2e71 7565 7279 5f63 6f75 6e74 203d  lf.query_count =
+0003acd0: 2030 0d0a 2020 2020 2020 2020 7365 6c66   0..        self
+0003ace0: 2e6f 7574 7075 745f 7a68 203d 204e 6f6e  .output_zh = Non
+0003acf0: 6520 2023 2075 6e73 7570 706f 7274 6564  e  # unsupported
+0003ad00: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
+0003ad10: 6e70 7574 5f6c 696d 6974 203d 2069 6e74  nput_limit = int
+0003ad20: 2831 6532 290d 0a20 2020 2020 2020 2073  (1e2)..        s
+0003ad30: 656c 662e 6465 6661 756c 745f 6672 6f6d  elf.default_from
+0003ad40: 5f6c 616e 6775 6167 6520 3d20 2766 7227  _language = 'fr'
+0003ad50: 0d0a 0d0a 2020 2020 4054 7365 2e64 6562  ....    @Tse.deb
+0003ad60: 7567 5f6c 616e 6775 6167 655f 6d61 700d  ug_language_map.
+0003ad70: 0a20 2020 2064 6566 2067 6574 5f6c 616e  .    def get_lan
+0003ad80: 6775 6167 655f 6d61 7028 7365 6c66 2c20  guage_map(self, 
+0003ad90: 6464 3a20 6469 6374 2c20 2a2a 6b77 6172  dd: dict, **kwar
+0003ada0: 6773 3a20 4c61 6e67 4d61 704b 7761 7267  gs: LangMapKwarg
+0003adb0: 7354 7970 6529 202d 3e20 6469 6374 3a0d  sType) -> dict:.
+0003adc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0003add0: 7b69 695b 2773 6f75 7263 655f 6c61 6e67  {ii['source_lang
+0003ade0: 7561 6765 275d 5b27 636f 6465 275d 3a20  uage']['code']: 
+0003adf0: 5b6a 6a5b 2774 6172 6765 745f 6c61 6e67  [jj['target_lang
+0003ae00: 7561 6765 275d 5b27 636f 6465 275d 2066  uage']['code'] f
+0003ae10: 6f72 206a 6a20 696e 2064 645b 276c 616e  or jj in dd['lan
+0003ae20: 6775 6167 655f 7061 6972 7327 5d20 6966  guage_pairs'] if
+0003ae30: 206a 6a5b 2773 6f75 7263 655f 6c61 6e67   jj['source_lang
+0003ae40: 7561 6765 275d 5b27 636f 6465 275d 203d  uage']['code'] =
+0003ae50: 3d20 6969 5b27 736f 7572 6365 5f6c 616e  = ii['source_lan
+0003ae60: 6775 6167 6527 5d5b 2763 6f64 6527 5d5d  guage']['code']]
+0003ae70: 2066 6f72 2069 6920 696e 2064 645b 276c   for ii in dd['l
+0003ae80: 616e 6775 6167 655f 7061 6972 7327 5d7d  anguage_pairs']}
+0003ae90: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
+0003aea0: 7072 6f66 6573 7369 6f6e 616c 5f66 6965  professional_fie
+0003aeb0: 6c64 5f6c 6973 7428 7365 6c66 2c20 6464  ld_list(self, dd
+0003aec0: 3a20 6469 6374 2920 2d3e 2073 6574 3a0d  : dict) -> set:.
+0003aed0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0003aee0: 7b69 745b 2774 7261 6e73 6c61 7469 6f6e  {it['translation
+0003aef0: 5f6d 6f64 656c 275d 5b27 636f 6465 275d  _model']['code']
+0003af00: 2066 6f72 2069 7420 696e 2064 645b 276c   for it in dd['l
+0003af10: 616e 6775 6167 655f 7061 6972 7327 5d7d  anguage_pairs']}
+0003af20: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
+0003af30: 6c61 6e67 7061 6972 5f64 6f6d 6169 6e28  langpair_domain(
+0003af40: 7365 6c66 2c20 6464 3a20 6469 6374 2920  self, dd: dict) 
+0003af50: 2d3e 2064 6963 743a 0d0a 2020 2020 2020  -> dict:..      
+0003af60: 2020 6461 7461 203d 207b 0d0a 2020 2020    data = {..    
+0003af70: 2020 2020 2020 2020 6627 7b69 7465 6d5b          f'{item[
+0003af80: 2273 6f75 7263 655f 6c61 6e67 7561 6765  "source_language
+0003af90: 225d 5b22 636f 6465 225d 7d5f 5f7b 6974  "]["code"]}__{it
+0003afa0: 656d 5b22 7461 7267 6574 5f6c 616e 6775  em["target_langu
+0003afb0: 6167 6522 5d5b 2263 6f64 6522 5d7d 5f5f  age"]["code"]}__
+0003afc0: 7b69 7465 6d5b 2274 7261 6e73 6c61 7469  {item["translati
+0003afd0: 6f6e 5f6d 6f64 656c 225d 5b22 636f 6465  on_model"]["code
+0003afe0: 225d 7d27 3a20 7b0d 0a20 2020 2020 2020  "]}': {..       
+0003aff0: 2020 2020 2020 2020 2027 7472 616e 736c           'transl
+0003b000: 6174 696f 6e5f 656e 6769 6e65 273a 2069  ation_engine': i
+0003b010: 7465 6d5b 2265 6e67 696e 6522 5d5b 2270  tem["engine"]["p
+0003b020: 6b22 5d2c 0d0a 2020 2020 2020 2020 2020  k"],..          
+0003b030: 2020 7d20 666f 7220 6974 656d 2069 6e20    } for item in 
+0003b040: 6464 5b27 6c61 6e67 7561 6765 5f70 6169  dd['language_pai
+0003b050: 7273 275d 0d0a 2020 2020 2020 2020 7d0d  rs']..        }.
+0003b060: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0003b070: 6461 7461 0d0a 0d0a 2020 2020 4054 7365  data....    @Tse
+0003b080: 2e74 696d 655f 7374 6174 0d0a 2020 2020  .time_stat..    
+0003b090: 4054 7365 2e63 6865 636b 5f71 7565 7279  @Tse.check_query
+0003b0a0: 0d0a 2020 2020 6465 6620 656c 6961 5f61  ..    def elia_a
+0003b0b0: 7069 2873 656c 662c 2071 7565 7279 5f74  pi(self, query_t
+0003b0c0: 6578 743a 2073 7472 2c20 6672 6f6d 5f6c  ext: str, from_l
+0003b0d0: 616e 6775 6167 653a 2073 7472 203d 2027  anguage: str = '
+0003b0e0: 6175 746f 272c 2074 6f5f 6c61 6e67 7561  auto', to_langua
+0003b0f0: 6765 3a20 7374 7220 3d20 2765 6e27 2c20  ge: str = 'en', 
+0003b100: 2a2a 6b77 6172 6773 3a20 4170 694b 7761  **kwargs: ApiKwa
+0003b110: 7267 7354 7970 6529 202d 3e20 556e 696f  rgsType) -> Unio
+0003b120: 6e5b 7374 722c 2064 6963 745d 3a0d 0a20  n[str, dict]:.. 
+0003b130: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0003b140: 2020 2020 6874 7470 733a 2f2f 656c 6961      https://elia
+0003b150: 2e65 7573 2f74 7261 6e73 6c61 746f 720d  .eus/translator.
+0003b160: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0003b170: 7175 6572 795f 7465 7874 3a20 7374 722c  query_text: str,
+0003b180: 206d 7573 742e 0d0a 2020 2020 2020 2020   must...        
+0003b190: 3a70 6172 616d 2066 726f 6d5f 6c61 6e67  :param from_lang
+0003b1a0: 7561 6765 3a20 7374 722c 2064 6566 6175  uage: str, defau
+0003b1b0: 6c74 2027 6175 746f 272e 0d0a 2020 2020  lt 'auto'...    
+0003b1c0: 2020 2020 3a70 6172 616d 2074 6f5f 6c61      :param to_la
+0003b1d0: 6e67 7561 6765 3a20 7374 722c 2064 6566  nguage: str, def
+0003b1e0: 6175 6c74 2027 656e 272e 0d0a 2020 2020  ault 'en'...    
+0003b1f0: 2020 2020 3a70 6172 616d 202a 2a6b 7761      :param **kwa
+0003b200: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+0003b210: 2020 2020 2020 3a70 6172 616d 2074 696d        :param tim
+0003b220: 656f 7574 3a20 666c 6f61 742c 2064 6566  eout: float, def
+0003b230: 6175 6c74 204e 6f6e 652e 0d0a 2020 2020  ault None...    
+0003b240: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0003b250: 616d 2070 726f 7869 6573 3a20 6469 6374  am proxies: dict
+0003b260: 2c20 6465 6661 756c 7420 4e6f 6e65 2e0d  , default None..
+0003b270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003b280: 203a 7061 7261 6d20 736c 6565 705f 7365   :param sleep_se
+0003b290: 636f 6e64 733a 2066 6c6f 6174 2c20 6465  conds: float, de
+0003b2a0: 6661 756c 7420 302e 0d0a 2020 2020 2020  fault 0...      
+0003b2b0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+0003b2c0: 2069 735f 6465 7461 696c 5f72 6573 756c   is_detail_resul
+0003b2d0: 743a 2062 6f6f 6c2c 2064 6566 6175 6c74  t: bool, default
+0003b2e0: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
+0003b2f0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+0003b300: 6966 5f69 676e 6f72 655f 6c69 6d69 745f  if_ignore_limit_
+0003b310: 6f66 5f6c 656e 6774 683a 2062 6f6f 6c2c  of_length: bool,
+0003b320: 2064 6566 6175 6c74 2046 616c 7365 2e0d   default False..
+0003b330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003b340: 203a 7061 7261 6d20 6c69 6d69 745f 6f66   :param limit_of
+0003b350: 5f6c 656e 6774 683a 2069 6e74 2c20 6465  _length: int, de
+0003b360: 6661 756c 7420 3230 3030 302e 0d0a 2020  fault 20000...  
+0003b370: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+0003b380: 6172 616d 2069 665f 6967 6e6f 7265 5f65  aram if_ignore_e
+0003b390: 6d70 7479 5f71 7565 7279 3a20 626f 6f6c  mpty_query: bool
+0003b3a0: 2c20 6465 6661 756c 7420 4661 6c73 652e  , default False.
+0003b3b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0003b3c0: 2020 3a70 6172 616d 2075 7064 6174 655f    :param update_
+0003b3d0: 7365 7373 696f 6e5f 6166 7465 725f 6672  session_after_fr
+0003b3e0: 6571 3a20 696e 742c 2064 6566 6175 6c74  eq: int, default
+0003b3f0: 2031 3030 302e 0d0a 2020 2020 2020 2020   1000...        
+0003b400: 2020 2020 2020 2020 3a70 6172 616d 2075          :param u
+0003b410: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
+0003b420: 7465 725f 7365 636f 6e64 733a 2066 6c6f  ter_seconds: flo
+0003b430: 6174 2c20 6465 6661 756c 7420 3135 3030  at, default 1500
+0003b440: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0003b450: 2020 203a 7061 7261 6d20 6966 5f73 686f     :param if_sho
+0003b460: 775f 7469 6d65 5f73 7461 743a 2062 6f6f  w_time_stat: boo
+0003b470: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+0003b480: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0003b490: 2020 203a 7061 7261 6d20 7368 6f77 5f74     :param show_t
+0003b4a0: 696d 655f 7374 6174 5f70 7265 6369 7369  ime_stat_precisi
+0003b4b0: 6f6e 3a20 696e 742c 2064 6566 6175 6c74  on: int, default
+0003b4c0: 2032 2e0d 0a20 2020 2020 2020 2020 2020   2...           
+0003b4d0: 2020 2020 203a 7061 7261 6d20 6966 5f70       :param if_p
+0003b4e0: 7269 6e74 5f77 6172 6e69 6e67 3a20 626f  rint_warning: bo
+0003b4f0: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+0003b500: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0003b510: 2020 203a 7061 7261 6d20 7072 6f66 6573     :param profes
+0003b520: 7369 6f6e 616c 5f66 6965 6c64 3a20 7374  sional_field: st
+0003b530: 722c 2064 6566 6175 6c74 2027 6765 6e65  r, default 'gene
+0003b540: 7261 6c27 2e20 4368 6f6f 7365 2066 726f  ral'. Choose fro
+0003b550: 6d20 2827 6765 6e65 7261 6c27 2c20 2761  m ('general', 'a
+0003b560: 646d 696e 2729 2e0d 0a20 2020 2020 2020  dmin')...       
+0003b570: 203a 7265 7475 726e 3a20 7374 7220 6f72   :return: str or
+0003b580: 2064 6963 740d 0a20 2020 2020 2020 2022   dict..        "
+0003b590: 2222 0d0a 0d0a 2020 2020 2020 2020 7573  ""....        us
+0003b5a0: 655f 646f 6d61 696e 203d 206b 7761 7267  e_domain = kwarg
+0003b5b0: 732e 6765 7428 2770 726f 6665 7373 696f  s.get('professio
+0003b5c0: 6e61 6c5f 6669 656c 6427 2c20 2767 656e  nal_field', 'gen
+0003b5d0: 6572 616c 2729 0d0a 2020 2020 2020 2020  eral')..        
+0003b5e0: 7469 6d65 6f75 7420 3d20 6b77 6172 6773  timeout = kwargs
+0003b5f0: 2e67 6574 2827 7469 6d65 6f75 7427 2c20  .get('timeout', 
+0003b600: 4e6f 6e65 290d 0a20 2020 2020 2020 2070  None)..        p
+0003b610: 726f 7869 6573 203d 206b 7761 7267 732e  roxies = kwargs.
+0003b620: 6765 7428 2770 726f 7869 6573 272c 204e  get('proxies', N
+0003b630: 6f6e 6529 0d0a 2020 2020 2020 2020 736c  one)..        sl
+0003b640: 6565 705f 7365 636f 6e64 7320 3d20 6b77  eep_seconds = kw
+0003b650: 6172 6773 2e67 6574 2827 736c 6565 705f  args.get('sleep_
+0003b660: 7365 636f 6e64 7327 2c20 3029 0d0a 2020  seconds', 0)..  
+0003b670: 2020 2020 2020 6966 5f70 7269 6e74 5f77        if_print_w
+0003b680: 6172 6e69 6e67 203d 206b 7761 7267 732e  arning = kwargs.
+0003b690: 6765 7428 2769 665f 7072 696e 745f 7761  get('if_print_wa
+0003b6a0: 726e 696e 6727 2c20 5472 7565 290d 0a20  rning', True).. 
+0003b6b0: 2020 2020 2020 2069 735f 6465 7461 696c         is_detail
+0003b6c0: 5f72 6573 756c 7420 3d20 6b77 6172 6773  _result = kwargs
+0003b6d0: 2e67 6574 2827 6973 5f64 6574 6169 6c5f  .get('is_detail_
+0003b6e0: 7265 7375 6c74 272c 2046 616c 7365 290d  result', False).
+0003b6f0: 0a20 2020 2020 2020 2075 7064 6174 655f  .        update_
+0003b700: 7365 7373 696f 6e5f 6166 7465 725f 6672  session_after_fr
+0003b710: 6571 203d 206b 7761 7267 732e 6765 7428  eq = kwargs.get(
+0003b720: 2775 7064 6174 655f 7365 7373 696f 6e5f  'update_session_
+0003b730: 6166 7465 725f 6672 6571 272c 2073 656c  after_freq', sel
+0003b740: 662e 6465 6661 756c 745f 7365 7373 696f  f.default_sessio
+0003b750: 6e5f 6672 6571 290d 0a20 2020 2020 2020  n_freq)..       
+0003b760: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
+0003b770: 6166 7465 725f 7365 636f 6e64 7320 3d20  after_seconds = 
+0003b780: 6b77 6172 6773 2e67 6574 2827 7570 6461  kwargs.get('upda
+0003b790: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
+0003b7a0: 5f73 6563 6f6e 6473 272c 2073 656c 662e  _seconds', self.
+0003b7b0: 6465 6661 756c 745f 7365 7373 696f 6e5f  default_session_
+0003b7c0: 7365 636f 6e64 7329 0d0a 2020 2020 2020  seconds)..      
+0003b7d0: 2020 7365 6c66 2e63 6865 636b 5f69 6e70    self.check_inp
+0003b7e0: 7574 5f6c 696d 6974 2871 7565 7279 5f74  ut_limit(query_t
+0003b7f0: 6578 742c 2073 656c 662e 696e 7075 745f  ext, self.input_
+0003b800: 6c69 6d69 7429 0d0a 0d0a 2020 2020 2020  limit)....      
+0003b810: 2020 6e6f 745f 7570 6461 7465 5f63 6f6e    not_update_con
+0003b820: 645f 6672 6571 203d 2031 2069 6620 7365  d_freq = 1 if se
+0003b830: 6c66 2e71 7565 7279 5f63 6f75 6e74 203c  lf.query_count <
+0003b840: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
+0003b850: 6166 7465 725f 6672 6571 2065 6c73 6520  after_freq else 
+0003b860: 300d 0a20 2020 2020 2020 206e 6f74 5f75  0..        not_u
+0003b870: 7064 6174 655f 636f 6e64 5f74 696d 6520  pdate_cond_time 
+0003b880: 3d20 3120 6966 2074 696d 652e 7469 6d65  = 1 if time.time
+0003b890: 2829 202d 2073 656c 662e 6265 6769 6e5f  () - self.begin_
+0003b8a0: 7469 6d65 203c 2075 7064 6174 655f 7365  time < update_se
+0003b8b0: 7373 696f 6e5f 6166 7465 725f 7365 636f  ssion_after_seco
+0003b8c0: 6e64 7320 656c 7365 2030 0d0a 2020 2020  nds else 0..    
+0003b8d0: 2020 2020 6966 206e 6f74 2028 7365 6c66      if not (self
+0003b8e0: 2e73 6573 7369 6f6e 2061 6e64 2073 656c  .session and sel
+0003b8f0: 662e 6c61 6e67 7561 6765 5f6d 6170 2061  f.language_map a
+0003b900: 6e64 206e 6f74 5f75 7064 6174 655f 636f  nd not_update_co
+0003b910: 6e64 5f66 7265 7120 616e 6420 6e6f 745f  nd_freq and not_
+0003b920: 7570 6461 7465 5f63 6f6e 645f 7469 6d65  update_cond_time
+0003b930: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0003b940: 7365 6c66 2e73 6573 7369 6f6e 203d 2072  self.session = r
+0003b950: 6571 7565 7374 732e 5365 7373 696f 6e28  equests.Session(
+0003b960: 290d 0a20 2020 2020 2020 2020 2020 2068  )..            h
+0003b970: 6f73 745f 6874 6d6c 203d 2073 656c 662e  ost_html = self.
+0003b980: 7365 7373 696f 6e2e 6765 7428 7365 6c66  session.get(self
+0003b990: 2e68 6f73 745f 7572 6c2c 2068 6561 6465  .host_url, heade
+0003b9a0: 7273 3d73 656c 662e 686f 7374 5f68 6561  rs=self.host_hea
+0003b9b0: 6465 7273 2c20 7469 6d65 6f75 743d 7469  ders, timeout=ti
+0003b9c0: 6d65 6f75 742c 2070 726f 7869 6573 3d70  meout, proxies=p
+0003b9d0: 726f 7869 6573 292e 7465 7874 0d0a 2020  roxies).text..  
+0003b9e0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0003b9f0: 6f6b 656e 203d 2072 652e 636f 6d70 696c  oken = re.compil
+0003ba00: 6528 2722 6373 7266 6d69 6464 6c65 7761  e('"csrfmiddlewa
+0003ba10: 7265 746f 6b65 6e22 3a20 2228 2e2a 3f29  retoken": "(.*?)
+0003ba20: 2227 292e 7365 6172 6368 2868 6f73 745f  "').search(host_
+0003ba30: 6874 6d6c 292e 6772 6f75 7028 3129 0d0a  html).group(1)..
+0003ba40: 2020 2020 2020 2020 2020 2020 645f 6c61              d_la
+0003ba50: 6e67 5f73 7472 203d 2072 652e 636f 6d70  ng_str = re.comp
+0003ba60: 696c 6528 2776 6172 206c 616e 6775 6167  ile('var languag
+0003ba70: 6550 6169 7273 203d 204a 534f 4e2e 7061  ePairs = JSON.pa
+0003ba80: 7273 655c 5c28 282e 2a3f 295c 5c29 3b27  rse\\((.*?)\\);'
+0003ba90: 292e 7365 6172 6368 2868 6f73 745f 6874  ).search(host_ht
+0003baa0: 6d6c 292e 6772 6f75 7028 290d 0a20 2020  ml).group()..   
+0003bab0: 2020 2020 2020 2020 2064 5f6c 616e 675f           d_lang_
+0003bac0: 6d61 7020 3d20 6a73 6f6e 2e6c 6f61 6473  map = json.loads
+0003bad0: 2864 5f6c 616e 675f 7374 725b 3433 3a2d  (d_lang_str[43:-
+0003bae0: 345d 2e72 6570 6c61 6365 2827 2671 756f  4].replace('&quo
+0003baf0: 743b 272c 2027 2227 2929 0d0a 2020 2020  t;', '"'))..    
+0003bb00: 2020 2020 2020 2020 6465 6275 675f 6c61          debug_la
+0003bb10: 6e67 5f6b 7761 7267 7320 3d20 7365 6c66  ng_kwargs = self
+0003bb20: 2e64 6562 7567 5f6c 616e 675f 6b77 6172  .debug_lang_kwar
+0003bb30: 6773 2866 726f 6d5f 6c61 6e67 7561 6765  gs(from_language
+0003bb40: 2c20 746f 5f6c 616e 6775 6167 652c 2073  , to_language, s
+0003bb50: 656c 662e 6465 6661 756c 745f 6672 6f6d  elf.default_from
+0003bb60: 5f6c 616e 6775 6167 652c 2069 665f 7072  _language, if_pr
+0003bb70: 696e 745f 7761 726e 696e 6729 0d0a 2020  int_warning)..  
+0003bb80: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0003bb90: 616e 6775 6167 655f 6d61 7020 3d20 7365  anguage_map = se
+0003bba0: 6c66 2e67 6574 5f6c 616e 6775 6167 655f  lf.get_language_
+0003bbb0: 6d61 7028 645f 6c61 6e67 5f6d 6170 2c20  map(d_lang_map, 
+0003bbc0: 2a2a 6465 6275 675f 6c61 6e67 5f6b 7761  **debug_lang_kwa
+0003bbd0: 7267 7329 0d0a 2020 2020 2020 2020 2020  rgs)..          
+0003bbe0: 2020 7365 6c66 2e70 726f 6665 7373 696f    self.professio
+0003bbf0: 6e61 6c5f 6669 656c 6420 3d20 7365 6c66  nal_field = self
+0003bc00: 2e67 6574 5f70 726f 6665 7373 696f 6e61  .get_professiona
+0003bc10: 6c5f 6669 656c 645f 6c69 7374 2864 5f6c  l_field_list(d_l
+0003bc20: 616e 675f 6d61 7029 0d0a 2020 2020 2020  ang_map)..      
+0003bc30: 2020 2020 2020 7365 6c66 2e6c 616e 6770        self.langp
+0003bc40: 6169 725f 646f 6d61 696e 203d 2073 656c  air_domain = sel
+0003bc50: 662e 6765 745f 6c61 6e67 7061 6972 5f64  f.get_langpair_d
+0003bc60: 6f6d 6169 6e28 645f 6c61 6e67 5f6d 6170  omain(d_lang_map
+0003bc70: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
+0003bc80: 6672 6f6d 5f6c 616e 6775 6167 6520 3d3d  from_language ==
+0003bc90: 2027 6175 746f 273a 0d0a 2020 2020 2020   'auto':..      
+0003bca0: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
+0003bcb0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+0003bcc0: 2020 2027 7465 7874 273a 2071 7565 7279     'text': query
+0003bcd0: 5f74 6578 742c 0d0a 2020 2020 2020 2020  _text,..        
+0003bce0: 2020 2020 2020 2020 2763 7372 666d 6964          'csrfmid
+0003bcf0: 646c 6577 6172 6574 6f6b 656e 273a 2073  dlewaretoken': s
+0003bd00: 656c 662e 746f 6b65 6e2c 0d0a 2020 2020  elf.token,..    
+0003bd10: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+0003bd20: 2020 2020 2020 2070 6179 6c6f 6164 203d         payload =
+0003bd30: 2075 726c 6c69 622e 7061 7273 652e 7572   urllib.parse.ur
+0003bd40: 6c65 6e63 6f64 6528 7061 796c 6f61 6429  lencode(payload)
+0003bd50: 0d0a 2020 2020 2020 2020 2020 2020 7220  ..            r 
+0003bd60: 3d20 7365 6c66 2e73 6573 7369 6f6e 2e70  = self.session.p
+0003bd70: 6f73 7428 7365 6c66 2e64 6574 6563 745f  ost(self.detect_
+0003bd80: 6c61 6e67 5f75 726c 2c20 6461 7461 3d70  lang_url, data=p
+0003bd90: 6179 6c6f 6164 2c20 6865 6164 6572 733d  ayload, headers=
+0003bda0: 7365 6c66 2e61 7069 5f68 6561 6465 7273  self.api_headers
+0003bdb0: 2c20 7469 6d65 6f75 743d 7469 6d65 6f75  , timeout=timeou
+0003bdc0: 742c 2070 726f 7869 6573 3d70 726f 7869  t, proxies=proxi
+0003bdd0: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+0003bde0: 2066 726f 6d5f 6c61 6e67 7561 6765 203d   from_language =
+0003bdf0: 2072 2e6a 736f 6e28 295b 276c 616e 675f   r.json()['lang_
+0003be00: 6964 275d 0d0a 2020 2020 2020 2020 6672  id']..        fr
+0003be10: 6f6d 5f6c 616e 6775 6167 652c 2074 6f5f  om_language, to_
+0003be20: 6c61 6e67 7561 6765 203d 2073 656c 662e  language = self.
+0003be30: 6368 6563 6b5f 6c61 6e67 7561 6765 2866  check_language(f
+0003be40: 726f 6d5f 6c61 6e67 7561 6765 2c20 746f  rom_language, to
+0003be50: 5f6c 616e 6775 6167 652c 2073 656c 662e  _language, self.
+0003be60: 6c61 6e67 7561 6765 5f6d 6170 290d 0a0d  language_map)...
+0003be70: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+0003be80: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
+0003be90: 2020 2769 6e70 7574 5f74 6578 7427 3a20    'input_text': 
+0003bea0: 7175 6572 795f 7465 7874 2c0d 0a20 2020  query_text,..   
+0003beb0: 2020 2020 2020 2020 2027 736f 7572 6365           'source
+0003bec0: 5f6c 616e 6775 6167 6527 3a20 6672 6f6d  _language': from
+0003bed0: 5f6c 616e 6775 6167 652c 0d0a 2020 2020  _language,..    
+0003bee0: 2020 2020 2020 2020 2774 6172 6765 745f          'target_
+0003bef0: 6c61 6e67 7561 6765 273a 2074 6f5f 6c61  language': to_la
+0003bf00: 6e67 7561 6765 2c0d 0a20 2020 2020 2020  nguage,..       
+0003bf10: 2020 2020 2027 7472 616e 736c 6174 696f       'translatio
+0003bf20: 6e5f 6d6f 6465 6c27 3a20 7573 655f 646f  n_model': use_do
+0003bf30: 6d61 696e 2c0d 0a20 2020 2020 2020 2020  main,..         
+0003bf40: 2020 2027 7472 616e 736c 6174 696f 6e5f     'translation_
+0003bf50: 656e 6769 6e65 273a 2031 2c0d 0a20 2020  engine': 1,..   
+0003bf60: 2020 2020 2020 2020 2027 6373 7266 6d69           'csrfmi
+0003bf70: 6464 6c65 7761 7265 746f 6b65 6e27 3a20  ddlewaretoken': 
+0003bf80: 7365 6c66 2e74 6f6b 656e 2c0d 0a20 2020  self.token,..   
+0003bf90: 2020 2020 207d 0d0a 0d0a 2020 2020 2020       }....      
+0003bfa0: 2020 646f 6d61 696e 5f70 6179 6c6f 6164    domain_payload
+0003bfb0: 203d 2073 656c 662e 6c61 6e67 7061 6972   = self.langpair
+0003bfc0: 5f64 6f6d 6169 6e2e 6765 7428 6627 7b66  _domain.get(f'{f
+0003bfd0: 726f 6d5f 6c61 6e67 7561 6765 7d5f 5f7b  rom_language}__{
+0003bfe0: 746f 5f6c 616e 6775 6167 657d 5f5f 7b75  to_language}__{u
+0003bff0: 7365 5f64 6f6d 6169 6e7d 2729 0d0a 2020  se_domain}')..  
+0003c000: 2020 2020 2020 6966 206e 6f74 2064 6f6d        if not dom
+0003c010: 6169 6e5f 7061 796c 6f61 643a 0d0a 2020  ain_payload:..  
+0003c020: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0003c030: 5472 616e 736c 6174 6f72 4572 726f 720d  TranslatorError.
+0003c040: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+0003c050: 2020 2020 2020 2020 2020 2020 7061 796c              payl
+0003c060: 6f61 642e 7570 6461 7465 2864 6f6d 6169  oad.update(domai
+0003c070: 6e5f 7061 796c 6f61 6429 0d0a 0d0a 2020  n_payload)....  
+0003c080: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
+0003c090: 7572 6c6c 6962 2e70 6172 7365 2e75 726c  urllib.parse.url
+0003c0a0: 656e 636f 6465 2870 6179 6c6f 6164 290d  encode(payload).
+0003c0b0: 0a20 2020 2020 2020 2072 203d 2073 656c  .        r = sel
+0003c0c0: 662e 7365 7373 696f 6e2e 706f 7374 2873  f.session.post(s
+0003c0d0: 656c 662e 6170 695f 7572 6c2c 2064 6174  elf.api_url, dat
+0003c0e0: 613d 7061 796c 6f61 642c 2068 6561 6465  a=payload, heade
+0003c0f0: 7273 3d73 656c 662e 6170 695f 6865 6164  rs=self.api_head
+0003c100: 6572 732c 2074 696d 656f 7574 3d74 696d  ers, timeout=tim
+0003c110: 656f 7574 2c20 7072 6f78 6965 733d 7072  eout, proxies=pr
+0003c120: 6f78 6965 7329 0d0a 2020 2020 2020 2020  oxies)..        
+0003c130: 722e 7261 6973 655f 666f 725f 7374 6174  r.raise_for_stat
+0003c140: 7573 2829 0d0a 2020 2020 2020 2020 6461  us()..        da
+0003c150: 7461 203d 2072 2e6a 736f 6e28 290d 0a20  ta = r.json().. 
+0003c160: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
+0003c170: 7028 736c 6565 705f 7365 636f 6e64 7329  p(sleep_seconds)
+0003c180: 0d0a 2020 2020 2020 2020 7365 6c66 2e71  ..        self.q
+0003c190: 7565 7279 5f63 6f75 6e74 202b 3d20 310d  uery_count += 1.
+0003c1a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0003c1b0: 6461 7461 2069 6620 6973 5f64 6574 6169  data if is_detai
+0003c1c0: 6c5f 7265 7375 6c74 2065 6c73 6520 6461  l_result else da
+0003c1d0: 7461 5b27 7472 616e 736c 6174 6564 5f74  ta['translated_t
+0003c1e0: 6578 7427 5d2e 7265 706c 6163 6528 273c  ext'].replace('<
+0003c1f0: 2f64 6976 3e27 2c20 275c 6e27 292e 7265  /div>', '\n').re
+0003c200: 706c 6163 6528 273c 6469 763e 272c 2027  place('<div>', '
+0003c210: 2729 2e72 6570 6c61 6365 2827 3c73 7061  ').replace('<spa
+0003c220: 6e3e 272c 2027 2729 2e72 6570 6c61 6365  n>', '').replace
+0003c230: 2827 3c2f 7370 616e 3e27 2c20 2727 290d  ('</span>', '').
+0003c240: 0a0d 0a0d 0a63 6c61 7373 204c 616e 6775  .....class Langu
+0003c250: 6167 6557 6972 6528 5473 6529 3a0d 0a20  ageWire(Tse):.. 
+0003c260: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0003c270: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+0003c280: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+0003c290: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+0003c2a0: 2e68 6f6d 655f 7572 6c20 3d20 2768 7474  .home_url = 'htt
+0003c2b0: 7073 3a2f 2f6a 7774 2e6c 616e 6775 6167  ps://jwt.languag
+0003c2c0: 6577 6972 652e 636f 6d27 0d0a 2020 2020  ewire.com'..    
+0003c2d0: 2020 2020 7365 6c66 2e68 6f73 745f 7572      self.host_ur
+0003c2e0: 6c20 3d20 2768 7474 7073 3a2f 2f77 7777  l = 'https://www
+0003c2f0: 2e6c 616e 6775 6167 6577 6972 652e 636f  .languagewire.co
+0003c300: 6d2f 656e 2f74 6563 686e 6f6c 6f67 792f  m/en/technology/
+0003c310: 6c61 6e67 7561 6765 7769 7265 2d74 7261  languagewire-tra
+0003c320: 6e73 6c61 7465 270d 0a20 2020 2020 2020  nslate'..       
+0003c330: 2073 656c 662e 6170 695f 7572 6c20 3d20   self.api_url = 
+0003c340: 2768 7474 7073 3a2f 2f6c 7774 2e6c 616e  'https://lwt.lan
+0003c350: 6775 6167 6577 6972 652e 636f 6d2f 662f  guagewire.com/f/
+0003c360: 6170 692f 7631 2f74 7261 6e73 6c61 7469  api/v1/translati
+0003c370: 6f6e 732f 7465 7874 270d 0a20 2020 2020  ons/text'..     
+0003c380: 2020 2073 656c 662e 6c61 6e67 5f75 726c     self.lang_url
+0003c390: 203d 2027 6874 7470 733a 2f2f 6c77 742e   = 'https://lwt.
+0003c3a0: 6c61 6e67 7561 6765 7769 7265 2e63 6f6d  languagewire.com
+0003c3b0: 2f66 2f61 7069 2f76 312f 6c61 6e67 7561  /f/api/v1/langua
+0003c3c0: 6765 2d70 6169 7273 3f69 6e63 6c75 6465  ge-pairs?include
+0003c3d0: 5661 7269 616e 7473 3d74 7275 6527 0d0a  Variants=true'..
+0003c3e0: 2020 2020 2020 2020 7365 6c66 2e63 6f6f          self.coo
+0003c3f0: 6b69 655f 7572 6c20 3d20 2768 7474 7073  kie_url = 'https
+0003c400: 3a2f 2f6c 7774 2e6c 616e 6775 6167 6577  ://lwt.languagew
+0003c410: 6972 652e 636f 6d2f 662f 6170 692f 7631  ire.com/f/api/v1
+0003c420: 2f61 7574 682f 636f 6f6b 6965 270d 0a20  /auth/cookie'.. 
+0003c430: 2020 2020 2020 2073 656c 662e 6c77 745f         self.lwt_
+0003c440: 6a73 5f75 726c 203d 2027 6874 7470 733a  js_url = 'https:
+0003c450: 2f2f 6c77 742e 6c61 6e67 7561 6765 7769  //lwt.languagewi
+0003c460: 7265 2e63 6f6d 2f65 6e2f 6d61 696e 2e36  re.com/en/main.6
+0003c470: 6632 3032 3935 6231 3034 6263 3532 612e  f20295b104bc52a.
+0003c480: 6a73 270d 0a20 2020 2020 2020 2073 656c  js'..        sel
+0003c490: 662e 686f 7374 5f68 6561 6465 7273 203d  f.host_headers =
+0003c4a0: 2073 656c 662e 6765 745f 6865 6164 6572   self.get_header
+0003c4b0: 7328 7365 6c66 2e68 6f6d 655f 7572 6c2c  s(self.home_url,
+0003c4c0: 2069 665f 6170 693d 4661 6c73 652c 2069   if_api=False, i
+0003c4d0: 665f 7265 6665 7265 725f 666f 725f 686f  f_referer_for_ho
+0003c4e0: 7374 3d54 7275 6529 0d0a 2020 2020 2020  st=True)..      
+0003c4f0: 2020 7365 6c66 2e61 7069 5f68 6561 6465    self.api_heade
+0003c500: 7273 203d 2073 656c 662e 6765 745f 6865  rs = self.get_he
+0003c510: 6164 6572 7328 7365 6c66 2e68 6f6d 655f  aders(self.home_
+0003c520: 7572 6c2c 2069 665f 6170 693d 5472 7565  url, if_api=True
+0003c530: 2c20 6966 5f6a 736f 6e5f 666f 725f 6170  , if_json_for_ap
+0003c540: 693d 5472 7565 290d 0a20 2020 2020 2020  i=True)..       
+0003c550: 2073 656c 662e 7365 7373 696f 6e20 3d20   self.session = 
+0003c560: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
+0003c570: 6c66 2e6c 616e 6775 6167 655f 6d61 7020  lf.language_map 
+0003c580: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
+0003c590: 7365 6c66 2e6c 7774 5f64 6174 6120 3d20  self.lwt_data = 
+0003c5a0: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
+0003c5b0: 6c66 2e71 7565 7279 5f63 6f75 6e74 203d  lf.query_count =
+0003c5c0: 2030 0d0a 2020 2020 2020 2020 7365 6c66   0..        self
+0003c5d0: 2e6f 7574 7075 745f 7a68 203d 204e 6f6e  .output_zh = Non
+0003c5e0: 6520 2023 2075 6e73 7570 706f 7274 6564  e  # unsupported
+0003c5f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
+0003c600: 6e70 7574 5f6c 696d 6974 203d 2069 6e74  nput_limit = int
+0003c610: 2835 6533 290d 0a20 2020 2020 2020 2073  (5e3)..        s
+0003c620: 656c 662e 6465 6661 756c 745f 6672 6f6d  elf.default_from
+0003c630: 5f6c 616e 6775 6167 6520 3d20 2766 7227  _language = 'fr'
+0003c640: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+0003c650: 6566 6175 6c74 5f65 6e5f 746f 5f6c 616e  efault_en_to_lan
+0003c660: 6775 6167 6520 3d20 2765 6e2d 5553 270d  guage = 'en-US'.
+0003c670: 0a0d 0a20 2020 2040 5473 652e 6465 6275  ...    @Tse.debu
+0003c680: 675f 6c61 6e67 7561 6765 5f6d 6170 0d0a  g_language_map..
+0003c690: 2020 2020 6465 6620 6765 745f 6c61 6e67      def get_lang
+0003c6a0: 7561 6765 5f6d 6170 2873 656c 662c 206c  uage_map(self, l
+0003c6b0: 616e 675f 7572 6c3a 2073 7472 2c20 7373  ang_url: str, ss
+0003c6c0: 3a20 5365 7373 696f 6e54 7970 652c 2068  : SessionType, h
+0003c6d0: 6561 6465 7273 3a20 6469 6374 2c20 7469  eaders: dict, ti
+0003c6e0: 6d65 6f75 743a 204f 7074 696f 6e61 6c5b  meout: Optional[
+0003c6f0: 666c 6f61 745d 2c20 7072 6f78 6965 733a  float], proxies:
+0003c700: 204f 7074 696f 6e61 6c5b 6469 6374 5d2c   Optional[dict],
+0003c710: 202a 2a6b 7761 7267 733a 204c 616e 674d   **kwargs: LangM
+0003c720: 6170 4b77 6172 6773 5479 7065 2920 2d3e  apKwargsType) ->
+0003c730: 2064 6963 743a 0d0a 2020 2020 2020 2020   dict:..        
+0003c740: 645f 6c61 6e67 5f6d 6170 203d 2073 732e  d_lang_map = ss.
+0003c750: 6765 7428 6c61 6e67 5f75 726c 2c20 6865  get(lang_url, he
+0003c760: 6164 6572 733d 6865 6164 6572 732c 2074  aders=headers, t
+0003c770: 696d 656f 7574 3d74 696d 656f 7574 2c20  imeout=timeout, 
+0003c780: 7072 6f78 6965 733d 7072 6f78 6965 7329  proxies=proxies)
+0003c790: 2e6a 736f 6e28 290d 0a20 2020 2020 2020  .json()..       
+0003c7a0: 2072 6574 7572 6e20 7b69 695b 2773 6f75   return {ii['sou
+0003c7b0: 7263 654c 616e 6775 6167 6527 5d5b 276d  rceLanguage']['m
+0003c7c0: 6d74 436f 6465 275d 3a20 5b6a 6a5b 2774  mtCode']: [jj['t
+0003c7d0: 6172 6765 744c 616e 6775 6167 6527 5d5b  argetLanguage'][
+0003c7e0: 276d 6d74 436f 6465 275d 2066 6f72 206a  'mmtCode'] for j
+0003c7f0: 6a20 696e 2064 5f6c 616e 675f 6d61 7020  j in d_lang_map 
+0003c800: 6966 206a 6a5b 2773 6f75 7263 654c 616e  if jj['sourceLan
+0003c810: 6775 6167 6527 5d5b 276d 6d74 436f 6465  guage']['mmtCode
+0003c820: 275d 203d 3d20 6969 5b27 736f 7572 6365  '] == ii['source
+0003c830: 4c61 6e67 7561 6765 275d 5b27 6d6d 7443  Language']['mmtC
+0003c840: 6f64 6527 5d5d 2066 6f72 2069 6920 696e  ode']] for ii in
+0003c850: 2064 5f6c 616e 675f 6d61 707d 0d0a 0d0a   d_lang_map}....
+0003c860: 2020 2020 2320 6465 6620 6765 745f 6c77      # def get_lw
+0003c870: 745f 6461 7461 2873 656c 662c 206c 7774  t_data(self, lwt
+0003c880: 5f6a 735f 7572 6c3a 2073 7472 2c20 7373  _js_url: str, ss
+0003c890: 3a20 5365 7373 696f 6e54 7970 652c 2068  : SessionType, h
+0003c8a0: 6561 6465 7273 3a20 6469 6374 2c20 7469  eaders: dict, ti
+0003c8b0: 6d65 6f75 743a 2066 6c6f 6174 2c20 7072  meout: float, pr
+0003c8c0: 6f78 6965 733a 2064 6963 7429 202d 3e20  oxies: dict) -> 
+0003c8d0: 6469 6374 3a0d 0a20 2020 2023 2020 2020  dict:..    #    
+0003c8e0: 206a 735f 6874 6d6c 203d 2073 732e 6765   js_html = ss.ge
+0003c8f0: 7428 6c77 745f 6a73 5f75 726c 2c20 6865  t(lwt_js_url, he
+0003c900: 6164 6572 733d 6865 6164 6572 732c 2074  aders=headers, t
+0003c910: 696d 656f 7574 3d74 696d 656f 7574 2c20  imeout=timeout, 
+0003c920: 7072 6f78 6965 733d 7072 6f78 6965 7329  proxies=proxies)
+0003c930: 2e74 6578 740d 0a20 2020 2023 2020 2020  .text..    #    
+0003c940: 206c 7774 5f64 6174 6120 3d20 7b0d 0a20   lwt_data = {.. 
+0003c950: 2020 2023 2020 2020 2020 2020 2027 782d     #         'x-
+0003c960: 6c77 742d 6170 706c 6963 6174 696f 6e2d  lwt-application-
+0003c970: 6964 273a 2072 652e 636f 6d70 696c 6528  id': re.compile(
+0003c980: 2722 582d 4c57 542d 4170 706c 6963 6174  '"X-LWT-Applicat
+0003c990: 696f 6e2d 4944 223a 2228 2e2a 3f29 2227  ion-ID":"(.*?)"'
+0003c9a0: 292e 7365 6172 6368 286a 735f 6874 6d6c  ).search(js_html
+0003c9b0: 292e 6772 6f75 7028 3129 2c0d 0a20 2020  ).group(1),..   
+0003c9c0: 2023 2020 2020 2020 2020 2027 782d 6c77   #         'x-lw
+0003c9d0: 742d 6275 696c 642d 6964 273a 2072 652e  t-build-id': re.
+0003c9e0: 636f 6d70 696c 6528 2722 582d 4c57 542d  compile('"X-LWT-
+0003c9f0: 4275 696c 642d 4944 223a 2228 2e2a 3f29  Build-ID":"(.*?)
+0003ca00: 2227 292e 7365 6172 6368 286a 735f 6874  "').search(js_ht
+0003ca10: 6d6c 292e 6772 6f75 7028 3129 2c0d 0a20  ml).group(1),.. 
+0003ca20: 2020 2023 2020 2020 207d 0d0a 2020 2020     #     }..    
+0003ca30: 2320 2020 2020 7265 7475 726e 206c 7774  #     return lwt
+0003ca40: 5f64 6174 610d 0a0d 0a20 2020 2064 6566  _data....    def
+0003ca50: 2067 6574 5f6c 7774 5f64 6174 6128 7365   get_lwt_data(se
+0003ca60: 6c66 2920 2d3e 2064 6963 743a 0d0a 2020  lf) -> dict:..  
+0003ca70: 2020 2020 2020 6c77 745f 6461 7461 203d        lwt_data =
+0003ca80: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+0003ca90: 2778 2d6c 7774 2d61 7070 6c69 6361 7469  'x-lwt-applicati
+0003caa0: 6f6e 2d69 6427 3a20 274c 5754 5f57 4542  on-id': 'LWT_WEB
+0003cab0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+0003cac0: 2778 2d6c 7774 2d62 7569 6c64 2d69 6427  'x-lwt-build-id'
+0003cad0: 3a20 2733 3436 3737 3527 2c0d 0a20 2020  : '346775',..   
+0003cae0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+0003caf0: 7265 7475 726e 206c 7774 5f64 6174 610d  return lwt_data.
+0003cb00: 0a0d 0a20 2020 2040 5473 652e 7469 6d65  ...    @Tse.time
+0003cb10: 5f73 7461 740d 0a20 2020 2040 5473 652e  _stat..    @Tse.
+0003cb20: 6368 6563 6b5f 7175 6572 790d 0a20 2020  check_query..   
+0003cb30: 2064 6566 206c 616e 6775 6167 6557 6972   def languageWir
+0003cb40: 655f 6170 6928 7365 6c66 2c20 7175 6572  e_api(self, quer
+0003cb50: 795f 7465 7874 3a20 7374 722c 2066 726f  y_text: str, fro
+0003cb60: 6d5f 6c61 6e67 7561 6765 3a20 7374 7220  m_language: str 
+0003cb70: 3d20 2761 7574 6f27 2c20 746f 5f6c 616e  = 'auto', to_lan
+0003cb80: 6775 6167 653a 2073 7472 203d 2027 656e  guage: str = 'en
+0003cb90: 272c 202a 2a6b 7761 7267 733a 2041 7069  ', **kwargs: Api
+0003cba0: 4b77 6172 6773 5479 7065 2920 2d3e 2055  KwargsType) -> U
+0003cbb0: 6e69 6f6e 5b73 7472 2c20 6469 6374 5d3a  nion[str, dict]:
+0003cbc0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0003cbd0: 2020 2020 2020 2068 7474 7073 3a2f 2f77         https://w
+0003cbe0: 7777 2e6c 616e 6775 6167 6577 6972 652e  ww.languagewire.
+0003cbf0: 636f 6d2f 656e 2f74 6563 686e 6f6c 6f67  com/en/technolog
+0003cc00: 792f 6c61 6e67 7561 6765 7769 7265 2d74  y/languagewire-t
+0003cc10: 7261 6e73 6c61 7465 0d0a 2020 2020 2020  ranslate..      
+0003cc20: 2020 3a70 6172 616d 2071 7565 7279 5f74    :param query_t
+0003cc30: 6578 743a 2073 7472 2c20 6d75 7374 2e0d  ext: str, must..
+0003cc40: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0003cc50: 6672 6f6d 5f6c 616e 6775 6167 653a 2073  from_language: s
+0003cc60: 7472 2c20 6465 6661 756c 7420 2761 7574  tr, default 'aut
+0003cc70: 6f27 2e0d 0a20 2020 2020 2020 203a 7061  o'...        :pa
+0003cc80: 7261 6d20 746f 5f6c 616e 6775 6167 653a  ram to_language:
+0003cc90: 2073 7472 2c20 6465 6661 756c 7420 2765   str, default 'e
+0003cca0: 6e27 2e0d 0a20 2020 2020 2020 203a 7061  n'...        :pa
+0003ccb0: 7261 6d20 2a2a 6b77 6172 6773 3a0d 0a20  ram **kwargs:.. 
+0003ccc0: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+0003ccd0: 7061 7261 6d20 7469 6d65 6f75 743a 2066  param timeout: f
+0003cce0: 6c6f 6174 2c20 6465 6661 756c 7420 4e6f  loat, default No
+0003ccf0: 6e65 2e0d 0a20 2020 2020 2020 2020 2020  ne...           
+0003cd00: 2020 2020 203a 7061 7261 6d20 7072 6f78       :param prox
+0003cd10: 6965 733a 2064 6963 742c 2064 6566 6175  ies: dict, defau
+0003cd20: 6c74 204e 6f6e 652e 0d0a 2020 2020 2020  lt None...      
+0003cd30: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+0003cd40: 2073 6c65 6570 5f73 6563 6f6e 6473 3a20   sleep_seconds: 
+0003cd50: 666c 6f61 742c 2064 6566 6175 6c74 2030  float, default 0
+0003cd60: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0003cd70: 2020 203a 7061 7261 6d20 6973 5f64 6574     :param is_det
+0003cd80: 6169 6c5f 7265 7375 6c74 3a20 626f 6f6c  ail_result: bool
+0003cd90: 2c20 6465 6661 756c 7420 4661 6c73 652e  , default False.
+0003cda0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0003cdb0: 2020 3a70 6172 616d 2069 665f 6967 6e6f    :param if_igno
+0003cdc0: 7265 5f6c 696d 6974 5f6f 665f 6c65 6e67  re_limit_of_leng
+0003cdd0: 7468 3a20 626f 6f6c 2c20 6465 6661 756c  th: bool, defaul
+0003cde0: 7420 4661 6c73 652e 0d0a 2020 2020 2020  t False...      
+0003cdf0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+0003ce00: 206c 696d 6974 5f6f 665f 6c65 6e67 7468   limit_of_length
+0003ce10: 3a20 696e 742c 2064 6566 6175 6c74 2032  : int, default 2
+0003ce20: 3030 3030 2e0d 0a20 2020 2020 2020 2020  0000...         
+0003ce30: 2020 2020 2020 203a 7061 7261 6d20 6966         :param if
+0003ce40: 5f69 676e 6f72 655f 656d 7074 795f 7175  _ignore_empty_qu
+0003ce50: 6572 793a 2062 6f6f 6c2c 2064 6566 6175  ery: bool, defau
+0003ce60: 6c74 2046 616c 7365 2e0d 0a20 2020 2020  lt False...     
+0003ce70: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+0003ce80: 6d20 7570 6461 7465 5f73 6573 7369 6f6e  m update_session
+0003ce90: 5f61 6674 6572 5f66 7265 713a 2069 6e74  _after_freq: int
+0003cea0: 2c20 6465 6661 756c 7420 3130 3030 2e0d  , default 1000..
+0003ceb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003cec0: 203a 7061 7261 6d20 7570 6461 7465 5f73   :param update_s
+0003ced0: 6573 7369 6f6e 5f61 6674 6572 5f73 6563  ession_after_sec
+0003cee0: 6f6e 6473 3a20 666c 6f61 742c 2064 6566  onds: float, def
+0003cef0: 6175 6c74 2031 3530 302e 0d0a 2020 2020  ault 1500...    
+0003cf00: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0003cf10: 616d 2069 665f 7368 6f77 5f74 696d 655f  am if_show_time_
+0003cf20: 7374 6174 3a20 626f 6f6c 2c20 6465 6661  stat: bool, defa
+0003cf30: 756c 7420 4661 6c73 652e 0d0a 2020 2020  ult False...    
+0003cf40: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0003cf50: 616d 2073 686f 775f 7469 6d65 5f73 7461  am show_time_sta
+0003cf60: 745f 7072 6563 6973 696f 6e3a 2069 6e74  t_precision: int
+0003cf70: 2c20 6465 6661 756c 7420 322e 0d0a 2020  , default 2...  
+0003cf80: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+0003cf90: 6172 616d 2069 665f 7072 696e 745f 7761  aram if_print_wa
+0003cfa0: 726e 696e 673a 2062 6f6f 6c2c 2064 6566  rning: bool, def
+0003cfb0: 6175 6c74 2054 7275 652e 0d0a 2020 2020  ault True...    
+0003cfc0: 2020 2020 3a72 6574 7572 6e3a 2073 7472      :return: str
+0003cfd0: 206f 7220 6469 6374 0d0a 2020 2020 2020   or dict..      
+0003cfe0: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
+0003cff0: 2074 696d 656f 7574 203d 206b 7761 7267   timeout = kwarg
+0003d000: 732e 6765 7428 2774 696d 656f 7574 272c  s.get('timeout',
+0003d010: 204e 6f6e 6529 0d0a 2020 2020 2020 2020   None)..        
+0003d020: 7072 6f78 6965 7320 3d20 6b77 6172 6773  proxies = kwargs
+0003d030: 2e67 6574 2827 7072 6f78 6965 7327 2c20  .get('proxies', 
+0003d040: 4e6f 6e65 290d 0a20 2020 2020 2020 2073  None)..        s
+0003d050: 6c65 6570 5f73 6563 6f6e 6473 203d 206b  leep_seconds = k
+0003d060: 7761 7267 732e 6765 7428 2773 6c65 6570  wargs.get('sleep
+0003d070: 5f73 6563 6f6e 6473 272c 2030 290d 0a20  _seconds', 0).. 
+0003d080: 2020 2020 2020 2069 665f 7072 696e 745f         if_print_
+0003d090: 7761 726e 696e 6720 3d20 6b77 6172 6773  warning = kwargs
+0003d0a0: 2e67 6574 2827 6966 5f70 7269 6e74 5f77  .get('if_print_w
+0003d0b0: 6172 6e69 6e67 272c 2054 7275 6529 0d0a  arning', True)..
+0003d0c0: 2020 2020 2020 2020 6973 5f64 6574 6169          is_detai
+0003d0d0: 6c5f 7265 7375 6c74 203d 206b 7761 7267  l_result = kwarg
+0003d0e0: 732e 6765 7428 2769 735f 6465 7461 696c  s.get('is_detail
+0003d0f0: 5f72 6573 756c 7427 2c20 4661 6c73 6529  _result', False)
+0003d100: 0d0a 2020 2020 2020 2020 7570 6461 7465  ..        update
+0003d110: 5f73 6573 7369 6f6e 5f61 6674 6572 5f66  _session_after_f
+0003d120: 7265 7120 3d20 6b77 6172 6773 2e67 6574  req = kwargs.get
+0003d130: 2827 7570 6461 7465 5f73 6573 7369 6f6e  ('update_session
+0003d140: 5f61 6674 6572 5f66 7265 7127 2c20 7365  _after_freq', se
+0003d150: 6c66 2e64 6566 6175 6c74 5f73 6573 7369  lf.default_sessi
+0003d160: 6f6e 5f66 7265 7129 0d0a 2020 2020 2020  on_freq)..      
+0003d170: 2020 7570 6461 7465 5f73 6573 7369 6f6e    update_session
+0003d180: 5f61 6674 6572 5f73 6563 6f6e 6473 203d  _after_seconds =
+0003d190: 206b 7761 7267 732e 6765 7428 2775 7064   kwargs.get('upd
+0003d1a0: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
+0003d1b0: 725f 7365 636f 6e64 7327 2c20 7365 6c66  r_seconds', self
+0003d1c0: 2e64 6566 6175 6c74 5f73 6573 7369 6f6e  .default_session
+0003d1d0: 5f73 6563 6f6e 6473 290d 0a20 2020 2020  _seconds)..     
+0003d1e0: 2020 2073 656c 662e 6368 6563 6b5f 696e     self.check_in
+0003d1f0: 7075 745f 6c69 6d69 7428 7175 6572 795f  put_limit(query_
+0003d200: 7465 7874 2c20 7365 6c66 2e69 6e70 7574  text, self.input
+0003d210: 5f6c 696d 6974 290d 0a0d 0a20 2020 2020  _limit)....     
+0003d220: 2020 206e 6f74 5f75 7064 6174 655f 636f     not_update_co
+0003d230: 6e64 5f66 7265 7120 3d20 3120 6966 2073  nd_freq = 1 if s
+0003d240: 656c 662e 7175 6572 795f 636f 756e 7420  elf.query_count 
+0003d250: 3c20 7570 6461 7465 5f73 6573 7369 6f6e  < update_session
+0003d260: 5f61 6674 6572 5f66 7265 7120 656c 7365  _after_freq else
+0003d270: 2030 0d0a 2020 2020 2020 2020 6e6f 745f   0..        not_
+0003d280: 7570 6461 7465 5f63 6f6e 645f 7469 6d65  update_cond_time
+0003d290: 203d 2031 2069 6620 7469 6d65 2e74 696d   = 1 if time.tim
+0003d2a0: 6528 2920 2d20 7365 6c66 2e62 6567 696e  e() - self.begin
+0003d2b0: 5f74 696d 6520 3c20 7570 6461 7465 5f73  _time < update_s
+0003d2c0: 6573 7369 6f6e 5f61 6674 6572 5f73 6563  ession_after_sec
+0003d2d0: 6f6e 6473 2065 6c73 6520 300d 0a20 2020  onds else 0..   
+0003d2e0: 2020 2020 2069 6620 6e6f 7420 2873 656c       if not (sel
+0003d2f0: 662e 7365 7373 696f 6e20 616e 6420 7365  f.session and se
+0003d300: 6c66 2e6c 616e 6775 6167 655f 6d61 7020  lf.language_map 
+0003d310: 616e 6420 6e6f 745f 7570 6461 7465 5f63  and not_update_c
+0003d320: 6f6e 645f 6672 6571 2061 6e64 206e 6f74  ond_freq and not
+0003d330: 5f75 7064 6174 655f 636f 6e64 5f74 696d  _update_cond_tim
+0003d340: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+0003d350: 2073 656c 662e 7365 7373 696f 6e20 3d20   self.session = 
+0003d360: 7265 7175 6573 7473 2e53 6573 7369 6f6e  requests.Session
+0003d370: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+0003d380: 5f20 3d20 7365 6c66 2e73 6573 7369 6f6e  _ = self.session
+0003d390: 2e67 6574 2873 656c 662e 686f 7374 5f75  .get(self.host_u
+0003d3a0: 726c 2c20 6865 6164 6572 733d 7365 6c66  rl, headers=self
+0003d3b0: 2e68 6f73 745f 6865 6164 6572 732c 2074  .host_headers, t
+0003d3c0: 696d 656f 7574 3d74 696d 656f 7574 2c20  imeout=timeout, 
+0003d3d0: 7072 6f78 6965 733d 7072 6f78 6965 7329  proxies=proxies)
+0003d3e0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0003d3f0: 6c66 2e6c 7774 5f64 6174 6120 3d20 7365  lf.lwt_data = se
+0003d400: 6c66 2e67 6574 5f6c 7774 5f64 6174 6128  lf.get_lwt_data(
+0003d410: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0003d420: 656c 662e 6170 695f 6865 6164 6572 732e  elf.api_headers.
+0003d430: 7570 6461 7465 2873 656c 662e 6c77 745f  update(self.lwt_
+0003d440: 6461 7461 290d 0a0d 0a20 2020 2020 2020  data)....       
+0003d450: 2020 2020 205f 203d 2073 656c 662e 7365       _ = self.se
+0003d460: 7373 696f 6e2e 706f 7374 2873 656c 662e  ssion.post(self.
+0003d470: 636f 6f6b 6965 5f75 726c 2c20 6865 6164  cookie_url, head
+0003d480: 6572 733d 7365 6c66 2e61 7069 5f68 6561  ers=self.api_hea
+0003d490: 6465 7273 2c20 7469 6d65 6f75 743d 7469  ders, timeout=ti
+0003d4a0: 6d65 6f75 742c 2070 726f 7869 6573 3d70  meout, proxies=p
+0003d4b0: 726f 7869 6573 290d 0a20 2020 2020 2020  roxies)..       
+0003d4c0: 2020 2020 2064 6562 7567 5f6c 616e 675f       debug_lang_
+0003d4d0: 6b77 6172 6773 203d 2073 656c 662e 6465  kwargs = self.de
+0003d4e0: 6275 675f 6c61 6e67 5f6b 7761 7267 7328  bug_lang_kwargs(
+0003d4f0: 6672 6f6d 5f6c 616e 6775 6167 652c 2074  from_language, t
+0003d500: 6f5f 6c61 6e67 7561 6765 2c20 7365 6c66  o_language, self
+0003d510: 2e64 6566 6175 6c74 5f66 726f 6d5f 6c61  .default_from_la
+0003d520: 6e67 7561 6765 2c20 6966 5f70 7269 6e74  nguage, if_print
+0003d530: 5f77 6172 6e69 6e67 290d 0a20 2020 2020  _warning)..     
+0003d540: 2020 2020 2020 2073 656c 662e 6c61 6e67         self.lang
+0003d550: 7561 6765 5f6d 6170 203d 2073 656c 662e  uage_map = self.
+0003d560: 6765 745f 6c61 6e67 7561 6765 5f6d 6170  get_language_map
+0003d570: 2873 656c 662e 6c61 6e67 5f75 726c 2c20  (self.lang_url, 
+0003d580: 7365 6c66 2e73 6573 7369 6f6e 2c20 7365  self.session, se
+0003d590: 6c66 2e61 7069 5f68 6561 6465 7273 2c20  lf.api_headers, 
+0003d5a0: 7469 6d65 6f75 742c 2070 726f 7869 6573  timeout, proxies
+0003d5b0: 2c20 2a2a 6465 6275 675f 6c61 6e67 5f6b  , **debug_lang_k
+0003d5c0: 7761 7267 7329 0d0a 0d0a 2020 2020 2020  wargs)....      
+0003d5d0: 2020 6966 2066 726f 6d5f 6c61 6e67 7561    if from_langua
+0003d5e0: 6765 203d 3d20 2761 7574 6f27 3a0d 0a20  ge == 'auto':.. 
+0003d5f0: 2020 2020 2020 2020 2020 2066 726f 6d5f             from_
+0003d600: 6c61 6e67 7561 6765 203d 2073 656c 662e  language = self.
+0003d610: 7761 726e 696e 675f 6175 746f 5f6c 616e  warning_auto_lan
+0003d620: 6728 276c 616e 6775 6167 6557 6972 6527  g('languageWire'
+0003d630: 2c20 7365 6c66 2e64 6566 6175 6c74 5f66  , self.default_f
+0003d640: 726f 6d5f 6c61 6e67 7561 6765 2c20 6966  rom_language, if
+0003d650: 5f70 7269 6e74 5f77 6172 6e69 6e67 290d  _print_warning).
+0003d660: 0a20 2020 2020 2020 2074 6f5f 6c61 6e67  .        to_lang
+0003d670: 7561 6765 203d 2073 656c 662e 6465 6661  uage = self.defa
+0003d680: 756c 745f 656e 5f74 6f5f 6c61 6e67 7561  ult_en_to_langua
+0003d690: 6765 2069 6620 746f 5f6c 616e 6775 6167  ge if to_languag
+0003d6a0: 6520 3d3d 2027 656e 2720 656c 7365 2074  e == 'en' else t
+0003d6b0: 6f5f 6c61 6e67 7561 6765 0d0a 2020 2020  o_language..    
+0003d6c0: 2020 2020 6672 6f6d 5f6c 616e 6775 6167      from_languag
+0003d6d0: 652c 2074 6f5f 6c61 6e67 7561 6765 203d  e, to_language =
+0003d6e0: 2073 656c 662e 6368 6563 6b5f 6c61 6e67   self.check_lang
+0003d6f0: 7561 6765 2866 726f 6d5f 6c61 6e67 7561  uage(from_langua
+0003d700: 6765 2c20 746f 5f6c 616e 6775 6167 652c  ge, to_language,
+0003d710: 2073 656c 662e 6c61 6e67 7561 6765 5f6d   self.language_m
+0003d720: 6170 2c20 6966 5f63 6865 636b 5f6c 616e  ap, if_check_lan
+0003d730: 675f 7265 7665 7273 653d 4661 6c73 6529  g_reverse=False)
+0003d740: 0d0a 0d0a 2020 2020 2020 2020 7061 796c  ....        payl
+0003d750: 6f61 6420 3d20 7b0d 0a20 2020 2020 2020  oad = {..       
+0003d760: 2020 2020 2027 736f 7572 6365 5465 7874       'sourceText
+0003d770: 273a 2071 7565 7279 5f74 6578 742c 0d0a  ': query_text,..
+0003d780: 2020 2020 2020 2020 2020 2020 2773 6f75              'sou
+0003d790: 7263 654c 616e 6775 6167 6527 3a20 6672  rceLanguage': fr
+0003d7a0: 6f6d 5f6c 616e 6775 6167 652c 0d0a 2020  om_language,..  
+0003d7b0: 2020 2020 2020 2020 2020 2774 6172 6765            'targe
+0003d7c0: 744c 616e 6775 6167 6527 3a20 746f 5f6c  tLanguage': to_l
+0003d7d0: 616e 6775 6167 652c 0d0a 2020 2020 2020  anguage,..      
+0003d7e0: 2020 7d0d 0a20 2020 2020 2020 2072 203d    }..        r =
+0003d7f0: 2073 656c 662e 7365 7373 696f 6e2e 706f   self.session.po
+0003d800: 7374 2873 656c 662e 6170 695f 7572 6c2c  st(self.api_url,
+0003d810: 206a 736f 6e3d 7061 796c 6f61 642c 2068   json=payload, h
+0003d820: 6561 6465 7273 3d73 656c 662e 6170 695f  eaders=self.api_
+0003d830: 6865 6164 6572 732c 2074 696d 656f 7574  headers, timeout
+0003d840: 3d74 696d 656f 7574 2c20 7072 6f78 6965  =timeout, proxie
+0003d850: 733d 7072 6f78 6965 7329 0d0a 2020 2020  s=proxies)..    
+0003d860: 2020 2020 722e 7261 6973 655f 666f 725f      r.raise_for_
+0003d870: 7374 6174 7573 2829 0d0a 2020 2020 2020  status()..      
+0003d880: 2020 6461 7461 203d 2072 2e6a 736f 6e28    data = r.json(
+0003d890: 290d 0a20 2020 2020 2020 2074 696d 652e  )..        time.
+0003d8a0: 736c 6565 7028 736c 6565 705f 7365 636f  sleep(sleep_seco
+0003d8b0: 6e64 7329 0d0a 2020 2020 2020 2020 7365  nds)..        se
+0003d8c0: 6c66 2e71 7565 7279 5f63 6f75 6e74 202b  lf.query_count +
+0003d8d0: 3d20 310d 0a20 2020 2020 2020 2072 6574  = 1..        ret
+0003d8e0: 7572 6e20 6461 7461 2069 6620 6973 5f64  urn data if is_d
+0003d8f0: 6574 6169 6c5f 7265 7375 6c74 2065 6c73  etail_result els
+0003d900: 6520 6461 7461 5b27 7472 616e 736c 6174  e data['translat
+0003d910: 696f 6e27 5d0d 0a0d 0a0d 0a63 6c61 7373  ion']......class
+0003d920: 204a 7564 6963 2854 7365 293a 0d0a 2020   Judic(Tse):..  
+0003d930: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0003d940: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
+0003d950: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+0003d960: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0003d970: 686f 6d65 5f75 726c 203d 2027 6874 7470  home_url = 'http
+0003d980: 733a 2f2f 6a75 6469 632e 696f 270d 0a20  s://judic.io'.. 
+0003d990: 2020 2020 2020 2073 656c 662e 686f 7374         self.host
+0003d9a0: 5f75 726c 203d 2027 6874 7470 733a 2f2f  _url = 'https://
+0003d9b0: 6a75 6469 632e 696f 2f65 6e2f 7472 616e  judic.io/en/tran
+0003d9c0: 736c 6174 6527 0d0a 2020 2020 2020 2020  slate'..        
+0003d9d0: 7365 6c66 2e61 7069 5f75 726c 203d 2027  self.api_url = '
+0003d9e0: 6874 7470 733a 2f2f 6a75 6469 632e 696f  https://judic.io
+0003d9f0: 2f74 7261 6e73 6c61 7465 2f74 6578 7427  /translate/text'
+0003da00: 0d0a 2020 2020 2020 2020 7365 6c66 2e68  ..        self.h
+0003da10: 6f73 745f 6865 6164 6572 7320 3d20 7365  ost_headers = se
+0003da20: 6c66 2e67 6574 5f68 6561 6465 7273 2873  lf.get_headers(s
+0003da30: 656c 662e 686f 6d65 5f75 726c 2c20 6966  elf.home_url, if
+0003da40: 5f61 7069 3d46 616c 7365 2c20 6966 5f72  _api=False, if_r
+0003da50: 6566 6572 6572 5f66 6f72 5f68 6f73 743d  eferer_for_host=
+0003da60: 5472 7565 290d 0a20 2020 2020 2020 2073  True)..        s
+0003da70: 656c 662e 6170 695f 6865 6164 6572 7320  elf.api_headers 
+0003da80: 3d20 7365 6c66 2e67 6574 5f68 6561 6465  = self.get_heade
+0003da90: 7273 2873 656c 662e 686f 6d65 5f75 726c  rs(self.home_url
+0003daa0: 2c20 6966 5f61 7069 3d54 7275 652c 2069  , if_api=True, i
+0003dab0: 665f 6a73 6f6e 5f66 6f72 5f61 7069 3d54  f_json_for_api=T
+0003dac0: 7275 6529 0d0a 2020 2020 2020 2020 7365  rue)..        se
+0003dad0: 6c66 2e73 6573 7369 6f6e 203d 204e 6f6e  lf.session = Non
+0003dae0: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+0003daf0: 6c61 6e67 5f6c 6973 7420 3d20 5b27 656e  lang_list = ['en
+0003db00: 272c 2027 6465 272c 2027 6672 272c 2027  ', 'de', 'fr', '
+0003db10: 6e6c 275d 0d0a 2020 2020 2020 2020 7365  nl']..        se
+0003db20: 6c66 2e6c 616e 6775 6167 655f 6d61 7020  lf.language_map 
+0003db30: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
+0003db40: 7365 6c66 2e71 7565 7279 5f63 6f75 6e74  self.query_count
+0003db50: 203d 2030 0d0a 2020 2020 2020 2020 7365   = 0..        se
+0003db60: 6c66 2e6f 7574 7075 745f 7a68 203d 204e  lf.output_zh = N
+0003db70: 6f6e 6520 2023 2075 6e73 7570 706f 7274  one  # unsupport
+0003db80: 6564 0d0a 2020 2020 2020 2020 7365 6c66  ed..        self
+0003db90: 2e69 6e70 7574 5f6c 696d 6974 203d 2069  .input_limit = i
+0003dba0: 6e74 2831 6533 290d 0a20 2020 2020 2020  nt(1e3)..       
+0003dbb0: 2073 656c 662e 6465 6661 756c 745f 6672   self.default_fr
+0003dbc0: 6f6d 5f6c 616e 6775 6167 6520 3d20 276e  om_language = 'n
+0003dbd0: 6c27 0d0a 0d0a 2020 2020 4054 7365 2e64  l'....    @Tse.d
+0003dbe0: 6562 7567 5f6c 616e 6775 6167 655f 6d61  ebug_language_ma
+0003dbf0: 700d 0a20 2020 2064 6566 2067 6574 5f6c  p..    def get_l
+0003dc00: 616e 6775 6167 655f 6d61 7028 7365 6c66  anguage_map(self
+0003dc10: 2c20 6c61 6e67 5f6c 6973 743a 204c 6973  , lang_list: Lis
+0003dc20: 745b 7374 725d 2c20 2a2a 6b77 6172 6773  t[str], **kwargs
+0003dc30: 3a20 4c61 6e67 4d61 704b 7761 7267 7354  : LangMapKwargsT
+0003dc40: 7970 6529 202d 3e20 6469 6374 3a0d 0a20  ype) -> dict:.. 
+0003dc50: 2020 2020 2020 2072 6574 7572 6e20 7b7d         return {}
+0003dc60: 2e66 726f 6d6b 6579 7328 6c61 6e67 5f6c  .fromkeys(lang_l
+0003dc70: 6973 742c 206c 616e 675f 6c69 7374 290d  ist, lang_list).
+0003dc80: 0a0d 0a20 2020 2040 5473 652e 7469 6d65  ...    @Tse.time
+0003dc90: 5f73 7461 740d 0a20 2020 2040 5473 652e  _stat..    @Tse.
+0003dca0: 6368 6563 6b5f 7175 6572 790d 0a20 2020  check_query..   
+0003dcb0: 2064 6566 206a 7564 6963 5f61 7069 2873   def judic_api(s
+0003dcc0: 656c 662c 2071 7565 7279 5f74 6578 743a  elf, query_text:
+0003dcd0: 2073 7472 2c20 6672 6f6d 5f6c 616e 6775   str, from_langu
+0003dce0: 6167 653a 2073 7472 203d 2027 6175 746f  age: str = 'auto
+0003dcf0: 272c 2074 6f5f 6c61 6e67 7561 6765 3a20  ', to_language: 
+0003dd00: 7374 7220 3d20 2765 6e27 2c20 2a2a 6b77  str = 'en', **kw
+0003dd10: 6172 6773 3a20 4170 694b 7761 7267 7354  args: ApiKwargsT
+0003dd20: 7970 6529 202d 3e20 556e 696f 6e5b 7374  ype) -> Union[st
+0003dd30: 722c 2064 6963 745d 3a0d 0a20 2020 2020  r, dict]:..     
+0003dd40: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+0003dd50: 6874 7470 733a 2f2f 6a75 6469 632e 696f  https://judic.io
+0003dd60: 2f65 6e2f 7472 616e 736c 6174 650d 0a20  /en/translate.. 
+0003dd70: 2020 2020 2020 203a 7061 7261 6d20 7175         :param qu
+0003dd80: 6572 795f 7465 7874 3a20 7374 722c 206d  ery_text: str, m
+0003dd90: 7573 742e 0d0a 2020 2020 2020 2020 3a70  ust...        :p
+0003dda0: 6172 616d 2066 726f 6d5f 6c61 6e67 7561  aram from_langua
+0003ddb0: 6765 3a20 7374 722c 2064 6566 6175 6c74  ge: str, default
+0003ddc0: 2027 6175 746f 272e 0d0a 2020 2020 2020   'auto'...      
+0003ddd0: 2020 3a70 6172 616d 2074 6f5f 6c61 6e67    :param to_lang
+0003dde0: 7561 6765 3a20 7374 722c 2064 6566 6175  uage: str, defau
+0003ddf0: 6c74 2027 656e 272e 0d0a 2020 2020 2020  lt 'en'...      
+0003de00: 2020 3a70 6172 616d 202a 2a6b 7761 7267    :param **kwarg
+0003de10: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+0003de20: 2020 2020 3a70 6172 616d 2074 696d 656f      :param timeo
+0003de30: 7574 3a20 666c 6f61 742c 2064 6566 6175  ut: float, defau
+0003de40: 6c74 204e 6f6e 652e 0d0a 2020 2020 2020  lt None...      
+0003de50: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+0003de60: 2070 726f 7869 6573 3a20 6469 6374 2c20   proxies: dict, 
+0003de70: 6465 6661 756c 7420 4e6f 6e65 2e0d 0a20  default None... 
+0003de80: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+0003de90: 7061 7261 6d20 736c 6565 705f 7365 636f  param sleep_seco
+0003dea0: 6e64 733a 2066 6c6f 6174 2c20 6465 6661  nds: float, defa
+0003deb0: 756c 7420 302e 0d0a 2020 2020 2020 2020  ult 0...        
+0003dec0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+0003ded0: 735f 6465 7461 696c 5f72 6573 756c 743a  s_detail_result:
+0003dee0: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
+0003def0: 616c 7365 2e0d 0a20 2020 2020 2020 2020  alse...         
+0003df00: 2020 2020 2020 203a 7061 7261 6d20 6966         :param if
+0003df10: 5f69 676e 6f72 655f 6c69 6d69 745f 6f66  _ignore_limit_of
+0003df20: 5f6c 656e 6774 683a 2062 6f6f 6c2c 2064  _length: bool, d
+0003df30: 6566 6175 6c74 2046 616c 7365 2e0d 0a20  efault False... 
+0003df40: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+0003df50: 7061 7261 6d20 6c69 6d69 745f 6f66 5f6c  param limit_of_l
+0003df60: 656e 6774 683a 2069 6e74 2c20 6465 6661  ength: int, defa
+0003df70: 756c 7420 3230 3030 302e 0d0a 2020 2020  ult 20000...    
+0003df80: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0003df90: 616d 2069 665f 6967 6e6f 7265 5f65 6d70  am if_ignore_emp
+0003dfa0: 7479 5f71 7565 7279 3a20 626f 6f6c 2c20  ty_query: bool, 
+0003dfb0: 6465 6661 756c 7420 4661 6c73 652e 0d0a  default False...
+0003dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003dfd0: 3a70 6172 616d 2075 7064 6174 655f 7365  :param update_se
+0003dfe0: 7373 696f 6e5f 6166 7465 725f 6672 6571  ssion_after_freq
+0003dff0: 3a20 696e 742c 2064 6566 6175 6c74 2031  : int, default 1
+0003e000: 3030 302e 0d0a 2020 2020 2020 2020 2020  000...          
+0003e010: 2020 2020 2020 3a70 6172 616d 2075 7064        :param upd
+0003e020: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
+0003e030: 725f 7365 636f 6e64 733a 2066 6c6f 6174  r_seconds: float
+0003e040: 2c20 6465 6661 756c 7420 3135 3030 2e0d  , default 1500..
+0003e050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003e060: 203a 7061 7261 6d20 6966 5f73 686f 775f   :param if_show_
+0003e070: 7469 6d65 5f73 7461 743a 2062 6f6f 6c2c  time_stat: bool,
+0003e080: 2064 6566 6175 6c74 2046 616c 7365 2e0d   default False..
+0003e090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003e0a0: 203a 7061 7261 6d20 7368 6f77 5f74 696d   :param show_tim
+0003e0b0: 655f 7374 6174 5f70 7265 6369 7369 6f6e  e_stat_precision
+0003e0c0: 3a20 696e 742c 2064 6566 6175 6c74 2032  : int, default 2
+0003e0d0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0003e0e0: 2020 203a 7061 7261 6d20 6966 5f70 7269     :param if_pri
+0003e0f0: 6e74 5f77 6172 6e69 6e67 3a20 626f 6f6c  nt_warning: bool
+0003e100: 2c20 6465 6661 756c 7420 5472 7565 2e0d  , default True..
+0003e110: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0003e120: 3a20 7374 7220 6f72 2064 6963 740d 0a20  : str or dict.. 
+0003e130: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
+0003e140: 2020 2020 2020 7469 6d65 6f75 7420 3d20        timeout = 
+0003e150: 6b77 6172 6773 2e67 6574 2827 7469 6d65  kwargs.get('time
+0003e160: 6f75 7427 2c20 4e6f 6e65 290d 0a20 2020  out', None)..   
+0003e170: 2020 2020 2070 726f 7869 6573 203d 206b       proxies = k
+0003e180: 7761 7267 732e 6765 7428 2770 726f 7869  wargs.get('proxi
+0003e190: 6573 272c 204e 6f6e 6529 0d0a 2020 2020  es', None)..    
+0003e1a0: 2020 2020 736c 6565 705f 7365 636f 6e64      sleep_second
+0003e1b0: 7320 3d20 6b77 6172 6773 2e67 6574 2827  s = kwargs.get('
+0003e1c0: 736c 6565 705f 7365 636f 6e64 7327 2c20  sleep_seconds', 
+0003e1d0: 3029 0d0a 2020 2020 2020 2020 6966 5f70  0)..        if_p
+0003e1e0: 7269 6e74 5f77 6172 6e69 6e67 203d 206b  rint_warning = k
+0003e1f0: 7761 7267 732e 6765 7428 2769 665f 7072  wargs.get('if_pr
+0003e200: 696e 745f 7761 726e 696e 6727 2c20 5472  int_warning', Tr
+0003e210: 7565 290d 0a20 2020 2020 2020 2069 735f  ue)..        is_
+0003e220: 6465 7461 696c 5f72 6573 756c 7420 3d20  detail_result = 
+0003e230: 6b77 6172 6773 2e67 6574 2827 6973 5f64  kwargs.get('is_d
+0003e240: 6574 6169 6c5f 7265 7375 6c74 272c 2046  etail_result', F
+0003e250: 616c 7365 290d 0a20 2020 2020 2020 2075  alse)..        u
+0003e260: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
+0003e270: 7465 725f 6672 6571 203d 206b 7761 7267  ter_freq = kwarg
+0003e280: 732e 6765 7428 2775 7064 6174 655f 7365  s.get('update_se
+0003e290: 7373 696f 6e5f 6166 7465 725f 6672 6571  ssion_after_freq
+0003e2a0: 272c 2073 656c 662e 6465 6661 756c 745f  ', self.default_
+0003e2b0: 7365 7373 696f 6e5f 6672 6571 290d 0a20  session_freq).. 
+0003e2c0: 2020 2020 2020 2075 7064 6174 655f 7365         update_se
+0003e2d0: 7373 696f 6e5f 6166 7465 725f 7365 636f  ssion_after_seco
+0003e2e0: 6e64 7320 3d20 6b77 6172 6773 2e67 6574  nds = kwargs.get
+0003e2f0: 2827 7570 6461 7465 5f73 6573 7369 6f6e  ('update_session
+0003e300: 5f61 6674 6572 5f73 6563 6f6e 6473 272c  _after_seconds',
+0003e310: 2073 656c 662e 6465 6661 756c 745f 7365   self.default_se
+0003e320: 7373 696f 6e5f 7365 636f 6e64 7329 0d0a  ssion_seconds)..
+0003e330: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
+0003e340: 636b 5f69 6e70 7574 5f6c 696d 6974 2871  ck_input_limit(q
+0003e350: 7565 7279 5f74 6578 742c 2073 656c 662e  uery_text, self.
+0003e360: 696e 7075 745f 6c69 6d69 7429 0d0a 0d0a  input_limit)....
+0003e370: 2020 2020 2020 2020 6e6f 745f 7570 6461          not_upda
+0003e380: 7465 5f63 6f6e 645f 6672 6571 203d 2031  te_cond_freq = 1
+0003e390: 2069 6620 7365 6c66 2e71 7565 7279 5f63   if self.query_c
+0003e3a0: 6f75 6e74 203c 2075 7064 6174 655f 7365  ount < update_se
+0003e3b0: 7373 696f 6e5f 6166 7465 725f 6672 6571  ssion_after_freq
+0003e3c0: 2065 6c73 6520 300d 0a20 2020 2020 2020   else 0..       
+0003e3d0: 206e 6f74 5f75 7064 6174 655f 636f 6e64   not_update_cond
+0003e3e0: 5f74 696d 6520 3d20 3120 6966 2074 696d  _time = 1 if tim
+0003e3f0: 652e 7469 6d65 2829 202d 2073 656c 662e  e.time() - self.
+0003e400: 6265 6769 6e5f 7469 6d65 203c 2075 7064  begin_time < upd
+0003e410: 6174 655f 7365 7373 696f 6e5f 6166 7465  ate_session_afte
+0003e420: 725f 7365 636f 6e64 7320 656c 7365 2030  r_seconds else 0
+0003e430: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+0003e440: 2028 7365 6c66 2e73 6573 7369 6f6e 2061   (self.session a
+0003e450: 6e64 2073 656c 662e 6c61 6e67 7561 6765  nd self.language
+0003e460: 5f6d 6170 2061 6e64 206e 6f74 5f75 7064  _map and not_upd
+0003e470: 6174 655f 636f 6e64 5f66 7265 7120 616e  ate_cond_freq an
+0003e480: 6420 6e6f 745f 7570 6461 7465 5f63 6f6e  d not_update_con
+0003e490: 645f 7469 6d65 293a 0d0a 2020 2020 2020  d_time):..      
+0003e4a0: 2020 2020 2020 7365 6c66 2e73 6573 7369        self.sessi
+0003e4b0: 6f6e 203d 2072 6571 7565 7374 732e 5365  on = requests.Se
+0003e4c0: 7373 696f 6e28 290d 0a20 2020 2020 2020  ssion()..       
+0003e4d0: 2020 2020 205f 203d 2073 656c 662e 7365       _ = self.se
+0003e4e0: 7373 696f 6e2e 6765 7428 7365 6c66 2e68  ssion.get(self.h
+0003e4f0: 6f73 745f 7572 6c2c 2068 6561 6465 7273  ost_url, headers
+0003e500: 3d73 656c 662e 686f 7374 5f68 6561 6465  =self.host_heade
+0003e510: 7273 2c20 7469 6d65 6f75 743d 7469 6d65  rs, timeout=time
+0003e520: 6f75 742c 2070 726f 7869 6573 3d70 726f  out, proxies=pro
+0003e530: 7869 6573 290d 0a20 2020 2020 2020 2020  xies)..         
+0003e540: 2020 2064 6562 7567 5f6c 616e 675f 6b77     debug_lang_kw
+0003e550: 6172 6773 203d 2073 656c 662e 6465 6275  args = self.debu
+0003e560: 675f 6c61 6e67 5f6b 7761 7267 7328 6672  g_lang_kwargs(fr
+0003e570: 6f6d 5f6c 616e 6775 6167 652c 2074 6f5f  om_language, to_
+0003e580: 6c61 6e67 7561 6765 2c20 7365 6c66 2e64  language, self.d
+0003e590: 6566 6175 6c74 5f66 726f 6d5f 6c61 6e67  efault_from_lang
+0003e5a0: 7561 6765 2c20 6966 5f70 7269 6e74 5f77  uage, if_print_w
+0003e5b0: 6172 6e69 6e67 290d 0a20 2020 2020 2020  arning)..       
+0003e5c0: 2020 2020 2073 656c 662e 6c61 6e67 7561       self.langua
+0003e5d0: 6765 5f6d 6170 203d 2073 656c 662e 6765  ge_map = self.ge
+0003e5e0: 745f 6c61 6e67 7561 6765 5f6d 6170 2873  t_language_map(s
+0003e5f0: 656c 662e 6c61 6e67 5f6c 6973 742c 202a  elf.lang_list, *
+0003e600: 2a64 6562 7567 5f6c 616e 675f 6b77 6172  *debug_lang_kwar
+0003e610: 6773 290d 0a0d 0a20 2020 2020 2020 2069  gs)....        i
+0003e620: 6620 6672 6f6d 5f6c 616e 6775 6167 6520  f from_language 
+0003e630: 3d3d 2027 6175 746f 273a 0d0a 2020 2020  == 'auto':..    
+0003e640: 2020 2020 2020 2020 6672 6f6d 5f6c 616e          from_lan
+0003e650: 6775 6167 6520 3d20 7365 6c66 2e77 6172  guage = self.war
+0003e660: 6e69 6e67 5f61 7574 6f5f 6c61 6e67 2827  ning_auto_lang('
+0003e670: 6a75 6469 6327 2c20 7365 6c66 2e64 6566  judic', self.def
+0003e680: 6175 6c74 5f66 726f 6d5f 6c61 6e67 7561  ault_from_langua
+0003e690: 6765 2c20 6966 5f70 7269 6e74 5f77 6172  ge, if_print_war
+0003e6a0: 6e69 6e67 290d 0a20 2020 2020 2020 2066  ning)..        f
+0003e6b0: 726f 6d5f 6c61 6e67 7561 6765 2c20 746f  rom_language, to
+0003e6c0: 5f6c 616e 6775 6167 6520 3d20 7365 6c66  _language = self
+0003e6d0: 2e63 6865 636b 5f6c 616e 6775 6167 6528  .check_language(
+0003e6e0: 6672 6f6d 5f6c 616e 6775 6167 652c 2074  from_language, t
+0003e6f0: 6f5f 6c61 6e67 7561 6765 2c20 7365 6c66  o_language, self
+0003e700: 2e6c 616e 6775 6167 655f 6d61 7029 0d0a  .language_map)..
+0003e710: 0d0a 2020 2020 2020 2020 7061 796c 6f61  ..        payloa
+0003e720: 6420 3d20 7b0d 0a20 2020 2020 2020 2020  d = {..         
+0003e730: 2020 2027 736f 7572 6365 5465 7874 273a     'sourceText':
+0003e740: 2071 7565 7279 5f74 6578 742c 0d0a 2020   query_text,..  
+0003e750: 2020 2020 2020 2020 2020 2769 6e70 7574            'input
+0003e760: 4c61 6e67 273a 2066 726f 6d5f 6c61 6e67  Lang': from_lang
+0003e770: 7561 6765 2c0d 0a20 2020 2020 2020 2020  uage,..         
+0003e780: 2020 2027 6f75 7470 7574 4c61 6e67 273a     'outputLang':
+0003e790: 2074 6f5f 6c61 6e67 7561 6765 0d0a 2020   to_language..  
+0003e7a0: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+0003e7b0: 2072 203d 2073 656c 662e 7365 7373 696f   r = self.sessio
+0003e7c0: 6e2e 706f 7374 2873 656c 662e 6170 695f  n.post(self.api_
+0003e7d0: 7572 6c2c 206a 736f 6e3d 7061 796c 6f61  url, json=payloa
+0003e7e0: 642c 2068 6561 6465 7273 3d73 656c 662e  d, headers=self.
+0003e7f0: 6170 695f 6865 6164 6572 732c 2074 696d  api_headers, tim
+0003e800: 656f 7574 3d74 696d 656f 7574 2c20 7072  eout=timeout, pr
+0003e810: 6f78 6965 733d 7072 6f78 6965 7329 0d0a  oxies=proxies)..
+0003e820: 2020 2020 2020 2020 722e 7261 6973 655f          r.raise_
+0003e830: 666f 725f 7374 6174 7573 2829 0d0a 2020  for_status()..  
+0003e840: 2020 2020 2020 6461 7461 203d 2072 2e6a        data = r.j
+0003e850: 736f 6e28 290d 0a20 2020 2020 2020 2074  son()..        t
+0003e860: 696d 652e 736c 6565 7028 736c 6565 705f  ime.sleep(sleep_
+0003e870: 7365 636f 6e64 7329 0d0a 2020 2020 2020  seconds)..      
+0003e880: 2020 7365 6c66 2e71 7565 7279 5f63 6f75    self.query_cou
+0003e890: 6e74 202b 3d20 310d 0a20 2020 2020 2020  nt += 1..       
+0003e8a0: 2072 6574 7572 6e20 6461 7461 2069 6620   return data if 
+0003e8b0: 6973 5f64 6574 6169 6c5f 7265 7375 6c74  is_detail_result
+0003e8c0: 2065 6c73 6520 6461 7461 5b27 7472 616e   else data['tran
+0003e8d0: 736c 6174 696f 6e27 5d0d 0a0d 0a0d 0a63  slation']......c
+0003e8e0: 6c61 7373 2059 6565 6b69 7428 5473 6529  lass Yeekit(Tse)
+0003e8f0: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
+0003e900: 745f 5f28 7365 6c66 293a 0d0a 2020 2020  t__(self):..    
+0003e910: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+0003e920: 6974 5f5f 2829 0d0a 2020 2020 2020 2020  it__()..        
+0003e930: 7365 6c66 2e68 6f6d 655f 7572 6c20 3d20  self.home_url = 
+0003e940: 2768 7474 7073 3a2f 2f77 7777 2e79 6565  'https://www.yee
+0003e950: 6b69 742e 636f 6d27 0d0a 2020 2020 2020  kit.com'..      
+0003e960: 2020 7365 6c66 2e68 6f73 745f 7572 6c20    self.host_url 
+0003e970: 3d20 2768 7474 7073 3a2f 2f77 7777 2e79  = 'https://www.y
+0003e980: 6565 6b69 742e 636f 6d2f 7369 7465 2f74  eekit.com/site/t
+0003e990: 7261 6e73 6c61 7465 270d 0a20 2020 2020  ranslate'..     
+0003e9a0: 2020 2073 656c 662e 6170 695f 7572 6c20     self.api_url 
+0003e9b0: 3d20 2768 7474 7073 3a2f 2f77 7777 2e79  = 'https://www.y
+0003e9c0: 6565 6b69 742e 636f 6d2f 7369 7465 2f64  eekit.com/site/d
+0003e9d0: 6f74 7261 6e73 6c61 7465 270d 0a20 2020  otranslate'..   
+0003e9e0: 2020 2020 2073 656c 662e 6c61 6e67 5f75       self.lang_u
+0003e9f0: 726c 203d 2027 6874 7470 733a 2f2f 7777  rl = 'https://ww
+0003ea00: 772e 7965 656b 6974 2e63 6f6d 2f6a 732f  w.yeekit.com/js/
+0003ea10: 7472 616e 736c 6174 652e 6a73 270d 0a20  translate.js'.. 
+0003ea20: 2020 2020 2020 2073 656c 662e 686f 7374         self.host
+0003ea30: 5f68 6561 6465 7273 203d 2073 656c 662e  _headers = self.
+0003ea40: 6765 745f 6865 6164 6572 7328 7365 6c66  get_headers(self
+0003ea50: 2e68 6f6d 655f 7572 6c2c 2069 665f 6170  .home_url, if_ap
+0003ea60: 693d 4661 6c73 652c 2069 665f 7265 6665  i=False, if_refe
+0003ea70: 7265 725f 666f 725f 686f 7374 3d54 7275  rer_for_host=Tru
+0003ea80: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
+0003ea90: 2e61 7069 5f68 6561 6465 7273 203d 2073  .api_headers = s
+0003eaa0: 656c 662e 6765 745f 6865 6164 6572 7328  elf.get_headers(
+0003eab0: 7365 6c66 2e68 6f6d 655f 7572 6c2c 2069  self.home_url, i
+0003eac0: 665f 6170 693d 5472 7565 2c20 6966 5f61  f_api=True, if_a
+0003ead0: 6a61 785f 666f 725f 6170 693d 5472 7565  jax_for_api=True
+0003eae0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0003eaf0: 7365 7373 696f 6e20 3d20 4e6f 6e65 0d0a  session = None..
+0003eb00: 2020 2020 2020 2020 7365 6c66 2e6c 616e          self.lan
+0003eb10: 675f 6c69 7374 203d 205b 277a 6827 2c20  g_list = ['zh', 
+0003eb20: 2765 6e27 2c20 2761 7227 2c20 2764 6527  'en', 'ar', 'de'
+0003eb30: 2c20 2772 7527 2c20 2766 7227 2c20 2763  , 'ru', 'fr', 'c
+0003eb40: 7a27 2c20 2770 7427 2c20 276a 7027 2c20  z', 'pt', 'jp', 
+0003eb50: 2765 7327 5d0d 0a20 2020 2020 2020 2073  'es']..        s
+0003eb60: 656c 662e 6c61 6e67 7561 6765 5f6d 6170  elf.language_map
+0003eb70: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
+0003eb80: 2073 656c 662e 7175 6572 795f 636f 756e   self.query_coun
+0003eb90: 7420 3d20 300d 0a20 2020 2020 2020 2073  t = 0..        s
+0003eba0: 656c 662e 6f75 7470 7574 5f7a 6820 3d20  elf.output_zh = 
+0003ebb0: 277a 6827 0d0a 2020 2020 2020 2020 7365  'zh'..        se
+0003ebc0: 6c66 2e69 6e70 7574 5f6c 696d 6974 203d  lf.input_limit =
+0003ebd0: 2069 6e74 2831 6533 290d 0a20 2020 2020   int(1e3)..     
+0003ebe0: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
+0003ebf0: 6672 6f6d 5f6c 616e 6775 6167 6520 3d20  from_language = 
+0003ec00: 7365 6c66 2e6f 7574 7075 745f 7a68 0d0a  self.output_zh..
+0003ec10: 0d0a 2020 2020 4054 7365 2e64 6562 7567  ..    @Tse.debug
+0003ec20: 5f6c 616e 6775 6167 655f 6d61 700d 0a20  _language_map.. 
+0003ec30: 2020 2064 6566 2067 6574 5f6c 616e 6775     def get_langu
+0003ec40: 6167 655f 6d61 7028 7365 6c66 2c20 6c61  age_map(self, la
+0003ec50: 6e67 5f6c 6973 743a 204c 6973 745b 7374  ng_list: List[st
+0003ec60: 725d 2c20 2a2a 6b77 6172 6773 3a20 4c61  r], **kwargs: La
+0003ec70: 6e67 4d61 704b 7761 7267 7354 7970 6529  ngMapKwargsType)
+0003ec80: 202d 3e20 6469 6374 3a0d 0a20 2020 2020   -> dict:..     
+0003ec90: 2020 2072 6574 7572 6e20 7b7d 2e66 726f     return {}.fro
+0003eca0: 6d6b 6579 7328 6c61 6e67 5f6c 6973 742c  mkeys(lang_list,
+0003ecb0: 206c 616e 675f 6c69 7374 290d 0a0d 0a20   lang_list).... 
+0003ecc0: 2020 2040 5473 652e 756e 6365 7274 6966     @Tse.uncertif
+0003ecd0: 6965 6420 2023 206e 6f74 2063 6f64 652c  ied  # not code,
+0003ece0: 2062 7574 2073 6572 7665 722e 0d0a 2020   but server...  
+0003ecf0: 2020 4054 7365 2e74 696d 655f 7374 6174    @Tse.time_stat
+0003ed00: 0d0a 2020 2020 4054 7365 2e63 6865 636b  ..    @Tse.check
+0003ed10: 5f71 7565 7279 0d0a 2020 2020 6465 6620  _query..    def 
+0003ed20: 7965 656b 6974 5f61 7069 2873 656c 662c  yeekit_api(self,
+0003ed30: 2071 7565 7279 5f74 6578 743a 2073 7472   query_text: str
+0003ed40: 2c20 6672 6f6d 5f6c 616e 6775 6167 653a  , from_language:
+0003ed50: 2073 7472 203d 2027 6175 746f 272c 2074   str = 'auto', t
+0003ed60: 6f5f 6c61 6e67 7561 6765 3a20 7374 7220  o_language: str 
+0003ed70: 3d20 2765 6e27 2c20 2a2a 6b77 6172 6773  = 'en', **kwargs
+0003ed80: 3a20 4170 694b 7761 7267 7354 7970 6529  : ApiKwargsType)
+0003ed90: 202d 3e20 556e 696f 6e5b 7374 722c 2064   -> Union[str, d
+0003eda0: 6963 745d 3a0d 0a20 2020 2020 2020 2022  ict]:..        "
+0003edb0: 2222 0d0a 2020 2020 2020 2020 6874 7470  ""..        http
+0003edc0: 733a 2f2f 7777 772e 7965 656b 6974 2e63  s://www.yeekit.c
+0003edd0: 6f6d 2f73 6974 652f 7472 616e 736c 6174  om/site/translat
+0003ede0: 650d 0a20 2020 2020 2020 203a 7061 7261  e..        :para
+0003edf0: 6d20 7175 6572 795f 7465 7874 3a20 7374  m query_text: st
+0003ee00: 722c 206d 7573 742e 0d0a 2020 2020 2020  r, must...      
+0003ee10: 2020 3a70 6172 616d 2066 726f 6d5f 6c61    :param from_la
+0003ee20: 6e67 7561 6765 3a20 7374 722c 2064 6566  nguage: str, def
+0003ee30: 6175 6c74 2027 6175 746f 272e 0d0a 2020  ault 'auto'...  
+0003ee40: 2020 2020 2020 3a70 6172 616d 2074 6f5f        :param to_
+0003ee50: 6c61 6e67 7561 6765 3a20 7374 722c 2064  language: str, d
+0003ee60: 6566 6175 6c74 2027 656e 272e 0d0a 2020  efault 'en'...  
+0003ee70: 2020 2020 2020 3a70 6172 616d 202a 2a6b        :param **k
+0003ee80: 7761 7267 733a 0d0a 2020 2020 2020 2020  wargs:..        
+0003ee90: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
+0003eea0: 696d 656f 7574 3a20 666c 6f61 742c 2064  imeout: float, d
+0003eeb0: 6566 6175 6c74 204e 6f6e 652e 0d0a 2020  efault None...  
+0003eec0: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+0003eed0: 6172 616d 2070 726f 7869 6573 3a20 6469  aram proxies: di
+0003eee0: 6374 2c20 6465 6661 756c 7420 4e6f 6e65  ct, default None
+0003eef0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0003ef00: 2020 203a 7061 7261 6d20 736c 6565 705f     :param sleep_
+0003ef10: 7365 636f 6e64 733a 2066 6c6f 6174 2c20  seconds: float, 
+0003ef20: 6465 6661 756c 7420 302e 0d0a 2020 2020  default 0...    
+0003ef30: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0003ef40: 616d 2069 735f 6465 7461 696c 5f72 6573  am is_detail_res
+0003ef50: 756c 743a 2062 6f6f 6c2c 2064 6566 6175  ult: bool, defau
+0003ef60: 6c74 2046 616c 7365 2e0d 0a20 2020 2020  lt False...     
+0003ef70: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+0003ef80: 6d20 6966 5f69 676e 6f72 655f 6c69 6d69  m if_ignore_limi
+0003ef90: 745f 6f66 5f6c 656e 6774 683a 2062 6f6f  t_of_length: boo
+0003efa0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+0003efb0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0003efc0: 2020 203a 7061 7261 6d20 6c69 6d69 745f     :param limit_
+0003efd0: 6f66 5f6c 656e 6774 683a 2069 6e74 2c20  of_length: int, 
+0003efe0: 6465 6661 756c 7420 3230 3030 302e 0d0a  default 20000...
+0003eff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003f000: 3a70 6172 616d 2069 665f 6967 6e6f 7265  :param if_ignore
+0003f010: 5f65 6d70 7479 5f71 7565 7279 3a20 626f  _empty_query: bo
+0003f020: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
+0003f030: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
+0003f040: 2020 2020 3a70 6172 616d 2075 7064 6174      :param updat
+0003f050: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
+0003f060: 6672 6571 3a20 696e 742c 2064 6566 6175  freq: int, defau
+0003f070: 6c74 2031 3030 302e 0d0a 2020 2020 2020  lt 1000...      
+0003f080: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+0003f090: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
+0003f0a0: 6166 7465 725f 7365 636f 6e64 733a 2066  after_seconds: f
+0003f0b0: 6c6f 6174 2c20 6465 6661 756c 7420 3135  loat, default 15
+0003f0c0: 3030 2e0d 0a20 2020 2020 2020 2020 2020  00...           
+0003f0d0: 2020 2020 203a 7061 7261 6d20 6966 5f73       :param if_s
+0003f0e0: 686f 775f 7469 6d65 5f73 7461 743a 2062  how_time_stat: b
+0003f0f0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+0003f100: 7365 2e0d 0a20 2020 2020 2020 2020 2020  se...           
+0003f110: 2020 2020 203a 7061 7261 6d20 7368 6f77       :param show
+0003f120: 5f74 696d 655f 7374 6174 5f70 7265 6369  _time_stat_preci
+0003f130: 7369 6f6e 3a20 696e 742c 2064 6566 6175  sion: int, defau
+0003f140: 6c74 2032 2e0d 0a20 2020 2020 2020 2020  lt 2...         
+0003f150: 2020 2020 2020 203a 7061 7261 6d20 6966         :param if
+0003f160: 5f70 7269 6e74 5f77 6172 6e69 6e67 3a20  _print_warning: 
+0003f170: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
+0003f180: 7565 2e0d 0a20 2020 2020 2020 203a 7265  ue...        :re
+0003f190: 7475 726e 3a20 7374 7220 6f72 2064 6963  turn: str or dic
+0003f1a0: 740d 0a20 2020 2020 2020 2022 2222 0d0a  t..        """..
+0003f1b0: 0d0a 2020 2020 2020 2020 7469 6d65 6f75  ..        timeou
+0003f1c0: 7420 3d20 6b77 6172 6773 2e67 6574 2827  t = kwargs.get('
+0003f1d0: 7469 6d65 6f75 7427 2c20 4e6f 6e65 290d  timeout', None).
+0003f1e0: 0a20 2020 2020 2020 2070 726f 7869 6573  .        proxies
+0003f1f0: 203d 206b 7761 7267 732e 6765 7428 2770   = kwargs.get('p
+0003f200: 726f 7869 6573 272c 204e 6f6e 6529 0d0a  roxies', None)..
+0003f210: 2020 2020 2020 2020 736c 6565 705f 7365          sleep_se
+0003f220: 636f 6e64 7320 3d20 6b77 6172 6773 2e67  conds = kwargs.g
+0003f230: 6574 2827 736c 6565 705f 7365 636f 6e64  et('sleep_second
+0003f240: 7327 2c20 3029 0d0a 2020 2020 2020 2020  s', 0)..        
+0003f250: 6966 5f70 7269 6e74 5f77 6172 6e69 6e67  if_print_warning
+0003f260: 203d 206b 7761 7267 732e 6765 7428 2769   = kwargs.get('i
+0003f270: 665f 7072 696e 745f 7761 726e 696e 6727  f_print_warning'
+0003f280: 2c20 5472 7565 290d 0a20 2020 2020 2020  , True)..       
+0003f290: 2069 735f 6465 7461 696c 5f72 6573 756c   is_detail_resul
+0003f2a0: 7420 3d20 6b77 6172 6773 2e67 6574 2827  t = kwargs.get('
+0003f2b0: 6973 5f64 6574 6169 6c5f 7265 7375 6c74  is_detail_result
+0003f2c0: 272c 2046 616c 7365 290d 0a20 2020 2020  ', False)..     
+0003f2d0: 2020 2075 7064 6174 655f 7365 7373 696f     update_sessio
+0003f2e0: 6e5f 6166 7465 725f 6672 6571 203d 206b  n_after_freq = k
+0003f2f0: 7761 7267 732e 6765 7428 2775 7064 6174  wargs.get('updat
+0003f300: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
+0003f310: 6672 6571 272c 2073 656c 662e 6465 6661  freq', self.defa
+0003f320: 756c 745f 7365 7373 696f 6e5f 6672 6571  ult_session_freq
+0003f330: 290d 0a20 2020 2020 2020 2075 7064 6174  )..        updat
+0003f340: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
+0003f350: 7365 636f 6e64 7320 3d20 6b77 6172 6773  seconds = kwargs
+0003f360: 2e67 6574 2827 7570 6461 7465 5f73 6573  .get('update_ses
+0003f370: 7369 6f6e 5f61 6674 6572 5f73 6563 6f6e  sion_after_secon
+0003f380: 6473 272c 2073 656c 662e 6465 6661 756c  ds', self.defaul
+0003f390: 745f 7365 7373 696f 6e5f 7365 636f 6e64  t_session_second
+0003f3a0: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
+0003f3b0: 2e63 6865 636b 5f69 6e70 7574 5f6c 696d  .check_input_lim
+0003f3c0: 6974 2871 7565 7279 5f74 6578 742c 2073  it(query_text, s
+0003f3d0: 656c 662e 696e 7075 745f 6c69 6d69 7429  elf.input_limit)
+0003f3e0: 0d0a 0d0a 2020 2020 2020 2020 6e6f 745f  ....        not_
+0003f3f0: 7570 6461 7465 5f63 6f6e 645f 6672 6571  update_cond_freq
+0003f400: 203d 2031 2069 6620 7365 6c66 2e71 7565   = 1 if self.que
+0003f410: 7279 5f63 6f75 6e74 203c 2075 7064 6174  ry_count < updat
+0003f420: 655f 7365 7373 696f 6e5f 6166 7465 725f  e_session_after_
+0003f430: 6672 6571 2065 6c73 6520 300d 0a20 2020  freq else 0..   
+0003f440: 2020 2020 206e 6f74 5f75 7064 6174 655f       not_update_
+0003f450: 636f 6e64 5f74 696d 6520 3d20 3120 6966  cond_time = 1 if
+0003f460: 2074 696d 652e 7469 6d65 2829 202d 2073   time.time() - s
+0003f470: 656c 662e 6265 6769 6e5f 7469 6d65 203c  elf.begin_time <
+0003f480: 2075 7064 6174 655f 7365 7373 696f 6e5f   update_session_
+0003f490: 6166 7465 725f 7365 636f 6e64 7320 656c  after_seconds el
+0003f4a0: 7365 2030 0d0a 2020 2020 2020 2020 6966  se 0..        if
+0003f4b0: 206e 6f74 2028 7365 6c66 2e73 6573 7369   not (self.sessi
+0003f4c0: 6f6e 2061 6e64 2073 656c 662e 6c61 6e67  on and self.lang
+0003f4d0: 7561 6765 5f6d 6170 2061 6e64 206e 6f74  uage_map and not
+0003f4e0: 5f75 7064 6174 655f 636f 6e64 5f66 7265  _update_cond_fre
+0003f4f0: 7120 616e 6420 6e6f 745f 7570 6461 7465  q and not_update
+0003f500: 5f63 6f6e 645f 7469 6d65 293a 0d0a 2020  _cond_time):..  
+0003f510: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0003f520: 6573 7369 6f6e 203d 2072 6571 7565 7374  ession = request
+0003f530: 732e 5365 7373 696f 6e28 290d 0a20 2020  s.Session()..   
+0003f540: 2020 2020 2020 2020 205f 203d 2073 656c           _ = sel
+0003f550: 662e 7365 7373 696f 6e2e 6765 7428 7365  f.session.get(se
+0003f560: 6c66 2e68 6f73 745f 7572 6c2c 2068 6561  lf.host_url, hea
+0003f570: 6465 7273 3d73 656c 662e 686f 7374 5f68  ders=self.host_h
+0003f580: 6561 6465 7273 2c20 7469 6d65 6f75 743d  eaders, timeout=
+0003f590: 7469 6d65 6f75 742c 2070 726f 7869 6573  timeout, proxies
+0003f5a0: 3d70 726f 7869 6573 290d 0a20 2020 2020  =proxies)..     
+0003f5b0: 2020 2020 2020 2064 6562 7567 5f6c 616e         debug_lan
+0003f5c0: 675f 6b77 6172 6773 203d 2073 656c 662e  g_kwargs = self.
+0003f5d0: 6465 6275 675f 6c61 6e67 5f6b 7761 7267  debug_lang_kwarg
+0003f5e0: 7328 6672 6f6d 5f6c 616e 6775 6167 652c  s(from_language,
+0003f5f0: 2074 6f5f 6c61 6e67 7561 6765 2c20 7365   to_language, se
+0003f600: 6c66 2e64 6566 6175 6c74 5f66 726f 6d5f  lf.default_from_
+0003f610: 6c61 6e67 7561 6765 2c20 6966 5f70 7269  language, if_pri
+0003f620: 6e74 5f77 6172 6e69 6e67 290d 0a20 2020  nt_warning)..   
+0003f630: 2020 2020 2020 2020 2073 656c 662e 6c61           self.la
+0003f640: 6e67 7561 6765 5f6d 6170 203d 2073 656c  nguage_map = sel
+0003f650: 662e 6765 745f 6c61 6e67 7561 6765 5f6d  f.get_language_m
+0003f660: 6170 2873 656c 662e 6c61 6e67 5f6c 6973  ap(self.lang_lis
+0003f670: 742c 202a 2a64 6562 7567 5f6c 616e 675f  t, **debug_lang_
+0003f680: 6b77 6172 6773 290d 0a0d 0a20 2020 2020  kwargs)....     
+0003f690: 2020 2069 6620 6672 6f6d 5f6c 616e 6775     if from_langu
+0003f6a0: 6167 6520 3d3d 2027 6175 746f 273a 0d0a  age == 'auto':..
+0003f6b0: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
+0003f6c0: 5f6c 616e 6775 6167 6520 3d20 7365 6c66  _language = self
+0003f6d0: 2e77 6172 6e69 6e67 5f61 7574 6f5f 6c61  .warning_auto_la
+0003f6e0: 6e67 2827 7965 656b 6974 272c 2073 656c  ng('yeekit', sel
+0003f6f0: 662e 6465 6661 756c 745f 6672 6f6d 5f6c  f.default_from_l
+0003f700: 616e 6775 6167 652c 2069 665f 7072 696e  anguage, if_prin
+0003f710: 745f 7761 726e 696e 6729 0d0a 2020 2020  t_warning)..    
+0003f720: 2020 2020 6672 6f6d 5f6c 616e 6775 6167      from_languag
+0003f730: 652c 2074 6f5f 6c61 6e67 7561 6765 203d  e, to_language =
+0003f740: 2073 656c 662e 6368 6563 6b5f 6c61 6e67   self.check_lang
+0003f750: 7561 6765 2866 726f 6d5f 6c61 6e67 7561  uage(from_langua
+0003f760: 6765 2c20 746f 5f6c 616e 6775 6167 652c  ge, to_language,
+0003f770: 2073 656c 662e 6c61 6e67 7561 6765 5f6d   self.language_m
+0003f780: 6170 290d 0a0d 0a20 2020 2020 2020 2070  ap)....        p
+0003f790: 6179 6c6f 6164 203d 207b 0d0a 2020 2020  ayload = {..    
+0003f7a0: 2020 2020 2020 2020 2763 6f6e 7465 6e74          'content
+0003f7b0: 5b5d 273a 2071 7565 7279 5f74 6578 742c  []': query_text,
+0003f7c0: 0d0a 2020 2020 2020 2020 2020 2020 2773  ..            's
+0003f7d0: 6f75 7263 654c 616e 6727 3a20 6627 6e7b  ourceLang': f'n{
+0003f7e0: 6672 6f6d 5f6c 616e 6775 6167 657d 272c  from_language}',
+0003f7f0: 0d0a 2020 2020 2020 2020 2020 2020 2774  ..            't
+0003f800: 6172 6765 744c 616e 6727 3a20 6627 6e7b  argetLang': f'n{
+0003f810: 746f 5f6c 616e 6775 6167 657d 272c 0d0a  to_language}',..
+0003f820: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+0003f830: 2020 2070 6179 6c6f 6164 203d 2075 726c     payload = url
+0003f840: 6c69 622e 7061 7273 652e 7572 6c65 6e63  lib.parse.urlenc
+0003f850: 6f64 6528 7061 796c 6f61 6429 0d0a 2020  ode(payload)..  
+0003f860: 2020 2020 2020 7220 3d20 7365 6c66 2e73        r = self.s
+0003f870: 6573 7369 6f6e 2e70 6f73 7428 7365 6c66  ession.post(self
+0003f880: 2e61 7069 5f75 726c 2c20 6461 7461 3d70  .api_url, data=p
+0003f890: 6179 6c6f 6164 2c20 6865 6164 6572 733d  ayload, headers=
+0003f8a0: 7365 6c66 2e61 7069 5f68 6561 6465 7273  self.api_headers
+0003f8b0: 2c20 7469 6d65 6f75 743d 7469 6d65 6f75  , timeout=timeou
+0003f8c0: 742c 2070 726f 7869 6573 3d70 726f 7869  t, proxies=proxi
+0003f8d0: 6573 290d 0a20 2020 2020 2020 2072 2e72  es)..        r.r
+0003f8e0: 6169 7365 5f66 6f72 5f73 7461 7475 7328  aise_for_status(
+0003f8f0: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
+0003f900: 3d20 722e 6a73 6f6e 2829 0d0a 2020 2020  = r.json()..    
+0003f910: 2020 2020 7469 6d65 2e73 6c65 6570 2873      time.sleep(s
+0003f920: 6c65 6570 5f73 6563 6f6e 6473 290d 0a20  leep_seconds).. 
+0003f930: 2020 2020 2020 2073 656c 662e 7175 6572         self.quer
+0003f940: 795f 636f 756e 7420 2b3d 2031 0d0a 2020  y_count += 1..  
+0003f950: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
+0003f960: 6120 6966 2069 735f 6465 7461 696c 5f72  a if is_detail_r
+0003f970: 6573 756c 7420 656c 7365 2027 5c6e 272e  esult else '\n'.
+0003f980: 6a6f 696e 2827 2027 2e6a 6f69 6e28 7029  join(' '.join(p)
+0003f990: 2066 6f72 2070 2069 6e20 6a73 6f6e 2e6c   for p in json.l
+0003f9a0: 6f61 6473 2864 6174 615b 305d 295b 2774  oads(data[0])['t
+0003f9b0: 7261 6e73 6c61 7469 6f6e 275d 5b30 5d5b  ranslation'][0][
+0003f9c0: 2774 7261 6e73 6c61 7465 6427 5d5b 305d  'translated'][0]
+0003f9d0: 5b27 7472 616e 736c 6174 696f 6e20 6c69  ['translation li
+0003f9e0: 7374 275d 290d 0a0d 0a0d 0a63 6c61 7373  st'])......class
+0003f9f0: 2054 7261 6e73 6c61 746f 7273 5365 7276   TranslatorsServ
+0003fa00: 6572 3a0d 0a20 2020 2064 6566 205f 5f69  er:..    def __i
+0003fa10: 6e69 745f 5f28 7365 6c66 293a 0d0a 2020  nit__(self):..  
+0003fa20: 2020 2020 2020 7365 6c66 2e63 7075 5f63        self.cpu_c
+0003fa30: 6e74 203d 206f 732e 6370 755f 636f 756e  nt = os.cpu_coun
+0003fa40: 7428 290d 0a20 2020 2020 2020 2073 656c  t()..        sel
+0003fa50: 662e 7365 7276 6572 5f72 6567 696f 6e20  f.server_region 
+0003fa60: 3d20 4775 6573 7453 6576 6572 5265 6769  = GuestSeverRegi
+0003fa70: 6f6e 2829 2e67 6574 5f73 6572 7665 725f  on().get_server_
+0003fa80: 7265 6769 6f6e 0d0a 2020 2020 2020 2020  region..        
+0003fa90: 7365 6c66 2e5f 616c 6962 6162 6120 3d20  self._alibaba = 
+0003faa0: 416c 6962 6162 6156 3228 290d 0a20 2020  AlibabaV2()..   
+0003fab0: 2020 2020 2073 656c 662e 616c 6962 6162       self.alibab
+0003fac0: 6120 3d20 7365 6c66 2e5f 616c 6962 6162  a = self._alibab
+0003fad0: 612e 616c 6962 6162 615f 6170 690d 0a20  a.alibaba_api.. 
+0003fae0: 2020 2020 2020 2073 656c 662e 5f61 7065         self._ape
+0003faf0: 7274 6975 6d20 3d20 4170 6572 7469 756d  rtium = Apertium
+0003fb00: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+0003fb10: 2e61 7065 7274 6975 6d20 3d20 7365 6c66  .apertium = self
+0003fb20: 2e5f 6170 6572 7469 756d 2e61 7065 7274  ._apertium.apert
+0003fb30: 6975 6d5f 6170 690d 0a20 2020 2020 2020  ium_api..       
+0003fb40: 2073 656c 662e 5f61 7267 6f73 203d 2041   self._argos = A
+0003fb50: 7267 6f73 2829 0d0a 2020 2020 2020 2020  rgos()..        
+0003fb60: 7365 6c66 2e61 7267 6f73 203d 2073 656c  self.argos = sel
+0003fb70: 662e 5f61 7267 6f73 2e61 7267 6f73 5f61  f._argos.argos_a
+0003fb80: 7069 0d0a 2020 2020 2020 2020 7365 6c66  pi..        self
+0003fb90: 2e5f 6261 6964 7520 3d20 4261 6964 7556  ._baidu = BaiduV
+0003fba0: 3128 2920 2023 2056 320d 0a20 2020 2020  1()  # V2..     
+0003fbb0: 2020 2073 656c 662e 6261 6964 7520 3d20     self.baidu = 
+0003fbc0: 7365 6c66 2e5f 6261 6964 752e 6261 6964  self._baidu.baid
+0003fbd0: 755f 6170 690d 0a20 2020 2020 2020 2073  u_api..        s
+0003fbe0: 656c 662e 5f62 696e 6720 3d20 4269 6e67  elf._bing = Bing
+0003fbf0: 2873 6572 7665 725f 7265 6769 6f6e 3d73  (server_region=s
+0003fc00: 656c 662e 7365 7276 6572 5f72 6567 696f  elf.server_regio
+0003fc10: 6e29 0d0a 2020 2020 2020 2020 7365 6c66  n)..        self
+0003fc20: 2e62 696e 6720 3d20 7365 6c66 2e5f 6269  .bing = self._bi
+0003fc30: 6e67 2e62 696e 675f 6170 690d 0a20 2020  ng.bing_api..   
+0003fc40: 2020 2020 2073 656c 662e 5f63 6169 7975       self._caiyu
+0003fc50: 6e20 3d20 4361 6979 756e 2829 0d0a 2020  n = Caiyun()..  
+0003fc60: 2020 2020 2020 7365 6c66 2e63 6169 7975        self.caiyu
+0003fc70: 6e20 3d20 7365 6c66 2e5f 6361 6979 756e  n = self._caiyun
+0003fc80: 2e63 6169 7975 6e5f 6170 690d 0a20 2020  .caiyun_api..   
+0003fc90: 2020 2020 2073 656c 662e 5f63 6c6f 7564       self._cloud
+0003fca0: 5969 203d 2043 6c6f 7564 5969 2829 0d0a  Yi = CloudYi()..
+0003fcb0: 2020 2020 2020 2020 7365 6c66 2e63 6c6f          self.clo
+0003fcc0: 7564 5969 203d 2073 656c 662e 5f63 6c6f  udYi = self._clo
+0003fcd0: 7564 5969 2e63 6c6f 7564 5969 5f61 7069  udYi.cloudYi_api
+0003fce0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+0003fcf0: 6465 6570 6c20 3d20 4465 6570 6c28 290d  deepl = Deepl().
+0003fd00: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
+0003fd10: 6570 6c20 3d20 7365 6c66 2e5f 6465 6570  epl = self._deep
+0003fd20: 6c2e 6465 6570 6c5f 6170 690d 0a20 2020  l.deepl_api..   
+0003fd30: 2020 2020 2073 656c 662e 5f65 6c69 6120       self._elia 
+0003fd40: 3d20 456c 6961 2829 0d0a 2020 2020 2020  = Elia()..      
+0003fd50: 2020 7365 6c66 2e65 6c69 6120 3d20 7365    self.elia = se
+0003fd60: 6c66 2e5f 656c 6961 2e65 6c69 615f 6170  lf._elia.elia_ap
+0003fd70: 690d 0a20 2020 2020 2020 2073 656c 662e  i..        self.
+0003fd80: 5f67 6f6f 676c 6520 3d20 476f 6f67 6c65  _google = Google
+0003fd90: 5632 2873 6572 7665 725f 7265 6769 6f6e  V2(server_region
+0003fda0: 3d73 656c 662e 7365 7276 6572 5f72 6567  =self.server_reg
+0003fdb0: 696f 6e29 0d0a 2020 2020 2020 2020 7365  ion)..        se
+0003fdc0: 6c66 2e67 6f6f 676c 6520 3d20 7365 6c66  lf.google = self
+0003fdd0: 2e5f 676f 6f67 6c65 2e67 6f6f 676c 655f  ._google.google_
+0003fde0: 6170 690d 0a20 2020 2020 2020 2073 656c  api..        sel
+0003fdf0: 662e 5f69 6369 6261 203d 2049 6369 6261  f._iciba = Iciba
+0003fe00: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+0003fe10: 2e69 6369 6261 203d 2073 656c 662e 5f69  .iciba = self._i
+0003fe20: 6369 6261 2e69 6369 6261 5f61 7069 0d0a  ciba.iciba_api..
+0003fe30: 2020 2020 2020 2020 7365 6c66 2e5f 6966          self._if
+0003fe40: 6c79 7465 6b20 3d20 4966 6c79 7465 6b56  lytek = IflytekV
+0003fe50: 3228 290d 0a20 2020 2020 2020 2073 656c  2()..        sel
+0003fe60: 662e 6966 6c79 7465 6b20 3d20 7365 6c66  f.iflytek = self
+0003fe70: 2e5f 6966 6c79 7465 6b2e 6966 6c79 7465  ._iflytek.iflyte
+0003fe80: 6b5f 6170 690d 0a20 2020 2020 2020 2073  k_api..        s
+0003fe90: 656c 662e 5f69 666c 7972 6563 203d 2049  elf._iflyrec = I
+0003fea0: 666c 7972 6563 2829 0d0a 2020 2020 2020  flyrec()..      
+0003feb0: 2020 7365 6c66 2e69 666c 7972 6563 203d    self.iflyrec =
+0003fec0: 2073 656c 662e 5f69 666c 7972 6563 2e69   self._iflyrec.i
+0003fed0: 666c 7972 6563 5f61 7069 0d0a 2020 2020  flyrec_api..    
+0003fee0: 2020 2020 7365 6c66 2e5f 6974 7261 6e73      self._itrans
+0003fef0: 6c61 7465 203d 2049 7472 616e 736c 6174  late = Itranslat
+0003ff00: 6528 290d 0a20 2020 2020 2020 2073 656c  e()..        sel
+0003ff10: 662e 6974 7261 6e73 6c61 7465 203d 2073  f.itranslate = s
+0003ff20: 656c 662e 5f69 7472 616e 736c 6174 652e  elf._itranslate.
+0003ff30: 6974 7261 6e73 6c61 7465 5f61 7069 0d0a  itranslate_api..
+0003ff40: 2020 2020 2020 2020 7365 6c66 2e5f 6a75          self._ju
+0003ff50: 6469 6320 3d20 4a75 6469 6328 290d 0a20  dic = Judic().. 
+0003ff60: 2020 2020 2020 2073 656c 662e 6a75 6469         self.judi
+0003ff70: 6320 3d20 7365 6c66 2e5f 6a75 6469 632e  c = self._judic.
+0003ff80: 6a75 6469 635f 6170 690d 0a20 2020 2020  judic_api..     
+0003ff90: 2020 2073 656c 662e 5f6c 616e 6775 6167     self._languag
+0003ffa0: 6557 6972 6520 3d20 4c61 6e67 7561 6765  eWire = Language
+0003ffb0: 5769 7265 2829 0d0a 2020 2020 2020 2020  Wire()..        
+0003ffc0: 7365 6c66 2e6c 616e 6775 6167 6557 6972  self.languageWir
+0003ffd0: 6520 3d20 7365 6c66 2e5f 6c61 6e67 7561  e = self._langua
+0003ffe0: 6765 5769 7265 2e6c 616e 6775 6167 6557  geWire.languageW
+0003fff0: 6972 655f 6170 690d 0a20 2020 2020 2020  ire_api..       
+00040000: 2073 656c 662e 5f6c 696e 6776 616e 6578   self._lingvanex
+00040010: 203d 204c 696e 6776 616e 6578 2829 0d0a   = Lingvanex()..
+00040020: 2020 2020 2020 2020 7365 6c66 2e6c 696e          self.lin
+00040030: 6776 616e 6578 203d 2073 656c 662e 5f6c  gvanex = self._l
+00040040: 696e 6776 616e 6578 2e6c 696e 6776 616e  ingvanex.lingvan
+00040050: 6578 5f61 7069 0d0a 2020 2020 2020 2020  ex_api..        
+00040060: 7365 6c66 2e5f 6e69 7574 7261 6e73 203d  self._niutrans =
+00040070: 204e 6975 7472 616e 7328 290d 0a20 2020   Niutrans()..   
+00040080: 2020 2020 2073 656c 662e 6e69 7574 7261       self.niutra
+00040090: 6e73 203d 2073 656c 662e 5f6e 6975 7472  ns = self._niutr
+000400a0: 616e 732e 6e69 7574 7261 6e73 5f61 7069  ans.niutrans_api
+000400b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000400c0: 6d67 6c69 7020 3d20 4d67 6c69 7028 290d  mglip = Mglip().
+000400d0: 0a20 2020 2020 2020 2073 656c 662e 6d67  .        self.mg
+000400e0: 6c69 7020 3d20 7365 6c66 2e5f 6d67 6c69  lip = self._mgli
+000400f0: 702e 6d67 6c69 705f 6170 690d 0a20 2020  p.mglip_api..   
+00040100: 2020 2020 2073 656c 662e 5f6d 6972 6169       self._mirai
+00040110: 203d 204d 6972 6169 2829 0d0a 2020 2020   = Mirai()..    
+00040120: 2020 2020 7365 6c66 2e6d 6972 6169 203d      self.mirai =
+00040130: 2073 656c 662e 5f6d 6972 6169 2e6d 6972   self._mirai.mir
+00040140: 6169 5f61 7069 0d0a 2020 2020 2020 2020  ai_api..        
+00040150: 7365 6c66 2e5f 6d6f 6465 726e 4d74 203d  self._modernMt =
+00040160: 204d 6f64 6572 6e4d 7428 290d 0a20 2020   ModernMt()..   
+00040170: 2020 2020 2073 656c 662e 6d6f 6465 726e       self.modern
+00040180: 4d74 203d 2073 656c 662e 5f6d 6f64 6572  Mt = self._moder
+00040190: 6e4d 742e 6d6f 6465 726e 4d74 5f61 7069  nMt.modernMt_api
+000401a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000401b0: 6d79 4d65 6d6f 7279 203d 204d 794d 656d  myMemory = MyMem
+000401c0: 6f72 7928 290d 0a20 2020 2020 2020 2073  ory()..        s
+000401d0: 656c 662e 6d79 4d65 6d6f 7279 203d 2073  elf.myMemory = s
+000401e0: 656c 662e 5f6d 794d 656d 6f72 792e 6d79  elf._myMemory.my
+000401f0: 4d65 6d6f 7279 5f61 7069 0d0a 2020 2020  Memory_api..    
+00040200: 2020 2020 7365 6c66 2e5f 7061 7061 676f      self._papago
+00040210: 203d 2050 6170 6167 6f28 290d 0a20 2020   = Papago()..   
+00040220: 2020 2020 2073 656c 662e 7061 7061 676f       self.papago
+00040230: 203d 2073 656c 662e 5f70 6170 6167 6f2e   = self._papago.
+00040240: 7061 7061 676f 5f61 7069 0d0a 2020 2020  papago_api..    
+00040250: 2020 2020 7365 6c66 2e5f 7171 4661 6e79      self._qqFany
+00040260: 6920 3d20 5151 4661 6e79 6928 290d 0a20  i = QQFanyi().. 
+00040270: 2020 2020 2020 2073 656c 662e 7171 4661         self.qqFa
+00040280: 6e79 6920 3d20 7365 6c66 2e5f 7171 4661  nyi = self._qqFa
+00040290: 6e79 692e 7171 4661 6e79 695f 6170 690d  nyi.qqFanyi_api.
+000402a0: 0a20 2020 2020 2020 2073 656c 662e 5f71  .        self._q
+000402b0: 7154 7261 6e53 6d61 7274 203d 2051 5154  qTranSmart = QQT
+000402c0: 7261 6e53 6d61 7274 2829 0d0a 2020 2020  ranSmart()..    
+000402d0: 2020 2020 7365 6c66 2e71 7154 7261 6e53      self.qqTranS
+000402e0: 6d61 7274 203d 2073 656c 662e 5f71 7154  mart = self._qqT
+000402f0: 7261 6e53 6d61 7274 2e71 7154 7261 6e53  ranSmart.qqTranS
+00040300: 6d61 7274 5f61 7069 0d0a 2020 2020 2020  mart_api..      
+00040310: 2020 7365 6c66 2e5f 7265 7665 7273 6f20    self._reverso 
+00040320: 3d20 5265 7665 7273 6f28 290d 0a20 2020  = Reverso()..   
+00040330: 2020 2020 2073 656c 662e 7265 7665 7273       self.revers
+00040340: 6f20 3d20 7365 6c66 2e5f 7265 7665 7273  o = self._revers
+00040350: 6f2e 7265 7665 7273 6f5f 6170 690d 0a20  o.reverso_api.. 
+00040360: 2020 2020 2020 2073 656c 662e 5f73 6f67         self._sog
+00040370: 6f75 203d 2053 6f67 6f75 2829 0d0a 2020  ou = Sogou()..  
+00040380: 2020 2020 2020 7365 6c66 2e73 6f67 6f75        self.sogou
+00040390: 203d 2073 656c 662e 5f73 6f67 6f75 2e73   = self._sogou.s
+000403a0: 6f67 6f75 5f61 7069 0d0a 2020 2020 2020  ogou_api..      
+000403b0: 2020 7365 6c66 2e5f 7379 7354 7261 6e20    self._sysTran 
+000403c0: 3d20 5379 7354 7261 6e28 290d 0a20 2020  = SysTran()..   
+000403d0: 2020 2020 2073 656c 662e 7379 7354 7261       self.sysTra
+000403e0: 6e20 3d20 7365 6c66 2e5f 7379 7354 7261  n = self._sysTra
+000403f0: 6e2e 7379 7354 7261 6e5f 6170 690d 0a20  n.sysTran_api.. 
+00040400: 2020 2020 2020 2073 656c 662e 5f74 696c         self._til
+00040410: 6465 203d 2054 696c 6465 2829 0d0a 2020  de = Tilde()..  
+00040420: 2020 2020 2020 7365 6c66 2e74 696c 6465        self.tilde
+00040430: 203d 2073 656c 662e 5f74 696c 6465 2e74   = self._tilde.t
+00040440: 696c 6465 5f61 7069 0d0a 2020 2020 2020  ilde_api..      
+00040450: 2020 7365 6c66 2e5f 7472 616e 736c 6174    self._translat
+00040460: 6543 6f6d 203d 2054 7261 6e73 6c61 7465  eCom = Translate
+00040470: 436f 6d28 290d 0a20 2020 2020 2020 2073  Com()..        s
+00040480: 656c 662e 7472 616e 736c 6174 6543 6f6d  elf.translateCom
+00040490: 203d 2073 656c 662e 5f74 7261 6e73 6c61   = self._transla
+000404a0: 7465 436f 6d2e 7472 616e 736c 6174 6543  teCom.translateC
+000404b0: 6f6d 5f61 7069 0d0a 2020 2020 2020 2020  om_api..        
+000404c0: 7365 6c66 2e5f 7472 616e 736c 6174 654d  self._translateM
+000404d0: 6520 3d20 5472 616e 736c 6174 654d 6528  e = TranslateMe(
+000404e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000404f0: 7472 616e 736c 6174 654d 6520 3d20 7365  translateMe = se
+00040500: 6c66 2e5f 7472 616e 736c 6174 654d 652e  lf._translateMe.
+00040510: 7472 616e 736c 6174 654d 655f 6170 690d  translateMe_api.
+00040520: 0a20 2020 2020 2020 2073 656c 662e 5f75  .        self._u
+00040530: 7469 6265 7420 3d20 5574 6962 6574 2829  tibet = Utibet()
+00040540: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00040550: 7469 6265 7420 3d20 7365 6c66 2e5f 7574  tibet = self._ut
+00040560: 6962 6574 2e75 7469 6265 745f 6170 690d  ibet.utibet_api.
+00040570: 0a20 2020 2020 2020 2073 656c 662e 5f76  .        self._v
+00040580: 6f6c 6345 6e67 696e 6520 3d20 566f 6c63  olcEngine = Volc
+00040590: 456e 6769 6e65 2829 0d0a 2020 2020 2020  Engine()..      
+000405a0: 2020 7365 6c66 2e76 6f6c 6345 6e67 696e    self.volcEngin
+000405b0: 6520 3d20 7365 6c66 2e5f 766f 6c63 456e  e = self._volcEn
+000405c0: 6769 6e65 2e76 6f6c 6345 6e67 696e 655f  gine.volcEngine_
+000405d0: 6170 690d 0a20 2020 2020 2020 2073 656c  api..        sel
+000405e0: 662e 5f79 616e 6465 7820 3d20 5961 6e64  f._yandex = Yand
+000405f0: 6578 2829 0d0a 2020 2020 2020 2020 7365  ex()..        se
+00040600: 6c66 2e79 616e 6465 7820 3d20 7365 6c66  lf.yandex = self
+00040610: 2e5f 7961 6e64 6578 2e79 616e 6465 785f  ._yandex.yandex_
+00040620: 6170 690d 0a20 2020 2020 2020 2073 656c  api..        sel
+00040630: 662e 5f79 6565 6b69 7420 3d20 5965 656b  f._yeekit = Yeek
+00040640: 6974 2829 0d0a 2020 2020 2020 2020 7365  it()..        se
+00040650: 6c66 2e79 6565 6b69 7420 3d20 7365 6c66  lf.yeekit = self
+00040660: 2e5f 7965 656b 6974 2e79 6565 6b69 745f  ._yeekit.yeekit_
+00040670: 6170 690d 0a20 2020 2020 2020 2073 656c  api..        sel
+00040680: 662e 5f79 6f75 6461 6f20 3d20 596f 7564  f._youdao = Youd
+00040690: 616f 5633 2829 0d0a 2020 2020 2020 2020  aoV3()..        
+000406a0: 7365 6c66 2e79 6f75 6461 6f20 3d20 7365  self.youdao = se
+000406b0: 6c66 2e5f 796f 7564 616f 2e79 6f75 6461  lf._youdao.youda
+000406c0: 6f5f 6170 690d 0a20 2020 2020 2020 2073  o_api..        s
+000406d0: 656c 662e 7472 616e 736c 6174 6f72 735f  elf.translators_
+000406e0: 6469 6374 203d 207b 0d0a 2020 2020 2020  dict = {..      
+000406f0: 2020 2020 2020 2761 6c69 6261 6261 273a        'alibaba':
+00040700: 2073 656c 662e 616c 6962 6162 612c 2027   self.alibaba, '
+00040710: 6170 6572 7469 756d 273a 2073 656c 662e  apertium': self.
+00040720: 6170 6572 7469 756d 2c20 2761 7267 6f73  apertium, 'argos
+00040730: 273a 2073 656c 662e 6172 676f 732c 2027  ': self.argos, '
+00040740: 6261 6964 7527 3a20 7365 6c66 2e62 6169  baidu': self.bai
+00040750: 6475 2c20 2762 696e 6727 3a20 7365 6c66  du, 'bing': self
+00040760: 2e62 696e 672c 0d0a 2020 2020 2020 2020  .bing,..        
+00040770: 2020 2020 2763 6169 7975 6e27 3a20 7365      'caiyun': se
+00040780: 6c66 2e63 6169 7975 6e2c 2027 636c 6f75  lf.caiyun, 'clou
+00040790: 6459 6927 3a20 7365 6c66 2e63 6c6f 7564  dYi': self.cloud
+000407a0: 5969 2c20 2764 6565 706c 273a 2073 656c  Yi, 'deepl': sel
+000407b0: 662e 6465 6570 6c2c 2027 656c 6961 273a  f.deepl, 'elia':
+000407c0: 2073 656c 662e 656c 6961 2c20 2767 6f6f   self.elia, 'goo
+000407d0: 676c 6527 3a20 7365 6c66 2e67 6f6f 676c  gle': self.googl
+000407e0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000407f0: 2769 6369 6261 273a 2073 656c 662e 6963  'iciba': self.ic
+00040800: 6962 612c 2027 6966 6c79 7465 6b27 3a20  iba, 'iflytek': 
+00040810: 7365 6c66 2e69 666c 7974 656b 2c20 2769  self.iflytek, 'i
+00040820: 666c 7972 6563 273a 2073 656c 662e 6966  flyrec': self.if
+00040830: 6c79 7265 632c 2027 6974 7261 6e73 6c61  lyrec, 'itransla
+00040840: 7465 273a 2073 656c 662e 6974 7261 6e73  te': self.itrans
+00040850: 6c61 7465 2c20 276a 7564 6963 273a 2073  late, 'judic': s
+00040860: 656c 662e 6a75 6469 632c 0d0a 2020 2020  elf.judic,..    
+00040870: 2020 2020 2020 2020 276c 616e 6775 6167          'languag
+00040880: 6557 6972 6527 3a20 7365 6c66 2e6c 616e  eWire': self.lan
+00040890: 6775 6167 6557 6972 652c 2027 6c69 6e67  guageWire, 'ling
+000408a0: 7661 6e65 7827 3a20 7365 6c66 2e6c 696e  vanex': self.lin
+000408b0: 6776 616e 6578 2c20 276e 6975 7472 616e  gvanex, 'niutran
+000408c0: 7327 3a20 7365 6c66 2e6e 6975 7472 616e  s': self.niutran
+000408d0: 732c 2027 6d67 6c69 7027 3a20 7365 6c66  s, 'mglip': self
+000408e0: 2e6d 676c 6970 2c20 276d 6f64 6572 6e4d  .mglip, 'modernM
+000408f0: 7427 3a20 7365 6c66 2e6d 6f64 6572 6e4d  t': self.modernM
+00040900: 742c 0d0a 2020 2020 2020 2020 2020 2020  t,..            
+00040910: 276d 794d 656d 6f72 7927 3a20 7365 6c66  'myMemory': self
+00040920: 2e6d 794d 656d 6f72 792c 2027 7061 7061  .myMemory, 'papa
+00040930: 676f 273a 2073 656c 662e 7061 7061 676f  go': self.papago
+00040940: 2c20 2771 7146 616e 7969 273a 2073 656c  , 'qqFanyi': sel
+00040950: 662e 7171 4661 6e79 692c 2027 7171 5472  f.qqFanyi, 'qqTr
+00040960: 616e 536d 6172 7427 3a20 7365 6c66 2e71  anSmart': self.q
+00040970: 7154 7261 6e53 6d61 7274 2c20 2772 6576  qTranSmart, 'rev
+00040980: 6572 736f 273a 2073 656c 662e 7265 7665  erso': self.reve
+00040990: 7273 6f2c 0d0a 2020 2020 2020 2020 2020  rso,..          
+000409a0: 2020 2773 6f67 6f75 273a 2073 656c 662e    'sogou': self.
+000409b0: 736f 676f 752c 2027 7379 7354 7261 6e27  sogou, 'sysTran'
+000409c0: 3a20 7365 6c66 2e73 7973 5472 616e 2c20  : self.sysTran, 
+000409d0: 2774 696c 6465 273a 2073 656c 662e 7469  'tilde': self.ti
+000409e0: 6c64 652c 2027 7472 616e 736c 6174 6543  lde, 'translateC
+000409f0: 6f6d 273a 2073 656c 662e 7472 616e 736c  om': self.transl
+00040a00: 6174 6543 6f6d 2c20 2774 7261 6e73 6c61  ateCom, 'transla
+00040a10: 7465 4d65 273a 2073 656c 662e 7472 616e  teMe': self.tran
+00040a20: 736c 6174 654d 652c 0d0a 2020 2020 2020  slateMe,..      
+00040a30: 2020 2020 2020 2775 7469 6265 7427 3a20        'utibet': 
+00040a40: 7365 6c66 2e75 7469 6265 742c 2027 766f  self.utibet, 'vo
+00040a50: 6c63 456e 6769 6e65 273a 2073 656c 662e  lcEngine': self.
+00040a60: 766f 6c63 456e 6769 6e65 2c20 2779 616e  volcEngine, 'yan
+00040a70: 6465 7827 3a20 7365 6c66 2e79 616e 6465  dex': self.yande
+00040a80: 782c 2027 7965 656b 6974 273a 2073 656c  x, 'yeekit': sel
+00040a90: 662e 7965 656b 6974 2c20 2779 6f75 6461  f.yeekit, 'youda
+00040aa0: 6f27 3a20 7365 6c66 2e79 6f75 6461 6f2c  o': self.youdao,
+00040ab0: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
+00040ac0: 2020 2020 2073 656c 662e 7472 616e 736c       self.transl
+00040ad0: 6174 6f72 735f 706f 6f6c 203d 206c 6973  ators_pool = lis
+00040ae0: 7428 7365 6c66 2e74 7261 6e73 6c61 746f  t(self.translato
+00040af0: 7273 5f64 6963 742e 6b65 7973 2829 290d  rs_dict.keys()).
+00040b00: 0a20 2020 2020 2020 2073 656c 662e 6e6f  .        self.no
+00040b10: 745f 656e 5f6c 616e 6773 203d 207b 2775  t_en_langs = {'u
+00040b20: 7469 6265 7427 3a20 2774 6927 2c20 276d  tibet': 'ti', 'm
+00040b30: 676c 6970 273a 2027 6d6f 6e27 7d0d 0a20  glip': 'mon'}.. 
+00040b40: 2020 2020 2020 2073 656c 662e 6e6f 745f         self.not_
+00040b50: 7a68 5f6c 616e 6773 203d 207b 276c 616e  zh_langs = {'lan
+00040b60: 6775 6167 6557 6972 6527 3a20 2766 7227  guageWire': 'fr'
+00040b70: 2c20 2774 696c 6465 273a 2027 6672 272c  , 'tilde': 'fr',
+00040b80: 2027 656c 6961 273a 2027 6672 272c 2027   'elia': 'fr', '
+00040b90: 6170 6572 7469 756d 273a 2027 7370 6127  apertium': 'spa'
+00040ba0: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
+00040bb0: 7072 655f 6163 6365 6c65 7261 7469 6f6e  pre_acceleration
+00040bc0: 5f6c 6162 656c 203d 2030 0d0a 2020 2020  _label = 0..    
+00040bd0: 2020 2020 7365 6c66 2e65 7861 6d70 6c65      self.example
+00040be0: 5f71 7565 7279 5f74 6578 7420 3d20 27e4  _query_text = '.
+00040bf0: bda0 e5a5 bde3 8082 5c6e e6ac a2e8 bf8e  ........\n......
+00040c00: e4bd a0ef bc81 270d 0a20 2020 2020 2020  ......'..       
+00040c10: 2073 656c 662e 7375 6363 6573 735f 7472   self.success_tr
+00040c20: 616e 736c 6174 6f72 735f 706f 6f6c 203d  anslators_pool =
+00040c30: 205b 5d0d 0a20 2020 2020 2020 2073 656c   []..        sel
+00040c40: 662e 6661 696c 7572 655f 7472 616e 736c  f.failure_transl
+00040c50: 6174 6f72 735f 706f 6f6c 203d 205b 5d0d  ators_pool = [].
+00040c60: 0a0d 0a20 2020 2064 6566 2074 7261 6e73  ...    def trans
+00040c70: 6c61 7465 5f74 6578 7428 7365 6c66 2c0d  late_text(self,.
+00040c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00040c90: 2020 2020 2020 2020 7175 6572 795f 7465          query_te
+00040ca0: 7874 3a20 7374 722c 0d0a 2020 2020 2020  xt: str,..      
+00040cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00040cc0: 2074 7261 6e73 6c61 746f 723a 2073 7472   translator: str
+00040cd0: 203d 2027 6269 6e67 272c 0d0a 2020 2020   = 'bing',..    
+00040ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00040cf0: 2020 2066 726f 6d5f 6c61 6e67 7561 6765     from_language
+00040d00: 3a20 7374 7220 3d20 2761 7574 6f27 2c0d  : str = 'auto',.
+00040d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00040d20: 2020 2020 2020 2020 746f 5f6c 616e 6775          to_langu
+00040d30: 6167 653a 2073 7472 203d 2027 656e 272c  age: str = 'en',
+00040d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00040d50: 2020 2020 2020 2020 2069 665f 7573 655f           if_use_
+00040d60: 7072 6561 6363 656c 6572 6174 696f 6e3a  preacceleration:
+00040d70: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+00040d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00040d90: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
+00040da0: 2041 7069 4b77 6172 6773 5479 7065 2c0d   ApiKwargsType,.
+00040db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00040dc0: 2020 2020 2020 2020 2920 2d3e 2055 6e69          ) -> Uni
+00040dd0: 6f6e 5b73 7472 2c20 6469 6374 5d3a 0d0a  on[str, dict]:..
+00040de0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00040df0: 2020 2020 203a 7061 7261 6d20 7175 6572       :param quer
+00040e00: 795f 7465 7874 3a20 7374 722c 206d 7573  y_text: str, mus
+00040e10: 742e 0d0a 2020 2020 2020 2020 3a70 6172  t...        :par
+00040e20: 616d 2074 7261 6e73 6c61 746f 723a 2073  am translator: s
+00040e30: 7472 2c20 6465 6661 756c 7420 2762 696e  tr, default 'bin
+00040e40: 6727 2e0d 0a20 2020 2020 2020 203a 7061  g'...        :pa
+00040e50: 7261 6d20 6672 6f6d 5f6c 616e 6775 6167  ram from_languag
+00040e60: 653a 2073 7472 2c20 6465 6661 756c 7420  e: str, default 
+00040e70: 2761 7574 6f27 2e0d 0a20 2020 2020 2020  'auto'...       
+00040e80: 203a 7061 7261 6d20 746f 5f6c 616e 6775   :param to_langu
+00040e90: 6167 653a 2073 7472 2c20 6465 6661 756c  age: str, defaul
+00040ea0: 7420 2765 6e27 2e0d 0a20 2020 2020 2020  t 'en'...       
+00040eb0: 203a 7061 7261 6d20 6966 5f75 7365 5f70   :param if_use_p
+00040ec0: 7265 6163 6365 6c65 7261 7469 6f6e 3a20  reacceleration: 
+00040ed0: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+00040ee0: 6c73 652e 0d0a 2020 2020 2020 2020 3a70  lse...        :p
+00040ef0: 6172 616d 202a 2a6b 7761 7267 733a 0d0a  aram **kwargs:..
+00040f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00040f10: 3a70 6172 616d 2069 735f 6465 7461 696c  :param is_detail
+00040f20: 5f72 6573 756c 743a 2062 6f6f 6c2c 2064  _result: bool, d
+00040f30: 6566 6175 6c74 2046 616c 7365 2e0d 0a20  efault False... 
+00040f40: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+00040f50: 7061 7261 6d20 7072 6f66 6573 7369 6f6e  param profession
+00040f60: 616c 5f66 6965 6c64 3a20 7374 722c 2073  al_field: str, s
+00040f70: 7570 706f 7274 2061 6c69 6261 6261 2829  upport alibaba()
+00040f80: 2c20 6261 6964 7528 292c 2063 6169 7975  , baidu(), caiyu
+00040f90: 6e28 292c 2063 6c6f 7564 5969 2829 2c20  n(), cloudYi(), 
+00040fa0: 656c 6961 2829 2c20 7379 7354 7261 6e28  elia(), sysTran(
+00040fb0: 292c 2079 6f75 6461 6f28 292c 2076 6f6c  ), youdao(), vol
+00040fc0: 6345 6e67 696e 6528 2920 6f6e 6c79 2e0d  cEngine() only..
+00040fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00040fe0: 203a 7061 7261 6d20 7469 6d65 6f75 743a   :param timeout:
+00040ff0: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
+00041000: 4e6f 6e65 2e0d 0a20 2020 2020 2020 2020  None...         
+00041010: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
+00041020: 6f78 6965 733a 2064 6963 742c 2064 6566  oxies: dict, def
+00041030: 6175 6c74 204e 6f6e 652e 0d0a 2020 2020  ault None...    
+00041040: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00041050: 616d 2073 6c65 6570 5f73 6563 6f6e 6473  am sleep_seconds
+00041060: 3a20 666c 6f61 742c 2064 6566 6175 6c74  : float, default
+00041070: 2030 2e0d 0a20 2020 2020 2020 2020 2020   0...           
+00041080: 2020 2020 203a 7061 7261 6d20 7570 6461       :param upda
+00041090: 7465 5f73 6573 7369 6f6e 5f61 6674 6572  te_session_after
+000410a0: 5f66 7265 713a 2069 6e74 2c20 6465 6661  _freq: int, defa
+000410b0: 756c 7420 3130 3030 2e0d 0a20 2020 2020  ult 1000...     
+000410c0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+000410d0: 6d20 7570 6461 7465 5f73 6573 7369 6f6e  m update_session
+000410e0: 5f61 6674 6572 5f73 6563 6f6e 6473 3a20  _after_seconds: 
+000410f0: 666c 6f61 742c 2064 6566 6175 6c74 2031  float, default 1
+00041100: 3530 302e 0d0a 2020 2020 2020 2020 2020  500...          
+00041110: 2020 2020 2020 3a70 6172 616d 2069 665f        :param if_
+00041120: 7573 655f 636e 5f68 6f73 743a 2062 6f6f  use_cn_host: boo
+00041130: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+00041140: 2e20 5375 7070 6f72 7420 676f 6f67 6c65  . Support google
+00041150: 2829 2c20 6269 6e67 2829 206f 6e6c 792e  (), bing() only.
+00041160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00041170: 2020 3a70 6172 616d 2072 6573 6574 5f68    :param reset_h
+00041180: 6f73 745f 7572 6c3a 2073 7472 2c20 6465  ost_url: str, de
+00041190: 6661 756c 7420 4e6f 6e65 2e20 5375 7070  fault None. Supp
+000411a0: 6f72 7420 676f 6f67 6c65 2829 2c20 6172  ort google(), ar
+000411b0: 676f 7328 292c 2079 616e 6465 7828 2920  gos(), yandex() 
+000411c0: 6f6e 6c79 2e0d 0a20 2020 2020 2020 2020  only...         
+000411d0: 2020 2020 2020 203a 7061 7261 6d20 6966         :param if
+000411e0: 5f63 6865 636b 5f72 6573 6574 5f68 6f73  _check_reset_hos
+000411f0: 745f 7572 6c3a 2062 6f6f 6c2c 2064 6566  t_url: bool, def
+00041200: 6175 6c74 2054 7275 652e 2053 7570 706f  ault True. Suppo
+00041210: 7274 2067 6f6f 676c 6528 292c 2079 616e  rt google(), yan
+00041220: 6465 7828 2920 6f6e 6c79 2e0d 0a20 2020  dex() only...   
+00041230: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+00041240: 7261 6d20 6966 5f69 676e 6f72 655f 656d  ram if_ignore_em
+00041250: 7074 795f 7175 6572 793a 2062 6f6f 6c2c  pty_query: bool,
+00041260: 2064 6566 6175 6c74 2046 616c 7365 2e0d   default False..
+00041270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00041280: 203a 7061 7261 6d20 6966 5f69 676e 6f72   :param if_ignor
+00041290: 655f 6c69 6d69 745f 6f66 5f6c 656e 6774  e_limit_of_lengt
+000412a0: 683a 2062 6f6f 6c2c 2064 6566 6175 6c74  h: bool, default
+000412b0: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
+000412c0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+000412d0: 6c69 6d69 745f 6f66 5f6c 656e 6774 683a  limit_of_length:
+000412e0: 2069 6e74 2c20 6465 6661 756c 7420 3230   int, default 20
+000412f0: 3030 302e 0d0a 2020 2020 2020 2020 2020  000...          
+00041300: 2020 2020 2020 3a70 6172 616d 2069 665f        :param if_
+00041310: 7368 6f77 5f74 696d 655f 7374 6174 3a20  show_time_stat: 
+00041320: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+00041330: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
+00041340: 2020 2020 2020 3a70 6172 616d 2073 686f        :param sho
+00041350: 775f 7469 6d65 5f73 7461 745f 7072 6563  w_time_stat_prec
+00041360: 6973 696f 6e3a 2069 6e74 2c20 6465 6661  ision: int, defa
+00041370: 756c 7420 322e 0d0a 2020 2020 2020 2020  ult 2...        
+00041380: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+00041390: 665f 7072 696e 745f 7761 726e 696e 673a  f_print_warning:
+000413a0: 2062 6f6f 6c2c 2064 6566 6175 6c74 2054   bool, default T
+000413b0: 7275 652e 0d0a 2020 2020 2020 2020 2020  rue...          
+000413c0: 2020 2020 2020 3a70 6172 616d 206c 696e        :param lin
+000413d0: 6776 616e 6578 5f6d 6f64 656c 3a20 7374  gvanex_model: st
+000413e0: 722c 2064 6566 6175 6c74 2027 4232 4327  r, default 'B2C'
+000413f0: 2c20 6368 6f6f 7365 2066 726f 6d20 2822  , choose from ("
+00041400: 4232 4322 2c20 2242 3242 2229 2e0d 0a20  B2C", "B2B")... 
+00041410: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+00041420: 7061 7261 6d20 6d79 4d65 6d6f 7279 5f6d  param myMemory_m
+00041430: 6f64 653a 2073 7472 2c20 6465 6661 756c  ode: str, defaul
+00041440: 7420 2277 6562 222c 2063 686f 6f73 6520  t "web", choose 
+00041450: 6672 6f6d 2028 2277 6562 222c 2022 6170  from ("web", "ap
+00041460: 6922 292e 0d0a 2020 2020 2020 2020 3a72  i")...        :r
+00041470: 6574 7572 6e3a 2073 7472 206f 7220 6469  eturn: str or di
+00041480: 6374 0d0a 2020 2020 2020 2020 2222 220d  ct..        """.
+00041490: 0a0d 0a20 2020 2020 2020 2069 6620 7472  ...        if tr
+000414a0: 616e 736c 6174 6f72 206e 6f74 2069 6e20  anslator not in 
+000414b0: 7365 6c66 2e74 7261 6e73 6c61 746f 7273  self.translators
+000414c0: 5f70 6f6f 6c3a 0d0a 2020 2020 2020 2020  _pool:..        
+000414d0: 2020 2020 7261 6973 6520 5472 616e 736c      raise Transl
+000414e0: 6174 6f72 4572 726f 720d 0a0d 0a20 2020  atorError....   
+000414f0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00041500: 2e70 7265 5f61 6363 656c 6572 6174 696f  .pre_acceleratio
+00041510: 6e5f 6c61 6265 6c20 616e 6420 6966 5f75  n_label and if_u
+00041520: 7365 5f70 7265 6163 6365 6c65 7261 7469  se_preaccelerati
+00041530: 6f6e 3a0d 0a20 2020 2020 2020 2020 2020  on:..           
+00041540: 205f 203d 2073 656c 662e 7072 6561 6363   _ = self.preacc
+00041550: 656c 6572 6174 6528 290d 0a0d 0a20 2020  elerate()....   
+00041560: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00041570: 2e74 7261 6e73 6c61 746f 7273 5f64 6963  .translators_dic
+00041580: 745b 7472 616e 736c 6174 6f72 5d28 7175  t[translator](qu
+00041590: 6572 795f 7465 7874 3d71 7565 7279 5f74  ery_text=query_t
+000415a0: 6578 742c 2066 726f 6d5f 6c61 6e67 7561  ext, from_langua
+000415b0: 6765 3d66 726f 6d5f 6c61 6e67 7561 6765  ge=from_language
+000415c0: 2c20 746f 5f6c 616e 6775 6167 653d 746f  , to_language=to
+000415d0: 5f6c 616e 6775 6167 652c 202a 2a6b 7761  _language, **kwa
+000415e0: 7267 7329 0d0a 0d0a 2020 2020 6465 6620  rgs)....    def 
+000415f0: 7472 616e 736c 6174 655f 6874 6d6c 2873  translate_html(s
+00041600: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
+00041610: 2020 2020 2020 2020 2020 2020 2068 746d               htm
+00041620: 6c5f 7465 7874 3a20 7374 722c 0d0a 2020  l_text: str,..  
+00041630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00041640: 2020 2020 2074 7261 6e73 6c61 746f 723a       translator:
+00041650: 2073 7472 203d 2027 6269 6e67 272c 0d0a   str = 'bing',..
+00041660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00041670: 2020 2020 2020 2066 726f 6d5f 6c61 6e67         from_lang
+00041680: 7561 6765 3a20 7374 7220 3d20 2761 7574  uage: str = 'aut
+00041690: 6f27 2c0d 0a20 2020 2020 2020 2020 2020  o',..           
+000416a0: 2020 2020 2020 2020 2020 2020 746f 5f6c              to_l
+000416b0: 616e 6775 6167 653a 2073 7472 203d 2027  anguage: str = '
+000416c0: 656e 272c 0d0a 2020 2020 2020 2020 2020  en',..          
+000416d0: 2020 2020 2020 2020 2020 2020 206e 5f6a               n_j
+000416e0: 6f62 733a 2069 6e74 203d 202d 312c 0d0a  obs: int = -1,..
+000416f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00041700: 2020 2020 2020 2069 665f 7573 655f 7072         if_use_pr
+00041710: 6561 6363 656c 6572 6174 696f 6e3a 2062  eacceleration: b
+00041720: 6f6f 6c20 3d20 4661 6c73 652c 0d0a 2020  ool = False,..  
+00041730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00041740: 2020 2020 202a 2a6b 7761 7267 733a 2041       **kwargs: A
+00041750: 7069 4b77 6172 6773 5479 7065 2c0d 0a20  piKwargsType,.. 
+00041760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00041770: 2020 2020 2020 2920 2d3e 2073 7472 3a0d        ) -> str:.
+00041780: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00041790: 2020 2020 2020 5472 616e 736c 6174 6520        Translate 
+000417a0: 7468 6520 6469 7370 6c61 7965 6420 636f  the displayed co
+000417b0: 6e74 656e 7420 6f66 2068 746d 6c20 7769  ntent of html wi
+000417c0: 7468 6f75 7420 6368 616e 6769 6e67 2074  thout changing t
+000417d0: 6865 2068 746d 6c20 7374 7275 6374 7572  he html structur
+000417e0: 652e 0d0a 2020 2020 2020 2020 3a70 6172  e...        :par
+000417f0: 616d 2068 746d 6c5f 7465 7874 3a20 7374  am html_text: st
+00041800: 722c 206d 7573 742e 0d0a 2020 2020 2020  r, must...      
+00041810: 2020 3a70 6172 616d 2074 7261 6e73 6c61    :param transla
+00041820: 746f 723a 2073 7472 2c20 6465 6661 756c  tor: str, defaul
+00041830: 7420 2762 696e 6727 2e0d 0a20 2020 2020  t 'bing'...     
+00041840: 2020 203a 7061 7261 6d20 6672 6f6d 5f6c     :param from_l
+00041850: 616e 6775 6167 653a 2073 7472 2c20 6465  anguage: str, de
+00041860: 6661 756c 7420 2761 7574 6f27 2e0d 0a20  fault 'auto'... 
+00041870: 2020 2020 2020 203a 7061 7261 6d20 746f         :param to
+00041880: 5f6c 616e 6775 6167 653a 2073 7472 2c20  _language: str, 
+00041890: 6465 6661 756c 7420 2765 6e27 2e0d 0a20  default 'en'... 
+000418a0: 2020 2020 2020 203a 7061 7261 6d20 6e5f         :param n_
+000418b0: 6a6f 6273 3a20 696e 742c 2064 6566 6175  jobs: int, defau
+000418c0: 6c74 202d 312c 206d 6561 6e73 206f 732e  lt -1, means os.
+000418d0: 6370 755f 636e 7428 292e 0d0a 2020 2020  cpu_cnt()...    
+000418e0: 2020 2020 3a70 6172 616d 2069 665f 7573      :param if_us
+000418f0: 655f 7072 6561 6363 656c 6572 6174 696f  e_preacceleratio
+00041900: 6e3a 2062 6f6f 6c2c 2064 6566 6175 6c74  n: bool, default
+00041910: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
+00041920: 203a 7061 7261 6d20 2a2a 6b77 6172 6773   :param **kwargs
+00041930: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00041940: 2020 203a 7061 7261 6d20 6973 5f64 6574     :param is_det
+00041950: 6169 6c5f 7265 7375 6c74 3a20 626f 6f6c  ail_result: bool
+00041960: 2c20 6465 6661 756c 7420 4661 6c73 652e  , default False.
+00041970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00041980: 2020 3a70 6172 616d 2070 726f 6665 7373    :param profess
+00041990: 696f 6e61 6c5f 6669 656c 643a 2073 7472  ional_field: str
+000419a0: 2c20 7375 7070 6f72 7420 616c 6962 6162  , support alibab
+000419b0: 6128 292c 2062 6169 6475 2829 2c20 6361  a(), baidu(), ca
+000419c0: 6979 756e 2829 2c20 636c 6f75 6459 6928  iyun(), cloudYi(
+000419d0: 292c 2065 6c69 6128 292c 2073 7973 5472  ), elia(), sysTr
+000419e0: 616e 2829 2c20 796f 7564 616f 2829 2c20  an(), youdao(), 
+000419f0: 766f 6c63 456e 6769 6e65 2829 206f 6e6c  volcEngine() onl
+00041a00: 792e 0d0a 2020 2020 2020 2020 2020 2020  y...            
+00041a10: 2020 2020 3a70 6172 616d 2074 696d 656f      :param timeo
+00041a20: 7574 3a20 666c 6f61 742c 2064 6566 6175  ut: float, defau
+00041a30: 6c74 204e 6f6e 652e 0d0a 2020 2020 2020  lt None...      
+00041a40: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+00041a50: 2070 726f 7869 6573 3a20 6469 6374 2c20   proxies: dict, 
+00041a60: 6465 6661 756c 7420 4e6f 6e65 2e0d 0a20  default None... 
+00041a70: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+00041a80: 7061 7261 6d20 736c 6565 705f 7365 636f  param sleep_seco
+00041a90: 6e64 733a 2066 6c6f 6174 2c20 6465 6661  nds: float, defa
+00041aa0: 756c 7420 302e 0d0a 2020 2020 2020 2020  ult 0...        
+00041ab0: 2020 2020 2020 2020 3a70 6172 616d 2075          :param u
+00041ac0: 7064 6174 655f 7365 7373 696f 6e5f 6166  pdate_session_af
+00041ad0: 7465 725f 6672 6571 3a20 696e 742c 2064  ter_freq: int, d
+00041ae0: 6566 6175 6c74 2031 3030 302e 0d0a 2020  efault 1000...  
+00041af0: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+00041b00: 6172 616d 2075 7064 6174 655f 7365 7373  aram update_sess
+00041b10: 696f 6e5f 6166 7465 725f 7365 636f 6e64  ion_after_second
+00041b20: 733a 2066 6c6f 6174 2c20 6465 6661 756c  s: float, defaul
+00041b30: 7420 3135 3030 2e0d 0a20 2020 2020 2020  t 1500...       
+00041b40: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00041b50: 6966 5f75 7365 5f63 6e5f 686f 7374 3a20  if_use_cn_host: 
+00041b60: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+00041b70: 6c73 652e 2053 7570 706f 7274 2067 6f6f  lse. Support goo
+00041b80: 676c 6528 292c 2062 696e 6728 2920 6f6e  gle(), bing() on
+00041b90: 6c79 2e0d 0a20 2020 2020 2020 2020 2020  ly...           
+00041ba0: 2020 2020 203a 7061 7261 6d20 7265 7365       :param rese
+00041bb0: 745f 686f 7374 5f75 726c 3a20 7374 722c  t_host_url: str,
+00041bc0: 2064 6566 6175 6c74 204e 6f6e 652e 2053   default None. S
+00041bd0: 7570 706f 7274 2067 6f6f 676c 6528 292c  upport google(),
+00041be0: 2061 7267 6f73 2829 2c20 7961 6e64 6578   argos(), yandex
+00041bf0: 2829 206f 6e6c 792e 0d0a 2020 2020 2020  () only...      
+00041c00: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+00041c10: 2069 665f 6368 6563 6b5f 7265 7365 745f   if_check_reset_
+00041c20: 686f 7374 5f75 726c 3a20 626f 6f6c 2c20  host_url: bool, 
+00041c30: 6465 6661 756c 7420 5472 7565 2e20 5375  default True. Su
+00041c40: 7070 6f72 7420 676f 6f67 6c65 2829 2c20  pport google(), 
+00041c50: 7961 6e64 6578 2829 206f 6e6c 792e 0d0a  yandex() only...
+00041c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00041c70: 3a70 6172 616d 2069 665f 6967 6e6f 7265  :param if_ignore
+00041c80: 5f65 6d70 7479 5f71 7565 7279 3a20 626f  _empty_query: bo
+00041c90: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
+00041ca0: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
+00041cb0: 2020 2020 3a70 6172 616d 2069 665f 6967      :param if_ig
+00041cc0: 6e6f 7265 5f6c 696d 6974 5f6f 665f 6c65  nore_limit_of_le
+00041cd0: 6e67 7468 3a20 626f 6f6c 2c20 6465 6661  ngth: bool, defa
+00041ce0: 756c 7420 4661 6c73 652e 0d0a 2020 2020  ult False...    
+00041cf0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00041d00: 616d 206c 696d 6974 5f6f 665f 6c65 6e67  am limit_of_leng
+00041d10: 7468 3a20 696e 742c 2064 6566 6175 6c74  th: int, default
+00041d20: 2032 3030 3030 2e0d 0a20 2020 2020 2020   20000...       
+00041d30: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00041d40: 6966 5f73 686f 775f 7469 6d65 5f73 7461  if_show_time_sta
+00041d50: 743a 2062 6f6f 6c2c 2064 6566 6175 6c74  t: bool, default
+00041d60: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
+00041d70: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00041d80: 7368 6f77 5f74 696d 655f 7374 6174 5f70  show_time_stat_p
+00041d90: 7265 6369 7369 6f6e 3a20 696e 742c 2064  recision: int, d
+00041da0: 6566 6175 6c74 2032 2e0d 0a20 2020 2020  efault 2...     
+00041db0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00041dc0: 6d20 6966 5f70 7269 6e74 5f77 6172 6e69  m if_print_warni
+00041dd0: 6e67 3a20 626f 6f6c 2c20 6465 6661 756c  ng: bool, defaul
+00041de0: 7420 5472 7565 2e0d 0a20 2020 2020 2020  t True...       
+00041df0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00041e00: 6c69 6e67 7661 6e65 785f 6d6f 6465 6c3a  lingvanex_model:
+00041e10: 2073 7472 2c20 6465 6661 756c 7420 2742   str, default 'B
+00041e20: 3243 272c 2063 686f 6f73 6520 6672 6f6d  2C', choose from
+00041e30: 2028 2242 3243 222c 2022 4232 4222 292e   ("B2C", "B2B").
+00041e40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00041e50: 2020 3a70 6172 616d 206d 794d 656d 6f72    :param myMemor
+00041e60: 795f 6d6f 6465 3a20 7374 722c 2064 6566  y_mode: str, def
+00041e70: 6175 6c74 2022 7765 6222 2c20 6368 6f6f  ault "web", choo
+00041e80: 7365 2066 726f 6d20 2822 7765 6222 2c20  se from ("web", 
+00041e90: 2261 7069 2229 2e0d 0a20 2020 2020 2020  "api")...       
+00041ea0: 203a 7265 7475 726e 3a20 7374 720d 0a20   :return: str.. 
+00041eb0: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
+00041ec0: 2020 2020 2020 6966 2074 7261 6e73 6c61        if transla
+00041ed0: 746f 7220 6e6f 7420 696e 2073 656c 662e  tor not in self.
+00041ee0: 7472 616e 736c 6174 6f72 735f 706f 6f6c  translators_pool
+00041ef0: 206f 7220 6b77 6172 6773 2e67 6574 2827   or kwargs.get('
+00041f00: 6973 5f64 6574 6169 6c5f 7265 7375 6c74  is_detail_result
+00041f10: 272c 2046 616c 7365 2920 6f72 206e 5f6a  ', False) or n_j
+00041f20: 6f62 7320 3e20 7365 6c66 2e63 7075 5f63  obs > self.cpu_c
+00041f30: 6e74 3a0d 0a20 2020 2020 2020 2020 2020  nt:..           
+00041f40: 2072 6169 7365 2054 7261 6e73 6c61 746f   raise Translato
+00041f50: 7245 7272 6f72 0d0a 0d0a 2020 2020 2020  rError....      
+00041f60: 2020 6966 206e 6f74 2073 656c 662e 7072    if not self.pr
+00041f70: 655f 6163 6365 6c65 7261 7469 6f6e 5f6c  e_acceleration_l
+00041f80: 6162 656c 2061 6e64 2069 665f 7573 655f  abel and if_use_
+00041f90: 7072 6561 6363 656c 6572 6174 696f 6e3a  preacceleration:
+00041fa0: 0d0a 2020 2020 2020 2020 2020 2020 5f20  ..            _ 
+00041fb0: 3d20 7365 6c66 2e70 7265 6163 6365 6c65  = self.preaccele
+00041fc0: 7261 7465 2829 0d0a 0d0a 2020 2020 2020  rate()....      
+00041fd0: 2020 6465 6620 5f74 7261 6e73 6c61 7465    def _translate
+00041fe0: 5f74 6578 7428 7365 6e74 656e 6365 3a20  _text(sentence: 
+00041ff0: 7374 7229 202d 3e20 5475 706c 655b 7374  str) -> Tuple[st
+00042000: 722c 2073 7472 5d3a 0d0a 2020 2020 2020  r, str]:..      
+00042010: 2020 2020 2020 7265 7475 726e 2073 656e        return sen
+00042020: 7465 6e63 652c 2073 656c 662e 7472 616e  tence, self.tran
+00042030: 736c 6174 6f72 735f 6469 6374 5b74 7261  slators_dict[tra
+00042040: 6e73 6c61 746f 725d 2871 7565 7279 5f74  nslator](query_t
+00042050: 6578 743d 7365 6e74 656e 6365 2c20 6672  ext=sentence, fr
+00042060: 6f6d 5f6c 616e 6775 6167 653d 6672 6f6d  om_language=from
+00042070: 5f6c 616e 6775 6167 652c 2074 6f5f 6c61  _language, to_la
+00042080: 6e67 7561 6765 3d74 6f5f 6c61 6e67 7561  nguage=to_langua
+00042090: 6765 2c20 2a2a 6b77 6172 6773 290d 0a0d  ge, **kwargs)...
+000420a0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
+000420b0: 203d 2072 652e 636f 6d70 696c 6528 2228   = re.compile("(
+000420c0: 3f3a 5e7c 283f 3c3d 3e29 2928 5b5c 5c73  ?:^|(?<=>))([\\s
+000420d0: 5c5c 535d 2a3f 2928 3f3a 283f 3d3c 297c  \\S]*?)(?:(?=<)|
+000420e0: 2429 2229 2020 2320 544f 444f 3a20 3c63  $)")  # TODO: <c
+000420f0: 6f64 653e 3c2f 636f 6465 3e20 3c64 6976  ode></code> <div
+00042100: 2063 6c61 7373 3d22 636f 6465 7465 7874   class="codetext
+00042110: 206e 6f74 7261 6e73 6c61 7465 223e 0d0a   notranslate">..
+00042120: 2020 2020 2020 2020 7365 6e74 656e 6365          sentence
+00042130: 5f6c 6973 7420 3d20 6c69 7374 2873 6574  _list = list(set
+00042140: 2870 6174 7465 726e 2e66 696e 6461 6c6c  (pattern.findall
+00042150: 2868 746d 6c5f 7465 7874 2929 290d 0a0d  (html_text)))...
+00042160: 0a20 2020 2020 2020 206e 5f6a 6f62 7320  .        n_jobs 
+00042170: 3d20 7365 6c66 2e63 7075 5f63 6e74 2069  = self.cpu_cnt i
+00042180: 6620 6e5f 6a6f 6273 203c 3d20 3020 656c  f n_jobs <= 0 el
+00042190: 7365 206e 5f6a 6f62 730d 0a20 2020 2020  se n_jobs..     
+000421a0: 2020 2077 6974 6820 7061 7468 6f73 2e6d     with pathos.m
+000421b0: 756c 7469 7072 6f63 6573 7369 6e67 2e50  ultiprocessing.P
+000421c0: 726f 6365 7373 506f 6f6c 286e 5f6a 6f62  rocessPool(n_job
+000421d0: 7329 2061 7320 706f 6f6c 3a0d 0a20 2020  s) as pool:..   
+000421e0: 2020 2020 2020 2020 2072 6573 756c 745f           result_
+000421f0: 6c69 7374 203d 2070 6f6f 6c2e 6d61 7028  list = pool.map(
+00042200: 5f74 7261 6e73 6c61 7465 5f74 6578 742c  _translate_text,
+00042210: 2073 656e 7465 6e63 655f 6c69 7374 290d   sentence_list).
+00042220: 0a0d 0a20 2020 2020 2020 2072 6573 756c  ...        resul
+00042230: 745f 6469 6374 203d 207b 7465 7874 3a20  t_dict = {text: 
+00042240: 7473 5f74 6578 7420 666f 7220 7465 7874  ts_text for text
+00042250: 2c20 7473 5f74 6578 7420 696e 2072 6573  , ts_text in res
+00042260: 756c 745f 6c69 7374 7d0d 0a20 2020 2020  ult_list}..     
+00042270: 2020 205f 6765 745f 7265 7375 6c74 5f66     _get_result_f
+00042280: 756e 6320 3d20 6c61 6d62 6461 206b 3a20  unc = lambda k: 
+00042290: 7265 7375 6c74 5f64 6963 742e 6765 7428  result_dict.get(
+000422a0: 6b2e 6772 6f75 7028 3129 2c20 2727 290d  k.group(1), '').
+000422b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000422c0: 7061 7474 6572 6e2e 7375 6228 7265 706c  pattern.sub(repl
+000422d0: 3d5f 6765 745f 7265 7375 6c74 5f66 756e  =_get_result_fun
+000422e0: 632c 2073 7472 696e 673d 6874 6d6c 5f74  c, string=html_t
+000422f0: 6578 7429 0d0a 0d0a 2020 2020 6465 6620  ext)....    def 
+00042300: 5f74 6573 745f 7472 616e 736c 6174 6528  _test_translate(
+00042310: 7365 6c66 2c20 5f74 733a 2073 7472 2c20  self, _ts: str, 
+00042320: 7469 6d65 6f75 743a 204f 7074 696f 6e61  timeout: Optiona
+00042330: 6c5b 666c 6f61 745d 203d 204e 6f6e 652c  l[float] = None,
+00042340: 2069 665f 7368 6f77 5f74 696d 655f 7374   if_show_time_st
+00042350: 6174 3a20 626f 6f6c 203d 2046 616c 7365  at: bool = False
+00042360: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+00042370: 2020 2066 726f 6d5f 6c61 6e67 7561 6765     from_language
+00042380: 203d 2073 656c 662e 6e6f 745f 7a68 5f6c   = self.not_zh_l
+00042390: 616e 6773 5b5f 7473 5d20 6966 205f 7473  angs[_ts] if _ts
+000423a0: 2069 6e20 7365 6c66 2e6e 6f74 5f7a 685f   in self.not_zh_
+000423b0: 6c61 6e67 7320 656c 7365 2027 6175 746f  langs else 'auto
+000423c0: 270d 0a20 2020 2020 2020 2074 6f5f 6c61  '..        to_la
+000423d0: 6e67 7561 6765 203d 2073 656c 662e 6e6f  nguage = self.no
+000423e0: 745f 656e 5f6c 616e 6773 5b5f 7473 5d20  t_en_langs[_ts] 
+000423f0: 6966 205f 7473 2069 6e20 7365 6c66 2e6e  if _ts in self.n
+00042400: 6f74 5f65 6e5f 6c61 6e67 7320 656c 7365  ot_en_langs else
+00042410: 2027 656e 270d 0a20 2020 2020 2020 2072   'en'..        r
+00042420: 6573 756c 7420 3d20 7365 6c66 2e74 7261  esult = self.tra
+00042430: 6e73 6c61 746f 7273 5f64 6963 745b 5f74  nslators_dict[_t
+00042440: 735d 280d 0a20 2020 2020 2020 2020 2020  s](..           
+00042450: 2071 7565 7279 5f74 6578 743d 7365 6c66   query_text=self
+00042460: 2e65 7861 6d70 6c65 5f71 7565 7279 5f74  .example_query_t
+00042470: 6578 742c 0d0a 2020 2020 2020 2020 2020  ext,..          
+00042480: 2020 7472 616e 736c 6174 6f72 3d5f 7473    translator=_ts
+00042490: 2c0d 0a20 2020 2020 2020 2020 2020 2066  ,..            f
+000424a0: 726f 6d5f 6c61 6e67 7561 6765 3d66 726f  rom_language=fro
+000424b0: 6d5f 6c61 6e67 7561 6765 2c0d 0a20 2020  m_language,..   
+000424c0: 2020 2020 2020 2020 2074 6f5f 6c61 6e67           to_lang
+000424d0: 7561 6765 3d74 6f5f 6c61 6e67 7561 6765  uage=to_language
+000424e0: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
+000424f0: 665f 7072 696e 745f 7761 726e 696e 673d  f_print_warning=
+00042500: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00042510: 2020 2020 7469 6d65 6f75 743d 7469 6d65      timeout=time
+00042520: 6f75 742c 0d0a 2020 2020 2020 2020 2020  out,..          
+00042530: 2020 6966 5f73 686f 775f 7469 6d65 5f73    if_show_time_s
+00042540: 7461 743d 6966 5f73 686f 775f 7469 6d65  tat=if_show_time
+00042550: 5f73 7461 740d 0a20 2020 2020 2020 2029  _stat..        )
+00042560: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00042570: 2072 6573 756c 740d 0a0d 0a20 2020 2064   result....    d
+00042580: 6566 2070 7265 6163 6365 6c65 7261 7465  ef preaccelerate
+00042590: 2873 656c 662c 2074 696d 656f 7574 3a20  (self, timeout: 
+000425a0: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d20  Optional[float] 
+000425b0: 3d20 4e6f 6e65 2c20 6966 5f73 686f 775f  = None, if_show_
+000425c0: 7469 6d65 5f73 7461 743a 2062 6f6f 6c20  time_stat: bool 
+000425d0: 3d20 5472 7565 2c20 2a2a 6b77 6172 6773  = True, **kwargs
+000425e0: 3a20 7374 7229 202d 3e20 6469 6374 3a0d  : str) -> dict:.
+000425f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00042600: 2e70 7265 5f61 6363 656c 6572 6174 696f  .pre_acceleratio
+00042610: 6e5f 6c61 6265 6c20 3e20 303a 0d0a 2020  n_label > 0:..  
+00042620: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00042630: 5472 616e 736c 6174 6f72 4572 726f 7228  TranslatorError(
+00042640: 2750 7265 6163 6365 6c65 7261 7469 6f6e  'Preacceleration
+00042650: 2063 616e 206f 6e6c 7920 6265 2070 6572   can only be per
+00042660: 666f 726d 6564 206f 6e63 652e 2729 0d0a  formed once.')..
+00042670: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
+00042680: 7861 6d70 6c65 5f71 7565 7279 5f74 6578  xample_query_tex
+00042690: 7420 3d20 6b77 6172 6773 2e67 6574 2827  t = kwargs.get('
+000426a0: 6578 616d 706c 655f 7175 6572 795f 7465  example_query_te
+000426b0: 7874 272c 2073 656c 662e 6578 616d 706c  xt', self.exampl
+000426c0: 655f 7175 6572 795f 7465 7874 290d 0a0d  e_query_text)...
+000426d0: 0a20 2020 2020 2020 2073 7973 2e73 7464  .        sys.std
+000426e0: 6572 722e 7772 6974 6528 2750 7265 6163  err.write('Preac
+000426f0: 6365 6c65 7261 7469 6f6e 2d50 726f 6365  celeration-Proce
+00042700: 7373 2077 696c 6c20 7461 6b65 2061 2066  ss will take a f
+00042710: 6577 206d 696e 7574 6573 2e5c 6e27 290d  ew minutes.\n').
+00042720: 0a20 2020 2020 2020 2073 7973 2e73 7464  .        sys.std
+00042730: 6572 722e 7772 6974 6528 2754 6970 733a  err.write('Tips:
+00042740: 2054 6865 2073 6d61 6c6c 6572 2060 7469   The smaller `ti
+00042750: 6d65 6f75 7460 2076 616c 7565 2c20 7468  meout` value, th
+00042760: 6520 6665 7765 7220 7472 616e 736c 6174  e fewer translat
+00042770: 6f72 7320 7061 7373 2074 6865 2074 6573  ors pass the tes
+00042780: 7420 270d 0a20 2020 2020 2020 2020 2020  t '..           
+00042790: 2020 2020 2020 2020 2020 2020 2020 2761                'a
+000427a0: 6e64 2074 6865 206c 6573 7320 7469 6d65  nd the less time
+000427b0: 2069 7420 7461 6b65 7320 746f 2070 7265   it takes to pre
+000427c0: 6163 6365 6c65 7261 7465 2e20 486f 7765  accelerate. Howe
+000427d0: 7665 722c 2074 6865 2073 6c6f 7720 7370  ver, the slow sp
+000427e0: 6565 6420 6f66 2027 0d0a 2020 2020 2020  eed of '..      
+000427f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00042800: 2020 2027 7072 6561 6363 656c 6572 6174     'preaccelerat
+00042810: 696f 6e20 646f 6573 206e 6f74 206d 6561  ion does not mea
+00042820: 6e20 7468 6520 736c 6f77 2073 7065 6564  n the slow speed
+00042830: 206f 6620 6c61 7465 7220 7472 616e 736c   of later transl
+00042840: 6174 696f 6e2e 5c6e 5c6e 2729 0d0a 0d0a  ation.\n\n')....
+00042850: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00042860: 2074 7164 6d2e 7471 646d 2872 616e 6765   tqdm.tqdm(range
+00042870: 286c 656e 2873 656c 662e 7472 616e 736c  (len(self.transl
+00042880: 6174 6f72 735f 706f 6f6c 2929 2c20 6465  ators_pool)), de
+00042890: 7363 3d27 5072 6561 6363 656c 6572 6174  sc='Preaccelerat
+000428a0: 696f 6e20 5072 6f63 6573 7327 2c20 6e63  ion Process', nc
+000428b0: 6f6c 733d 3830 293a 0d0a 2020 2020 2020  ols=80):..      
+000428c0: 2020 2020 2020 5f74 7320 3d20 7365 6c66        _ts = self
+000428d0: 2e74 7261 6e73 6c61 746f 7273 5f70 6f6f  .translators_poo
+000428e0: 6c5b 695d 0d0a 2020 2020 2020 2020 2020  l[i]..          
+000428f0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00042900: 2020 2020 2020 2020 5f20 3d20 7365 6c66          _ = self
+00042910: 2e5f 7465 7374 5f74 7261 6e73 6c61 7465  ._test_translate
+00042920: 285f 7473 2c20 7469 6d65 6f75 742c 2069  (_ts, timeout, i
+00042930: 665f 7368 6f77 5f74 696d 655f 7374 6174  f_show_time_stat
+00042940: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00042950: 2020 2073 656c 662e 7375 6363 6573 735f     self.success_
+00042960: 7472 616e 736c 6174 6f72 735f 706f 6f6c  translators_pool
+00042970: 2e61 7070 656e 6428 5f74 7329 0d0a 2020  .append(_ts)..  
+00042980: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00042990: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000429a0: 2020 2073 656c 662e 6661 696c 7572 655f     self.failure_
+000429b0: 7472 616e 736c 6174 6f72 735f 706f 6f6c  translators_pool
+000429c0: 2e61 7070 656e 6428 5f74 7329 0d0a 0d0a  .append(_ts)....
+000429d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000429e0: 2e70 7265 5f61 6363 656c 6572 6174 696f  .pre_acceleratio
+000429f0: 6e5f 6c61 6265 6c20 2b3d 2031 0d0a 2020  n_label += 1..  
+00042a00: 2020 2020 2020 7265 7475 726e 207b 2773        return {'s
+00042a10: 7563 6365 7373 273a 2073 656c 662e 7375  uccess': self.su
+00042a20: 6363 6573 735f 7472 616e 736c 6174 6f72  ccess_translator
+00042a30: 735f 706f 6f6c 2c20 2766 6169 6c75 7265  s_pool, 'failure
+00042a40: 273a 2073 656c 662e 6661 696c 7572 655f  ': self.failure_
+00042a50: 7472 616e 736c 6174 6f72 735f 706f 6f6c  translators_pool
+00042a60: 7d0d 0a0d 0a20 2020 2064 6566 2073 7065  }....    def spe
+00042a70: 6564 7465 7374 2873 656c 662c 202a 2a6b  edtest(self, **k
+00042a80: 7761 7267 733a 204c 6973 745b 7374 725d  wargs: List[str]
+00042a90: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+00042aa0: 2020 2020 6966 2073 656c 662e 7072 655f      if self.pre_
+00042ab0: 6163 6365 6c65 7261 7469 6f6e 5f6c 6162  acceleration_lab
+00042ac0: 656c 203c 2031 3a0d 0a20 2020 2020 2020  el < 1:..       
+00042ad0: 2020 2020 2072 6169 7365 2054 7261 6e73       raise Trans
+00042ae0: 6c61 746f 7245 7272 6f72 2827 5072 6561  latorError('Prea
+00042af0: 6363 656c 6572 6174 696f 6e20 6669 7273  cceleration firs
+00042b00: 742e 2729 0d0a 0d0a 2020 2020 2020 2020  t.')....        
+00042b10: 7465 7374 5f74 7261 6e73 6c61 746f 7273  test_translators
+00042b20: 5f70 6f6f 6c20 3d20 6b77 6172 6773 2e67  _pool = kwargs.g
+00042b30: 6574 2827 7465 7374 5f74 7261 6e73 6c61  et('test_transla
+00042b40: 746f 7273 5f70 6f6f 6c27 2c20 7365 6c66  tors_pool', self
+00042b50: 2e73 7563 6365 7373 5f74 7261 6e73 6c61  .success_transla
+00042b60: 746f 7273 5f70 6f6f 6c29 0d0a 0d0a 2020  tors_pool)....  
+00042b70: 2020 2020 2020 7379 732e 7374 6465 7272        sys.stderr
+00042b80: 2e77 7269 7465 2827 5370 6565 6454 6573  .write('SpeedTes
+00042b90: 742d 5072 6f63 6573 7320 7769 6c6c 2074  t-Process will t
+00042ba0: 616b 6520 6120 6665 7720 7365 636f 6e64  ake a few second
+00042bb0: 732e 5c6e 5c6e 2729 0d0a 2020 2020 2020  s.\n\n')..      
+00042bc0: 2020 666f 7220 6920 696e 2074 7164 6d2e    for i in tqdm.
+00042bd0: 7471 646d 2872 616e 6765 286c 656e 2874  tqdm(range(len(t
+00042be0: 6573 745f 7472 616e 736c 6174 6f72 735f  est_translators_
+00042bf0: 706f 6f6c 2929 2c20 6465 7363 3d27 5370  pool)), desc='Sp
+00042c00: 6565 6454 6573 7420 5072 6f63 6573 7327  eedTest Process'
+00042c10: 2c20 6e63 6f6c 733d 3830 293a 0d0a 2020  , ncols=80):..  
+00042c20: 2020 2020 2020 2020 2020 5f74 7320 3d20            _ts = 
+00042c30: 7465 7374 5f74 7261 6e73 6c61 746f 7273  test_translators
+00042c40: 5f70 6f6f 6c5b 695d 0d0a 2020 2020 2020  _pool[i]..      
+00042c50: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00042c60: 2020 2020 2020 2020 2020 2020 5f20 3d20              _ = 
+00042c70: 7365 6c66 2e5f 7465 7374 5f74 7261 6e73  self._test_trans
+00042c80: 6c61 7465 285f 7473 2c20 7469 6d65 6f75  late(_ts, timeou
+00042c90: 743d 4e6f 6e65 2c20 6966 5f73 686f 775f  t=None, if_show_
+00042ca0: 7469 6d65 5f73 7461 743d 5472 7565 290d  time_stat=True).
+00042cb0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00042cc0: 6570 743a 0d0a 2020 2020 2020 2020 2020  ept:..          
+00042cd0: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
+00042ce0: 2020 2020 7265 7475 726e 0d0a 0d0a 2020      return....  
+00042cf0: 2020 6465 6620 7072 6561 6363 656c 6572    def preacceler
+00042d00: 6174 655f 616e 645f 7370 6565 6474 6573  ate_and_speedtes
+00042d10: 7428 7365 6c66 2c20 7469 6d65 6f75 743a  t(self, timeout:
+00042d20: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
+00042d30: 203d 204e 6f6e 652c 202a 2a6b 7761 7267   = None, **kwarg
+00042d40: 733a 2073 7472 2920 2d3e 2064 6963 743a  s: str) -> dict:
+00042d50: 0d0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00042d60: 203d 2073 656c 662e 7072 6561 6363 656c   = self.preaccel
+00042d70: 6572 6174 6528 7469 6d65 6f75 743d 7469  erate(timeout=ti
+00042d80: 6d65 6f75 742c 202a 2a6b 7761 7267 7329  meout, **kwargs)
+00042d90: 0d0a 2020 2020 2020 2020 7379 732e 7374  ..        sys.st
+00042da0: 6465 7272 2e77 7269 7465 2827 5c6e 5c6e  derr.write('\n\n
+00042db0: 2729 0d0a 2020 2020 2020 2020 7365 6c66  ')..        self
+00042dc0: 2e73 7065 6564 7465 7374 2829 0d0a 2020  .speedtest()..  
+00042dd0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00042de0: 756c 740d 0a0d 0a0d 0a74 7373 203d 2054  ult......tss = T
+00042df0: 7261 6e73 6c61 746f 7273 5365 7276 6572  ranslatorsServer
+00042e00: 2829 0d0a 0d0a 5f61 6c69 6261 6261 203d  ()...._alibaba =
+00042e10: 2074 7373 2e5f 616c 6962 6162 610d 0a61   tss._alibaba..a
+00042e20: 6c69 6261 6261 203d 2074 7373 2e61 6c69  libaba = tss.ali
+00042e30: 6261 6261 0d0a 5f61 7065 7274 6975 6d20  baba.._apertium 
+00042e40: 3d20 7473 732e 5f61 7065 7274 6975 6d0d  = tss._apertium.
+00042e50: 0a61 7065 7274 6975 6d20 3d20 7473 732e  .apertium = tss.
+00042e60: 6170 6572 7469 756d 0d0a 5f61 7267 6f73  apertium.._argos
+00042e70: 203d 2074 7373 2e5f 6172 676f 730d 0a61   = tss._argos..a
+00042e80: 7267 6f73 203d 2074 7373 2e61 7267 6f73  rgos = tss.argos
+00042e90: 0d0a 5f62 6169 6475 203d 2074 7373 2e5f  .._baidu = tss._
+00042ea0: 6261 6964 750d 0a62 6169 6475 203d 2074  baidu..baidu = t
+00042eb0: 7373 2e62 6169 6475 0d0a 5f62 696e 6720  ss.baidu.._bing 
+00042ec0: 3d20 7473 732e 5f62 696e 670d 0a62 696e  = tss._bing..bin
+00042ed0: 6720 3d20 7473 732e 6269 6e67 0d0a 5f63  g = tss.bing.._c
+00042ee0: 6169 7975 6e20 3d20 7473 732e 5f63 6169  aiyun = tss._cai
+00042ef0: 7975 6e0d 0a63 6169 7975 6e20 3d20 7473  yun..caiyun = ts
+00042f00: 732e 6361 6979 756e 0d0a 5f63 6c6f 7564  s.caiyun.._cloud
+00042f10: 5969 203d 2074 7373 2e5f 636c 6f75 6459  Yi = tss._cloudY
+00042f20: 690d 0a63 6c6f 7564 5969 203d 2074 7373  i..cloudYi = tss
+00042f30: 2e63 6c6f 7564 5969 0d0a 5f64 6565 706c  .cloudYi.._deepl
+00042f40: 203d 2074 7373 2e5f 6465 6570 6c0d 0a64   = tss._deepl..d
+00042f50: 6565 706c 203d 2074 7373 2e64 6565 706c  eepl = tss.deepl
+00042f60: 0d0a 5f65 6c69 6120 3d20 7473 732e 5f65  .._elia = tss._e
+00042f70: 6c69 610d 0a65 6c69 6120 3d20 7473 732e  lia..elia = tss.
+00042f80: 656c 6961 0d0a 5f67 6f6f 676c 6520 3d20  elia.._google = 
+00042f90: 7473 732e 5f67 6f6f 676c 650d 0a67 6f6f  tss._google..goo
+00042fa0: 676c 6520 3d20 7473 732e 676f 6f67 6c65  gle = tss.google
+00042fb0: 0d0a 5f69 6369 6261 203d 2074 7373 2e5f  .._iciba = tss._
+00042fc0: 6963 6962 610d 0a69 6369 6261 203d 2074  iciba..iciba = t
+00042fd0: 7373 2e69 6369 6261 0d0a 5f69 666c 7974  ss.iciba.._iflyt
+00042fe0: 656b 203d 2074 7373 2e5f 6966 6c79 7465  ek = tss._iflyte
+00042ff0: 6b0d 0a69 666c 7974 656b 203d 2074 7373  k..iflytek = tss
+00043000: 2e69 666c 7974 656b 0d0a 5f69 666c 7972  .iflytek.._iflyr
+00043010: 6563 203d 2074 7373 2e5f 6966 6c79 7265  ec = tss._iflyre
+00043020: 630d 0a69 666c 7972 6563 203d 2074 7373  c..iflyrec = tss
+00043030: 2e69 666c 7972 6563 0d0a 5f69 7472 616e  .iflyrec.._itran
+00043040: 736c 6174 6520 3d20 7473 732e 5f69 7472  slate = tss._itr
+00043050: 616e 736c 6174 650d 0a69 7472 616e 736c  anslate..itransl
+00043060: 6174 6520 3d20 7473 732e 6974 7261 6e73  ate = tss.itrans
+00043070: 6c61 7465 0d0a 5f6a 7564 6963 203d 2074  late.._judic = t
+00043080: 7373 2e5f 6a75 6469 630d 0a6a 7564 6963  ss._judic..judic
+00043090: 203d 2074 7373 2e6a 7564 6963 0d0a 5f6c   = tss.judic.._l
+000430a0: 616e 6775 6167 6557 6972 6520 3d20 7473  anguageWire = ts
+000430b0: 732e 5f6c 616e 6775 6167 6557 6972 650d  s._languageWire.
+000430c0: 0a6c 616e 6775 6167 6557 6972 6520 3d20  .languageWire = 
+000430d0: 7473 732e 6c61 6e67 7561 6765 5769 7265  tss.languageWire
+000430e0: 0d0a 5f6c 696e 6776 616e 6578 203d 2074  .._lingvanex = t
+000430f0: 7373 2e5f 6c69 6e67 7661 6e65 780d 0a6c  ss._lingvanex..l
+00043100: 696e 6776 616e 6578 203d 2074 7373 2e6c  ingvanex = tss.l
+00043110: 696e 6776 616e 6578 0d0a 5f6e 6975 7472  ingvanex.._niutr
+00043120: 616e 7320 3d20 7473 732e 5f6e 6975 7472  ans = tss._niutr
+00043130: 616e 730d 0a6e 6975 7472 616e 7320 3d20  ans..niutrans = 
+00043140: 7473 732e 6e69 7574 7261 6e73 0d0a 5f6d  tss.niutrans.._m
+00043150: 676c 6970 203d 2074 7373 2e5f 6d67 6c69  glip = tss._mgli
+00043160: 700d 0a6d 676c 6970 203d 2074 7373 2e6d  p..mglip = tss.m
+00043170: 676c 6970 0d0a 5f6d 6972 6169 203d 2074  glip.._mirai = t
+00043180: 7373 2e5f 6d69 7261 690d 0a6d 6972 6169  ss._mirai..mirai
+00043190: 203d 2074 7373 2e6d 6972 6169 0d0a 5f6d   = tss.mirai.._m
+000431a0: 6f64 6572 6e4d 7420 3d20 7473 732e 5f6d  odernMt = tss._m
+000431b0: 6f64 6572 6e4d 740d 0a6d 6f64 6572 6e4d  odernMt..modernM
+000431c0: 7420 3d20 7473 732e 6d6f 6465 726e 4d74  t = tss.modernMt
+000431d0: 0d0a 5f6d 794d 656d 6f72 7920 3d20 7473  .._myMemory = ts
+000431e0: 732e 5f6d 794d 656d 6f72 790d 0a6d 794d  s._myMemory..myM
+000431f0: 656d 6f72 7920 3d20 7473 732e 6d79 4d65  emory = tss.myMe
+00043200: 6d6f 7279 0d0a 5f70 6170 6167 6f20 3d20  mory.._papago = 
+00043210: 7473 732e 5f70 6170 6167 6f0d 0a70 6170  tss._papago..pap
+00043220: 6167 6f20 3d20 7473 732e 7061 7061 676f  ago = tss.papago
+00043230: 0d0a 5f71 7146 616e 7969 203d 2074 7373  .._qqFanyi = tss
+00043240: 2e5f 7171 4661 6e79 690d 0a71 7146 616e  ._qqFanyi..qqFan
+00043250: 7969 203d 2074 7373 2e71 7146 616e 7969  yi = tss.qqFanyi
+00043260: 0d0a 5f71 7154 7261 6e53 6d61 7274 203d  .._qqTranSmart =
+00043270: 2074 7373 2e5f 7171 5472 616e 536d 6172   tss._qqTranSmar
+00043280: 740d 0a71 7154 7261 6e53 6d61 7274 203d  t..qqTranSmart =
+00043290: 2074 7373 2e71 7154 7261 6e53 6d61 7274   tss.qqTranSmart
+000432a0: 0d0a 5f72 6576 6572 736f 203d 2074 7373  .._reverso = tss
+000432b0: 2e5f 7265 7665 7273 6f0d 0a72 6576 6572  ._reverso..rever
+000432c0: 736f 203d 2074 7373 2e72 6576 6572 736f  so = tss.reverso
+000432d0: 0d0a 5f73 6f67 6f75 203d 2074 7373 2e5f  .._sogou = tss._
+000432e0: 736f 676f 750d 0a73 6f67 6f75 203d 2074  sogou..sogou = t
+000432f0: 7373 2e73 6f67 6f75 0d0a 5f73 7973 5472  ss.sogou.._sysTr
+00043300: 616e 203d 2074 7373 2e5f 7379 7354 7261  an = tss._sysTra
+00043310: 6e0d 0a73 7973 5472 616e 203d 2074 7373  n..sysTran = tss
+00043320: 2e73 7973 5472 616e 0d0a 5f74 696c 6465  .sysTran.._tilde
+00043330: 203d 2074 7373 2e5f 7469 6c64 650d 0a74   = tss._tilde..t
+00043340: 696c 6465 203d 2074 7373 2e74 696c 6465  ilde = tss.tilde
+00043350: 0d0a 5f74 7261 6e73 6c61 7465 436f 6d20  .._translateCom 
+00043360: 3d20 7473 732e 5f74 7261 6e73 6c61 7465  = tss._translate
+00043370: 436f 6d0d 0a74 7261 6e73 6c61 7465 436f  Com..translateCo
+00043380: 6d20 3d20 7473 732e 7472 616e 736c 6174  m = tss.translat
+00043390: 6543 6f6d 0d0a 5f74 7261 6e73 6c61 7465  eCom.._translate
+000433a0: 4d65 203d 2074 7373 2e5f 7472 616e 736c  Me = tss._transl
+000433b0: 6174 654d 650d 0a74 7261 6e73 6c61 7465  ateMe..translate
+000433c0: 4d65 203d 2074 7373 2e74 7261 6e73 6c61  Me = tss.transla
+000433d0: 7465 4d65 0d0a 5f75 7469 6265 7420 3d20  teMe.._utibet = 
+000433e0: 7473 732e 5f75 7469 6265 740d 0a75 7469  tss._utibet..uti
+000433f0: 6265 7420 3d20 7473 732e 7574 6962 6574  bet = tss.utibet
+00043400: 0d0a 5f76 6f6c 6345 6e67 696e 6520 3d20  .._volcEngine = 
+00043410: 7473 732e 5f76 6f6c 6345 6e67 696e 650d  tss._volcEngine.
+00043420: 0a76 6f6c 6345 6e67 696e 6520 3d20 7473  .volcEngine = ts
+00043430: 732e 766f 6c63 456e 6769 6e65 0d0a 5f79  s.volcEngine.._y
+00043440: 616e 6465 7820 3d20 7473 732e 5f79 616e  andex = tss._yan
+00043450: 6465 780d 0a79 616e 6465 7820 3d20 7473  dex..yandex = ts
+00043460: 732e 7961 6e64 6578 0d0a 5f79 6565 6b69  s.yandex.._yeeki
+00043470: 7420 3d20 7473 732e 5f79 6565 6b69 740d  t = tss._yeekit.
+00043480: 0a79 6565 6b69 7420 3d20 7473 732e 7965  .yeekit = tss.ye
+00043490: 656b 6974 0d0a 5f79 6f75 6461 6f20 3d20  ekit.._youdao = 
+000434a0: 7473 732e 5f79 6f75 6461 6f0d 0a79 6f75  tss._youdao..you
+000434b0: 6461 6f20 3d20 7473 732e 796f 7564 616f  dao = tss.youdao
+000434c0: 0d0a 0d0a 7472 616e 736c 6174 655f 7465  ....translate_te
+000434d0: 7874 203d 2074 7373 2e74 7261 6e73 6c61  xt = tss.transla
+000434e0: 7465 5f74 6578 740d 0a74 7261 6e73 6c61  te_text..transla
+000434f0: 7465 5f68 746d 6c20 3d20 7473 732e 7472  te_html = tss.tr
+00043500: 616e 736c 6174 655f 6874 6d6c 0d0a 7472  anslate_html..tr
+00043510: 616e 736c 6174 6f72 735f 706f 6f6c 203d  anslators_pool =
+00043520: 2074 7373 2e74 7261 6e73 6c61 746f 7273   tss.translators
+00043530: 5f70 6f6f 6c0d 0a0d 0a70 7265 6163 6365  _pool....preacce
+00043540: 6c65 7261 7465 203d 2074 7373 2e70 7265  lerate = tss.pre
+00043550: 6163 6365 6c65 7261 7465 0d0a 7370 6565  accelerate..spee
+00043560: 6474 6573 7420 3d20 7473 732e 7370 6565  dtest = tss.spee
+00043570: 6474 6573 740d 0a70 7265 6163 6365 6c65  dtest..preaccele
+00043580: 7261 7465 5f61 6e64 5f73 7065 6564 7465  rate_and_speedte
+00043590: 7374 203d 2074 7373 2e70 7265 6163 6365  st = tss.preacce
+000435a0: 6c65 7261 7465 5f61 6e64 5f73 7065 6564  lerate_and_speed
+000435b0: 7465 7374 0d0a 2320 7379 732e 7374 6465  test..# sys.stde
+000435c0: 7272 2e77 7269 7465 2866 2753 7570 706f  rr.write(f'Suppo
+000435d0: 7274 2074 7261 6e73 6c61 746f 7273 207b  rt translators {
+000435e0: 7472 616e 736c 6174 6f72 735f 706f 6f6c  translators_pool
+000435f0: 7d20 6f6e 6c79 2e5c 6e27 290d 0a         } only.\n')..
```

### Comparing `translators-5.7.7/translators.egg-info/PKG-INFO` & `translators-5.7.8/translators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translators
-Version: 5.7.7
+Version: 5.7.8
 Summary: Translators is a library which aims to bring free, multiple, enjoyable translation to individuals and students in Python.
 Home-page: https://github.com/uliontse/translators
 Author: UlionTse
 Author-email: uliontse@outlook.com
 License: GPLv3
 Project-URL: Source, https://github.com/UlionTse/translators
 Project-URL: Changelog, https://github.com/UlionTse/translators/blob/master/change_log.txt
@@ -24,37 +24,37 @@
 Provides-Extra: pypi
 License-File: LICENSE
 
 <p align="center">
   <img src="https://github.com/UlionTse/translators/blob/master/docs/translators_logo.png" width="500"/>
 </p>
 <p align="center">
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/translators.svg"></a>
-  <a href="https://anaconda.org/conda-forge/translators"><img alt="Conda - Version" src="https://img.shields.io/conda/vn/conda-forge/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Python" src="https://img.shields.io/pypi/pyversions/translators.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="PyPI - Status" src="https://img.shields.io/pypi/status/translators.svg"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/translators.svg?color=blue"></a>
+  <a href="https://anaconda.org/conda-forge/translators"><img alt="Conda - Version" src="https://img.shields.io/conda/vn/conda-forge/translators.svg?color=blue"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/translators.svg?color=brightgreen"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Python" src="https://img.shields.io/pypi/pyversions/translators.svg?color=blue"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Status" src="https://img.shields.io/pypi/status/translators.svg?color=brightgreen"></a>
   <a href="https://pypi.org/project/translators"><img alt="PyPI - Wheel" src="https://img.shields.io/badge/wheel-yes-brightgreen.svg"></a>
-  <a href="https://pypi.org/project/translators"><img alt="Downloads" src="https://pepy.tech/badge/translators"></a>
+  <a href="https://pypi.org/project/translators"><img alt="PyPI - Downloads" src="https://static.pepy.tech/personalized-badge/translators?left_text=downloads&left_color=gray&right_color=blue"></a>
 </p>
 
 * * *
 
 **Translators** is a library which aims to bring **free, multiple, enjoyable** translation to individuals and students in Python. 
 
 <details>
 <summary>Supported Translation Services</summary>
 
 | ID  | Translator                                                                        | Number of Supported Languages | Advantage                                                                                   | Service                                                                                                           | Status                          |
 | --- | --------------------------------------------------------------------------------- | ----------------------------- | ------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ------------------------------- |
-| 1   | [Niutrans](https://niutrans.com/trans)                                            | 302                           | support the most languages in the world                                                     | [Northeastern University](http://english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China            | /                               |
-| 2   | [Alibaba](https://translate.alibaba.com)                                          | 221                           | support most languages, support professional field                                          | [Alibaba](https://damo.alibaba.com/about?lang=en), China                                                          | stable                          |
-| 3   | [Baidu](https://fanyi.baidu.com)                                                  | 201                           | support most languages, support professional field, support classical Chinese               | [Baidu](https://ir.baidu.com/company-overview), China                                                             | stable                          |
-| 4   | [Iciba](https://www.iciba.com/fy)                                                 | 187                           | support the most languages in the world                                                     | [Kingsoft](https://www.wps.com/about-us/) / [Xiaomi](https://www.mi.com/us/about/), China                         | stable                          |
-| 5   | [MyMemory](https://mymemory.translated.net)                                       | 151                           | support the most languages in the world, good at Creole English, Creole French              | [Translated](https://translatedlabs.com/welcome), Italy                                                           | stable                          |
+| 1   | [MyMemory](https://mymemory.translated.net)                                       | 330                           | support the most languages in the world                                                     | [Translated](https://translatedlabs.com/welcome), Italy                                                           | stable                          |
+| 2   | [Niutrans](https://niutrans.com/trans)                                            | 302                           | support the most languages in the world                                                     | [Northeastern University](http://english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China            | /                               |
+| 3   | [Alibaba](https://translate.alibaba.com)                                          | 221                           | support most languages, support professional field                                          | [Alibaba](https://damo.alibaba.com/about?lang=en), China                                                          | stable                          |
+| 4   | [Baidu](https://fanyi.baidu.com)                                                  | 201                           | support most languages, support professional field, support classical Chinese               | [Baidu](https://ir.baidu.com/company-overview), China                                                             | stable                          |
+| 5   | [Iciba](https://www.iciba.com/fy)                                                 | 187                           | support the most languages in the world                                                     | [Kingsoft](https://www.wps.com/about-us/) / [Xiaomi](https://www.mi.com/us/about/), China                         | stable                          |
 | 6   | [Iflytek](https://fanyi.xfyun.cn/console/trans/text)                              | 140                           | support the most languages in the world                                                     | [Iflytek](https://www.iflytek.com/en/about-us.html), China                                                        | /                               |
 | 7   | [Google](https://translate.google.com)                                            | 134                           | support more languages in the world                                                         | [Google](https://about.google/), America                                                                          | stable(offline in China inland) |
 | 8   | [VolcEngine](https://translate.volcengine.com)                                    | 122                           | support more languages in the world, support professional field                             | [ByteDance](https://www.bytedance.com/en/), China                                                                 | /                               |
 | 9   | [Lingvanex](https://lingvanex.com/demo)                                           | 112                           | support translation of different regions but the same language                              | [Lingvanex](https://lingvanex.com/about-us/), Cyprus                                                              | stable                          |
 | 10  | [Bing](https://www.bing.com/Translator)                                           | 110                           | support more languages in the world                                                         | [Microsoft](https://www.microsoft.com/en-us/about), America                                                       | stable                          |
 | 11  | [Yandex](https://translate.yandex.com)                                            | 102                           | support more languages in the world, support word to emoji                                  | [Yandex](https://yandex.com/company/), Russia                                                                     | /                               |
 | 12  | [Itranslate](https://itranslate.com/webapp)                                       | 101                           | support translation of different regions but the same language, such as en-US, en-UK, en-AU | [Itranslate](https://itranslate.com/about), Austria                                                               | stable                          |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: translators Version: 5.7.7 Summary: Translators is
+Metadata-Version: 2.1 Name: translators Version: 5.7.8 Summary: Translators is
 a library which aims to bring free, multiple, enjoyable translation to
 individuals and students in Python. Home-page: https://github.com/uliontse/
 translators Author: UlionTse Author-email: uliontse@outlook.com License: GPLv3
 Project-URL: Source, https://github.com/UlionTse/translators Project-URL:
 Changelog, https://github.com/UlionTse/translators/blob/master/change_log.txt
 Project-URL: Documentation, https://github.com/UlionTse/translators/blob/
 master/README.md Keywords:
@@ -13,99 +13,98 @@
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Provides-Extra: pypi License-File: LICENSE
 [https://github.com/UlionTse/translators/blob/master/docs/translators_logo.png]
   [PyPI_-_Version] [Conda_-_Version] [PyPI_-_License] [PyPI_-_Python] [PyPI_-
-                      Status] [PyPI_-_Wheel] [Downloads]
+                   Status] [PyPI_-_Wheel] [PyPI_-_Downloads]
 * * * **Translators** is a library which aims to bring **free, multiple,
 enjoyable** translation to individuals and students in Python.  Supported
 Translation Services | ID | Translator | Number of Supported Languages |
 Advantage | Service | Status | | --- | ----------------------------------------
 ----------------------------------------- | ----------------------------- | ---
 -------------------------------------------------------------------------------
 --------- | -------------------------------------------------------------------
 ---------------------------------------------- | ------------------------------
-- | | 1 | [Niutrans](https://niutrans.com/trans) | 302 | support the most
-languages in the world | [Northeastern University](http://english.neu.edu.cn/
-) / [Niutrans](https://github.com/NiuTrans), China | / | | 2 | [Alibaba](https:
-//translate.alibaba.com) | 221 | support most languages, support professional
-field | [Alibaba](https://damo.alibaba.com/about?lang=en), China | stable | | 3
-| [Baidu](https://fanyi.baidu.com) | 201 | support most languages, support
-professional field, support classical Chinese | [Baidu](https://ir.baidu.com/
-company-overview), China | stable | | 4 | [Iciba](https://www.iciba.com/fy) |
-187 | support the most languages in the world | [Kingsoft](https://www.wps.com/
-about-us/) / [Xiaomi](https://www.mi.com/us/about/), China | stable | | 5 |
-[MyMemory](https://mymemory.translated.net) | 151 | support the most languages
-in the world, good at Creole English, Creole French | [Translated](https://
-translatedlabs.com/welcome), Italy | stable | | 6 | [Iflytek](https://
-fanyi.xfyun.cn/console/trans/text) | 140 | support the most languages in the
-world | [Iflytek](https://www.iflytek.com/en/about-us.html), China | / | | 7 |
-[Google](https://translate.google.com) | 134 | support more languages in the
-world | [Google](https://about.google/), America | stable(offline in China
-inland) | | 8 | [VolcEngine](https://translate.volcengine.com) | 122 | support
-more languages in the world, support professional field | [ByteDance](https://
-www.bytedance.com/en/), China | / | | 9 | [Lingvanex](https://lingvanex.com/
-demo) | 112 | support translation of different regions but the same language |
-[Lingvanex](https://lingvanex.com/about-us/), Cyprus | stable | | 10 | [Bing]
-(https://www.bing.com/Translator) | 110 | support more languages in the world |
-[Microsoft](https://www.microsoft.com/en-us/about), America | stable | | 11 |
-[Yandex](https://translate.yandex.com) | 102 | support more languages in the
-world, support word to emoji | [Yandex](https://yandex.com/company/), Russia |
-/ | | 12 | [Itranslate](https://itranslate.com/webapp) | 101 | support
-translation of different regions but the same language, such as en-US, en-UK,
-en-AU | [Itranslate](https://itranslate.com/about), Austria | stable | | 13 |
-[Sogou](https://fanyi.sogou.com/text) | 61 | support more languages in the
-world | [Tencent](https://www.tencent.com/en-us/about.html), China | stable | |
-14 | [ModernMt](https://www.modernmt.com/translate) | 56 | open-source, support
-more languages in the world | [Modernmt](https://github.com/modernmt) /
-[Translated](https://translatedlabs.com/welcome), Italy | stable | | 15 |
-[SysTran](https://www.systran.net/translate/) | 52 | support more languages in
-the world | [SysTran](https://www.systran.net/about/), France | stable | | 16 |
-[Apertium](https://www.apertium.org/) | 45 | open-source | [Apertium](https://
-github.com/apertium), Spain | stable | | 17 | [Reverso](https://
-www.reverso.net/text-translation) | 42 | popular on Mac and Iphone | [Reverso]
-(https://www.corporate-translation.reverso.com/about-us), France | stable | |
-18 | [CloudYi](https://www.cloudtranslation.com/#/translate) | 28 | support
-main languages | [Xiamen University](http://nlp.xmu.edu.cn/) /
-[CloudTranslation](https://www.cloudtranslation.com/#/about), China | stable |
-| 19 | [Deepl](https://www.deepl.com/translator) | 27 | high quality to
-translate but response slowly | [Deepl](https://jobs.deepl.com/l/en), Germany |
-stable | | 20 | [QQTranSmart](https://transmart.qq.com) | 22 | support main
-languages | [Tencent](https://www.tencent.com/en-us/about.html), China | stable
-| | 21 | [TranslateCom](https://www.translate.com/machine-translation) | 21 |
-good at English translation | [TranslateCom](https://www.translate.com/about-
-us), America | stable | | 22 | [Tilde](https://translate.tilde.com/) | 21 |
-good at lv, de, fr translation | [Tilde](https://tilde.com/about), Latvia | / |
-| 23 | [QQFanyi](https://fanyi.qq.com) | 17 | support main languages |
-[Tencent](https://www.tencent.com/en-us/about.html), China | stable | | 24 |
-[Argos](https://translate.argosopentech.com) | 17 | open-source | [Argos]
-(https://github.com/argosopentech) / [Libre](https://github.com/
-LibreTranslate), America | stable | | 25 | [TranslateMe](https://
-translateme.network/) | 16 | good at English translation | [TranslateMe](https:
-//translateme.network/our-team/) / [Neosus](https://neosus.net/about/),
-Lithuania | / | | 26 | [Youdao](https://ai.youdao.com/product-fanyi-text.s) |
-15 | support main languages, high quality | [Netease](https://ir.netease.com/
-company-overview/corporate-profile), China | stable | | 27 | [Papago](https://
-papago.naver.com) | 15 | good at Korean translation | [Naver](https://
-www.navercorp.com/en/naver/company), South Korea | stable | | 28 | [Marai]
-(https://miraitranslate.com/trial/) | 15 | good at Japanese translation |
-[MaraiTranslate](https://miraitranslate.com/en/company/), Japan | / | | 29 |
-[Iflyrec](https://fanyi.iflyrec.com) | 12 | good at Chinese translation |
-[Iflytek](https://www.iflytek.com/en/about-us.html), China | stable | | 30 |
-[Yeekit](https://www.yeekit.com/site/translate) | 10 | support main languages |
-[CTC](https://www.ctpc.com.cn/cms/enAboutUs.htm), China | / | | 31 |
-[LanguageWire](https://www.languagewire.com/en/technology/languagewire-
-translate) | 8 | good at English translation | [LanguageWire](https://
-www.languagewire.com/about-us), Denmark | stable | | 32 | [Caiyun](https://
-fanyi.caiyunapp.com) | 7 | high quality to translate but response slowly,
-support professional field | [ColorfulClouds](http://caiyunapp.com/jobs/),
-China | stable | | 33 | [Elia](https://elia.eus/translator) | 6 | good at
-Basque translation | [Elhuyar](https://www.elhuyar.eus/eu/nor-gara), Spain |
+- | | 1 | [MyMemory](https://mymemory.translated.net) | 330 | support the most
+languages in the world | [Translated](https://translatedlabs.com/welcome),
+Italy | stable | | 2 | [Niutrans](https://niutrans.com/trans) | 302 | support
+the most languages in the world | [Northeastern University](http://
+english.neu.edu.cn/) / [Niutrans](https://github.com/NiuTrans), China | / | | 3
+| [Alibaba](https://translate.alibaba.com) | 221 | support most languages,
+support professional field | [Alibaba](https://damo.alibaba.com/about?lang=en),
+China | stable | | 4 | [Baidu](https://fanyi.baidu.com) | 201 | support most
+languages, support professional field, support classical Chinese | [Baidu]
+(https://ir.baidu.com/company-overview), China | stable | | 5 | [Iciba](https:/
+/www.iciba.com/fy) | 187 | support the most languages in the world | [Kingsoft]
+(https://www.wps.com/about-us/) / [Xiaomi](https://www.mi.com/us/about/), China
+| stable | | 6 | [Iflytek](https://fanyi.xfyun.cn/console/trans/text) | 140 |
+support the most languages in the world | [Iflytek](https://www.iflytek.com/en/
+about-us.html), China | / | | 7 | [Google](https://translate.google.com) | 134
+| support more languages in the world | [Google](https://about.google/),
+America | stable(offline in China inland) | | 8 | [VolcEngine](https://
+translate.volcengine.com) | 122 | support more languages in the world, support
+professional field | [ByteDance](https://www.bytedance.com/en/), China | / | |
+9 | [Lingvanex](https://lingvanex.com/demo) | 112 | support translation of
+different regions but the same language | [Lingvanex](https://lingvanex.com/
+about-us/), Cyprus | stable | | 10 | [Bing](https://www.bing.com/Translator) |
+110 | support more languages in the world | [Microsoft](https://
+www.microsoft.com/en-us/about), America | stable | | 11 | [Yandex](https://
+translate.yandex.com) | 102 | support more languages in the world, support word
+to emoji | [Yandex](https://yandex.com/company/), Russia | / | | 12 |
+[Itranslate](https://itranslate.com/webapp) | 101 | support translation of
+different regions but the same language, such as en-US, en-UK, en-AU |
+[Itranslate](https://itranslate.com/about), Austria | stable | | 13 | [Sogou]
+(https://fanyi.sogou.com/text) | 61 | support more languages in the world |
+[Tencent](https://www.tencent.com/en-us/about.html), China | stable | | 14 |
+[ModernMt](https://www.modernmt.com/translate) | 56 | open-source, support more
+languages in the world | [Modernmt](https://github.com/modernmt) / [Translated]
+(https://translatedlabs.com/welcome), Italy | stable | | 15 | [SysTran](https:/
+/www.systran.net/translate/) | 52 | support more languages in the world |
+[SysTran](https://www.systran.net/about/), France | stable | | 16 | [Apertium]
+(https://www.apertium.org/) | 45 | open-source | [Apertium](https://github.com/
+apertium), Spain | stable | | 17 | [Reverso](https://www.reverso.net/text-
+translation) | 42 | popular on Mac and Iphone | [Reverso](https://
+www.corporate-translation.reverso.com/about-us), France | stable | | 18 |
+[CloudYi](https://www.cloudtranslation.com/#/translate) | 28 | support main
+languages | [Xiamen University](http://nlp.xmu.edu.cn/) / [CloudTranslation]
+(https://www.cloudtranslation.com/#/about), China | stable | | 19 | [Deepl]
+(https://www.deepl.com/translator) | 27 | high quality to translate but
+response slowly | [Deepl](https://jobs.deepl.com/l/en), Germany | stable | | 20
+| [QQTranSmart](https://transmart.qq.com) | 22 | support main languages |
+[Tencent](https://www.tencent.com/en-us/about.html), China | stable | | 21 |
+[TranslateCom](https://www.translate.com/machine-translation) | 21 | good at
+English translation | [TranslateCom](https://www.translate.com/about-us),
+America | stable | | 22 | [Tilde](https://translate.tilde.com/) | 21 | good at
+lv, de, fr translation | [Tilde](https://tilde.com/about), Latvia | / | | 23 |
+[QQFanyi](https://fanyi.qq.com) | 17 | support main languages | [Tencent]
+(https://www.tencent.com/en-us/about.html), China | stable | | 24 | [Argos]
+(https://translate.argosopentech.com) | 17 | open-source | [Argos](https://
+github.com/argosopentech) / [Libre](https://github.com/LibreTranslate), America
+| stable | | 25 | [TranslateMe](https://translateme.network/) | 16 | good at
+English translation | [TranslateMe](https://translateme.network/our-team/) /
+[Neosus](https://neosus.net/about/), Lithuania | / | | 26 | [Youdao](https://
+ai.youdao.com/product-fanyi-text.s) | 15 | support main languages, high quality
+| [Netease](https://ir.netease.com/company-overview/corporate-profile), China |
+stable | | 27 | [Papago](https://papago.naver.com) | 15 | good at Korean
+translation | [Naver](https://www.navercorp.com/en/naver/company), South Korea
+| stable | | 28 | [Marai](https://miraitranslate.com/trial/) | 15 | good at
+Japanese translation | [MaraiTranslate](https://miraitranslate.com/en/company/
+), Japan | / | | 29 | [Iflyrec](https://fanyi.iflyrec.com) | 12 | good at
+Chinese translation | [Iflytek](https://www.iflytek.com/en/about-us.html),
+China | stable | | 30 | [Yeekit](https://www.yeekit.com/site/translate) | 10 |
+support main languages | [CTC](https://www.ctpc.com.cn/cms/enAboutUs.htm),
+China | / | | 31 | [LanguageWire](https://www.languagewire.com/en/technology/
+languagewire-translate) | 8 | good at English translation | [LanguageWire]
+(https://www.languagewire.com/about-us), Denmark | stable | | 32 | [Caiyun]
+(https://fanyi.caiyunapp.com) | 7 | high quality to translate but response
+slowly, support professional field | [ColorfulClouds](http://caiyunapp.com/
+jobs/), China | stable | | 33 | [Elia](https://elia.eus/translator) | 6 | good
+at Basque translation | [Elhuyar](https://www.elhuyar.eus/eu/nor-gara), Spain |
 stable | | 34 | [Judic](https://judic.io/en/translate) | 4 | good at European
 translation | [CrossLang](https://crosslang.com/about-us/), Belgium | stable |
 | 35 | [Mglip](http://fy.mglip.com/pc) | 3 | good at Mongolia translation |
 [Inner Mongolia University](https://www.imu.edu.cn/yw/Home.htm), China | stable
 | | 36 | [Utibet](http://mt.utibet.edu.cn/mt) | 2 | good at Tibet translation |
 [Tibet University](http://www.utibet.edu.cn/), China | stable |   Installation
 ```sh # PYPI pip install --upgrade translators # Conda conda install -c conda-
```

