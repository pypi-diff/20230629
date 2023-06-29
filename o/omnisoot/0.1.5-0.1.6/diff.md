# Comparing `tmp/omnisoot-0.1.5-cp39-cp39-win_amd64.whl.zip` & `tmp/omnisoot-0.1.6-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,23 @@
-Zip file size: 799509 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat      617 b- defN 23-Jun-22 13:04 omnisoot/__init__.py
--rw-rw-rw-  2.0 fat     6093 b- defN 23-May-31 12:31 omnisoot/cpfr.py
--rw-rw-rw-  2.0 fat      679 b- defN 23-May-31 12:31 omnisoot/omnisoot.py
--rw-rw-rw-  2.0 fat      644 b- defN 23-May-31 12:31 omnisoot/psr.py
+Zip file size: 772438 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat      631 b- defN 23-Jun-25 20:54 omnisoot/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-05 04:38 omnisoot/apps/__init__.py
 -rw-rw-rw-  2.0 fat     1047 b- defN 23-May-31 12:31 omnisoot/apps/flame.py
 -rw-rw-rw-  2.0 fat     2231 b- defN 23-Jun-22 12:56 omnisoot/apps/pahgrowth.py
--rw-rw-rw-  2.0 fat    10743 b- defN 23-Jun-23 13:00 omnisoot/apps/reactors.py
+-rw-rw-rw-  2.0 fat    10742 b- defN 23-Jun-29 16:43 omnisoot/apps/reactors.py
 -rw-rw-rw-  2.0 fat      265 b- defN 23-Apr-05 04:46 omnisoot/apps/solutionarray.py
--rw-rw-rw-  2.0 fat     6397 b- defN 23-Jun-22 16:36 omnisoot/apps/solutionmodifier.py
+-rw-rw-rw-  2.0 fat     6505 b- defN 23-Jun-26 01:39 omnisoot/apps/solutionmodifier.py
 -rw-rw-rw-  2.0 fat     4228 b- defN 23-Jun-16 20:57 omnisoot/apps/sootgas.py
--rw-rw-rw-  2.0 fat     1900 b- defN 23-Jun-01 22:16 omnisoot/apps/sootmodels.py
+-rw-rw-rw-  2.0 fat     1875 b- defN 23-Jun-29 13:41 omnisoot/apps/sootmodels.py
 -rw-rw-rw-  2.0 fat      718 b- defN 23-Jun-18 01:19 omnisoot/apps/sootthermo.py
 -rw-rw-rw-  2.0 fat     5993 b- defN 23-May-31 12:31 omnisoot/apps/sootwrappers.py
 -rw-rw-rw-  2.0 fat      239 b- defN 23-May-31 12:31 omnisoot/apps/surfacereactions.py
--rw-rw-rw-  2.0 fat  2175488 b- defN 23-Jun-25 18:41 omnisoot/lib/_omnisoot.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1586 b- defN 23-Jun-25 18:41 omnisoot-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-25 18:41 omnisoot-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-25 18:40 omnisoot-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1622 b- defN 23-Jun-25 18:41 omnisoot-0.1.5.dist-info/RECORD
-20 files, 2220599 bytes uncompressed, 796877 bytes compressed:  64.1%
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-25 20:54 omnisoot/legacy/__init__.py
+-rw-rw-rw-  2.0 fat     6101 b- defN 23-Jun-25 20:54 omnisoot/legacy/cpfr.py
+-rw-rw-rw-  2.0 fat      687 b- defN 23-Jun-25 20:54 omnisoot/legacy/eptlsoot.py
+-rw-rw-rw-  2.0 fat      652 b- defN 23-Jun-26 01:50 omnisoot/legacy/psr.py
+-rw-rw-rw-  2.0 fat  2092544 b- defN 23-Jun-29 17:01 omnisoot/lib/_omnisoot.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1586 b- defN 23-Jun-29 17:01 omnisoot-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-29 17:01 omnisoot-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-29 17:00 omnisoot-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1724 b- defN 23-Jun-29 17:01 omnisoot-0.1.6.dist-info/RECORD
+21 files, 2137879 bytes uncompressed, 769634 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,19 +1,10 @@
 Filename: omnisoot/__init__.py
 Comment: 
 
-Filename: omnisoot/cpfr.py
-Comment: 
-
-Filename: omnisoot/omnisoot.py
-Comment: 
-
-Filename: omnisoot/psr.py
-Comment: 
-
 Filename: omnisoot/apps/__init__.py
 Comment: 
 
 Filename: omnisoot/apps/flame.py
 Comment: 
 
 Filename: omnisoot/apps/pahgrowth.py
