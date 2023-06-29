# Comparing `tmp/pontos-23.6.1.tar.gz` & `tmp/pontos-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.6.1.tar", max compression
+gzip compressed data, was "pontos-23.6.2.tar", max compression
```

## Comparing `pontos-23.6.1.tar` & `pontos-23.6.2.tar`

### file list

```diff
@@ -1,253 +1,253 @@
--rw-r--r--   0        0        0    35149 2023-06-22 07:56:38.365392 pontos-23.6.1/LICENSE
--rw-r--r--   0        0        0     3836 2023-06-22 07:56:38.365392 pontos-23.6.1/README.md
--rw-r--r--   0        0        0   110390 2023-06-22 07:56:38.369392 pontos-23.6.1/poetry.lock
--rw-r--r--   0        0        0       32 2023-06-22 07:56:38.369392 pontos-23.6.1/poetry.toml
--rw-r--r--   0        0        0      791 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9995 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4393 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/git/__init__.py
--rw-r--r--   0        0        0    16153 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     7327 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3561 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/release/main.py
--rw-r--r--   0        0        0     8333 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/release/parser.py
--rw-r--r--   0        0        0    14408 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/release/release.py
--rw-r--r--   0        0        0    12499 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12149 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1596 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2723 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7752 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6445 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_java.py
--rw-r--r--   0        0        0     6263 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     8216 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13439 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2159 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16043 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/version.py
--rw-r--r--   0        0        0     2911 2023-06-22 07:56:38.377392 pontos-23.6.1/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17925 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/git/__init__.py
--rw-r--r--   0        0        0    28296 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     5430 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/test_helper.py
--rw-r--r--   0        0        0     9077 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/test_parser.py
--rw-r--r--   0        0        0    83503 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/test_helper.py
--rw-r--r--   0        0        0     1685 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15848 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    11614 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/commands/test_java.py
--rw-r--r--   0        0        0    15376 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25664 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_version.py
--rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 pontos-23.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-29 09:25:08.849093 pontos-23.6.2/LICENSE
+-rw-r--r--   0        0        0     3836 2023-06-29 09:25:08.849093 pontos-23.6.2/README.md
+-rw-r--r--   0        0        0   110365 2023-06-29 09:25:08.853093 pontos-23.6.2/poetry.lock
+-rw-r--r--   0        0        0       32 2023-06-29 09:25:08.853093 pontos-23.6.2/poetry.toml
+-rw-r--r--   0        0        0      791 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9995 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4393 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     7327 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4732 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2177 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     7339 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2646 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    11470 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3561 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/main.py
+-rw-r--r--   0        0        0     8333 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/parser.py
+-rw-r--r--   0        0        0    14408 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/release.py
+-rw-r--r--   0        0        0    12499 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12149 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1596 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2723 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7752 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6445 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_java.py
+-rw-r--r--   0        0        0     6365 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8216 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13439 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2159 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16043 2023-06-29 09:25:08.861093 pontos-23.6.2/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-06-29 09:25:08.861093 pontos-23.6.2/pontos/version/version.py
+-rw-r--r--   0        0        0     2911 2023-06-29 09:25:08.861093 pontos-23.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17925 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     5430 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/test_helper.py
+-rw-r--r--   0        0        0     9077 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/test_parser.py
+-rw-r--r--   0        0        0    83503 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/test_helper.py
+-rw-r--r--   0        0        0     1685 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15848 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    11614 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_java.py
+-rw-r--r--   0        0        0    17081 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25664 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_version.py
+-rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 pontos-23.6.2/PKG-INFO
```

### Comparing `pontos-23.6.1/LICENSE` & `pontos-23.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/README.md` & `pontos-23.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/poetry.lock` & `pontos-23.6.2/poetry.lock`

 * *Files 0% similar despite different names*

```diff
@@ -770,34 +770,34 @@
 cssselect = ["cssselect (>=0.7)"]
 html5 = ["html5lib"]
 htmlsoup = ["BeautifulSoup4"]
 source = ["Cython (>=0.29.7)"]
 
 [[package]]
 name = "markdown-it-py"
-version = "2.2.0"
+version = "3.0.0"
 description = "Python port of markdown-it. Markdown parsing, done right!"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "markdown-it-py-2.2.0.tar.gz", hash = "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"},
