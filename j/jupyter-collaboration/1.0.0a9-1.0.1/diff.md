# Comparing `tmp/jupyter_collaboration-1.0.0a9.tar.gz` & `tmp/jupyter_collaboration-1.0.1.tar.gz`

## Comparing `jupyter_collaboration-1.0.0a9.tar` & `jupyter_collaboration-1.0.1.tar`

### file list

```diff
@@ -1,108 +1,109 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.eslintrc.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.flake8
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.gitconfig
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.licenserc.yaml
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.npmignore
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.prettierrc
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.readthedocs.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.stylelintrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.yarnrc.yml
--rw-r--r--   0        0        0    42584 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/CHANGELOG.md
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/CONTRIBUTING.md
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/RELEASE.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/codecov.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/install.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/lerna.json
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/package.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/setup.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/tsconfig.json
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/tsconfig.test.json
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/typedoc.json
--rw-r--r--   0        0        0   488215 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/yarn.lock
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/Makefile
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/make.bat
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/conf.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/configuration.md
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/index.md
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/_static/jupyter_logo.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/_static/logo-icon.png
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/developer/architecture.md
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/developer/contributing.rst
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/developer/javascript_api.rst
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/developer/python_api.rst
--rw-r--r--   0        0        0    61242 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/docs/source/images/rtc_shared_cursors.png
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter-config/jupyter_collaboration.json
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/_version.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/app.py
--rw-r--r--   0        0        0    12505 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/handlers.py
--rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/loaders.py
--rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/rooms.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/stores.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/utils.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/websocketserver.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/events/session.yaml
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/package.json
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/shared-link.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/413.cf154c48ecaa08648e56.js
--rw-r--r--   0        0        0    11162 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/493.efdf15c07c2318ee4cd7.js
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/760.c3c71c52d5e0ace455c5.js
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/8.883cdb5327aeb22e2587.js
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/839.14d748171b9c87a422f9.js
--rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/87.c69c6c0210f40538f288.js
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/933.737bcc7ac7d9a6826f35.js
--rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/remoteEntry.f78dd7195bd101ba931a.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/style.js
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/scripts/bump_version.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/tests/__init__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/tests/conftest.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/tests/test_loaders.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/README.md
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/tsconfig.json
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/collaboratorspanel.tsx
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/components.tsx
--rw-r--r--   0        0        0    11792 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/cursors.ts
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/index.ts
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/menu.ts
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/sharedlink.ts
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/tokens.ts
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/src/userinfopanel.tsx
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/style/base.css
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/style/index.js
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/style/menu.css
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration/style/sidepanel.css
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/README.md
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/tsconfig.json
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/schema/shared-link.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/schema/user-menu-bar.json
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/collaboration.ts
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/filebrowser.ts
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/index.ts
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/sharedlink.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/collaboration-extension/style/index.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/babel.config.js
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/jest.config.js
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/package.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/tsconfig.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/tsconfig.test.json
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/index.ts
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/requests.ts
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/tokens.ts
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/ydrive.ts
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/yprovider.ts
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/packages/docprovider/src/__tests__/yprovider.spec.ts
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/LICENSE
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/README.md
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/pyproject.toml
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a9/PKG-INFO
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.eslintrc.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.flake8
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.gitconfig
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.licenserc.yaml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.npmignore
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.prettierrc
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.stylelintrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.yarnrc.yml
+-rw-r--r--   0        0        0    45733 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/RELEASE.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/codecov.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/install.json
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/lerna.json
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/package.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/setup.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/tsconfig.json
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/tsconfig.test.json
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/typedoc.json
+-rw-r--r--   0        0        0   488218 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/yarn.lock
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/configuration.md
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/index.md
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/_static/jupyter_logo.svg
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/_static/logo-icon.png
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/developer/architecture.md
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/developer/contributing.rst
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/developer/javascript_api.rst
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/developer/python_api.rst
+-rw-r--r--   0        0        0    61242 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/images/rtc_shared_cursors.png
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter-config/jupyter_collaboration.json
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/_version.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/app.py
+-rw-r--r--   0        0        0    13760 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/handlers.py
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/loaders.py
+-rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/rooms.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/stores.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/utils.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/websocketserver.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/events/session.yaml
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/package.json
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/shared-link.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/252.856eca7b3cd3748103bd.js
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/299.40530f9f1ff8893867f0.js
+-rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/413.c23fa684c321e1bc178c.js
+-rw-r--r--   0        0        0    11293 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/760.44dd9522edcf2585c0a2.js
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/839.14d748171b9c87a422f9.js
+-rw-r--r--   0        0        0    10890 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/87.a9066e8e77b73733ee8e.js
+-rw-r--r--   0        0        0     7951 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/899.d8ce2a60114cd6e1ebea.js
+-rw-r--r--   0        0        0     9528 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/remoteEntry.63a4bd8fd0be235c05a7.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/style.js
+-rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/scripts/bump_version.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/tests/test_loaders.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/README.md
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/tsconfig.json
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/collaboratorspanel.tsx
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/components.tsx
+-rw-r--r--   0        0        0    11792 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/cursors.ts
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/index.ts
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/menu.ts
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/sharedlink.ts
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/tokens.ts
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/userinfopanel.tsx
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/style/base.css
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/style/index.js
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/style/menu.css
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/style/sidepanel.css
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/README.md
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/tsconfig.json
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/schema/shared-link.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/schema/user-menu-bar.json
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/src/collaboration.ts
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/src/filebrowser.ts
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/src/index.ts
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/src/sharedlink.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/style/index.css
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/style/index.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/babel.config.js
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/jest.config.js
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/package.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/tsconfig.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/tsconfig.test.json
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/awareness.ts
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/index.ts
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/requests.ts
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/tokens.ts
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/ydrive.ts
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/yprovider.ts
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/__tests__/yprovider.spec.ts
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/README.md
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/PKG-INFO
```

