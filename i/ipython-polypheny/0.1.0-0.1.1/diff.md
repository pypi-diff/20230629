# Comparing `tmp/ipython-polypheny-0.1.0.tar.gz` & `tmp/ipython-polypheny-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython-polypheny-0.1.0.tar", last modified: Mon Jun 26 09:41:46 2023, max compression
+gzip compressed data, was "ipython-polypheny-0.1.1.tar", last modified: Thu Jun 29 15:54:53 2023, max compression
```

## Comparing `ipython-polypheny-0.1.0.tar` & `ipython-polypheny-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 09:41:46.955444 ipython-polypheny-0.1.0/
--rw-rw-rw-   0        0        0    10349 2023-06-26 09:12:17.000000 ipython-polypheny-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4011 2023-06-26 09:41:46.956447 ipython-polypheny-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3555 2023-06-26 09:12:17.000000 ipython-polypheny-0.1.0/README.md
--rw-rw-rw-   0        0        0       82 2023-06-26 09:12:17.000000 ipython-polypheny-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      685 2023-06-26 09:41:46.964445 ipython-polypheny-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-26 09:41:46.907446 ipython-polypheny-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 09:41:46.948552 ipython-polypheny-0.1.0/src/ipython_polypheny.egg-info/
--rw-rw-rw-   0        0        0     4011 2023-06-26 09:41:46.000000 ipython-polypheny-0.1.0/src/ipython_polypheny.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-06-26 09:41:46.000000 ipython-polypheny-0.1.0/src/ipython_polypheny.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 09:41:46.000000 ipython-polypheny-0.1.0/src/ipython_polypheny.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-26 09:41:46.000000 ipython-polypheny-0.1.0/src/ipython_polypheny.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-26 09:41:46.000000 ipython-polypheny-0.1.0/src/ipython_polypheny.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 09:41:46.954448 ipython-polypheny-0.1.0/src/poly/
--rw-rw-rw-   0        0        0      110 2023-06-26 09:12:17.000000 ipython-polypheny-0.1.0/src/poly/__init__.py
--rw-rw-rw-   0        0        0      942 2023-06-26 09:12:17.000000 ipython-polypheny-0.1.0/src/poly/http_interface.py
--rw-rw-rw-   0        0        0     5302 2023-06-26 09:12:17.000000 ipython-polypheny-0.1.0/src/poly/poly_magic.py
--rw-rw-rw-   0        0        0     2453 2023-06-26 09:12:17.000000 ipython-polypheny-0.1.0/src/poly/poly_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:54:53.693428 ipython-polypheny-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-29 15:54:44.000000 ipython-polypheny-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-29 15:54:53.693428 ipython-polypheny-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-29 15:54:44.000000 ipython-polypheny-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-29 15:54:44.000000 ipython-polypheny-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-29 15:54:53.693428 ipython-polypheny-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:54:53.689428 ipython-polypheny-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:54:53.693428 ipython-polypheny-0.1.1/src/ipython_polypheny.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-29 15:54:53.000000 ipython-polypheny-0.1.1/src/ipython_polypheny.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 15:54:53.000000 ipython-polypheny-0.1.1/src/ipython_polypheny.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:54:53.000000 ipython-polypheny-0.1.1/src/ipython_polypheny.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 15:54:53.000000 ipython-polypheny-0.1.1/src/ipython_polypheny.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 15:54:53.000000 ipython-polypheny-0.1.1/src/ipython_polypheny.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:54:53.693428 ipython-polypheny-0.1.1/src/poly/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-29 15:54:44.000000 ipython-polypheny-0.1.1/src/poly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-29 15:54:44.000000 ipython-polypheny-0.1.1/src/poly/http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-29 15:54:44.000000 ipython-polypheny-0.1.1/src/poly/poly_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-29 15:54:44.000000 ipython-polypheny-0.1.1/src/poly/poly_result.py
```

### Comparing `ipython-polypheny-0.1.0/LICENSE` & `ipython-polypheny-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
    END OF TERMS AND CONDITIONS