-    {file = "markdown_it_py-2.2.0-py3-none-any.whl", hash = "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30"},
+    {file = "markdown-it-py-3.0.0.tar.gz", hash = "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"},
+    {file = "markdown_it_py-3.0.0-py3-none-any.whl", hash = "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1"},
 ]
 
 [package.dependencies]
 mdurl = ">=0.1,<1.0"
 
 [package.extras]
 benchmarking = ["psutil", "pytest", "pytest-benchmark"]
 code-style = ["pre-commit (>=3.0,<4.0)"]
 compare = ["commonmark (>=0.9,<1.0)", "markdown (>=3.4,<4.0)", "mistletoe (>=1.0,<2.0)", "mistune (>=2.0,<3.0)", "panflute (>=2.3,<3.0)"]
 linkify = ["linkify-it-py (>=1,<3)"]
 plugins = ["mdit-py-plugins"]
 profiling = ["gprof2dot"]
-rtd = ["attrs", "myst-parser", "pyyaml", "sphinx", "sphinx-copybutton", "sphinx-design", "sphinx_book_theme"]
+rtd = ["jupyter_sphinx", "mdit-py-plugins", "myst-parser", "pyyaml", "sphinx", "sphinx-copybutton", "sphinx-design", "sphinx_book_theme"]
 testing = ["coverage", "pytest", "pytest-cov", "pytest-regressions"]
 
 [[package]]
 name = "markupsafe"
 version = "2.1.3"
 description = "Safely add untrusted strings to HTML/XML markup."
 optional = false
@@ -864,29 +864,29 @@
 files = [
     {file = "mccabe-0.7.0-py2.py3-none-any.whl", hash = "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"},
     {file = "mccabe-0.7.0.tar.gz", hash = "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325"},
 ]
 
 [[package]]
 name = "mdit-py-plugins"
-version = "0.3.5"
+version = "0.4.0"
 description = "Collection of plugins for markdown-it-py"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "mdit-py-plugins-0.3.5.tar.gz", hash = "sha256:eee0adc7195e5827e17e02d2a258a2ba159944a0748f59c5099a4a27f78fcf6a"},
-    {file = "mdit_py_plugins-0.3.5-py3-none-any.whl", hash = "sha256:ca9a0714ea59a24b2b044a1831f48d817dd0c817e84339f20e7889f392d77c4e"},
+    {file = "mdit_py_plugins-0.4.0-py3-none-any.whl", hash = "sha256:b51b3bb70691f57f974e257e367107857a93b36f322a9e6d44ca5bf28ec2def9"},
+    {file = "mdit_py_plugins-0.4.0.tar.gz", hash = "sha256:d8ab27e9aed6c38aa716819fedfde15ca275715955f8a185a8e1cf90fb1d2c1b"},
 ]
 
 [package.dependencies]
-markdown-it-py = ">=1.0.0,<3.0.0"
+markdown-it-py = ">=1.0.0,<4.0.0"
 
 [package.extras]
 code-style = ["pre-commit"]
-rtd = ["attrs", "myst-parser (>=0.16.1,<0.17.0)", "sphinx-book-theme (>=0.1.0,<0.2.0)"]
+rtd = ["myst-parser", "sphinx-book-theme"]
 testing = ["coverage", "pytest", "pytest-cov", "pytest-regressions"]
 
 [[package]]
 name = "mdurl"
 version = "0.1.2"
 description = "Markdown URL utilities"
 optional = false
@@ -905,35 +905,35 @@
 files = [
     {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 
 [[package]]
 name = "myst-parser"
-version = "1.0.0"
+version = "2.0.0"
 description = "An extended [CommonMark](https://spec.commonmark.org/) compliant parser,"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "myst-parser-1.0.0.tar.gz", hash = "sha256:502845659313099542bd38a2ae62f01360e7dd4b1310f025dd014dfc0439cdae"},
-    {file = "myst_parser-1.0.0-py3-none-any.whl", hash = "sha256:69fb40a586c6fa68995e6521ac0a525793935db7e724ca9bac1d33be51be9a4c"},
+    {file = "myst_parser-2.0.0-py3-none-any.whl", hash = "sha256:7c36344ae39c8e740dad7fdabf5aa6fc4897a813083c6cc9990044eb93656b14"},
+    {file = "myst_parser-2.0.0.tar.gz", hash = "sha256:ea929a67a6a0b1683cdbe19b8d2e724cd7643f8aa3e7bb18dd65beac3483bead"},
 ]
 
 [package.dependencies]
-docutils = ">=0.15,<0.20"
+docutils = ">=0.16,<0.21"
 jinja2 = "*"
-markdown-it-py = ">=1.0.0,<3.0.0"
-mdit-py-plugins = ">=0.3.4,<0.4.0"
+markdown-it-py = ">=3.0,<4.0"
+mdit-py-plugins = ">=0.4,<1.0"
 pyyaml = "*"
-sphinx = ">=5,<7"
+sphinx = ">=6,<8"
 
 [package.extras]
 code-style = ["pre-commit (>=3.0,<4.0)"]
