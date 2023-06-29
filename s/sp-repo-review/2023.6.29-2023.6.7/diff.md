# Comparing `tmp/sp_repo_review-2023.6.29.tar.gz` & `tmp/sp_repo_review-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Jun 29 21:04:37 2023, max compression
+gzip compressed data, last modified: Wed Jun  7 22:19:41 2023, max compression
```

## Comparing `sp_repo_review-2023.6.29.tar` & `sp_repo_review-2023.6.7.tar`

### file list

```diff
@@ -1,123 +1,116 @@
--rw-r--r--   0        0        0      125 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.git_archival.txt
--rw-r--r--   0        0        0       45 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.gitattributes
--rw-r--r--   0        0        0     2223 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.pre-commit-config.yaml
--rw-r--r--   0        0        0      179 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      572 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.readthedocs.yaml
--rw-r--r--   0        0        0        6 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.ruby-version
--rw-r--r--   0        0        0      894 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/Gemfile
--rw-r--r--   0        0        0     2106 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/Gemfile.lock
--rw-r--r--   0        0        0    18489 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/README.md
--rw-r--r--   0        0        0     1057 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/_config.yml
--rw-r--r--   0        0        0      763 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/action.yml
--rw-r--r--   0        0        0      799 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/cookiecutter.json
--rw-r--r--   0        0        0     2112 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/copier.yml
--rw-r--r--   0        0        0      616 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/extensions.py
--rw-r--r--   0        0        0    11067 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/noxfile.py
--rw-r--r--   0        0        0      640 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      162 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.github/dependabot.yml
--rw-r--r--   0        0        0      793 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.github/workflows/bump.yml
--rw-r--r--   0        0        0      726 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1219 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2109 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.github/workflows/reusable-change-detection.yml
--rw-r--r--   0        0        0     5295 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.github/workflows/reusable-cookie.yml
--rw-r--r--   0        0        0     1262 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.github/workflows/reusable-rr-tests.yml
--rw-r--r--   0        0        0      251 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/LICENSE
--rw-r--r--   0        0        0      829 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/README.md
--rw-r--r--   0        0        0     2180 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/_includes/head.html
--rw-r--r--   0        0        0     1019 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/_includes/head_custom.html
--rw-r--r--   0        0        0      545 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/_includes/interactive_repo_review.html
--rw-r--r--   0        0        0       92 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/_includes/rr.html
--rw-r--r--   0        0        0      145 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/_includes/toc.html
--rw-r--r--   0        0        0       22 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/_sass/color_schemes/skhep.scss
--rw-r--r--   0        0        0     2611 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/_sass/custom/custom.scss
--rw-r--r--   0        0        0    15086 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/assets/favicon.ico
--rw-r--r--   0        0        0     8070 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      652 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/assets/js/tabs.js
--rw-r--r--   0        0        0    10211 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/assets/js/webapp.js
--rw-r--r--   0        0        0     3322 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/index.md
--rw-r--r--   0        0        0     4562 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/coverage.md
--rw-r--r--   0        0        0     9088 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/docs.md
--rw-r--r--   0        0        0    11346 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/gha_basic.md
--rw-r--r--   0        0        0     9249 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/gha_pure.md
--rw-r--r--   0        0        0     8257 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/gha_wheels.md
--rw-r--r--   0        0        0     2741 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/index.md
--rw-r--r--   0        0        0    10386 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/mypy.md
--rw-r--r--   0        0        0    18365 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/packaging_classic.md
--rw-r--r--   0        0        0     9597 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/packaging_simple.md
--rw-r--r--   0        0        0    14474 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/pytest.md
--rw-r--r--   0        0        0      947 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/repo_review.md
--rw-r--r--   0        0        0    28623 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/style.md
--rw-r--r--   0        0        0     9139 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/guides/tasks.md
--rw-r--r--   0        0        0     4260 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/patterns/backports.md
--rw-r--r--   0        0        0     7192 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/patterns/data_files.md
--rw-r--r--   0        0        0     3104 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/patterns/exports.md
--rw-r--r--   0        0        0      738 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/patterns/index.md
--rw-r--r--   0        0        0    11217 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/principles/design.md
--rw-r--r--   0        0        0      561 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/principles/index.md
--rw-r--r--   0        0        0     2209 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/principles/process.md
--rw-r--r--   0        0        0     4836 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/tutorials/dev-environment.md
--rw-r--r--   0        0        0     4795 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/tutorials/docs.md
--rw-r--r--   0        0        0      998 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/tutorials/index.md
--rw-r--r--   0        0        0     2578 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/tutorials/module.md
--rw-r--r--   0        0        0     3300 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/tutorials/packaging.md
--rw-r--r--   0        0        0     4645 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/docs/pages/tutorials/test.md
--rw-r--r--   0        0        0      246 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/__init__.py
--rw-r--r--   0        0        0      168 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/_version.pyi
--rw-r--r--   0        0        0      822 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/families.py
--rw-r--r--   0        0        0        0 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0      152 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/checks/__init__.py
--rw-r--r--   0        0        0     2849 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/checks/general.py
--rw-r--r--   0        0        0     5018 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/checks/github.py
--rw-r--r--   0        0        0     4133 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/checks/mypy.py
--rw-r--r--   0        0        0     3162 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/checks/precommit.py
--rw-r--r--   0        0        0     5339 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/checks/pyproject.py
--rw-r--r--   0        0        0     2565 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/checks/readthedocs.py
--rw-r--r--   0        0        0     2868 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/src/sp_repo_review/checks/ruff.py
--rw-r--r--   0        0        0      412 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/tests/test_cmd.py
--rw-r--r--   0        0        0      597 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/tests/test_package.py
--rw-r--r--   0        0        0      125 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.gitattributes
--rw-r--r--   0        0        0     2218 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2905 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.readthedocs.yml
--rw-r--r--   0        0        0     1689 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0     2928 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/noxfile.py
--rw-r--r--   0        0        0     8577 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      123 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}MANIFEST.in{% endif %}
--rw-r--r--   0        0        0     2021 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}
--rw-r--r--   0        0        0      691 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}
--rw-r--r--   0        0        0      915 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}
--rw-r--r--   0        0        0      727 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}
--rw-r--r--   0        0        0      376 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='setuptools' %}setup.py{% endif %}
--rw-r--r--   0        0        0      280 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='skbuild' %}CMakeLists.txt{% endif %}
--rw-r--r--   0        0        0    11380 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'Apache' %}LICENSE{% endif %}
--rw-r--r--   0        0        0     1559 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'BSD' %}LICENSE{% endif %}
--rw-r--r--   0        0        0     1089 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'MIT' %}LICENSE{% endif %}
--rw-r--r--   0        0        0      102 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{{cookiecutter.__answers}}
--rw-r--r--   0        0        0     2528 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.github/matchers/pylint.json
--rw-r--r--   0        0        0     3424 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1573 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type == 'compiled' %}wheels.yml{% endif %}
--rw-r--r--   0        0        0      934 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/docs/conf.py
--rw-r--r--   0        0        0      218 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0      632 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}
--rw-r--r--   0        0        0      562 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}
--rw-r--r--   0        0        0      422 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/py.typed
--rw-r--r--   0        0        0      117 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.__type=='compiled' %}_core.pyi{% endif %}
--rw-r--r--   0        0        0      118 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.backend in ['setuptools', 'pybind11'] %}_version.pyi{% endif %}
--rw-r--r--   0        0        0      215 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/__init__.py
--rw-r--r--   0        0        0      573 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/typing.py
--rw-r--r--   0        0        0      378 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/tests/test_package.py
--rw-r--r--   0        0        0      190 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/tests/{% if cookiecutter.__type=='compiled' %}test_compiled.py{% endif %}
--rw-r--r--   0        0        0     2249 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/.gitignore
--rw-r--r--   0        0        0     1525 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/LICENSE
--rw-r--r--   0        0        0     5507 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/pyproject.toml
--rw-r--r--   0        0        0    10038 2023-06-29 21:04:37.000000 sp_repo_review-2023.6.29/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.gitattributes
+-rw-r--r--   0        0        0     2227 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      179 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      571 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.readthedocs.yml
+-rw-r--r--   0        0        0        6 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.ruby-version
+-rw-r--r--   0        0        0     1294 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/Gemfile
+-rw-r--r--   0        0        0     2171 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/Gemfile.lock
+-rw-r--r--   0        0        0     8658 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/README.md
+-rw-r--r--   0        0        0     1160 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/_config.yml
+-rw-r--r--   0        0        0      763 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/action.yml
+-rw-r--r--   0        0        0      563 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/cookiecutter.json
+-rw-r--r--   0        0        0     7033 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/noxfile.py
+-rw-r--r--   0        0        0      640 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      726 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1219 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2018 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-change-detection.yml
+-rw-r--r--   0        0        0     5153 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-cookie.yml
+-rw-r--r--   0        0        0      919 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-rr-tests.yml
+-rw-r--r--   0        0        0      251 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/LICENSE
+-rw-r--r--   0        0        0      730 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/README.md
+-rw-r--r--   0        0        0     2180 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/head.html
+-rw-r--r--   0        0        0     1019 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/head_custom.html
+-rw-r--r--   0        0        0      547 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/interactive_repo_review.html
+-rw-r--r--   0        0        0       92 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/rr.html
+-rw-r--r--   0        0        0      150 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/toc.html
+-rw-r--r--   0        0        0       22 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_sass/color_schemes/skhep.scss
+-rw-r--r--   0        0        0     2611 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_sass/custom/custom.scss
+-rw-r--r--   0        0        0    15086 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     8070 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      652 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/js/tabs.js
+-rw-r--r--   0        0        0    10234 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/js/webapp.js
+-rw-r--r--   0        0        0     2219 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/index.md
+-rw-r--r--   0        0        0     4512 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/coverage.md
+-rw-r--r--   0        0        0    11293 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_basic.md
+-rw-r--r--   0        0        0     9205 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_pure.md
+-rw-r--r--   0        0        0     8224 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_wheels.md
+-rw-r--r--   0        0        0     2162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/index.md
+-rw-r--r--   0        0        0     8606 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/mypy.md
+-rw-r--r--   0        0        0    17927 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/packaging_classic.md
+-rw-r--r--   0        0        0     9182 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/packaging_simple.md
+-rw-r--r--   0        0        0    14552 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/pytest.md
+-rw-r--r--   0        0        0      932 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/repo_review.md
+-rw-r--r--   0        0        0    28595 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/style.md
+-rw-r--r--   0        0        0     8853 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/tasks.md
+-rw-r--r--   0        0        0     5310 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/writing-docs.md
+-rw-r--r--   0        0        0     7027 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/patterns/data_files.md
+-rw-r--r--   0        0        0      517 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/patterns/index.md
+-rw-r--r--   0        0        0    11200 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/design.md
+-rw-r--r--   0        0        0      561 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/index.md
+-rw-r--r--   0        0        0     2209 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/process.md
+-rw-r--r--   0        0        0     4816 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/dev-environment.md
+-rw-r--r--   0        0        0      998 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/index.md
+-rw-r--r--   0        0        0     2557 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/module.md
+-rw-r--r--   0        0        0     3272 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/packaging.md
+-rw-r--r--   0        0        0     4621 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/test.md
+-rw-r--r--   0        0        0     1063 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      168 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      228 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_version.pyi
+-rw-r--r--   0        0        0      753 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/families.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0      290 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/__init__.py
+-rw-r--r--   0        0        0     2849 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/general.py
+-rw-r--r--   0        0        0     5018 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/github.py
+-rw-r--r--   0        0        0     4133 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/mypy.py
+-rw-r--r--   0        0        0     3162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/precommit.py
+-rw-r--r--   0        0        0     5339 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/pyproject.py
+-rw-r--r--   0        0        0     2868 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/ruff.py
+-rw-r--r--   0        0        0      412 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/tests/test_cmd.py
+-rw-r--r--   0        0        0      597 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/tests/test_package.py
+-rw-r--r--   0        0        0      125 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitattributes
+-rw-r--r--   0        0        0     2218 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2930 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      456 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.readthedocs.yml
+-rw-r--r--   0        0        0      280 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/CMakeLists-skbuild.txt
+-rw-r--r--   0        0        0      685 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/Cargo-maturin.toml
+-rw-r--r--   0        0        0    14162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/LICENSE
+-rw-r--r--   0        0        0      123 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/MANIFEST-setuptools,pybind11.in
+-rw-r--r--   0        0        0     1910 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      909 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/meson-mesonpy.build
+-rw-r--r--   0        0        0     2312 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/noxfile.py
+-rw-r--r--   0        0        0     8580 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      723 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-pybind11.py
+-rw-r--r--   0        0        0     1980 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools,pybind11.cfg
+-rw-r--r--   0        0        0      374 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools.py
+-rw-r--r--   0        0        0     2533 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     3414 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1573 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/wheels-pybind11,skbuild,mesonpy,maturin.yml
+-rw-r--r--   0        0        0     2031 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/docs/conf.py
+-rw-r--r--   0        0        0      286 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/docs/index.rst
+-rw-r--r--   0        0        0      562 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/lib-maturin.rs
+-rw-r--r--   0        0        0      632 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/main-pybind11,skbuild,mesonpy.cpp
+-rw-r--r--   0        0        0      430 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_core-pybind11,skbuild,mesonpy,maturin.pyi
+-rw-r--r--   0        0        0      118 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_version-setuptools,pybind11.pyi
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/py.typed
+-rw-r--r--   0        0        0      213 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_compat/__init__.py
+-rw-r--r--   0        0        0      498 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_compat/typing.py
+-rw-r--r--   0        0        0      188 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/tests/test_compiled-pybind11,skbuild,mesonpy,maturin.py
+-rw-r--r--   0        0        0      431 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/tests/test_package.py
+-rw-r--r--   0        0        0     2248 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.gitignore
+-rw-r--r--   0        0        0     1525 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/LICENSE
+-rw-r--r--   0        0        0     2375 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/README-rr.md
+-rw-r--r--   0        0        0     5180 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/pyproject.toml
+-rw-r--r--   0        0        0     3894 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/PKG-INFO
```

### Comparing `sp_repo_review-2023.6.29/.pre-commit-config.yaml` & `sp_repo_review-2023.6.7/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.3.0
     hooks:
       - id: mypy
-        files: "(src|tests)"
+        files: "(src|web|tests)"
         args: []
         additional_dependencies:
           - click
           - markdown-it-py
           - pytest
           - repo-review
           - rich
```

### Comparing `sp_repo_review-2023.6.29/.readthedocs.yaml` & `sp_repo_review-2023.6.7/.readthedocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# .readthedocs.yaml
+# .readthedocs.yml
 # Read the Docs configuration file
 # See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
 
 # Required
 version: 2
 
 # Set the version of Python and other tools you might need
```

### Comparing `sp_repo_review-2023.6.29/_config.yml` & `sp_repo_review-2023.6.7/_config.yml`

 * *Files 24% similar despite different names*

```diff
@@ -11,36 +11,36 @@
 markdown: kramdown
 theme: "just-the-docs"
 plugins:
   - jekyll-feed
 
 # Theme settings
 
+color_scheme: skhep
+
 logo: "/assets/images/logo.svg"
 
 # Enable or disable the site search
 search_enabled: true
 
 # Aux links for the upper right navigation
 aux_links:
   "Scientific Python Cookie":
     - "//github.com/scientific-python/cookie"
 
 gh_edit_link: true
 gh_edit_link_text: "View source for this page on GitHub."
 gh_edit_repository: "https://github.com/scientific-python/cookie"
 gh_edit_branch: "main"