```

### Comparing `ipython-polypheny-0.1.0/src/poly/poly_magic.py` & `ipython-polypheny-0.1.1/src/poly/poly_magic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-import re
-
-from IPython.core.magic import (
-    Magics,
-    magics_class,
-    needs_local_scope,
-    line_cell_magic, no_var_expand
-)
-from IPython.core.magic_arguments import magic_arguments, argument, parse_argstring
-from IPython.display import display, JSON
-from .poly_result import build_result
-
-from .http_interface import HttpInterface
-
-
-@magics_class
-class PolyMagics(Magics):
-
-    def __init__(self, shell):
-        super().__init__(shell)
-        print('Initialized ipython-polypheny extension')
-        self.database = HttpInterface()
-        self.ns = None
-
-    # To correctly detect where the args end and the query starts, the first occurrence of ':' is used.
-    # For cell_magic, ':' can be omitted if the initial line contains precisely the args.
-    # IMPORTANT: future (optional) arguments and their expected values may not contain a ':' symbol.
-    @needs_local_scope
-    @line_cell_magic
-    @no_var_expand  # we implement custom variable expansion logic
-    @magic_arguments()
-    @argument(
-        "command",
-        choices=('db', 'info', 'help', 'sql', 'mql', 'cypher', 'pig', 'cql', 'load'),  # Specifies all possible subcommands
-        help="Specify the command to be used.",
-    )
-    @argument(
-        "-j",
-        "--json",
-        action='store_true',
-        dest='display_json',
-        help="Display a JSON representation of the query result.",
-    )
-    @argument(
-        "-i",
-        "--input",
-        action='store_true',
-        dest='load_from_input',
-        help="When using load, request the query result via an input prompt.",
-    )
-    @argument(
-        "-t",
-        "--template",
-        action='store_true',
-        dest='is_template',
-        help="Treat the query as a template. "
-             "Parameters like ${my_param} will be expanded to their corresponding value. "
-             "Warning: This can lead to arbitrary query injections, as the parameters do not get escaped.",
-    )
-    @argument(
-        "-h",
-        "--help",
-        action='store_true',
-        help="Print command-specific help.",
-    )
-    @argument(
-        "namespace",
-        nargs='?',
-        default='public',
-        help="Specify the default namespace to be used. If no argument is given, 'public' is used.",
-    )
-    def poly(self, line, cell=None, local_ns=None):
-        """    : [value]
-
-
-        Line and Cell magics for querying Polypheny.
-        Instead of the ':' separator between command and value, the value can be written on a new line in cell magics.
-
-        Examples:
-            %poly db: localhost:13137
-
-            %poly sql: SELECT * FROM xyz
-
-            %%poly sql
-            SELECT * FROM xyz
-
-            %%poly mql my_documents
-            db.collection.find({})
-
-
-          value\t\t\tSpecify the query (for sql,mql,cypher,pig,cql,load) or the URL (for the db command).
-        """
-
-        self.ns = self.shell.user_ns.copy()
-
-        raw_args, value = separate_args(line, cell)
-        if not (raw_args and value):
-            if not 'help' in raw_args:
-                print("Did you forget to terminate your arguments with ':' ?")
-            self.poly.parser.print_help()
-            return
-
-        if cell is None:
-            self.ns.update(local_ns)  # Add local namespace to global namespace (local can only differ in line magics)
-
-        args = parse_argstring(self.poly, raw_args)
-
-        return self.handle(args, value)
-
-    def handle(self, args, value):
-        command = args.command
-
-        if args.help or command == 'help':
-            # TODO: add command specific help
-            self.poly.parser.print_help()
-            return
-        if command == 'db':
-            self.database.set_url(value)
-            return
-        elif command == 'info':
-            return str(self.database)
-
-        if args.is_template:
-            value = self.expand_variables(value)
-
-        if command == 'load':
-            result = build_result(input(value)) if args.load_from_input else build_result(value)
-        else:
-            result = self.database.request(value, command, args.namespace)
-
-        if args.display_json:
-            display(JSON(result.result_set))
-        return result
-
-    def expand_variables(self, template):
-        pattern = r'\$\{([^\} ]+)\}'  # '${<my_var>}', where <my_var> has at least length 1 and contains no space or '}'
-        matches = re.findall(pattern, template)  # Find all matches of the pattern
-
-        for match in matches:
-            if match in self.ns:
-                template = template.replace('${' + match + '}', str(self.ns[match]))
-
-        return template
-
-
-def separate_args(line, cell, split_str=":"):
-    """
-    Finds the first occurence of an element of termination_strings in line. The line is split after this element and
-    the two parts are returned.
-    """
-    if cell is None:
-        split_str += ' '  # if line_magic, check for space after split_str. (e.g. to ignore http://)
-
-    idx = line.find(split_str)
-    if idx == -1:
-        return line, cell
-    args = line[:idx]
-    value = line[idx + 1:]
-    if cell is not None:
-        value += '\n' + cell
-    return args, value.strip()
+import re
+
+from IPython.core.magic import (
+    Magics,
+    magics_class,
+    needs_local_scope,
+    line_cell_magic, no_var_expand
+)
+from IPython.core.magic_arguments import magic_arguments, argument, parse_argstring
+from IPython.display import display, JSON
+from .poly_result import build_result
+
+from .http_interface import HttpInterface
+
+
+@magics_class
+class PolyMagics(Magics):
+
+    def __init__(self, shell):
+        super().__init__(shell)
+        self.database = HttpInterface()
+        self.ns = None
+
+    # To correctly detect where the args end and the query starts, the first occurrence of ':' is used.
+    # For cell_magic, ':' can be omitted if the initial line contains precisely the args.
+    # IMPORTANT: future (optional) arguments and their expected values may not contain a ':' symbol.
+    @needs_local_scope
+    @line_cell_magic
+    @no_var_expand  # we implement custom variable expansion logic
+    @magic_arguments()
+    @argument(
+        "command",
+        choices=('db', 'info', 'help', 'sql', 'mql', 'cypher', 'pig', 'cql', 'load'),
+        # Specifies all possible subcommands
+        help="Specify the command to be used.",
+    )
+    @argument(
+        "-j",
+        "--json",
+        action='store_true',
+        dest='display_json',
+        help="Display a JSON representation of the query result.",
+    )
+    @argument(
+        "-i",
+        "--input",
+        action='store_true',
+        dest='load_from_input',
+        help="When using load, request the query result via an input prompt.",
+    )
+    @argument(
+        "-t",
+        "--template",
+        action='store_true',
+        dest='is_template',
+        help="Treat the query as a template. "
+             "Parameters like ${my_param} will be expanded to their corresponding value. "
+             "Warning: This can lead to arbitrary query injections, as the parameters do not get escaped.",
+    )
+    @argument(
+        "-h",
+        "--help",
+        action='store_true',
+        help="Print command-specific help.",
+    )
+    @argument(
+        "namespace",
+        nargs='?',
+        default='public',
+        help="Specify the default namespace to be used. If no argument is given, 'public' is used.",
+    )
+    def poly(self, line, cell=None, local_ns=None):
+        """    : [value]
+
+
+        Line and Cell magics for querying Polypheny.
+        Instead of the ':' separator between command and value, the value can be written on a new line in cell magics.
+
+        Examples:
+            %poly db: localhost:13137
+
+            %poly sql: SELECT * FROM xyz
+
+            %%poly sql
+            SELECT * FROM xyz
+
+            %%poly mql my_documents
+            db.collection.find({})
+
+
+          value\t\t\tSpecify the query (for sql,mql,cypher,pig,cql,load) or the URL (for the db command).
+        """
+
+        self.ns = self.shell.user_ns.copy()
+
+        raw_args, value = separate_args(line, cell)
+        if not (raw_args and value):
+            if not 'help' in raw_args:
+                print("Did you forget to terminate your arguments with ':' ?")
+            self.poly.parser.print_help()
+            return
+
+        if cell is None:
+            self.ns.update(local_ns)  # Add local namespace to global namespace (local can only differ in line magics)
+
+        args = parse_argstring(self.poly, raw_args)
+
+        return self.handle(args, value)
+
+    def handle(self, args, value):
+        command = args.command
+
+        if args.help or command == 'help':
+            # TODO: add command specific help
+            self.poly.parser.print_help()
+            return
+        if command == 'db':
+            self.database.set_url(value)
+            return
+        elif command == 'info':
+            return str(self.database)
+
+        if args.is_template:
+            value = self.expand_variables(value)
+
+        if command == 'load':
+            result = build_result(input(value)) if args.load_from_input else build_result(value)
+        else:
+            result = self.database.request(value, command, args.namespace)
+
+        if args.display_json:
+            display(JSON(result.result_set))
+        return result
+
+    def expand_variables(self, template):
+        pattern = r'\$\{([^\} ]+)\}'  # '${<my_var>}', where <my_var> has at least length 1 and contains no space or '}'
+        matches = re.findall(pattern, template)  # Find all matches of the pattern
+
+        for match in matches:
+            if match in self.ns:
+                template = template.replace('${' + match + '}', str(self.ns[match]))
+
+        return template
+
+
+def separate_args(line, cell, split_str=":"):
+    """
+    Finds the first occurence of an element of termination_strings in line. The line is split after this element and
+    the two parts are returned.
+    """
+    if cell is None:
+        split_str += ' '  # if line_magic, check for space after split_str. (e.g. to ignore http://)
+
+    idx = line.find(split_str)
+    if idx == -1:
+        return line, cell
+    args = line[:idx]
+    value = line[idx + 1:]
+    if cell is not None:
+        value += '\n' + cell
+    return args, value.strip()
```