-linkify = ["linkify-it-py (>=1.0,<2.0)"]
-rtd = ["ipython", "pydata-sphinx-theme (==v0.13.0rc4)", "sphinx-autodoc2 (>=0.4.2,<0.5.0)", "sphinx-book-theme (==1.0.0rc2)", "sphinx-copybutton", "sphinx-design2", "sphinx-pyscript", "sphinx-tippy (>=0.3.1)", "sphinx-togglebutton", "sphinxext-opengraph (>=0.7.5,<0.8.0)", "sphinxext-rediraffe (>=0.2.7,<0.3.0)"]
+linkify = ["linkify-it-py (>=2.0,<3.0)"]
+rtd = ["ipython", "pydata-sphinx-theme (==v0.13.0rc4)", "sphinx-autodoc2 (>=0.4.2,<0.5.0)", "sphinx-book-theme (==1.0.0rc2)", "sphinx-copybutton", "sphinx-design2", "sphinx-pyscript", "sphinx-tippy (>=0.3.1)", "sphinx-togglebutton", "sphinxext-opengraph (>=0.8.2,<0.9.0)", "sphinxext-rediraffe (>=0.2.7,<0.3.0)"]
 testing = ["beautifulsoup4", "coverage[toml]", "pytest (>=7,<8)", "pytest-cov", "pytest-param-files (>=0.3.4,<0.4.0)", "pytest-regressions", "sphinx-pytest"]
 testing-docutils = ["pygments", "pytest (>=7,<8)", "pytest-param-files (>=0.3.4,<0.4.0)"]
 
 [[package]]
 name = "packaging"
 version = "23.1"
 description = "Core utilities for Python packages"
@@ -1208,28 +1208,28 @@
 files = [
     {file = "soupsieve-2.4.1-py3-none-any.whl", hash = "sha256:1c1bfee6819544a3447586c889157365a27e10d88cde3ad3da0cf0ddf646feb8"},
     {file = "soupsieve-2.4.1.tar.gz", hash = "sha256:89d12b2d5dfcd2c9e8c22326da9d9aa9cb3dfab0a83a024f05704076ee8d35ea"},
 ]
 
 [[package]]
 name = "sphinx"
-version = "6.2.1"
+version = "7.0.1"
 description = "Python documentation generator"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "Sphinx-6.2.1.tar.gz", hash = "sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b"},
-    {file = "sphinx-6.2.1-py3-none-any.whl", hash = "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"},
+    {file = "Sphinx-7.0.1.tar.gz", hash = "sha256:61e025f788c5977d9412587e733733a289e2b9fdc2fef8868ddfbfc4ccfe881d"},
+    {file = "sphinx-7.0.1-py3-none-any.whl", hash = "sha256:60c5e04756c1709a98845ed27a2eed7a556af3993afb66e77fec48189f742616"},
 ]
 
 [package.dependencies]
 alabaster = ">=0.7,<0.8"
 babel = ">=2.9"
 colorama = {version = ">=0.4.5", markers = "sys_platform == \"win32\""}
-docutils = ">=0.18.1,<0.20"
+docutils = ">=0.18.1,<0.21"
 imagesize = ">=1.3"
 importlib-metadata = {version = ">=4.8", markers = "python_version < \"3.10\""}
 Jinja2 = ">=3.0"
 packaging = ">=21.0"
 Pygments = ">=2.13"
 requests = ">=2.25.0"
 snowballstemmer = ">=2.0"
