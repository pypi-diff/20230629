# Comparing `tmp/anywidget-0.6.0.tar.gz` & `tmp/anywidget-0.6.1.tar.gz`

## Comparing `anywidget-0.6.0.tar` & `anywidget-0.6.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.6.0/.pre-commit-config.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.6.0/CHANGELOG.md -> packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.6.0/CITATION.cff
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 anywidget-0.6.0/CONTRIBUTING.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget.json
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 anywidget-0.6.0/package.json
--rw-r--r--   0        0        0   267802 2020-02-02 00:00:00.000000 anywidget-0.6.0/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.6.0/pnpm-workspace.yaml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 anywidget-0.6.0/tsconfig.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.6.0/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/__init__.py
--rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/_protocols.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/_util.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/_version.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/experimental.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/widget.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/static/138.3fd6605047ad3df65a9e.js
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/static/326.c68678f64e2971595925.js
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/static/remoteEntry.cba6b4061725caaf22a8.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/astro.config.js
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/scripts/render.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/en/experimental.md
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 anywidget-0.6.0/examples/Counter.ipynb
--rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 anywidget-0.6.0/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/package.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/tsconfig.json
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/__tests__/widget.test.ts
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_descriptor.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_experimental.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_protocols.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_utils.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.6.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.6.0/LICENSE
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 anywidget-0.6.0/README.md
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 anywidget-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 anywidget-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.6.1/.pre-commit-config.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.6.1/CHANGELOG.md -> packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.6.1/CITATION.cff
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 anywidget-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget.json
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 anywidget-0.6.1/package.json
+-rw-r--r--   0        0        0   273627 2020-02-02 00:00:00.000000 anywidget-0.6.1/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.6.1/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 anywidget-0.6.1/tsconfig.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.6.1/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/__init__.py
+-rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/_version.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/experimental.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/widget.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/static/138.6d69013365e0a65d34c8.js
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/static/326.44c2db4e788cbf8b5f08.js
+-rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/static/remoteEntry.2cf77409ad03a77cbd09.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/astro.config.js
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/scripts/render.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/en/experimental.md
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 anywidget-0.6.1/examples/Counter.ipynb
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 anywidget-0.6.1/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/package.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/tsconfig.json
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/__tests__/widget.test.ts
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_descriptor.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_experimental.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_utils.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 anywidget-0.6.1/README.md
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 anywidget-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 anywidget-0.6.1/PKG-INFO
```

### Comparing `anywidget-0.6.0/.pre-commit-config.yaml` & `anywidget-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/CITATION.cff` & `anywidget-0.6.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/CONTRIBUTING.md` & `anywidget-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/package.json` & `anywidget-0.6.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333333%*

 * *Differences: {"'devDependencies'": "{'esbuild': '^0.18.10'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "devDependencies": {
         "@changesets/cli": "^2.26.1",
         "@svitejs/changesets-changelog-github-compact": "^1.1.0",
-        "esbuild": "^0.18.6",
+        "esbuild": "^0.18.10",
         "happy-dom": "^9.20.3",
         "typescript": "^5.1.3",
         "vitest": "^0.32.2"
     },
     "name": "@anywidget/monorepo",
     "packageManager": "pnpm@8.6.1",
     "scripts": {
```

### Comparing `anywidget-0.6.0/pnpm-lock.yaml` & `anywidget-0.6.1/pnpm-lock.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lockfileVersion: '6.0'
+lockfileVersion: '6.1'
 
 settings:
   autoInstallPeers: true
   excludeLinksFromLockfile: false
 
 importers:
 
@@ -11,16 +11,16 @@
       '@changesets/cli':
         specifier: ^2.26.1
         version: 2.26.1
       '@svitejs/changesets-changelog-github-compact':
         specifier: ^1.1.0
         version: 1.1.0
       esbuild:
-        specifier: ^0.18.6
-        version: 0.18.6
+        specifier: ^0.18.10
+        version: 0.18.10
       happy-dom:
         specifier: ^9.20.3
         version: 9.20.3
       typescript:
         specifier: ^5.1.3
         version: 5.1.3
       vitest:
@@ -112,16 +112,16 @@
         specifier: ^2 || ^3 || ^4 || ^5 || ^6
         version: 2.0.0
     devDependencies:
       '@jupyter-widgets/base-manager':
         specifier: ^1.0.5
         version: 1.0.5(crypto@1.0.1)
       '@jupyterlab/builder':
-        specifier: ^4.0.2
-        version: 4.0.2(esbuild@0.18.6)
+        specifier: ^3.6.5
+        version: 3.6.5(crypto@1.0.1)(esbuild@0.18.10)
 
   packages/types: {}
 
   packages/vite:
     devDependencies:
       vite:
         specifier: ^4.3.9
@@ -874,16 +874,16 @@
     resolution: {integrity: sha512-KBMWvEZooR7+kzY0BtbTQn0OAYY7CsiydT63pVEaPtVYF0hXbUaOyZog37DKxK7NF3XacBJOpYT4adIJh+avxA==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [android]
     requiresBuild: true
     optional: true
 
-  /@esbuild/android-arm64@0.18.6:
-    resolution: {integrity: sha512-pL0Ci8P9q1sWbtPx8CXbc8JvPvvYdJJQ+LO09PLFsbz3aYNdFBGWJjiHU+CaObO4Ames+GOFpXRAJZS2L3ZK/A==}
+  /@esbuild/android-arm64@0.18.10:
+    resolution: {integrity: sha512-ynm4naLbNbK0ajf9LUWtQB+6Vfg1Z/AplArqr4tGebC00Z6m9Y91OVIcjDa461wGcZwcaHYaZAab4yJxfhisTQ==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -891,16 +891,16 @@
     resolution: {integrity: sha512-rIKddzqhmav7MSmoFCmDIb6e2W57geRsM94gV2l38fzhXMwq7hZoClug9USI2pFRGL06f4IOPHHpFNOkWieR8A==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [android]
     requiresBuild: true
     optional: true
 
-  /@esbuild/android-arm@0.18.6:
-    resolution: {integrity: sha512-J3lwhDSXBBppSzm/LC1uZ8yKSIpExc+5T8MxrYD9KNVZG81FOAu2VF2gXi/6A/LwDDQQ+b6DpQbYlo3VwxFepQ==}
+  /@esbuild/android-arm@0.18.10:
+    resolution: {integrity: sha512-3KClmVNd+Fku82uZJz5C4Rx8m1PPmWUFz5Zkw8jkpZPOmsq+EG1TTOtw1OXkHuX3WczOFQigrtf60B1ijKwNsg==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -908,16 +908,16 @@
     resolution: {integrity: sha512-uUTTc4xGNDT7YSArp/zbtmbhO0uEEK9/ETW29Wk1thYUJBz3IVnvgEiEwEa9IeLyvnpKrWK64Utw2bgUmDveww==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [android]
     requiresBuild: true
     optional: true
 
-  /@esbuild/android-x64@0.18.6:
-    resolution: {integrity: sha512-hE2vZxOlJ05aY28lUpB0y0RokngtZtcUB+TVl9vnLEnY0z/8BicSvrkThg5/iI1rbf8TwXrbr2heEjl9fLf+EA==}
+  /@esbuild/android-x64@0.18.10:
+    resolution: {integrity: sha512-vFfXj8P9Yfjh54yqUDEHKzqzYuEfPyAOl3z7R9hjkwt+NCvbn9VMxX+IILnAfdImRBfYVItgSUsqGKhJFnBwZw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -925,16 +925,16 @@
     resolution: {integrity: sha512-80wEoCfF/hFKM6WE1FyBHc9SfUblloAWx6FJkFWTWiCoht9Mc0ARGEM47e67W9rI09YoUxJL68WHfDRYEAvOhg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [darwin]
     requiresBuild: true
     optional: true
 
-  /@esbuild/darwin-arm64@0.18.6:
-    resolution: {integrity: sha512-/tuyl4R+QhhoROQtuQj9E/yfJtZNdv2HKaHwYhhHGQDN1Teziem2Kh7BWQMumfiY7Lu9g5rO7scWdGE4OsQ6MQ==}
+  /@esbuild/darwin-arm64@0.18.10:
+    resolution: {integrity: sha512-k2OJQ7ZxE6sVc91+MQeZH9gFeDAH2uIYALPAwTjTCvcPy9Dzrf7V7gFUQPYkn09zloWhQ+nvxWHia2x2ZLR0sQ==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -942,16 +942,16 @@
     resolution: {integrity: sha512-IJM4JJsLhRYr9xdtLytPLSH9k/oxR3boaUIYiHkAawtwNOXKE8KoU8tMvryogdcT8AU+Bflmh81Xn6Q0vTZbQw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [darwin]
     requiresBuild: true
     optional: true
 
-  /@esbuild/darwin-x64@0.18.6:
-    resolution: {integrity: sha512-L7IQga2pDT+14Ti8HZwsVfbCjuKP4U213T3tuPggOzyK/p4KaUJxQFXJgfUFHKzU0zOXx8QcYRYZf0hSQtppkw==}
+  /@esbuild/darwin-x64@0.18.10:
+    resolution: {integrity: sha512-tnz/mdZk1L1Z3WpGjin/L2bKTe8/AKZpI8fcCLtH+gq8WXWsCNJSxlesAObV4qbtTl6pG5vmqFXfWUQ5hV8PAQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -959,16 +959,16 @@
     resolution: {integrity: sha512-pBwbc7DufluUeGdjSU5Si+P3SoMF5DQ/F/UmTSb8HXO80ZEAJmrykPyzo1IfNbAoaqw48YRpv8shwd1NoI0jcQ==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [freebsd]
     requiresBuild: true
     optional: true
 
-  /@esbuild/freebsd-arm64@0.18.6:
-    resolution: {integrity: sha512-bq10jFv42V20Kk77NvmO+WEZaLHBKuXcvEowixnBOMkaBgS7kQaqTc77ZJDbsUpXU3KKNLQFZctfaeINmeTsZA==}
+  /@esbuild/freebsd-arm64@0.18.10:
+    resolution: {integrity: sha512-QJluV0LwBrbHnYYwSKC+K8RGz0g/EyhpQH1IxdoFT0nM7PfgjE+aS8wxq/KFEsU0JkL7U/EEKd3O8xVBxXb2aA==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -976,16 +976,16 @@
     resolution: {integrity: sha512-4lu+n8Wk0XlajEhbEffdy2xy53dpR06SlzvhGByyg36qJw6Kpfk7cp45DR/62aPH9mtJRmIyrXAS5UWBrJT6TQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [freebsd]
     requiresBuild: true
     optional: true
 
-  /@esbuild/freebsd-x64@0.18.6:
-    resolution: {integrity: sha512-HbDLlkDZqUMBQaiday0pJzB6/8Xx/10dI3xRebJBReOEeDSeS+7GzTtW9h8ZnfB7/wBCqvtAjGtWQLTNPbR2+g==}
+  /@esbuild/freebsd-x64@0.18.10:
+    resolution: {integrity: sha512-Hi/ycUkS6KTw+U9G5PK5NoK7CZboicaKUSVs0FSiPNtuCTzK6HNM4DIgniH7hFaeuszDS9T4dhAHWiLSt/Y5Ng==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -993,16 +993,16 @@
     resolution: {integrity: sha512-ct1Tg3WGwd3P+oZYqic+YZF4snNl2bsnMKRkb3ozHmnM0dGWuxcPTTntAF6bOP0Sp4x0PjSF+4uHQ1xvxfRKqg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-arm64@0.18.6:
-    resolution: {integrity: sha512-NMY9yg/88MskEZH2s4i6biz/3av+M8xY5ua4HE7CCz5DBz542cr7REe317+v7oKjnYBCijHpkzo5vU85bkXQmQ==}
+  /@esbuild/linux-arm64@0.18.10:
+    resolution: {integrity: sha512-Nz6XcfRBOO7jSrVpKAyEyFOPGhySPNlgumSDhWAspdQQ11ub/7/NZDMhWDFReE9QH/SsCOCLQbdj0atAk/HMOQ==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1010,16 +1010,16 @@
     resolution: {integrity: sha512-cdmT3KxjlOQ/gZ2cjfrQOtmhG4HJs6hhvm3mWSRDPtZ/lP5oe8FWceS10JaSJC13GBd4eH/haHnqf7hhGNLerA==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-arm@0.18.6:
-    resolution: {integrity: sha512-C+5kb6rgsGMmvIdUI7v1PPgC98A6BMv233e97aXZ5AE03iMdlILFD/20HlHrOi0x2CzbspXn9HOnlE4/Ijn5Kw==}
+  /@esbuild/linux-arm@0.18.10:
+    resolution: {integrity: sha512-HfFoxY172tVHPIvJy+FHxzB4l8xU7e5cxmNS11cQ2jt4JWAukn/7LXaPdZid41UyTweqa4P/1zs201gRGCTwHw==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1027,16 +1027,16 @@
     resolution: {integrity: sha512-w4IRhSy1VbsNxHRQpeGCHEmibqdTUx61Vc38APcsRbuVgK0OPEnQ0YD39Brymn96mOx48Y2laBQGqgZ0j9w6SQ==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-ia32@0.18.6:
-    resolution: {integrity: sha512-AXazA0ljvQEp7cA9jscABNXsjodKbEcqPcAE3rDzKN82Vb3lYOq6INd+HOCA7hk8IegEyHW4T72Z7QGIhyCQEA==}
+  /@esbuild/linux-ia32@0.18.10:
+    resolution: {integrity: sha512-otMdmSmkMe+pmiP/bZBjfphyAsTsngyT9RCYwoFzqrveAbux9nYitDTpdgToG0Z0U55+PnH654gCH2GQ1aB6Yw==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1044,16 +1044,16 @@
     resolution: {integrity: sha512-2iAngUbBPMq439a+z//gE+9WBldoMp1s5GWsUSgqHLzLJ9WoZLZhpwWuym0u0u/4XmZ3gpHmzV84PonE+9IIdQ==}
     engines: {node: '>=12'}
     cpu: [loong64]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-loong64@0.18.6:
-    resolution: {integrity: sha512-JjBf7TwY7ldcPgHYt9UcrjZB03+WZqg/jSwMAfzOzM5ZG+tu5umUqzy5ugH/crGI4eoDIhSOTDp1NL3Uo/05Fw==}
+  /@esbuild/linux-loong64@0.18.10:
+    resolution: {integrity: sha512-t8tjFuON1koxskzQ4VFoh0T5UDUMiLYjwf9Wktd0tx8AoK6xgU+5ubKOpWpcnhEQ2tESS5u0v6QuN8PX/ftwcQ==}
     engines: {node: '>=12'}
     cpu: [loong64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1061,16 +1061,16 @@
     resolution: {integrity: sha512-LKJltc4LVdMKHsrFe4MGNPp0hqDFA1Wpt3jE1gEyM3nKUvOiO//9PheZZHfYRfYl6AwdTH4aTcXSqBerX0ml4A==}
     engines: {node: '>=12'}
     cpu: [mips64el]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-mips64el@0.18.6:
-    resolution: {integrity: sha512-kATNsslryVxcH1sO3KP2nnyUWtZZVkgyhAUnyTVVa0OQQ9pmDRjTpHaE+2EQHoCM5wt/uav2edrAUqbwn3tkKQ==}
+  /@esbuild/linux-mips64el@0.18.10:
+    resolution: {integrity: sha512-+dUkcVzcfEJHz3HEnVpIJu8z8Wdn2n/nWMWdl6FVPFGJAVySO4g3+XPzNKFytVFwf8hPVDwYXzVcu8GMFqsqZw==}
     engines: {node: '>=12'}
     cpu: [mips64el]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1078,16 +1078,16 @@
     resolution: {integrity: sha512-/c/DGybs95WXNS8y3Ti/ytqETiW7EU44MEKuCAcpPto3YjQbyK3IQVKfF6nbghD7EcLUGl0NbiL5Rt5DMhn5tg==}
     engines: {node: '>=12'}
     cpu: [ppc64]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-ppc64@0.18.6:
-    resolution: {integrity: sha512-B+wTKz+8pi7mcWXFQV0LA79dJ+qhiut5uK9q0omoKnq8yRIwQJwfg3/vclXoqqcX89Ri5Y5538V0Se2v5qlcLA==}
+  /@esbuild/linux-ppc64@0.18.10:
+    resolution: {integrity: sha512-sO3PjjxEGy+PY2qkGe2gwJbXdZN9wAYpVBZWFD0AwAoKuXRkWK0/zaMQ5ekUFJDRDCRm8x5U0Axaub7ynH/wVg==}
     engines: {node: '>=12'}
     cpu: [ppc64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1095,16 +1095,16 @@
     resolution: {integrity: sha512-FC3nUAWhvFoutlhAkgHf8f5HwFWUL6bYdvLc/TTuxKlvLi3+pPzdZiFKSWz/PF30TB1K19SuCxDTI5KcqASJqA==}
     engines: {node: '>=12'}
     cpu: [riscv64]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-riscv64@0.18.6:
-    resolution: {integrity: sha512-h44RBLVXFUSjvhOfseE+5UxQ/r9LVeqK2S8JziJKOm9W7SePYRPDyn7MhzhNCCFPkcjIy+soCxfhlJXHXXCR0A==}
+  /@esbuild/linux-riscv64@0.18.10:
+    resolution: {integrity: sha512-JDtdbJg3yjDeXLv4lZYE1kiTnxv73/8cbPHY9T/dUKi8rYOM/k5b3W4UJLMUksuQ6nTm5c89W1nADsql6FW75A==}
     engines: {node: '>=12'}
     cpu: [riscv64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1112,16 +1112,16 @@
     resolution: {integrity: sha512-IbFsFbxMWLuKEbH+7sTkKzL6NJmG2vRyy6K7JJo55w+8xDk7RElYn6xvXtDW8HCfoKBFK69f3pgBJSUSQPr+4Q==}
     engines: {node: '>=12'}
     cpu: [s390x]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-s390x@0.18.6:
-    resolution: {integrity: sha512-FlYpyr2Xc2AUePoAbc84NRV+mj7xpsISeQ36HGf9etrY5rTBEA+IU9HzWVmw5mDFtC62EQxzkLRj8h5Hq85yOQ==}
+  /@esbuild/linux-s390x@0.18.10:
+    resolution: {integrity: sha512-NLuSKcp8WckjD2a7z5kzLiCywFwBTMlIxDNuud1AUGVuwBBJSkuubp6cNjJ0p5c6CZaA3QqUGwjHJBiG1SoOFw==}
     engines: {node: '>=12'}
     cpu: [s390x]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1129,16 +1129,16 @@
     resolution: {integrity: sha512-68ngA9lg2H6zkZcyp22tsVt38mlhWde8l3eJLWkyLrp4HwMUr3c1s/M2t7+kHIhvMjglIBrFpncX1SzMckomGw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-x64@0.18.6:
-    resolution: {integrity: sha512-Mc4EUSYwzLci77u0Kao6ajB2WbTe5fNc7+lHwS3a+vJISC/oprwURezUYu1SdWAYoczbsyOvKAJwuNftoAdjjg==}
+  /@esbuild/linux-x64@0.18.10:
+    resolution: {integrity: sha512-wj2KRsCsFusli+6yFgNO/zmmLslislAWryJnodteRmGej7ZzinIbMdsyp13rVGde88zxJd5vercNYK9kuvlZaQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1146,16 +1146,16 @@
     resolution: {integrity: sha512-CwFq42rXCR8TYIjIfpXCbRX0rp1jo6cPIUPSaWwzbVI4aOfX96OXY8M6KNmtPcg7QjYeDmN+DD0Wp3LaBOLf4Q==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [netbsd]
     requiresBuild: true
     optional: true
 
-  /@esbuild/netbsd-x64@0.18.6:
-    resolution: {integrity: sha512-3hgZlp7NqIM5lNG3fpdhBI5rUnPmdahraSmwAi+YX/bp7iZ7mpTv2NkypGs/XngdMtpzljICxnUG3uPfqLFd3w==}
+  /@esbuild/netbsd-x64@0.18.10:
+    resolution: {integrity: sha512-pQ9QqxEPI3cVRZyUtCoZxhZK3If+7RzR8L2yz2+TDzdygofIPOJFaAPkEJ5rYIbUO101RaiYxfdOBahYexLk5A==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [netbsd]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1163,16 +1163,16 @@
     resolution: {integrity: sha512-cnq5brJYrSZ2CF6c35eCmviIN3k3RczmHz8eYaVlNasVqsNY+JKohZU5MKmaOI+KkllCdzOKKdPs762VCPC20g==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [openbsd]
     requiresBuild: true
     optional: true
 
-  /@esbuild/openbsd-x64@0.18.6:
-    resolution: {integrity: sha512-aEWTdZQHtSRROlDYn7ygB8yAqtnall/UnmoVIJVqccKitkAWVVSYocQUWrBOxLEFk8XdlRouVrLZe6WXszyviA==}
+  /@esbuild/openbsd-x64@0.18.10:
+    resolution: {integrity: sha512-k8GTIIW9I8pEEfoOUm32TpPMgSg06JhL5DO+ql66aLTkOQUs0TxCA67Wi7pv6z8iF8STCGcNbm3UWFHLuci+ag==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [openbsd]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1180,16 +1180,16 @@
     resolution: {integrity: sha512-vCRT7yP3zX+bKWFeP/zdS6SqdWB8OIpaRq/mbXQxTGHnIxspRtigpkUcDMlSCOejlHowLqII7K2JKevwyRP2rg==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [sunos]
     requiresBuild: true
     optional: true
 
-  /@esbuild/sunos-x64@0.18.6:
-    resolution: {integrity: sha512-uxk/5yAGpjKZUHOECtI9W+9IcLjKj+2m0qf+RG7f7eRBHr8wP6wsr3XbNbgtOD1qSpPapd6R2ZfSeXTkCcAo5g==}
+  /@esbuild/sunos-x64@0.18.10:
+    resolution: {integrity: sha512-vIGYJIdEI6d4JBucAx8py792G8J0GP40qSH+EvSt80A4zvGd6jph+5t1g+eEXcS2aRpgZw6CrssNCFZxTdEsxw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [sunos]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1197,16 +1197,16 @@
     resolution: {integrity: sha512-yYx+8jwowUstVdorcMdNlzklLYhPxjniHWFKgRqH7IFlUEa0Umu3KuYplf1HUZZ422e3NU9F4LGb+4O0Kdcaag==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [win32]
     requiresBuild: true
     optional: true
 
-  /@esbuild/win32-arm64@0.18.6:
-    resolution: {integrity: sha512-oXlXGS9zvNCGoAT/tLHAsFKrIKye1JaIIP0anCdpaI+Dc10ftaNZcqfLzEwyhdzFAYInXYH4V7kEdH4hPyo9GA==}
+  /@esbuild/win32-arm64@0.18.10:
+    resolution: {integrity: sha512-kRhNcMZFGMW+ZHCarAM1ypr8OZs0k688ViUCetVCef9p3enFxzWeBg9h/575Y0nsFu0ZItluCVF5gMR2pwOEpA==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1214,16 +1214,16 @@
     resolution: {integrity: sha512-eggDKanJszUtCdlVs0RB+h35wNlb5v4TWEkq4vZcmVt5u/HiDZrTXe2bWFQUez3RgNHwx/x4sk5++4NSSicKkw==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [win32]
     requiresBuild: true
     optional: true
 
-  /@esbuild/win32-ia32@0.18.6:
-    resolution: {integrity: sha512-qh7IcAHUvvmMBmoIG+V+BbE9ZWSR0ohF51e5g8JZvU08kZF58uDFL5tHs0eoYz31H6Finv17te3W3QB042GqVA==}
+  /@esbuild/win32-ia32@0.18.10:
+    resolution: {integrity: sha512-AR9PX1whYaYh9p0EOaKna0h48F/A101Mt/ag72+kMkkBZXPQ7cjbz2syXI/HI3OlBdUytSdHneljfjvUoqwqiQ==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1231,23 +1231,27 @@
     resolution: {integrity: sha512-lAhycmKnVOuRYNtRtatQR1LPQf2oYCkRGkSFnseDAKPl8lu5SOsK/e1sXe5a0Pc5kHIHe6P2I/ilntNv2xf3cA==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     optional: true
 
-  /@esbuild/win32-x64@0.18.6:
-    resolution: {integrity: sha512-9UDwkz7Wlm4N9jnv+4NL7F8vxLhSZfEkRArz2gD33HesAFfMLGIGNVXRoIHtWNw8feKsnGly9Hq1EUuRkWl0zA==}
+  /@esbuild/win32-x64@0.18.10:
+    resolution: {integrity: sha512-5sTkYhAGHNRr6bVf4RM0PsscqVr6/DBYdrlMh168oph3usid3lKHcHEEHmr34iZ9GHeeg2juFOxtpl6XyC3tpw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@gar/promisify@1.1.3:
+    resolution: {integrity: sha512-k2Ty1JcVojjJFwrg/ThKi2ujJ7XNLYaFGNB/bWT9wGR+oSMJHMa5w+CUq6p/pVrKeNNgA7pCqEcjSnHVoqJQFw==}
+    dev: true
+
   /@jridgewell/gen-mapping@0.3.3:
     resolution: {integrity: sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==}
     engines: {node: '>=6.0.0'}
     dependencies:
       '@jridgewell/set-array': 1.1.2
       '@jridgewell/sourcemap-codec': 1.4.15
       '@jridgewell/trace-mapping': 0.3.18
@@ -1328,52 +1332,59 @@
     transitivePeerDependencies:
       - bufferutil
       - crypto
       - encoding
       - utf-8-validate
     dev: true
 
-  /@jupyterlab/builder@4.0.2(esbuild@0.18.6):
-    resolution: {integrity: sha512-b4NPnnMNkfs07jeqxD2kctsZqYGncXWTmo0VsiMeiO4P19QaRMJrigjI56SC3V6100FpQby24yDZK625CR41lg==}
+  /@jupyterlab/builder@3.6.5(crypto@1.0.1)(esbuild@0.18.10):
+    resolution: {integrity: sha512-J9WO50gxjJ1bUo7BCix0fSxpRySCwaR8AaWNQ5QdYT1ARSGuSnfM9ZyeUOS61DvL3+h7IqsPTQQr5tbhIWv91Q==}
     hasBin: true
     dependencies:
-      '@lumino/algorithm': 2.0.0
-      '@lumino/application': 2.2.0
-      '@lumino/commands': 2.1.2
-      '@lumino/coreutils': 2.1.1
-      '@lumino/disposable': 2.1.1
-      '@lumino/domutils': 2.0.0
-      '@lumino/dragdrop': 2.1.2
-      '@lumino/messaging': 2.0.0
-      '@lumino/properties': 2.0.0
-      '@lumino/signaling': 2.1.1
-      '@lumino/virtualdom': 2.0.0
-      '@lumino/widgets': 2.2.0
-      ajv: 8.12.0
-      commander: 9.5.0
-      css-loader: 6.8.1(webpack@5.88.0)
+      '@lumino/algorithm': 1.9.2
+      '@lumino/application': 1.31.4(crypto@1.0.1)
+      '@lumino/commands': 1.21.1(crypto@1.0.1)
+      '@lumino/coreutils': 1.12.1(crypto@1.0.1)
+      '@lumino/disposable': 1.10.4
+      '@lumino/domutils': 1.8.2
+      '@lumino/dragdrop': 1.14.5(crypto@1.0.1)
+      '@lumino/messaging': 1.10.3
+      '@lumino/properties': 1.8.2
+      '@lumino/signaling': 1.11.1
+      '@lumino/virtualdom': 1.14.3
+      '@lumino/widgets': 1.37.2(crypto@1.0.1)
+      ajv: 6.12.6
+      commander: 6.0.0
+      css-loader: 5.2.7(webpack@5.88.0)
       duplicate-package-checker-webpack-plugin: 3.0.0
-      fs-extra: 10.1.0
+      file-loader: 6.0.0(webpack@5.88.0)
+      fs-extra: 9.1.0
       glob: 7.1.7
       license-webpack-plugin: 2.3.21(webpack@5.88.0)
-      mini-css-extract-plugin: 2.7.6(webpack@5.88.0)
-      mini-svg-data-uri: 1.4.4
+      mini-css-extract-plugin: 1.3.9(webpack@5.88.0)
       path-browserify: 1.0.1
       process: 0.11.10
+      raw-loader: 4.0.2(webpack@5.88.0)
       source-map-loader: 1.0.2(webpack@5.88.0)
-      style-loader: 3.3.3(webpack@5.88.0)
+      style-loader: 2.0.0(webpack@5.88.0)
       supports-color: 7.2.0
-      terser-webpack-plugin: 5.3.9(esbuild@0.18.6)(webpack@5.88.0)
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
-      webpack-cli: 5.1.4(webpack@5.88.0)
+      svg-url-loader: 6.0.0(webpack@5.88.0)
+      terser-webpack-plugin: 4.2.3(webpack@5.88.0)
+      to-string-loader: 1.2.0
+      url-loader: 4.1.1(file-loader@6.0.0)(webpack@5.88.0)
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack-cli: 4.10.0(webpack@5.88.0)
       webpack-merge: 5.9.0
       worker-loader: 3.0.8(webpack@5.88.0)
     transitivePeerDependencies:
       - '@swc/core'
       - '@webpack-cli/generators'
+      - '@webpack-cli/migrate'
+      - bluebird
+      - crypto
       - esbuild
       - uglify-js
       - webpack-bundle-analyzer
       - webpack-dev-server
     dev: true
 
   /@jupyterlab/coreutils@3.2.0:
@@ -1504,179 +1515,110 @@
   /@ljharb/has-package-exports-patterns@0.0.2:
     resolution: {integrity: sha512-4/RWEeXDO6bocPONheFe6gX/oQdP/bEpv0oL4HqjPP5DCenBSt0mHgahppY49N0CpsaqffdwPq+TlX9CYOq2Dw==}
 
   /@lumino/algorithm@1.9.2:
     resolution: {integrity: sha512-Z06lp/yuhz8CtIir3PNTGnuk7909eXt4ukJsCzChsGuot2l5Fbs96RJ/FOHgwCedaX74CtxPjXHXoszFbUA+4A==}
     dev: true
 
-  /@lumino/algorithm@2.0.0:
-    resolution: {integrity: sha512-SwM/8U1zlMWMJj00wTCThdTUit9zap2Xghuo4uUxvZ+mfog5b1UIk2j1dP8TPpzEXHCDPEb85s2/ERo1tee3Dw==}
-    dev: true
-
-  /@lumino/application@2.2.0:
-    resolution: {integrity: sha512-hivdDH2/YiOLtvsfY60GSUc+d6Rxh07dz6wp8ZnoalFmzdqqI8mcW4H30PchVdmqxXK0qxZIjLlP9A3fOu/xIw==}
+  /@lumino/application@1.31.4(crypto@1.0.1):
+    resolution: {integrity: sha512-dOSsDJ1tXOxC3fnSHvtDQK5RcICLEVPtO19HeCGwurb5W2ZZ55SZT2b5jZu6V/v8lGdtkNbr1RJltRpJRSRb/A==}
     dependencies:
-      '@lumino/commands': 2.1.2
-      '@lumino/coreutils': 2.1.1
-      '@lumino/widgets': 2.2.0
+      '@lumino/commands': 1.21.1(crypto@1.0.1)
+      '@lumino/coreutils': 1.12.1(crypto@1.0.1)
+      '@lumino/widgets': 1.37.2(crypto@1.0.1)
+    transitivePeerDependencies:
+      - crypto
     dev: true
 
   /@lumino/collections@1.9.3:
     resolution: {integrity: sha512-2i2Wf1xnfTgEgdyKEpqM16bcYRIhUOGCDzaVCEZACVG9R1CgYwOe3zfn71slBQOVSjjRgwYrgLXu4MBpt6YK+g==}
     dependencies:
       '@lumino/algorithm': 1.9.2
     dev: true
 
-  /@lumino/collections@2.0.0:
-    resolution: {integrity: sha512-uQvsRaQ8R8x/fTI2mk4+Z3EdUBDg/RtnqePDKtggWuu+BEjfk6vJ1jo42OGvEcurvhrrIZhFcpQJhtC+nNk4lA==}
-    dependencies:
-      '@lumino/algorithm': 2.0.0
-    dev: true
-
   /@lumino/commands@1.21.1(crypto@1.0.1):
     resolution: {integrity: sha512-d1zJmwz5bHU0BM/Rl3tRdZ7/WgXnFB0bM7x7Bf0XDlmX++jnU9k0j3mh6/5JqCGLmIApKCRwVqSaV7jPmSJlcQ==}
     dependencies:
       '@lumino/algorithm': 1.9.2
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
       '@lumino/disposable': 1.10.4
       '@lumino/domutils': 1.8.2
       '@lumino/keyboard': 1.8.2
       '@lumino/signaling': 1.11.1
       '@lumino/virtualdom': 1.14.3
     transitivePeerDependencies:
       - crypto
     dev: true
 
-  /@lumino/commands@2.1.2:
-    resolution: {integrity: sha512-wdA7kx2z0oygD44yQo5Tlk+yViKqmjTqwQSg2jfKfGyVOrwM3i1NXdZ8ntIV8WQIHmg24D2WqElwjUq5G7bGlw==}
-    dependencies:
-      '@lumino/algorithm': 2.0.0
-      '@lumino/coreutils': 2.1.1
-      '@lumino/disposable': 2.1.1
-      '@lumino/domutils': 2.0.0
-      '@lumino/keyboard': 2.0.0
-      '@lumino/signaling': 2.1.1
-      '@lumino/virtualdom': 2.0.0
-    dev: true
-
   /@lumino/coreutils@1.12.1(crypto@1.0.1):
     resolution: {integrity: sha512-JLu3nTHzJk9N8ohZ85u75YxemMrmDzJdNgZztfP7F7T7mxND3YVNCkJG35a6aJ7edu1sIgCjBxOvV+hv27iYvQ==}
     peerDependencies:
       crypto: 1.0.1
     dependencies:
       crypto: 1.0.1
     dev: true
 
-  /@lumino/coreutils@2.1.1:
-    resolution: {integrity: sha512-OmEzvphZC/EVpFfwBkmcuzNwKXvkij6gJo1mbf4/tZMC1/8NO3aVnjK1FsgC0TlaGwMD1BLIFgGay2mC/I/cyQ==}
-    dev: true
-
   /@lumino/disposable@1.10.4:
     resolution: {integrity: sha512-4ZxyYcyzUS+ZeB2KAH9oAH3w0DUUceiVr+FIZHZ2TAYGWZI/85WlqJtfm0xjwEpCwLLW1TDqJrISuZu3iMmVMA==}
     dependencies:
       '@lumino/algorithm': 1.9.2
       '@lumino/signaling': 1.11.1
     dev: true
 
-  /@lumino/disposable@2.1.1:
-    resolution: {integrity: sha512-zGl5hDDgDgPlrCN8b37gmNRjmYrTXnVq4WaseRtEgjj/en+gHLQW7sgTzkLgPj5rFaVETPkyrDTQ5uZVewFOAw==}
-    dependencies:
-      '@lumino/signaling': 2.1.1
-    dev: true
-
   /@lumino/domutils@1.8.2:
     resolution: {integrity: sha512-QIpMfkPJrs4GrWBuJf2Sn1fpyVPmvqUUAeD8xAQo8+4V5JAT0vUDLxZ9HijefMgNCi3+Bs8Z3lQwRCrz+cFP1A==}
     dev: true
 
-  /@lumino/domutils@2.0.0:
-    resolution: {integrity: sha512-GYsz6CS6Gd+7r9IBe/0m+3/xAuOKrjfiXwWt7OLsOM1icRv93yS+gxleCLp2+LSwoqU90sqfav+uYABtPkA4QA==}
-    dev: true
-
   /@lumino/dragdrop@1.14.5(crypto@1.0.1):
     resolution: {integrity: sha512-LC5xB82+xGF8hFyl716TMpV32OIMIMl+s3RU1PaqDkD6B7PkgiVk6NkJ4X9/GcEvl2igkvlGQt/3L7qxDAJNxw==}
     dependencies:
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
       '@lumino/disposable': 1.10.4
     transitivePeerDependencies:
       - crypto
     dev: true
 
-  /@lumino/dragdrop@2.1.2:
-    resolution: {integrity: sha512-89Sc2HpGHQnzQx4/A/oVmS1uOfy4YjRJtNvdr/7zoUeJTib9vxKvlzrsRopLqvmyQPzJMnulEkiWuWsgzNnLeA==}
-    dependencies:
-      '@lumino/coreutils': 2.1.1
-      '@lumino/disposable': 2.1.1
-    dev: true
-
   /@lumino/keyboard@1.8.2:
     resolution: {integrity: sha512-Dy+XqQ1wXbcnuYtjys5A0pAqf4SpAFl9NY6owyIhXAo0Va7w3LYp3jgiP1xAaBAwMuUppiUAfrbjrysZuZ625g==}
     dev: true
 
-  /@lumino/keyboard@2.0.0:
-    resolution: {integrity: sha512-bX42YYLJPuATGKH7DQaQrji28HXJJVU2QwAK/vrTiLpiZD28x6Q0QhwKaP5x4wNH8ikhwR9jRP7b9PNNtUGGfg==}
-    dev: true
-
   /@lumino/messaging@1.10.3:
     resolution: {integrity: sha512-F/KOwMCdqvdEG8CYAJcBSadzp6aI7a47Fr60zAKGqZATSRRRV41q53iXU7HjFPqQqQIvdn9Z7J32rBEAyQAzww==}
     dependencies:
       '@lumino/algorithm': 1.9.2
       '@lumino/collections': 1.9.3
     dev: true
 
-  /@lumino/messaging@2.0.0:
-    resolution: {integrity: sha512-B8cMK36hrkngntsdLNic3GEPfAk4qp6HIYWDrRSC1z7pjgjH8EEKUOO2MNNYNKNq3Hzpog7FM0nhT1tLqoFAYA==}
-    dependencies:
-      '@lumino/algorithm': 2.0.0
-      '@lumino/collections': 2.0.0
-    dev: true
-
   /@lumino/polling@1.11.4(crypto@1.0.1):
     resolution: {integrity: sha512-yC7JLssj3mqVK6TsYj7dg4AG0rcsC42YtpoDLtz9yzO84Q5flQUfmjAPQB6oPA6wZOlISs3iasF+uO2w1ls5jg==}
     dependencies:
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
       '@lumino/disposable': 1.10.4
       '@lumino/signaling': 1.11.1
     transitivePeerDependencies:
       - crypto
     dev: true
 
   /@lumino/properties@1.8.2:
     resolution: {integrity: sha512-EkjI9Cw8R0U+xC9HxdFSu7X1tz1H1vKu20cGvJ2gU+CXlMB1DvoYJCYxCThByHZ+kURTAap4SE5x8HvKwNPbig==}
     dev: true
 
-  /@lumino/properties@2.0.0:
-    resolution: {integrity: sha512-2TZE3gu1EZj5x2kEUBmr1aSemtgkkGlLkd3CwK0zjlukUhdrONveLsOX/Hr8+EnXv070i5lSr+9PzNNVqs9vPg==}
-    dev: true
-
   /@lumino/signaling@1.11.1:
     resolution: {integrity: sha512-YCUmgw08VoyMN5KxzqPO3KMx+cwdPv28tAN06C0K7Q/dQf+oufb1XocuhZb5selTrTmmuXeizaYxgLIQGdS1fA==}
     dependencies:
       '@lumino/algorithm': 1.9.2
       '@lumino/properties': 1.8.2
     dev: true
 
-  /@lumino/signaling@2.1.1:
-    resolution: {integrity: sha512-EUPJlC/kis5DEPA4UxsJRPidGk4qcgS+rfQlYfGfA4Z6vR8nzcwU9WE0UIWdqo6GN7cLWR8lGLzZzyIGY3+qiA==}
-    dependencies:
-      '@lumino/algorithm': 2.0.0
-      '@lumino/coreutils': 2.1.1
-    dev: true
-
   /@lumino/virtualdom@1.14.3:
     resolution: {integrity: sha512-5joUC1yuxeXbpfbSBm/OR8Mu9HoTo6PDX0RKqzlJ9o97iml7zayFN/ynzcxScKGQAo9iaXOY8uVIvGUT8FnsGw==}
     dependencies:
       '@lumino/algorithm': 1.9.2
     dev: true
 
-  /@lumino/virtualdom@2.0.0:
-    resolution: {integrity: sha512-N+Q4+ZcoaeQUb4cwxSzyy/DSuiCdHAtrGegrRo1M2KChKKa9DoyuQy3H9jZItrPpqh5VIQDu3UHMY0BsiwdgUA==}
-    dependencies:
-      '@lumino/algorithm': 2.0.0
-    dev: true
-
   /@lumino/widgets@1.37.2(crypto@1.0.1):
     resolution: {integrity: sha512-NHKu1NBDo6ETBDoNrqSkornfUCwc8EFFzw6+LWBfYVxn2PIwciq2SdiJGEyNqL+0h/A9eVKb5ui5z4cwpRekmQ==}
     dependencies:
       '@lumino/algorithm': 1.9.2
       '@lumino/commands': 1.21.1(crypto@1.0.1)
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
       '@lumino/disposable': 1.10.4
@@ -1687,30 +1629,14 @@
       '@lumino/properties': 1.8.2
       '@lumino/signaling': 1.11.1
       '@lumino/virtualdom': 1.14.3
     transitivePeerDependencies:
       - crypto
     dev: true
 
-  /@lumino/widgets@2.2.0:
-    resolution: {integrity: sha512-nQ5UXjcl+Tvddeev0We5aoW2erm5KffKCJZEo6/1i4t2cj90v2ndqtXtbiCjeQOBDojIH6u1BVPtUExTh00cbA==}
-    dependencies:
-      '@lumino/algorithm': 2.0.0
-      '@lumino/commands': 2.1.2
-      '@lumino/coreutils': 2.1.1
-      '@lumino/disposable': 2.1.1
-      '@lumino/domutils': 2.0.0
-      '@lumino/dragdrop': 2.1.2
-      '@lumino/keyboard': 2.0.0
-      '@lumino/messaging': 2.0.0
-      '@lumino/properties': 2.0.0
-      '@lumino/signaling': 2.1.1
-      '@lumino/virtualdom': 2.0.0
-    dev: true
-
   /@manypkg/find-root@1.1.0:
     resolution: {integrity: sha512-mki5uBvhHzO8kYYix/WRy2WX8S3B5wdVSc9D6KcU5lQNglP2yt58/VfLuAK49glRXChosY8ap2oJ1qgma3GUVA==}
     dependencies:
       '@babel/runtime': 7.22.5
       '@types/node': 12.20.55
       find-up: 4.1.0
       fs-extra: 8.1.0
@@ -1765,14 +1691,30 @@
   /@nodelib/fs.walk@1.2.8:
     resolution: {integrity: sha512-oGB+UxlgWcgQkgwo8GcEGwemoTFt3FIO9ababBmaGwXIoBKZ+GTy0pP185beGg7Llih/NSHSV2XAs1lnznocSg==}
     engines: {node: '>= 8'}
     dependencies:
       '@nodelib/fs.scandir': 2.1.5
       fastq: 1.15.0
 
+  /@npmcli/fs@1.1.1:
+    resolution: {integrity: sha512-8KG5RD0GVP4ydEzRn/I4BNDuxDtqVbOdm8675T49OIG/NGhaK0pjPX7ZcDlvKYbA+ulvVK3ztfcF4uBdOxuJbQ==}
+    dependencies:
+      '@gar/promisify': 1.1.3
+      semver: 7.5.3
+    dev: true
+
+  /@npmcli/move-file@1.1.2:
+    resolution: {integrity: sha512-1SUf/Cg2GzGDyaf15aR9St9TWlb+XvbZXWpDx8YKs7MLzMH/BCeopv+y9vzrzgkfykCGuWOlSu3mZhj2+FQcrg==}
+    engines: {node: '>=10'}
+    deprecated: This functionality has been moved to @npmcli/fs
+    dependencies:
+      mkdirp: 1.0.4
+      rimraf: 3.0.2
+    dev: true
+
   /@phosphor/algorithm@1.2.0:
     resolution: {integrity: sha512-C9+dnjXyU2QAkWCW6QVDGExk4hhwxzAKf5/FIuYlHAI9X5vFv99PYm0EREDxX1PbMuvfFBZhPNu0PvuSDQ7sFA==}
     dev: false
 
   /@phosphor/collections@1.2.0:
     resolution: {integrity: sha512-T9/0EjSuY6+ga2LIFRZ0xupciOR3Qnyy8Q95lhGTC0FXZUFwC8fl9e8On6IcwasCszS+1n8dtZUWSIynfgdpzw==}
     dependencies:
@@ -2250,49 +2192,43 @@
   /@webassemblyjs/wast-printer@1.11.6:
     resolution: {integrity: sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==}
     dependencies:
       '@webassemblyjs/ast': 1.11.6
       '@xtuc/long': 4.2.2
     dev: true
 
-  /@webpack-cli/configtest@2.1.1(webpack-cli@5.1.4)(webpack@5.88.0):
-    resolution: {integrity: sha512-wy0mglZpDSiSS0XHrVR+BAdId2+yxPSoJW8fsna3ZpYSlufjvxnP4YbKTCBZnNIcGN4r6ZPXV55X4mYExOfLmw==}
-    engines: {node: '>=14.15.0'}
+  /@webpack-cli/configtest@1.2.0(webpack-cli@4.10.0)(webpack@5.88.0):
+    resolution: {integrity: sha512-4FB8Tj6xyVkyqjj1OaTqCjXYULB9FMkqQ8yGrZjRDrYh0nOE+7Lhs45WioWQQMV+ceFlE368Ukhe6xdvJM9Egg==}
     peerDependencies:
-      webpack: 5.x.x
-      webpack-cli: 5.x.x
+      webpack: 4.x.x || 5.x.x
+      webpack-cli: 4.x.x
     dependencies:
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
-      webpack-cli: 5.1.4(webpack@5.88.0)
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack-cli: 4.10.0(webpack@5.88.0)
     dev: true
 
-  /@webpack-cli/info@2.0.2(webpack-cli@5.1.4)(webpack@5.88.0):
-    resolution: {integrity: sha512-zLHQdI/Qs1UyT5UBdWNqsARasIA+AaF8t+4u2aS2nEpBQh2mWIVb8qAklq0eUENnC5mOItrIB4LiS9xMtph18A==}
-    engines: {node: '>=14.15.0'}
+  /@webpack-cli/info@1.5.0(webpack-cli@4.10.0):
+    resolution: {integrity: sha512-e8tSXZpw2hPl2uMJY6fsMswaok5FdlGNRTktvFk2sD8RjH0hE2+XistawJx1vmKteh4NmGmNUrp+Tb2w+udPcQ==}
     peerDependencies:
-      webpack: 5.x.x
-      webpack-cli: 5.x.x
+      webpack-cli: 4.x.x
     dependencies:
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
-      webpack-cli: 5.1.4(webpack@5.88.0)
+      envinfo: 7.9.0
+      webpack-cli: 4.10.0(webpack@5.88.0)
     dev: true
 
-  /@webpack-cli/serve@2.0.5(webpack-cli@5.1.4)(webpack@5.88.0):
-    resolution: {integrity: sha512-lqaoKnRYBdo1UgDX8uF24AfGMifWK19TxPmM5FHc2vAGxrJ/qtyUyFBWoY1tISZdelsQ5fBcOusifo5o5wSJxQ==}
-    engines: {node: '>=14.15.0'}
+  /@webpack-cli/serve@1.7.0(webpack-cli@4.10.0):
+    resolution: {integrity: sha512-oxnCNGj88fL+xzV+dacXs44HcDwf1ovs3AuEzvP7mqXw7fQntqIhQ1BRmynh4qEKQSSSRSWVyXRjmTbZIX9V2Q==}
     peerDependencies:
-      webpack: 5.x.x
-      webpack-cli: 5.x.x
+      webpack-cli: 4.x.x
       webpack-dev-server: '*'
     peerDependenciesMeta:
       webpack-dev-server:
         optional: true
     dependencies:
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
-      webpack-cli: 5.1.4(webpack@5.88.0)
+      webpack-cli: 4.10.0(webpack@5.88.0)
     dev: true
 
   /@xtuc/ieee754@1.2.0:
     resolution: {integrity: sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==}
     dev: true
 
   /@xtuc/long@4.2.2:
@@ -2325,59 +2261,38 @@
     dev: true
 
   /acorn@8.9.0:
     resolution: {integrity: sha512-jaVNAFBHNLXspO543WnNNPZFRtavh3skAkITqD0/2aeMkKZTN+254PyhwxFYrk3vQ1xfY+2wbesJMs/JC8/PwQ==}
     engines: {node: '>=0.4.0'}
     hasBin: true
 
-  /ajv-formats@2.1.1(ajv@8.12.0):
-    resolution: {integrity: sha512-Wx0Kx52hxE7C18hkMEggYlEifqWZtYaRgouJor+WMdPnQyEK13vgEWyVNup7SoeeoLMsr4kf5h6dOW11I15MUA==}
-    peerDependencies:
-      ajv: ^8.0.0
-    peerDependenciesMeta:
-      ajv:
-        optional: true
+  /aggregate-error@3.1.0:
+    resolution: {integrity: sha512-4I7Td01quW/RpocfNayFdFVk1qSuoh0E7JrbRJ16nH01HhKFQ88INq9Sd+nd72zqRySlr9BmDA8xlEJ6vJMrYA==}
+    engines: {node: '>=8'}
     dependencies:
-      ajv: 8.12.0
+      clean-stack: 2.2.0
+      indent-string: 4.0.0
     dev: true
 
   /ajv-keywords@3.5.2(ajv@6.12.6):
     resolution: {integrity: sha512-5p6WTN0DdTGVQk6VjcEju19IgaHudalcfabD7yhDGeA6bcQnmL+CpveLJq/3hvfwd1aof6L386Ougkx6RfyMIQ==}
     peerDependencies:
       ajv: ^6.9.1
     dependencies:
       ajv: 6.12.6
     dev: true
 
-  /ajv-keywords@5.1.0(ajv@8.12.0):
-    resolution: {integrity: sha512-YCS/JNFAUyr5vAuhk1DWm1CBxRHW9LbJ2ozWeemrIqpbsqKjHVxYPyi5GC0rjZIT5JxJ3virVTS8wk4i/Z+krw==}
-    peerDependencies:
-      ajv: ^8.8.2
-    dependencies:
-      ajv: 8.12.0
-      fast-deep-equal: 3.1.3
-    dev: true
-
   /ajv@6.12.6:
     resolution: {integrity: sha512-j3fVLgvTo527anyYyJOGTYJbG+vnnQYvE0m5mmkc1TK+nxAppkCLMIL0aZ4dblVCNoGShhm+kzE4ZUykBoMg4g==}
     dependencies:
       fast-deep-equal: 3.1.3
       fast-json-stable-stringify: 2.1.0
       json-schema-traverse: 0.4.1
       uri-js: 4.4.1
 
-  /ajv@8.12.0:
-    resolution: {integrity: sha512-sRu1kpcO9yLtYxBKvqfTeh9KzZEwO3STyX1HT+4CaDzC6HpTGYhIhPIzj9XuKU7KYDwnaeh5hcOwjy1QuJzBPA==}
-    dependencies:
-      fast-deep-equal: 3.1.3
-      json-schema-traverse: 1.0.0
-      require-from-string: 2.0.2
-      uri-js: 4.4.1
-    dev: true
-
   /algoliasearch@4.18.0:
     resolution: {integrity: sha512-pCuVxC1SVcpc08ENH32T4sLKSyzoU7TkRIDBMwSLfIiW+fq4znOmWDkAygHZ6pRcO9I1UJdqlfgnV7TRj+MXrA==}
     dependencies:
       '@algolia/cache-browser-local-storage': 4.18.0
       '@algolia/cache-common': 4.18.0
       '@algolia/cache-in-memory': 4.18.0
       '@algolia/client-account': 4.18.0
@@ -2568,14 +2483,19 @@
       - less
       - sass
       - stylus
       - sugarss
       - supports-color
       - terser
 
+  /at-least-node@1.0.0:
+    resolution: {integrity: sha512-+q/t7Ekv1EDY2l6Gda6LLiX14rU9TV20Wa3ofeQmwPFZbOMo9DXrLbOjFaaclkXKWidIaopwAObQDqwWtGUjqg==}
+    engines: {node: '>= 4.0.0'}
+    dev: true
+
   /autoprefixer@10.4.14(postcss@8.4.24):
     resolution: {integrity: sha512-FQzyfOsTlwVzjHxKEqRIAdJx9niO6VCBCoEwax/VLSoQF29ggECcPuBqUMZ+u8jCZOPSy8b8/8KnuFbp0SaFZQ==}
     engines: {node: ^10 || ^12 || >=14}
     hasBin: true
     peerDependencies:
       postcss: ^8.1.0
     dependencies:
@@ -2731,14 +2651,40 @@
       streamsearch: 1.1.0
 
   /cac@6.7.14:
     resolution: {integrity: sha512-b6Ilus+c3RrdDk+JhLKUAQfzzgLEPy6wcXqS7f/xe1EETvsDP6GORG7SFuOs6cID5YkqchW/LXZbX5bc8j7ZcQ==}
     engines: {node: '>=8'}
     dev: true
 
+  /cacache@15.3.0:
+    resolution: {integrity: sha512-VVdYzXEn+cnbXpFgWs5hTT7OScegHVmLhJIR8Ufqk3iFD6A6j5iSX1KuBTfNEv4tdJWE2PzA6IVFtcLC7fN9wQ==}
+    engines: {node: '>= 10'}
+    dependencies:
+      '@npmcli/fs': 1.1.1
+      '@npmcli/move-file': 1.1.2
+      chownr: 2.0.0
+      fs-minipass: 2.1.0
+      glob: 7.1.7
+      infer-owner: 1.0.4
+      lru-cache: 6.0.0
+      minipass: 3.3.6
+      minipass-collect: 1.0.2
+      minipass-flush: 1.0.5
+      minipass-pipeline: 1.2.4
+      mkdirp: 1.0.4
+      p-map: 4.0.0
+      promise-inflight: 1.0.1
+      rimraf: 3.0.2
+      ssri: 8.0.1
+      tar: 6.1.15
+      unique-filename: 1.1.1
+    transitivePeerDependencies:
+      - bluebird
+    dev: true
+
   /call-bind@1.0.2:
     resolution: {integrity: sha512-7O+FbCihrB5WGbFYesctwmTKae6rOiIzmz1icreWJ+0aA7LJfuqhEso2T9ncpcFtzMQtzXf2QGGueWJGTYsqrA==}
     dependencies:
       function-bind: 1.1.1
       get-intrinsic: 1.2.1
     dev: true
 
@@ -2834,23 +2780,33 @@
       is-binary-path: 2.1.0
       is-glob: 4.0.3
       normalize-path: 3.0.0
       readdirp: 3.6.0
     optionalDependencies:
       fsevents: 2.3.2
 
+  /chownr@2.0.0:
+    resolution: {integrity: sha512-bIomtDF5KGpdogkLd9VspvFzk9KfpyyGlS8YFVZl7TGPBHL5snIOnxeshwVgPteQ9b4Eydl+pVbIyE1DcvCWgQ==}
+    engines: {node: '>=10'}
+    dev: true
+
   /chrome-trace-event@1.0.3:
     resolution: {integrity: sha512-p3KULyQg4S7NIHixdwbGX+nFHkoBiA4YQmyWtjb8XngSKV124nJmRysgAeujbUVb15vh+RvFUfCPqU7rXk+hZg==}
     engines: {node: '>=6.0'}
     dev: true
 
   /ci-info@3.8.0:
     resolution: {integrity: sha512-eXTggHWSooYhq49F2opQhuHWgzucfF2YgODK4e1566GQs5BIfP30B0oenwBJHfWxAs2fyPB1s7Mg949zLf61Yw==}
     engines: {node: '>=8'}
 
+  /clean-stack@2.2.0:
+    resolution: {integrity: sha512-4diC9HaTE+KRAMWhDhrGOECgWZxoevMc5TlkObMqNSsVU62PYzXZ/SMTjzyGAFF1YusgxGcSWTEXBhp0CPwQ1A==}
+    engines: {node: '>=6'}
+    dev: true
+
   /cli-boxes@3.0.0:
     resolution: {integrity: sha512-/lzGpEWL/8PfI0BmBOPRwp0c/wFNX1RdUML3jK/RcSBA9T8mZDdQpqYBKtCFTOfQbwPqWEOpjqW+Fnayc0969g==}
     engines: {node: '>=10'}
 
   /cli-cursor@4.0.0:
     resolution: {integrity: sha512-VGtlMu3x/4DOtIUwEkRezxUZ2lBacNJCHash0N0WeZDBS+7Ux1dm3XWAgWYxLJFMMdOeXMHXorshEFhbMSGelg==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
@@ -2911,36 +2867,40 @@
   /colorette@2.0.20:
     resolution: {integrity: sha512-IfEDxwoWIjkeXL1eXcDiow4UbKjhLdq6/EuSVR9GMN7KVH3r9gQ83e73hsz1Nd1T3ijd5xv1wcWRYO+D6kCI2w==}
     dev: true
 
   /comma-separated-tokens@2.0.3:
     resolution: {integrity: sha512-Fu4hJdvzeylCfQPp9SGWidpzrMs7tTrlu6Vb8XGaRGck8QSNZJJp538Wrb60Lax4fPwR64ViY468OIUTbRlGZg==}
 
-  /commander@10.0.1:
-    resolution: {integrity: sha512-y4Mg2tXshplEbSGzx7amzPwKKOCGuoSRP/CjEdwwk0FOGlUbq6lKuoyDZTNZkmxHdJtp54hdfY/JUrdL7Xfdug==}
-    engines: {node: '>=14'}
-    dev: true
-
   /commander@2.20.3:
     resolution: {integrity: sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==}
     dev: true
 
   /commander@4.1.1:
     resolution: {integrity: sha512-NOKm8xhkzAjzFx8B2v5OAHT+u5pRQc2UCa2Vq9jYL/31o2wi9mxBA7LIFs3sV5VSC49z6pEhfbMULvShKj26WA==}
     engines: {node: '>= 6'}
     dev: false
 
-  /commander@9.5.0:
-    resolution: {integrity: sha512-KRs7WVDKg86PWiuAqhDrAQnTXZKraVcCc6vFdL14qrZ/DcWwuRo7VoiYXalXO7S5GKpqYiVEwCbgFDfxNHKJBQ==}
-    engines: {node: ^12.20.0 || >=14}
+  /commander@6.0.0:
+    resolution: {integrity: sha512-s7EA+hDtTYNhuXkTlhqew4txMZVdszBmKWSPEMxGr8ru8JXR7bLUFIAtPhcSuFdJQ0ILMxnJi8GkQL0yvDy/YA==}
+    engines: {node: '>= 6'}
+    dev: true
+
+  /commander@7.2.0:
+    resolution: {integrity: sha512-QrWXB+ZQSVPmIWIhtEO9H+gwHaMGYiF5ChvoJ+K9ZGHG/sVsa6yiesAD1GC/x46sET00Xlwo1u49RVVVzvcSkw==}
+    engines: {node: '>= 10'}
     dev: true
 
   /common-ancestor-path@1.0.1:
     resolution: {integrity: sha512-L3sHRo1pXXEqX8VU28kfgUY+YGsk09hPqZiZmLacNib6XNTCM8ubYeT7ryXQw8asB1sKgcU5lkB7ONug08aB8w==}
 
+  /commondir@1.0.1:
+    resolution: {integrity: sha512-W9pAhw0ja1Edb5GVdIF1mjZw/ASI0AlShXM83UUGe2DVr5TdAPEA1OA8m/g8zWp9x6On7gqufY+FatDbC3MDQg==}
+    dev: true
+
   /concat-map@0.0.1:
     resolution: {integrity: sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==}
 
   /concordance@5.0.4:
     resolution: {integrity: sha512-OAcsnTEYu1ARJqWVGwf4zh4JDfHZEaSNlNccFmt8YjB2l/n19/PF2viLINHc57vO4FKIAFl2FWASIGZZWZ2Kxw==}
     engines: {node: '>=10.18.0 <11 || >=12.14.0 <13 || >=14'}
     dependencies:
@@ -2978,29 +2938,31 @@
       which: 2.0.2
 
   /crypto@1.0.1:
     resolution: {integrity: sha512-VxBKmeNcqQdiUQUW2Tzq0t377b54N2bMtXO/qiLa+6eRRmmC4qT3D4OnTGoT/U6O9aklQ/jTwbOtRMTTY8G0Ig==}
     deprecated: This package is no longer supported. It's now a built-in Node module. If you've depended on crypto, you should switch to the one that's built-in.
     dev: true
 
-  /css-loader@6.8.1(webpack@5.88.0):
-    resolution: {integrity: sha512-xDAXtEVGlD0gJ07iclwWVkLoZOpEvAWaSyf6W18S2pOC//K8+qUDIx8IIT3D+HjnmkJPQeesOPv5aiUaJsCM2g==}
-    engines: {node: '>= 12.13.0'}
+  /css-loader@5.2.7(webpack@5.88.0):
+    resolution: {integrity: sha512-Q7mOvpBNBG7YrVGMxRxcBJZFL75o+cH2abNASdibkj/fffYD8qWbInZrD0S9ccI6vZclF3DsHE7njGlLtaHbhg==}
+    engines: {node: '>= 10.13.0'}
     peerDependencies:
-      webpack: ^5.0.0
+      webpack: ^4.27.0 || ^5.0.0
     dependencies:
       icss-utils: 5.1.0(postcss@8.4.24)
+      loader-utils: 2.0.4
       postcss: 8.4.24
       postcss-modules-extract-imports: 3.0.0(postcss@8.4.24)
       postcss-modules-local-by-default: 4.0.3(postcss@8.4.24)
       postcss-modules-scope: 3.0.0(postcss@8.4.24)
       postcss-modules-values: 4.0.0(postcss@8.4.24)
       postcss-value-parser: 4.2.0
+      schema-utils: 3.3.0
       semver: 7.5.3
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
     dev: true
 
   /css.escape@1.5.1:
     resolution: {integrity: sha512-YUifsXXuknHlUsmlgyY0PKzgPOr7/FjCePfHNt0jxm83wHZi44VDMQ7/fGNkjY3/jV1MC+1CmZbaHzugyeRtpg==}
     dev: true
 
   /cssesc@3.0.0:
@@ -3358,42 +3320,42 @@
       '@esbuild/netbsd-x64': 0.17.19
       '@esbuild/openbsd-x64': 0.17.19
       '@esbuild/sunos-x64': 0.17.19
       '@esbuild/win32-arm64': 0.17.19
       '@esbuild/win32-ia32': 0.17.19
       '@esbuild/win32-x64': 0.17.19
 
-  /esbuild@0.18.6:
-    resolution: {integrity: sha512-5QgxWaAhU/tPBpvkxUmnFv2YINHuZzjbk0LeUUnC2i3aJHjfi5yR49lgKgF7cb98bclOp/kans8M5TGbGFfJlQ==}
+  /esbuild@0.18.10:
+    resolution: {integrity: sha512-33WKo67auOXzZHBY/9DTJRo7kIvfU12S+D4sp2wIz39N88MDIaCGyCwbW01RR70pK6Iya0I74lHEpyLfFqOHPA==}
     engines: {node: '>=12'}
     hasBin: true
     requiresBuild: true
     optionalDependencies:
-      '@esbuild/android-arm': 0.18.6
-      '@esbuild/android-arm64': 0.18.6
-      '@esbuild/android-x64': 0.18.6
-      '@esbuild/darwin-arm64': 0.18.6
-      '@esbuild/darwin-x64': 0.18.6
-      '@esbuild/freebsd-arm64': 0.18.6
-      '@esbuild/freebsd-x64': 0.18.6
-      '@esbuild/linux-arm': 0.18.6
-      '@esbuild/linux-arm64': 0.18.6
-      '@esbuild/linux-ia32': 0.18.6
-      '@esbuild/linux-loong64': 0.18.6
-      '@esbuild/linux-mips64el': 0.18.6
-      '@esbuild/linux-ppc64': 0.18.6
-      '@esbuild/linux-riscv64': 0.18.6
-      '@esbuild/linux-s390x': 0.18.6
-      '@esbuild/linux-x64': 0.18.6
-      '@esbuild/netbsd-x64': 0.18.6
-      '@esbuild/openbsd-x64': 0.18.6
-      '@esbuild/sunos-x64': 0.18.6
-      '@esbuild/win32-arm64': 0.18.6
-      '@esbuild/win32-ia32': 0.18.6
-      '@esbuild/win32-x64': 0.18.6
+      '@esbuild/android-arm': 0.18.10
+      '@esbuild/android-arm64': 0.18.10
+      '@esbuild/android-x64': 0.18.10
+      '@esbuild/darwin-arm64': 0.18.10
+      '@esbuild/darwin-x64': 0.18.10
+      '@esbuild/freebsd-arm64': 0.18.10
+      '@esbuild/freebsd-x64': 0.18.10
+      '@esbuild/linux-arm': 0.18.10
+      '@esbuild/linux-arm64': 0.18.10
+      '@esbuild/linux-ia32': 0.18.10
+      '@esbuild/linux-loong64': 0.18.10
+      '@esbuild/linux-mips64el': 0.18.10
+      '@esbuild/linux-ppc64': 0.18.10
+      '@esbuild/linux-riscv64': 0.18.10
+      '@esbuild/linux-s390x': 0.18.10
+      '@esbuild/linux-x64': 0.18.10
+      '@esbuild/netbsd-x64': 0.18.10
+      '@esbuild/openbsd-x64': 0.18.10
+      '@esbuild/sunos-x64': 0.18.10
+      '@esbuild/win32-arm64': 0.18.10
+      '@esbuild/win32-ia32': 0.18.10
+      '@esbuild/win32-x64': 0.18.10
     dev: true
 
   /escalade@3.1.1:
     resolution: {integrity: sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==}
     engines: {node: '>=6'}
 
   /escape-string-regexp@1.0.5:
@@ -3586,28 +3548,48 @@
 
   /fault@2.0.1:
     resolution: {integrity: sha512-WtySTkS4OKev5JtpHXnib4Gxiurzh5NCGvWrFaZ34m6JehfTUhKZvn9njTfw48t6JumVQOmrKqpmGcdwxnhqBQ==}
     dependencies:
       format: 0.2.2
     dev: false
 
+  /file-loader@6.0.0(webpack@5.88.0):
+    resolution: {integrity: sha512-/aMOAYEFXDdjG0wytpTL5YQLfZnnTmLNjn+AIrJ/6HVnTfDqLsVKUUwkDf4I4kgex36BvjuXEn/TX9B/1ESyqQ==}
+    engines: {node: '>= 10.13.0'}
+    peerDependencies:
+      webpack: ^4.0.0 || ^5.0.0
+    dependencies:
+      loader-utils: 2.0.4
+      schema-utils: 2.7.1
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+    dev: true
+
   /fill-range@7.0.1:
     resolution: {integrity: sha512-qOo9F+dMUmC2Lcb4BbVvnKJxTPjCm+RRpe4gDuGrzkL7mEVl/djYSu2OdQ2Pa302N4oqkSg9ir6jaLWJ2USVpQ==}
     engines: {node: '>=8'}
     dependencies:
       to-regex-range: 5.0.1
 
   /find-babel-config@2.0.0:
     resolution: {integrity: sha512-dOKT7jvF3hGzlW60Gc3ONox/0rRZ/tz7WCil0bqA1In/3I8f1BctpXahRnEKDySZqci7u+dqq93sZST9fOJpFw==}
     engines: {node: '>=16.0.0'}
     dependencies:
       json5: 2.2.3
       path-exists: 4.0.0
     dev: false
 
+  /find-cache-dir@3.3.2:
+    resolution: {integrity: sha512-wXZV5emFEjrridIgED11OoUKLxiYjAcqot/NJdAkOhlJ+vGzwhOAfcG5OX1jP+S0PcjEn8bdMJv+g2jwQ3Onig==}
+    engines: {node: '>=8'}
+    dependencies:
+      commondir: 1.0.1
+      make-dir: 3.1.0
+      pkg-dir: 4.2.0
+    dev: true
+
   /find-root@1.1.0:
     resolution: {integrity: sha512-NKfW6bec6GfKc0SGx1e07QZY9PE99u0Bft/0rzSD5k3sO/vwkVUpDUKVm5Gpp5Ue3YfShPFTX2070tDs5kB9Ng==}
     dev: true
 
   /find-up@3.0.0:
     resolution: {integrity: sha512-1yD6RmLI1XBfxugvORwlck6f75tYL+iR0jqwsOrOxMZyGYqUuDhJ0l4AXdO1iX/FTs9cBAMEk1gWSEx1kSbylg==}
     engines: {node: '>=6'}
@@ -3646,23 +3628,14 @@
     engines: {node: '>=0.4.x'}
     dev: false
 
   /fraction.js@4.2.0:
     resolution: {integrity: sha512-MhLuK+2gUcnZe8ZHlaaINnQLl0xRIGRfcGk2yl8xoQAfHrSsL3rYu6FCmBdkdbhc9EPlwyGHewaRsvwRMJtAlA==}
     dev: false
 
-  /fs-extra@10.1.0:
-    resolution: {integrity: sha512-oRXApq54ETRj4eMiFzGnHWGy+zo5raudjuxN0b8H7s/RU2oW0Wvsx9O0ACRN/kRq9E8Vu/ReskGB5o3ji+FzHQ==}
-    engines: {node: '>=12'}
-    dependencies:
-      graceful-fs: 4.2.11
-      jsonfile: 6.1.0
-      universalify: 2.0.0
-    dev: true
-
   /fs-extra@7.0.1:
     resolution: {integrity: sha512-YJDaCJZEnBmcbw13fvdAM9AwNOJwOzrE4pqMqBq5nFiEqXUqHwlK4B+3pUw6JNvfSPtX05xFHtYy/1ni01eGCw==}
     engines: {node: '>=6 <7 || >=8'}
     dependencies:
       graceful-fs: 4.2.11
       jsonfile: 4.0.0
       universalify: 0.1.2
@@ -3673,14 +3646,31 @@
     engines: {node: '>=6 <7 || >=8'}
     dependencies:
       graceful-fs: 4.2.11
       jsonfile: 4.0.0
       universalify: 0.1.2
     dev: true
 
+  /fs-extra@9.1.0:
+    resolution: {integrity: sha512-hcg3ZmepS30/7BSFqRvoo3DOMQu7IjqxO5nCDt+zM9XWjb33Wg7ziNT+Qvqbuc3+gWpzO02JubVyk2G4Zvo1OQ==}
+    engines: {node: '>=10'}
+    dependencies:
+      at-least-node: 1.0.0
+      graceful-fs: 4.2.11
+      jsonfile: 6.1.0
+      universalify: 2.0.0
+    dev: true
+
+  /fs-minipass@2.1.0:
+    resolution: {integrity: sha512-V/JgOLFCS+R6Vcq0slCuaeWEdNC3ouDlJMNIsacH2VtALiu9mV4LPrHc5cDl8k5aw6J8jwgWWpiTo5RYhmIzvg==}
+    engines: {node: '>= 8'}
+    dependencies:
+      minipass: 3.3.6
+    dev: true
+
   /fs.realpath@1.0.0:
     resolution: {integrity: sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==}
 
   /fsevents@2.3.2:
     resolution: {integrity: sha512-xiqMQR4xAeHTuB9uWm+fFRcIOgKBMiOBP+eXiyT7jsgVCq1bkVygt00oASowB7EdtpOHaaPgKt812P9ab+DDKA==}
     engines: {node: ^8.16.0 || ^10.6.0 || >=11.0.0}
     os: [darwin]
@@ -4065,19 +4055,28 @@
       pkg-dir: 4.2.0
       resolve-cwd: 3.0.0
     dev: true
 
   /import-meta-resolve@2.2.2:
     resolution: {integrity: sha512-f8KcQ1D80V7RnqVm+/lirO9zkOxjGxhaTC1IPrBGd3MEfNgmNG67tSUO9gTi2F3Blr2Az6g1vocaxzkVnWl9MA==}
 
+  /imurmurhash@0.1.4:
+    resolution: {integrity: sha512-JmXMZ6wuvDmLiHEml9ykzqO6lwFbof0GG4IkcGaENdCRDDmMVnny7s5HsIgHCbaq0w2MyPhDqkhTUgS2LU2PHA==}
+    engines: {node: '>=0.8.19'}
+    dev: true
+
   /indent-string@4.0.0:
     resolution: {integrity: sha512-EdDDZu4A2OyIK7Lr/2zG+w5jmbuk1DVBnEwREQvBzspBJkCEbRa8GxU1lghYcaGJCnRWibjDXlq779X1/y5xwg==}
     engines: {node: '>=8'}
     dev: true
 
+  /infer-owner@1.0.4:
+    resolution: {integrity: sha512-IClj+Xz94+d7irH5qRyfJonOdfTzuDaifE6ZPWfx0N0+/ATZCbuTPq2prFl526urkQd90WyUKIh1DfBQ2hMz9A==}
+    dev: true
+
   /inflight@1.0.6:
     resolution: {integrity: sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==}
     dependencies:
       once: 1.4.0
       wrappy: 1.0.2
 
   /inherits@2.0.4:
@@ -4092,17 +4091,17 @@
     engines: {node: '>= 0.4'}
     dependencies:
       get-intrinsic: 1.2.1
       has: 1.0.3
       side-channel: 1.0.4
     dev: true
 
-  /interpret@3.1.1:
-    resolution: {integrity: sha512-6xwYfHbajpoF0xLW+iwLkhwgvLoZDfjYfoFNu8ftMoXINzwuymNLd9u/KmwtdT2GbR+/Cz66otEGEVVUHX9QLQ==}
-    engines: {node: '>=10.13.0'}
+  /interpret@2.2.0:
+    resolution: {integrity: sha512-Ju0Bz/cEia55xDwUWEa8+olFpCiQoypjnQySseKtmjNrnps3P+xfpUmGr90T7yjlVJmOtybRvPXhKMbHr+fWnw==}
+    engines: {node: '>= 0.10'}
     dev: true
 
   /is-alphabetical@2.0.1:
     resolution: {integrity: sha512-FWyyY60MeTNyeSRpkM2Iry0G9hpr7/9kD40mD/cGQEuilcZYS4okz8SN2Q6rLCJ8gbCt6fN+rC+6tMGS99LaxQ==}
     dev: false
 
   /is-alphanumerical@2.0.1:
@@ -4341,14 +4340,23 @@
     resolution: {integrity: sha512-RHxMLp9lnKHGHRng9QFhRCMbYAcVpn69smSGcq3f36xjgVVWThj4qqLbTLlq7Ssj8B+fIQ1EuCEGI2lKsyQeIw==}
 
   /isobject@3.0.1:
     resolution: {integrity: sha512-WhB9zCku7EGTj/HQQRz5aUQEUeoQZH2bWcltRErOpymJ4boYE6wL9Tbr23krRPSZ+C5zqNSrSw+Cc7sZZ4b7vg==}
     engines: {node: '>=0.10.0'}
     dev: true
 
+  /jest-worker@26.6.2:
+    resolution: {integrity: sha512-KWYVV1c4i+jbMpaBC+U++4Va0cp8OisU185o73T1vo99hqi7w8tSJfUXYswwqqrjzwxa6KpRK54WhPvwf5w6PQ==}
+    engines: {node: '>= 10.13.0'}
+    dependencies:
+      '@types/node': 18.0.0
+      merge-stream: 2.0.0
+      supports-color: 7.2.0
+    dev: true
+
   /jest-worker@27.5.1:
     resolution: {integrity: sha512-7vuh85V5cdDofPyxn58nrPjBktZo0u9x1g8WtjQol+jZDaE+fhN+cIvTj11GndBnMnyfrUOG1sZQxCdjKh+DKg==}
     engines: {node: '>= 10.13.0'}
     dependencies:
       '@types/node': 18.0.0
       merge-stream: 2.0.0
       supports-color: 8.1.1
@@ -4391,16 +4399,19 @@
   /json-parse-even-better-errors@2.3.1:
     resolution: {integrity: sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==}
     dev: true
 
   /json-schema-traverse@0.4.1:
     resolution: {integrity: sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==}
 
-  /json-schema-traverse@1.0.0:
-    resolution: {integrity: sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==}
+  /json5@1.0.2:
+    resolution: {integrity: sha512-g1MWMLBiz8FKi1e4w0UyVL3w+iJceWAFBAaBnnGKOpNa5f8TLktkbre1+s6oICydWAm+HRUGTmI+//xv2hvXYA==}
+    hasBin: true
+    dependencies:
+      minimist: 1.2.8
     dev: true
 
   /json5@2.2.3:
     resolution: {integrity: sha512-XmOWe7eyHYH14cLdVPoyg+GOH3rYX++KpzrylJwSW98t3Nk+U8XOl8FWKOgwtzdb8lXGf6zYwDUzeHMWfxasyg==}
     engines: {node: '>=6'}
     hasBin: true
 
@@ -4441,15 +4452,15 @@
     peerDependencies:
       webpack: '*'
     peerDependenciesMeta:
       webpack:
         optional: true
     dependencies:
       '@types/webpack-sources': 0.1.9
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
       webpack-sources: 1.4.3
     dev: true
 
   /lilconfig@2.1.0:
     resolution: {integrity: sha512-utWOt/GHzuUxnLKxB6dk81RoOeoNeHgbrXiuGk4yyF5qlRz+iIVWu56E2fqGHFrXz0QNUhLB/8nKqvRH66JKGQ==}
     engines: {node: '>=10'}
     dev: false
@@ -4467,14 +4478,23 @@
       strip-bom: 3.0.0
 
   /loader-runner@4.3.0:
     resolution: {integrity: sha512-3R/1M+yS3j5ou80Me59j7F9IMs4PXs3VqRrm0TU3AbKPxlmpoY1TNscJV/oGJXo8qCatFGTfDbY6W6ipGOYXfg==}
     engines: {node: '>=6.11.5'}
     dev: true
 
+  /loader-utils@1.4.2:
+    resolution: {integrity: sha512-I5d00Pd/jwMD2QCduo657+YM/6L3KZu++pmX9VFncxaxvHcru9jx1lBaFft+r4Mt2jK0Yhp41XlRAihzPxHNCg==}
+    engines: {node: '>=4.0.0'}
+    dependencies:
+      big.js: 5.2.2
+      emojis-list: 3.0.0
+      json5: 1.0.2
+    dev: true
+
   /loader-utils@2.0.4:
     resolution: {integrity: sha512-xXqpXoINfFhgua9xiqD8fPFHgkoq1mmmpE92WlDbm9rNRd/EbRb+Gqf908T2DMfuHjjJlksiK2RbHVOdD/MqSw==}
     engines: {node: '>=8.9.0'}
     dependencies:
       big.js: 5.2.2
       emojis-list: 3.0.0
       json5: 2.2.3
@@ -4562,14 +4582,21 @@
   /magic-string@0.30.0:
     resolution: {integrity: sha512-LA+31JYDJLs82r2ScLrlz1GjSgu66ZV518eyWT+S8VhyQn/JL0u9MeBOvQMGYiPk1DBiSN9DDMOcXvigJZaViQ==}
     engines: {node: '>=12'}
     dependencies:
       '@jridgewell/sourcemap-codec': 1.4.15
     dev: true
 
+  /make-dir@3.1.0:
+    resolution: {integrity: sha512-g3FeP20LNwhALb/6Cz6Dd4F2ngze0jz7tbzrD2wAV+o9FeNHe4rL+yK2md0J/fiSf1sa1ADhXqi5+oVwOM/eGw==}
+    engines: {node: '>=8'}
+    dependencies:
+      semver: 6.3.0
+    dev: true
+
   /map-obj@1.0.1:
     resolution: {integrity: sha512-7N/q3lyZ+LVCp7PzuxrJr4KMbBE2hW7BT7YNia330OFxIf4d3r5zVpicP2650l7CPN6RM9zOJRl3NGpqSiw3Eg==}
     engines: {node: '>=0.10.0'}
     dev: true
 
   /map-obj@4.3.0:
     resolution: {integrity: sha512-hdN1wVrZbb29eBGiGjJbeP8JbKjq1urkHJ/LIP/NY48MZ1QVXUsQBV1G1zvYFHn1XE06cwjBsOI2K3Ulnj1YXQ==}
@@ -5144,27 +5171,24 @@
     engines: {node: '>=12'}
 
   /min-indent@1.0.1:
     resolution: {integrity: sha512-I9jwMn07Sy/IwOj3zVkVik2JTvgpaykDZEigL6Rx6N9LbMywwUSMtxET+7lVoDLLd3O3IXwJwvuuns8UB/HeAg==}
     engines: {node: '>=4'}
     dev: true
 
-  /mini-css-extract-plugin@2.7.6(webpack@5.88.0):
-    resolution: {integrity: sha512-Qk7HcgaPkGG6eD77mLvZS1nmxlao3j+9PkrT9Uc7HAE1id3F41+DdBRYRYkbyfNRGzm8/YWtzhw7nVPmwhqTQw==}
-    engines: {node: '>= 12.13.0'}
+  /mini-css-extract-plugin@1.3.9(webpack@5.88.0):
+    resolution: {integrity: sha512-Ac4s+xhVbqlyhXS5J/Vh/QXUz3ycXlCqoCPpg0vdfhsIBH9eg/It/9L1r1XhSCH737M1lqcWnMuWL13zcygn5A==}
+    engines: {node: '>= 10.13.0'}
     peerDependencies:
-      webpack: ^5.0.0
+      webpack: ^4.4.0 || ^5.0.0
     dependencies:
-      schema-utils: 4.2.0
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
-    dev: true
-
-  /mini-svg-data-uri@1.4.4:
-    resolution: {integrity: sha512-r9deDe9p5FJUPZAk3A59wGH7Ii9YrjjWw0jmw/liSbHl2CHiyXj6FcDXDu2K3TjVAXqiJdaw3xxwlZZr9E6nHg==}
-    hasBin: true
+      loader-utils: 2.0.4
+      schema-utils: 3.3.0
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack-sources: 1.4.3
     dev: true
 
   /minimatch@3.1.2:
     resolution: {integrity: sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==}
     dependencies:
       brace-expansion: 1.1.11
 
@@ -5183,19 +5207,66 @@
       is-plain-obj: 1.1.0
       kind-of: 6.0.3
     dev: true
 
   /minimist@1.2.8:
     resolution: {integrity: sha512-2yyAR8qBkN3YuheJanUpWC5U3bb5osDywNB8RzDVlDwDHbocAJveqqj1u8+SVD7jkWT4yvsHCpWqqWqAxb0zCA==}
 
+  /minipass-collect@1.0.2:
+    resolution: {integrity: sha512-6T6lH0H8OG9kITm/Jm6tdooIbogG9e0tLgpY6mphXSm/A9u8Nq1ryBG+Qspiub9LjWlBPsPS3tWQ/Botq4FdxA==}
+    engines: {node: '>= 8'}
+    dependencies:
+      minipass: 3.3.6
+    dev: true
+
+  /minipass-flush@1.0.5:
+    resolution: {integrity: sha512-JmQSYYpPUqX5Jyn1mXaRwOda1uQ8HP5KAT/oDSLCzt1BYRhQU0/hDtsB1ufZfEEzMZ9aAVmsBw8+FWsIXlClWw==}
+    engines: {node: '>= 8'}
+    dependencies:
+      minipass: 3.3.6
+    dev: true
+
+  /minipass-pipeline@1.2.4:
+    resolution: {integrity: sha512-xuIq7cIOt09RPRJ19gdi4b+RiNvDFYe5JH+ggNvBqGqpQXcru3PcRmOZuHBKWK1Txf9+cQ+HMVN4d6z46LZP7A==}
+    engines: {node: '>=8'}
+    dependencies:
+      minipass: 3.3.6
+    dev: true
+
+  /minipass@3.3.6:
+    resolution: {integrity: sha512-DxiNidxSEK+tHG6zOIklvNOwm3hvCrbUrdtzY74U6HKTJxvIDfOUL5W5P2Ghd3DTkhhKPYGqeNUIh5qcM4YBfw==}
+    engines: {node: '>=8'}
+    dependencies:
+      yallist: 4.0.0
+    dev: true
+
+  /minipass@5.0.0:
+    resolution: {integrity: sha512-3FnjYuehv9k6ovOEbyOswadCDPX1piCfhV8ncmYtHOjuPwylVWsghTLo7rabjC3Rx5xD4HDx8Wm1xnMF7S5qFQ==}
+    engines: {node: '>=8'}
+    dev: true
+
+  /minizlib@2.1.2:
+    resolution: {integrity: sha512-bAxsR8BVfj60DWXHE3u30oHzfl4G7khkSuPW+qvpd7jFRHm7dLxOjUk1EHACJ/hxLY8phGJ0YhYHZo7jil7Qdg==}
+    engines: {node: '>= 8'}
+    dependencies:
+      minipass: 3.3.6
+      yallist: 4.0.0
+    dev: true
+
   /mixme@0.5.9:
     resolution: {integrity: sha512-VC5fg6ySUscaWUpI4gxCBTQMH2RdUpNrk+MsbpCYtIvf9SBJdiUey4qE7BXviJsJR4nDQxCZ+3yaYNW3guz/Pw==}
     engines: {node: '>= 8.0.0'}
     dev: true
 
+  /mkdirp@1.0.4:
+    resolution: {integrity: sha512-vVqVZQyf3WLx2Shd0qJ9xuvqgAyKPLAiqITEtqW0oIUjzo3PePDd6fW9iFz30ef7Ysp/oiWqbhszeGWW2T6Gzw==}
+    engines: {node: '>=10'}
+    hasBin: true
+    dev: true
+
   /mlly@1.4.0:
     resolution: {integrity: sha512-ua8PAThnTwpprIaU47EPeZ/bPUVp2QYBbWMphUQpVdBI3Lgqzm5KZQ45Agm3YJedHXaIHl6pBGabaLSUPPSptg==}
     dependencies:
       acorn: 8.9.0
       pathe: 1.1.1
       pkg-types: 1.0.3
       ufo: 1.1.2
@@ -5400,14 +5471,21 @@
       p-limit: 3.1.0
 
   /p-map@2.1.0:
     resolution: {integrity: sha512-y3b8Kpd8OAN444hxfBbFfj1FY/RjtTd8tzYwhUqNYXx0fXx2iX4maP4Qr6qhIKbQXI02wTLAda4fYUbDagTUFw==}
     engines: {node: '>=6'}
     dev: true
 
+  /p-map@4.0.0:
+    resolution: {integrity: sha512-/bjOqmgETBYB5BoEeGVea8dmvHb2m9GLy1E9W43yeyfP6QQCZGFNa+XRceJEuDB6zqr+gKpIAmlLebMpykw/MQ==}
+    engines: {node: '>=10'}
+    dependencies:
+      aggregate-error: 3.1.0
+    dev: true
+
   /p-try@2.2.0:
     resolution: {integrity: sha512-R4nPAVTAU0B9D35/Gk3uJf/7XYbQcyohSKdvAxIRSNghFl4e71hVoGnBNQz9cWaXxO2I10KTC+3jMdvvoKw6dQ==}
     engines: {node: '>=6'}
 
   /parse-entities@4.0.1:
     resolution: {integrity: sha512-SWzvYcSJh4d/SGLIOQfZ/CoNv6BTlI6YEQ7Nj82oDVnRpwe/Z/F1EMx42x3JAOwGBlCjeCH0BRJQbQ/opHL17w==}
     dependencies:
@@ -5721,14 +5799,23 @@
     engines: {node: '>=6'}
 
   /process@0.11.10:
     resolution: {integrity: sha512-cdGef/drWFoydD1JsMzuFf8100nZl+GT+yacc2bEced5f9Rjk4z+WtFUTBu9PhOi9j/jfmBPu0mMEY4wIdAF8A==}
     engines: {node: '>= 0.6.0'}
     dev: true
 
+  /promise-inflight@1.0.1:
+    resolution: {integrity: sha512-6zWPyEOFaQBJYcGMHBKTKJ3u6TBsnMFOIZSa6ce1e/ZrrsOlnHRHbabMjLiBYKp+n44X9eUI6VUPaukCXHuG4g==}
+    peerDependencies:
+      bluebird: '*'
+    peerDependenciesMeta:
+      bluebird:
+        optional: true
+    dev: true
+
   /prompts@2.4.2:
     resolution: {integrity: sha512-NxNv/kLguCA7p3jE8oL2aEBsrJWgAakBpgmgK6lpPWV+WuOmY6r2/zbAVnP+T8bQlA0nzHXSJSJW0Hq7ylaD2Q==}
     engines: {node: '>= 6'}
     dependencies:
       kleur: 3.0.3
       sisteransi: 1.0.5
 
@@ -5756,14 +5843,25 @@
 
   /randombytes@2.1.0:
     resolution: {integrity: sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==}
     dependencies:
       safe-buffer: 5.2.1
     dev: true
 
+  /raw-loader@4.0.2(webpack@5.88.0):
+    resolution: {integrity: sha512-ZnScIV3ag9A4wPX/ZayxL/jZH+euYb6FcUinPcgiQW0+UBtEv0O6Q3lGd3cqJ+GHH+rksEv3Pj99oxJ3u3VIKA==}
+    engines: {node: '>= 10.13.0'}
+    peerDependencies:
+      webpack: ^4.0.0 || ^5.0.0
+    dependencies:
+      loader-utils: 2.0.4
+      schema-utils: 3.3.0
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+    dev: true
+
   /react-dom@18.2.0(react@18.2.0):
     resolution: {integrity: sha512-6IMTriUmvsjHUjNtEDudZfuDQUoWXVxKHhlEGSk81n4YFS+r/Kl99wXiwlVXtPBtJenozv2P+hxDsw9eA7Xo6g==}
     peerDependencies:
       react: ^18.2.0
     dependencies:
       loose-envify: 1.4.0
       react: 18.2.0
@@ -5826,17 +5924,17 @@
 
   /readdirp@3.6.0:
     resolution: {integrity: sha512-hOS089on8RduqdbhvQ5Z37A0ESjsqz6qnRcffsMU3495FuTdqSm+7bhJ29JvIOsBDEEnan5DPu9t3To9VRlMzA==}
     engines: {node: '>=8.10.0'}
     dependencies:
       picomatch: 2.3.1
 
-  /rechoir@0.8.0:
-    resolution: {integrity: sha512-/vxpCXddiX8NGfGO/mTafwjq4aFa/71pvamip0++IQk3zG8cbCj0fifNPrjjF1XMXUne91jL9OoxmdykoEtifQ==}
-    engines: {node: '>= 10.13.0'}
+  /rechoir@0.7.1:
+    resolution: {integrity: sha512-/njmZ8s1wVeR6pjTZ+0nCnv8SpZNRMT2D1RLOJQESlYFDBvwpTA4KWJpZ+sBJ4+vhjILRcK7JIFdGCdxEAAitg==}
+    engines: {node: '>= 0.10'}
     dependencies:
       resolve: 1.22.2
     dev: true
 
   /redent@3.0.0:
     resolution: {integrity: sha512-6tDA8g98We0zd0GvVeMT9arEOnTw9qM03L9cJXaCjrip1OO764RDBLBfrB4cwzNGDj5OA5ioymC9GkizgWJDUg==}
     engines: {node: '>=8'}
@@ -5942,19 +6040,14 @@
       unist-util-visit: 4.1.2
 
   /require-directory@2.1.1:
     resolution: {integrity: sha512-fGxEI7+wsG9xrvdjsrlmL22OMTTiHRwAMroiEeMgq8gzoLC/PQr7RsRDSTLUg/bZAZtF+TVIkHc6/4RIKrui+Q==}
     engines: {node: '>=0.10.0'}
     dev: true
 
-  /require-from-string@2.0.2:
-    resolution: {integrity: sha512-Xf0nWe6RseziFMu+Ap9biiUbmplq6S9/p+7w7YXP/JBHhrUDDUhwa+vANyubuqfZWTveU//DYVGsDG7RKL/vEw==}
-    engines: {node: '>=0.10.0'}
-    dev: true
-
   /require-main-filename@2.0.0:
     resolution: {integrity: sha512-NKN5kMDylKuldxYLSUfrbo5Tuzh4hd+2E8NPPX02mZtn1VuREQToYe/ZdlJy+J3uCpfaiGF05e7B8W0iXbQHmg==}
     dev: true
 
   /requires-port@1.0.0:
     resolution: {integrity: sha512-KigOCHcocU3XODJxsu8i/j8T9tzT4adHiecwORRQ0ZZFcp7ahwXuRU1m+yuO90C5ZUyGeGfocHDI14M3L3yDAQ==}
 
@@ -6020,14 +6113,21 @@
       retext-stringify: 3.1.0
       unified: 10.1.2
 
   /reusify@1.0.4:
     resolution: {integrity: sha512-U9nH88a3fc/ekCF1l0/UP1IosiuIjyTh7hBvXVMHYgVcfGvt897Xguj2UOLDeI5BG2m7/uwyaLVT6fbtCwTyzw==}
     engines: {iojs: '>=1.0.0', node: '>=0.10.0'}
 
+  /rimraf@3.0.2:
+    resolution: {integrity: sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==}
+    hasBin: true
+    dependencies:
+      glob: 7.1.7
+    dev: true
+
   /rollup@3.25.1:
     resolution: {integrity: sha512-tywOR+rwIt5m2ZAWSe5AIJcTat8vGlnPFAv15ycCrw33t6iFsXZ6mzHVFh2psSjxQPmI+xgzMZZizUAukBI4aQ==}
     engines: {node: '>=14.18.0', npm: '>=8.0.0'}
     hasBin: true
     optionalDependencies:
       fsevents: 2.3.2
 
@@ -6102,24 +6202,14 @@
     engines: {node: '>= 10.13.0'}
     dependencies:
       '@types/json-schema': 7.0.12
       ajv: 6.12.6
       ajv-keywords: 3.5.2(ajv@6.12.6)
     dev: true
 
-  /schema-utils@4.2.0:
-    resolution: {integrity: sha512-L0jRsrPpjdckP3oPug3/VxNKt2trR8TcabrM6FOAAlvC/9Phcmm+cuAgTlxBqdBR1WJx7Naj9WHw+aOmheSVbw==}
-    engines: {node: '>= 12.13.0'}
-    dependencies:
-      '@types/json-schema': 7.0.12
-      ajv: 8.12.0
-      ajv-formats: 2.1.1(ajv@8.12.0)
-      ajv-keywords: 5.1.0(ajv@8.12.0)
-    dev: true
-
   /section-matter@1.0.0:
     resolution: {integrity: sha512-vfD3pmTzGpufjScBh50YHKzEu2lxBWhVEHsNGoEXmCmn2hKGfeNLYMzCJpe8cD7gqX7TJluOVpBkAequ6dgMmA==}
     engines: {node: '>=4'}
     dependencies:
       extend-shallow: 2.0.1
       kind-of: 6.0.3
 
@@ -6135,14 +6225,20 @@
   /semver@7.5.3:
     resolution: {integrity: sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==}
     engines: {node: '>=10'}
     hasBin: true
     dependencies:
       lru-cache: 6.0.0
 
+  /serialize-javascript@5.0.1:
+    resolution: {integrity: sha512-SaaNal9imEO737H2c05Og0/8LUXG7EnsZyMa8MzkmuHoELfT6txuj0cMqRj6zfPKnmQ1yasR4PCJc8x+M4JSPA==}
+    dependencies:
+      randombytes: 2.1.0
+    dev: true
+
   /serialize-javascript@6.0.1:
     resolution: {integrity: sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==}
     dependencies:
       randombytes: 2.1.0
     dev: true
 
   /server-destroy@1.0.1:
@@ -6244,15 +6340,15 @@
       webpack: ^4.0.0 || ^5.0.0
     dependencies:
       data-urls: 2.0.0
       iconv-lite: 0.6.3
       loader-utils: 2.0.4
       schema-utils: 2.7.1
       source-map: 0.6.1
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
     dev: true
 
   /source-map-support@0.5.21:
     resolution: {integrity: sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==}
     dependencies:
       buffer-from: 1.1.2
       source-map: 0.6.1
@@ -6299,14 +6395,21 @@
   /spdx-license-ids@3.0.13:
     resolution: {integrity: sha512-XkD+zwiqXHikFZm4AX/7JSCXA98U5Db4AFd5XUg/+9UNtnH75+Z9KxtpYiJZx36mUDVOwH83pl7yvCer6ewM3w==}
     dev: true
 
   /sprintf-js@1.0.3:
     resolution: {integrity: sha512-D9cPgkvLlV3t3IzL0D0YLvGA9Ahk4PcvVwUbN0dSGr1aP0Nrt4AEnTUbuGvquEC0mA64Gqt1fzirlRs5ibXx8g==}
 
+  /ssri@8.0.1:
+    resolution: {integrity: sha512-97qShzy1AiyxvPNIkLWoGua7xoQzzPjQ0HAH4B0rWKo7SZ6USuPcrUiAFrws0UH8RrbWmgq3LMTObhPIHbbBeQ==}
+    engines: {node: '>= 8'}
+    dependencies:
+      minipass: 3.3.6
+    dev: true
+
   /stackback@0.0.2:
     resolution: {integrity: sha512-1XMJE5fQo1jGH6Y/7ebnwPOBEkIEnT4QF32d5R1+VXdXveM0IBMJt8zfaxX1P3QhVwrYe+576+jkANtSS2mBbw==}
     dev: true
 
   /std-env@3.3.3:
     resolution: {integrity: sha512-Rz6yejtVyWnVjC1RFvNmYL10kgjC49EOghxWn0RFqlCHGFpQx+Xe7yW3I4ceK1SGrWIGMjD5Kbue8W/udkbMJg==}
     dev: true
@@ -6420,21 +6523,23 @@
 
   /strip-literal@1.0.1:
     resolution: {integrity: sha512-QZTsipNpa2Ppr6v1AmJHESqJ3Uz247MUS0OjrnnZjFAvEoWqxuyFuXn2xLgMtRnijJShAa1HL0gtJyUs7u7n3Q==}
     dependencies:
       acorn: 8.9.0
     dev: true
 
-  /style-loader@3.3.3(webpack@5.88.0):
-    resolution: {integrity: sha512-53BiGLXAcll9maCYtZi2RCQZKa8NQQai5C4horqKyRmHj9H7QmcUyucrH+4KW/gBQbXM2AsB0axoEcFZPlfPcw==}
-    engines: {node: '>= 12.13.0'}
+  /style-loader@2.0.0(webpack@5.88.0):
+    resolution: {integrity: sha512-Z0gYUJmzZ6ZdRUqpg1r8GsaFKypE+3xAzuFeMuoHgjc9KZv3wMyCRjQIWEbhoFSq7+7yoHXySDJyyWQaPajeiQ==}
+    engines: {node: '>= 10.13.0'}
     peerDependencies:
-      webpack: ^5.0.0
+      webpack: ^4.0.0 || ^5.0.0
     dependencies:
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+      loader-utils: 2.0.4
+      schema-utils: 3.3.0
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
     dev: true
 
   /style-to-object@0.4.1:
     resolution: {integrity: sha512-HFpbb5gr2ypci7Qw+IOhnP2zOU7e77b+rzM+wTzXzfi1PrtBCX0E7Pk4wL4iTLnhzZ+JgEGAhX81ebTg/aYjQw==}
     dependencies:
       inline-style-parser: 0.1.1
     dev: false
@@ -6482,14 +6587,24 @@
     dependencies:
       has-package-exports: 1.3.0
 
   /supports-preserve-symlinks-flag@1.0.0:
     resolution: {integrity: sha512-ot0WnXS9fgdkgIcePe6RHNk1WA8+muPa6cSjeR3V8K27q9BB1rTE3R1p7Hv0z1ZyAc8s6Vvv8DIyWf681MAt0w==}
     engines: {node: '>= 0.4'}
 
+  /svg-url-loader@6.0.0(webpack@5.88.0):
+    resolution: {integrity: sha512-Qr5SCKxyxKcRnvnVrO3iQj9EX/v40UiGEMshgegzV7vpo3yc+HexELOdtWcA3MKjL8IyZZ1zOdcILmDEa/8JJQ==}
+    peerDependencies:
+      webpack: ^4.0.0 || ^5.0.0
+    dependencies:
+      file-loader: 6.0.0(webpack@5.88.0)
+      loader-utils: 2.0.4
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+    dev: true
+
   /synckit@0.8.5:
     resolution: {integrity: sha512-L1dapNV6vu2s/4Sputv8xGsCdAVlb5nRDMFU/E27D44l5U6cw1g0dGd45uLc+OXjNMmF4ntiMdCimzcjFKQI8Q==}
     engines: {node: ^14.18.0 || >=16.0.0}
     dependencies:
       '@pkgr/utils': 2.4.1
       tslib: 2.5.3
 
@@ -6526,20 +6641,52 @@
     dev: false
 
   /tapable@2.2.1:
     resolution: {integrity: sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==}
     engines: {node: '>=6'}
     dev: true
 
+  /tar@6.1.15:
+    resolution: {integrity: sha512-/zKt9UyngnxIT/EAGYuxaMYgOIJiP81ab9ZfkILq4oNLPFX50qyYmu7jRj9qeXoxmJHjGlbH0+cm2uy1WCs10A==}
+    engines: {node: '>=10'}
+    dependencies:
+      chownr: 2.0.0
+      fs-minipass: 2.1.0
+      minipass: 5.0.0
+      minizlib: 2.1.2
+      mkdirp: 1.0.4
+      yallist: 4.0.0
+    dev: true
+
   /term-size@2.2.1:
     resolution: {integrity: sha512-wK0Ri4fOGjv/XPy8SBHZChl8CM7uMc5VML7SqiQ0zG7+J5Vr+RMQDoHa2CNT6KHUnTGIXH34UDMkPzAUyapBZg==}
     engines: {node: '>=8'}
     dev: true
 
-  /terser-webpack-plugin@5.3.9(esbuild@0.18.6)(webpack@5.88.0):
+  /terser-webpack-plugin@4.2.3(webpack@5.88.0):
+    resolution: {integrity: sha512-jTgXh40RnvOrLQNgIkwEKnQ8rmHjHK4u+6UBEi+W+FPmvb+uo+chJXntKe7/3lW5mNysgSWD60KyesnhW8D6MQ==}
+    engines: {node: '>= 10.13.0'}
+    peerDependencies:
+      webpack: ^4.0.0 || ^5.0.0
+    dependencies:
+      cacache: 15.3.0
+      find-cache-dir: 3.3.2
+      jest-worker: 26.6.2
+      p-limit: 3.1.0
+      schema-utils: 3.3.0
+      serialize-javascript: 5.0.1
+      source-map: 0.6.1
+      terser: 5.18.1
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack-sources: 1.4.3
+    transitivePeerDependencies:
+      - bluebird
+    dev: true
+
+  /terser-webpack-plugin@5.3.9(esbuild@0.18.10)(webpack@5.88.0):
     resolution: {integrity: sha512-ZuXsqE07EcggTWQjXUj+Aot/OMcD0bMKGgF63f7UxYcu5/AJF53aIpK1YoP5xR9l6s/Hy2b+t1AM0bLNPRuhwA==}
     engines: {node: '>= 10.13.0'}
     peerDependencies:
       '@swc/core': '*'
       esbuild: '*'
       uglify-js: '*'
       webpack: ^5.1.0
@@ -6548,20 +6695,20 @@
         optional: true
       esbuild:
         optional: true
       uglify-js:
         optional: true
     dependencies:
       '@jridgewell/trace-mapping': 0.3.18
-      esbuild: 0.18.6
+      esbuild: 0.18.10
       jest-worker: 27.5.1
       schema-utils: 3.3.0
       serialize-javascript: 6.0.1
       terser: 5.18.1
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
     dev: true
 
   /terser@5.18.1:
     resolution: {integrity: sha512-j1n0Ao919h/Ai5r43VAnfV/7azUYW43GPxK7qSATzrsERfW7+y2QW9Cp9ufnRF5CQUWbnLSo7UJokSWCqg4tsQ==}
     engines: {node: '>=10'}
     hasBin: true
     dependencies:
@@ -6620,14 +6767,20 @@
 
   /to-regex-range@5.0.1:
     resolution: {integrity: sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==}
     engines: {node: '>=8.0'}
     dependencies:
       is-number: 7.0.0
 
+  /to-string-loader@1.2.0:
+    resolution: {integrity: sha512-KsWUL8FccgBW9FPFm4vYoQbOOcO5m6hKOGYoXjbseD9/4Ft+ravXN5jolQ9kTKYcK4zPt1j+khx97GPGnVoi6A==}
+    dependencies:
+      loader-utils: 1.4.2
+    dev: true
+
   /tr46@0.0.3:
     resolution: {integrity: sha512-N3WMsuqV66lT30CrXNbEjx4GEwlow3v6rr4mCcv6prnfwhS01rkgyFdjPNBYd9br7LpXV1+Emh01fHnq2Gdgrw==}
 
   /tr46@2.1.0:
     resolution: {integrity: sha512-15Ih7phfcdP5YxqiB+iDtLoaTz4Nd35+IiAv0kQ5FNKHzXgdWqPoTIqEDDJmXceQt4JZk6lVPT8lnDlPpGDppw==}
     engines: {node: '>=8'}
     dependencies:
@@ -6744,14 +6897,26 @@
       bail: 2.0.2
       extend: 3.0.2
       is-buffer: 2.0.5
       is-plain-obj: 4.1.0
       trough: 2.1.0
       vfile: 5.3.7
 
+  /unique-filename@1.1.1:
+    resolution: {integrity: sha512-Vmp0jIp2ln35UTXuryvjzkjGdRyf9b2lTXuSYUiPmzRcl3FDtYqAwOnTJkAngD9SWhnoJzDbTKwaOrZ+STtxNQ==}
+    dependencies:
+      unique-slug: 2.0.2
+    dev: true
+
+  /unique-slug@2.0.2:
+    resolution: {integrity: sha512-zoWr9ObaxALD3DOPfjPSqxt4fnZiWblxHIgeWqW8x7UqDzEtHEQLzji2cuJYQFCU6KmoJikOYAZlrTHHebjx2w==}
+    dependencies:
+      imurmurhash: 0.1.4
+    dev: true
+
   /unist-util-generated@2.0.1:
     resolution: {integrity: sha512-qF72kLmPxAw0oN2fwpWIqbXAVyEqUzDHMsbtPvOudIlUzXYFIeQIuxXQCRCFh22B7cixvU0MG7m3MW8FTq/S+A==}
 
   /unist-util-is@5.2.1:
     resolution: {integrity: sha512-u9njyyfEh43npf1M+yGKDGVPbY/JWEemg5nH05ncKPfi+kBbKBJoTdsogMu33uhytuLlv9y0O7GH7fEdwLdLQw==}
     dependencies:
       '@types/unist': 2.0.6
@@ -6828,14 +6993,31 @@
       picocolors: 1.0.0
 
   /uri-js@4.4.1:
     resolution: {integrity: sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==}
     dependencies:
       punycode: 2.3.0
 
+  /url-loader@4.1.1(file-loader@6.0.0)(webpack@5.88.0):
+    resolution: {integrity: sha512-3BTV812+AVHHOJQO8O5MkWgZ5aosP7GnROJwvzLS9hWDj00lZ6Z0wNak423Lp9PBZN05N+Jk/N5Si8jRAlGyWA==}
+    engines: {node: '>= 10.13.0'}
+    peerDependencies:
+      file-loader: '*'
+      webpack: ^4.0.0 || ^5.0.0
+    peerDependenciesMeta:
+      file-loader:
+        optional: true
+    dependencies:
+      file-loader: 6.0.0(webpack@5.88.0)
+      loader-utils: 2.0.4
+      mime-types: 2.1.35
+      schema-utils: 3.3.0
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+    dev: true
+
   /url-parse@1.4.7:
     resolution: {integrity: sha512-d3uaVyzDB9tQoSXFvuSUNFibTd9zxd2bkVrDRvF5TmvWWQwqE4lgYJ5m+x1DbecWkw+LK4RNl2CU1hHuOKPVlg==}
     dependencies:
       querystringify: 2.2.0
       requires-port: 1.0.0
     dev: false
 
@@ -7090,44 +7272,46 @@
     dev: true
 
   /webidl-conversions@7.0.0:
     resolution: {integrity: sha512-VwddBukDzu71offAQR975unBIGqfKZpM+8ZX6ySk8nYhVoo5CYaZyzt3YBvYtRtO+aoGlqxPg/B87NGVZ/fu6g==}
     engines: {node: '>=12'}
     dev: true
 
-  /webpack-cli@5.1.4(webpack@5.88.0):
-    resolution: {integrity: sha512-pIDJHIEI9LR0yxHXQ+Qh95k2EvXpWzZ5l+d+jIo+RdSm9MiHfzazIxwwni/p7+x4eJZuvG1AJwgC4TNQ7NRgsg==}
-    engines: {node: '>=14.15.0'}
+  /webpack-cli@4.10.0(webpack@5.88.0):
+    resolution: {integrity: sha512-NLhDfH/h4O6UOy+0LSso42xvYypClINuMNBVVzX4vX98TmTaTUxwRbXdhucbFMd2qLaCTcLq/PdYrvi8onw90w==}
+    engines: {node: '>=10.13.0'}
     hasBin: true
     peerDependencies:
       '@webpack-cli/generators': '*'
-      webpack: 5.x.x
+      '@webpack-cli/migrate': '*'
+      webpack: 4.x.x || 5.x.x
       webpack-bundle-analyzer: '*'
       webpack-dev-server: '*'
     peerDependenciesMeta:
       '@webpack-cli/generators':
         optional: true
+      '@webpack-cli/migrate':
+        optional: true
       webpack-bundle-analyzer:
         optional: true
       webpack-dev-server:
         optional: true
     dependencies:
       '@discoveryjs/json-ext': 0.5.7
-      '@webpack-cli/configtest': 2.1.1(webpack-cli@5.1.4)(webpack@5.88.0)
-      '@webpack-cli/info': 2.0.2(webpack-cli@5.1.4)(webpack@5.88.0)
-      '@webpack-cli/serve': 2.0.5(webpack-cli@5.1.4)(webpack@5.88.0)
+      '@webpack-cli/configtest': 1.2.0(webpack-cli@4.10.0)(webpack@5.88.0)
+      '@webpack-cli/info': 1.5.0(webpack-cli@4.10.0)
+      '@webpack-cli/serve': 1.7.0(webpack-cli@4.10.0)
       colorette: 2.0.20
-      commander: 10.0.1
+      commander: 7.2.0
       cross-spawn: 7.0.3
-      envinfo: 7.9.0
       fastest-levenshtein: 1.0.16
       import-local: 3.1.0
-      interpret: 3.1.1
-      rechoir: 0.8.0
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+      interpret: 2.2.0
+      rechoir: 0.7.1
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
       webpack-merge: 5.9.0
     dev: true
 
   /webpack-merge@5.9.0:
     resolution: {integrity: sha512-6NbRQw4+Sy50vYNTw7EyOn41OZItPiXB8GNv3INSoe3PSFaHJEz3SHTrYVaRm2LilNGnFUzh0FAwqPEmU/CwDg==}
     engines: {node: '>=10.0.0'}
     dependencies:
@@ -7143,15 +7327,15 @@
     dev: true
 
   /webpack-sources@3.2.3:
     resolution: {integrity: sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==}
     engines: {node: '>=10.13.0'}
     dev: true
 
-  /webpack@5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4):
+  /webpack@5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0):
     resolution: {integrity: sha512-O3jDhG5e44qIBSi/P6KpcCcH7HD+nYIHVBhdWFxcLOcIGN8zGo5nqF3BjyNCxIh4p1vFdNnreZv2h2KkoAw3lw==}
     engines: {node: '>=10.13.0'}
     hasBin: true
     peerDependencies:
       webpack-cli: '*'
     peerDependenciesMeta:
       webpack-cli:
@@ -7174,17 +7358,17 @@
       graceful-fs: 4.2.11
       json-parse-even-better-errors: 2.3.1
       loader-runner: 4.3.0
       mime-types: 2.1.35
       neo-async: 2.6.2
       schema-utils: 3.3.0
       tapable: 2.2.1
-      terser-webpack-plugin: 5.3.9(esbuild@0.18.6)(webpack@5.88.0)
+      terser-webpack-plugin: 5.3.9(esbuild@0.18.10)(webpack@5.88.0)
       watchpack: 2.4.0
-      webpack-cli: 5.1.4(webpack@5.88.0)
+      webpack-cli: 4.10.0(webpack@5.88.0)
       webpack-sources: 3.2.3
     transitivePeerDependencies:
       - '@swc/core'
       - esbuild
       - uglify-js
     dev: true
 
@@ -7298,15 +7482,15 @@
     resolution: {integrity: sha512-XQyQkIFeRVC7f7uRhFdNMe/iJOdO6zxAaR3EWbDp45v3mDhrTi+++oswKNxShUNjPC/1xUp5DB29YKLhFo129g==}
     engines: {node: '>= 10.13.0'}
     peerDependencies:
       webpack: ^4.0.0 || ^5.0.0
     dependencies:
       loader-utils: 2.0.4
       schema-utils: 3.3.0
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
     dev: true
 
   /wrap-ansi@6.2.0:
     resolution: {integrity: sha512-r6lPcBGxZXlIcymEu7InxDMhdW0KDxpLgoFLcguasxCaJ/SOIZwINatK9KY/tf+ZrlywOKU0UDj3ATXUBfxJXA==}
     engines: {node: '>=8'}
     dependencies:
       ansi-styles: 4.3.0
```

### Comparing `anywidget-0.6.0/anywidget/_descriptor.py` & `anywidget-0.6.1/anywidget/_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/anywidget/_file_contents.py` & `anywidget-0.6.1/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/anywidget/_protocols.py` & `anywidget-0.6.1/anywidget/_protocols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Literal, Protocol, Sequence
+from typing import TYPE_CHECKING, Sequence
 
-from typing_extensions import TypedDict
+from typing_extensions import Literal, Protocol, TypedDict
 
 if TYPE_CHECKING:
     from ._descriptor import MimeBundleDescriptor
 
 
 class UpdateData(TypedDict):
     method: Literal["update"]
```

### Comparing `anywidget-0.6.0/anywidget/_util.py` & `anywidget-0.6.1/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/anywidget/experimental.py` & `anywidget-0.6.1/anywidget/experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/anywidget/widget.py` & `anywidget-0.6.1/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/anywidget/labextension/package.json` & `anywidget-0.6.1/anywidget/labextension/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9507211538461539%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^3.6.5'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.2cf77409ad03a77cbd09.js'}}",*

 * * "'version'": "'0.6.1'"}*

```diff
@@ -3,15 +3,15 @@
     "dependencies": {
         "@anywidget/types": "workspace:~",
         "@anywidget/vite": "workspace:~",
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6"
     },
     "devDependencies": {
         "@jupyter-widgets/base-manager": "^1.0.5",
-        "@jupyterlab/builder": "^4.0.2"
+        "@jupyterlab/builder": "^3.6.5"
     },
     "exports": {
         ".": "./dist/index.js",
         "./types": {
             "import": "./dist/types.mjs",
             "require": "./dist/types.cjs",
             "types": "./dist/types.d.ts"
@@ -23,15 +23,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.cba6b4061725caaf22a8.js"
+            "load": "static/remoteEntry.2cf77409ad03a77cbd09.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -45,9 +45,9 @@
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs",
         "typecheck": "tsc --noEmit"
     },
     "type": "module",
-    "version": "0.6.0"
+    "version": "0.6.1"
 }
```

### Comparing `anywidget-0.6.0/anywidget/labextension/static/138.3fd6605047ad3df65a9e.js` & `anywidget-0.6.1/anywidget/labextension/static/138.6d69013365e0a65d34c8.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -117,11 +117,11 @@
                             return await this._anywidget_cached_cleanup(), super.remove()
                         }
                     }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.6.0"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.6.1"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.6.0/anywidget/labextension/static/326.c68678f64e2971595925.js` & `anywidget-0.6.1/anywidget/labextension/static/326.44c2db4e788cbf8b5f08.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -135,11 +135,11 @@
                             return await this._anywidget_cached_cleanup(), super.remove()
                         }
                     }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.6.0"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.6.1"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.6.0/anywidget/labextension/static/remoteEntry.cba6b4061725caaf22a8.js` & `anywidget-0.6.1/anywidget/labextension/static/remoteEntry.2cf77409ad03a77cbd09.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, f, l, s, d, p, c, h, v, g = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, g = {
             408: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(138).then((() => () => t(138))),
                         "./extension": () => t.e(326).then((() => () => t(326)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -20,112 +20,112 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        b = {};
+        m = {};
 
-    function m(e) {
-        var r = b[e];
+    function y(e) {
+        var r = m[e];
         if (void 0 !== r) return r.exports;
-        var t = b[e] = {
+        var t = m[e] = {
             exports: {}
         };
-        return g[e](t, t.exports, m), t.exports
+        return g[e](t, t.exports, y), t.exports
     }
-    m.m = g, m.c = b, m.n = e => {
+    y.m = g, y.c = m, y.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return m.d(r, {
+        return y.d(r, {
             a: r
         }), r
-    }, m.d = (e, r) => {
-        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
+    }, y.d = (e, r) => {
+        for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        138: "3fd6605047ad3df65a9e",
-        326: "c68678f64e2971595925"
+    }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
+        138: "6d69013365e0a65d34c8",
+        326: "44c2db4e788cbf8b5f08"
     } [e] + ".js?v=" + {
-        138: "3fd6605047ad3df65a9e",
-        326: "c68678f64e2971595925"
-    } [e], m.g = function() {
+        138: "6d69013365e0a65d34c8",
+        326: "44c2db4e788cbf8b5f08"
+    } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
+    }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", y.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
-                    var s = f[l];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, y.nc && i.setAttribute("nonce", y.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, m.r = e => {
+    }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        m.S = {};
+        y.S = {};
         var e = {},
             r = {};
-        m.I = (t, n) => {
+        y.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                m.o(m.S, t) || (m.S[t] = {});
-                var a = m.S[t],
+                y.o(y.S, t) || (y.S[t] = {});
+                var a = y.S[t],
                     i = "anywidget",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => m.e(138).then((() => () => m(138))),
+                        get: () => y.e(138).then((() => () => y(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.6.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.6.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        m.g.importScripts && (e = m.g.location + "");
-        var r = m.g.document;
+        y.g.importScripts && (e = y.g.location + "");
+        var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
                 for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), y.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -148,130 +148,130 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
         for (a = 1; a < e.length; a++) {
             var u = e[a];
-            i.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return f();
+        return l();
 
-        function f() {
+        function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, u = 1, f = !0;; u++, i++) {
-                var l, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !f || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == s) {
-                    if (!f || "u" != d) return !1
-                } else if (f)
-                    if (d == s)
+            for (var i = 0, u = 1, l = !0;; u++, i++) {
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == f) {
+                    if (!l || "u" != d) return !1
+                } else if (l)
+                    if (d == f)
                         if (u <= n) {
-                            if (l != e[u]) return !1
+                            if (s != e[u]) return !1
                         } else {
-                            if (o ? l > e[u] : l < e[u]) return !1;
-                            l != e[u] && (f = !1)
+                            if (o ? s > e[u] : s < e[u]) return !1;
+                            s != e[u] && (l = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
-                    f = !1, u--
+                    l = !1, u--
                 } else {
-                    if (u <= n || s < d != o) return !1;
-                    f = !1
-                } else "s" != d && "n" != d && (f = !1, u--)
+                    if (u <= n || f < d != o) return !1;
+                    l = !1
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = m.S[e];
-        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = y.S[e];
+        if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || s(f(e, t, o, n)), d(e[t][o])
-    }, s = e => {
+        return a(n, o) || f(l(e, t, o, n)), d(e[t][o])
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
-        var a = m.I(r);
-        return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), c = {}, h = {
+        var a = y.I(r);
+        return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
         395: () => p("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, v = {
         326: [395]
-    }, m.f.consumes = (e, r) => {
-        m.o(v, e) && v[e].forEach((e => {
-            if (m.o(c, e)) return r.push(c[e]);
+    }, y.f.consumes = (e, r) => {
+        y.o(v, e) && v[e].forEach((e => {
+            if (y.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    c[e] = 0, m.m[e] = t => {
-                        delete m.c[e], t.exports = r()
+                    c[e] = 0, y.m[e] = t => {
+                        delete y.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete c[e], m.m[e] = t => {
-                        throw delete m.c[e], r
+                    delete c[e], y.m[e] = t => {
+                        throw delete y.c[e], r
                     }
                 };
             try {
                 var o = h[e]();
                 o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
         };
-        m.f.j = (r, t) => {
-            var n = m.o(e, r) ? e[r] : void 0;
+        y.f.j = (r, t) => {
+            var n = y.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = m.p + m.u(r),
+                    var a = y.p + y.u(r),
                         i = new Error;
-                    m.l(a, (t => {
-                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    y.l(a, (t => {
+                        if (y.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
-                    f = 0;
+                    l = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
-                    u && u(m)
+                    for (n in i) y.o(i, n) && (y.m[n] = i[n]);
+                    u && u(y)
                 }
-                for (r && r(t); f < a.length; f++) o = a[f], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], y.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var y = m(408);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = y
+    var b = y(408);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = b
 })();
```

### Comparing `anywidget-0.6.0/anywidget/nbextension/index.js` & `anywidget-0.6.1/anywidget/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.6.0";
+var version = "0.6.1";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
```

### Comparing `anywidget-0.6.0/docs/README.md` & `anywidget-0.6.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/astro.config.js` & `anywidget-0.6.1/docs/astro.config.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/package.json` & `anywidget-0.6.1/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/public/anywidget-overview.png` & `anywidget-0.6.1/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/public/banner-dark.png` & `anywidget-0.6.1/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/public/banner-light.png` & `anywidget-0.6.1/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/public/banner-minimal.png` & `anywidget-0.6.1/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/public/client-js-diagram.png` & `anywidget-0.6.1/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/public/default-og-image.png` & `anywidget-0.6.1/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/public/favicon.svg` & `anywidget-0.6.1/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/public/widget-overview.png` & `anywidget-0.6.1/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/scripts/ipynb.mjs` & `anywidget-0.6.1/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/scripts/utils.mjs` & `anywidget-0.6.1/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/consts.ts` & `anywidget-0.6.1/docs/src/consts.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/CodeHero.astro` & `anywidget-0.6.1/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/CounterButton.astro` & `anywidget-0.6.1/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/HeadCommon.astro` & `anywidget-0.6.1/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/HeadSEO.astro` & `anywidget-0.6.1/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Hero.astro` & `anywidget-0.6.1/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.6.1/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.6.1/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.6.1/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Header/Header.astro` & `anywidget-0.6.1/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Header/HeaderButton.css` & `anywidget-0.6.1/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.6.1/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.6.1/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Header/Search.css` & `anywidget-0.6.1/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Header/Search.tsx` & `anywidget-0.6.1/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.6.1/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.6.1/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.6.1/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.6.1/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.6.1/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.6.1/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.6.1/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.6.1/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/components/examples/Counter.astro` & `anywidget-0.6.1/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/layouts/MainLayout.astro` & `anywidget-0.6.1/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/layouts/SplashLayout.astro` & `anywidget-0.6.1/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.6.1/docs/src/pages/blog/anywidget-02.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.6.1/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/pages/en/bundling.md` & `anywidget-0.6.1/docs/src/pages/en/bundling.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/pages/en/experimental.md` & `anywidget-0.6.1/docs/src/pages/en/experimental.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/pages/en/getting-started.mdx` & `anywidget-0.6.1/docs/src/pages/en/getting-started.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.6.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.6.1/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/styles/index.css` & `anywidget-0.6.1/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/docs/src/styles/theme.css` & `anywidget-0.6.1/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/examples/Counter.ipynb` & `anywidget-0.6.1/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/examples/minimal_example.ipynb` & `anywidget-0.6.1/examples/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/packages/anywidget/CHANGELOG.md` & `anywidget-0.6.1/packages/anywidget/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # anywidget
 
+## 0.6.1
+
+### Patch Changes
+
+- feat: Bring back support for Python 3.7 ([#167](https://github.com/manzt/anywidget/pull/167))
+
 ## 0.6.0
 
 ### Minor Changes
 
 - feat!: Drop support for Python 3.7 ([#161](https://github.com/manzt/anywidget/pull/161))
 
 ### Patch Changes
```

### Comparing `anywidget-0.6.0/packages/anywidget/build.mjs` & `anywidget-0.6.1/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/packages/anywidget/package.json` & `anywidget-0.6.1/packages/anywidget/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9519230769230769%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^3.6.5'}", "'version'": "'0.6.1'"}*

```diff
@@ -3,15 +3,15 @@
     "dependencies": {
         "@anywidget/types": "workspace:~",
         "@anywidget/vite": "workspace:~",
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6"
     },
     "devDependencies": {
         "@jupyter-widgets/base-manager": "^1.0.5",
-        "@jupyterlab/builder": "^4.0.2"
+        "@jupyterlab/builder": "^3.6.5"
     },
     "exports": {
         ".": "./dist/index.js",
         "./types": {
             "import": "./dist/types.mjs",
             "require": "./dist/types.cjs",
             "types": "./dist/types.d.ts"
@@ -41,9 +41,9 @@
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs",
         "typecheck": "tsc --noEmit"
     },
     "type": "module",
-    "version": "0.6.0"
+    "version": "0.6.1"
 }
```

### Comparing `anywidget-0.6.0/packages/anywidget/__tests__/widget.test.ts` & `anywidget-0.6.1/packages/anywidget/__tests__/widget.test.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/packages/anywidget/src/plugin.js` & `anywidget-0.6.1/packages/anywidget/src/plugin.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/packages/anywidget/src/widget.js` & `anywidget-0.6.1/packages/anywidget/src/widget.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/tests/test_descriptor.py` & `anywidget-0.6.1/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/tests/test_experimental.py` & `anywidget-0.6.1/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/tests/test_file_contents.py` & `anywidget-0.6.1/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/tests/test_utils.py` & `anywidget-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/tests/test_widget.py` & `anywidget-0.6.1/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/LICENSE` & `anywidget-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/README.md` & `anywidget-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.0/pyproject.toml` & `anywidget-0.6.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [build-system]
-requires = ["hatchling", "jupyterlab==4.*"]
+requires = ["hatchling", "jupyterlab==3.*"]
 build-backend = "hatchling.build"
 
 [project]
 name = "anywidget"
 description = "custom jupyter widgets made easy"
 authors = [
     { name = "Trevor Manz", email = "trevor.j.manz@gmail.com" }
 ]
 license = { text = "MIT" }
 dynamic = ["version"]
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 dependencies = [
     "ipywidgets>=7.6.0",
+    "importlib-metadata; python_version < '3.8'",
     "typing-extensions>=4.2.0",
     "psygnal>=0.8.1",
 ]
 
 [project.optional-dependencies]
 test = [
     "black[jupyter]",
     "pydantic",
     "pytest",
     "pytest-cov",
     "ruff",
-    "msgspec",
+    "msgspec; python_version > '3.7'",
     "ipython<8.13; python_version < '3.9'",
 ]
 dev = [
     "comm>=0.1.0",
     "watchfiles>=0.18.0",
 ]
 
@@ -73,22 +74,28 @@
 path = "packages/anywidget/package.json"
 pattern = "\"version\": \"(?P<version>.+?)\""
 
 [tool.hatch.envs.default]
 features = ["test", "dev"]
 
 [tool.hatch.envs.default.scripts]
-fmt = "black ."
-lint = "ruff ."
+lint = [
+  "ruff {args:.}",
+  "black --check --diff {args:.}",
+]
+fmt = [
+  "black {args:.}",
+  "ruff --fix {args:.}",
+]
 test = "pytest . --cov anywidget --cov-report term-missing"
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]
 line-length = 88
-target-version = "py38"
+target-version = "py37"
 src = ["anywidget", "tests"]
 extend-select = [
     "E",    # style errors
     "F",    # flakes
     "D",    # pydocstyle
     "I",    # isort
     "UP",   # pyupgrade
```

### Comparing `anywidget-0.6.0/PKG-INFO` & `anywidget-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.6.0
+Version: 0.6.1
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
-Requires-Python: >=3.8
+Requires-Python: >=3.7
+Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: ipywidgets>=7.6.0
 Requires-Dist: psygnal>=0.8.1
 Requires-Dist: typing-extensions>=4.2.0
 Provides-Extra: dev
 Requires-Dist: comm>=0.1.0; extra == 'dev'
 Requires-Dist: watchfiles>=0.18.0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: black[jupyter]; extra == 'test'
 Requires-Dist: ipython<8.13; python_version < '3.9' and extra == 'test'
-Requires-Dist: msgspec; extra == 'test'
+Requires-Dist: msgspec; python_version > '3.7' and extra == 'test'
 Requires-Dist: pydantic; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: ruff; extra == 'test'
 Description-Content-Type: text/markdown
 
 # anywidget <a href="https://github.com/manzt/anywidget"><img align="right" src="https://raw.githubusercontent.com/manzt/anywidget/main/docs/public/favicon.svg" height="38"></img></a>
```