@@ -39,23 +30,35 @@
 
 Filename: omnisoot/apps/sootwrappers.py
 Comment: 
 
 Filename: omnisoot/apps/surfacereactions.py
 Comment: 
 
+Filename: omnisoot/legacy/__init__.py
+Comment: 
+
+Filename: omnisoot/legacy/cpfr.py
+Comment: 
+
+Filename: omnisoot/legacy/eptlsoot.py
+Comment: 
+
+Filename: omnisoot/legacy/psr.py
+Comment: 
+
 Filename: omnisoot/lib/_omnisoot.cp39-win_amd64.pyd
 Comment: 
 
-Filename: omnisoot-0.1.5.dist-info/METADATA
+Filename: omnisoot-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: omnisoot-0.1.5.dist-info/WHEEL
+Filename: omnisoot-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: omnisoot-0.1.5.dist-info/top_level.txt
+Filename: omnisoot-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: omnisoot-0.1.5.dist-info/RECORD
+Filename: omnisoot-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omnisoot/__init__.py

```diff
@@ -1,9 +1,9 @@
-from .omnisoot import SootModel, Reactor, ReactorSoot, FlameSolver, FlameSolverOpt
-from .cpfr import CPFR
+from .legacy.eptlsoot import SootModel, Reactor, ReactorSoot, FlameSolver, FlameSolverOpt
+from .legacy.cpfr import CPFR
 from .apps.sootgas import SootGas
 from .apps.sootmodels import MonodisperseSootModel
 from .apps.reactors import PlugFlowReactor, ConstantVolumeReactor, Inlet, PerfectlyStirredReactor
 from .apps.pahgrowth import ReactDim, DimerCoal
 from .apps.flame import TempFlameSolver, TempFlameSolverOpt, FVSolver, FDSolver, FDSolverTemp
 from .apps.sootwrappers import SootWrapper
 from .apps.solutionarray import SolutionArray
```

## omnisoot/apps/reactors.py

```diff
@@ -41,15 +41,15 @@
         # Inlet
         self.inlet = Inlet(self);
         # Solver
         self.solver = None;
         # Max length
         self.max_length = 100;
         # First step
-        self.first_step = 1e-10;
+        self.first_step = None;
         # Max step
         self.max_step = 1e-3;
 
     def start(self):
         if self.check_soot_array(self.inlet.soot):
             self.T = self.inlet.T;
             self.P = self.inlet.P;
@@ -173,20 +173,20 @@
         # Reactor pressure
         self.P = self.soot_gas.P;
         # Solver
         self.solver = None;
         # Max residence time
         self.max_time = 100;
         # First step
-        self.first_step = 1e-10;
+        self.first_step = None;
         # Max step
         self.max_step = 1e-3;
         # Tol
-        self.rtol= 1e-5
-        self.atol= 1e-10;
+        self.rtol= 1e-7;
+        self.atol= 1e-12;
         # Initial soot
         self.initial_soot = self.soot_wrapper.min_array;
         # Temperature solver
         self.temperature_solver_type = "energy_equation";
 
 
 
@@ -198,20 +198,20 @@
         # Reactor pressure
         self.P = self.soot_gas.P;
         # Solver
         self.solver = None;
         # Max residence time
         self.max_time = 100;
         # First step
-        self.first_step = 1e-10;
+        self.first_step = None;
         # Max step
         self.max_step = 1e-3;
         # Tol
-        self.rtol= 1e-5
-        self.atol= 1e-10;
+        self.rtol= 1e-7;
+        self.atol= 1e-12;
         # Initial soot
         self.initial_soot = self.soot_wrapper.min_array;
         # Temperature solver
         self.temperature_solver_type = "energy_equation";
 
 class ConstantVolumeReactor:
     def __new__(cls, soot_gas, high_concentration = False):
```

## omnisoot/apps/solutionmodifier.py