@@ -1538,8 +1538,8 @@
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.9"
-content-hash = "996a2f97e2c2fdcfd0da98b3d90a7728fb68b591905853b1fda4a275c4a9fb40"
+content-hash = "51dc5a3613b66d7e6b27730328d591479c920e148b95bf94b37f5f17be6ee117"
```

### Comparing `pontos-23.6.1/pontos/__init__.py` & `pontos-23.6.2/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/changelog/__init__.py` & `pontos-23.6.2/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/changelog/conventional_commits.py` & `pontos-23.6.2/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/changelog/errors.py` & `pontos-23.6.2/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/changelog/main.py` & `pontos-23.6.2/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/errors.py` & `pontos-23.6.2/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/git/__init__.py` & `pontos-23.6.2/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/git/git.py` & `pontos-23.6.2/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/git/status.py` & `pontos-23.6.2/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/__init__.py` & `pontos-23.6.2/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/actions/__init__.py` & `pontos-23.6.2/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/actions/argparser.py` & `pontos-23.6.2/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/actions/cmds.py` & `pontos-23.6.2/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/actions/core.py` & `pontos-23.6.2/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/actions/env.py` & `pontos-23.6.2/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/actions/errors.py` & `pontos-23.6.2/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/actions/event.py` & `pontos-23.6.2/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/actions/main.py` & `pontos-23.6.2/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/__init__.py` & `pontos-23.6.2/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/api.py` & `pontos-23.6.2/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/artifacts.py` & `pontos-23.6.2/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/branch.py` & `pontos-23.6.2/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/client.py` & `pontos-23.6.2/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/contents.py` & `pontos-23.6.2/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/errors.py` & `pontos-23.6.2/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/helper.py` & `pontos-23.6.2/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/labels.py` & `pontos-23.6.2/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/organizations.py` & `pontos-23.6.2/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/pull_requests.py` & `pontos-23.6.2/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/release.py` & `pontos-23.6.2/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/repositories.py` & `pontos-23.6.2/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/search.py` & `pontos-23.6.2/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/tags.py` & `pontos-23.6.2/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/teams.py` & `pontos-23.6.2/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/api/workflows.py` & `pontos-23.6.2/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/argparser.py` & `pontos-23.6.2/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/cmds.py` & `pontos-23.6.2/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/main.py` & `pontos-23.6.2/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/models/__init__.py` & `pontos-23.6.2/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/models/artifact.py` & `pontos-23.6.2/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/models/base.py` & `pontos-23.6.2/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/models/branch.py` & `pontos-23.6.2/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/models/organization.py` & `pontos-23.6.2/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/models/pull_request.py` & `pontos-23.6.2/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/models/release.py` & `pontos-23.6.2/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/models/search.py` & `pontos-23.6.2/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/models/tag.py` & `pontos-23.6.2/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/models/workflow.py` & `pontos-23.6.2/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/pr_template.md` & `pontos-23.6.2/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/script/__init__.py` & `pontos-23.6.2/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/script/errors.py` & `pontos-23.6.2/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/script/load.py` & `pontos-23.6.2/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/github/script/parser.py` & `pontos-23.6.2/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/helper.py` & `pontos-23.6.2/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/models/__init__.py` & `pontos-23.6.2/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/nvd/__init__.py` & `pontos-23.6.2/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/nvd/api.py` & `pontos-23.6.2/pontos/nvd/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
 from abc import ABC
 from datetime import datetime, timezone
 from types import TracebackType
-from typing import Any, Dict, Optional, Type
+from typing import Any, Dict, Optional, Type, Union
 
 from httpx import AsyncClient, Response, Timeout
 
 from pontos.helper import snake_case
 
 SLEEP_TIMEOUT = 30.0  # in seconds
 DEFAULT_TIMEOUT = 180.0  # three minutes
 DEFAULT_TIMEOUT_CONFIG = Timeout(DEFAULT_TIMEOUT)  # three minutes
 
 Headers = Dict[str, str]
-Params = Dict[str, str]
+Params = Dict[str, Union[str, int]]
 
 __all__ = (
     "convert_camel_case",
     "format_date",
     "now",
     "NVDApi",
 )
@@ -111,15 +111,15 @@
                 Default: True.
         """
         self._url = url
         self._token = token
         self._client = AsyncClient(http2=True, timeout=timeout)
 
         if rate_limit:
-            self._rate_limit = 50 if token else 5
+            self._rate_limit: Optional[int] = 50 if token else 5
         else:
             self._rate_limit = None
 
         self._request_count = 0
 
     def _request_headers(self) -> Headers:
         """
@@ -166,8 +166,10 @@
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> Optional[bool]:
-        return await self._client.__aexit__(exc_type, exc_value, traceback)
+        return await self._client.__aexit__(  # type: ignore
+            exc_type, exc_value, traceback
+        )
```

### Comparing `pontos-23.6.1/pontos/nvd/cpe/__init__.py` & `pontos-23.6.2/pontos/nvd/cpe/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
 from argparse import ArgumentParser, Namespace
+from typing import Callable
 
 from pontos.nvd.cpe.api import CPEApi
 
 __all__ = ("CPEApi",)
 
 
 async def query_cpe(args: Namespace) -> None:
@@ -60,13 +61,13 @@
         help="Search for CPEs containing the keyword in their titles and "
         "references.",
     )
 
     main(parser, query_cpes)
 
 
-def main(parser: ArgumentParser, func: callable) -> None:
+def main(parser: ArgumentParser, func: Callable) -> None:
     try:
         args = parser.parse_args()
         asyncio.run(func(args))
     except KeyboardInterrupt:
         pass
```

### Comparing `pontos-23.6.1/pontos/nvd/cpe/api.py` & `pontos-23.6.2/pontos/nvd/cpe/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,25 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
 from datetime import datetime
