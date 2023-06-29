# Comparing `tmp/fsaa-0.0.1.tar.gz` & `tmp/fsaa-0.0.3.tar.gz`

## Comparing `fsaa-0.0.1.tar` & `fsaa-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,53 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fsaa-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.1/environment.yml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 fsaa-0.0.1/requirements.txt
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.1/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/__init__.py
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/attack.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/core.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/utils.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/examples/tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/initializers/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/initializers/random.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/initializers/random_sign.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/losses/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/losses/cossim_loss.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/losses/lpips_loss.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/losses/mse_loss.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/masks/__init__.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/masks/custom.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/masks/jnd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/transforms/__init__.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/transforms/compose.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/transforms/normalize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/updaters/__init__.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/updaters/fgsm.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/updaters/langevin.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/updaters/pgd.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.1/fsaa/updaters/random.py
--rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.1/imgs/adv.png
--rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.1/imgs/mask.png
--rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.1/imgs/orig.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.1/tests/test_attack.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.1/tests/test_initializers.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.1/tests/test_masks.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.1/tests/test_transforms.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.1/tests/test_updaters.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 fsaa-0.0.1/.gitignore
--rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.1/LICENSE
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 fsaa-0.0.1/README.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fsaa-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 fsaa-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fsaa-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.3/CITATION.cff
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.3/CODEOWNERS
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.3/environment.yml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fsaa-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.3/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/attack.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/core.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/utils.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/examples/tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/initializers/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/initializers/random.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/initializers/random_sign.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/losses/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/losses/cossim_loss.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/losses/lpips_loss.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/losses/mse_loss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/masks/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/masks/custom.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/masks/jnd.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/masks/nomask.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/dinov2/dinov2.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/hf_models/hf_models.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/ibot/ibot.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/ibot/utils.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/ibot/vits.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/transforms/__init__.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/transforms/compose.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/transforms/normalize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/updaters/__init__.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/updaters/fgsm.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/updaters/langevin.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/updaters/pgd.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/updaters/random.py
+-rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.3/imgs/adv.png
+-rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.3/imgs/mask.png
+-rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.3/imgs/orig.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_attack.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_initializers.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_masks.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_models.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_transforms.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_updaters.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.3/.gitignore
+-rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 fsaa-0.0.3/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 fsaa-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 fsaa-0.0.3/PKG-INFO
```

### Comparing `fsaa-0.0.1/.pre-commit-config.yaml` & `fsaa-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/environment.yml` & `fsaa-0.0.3/environment.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/.vscode/launch.json` & `fsaa-0.0.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/fsaa/attack.py` & `fsaa-0.0.3/fsaa/attack.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,16 @@
 
     # Getting the mask
     mask = None if perceptual_mask is None else perceptual_mask(x).detach()
 
     # Performing attack
     best_loss = float("inf")
     best_adv = x_adv
-    bar = range(steps) if not pbar else tqdm(range(steps), desc="Attack")
+    bar = range(steps) if not pbar else tqdm(
+        range(steps), desc="Attack", leave=False)
     for step in bar:
         # Getting feature representation
         x_adv.requires_grad = True
         features = model(x_adv)
 
         # Computing the gradient w.r.t loss
         i_loss = 0 if ilw == 0 else ilw * image_loss(x_adv, x).mean()
```

### Comparing `fsaa-0.0.1/fsaa/core.py` & `fsaa-0.0.3/fsaa/core.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/fsaa/examples/tutorial.py` & `fsaa-0.0.3/fsaa/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/fsaa/losses/lpips_loss.py` & `fsaa-0.0.3/fsaa/losses/lpips_loss.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/fsaa/masks/jnd.py` & `fsaa-0.0.3/fsaa/masks/jnd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/fsaa/transforms/normalize.py` & `fsaa-0.0.3/fsaa/transforms/normalize.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/fsaa/updaters/langevin.py` & `fsaa-0.0.3/fsaa/updaters/langevin.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/fsaa/updaters/pgd.py` & `fsaa-0.0.3/fsaa/updaters/pgd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/fsaa/updaters/random.py` & `fsaa-0.0.3/fsaa/updaters/random.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/imgs/adv.png` & `fsaa-0.0.3/imgs/adv.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/imgs/mask.png` & `fsaa-0.0.3/imgs/mask.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/imgs/orig.png` & `fsaa-0.0.3/imgs/orig.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/tests/test_attack.py` & `fsaa-0.0.3/tests/test_attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/tests/test_initializers.py` & `fsaa-0.0.3/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/tests/test_masks.py` & `fsaa-0.0.3/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/tests/test_updaters.py` & `fsaa-0.0.3/tests/test_updaters.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/.gitignore` & `fsaa-0.0.3/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Data
 data/
 
+# Cache folders
+.*cache/
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 */__pycache__/
 *.py[cod]
 *$py.class
 
 # Experiment results
```

### Comparing `fsaa-0.0.1/LICENSE` & `fsaa-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.1/README.md` & `fsaa-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,20 @@
 
 | Original | Corrupted | JND Mask |
 | :------: | :-------: | :------: |
 | <img src="imgs/orig.png" width="300px" /> | <img src="imgs/adv.png" width="300px" /> | <img src="imgs/mask.png" width="300px" />|
 
 </center>
 
+The library also comes with support for pre-trained SSL models from huggingface and other repositories:
+```python
+from fsaa.utils import get_model, SUPPORTED_MODELS
+
+model = get_model("microsoft/beit-base-patch16-224").eval().to(device)
+```
 ___
 
 ## Contributing
 Contributions are highly welcome! Please refer to the [contributing guidelines](./CONTRIBUTING.md).
 ___
 ## License
 The code is distributed according to the **Attribution-NonCommercial 4.0 International** [LICENSE](./LICENSE).
```

### Comparing `fsaa-0.0.1/PKG-INFO` & `fsaa-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 Metadata-Version: 2.1
 Name: fsaa
-Version: 0.0.1
+Version: 0.0.3
 Summary: A simple library for adversarial attacks in feature space.
 Project-URL: Homepage, https://github.com/BrianPulfer/fsaa
 Project-URL: Bug Tracker, https://github.com/BrianPulfer/fsaa/issues
 Author-email: Brian Pulfer <brianpulfer95@gmail.com>
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # FSAA: Feature Space Adversarial Attacks
 FSAA allows to create adversarial examples that corrupt the features of the victim models. Various attacks are possible, by altering initialization and update strategies, losses and perceptual masks.
 FSAA is written in Python and is based on PyTorch.
 ___
 
@@ -98,14 +105,20 @@
 
 | Original | Corrupted | JND Mask |
 | :------: | :-------: | :------: |
 | <img src="imgs/orig.png" width="300px" /> | <img src="imgs/adv.png" width="300px" /> | <img src="imgs/mask.png" width="300px" />|
 
 </center>
 
+The library also comes with support for pre-trained SSL models from huggingface and other repositories:
+```python
+from fsaa.utils import get_model, SUPPORTED_MODELS
+
+model = get_model("microsoft/beit-base-patch16-224").eval().to(device)
+```
 ___
 
 ## Contributing
 Contributions are highly welcome! Please refer to the [contributing guidelines](./CONTRIBUTING.md).
 ___
 ## License
 The code is distributed according to the **Attribution-NonCommercial 4.0 International** [LICENSE](./LICENSE).
```

