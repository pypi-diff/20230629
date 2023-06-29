# Comparing `tmp/ms2rescore-2.1.3.tar.gz` & `tmp/ms2rescore-3.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2rescore-2.1.3.tar", last modified: Tue Aug 30 12:12:53 2022, max compression
+gzip compressed data, was "ms2rescore-3.0.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ms2rescore-2.1.3.tar` & `ms2rescore-3.0.0.dev1.tar`

### file list

```diff
@@ -1,39 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 12:12:53.860371 ms2rescore-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13105 2022-08-30 12:12:53.860371 ms2rescore-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10123 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 12:12:53.808370 ms2rescore-2.1.3/ms2rescore/
--rw-r--r--   0 runner    (1001) docker     (121)    11614 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6309 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    10756 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/gui.py
--rw-r--r--   0 runner    (1001) docker     (121)    24600 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/id_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    19252 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/maxquant.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 12:12:53.808370 ms2rescore-2.1.3/ms2rescore/package_data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/package_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2875 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/package_data/config_default.json
--rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/package_data/config_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 12:12:53.860371 ms2rescore-2.1.3/ms2rescore/package_data/img/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 12:12:40.000000 ms2rescore-2.1.3/ms2rescore/package_data/img/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121) 44669194 2022-08-30 12:12:41.000000 ms2rescore-2.1.3/ms2rescore/package_data/img/config_icon.png
--rw-r--r--   0 runner    (1001) docker     (121)    43034 2022-08-30 12:12:41.000000 ms2rescore-2.1.3/ms2rescore/package_data/img/program_icon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     5492 2022-08-30 12:12:41.000000 ms2rescore-2.1.3/ms2rescore/parse_mgf.py
--rw-r--r--   0 runner    (1001) docker     (121)     5177 2022-08-30 12:12:41.000000 ms2rescore-2.1.3/ms2rescore/peptide_record.py
--rw-r--r--   0 runner    (1001) docker     (121)     7252 2022-08-30 12:12:41.000000 ms2rescore-2.1.3/ms2rescore/peptideshaker.py
--rw-r--r--   0 runner    (1001) docker     (121)    20259 2022-08-30 12:12:41.000000 ms2rescore-2.1.3/ms2rescore/percolator.py
--rw-r--r--   0 runner    (1001) docker     (121)    21928 2022-08-30 12:12:41.000000 ms2rescore-2.1.3/ms2rescore/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)    22674 2022-08-30 12:12:41.000000 ms2rescore-2.1.3/ms2rescore/rescore_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     9725 2022-08-30 12:12:41.000000 ms2rescore-2.1.3/ms2rescore/retention_time.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-08-30 12:12:41.000000 ms2rescore-2.1.3/ms2rescore/setup_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 12:12:53.808370 ms2rescore-2.1.3/ms2rescore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13105 2022-08-30 12:12:53.000000 ms2rescore-2.1.3/ms2rescore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-08-30 12:12:53.000000 ms2rescore-2.1.3/ms2rescore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-30 12:12:53.000000 ms2rescore-2.1.3/ms2rescore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-30 12:12:53.000000 ms2rescore-2.1.3/ms2rescore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-08-30 12:12:53.000000 ms2rescore-2.1.3/ms2rescore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-30 12:12:53.000000 ms2rescore-2.1.3/ms2rescore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-30 12:12:53.860371 ms2rescore-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-08-30 12:12:41.000000 ms2rescore-2.1.3/setup.py
+-rw-r--r--   0        0        0    11357 2023-06-29 15:36:34.740234 ms2rescore-3.0.0.dev1/LICENSE
+-rw-r--r--   0        0        0    11395 2023-06-29 15:36:34.740234 ms2rescore-3.0.0.dev1/README.md
+-rw-r--r--   0        0        0      376 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/__init__.py
+-rw-r--r--   0        0        0     1346 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/__main__.py
+-rw-r--r--   0        0        0     6817 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/config_parser.py
+-rw-r--r--   0        0        0      428 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/exceptions.py
+-rw-r--r--   0        0        0      415 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/feature_generators/__init__.py
+-rw-r--r--   0        0        0     9563 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/feature_generators/deeplc.py
+-rw-r--r--   0        0        0    14146 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/feature_generators/intensity.py
+-rw-r--r--   0        0        0     5472 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/feature_generators/maxquant.py
+-rw-r--r--   0        0        0    33210 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/gui.py
+-rw-r--r--   0        0        0     6103 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/ms2rescore_main.py
+-rw-r--r--   0        0        0     4514 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/package_data/MS2Rescore_gui_theme.json
+-rw-r--r--   0        0        0        0 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/package_data/__init__.py
+-rw-r--r--   0        0        0      778 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/package_data/config_default.json
+-rw-r--r--   0        0        0     6239 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/package_data/config_schema.json
+-rw-r--r--   0        0        0        0 2023-06-29 15:36:35.644229 ms2rescore-3.0.0.dev1/ms2rescore/package_data/img/__init__.py
+-rw-r--r--   0        0        0 44669194 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/ms2rescore/package_data/img/config_icon.png
+-rw-r--r--   0        0        0     4837 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/ms2rescore/package_data/img/github-mark-white.png
+-rw-r--r--   0        0        0     5557 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/ms2rescore/package_data/img/github-mark.png
+-rw-r--r--   0        0        0    52066 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/ms2rescore/package_data/img/ms2rescore_logo.png
+-rw-r--r--   0        0        0    43034 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/ms2rescore/package_data/img/program_icon.ico
+-rw-r--r--   0        0        0     1420 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/ms2rescore/parse_mgf.py
+-rw-r--r--   0        0        0    33752 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/ms2rescore/plotting.py
+-rw-r--r--   0        0        0      407 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/ms2rescore/rescoring_engines/__init__.py
+-rw-r--r--   0        0        0     3671 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/ms2rescore/rescoring_engines/percolator.py
+-rw-r--r--   0        0        0     1082 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/ms2rescore/setup_logging.py
+-rw-r--r--   0        0        0     2667 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/ms2rescore/utils.py
+-rw-r--r--   0        0        0     2248 2023-06-29 15:36:35.748228 ms2rescore-3.0.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0    13553 1970-01-01 00:00:00.000000 ms2rescore-3.0.0.dev1/PKG-INFO
```

### Comparing `ms2rescore-2.1.3/LICENSE` & `ms2rescore-3.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2rescore-2.1.3/PKG-INFO` & `ms2rescore-3.0.0.dev1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,248 +1,303 @@
 Metadata-Version: 2.1
 Name: ms2rescore
-Version: 2.1.3
+Version: 3.0.0.dev1
 Summary: MS²Rescore: Sensitive PSM rescoring with predicted MS² peak intensities and retention times.
