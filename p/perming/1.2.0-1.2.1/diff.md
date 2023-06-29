# Comparing `tmp/perming-1.2.0-py3-none-any.whl.zip` & `tmp/perming-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12716 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      849 b- defN 23-Jun-28 11:12 perming/__init__.py
+Zip file size: 12742 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      850 b- defN 23-Jun-29 11:51 perming/__init__.py
 -rw-rw-rw-  2.0 fat      176 b- defN 23-May-29 15:03 perming/_typing.py
--rw-rw-rw-  2.0 fat    20144 b- defN 23-Jun-28 11:39 perming/_utils.py
+-rw-rw-rw-  2.0 fat    20070 b- defN 23-Jun-29 11:56 perming/_utils.py
 -rw-rw-rw-  2.0 fat      568 b- defN 23-May-29 16:53 perming/_version.py
--rw-rw-rw-  2.0 fat    10402 b- defN 23-Jun-28 11:36 perming/common.py
--rw-rw-rw-  2.0 fat     5523 b- defN 23-Jun-28 11:35 perming/general.py
--rw-rw-rw-  2.0 fat     7523 b- defN 23-Jun-28 11:42 perming-1.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-28 11:42 perming-1.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-28 11:42 perming-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      746 b- defN 23-Jun-28 11:42 perming-1.2.0.dist-info/RECORD
-10 files, 46031 bytes uncompressed, 11462 bytes compressed:  75.1%
+-rw-rw-rw-  2.0 fat    10505 b- defN 23-Jun-29 11:52 perming/common.py
+-rw-rw-rw-  2.0 fat     5490 b- defN 23-Jun-29 11:38 perming/general.py
+-rw-rw-rw-  2.0 fat     7523 b- defN 23-Jun-29 11:57 perming-1.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-29 11:57 perming-1.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-29 11:57 perming-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      746 b- defN 23-Jun-29 11:57 perming-1.2.1.dist-info/RECORD
+10 files, 46028 bytes uncompressed, 11488 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: perming/common.py
 Comment: 
 
 Filename: perming/general.py
 Comment: 
 
-Filename: perming-1.2.0.dist-info/METADATA
+Filename: perming-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: perming-1.2.0.dist-info/WHEEL
+Filename: perming-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: perming-1.2.0.dist-info/top_level.txt
+Filename: perming-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: perming-1.2.0.dist-info/RECORD
+Filename: perming-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perming/__init__.py

```diff
@@ -19,11 +19,11 @@
 from .common import Regressier, Binarier, Mutipler
 
 GENERAL_BOX = Box
 
 COMMON_MODELS = {
     'Regression': Regressier,
     'Binary-classification': Binarier,
-    'Multi-classification': Mutipler
+    'Multi-classification': Mutipler,
 }
 
-__version__ = '1.2.0'
+__version__ = '1.2.1'
```

## perming/_utils.py