-from typing import Any, AsyncIterator, Dict, List, Optional, Union
+from types import TracebackType
+from typing import (
+    Any,
+    AsyncIterator,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Type,
+    Union,
+)
 
 from httpx import Timeout
 
 from pontos.errors import PontosError
 from pontos.nvd.api import (
     DEFAULT_TIMEOUT_CONFIG,
     NVDApi,
@@ -149,15 +159,15 @@
 
                 async with CPEApi() as api:
                     async for cpe in api.cpes(keywords=["Mac OS X"]):
                         print(cpe.cpe_name, cpe.cpe_name_id)
         """
         total_results = None
 
-        params = {}
+        params: Dict[str, Union[str, int]] = {}
         if last_modified_start_date:
             params["lastModStartDate"] = format_date(last_modified_start_date)
             if not last_modified_end_date:
                 params["lastModEndDate"] = format_date(now())
         if last_modified_end_date:
             params["lastModEndDate"] = format_date(last_modified_end_date)
 
@@ -187,15 +197,30 @@
             response = await self._get(params=params)
             response.raise_for_status()
 
             data: Dict[str, Union[int, str, Dict[str, Any]]] = response.json(
                 object_hook=convert_camel_case
             )
 
-            results_per_page: int = data["results_per_page"]
-            total_results: int = data["total_results"]
-            products = data.get("products", [])
+            results_per_page: int = data["results_per_page"]  # type: ignore
+            total_results: int = data["total_results"]  # type: ignore
+            products: Iterable = data.get("products", [])  # type: ignore
 
             for product in products:
                 yield CPE.from_dict(product["cpe"])
 
-            start_index += results_per_page
+            if results_per_page is not None:
+                start_index += results_per_page
+
+    async def __aenter__(self) -> "CPEApi":
+        await super().__aenter__()
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> Optional[bool]:
+        return await super().__aexit__(  # type: ignore
+            exc_type, exc_value, traceback
+        )
```

### Comparing `pontos-23.6.1/pontos/nvd/cve/__init__.py` & `pontos-23.6.2/pontos/nvd/cve/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
 from argparse import ArgumentParser, Namespace
+from typing import Callable
 
 from pontos.nvd.cve.api import *
 
 __all__ = ("CVEApi",)
 
 
 async def query_cves(args: Namespace) -> None:
@@ -73,13 +74,13 @@
     parser = ArgumentParser()
     parser.add_argument("--token", help="API key to use for querying.")
     parser.add_argument("cve_id", metavar="CVE-ID", help="ID of the CVE")
 
     main(parser, query_cve)
 
 
-def main(parser: ArgumentParser, func: callable) -> None:
+def main(parser: ArgumentParser, func: Callable) -> None:
     try:
         args = parser.parse_args()
         asyncio.run(func(args))
     except KeyboardInterrupt:
         pass
```

### Comparing `pontos-23.6.1/pontos/nvd/cve/api.py` & `pontos-23.6.2/pontos/nvd/cve/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,33 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from datetime import datetime
-from typing import Any, AsyncIterator, Dict, List, Optional, Union
+from types import TracebackType
+from typing import (
+    Any,
+    AsyncIterator,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Type,
+    Union,
+)
 
 from httpx import Timeout
 
 from pontos.errors import PontosError
 from pontos.nvd.api import (
     DEFAULT_TIMEOUT_CONFIG,
     NVDApi,
+    Params,
     convert_camel_case,
     format_date,
     now,
 )
 from pontos.nvd.models.cve import CVE
 from pontos.nvd.models.cvss_v2 import Severity as CVSSv2Severity
 from pontos.nvd.models.cvss_v3 import Severity as CVSSv3Severity
@@ -158,17 +169,17 @@
 
                 from pontos.nvd.cve import CVEApi
 
                 async with CVEApi() as api:
                     async for cve in api.cves(keywords=["Mac OS X", "kernel"]):
                         print(cve.id)
         """
-        total_results = None
+        total_results: Optional[int] = None
 
-        params = {}
+        params: Params = {}
         if last_modified_start_date:
             params["lastModStartDate"] = format_date(last_modified_start_date)
             if not last_modified_end_date:
                 params["lastModEndDate"] = format_date(now())
         if last_modified_end_date:
             params["lastModEndDate"] = format_date(last_modified_end_date)
 
@@ -215,15 +226,15 @@
         if has_cert_notes:
             params["hasCertNotes"] = ""
         if has_kev:
             params["hasKev"] = ""
         if has_oval:
             params["hasOval"] = ""
 
-        start_index = 0
+        start_index: int = 0
         results_per_page = None
 
         while total_results is None or start_index < total_results:
             params["startIndex"] = start_index
 
             if results_per_page is not None:
                 params["resultsPerPage"] = results_per_page
@@ -231,22 +242,25 @@
             response = await self._get(params=params)
             response.raise_for_status()
 
             data: Dict[str, Union[int, str, Dict[str, Any]]] = response.json(
                 object_hook=convert_camel_case
             )
 
-            results_per_page: int = data["results_per_page"]
-            total_results: int = data["total_results"]
-            vulnerabilities = data.get("vulnerabilities", [])
+            total_results = data["total_results"]  # type: ignore
+            results_per_page: int = data["results_per_page"]  # type: ignore
+            vulnerabilities: Iterable = data.get(  # type: ignore
+                "vulnerabilities", []
+            )
 
             for vulnerability in vulnerabilities:
                 yield CVE.from_dict(vulnerability["cve"])
 
-            start_index += results_per_page
+            if results_per_page is not None:
+                start_index += results_per_page
 
     async def cve(self, cve_id: str) -> CVE:
         """
         Returns a single CVE matching the CVE ID. Vulnerabilities not yet
         published in the NVD are not available.
 
         Args:
@@ -276,7 +290,21 @@
         data = response.json(object_hook=convert_camel_case)
         vulnerabilities = data["vulnerabilities"]
         if not vulnerabilities:
             raise PontosError(f"No CVE with CVE ID '{cve_id}' found.")
 
         vulnerability = vulnerabilities[0]
         return CVE.from_dict(vulnerability["cve"])
+
+    async def __aenter__(self) -> "CVEApi":
+        await super().__aenter__()
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> Optional[bool]:
+        return await super().__aexit__(  # type: ignore
+            exc_type, exc_value, traceback
+        )
```

### Comparing `pontos-23.6.1/pontos/nvd/models/__init__.py` & `pontos-23.6.2/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/nvd/models/cpe.py` & `pontos-23.6.2/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/nvd/models/cve.py` & `pontos-23.6.2/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/nvd/models/cvss_v2.py` & `pontos-23.6.2/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/nvd/models/cvss_v3.py` & `pontos-23.6.2/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/pontos.py` & `pontos-23.6.2/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/release/__init__.py` & `pontos-23.6.2/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/release/helper.py` & `pontos-23.6.2/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/release/main.py` & `pontos-23.6.2/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/release/parser.py` & `pontos-23.6.2/pontos/release/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/release/release.py` & `pontos-23.6.2/pontos/release/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/release/sign.py` & `pontos-23.6.2/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/terminal/__init__.py` & `pontos-23.6.2/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/terminal/null.py` & `pontos-23.6.2/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/terminal/rich.py` & `pontos-23.6.2/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/terminal/terminal.py` & `pontos-23.6.2/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/testing/__init__.py` & `pontos-23.6.2/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/updateheader/__init__.py` & `pontos-23.6.2/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/updateheader/__main__.py` & `pontos-23.6.2/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/updateheader/updateheader.py` & `pontos-23.6.2/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/__init__.py` & `pontos-23.6.2/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/__main__.py` & `pontos-23.6.2/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/_calculator.py` & `pontos-23.6.2/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/commands/__init__.py` & `pontos-23.6.2/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/commands/_cargo.py` & `pontos-23.6.2/pontos/version/commands/_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/commands/_cmake.py` & `pontos-23.6.2/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/commands/_command.py` & `pontos-23.6.2/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/commands/_go.py` & `pontos-23.6.2/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/commands/_java.py` & `pontos-23.6.2/pontos/version/commands/_java.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/commands/_javascript.py` & `pontos-23.6.2/pontos/version/commands/_javascript.py`

 * *Files 9% similar despite different names*

```diff
@@ -135,19 +135,22 @@
         """
         Update the version file with the new version
         """
         if not version_file.exists():
             return False
 
         content = version_file.read_text(encoding="utf-8")
-        content = re.sub(
-            pattern=r'VERSION = "(?P<version>.*)"',
-            repl=f'VERSION = "{new_version}"',
+        match = re.search(
+            pattern=r'VERSION = (?P<quote>[\'"])(?P<version>.*)(?P=quote)',
             string=content,
         )
+        if not match:
+            return False
+
+        content = content.replace(match.group("version"), str(new_version))
         version_file.write_text(content, encoding="utf-8")
         return True
 
     def update_version(
         self, new_version: Version, *, force: bool = False
     ) -> VersionUpdate:
         package_version = self.get_current_version()
```

### Comparing `pontos-23.6.1/pontos/version/commands/_python.py` & `pontos-23.6.2/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/errors.py` & `pontos-23.6.2/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/helper.py` & `pontos-23.6.2/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/main.py` & `pontos-23.6.2/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/parser.py` & `pontos-23.6.2/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/project.py` & `pontos-23.6.2/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/schemes/__init__.py` & `pontos-23.6.2/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/schemes/_pep440.py` & `pontos-23.6.2/pontos/version/schemes/_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/schemes/_scheme.py` & `pontos-23.6.2/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/schemes/_semantic.py` & `pontos-23.6.2/pontos/version/schemes/_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pontos/version/version.py` & `pontos-23.6.2/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/pyproject.toml` & `pontos-23.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.6.1"
+version = "23.6.2"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
@@ -50,15 +50,15 @@
 autohooks = ">=22.7.0"
 autohooks-plugin-pylint = ">=21.6.0"
 autohooks-plugin-black = ">=22.7.0"
 autohooks-plugin-isort = ">=22.3.0"
 rope = "^1.8.0"
 coverage = "^7.2"
 myst-parser = ">=0.19.1"
-Sphinx = "^6.2.1"
+Sphinx = "^7.0.1"
 furo = "^2023.5.20"
 sphinx-autobuild = "^2021.3.14"
 
 [tool.black]
 line-length = 80
 target-version = ['py39', 'py310', 'py311']
 exclude = '''
```

### Comparing `pontos-23.6.1/scripts/github/artifacts-download.py` & `pontos-23.6.2/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/artifacts.py` & `pontos-23.6.2/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/branchprotection.py` & `pontos-23.6.2/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/create-repository.py` & `pontos-23.6.2/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/enforce-admins.py` & `pontos-23.6.2/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/lock-branch.py` & `pontos-23.6.2/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/members.py` & `pontos-23.6.2/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/release-assets-download.py` & `pontos-23.6.2/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/repositories.py` & `pontos-23.6.2/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/search-repositories.py` & `pontos-23.6.2/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/team-repositories.py` & `pontos-23.6.2/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/teams.py` & `pontos-23.6.2/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/scripts/github/workflow-runs.py` & `pontos-23.6.2/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/__init__.py` & `pontos-23.6.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/changelog/__init__.py` & `pontos-23.6.2/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/changelog/test_conventional_commits.py` & `pontos-23.6.2/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/changelog/test_parser.py` & `pontos-23.6.2/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/git/__init__.py` & `pontos-23.6.2/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/git/test_git.py` & `pontos-23.6.2/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/git/test_status.py` & `pontos-23.6.2/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/__init__.py` & `pontos-23.6.2/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/actions/__init__.py` & `pontos-23.6.2/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/actions/test-pull-request-event.json` & `pontos-23.6.2/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/actions/test_core.py` & `pontos-23.6.2/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/actions/test_env.py` & `pontos-23.6.2/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/actions/test_event.py` & `pontos-23.6.2/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/__init__.py` & `pontos-23.6.2/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/pr-files.json` & `pontos-23.6.2/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/release-response.json` & `pontos-23.6.2/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_artifacts.py` & `pontos-23.6.2/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_branch.py` & `pontos-23.6.2/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_client.py` & `pontos-23.6.2/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_contents.py` & `pontos-23.6.2/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_labels.py` & `pontos-23.6.2/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_organizations.py` & `pontos-23.6.2/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_pull_requests.py` & `pontos-23.6.2/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_release.py` & `pontos-23.6.2/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_repositories.py` & `pontos-23.6.2/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_search.py` & `pontos-23.6.2/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_tags.py` & `pontos-23.6.2/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_teams.py` & `pontos-23.6.2/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/api/test_workflows.py` & `pontos-23.6.2/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/models/__init__.py` & `pontos-23.6.2/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/models/test_artifact.py` & `pontos-23.6.2/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/models/test_base.py` & `pontos-23.6.2/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/models/test_branch.py` & `pontos-23.6.2/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/models/test_organization.py` & `pontos-23.6.2/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/models/test_pull_request.py` & `pontos-23.6.2/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/models/test_release.py` & `pontos-23.6.2/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/models/test_search.py` & `pontos-23.6.2/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/models/test_tag.py` & `pontos-23.6.2/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/models/test_workflow.py` & `pontos-23.6.2/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/script/__init__.py` & `pontos-23.6.2/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/script/test_load.py` & `pontos-23.6.2/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/script/test_parser.py` & `pontos-23.6.2/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/test_argparser.py` & `pontos-23.6.2/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/github/test_cmds.py` & `pontos-23.6.2/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/models/__init__.py` & `pontos-23.6.2/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/models/test_models.py` & `pontos-23.6.2/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/nvd/__init__.py` & `pontos-23.6.2/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/nvd/cpe/__init__.py` & `pontos-23.6.2/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/nvd/cpe/test_api.py` & `pontos-23.6.2/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/nvd/cve/__init__.py` & `pontos-23.6.2/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/nvd/cve/test_api.py` & `pontos-23.6.2/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/nvd/models/__init__.py` & `pontos-23.6.2/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/nvd/models/test_cpe.py` & `pontos-23.6.2/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/nvd/models/test_cve.py` & `pontos-23.6.2/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/nvd/test_api.py` & `pontos-23.6.2/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/release/__init__.py` & `pontos-23.6.2/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/release/test_helper.py` & `pontos-23.6.2/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/release/test_parser.py` & `pontos-23.6.2/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/release/test_release.py` & `pontos-23.6.2/tests/release/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/release/test_sign.py` & `pontos-23.6.2/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/terminal/__init__.py` & `pontos-23.6.2/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/terminal/test_terminal.py` & `pontos-23.6.2/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/test_helper.py` & `pontos-23.6.2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/test_pontos.py` & `pontos-23.6.2/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/testing/__init__.py` & `pontos-23.6.2/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/testing/test_testing.py` & `pontos-23.6.2/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/updateheader/__init__.py` & `pontos-23.6.2/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/updateheader/test_header.py` & `pontos-23.6.2/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/__init__.py` & `pontos-23.6.2/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/commands/__init__.py` & `pontos-23.6.2/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/commands/test_cargo.py` & `pontos-23.6.2/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/commands/test_cmake.py` & `pontos-23.6.2/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/commands/test_go.py` & `pontos-23.6.2/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/commands/test_java.py` & `pontos-23.6.2/tests/version/commands/test_java.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/commands/test_javascript.py` & `pontos-23.6.2/tests/version/commands/test_javascript.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,61 @@
 
             self.assertEqual(
                 js_version_file.read_text(encoding="utf8"),
                 'const foo = "bar";\nconst VERSION = "22.4.0";\n'
                 "const func = () => ();\n",
             )
 
+    def test_update_js_version_file_with_single_quotes(self):
+        content = '{"name":"foo", "version":"1.2.3"}'
+        js_content = """const foo = "bar";
+const VERSION = '1.2.3';
+const func = () => ();
+"""
+
+        with temp_directory(change_into=True) as temp_dir:
+            package_json = temp_dir / "package.json"
+            package_json.write_text(content, encoding="utf8")
+            js_version_file = (
+                temp_dir / JavaScriptVersionCommand.version_file_paths[0]
+            )
+            js_version_file.parent.mkdir()
+            js_version_file.write_text(js_content, encoding="utf8")
+
+            cmd = JavaScriptVersionCommand(SemanticVersioningScheme)
+            updated = cmd.update_version(
+                SemanticVersioningScheme.parse_version("22.4.0")
+            )
+
+            self.assertEqual(
+                updated.previous,
+                SemanticVersioningScheme.parse_version("1.2.3"),
+            )
+            self.assertEqual(
+                updated.new, SemanticVersioningScheme.parse_version("22.4.0")
+            )
+            self.assertEqual(
+                updated.changed_files,
+                [
+                    package_json.resolve(),
+                    JavaScriptVersionCommand.version_file_paths[0],
+                ],
+            )
+
+            with package_json.open(mode="r", encoding="utf-8") as fp:
+                fake_package = json.load(fp)
+
+            self.assertEqual(fake_package["version"], "22.4.0")
+
+            self.assertEqual(
+                js_version_file.read_text(encoding="utf8"),
+                "const foo = \"bar\";\nconst VERSION = '22.4.0';\n"
+                "const func = () => ();\n",
+            )
+
     def test_update_version_files(self):
         content = '{"name":"foo", "version":"1.2.3"}'
         file_content = """const foo = "bar";
 const VERSION = "1.2.3";
 const func = () => ();
 """
```

### Comparing `pontos-23.6.1/tests/version/commands/test_python.py` & `pontos-23.6.2/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/schemes/__init__.py` & `pontos-23.6.2/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/schemes/test_pep440.py` & `pontos-23.6.2/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/schemes/test_semantic.py` & `pontos-23.6.2/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/test_commands.py` & `pontos-23.6.2/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/test_errors.py` & `pontos-23.6.2/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/test_helper.py` & `pontos-23.6.2/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/test_main.py` & `pontos-23.6.2/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/test_parser.py` & `pontos-23.6.2/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/test_project.py` & `pontos-23.6.2/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/tests/version/test_version.py` & `pontos-23.6.2/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.1/PKG-INFO` & `pontos-23.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.6.1
+Version: 23.6.2
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