-gh_edit_source: "docs"
 gh_edit_view_mode: "tree" # "tree" or "edit"
 
-callouts:
-  warning:
-    color: red
-    title: Warning
-  note:
-    color: yellow
-    title: Note
-  important:
-    color: green
-    title: Important
-  highlight:
-    color: blue
+# Exclude from processing.
+# The following items will not be processed, by default. Create a custom list
+# to override the default setting.
+# exclude:
+#   - Gemfile
+#   - Gemfile.lock
+#   - node_modules
+#   - vendor/bundle/
+#   - vendor/cache/
+#   - vendor/gems/
+#   - vendor/ruby/
```

### Comparing `sp_repo_review-2023.6.29/action.yml` & `sp_repo_review-2023.6.7/action.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/cookiecutter.json` & `sp_repo_review-2023.6.7/cookiecutter.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5333333333333333%*

 * *Differences: {"'project_type'": "['hatch', 'setuptools', 'setuptools621', 'pybind11', 'skbuild', 'mesonpy', "*

 * *                   "'poetry', 'flit', 'pdm', 'trampolim', 'whey', 'maturin']",*

 * * "'year'": '"{% now \'utc\', \'%Y\' %}"',*

 * * 'delete': "['backend', '__year', '__project_slug', '__type', '__answers']"}*

```diff
@@ -1,34 +1,31 @@
 {
-    "__answers": "",
-    "__project_slug": "{{ cookiecutter.project_name | lower | replace('-', '_') | replace('.', '_') }}",
-    "__type": "{{ 'compiled' if cookiecutter.backend in ['pybind11', 'skbuild', 'mesonpy', 'maturin'] else 'pure' }}",
-    "__year": "{% now 'utc', '%Y' %}",
     "_extensions": [
         "jinja2_time.TimeExtension"
     ],
-    "backend": [
-        "hatch",
-        "flit",
-        "pdm",
-        "trampolim",
-        "whey",
-        "poetry",
-        "setuptools621",
-        "setuptools",
-        "pybind11",
-        "skbuild",
-        "mesonpy",
-        "maturin"
-    ],
     "email": "me@email.com",
     "full_name": "My Name",
     "license": [
         "BSD",
         "Apache",
         "MIT"
     ],
     "org": "org",
     "project_name": "package",
     "project_short_description": "A great package.",
-    "url": "https://github.com/{{ cookiecutter.org }}/{{ cookiecutter.project_name }}"
+    "project_type": [
+        "hatch",
+        "setuptools",
+        "setuptools621",
+        "pybind11",
+        "skbuild",
+        "mesonpy",
+        "poetry",
+        "flit",
+        "pdm",
+        "trampolim",
+        "whey",
+        "maturin"
+    ],
+    "url": "https://github.com/{{ cookiecutter.org }}/{{ cookiecutter.project_name }}",
+    "year": "{% now 'utc', '%Y' %}"
 }
```

### Comparing `sp_repo_review-2023.6.29/.devcontainer/devcontainer.json` & `sp_repo_review-2023.6.7/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/.github/workflows/cd.yml` & `sp_repo_review-2023.6.7/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/.github/workflows/ci.yml` & `sp_repo_review-2023.6.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/.github/workflows/reusable-change-detection.yml` & `sp_repo_review-2023.6.7/.github/workflows/reusable-change-detection.yml`

 * *Files 8% similar despite different names*

```diff
@@ -3,62 +3,57 @@
   workflow_call:
     outputs:
       run-cookie:
         description: Whether or not run the cookiecutter tests
         value: ${{ jobs.change-detection.outputs.run-cookie || false }}
       run-rr:
         description: Whether or not run the repo-review tests
-        value: ${{ jobs.change-detection.outputs.run-rr || false }}
+        value: ${{ jobs.change-detection.outputs.run-cookie || false }}
 
 jobs:
   change-detection:
     name: Identify source changes
     runs-on: ubuntu-latest
     timeout-minutes: 1
     outputs:
       run-cookie: ${{ steps.cookie-changes.outputs.run-cookie || false }}
       run-rr: ${{ steps.rr-changes.outputs.run-rr || false }}
     steps:
       - uses: actions/checkout@v3
 
-      - name: Changed cookie-related files
+      - name: Get a list of the changed runtime-related files
         if: github.event_name == 'pull_request'
         id: changed-cookie-files
         uses: Ana06/get-changed-files@v2.2.0
         with:
-          format: "json"
           filter: |
             {{cookiecutter.project_name}}/**
             .github/workflows/ci.yml
             .github/workflows/reusable-cookie.yml
             noxfile.py
             hooks/**
             cookiecutter.json
-            copier.yml
-            extensions.py
       - name: Set a flag for running the tests
         if: >-
           github.event_name != 'pull_request' ||
-          steps.changed-cookie-files.outputs.added_modified_renamed != '[]'
+          steps.changed-cookie-files.outputs.added_modified_renamed != ''
         id: cookie-changes
         run: echo "run-cookie=true" >> "${GITHUB_OUTPUT}"
 
-      - name: Changed sp-repo-review-related files
+      - name: Get a list of the changed runtime-related files
         if: github.event_name == 'pull_request'
         id: changed-rr-files
         uses: Ana06/get-changed-files@v2.2.0
         with:
-          format: "json"
           filter: |
+            tests/**
             .github/workflows/ci.yml
             .github/workflows/reusable-rr-tests.yml
-            README.md
             noxfile.py
-            pyproject.toml
             src/**
-            tests/**
+            pyproject.toml
       - name: Set a flag for running the tests
         if: >-
           github.event_name != 'pull_request' ||
-          steps.changed-rr-files.outputs.added_modified_renamed != '[]'
+          steps.changed-rr-files.outputs.added_modified_renamed != ''
         id: rr-changes
         run: echo "run-rr=true" >> "${GITHUB_OUTPUT}"
```

### Comparing `sp_repo_review-2023.6.29/.github/workflows/reusable-cookie.yml` & `sp_repo_review-2023.6.7/.github/workflows/reusable-cookie.yml`

 * *Files 5% similar despite different names*

```diff
@@ -51,28 +51,27 @@
 
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.12"]
+        python-version: ["3.7", "3.11", "3.12-dev"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
         include:
-          - python-version: pypy-3.9
+          - python-version: pypy-3.8
             runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
-          allow-prereleases: true
 
       - name: Install nox
         run: pip install nox
 
       - name: Test setuptools
         run: nox -s 'tests(setuptools)'
 
@@ -106,29 +105,24 @@
       - name: Test setuptools PEP 621
         run: nox -s 'tests(setuptools621)'
 
       - name: Native poetry tooling
         run: nox -s 'native(poetry)'
 
       - name: Native pdm tooling
+        if: matrix.python-version != 'pypy-3.7'
         run: nox -s 'native(pdm)'
 
       - name: Activate MSVC for Meson
         if: runner.os == 'Windows'
         uses: ilammy/msvc-dev-cmd@v1
 
       - name: Test meson-python
         run: nox -s 'tests(mesonpy)'
 
-      - name: Compare copier template generation
-        run: nox -s compare_copier
-
-      - name: Compare cruft template generation
-        run: nox -s compare_cruft
-
   nox:
     name: Check included Noxfile
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `sp_repo_review-2023.6.29/.github/workflows/reusable-rr-tests.yml` & `sp_repo_review-2023.6.7/.github/workflows/reusable-rr-tests.yml`

 * *Files 23% similar despite different names*

```diff
@@ -39,24 +39,7 @@
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Run sp-repo-review action
         uses: ./
-
-  cog:
-    name: Run cog on README
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-
-      - uses: actions/setup-python@v4
-        with:
-          python-version: "3.11"
-
-      - name: Rerender README
-        run: |
-          pipx run nox -s readme
-          git diff --exit-code
```

### Comparing `sp_repo_review-2023.6.29/docs/README.md` & `sp_repo_review-2023.6.7/docs/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Scientific Python Library Development Guide
 
 This is maintained by the scientific Python community for the benefit of fellow
 scientists and research software engineers. The repository contains:
 
 - A guide