### Comparing `jupyter_collaboration-1.0.0a9/.eslintrc.js` & `jupyter_collaboration-1.0.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/.licenserc.yaml` & `jupyter_collaboration-1.0.1/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/.pre-commit-config.yaml` & `jupyter_collaboration-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/CHANGELOG.md` & `jupyter_collaboration-1.0.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,55 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.0.1
+
+([Full Changelog](https://github.com/jupyterlab/jupyter-collaboration/compare/@jupyter/collaboration-extension@1.0.0...e97855f7ad4160cc4e6f5dbe9361806d6b9f3c31))
+
+### Enhancements made
+
+- Support ypy-websocket v0.12 [#168](https://github.com/jupyterlab/jupyter-collaboration/pull/168) ([@davidbrochart](https://github.com/davidbrochart))
+- Chat subprotocol [#167](https://github.com/jupyterlab/jupyter-collaboration/pull/167) ([@hbcarlos](https://github.com/hbcarlos))
+
+### Maintenance and upkeep improvements
+
+- Support ypy-websocket v0.12 [#168](https://github.com/jupyterlab/jupyter-collaboration/pull/168) ([@davidbrochart](https://github.com/davidbrochart))
+- Fix npm tag for publication of final version [#158](https://github.com/jupyterlab/jupyter-collaboration/pull/158) ([@fcollonval](https://github.com/fcollonval))
+
+### Documentation improvements
+
+- Remove link share mention [#169](https://github.com/jupyterlab/jupyter-collaboration/pull/169) ([@fcollonval](https://github.com/fcollonval))
+- Fix install instructions to use correct name [#166](https://github.com/jupyterlab/jupyter-collaboration/pull/166) ([@fperez](https://github.com/fperez))
+- Fix package name in README [#159](https://github.com/jupyterlab/jupyter-collaboration/pull/159) ([@fcollonval](https://github.com/fcollonval))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab/jupyter-collaboration/graphs/contributors?from=2023-06-02&to=2023-06-29&type=c))
+
+[@codecov-commenter](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Acodecov-commenter+updated%3A2023-06-02..2023-06-29&type=Issues) | [@davidbrochart](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Adavidbrochart+updated%3A2023-06-02..2023-06-29&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Afcollonval+updated%3A2023-06-02..2023-06-29&type=Issues) | [@fperez](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Afperez+updated%3A2023-06-02..2023-06-29&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Agithub-actions+updated%3A2023-06-02..2023-06-29&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Ahbcarlos+updated%3A2023-06-02..2023-06-29&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
+## 1.0.0
+
+([Full Changelog](https://github.com/jupyterlab/jupyter_collaboration/compare/@jupyter/collaboration-extension@1.0.0-alpha.9...4da43013daa89869035d77417971a80143b0ac61))
+
+### Maintenance and upkeep improvements
+
+- Remove spurious `'` [#156](https://github.com/jupyterlab/jupyter_collaboration/pull/156) ([@krassowski](https://github.com/krassowski))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab/jupyter_collaboration/graphs/contributors?from=2023-05-30&to=2023-06-02&type=c))
+
+[@krassowski](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Akrassowski+updated%3A2023-05-30..2023-06-02&type=Issues)
+
 ## 1.0.0alpha9
 
 ([Full Changelog](https://github.com/jupyterlab/jupyter_collaboration/compare/@jupyter/collaboration-extension@1.0.0-alpha.8...fbae4ff5054bf98507ac87429e0322c22be6b830))
 
 ### Enhancements made
 
 - Add share link feature [#150](https://github.com/jupyterlab/jupyter_collaboration/pull/150) ([@fcollonval](https://github.com/fcollonval))
@@ -33,16 +75,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab/jupyter_collaboration/graphs/contributors?from=2023-04-24&to=2023-05-30&type=c))
 
 [@codecov-commenter](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Acodecov-commenter+updated%3A2023-04-24..2023-05-30&type=Issues) | [@davidbrochart](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Adavidbrochart+updated%3A2023-04-24..2023-05-30&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Afcollonval+updated%3A2023-04-24..2023-05-30&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Agithub-actions+updated%3A2023-04-24..2023-05-30&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Ahbcarlos+updated%3A2023-04-24..2023-05-30&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Akrassowski+updated%3A2023-04-24..2023-05-30&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Awelcome+updated%3A2023-04-24..2023-05-30&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.0.0alpha8
 
 ([Full Changelog](https://github.com/jupyterlab/jupyter_collaboration/compare/@jupyter/collaboration-extension@1.0.0-alpha.7...2e5a6cc66961a5552e8a89c0850c7483c1e1acb2))
 
 ### Enhancements made
 
 - Follow up #133 [#136](https://github.com/jupyterlab/jupyter_collaboration/pull/136) ([@hbcarlos](https://github.com/hbcarlos))
```

### Comparing `jupyter_collaboration-1.0.0a9/package.json` & `jupyter_collaboration-1.0.1/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'1.0.1'"}*

```diff
@@ -59,14 +59,14 @@
         "stylelint:check": "stylelint --cache \"packages/**/style/**/*.css\"",
         "test": "lerna run test",
         "test:cov": "lerna run test:cov",
         "test:debug": "lerna run test:debug",
         "test:debug:watch": "lerna run test:debug:watch",
         "watch": "lerna run watch"
     },
-    "version": "1.0.0-alpha.9",
+    "version": "1.0.1",
     "workspaces": {
         "packages": [
             "packages/*"
         ]
     }
 }
```

### Comparing `jupyter_collaboration-1.0.0a9/typedoc.json` & `jupyter_collaboration-1.0.1/typedoc.json`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/yarn.lock` & `jupyter_collaboration-1.0.1/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -2015,16 +2015,16 @@
   languageName: node
   linkType: hard
 
 "@jupyter/collaboration-extension@workspace:packages/collaboration-extension":
   version: 0.0.0-use.local
   resolution: "@jupyter/collaboration-extension@workspace:packages/collaboration-extension"
   dependencies:
-    "@jupyter/collaboration": ^1.0.0-alpha.9
-    "@jupyter/docprovider": ^1.0.0-alpha.9
+    "@jupyter/collaboration": ^1.0.1
+    "@jupyter/docprovider": ^1.0.1
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/apputils": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/codemirror": ^4.0.0
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/docregistry": ^4.0.0
     "@jupyterlab/filebrowser": ^4.0.0
@@ -2044,20 +2044,21 @@
     typescript: ~5.0.4
     y-protocols: ^1.0.5
     y-websocket: ^1.3.15
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
-"@jupyter/collaboration@^1.0.0-alpha.9, @jupyter/collaboration@workspace:packages/collaboration":
+"@jupyter/collaboration@^1.0.1, @jupyter/collaboration@workspace:packages/collaboration":
   version: 0.0.0-use.local
   resolution: "@jupyter/collaboration@workspace:packages/collaboration"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.7.0
+    "@jupyter/docprovider": ^1.0.1
     "@jupyterlab/apputils": ^4.0.0
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/services": ^7.0.0
     "@jupyterlab/ui-components": ^4.0.0
     "@lumino/coreutils": ^2.1.0
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.0
@@ -2066,15 +2067,15 @@
     rimraf: ^4.1.2
     typescript: ~5.0.4
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
-"@jupyter/docprovider@^1.0.0-alpha.9, @jupyter/docprovider@workspace:packages/docprovider":
+"@jupyter/docprovider@^1.0.1, @jupyter/docprovider@workspace:packages/docprovider":
   version: 0.0.0-use.local
   resolution: "@jupyter/docprovider@workspace:packages/docprovider"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/services": ^7.0.0
     "@jupyterlab/testing": ^4.0.0
```

### Comparing `jupyter_collaboration-1.0.0a9/docs/Makefile` & `jupyter_collaboration-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/docs/make.bat` & `jupyter_collaboration-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/docs/source/conf.py` & `jupyter_collaboration-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/docs/source/configuration.md` & `jupyter_collaboration-1.0.1/docs/source/configuration.md`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/docs/source/index.md` & `jupyter_collaboration-1.0.1/docs/source/index.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,28 +12,23 @@
 editing using the [Yjs shared editing framework](https://github.com/yjs/yjs).
 Editors are not collaborative by default; to activate it, install the extension
 `jupyter_collaboration`.
 
 Installation using mamba/conda:
 
 ```sh
-mamba install -c conda-forge jupyter_collaboration
+mamba install -c conda-forge jupyter-collaboration
 ```
 
 Installation using pip:
 
 ```sh
-pip install jupyter_collaboration
+pip install jupyter-collaboration
 ```
 
-To share a document with other users, you can copy the URL and send it, or you
-can install a helpful extension called
-[jupyterlab-link-share](https://github.com/jupyterlab-contrib/jupyterlab-link-share)
-that might help to share the link including the token.
-
 The new collaborative editing feature enables collaboration in real-time
 between multiple clients without user roles. When sharing the URL of a
 document to other users, they will have access to the same environment you
 are working on (they can e.g. write and execute the cells of a notebook).
 
 Moreover, you can see the cursors from other users with an anonymous
 username, a username that will disappear in a few seconds to make room
```

### Comparing `jupyter_collaboration-1.0.0a9/docs/source/_static/jupyter_logo.svg` & `jupyter_collaboration-1.0.1/docs/source/_static/jupyter_logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/docs/source/_static/logo-icon.png` & `jupyter_collaboration-1.0.1/docs/source/_static/logo-icon.png`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/docs/source/developer/contributing.rst` & `jupyter_collaboration-1.0.1/docs/source/developer/contributing.rst`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/docs/source/images/rtc_shared_cursors.png` & `jupyter_collaboration-1.0.1/docs/source/images/rtc_shared_cursors.png`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/app.py` & `jupyter_collaboration-1.0.1/jupyter_collaboration/app.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/handlers.py` & `jupyter_collaboration-1.0.1/jupyter_collaboration/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,24 @@
 from jupyter_server.auth import authorized
 from jupyter_server.base.handlers import APIHandler, JupyterHandler
 from jupyter_ydoc import ydocs as YDOCS
 from tornado import web
 from tornado.websocket import WebSocketHandler
 from ypy_websocket.websocket_server import YRoom
 from ypy_websocket.ystore import BaseYStore
-from ypy_websocket.yutils import YMessageType
+from ypy_websocket.yutils import YMessageType, write_var_uint
 
 from .loaders import FileLoaderMapping
 from .rooms import DocumentRoom, TransientRoom
-from .utils import JUPYTER_COLLABORATION_EVENTS_URI, LogLevel, decode_file_path
+from .utils import (
+    JUPYTER_COLLABORATION_EVENTS_URI,
+    LogLevel,
+    MessageType,
+    decode_file_path,
+)
 from .websocketserver import JupyterWebsocketServer
 
 YFILE = YDOCS["file"]
 
 SERVER_SESSION = str(uuid.uuid4())
 
 
@@ -45,36 +50,31 @@
        ``_message_queue``, from which we get them asynchronously.
     - The ``send(message)`` method is async and calls Tornado's ``write_message(message)``.
     - Although it's currently not used in ypy-websocket, ``recv()`` is an async method for
        receiving a message.
     """
 
     _message_queue: asyncio.Queue[Any]
+    _background_tasks: set[asyncio.Task]
 
-    def initialize(
-        self,
-        ywebsocket_server: JupyterWebsocketServer,
-        file_loaders: FileLoaderMapping,
-        ystore_class: type[BaseYStore],
-        document_cleanup_delay: float | None = 60.0,
-        document_save_delay: float | None = 1.0,
-    ) -> None:
-        # File ID manager cannot be passed as argument as the extension may load after this one
-        self._file_id_manager = self.settings["file_id_manager"]
-        self._file_loaders = file_loaders
-        self._cleanup_delay = document_cleanup_delay
-        self._websocket_server = ywebsocket_server
-
-        self._message_queue = asyncio.Queue()
+    def create_task(self, aw):
+        task = asyncio.create_task(aw)
+        self._background_tasks.add(task)
+        task.add_done_callback(self._background_tasks.discard)
+
+    async def prepare(self):
+        if not self._websocket_server.started.is_set():
+            self.create_task(self._websocket_server.start())
+            await self._websocket_server.started.wait()
 
         # Get room
         self._room_id: str = self.request.path.split("/")[-1]
 
         if self._websocket_server.room_exists(self._room_id):
-            self.room: YRoom = self._websocket_server.get_room(self._room_id)
+            self.room: YRoom = await self._websocket_server.get_room(self._room_id)
 
         else:
             if self._room_id.count(":") >= 2:
                 # DocumentRoom
                 file_format, file_type, file_id = decode_file_path(self._room_id)
                 if file_id in self._file_loaders:
                     self._emit(
@@ -83,33 +83,54 @@
                         "There is another collaborative session accessing the same file.\nThe synchronization between rooms is not supported and you might lose some of your changes.",
                     )
 
                 file = self._file_loaders[file_id]
                 path = self._file_id_manager.get_path(file_id)
                 path = Path(path)
                 updates_file_path = str(path.parent / f".{file_type}:{path.name}.y")
-                ystore = ystore_class(path=updates_file_path, log=self.log)
+                ystore = self._ystore_class(path=updates_file_path, log=self.log)
                 self.room = DocumentRoom(
                     self._room_id,
                     file_format,
                     file_type,
                     file,
                     self.event_logger,
                     ystore,
                     self.log,
-                    document_save_delay,
+                    self._document_save_delay,
                 )
 
             else:
                 # TransientRoom
                 # it is a transient document (e.g. awareness)
                 self.room = TransientRoom(self._room_id, self.log)
 
+            await self._websocket_server.start_room(self.room)
             self._websocket_server.add_room(self._room_id, self.room)
 
+        return await super().prepare()
+
+    def initialize(
+        self,
+        ywebsocket_server: JupyterWebsocketServer,
+        file_loaders: FileLoaderMapping,
+        ystore_class: type[BaseYStore],
+        document_cleanup_delay: float | None = 60.0,
+        document_save_delay: float | None = 1.0,
+    ) -> None:
+        self._background_tasks = set()
+        # File ID manager cannot be passed as argument as the extension may load after this one
+        self._file_id_manager = self.settings["file_id_manager"]
+        self._file_loaders = file_loaders
+        self._ystore_class = ystore_class
+        self._cleanup_delay = document_cleanup_delay
+        self._document_save_delay = document_save_delay
+        self._websocket_server = ywebsocket_server
+        self._message_queue = asyncio.Queue()
+
     @property
     def path(self):
         """
         Returns the room id. It needs to be called 'path' for compatibility with
         the WebsocketServer (websocket.path).
         """
         return self._room_id
@@ -141,17 +162,15 @@
             raise web.HTTPError(403)
         return await super().get(*args, **kwargs)
 
     async def open(self, room_id):
         """
         On connection open.
         """
-        task = asyncio.create_task(self._websocket_server.serve(self))
-        self._websocket_server.background_tasks.add(task)
-        task.add_done_callback(self._websocket_server.background_tasks.discard)
+        self.create_task(self._websocket_server.serve(self))
 
         if isinstance(self.room, DocumentRoom):
             # Close the connection if the document session expired
             session_id = self.get_query_argument("sessionId", "")
             if SERVER_SESSION != session_id:
                 self.close(
                     1003,
@@ -193,14 +212,16 @@
         return message
 
     def on_message(self, message):
         """
         On message receive.
         """
         message_type = message[0]
+        print("message type:", message_type)
+
         if message_type == YMessageType.AWARENESS:
             # awareness
             skip = False
             changes = self.room.awareness.get_changes(message[1:])
             added_users = changes["added"]
             removed_users = changes["removed"]
             for i, user in enumerate(added_users):
@@ -218,14 +239,26 @@
             if skip:
                 self.log.debug(
                     "Filtered out Y message of type: %s",
                     YMessageType(message_type).name,
                 )
                 return skip
 
+        if message_type == MessageType.CHAT:
+            msg = message[2:].decode("utf-8")
+            user = self.get_current_user()
+            data = json.dumps({"username": user.username, "msg": msg}).encode("utf8")
+            for client in self.room.clients:
+                if client != self:
+                    task = asyncio.create_task(
+                        client.send(bytes([MessageType.CHAT]) + write_var_uint(len(data)) + data)
+                    )
+                    self._websocket_server.background_tasks.add(task)
+                    task.add_done_callback(self._websocket_server.background_tasks.discard)
+
         self._message_queue.put_nowait(message)
         self._websocket_server.ypatch_nb += 1
 
     def on_close(self) -> None:
         """
         On connection close.
         """
```

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/loaders.py` & `jupyter_collaboration-1.0.1/jupyter_collaboration/loaders.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/rooms.py` & `jupyter_collaboration-1.0.1/jupyter_collaboration/rooms.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/stores.py` & `jupyter_collaboration-1.0.1/jupyter_collaboration/stores.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/utils.py` & `jupyter_collaboration-1.0.1/jupyter_collaboration/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 import pathlib
-from enum import Enum
+from enum import Enum, IntEnum
 from typing import Tuple
 
 JUPYTER_COLLABORATION_EVENTS_URI = "https://schema.jupyter.org/jupyter_collaboration/session/v1"
 EVENTS_SCHEMA_PATH = pathlib.Path(__file__).parent / "events" / "session.yaml"
 
 
+class MessageType(IntEnum):
+    SYNC = 0
+    AWARENESS = 1
+    CHAT = 125
+
+
 class LogLevel(Enum):
     INFO = "INFO"
     DEBUG = "DEBUG"
     WARNING = "WARNING"
     ERROR = "ERROR"
     CRITICAL = "CRITICAL"
```

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/websocketserver.py` & `jupyter_collaboration-1.0.1/jupyter_collaboration/websocketserver.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,29 +54,19 @@
         # if room_tasks:
         #     _, pending = await asyncio.wait(room_tasks, timeout=3)
         #     if pending:
         #         msg = f"{len(pending)} room task(s) are pending."
         #         self.log.warning(msg)
         #         self.log.debug("Pending tasks: %r", pending)
 
+        self.stop()
         tasks = []
-        for name, room in list(self.rooms.items()):
-            try:
-                self.delete_room(name=name)
-            except Exception as e:  # Capture exception as room may be auto clean
-                msg = f"Failed to delete room {name}"
-                self.log.debug(msg, exc_info=e)
-            else:
-                tasks.append(room._broadcast_task)  # FIXME should be upstreamed
         if self.monitor_task is not None:
             self.monitor_task.cancel()
             tasks.append(self.monitor_task)
-        for task in self.background_tasks:
-            task.cancel()  # FIXME should be upstreamed
-            tasks.append(task)
 
         if tasks:
             _, pending = await asyncio.wait(tasks, timeout=3)
             if pending:
                 msg = f"{len(pending)} task(s) are pending."
                 self.log.warning(msg)
                 self.log.debug("Pending tasks: %r", pending)
@@ -99,15 +89,15 @@
 
             Parameters:
                 path (str): Room ID.
                 room (YRoom): A room.
         """
         self.rooms[path] = room
 
-    def get_room(self, path: str) -> YRoom:
+    async def get_room(self, path: str) -> YRoom:
         """
         Returns the room for the specified room ID or raises a RoomNotFound
         error if the room doesn't exist.
 
             Parameters:
                 path (str): Room ID.
 
@@ -117,15 +107,17 @@
             Raises
                 RoomNotFound
         """
         if path not in self.rooms:
             # Document rooms need a file
             raise RoomNotFound
 
-        return self.rooms[path]
+        room = self.rooms[path]
+        await self.start_room(room)
+        return room
 
     async def serve(self, websocket: WebSocketHandler) -> None:
         # start monitoring here as the event loop is not yet available when initializing the object
         if self.monitor_task is None:
             self.monitor_task = asyncio.create_task(self._monitor())
 
         await super().serve(websocket)
```

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/events/session.yaml` & `jupyter_collaboration-1.0.1/jupyter_collaboration/events/session.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/package.json` & `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9758748196248196%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.0.1', '@jupyter/docprovider': '^1.0.1'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.63a4bd8fd0be235c05a7.js'}}",*

 * * "'version'": "'1.0.1'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.0-alpha.9",
-        "@jupyter/docprovider": "^1.0.0-alpha.9",
+        "@jupyter/collaboration": "^1.0.1",
+        "@jupyter/docprovider": "^1.0.1",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/codemirror": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/fileeditor": "^4.0.0",
@@ -45,15 +45,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter_collaboration",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f78dd7195bd101ba931a.js",
+            "load": "static/remoteEntry.63a4bd8fd0be235c05a7.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/filebrowser-extension:defaultFileBrowser"
         ],
         "extension": true,
         "outputDir": "../../jupyter_collaboration/labextension",
@@ -129,9 +129,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.9"
+    "version": "1.0.1"
 }
```

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig` & `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.0.1', '@jupyter/docprovider': '^1.0.1'}",*

 * * "'version'": "'1.0.1'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.0-alpha.9",
-        "@jupyter/docprovider": "^1.0.0-alpha.9",
+        "@jupyter/collaboration": "^1.0.1",
+        "@jupyter/docprovider": "^1.0.1",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/codemirror": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/fileeditor": "^4.0.0",
@@ -124,9 +124,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.9"
+    "version": "1.0.1"
 }
```

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/760.c3c71c52d5e0ace455c5.js` & `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/760.44dd9522edcf2585c0a2.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -15,16 +15,16 @@
                 showSharedLinkDialog: () => L
             });
             var r = n(7930);
             const s = new r.Token("@jupyter/collaboration:IUserMenu"),
                 o = new r.Token("@jupyter/collaboration:IGlobalAwareness");
             var a = n(6029),
                 i = n(8778),
-                l = n(9324),
-                c = n(9474);
+                l = n(5350),
+                c = n(9993);
             const d = "jp-Collaborator";
             class u extends i.Panel {
                 constructor(e, t, n) {
                     super({}), this._onAwarenessChanged = () => {
                         const e = this._awareness.getStates(),
                             t = [];
                         e.forEach(((e, n) => {
@@ -248,15 +248,15 @@
                         parent: document.body
                     })]
                 });
 
             function x(e) {
                 return [f.of(e), C]
             }
-            var j = n(3897),
+            var j = n(2189),
                 A = n(4059);
             class I extends i.MenuBar.Renderer {
                 constructor(e) {
                     super(), this._user = e
                 }
                 renderItem(e) {
                     const t = this.createItemClass(e),
@@ -292,15 +292,15 @@
                 }
             }
             class P extends i.Menu {
                 constructor(e) {
                     super(e)
                 }
             }
-            var E = n(7387);
+            var E = n(926);
             async function L({
                 translator: e
             }) {
                 const t = (null != e ? e : E.nullTranslator).load("collaboration"),
                     n = c.PageConfig.getToken(),
                     r = new URL(c.URLExt.normalize(c.PageConfig.getUrl({
                         workspace: c.PageConfig.defaultWorkspace
```

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/8.883cdb5327aeb22e2587.js` & `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/252.856eca7b3cd3748103bd.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,150 +1,187 @@
 "use strict";
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
-    [8, 933], {
-        2008: (e, t, s) => {
-            s.r(t), s.d(t, {
-                ICollaborativeDrive: () => _,
-                WebSocketProvider: () => h,
-                YDrive: () => d
+    [252, 299], {
+        4299: (e, s, t) => {
+            t.r(s), t.d(s, {
+                ICollaborativeDrive: () => v,
+                MessageType: () => o,
+                WebSocketAwarenessProvider: () => c,
+                WebSocketProvider: () => p,
+                YDrive: () => y
             });
-            var o = s(9474),
-                r = s(3020),
-                n = s(9324),
-                i = s(7930),
-                a = s(4901),
-                c = s(7099);
-            class h {
+            var o, r = t(4901),
+                n = t(2256),
+                i = t(9476),
+                a = t(7099);
+            ! function(e) {
+                e[e.CHAT = 125] = "CHAT"
+            }(o || (o = {}));
+            class c extends a.WebsocketProvider {
+                constructor(e) {
+                    super(e.url, e.roomID, e.awareness.doc, {
+                        awareness: e.awareness
+                    }), this._isDisposed = !1, this._awareness = e.awareness;
+                    const s = e.user;
+                    s.ready.then((() => this._onUserChanged(s))).catch((e => console.error(e))), s.userChanged.connect(this._onUserChanged, this), this._chatMessage = new r.Signal(this), this.messageHandlers[o.CHAT] = (e, s, t, o, r) => {
+                        const i = n.kf(s),
+                            a = JSON.parse(i);
+                        console.debug("Chat:", a), this._chatMessage.emit(a)
+                    }
+                }
+                get isDisposed() {
+                    return this._isDisposed
+                }
+                get chatMessage() {
+                    return this._chatMessage
+                }
+                dispose() {
+                    this._isDisposed || (this.destroy(), this._isDisposed = !0)
+                }
+                sendMessage(e) {
+                    console.debug("Send message:", e);
+                    const s = i.Mf();
+                    i.uE(s, o.CHAT), i.uw(s, e), this.ws.send(i._f(s))
+                }
+                _onUserChanged(e) {
+                    this._awareness.setLocalStateField("user", e.identity)
+                }
+            }
+            var h = t(9993),
+                d = t(4238),
+                l = t(5350),
+                _ = t(7930);
+            class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
-                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, n.showErrorMessage)(this._trans.__("Document session error"), e.reason, [n.Dialog.okButton()]), this._sharedModel.dispose())
+                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, l.showErrorMessage)(this._trans.__("Document session error"), e.reason, [l.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
-                        var t;
-                        e && (this._ready.resolve(), null === (t = this._yWebsocketProvider) || void 0 === t || t.off("sync", this._onSync))
-                    }, this._ready = new i.PromiseDelegate, this._isDisposed = !1, this._path = e.path, this._contentType = e.contentType, this._format = e.format, this._serverUrl = e.url, this._sharedModel = e.model, this._awareness = e.model.awareness, this._yWebsocketProvider = null, this._trans = e.translator;
-                    const t = e.user;
-                    t.ready.then((() => {
-                        this._onUserChanged(t)
-                    })).catch((e => console.error(e))), t.userChanged.connect(this._onUserChanged, this), this._connect().catch((e => console.warn(e)))
+                        var s;
+                        e && (this._ready.resolve(), null === (s = this._yWebsocketProvider) || void 0 === s || s.off("sync", this._onSync))
+                    }, this._ready = new _.PromiseDelegate, this._isDisposed = !1, this._path = e.path, this._contentType = e.contentType, this._format = e.format, this._serverUrl = e.url, this._sharedModel = e.model, this._awareness = e.model.awareness, this._yWebsocketProvider = null, this._trans = e.translator;
+                    const s = e.user;
+                    s.ready.then((() => {
+                        this._onUserChanged(s)
+                    })).catch((e => console.error(e))), s.userChanged.connect(this._onUserChanged, this), this._connect().catch((e => console.warn(e)))
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 get ready() {
                     return this._ready.promise
                 }
                 dispose() {
-                    var e, t, s;
-                    this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (t = this._yWebsocketProvider) || void 0 === t || t.off("sync", this._onSync), null === (s = this._yWebsocketProvider) || void 0 === s || s.destroy(), a.Signal.clearData(this))
+                    var e, s, t;
+                    this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (s = this._yWebsocketProvider) || void 0 === s || s.off("sync", this._onSync), null === (t = this._yWebsocketProvider) || void 0 === t || t.destroy(), r.Signal.clearData(this))
                 }
                 async _connect() {
-                    const e = await async function(e, t, s) {
-                        const n = r.ServerConnection.makeSettings(),
-                            i = o.URLExt.join(n.baseUrl, "api/collaboration/session", encodeURIComponent(s)),
-                            a = {
+                    const e = await async function(e, s, t) {
+                        const o = d.ServerConnection.makeSettings(),
+                            r = h.URLExt.join(o.baseUrl, "api/collaboration/session", encodeURIComponent(t)),
+                            n = {
                                 method: "PUT",
                                 body: JSON.stringify({
                                     format: e,
-                                    type: t
+                                    type: s
                                 })
                             };
-                        let c;
+                        let i;
                         try {
-                            c = await r.ServerConnection.makeRequest(i, a, n)
+                            i = await d.ServerConnection.makeRequest(r, n, o)
                         } catch (e) {
-                            throw new r.ServerConnection.NetworkError(e)
+                            throw new d.ServerConnection.NetworkError(e)
                         }
-                        let h = await c.text();
-                        if (h.length > 0) try {
-                            h = JSON.parse(h)
+                        let a = await i.text();
+                        if (a.length > 0) try {
+                            a = JSON.parse(a)
                         } catch (e) {
-                            console.log("Not a JSON response body.", c)
+                            console.log("Not a JSON response body.", i)
                         }
-                        if (!c.ok) throw new r.ServerConnection.ResponseError(c, h.message || h);
-                        return h
+                        if (!i.ok) throw new d.ServerConnection.ResponseError(i, a.message || a);
+                        return a
                     }(this._format, this._contentType, this._path);
-                    this._yWebsocketProvider = new c.WebsocketProvider(this._serverUrl, `${e.format}:${e.type}:${e.fileId}`, this._sharedModel.ydoc, {
+                    this._yWebsocketProvider = new a.WebsocketProvider(this._serverUrl, `${e.format}:${e.type}:${e.fileId}`, this._sharedModel.ydoc, {
                         disableBc: !0,
                         params: {
                             sessionId: e.sessionId
                         },
                         awareness: this._awareness
                     }), this._yWebsocketProvider.on("sync", this._onSync), this._yWebsocketProvider.on("connection-close", this._onConnectionClosed)
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            class d extends r.Drive {
-                constructor(e, t) {
+            class y extends d.Drive {
+                constructor(e, s) {
                     super({
                         name: "RTC"
-                    }), this._onCreate = (e, t) => {
+                    }), this._onCreate = (e, s) => {
                         if ("string" == typeof e.format) try {
-                            const s = new h({
-                                    url: o.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
+                            const t = new p({
+                                    url: h.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
                                     path: e.path,
                                     format: e.format,
                                     contentType: e.contentType,
-                                    model: t,
+                                    model: s,
                                     user: this._user,
                                     translator: this._trans
                                 }),
-                                r = `${e.format}:${e.contentType}:${e.path}`;
-                            this._providers.set(r, s), t.disposed.connect((() => {
-                                const e = this._providers.get(r);
-                                e && (e.dispose(), this._providers.delete(r))
+                                o = `${e.format}:${e.contentType}:${e.path}`;
+                            this._providers.set(o, t), s.disposed.connect((() => {
+                                const e = this._providers.get(o);
+                                e && (e.dispose(), this._providers.delete(o))
                             }))
-                        } catch (t) {
-                            console.error(`Failed to open websocket connection for ${e.path}.\n:${t}`)
+                        } catch (s) {
+                            console.error(`Failed to open websocket connection for ${e.path}.\n:${s}`)
                         }
-                    }, this._user = e, this._trans = t, this._providers = new Map, this.sharedModelFactory = new l(this._onCreate)
+                    }, this._user = e, this._trans = s, this._providers = new Map, this.sharedModelFactory = new u(this._onCreate)
                 }
                 dispose() {
                     this.isDisposed || (this._providers.forEach((e => e.dispose())), this._providers.clear(), super.dispose())
                 }
-                async get(e, t) {
-                    if (t && t.format && t.type) {
-                        const s = `${t.format}:${t.type}:${e}`,
-                            o = this._providers.get(s);
+                async get(e, s) {
+                    if (s && s.format && s.type) {
+                        const t = `${s.format}:${s.type}:${e}`,
+                            o = this._providers.get(t);
                         if (o) {
-                            const s = super.get(e, {
-                                ...t,
+                            const t = super.get(e, {
+                                ...s,
                                 content: !1
                             });
-                            return await o.ready, s
+                            return await o.ready, t
                         }
                     }
-                    return super.get(e, t)
+                    return super.get(e, s)
                 }
-                async save(e, t = {}) {
-                    if (t.format && t.type) {
-                        const s = `${t.format}:${t.type}:${e}`;
-                        if (this._providers.get(s)) return this.get(e, {
-                            ...t,
+                async save(e, s = {}) {
+                    if (s.format && s.type) {
+                        const t = `${s.format}:${s.type}:${e}`;
+                        if (this._providers.get(t)) return this.get(e, {
+                            ...s,
                             content: !1
                         })
                     }
-                    return super.save(e, t)
+                    return super.save(e, s)
                 }
             }
-            class l {
+            class u {
                 constructor(e) {
                     this._onCreate = e, this.collaborative = !0, this._documentFactories = new Map
                 }
-                registerDocumentFactory(e, t) {
+                registerDocumentFactory(e, s) {
                     if (this._documentFactories.has(e)) throw new Error(`The content type ${e} already exists`);
-                    this._documentFactories.set(e, t)
+                    this._documentFactories.set(e, s)
                 }
                 createNew(e) {
                     if ("string" == typeof e.format) {
                         if (e.collaborative && this._documentFactories.has(e.contentType)) {
-                            const t = this._documentFactories.get(e.contentType)(e);
-                            return this._onCreate(e, t), t
+                            const s = this._documentFactories.get(e.contentType)(e);
+                            return this._onCreate(e, s), s
                         }
                     } else console.warn(`Only defined format are supported; got ${e.format}.`)
                 }
             }
-            const _ = new i.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
+            const v = new _.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
         }
     }
 ]);
```

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/839.14d748171b9c87a422f9.js` & `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/839.14d748171b9c87a422f9.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/87.c69c6c0210f40538f288.js` & `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/87.a9066e8e77b73733ee8e.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,288 +1,465 @@
 "use strict";
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
     [87], {
-        5087: (e, o, t) => {
-            t.r(o), t.d(o, {
-                default: () => B
+        2019: (e, t, o) => {
+            o.d(t, {
+                y: () => n
             });
-            var r, a = t(2177),
-                n = t(9324),
-                s = t(5355),
-                i = t(2497),
-                l = t(5116),
-                c = t(899),
-                d = t(94),
-                u = t(7387),
-                p = t(2293),
-                v = t(1039);
+            var a = o(3205),
+                s = o(6834);
+            const r = Array.from;
+            Array.isArray;
+            class n {
+                constructor() {
+                    this._observers = a.Ue()
+                }
+                on(e, t) {
+                    a.Yu(this._observers, e, s.Ue).add(t)
+                }
+                once(e, t) {
+                    const o = (...a) => {
+                        this.off(e, o), t(...a)
+                    };
+                    this.on(e, o)
+                }
+                off(e, t) {
+                    const o = this._observers.get(e);
+                    void 0 !== o && (o.delete(t), 0 === o.size && this._observers.delete(e))
+                }
+                emit(e, t) {
+                    return r((this._observers.get(e) || a.Ue()).values()).forEach((e => e(...t)))
+                }
+                destroy() {
+                    this._observers = a.Ue()
+                }
+            }
+        },
+        6834: (e, t, o) => {
+            o.d(t, {
+                Ue: () => a
+            });
+            const a = () => new Set
+        },
+        870: (e, t, o) => {
+            o.d(t, {
+                ZG: () => a
+            });
+            const a = Date.now
+        },
+        6493: (e, t, o) => {
+            o.d(t, {
+                Ag: () => d,
+                GL: () => c,
+                oy: () => h,
+                xq: () => u
+            });
+            var a = o(9476),
+                s = o(2256),
+                r = o(870),
+                n = o(1332),
+                i = o(2019),
+                l = o(1872);
+            o(981);
+            class c extends i.y {
+                constructor(e) {
+                    super(), this.doc = e, this.clientID = e.clientID, this.states = new Map, this.meta = new Map, this._checkInterval = setInterval((() => {
+                        const e = r.ZG();
+                        null !== this.getLocalState() && 15e3 <= e - this.meta.get(this.clientID).lastUpdated && this.setLocalState(this.getLocalState());
+                        const t = [];
+                        this.meta.forEach(((o, a) => {
+                            a !== this.clientID && 3e4 <= e - o.lastUpdated && this.states.has(a) && t.push(a)
+                        })), t.length > 0 && d(this, t, "timeout")
+                    }), n.GW(3e3)), e.on("destroy", (() => {
+                        this.destroy()
+                    })), this.setLocalState({})
+                }
+                destroy() {
+                    this.emit("destroy", [this]), this.setLocalState(null), super.destroy(), clearInterval(this._checkInterval)
+                }
+                getLocalState() {
+                    return this.states.get(this.clientID) || null
+                }
+                setLocalState(e) {
+                    const t = this.clientID,
+                        o = this.meta.get(t),
+                        a = void 0 === o ? 0 : o.clock + 1,
+                        s = this.states.get(t);
+                    null === e ? this.states.delete(t) : this.states.set(t, e), this.meta.set(t, {
+                        clock: a,
+                        lastUpdated: r.ZG()
+                    });
+                    const n = [],
+                        i = [],
+                        c = [],
+                        d = [];
+                    null === e ? d.push(t) : null == s ? null != e && n.push(t) : (i.push(t), l.Hi(s, e) || c.push(t)), (n.length > 0 || c.length > 0 || d.length > 0) && this.emit("change", [{
+                        added: n,
+                        updated: c,
+                        removed: d
+                    }, "local"]), this.emit("update", [{
+                        added: n,
+                        updated: i,
+                        removed: d
+                    }, "local"])
+                }
+                setLocalStateField(e, t) {
+                    const o = this.getLocalState();
+                    null !== o && this.setLocalState({
+                        ...o,
+                        [e]: t
+                    })
+                }
+                getStates() {
+                    return this.states
+                }
+            }
+            const d = (e, t, o) => {
+                    const a = [];
+                    for (let o = 0; o < t.length; o++) {
+                        const s = t[o];
+                        if (e.states.has(s)) {
+                            if (e.states.delete(s), s === e.clientID) {
+                                const t = e.meta.get(s);
+                                e.meta.set(s, {
+                                    clock: t.clock + 1,
+                                    lastUpdated: r.ZG()
+                                })
+                            }
+                            a.push(s)
+                        }
+                    }
+                    a.length > 0 && (e.emit("change", [{
+                        added: [],
+                        updated: [],
+                        removed: a
+                    }, o]), e.emit("update", [{
+                        added: [],
+                        updated: [],
+                        removed: a
+                    }, o]))
+                },
+                u = (e, t, o = e.states) => {
+                    const s = t.length,
+                        r = a.Mf();
+                    a.uE(r, s);
+                    for (let n = 0; n < s; n++) {
+                        const s = t[n],
+                            i = o.get(s) || null,
+                            l = e.meta.get(s).clock;
+                        a.uE(r, s), a.uE(r, l), a.uw(r, JSON.stringify(i))
+                    }
+                    return a._f(r)
+                },
+                h = (e, t, o) => {
+                    const a = s.l1(t),
+                        n = r.ZG(),
+                        i = [],
+                        c = [],
+                        d = [],
+                        u = [],
+                        h = s.yg(a);
+                    for (let t = 0; t < h; t++) {
+                        const t = s.yg(a);
+                        let o = s.yg(a);
+                        const r = JSON.parse(s.kf(a)),
+                            h = e.meta.get(t),
+                            p = e.states.get(t),
+                            g = void 0 === h ? 0 : h.clock;
+                        (g < o || g === o && null === r && e.states.has(t)) && (null === r ? t === e.clientID && null != e.getLocalState() ? o++ : e.states.delete(t) : e.states.set(t, r), e.meta.set(t, {
+                            clock: o,
+                            lastUpdated: n
+                        }), void 0 === h && null !== r ? i.push(t) : void 0 !== h && null === r ? u.push(t) : null !== r && (l.Hi(r, p) || d.push(t), c.push(t)))
+                    }(i.length > 0 || d.length > 0 || u.length > 0) && e.emit("change", [{
+                        added: i,
+                        updated: d,
+                        removed: u
+                    }, o]), (i.length > 0 || c.length > 0 || u.length > 0) && e.emit("update", [{
+                        added: i,
+                        updated: c,
+                        removed: u
+                    }, o])
+                }
+        },
+        5087: (e, t, o) => {
+            o.r(t), o.d(t, {
+                default: () => E
+            });
+            var a, s = o(4163),
+                r = o(5350),
+                n = o(2164),
+                i = o(8486),
+                l = o(9350),
+                c = o(1919),
+                d = o(56),
+                u = o(926),
+                h = o(2293),
+                p = o(4822);
             ! function(e) {
                 e.openPath = "filebrowser:open-path"
-            }(r || (r = {}));
-            const m = {
+            }(a || (a = {}));
+            const g = {
                     id: "@jupyter/collaboration-extension:drive",
                     description: "The default collaborative drive provider",
-                    provides: v.ICollaborativeDrive,
+                    provides: p.ICollaborativeDrive,
                     requires: [u.ITranslator],
                     optional: [],
-                    activate: (e, o) => {
-                        const t = o.load("jupyter_collaboration"),
-                            r = new v.YDrive(e.serviceManager.user, t);
-                        return e.serviceManager.contents.addDrive(r), r
+                    activate: (e, t) => {
+                        const o = t.load("jupyter_collaboration"),
+                            a = new p.YDrive(e.serviceManager.user, o);
+                        return e.serviceManager.contents.addDrive(a), a
                     }
                 },
-                g = {
+                v = {
                     id: "@jupyter/collaboration-extension:yfile",
                     description: "Plugin to register the shared model factory for the content type 'file'",
                     autoStart: !0,
-                    requires: [v.ICollaborativeDrive],
+                    requires: [p.ICollaborativeDrive],
                     optional: [],
-                    activate: (e, o) => {
-                        o.sharedModelFactory.registerDocumentFactory("file", (() => new p.YFile))
+                    activate: (e, t) => {
+                        t.sharedModelFactory.registerDocumentFactory("file", (() => new h.YFile))
                     }
                 },
-                y = {
+                m = {
                     id: "@jupyter/collaboration-extension:ynotebook",
                     description: "Plugin to register the shared model factory for the content type 'notebook'",
                     autoStart: !0,
-                    requires: [v.ICollaborativeDrive],
+                    requires: [p.ICollaborativeDrive],
                     optional: [d.ISettingRegistry],
-                    activate: (e, o, t) => {
-                        let r = !0;
-                        t && t.load("@jupyterlab/notebook-extension:tracker").then((e => {
-                            const o = e => {
-                                var o;
-                                const t = null == e ? void 0 : e.get("experimentalEnableDocumentWideUndoRedo").composite;
-                                r = null === (o = !t) || void 0 === o || o
+                    activate: (e, t, o) => {
+                        let a = !0;
+                        o && o.load("@jupyterlab/notebook-extension:tracker").then((e => {
+                            const t = e => {
+                                var t;
+                                const o = null == e ? void 0 : e.get("experimentalEnableDocumentWideUndoRedo").composite;
+                                a = null === (t = !o) || void 0 === t || t
                             };
-                            o(e), e.changed.connect((e => o(e)))
-                        })), o.sharedModelFactory.registerDocumentFactory("notebook", (() => new p.YNotebook({
-                            disableDocumentWideUndoRedo: r
+                            t(e), e.changed.connect((e => t(e)))
+                        })), t.sharedModelFactory.registerDocumentFactory("notebook", (() => new h.YNotebook({
+                            disableDocumentWideUndoRedo: a
                         })))
                     }
                 },
-                b = {
+                y = {
                     id: "@jupyter/collaboration-extension:defaultFileBrowser",
                     description: "The default file browser factory provider",
-                    provides: s.IDefaultFileBrowser,
-                    requires: [v.ICollaborativeDrive, s.IFileBrowserFactory],
-                    optional: [a.IRouter, a.JupyterFrontEnd.ITreeResolver, a.ILabShell, d.ISettingRegistry],
-                    activate: async (e, o, t, r, a, n) => {
+                    provides: n.IDefaultFileBrowser,
+                    requires: [p.ICollaborativeDrive, n.IFileBrowserFactory],
+                    optional: [s.IRouter, s.JupyterFrontEnd.ITreeResolver, s.ILabShell, d.ISettingRegistry],
+                    activate: async (e, t, o, a, s, r) => {
                         const {
-                            commands: s
+                            commands: n
                         } = e;
-                        e.serviceManager.contents.addDrive(o);
-                        const i = t.createFileBrowser("filebrowser", {
+                        e.serviceManager.contents.addDrive(t);
+                        const i = o.createFileBrowser("filebrowser", {
                             auto: !1,
                             restore: !1,
-                            driveName: o.name
+                            driveName: t.name
                         });
-                        return w.restoreBrowser(i, s, r, a, n), i
+                        return w.restoreBrowser(i, n, a, s, r), i
                     }
                 },
-                h = {
+                b = {
                     id: "@jupyter/collaboration-extension:logger",
                     description: "A logging plugin for debugging purposes.",
                     autoStart: !0,
                     optional: [l.ILoggerRegistry, i.IEditorTracker, c.INotebookTracker, u.ITranslator],
-                    activate: (e, o, t, r, a) => {
-                        const s = (null != a ? a : u.nullTranslator).load("jupyter_collaboration"),
+                    activate: (e, t, o, a, s) => {
+                        const n = (null != s ? s : u.nullTranslator).load("jupyter_collaboration"),
                             i = "https://schema.jupyter.org/jupyter_collaboration/session/v1";
-                        if (!o) return void e.serviceManager.events.stream.connect(((e, o) => {
-                            var t, r;
-                            o.schema_id === i && (console.debug(`[${o.room}(${o.path})] ${null!==(t=o.action)&&void 0!==t?t:""}: ${null!==(r=o.msg)&&void 0!==r?r:""}`), "WARNING" === o.level && (0, n.showDialog)({
-                                title: s.__("Warning"),
-                                body: s.__(`Two collaborative sessions are accessing the file ${o.path} simultaneously.\n                \nOpening the same file using different views simultaneously is not supported. Please, close one view; otherwise, you might lose some of your progress.`),
-                                buttons: [n.Dialog.okButton()]
+                        if (!t) return void e.serviceManager.events.stream.connect(((e, t) => {
+                            var o, a;
+                            t.schema_id === i && (console.debug(`[${t.room}(${t.path})] ${null!==(o=t.action)&&void 0!==o?o:""}: ${null!==(a=t.msg)&&void 0!==a?a:""}`), "WARNING" === t.level && (0, r.showDialog)({
+                                title: n.__("Warning"),
+                                body: n.__(`Two collaborative sessions are accessing the file ${t.path} simultaneously.\n                \nOpening the same file using different views simultaneously is not supported. Please, close one view; otherwise, you might lose some of your progress.`),
+                                buttons: [r.Dialog.okButton()]
                             }))
                         }));
                         const l = new Map,
-                            c = (e, t) => {
-                                const r = o.getLogger(t.context.path);
-                                l.set(t.context.localPath, r), t.disposed.connect((e => {
+                            c = (e, o) => {
+                                const a = t.getLogger(o.context.path);
+                                l.set(o.context.localPath, a), o.disposed.connect((e => {
                                     l.delete(e.context.localPath)
                                 }))
                             };
-                        t && t.widgetAdded.connect(c), r && r.widgetAdded.connect(c), (async () => {
-                            var o, t;
+                        o && o.widgetAdded.connect(c), a && a.widgetAdded.connect(c), (async () => {
+                            var t, o;
                             const {
-                                events: r
+                                events: a
                             } = e.serviceManager;
-                            for await (const e of r.stream) if (e.schema_id === i) {
-                                const r = l.get(e.path);
-                                null == r || r.log({
+                            for await (const e of a.stream) if (e.schema_id === i) {
+                                const a = l.get(e.path);
+                                null == a || a.log({
                                     type: "text",
                                     level: e.level.toLowerCase(),
-                                    data: `[${e.room}] ${null!==(o=e.action)&&void 0!==o?o:""}: ${null!==(t=e.msg)&&void 0!==t?t:""}`
-                                }), "WARNING" === e.level && (0, n.showDialog)({
-                                    title: s.__("Warning"),
-                                    body: s.__("Two collaborative sessions are accessing the file %1 simultaneously.\n                \n'Opening a document with multiple views simultaneously is not supported. Please close one view; otherwise, you might lose some of your progress.", e.path),
-                                    buttons: [n.Dialog.warnButton({
-                                        label: s.__("Ok")
+                                    data: `[${e.room}] ${null!==(t=e.action)&&void 0!==t?t:""}: ${null!==(o=e.msg)&&void 0!==o?o:""}`
+                                }), "WARNING" === e.level && (0, r.showDialog)({
+                                    title: n.__("Warning"),
+                                    body: n.__("Two collaborative sessions are accessing the file %1 simultaneously.\n                \nOpening a document with multiple views simultaneously is not supported. Please close one view; otherwise, you might lose some of your progress.", e.path),
+                                    buttons: [r.Dialog.warnButton({
+                                        label: n.__("Ok")
                                     })]
                                 })
                             }
                         })()
                     }
                 };
             var w;
             ! function(e) {
-                e.restoreBrowser = async function(e, o, t, a, n) {
-                    const s = "jp-mod-restoring";
-                    if (e.addClass(s), !t) return await e.model.restore(e.id), await e.model.refresh(), void e.removeClass(s);
+                e.restoreBrowser = async function(e, t, o, s, r) {
+                    const n = "jp-mod-restoring";
+                    if (e.addClass(n), !o) return await e.model.restore(e.id), await e.model.refresh(), void e.removeClass(n);
                     const i = async () => {
-                        t.routed.disconnect(i);
-                        const l = await (null == a ? void 0 : a.paths);
-                        (null == l ? void 0 : l.file) || (null == l ? void 0 : l.browser) ? (await e.model.restore(e.id, !1), l.file && await o.execute(r.openPath, {
+                        o.routed.disconnect(i);
+                        const l = await (null == s ? void 0 : s.paths);
+                        (null == l ? void 0 : l.file) || (null == l ? void 0 : l.browser) ? (await e.model.restore(e.id, !1), l.file && await t.execute(a.openPath, {
                             path: l.file,
                             dontShowBrowser: !0
-                        }), l.browser && await o.execute(r.openPath, {
+                        }), l.browser && await t.execute(a.openPath, {
                             path: l.browser,
                             dontShowBrowser: !0
-                        })) : (await e.model.restore(e.id), await e.model.refresh()), e.removeClass(s), (null == n ? void 0 : n.isEmpty("main")) && o.execute("launcher:create")
+                        })) : (await e.model.restore(e.id), await e.model.refresh()), e.removeClass(n), (null == r ? void 0 : r.isEmpty("main")) && t.execute("launcher:create")
                     };
-                    t.routed.connect(i)
+                    o.routed.connect(i)
                 }
             }(w || (w = {}));
-            var f = t(674),
-                I = t(6903),
-                _ = t(3897),
-                x = t(8778),
-                j = t(9474),
-                k = t(3020),
-                C = t(1802),
-                S = t(981),
-                M = t(6493),
-                D = t(7099);
-            const P = {
+            var f = o(2927),
+                I = o(1255),
+                _ = o(2189),
+                S = o(8778),
+                k = o(9993),
+                x = o(4238),
+                D = o(1617),
+                M = o(981),
+                j = o(6493);
+            const U = {
                     id: "@jupyter/collaboration-extension:userMenu",
                     description: "Provide connected user menu.",
                     requires: [],
                     provides: I.IUserMenu,
                     activate: e => {
                         const {
-                            commands: o
+                            commands: t
                         } = e, {
-                            user: t
+                            user: o
                         } = e.serviceManager;
                         return new I.UserMenu({
-                            commands: o,
-                            user: t
+                            commands: t,
+                            user: o
                         })
                     }
                 },
-                T = {
+                C = {
                     id: "@jupyter/collaboration-extension:user-menu-bar",
                     description: "Add user menu to the interface.",
                     autoStart: !0,
-                    requires: [I.IUserMenu, n.IToolbarWidgetRegistry],
-                    activate: async (e, o, t) => {
+                    requires: [I.IUserMenu, r.IToolbarWidgetRegistry],
+                    activate: async (e, t, o) => {
                         const {
-                            user: r
-                        } = e.serviceManager, a = new x.MenuBar({
+                            user: a
+                        } = e.serviceManager, s = new S.MenuBar({
                             forceItemsPosition: {
                                 forceX: !1,
                                 forceY: !1
                             },
-                            renderer: new I.RendererUserMenu(r)
+                            renderer: new I.RendererUserMenu(a)
                         });
-                        a.id = "jp-UserMenu", r.userChanged.connect((() => a.update())), a.addMenu(o), t.addFactory("TopBar", "user-menu", (() => a))
+                        s.id = "jp-UserMenu", a.userChanged.connect((() => s.update())), s.addMenu(t), o.addFactory("TopBar", "user-menu", (() => s))
                     }
                 },
-                R = {
+                L = {
                     id: "@jupyter/collaboration-extension:rtcGlobalAwareness",
                     description: "Add global awareness to share working document of users.",
-                    requires: [C.IStateDB],
+                    requires: [D.IStateDB],
                     provides: I.IGlobalAwareness,
-                    activate: (e, o) => {
+                    activate: (e, t) => {
                         const {
-                            user: t
-                        } = e.serviceManager, r = new S.Doc, a = new M.GL(r), n = k.ServerConnection.makeSettings(), s = j.URLExt.join(n.wsUrl, "api/collaboration/room");
-                        new D.WebsocketProvider(s, "JupyterLab:globalAwareness", r, {
-                            awareness: a
-                        });
-                        const i = () => {
-                            a.setLocalStateField("user", t.identity)
-                        };
-                        return t.isReady && i(), t.ready.then(i).catch((e => console.error(e))), t.userChanged.connect(i), o.changed.connect((async () => {
-                            var e, t;
-                            const r = (null === (t = null === (e = (await o.toJSON())["layout-restorer:data"]) || void 0 === e ? void 0 : e.main) || void 0 === t ? void 0 : t.current) || "";
-                            r.startsWith("editor") || r.startsWith("notebook") ? a.setLocalStateField("current", r) : a.setLocalStateField("current", null)
-                        })), a
+                            user: o
+                        } = e.serviceManager, a = new M.Doc, s = new j.GL(a), r = x.ServerConnection.makeSettings(), n = k.URLExt.join(r.wsUrl, "api/collaboration/room");
+                        return new p.WebSocketAwarenessProvider({
+                            url: n,
+                            roomID: "JupyterLab:globalAwareness",
+                            awareness: s,
+                            user: o
+                        }), t.changed.connect((async () => {
+                            var e, o;
+                            const a = (null === (o = null === (e = (await t.toJSON())["layout-restorer:data"]) || void 0 === e ? void 0 : e.main) || void 0 === o ? void 0 : o.current) || "";
+                            a.startsWith("editor") || a.startsWith("notebook") ? s.setLocalStateField("current", a) : s.setLocalStateField("current", null)
+                        })), s
                     }
                 },
-                F = {
+                A = {
                     id: "@jupyter/collaboration-extension:rtcPanel",
                     description: "Add side panel to display all currently connected users.",
                     autoStart: !0,
                     requires: [I.IGlobalAwareness],
                     optional: [u.ITranslator],
-                    activate: (e, o, t) => {
+                    activate: (e, t, o) => {
                         const {
-                            user: r
-                        } = e.serviceManager, a = (null != t ? t : u.nullTranslator).load("jupyter_collaboration"), s = new _.SidePanel({
+                            user: a
+                        } = e.serviceManager, s = (null != o ? o : u.nullTranslator).load("jupyter_collaboration"), n = new _.SidePanel({
                             alignment: "justify"
                         });
-                        s.id = n.DOMUtils.createDomID(), s.title.icon = _.usersIcon, s.title.caption = a.__("Collaboration"), s.addClass("jp-RTCPanel"), e.shell.add(s, "left", {
+                        n.id = r.DOMUtils.createDomID(), n.title.icon = _.usersIcon, n.title.caption = s.__("Collaboration"), n.addClass("jp-RTCPanel"), e.shell.add(n, "left", {
                             rank: 300
                         });
-                        const i = new I.UserInfoPanel(r);
-                        i.title.label = a.__("User info"), i.title.caption = a.__("User information"), s.addWidget(i);
-                        const l = new I.CollaboratorsPanel(r, o, (o => {
+                        const i = new I.UserInfoPanel(a);
+                        i.title.label = s.__("User info"), i.title.caption = s.__("User information"), n.addWidget(i);
+                        const l = new I.CollaboratorsPanel(a, t, (t => {
                             e.commands.execute("docmanager:open", {
-                                path: o
+                                path: t
                             })
                         }));
-                        l.title.label = a.__("Online Collaborators"), s.addWidget(l)
+                        l.title.label = s.__("Online Collaborators"), n.addWidget(l)
                     }
                 },
-                U = {
+                P = {
                     id: "@jupyter/collaboration-extension:userEditorCursors",
                     description: "Add CodeMirror extension to display remote user cursors and selections.",
                     autoStart: !0,
                     requires: [f.IEditorExtensionRegistry],
-                    activate: (e, o) => {
-                        o.addExtension({
+                    activate: (e, t) => {
+                        t.addExtension({
                             name: "remote-user-cursors",
                             factory(e) {
                                 const {
-                                    awareness: o,
-                                    ysource: t
+                                    awareness: t,
+                                    ysource: o
                                 } = e.model.sharedModel;
                                 return f.EditorExtensionRegistry.createImmutableExtension((0, I.remoteUserCursors)({
-                                    awareness: o,
-                                    ytext: t
+                                    awareness: t,
+                                    ytext: o
                                 }))
                             }
                         })
                     }
                 };
-            var A;
+            var T;
             ! function(e) {
                 e.share = "collaboration:shared-link"
-            }(A || (A = {}));
-            const B = [m, g, y, b, h, P, T, R, F, {
+            }(T || (T = {}));
+            const E = [g, v, m, y, b, U, C, L, A, {
                 id: "@jupyter/collaboration-extension:shared-link",
                 autoStart: !0,
-                optional: [n.ICommandPalette, u.ITranslator],
-                activate: async (e, o, t) => {
+                optional: [r.ICommandPalette, u.ITranslator],
+                activate: async (e, t, o) => {
                     const {
-                        commands: r
-                    } = e, a = (null != t ? t : u.nullTranslator).load("collaboration");
-                    r.addCommand(A.share, {
-                        label: a.__("Generate a Shared Link"),
+                        commands: a
+                    } = e, s = (null != o ? o : u.nullTranslator).load("collaboration");
+                    a.addCommand(T.share, {
+                        label: s.__("Generate a Shared Link"),
                         icon: _.shareIcon,
                         execute: async () => {
                             const e = await (0, I.showSharedLinkDialog)({
-                                translator: t
+                                translator: o
                             });
-                            e.button.accept && e.value && n.Clipboard.copyToSystem(e.value)
+                            e.button.accept && e.value && r.Clipboard.copyToSystem(e.value)
                         }
-                    }), o && o.addItem({
-                        command: A.share,
-                        category: a.__("Server")
+                    }), t && t.addItem({
+                        command: T.share,
+                        category: s.__("Server")
                     })
                 }
-            }, U]
+            }, P]
         }
     }
 ]);
```

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/933.737bcc7ac7d9a6826f35.js` & `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/299.40530f9f1ff8893867f0.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,150 +1,187 @@
 "use strict";
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
-    [933, 8], {
-        2008: (e, t, s) => {
-            s.r(t), s.d(t, {
-                ICollaborativeDrive: () => _,
-                WebSocketProvider: () => h,
-                YDrive: () => d
+    [299, 252], {
+        4299: (e, s, t) => {
+            t.r(s), t.d(s, {
+                ICollaborativeDrive: () => v,
+                MessageType: () => o,
+                WebSocketAwarenessProvider: () => c,
+                WebSocketProvider: () => p,
+                YDrive: () => y
             });
-            var o = s(9474),
-                r = s(3020),
-                n = s(9324),
-                i = s(7930),
-                a = s(4901),
-                c = s(7099);
-            class h {
+            var o, r = t(4901),
+                n = t(2256),
+                i = t(9476),
+                a = t(7099);
+            ! function(e) {
+                e[e.CHAT = 125] = "CHAT"
+            }(o || (o = {}));
+            class c extends a.WebsocketProvider {
+                constructor(e) {
+                    super(e.url, e.roomID, e.awareness.doc, {
+                        awareness: e.awareness
+                    }), this._isDisposed = !1, this._awareness = e.awareness;
+                    const s = e.user;
+                    s.ready.then((() => this._onUserChanged(s))).catch((e => console.error(e))), s.userChanged.connect(this._onUserChanged, this), this._chatMessage = new r.Signal(this), this.messageHandlers[o.CHAT] = (e, s, t, o, r) => {
+                        const i = n.kf(s),
+                            a = JSON.parse(i);
+                        console.debug("Chat:", a), this._chatMessage.emit(a)
+                    }
+                }
+                get isDisposed() {
+                    return this._isDisposed
+                }
+                get chatMessage() {
+                    return this._chatMessage
+                }
+                dispose() {
+                    this._isDisposed || (this.destroy(), this._isDisposed = !0)
+                }
+                sendMessage(e) {
+                    console.debug("Send message:", e);
+                    const s = i.Mf();
+                    i.uE(s, o.CHAT), i.uw(s, e), this.ws.send(i._f(s))
+                }
+                _onUserChanged(e) {
+                    this._awareness.setLocalStateField("user", e.identity)
+                }
+            }
+            var h = t(9993),
+                d = t(4238),
+                l = t(5350),
+                _ = t(7930);
+            class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
-                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, n.showErrorMessage)(this._trans.__("Document session error"), e.reason, [n.Dialog.okButton()]), this._sharedModel.dispose())
+                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, l.showErrorMessage)(this._trans.__("Document session error"), e.reason, [l.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
-                        var t;
-                        e && (this._ready.resolve(), null === (t = this._yWebsocketProvider) || void 0 === t || t.off("sync", this._onSync))
-                    }, this._ready = new i.PromiseDelegate, this._isDisposed = !1, this._path = e.path, this._contentType = e.contentType, this._format = e.format, this._serverUrl = e.url, this._sharedModel = e.model, this._awareness = e.model.awareness, this._yWebsocketProvider = null, this._trans = e.translator;
-                    const t = e.user;
-                    t.ready.then((() => {
-                        this._onUserChanged(t)
-                    })).catch((e => console.error(e))), t.userChanged.connect(this._onUserChanged, this), this._connect().catch((e => console.warn(e)))
+                        var s;
+                        e && (this._ready.resolve(), null === (s = this._yWebsocketProvider) || void 0 === s || s.off("sync", this._onSync))
+                    }, this._ready = new _.PromiseDelegate, this._isDisposed = !1, this._path = e.path, this._contentType = e.contentType, this._format = e.format, this._serverUrl = e.url, this._sharedModel = e.model, this._awareness = e.model.awareness, this._yWebsocketProvider = null, this._trans = e.translator;
+                    const s = e.user;
+                    s.ready.then((() => {
+                        this._onUserChanged(s)
+                    })).catch((e => console.error(e))), s.userChanged.connect(this._onUserChanged, this), this._connect().catch((e => console.warn(e)))
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 get ready() {
                     return this._ready.promise
                 }
                 dispose() {
-                    var e, t, s;
-                    this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (t = this._yWebsocketProvider) || void 0 === t || t.off("sync", this._onSync), null === (s = this._yWebsocketProvider) || void 0 === s || s.destroy(), a.Signal.clearData(this))
+                    var e, s, t;
+                    this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (s = this._yWebsocketProvider) || void 0 === s || s.off("sync", this._onSync), null === (t = this._yWebsocketProvider) || void 0 === t || t.destroy(), r.Signal.clearData(this))
                 }
                 async _connect() {
-                    const e = await async function(e, t, s) {
-                        const n = r.ServerConnection.makeSettings(),
-                            i = o.URLExt.join(n.baseUrl, "api/collaboration/session", encodeURIComponent(s)),
-                            a = {
+                    const e = await async function(e, s, t) {
+                        const o = d.ServerConnection.makeSettings(),
+                            r = h.URLExt.join(o.baseUrl, "api/collaboration/session", encodeURIComponent(t)),
+                            n = {
                                 method: "PUT",
                                 body: JSON.stringify({
                                     format: e,
-                                    type: t
+                                    type: s
                                 })
                             };
-                        let c;
+                        let i;
                         try {
-                            c = await r.ServerConnection.makeRequest(i, a, n)
+                            i = await d.ServerConnection.makeRequest(r, n, o)
                         } catch (e) {
-                            throw new r.ServerConnection.NetworkError(e)
+                            throw new d.ServerConnection.NetworkError(e)
                         }
-                        let h = await c.text();
-                        if (h.length > 0) try {
-                            h = JSON.parse(h)
+                        let a = await i.text();
+                        if (a.length > 0) try {
+                            a = JSON.parse(a)
                         } catch (e) {
-                            console.log("Not a JSON response body.", c)
+                            console.log("Not a JSON response body.", i)
                         }
-                        if (!c.ok) throw new r.ServerConnection.ResponseError(c, h.message || h);
-                        return h
+                        if (!i.ok) throw new d.ServerConnection.ResponseError(i, a.message || a);
+                        return a
                     }(this._format, this._contentType, this._path);
-                    this._yWebsocketProvider = new c.WebsocketProvider(this._serverUrl, `${e.format}:${e.type}:${e.fileId}`, this._sharedModel.ydoc, {
+                    this._yWebsocketProvider = new a.WebsocketProvider(this._serverUrl, `${e.format}:${e.type}:${e.fileId}`, this._sharedModel.ydoc, {
                         disableBc: !0,
                         params: {
                             sessionId: e.sessionId
                         },
                         awareness: this._awareness
                     }), this._yWebsocketProvider.on("sync", this._onSync), this._yWebsocketProvider.on("connection-close", this._onConnectionClosed)
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            class d extends r.Drive {
-                constructor(e, t) {
+            class y extends d.Drive {
+                constructor(e, s) {
                     super({
                         name: "RTC"
-                    }), this._onCreate = (e, t) => {
+                    }), this._onCreate = (e, s) => {
                         if ("string" == typeof e.format) try {
-                            const s = new h({
-                                    url: o.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
+                            const t = new p({
+                                    url: h.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
                                     path: e.path,
                                     format: e.format,
                                     contentType: e.contentType,
-                                    model: t,
+                                    model: s,
                                     user: this._user,
                                     translator: this._trans
                                 }),
-                                r = `${e.format}:${e.contentType}:${e.path}`;
-                            this._providers.set(r, s), t.disposed.connect((() => {
-                                const e = this._providers.get(r);
-                                e && (e.dispose(), this._providers.delete(r))
+                                o = `${e.format}:${e.contentType}:${e.path}`;
+                            this._providers.set(o, t), s.disposed.connect((() => {
+                                const e = this._providers.get(o);
+                                e && (e.dispose(), this._providers.delete(o))
                             }))
-                        } catch (t) {
-                            console.error(`Failed to open websocket connection for ${e.path}.\n:${t}`)
+                        } catch (s) {
+                            console.error(`Failed to open websocket connection for ${e.path}.\n:${s}`)
                         }
-                    }, this._user = e, this._trans = t, this._providers = new Map, this.sharedModelFactory = new l(this._onCreate)
+                    }, this._user = e, this._trans = s, this._providers = new Map, this.sharedModelFactory = new u(this._onCreate)
                 }
                 dispose() {
                     this.isDisposed || (this._providers.forEach((e => e.dispose())), this._providers.clear(), super.dispose())
                 }
-                async get(e, t) {
-                    if (t && t.format && t.type) {
-                        const s = `${t.format}:${t.type}:${e}`,
-                            o = this._providers.get(s);
+                async get(e, s) {
+                    if (s && s.format && s.type) {
+                        const t = `${s.format}:${s.type}:${e}`,
+                            o = this._providers.get(t);
                         if (o) {
-                            const s = super.get(e, {
-                                ...t,
+                            const t = super.get(e, {
+                                ...s,
                                 content: !1
                             });
-                            return await o.ready, s
+                            return await o.ready, t
                         }
                     }
-                    return super.get(e, t)
+                    return super.get(e, s)
                 }
-                async save(e, t = {}) {
-                    if (t.format && t.type) {
-                        const s = `${t.format}:${t.type}:${e}`;
-                        if (this._providers.get(s)) return this.get(e, {
-                            ...t,
+                async save(e, s = {}) {
+                    if (s.format && s.type) {
+                        const t = `${s.format}:${s.type}:${e}`;
+                        if (this._providers.get(t)) return this.get(e, {
+                            ...s,
                             content: !1
                         })
                     }
-                    return super.save(e, t)
+                    return super.save(e, s)
                 }
             }
-            class l {
+            class u {
                 constructor(e) {
                     this._onCreate = e, this.collaborative = !0, this._documentFactories = new Map
                 }
-                registerDocumentFactory(e, t) {
+                registerDocumentFactory(e, s) {
                     if (this._documentFactories.has(e)) throw new Error(`The content type ${e} already exists`);
-                    this._documentFactories.set(e, t)
+                    this._documentFactories.set(e, s)
                 }
                 createNew(e) {
                     if ("string" == typeof e.format) {
                         if (e.collaborative && this._documentFactories.has(e.contentType)) {
-                            const t = this._documentFactories.get(e.contentType)(e);
-                            return this._onCreate(e, t), t
+                            const s = this._documentFactories.get(e.contentType)(e);
+                            return this._onCreate(e, s), s
                         }
                     } else console.warn(`Only defined format are supported; got ${e.format}.`)
                 }
             }
-            const _ = new i.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
+            const v = new _.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
         }
     }
 ]);
```

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/remoteEntry.f78dd7195bd101ba931a.js` & `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/remoteEntry.63a4bd8fd0be235c05a7.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, l, i, u, d, f, s, c, p, b, h, v, y, m, g, j = {
+    var e, r, t, a, o, n, i, l, u, f, d, c, s, p, b, h, v, y, m, g, j = {
             6746: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(493), t.e(619), t.e(981), t.e(296), t.e(744), t.e(87)]).then((() => () => t(5087))),
-                        "./extension": () => Promise.all([t.e(493), t.e(619), t.e(981), t.e(296), t.e(744), t.e(87)]).then((() => () => t(5087))),
+                        "./index": () => Promise.all([t.e(899), t.e(981), t.e(662), t.e(46), t.e(238), t.e(87)]).then((() => () => t(5087))),
+                        "./extension": () => Promise.all([t.e(899), t.e(981), t.e(662), t.e(46), t.e(238), t.e(87)]).then((() => () => t(5087))),
                         "./style": () => t.e(839).then((() => () => t(8839)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -43,71 +43,71 @@
         }), r
     }, P.d = (e, r) => {
         for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
-        8: "883cdb5327aeb22e2587",
-        87: "c69c6c0210f40538f288",
-        296: "66b569f73a5e447ea765",
-        413: "cf154c48ecaa08648e56",
-        493: "efdf15c07c2318ee4cd7",
-        619: "3ea832ff8016a41a4d10",
-        744: "8d88ecfc016bf00dba1c",
-        760: "c3c71c52d5e0ace455c5",
+        46: "208d560cd92dfb43b720",
+        87: "a9066e8e77b73733ee8e",
+        238: "86e88a3059c9a5a0803f",
+        252: "856eca7b3cd3748103bd",
+        299: "40530f9f1ff8893867f0",
+        314: "352e97cabfe87ffaafa9",
+        413: "c23fa684c321e1bc178c",
+        662: "a45c67772b045e9d4102",
+        760: "44dd9522edcf2585c0a2",
         839: "14d748171b9c87a422f9",
-        901: "a771e814402df392d806",
+        899: "d8ce2a60114cd6e1ebea",
         930: "50b2067c71cf2a3ca014",
-        933: "737bcc7ac7d9a6826f35",
         981: "9b18765371d0668dbc59"
     } [e] + ".js?v=" + {
-        8: "883cdb5327aeb22e2587",
-        87: "c69c6c0210f40538f288",
-        296: "66b569f73a5e447ea765",
-        413: "cf154c48ecaa08648e56",
-        493: "efdf15c07c2318ee4cd7",
-        619: "3ea832ff8016a41a4d10",
-        744: "8d88ecfc016bf00dba1c",
-        760: "c3c71c52d5e0ace455c5",
+        46: "208d560cd92dfb43b720",
+        87: "a9066e8e77b73733ee8e",
+        238: "86e88a3059c9a5a0803f",
+        252: "856eca7b3cd3748103bd",
+        299: "40530f9f1ff8893867f0",
+        314: "352e97cabfe87ffaafa9",
+        413: "c23fa684c321e1bc178c",
+        662: "a45c67772b045e9d4102",
+        760: "44dd9522edcf2585c0a2",
         839: "14d748171b9c87a422f9",
-        901: "a771e814402df392d806",
+        899: "d8ce2a60114cd6e1ebea",
         930: "50b2067c71cf2a3ca014",
-        933: "737bcc7ac7d9a6826f35",
         981: "9b18765371d0668dbc59"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter/collaboration-extension:", P.l = (t, a, o, n) => {
         if (e[t]) e[t].push(a);
         else {
-            var l, i;
+            var i, l;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
-                    var f = u[d];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        l = f;
+                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
+                    var d = u[f];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
-            l || (i = !0, (l = document.createElement("script")).charset = "utf-8", l.timeout = 120, P.nc && l.setAttribute("nonce", P.nc), l.setAttribute("data-webpack", r + o), l.src = t), e[t] = [a];
-            var s = (r, a) => {
-                    l.onerror = l.onload = null, clearTimeout(c);
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
+            var c = (r, a) => {
+                    i.onerror = i.onload = null, clearTimeout(s);
                     var o = e[t];
-                    if (delete e[t], l.parentNode && l.parentNode.removeChild(l), o && o.forEach((e => e(a))), r) return r(a)
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
-                c = setTimeout(s.bind(null, void 0, {
+                s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
-                    target: l
+                    target: i
                 }), 12e4);
-            l.onerror = s.bind(null, l.onerror), l.onload = s.bind(null, l.onload), i && document.head.appendChild(l)
+            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -118,26 +118,26 @@
         P.I = (t, a) => {
             a || (a = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(a.indexOf(o) >= 0)) {
                 if (a.push(o), e[t]) return e[t];
                 P.o(P.S, t) || (P.S[t] = {});
                 var n = P.S[t],
-                    l = "@jupyter/collaboration-extension",
-                    i = (e, r, t, a) => {
+                    i = "@jupyter/collaboration-extension",
+                    l = (e, r, t, a) => {
                         var o = n[e] = n[e] || {},
-                            i = o[r];
-                        (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (o[r] = {
+                            l = o[r];
+                        (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
-                            from: l,
+                            from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (i("@jupyter/collaboration-extension", "1.0.0-alpha.9", (() => Promise.all([P.e(493), P.e(619), P.e(981), P.e(296), P.e(744), P.e(87)]).then((() => () => P(5087))))), i("@jupyter/collaboration", "1.0.0-alpha.9", (() => Promise.all([P.e(930), P.e(619), P.e(981), P.e(760), P.e(296)]).then((() => () => P(4760))))), i("@jupyter/docprovider", "1.0.0-alpha.9", (() => Promise.all([P.e(930), P.e(619), P.e(744), P.e(901), P.e(8)]).then((() => () => P(2008))))), i("y-websocket", "1.5.0", (() => Promise.all([P.e(493), P.e(413), P.e(981)]).then((() => () => P(413)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyter/collaboration-extension", "1.0.1", (() => Promise.all([P.e(899), P.e(981), P.e(662), P.e(46), P.e(238), P.e(87)]).then((() => () => P(5087))))), l("@jupyter/collaboration", "1.0.1", (() => Promise.all([P.e(981), P.e(930), P.e(662), P.e(760), P.e(46)]).then((() => () => P(4760))))), l("@jupyter/docprovider", "1.0.1", (() => Promise.all([P.e(899), P.e(930), P.e(662), P.e(314), P.e(238), P.e(299)]).then((() => () => P(4299))))), l("y-websocket", "1.5.0", (() => Promise.all([P.e(899), P.e(413), P.e(981)]).then((() => () => P(413)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -155,128 +155,128 @@
     }, a = (e, r) => {
         e = t(e), r = t(r);
         for (var a = 0;;) {
             if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
             var o = e[a],
                 n = (typeof o)[0];
             if (a >= r.length) return "u" == n;
-            var l = r[a],
-                i = (typeof l)[0];
-            if (n != i) return "o" == n && "n" == i || "s" == i || "u" == n;
-            if ("o" != n && "u" != n && o != l) return o < l;
+            var i = r[a],
+                l = (typeof i)[0];
+            if (n != l) return "o" == n && "n" == l || "s" == l || "u" == n;
+            if ("o" != n && "u" != n && o != i) return o < i;
             a++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(i = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, i);
+            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(l = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
             return t
         }
-        var l = [];
+        var i = [];
         for (n = 1; n < e.length; n++) {
-            var i = e[n];
-            l.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? l.pop() + " " + l.pop() : o(i))
+            var l = e[n];
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
         }
         return u();
 
         function u() {
-            return l.pop().replace(/^\((.+)\)$/, "$1")
+            return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 o = a < 0;
             o && (a = -a - 1);
-            for (var l = 0, i = 1, u = !0;; i++, l++) {
-                var d, f, s = i < e.length ? (typeof e[i])[0] : "";
-                if (l >= r.length || "o" == (f = (typeof(d = r[l]))[0])) return !u || ("u" == s ? i > a && !o : "" == s != o);
-                if ("u" == f) {
-                    if (!u || "u" != s) return !1
+            for (var i = 0, l = 1, u = !0;; l++, i++) {
+                var f, d, c = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !u || ("u" == c ? l > a && !o : "" == c != o);
+                if ("u" == d) {
+                    if (!u || "u" != c) return !1
                 } else if (u)
-                    if (s == f)
-                        if (i <= a) {
-                            if (d != e[i]) return !1
+                    if (c == d)
+                        if (l <= a) {
+                            if (f != e[l]) return !1
                         } else {
-                            if (o ? d > e[i] : d < e[i]) return !1;
-                            d != e[i] && (u = !1)
+                            if (o ? f > e[l] : f < e[l]) return !1;
+                            f != e[l] && (u = !1)
                         }
-                else if ("s" != s && "n" != s) {
-                    if (o || i <= a) return !1;
-                    u = !1, i--
+                else if ("s" != c && "n" != c) {
+                    if (o || l <= a) return !1;
+                    u = !1, l--
                 } else {
-                    if (i <= a || f < s != o) return !1;
+                    if (l <= a || d < c != o) return !1;
                     u = !1
-                } else "s" != s && "n" != s && (u = !1, i--)
+                } else "s" != c && "n" != c && (u = !1, l--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
-        for (l = 1; l < e.length; l++) {
-            var b = e[l];
-            c.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? n(b, r) : !p())
+        var s = [],
+            p = s.pop.bind(s);
+        for (i = 1; i < e.length; i++) {
+            var b = e[i];
+            s.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? n(b, r) : !p())
         }
         return !!p()
-    }, l = (e, r) => {
+    }, i = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, i = (e, r) => {
+    }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", d = (e, r, t, a) => {
-        var o = i(e, t);
-        return n(a, o) || s(u(e, t, o, a)), c(e[t][o])
-    }, f = (e, r, t) => {
+    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", f = (e, r, t, a) => {
+        var o = l(e, t);
+        return n(a, o) || c(u(e, t, o, a)), s(e[t][o])
+    }, d = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !n(t, r) || e && !a(e, r) ? e : r), 0)) && o[r]
-    }, s = e => {
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), b = (p = e => function(r, t, a, o) {
+    }, s = e => (e.loaded = 1, e.get()), b = (p = e => function(r, t, a, o) {
         var n = P.I(r);
         return n && n.then ? n.then(e.bind(e, r, P.S[r], t, a, o)) : e(r, P.S[r], t, a, o)
-    })(((e, r, t, a) => (l(e, t), d(r, 0, t, a)))), h = p(((e, r, t, a, o) => r && P.o(r, t) ? d(r, 0, t, a) : o())), v = p(((e, r, t, a, o) => {
-        var n = r && P.o(r, t) && f(r, t, a);
-        return n ? c(n) : o()
+    })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), h = p(((e, r, t, a, o) => r && P.o(r, t) ? f(r, 0, t, a) : o())), v = p(((e, r, t, a, o) => {
+        var n = r && P.o(r, t) && d(r, t, a);
+        return n ? s(n) : o()
     })), y = {}, m = {
-        9324: () => b("default", "@jupyterlab/apputils", [1, 4, 1, 1]),
-        9474: () => b("default", "@jupyterlab/coreutils", [1, 6, 0, 1]),
         981: () => b("default", "yjs", [1, 13, 5, 40]),
-        3897: () => b("default", "@jupyterlab/ui-components", [1, 4, 0, 1]),
-        7387: () => b("default", "@jupyterlab/translation", [1, 4, 0, 1]),
+        5350: () => b("default", "@jupyterlab/apputils", [1, 4, 1, 2]),
+        9993: () => b("default", "@jupyterlab/coreutils", [1, 6, 0, 2]),
+        926: () => b("default", "@jupyterlab/translation", [1, 4, 0, 2]),
+        2189: () => b("default", "@jupyterlab/ui-components", [1, 4, 0, 2]),
         8778: () => b("default", "@lumino/widgets", [1, 2, 0, 1]),
-        3020: () => b("default", "@jupyterlab/services", [1, 7, 0, 1]),
-        7099: () => v("default", "y-websocket", [1, 1, 3, 15], (() => Promise.all([P.e(493), P.e(413), P.e(981)]).then((() => () => P(413))))),
-        94: () => b("default", "@jupyterlab/settingregistry", [1, 4, 0, 1]),
-        674: () => b("default", "@jupyterlab/codemirror", [1, 4, 0, 1]),
-        899: () => b("default", "@jupyterlab/notebook", [1, 4, 0, 1]),
-        1039: () => h("default", "@jupyter/docprovider", [1, 1, 0, 0, , "alpha", 9], (() => Promise.all([P.e(930), P.e(901), P.e(933)]).then((() => () => P(2008))))),
-        1802: () => b("default", "@jupyterlab/statedb", [1, 4, 0, 1]),
-        2177: () => b("default", "@jupyterlab/application", [1, 4, 0, 1]),
+        4238: () => b("default", "@jupyterlab/services", [1, 7, 0, 2]),
+        56: () => b("default", "@jupyterlab/settingregistry", [1, 4, 0, 2]),
+        1255: () => h("default", "@jupyter/collaboration", [1, 1, 0, 1], (() => Promise.all([P.e(930), P.e(760)]).then((() => () => P(4760))))),
+        1617: () => b("default", "@jupyterlab/statedb", [1, 4, 0, 2]),
+        1919: () => b("default", "@jupyterlab/notebook", [1, 4, 0, 2]),
+        2164: () => b("default", "@jupyterlab/filebrowser", [1, 4, 0, 2]),
         2293: () => b("default", "@jupyter/ydoc", [1, 1, 0, 2]),
-        2497: () => b("default", "@jupyterlab/fileeditor", [1, 4, 0, 1]),
-        5116: () => b("default", "@jupyterlab/logconsole", [1, 4, 0, 1]),
-        5355: () => b("default", "@jupyterlab/filebrowser", [1, 4, 0, 1]),
-        6903: () => h("default", "@jupyter/collaboration", [1, 1, 0, 0, , "alpha", 9], (() => Promise.all([P.e(930), P.e(760)]).then((() => () => P(4760))))),
+        2927: () => b("default", "@jupyterlab/codemirror", [1, 4, 0, 2]),
+        4163: () => b("default", "@jupyterlab/application", [1, 4, 0, 2]),
+        4822: () => h("default", "@jupyter/docprovider", [1, 1, 0, 1], (() => Promise.all([P.e(930), P.e(314), P.e(252)]).then((() => () => P(4299))))),
+        8486: () => b("default", "@jupyterlab/fileeditor", [1, 4, 0, 2]),
+        9350: () => b("default", "@jupyterlab/logconsole", [1, 4, 0, 2]),
         7930: () => b("default", "@lumino/coreutils", [1, 2, 0, 0]),
         4059: () => b("default", "@lumino/virtualdom", [1, 2, 0, 0]),
         6029: () => b("default", "react", [1, 18, 2, 0]),
         6211: () => b("default", "@codemirror/view", [1, 6, 9, 6]),
         8204: () => b("default", "@codemirror/state", [1, 6, 2, 0]),
-        4901: () => b("default", "@lumino/signaling", [1, 2, 0, 0])
+        4901: () => b("default", "@lumino/signaling", [1, 2, 0, 0]),
+        7099: () => v("default", "y-websocket", [1, 1, 3, 15], (() => Promise.all([P.e(413), P.e(981)]).then((() => () => P(413)))))
     }, g = {
-        87: [94, 674, 899, 1039, 1802, 2177, 2293, 2497, 5116, 5355, 6903],
-        296: [3897, 7387, 8778],
-        619: [9324, 9474],
-        744: [3020, 7099],
+        46: [926, 2189, 8778],
+        87: [56, 1255, 1617, 1919, 2164, 2293, 2927, 4163, 4822, 8486, 9350],
+        238: [4238],
+        314: [4901, 7099],
+        662: [5350, 9993],
         760: [4059, 6029, 6211, 8204],
-        901: [4901],
         930: [7930],
         981: [981]
     }, P.f.consumes = (e, r) => {
         P.o(g, e) && g[e].forEach((e => {
             if (P.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, P.m[e] = t => {
@@ -299,35 +299,35 @@
         var e = {
             510: 0
         };
         P.f.j = (r, t) => {
             var a = P.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(9(01|30|81)|296|619|744)$/.test(r)) e[r] = 0;
+                else if (/^(238|314|46|662|930|981)$/.test(r)) e[r] = 0;
             else {
                 var o = new Promise(((t, o) => a = e[r] = [t, o]));
                 t.push(a[2] = o);
                 var n = P.p + P.u(r),
-                    l = new Error;
+                    i = new Error;
                 P.l(n, (t => {
                     if (P.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
                             n = t && t.target && t.target.src;
-                        l.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", l.name = "ChunkLoadError", l.type = o, l.request = n, a[1](l)
+                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var a, o, [n, l, i] = t,
+                var a, o, [n, i, l] = t,
                     u = 0;
                 if (n.some((r => 0 !== e[r]))) {
-                    for (a in l) P.o(l, a) && (P.m[a] = l[a]);
-                    i && i(P)
+                    for (a in i) P.o(i, a) && (P.m[a] = i[a]);
+                    l && l(P)
                 }
                 for (r && r(t); u < n.length; u++) o = n[u], P.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), P.nc = void 0;
     var S = P(6746);
```

### Comparing `jupyter_collaboration-1.0.0a9/jupyter_collaboration/labextension/static/third-party-licenses.json` & `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '1.0.1'}, 1: {'versionInfo': '1.0.1'}}"}*

```diff
@@ -1,20 +1,20 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/collaboration",
-            "versionInfo": "1.0.0-alpha.9"
+            "versionInfo": "1.0.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/docprovider",
-            "versionInfo": "1.0.0-alpha.9"
+            "versionInfo": "1.0.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "6.7.3"
         },
```

### Comparing `jupyter_collaboration-1.0.0a9/scripts/bump_version.py` & `jupyter_collaboration-1.0.1/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/tests/test_loaders.py` & `jupyter_collaboration-1.0.1/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration/package.json` & `jupyter_collaboration-1.0.1/packages/collaboration/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.973076923076923%*

 * *Differences: {"'dependencies'": "{'@jupyter/docprovider': '^1.0.1'}", "'version'": "'1.0.1'"}*

```diff
@@ -2,14 +2,15 @@
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
         "@codemirror/state": "^6.2.0",
         "@codemirror/view": "^6.7.0",
+        "@jupyter/docprovider": "^1.0.1",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/services": "^7.0.0",
         "@jupyterlab/ui-components": "^4.0.0",
         "@lumino/coreutils": "^2.1.0",
         "@lumino/virtualdom": "^2.0.0",
         "@lumino/widgets": "^2.1.0",
@@ -62,9 +63,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.9"
+    "version": "1.0.1"
 }
```

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration/src/collaboratorspanel.tsx` & `jupyter_collaboration-1.0.1/packages/collaboration/src/collaboratorspanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration/src/components.tsx` & `jupyter_collaboration-1.0.1/packages/collaboration/src/components.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration/src/cursors.ts` & `jupyter_collaboration-1.0.1/packages/collaboration/src/cursors.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration/src/menu.ts` & `jupyter_collaboration-1.0.1/packages/collaboration/src/menu.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration/src/sharedlink.ts` & `jupyter_collaboration-1.0.1/packages/collaboration/src/sharedlink.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration/src/tokens.ts` & `jupyter_collaboration-1.0.1/packages/collaboration/src/tokens.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 // Copyright (c) Jupyter Development Team.
 // Distributed under the terms of the Modified BSD License.
 
 import type { Menu } from '@lumino/widgets';
 import { Token } from '@lumino/coreutils';
-import type { Awareness } from 'y-protocols/awareness';
+import { IAwareness } from '@jupyter/docprovider';
 import type { User } from '@jupyterlab/services';
 
 /**
  * The user menu token.
  *
  * NOTE: Require this token in your extension to access the user menu
  * (top-right menu in JupyterLab's interface).
@@ -20,19 +20,14 @@
  * The global awareness token.
  */
 export const IGlobalAwareness = new Token<IAwareness>(
   '@jupyter/collaboration:IGlobalAwareness'
 );
 
 /**
- * The awareness interface.
- */
-export type IAwareness = Awareness;
-
-/**
  * An interface describing the user menu.
  */
 export interface IUserMenu {
   /**
    * Dispose of the resources held by the menu.
    */
   dispose(): void;
```

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration/src/userinfopanel.tsx` & `jupyter_collaboration-1.0.1/packages/collaboration/src/userinfopanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration/style/menu.css` & `jupyter_collaboration-1.0.1/packages/collaboration/style/menu.css`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration/style/sidepanel.css` & `jupyter_collaboration-1.0.1/packages/collaboration/style/sidepanel.css`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration-extension/package.json` & `jupyter_collaboration-1.0.1/packages/collaboration-extension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.0.1', '@jupyter/docprovider': '^1.0.1'}",*

 * * "'version'": "'1.0.1'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.0-alpha.9",
-        "@jupyter/docprovider": "^1.0.0-alpha.9",
+        "@jupyter/collaboration": "^1.0.1",
+        "@jupyter/docprovider": "^1.0.1",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/codemirror": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/fileeditor": "^4.0.0",
@@ -124,9 +124,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.9"
+    "version": "1.0.1"
 }
```

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/collaboration.ts` & `jupyter_collaboration-1.0.1/packages/collaboration-extension/src/collaboration.ts`

 * *Files 3% similar despite different names*

```diff
@@ -12,32 +12,31 @@
 import { DOMUtils, IToolbarWidgetRegistry } from '@jupyterlab/apputils';
 import {
   EditorExtensionRegistry,
   IEditorExtensionRegistry
 } from '@jupyterlab/codemirror';
 import {
   CollaboratorsPanel,
-  IAwareness,
   IGlobalAwareness,
   IUserMenu,
   remoteUserCursors,
   RendererUserMenu,
   UserInfoPanel,
   UserMenu
 } from '@jupyter/collaboration';
+import { IAwareness, WebSocketAwarenessProvider } from '@jupyter/docprovider';
 import { SidePanel, usersIcon } from '@jupyterlab/ui-components';
 import { Menu, MenuBar } from '@lumino/widgets';
 import { URLExt } from '@jupyterlab/coreutils';
 import { ServerConnection } from '@jupyterlab/services';
 import { IStateDB, StateDB } from '@jupyterlab/statedb';
 import { ITranslator, nullTranslator } from '@jupyterlab/translation';
 
 import * as Y from 'yjs';
 import { Awareness } from 'y-protocols/awareness';
-import { WebsocketProvider } from 'y-websocket';
 
 /**
  * Jupyter plugin providing the IUserMenu.
  */
 export const userMenuPlugin: JupyterFrontEndPlugin<IUserMenu> = {
   id: '@jupyter/collaboration-extension:userMenu',
   description: 'Provide connected user menu.',
@@ -86,34 +85,28 @@
 export const rtcGlobalAwarenessPlugin: JupyterFrontEndPlugin<IAwareness> = {
   id: '@jupyter/collaboration-extension:rtcGlobalAwareness',
   description: 'Add global awareness to share working document of users.',
   requires: [IStateDB],
   provides: IGlobalAwareness,
   activate: (app: JupyterFrontEnd, state: StateDB): IAwareness => {
     const { user } = app.serviceManager;
-    const ydoc = new Y.Doc();
 
+    const ydoc = new Y.Doc();
     const awareness = new Awareness(ydoc);
 
     const server = ServerConnection.makeSettings();
     const url = URLExt.join(server.wsUrl, 'api/collaboration/room');
 
-    new WebsocketProvider(url, 'JupyterLab:globalAwareness', ydoc, {
-      awareness: awareness
+    new WebSocketAwarenessProvider({
+      url: url,
+      roomID: 'JupyterLab:globalAwareness',
+      awareness: awareness,
+      user: user
     });
 
-    const userChanged = () => {
-      awareness.setLocalStateField('user', user.identity);
-    };
-    if (user.isReady) {
-      userChanged();
-    }
-    user.ready.then(userChanged).catch(e => console.error(e));
-    user.userChanged.connect(userChanged);
-
     state.changed.connect(async () => {
       const data: any = await state.toJSON();
       const current = data['layout-restorer:data']?.main?.current || '';
 
       if (current.startsWith('editor') || current.startsWith('notebook')) {
         awareness.setLocalStateField('current', current);
       } else {
```

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/filebrowser.ts` & `jupyter_collaboration-1.0.1/packages/collaboration-extension/src/filebrowser.ts`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
           });
 
           if (emission.level === 'WARNING') {
             showDialog({
               title: trans.__('Warning'),
               body: trans.__(
                 `Two collaborative sessions are accessing the file %1 simultaneously.
-                \n'Opening a document with multiple views simultaneously is not supported. Please close one view; otherwise, you might lose some of your progress.`,
+                \nOpening a document with multiple views simultaneously is not supported. Please close one view; otherwise, you might lose some of your progress.`,
                 emission.path
               ),
               buttons: [Dialog.warnButton({ label: trans.__('Ok') })]
             });
           }
         }
       }
```

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/index.ts` & `jupyter_collaboration-1.0.1/packages/collaboration-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/collaboration-extension/src/sharedlink.ts` & `jupyter_collaboration-1.0.1/packages/collaboration-extension/src/sharedlink.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/docprovider/jest.config.js` & `jupyter_collaboration-1.0.1/packages/docprovider/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/docprovider/package.json` & `jupyter_collaboration-1.0.1/packages/docprovider/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'1.0.1'"}*

```diff
@@ -61,9 +61,9 @@
     ],
     "typedoc": {
         "displayName": "@jupyter/docprovider",
         "entryPoint": "./src/index.ts",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.9"
+    "version": "1.0.1"
 }
```

### Comparing `jupyter_collaboration-1.0.0a9/packages/docprovider/src/requests.ts` & `jupyter_collaboration-1.0.1/packages/docprovider/src/requests.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/docprovider/src/tokens.ts` & `jupyter_collaboration-1.0.1/packages/docprovider/src/tokens.ts`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 // Copyright (c) Jupyter Development Team.
 // Distributed under the terms of the Modified BSD License.
 
 import { DocumentChange, YDocument } from '@jupyter/ydoc';
 import { Contents } from '@jupyterlab/services';
+
 import { Token } from '@lumino/coreutils';
+import { ISignal } from '@lumino/signaling';
+
+import type { Awareness } from 'y-protocols/awareness';
+
+import { IChatMessage } from './awareness';
 
 /**
  * The collaborative drive.
  */
 export const ICollaborativeDrive = new Token<ICollaborativeDrive>(
   '@jupyter/collaboration-extension:ICollaborativeDrive'
 );
@@ -41,7 +47,31 @@
    * @param factory Document factory
    */
   registerDocumentFactory(
     type: Contents.ContentType,
     factory: SharedDocumentFactory
   ): void;
 }
+
+/**
+ * The awareness interface.
+ *
+ * TODO: Move to @jupyter/YDoc
+ */
+export type IAwareness = Awareness;
+
+/**
+ * A provider interface for global awareness features.
+ */
+export interface IAwarenessProvider {
+  /**
+   * A signal to subscribe for incoming messages.
+   */
+  get chatMessage(): ISignal<this, IChatMessage>;
+
+  /**
+   * Send a message to every collaborator.
+   *
+   * @param msg message
+   */
+  sendMessage(msg: string): void;
+}
```

### Comparing `jupyter_collaboration-1.0.0a9/packages/docprovider/src/ydrive.ts` & `jupyter_collaboration-1.0.1/packages/docprovider/src/ydrive.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/packages/docprovider/src/yprovider.ts` & `jupyter_collaboration-1.0.1/packages/docprovider/src/yprovider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/.gitignore` & `jupyter_collaboration-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/LICENSE` & `jupyter_collaboration-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a9/README.md` & `jupyter_collaboration-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 ## Installation and Basic usage
 
 To install the latest release locally, make sure you have
 [pip installed](https://pip.readthedocs.io/en/stable/installing/) and run:
 
 ```bash
-pip install jupyter_collaboration
+pip install jupyter-collaboration
 ```
 
 Or using ``conda``/``mamba``:
 
 ```bash
-conda install jupyter_collaboration
+conda install jupyter-collaboration
 ```
 
 ### Testing
 
 See [CONTRIBUTING](./docs/source/developer/contributing.rst#running-tests).
 
 ## Contributing
```

### Comparing `jupyter_collaboration-1.0.0a9/pyproject.toml` & `jupyter_collaboration-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Framework :: Jupyter :: JupyterLab :: 4",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
 ]
 dependencies = [
     "jupyter_server>=2.0.0,<3.0.0",
     "jupyter_ydoc>=1.0.1,<2.0.0",
-    "ypy-websocket>=0.8.3,<0.9.0",
+    "ypy-websocket>=0.12.1,<0.13.0",
     "jupyter_events",
     "jupyter_server_fileid>=0.6.0,<1"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 dev = [
@@ -96,15 +96,14 @@
 build_cmd = "build:prod"
 editable_build_cmd = "install:extension"
 
 [tool.jupyter-releaser]
 skip = ["check-links"]
 
 [tool.jupyter-releaser.options]
-npm-cmd = "npm publish --tag next"
 version-cmd = "python scripts/bump_version.py --force"
 
 [tool.jupyter-releaser.hooks]
 before-build-npm = [
     "YARN_ENABLE_IMMUTABLE_INSTALLS=0 jlpm build:prod"
 ]
 before-build-python = [
```

### Comparing `jupyter_collaboration-1.0.0a9/PKG-INFO` & `jupyter_collaboration-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_collaboration
-Version: 1.0.0a9
+Version: 1.0.1
 Summary: JupyterLab Extension enabling Real-Time Collaboration
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter_collaboration
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter_collaboration/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter_collaboration.git
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
         
@@ -81,15 +81,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: jupyter-events
 Requires-Dist: jupyter-server-fileid<1,>=0.6.0
 Requires-Dist: jupyter-server<3.0.0,>=2.0.0
 Requires-Dist: jupyter-ydoc<2.0.0,>=1.0.1
-Requires-Dist: ypy-websocket<0.9.0,>=0.8.3
+Requires-Dist: ypy-websocket<0.13.0,>=0.12.1
 Provides-Extra: dev
 Requires-Dist: click; extra == 'dev'
 Requires-Dist: jupyter-releaser; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: jupyterlab>=4.0.0; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
@@ -113,21 +113,21 @@
 
 ## Installation and Basic usage
 
 To install the latest release locally, make sure you have
 [pip installed](https://pip.readthedocs.io/en/stable/installing/) and run:
 
 ```bash
-pip install jupyter_collaboration
+pip install jupyter-collaboration
 ```
 
 Or using ``conda``/``mamba``:
 
 ```bash
-conda install jupyter_collaboration
+conda install jupyter-collaboration
 ```
 
 ### Testing
 
 See [CONTRIBUTING](./docs/source/developer/contributing.rst#running-tests).
 
 ## Contributing
```