```diff
@@ -11,52 +11,52 @@
     head = name.rstrip('0123456789')
     tail = name[len(head):]
     return head, tail
 
 
 def k_f1_dict(PAH, **kwargs):
     PAH_n_C = PAH.composition["C"];
-    A = 9.8e1 * PAH_n_C;
+    A = 9.8e1 * PAH_n_C; #[mol/m3-s] 
     b = 1.84;
     Ea = 62886.6; #[j/mol];
-    return {"rate-constant": {"A": A/1e3, "b": b, "Ea": Ea}};
+    return {"rate-constant": {"A": A*1e3, "b": b, "Ea": Ea*1e3}};
 
 #----------------------------------------------------------------------------
 ### Reaction rate constant dict constructor functions
 def k_r1_dict(**kwargs):
 #     Ref: Semenikhin et al.(2017); Rate constants for H abstraction from benzo(a)pyrene and chrysene: a theoretical study
     A = 1.60e-2;
     b = 2.63;
     Ea = 17837.4; #[j/mol];
-    return {"rate-constant": {"A": A/1e3, "b": b, "Ea": Ea}};
+    return {"rate-constant": {"A": A*1e3, "b": b, "Ea": Ea*1e3}};
 
 def k_f2_dict(**kwargs):
     #   Ref: Hadrings (2005); Predictive Theory for Hydrogen Atom-Hydrocarbon Radical Association Kinetics
     A = 8.08e-11 * 1e-6 * Avogadro;
     b = 0.13;
     Ea = 0.0;
-    return {"rate-constant": {"A": A/1e3, "b": b, "Ea": Ea}};
+    return {"rate-constant": {"A": A*1e3, "b": b, "Ea": Ea*1e3}};
 
 def k_f3_dict(PAH_i, PAH_j, **kwargs):
     PAH_mass_i = PAH_i.molecular_weight / (Avogadro*1e3); #kg
     PAH_mass_j = PAH_j.molecular_weight / (Avogadro*1e3); #kg
     d_mi = (6*PAH_mass_i/(Pi*rho_soot))**(1.0/3.0);
     d_mj = (6*PAH_mass_j/(Pi*rho_soot))**(1.0/3.0);
     mu = PAH_mass_i * PAH_mass_j / (PAH_mass_i + PAH_mass_j);
     A = Avogadro * C * (1.0 / mu)**0.5 * (d_mi + d_mj) ** 2.0;
     b = 0.5;
     Ea = 0.0;
-    return {"rate-constant": {"A": A/1e3, "b": b, "Ea": Ea}};
+    return {"rate-constant": {"A": A*1e3, "b": b, "Ea": Ea*1e3}};
 
 
 def k_r3_dict(**kwargs):
     A = 1.3e83;
     b = -20.162;
     Ea = 401287.44;
-    return {"rate-constant": {"A": A/1e3, "b": b, "Ea": Ea}};
+    return {"rate-constant": {"A": A*1e3, "b": b, "Ea": Ea*1e3}};
 #----------------------------------------------------------------------------
 
 def add_e_bridge(gas, precursor_list, n_steps = 4):
     e_bridge_species = [];
     e_bridge_reactions = [];
 
     for precursor_name in precursor_list:
@@ -102,15 +102,17 @@
             ## Radical hydrogenation forward reaction
             reaction_rate = ct.ReactionRate.from_dict(k_f2_dict())
             reaction_dict = {
                 "reactants" : {radical.name: 1.0, "H": 1.0},
                 "products"  : {PAH.name: 1.0},
                 "rate"      : reaction_rate,
             }
-            e_bridge_reactions.append(ct.Reaction(**reaction_dict));
+            reaction = ct.Reaction(**reaction_dict)
+            reaction.reversible = False;
+            e_bridge_reactions.append(reaction);
             if (polymer_index < (n_steps-1)):
                 ## New Polymer
                 polymer_dict = {
                     "name":  f"{precursor.name}e{(polymer_index+2)}",
                     "composition": {"C": (radical.composition["C"]+precursor.composition["C"]),
                                     "H": (radical.composition["H"]+precursor.composition["H"]-1)},
                     "charge" : PAH.charge,
```

## omnisoot/apps/sootmodels.py