-Home-page: https://compomics.github.io/projects/ms2rescore/
-Author: Ralf Gabriels, Arthur Declercq, Ana Sílvia C. Silva, Tim Van Den Bossche
-Author-email: compomics.list@gmail.com
-License: apache-2.0
-Project-URL: Documentation, http://compomics.github.io/projects/ms2rescore
-Project-URL: Source, https://github.com/compomics/ms2rescore
-Project-URL: Tracker, https://github.com/compomics/ms2rescore/issues
-Project-URL: Publication, https://doi.org/10.1093/bioinformatics/btz383
-Description: <img src="https://github.com/compomics/ms2rescore/raw/master/img/ms2rescore_logo.png" width="150" height="150" />
-        <br/><br/>
-        
-        [![GitHub release](https://img.shields.io/github/release-pre/compomics/ms2rescore.svg?style=flat-square)](https://github.com/compomics/ms2rescore/releases)
-        [![PyPI](https://flat.badgen.net/pypi/v/ms2rescore)](https://pypi.org/project/ms2rescore/)
-        [![GitHub Workflow Status](https://flat.badgen.net/github/checks/compomics/ms2rescore/master)](https://github.com/compomics/ms2rescore/actions/)
-        [![GitHub issues](https://img.shields.io/github/issues/compomics/ms2rescore?style=flat-square)](https://github.com/compomics/ms2rescore/issues)
-        [![GitHub](https://img.shields.io/github/license/compomics/ms2rescore.svg?style=flat-square)](https://www.apache.org/licenses/LICENSE-2.0)
-        [![Last commit](https://flat.badgen.net/github/last-commit/compomics/ms2rescore)](https://github.com/compomics/ms2rescore/commits/)
-        [![Twitter](https://flat.badgen.net/twitter/follow/compomics?icon=twitter)](https://twitter.com/compomics)
-        
-        
-        Sensitive peptide identification rescoring with predicted spectra using
-        [MS²PIP](https://github.com/compomics/ms2pip_c),
-        [DeepLC](https://github.com/compomics/deeplc), and
-        [Percolator](https://github.com/percolator/percolator/).
-        
-        ---
-        
-        - [About MS²Rescore](#about-msrescore)
-        - [Installation](#installation)
-          - [Python package](#python-package)
-          - [Windows installer](#windows-installer)
-        - [Usage](#usage)
-          - [GUI](#gui)
-          - [Command line interface](#command-line-interface)
-          - [Configuration file](#configuration-file)
-          - [Notes for specific search engines](#notes-for-specific-search-engines)
-          - [Output](#output)
-        - [Contributing](#contributing)
-        
-        ---
-        
-        ## About MS²Rescore
-        
-        MS²Rescore performs sensitive peptide identification rescoring with predicted
-        spectra using [MS²PIP](https://github.com/compomics/ms2pip_c),
-        [DeepLC](https://github.com/compomics/deeplc), and
-        [Percolator](https://github.com/percolator/percolator/). This results in more confident
-        peptide identifications, which allows you to get **more peptide IDs** at the same false
-        discovery rate (FDR) threshold, or to set a **more stringent FDR threshold** while still
-        retaining a similar number of peptide IDs. MS²Rescore is **ideal for challenging
-        proteomics identification workflows**, such as proteogenomics, metaproteomics, or
-        immunopeptidomics.
-        
-        MS²Rescore uses identifications from a
-        [Percolator IN (PIN) file](https://github.com/percolator/percolator/wiki/Interface#tab-delimited-file-format),
-        or from the output of one of these search engines:
-        
-        - [MaxQuant](https://www.maxquant.org/): Start from `msms.txt` identification
-          file and directory with `.mgf` files.
-        - [MSGFPlus](https://omics.pnl.gov/software/ms-gf): Start with an `.mzid`
-          identification file and corresponding `.mgf`.
-        - [X!Tandem](https://www.thegpm.org/tandem/): Start with an X!Tandem `.xml`
-          identification file and corresponding `.mgf`.
-        - [PEAKS](https://www.bioinfor.com/peaksdb/): Start with an `.mzid` identification
-          file and directory with `.mgf` files.
-        - [PeptideShaker](http://compomics.github.io/projects/peptide-shaker): Start with a
-          PeptideShaker Extended PSM Report and corresponding `.mgf` file.
-        
-        <br>
-        
-        If you use MS²Rescore, please cite the following article:
-        > **MS2Rescore: Data-driven rescoring dramatically boosts immunopeptide identification rates.**  \
-        Arthur Declercq, Robbin Bouwmeester, Sven Degroeve, Lennart Martens, and Ralf Gabriels.  \
-        _bioRxiv_ (2021) [doi:10.1101/2021.11.02.466886](https://doi.org/10.1101/2021.11.02.466886)
-        
-        <br>
-        
-        The concept of rescoring with predicted spectrum features was first described in:
-        
-        > **Accurate peptide fragmentation predictions allow data driven approaches to replace
-        and improve upon proteomics search engine scoring functions.**  \
-        Ana S C Silva, Robbin Bouwmeester, Lennart Martens, and Sven Degroeve.  \
-        _Bioinformatics_ (2019) [doi:10.1093/bioinformatics/btz383](https://doi.org/10.1093/bioinformatics/btz383)
-        
-        To replicate the experiments described in this article, check out the
-        [pub branch](https://github.com/compomics/ms2rescore/tree/pub) of this repository.
-        
-        ---
-        
-        ## Installation
-        
-        ### Python package
-        
-        [![install pip](https://flat.badgen.net/badge/install%20with/pip/green?icon=pypi)](https://pypi.org/project/ms2rescore/)
-        
-        
-        MS²Rescore requires:
-        - Python 3.7 or 3.8 on Linux, macOS, or Windows
-        - If the option `run_percolator` is set to `True`,
-        [Percolator](https://github.com/percolator/percolator/) needs to be installed and
-        callable with the `percolator` command (tested with v3.02.1)
-        - Some pipelines require the Percolator converters, such as `tandem2pin`, as well. These
-        are usually installed alongside Percolator.
-        
-        Minimal installation:
-        ```sh
-        pip install ms2rescore
-        ```
-        
-        Installation including dependencies for the graphical user interface:
-        ```sh
-        pip install ms2rescore[gui]
-        ```
-        
-        We highly recommend using a [venv](https://docs.python.org/3/library/venv.html) or
-        [conda](https://docs.conda.io/en/latest/) virtual environment.
-        
-        
-        ### Windows installer
-        [![get for windows](https://flat.badgen.net/badge/install%20for/windows/blue?icon=windows)](https://github.com/compomics/ms2rescore/releases)
-        
-        1. Download and install [Percolator](https://github.com/percolator/percolator/releases/latest)
-        and the percolator-converters. Make sure to select "Add percolator to the system PATH
-        for all users" during setup.
-        2. Download the zip file from the [latest release](https://github.com/compomics/ms2rescore/releases)
-        and unzip.
-        3. Run `install-gui-windows.bat` to install Python and MS²Rescore.
-        4. Run `start-gui-windows.bat` to start the MS²Rescore GUI.
-        
-        If Microsoft Defender SmartScreen displays a warning, click "More info" and then click
-        "Run anyway". When starting the GUI, don't mind the terminal window that opens next
-        to the GUI.
-        
-        To install a newer version of MS²Rescore, run `upgrade-gui-windows.bat`.
-        
-        ---
-        
-        ## Usage
-        
-        ### GUI
-        
-        Run `start-gui-windows.bat` or run `ms2rescore-gui` or
-        `python -m ms2rescore.gui`in your terminal to start the graphical user
-        interface. Most common settings can be configured through the
-        UI. For some advanced settings, see [Configuration file](#configuration-file).
-        
-        <img src="img/gui-screenshot.png" height=480 />
-        
-        
-        ### Command line interface
-        
-        Run MS²Rescore from the command line as follows:
-        
-        ```
-        ms2rescore -c <path-to-config-file> -m <path-to-mgf> <path-to-identification-file>
-        ```
-        
-        Run `ms2rescore --help` to see all command line options.
-        
-        ### Configuration file
-        
-        Although most options can be configered through the CLI and the GUI, MS²Rescore can be
-        further configured through a **JSON configuration file**. A correct configuration is
-        required to, for example, correctly parse the peptide modifications from the search
-        engine output. If no configuration file is passed, or some options are not configured,
-        the
-        [default values](https://github.com/compomics/ms2rescore/blob/master/ms2rescore/package_data/config_default.json)
-        for these settings will be used. Options passed from the CLI and the GUI will override
-        the configuration file. The full configuration is validated against a
-        [JSON Schema](https://github.com/compomics/ms2rescore/blob/master/ms2rescore/package_data/config_schema.json).
-        
-        A full example configuration file can be found in
-        [ms2rescore/package_data/config_default.json](https://github.com/compomics/ms2rescore/blob/master/ms2rescore/package_data/config_default.json).
-        
-        The config file contains three top level categories (`general`, `ms2pip` and
-        `percolator`) and an additional categories for specific search engines
-        (e.g. `maxquant`). The most important options in `general` are:
-        - **`pipeline`** *(string)*: Pipeline to use, depending on input format. Must be one of:
-        `['infer', 'pin', 'tandem', 'maxquant', 'msgfplus', 'peptideshaker']`. Default: `infer`.
-        - **`feature_sets`** *(array)*: Feature sets for which to generate PIN files and optionally run Percolator. Default: `['searchengine', 'rt', 'ms2pip']`.
-            - **Items** *(array)*
-              - **Items** *(string)*: Must be one of: `['searchengine', 'rt', 'ms2pip']`.
-        
-        An overview of all options can be found in [configuration.md](https://github.com/compomics/ms2rescore/blob/master/configuration.md)
-        
-        ### Notes for specific search engines
-        
-        - **MSGFPlus:** Run MSGFPlus in a concatenated target-decoy search, with the
-        `-addFeatures 1` flag.
-        - **MaxQuant:**
-          - Run MaxQuant without FDR filtering (set to 1)
-          - MaxQuant requires additional options in the configuration file:
-            - `modification_mapping`: Maps MaxQuant output to MS²PIP modifications list.
-        Keys must contain MaxQuant's two-letter modification codes and values must match
-        one of the modifications listed in the MS²PIP configuration (see
-        [MS2PIP config](#MS2PIP)).
-            - `fixed_modifications`: Must list all modifications set as fixed during the
-        MaxQuant search (as this is not denoted in the msms.txt file). Keys refer to the
-        amino acid, values to the modification name used in the MS²PIP configuration.
-            - The maxquant specific configuration could for example be:
-              ```json
-              "maxquant_to_rescore": {
-                "modification_mapping":{
-                  "ox":"Oxidation",
-                  "cm":"Carbamidomethyl"
-                },
-                "fixed_modifications":{
-                  "C":"Carbamidomethyl"
-                }
-              ```
-        
-        As a general rule, MS²Rescore always needs access to all target and decoy PSMs, not
-        only the FDR-filtered targets.
-        
-        
-        ### Output
-        Several intermediate files are created when the entire pipeline is run. These can be
-        accessed by specifying the `tmp_dir` or `Temporary file directory` option. Depending on whether or not Percolator is
-        run, the following output files can be expected:
-        
-        For each feature set combination (e.g. [`rt`, `ms2pip`, `searchengine`]):
-        - `<file>.pin` Percolator IN file
-        - `<file>.pout` Percolator OUT file with target PSMs
-        - `<file>.pout_dec` Percolator OUT file with decoy PSMs
-        - `<file>.weights` Internal feature weights used by Percolator's scoring function.
-        
-        ---
-        
-        ## Contributing
-        Bugs, questions or suggestions? Feel free to post an issue in the
-        [issue tracker](https://github.com/compomics/ms2rescore/issues/) or to make a pull
-        request!
-        
-Keywords: MS2Rescore,MS2PIP,DeepLC,Percolator,Proteomics,peptide,peak intensity prediction,spectrum,machine learning
-Platform: UNKNOWN
+Keywords: MS2Rescore,MS2PIP,DeepLC,Percolator,proteomics,mass spectrometry,peptide identification,rescoring,machine learning
+Author: Ana Sílvia C. Silva, Robbin Bouwmeester, Louise Buur
+Author-email: Ralf Gabriels <ralf@gabriels.dev>, Arthur Declercq <arthur.declercq@ugent.be>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: gui
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Dist: numpy>=1.16.0,<2
+Requires-Dist: pandas>=0.24.0,<3
+Requires-Dist: rich>=12
+Requires-Dist: pyteomics>=4.1.0,<5
+Requires-Dist: lxml>=4.5,<5
+Requires-Dist: ms2pip>=4.0.0-dev,<5
+Requires-Dist: click>=7
+Requires-Dist: cascade-config>=0.3.0,<2
+Requires-Dist: deeplc>=1.2.1
+Requires-Dist: deeplcretrainer==0.1.17
+Requires-Dist: tomlkit
+Requires-Dist: psm_utils>=0.3
+Requires-Dist: customtkinter>=5,<6
+Requires-Dist: ruff ; extra == "dev"
+Requires-Dist: black ; extra == "dev"
+Requires-Dist: pytest ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: sphinx ; extra == "doc"
+Requires-Dist: numpydoc>=1,<2 ; extra == "doc"
+Requires-Dist: recommonmark ; extra == "doc"
+Requires-Dist: sphinx-mdinclude ; extra == "doc"
+Requires-Dist: toml ; extra == "doc"
+Requires-Dist: semver>=2 ; extra == "doc"
+Requires-Dist: sphinx_rtd_theme ; extra == "doc"
+Requires-Dist: sphinx-autobuild ; extra == "doc"
+Requires-Dist: matplotlib>=3 ; extra == "plotting"
+Requires-Dist: seaborn>=0.11 ; extra == "plotting"
+Project-URL: CompOmics, https://www.compomics.com
+Project-URL: GitHub, https://github.com/compomics/ms2rescore
+Project-URL: PyPi, https://pypi.org/project/ms2rescore/
+Project-URL: ReadTheDocs, https://ms2rescore.readthedocs.io
+Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: plotting
+
+<img src="https://github.com/compomics/ms2rescore/raw/master/img/ms2rescore_logo.png" width="150" height="150" />
+<br/><br/>
+
+[![GitHub release](https://img.shields.io/github/release-pre/compomics/ms2rescore.svg?style=flat-square)](https://github.com/compomics/ms2rescore/releases)
+[![PyPI](https://flat.badgen.net/pypi/v/ms2rescore)](https://pypi.org/project/ms2rescore/)
+[![GitHub Workflow Status](https://flat.badgen.net/github/checks/compomics/ms2rescore/master)](https://github.com/compomics/ms2rescore/actions/)
+[![GitHub issues](https://img.shields.io/github/issues/compomics/ms2rescore?style=flat-square)](https://github.com/compomics/ms2rescore/issues)
+[![GitHub](https://img.shields.io/github/license/compomics/ms2rescore.svg?style=flat-square)](https://www.apache.org/licenses/LICENSE-2.0)
+[![Last commit](https://flat.badgen.net/github/last-commit/compomics/ms2rescore)](https://github.com/compomics/ms2rescore/commits/)
+[![Twitter](https://flat.badgen.net/twitter/follow/compomics?icon=twitter)](https://twitter.com/compomics)
+
+
+Sensitive peptide identification rescoring with predicted spectra using
+[MS²PIP](https://github.com/compomics/ms2pip_c),
+[DeepLC](https://github.com/compomics/deeplc), and
+[Percolator](https://github.com/percolator/percolator/).
+
+---
+
+- [About MS²Rescore](#about-msrescore)
+- [Installation](#installation)
+  - [Python package](#python-package)
+  - [Windows installer](#windows-installer)
+- [Usage](#usage)
+  - [GUI](#gui)
+  - [Command line interface](#command-line-interface)
+  - [Configuration file](#configuration-file)
+  - [Notes for specific search engines](#notes-for-specific-search-engines)
+  - [Output](#output)
+  - [Plotting](#plotting)
+- [Contributing](#contributing)
+
+---
+
+## About MS²Rescore
+
+MS²Rescore performs sensitive peptide identification rescoring with predicted
+spectra using [MS²PIP](https://github.com/compomics/ms2pip_c),
+[DeepLC](https://github.com/compomics/deeplc), and
+[Percolator](https://github.com/percolator/percolator/). This results in more confident
+peptide identifications, which allows you to get **more peptide IDs** at the same false
+discovery rate (FDR) threshold, or to set a **more stringent FDR threshold** while still
+retaining a similar number of peptide IDs. MS²Rescore is **ideal for challenging
+proteomics identification workflows**, such as proteogenomics, metaproteomics, or
+immunopeptidomics.
+
+MS²Rescore uses identifications from a
+[Percolator IN (PIN) file](https://github.com/percolator/percolator/wiki/Interface#tab-delimited-file-format),
+or from the output of one of these search engines:
+
+- [MaxQuant](https://www.maxquant.org/): Start from `msms.txt` identification
+  file and directory with `.mgf` files.
+- [MSGFPlus](https://omics.pnl.gov/software/ms-gf): Start with an `.mzid`
+  identification file and corresponding `.mgf`.
+- [X!Tandem](https://www.thegpm.org/tandem/): Start with an X!Tandem `.xml`
+  identification file and corresponding `.mgf`.
+- [PEAKS](https://www.bioinfor.com/peaksdb/): Start with an `.mzid` identification
+  file and directory with `.mgf` files.
+- [PeptideShaker](http://compomics.github.io/projects/peptide-shaker): Start with a
+  PeptideShaker Extended PSM Report and corresponding `.mgf` file.
+
+<br>
+
+If you use MS²Rescore, please cite the following article:
+> **MS2Rescore: Data-driven rescoring dramatically boosts immunopeptide identification rates.**  \
+Arthur Declercq, Robbin Bouwmeester, Sven Degroeve, Lennart Martens, and Ralf Gabriels.  \
+_bioRxiv_ (2021) [doi:10.1101/2021.11.02.466886](https://doi.org/10.1101/2021.11.02.466886)
+
+<br>
+
+The concept of rescoring with predicted spectrum features was first described in:
+
+> **Accurate peptide fragmentation predictions allow data driven approaches to replace
+and improve upon proteomics search engine scoring functions.**  \
+Ana S C Silva, Robbin Bouwmeester, Lennart Martens, and Sven Degroeve.  \
+_Bioinformatics_ (2019) [doi:10.1093/bioinformatics/btz383](https://doi.org/10.1093/bioinformatics/btz383)
+
+To replicate the experiments described in this article, check out the
+[pub branch](https://github.com/compomics/ms2rescore/tree/pub) of this repository.
+
+---
+
+## Installation
+
+### Python package
+
+[![install pip](https://flat.badgen.net/badge/install%20with/pip/green?icon=pypi)](https://pypi.org/project/ms2rescore/)
+
+
+MS²Rescore requires:
+- Python 3.7 or 3.8 on Linux, macOS, or Windows
+- If the option `run_percolator` is set to `True`,
+[Percolator](https://github.com/percolator/percolator/) needs to be installed and
+callable with the `percolator` command (tested with v3.02.1)
+- Some pipelines require the Percolator converters, such as `tandem2pin`, as well. These
+are usually installed alongside Percolator.
+
+Minimal installation:
+```sh
+pip install ms2rescore
+```
+
+Installation including dependencies for the graphical user interface:
+```sh
+pip install ms2rescore[gui]
+```
+
+We highly recommend using a [venv](https://docs.python.org/3/library/venv.html) or
+[conda](https://docs.conda.io/en/latest/) virtual environment.
+
+
+### Windows installer
+[![get for windows](https://flat.badgen.net/badge/install%20for/windows/blue?icon=windows)](https://github.com/compomics/ms2rescore/releases)
+
+1. Download and install [Percolator](https://github.com/percolator/percolator/releases/latest)
+and the percolator-converters. Make sure to select "Add percolator to the system PATH
+for all users" during setup.
+2. Download the zip file from the [latest release](https://github.com/compomics/ms2rescore/releases)
+and unzip.
+3. Run `install-gui-windows.bat` to install Python and MS²Rescore.
+4. Run `start-gui-windows.bat` to start the MS²Rescore GUI.
+
+If Microsoft Defender SmartScreen displays a warning, click "More info" and then click
+"Run anyway". When starting the GUI, don't mind the terminal window that opens next
+to the GUI.
+
+To install a newer version of MS²Rescore, run `upgrade-gui-windows.bat`.
+
+---
+
+## Usage
+
+### GUI
+
+Run `start-gui-windows.bat` or run `ms2rescore-gui` or
+`python -m ms2rescore.gui`in your terminal to start the graphical user
+interface. Most common settings can be configured through the
+UI. For some advanced settings, see [Configuration file](#configuration-file).
+
+<img src="img/gui-screenshot.png" height=480 />
+
+
+### Command line interface
+
+Run MS²Rescore from the command line as follows:
+
+```
+ms2rescore -c <path-to-config-file> -m <path-to-mgf> <path-to-identification-file>
+```
+
+Run `ms2rescore --help` to see all command line options.
+
+### Configuration file
+
+Although most options can be configered through the CLI and the GUI, MS²Rescore can be
+further configured through a **JSON configuration file**. A correct configuration is
+required to, for example, correctly parse the peptide modifications from the search
+engine output. If no configuration file is passed, or some options are not configured,
+the
+[default values](https://github.com/compomics/ms2rescore/blob/master/ms2rescore/package_data/config_default.json)
+for these settings will be used. Options passed from the CLI and the GUI will override
+the configuration file. The full configuration is validated against a
+[JSON Schema](https://github.com/compomics/ms2rescore/blob/master/ms2rescore/package_data/config_schema.json).
+
+A full example configuration file can be found in
+[ms2rescore/package_data/config_default.json](https://github.com/compomics/ms2rescore/blob/master/ms2rescore/package_data/config_default.json).
+
+The config file contains three top level categories (`general`, `ms2pip` and
+`percolator`) and an additional categories for specific search engines
+(e.g. `maxquant`). The most important options in `general` are:
+- **`pipeline`** *(string)*: Pipeline to use, depending on input format. Must be one of:
+`['infer', 'pin', 'tandem', 'maxquant', 'msgfplus', 'peptideshaker']`. Default: `infer`.
+- **`feature_sets`** *(array)*: Feature sets for which to generate PIN files and optionally run Percolator. Default: `['searchengine', 'rt', 'ms2pip']`.
+    - **Items** *(array)*
+      - **Items** *(string)*: Must be one of: `['searchengine', 'rt', 'ms2pip']`.
+
+An overview of all options can be found in [configuration.md](https://github.com/compomics/ms2rescore/blob/master/configuration.md)
+
+### Notes for specific search engines
+
+- **MSGFPlus:** Run MSGFPlus in a concatenated target-decoy search, with the
+`-addFeatures 1` flag.
+- **MaxQuant:**
+  - Run MaxQuant without FDR filtering (set to 1)
+  - MaxQuant requires additional options in the configuration file:
+    - `modification_mapping`: Maps MaxQuant output to MS²PIP modifications list.
+Keys must contain MaxQuant's two-letter modification codes and values must match
+one of the modifications listed in the MS²PIP configuration (see
+[MS2PIP config](#MS2PIP)).
+    - `fixed_modifications`: Must list all modifications set as fixed during the
+MaxQuant search (as this is not denoted in the msms.txt file). Keys refer to the
+amino acid, values to the modification name used in the MS²PIP configuration.
+    - The maxquant specific configuration could for example be:
+      ```json
+      "maxquant_to_rescore": {
+        "modification_mapping":{
+          "ox":"Oxidation",
+          "cm":"Carbamidomethyl"
+        },
+        "fixed_modifications":{
+          "C":"Carbamidomethyl"
+        }
+      ```
+
+As a general rule, MS²Rescore always needs access to all target and decoy PSMs, not
+only the FDR-filtered targets.
+
+
+### Output
+Several intermediate files are created when the entire pipeline is run. These can be
+accessed by specifying the `tmp_dir` or `Temporary file directory` option. Depending on whether or not Percolator is
+run, the following output files can be expected:
+
+For each feature set combination (e.g. [`rt`, `ms2pip`, `searchengine`]):
+- `<file>.pin` Percolator IN file
+- `<file>_target_psms.pout` Percolator OUT file with target PSMs
+- `<file>_decoy_psms.pout` Percolator OUT file with decoy PSMs
+- `<file>_target_peptides.pout` Percolator OUT file with target peptides
+- `<file>_decoy_peptides.pout` Percolator OUT file with decoy peptides
+- `<file>.weights` Internal feature weights used by Percolator's scoring function.
+
+### Plotting
+When running MS²Rescore you can automatically generate plots (pdf) by setting the plotting parameter in the config to `True.
+Generaly these plots show (unique) identifications for 1% and 0.1% FDR 
+and the percolator weights for the first feature set combination. 
+You can also use the CLI create these plots as follows:
+```
+ms2rescore-plotting <path-to-pin-file> 
+-p <path-to-pout-file> 
+-d <path-to-pout_dec-file> 
+-f <feature-sets-used> 
+-s <pin-file-score-column-name>
+```
+
+Run `ms2rescore-plotting --help` to see all command line options.
+
+If you want to compare MS²Rescore runs with different features sets you can add multiple -p -d and -f flags as follows:
+```
+ms2rescore-plotting <path-to-pin-file> 
+-p <path-to-first-pout-file> -p <path-to-second-pout-file> 
+-d <path-to-first-pout_dec-file> -d <path-to-second-pout_dec-file> 
+-f <first-feature-sets-used> -f <second-feature-sets-used>  
+-s <pin-file-score-column-name>
+```
+
+The pin files are the same for the same MS²Rescore files are be the same in terms of identifications so only one pin file is needed.
+
+---
+## Contributing
+Bugs, questions or suggestions? Feel free to post an issue in the
+[issue tracker](https://github.com/compomics/ms2rescore/issues/) or to make a pull
+request!
+
```

### Comparing `ms2rescore-2.1.3/README.md` & `ms2rescore-3.0.0.dev1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   - [Windows installer](#windows-installer)
 - [Usage](#usage)
   - [GUI](#gui)
   - [Command line interface](#command-line-interface)
   - [Configuration file](#configuration-file)
   - [Notes for specific search engines](#notes-for-specific-search-engines)
   - [Output](#output)
+  - [Plotting](#plotting)
 - [Contributing](#contributing)
 
 ---
 
 ## About MS²Rescore
 
 MS²Rescore performs sensitive peptide identification rescoring with predicted
@@ -208,17 +209,44 @@
 ### Output
 Several intermediate files are created when the entire pipeline is run. These can be
 accessed by specifying the `tmp_dir` or `Temporary file directory` option. Depending on whether or not Percolator is
 run, the following output files can be expected:
 
 For each feature set combination (e.g. [`rt`, `ms2pip`, `searchengine`]):
 - `<file>.pin` Percolator IN file
-- `<file>.pout` Percolator OUT file with target PSMs
-- `<file>.pout_dec` Percolator OUT file with decoy PSMs
+- `<file>_target_psms.pout` Percolator OUT file with target PSMs
+- `<file>_decoy_psms.pout` Percolator OUT file with decoy PSMs
+- `<file>_target_peptides.pout` Percolator OUT file with target peptides
+- `<file>_decoy_peptides.pout` Percolator OUT file with decoy peptides
 - `<file>.weights` Internal feature weights used by Percolator's scoring function.
 
----
+### Plotting
+When running MS²Rescore you can automatically generate plots (pdf) by setting the plotting parameter in the config to `True.
+Generaly these plots show (unique) identifications for 1% and 0.1% FDR 
+and the percolator weights for the first feature set combination. 
+You can also use the CLI create these plots as follows:
+```
+ms2rescore-plotting <path-to-pin-file> 
+-p <path-to-pout-file> 
+-d <path-to-pout_dec-file> 
+-f <feature-sets-used> 
+-s <pin-file-score-column-name>
+```
 
+Run `ms2rescore-plotting --help` to see all command line options.
+
+If you want to compare MS²Rescore runs with different features sets you can add multiple -p -d and -f flags as follows:
+```
+ms2rescore-plotting <path-to-pin-file> 
+-p <path-to-first-pout-file> -p <path-to-second-pout-file> 
+-d <path-to-first-pout_dec-file> -d <path-to-second-pout_dec-file> 
+-f <first-feature-sets-used> -f <second-feature-sets-used>  
+-s <pin-file-score-column-name>
+```
+
+The pin files are the same for the same MS²Rescore files are be the same in terms of identifications so only one pin file is needed.
+
+---
 ## Contributing
 Bugs, questions or suggestions? Feel free to post an issue in the
 [issue tracker](https://github.com/compomics/ms2rescore/issues/) or to make a pull
 request!
```

### Comparing `ms2rescore-2.1.3/ms2rescore/config_parser.py` & `ms2rescore-3.0.0.dev1/ms2rescore/ms2rescore_main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,205 +1,155 @@
-"""Parse configuration from command line arguments and configuration files."""
-
-import argparse
-import json
-import multiprocessing as mp
-import os
+import logging
 import re
+import subprocess
+from multiprocessing import cpu_count
+from pathlib import Path
 from typing import Dict, Optional
 
-from cascade_config import CascadeConfig
+import psm_utils.io
+from rich.console import Console
 
-from ms2rescore import package_data
-from ms2rescore._exceptions import MS2RescoreConfigurationError
-from ms2rescore._version import __version__
-
-try:
-    import importlib.resources as pkg_resources
-except ImportError:
-    import importlib_resources as pkg_resources
-
-
-def _parse_arguments() -> argparse.Namespace:
-    """Parse CLI arguments."""
-    parser = argparse.ArgumentParser(
-        description="MS²ReScore: Sensitive PSM rescoring with predicted MS²\
-            peak intensities."
-    )
-    parser.add_argument("-v", "--version", action="version", version=__version__)
-    parser.add_argument(
-        "identification_file",
-        type=str,
-        help="path to identification file (pin, mzid, msms.txt, tandem xml...)",
-    )
-    parser.add_argument(
-        "-m",
-        metavar="FILE",
-        action="store",
-        type=str,
-        dest="mgf_path",
-        help="path to MGF file or directory with MGF files (default: derived from\
-            identification file)",
-    )
-    parser.add_argument(
-        "-c",
-        metavar="FILE",
-        action="store",
-        type=str,
-        dest="config_file",
-        help="path to MS²ReScore configuration file (see README.md)",
-    )
-    parser.add_argument(
-        "-t",
-        metavar="PATH",
-        action="store",
-        type=str,
-        dest="tmp_path",
-        help="path to directory to place temporary files"
-    )
-    parser.add_argument(
-        "-o",
-        metavar="FILE",
-        action="store",
-        type=str,
-        dest="output_filename",
-        help="name for output files (default: derive from identification file)",
-    )
-    parser.add_argument(
-        "-l",
-        metavar="LEVEL",
-        action="store",
-        type=str,
-        dest="log_level",
-        default="info",
-        help="logging level (default: `info`)",
-    )
-    parser.add_argument(
-        "-n",
-        metavar="VALUE",
-        action="store",
-        type=int,
-        dest="num_cpu",
-        default=None,
-        help="number of cpus available to MS²Rescore",
-    )
-    parser.add_argument(
-        "--pipeline",
-        metavar="PIPELINE",
-        action="store",
-        type=str,
-        dest="pipeline",
-        default=None,
-        help="determines which pipeline to use (default: 'infer')",
-    )
-    parser.add_argument(
-        "--percolator",
-        metavar="BOOL",
-        action="store",
-        type=bool,
-        dest="run_percolator",
-        default=None,
-        help="run percolator (default: 'True')",
-    )
-    parser.add_argument(
-        "--plotting",
-        metavar="BOOL",
-        action="store",
-        type=bool,
-        dest="plotting",
-        default=None,
-        help="write PDF with result plots",
-    )
-    return parser.parse_args()
-
-
-def _validate_filenames(config: Dict) -> Dict:
-    """Validate and infer input/output filenames."""
-    # identification_file should exist
-    id_file = config["general"]["identification_file"]
-    if not os.path.isfile(id_file):
-        raise FileNotFoundError(id_file)
-
-    # MGF path should either be None, or existing path to file or dir
-    mgf_path = config["general"]["mgf_path"]
-    if mgf_path:
-        if not os.path.exists(mgf_path):
-            raise FileNotFoundError(mgf_path)
-
-    # Output filename should be None or its path should exist. If not, make path.
-    if config["general"]["output_filename"]:
-        output_path = os.path.abspath(config["general"]["output_filename"])
-        if not os.path.isdir(output_path):
-            os.makedirs(output_path, exist_ok=True)
-    else:
-        config["general"]["output_filename"] = os.path.splitext(id_file)[0]
-
-    return config
-
-
-def _validate_num_cpu(config: Dict) -> Dict:
-    """Validate requested num_cpu with available cpu count."""
-    n_available = mp.cpu_count()
-    if (config["general"]["num_cpu"] == -1) or (
-        config["general"]["num_cpu"] > n_available
-    ):
-        config["general"]["num_cpu"] = n_available
-    return config
+from ms2rescore import setup_logging
+from ms2rescore.config_parser import parse_config
+from ms2rescore.exceptions import MS2RescoreConfigurationError, MS2RescoreError
+from ms2rescore.feature_generators.deeplc import DeepLCFeatureGenerator
+from ms2rescore.feature_generators.intensity import MS2PIPFeatureGenerator
+from ms2rescore.feature_generators.maxquant import MaxquantFeatureGenerator
+from ms2rescore.rescoring_engines.percolator import PercolatorRescoring
 
+logger = logging.getLogger(__name__)
+
+id_file_parser = None
+
+FEATURE_GENERATORS = {
+    "ms2pip": MS2PIPFeatureGenerator,
+    "deeplc": DeepLCFeatureGenerator,
+    "maxquant": MaxquantFeatureGenerator,
+}
 
-def parse_config(parse_cli_args: bool = True, config_class: Optional[Dict] = None) -> Dict:
-    """
-    Parse and validate MS²ReScore configuration files and arguments.
 
-    Default configuration, user configuration files, and CLI/class arguments are parsed
-    in cascading order.
+class MS2Rescore:
+    """
+    MS²Rescore: Sensitive PSM rescoring with predicted MS² peak intensities and RTs.
 
     Parameters
     ----------
-    parse_cli_args : bool
-        parse command line arguments or not, default True
-    config_class : Dict
-        dictionary with arguments from the Python class; required if `parse_cli_args`
-        is False
+    parse_cli_args : bool, optional
+        parse command line arguments, default True
+    configuration : dict, optional
+        dict containing general ms2rescore configuration; should at least contain
+        `identification_file`; required if `parse_cli_args` is False
+    set_logger : bool, optional
+        set custom logger or not, default False
     """
-    config_schema = pkg_resources.open_text(package_data, "config_schema.json")
-    config_default = pkg_resources.open_text(package_data, "config_default.json")
 
-    # MS²ReScore can be run from the CLI, or as a Python module
-    if parse_cli_args:
-        args = _parse_arguments()
-        config_user = args.config_file
-        if config_class:
-            raise MS2RescoreConfigurationError(
-                "If `parse_cli_args` is True, `config_class` must be None."
+    def __init__(
+        self,
+        parse_cli_args: bool = True,
+        configuration: Optional[Dict] = None,
+        set_logger: bool = False,
+        rich_console: Optional[Console] = None,
+    ) -> None:
+        """Initialize MS2ReScore object."""
+        self.config = parse_config(parse_cli_args=parse_cli_args, config_class=configuration)
+        # Set output and temporary paths
+        self.output_path = self.config["ms2rescore"]["output_path"]
+        self.output_file_root = str(
+            Path(self.output_path) / Path(self.config["ms2rescore"]["psm_file"]).stem
+        )
+        self.tmp_path = self.config["ms2rescore"]["tmp_path"]
+        self.tmp_file_root = str(
+            Path(self.tmp_path) / Path(self.config["ms2rescore"]["psm_file"]).stem
+        )
+
+        # Set logger
+        self._rich_console = rich_console or Console(record=True)
+        self.log_level = self.config["ms2rescore"]["log_level"]
+        if set_logger:
+            setup_logging.setup_logging(
+                self.log_level,
+                log_file=self.output_file_root + "-ms2rescore-log.txt",
+                rich_console=self._rich_console,
             )
-    elif config_class:
-        args = None
-        config_user = config_class["general"]["config_file"]
-    else:
-        raise MS2RescoreConfigurationError(
-            "If `parse_cli_args` is False, `config_class` arguments are required."
+
+        logger.debug(
+            "Using %i of %i available CPUs.",
+            self.config["ms2rescore"]["processes"],
+            cpu_count(),
         )
 
-    cascade_conf = CascadeConfig(validation_schema=json.load(config_schema))
-    cascade_conf.add_dict(json.load(config_default))
-    if config_user:
-        cascade_conf.add_json(config_user)
-    if parse_cli_args:
-        cascade_conf.add_namespace(args, subkey="general")
-    elif config_class:
-        cascade_conf.add_dict(config_class)
-    config = cascade_conf.parse()
-
-    config = _validate_filenames(config)
-    config = _validate_num_cpu(config)
-
-    config["general"]["pipeline"] = config["general"]["pipeline"].lower()
-
-    try:
-        config["maxquant_to_rescore"]["mgf_title_pattern"] = re.compile(config["maxquant_to_rescore"]["mgf_title_pattern"])
-    except re.error:
-        raise MS2RescoreConfigurationError(
-            "Invalid regex pattern, please provide valid regex patttern"
+    def run(self):
+        # Read PSMs
+        logger.info("Reading PSMs...")
+        psm_list = psm_utils.io.read_file(
+            self.config["ms2rescore"]["psm_file"],
+            filetype=self.config["ms2rescore"]["psm_file_type"],
+            show_progressbar=True,
         )
 
-    return config
+        logger.debug("Finding decoys...")
+        if self.config["ms2rescore"]["id_decoy_pattern"]:
+            psm_list.find_decoys(self.config["ms2rescore"]["id_decoy_pattern"])
+        n_psms = len(psm_list)
+        percent_decoys = sum(psm_list["is_decoy"]) / n_psms * 100
+        logger.info(f"Found {n_psms} PSMs, of which {percent_decoys:.2f}% are decoys.")
+        if not any(psm_list["is_decoy"]):
+            raise MS2RescoreConfigurationError(
+                "No decoy PSMs found. Please check if decoys are present in the PSM file and that "
+                "the `id_decoy_pattern` option is correct."
+            )
+
+        logger.debug("Parsing modifications...")
+        psm_list.rename_modifications(self.config["ms2rescore"]["modification_mapping"])
+        psm_list.add_fixed_modifications(self.config["ms2rescore"]["fixed_modifications"])
+        psm_list.apply_fixed_modifications()
+
+        logger.debug("Applying `psm_id_pattern`...")
+        if self.config["ms2rescore"]["psm_id_pattern"]:
+            pattern = re.compile(self.config["ms2rescore"]["psm_id_pattern"])
+
+            def _match_ids(old_id):
+                match = re.search(pattern, str(old_id))
+                try:
+                    return match[1]
+                except (TypeError, IndexError):
+                    raise MS2RescoreError(
+                        "`psm_id_pattern` could not be matched to all PSM spectrum IDs."
+                        " Are you sure that the regex contains a capturing group?"
+                    )
+
+            new_ids = [_match_ids(old_id) for old_id in psm_list["spectrum_id"]]
+            psm_list["spectrum_id"] = new_ids
+
+        psm_list["spectrum_id"] = [str(spec_id) for spec_id in psm_list["spectrum_id"]]
+        
+        for feature_generator in self.config["ms2rescore"]["feature_generators"]:
+            FEATURE_GENERATORS[feature_generator](config=self.config).add_features(psm_list)
+            psm_list = psm_list[psm_list["rescoring_features"] != None]
+
+        if self.config["ms2rescore"]["USI"]:
+            logging.debug(f"Creating USIs for {len(psm_list)} PSMs")
+            psm_list["spectrum_id"] = [psm.get_usi(as_url=False) for psm in psm_list]
+
+        logging.debug(f"Writing {self.output_file_root}.pin file")
+        if self.config["ms2rescore"]["rescoring_engine"] == "percolator":
+            percolator = PercolatorRescoring(psm_list, self.config)
+            percolator.rescore()
+
+    @staticmethod
+    def _validate_cli_dependency(command):
+        """Validate that command returns zero exit status."""
+        if subprocess.getstatusoutput(command)[0] != 0:
+            logger.critical(
+                "`%s` returned non-zero exit status. Please verify installation.",
+                command,
+            )
+            exit(1)
+
+    def save_log(self) -> None:
+        """Save full rich-text log to HTML."""
+        if self._rich_console:
+            self._rich_console.save_html(
+                self.output_file_root + "-ms2rescore-log.html",
+            )
+        else:
+            logger.warning("Could not write logs to HTML: rich console is not defined.")
```

### Comparing `ms2rescore-2.1.3/ms2rescore/package_data/config_schema.json` & `ms2rescore-3.0.0.dev1/ms2rescore/package_data/config_schema.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'description'": "'MS²Rescore JSON configuration file.'",*

 * * "'properties'": "{replace: OrderedDict([('ms2rescore', OrderedDict([('description', 'General "*

 * *                 "MS²Rescore settings.'), ('type', 'object'), ('additionalProperties', False), "*

 * *                 "('properties', OrderedDict([('feature_generators', OrderedDict([('description', "*

 * *                 "'Feature generators to use.'), ('type', 'array'), ('items', "*

 * *                 "OrderedDict([('type', 'string'), ('enum', ['ms2pip', 'deeplc', […]*

```diff
@@ -1,252 +1,244 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "MS\u00b2ReScore JSON configuration file.",
+    "description": "MS\u00b2Rescore JSON configuration file.",
     "properties": {
-        "definitions": {
-            "modifications": {
-                "additionalProperties": false,
-                "description": "Peptide mass modifications, per amino acid",
-                "properties": {
-                    "amino_acid": {
-                        "description": "Amino acid one-letter code, or null if amino acid-agnostic (e.g. N-term acetylation)",
-                        "oneOf": [
-                            {
-                                "maxLength": 1,
-                                "minLength": 1,
-                                "type": "string"
-                            },
-                            {
-                                "type": "null"
-                            }
-                        ]
-                    },
-                    "c_term": {
-                        "description": "Modification is C-terminal (only implemented for MSGF+ mzid and Percolator PIN input formats)",
-                        "type": "boolean"
-                    },
-                    "mass_shift": {
-                        "description": "Mono-isotopic mass shift",
-                        "type": "number"
-                    },
-                    "n_term": {
-                        "description": "Modification is N-terminal",
-                        "type": "boolean"
-                    },
-                    "name": {
-                        "description": "Unique name for modification",
-                        "type": "string"
-                    },
-                    "unimod_accession": {
-                        "description": "Unimod accession of modification",
-                        "multipleOf": 1,
-                        "type": "number"
-                    }
-                },
-                "required": [
-                    "name",
-                    "unimod_accession",
-                    "mass_shift",
-                    "amino_acid",
-                    "n_term",
-                    "c_term"
-                ],
-                "type": "object"
-            }
+        "deeplc": {
+            "additionalProperties": true,
+            "description": "DeepLC keyword arguments",
+            "properties": {
+                "calibration_set_size": {
+                    "default": 0.15,
+                    "description": "Calibration set size",
+                    "oneOf": [
+                        {
+                            "type": "integer"
+                        },
+                        {
+                            "type": "number"
+                        }
+                    ]
+                }
+            },
+            "type": "object"
         },
-        "general": {
+        "ms2pip": {
             "additionalProperties": false,
-            "description": "General MS\u00b2ReScore settings.",
-            "maxquant_to_rescore": {
-                "additionalProperties": false,
-                "description": "Settings specific to the MaxQuant pipeline",
-                "properties": {
-                    "fixed_modifications": {
-                        "default": {},
-                        "description": "Mapping of amino acids with fixed modifications to the modification name",
-                        "type": "object"
-                    },
-                    "mgf_title_pattern": {
-                        "default": "TITLE=.*scan=([0-9]+).*$",
-                        "description": "regex pattern to extract index or scan number from maxquant mgf TITLE field",
-                        "format": "regex",
-                        "type": "string"
-                    },
-                    "modification_mapping": {
-                        "default": {},
-                        "description": "Mapping of MaxQuant modification labels to modifications names for MS\u00b2PIP",
-                        "type": "object"
-                    }
-                },
-                "required": [
-                    "modification_mapping",
-                    "fixed_modifications"
-                ],
-                "type": "object"
-            },
-            "ms2pip": {
-                "additionalProperties": false,
-                "description": "MS\u00b2PIP settings.",
-                "properties": {
-                    "frag_error": {
-                        "default": 0.02,
-                        "description": "MS2 error tolerance in Da",
-                        "minimum": 0,
-                        "type": "number"
-                    },
-                    "model": {
-                        "default": "HCD",
-                        "description": "MS\u00b2PIP model to use (see MS\u00b2PIP documentation)",
-                        "type": "string"
-                    },
-                    "modifications": {
-                        "description": "Array of peptide mass modifications",
-                        "items": {
-                            "$ref": "#/definitions/modifications"
-                        },
-                        "type": "array"
-                    }
+            "description": "MS\u00b2PIP settings.",
+            "properties": {
+                "model": {
+                    "default": "HCD",
+                    "description": "MS\u00b2PIP model to use (see MS\u00b2PIP documentation)",
+                    "type": "string"
                 },
-                "type": "object"
-            },
-            "percolator": {
-                "description": "Command line options directly passed to Percolator (see the Percolator wiki)",
-                "type": "object"
+                "ms2_tolerance": {
+                    "default": 0.02,
+                    "description": "MS2 error tolerance in Da",
+                    "minimum": 0,
+                    "type": "number"
+                }
             },
+            "type": "object"
+        },
+        "ms2rescore": {
+            "additionalProperties": false,
+            "description": "General MS\u00b2Rescore settings.",
             "properties": {
+                "USI": {
+                    "description": "Use universal spectrum identifier (USI)",
+                    "type": "boolean"
+                },
                 "config_file": {
                     "description": "Path to configuration file",
                     "oneOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ]
                 },
-                "feature_sets": {
+                "feature_generators": {
                     "default": [
-                        "searchengine",
-                        "rt",
-                        "ms2pip"
+                        "ms2pip",
+                        "deeplc"
                     ],
-                    "description": "Feature sets for which to generate PIN files and optionally run Percolator.",
+                    "description": "Feature generators to use.",
                     "items": {
-                        "items": {
-                            "enum": [
-                                "searchengine",
-                                "rt",
-                                "ms2pip"
-                            ],
-                            "type": "string"
-                        },
-                        "minitems": 1,
-                        "type": "array"
+                        "enum": [
+                            "ms2pip",
+                            "deeplc",
+                            "maxquant"
+                        ],
+                        "type": "string"
                     },
                     "minItems": 1,
                     "type": "array",
                     "uniqueItems": true
                 },
+                "fixed_modifications": {
+                    "additionalProperties": true,
+                    "default": {},
+                    "description": "Mapping of amino acids with fixed modifications to the modification name.",
+                    "type": "object"
+                },
                 "id_decoy_pattern": {
                     "default": null,
-                    "description": "Pattern used to identify the decoy PSMs in identification file. Passed to `--pattern` option of Percolator converters.",
+                    "description": "Regex pattern used to identify the decoy PSMs in identification file.",
                     "oneOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ]
                 },
-                "identification_file": {
-                    "description": "Path to identification file",
-                    "type": "string"
-                },
                 "log_level": {
                     "description": "Logging level",
                     "enum": [
                         "debug",
                         "info",
                         "warning",
                         "error",
                         "critical"
                     ],
                     "type": "string"
                 },
-                "mgf_path": {
-                    "description": "Path to MGF file or directory with MGF files",
+                "lower_score_is_better": {
+                    "default": false,
+                    "description": "Bool indicating if lower score is better",
+                    "type": "boolean"
+                },
+                "modification_mapping": {
+                    "default": {},
+                    "description": "Mapping of modification labels to each replacement label.",
+                    "type": "object"
+                },
+                "output_path": {
+                    "description": "Path and root name for output files",
                     "oneOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ]
                 },
-                "num_cpu": {
+                "processes": {
                     "default": -1,
                     "description": "Number of parallel processes to use; -1 for all available",
                     "minimum": -1,
                     "multipleOf": 1,
                     "type": "number"
                 },
-                "output_filename": {
-                    "description": "Path and root name for output files",
+                "psm_file": {
+                    "description": "Path to file with peptide-spectrum matches.",
                     "oneOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ]
                 },
-                "pipeline": {
+                "psm_file_type": {
                     "default": "infer",
-                    "description": "Pipeline to use, depending on input format",
+                    "description": "PSM file type. By default inferred from file extension.",
+                    "type": "string"
+                },
+                "psm_id_pattern": {
+                    "default": "(.*)",
+                    "description": "Regex pattern to extract index or scan number from PSM file. Requires at least one capturing group.",
+                    "format": "regex",
+                    "oneOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ]
+                },
+                "rescoring_engine": {
+                    "default": "percolator",
+                    "description": "Rescoring engine to use.",
                     "enum": [
-                        "infer",
-                        "pin",
-                        "tandem",
-                        "maxquant",
-                        "msgfplus",
-                        "peptideshaker",
-                        "peaks"
+                        null,
+                        "percolator"
                     ],
-                    "type": "string"
+                    "oneOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ]
                 },
-                "plotting": {
-                    "default": false,
-                    "description": "Output PDF with additional Rescore plots",
-                    "type": "boolean"
+                "spectrum_id_pattern": {
+                    "default": "(.*)",
+                    "description": "Regex pattern to extract index or scan number from spectrum file. Requires at least one capturing group.",
+                    "format": "regex",
+                    "oneOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ]
                 },
-                "run_percolator": {
-                    "default": false,
-                    "description": "Run Percolator within MS\u00b2ReScore",
-                    "type": "boolean"
+                "spectrum_path": {
+                    "description": "Path to spectrum file or directory with spectrum files",
+                    "oneOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ]
                 },
                 "tmp_path": {
                     "description": "Path to directory to place temporary files",
                     "oneOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ]
                 }
             },
             "type": "object"
+        },
+        "percolator": {
+            "additionalProperties": true,
+            "description": "Percolator settings",
+            "properties": {
+                "init-weights": {
+                    "default": false,
+                    "description": "Weights file for scoring function",
+                    "oneOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "boolean"
+                        }
+                    ]
+                }
+            },
+            "type": "object"
         }
     },
     "required": [
-        "general",
-        "ms2pip",
-        "percolator"
+        "ms2rescore"
     ],
-    "title": "MS\u00b2ReScore configuration",
+    "title": "MS\u00b2Rescore configuration",
     "type": "object"
 }
```

### Comparing `ms2rescore-2.1.3/ms2rescore/package_data/img/config_icon.png` & `ms2rescore-3.0.0.dev1/ms2rescore/package_data/img/config_icon.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-2.1.3/ms2rescore/package_data/img/program_icon.ico` & `ms2rescore-3.0.0.dev1/ms2rescore/package_data/img/program_icon.ico`

 * *Files identical despite different names*

### Comparing `ms2rescore-2.1.3/ms2rescore/retention_time.py` & `ms2rescore-3.0.0.dev1/ms2rescore/feature_generators/deeplc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,268 +1,226 @@
-"""Add retention time related features to rescoring."""
+"""DeepLC retention time-based feature generator."""
 
+import contextlib
 import logging
 import os
-from typing import Optional, Union
+from collections import defaultdict
+from itertools import chain
+from pathlib import Path
 
-import click
+import numpy as np
 import pandas as pd
+from psm_utils import PSMList
+from psm_utils.io import peptide_record
 
-from ms2rescore.peptide_record import PeptideRecord
+from ms2rescore.exceptions import MS2RescoreError
+from ms2rescore.feature_generators import FeatureGenerator
+from ms2rescore.parse_mgf import parse_mgf_title_rt
+from ms2rescore.utils import infer_spectrum_path
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
-
-
 logger = logging.getLogger(__name__)
 
 
-class RetentionTimeIntegration:
-    """Retention time integration for MS²ReScore, using DeepLC."""
-
+class DeepLCFeatureGenerator(FeatureGenerator):
     def __init__(
         self,
-        peprec_path: str,
-        feature_path: str,
-        higher_psm_score_better: bool = True,
-        calibration_set_size: Optional[Union[int, float]] = 0.20,
-        num_cpu: Optional[int] = None,
-    ):
+        config,
+        *args,
+        **kwargs,
+    ) -> None:
         """
-        Retention time integration for MS²ReScore, using DeepLC.
+        Generate DeepLC-based features for rescoring.
 
         Parameters
         ----------
-        peprec_path: str
-            Path to PEPREC file with PSMs
-        feature_path: str
-            Path to feature file to write features to.
+        psm_list: psm_utils.PSMList
+            List of PSMs to which to add features.
         higher_psm_score_better: bool
-            Wheter a higher PSM score (`psm_score` column in PEPREC) denotes a better
+            Whether a higher PSM score (`psm_score` column in PEPREC) denotes a better
             score. (default: True)
         calibration_set_size: int or float
             Amount of best PSMs to use for DeepLC calibration. If this value is lower
             than the number of available PSMs, all PSMs will be used. (default: 0.20)
         num_cpu: {int, None}
             Number of processes to use in DeepLC
 
-        Properties
-        ----------
-        calibration_data: pandas.DataFrame
-            Get calibration peptides (N best PSMs in PEPREC).
-        prediction_data: pandas.DataFrame
-            Get prediction peptides.
-
-        Methods
-        -------
-        run()
-            Get retention time predictions for PEPREC and calculate features.
-
         """
-        self.peprec_path = peprec_path
-        self.feature_path = feature_path
-        self.higher_psm_score_better = higher_psm_score_better
-        self.calibration_set_size = calibration_set_size
-        self.num_cpu = num_cpu
-
-        # Until fixed upstream: https://github.com/compomics/DeepLC/issues/19
-        if "NUMEXPR_MAX_THREADS" not in os.environ:
-            os.environ["NUMEXPR_MAX_THREADS"] = str(self.num_cpu)
-
-        self.peprec = None
-        self.feature_df = None
-
-        if self.peprec_path:
-            self.peprec = PeptideRecord(path=self.peprec_path)
-
-    def num_calibration_psms(self, peprec):
-        """Get number of calibration PSMs given `calibration_set_size` and total number of PSMs."""
-        if isinstance(self.calibration_set_size, float):
-            if self.calibration_set_size > 1:
-                raise ValueError("`calibration_set_size` cannot be larger than 1.")
-            elif self.calibration_set_size <= 0:
-                raise ValueError(
-                    "`calibration_set_size` cannot be smaller than or equal to 0."
-                )
-            else:
-                num_calibration_psms = round(
-                    len(peprec) * self.calibration_set_size
-                )
-        elif isinstance(self.calibration_set_size, int):
-            if self.calibration_set_size > len(peprec):
-                logger.warning(
-                    "Requested number of calibration PSMs (%s) is larger than total number "
-                    "of PSMs in PEPREC (%s). Using all PSMs for calibration.",
-                    self.calibration_set_size,
-                    peprec,
-                )
-                num_calibration_psms = len(peprec)
-            else:
-                num_calibration_psms = self.calibration_set_size
-        else:
-            raise TypeError(
-                "Expected float or int for `calibration_set_size`. Got "
-                f"{type(self.calibration_set_size)} instead"
-            )
-        logger.debug("Using %i PSMs for calibration", num_calibration_psms)
-        return num_calibration_psms
-
-    def get_calibration_data(self, peprec):
-        """Get calibration peptides (N best PSMs in PEPREC)."""
-        ascending = not self.higher_psm_score_better
-        if "label" in peprec.columns:
-            label_col = "label"
-        elif "Label" in peprec.columns:
-            label_col = "Label"
-        else:
-            raise ValueError("No label column found in peptide record.")
-        calibration_data = (
-            peprec[peprec[label_col] == 1]
-            .sort_values(["psm_score"], ascending=ascending)
-            .head(self.num_calibration_psms(peprec=peprec))
-            .rename(
-                columns={
-                    "observed_retention_time": "tr",
-                    "peptide": "seq",
-                }
-            )[["tr", "seq", "modifications"]]
-            .copy()
+        super().__init__(*args, **kwargs)
+        self.config = config
+        self.tmp_file_root = str(
+            Path(self.config["ms2rescore"]["tmp_path"])
+            / Path(self.config["ms2rescore"]["psm_file"]).stem
         )
-        return calibration_data
+        self.feature_names = []
+        self.higher_psm_score_better = self.config["ms2rescore"]["lower_score_is_better"]
+        try:
+            self.calibration_set_size = self.config["deeplc"].pop("calibration_set_size")
+        except KeyError:
+            self.calibration_set_size = 0.15
+        self.num_cpu = 1
 
-    def get_prediction_data(self, peprec):
-        """Get prediction peptides."""
-        return peprec[["peptide", "modifications"]].rename(
-            columns={
-                "peptide": "seq",
-            }
-        )
+        if "deeplc_retrain" not in self.config["deeplc"]:
+            self.config["deeplc"]["deeplc_retrain"] = True
 
-    def _calculate_features(self):
-        """Calculate retention time features for rescoring."""
-        # Absolute difference between observed and predicted'
-        self.feature_df = self.peprec.df.copy()
-        self.feature_df["rt_diff"] = (
-            self.feature_df["observed_retention_time"]
-            - self.feature_df["predicted_retention_time"]
-        ).abs()
-
-        # Minimum RT difference for a peptidoform
-        min_rt_diff = self.feature_df[
-            [
-                "peptide",
-                "modifications",
-                "observed_retention_time",
-                "predicted_retention_time",
-                "rt_diff",
-            ]
-        ].copy()
-
-        min_rt_diff = (
-            min_rt_diff.sort_values("rt_diff", ascending=True)
-            .drop_duplicates(subset=["peptide", "modifications"], keep="first")
-            .rename(
-                columns={
-                    "rt_diff": "rt_diff_best",
-                    "observed_retention_time": "observed_retention_time_best",
-                    "predicted_retention_time": "predicted_retention_time_best",
-                }
-            )
-        )
-
-        # Merging minimum RT difference features to full set
-        self.feature_df = self.feature_df.merge(
-            min_rt_diff, on=["peptide", "modifications"], how="left"
-        )
+        self.deeplc_predictor = None
+        self.selected_model = None
 
-        # Only keep feature columns
-        id_columns = ["spec_id", "charge", "peptide", "modifications"]
-        feature_columns = [
+        self.feature_names = [
             "observed_retention_time",
             "predicted_retention_time",
             "rt_diff",
-            "rt_diff_best",
             "observed_retention_time_best",
             "predicted_retention_time_best",
+            "rt_diff_best",
         ]
-        self.feature_df = self.feature_df[id_columns + feature_columns].copy()
-
-    def run(self):
-        """Get retention time predictions for PEPREC and calculate features."""
 
+    def add_features(self, psm_list: PSMList) -> None:
+        """Add DeepLC-derived features to PSMs."""
         from deeplc import DeepLC
 
-        if "Raw file" in self.peprec.df.columns:
-            raw_specific_predicted_dfs = []
-            for i, (raw_file, df) in enumerate(self.peprec.df.groupby("Raw file")):
-                logger.info(f"Calibrating {raw_file}")
-
-                peprec_raw_df = df.copy().reset_index()
-                retention_time_df = pd.DataFrame(
-                    columns=["spec_id", "predicted_retention_time"]
-                )
+        logger.info("Adding DeepLC-derived features to PSMs.")
 
-                if i == 0:
-                    self.deeplc_predictor = DeepLC(
-                        split_cal=10,
-                        n_jobs=self.num_cpu,
-                        cnn_model=True,
-                        verbose=False
-                    )
-                    self.deeplc_predictor.calibrate_preds(
-                        seq_df=self.get_calibration_data(peprec_raw_df)
-                    )
-                    self.deeplc_model = list(self.deeplc_predictor.model.keys())
-                else:
+        # Get easy-access nested version of PSMList
+        psm_dict = psm_list.get_psm_dict()
+        peptide_rt_diff_dict = defaultdict(
+            lambda: {
+                "observed_retention_time_best": np.Inf,
+                "predicted_retention_time_best": np.Inf,
+                "rt_diff_best": np.Inf,
+            }
+        )
+
+        # Run MS²PIP for each spectrum file
+        for collection, runs in psm_dict.items():
+            # Reset DeepLC predictor for each collection of runs
+
+            self.deeplc_predictor = None
+            self.selected_model = None
+            for run, psms in runs.items():
+                logger.info(f"Running DeepLC for PSMs from run `{run}`...")
+                # Prepare PSM file
+                with contextlib.redirect_stdout(open(os.devnull, "w")):
+                    psm_list_run = PSMList(psm_list=list(chain.from_iterable(psms.values())))
+
+                    if not all(psm_list["retention_time"]):
+                        retention_times = psm_list_run["retention_time"]
+                        spec_ids = psm_list_run["retention_time"]
+                        retention_time_dict = self.read_rt_from_spectrum_file(run)
+
+                        try:
+                            # psm_list["retention_time"] = [rt if rt else retention_time_dict[spec_ids[i]] for i, rt in enumerate(retention_times)]
+                            psm_list_run["retention_time"] = [
+                                retention_time_dict[psm_id]
+                                for psm_id in psm_list_run["spectrum_id"]
+                            ]  # Probably faster to replace all
+                        except KeyError:
+                            raise MS2RescoreError(
+                                "Could not map all spectrum ids to retention times"
+                            )
+
+                    psm_list_calibration = self.get_calibration_psms(psm_list_run)
+
+                    logger.debug("Calibrating DeepLC")
                     self.deeplc_predictor = DeepLC(
-                        split_cal=10,
                         n_jobs=self.num_cpu,
-                        cnn_model=True,
                         verbose=False,
-                        path_model=self.deeplc_model
+                        path_model=self.selected_model,
+                        **self.config["deeplc"],
                     )
                     self.deeplc_predictor.calibrate_preds(
-                        seq_df=self.get_calibration_data(peprec_raw_df)
+                        seq_df=self._psm_list_to_deeplc_peprec(psm_list_calibration)
                     )
-                predicted_rts = pd.Series(
-                    self.deeplc_predictor.make_preds(
-                        seq_df=self.get_prediction_data(peprec_raw_df)
+                    # Still calibrate for each run, but do not try out all model options.
+                    # Just use model that was selected based on first run
+                    if not self.selected_model:
+                        self.selected_model = list(self.deeplc_predictor.model.keys())
+                        logger.debug(
+                            f"Selected DeepLC model {self.selected_model} based on "
+                            "calibration of first run. Using this model (after new "
+                            "calibrations) for the remaining runs."
+                        )
+
+                    predictions = np.array(
+                        self.deeplc_predictor.make_preds(
+                            seq_df=self._psm_list_to_deeplc_peprec(psm_list_run)
+                        )
                     )
-                )
-                retention_time_df["spec_id"] = peprec_raw_df["spec_id"].copy()
-                retention_time_df["predicted_retention_time"] = predicted_rts
+                    observations = psm_list_run["retention_time"]
+                    rt_diffs_run = np.abs(predictions - observations)
 
-                raw_specific_predicted_dfs.append(retention_time_df)
-            self.peprec.df = pd.merge(
-                self.peprec.df,
-                pd.concat(raw_specific_predicted_dfs, ignore_index=True),
-                on="spec_id",
-                how="inner",
-            )
-        else:
-            self.deeplc_predictor = DeepLC(
-                split_cal=10, n_jobs=self.num_cpu, cnn_model=True, verbose=False
-            )
-            self.deeplc_predictor.calibrate_preds(
-                seq_df=self.get_calibration_data(self.peprec.df)
-            )
-            predicted_rts = pd.Series(
-                self.deeplc_predictor.make_preds(
-                    seq_df=self.get_prediction_data(self.peprec.df)
-                )
-            )
-            self.peprec.df["predicted_retention_time"] = predicted_rts
-
-        self._calculate_features()
-        self.feature_df.to_csv(self.feature_path, index=False)
+                    for i, psm in enumerate(psm_list_run):
+                        psm["rescoring_features"].update(
+                            {
+                                "observed_retention_time": observations[i],
+                                "predicted_retention_time": predictions[i],
+                                "rt_diff": rt_diffs_run[i],
+                            }
+                        )
+                        peptide = psm.peptidoform.proforma.split("\\")[0]  # remove charge
+                        if peptide_rt_diff_dict[peptide]["rt_diff_best"] > rt_diffs_run[i]:
+                            peptide_rt_diff_dict[peptide] = {
+                                "observed_retention_time_best": observations[i],
+                                "predicted_retention_time_best": predictions[i],
+                                "rt_diff_best": rt_diffs_run[i],
+                            }
+
+        for psm in psm_list:
+            psm["rescoring_features"].update(
+                peptide_rt_diff_dict[psm.peptidoform.proforma.split("\\")[0]]
+            )
+
+    def read_rt_from_spectrum_file(self, run_name):
+        # Prepare spectrum filenames
+        spectrum_filename = infer_spectrum_path(
+            self.config["ms2rescore"]["spectrum_path"], run_name
+        )
 
+        return parse_mgf_title_rt(spectrum_filename)
 
-@click.command()
-@click.argument("peprec")
-@click.argument("features")
-def main(**kwargs):
-    """Run ms2rescore.retention_time."""
-    rt = RetentionTimeIntegration(kwargs["peprec"], kwargs["features"])
-    rt.run()
+    # TODO: Remove when DeepLC supports PSMList directly
+    @staticmethod
+    def _psm_list_to_deeplc_peprec(psm_list: PSMList) -> pd.DataFrame:
+        peprec = peptide_record.to_dataframe(psm_list)
+        peprec = peprec.rename(
+            columns={
+                "observed_retention_time": "tr",
+                "peptide": "seq",
+            }
+        )[["tr", "seq", "modifications"]]
+        return peprec
 
+    def get_calibration_psms(self, psm_list: PSMList):
+        """Get N best scoring target PSMs for calibration."""
+        psm_list_targets = psm_list[~psm_list["is_decoy"]]
+        n_psms = self.get_number_of_calibration_psms(psm_list_targets)
+        indices = np.argsort(psm_list_targets["score"])
+        indices = indices[-n_psms:] if self.higher_psm_score_better else indices[:n_psms]
+        return psm_list[indices]
 
-if __name__ == "__main__":
-    main()
+    def get_number_of_calibration_psms(self, psm_list):
+        """Get number of calibration PSMs given `calibration_set_size` and total number of PSMs."""
+        if isinstance(self.calibration_set_size, float):
+            if not 0 < self.calibration_set_size <= 1:
+                raise ValueError(
+                    "If `calibration_set_size` is a float, it cannot be smaller than "
+                    "or equal to 0 or larger than 1."
+                )
+            else:
+                num_calibration_psms = round(len(psm_list) * self.calibration_set_size)
+        elif isinstance(self.calibration_set_size, int):
+            if self.calibration_set_size > len(psm_list):
+                logger.warning(
+                    f"Requested number of calibration PSMs ({self.calibration_set_size}"
+                    f") is larger than total number of PSMs ({len(psm_list)}). Using "
+                    "all PSMs for calibration."
+                )
+                num_calibration_psms = len(psm_list)
+            else:
+                num_calibration_psms = self.calibration_set_size
+        else:
+            raise TypeError(
+                "Expected float or int for `calibration_set_size`. Got "
+                f"{type(self.calibration_set_size)} instead. "
+            )
+        logger.debug(f"Using {num_calibration_psms} PSMs for calibration")
+        return num_calibration_psms
```