-- A copier/cookiecutter template that generates a template for a scientific
-  Python library
-- sp-repo-review, a plugin for [repo-review](https://repo-review.readthedocs.io)
+- A cookiecutter that generates a template for a scientific Python library
 
 ## Contributing to the documentation
 
 To build locally, install rbenv (remember to run `rbenv init` after installing,
 and `rbenv install 3.1.2`). Then:
 
 ```bash
```

### Comparing `sp_repo_review-2023.6.29/docs/_includes/head.html` & `sp_repo_review-2023.6.7/docs/_includes/head.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/docs/_includes/head_custom.html` & `sp_repo_review-2023.6.7/docs/_includes/head_custom.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/docs/_includes/interactive_repo_review.html` & `sp_repo_review-2023.6.7/docs/_includes/interactive_repo_review.html`

 * *Files 19% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 <script type="text/babel">
   const root = ReactDOM.createRoot(
     document.getElementById("interactive-repo-review-root")
   );
   root.render(
     <App
       header={false}
-      deps={["sp-repo-review==2023.06.29", "repo-review==0.8.0"]}
+      deps={["sp_repo_review==2023.06.01", "repo-review==0.7.0b8"]}
     />
   );
 </script>
```

### Comparing `sp_repo_review-2023.6.29/docs/_sass/custom/custom.scss` & `sp_repo_review-2023.6.7/docs/_sass/custom/custom.scss`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/docs/assets/favicon.ico` & `sp_repo_review-2023.6.7/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/docs/assets/images/logo.svg` & `sp_repo_review-2023.6.7/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/docs/assets/js/tabs.js` & `sp_repo_review-2023.6.7/docs/assets/js/tabs.js`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/docs/assets/js/webapp.js` & `sp_repo_review-2023.6.7/docs/assets/js/webapp.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -272,15 +272,15 @@
         /MaterialUI.ThemeProvider>
     );
 }
 
 class App extends React.Component {
     constructor(props) {
         super(props);
-        const deps_str = props.deps.join(" ");
+        const deps_str = props.deps.map((i) => `"${i}"`).join(", ");
         this.state = {
             results: [],
             repo: urlParams.get("repo") || "",
             branch: urlParams.get("branch") || "",
             msg: `${DEFAULT_MSG} Packages: ${deps_str}`,
             progress: false,
             err_msg: "",
@@ -352,15 +352,15 @@
             }
             console.log(families);
             for (const val of results_list) {
                 results[val.family].push({
                     name: val.name.toString(),
                     description: val.description.toString(),
                     state: val.result,
-                    err_msg: val.err_as_html().toString(),
+                    err_msg: val.err_markdown().toString(),
                     url: val.url.toString(),
                 });
             }
 
             this.setState({
                 results: results,
                 families: families,
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/guides/coverage.md` & `sp_repo_review-2023.6.7/docs/pages/guides/coverage.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 permalink: /guides/coverage/
 nav_order: 3
 parent: Topical Guides
 ---
 
 {% include toc.html %}
 
-# Code Coverage
-
 The "Code coverage" value of a codebase indicates how much of the
 production/development code is covered by the running unit tests. Maintainers
 try their best to keep this percentage high, and this process is often automated
 using tools such as `GitHub Actions` and `Codecov`. Hence, code coverage becomes
 a good metric (not always) to check if a particular codebase is well tested and
 reliable.
 
@@ -21,42 +19,38 @@
 
 - `pytest-cov`: allows developers to calculate and visualize the coverage value
 - `Codecov`: integrates with remote repositories, allowing developers to see and
   compare coverage value with each CI run
 - `GitHub Actions`: allows users to automatically upload coverage reports to
   `Codecov`
 
-{: .note-title }
-
-> Are there any alternatives?
+> ### Are there any alternatives?
 >
 > `coverage.py` is a popular Python library used to calculate coverage values,
 > but it is usually paired with python's `unittest`. On the other hand,
 > `pytest-cov` is built to integrate with `pytest` with minimal extra
 > configurations. Further, Coveralls is an alternative coverage platform, but we
 > recommend using Codecov because of its ease of use and integration with GitHub
 > Actions.
 
-{: .highlight-title }
-
-> Should increasing the coverage value be my top priority?
+> ### Should increasing the coverage value be my top priority?
 >
 > A low coverage percentage will definitely motivate you to add more tests, but
 > adding weak tests just for coverage's sake is not a good idea. The tests
 > should test your codebase thoroughly and should not be unreliable.
 
 ### Calculating code coverage locally
 
 `pytest` allows users to pass the `--cov` option to automatically invoke
 `pytest-cov`, which then generates a `.coverage` file with the calculated
 coverage value. The value of `--cov` option should be set to the name of your
 package. For example, run the following command to run tests to generate a
 `.coverage` file for the vector package -
 
-```bash
+```
 python -m pytest -ra --cov=vector --cov-branch tests/
 ```
 
 `--cov` option will also print a minimal coverage report in the terminal itself!
 See the [docs](https://pytest-cov.readthedocs.io/en/latest/) for more options.
 The `--cov-branch` option will enable
 [branch coverage](https://linearb.io/blog/what-is-branch-coverage/).
@@ -64,15 +58,15 @@
 ### Calculating code coverage in your workflows
 
 Your workflows should also run tests with the `--cov` option, which must be set
 to your package name. For example -
 
 ```yaml
 - name: Test package
-  run: python -m pytest --cov=vector tests/
+  run: python -m pytest -ra --cov=vector tests/
 ```
 
 This will automatically invoke `pytest-cov`, and generate a `.coverage` file,
 which can then be uploaded to `Codecov` using the [codecov/codecov-action][]
 action.
 
 ### Configuring Codecov and uploading coverage reports
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/guides/docs.md` & `sp_repo_review-2023.6.7/docs/pages/guides/tasks.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,312 +1,276 @@
 ---
 layout: page
-title: Writing documentation
-permalink: /guides/docs/
-nav_order: 4
+title: Task runners
+permalink: /guides/tasks/
+nav_order: 30
 parent: Topical Guides
 ---
 
 {% include toc.html %}
 
-# Writing documentation
+A task runner, like [make][] (fully general), [rake][] (Ruby general),
+[invoke][] (Python general), [tox][] (Python packages), or [nox][] (Python
+simi-general), is a tool that lets you specify a set of tasks via a common
+interface. These have been discouraged by some community projects in the past,
+since they can be a crutch, allowing poor packaging practices to be employed
+behind a custom script, and they can hide what is actually happening.
+
+We are carefully allowing an exception: [nox][]. Nox has two strong points that
+help with the above concerns. First, it is very explicit, and even prints what
+it is doing as it operates. Unlike the older tox, it does not have any implicit
+assumptions built-in. Second, it has very elegant built-in support for both
+virtual and Conda environments. This can greatly reduce new contributor friction
+with your codebase.
+
+A daily developer is _not_ expected to use nox for simple tasks, like running
+tests or linting. You should _not_ rely on nox to make a task that should be
+made simple and standard (like building a package) complicated. You are not
+expected to use nox for linting on CI, or often even for testing on CI, even if
+those tasks are provided for users. Nox is a few seconds slower than running
+directly in a custom environment - but for new users, and rarely run tasks, it
+is _much_ faster than explaining how to get setup or manually messing with
+virtual environments. It is also highly reproducible, creating and destroying
+the temporary environment each time.
+
+{% include rr.html id="PY007" %} You _should_ use nox to make it easy and simple
+for new contributors to run things. You _should_ use nox to make specialized
+developer tasks easy. You _should_ use nox to avoid making single-use virtual
+environments for docs and other rarely run tasks.
+
+Nox doesn't handle binary builds very well, so for compiled projects, it might
+be best left to just specialized tasks.
+
+[nox]: https://nox.thea.codes
+[tox]: https://tox.readthedocs.io
+[invoke]: https://www.pyinvoke.org
+[rake]: https://ruby.github.io/rake/
+[make]: https://www.gnu.org/software/make/
+
+## Nox
+
+### Installing
+
+Installing nox should be handled like any other Python _application_. You should
+either use a good package manager, like brew on macOS, or you should use pipx;
+either permanently (`pipx install nox`) or by running `pipx run nox` instead of
+`nox`.
+
+On GitHub Actions or Azure, pipx is available by default, so you should use
+`pipx run nox`. To give it access to all Python versions, you can use this
+action:
 
-Documentation used to require learning RestructureText (sometimes referred to as
-ReST / RST), but today we have great choices for documentation in markdown, the
-same format used by GitHub, Wikipedia, and others. There are two two major
-documentation toolchains, sphinx and mkdocs. This guide covers Sphinx, and uses
-the modern MyST plugin to get markdown support.
-
-## What to include
-
-Ideally, software documentation should include:
-
-- Introductory **tutorials**, to help new users (or potential users) understand
-  what the software can do and take their first steps.
-- Task-oriented **guides**, examples that address specific uses.
-- **Reference**, specifying the detailed inputs and outputs of every public
-  object in the codebase.
-- **Explanations** to convey deeper understanding of why and how the software
-  operates the way it does.
+```yaml
+- uses: wntrblm/nox@2022.8.7
+```
 
-This overall framework has a name, [Diátaxis][], and you can read more about it
-if you are interested.
+You can now access all current versions of Python from nox. At least in GitHub
+Actions, you should add `--forcecolor` to your nox runs to get color output in
+your logs, or set `env: FORCE_COLOR: 3`. If you'd like to customise the versions
+of Python prepared for you, then use this input:
 
-## Hand-written docs
+```yaml
+- uses: wntrblm/nox@2022.8.7
+  with:
+    python-versions:
+      "3.7, 3.8, 3.9, 3.10, 3.11, 3.12, pypy-3.8, pypy-3.9-nightly"
+```
 
-Create `docs/` directory within your project (i.e. next to `src/`). There is a
-sphinx-quickstart tool, but unnecessary files (make/bat, we recommend a
-cross-platform noxfile instead), and uses rst instead of markdown. Instead, this
-is our recommended starting point for `conf.py`:
+### Introduction
 
-### conf.py
+Nox is a tool for running tasks, called "sessions", inside temporary virtual
+environments. It is configured through Python and is designed to resemble
+pytest. The file it looks for is called `noxfile.py` by default. This is an
+example of a simple nox file:
 
 ```python
-from __future__ import annotations
-
-import importlib.metadata
+import nox
 
-project = "<package-name-here>"
-copyright = "2023, Your Name"
-author = "Your Name"
-version = release = importlib.metadata.version("<package-name-here>")
 
-extensions = [
-    "myst_parser",
-    "sphinx.ext.autodoc",
-    "sphinx.ext.intersphinx",
-    "sphinx.ext.mathjax",
-    "sphinx.ext.napoleon",
-    "sphinx_autodoc_typehints",
-    "sphinx_copybutton",
-]
-
-source_suffix = [".md", ".rst"]
-exclude_patterns = [
-    "_build",
-    "Thumbs.db",
-    ".DS_Store",
-    "**.ipynb_checkpoints",
-    ".env",
-    ".venv",
-]
-
-html_theme = "furo"
-
-intersphinx_mapping = {
-    "python": ("https://docs.python.org/3", None),
-}
-
-myst_enable_extensions = [
-    "colon_fence",
-]
-
-nitpick_ignore = [
-    ("py:class", "_io.StringIO"),
-    ("py:class", "_io.BytesIO"),
-]
-
-always_document_param_types = True
+@nox.session
+def tests(session: nox.Session) -> None:
+    """
+    Run the unit and regular tests.
+    """
+    session.install(".[test]")
+    session.run("pytest", *session.posargs)
 ```
 
-We start by setting some configuration values, but most notably we are getting
-the package version from the installed version of your package. We are listing
-several good extensions:
-
-- [`myst_parser`][myst] is the markdown parsing engine for sphinx.
-- `sphinx.ext.autodoc` will help us build API docs via Restructured Text and
-  dynamic analysis. Also see the package [sphinx-autodoc2][], which supports
-  markdown and uses static analysis; it might not be as battle tested at this
-  time, though.
-- `sphinx.ext.intersphinx` will cross-link to other documentation.
-- `sphinx.ext.mathjax` allows you to include mathematical formulas.
-- [`sphinx.ext.napoleon`][] adds support for several common documentation styles
-  like numpydoc.
-- `sphinx_autodoc_typehints` handles type hints
-- `sphinx_copybutton` adds a handle little copy button to code snipits.
-
-We are including both possible file extensions. We are also avoiding some common
-file patterns, just in case.
-
-For theme, you have several good options. The clean, light-weight `furo` theme
-is shown above; a related theme from the same author is being used for the
-CPython documentation in CPython 3.13. Many scientific packages choose the
-`sphinx-py-data` theme, which is also a good choice (no dark mode, though).
-
-We are enabling a useful MyST extension: `colon_fence` allows you to use three
-colons for directives, which might be highlighted better if the directive
-contains text than three backticks. See more built-in extensions in
-[MyST's docs](https://myst-parser.readthedocs.io/en/latest/syntax/optional.html).
-
-One key feature of Sphinx is interphinx, which allows documentation to
-cross-reference each other. You can list other projects you are using, but a
-good minimum is to at least link to the CPython docs. You need to provide the
-path to the `objects.inv` file, usually at the main documentation URL.
-
-We are going to be enabling nitpick mode, and when we do, there's a chance some
-classes will complain if they don't link with intersphinx. A couple of common
-examples are listed here (StringIO/BytesIO don't point at the right thing) -
-feel free to add/remove as needed.
+This will create a session called `tests`. The function receives the "session"
+argument, which gives you access to the virtual environment it creates. You can
+use `.install()` to install inside the environment, and `.run()` to run inside
+the environment. We are also using `session.posargs` to allow extra arguments to
+be passed through to pytest. There are
+[more useful methods](https://nox.thea.codes/en/stable/config.html#module-nox.sessions)
+as well.
 
-Finally, when we have static types, we'll want them always listed in the
-docstrings, even if the parameter isn't documented yet. Feel free to check
-[sphinx-autodoc-typehints](https://github.com/tox-dev/sphinx-autodoc-typehints)
-for more options.
+You can run this using:
 
-## index.md
+```console
+$ nox -s tests
+```
 
-Your `index.md` file can start out like this:
+You can see all defined sessions (along with the docstrings) using:
 
-````md
-# Project name
+```console
+$ nox -l
+```
 
-```{toctree}
-:maxdepth: 2
-:hidden:
+It is a good idea to list the sessions you want by default by setting
+`nox.options.sessions` near the top of your file:
 
+```python
+nox.options.sessions = ["lint", "tests"]
 ```
 
-```{include} ../README.md
-:start-after: <!-- SPHINX-START -->
-```
+This will keep you from running extra things like `docs` by default.
 
-## Indices and tables
+### Parametrizing
 
-- {ref}`genindex`
-- {ref}`modindex`
-- {ref}`search`
-````
+You can parametrize sessions. either on Python or on any other item.
 
-You can put your project name in as the title. The `toctree` directive houses
-your table of contents; you'll list each new page you add inside that directive.
+```python
+# Shortcut to parametrize Python
+@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"])
+def my_session(session: nox.Session) -> None:
+    ...
 
-If you want to inject a readme, you can use the `include` directive shown above.
-You don't want to add the README's title (and probably your badges) to your
-docs, so you can add a expression to your README (`<!-- SPHINX-START -->` above)
-to mark where you want the docs portion to start.
 
-You can add the standard indices and tables at the end.
+# General parametrization
+@nox.session
+@nox.parametrize("letter", ["a", "b"], ids=["a", "b"])
+def my_session(session: nox.Session, letter: str) -> None:
+    ...
+```
 
-### pyproject.toml additions
+The optional `ids=` parameter can give the parametrization nice names, like in
+pytest.
 
-Setting a `docs` extra looks like this:
+If a user does not have a particular version of Python installed, it will be
+skipped. You can use a Docker container to run in an environment where all
+Python's (3.6+) are available:
 
-```toml
-[project.optional-dependencies]
-docs = [
-  "furo",
-  "myst_parser >=0.13",
-  "sphinx >=4.0",
-  "sphinx-copybutton",
-  "sphinx-autodoc-typehints",
-]
+```console
+$ docker run --rm -itv $PWD:/src -w /src quay.io/pypa/manylinux_2_24_x86_64:latest pipx run nox
 ```
 
-While there are other ways to specify docs, and you don't have to make the docs
-requirements an extra, this is a good idea as it forces docs building to always
-install the project, rather than being tempted to install only sphinx and
-plugins and try to build against an uninstalled version of your project.
+Another container you can use is `thekevjames/nox:latest`; this has nox
+pre-installed (no pipx) and Python 2.7 and 3.5 as well.
 
-### .readthedocs.yaml
+### Useful sessions
 
-In order to use <https://readthedocs.org> to build, host, and preview your
-documentation, you must have a `.reathedocs.yml` file
-{% include rr.html id="RTD100" %} like this:
+Things like bumping the versions can be made sessions - since nox handles the
+environment for you, you can use any Python dependencies you like, and not have
+to worry about installing anything. Here are some commonly useful sessions that
+will likely look similar across different projects:
 
-```yaml
-# Read the Docs configuration file
-# See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
-
-version: 2
+#### Lint
 
-build:
-  os: ubuntu-22.04
-  tools:
-    python: "3.11"
+Ideally, all developers should be using pre-commit directly, but this helps new
+users.
 
-sphinx:
-  configuration: docs/conf.py
-
-python:
-  install:
-    - method: pip
-      path: .
-      extra_requirements:
-        - docs
+```python
+@nox.session
+def lint(session: nox.Session) -> None:
+    """
+    Run the linter.
+    """
+    session.install("pre-commit")
+    session.run(
+        "pre-commit", "run", "--show-diff-on-failure", "--all-files", *session.posargs
+    )
 ```
 
-This sets the readthedocs config version (2 is required)
-{% include rr.html id="RTD101" %}.
-
-The `build` table is the modern way to specify a runner. You need an `os` (a
-modern ubuntu should be fine) {% include rr.html id="RTD102" %}, a `tools` table
-(we'll use Python {% include rr.html id="RTD103" %}, several languages are
-supported here).
+#### Tests
 
-Adding a `sphinx` table tells readthedocs to enable Sphinx integration. MkDocs
-is supported too.
+```python
+import nox
 
-Finally, we have a `python` table with an `install` key to describe how to
-install our project. This will enable our "docs" extra.
 
-### noxfile.py additions
+@nox.session
+def tests(session: nox.Session) -> None:
+    """
+    Run the unit and regular tests.
+    """
+    session.install(".[test]")
+    session.run("pytest", *session.posargs)
+```
 
-Add a session to your `noxfile.py` to generate docs:
+#### Docs
 
 ```python
-@nox.session(reuse_venv=True)
+@nox.session
 def docs(session: nox.Session) -> None:
     """
-    Build the docs. Pass "--serve" to serve.
+    Build the docs. Pass "serve" to serve.
     """
 
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--serve", action="store_true", help="Serve after building")
-    args, posargs = parser.parse_known_args(session.posargs)
-
-    session.install("-e.[docs]")
+    session.install(".[docs]")
     session.chdir("docs")
+    session.run("sphinx-build", "-M", "html", ".", "_build")
 
-    session.run(
-        "sphinx-build",
-        "-n",  # nitpicky mode
-        "--keep-going",  # show all errors
-        "-T",  # full tracebacks
-        "-b",
-        "html",
-        ".",
-        f"_build/html",
-        *posargs,
-    )
-
-    if args.serve:
-        session.log("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
-        session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
+    if session.posargs:
+        if "serve" in session.posargs:
+            print("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
+            session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
+        else:
+            print("Unsupported argument to docs")
 ```
 
-## API docs
+This supports setting up a quick server as well, run like this:
+
+```console
+$ nox -s docs -- serve
+```
 
-To build API docs, you need to add the following nox job:
+#### Build (pure Python)
 
-### noxfile.py additions
+For pure Python packages, this could be useful:
 
 ```python
+from pathlib import Path
+import shutil
+
+DIR = Path(__file__).parent.resolve()
+
+
 @nox.session
-def build_api_docs(session: nox.Session) -> None:
+def build(session: nox.Session) -> None:
     """
-    Build (regenerate) API docs.
+    Build an SDist and wheel.
     """
-    session.install("sphinx")
-    session.chdir("docs")
-    session.run(
-        "sphinx-apidoc",
-        "-o",
-        "api/",
-        "--module-first",
-        "--no-toc",
-        "--force",
-        "../src/<package-name-here>",
-    )
+
+    build_p = DIR.joinpath("build")
+    if build_p.exists():
+        shutil.rmtree(build_p)
+
+    session.install("build")
+    session.run("python", "-m", "build")
 ```
 
-And you'll need this added to your `docs/index.md`:
+### Examples
 
-````md
-```{toctree}
-:maxdepth: 2
-:hidden:
-:caption: API
-
-api/<package-name-here>
-```
-````
-
-Note that your docstrings are still parsed as Restructured Text.
-
-<!-- prettier-ignore-start -->
-[diátaxis]: https://diataxis.fr/
-[sphinx]: https://www.sphinx-doc.org/
-[myst]: https://myst-parser.readthedocs.io/
-[organizing content]: https://myst-parser.readthedocs.io/en/latest/syntax/organising_content.html
-[sphinx-autodoc2]: https://sphinx-autodoc2.readthedocs.io/
-[`sphinx.ext.napoleon`]: https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html
-<!-- prettier-ignore-end -->
+A standard
+[powered by nox](https://github.com/scikit-hep/hist/blob/main/noxfile.py)
+package in Pure Python can be found in the Hist project of Scikit-HEP.
+
+A package that happens to use PDM (like Poetry but better) is Scikit-HEP UHI,
+which is
+[powered by nox](https://github.com/scikit-hep/uhi/blob/main/noxfile.py). Nox
+can setup a conda environment with ROOT (slow, but only nox and conda are
+required). There also is a version bump session, and does some custom logic too.
+
+The complex testing procedure powering Scientific Python Cookie is
+[powered by nox](https://github.com/scientific-python/cookie/blob/main/noxfile.py).
+It allows the complex CI jobs that generate projects and lint/test/build them to
+be run locally with no other setup.
+
+PyPA's cibuildwheel also is
+[powered by nox](https://github.com/pypa/cibuildwheel/blob/main/noxfile.py),
+running pip-tools' compile on every Python version to pin dependencies, as well
+as providing a standard interface to update Python and project listing update
+scripts. The docs job there runs mkdocs instead of Sphinx. Other PyPA projects
+using nox include [pip](https://github.com/pypa/pip/blob/main/noxfile.py),
+[pipx](https://github.com/pypa/pipx/blob/main/noxfile.py),
+[manylinux](https://github.com/pypa/manylinux/blob/main/noxfile.py),
+[packaging](https://github.com/pypa/packaging/blob/main/noxfile.py), and
+[packaging.python.org](https://github.com/pypa/packaging.python.org/blob/main/noxfile.py).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/guides/gha_basic.md` & `sp_repo_review-2023.6.7/docs/pages/guides/gha_basic.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 nav_order: 11
 parent: Topical Guides
 custom_title: GitHub Actions introduction
 ---
 
 {% include toc.html %}
 
-# GitHub Actions: Intro
-
 {% include rr.html id="GH100" %} The recommended CI for scientific Python
 projects is GitHub Actions (GHA), although its predecessor Azure is also in
 heavy usage, and other popular services (Travis, Appveyor, and Circle CI) may be
 found in a few packages. GHA is preferred due to the flexible, extensible design
 and the tight integration with the GitHub permissions model (and UI). Here is a
 guide in setting up a new package with GHA.
 
@@ -86,28 +84,27 @@
 ```yaml
 tests:
   runs-on: ubuntu-latest
   strategy:
     fail-fast: false
     matrix:
       python-version:
-        - "3.8"
+        - "3.7"
         - "3.11"
-        - "3.12"
+        - "3.12-dev"
   name: Check Python ${{ matrix.python-version }}
   steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0 # Only needed if using setuptools-scm
 
     - name: Setup Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-        allow-prereleases: true
 
     - name: Install package
       run: python -m pip install -e .[test]
 
     - name: Test package
       run: python -m pytest
 ```
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/guides/gha_pure.md` & `sp_repo_review-2023.6.7/docs/pages/guides/gha_pure.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,24 @@
 nav_order: 12
 parent: Topical Guides
 custom_title: GitHub Actions for pure Python wheels
 ---
 
 {% include toc.html %}
 
-# GitHub Actions: Pure Python wheels
-
 We will cover binary wheels [on the next page][], but if you do not have a
 compiled extension, this is called a universal (pure Python) package, and the
 procedure to make a "built" wheel is simple. At the end of this page, there is a
 recipe that can often be used exactly for pure Python wheels (if the previous
 recommendations were followed).
 
-{: .note }
-
-> Why make a wheel when there is nothing to compile? There are a multitude of
-> reasons that a wheel is better than only providing an sdist:
+> Note: Why make a wheel when there is nothing to compile? There are a multitude
+> of reasons that a wheel is better than only providing an sdist:
 >
-> - Wheels do not run `setup.py`, but simply install files into locations
+> - Wheels do not run setup.py, but simply install files into locations
 >   - Lower install requirements - users don't need your setup tools
 >   - Faster installs
 >   - Safer installs - no arbitrary code execution
 >   - Highly consistent installs
 > - Wheels pre-compile bytecode when they install
 >   - Initial import is not slower than subsequent import
 >   - Less chance of a permission issue
@@ -58,14 +54,17 @@
 instead of the releases - however, _please_ remember to make a GitHub release of
 your tag! It shows up in the GUI and it notifies anyone watching
 releases(-only). You will also need to change the event filter below.
 
 You can merge the CI job and the CD job if you want. To do that, preferably with
 the name "CI/CD", you can just combine the two `on` dicts.
 
+[`workflow_dispatch`]:
+  https://github.blog/changelog/2020-07-06-github-actions-manual-triggers-with-workflow_dispatch/
+
 ## Distribution: Pure Python wheels
 
 {% raw %}
 
 ```yaml
 dist:
   runs-on: ubuntu-latest
@@ -316,13 +315,11 @@
 </details>
 
 <!-- prettier-ignore-start -->
 
 [pep 517]: https://www.python.org/dev/peps/pep-0517/
 [pep 518]: https://www.python.org/dev/peps/pep-0518/
 [pypi trusted publisher docs]: https://docs.pypi.org/trusted-publishers/creating-a-project-through-oidc/
-[`workflow_dispatch`]: https://github.blog/changelog/2020-07-06-github-actions-manual-triggers-with-workflow_dispatch/
-
 
 <!-- prettier-ignore-end -->
 
 <script src="{% link assets/js/tabs.js %}"></script>
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/guides/gha_wheels.md` & `sp_repo_review-2023.6.7/docs/pages/guides/gha_wheels.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 nav_order: 13
 parent: Topical Guides
 custom_title: GitHub Actions for Binary Wheels
 ---
 
 {% include toc.html %}
 
-# GitHub Actions: Binary wheels
-
 Building binary wheels is a bit more involved, but can still be done effectively
 with GHA. This document will introduce [cibuildwheel][] for use in your project.
 The benefits of cibuildwheel are a larger user base, fast fixes from CI and pip,
 works on all major CI vendors (no lock-in), and covers cases we were not able to
 cover (like ARM). We will focus on GHA below.
 
 ## Header
@@ -117,15 +115,15 @@
 
   steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
         submodules: true
 
-    - uses: pypa/cibuildwheel@v2.13.1
+    - uses: pypa/cibuildwheel@v2.13.0
 
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         path: wheelhouse/*.whl
 ```
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/guides/mypy.md` & `sp_repo_review-2023.6.7/docs/pages/guides/mypy.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 permalink: /guides/mypy/
 nav_order: 8
 parent: Topical Guides
 ---
 
 {% include toc.html %}
 
-# Static type checking
-
 ## Basics
 
 The most exciting thing happening right now in Python development is static
 typing. Since Python 3.0, we've had function annotations, and since 3.6,
 variable annotations. In 3.5, we got a "typing" library, which provides tools to
 describe types. This is what static type hints look like:
 
@@ -125,15 +123,15 @@
 ### Protocols
 
 One of the best features of MyPy is support for structural subtyping via
 Protocols - formalized duck-typing, basically. This allows cross library
 interoperability, unlike traditional inheritance. Here’s how it works:
 
 ```python
-from typing import Protocol
+from typing import Protocol  # or typing_extensions for < 3.8
 
 
 class Duck(Protocol):
     def quack() -> str:
         ...
 ```
 
@@ -240,66 +238,14 @@
 syntax in non annotation locations (like unions in `isinstance`) unless Python
 supports it at runtime. And some libraries, like Typer and cattrs, use the
 annotations at runtime.
 
 You can use the above in earlier Python versions if you use strings manually,
 with the same caveats.
 
-## Tips for good types
-
-These are some guidelines to help you in writing good type hints.
-
-### Loose vs. specific types
-
-When you have a function, you should take as generic a type as possible, and
-return as specific a type as possible. For example:
-
-```python
-from __future__ import annotations
-from collections.abc import Iterable, Mapping
-
-
-# Bad!!!
-def count(x: list[str]) -> Mapping[str, int]:
-    result = {}
-    for item in x:
-        result[x] = result.get(x, 0) + 1
-    return result
-```
-
-This will require the user pass a list to use this function, when in fact any
-iterable of strings would work just fine. Then, using valid dictionary
-operations on the return value, like mutating operations, will be marked as
-invalid, since your type checker don't know you have an actual dict. Compare
-with this:
-
-```python
-# Good
-def count(x: Iterable[str]) -> dict[str, int]:
-    result = {}
-    for item in x:
-        result[x] = result.get(x, 0) + 1
-    return result
-```
-
-Now all iterables are accepted, and the type checkers knows you have an actual
-dict in the return. Usually functions should take `Iterable` (if the argument is
-iterated once) or `Sequence` (if it is iterated multiple times or used with
-`in`), or `Mapping`, or `Set`. Very rarely you might need `MutableMapping` or
-`MutableSet`, and if you really do, having it in the type helps a reader know
-that it's going to be mutated.
-
-If you have an output type that depends on an input type, try to pass that
-through, usually using TypeVar (or the new generic syntax in Python 3.12, but
-that's not available for older Pythons via an import).
-
-Also note that the best place to get these in modern Python is
-`collections.abc`, but if you need to subscript them at runtime, you'll need
-Python 3.9+ or the versions in `typing`.
-
 ## Final words
 
 When run alongside a good linter like flake8, this can catch a huge number of
 issues before tests or they are discovered in the wild! It also prompts _better
 design_, because you are thinking about how types work and interact. It's also
 more readable, since if I give you code like this:
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/guides/packaging_classic.md` & `sp_repo_review-2023.6.7/docs/pages/guides/packaging_classic.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 ---
 layout: page
-title: Classic packaging
+title: Classic Packaging
 permalink: /guides/packaging_classic/
 nav_order: 6
 parent: Topical Guides
 ---
 
 {% include toc.html %}
 
-# Classic packaging
-
 The libraries in the scientific Python ecosytem have a variety of different
 packaging styles, but this document is intended to outline a recommended style
 that new packages should follow, and existing packages should slowly adopt. The
 reasoning for each decision is outlined as well.
 
 There are currently several popular packaging systems. This guide covers
 [Setuptools][], which is currently the only system that supports compiled
 extensions. If you are not planning on writing C/C++ code, other systems like
 [Hatch][] are drastically simpler - most of this page is unneeded for those
 systems.
 
 Also see the [Python packaging guide][], especially the [Python packaging
 tutorial][].
 
-{: .note }
-
+> <h2 class="no_toc">Note:</h2>
+>
 > Raw source lives in git and has a `setup.py`. You _can_ install directly from
 > git via pip, but normally users install from distributions hosted on PyPI.
 > There are three options: **A)** A source package, called an SDist and has a
 > name that ends in `.tar.gz`. This is a copy of the GitHub repository, stripped
 > of a few specifics like CI files, and possibly with submodules included (if
 > there are any). **B)** A pure python wheel, which ends in `.whl`; this is only
 > possible if there are no compiled extensions in the library. This does _not_
 > contain a setup.py, but rather a `PKG_INFO` file that is rendered from
 > setup.py (or from another build system). **C)** If not pure Python, a
 > collection of wheels for every binary platform, generally one per supported
 > Python version and OS as well.
 >
 > Developer requirements (users of A or git) are generally higher than the
-> requirements to use B or C. Poetry and optionally flit create SDists that
-> include a `setup.py`, and all alternate packing systems produce "normal"
-> wheels.
+> requirements to use B or C. Poetry creates SDists that include a setup.py, and
+> both alternate packing systems produce "normal" wheels.
 
 ## Package structure (medium priority)
 
 All packages _should_ have a `src` folder, with the package code residing inside
 it, such as `src/<package>/`. This may seem like extra hassle; after all, you
 can type "`python`" in the main directory and avoid installing it if you don't
 have a `src` folder! However, this is a bad practice, and it causes several
@@ -194,17 +191,15 @@
 ```
 
 {% endraw %}
 
 If you fill in the override version setting when triggering a manual workflow
 run, that version will be forced, otherwise, it works as normal.
 
-{: .note }
-
-> Make sure you have a good gitignore, probably starting from
+> Note: Make sure you have a good gitignore, probably starting from
 > [GitHub's Python one](https://github.com/github/gitignore/blob/main/Python.gitignore)
 > or using a [generator site](https://www.toptal.com/developers/gitignore).
 
 You should also add these two files:
 
 `.git_archival.txt`:
 
@@ -218,16 +213,16 @@
 And `.gitattributes` (or add this line if you are already using this file):
 
 ```text
 .git_archival.txt  export-subst
 ```
 
 This will allow git archives (including the ones generated from GitHub) to also
-support versioning. This will only work with `setuptools_scm>=7` (though adding
-the files won't hurt older versions).
+support versioning. This will only work with `setuptools_scm>=7`, which requires
+Python 3.7+ (though adding the files won't hurt older versions).
 
 ### Classic in-source versioning
 
 Recent versions of `setuptools` have improved in-source versioning. If you have
 a simple file that includes a line with a simple PEP 440 style version, like
 `version = "2.3.4.beta1"`, then you can use a line like this in your
 `setup.cfg`:
@@ -277,14 +272,15 @@
     Operating System :: MacOS
     Operating System :: Microsoft :: Windows
     Operating System :: POSIX
     Operating System :: Unix
     Programming Language :: C++
     Programming Language :: Python
     Programming Language :: Python :: 3 :: Only
+    Programming Language :: Python :: 3.7
     Programming Language :: Python :: 3.8
     Programming Language :: Python :: 3.9
     Programming Language :: Python :: 3.10
     Programming Language :: Python :: 3.11
     Programming Language :: Python :: 3.12
     Topic :: Scientific/Engineering
     Topic :: Scientific/Engineering :: Information Analysis
@@ -299,15 +295,15 @@
     Changelog = https://package.readthedocs.io/en/latest/changelog.html
 
 
 [options]
 packages = find:
 install_requires =
     numpy>=1.13.3
-python_requires = >=3.8
+python_requires = >=3.7
 include_package_data = True
 package_dir =
     =src
 zip_safe = False
 
 [options.packages.find]
 where = src
@@ -433,30 +429,14 @@
 
 include LICENSE README.md pyproject.toml setup.py setup.cfg
 global-exclude __pycache__ *.py[cod] .*
 ```
 
 Note that Scikit-build currently may have issues with MANIFEST.in.
 
-## Command line
-
-If you want to ship an "app" that a user can run from the command line, you need
-to add a `console_scripts` entry point. The form is:
-
-```ini
-[options.entry_points]
-console_scripts =
-    cliapp = packakge.__main__:main
-```
-
-The format is command line app name as the key, and the value is the path to the
-function, followed by a colon, then the function to call. If you use
-`__main__.py` as the file, then `python -m` + the module will also work to call
-the app.
-
 [^1]:
     You shouldn't ever have to run commands like this, they are implementation
     details of setuptools. For this command, you should use `python -m build -s`
     instead (and `pip install build`).
 
 [^2]:
     Actually, Flit produces a backward-compatible `setup.py` by default when
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/guides/packaging_simple.md` & `sp_repo_review-2023.6.7/docs/pages/guides/packaging_simple.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 ---
 layout: page
-title: Simple packaging
+title: Simple Packaging
 permalink: /guides/packaging-simple/
 nav_order: 5
 parent: Topical Guides
 ---
 
 {% include toc.html %}
 
-# Simple packaging
-
 Python packages without binary extensions and fairly simple builds can use a
 modern build system instead of the classic but verbose setuptools and
 `setup.py`. The one you select doesn't really matter that much; they all use a
 [standard configuration language][metadata] introduced in [PEP 621][]. The
 PyPA's Flit is a great option. [scikit-build-core][] and [meson-python][] are
 being developed to support this sort of configuration, enabling binary extension
 packages to benefit too. These [PEP 621][] tools currently include [Hatch][],
 [PDM][], [Flit][], [Trampolim][], [Whey][], and [Setuptools][]. [Poetry][] will
 eventually gain support in 2.0.
 
 Binaries mostly are unsupported in existing PEP 621 tools, though better support
 is coming.
 
-{: .note-title }
-
-> Classic files
+> ## Classic files
 >
 > These systems do not use or require `setup.py`, `setup.cfg`, or `MANIFEST.in`.
 > Those are for setuptools. Unless you are using setuptools, of course, which
 > still uses `MANIFEST.in`. You can convert the old files using
 > `pipx run hatch new --init` or with
 > [ini2toml](https://ini2toml.readthedocs.io/en/latest/).
 
-{: .highlight-title }
-
-> Selecting a backend
+> ## Selecting a backend
 >
 > Backends handle metadata the same way, so the choice comes down to how you
 > specify what files go into an SDist and extra features, like getting a version
 > from VCS. If you don't have an existing preference, hatchling is an excellent
 > choice, balancing speed, configurability, and extendability.
 
 ## pyproject.toml: build-system
@@ -94,24 +88,25 @@
 readme = "README.md"
 authors = [
   { name = "My Name", email = "me@email.com" },
 ]
 maintainers = [
   { name = "My Organization", email = "myemail@email.com" },
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 
 dependencies = [
   "numpy>=1.13.3",
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering :: Physics",
 ]
@@ -219,26 +214,28 @@
   (which is a good idea anyway).
 - [Flit info here](https://flit.readthedocs.io/en/latest/pyproject_toml.html#sdist-section).
   Flit requires manual inclusion/exclusion in many cases, like using a dirty
   working directory.
 - [PDM info here](https://pdm.fming.dev/pyproject/tool-pdm/#include-and-exclude-package-files).
 - Setuptools still uses `MANIFEST.in`.
 
-{: .warning }
+<details markdown="1"><summary>Warning for Flit</summary>
 
-> Flit will not use VCS (like git) to populate the SDist if you use standard
-> tooling, even if it can do that using its own tooling. So make sure you list
-> explicit include/exclude rules, and test the contents:
->
-> ```bash
-> # Show SDist contents
-> tar -tvf dist/*.tar.gz
-> # Show wheel contents
-> unzip -l dist/*.whl
-> ```
+Flit will not use VCS (like git) to populate the SDist if you use standard
+tooling, even if it can do that using its own tooling. So make sure you list
+explicit include/exclude rules, and test the contents:
+
+```bash
+# Show SDist contents
+tar -tvf dist/*.tar.gz
+# Show wheel contents
+unzip -l dist/*.whl
+```
+
+</details>
 
 ## Extras
 
 It is recommended to use extras instead of or in addition to making requirement
 files. These extras a) correctly interact with install requires and other
 built-in tools, b) are available directly when installing via PyPI, and c) are
 allowed in `requirements.txt`, `install_requires`, `pyproject.toml`, and most
@@ -254,30 +251,15 @@
 mpl = [
   "matplotlib >=2.0",
 ]
 ```
 
 Self dependencies can be used by using the name of the package, such as
 `dev = ["package[test,examples]"]`, but this requires Pip 21.2 or newer. We
-recommend providing at least `test` and `docs`.
-
-## Command line
-
-If you want to ship an "app" that a user can run from the command line, you need
-to add a `script` entry point. The form is:
-
-```toml
-[project.scripts]
-cliapp = "packakge.__main__:main"
-```
-
-The format is command line app name as the key, and the value is the path to the
-function, followed by a colon, then the function to call. If you use
-`__main__.py` as the file, then `python -m` + the module will also work to call
-the app.
+recommend providing at least `test`, `docs`, and `dev`.
 
 [flit]: https://flit.readthedocs.io
 [poetry]: https://python-poetry.org
 [pdm]: https://pdm.fming.dev
 [trampolim]: https://github.com/FFY00/trampolim
 [whey]: https://whey.readthedocs.io
 [hatch]: https://hatch.pypa.io/latest
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/guides/pytest.md` & `sp_repo_review-2023.6.7/docs/pages/guides/pytest.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 permalink: /guides/pytest/
 nav_order: 2
 parent: Topical Guides
 ---
 
 {% include toc.html %}
 
-# Testing with pytest
-
 Tests are crucial to writing reliable software. A good test suite allows you to:
 
 - Immediately know if a new platform or software version works,
 - Refactor and cleanup your code with confidence,
 - Evaluate the effect of additions and changes.
 
 Python used to have three major choices for tests; but now [pytest][] is used
@@ -25,17 +23,15 @@
 - Coverage: using as many inputs as possible increases the chances of finding
   something that breaks.
 - Performance: the faster the tests, the more situations you can run your tests
   in CI.
 - Reporting: when things break, you should get good information about what
   broke.
 
-{: .note-title }
-
-> What about other choices?
+> ### What about other choices?
 >
 > The alternative library, `nose`, has been abandoned in favor of `pytest`,
 > which can run nose-style tests. The standard library has a test suite as well,
 > but it's extremely verbose and complex; and since "developers" run tests, your
 > test requirements don't affect users. And `pytest` can run stdlib style
 > testing too. So just use `pytest`. All major packages use it too, including
 > `NumPy`. Most other choices, like [Hypothesis][], are related to `pytest` and
@@ -75,14 +71,15 @@
 minversion = "6.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = ["error"]
 log_cli_level = "info"
 testpaths = [
   "tests",
+  "ignore:(ast.Str|Attribute s|ast.NameConstant|ast.Num) is deprecated:DeprecationWarning:_pytest",
 ]
 ```
 
 {% include rr.html id="PP302" %} The `minversion` will print a nicer error if
 your `pytest` is too old (though, ironically, it won't read this is the version
 is too old, so setting "6" or less in `pyproject.toml` is rather pointless). The
 `addopts` setting will add whatever you put there to the command line when you
@@ -134,18 +131,19 @@
 `filename.py::test_name`.
 
 If a test fails, you have lots of options to save time in debugging. Adding
 `-l`/`--showlocals` will print out the local values in the tracebacks (and can
 be added by default, see above). You can run `pytest` with `--pdb`, which will
 drop you into a debugger on each failure. Or you can use `--trace` which will
 drop you into a debugger at the start of each test selected (so probably use the
-selection methods above). `pytest` also supports `breakpoint()`. You can also
-start out in your debugger at the beginning of the last failed test with
-`--trace --lf`. [See the docs](https://docs.pytest.org/en/stable/usage.html) for
-more running tips.
+selection methods above). `pytest` also supports `breakpoint()` in Python 3.7+.
+You can also start out in your debugger at the beginning of the last failed test
+with `--trace --lf`.
+[See the docs](https://docs.pytest.org/en/stable/usage.html) for more running
+tips.
 
 ## Guidelines for writing good tests
 
 Time spent learning all the powerful tools pytest has to offer will be well
 spent! You can make your tests more granular, mock things that aren't available
 (or are slow to run), parametrize, and much more.
 
@@ -279,21 +277,21 @@
 like tests marked "slow", for example. Just add `-m <marker>` when running
 pytest to run a group of marked tests. This is an expression; you can use
 `not <marker>` as well.
 
 Probably the most useful built-in mark is `skipif`:
 
 ```python
-@pytest.mark.skipif("sys.version_info >= (3, 8)")
-def test_only_on_38plus():
+@pytest.mark.skipif("sys.version_info >= (3, 7)")
+def test_only_on_37plus():
     x = 3
     assert f"{x = }" == "x = 3"
 ```
 
-Now this test will only run on Python 3.8 or newer, and will be skipped on
+Now this test will only run on Python 3.7 or newer, and will be skipped on
 earlier versions. You don't have to use a string for the condition, but if you
 don't, add a `reason=` so there will still be a nice printout explaining why the
 test was skipped.
 
 You can also use `xfail` for tests that are expected to fail (you can even
 strictly test them as failing if you want). You can use `parametrize` to make a
 single parameterized test instead of sharing them (with fixtures). There's a
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/guides/repo_review.md` & `sp_repo_review-2023.6.7/docs/pages/guides/repo_review.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 ---
 layout: page
-title: Repo-Review
+title: Repo Review
 permalink: /guides/repo-review/
 nav_order: 110
 parent: Topical Guides
 interactive_repo_review: true
 ---
 
-# Repo-Review
-
 You can check the style of a GitHub repository below. Enter any repository, such
 as `scikit-hep/hist`, and the branch you want to check, such as `main` (it must
 exist). This will produce a list of results - green checkmarks mean this rule is
 followed, red errors mean the rule is not. A yellow warning sign means that the
 check was skipped because a previous required check failed. Some checks will
 fail, that's okay - the goal is bring all possible issues to your attention, not
 to force compliance with arbitrary checks.
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/guides/style.md` & `sp_repo_review-2023.6.7/docs/pages/guides/style.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 nav_order: 8
 parent: Topical Guides
 custom_title: Style guide
 ---
 
 {% include toc.html %}
 
-# Style (static checkers)
-
 ## Pre-commit
 
 {% include rr.html id="PY006" %} Scientific Python projects often use
 [pre-commit][] to check code style. It can be installed through `brew` (macOS)
 or `pip` (anywhere). There are two modes to use it locally; you can check
 manually with `pre-commit run` (changes only) or `pre-commit run --all-files`
 (all). You can also run `pre-commit install` to add checks as a git pre-commit
@@ -137,36 +135,36 @@
 {% include rr.html id="PC111" %} If you want Black used in your documentation,
 you can use blacken-docs. This can even catch syntax errors in code snippets! It
 supports markdown and restructured text. Note that because black is in
 `additional_dependencies`, you'll have to keep it up to date manually.
 
 ```yaml
 - repo: https://github.com/asottile/blacken-docs
-  rev: "1.14.0"
+  rev: "1.13.0"
   hooks:
     - id: blacken-docs
-      additional_dependencies: [black==23.3.0]
+      additional_dependencies: [black==23.1.0]
 ```
 
 </details>
 
 ## Ruff
 
 {% include rr.html id="PC190" %} [Ruff][] [(docs)][ruff docs] is a Python code
 linter and autofixer that replaces many other tools in the ecosystem with a
 ultra-fast (written in Rust), single zero-dependency package. All plugins are
 compiled in, so you can't get new failures from plugins updating without
 updating your pre-commit hook.
 
 [ruff docs]: https://beta.ruff.rs
-[ruff]: https://github.com/astral-sh/ruff
+[ruff]: https://github.com/charliermarsh/ruff
 
 ```yaml
-- repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: "v0.0.275"
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  rev: "v0.0.271"
   hooks:
     - id: ruff
       args: ["--fix", "--show-fixes"]
 ```
 
 {% include rr.html id="PC191" %} The `--fix` argument is optional, but
 recommended, since you can inspect and undo changes in git.
@@ -202,15 +200,15 @@
   "PD",          # pandas-vet
 ]
 extend-ignore = [
   "PLR",    # Design related pylint codes
   "E501",   # Line too long
   "PT004",  # Use underscore for non-returning fixture (use usefixture instead)
 ]
-target-version = "py38"
+target-version = "py37"
 typing-modules = ["mypackage._compat.typing"]
 src = ["src"]
 unfixable = [
   "T20",  # Removes print statements
   "F841", # Removes unused variables
 ]
 exclude = []
@@ -378,15 +376,15 @@
 
 Over time, you can end up with extra "noqa" comments that are no longer needed.
 This is a flake8 helper that removes those comments when they are no longer
 required.
 
 ```yaml
 - repo: https://github.com/asottile/yesqa
-  rev: "v1.5.0"
+  rev: "v1.4.0"
   hooks:
     - id: yesqa
 ```
 
 You need to have the same extra dependencies as flake8. In YAML, you can save
 the list given to yesqa and repeat it in flake8 using `&flake8-dependencies` and
 `*flake8-dependencies` after the colon.
@@ -425,26 +423,26 @@
 style syntax. Most useful to keep Python 2 outdated constructs out, it can even
 do some code updates for different versions of Python 3, like adding f-strings
 when clearly better (please always use them, they are faster) if you set
 `--py36-plus` (for example). This is a recommended addition for any project.
 
 ```yaml
 - repo: https://github.com/asottile/pyupgrade
-  rev: "v3.7.0"
+  rev: "v3.4.0"
   hooks:
     - id: pyupgrade
-      args: ["--py38-plus"]
+      args: ["--py37-plus"]
 ```
 
 [pyupgrade]: https://github.com/asottile/pyupgrade:
 
 > <h4 class="no_toc">Note:</h4>
 >
-> If you set this to at least `--py37-plus`, you can add the annotations import
-> by adding the following line to your isort pre-commit hook configuration:
+> If you set this to `--py37-plus`, you can add the annotations import by adding
+> the following line to your isort pre-commit hook configuration:
 >
 > ```yaml
 > args: ["-a", "from __future__ import annotations"]
 > ```
 >
 > Also make sure isort comes before pyupgrade. Now when you run pre-commit, it
 > will clean up your annotations to 3.7+ style, too!
@@ -471,15 +469,15 @@
 
 Read more about type checking on the [dedicated page][mypy page].
 
 The MyPy addition for pre-commit:
 
 ```yaml
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: "v1.4.1"
+  rev: "v1.3.0"
   hooks:
     - id: mypy
       files: src
       args: []
 ```
 
 You should always specify args, as the hook's default hides issues - it's
@@ -492,15 +490,15 @@
 
 {% include rr.html id="MY100" %} MyPy has a config section in `pyproject.toml`
 that looks like this:
 
 ```ini
 [tool.mypy]
 files = "src"
-python_version = "3.8"
+python_version = "3.7"
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 
 
 # You can disable imports or control per-module/file settings here
@@ -606,15 +604,15 @@
 {% include rr.html id="PC160" %} You can and should check for spelling errors in
 your code too. If you want to add this, you can use [codespell][] for common
 spelling mistakes. Unlike most spell checkers, this has a list of mistakes it
 looks for, rather than a list of "valid" words. To use:
 
 ```yaml
 - repo: https://github.com/codespell-project/codespell
-  rev: "v2.2.5"
+  rev: "v2.2.4"
   hooks:
     - id: codespell
       args: ["-L", "sur,nd"]
 ```
 
 You can list allowed spellings in a comma separated string passed to `-L` (or
 `--ignore-words-list` - usually it is better to use long options when you are
@@ -678,15 +676,15 @@
 ## Clang-format (C++ only)
 
 If you have C++ code, you should have a `.clang-format` file and use the
 following pre-commit config:
 
 ```yaml
 - repo: https://github.com/pre-commit/mirrors-clang-format
-  rev: "v16.0.6"
+  rev: "v16.0.4"
   hooks:
     - id: clang-format
       types_or: [c++, c, cuda]
 ```
 
 This will use 1-2 MB binary wheels from PyPI on all common platforms. You can
 generated such a file using
@@ -740,15 +738,15 @@
 get some very nice linting, including catching some problematic code that
 otherwise is hard to catch. PyLint is generally not a good candidate for
 pre-commit, since it needs to have your package installed - it is less static of
 check than Flake8. Here is a suggested pyproject.toml entry to get you started:
 
 ```toml
 [tool.pylint]
-py-version = "3.8"
+py-version = "3.7"
 jobs = "0"
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.enable = ["useless-suppression"]
 messages_control.disable = [
   "design",
   "fixme",
@@ -778,15 +776,15 @@
 [nbQA](https://github.com/nbQA-dev/nbQA). The most useful one is probably Ruff:
 
 ```yaml
 - repo: https://github.com/nbQA-dev/nbQA
   rev: "1.7.0"
   hooks:
     - id: nbqa-ruff
-      additional_dependencies: [ruff==0.0.275]
+      additional_dependencies: [ruff==0.0.253]
 ```
 
 You can pass extra flags to Ruff via the hook, like
 `args: ["--extend-ignore=F821,F401"]`.
 
 ### Black
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/patterns/data_files.md` & `sp_repo_review-2023.6.7/docs/pages/patterns/data_files.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ---
 layout: page
 title: Including data files
 permalink: /patterns/data_files/
-nav_order: 3
+nav_order: 30
 parent: Patterns
 ---
 
 {% include toc.html %}
 
-# Including data files
+# Including Data Files
 
 In this section you will:
 
 - Understand the importance of keeping large files out of your package.
 - Learn some alternative approaches.
 - Learn how to include small data files in your package.
 
@@ -36,17 +36,17 @@
   enough to simulate it accurately, you don't know enough to write useful tests
   against it.
 - Can you write a Python function that fetches the data on demand from some
   public URL? This is the approach used by projects such as scikit-learn that
   need to download large datasets for their examples and tests.
 
 If you use one these alternatives, add the names of the generated or downloaded
-files to the project's `.gitignore` file, which is provided by the
-[copier][]/[cookiecutter][] template. This helps protect you against
-accidentally committing the file to git.
+files to the project's `.gitignore` file, which was provided by the cookiecutter
+template. This helps protect you against accidentally committing the file to
+git.
 
 If the file in question is a text file and not very large (\< 100 kB) than it's
 reasonable to just bundle it with the package. If not, see the recommendation at
 the end.
 
 ## How to Package Data Files
 
@@ -197,15 +197,11 @@
     known_hash="sha256:50ef9a52c621b7c0c506ad1fe1b8ee8a158a4d7c8e50ddfce1e273a422dca3f9",
 )
 ```
 
 On repeated runs of this command, the locally cached filename would be used
 instead of downloading the data again.
 
-<!-- prettier-ignore-start -->
 [importlib_resources]: https://importlib-resources.readthedocs.io/en/latest/
 [osf.io]: https://osf.io/
 [pooch]: https://www.fatiando.org/pooch/latest/
 [zenodo]: https://zenodo.org/
-[copier]: https://copier.readthedocs.io
-[cookiecutter]: https://cookiecutter.readthedocs.io
-<!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/principles/design.md` & `sp_repo_review-2023.6.7/docs/pages/principles/design.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,52 +4,50 @@
 permalink: /principles/design/
 nav_order: 2
 parent: Principles
 ---
 
 {% include toc.html %}
 
-# Design recommendations
+# Design Recommendations
 
-## Keep I/O separate
+## Keep I/O Separate
 
 One of the biggest impediments to reuse of scientific code is when I/O
 code---assuming certain file locations, names, formats, or layouts---is
 interspersed with scientific logic.
 
 I/O-related functions should _only_ perform I/O. For example, they should take
 in a filepath and return a numpy array, or a dictionary of arrays and metadata.
 The valuable scientific logic should be encoded in functions that take in
 standard data types and return standard data types. This makes them easier to
 test, maintain when data formats change, or reuse for unforeseen applications.
 
-## Duck typing is a good idea
+## Duck Typing is a Good Idea
 
 [Duck typing][] treats objects based on what they can _do_, not based on what
 type they _are_. "If it walks like a duck and it quacks like a duck, then it
 must be a duck."
 
 Python in general and scientific Python in particular leverage _interfaces_
 (also known as Protocols) to support interoperability and reuse. For example, it
 is possible to pass a pandas DataFrame to the `numpy.sum` function even though
 pandas was created long after `numpy.sum`. This is because `numpy.sum` avoids
 assuming it will be passed specific data types; it accepts any object that
 provides the right methods (interfaces). Where possible, avoid `isinstance`
 checks in your code, and try to make your functions work on the broadest
 possible range of input types.
 
-## Consider: can this just be a function?
+## Consider: Can this just be a function?
 
 Not everything needs to be object-oriented. Object-oriented design needs to
 follow the same principles as other code, like modularity, and be well tested.
 If you can get away with writing functions processing existing datatypes like a
 DataFrame, do so.
 
-{: .highlight }
-
 > It is better to have 100 functions operate on one data structure than 10
 > functions on 10 data structures.
 >
 > -- From ACM's SIGPLAN publication, (September, 1982), Article "Epigrams in
 > Programming", by Alan J. Perlis of Yale University.
 
 A popular talk, ["Stop Writing Classes"][], illustrates how some situations that
@@ -97,15 +95,15 @@
 
 These classes don’t have to be immutable. Maybe you can load more data to loaded
 data. But they are easier to use correctly when they at least avoid a mutating
 state that makes subsets of available operations (i.e. methods) invalid. Note
 that tab completion in this case would show exactly the allowed set of
 operations each time.
 
-## Consider: do I really want a custom class?
+## Consider: Do I really want a custom class?
 
 Using built-in Python types (`int`, `float`, `str`) and standard scientific
 Python types like NumPy array and Pandas DataFrame makes code interoperable. It
 enables data to flow between different libraries smoothly, and to be extended in
 unforeseen ways.
 
 As an example, the widely-used library scikit-image initially experimented with
@@ -143,15 +141,15 @@
 You'll remember (well, at least you are more likely to remember) to handle
 special cases like lists vs strings or values that could also be `None`.
 
 When using static typing, duck typing is expressed via Protocols. These should
 be strongly preferred over older solutions like inheritance or ABCs if possible,
 as they trade a little extra code to remove dependencies between objects.
 
-## Permissiveness isn't always convenient
+## Permissiveness Isn't Always Convenient
 
 Overly permissive code can lead to very confusing bugs. If you need a flexible
 user-facing interface that tries to "do the right thing" by guessing what the
 users wants, separate it into two layers: a thin "friendly" layer on top of a
 "cranky" layer that takes in only exactly what it needs and does the actual
 work. The cranky layer should be easy to test; it should be constrained about
 what it accepts and what it returns. This layered design makes it possible to
@@ -163,28 +161,28 @@
 
 Exceptions should just be raised: don't catch them and print. Exceptions are a
 tool for being clear about what the code needs and letting the caller decide
 what to do about it. _Application_ code (e.g. GUIs) should catch and handle
 errors to avoid crashing, but _library_ code should generally raise errors
 unless it is sure how the user or the caller wants to handle them.
 
-## Write useful error messages
+## Write Useful Error Messages
 
 Be specific. Include what the wrong value was, what was wrong with it, and
 perhaps how it might be fixed. For example, if the code fails to locate a file
 it needs, it should say what it was looking for and where it looked.
 
-## Write for readability
+## Write for Readability
 
 Unless you are writing a script that you plan to delete tomorrow or next week,
 your code will probably be read many more times than it is written. And today's
 "temporary solution" often becomes tomorrow's critical code. Therefore, optimize
 for clarity over brevity, using descriptive and consistent names.
 
-## Complexity is always conserved
+## Complexity is Always Conserved
 
 Complexity is always conserved and is strictly greater than the system the code
 is modeling. Attempts to hide complexity from the user frequently backfire.
 
 For example, it is often tempting to hide certain reused keywords in a function,
 shortening this:
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/principles/index.md` & `sp_repo_review-2023.6.7/docs/pages/principles/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/docs/pages/principles/process.md` & `sp_repo_review-2023.6.7/docs/pages/principles/process.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 permalink: /principles/process/
 nav_order: 1
 parent: Principles
 ---
 
 {% include toc.html %}
 
-# Process recommendations
+# Process Recommendations
 
 ## Collaborate
 
 Software developed by several people is preferable to software developed by one.
 By adopting the conventions and tooling used by many other scientific software
 projects, you are well on your way to making it easy for others to contribute.
 Familiarity works in both directions: it will be easier for others to understand
@@ -29,23 +29,23 @@
 Having more than one person understanding every part of the code prevents
 systematic risks for the project and keeps you from being tied to that code.
 
 If you can bring together contributors with diverse scientific backgrounds, it
 becomes easier to identify functionality that should be generalized for reuse by
 different fields.
 
-## Don't be afraid to refactor
+## Don't Be Afraid to Refactor
 
 No code is ever right the first (or second) time.
 
 Refactoring the code once you understand the problem and the design trade-offs
 more fully helps keep the code maintainable. Version control, tests, and linting
 are your safety net, empowering you to make changes with confidence.
 
-## Prefer "wide" over "deep"
+## Prefer "Wide" over "Deep"
 
 It should be possible to reuse pieces of software in a way not anticipated by
 the original author. That is, branching out from the initial use case should
 enable unplanned functionality without a massive increase in complexity.
 
 When building new things, work your way down to the lowest level, understand
 that level, and then build back up. Try to imagine what else you would want to
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/tutorials/dev-environment.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/dev-environment.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 permalink: /tutorials/dev-environment/
 nav_order: 1
 parent: Tutorials
 ---
 
 {% include toc.html %}
 
-# Intro to development
-
 In this section you will:
 
 - Create an isolated software area ("virtual environment") to work in.
 - Open a code editor.
 
-## Development environment
+# Development environment
 
 If you want to work on Python software, you should _always_ have a virtual
 environment, an area to install the software that is isolated from other
 programs running on your system. A user may not always have one, but a developer
 always should.
 
 Why? You do not want to risk interfering with your main system environment, you
@@ -29,15 +27,15 @@
 delete one and start over---while it is very hard to clean up or update a main
 system environment.
 
 There are many (arguably _too_ many) ways to do this in Python. Any modern tool
 should be fine, but here we recommend two options popular in the scientific
 Python community. If you already use a different way, that's fine, use that.
 
-### Option 1: Using pip
+## Option 1: Using pip
 
 The most basic option is to use `venv`, which comes by default with Python.
 
 ```bash
 python3 -m venv .venv
 ```
 
@@ -74,30 +72,26 @@
 script `activate` in your current shell. This causes `pip` and `python` to work
 within this new environment, isolated from system-wide packages. It adds a bit
 of text to your prompt so you don't forget that you are in an environment.
 
 The activation script installs a function `deactivate`; type that at any time to
 leave the environment (or just close your shell).
 
-{: .note-title }
-
-> Optional Alternative
+> <h4 class="no_toc">Optional Alternative</h4>
 >
 > Alternatively, you can use the `virtualenv` package, which has the same syntax
 > as `venv` and is a little faster. Unlike `venv`, it is not built in to Python;
 > it has to be installed as `pip install virtualenv`.
 
-{: .highlight-title }
-
-> For Advanced Users Using Custom Shells
+> <h4 class="no_toc">For Advanced Users Using Custom Shells</h4>
 >
 > If you like a different shell, like fish, there are several `activate`
 > scripts; the default one expects a bash-like shell.
 
-### Option 2: Using conda
+## Option 2: Using conda
 
 You can also develop in conda. This is an especially good option if:
 
 - You want an easy way to choose a specific version of Python
 - Your project will depend on complex software libraries that are not readily
   pip-installable
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/tutorials/docs.md` & `sp_repo_review-2023.6.7/docs/pages/guides/writing-docs.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 ---
 layout: page
 title: Writing documentation
-permalink: /tutorials/docs/
-nav_order: 5
-parent: Tutorials
+permalink: /guides/writing-docs/
+nav_order: 4
+parent: Topical Guides
 ---
 
 {% include toc.html %}
 
-# Writing documentation
+# Writing Documentation
+
+## What to include
+
+Ideally, software documentation should include:
+
+- Introductory **tutorials**, to help new users (or potential users) understand
+  what the software can do and take their first steps
+- Task-oriented **guides**, examples that address specific uses
+- **Reference**, specifying the detailed inputs and outputs of every public
+  object in the codebase
+- **Explanations** to convey deeper understanding of why and how the software
+  operates the way it does
+
+This overall framework has a name, [Diátaxis][], and you can read more about it
+if you are interested.
 
 ## Build the documentation
 
 Scientific Python software documentation can be written in the Markdown syntax,
 which looks like this:
 
 ````markdown
@@ -51,15 +66,14 @@
 `docs/conf.py`.
 
 ```py
 # content of docs/conf.py
 
 project = "example"
 extensions = ["myst_parser"]
-source_suffix = [".rst", ".md"]
 ```
 
 And, at `docs/index.md`, we will create a minimal front page for our
 documentation.
 
 ```markdown
 # Example documentation
@@ -150,30 +164,37 @@
 inputs and outputs of every public object in the codebase. This should not be
 written by hand; that would be tedious and have a high probably of human error
 or drifting out of sync over time.
 
 MyST recommends using [sphinx-autodoc2][]. However, we currently recommend using
 the built-in sphinx `autodoc` and `autosummary` extensions because they
 interoperates well with docstrings written to the numpydoc standard. To invoke
-them, we need to employ yet another syntax (reST). Fortunately, you can simply
+them, we need to employ yet another syntax (reST). F:ortunately, you can simply
 copy/paste these examples.
 
+Install `numpydoc`.
+
+```bash
+pip install numpydoc
+```
+
 In `docs/conf.py`, add to the list of extensions.
 
 ```py
 extensions = [
     # whatever you already have in here...
+
+    "numpydoc",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
-    "sphinx.ext.napoleon",
 ]
 ```
 
-(Note that these extensions come with `sphinx`, so there is nothing more to
-install.)
+(Note that `sphinx.ext.autodoc` and `sphinx.ext.autosummary` come installed with
+`sphinx`, so there is nothing more to install.)
 
 You can document a single object (e.g. function), shown inline on the page
 
 ````markdown
 ```{eval-rst}
 .. autofunction:: example.refraction.snell
     :noindex:
@@ -189,17 +210,14 @@
     :nosignatures:
     :toctree: generated
 
     example.refraction.snell
 ```
 ````
 
-See the [guide]({% link pages/guides/docs.md %}) for more information on how to
-integrate this into a package, and setup for nox.
-
 <!-- prettier-ignore-start -->
 [diátaxis]: https://diataxis.fr/
 [sphinx]: https://www.sphinx-doc.org/
 [myst]: https://myst-parser.readthedocs.io/
 [organizing content]: https://myst-parser.readthedocs.io/en/latest/syntax/organising_content.html
 [sphinx-autodoc2]: https://sphinx-autodoc2.readthedocs.io/
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/tutorials/index.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/docs/pages/tutorials/module.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/module.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 permalink: /tutorials/module/
 nav_order: 2
 parent: Tutorials
 ---
 
 {% include toc.html %}
 
-# Inline documentation
-
 In this section you will:
 
 - Place some code in a module.
 - Provide inline documentation (a "docstring").
 
-## Module
+# Module
 
 As a concrete example, let's suppose we have a simple function that encodes
 [Snell's Law][]. Perhaps this function currently lives in a Jupyter notebook or
 a `.py` file in an email attachment. We want to put into some more lasting,
 maintainable, reusable, and/or shareable form.
 
 Here is the code:
@@ -70,15 +68,15 @@
 - At the top, there is a succinct, one-line summary of the function's purpose.
   It must one line.
 
 - (Optional) There is an paragraph elaborating on that summary.
 
 - There is a section listing input parameters, with the structure
 
-  ```
+  ```none
   parameter_name : parameter_type
       optional description
   ```
 
   Note that space before the `:`. That is part of the standard.
 
 - Similar parameters may be combined into one entry for brevity's sake, as we
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/tutorials/packaging.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/packaging.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 ---
 layout: page
-title: Packaging
+title: Package
 permalink: /tutorials/packaging/
 nav_order: 3
 parent: Tutorials
 ---
 
-{% include toc.html %}
-
-# Packaging
-
 In the section you will:
 
 - Place your module in an installable package.
 - Employ version control.
 - Install and use the package.
 
 For more about packaging, see our [packaging guide][].
 
+# Package
+
 ## Create a minimal installable Python package
 
 Let’s create a Python package that contains this function.
 
 First, create a new directory for your software package, called `example`, and
 move into that:
```

### Comparing `sp_repo_review-2023.6.29/docs/pages/tutorials/test.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/test.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 layout: page
 title: Test
 permalink: /tutorials/test/
 nav_order: 4
 parent: Tutorials
 ---
 
-{% include toc.html %}
-
-# Test
-
 In this section you will:
 
 - Write a test to verify the correctness of the code.
 
 If you already know pytest, check our advanced [pytest guide][].
 
+# Test
+
 You should add a test right away while the details are still fresh in mind.
 Writing tests lets you make future improvements with confidence that any
 unintended changes or breakage with not go unnoticed. Writing tests also tends
 to encouraging you to write modular, reusable code, because it is easier to
 test.
 
 ## Write some tests
```

### Comparing `sp_repo_review-2023.6.29/src/sp_repo_review/families.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/families.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,11 +32,8 @@
         ),
         "mypy": Family(
             name="MyPy",
         ),
         "ruff": Family(
             name="Ruff",
         ),
-        "docs": Family(
-            name="Documentation",
-        ),
     }
```

### Comparing `sp_repo_review-2023.6.29/src/sp_repo_review/checks/general.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/general.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/src/sp_repo_review/checks/github.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/github.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/src/sp_repo_review/checks/mypy.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/mypy.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/src/sp_repo_review/checks/precommit.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/precommit.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/src/sp_repo_review/checks/pyproject.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/pyproject.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/src/sp_repo_review/checks/ruff.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/ruff.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/tests/test_package.py` & `sp_repo_review-2023.6.7/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.gitignore` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -46,25 +46,25 @@
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: "v0.0.264"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
-{%- if cookiecutter.backend == "setuptools" or cookiecutter.backend == "pybind11" %}
+{%- if cookiecutter.project_type == "setuptools" or cookiecutter.project_type == "pybind11" %}
 
   - repo: https://github.com/asottile/setup-cfg-fmt
     rev: "v2.2.0"
     hooks:
       - id: setup-cfg-fmt
-        args: [--include-version-classifiers, --max-py-version=3.12]
+        args: [--include-version-classifiers, --max-py-version=3.11]
 
 {%- endif %}
 
-{%- if cookiecutter.backend in ["pybind11", "skbuild", "mesonpy"] %}
+{%- if cookiecutter.project_type in ["pybind11", "skbuild", "mesonpy"] %}
 
   - repo: https://github.com/pre-commit/mirrors-clang-format
     rev: "v16.0.2"
     hooks:
       - id: clang-format
         types_or: [c++, c, cuda]
 
@@ -93,24 +93,24 @@
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
         exclude: .pre-commit-config.yaml
 
-{%- if cookiecutter.backend in ["setuptools", "pybind11"] %}
+{%- if cookiecutter.project_type in ["setuptools", "pybind11"] %}
 
   - repo: https://github.com/mgedmin/check-manifest
     rev: "0.49"
     hooks:
       - id: check-manifest
         stages: [manual]
 {%- endif %}
 
-{%- if cookiecutter.backend == "skbuild" %}
+{%- if cookiecutter.project_type == "skbuild" %}
 
   - repo: https://github.com/cheshirekow/cmake-format-precommit
     rev: "v0.6.13"
     hooks:
       - id: cmake-format
 
 {%- endif %}
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/README.md` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 [![Documentation Status][rtd-badge]][rtd-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![Conda-Forge][conda-badge]][conda-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
-{%- if cookiecutter.org | lower == "scikit-hep" %}
+[![Gitter][gitter-badge]][gitter-link]
+{%- if cookiecutter.org == "Scikit-HEP" %}
 [![Scikit-HEP][sk-badge]](https://scikit-hep.org/)
 {%- endif %}
 
-<!-- SPHINX-START -->
-
 <!-- prettier-ignore-start -->
 [actions-badge]:            {{cookiecutter.url}}/workflows/CI/badge.svg
 [actions-link]:             {{cookiecutter.url}}/actions
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/{{cookiecutter.project_name}}
 [conda-link]:               https://github.com/conda-forge/{{cookiecutter.project_name}}-feedstock
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
 [github-discussions-link]:  {{cookiecutter.url}}/discussions
+[gitter-badge]:             https://badges.gitter.im/{{cookiecutter.url}}/community.svg
+[gitter-link]:              https://gitter.im/{{cookiecutter.url}}/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
 [pypi-link]:                https://pypi.org/project/{{cookiecutter.project_name}}/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/{{cookiecutter.project_name}}
 [pypi-version]:             https://img.shields.io/pypi/v/{{cookiecutter.project_name}}
 [rtd-badge]:                https://readthedocs.org/projects/{{cookiecutter.project_name}}/badge/?version=latest
 [rtd-link]:                 https://{{cookiecutter.project_name}}.readthedocs.io/en/latest/?badge=latest
-{%- if cookiecutter.org | lower == "scikit-hep" %}
+{%- if cookiecutter.org == "Scikit-HEP" %}
 [sk-badge]:                 https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
 {%- endif %}
 
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/noxfile.py` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/noxfile.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import argparse
-{%- if cookiecutter.backend != "pybind11" %}
+{%- if cookiecutter.project_type != "pybind11" %}
 import shutil
 from pathlib import Path
 {%- endif %}
 
 import nox
 
-{% if cookiecutter.backend != "pybind11" -%}
+{% if cookiecutter.project_type != "pybind11" -%}
 DIR = Path(__file__).parent.resolve()
 
 {% endif -%}
 
 nox.options.sessions = ["lint", "pylint", "tests"]
 
 
@@ -49,46 +49,22 @@
 def docs(session: nox.Session) -> None:
     """
     Build the docs. Pass "--serve" to serve.
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--serve", action="store_true", help="Serve after building")
-    parser.add_argument(
-        "-b", dest="builder", default="html", help="Build target (default: html)"
-    )
-    args, posargs = parser.parse_known_args(session.posargs)
-
-    if args.builder != "html" and args.serve:
-        session.error("Must not specify non-HTML builder with --serve")
+    args = parser.parse_args(session.posargs)
 
     session.install(".[docs]")
     session.chdir("docs")
-
-    if args.builder == "linkcheck":
-        session.run(
-            "sphinx-build", "-b", "linkcheck", ".", "_build/linkcheck", *posargs
-        )
-        return
-
-    session.run(
-        "sphinx-build",
-        "-n",  # nitpicky mode
-        "-T",  # full tracebacks
-        "-W",  # Warnings as errors
-        "--keep-going",  # See all errors
-        "-b",
-        args.builder,
-        ".",
-        f"_build/{args.builder}",
-        *posargs,
-    )
+    session.run("sphinx-build", "-M", "html", ".", "_build")
 
     if args.serve:
-        session.log("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
+        print("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
         session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
 
 
 @nox.session
 def build_api_docs(session: nox.Session) -> None:
     """
     Build (regenerate) API docs.
@@ -96,22 +72,22 @@
 
     session.install("sphinx")
     session.chdir("docs")
     session.run(
         "sphinx-apidoc",
         "-o",
         "api/",
-        "--module-first",
         "--no-toc",
         "--force",
-        "../src/{{ cookiecutter.__project_slug }}",
+        "--module-first",
+        "../src/{{ cookiecutter.project_name.replace('-', '_') }}",
     )
 
 
-{%- if cookiecutter.backend != "pybind11" %}
+{%- if cookiecutter.project_type != "pybind11" %}
 
 
 @nox.session
 def build(session: nox.Session) -> None:
     """
     Build an SDist and wheel.
     """
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/pyproject.toml` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 [build-system]
-{%- if cookiecutter.backend == "trampolim" %}
+{%- if cookiecutter.project_type == "trampolim" %}
 requires = ["trampolim>=0.1.0"]
 build-backend = "trampolim"
-{%- elif cookiecutter.backend == "whey" %}
+{%- elif cookiecutter.project_type == "whey" %}
 requires = ["whey>=0.0.17"]
 build-backend = "whey"
-{%- elif cookiecutter.backend == "pdm" %}
+{%- elif cookiecutter.project_type == "pdm" %}
 requires = ["pdm-backend"]
 build-backend = "pdm.backend"
-{%- elif cookiecutter.backend == "maturin" %}
+{%- elif cookiecutter.project_type == "maturin" %}
 requires = ["maturin>=0.12,<0.15"]
 build-backend = "maturin"
-{%- elif cookiecutter.backend == "hatch" %}
+{%- elif cookiecutter.project_type == "hatch" %}
 requires = ["hatchling"]
 build-backend = "hatchling.build"
-{%- elif cookiecutter.backend == "setuptools621" %}
+{%- elif cookiecutter.project_type == "setuptools621" %}
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
-{%- elif cookiecutter.backend == "flit" %}
+{%- elif cookiecutter.project_type == "flit" %}
 requires = ["flit_core >=3.4"]
 build-backend = "flit_core.buildapi"
-{%- elif cookiecutter.backend == "setuptools" %}
+{%- elif cookiecutter.project_type == "setuptools" %}
 requires = ["setuptools>=42", "setuptools_scm[toml]>=3.4"]
 build-backend = "setuptools.build_meta"
-{%- elif cookiecutter.backend == "pybind11" %}
+{%- elif cookiecutter.project_type == "pybind11" %}
 requires = ["setuptools>=42", "setuptools_scm[toml]>=3.4", "pybind11"]
 build-backend = "setuptools.build_meta"
-{%- elif cookiecutter.backend == "skbuild"  %}
+{%- elif cookiecutter.project_type == "skbuild"  %}
 requires = ["pybind11", "scikit-build-core"]
 build-backend = "scikit_build_core.build"
-{%- elif cookiecutter.backend == "mesonpy"  %}
+{%- elif cookiecutter.project_type == "mesonpy"  %}
 requires = ["pybind11", "meson-python"]
 build-backend = "mesonpy"
-{%- elif cookiecutter.backend == "poetry" %}
+{%- elif cookiecutter.project_type == "poetry" %}
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 {%- endif %}
 
-{%- if cookiecutter.backend in ["setuptools", "pybind11"] %}
+{%- if cookiecutter.project_type in ["setuptools", "pybind11"] %}
 
 
 [tool.setuptools_scm]
-write_to = "src/{{ cookiecutter.__project_slug }}/_version.py"
+write_to = "src/{{ cookiecutter.project_slug }}/_version.py"
 
 
 [tool.check-manifest]
 ignore = [
   ".github/**",
   "docs/**",
   ".pre-commit-config.yaml",
-  ".readthedocs.yaml",
+  ".readthedocs.yml",
   "src/*/_version.py",
   "noxfile.py",
 ]
 
-{%- elif cookiecutter.backend == "poetry" %}
+{%- elif cookiecutter.project_type == "poetry" %}
 
 
 [tool.poetry]
 name = "{{ cookiecutter.project_name }}"
 version = "0.1.0"
 authors = [
   "{{ cookiecutter.full_name }} <{{ cookiecutter.email }}>",
 ]
-{%- if cookiecutter.org == "scikit-hep" %}
+{%- if cookiecutter.org == "Scikit-HEP" %}
 maintainers = [
   "The Scikit-HEP admins <scikit-hep-admins@googlegroups.com>",
 ]
 {%- endif %}
 homepage = "{{ cookiecutter.url }}"
 repository = "{{ cookiecutter.url }}"
 {%- if cookiecutter.license == "BSD" %}
@@ -86,60 +86,58 @@
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8"
-typing_extensions = { version = ">=4.6", python = "<3.11" }
+python = ">=3.7"
+typing_extensions = { version = ">=3.7", python = "<3.8" }
 
 furo = { version = ">=22", optional = true }
 myst_parser = { version = ">=0.13", optional = true }
 pytest = { version = ">=6", optional = true }
 pytest-cov = { version = ">=3", optional = true }
 sphinx = { version = ">=4.0", optional = true }
 sphinx_copybutton = { version = ">=0.3.0", optional = true }
-sphinx-autodoc-typehints = { version = "*", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = ">= 6"
 pytest-cov = ">= 3"
 
 [tool.poetry.extras]
 test = ["pytest", "pytest-cov"]
 dev = ["pytest", "pytest-cov"]
 docs = [
   "furo",
   "myst_parser",
   "sphinx",
-  "sphinx_autodoc_typehints",
   "sphinx_copybutton",
 ]
 
 
 {%- else %}
 
 
 [project]
 name = "{{ cookiecutter.project_name }}"
-{%- if cookiecutter.backend not in ["trampolim", "flit", "hatch"] %}
+{%- if cookiecutter.project_type not in ["trampolim", "flit", "hatch"] %}
 version = "0.1.0"
 {%- endif %}
 authors = [
   { name = "{{ cookiecutter.full_name }}", email = "{{ cookiecutter.email }}" },
 ]
-{%- if cookiecutter.org | lower == "scikit-hep" %}
+{%- if cookiecutter.org == "Scikit-HEP" %}
 maintainers = [
   { name = "The Scikit-HEP admins", email = "scikit-hep-admins@googlegroups.com" },
 ]
 {%- endif %}
 description = "{{ cookiecutter.project_short_description }}"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
 {%- if cookiecutter.license == "BSD" %}
   "License :: OSI Approved :: BSD License",
 {%- elif cookiecutter.license == "Apache" %}
@@ -147,73 +145,73 @@
 {%- elif cookiecutter.license == "MIT" %}
   "License :: OSI Approved :: MIT License",
 {%- endif %}
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
-{%- if cookiecutter.backend in ["trampolim", "flit", "hatch"] %}
+{%- if cookiecutter.project_type in ["trampolim", "flit", "hatch"] %}
 dynamic = ["version"]
 {%- endif %}
 dependencies = [
-  "typing_extensions >=4.6; python_version<'3.11'",
+  "typing_extensions >=3.7; python_version<'3.8'",
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
   "pytest-cov >=3",
 ]
 dev = [
   "pytest >=6",
   "pytest-cov >=3",
 ]
 docs = [
   "sphinx>=4.0",
   "myst_parser>=0.13",
-  "sphinx_book_theme>=0.1.0",
+  "sphinx-book-theme>=0.1.0",
   "sphinx_copybutton",
-  "sphinx_autodoc_typehints",
   "furo",
 ]
 
 [project.urls]
 Homepage = "{{ cookiecutter.url }}"
 "Bug Tracker" = "{{ cookiecutter.url }}/issues"
 Discussions = "{{ cookiecutter.url }}/discussions"
 Changelog = "{{ cookiecutter.url }}/releases"
 {%- endif %}
 
 
-{%- if cookiecutter.backend == "skbuild" %}
+{%- if cookiecutter.project_type == "skbuild" %}
 [tool.scikit-build]
 minimum-version = "0.2"
 build-dir = "build/{cache_tag}"
-{%- elif cookiecutter.backend == "whey" %}
+{%- elif cookiecutter.project_type == "whey" %}
 [tool.whey]
 source-dir = "src"
-{%- elif cookiecutter.backend == "trampolim" %}
+{%- elif cookiecutter.project_type == "trampolim" %}
 [tool.trampolim]
 module-location = "src"
-{%- elif cookiecutter.backend == "hatch" %}
+{%- elif cookiecutter.project_type == "hatch" %}
 [tool.hatch]
-version.path = "src/{{ cookiecutter.__project_slug  }}/__init__.py"
+version.path = "src/{{ cookiecutter.project_slug  }}/__init__.py"
 envs.default.dependencies = [
   "pytest",
   "pytest-cov",
 ]
-{%- elif cookiecutter.backend == "pdm" %}
+{%- elif cookiecutter.project_type == "pdm" %}
 [tool.pdm.dev-dependencies]
 devtest = ["pytest", "pytest-cov"]
 {%- endif %}
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
@@ -226,34 +224,34 @@
 log_cli_level = "INFO"
 testpaths = [
   "tests",
 ]
 
 
 [tool.coverage]
-run.source = ["{{ cookiecutter.__project_slug }}"]
+run.source = ["{{ cookiecutter.project_slug }}"]
 port.exclude_lines = [
   'pragma: no cover',
   '\.\.\.',
   'if typing.TYPE_CHECKING:',
 ]
 
 [tool.mypy]
 files = ["src", "tests"]
-python_version = "3.8"
+python_version = "3.7"
 warn_unused_configs = true
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 disallow_untyped_defs = false
 disallow_incomplete_defs = false
 
 [[tool.mypy.overrides]]
-module = "{{ cookiecutter.__project_slug  }}.*"
+module = "{{ cookiecutter.project_slug  }}.*"
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
@@ -280,16 +278,16 @@
   "NPY",         # NumPy specific rules
   "PD",          # pandas-vet
 ]
 extend-ignore = [
   "PLR",    # Design related pylint codes
   "E501",   # Line too long
 ]
-target-version = "py38"
-typing-modules = ["{{ cookiecutter.__project_slug }}._compat.typing"]
+target-version = "py37"
+typing-modules = ["{{ cookiecutter.project_slug }}._compat.typing"]
 src = ["src"]
 unfixable = [
   "T20",  # Removes print statements
   "F841", # Removes unused variables
 ]
 exclude = []
 flake8-unused-arguments.ignore-variadic-names = true
@@ -297,16 +295,16 @@
 
 [tool.ruff.per-file-ignores]
 "tests/**" = ["T20"]
 "noxfile.py" = ["T20"]
 
 
 [tool.pylint]
-py-version = "3.8"
-ignore-paths= ["src/{{ cookiecutter.__project_slug }}/_version.py"]
+py-version = "3.7"
+ignore-paths= ["src/{{ cookiecutter.project_slug }}/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
   "design",
   "fixme",
   "line-too-long",
   "missing-module-docstring",
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools,pybind11.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
-name = {{ cookiecutter.__project_slug }}
+name = {{ cookiecutter.project_slug }}
 description = {{ cookiecutter.project_short_description }}
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = {{ cookiecutter.url }}
 author = {{ cookiecutter.full_name }}
 author_email = {{ cookiecutter.email }}
-{%- if cookiecutter.org | lower == "scikit-hep" %}
+{%- if cookiecutter.org == "Scikit-HEP" %}
 maintainer = The Scikit-HEP admins
 maintainer_email = scikit-hep-admins@googlegroups.com
 {%- endif %}
 license = BSD-3-Clause
 license_file = LICENSE
 platforms =
     Any
@@ -25,32 +25,32 @@
 {%- elif cookiecutter.license == "MIT" %}
     License :: OSI Approved :: MIT License
 {%- endif %}
     Operating System :: OS Independent
     Programming Language :: Python
     Programming Language :: Python :: 3
     Programming Language :: Python :: 3 :: Only
+    Programming Language :: Python :: 3.7
     Programming Language :: Python :: 3.8
     Programming Language :: Python :: 3.9
     Programming Language :: Python :: 3.10
     Programming Language :: Python :: 3.11
-    Programming Language :: Python :: 3.12
     Topic :: Scientific/Engineering
     Typing :: Typed
 project_urls =
     Documentation = https://{{ cookiecutter.project_name }}.readthedocs.io/
     Bug Tracker = {{ cookiecutter.url }}/issues
     Discussions = {{ cookiecutter.url }}/discussions
     Changelog = {{ cookiecutter.url }}/releases
 
 [options]
 packages = find:
 install_requires =
-    typing-extensions>=4.6;python_version<'3.11'
-python_requires = >=3.8
+    typing-extensions>=3.7;python_version<'3.8'
+python_requires = >=3.7
 include_package_data = True
 package_dir =
     =src
 
 [options.packages.find]
 where = src
 
@@ -58,12 +58,11 @@
 dev =
     pytest>=6
     pytest-cov>=3
 docs =
     furo>=22
     myst-parser>=0.13
     sphinx>=4.0
-    sphinx-autodoc-typehints
     sphinx-copybutton
 test =
     pytest>=6
     pytest-cov>=3
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/Cargo-maturin.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
-name = "{{ cookiecutter.__project_slug }}"
+name = "{{ cookiecutter.project_slug }}"
 version = "0.1.0"
 edition = "2018"
 
 [lib]
 name = "_core"
 # "cdylib" is necessary to produce a shared library for Python to import from.
 crate-type = ["cdylib"]
 
 [package.metadata.maturin]
-name = "{{ cookiecutter.__project_slug }}._core"
-python-packages = ["{{ cookiecutter.__project_slug }}"]
+name = "{{ cookiecutter.project_slug }}._core"
+python-packages = ["{{ cookiecutter.project_slug }}"]
 python-source = "src"
 
 [dependencies]
 rand = "0.8.3"
 
 [dependencies.pyo3]
 version = "0.18.1"
 # "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
-# "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.8
-features = ["extension-module", "abi3-py38"]
+# "abi3-py37" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.7
+features = ["extension-module", "abi3-py37"]
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/meson-mesonpy.build`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 project(
-  '{{ cookiecutter.__project_slug }}',
+  '{{ cookiecutter.project_slug }}',
   'cpp',
   version: '0.1.0',
   license: '{{ cookiecutter.license }}',
   meson_version: '>= 0.64.0',
   default_options: [
     'buildtype=debugoptimized',
     'cpp_std=c++11',
   ],
 )
-name = '{{ cookiecutter.__project_slug }}'
+name = '{{ cookiecutter.project_slug }}'
 
 py_mod = import('python')
 py = py_mod.find_installation(pure: false)
 
 pybind11_config = find_program('pybind11-config')
 pybind11_config_ret = run_command(pybind11_config, ['--includes'], check: true)
 pybind11 = declare_dependency(
     include_directories: [pybind11_config_ret.stdout().split('-I')[-1].strip()],
 )
 
 install_subdir('src' / name, install_dir: py.get_install_dir() / name, strip_directory: true)
 
 py.extension_module('_core',
     'src/main.cpp',
-    subdir: '{{ cookiecutter.__project_slug }}',
+    subdir: '{{ cookiecutter.project_slug }}',
     install: true,
     dependencies : [pybind11],
     link_language : 'cpp',
     override_options: [
         'cpp_rtti=true',
     ]
 )
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-pybind11.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) {{ cookiecutter.__year }}, {{ cookiecutter.full_name }}
+# Copyright (c) {{ cookiecutter.year }}, {{ cookiecutter.full_name }}
 #
 # Distributed under the 3-clause BSD license, see accompanying file LICENSE
 # or {{ cookiecutter.url }} for details.
 
 from __future__ import annotations
 
 from setuptools import setup  # isort:skip
@@ -12,15 +12,15 @@
 
 # Note:
 #   Sort input source files if you glob sources to ensure bit-for-bit
 #   reproducible builds (https://github.com/pybind/python_example/pull/53)
 
 ext_modules = [
     Pybind11Extension(
-        "{{ cookiecutter.__project_slug }}._core",
+        "{{ cookiecutter.project_slug }}._core",
         ["src/main.cpp"],
         cxx_std=11,
     ),
 ]
 
 
 setup(
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'Apache' %}LICENSE{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/LICENSE`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+{%- if cookiecutter.license == "BSD" %}
+BSD 3-Clause License
+
+Copyright (c) {{ cookiecutter.year }}, {{ cookiecutter.full_name }}.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the vector package developers nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+{%- elif cookiecutter.license == "Apache" %}
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -183,20 +214,41 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright {{ cookiecutter.__year }} {{ cookiecutter.full_name }}
+   Copyright {{ cookiecutter.year }} {{ cookiecutter.full_name }}
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
+{%- elif cookiecutter.license == "MIT" %}
+Copyright {{ cookiecutter.year }} {{ cookiecutter.full_name }}
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+{%- endif %}
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'BSD' %}LICENSE{% endif %}` & `sp_repo_review-2023.6.7/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) {{ cookiecutter.__year }}, {{ cookiecutter.full_name }}.
+Copyright (c) 2021, Henry Schreiner.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Nox handles everything for you, including setting up an temporary virtual
 environment for each run.
 
 # Setting up a development environment manually
 
 You can set up a development environment by running:
 
-{% if cookiecutter.backend == "poetry" -%}
+{% if cookiecutter.project_type == "poetry" -%}
 
 ```bash
 poetry install
 ```
 
 {%- else -%}
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.github/matchers/pylint.json` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.github/workflows/ci.yml` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/ci.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- set compiled = cookiecutter.backend in ["pybind11", "maturin", "skbuild", "mesonpy"] -%}
+{%- set compiled = cookiecutter.project_type in ["pybind11", "maturin", "skbuild", "mesonpy"] -%}
 name: CI
 
 on:
   workflow_dispatch:
   pull_request:
   push:
     branches:
@@ -44,32 +44,31 @@
   checks:
     name: {% raw %}Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}{% endraw %}
     runs-on: {% raw %}${{ matrix.runs-on }}{% endraw %}
     needs: [pre-commit]
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.11", "3.12"]
+        python-version: ["3.7", "3.11", "3.12-dev"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
         include:
-          - python-version: pypy-3.9
+          - python-version: pypy-3.8
             runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - uses: actions/setup-python@v4
         with:
           python-version: {% raw %}${{ matrix.python-version }}{% endraw %}
-          allow-prereleases: true
 
-      {%- if cookiecutter.backend == "mesonpy" %}
+      {%- if cookiecutter.project_type == "mesonpy" %}
       - name: Activate MSVC for Meson
         if: runner.os == 'Windows'
         uses: ilammy/msvc-dev-cmd@v1
       {%- endif %}
 
       - name: Install package
         run: python -m pip install .[test]
@@ -97,15 +96,15 @@
       - name: Build sdist and wheel
         run: pipx run build
 
       - uses: actions/upload-artifact@v3
         with:
           path: dist
 
-      {%- if cookiecutter.backend != "trampolim" %}
+      {%- if cookiecutter.project_type != "trampolim" %}
 
       - name: Check products
         run: pipx run twine check dist/*
 
       {%- endif %}
 
   publish:
@@ -125,13 +124,13 @@
 
       - uses: pypa/gh-action-pypi-publish@release/v1
         if: github.event_name == 'release' && github.event.action == 'published'
         with:
           # Remember to tell (test-)pypi about this repo before publishing
           # Remove this line to publish to PyPI
           repository-url: https://test.pypi.org/legacy/
-          {%- if cookiecutter.backend == "trampolim" %}
+          {%- if cookiecutter.project_type == "trampolim" %}
           # Check not supported currently by twine + trampolim
           verify-metadata: false
           {%- endif %}
 
   {%- endif %}
```

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type == 'compiled' %}wheels.yml{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/wheels-pybind11,skbuild,mesonpy,maturin.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/main-pybind11,skbuild,mesonpy.cpp`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/lib-maturin.rs`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.29/.gitignore` & `sp_repo_review-2023.6.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
 # setuptools_scm
-src/*/_version.py
+src/*/version.py
 
 # Jeykll stuff
 .jekyll-cache/
 .jekyll-metadata
 _site/
 
 # NodeJS stuff, just in case (developer tooling)
```

### Comparing `sp_repo_review-2023.6.29/pyproject.toml` & `sp_repo_review-2023.6.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
-requires = ["hatchling", "hatch-vcs", "hatch-fancy-pypi-readme"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "sp_repo_review"
 authors = [
   { name = "Henry Schreiner", email = "henryfs@princeton.edu" },
 ]
 description = "Review repos for compliance to the Scientific-Python development guidelines"
+readme = "README-rr.md"
 requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Environment :: WebAssembly :: Emscripten",
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
@@ -24,98 +25,88 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python",
   "Topic :: Scientific/Engineering",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Software Development :: Quality Assurance",
   "Typing :: Typed",
 ]
-dynamic = ["version", "readme"]
+dynamic = ["version"]
 dependencies = [
   "pyyaml",
-  "repo-review>=0.7,<0.9",
+  "repo-review>=0.7.0b4,<0.8",
 ]
 
 [project.optional-dependencies]
 cli = [
   "repo-review[cli]",
 ]
 test = [
   "pytest >=7",
 ]
 dev = [
   "pytest >=7",
 ]
 
 [project.urls]
-Guide = "https://learn.scientific-python.org/development"
-Homepage = "https://scientific-python.github.io/cookie"
+Homepage = "https://github.com/scientific-python/cookie"
+Webpage = "https://scientific-python.github.io/cookie"
 Preview = "https://scientific-python-cookie.readthedocs.io"
-Source = "https://github.com/scientific-python/cookie"
 
 
 [project.entry-points."pipx.run"]
 sp-repo-review = "repo_review.__main__:main"
 
 [project.entry-points."repo_review.checks"]
 general = "sp_repo_review.checks.general:repo_review_checks"
 pyproject = "sp_repo_review.checks.pyproject:repo_review_checks"
 precommit = "sp_repo_review.checks.precommit:repo_review_checks"
 ruff = "sp_repo_review.checks.ruff:repo_review_checks"
 mypy = "sp_repo_review.checks.mypy:repo_review_checks"
 github = "sp_repo_review.checks.github:repo_review_checks"
-readthedocs = "sp_repo_review.checks.readthedocs:repo_review_checks"
 
 [project.entry-points."repo_review.fixtures"]
 workflows = "sp_repo_review.checks.github:workflows"
 dependabot = "sp_repo_review.checks.github:dependabot"
 precommit = "sp_repo_review.checks.precommit:precommit"
-readthedocs = "sp_repo_review.checks.readthedocs:readthedocs"
 
 [project.entry-points."repo_review.families"]
 scikit-hep = "sp_repo_review.families:get_familes"
 
-
 [tool.hatch]
 version.source = "vcs"
 build.hooks.vcs.version-file = "src/sp_repo_review/_version.py"
 
-[tool.hatch.metadata.hooks.fancy-pypi-readme]
-content-type = "text/markdown"
-
-[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
-path = "README.md"
-start-after = "<!-- sp-repo-review -->"
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = ["-ra", "--strict-markers", "--strict-config"]
 xfail_strict = true
 log_cli_level = "INFO"
 filterwarnings = [
   'error',
+  'ignore:(ast.Str|Attribute s|ast.NameConstant|ast.Num) is deprecated:DeprecationWarning:_pytest',
 ]
 norecursedirs = ['{{cookiecutter.project_name}}']
 testpaths = ["tests"]
 
 
 [tool.mypy]
-files = ["src", "tests"]
+files = ["src", "web", "tests"]
 python_version = "3.10"
 warn_unused_configs = true
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 disallow_untyped_defs = false
 
 [[tool.mypy.overrides]]
 module = "sp_repo_review.*"
 disallow_untyped_defs = true
 
-
 [tool.pylint]
 master.py-version = "3.10"
 master.ignore-paths= ["src/sp_repo_review/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
   "design",
@@ -176,10 +167,7 @@
 "typing.Sequence".msg = "Use collections.abc.Sequence instead."
 "typing.Set".msg = "Use collections.abc.Set instead."
 "importlib.abc".msg = "Use sp_repo_review._compat.importlib.resources.abc instead."
 "importlib.resources.abc".msg = "Use sp_repo_review._compat.importlib.resources.abc instead."
 
 [tool.ruff.per-file-ignores]
 "src/sp_repo_review/_compat/**.py" = ["TID251"]
-
-[tool.repo-review]
-ignore = ["RTD103"]
```