```diff
@@ -1,8 +1,8 @@
-from ..lib._omnisoot import CMonodisperseSootModel, CMonodisperseCoalesceSootModel
+from ..lib._omnisoot import CMonodisperseSootModel
 
 class MonodisperseSootModel(CMonodisperseSootModel):
     serialized_name = "Monodisperse"
     soot_att = ["N_agg", "N_pri", "H_tot", "C_tot", "A_tot",
               "d_p", "d_m", "d_g", "d_v", "n_p",
               "SSA", "total_mass", "volume_fraction",
               "carbon_mass", "hydrogen_mass",
@@ -18,30 +18,30 @@
         super().__init__(soot_wrapper);
 
     def det_soot_att(self, name):
         if name in self.soot_att:
             att_func = getattr(self, name);
             return att_func();
 
-class MonodisperseSootCoalesceModel(CMonodisperseCoalesceSootModel):
-    serialized_name = "MonodisperseCoalesce"
-    soot_att = ["N_agg", "N_pri", "H_tot", "C_tot", "A_tot",
-              "d_p", "d_m", "d_g", "d_v", "n_p",
-              "SSA", "total_mass", "volume_fraction",
-              "carbon_mass", "hydrogen_mass",
-              "inception_mass", "inception_vol",
-              "PAH_adsorption_mass", "PAH_adsorption_vol",
-              "surface_growth_mass", "surface_growth_vol",
-              "oxidation_mass", "oxidation_vol",
-              "coagulation_mass", "coagulation_vol",
-              "min_array"
-              ]
+# class MonodisperseSootCoalesceModel(CMonodisperseCoalesceSootModel):
+#     serialized_name = "MonodisperseCoalesce"
+#     soot_att = ["N_agg", "N_pri", "H_tot", "C_tot", "A_tot",
+#               "d_p", "d_m", "d_g", "d_v", "n_p",
+#               "SSA", "total_mass", "volume_fraction",
+#               "carbon_mass", "hydrogen_mass",
+#               "inception_mass", "inception_vol",
+#               "PAH_adsorption_mass", "PAH_adsorption_vol",
+#               "surface_growth_mass", "surface_growth_vol",
+#               "oxidation_mass", "oxidation_vol",
+#               "coagulation_mass", "coagulation_vol",
+#               "min_array"
+#               ]
     
-    def __init__(self, soot_wrapper):
-        super().__init__(soot_wrapper);
+#     def __init__(self, soot_wrapper):
+#         super().__init__(soot_wrapper);
 
-    def det_soot_att(self, name):
-        if name in self.soot_att:
-            att_func = getattr(self, name);
-            return att_func();
+#     def det_soot_att(self, name):
+#         if name in self.soot_att:
+#             att_func = getattr(self, name);
+#             return att_func();
 
-SOOT_MODELS = [MonodisperseSootModel, MonodisperseSootCoalesceModel]
+SOOT_MODELS = [MonodisperseSootModel]
```

## Comparing `omnisoot/cpfr.py` & `omnisoot/legacy/cpfr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Decelarations
 import cantera as ct
 import numpy as np
 import scipy.integrate
-from .lib._omnisoot import CSootModel, CPFROde
+from omnisoot.lib._omnisoot import CSootModel, CPFROde
 
 class Inlet:
     def __init__(self, name, phase):
         self.phase = phase;
         self.name = name;
         self.X = {};
         self.T = None; #[K]
```

## Comparing `omnisoot/omnisoot.py` & `omnisoot/legacy/eptlsoot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .lib._omnisoot import CSootModel, CPFROde, CPFRSootOde, CFlameSolver, CFlameSolverOpt
+from omnisoot.lib._omnisoot import CSootModel, CPFROde, CPFRSootOde, CFlameSolver, CFlameSolverOpt
 
 class SootModel(CSootModel):
     def __init__(self):
         super().__init__()
 
 
 class Reactor(CPFROde):
```

## Comparing `omnisoot/psr.py` & `omnisoot/legacy/psr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Decelarations
 import cantera as ct
 import numpy as np
 import scipy.integrate
-from .lib._omnisoot import CSootModel
+from omnisoot.lib._omnisoot import CSootModel
 
 
 class Inlet:
     def __init__(self, name, phase):
         self.phase = phase;
         self.name = name;
         self.X = {};
```

## Comparing `omnisoot-0.1.5.dist-info/METADATA` & `omnisoot-0.1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnisoot
-Version: 0.1.5
+Version: 0.1.6
 Summary: a computational tool for modeling soot
 Author-email: Mo Adib <moademic@gmail.com>
 Project-URL: Homepage, https://carleton.ca/eptl/people/336/
 Keywords: computational,soot
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