```diff
@@ -157,20 +157,19 @@
         :param worker_set: Dict[str, int], load the configuration of DataLoader with multi-threaded. default: {'train': 8, 'test': 2, 'val': 1}.
         :param random_seed: int | None, random.seed(random_seed) used for fixed random datasets. default: None.
         '''
         assert ratio_set['train'] > 0 and ratio_set['test'] > 0 and ratio_set['val'] > 0
         assert ratio_set['train'] > 4 * ratio_set['test'], "The training set needs to be larger than the test set."
         assert ratio_set['train'] + ratio_set['test'] + ratio_set['val'] == 10, "The sum of 3 datasets' ratio needs to be 10."
         assert isinstance(features, TabularData) and features.ndim == 2, 'Please ensure features with dimension at (n_samples, n_features).'
-        assert features.shape[1] > 1 and features.shape[1] == self.input, "Please ensure `input_` is equal to `features.shape[1]`."
+        assert features.shape[1] == self.input, "Please ensure `input_` is equal to `features.shape[1]`."
         assert isinstance(target, TabularData), "Please ensure target format at numpy.ndarray noted as TabularData."
         if isinstance(target[0], TabularData): # (n_samples, n_outputs)
             raise RuntimeError("data_loader not support target with (n_samples, n_ouputs) yet.")
         else: # (n_samples,)
-            assert len(target.shape) == 1 and target.shape[0] > 0, "Please ensure target is 1d scalar value."
             if self.num_classes >= 2:
                 self.unique = numpy.unique(target) # int indexes -> any class with single value noted
                 assert len(self.unique) == self.num_classes, "Please ensure `num_classes` is equal to `len(numpy.unique(labels))`."
                 self.indices = dict(zip(self.unique, range(self.num_classes))) # original classes -> int indexes
                 target = numpy.array([self.indices[value] for value in target], dtype=numpy.int8) # adjust int8 -> any int dtype
             else:
                 assert str(target.dtype).startswith("float"), "Please ensure target.dtype in any float type of numpy.dtype"
@@ -191,14 +190,15 @@
         :param backend: str, "threading", "multiprocessing, "locky". default: "threading".
         :param n_jobs: int, accelerate processing of validation. default: -1.
         '''
         assert num_epochs > 0 and interval > 0, 'With num_epochs > 0 and interval > 0 to train parameters into outputs.'
         assert n_jobs == -1 or n_jobs > 0, 'Take full jobs with setting n_jobs=-1 or manually set nums of jobs.'
         total_step = len(self.train_loader)
         self._set_container(backend, n_jobs)
+        val_length = len(self.val_container)
         for epoch in range(num_epochs):
             gc.collect()
             torch.cuda.empty_cache()
             for i, (features, target) in enumerate(self.train_loader):
                 features = features.to(self.device)
                 target = target.to(self.device)
 
@@ -214,15 +214,15 @@
                 # validation with val_container
                 self.val_loss = 0
                 with parallel_backend(backend, n_jobs=n_jobs):
                     for val_set in self.val_container:
                         outputs_val = self.model(val_set[0].to(self.device))
                         self.val_loss += self.criterion(outputs_val, val_set[1].to(self.device))
 
-                self.val_loss /= len(self.val_container)
+                self.val_loss /= val_length
 
                 # console print
                 if (i + 1) % interval == 0:
                     print ('Epoch [{}/{}], Step [{}/{}], Training Loss: {:.4f}, Validation Loss: {:.4f}'.format(epoch+1, num_epochs, i+1, total_step, self.train_loss.item(), self.val_loss.item()))
 
     def test(self, 
              sort_by: str='accuracy',
@@ -248,25 +248,25 @@
                 self.test_loss += self.criterion(outputs, target)
             self.test_loss /= test_loader_step
             print('loss of {0} on the {1} test dataset: {2}. accuracy: {3:.4f} %'.format(self.__class__.__name__, test_total, self.test_loss.item(), 100 * correct / test_total))
         return OrderedDict(self._packing(sort_by, sort_state))
     
     def save(self, show: bool=True, dir: str='./model') -> None:
         '''
-        Save Model Checkpoint with Classifier and Regressier.
+        Save Model Checkpoint with Box, Regressier, Binarier, and Multipler.
         :param show: bool, whether to show `model.state_dict()`. default: True.
         :param dir: str, model save to dir. default: './model'.
         '''
         if show:
             print(self.model.state_dict())
         torch.save(self.model.state_dict(), dir)
 
     def load(self, show: bool=True, dir: str='./model') -> None:
         '''
-        Save Model Checkpoint with Classifier and Regressier.
+        Load Model Checkpoint with Box, Regressier, Binarier, and Multipler.
         :param show: bool, whether to show `model.state_dict()`. default: True.
         :param dir: str, model load from dir. default: './model'.
         '''
         params = torch.load(dir)
         self.model.load_state_dict(params)
         if show:
             print(self.model.state_dict())
```

## perming/common.py

```diff
@@ -135,15 +135,15 @@
         if criterion == 'BCELoss':
             return torch.nn.BCELoss()
         elif criterion == 'BCEWithLogitsLoss':
             return torch.nn.BCEWithLogitsLoss()
         else:
             raise ValueError("Criterion Configuration Supports Options: BCELoss, BCEWithLogitsLoss.")
 
-class Mutipler:
+class Mutipler(BaseModel):
     '''
     Mutiple Supervised Learning Classifier for Tabular Data.
     :param input_: int, features' dimension of tabular data is input_.
     :param num_classes: int, total number of correct label categories.
     :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer. default: (100,).
     :param activation: str, configure function that activates the hidden layer. default: relu.
     :param inplace_on: bool, whether to use `inplace=True` on activation. default: False.
@@ -171,15 +171,15 @@
                                        torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
                                        self._activate(activation), 
                                        self._criterion(criterion), 
                                        solver, 
                                        batch_size, 
                                        learning_rate_init, 
                                        lr_scheduler)
-        assert num_classes >= 2
+        assert num_classes >= 2, "The predefined options of Multipler are more suitable for Multi-classification problems."
 
     def _activate(self, activation: str):
         '''
         Configure Activation with `activation` and `inplace_on`.
         :param activation: str, "relu", "rrelu", "leaky_relu", "elu", "celu".
         '''
         if activation == 'relu':
```

## perming/general.py

```diff
@@ -38,15 +38,14 @@
                                   self._device(device), 
                                   self._activate(activation, inplace_on), 
                                   self._criterion(criterion), 
                                   solver, 
                                   batch_size, 
                                   learning_rate_init, 
                                   lr_scheduler)
-        assert num_classes >= 1
 
     def _device(self, option: str) -> None:
         '''
         Set Device for Model and Training.
         :param option: device configuration. str, "cuda" or "cpu".
         '''
         if option == "cuda":
```

## Comparing `perming-1.2.0.dist-info/METADATA` & `perming-1.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perming
-Version: 1.2.0
+Version: 1.2.1
 Summary: The supervised learning framework based on perceptron for tabular data.
 Home-page: https://github.com/linjing-lab/easy-pytorch/tree/main/released_box
 Download-URL: https://github.com/linjing-lab/easy-pytorch/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MPL 2.0
 Project-URL: Source, https://github.com/linjing-lab/easy-pytorch/tree/main/released_box/perming
```