## Comparing `omnisoot-0.1.5.dist-info/RECORD` & `omnisoot-0.1.6.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-omnisoot/__init__.py,sha256=HDxZmHRSLudX4GdBaj6opPgIzlotsxIW3H2_j1cY-yY,617
-omnisoot/cpfr.py,sha256=xFQv12SM3syCwom0HMoNxobCV-bcnETupPmOUTgDcpU,6093
-omnisoot/omnisoot.py,sha256=ZIMyVmZ9ct1fIzW-yAG9fkEjdRXY8oLaRLi5WkEoEmY,679
-omnisoot/psr.py,sha256=BsWn_vupqnpCQzaJPoOIRHBfukoc9Y0vje42dEMFeFA,644
+omnisoot/__init__.py,sha256=PfYx7SQYWxFa9eoDhFlLVC9J1ro1T68S1ZbXVqtP-oY,631
 omnisoot/apps/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 omnisoot/apps/flame.py,sha256=Zg9CxaQIMwrK0RkirXHLnXnXlIi4OLzzEdUVvMe1UeA,1047
 omnisoot/apps/pahgrowth.py,sha256=RqUqPD6tNeFVXKnCiitP1zudF1Ic-tJjuduyjThoKx8,2231
-omnisoot/apps/reactors.py,sha256=FoJNAPaspFmf_epwRvr6DEJR_t0vP5kmWwpzrn8eNxQ,10743
+omnisoot/apps/reactors.py,sha256=uQblNnltupDXS5vZfk5_9dq6Xiro5Vq7Bf1XMFRfKeM,10742
 omnisoot/apps/solutionarray.py,sha256=gGyAu8LnGNU3CuDvae8rXD3TrEnAanYeWOa1QErsV8U,265
-omnisoot/apps/solutionmodifier.py,sha256=rlz-VMQomKr95vWOl3r-UjAfkLApP99g-UvYJAOBcyw,6397
+omnisoot/apps/solutionmodifier.py,sha256=cgRZDOI9ms4eyWmGnx-43DGbhHZTliUiRjaPtltbjGg,6505
 omnisoot/apps/sootgas.py,sha256=eJWYyfq94aGZSr38Pa8IjiLJ9zPLGl0mYEmdQDPycHg,4228
-omnisoot/apps/sootmodels.py,sha256=Ts77fMwWQ5t9wRlFZrcSb3AAQtpLHOQkKAODCBMMBBk,1900
+omnisoot/apps/sootmodels.py,sha256=MYJFUU03YaiOrdMI__Fe-y430chbOf0kEl1Lk4APPbg,1875
 omnisoot/apps/sootthermo.py,sha256=DX0q6KRwR2Qfapmjnk0zz727uVoQ1oxt4xdcSxDvnBI,718
 omnisoot/apps/sootwrappers.py,sha256=YFhbFT2JUGmlMKkT9eSfZa0_IMU1sjpB331_G5xv1eM,5993
 omnisoot/apps/surfacereactions.py,sha256=5zgz_HKCeGgBW6L1nYUp_mFEFIgjDQchT3ZejRGV2BY,239
-omnisoot/lib/_omnisoot.cp39-win_amd64.pyd,sha256=Tuy54g7Wtx30s_TcB8ocLMnXtOp5TlXiPkI0qUinHfs,2175488
-omnisoot-0.1.5.dist-info/METADATA,sha256=7OZo3JspQmzdcz7FIFCpHe1XPheaCSl7OknX46a0FNA,1586
-omnisoot-0.1.5.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-omnisoot-0.1.5.dist-info/top_level.txt,sha256=k7bKrgnA_SQG4D5xcsVXUOdVMLes9lFzeDbvtIw7oAo,9
-omnisoot-0.1.5.dist-info/RECORD,,
+omnisoot/legacy/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+omnisoot/legacy/cpfr.py,sha256=bUBkQXbdMtEvWnqdoJKu4rX5hvd4RkgBv5TIRxTQ0NM,6101
+omnisoot/legacy/eptlsoot.py,sha256=ZwZRTP-ofLkOCkWyG9XqR5e_1QnfglmMtfCZnbyEgTc,687
+omnisoot/legacy/psr.py,sha256=3J1ldQlFrFEnumCW-UrHhsoghhby0j-l51p6L87bpI0,652
+omnisoot/lib/_omnisoot.cp39-win_amd64.pyd,sha256=VRd3SLGu7HNh7haDjbFWaOcSzooemxoxQRvQ6ajVk0s,2092544
+omnisoot-0.1.6.dist-info/METADATA,sha256=goG5uLU6_lXeZv6c-KtjUMGaOU6GhAOdT6gyuXwHcGM,1586
+omnisoot-0.1.6.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+omnisoot-0.1.6.dist-info/top_level.txt,sha256=k7bKrgnA_SQG4D5xcsVXUOdVMLes9lFzeDbvtIw7oAo,9
+omnisoot-0.1.6.dist-info/RECORD,,
```

