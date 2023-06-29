# Comparing `tmp/drillvision-0.0.5.tar.gz` & `tmp/drillvision-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drillvision-0.0.5.tar", last modified: Mon Jun 19 21:36:56 2023, max compression
+gzip compressed data, was "drillvision-0.0.6.tar", last modified: Thu Jun 29 18:49:04 2023, max compression
```

## Comparing `drillvision-0.0.5.tar` & `drillvision-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:36:56.092094 drillvision-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-19 21:35:29.000000 drillvision-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-19 21:36:56.092094 drillvision-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-19 21:35:29.000000 drillvision-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:36:56.088094 drillvision-0.0.5/drillvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-19 21:36:55.000000 drillvision-0.0.5/drillvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-19 21:36:56.000000 drillvision-0.0.5/drillvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:36:56.000000 drillvision-0.0.5/drillvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-19 21:36:56.000000 drillvision-0.0.5/drillvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 21:36:56.000000 drillvision-0.0.5/drillvision.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:36:56.088094 drillvision-0.0.5/neural_network_model/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25121 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/bit_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-19 21:35:29.000000 drillvision-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-19 21:35:29.000000 drillvision-0.0.5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-19 21:35:29.000000 drillvision-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 21:36:56.092094 drillvision-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-19 21:35:29.000000 drillvision-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:49:04.650005 drillvision-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-29 18:47:26.000000 drillvision-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-29 18:49:04.650005 drillvision-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-06-29 18:47:26.000000 drillvision-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:49:04.650005 drillvision-0.0.6/drillvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-29 18:49:04.000000 drillvision-0.0.6/drillvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-29 18:49:04.000000 drillvision-0.0.6/drillvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:49:04.000000 drillvision-0.0.6/drillvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-29 18:49:04.000000 drillvision-0.0.6/drillvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 18:49:04.000000 drillvision-0.0.6/drillvision.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:49:04.650005 drillvision-0.0.6/neural_network_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29087 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/bit_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62009 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/cam.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15052 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/script_run_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26981 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/transfer_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-29 18:47:26.000000 drillvision-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 18:47:26.000000 drillvision-0.0.6/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 18:47:26.000000 drillvision-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:49:04.650005 drillvision-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-29 18:47:26.000000 drillvision-0.0.6/setup.py
```

### Comparing `drillvision-0.0.5/PKG-INFO` & `drillvision-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.0.5
+Version: 0.0.6
 Summary: DrillBitVision
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -38,47 +38,64 @@
 It also removes any files that are in the ignore list specified in the SETTING module. 
 The image_dict method returns a dictionary with the number of images and a list of image 
 file paths for each category. The augment_data method augments the images in each 
 category using the ImageDataGenerator class from keras.preprocessing.image module. 
 The augmented images are saved to the dataset_augmented directory.
 
 ### Bit Vision Module
-The BitVision class is designed to train a neural network model for bit vision. It provides various methods for assembling and training the model, as well as performing predictions and visualizations.
-The class has an initialization method that sets the train_test_val_dir attribute, which represents the directory where the training, testing, and validation data is stored. It also initializes other attributes such as model, train_vali_gens, and model_class_indices.
-The categories property returns a list of categories based on the subdirectories in the train_test_val_dir. It filters out any unwanted categories specified in the IGNORE_LIST.
-The data_details property returns a dictionary containing the details of the training, testing, and validation data. It counts the number of files in each category and stores the information in the dictionary.
-The assemble_deep_net_model method creates a sequential model for the neural network. It adds convolutional, batch normalization, max pooling, dropout, and dense layers to the model based on predefined settings.
-The compile_model method compiles the model by specifying the optimizer, loss function, and metrics to be used during training.
-The plot_image_category method plots images from the training data for each category. It accepts parameters such as the number of rows and columns in the plot, the subdirectory (e.g., "train"), and the figure size.
-The _rescaling method is responsible for rescaling the images before training. It uses the ImageDataGenerator class from Keras to rescale the images based on the specified settings.
-The check_points method returns a ModelCheckpoint object, which is used to save the best model during training based on a specified monitor metric.
-The train_model method trains the model using the training and validation data. It uses the fit_generator function to perform the training, specifying various parameters such as the number of epochs, validation data, class weights, and callbacks (including the checkpoint).
-The plot_history method plots the training and validation loss and accuracy over epochs. It generates separate plots for each metric and saves the figure as "history.png".
-The filter_out_list method filters out unwanted elements from a given list based on a predefined ignore list.
-The predict method performs predictions on test images using the trained model. It loads the model, iterates over each category, selects test images, and predicts their labels. It plots the images with their predicted labels and saves the figures in a specified directory.
-The grad_cam_viz method visualizes the class activation heatmap using Grad-CAM. It loads the model, prepares the input image, generates the heatmap using the last convolutional layer, and displays the heatmap along with the original image. The resulting heatmap is saved as an image file.
-Overall, the BitVision class provides functionality for training, evaluating, and visualizing a neural network model for bit vision tasks. It encapsulates the necessary preprocessing steps, model assembly, training process, and prediction visualization, making it convenient to use for bit vision applications.
-
-### Process Module
-```mermaid
-flowchart LR
-
-A[Download Data\n Bing module] --> B[1-find category names\n 2-make an image dictionary]
-B --> C[Augment data] --> D
-D[Train Test  Val Split] --> E[Populate images into the\ntrain test val folders] --> F[Train the model]
-```
 
 
-### Bit Vision Module
-```mermaid
-flowchart LR
-A[Categories\nproperty] --> B[Data Details\nproperty]
-B --> C[Assemble Model] --> D[Compile Model] --> E[Rescale Images\nTrain and Val] 
---> F[Fit Model] --> G[Save Model]
-```
+BitVision is a versatile library initially designed for training, evaluating, and visualizing neural network models specifically tailored to subject with focus on drilling engineering classification tasks. However, it has since evolved to support general classification problems beyond drilling bits. With BitVision, you can effortlessly assemble and train models, make predictions, and generate visualizations for various classification applications, including but not limited to drilling bits.
+- **Model Assembly**: BitVision provides methods to assemble deep neural network models for bit vision tasks. You can add convolutional layers, batch normalization, max pooling, dropout, and dense layers based on predefined settings.
+
+- **Data Preparation**: The library handles data preprocessing tasks such as rescaling images using the ImageDataGenerator class from Keras. It also allows you to obtain details about the training, testing, and validation data, including the number of files in each category.
+
+- **Training and Evaluation**: BitVision simplifies the model training process with the fit_generator function. You can specify the number of epochs, validation data, class weights, and utilize ModelCheckpoint to save the best model based on a chosen metric. Additionally, the library provides methods to plot training and validation loss and accuracy over epochs.
+
+- **Prediction Visualization**: With BitVision, you can easily perform predictions on test images using the trained model. The library facilitates plotting images with their predicted labels and saving the figures for analysis and presentation.
+
+- **Grad-CAM Visualization**: BitVision offers functionality to visualize class activation heatmaps using Grad-CAM. You can overlay the heatmaps on the original images and save the resulting visualizations.
+
+### Transfer Learning Module
+
+The code imports necessary libraries and modules, including TensorFlow, NumPy, pandas, seaborn, and matplotlib.
+The code defines a class called TransferModel that inherits from two other classes: Preprocessing and BitVision. These classes seem to provide additional functionality for data preprocessing and working with images.
+The TransferModel class has several methods for preparing the data, plotting class distributions, analyzing image names, plotting images, performing train-test split, creating data generators, and creating the model.
+The TransferModel class uses the MobileNetV2 architecture for transfer learning. It includes methods for creating data generators using ImageDataGenerator from TensorFlow and training the model.
+
+
+[//]: # (### Process Module)
+
+[//]: # (```mermaid)
+
+[//]: # (flowchart LR)
+
+[//]: # ()
+[//]: # (A[Download Data\n Bing module] --> B[1-find category names\n 2-make an image dictionary])
+
+[//]: # (B --> C[Augment data] --> D)
+
+[//]: # (D[Train Test  Val Split] --> E[Populate images into the\ntrain test val folders] --> F[Train the model])
+
+[//]: # (```)
+
+
+[//]: # (### Bit Vision Module)
+
+[//]: # (```mermaid)
+
+[//]: # (flowchart LR)
+
+[//]: # (A[Categories\nproperty] --> B[Data Details\nproperty])
+
+[//]: # (B --> C[Assemble Model] --> D[Compile Model] --> E[Rescale Images\nTrain and Val] )
+
+[//]: # (--> F[Fit Model] --> G[Save Model])
+
+[//]: # (```)
 
 ## Grad Cam Heatmap - Rollercone Bit
 ![alt text](figures/grad_cam_rc_1.png "Logo Title Text 1")
 
 ## Grad Cam Heatmap - PDC Bit
 ![alt text](figures/grad_cam_pdc_1.png "Logo Title Text 1")
 
@@ -94,51 +111,85 @@
 from neural_network_model.process_data import Preprocessing
 from neural_network_model.bit_vision import BitVision
 
 
 if __name__ == "__main__":
     # download the images
     obj = Preprocessing(dataset_address=Path(__file__).parent / "dataset")
-    obj.download_images(limit=25)
+    obj.download_images(limit=10)
     print(obj.image_dict)
     obj.augment_data(
-        number_of_images_tobe_gen=100,
+        number_of_images_tobe_gen=10,
         augment_data_address=Path(__file__).parent / "augmented_dataset"
     )
     obj.train_test_split(
         augmented_data_address=Path(__file__).parent / "augmented_dataset",
         train_test_val_split_dir_address=Path(__file__).parent / "dataset_train_test_val"
     )
 
     obj = BitVision(train_test_val_dir=Path(__file__).parent / "dataset_train_test_val")
     print(obj.categories)
     print(obj.data_details)
     obj.plot_image_category()
     obj.compile_model()
-
+    #
     model_name = "model_epoch_{epoch:02d}_loss_{loss:.2f}_acc_{accuracy:.2f}_val_acc_{val_accuracy:.2f}_.h5"
     obj.train_model(
+        epochs=8,
         model_save_address=Path(__file__).parent / "deep_model",
-        model_name=model_name,
-        epochs=40,
+        model_name=model_name
     )
     obj.plot_history(fig_folder_address=Path(__file__).parent / "figures")
 
+    best_model = obj.return_best_model_name(directory="deep_model")
+
     obj.predict(
         fig_save_address=Path(__file__).parent / "figures",
-        model_path=Path(__file__).parent / "deep_model" / model_name,
+        model_path=Path(__file__).parent / "deep_model" / best_model,
         test_folder_address=Path(__file__).parent / "dataset_train_test_val" / "test"
     )
 
     # find list of images in the Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     directory_path = Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     list_of_images = [str(x) for x in directory_path.glob("*.jpeg")]
+
     obj.grad_cam_viz(
-        model_path=Path(__file__).parent / "deep_model" / model_name,
+        model_path=Path(__file__).parent / "deep_model" / best_model,
         fig_to_save_address=Path(__file__).parent / "figures",
         img_to_be_applied_path=Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit" / list_of_images[0],
         output_gradcam_fig_name="gradcam.png"
     )
+```
 
+## Using TransferLearning Module
+```python
+from neural_network_model.transfer_learning import TransferModel
+from pathlib import Path
+
+
+transfer_model = TransferModel(
+        dataset_address=Path(__file__).parent / "dataset"
+    )
 
+transfer_model.plot_classes_number()
+transfer_model.analyze_image_names()
+transfer_model.plot_data_images(num_rows=3, num_cols=3)
+transfer_model.train_model()
+transfer_model.plot_metrics_results()
+transfer_model.results()
+transfer_model.predcit_test()
+transfer_model.grad_cam_viz(num_rows=3, num_cols=2)
+```
+
+Note that the dataset structure should be as follows:
+```
+├── dataset
+│   ├── class 1
+│   └── class 2
+│   └── class 3
+│   └── class .
+│   └── class .
+│   └── class .
+│   └── class N      
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `drillvision-0.0.5/README.md` & `drillvision-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -23,47 +23,64 @@
 It also removes any files that are in the ignore list specified in the SETTING module. 
 The image_dict method returns a dictionary with the number of images and a list of image 
 file paths for each category. The augment_data method augments the images in each 
 category using the ImageDataGenerator class from keras.preprocessing.image module. 
 The augmented images are saved to the dataset_augmented directory.
 
 ### Bit Vision Module
-The BitVision class is designed to train a neural network model for bit vision. It provides various methods for assembling and training the model, as well as performing predictions and visualizations.
-The class has an initialization method that sets the train_test_val_dir attribute, which represents the directory where the training, testing, and validation data is stored. It also initializes other attributes such as model, train_vali_gens, and model_class_indices.
-The categories property returns a list of categories based on the subdirectories in the train_test_val_dir. It filters out any unwanted categories specified in the IGNORE_LIST.
-The data_details property returns a dictionary containing the details of the training, testing, and validation data. It counts the number of files in each category and stores the information in the dictionary.
-The assemble_deep_net_model method creates a sequential model for the neural network. It adds convolutional, batch normalization, max pooling, dropout, and dense layers to the model based on predefined settings.
-The compile_model method compiles the model by specifying the optimizer, loss function, and metrics to be used during training.
-The plot_image_category method plots images from the training data for each category. It accepts parameters such as the number of rows and columns in the plot, the subdirectory (e.g., "train"), and the figure size.
-The _rescaling method is responsible for rescaling the images before training. It uses the ImageDataGenerator class from Keras to rescale the images based on the specified settings.
-The check_points method returns a ModelCheckpoint object, which is used to save the best model during training based on a specified monitor metric.
-The train_model method trains the model using the training and validation data. It uses the fit_generator function to perform the training, specifying various parameters such as the number of epochs, validation data, class weights, and callbacks (including the checkpoint).
-The plot_history method plots the training and validation loss and accuracy over epochs. It generates separate plots for each metric and saves the figure as "history.png".
-The filter_out_list method filters out unwanted elements from a given list based on a predefined ignore list.
-The predict method performs predictions on test images using the trained model. It loads the model, iterates over each category, selects test images, and predicts their labels. It plots the images with their predicted labels and saves the figures in a specified directory.
-The grad_cam_viz method visualizes the class activation heatmap using Grad-CAM. It loads the model, prepares the input image, generates the heatmap using the last convolutional layer, and displays the heatmap along with the original image. The resulting heatmap is saved as an image file.
-Overall, the BitVision class provides functionality for training, evaluating, and visualizing a neural network model for bit vision tasks. It encapsulates the necessary preprocessing steps, model assembly, training process, and prediction visualization, making it convenient to use for bit vision applications.
-
-### Process Module
-```mermaid
-flowchart LR
-
-A[Download Data\n Bing module] --> B[1-find category names\n 2-make an image dictionary]
-B --> C[Augment data] --> D
-D[Train Test  Val Split] --> E[Populate images into the\ntrain test val folders] --> F[Train the model]
-```
 
 
-### Bit Vision Module
-```mermaid
-flowchart LR
-A[Categories\nproperty] --> B[Data Details\nproperty]
-B --> C[Assemble Model] --> D[Compile Model] --> E[Rescale Images\nTrain and Val] 
---> F[Fit Model] --> G[Save Model]
-```
+BitVision is a versatile library initially designed for training, evaluating, and visualizing neural network models specifically tailored to subject with focus on drilling engineering classification tasks. However, it has since evolved to support general classification problems beyond drilling bits. With BitVision, you can effortlessly assemble and train models, make predictions, and generate visualizations for various classification applications, including but not limited to drilling bits.
+- **Model Assembly**: BitVision provides methods to assemble deep neural network models for bit vision tasks. You can add convolutional layers, batch normalization, max pooling, dropout, and dense layers based on predefined settings.
+
+- **Data Preparation**: The library handles data preprocessing tasks such as rescaling images using the ImageDataGenerator class from Keras. It also allows you to obtain details about the training, testing, and validation data, including the number of files in each category.
+
+- **Training and Evaluation**: BitVision simplifies the model training process with the fit_generator function. You can specify the number of epochs, validation data, class weights, and utilize ModelCheckpoint to save the best model based on a chosen metric. Additionally, the library provides methods to plot training and validation loss and accuracy over epochs.
+
+- **Prediction Visualization**: With BitVision, you can easily perform predictions on test images using the trained model. The library facilitates plotting images with their predicted labels and saving the figures for analysis and presentation.
+
+- **Grad-CAM Visualization**: BitVision offers functionality to visualize class activation heatmaps using Grad-CAM. You can overlay the heatmaps on the original images and save the resulting visualizations.
+
+### Transfer Learning Module
+
+The code imports necessary libraries and modules, including TensorFlow, NumPy, pandas, seaborn, and matplotlib.
+The code defines a class called TransferModel that inherits from two other classes: Preprocessing and BitVision. These classes seem to provide additional functionality for data preprocessing and working with images.
+The TransferModel class has several methods for preparing the data, plotting class distributions, analyzing image names, plotting images, performing train-test split, creating data generators, and creating the model.
+The TransferModel class uses the MobileNetV2 architecture for transfer learning. It includes methods for creating data generators using ImageDataGenerator from TensorFlow and training the model.
+
+
+[//]: # (### Process Module)
+
+[//]: # (```mermaid)
+
+[//]: # (flowchart LR)
+
+[//]: # ()
+[//]: # (A[Download Data\n Bing module] --> B[1-find category names\n 2-make an image dictionary])
+
+[//]: # (B --> C[Augment data] --> D)
+
+[//]: # (D[Train Test  Val Split] --> E[Populate images into the\ntrain test val folders] --> F[Train the model])
+
+[//]: # (```)
+
+
+[//]: # (### Bit Vision Module)
+
+[//]: # (```mermaid)
+
+[//]: # (flowchart LR)
+
+[//]: # (A[Categories\nproperty] --> B[Data Details\nproperty])
+
+[//]: # (B --> C[Assemble Model] --> D[Compile Model] --> E[Rescale Images\nTrain and Val] )
+
+[//]: # (--> F[Fit Model] --> G[Save Model])
+
+[//]: # (```)
 
 ## Grad Cam Heatmap - Rollercone Bit
 ![alt text](figures/grad_cam_rc_1.png "Logo Title Text 1")
 
 ## Grad Cam Heatmap - PDC Bit
 ![alt text](figures/grad_cam_pdc_1.png "Logo Title Text 1")
 
@@ -79,49 +96,83 @@
 from neural_network_model.process_data import Preprocessing
 from neural_network_model.bit_vision import BitVision
 
 
 if __name__ == "__main__":
     # download the images
     obj = Preprocessing(dataset_address=Path(__file__).parent / "dataset")
-    obj.download_images(limit=25)
+    obj.download_images(limit=10)
     print(obj.image_dict)
     obj.augment_data(
-        number_of_images_tobe_gen=100,
+        number_of_images_tobe_gen=10,
         augment_data_address=Path(__file__).parent / "augmented_dataset"
     )
     obj.train_test_split(
         augmented_data_address=Path(__file__).parent / "augmented_dataset",
         train_test_val_split_dir_address=Path(__file__).parent / "dataset_train_test_val"
     )
 
     obj = BitVision(train_test_val_dir=Path(__file__).parent / "dataset_train_test_val")
     print(obj.categories)
     print(obj.data_details)
     obj.plot_image_category()
     obj.compile_model()
-
+    #
     model_name = "model_epoch_{epoch:02d}_loss_{loss:.2f}_acc_{accuracy:.2f}_val_acc_{val_accuracy:.2f}_.h5"
     obj.train_model(
+        epochs=8,
         model_save_address=Path(__file__).parent / "deep_model",
-        model_name=model_name,
-        epochs=40,
+        model_name=model_name
     )
     obj.plot_history(fig_folder_address=Path(__file__).parent / "figures")
 
+    best_model = obj.return_best_model_name(directory="deep_model")
+
     obj.predict(
         fig_save_address=Path(__file__).parent / "figures",
-        model_path=Path(__file__).parent / "deep_model" / model_name,
+        model_path=Path(__file__).parent / "deep_model" / best_model,
         test_folder_address=Path(__file__).parent / "dataset_train_test_val" / "test"
     )
 
     # find list of images in the Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     directory_path = Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     list_of_images = [str(x) for x in directory_path.glob("*.jpeg")]
+
     obj.grad_cam_viz(
-        model_path=Path(__file__).parent / "deep_model" / model_name,
+        model_path=Path(__file__).parent / "deep_model" / best_model,
         fig_to_save_address=Path(__file__).parent / "figures",
         img_to_be_applied_path=Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit" / list_of_images[0],
         output_gradcam_fig_name="gradcam.png"
     )
+```
 
+## Using TransferLearning Module
+```python
+from neural_network_model.transfer_learning import TransferModel
+from pathlib import Path
+
+
+transfer_model = TransferModel(
+        dataset_address=Path(__file__).parent / "dataset"
+    )
 
+transfer_model.plot_classes_number()
+transfer_model.analyze_image_names()
+transfer_model.plot_data_images(num_rows=3, num_cols=3)
+transfer_model.train_model()
+transfer_model.plot_metrics_results()
+transfer_model.results()
+transfer_model.predcit_test()
+transfer_model.grad_cam_viz(num_rows=3, num_cols=2)
+```
+
+Note that the dataset structure should be as follows:
+```
+├── dataset
+│   ├── class 1
+│   └── class 2
+│   └── class 3
+│   └── class .
+│   └── class .
+│   └── class .
+│   └── class N      
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `drillvision-0.0.5/drillvision.egg-info/PKG-INFO` & `drillvision-0.0.6/drillvision.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.0.5
+Version: 0.0.6
 Summary: DrillBitVision
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -38,47 +38,64 @@
 It also removes any files that are in the ignore list specified in the SETTING module. 
 The image_dict method returns a dictionary with the number of images and a list of image 
 file paths for each category. The augment_data method augments the images in each 
 category using the ImageDataGenerator class from keras.preprocessing.image module. 
 The augmented images are saved to the dataset_augmented directory.
 
 ### Bit Vision Module
-The BitVision class is designed to train a neural network model for bit vision. It provides various methods for assembling and training the model, as well as performing predictions and visualizations.
-The class has an initialization method that sets the train_test_val_dir attribute, which represents the directory where the training, testing, and validation data is stored. It also initializes other attributes such as model, train_vali_gens, and model_class_indices.
-The categories property returns a list of categories based on the subdirectories in the train_test_val_dir. It filters out any unwanted categories specified in the IGNORE_LIST.
-The data_details property returns a dictionary containing the details of the training, testing, and validation data. It counts the number of files in each category and stores the information in the dictionary.
-The assemble_deep_net_model method creates a sequential model for the neural network. It adds convolutional, batch normalization, max pooling, dropout, and dense layers to the model based on predefined settings.
-The compile_model method compiles the model by specifying the optimizer, loss function, and metrics to be used during training.
-The plot_image_category method plots images from the training data for each category. It accepts parameters such as the number of rows and columns in the plot, the subdirectory (e.g., "train"), and the figure size.
-The _rescaling method is responsible for rescaling the images before training. It uses the ImageDataGenerator class from Keras to rescale the images based on the specified settings.
-The check_points method returns a ModelCheckpoint object, which is used to save the best model during training based on a specified monitor metric.
-The train_model method trains the model using the training and validation data. It uses the fit_generator function to perform the training, specifying various parameters such as the number of epochs, validation data, class weights, and callbacks (including the checkpoint).
-The plot_history method plots the training and validation loss and accuracy over epochs. It generates separate plots for each metric and saves the figure as "history.png".
-The filter_out_list method filters out unwanted elements from a given list based on a predefined ignore list.
-The predict method performs predictions on test images using the trained model. It loads the model, iterates over each category, selects test images, and predicts their labels. It plots the images with their predicted labels and saves the figures in a specified directory.
-The grad_cam_viz method visualizes the class activation heatmap using Grad-CAM. It loads the model, prepares the input image, generates the heatmap using the last convolutional layer, and displays the heatmap along with the original image. The resulting heatmap is saved as an image file.
-Overall, the BitVision class provides functionality for training, evaluating, and visualizing a neural network model for bit vision tasks. It encapsulates the necessary preprocessing steps, model assembly, training process, and prediction visualization, making it convenient to use for bit vision applications.
-
-### Process Module
-```mermaid
-flowchart LR
-
-A[Download Data\n Bing module] --> B[1-find category names\n 2-make an image dictionary]
-B --> C[Augment data] --> D
-D[Train Test  Val Split] --> E[Populate images into the\ntrain test val folders] --> F[Train the model]
-```
 
 
-### Bit Vision Module
-```mermaid
-flowchart LR
-A[Categories\nproperty] --> B[Data Details\nproperty]
-B --> C[Assemble Model] --> D[Compile Model] --> E[Rescale Images\nTrain and Val] 
---> F[Fit Model] --> G[Save Model]
-```
+BitVision is a versatile library initially designed for training, evaluating, and visualizing neural network models specifically tailored to subject with focus on drilling engineering classification tasks. However, it has since evolved to support general classification problems beyond drilling bits. With BitVision, you can effortlessly assemble and train models, make predictions, and generate visualizations for various classification applications, including but not limited to drilling bits.
+- **Model Assembly**: BitVision provides methods to assemble deep neural network models for bit vision tasks. You can add convolutional layers, batch normalization, max pooling, dropout, and dense layers based on predefined settings.
+
+- **Data Preparation**: The library handles data preprocessing tasks such as rescaling images using the ImageDataGenerator class from Keras. It also allows you to obtain details about the training, testing, and validation data, including the number of files in each category.
+
+- **Training and Evaluation**: BitVision simplifies the model training process with the fit_generator function. You can specify the number of epochs, validation data, class weights, and utilize ModelCheckpoint to save the best model based on a chosen metric. Additionally, the library provides methods to plot training and validation loss and accuracy over epochs.
+
+- **Prediction Visualization**: With BitVision, you can easily perform predictions on test images using the trained model. The library facilitates plotting images with their predicted labels and saving the figures for analysis and presentation.
+
+- **Grad-CAM Visualization**: BitVision offers functionality to visualize class activation heatmaps using Grad-CAM. You can overlay the heatmaps on the original images and save the resulting visualizations.
+
+### Transfer Learning Module
+
+The code imports necessary libraries and modules, including TensorFlow, NumPy, pandas, seaborn, and matplotlib.
+The code defines a class called TransferModel that inherits from two other classes: Preprocessing and BitVision. These classes seem to provide additional functionality for data preprocessing and working with images.
+The TransferModel class has several methods for preparing the data, plotting class distributions, analyzing image names, plotting images, performing train-test split, creating data generators, and creating the model.
+The TransferModel class uses the MobileNetV2 architecture for transfer learning. It includes methods for creating data generators using ImageDataGenerator from TensorFlow and training the model.
+
+
+[//]: # (### Process Module)
+
+[//]: # (```mermaid)
+
+[//]: # (flowchart LR)
+
+[//]: # ()
+[//]: # (A[Download Data\n Bing module] --> B[1-find category names\n 2-make an image dictionary])
+
+[//]: # (B --> C[Augment data] --> D)
+
+[//]: # (D[Train Test  Val Split] --> E[Populate images into the\ntrain test val folders] --> F[Train the model])
+
+[//]: # (```)
+
+
+[//]: # (### Bit Vision Module)
+
+[//]: # (```mermaid)
+
+[//]: # (flowchart LR)
+
+[//]: # (A[Categories\nproperty] --> B[Data Details\nproperty])
+
+[//]: # (B --> C[Assemble Model] --> D[Compile Model] --> E[Rescale Images\nTrain and Val] )
+
+[//]: # (--> F[Fit Model] --> G[Save Model])
+
+[//]: # (```)
 
 ## Grad Cam Heatmap - Rollercone Bit
 ![alt text](figures/grad_cam_rc_1.png "Logo Title Text 1")
 
 ## Grad Cam Heatmap - PDC Bit
 ![alt text](figures/grad_cam_pdc_1.png "Logo Title Text 1")
 
@@ -94,51 +111,85 @@
 from neural_network_model.process_data import Preprocessing
 from neural_network_model.bit_vision import BitVision
 
 
 if __name__ == "__main__":
     # download the images
     obj = Preprocessing(dataset_address=Path(__file__).parent / "dataset")
-    obj.download_images(limit=25)
+    obj.download_images(limit=10)
     print(obj.image_dict)
     obj.augment_data(
-        number_of_images_tobe_gen=100,
+        number_of_images_tobe_gen=10,
         augment_data_address=Path(__file__).parent / "augmented_dataset"
     )
     obj.train_test_split(
         augmented_data_address=Path(__file__).parent / "augmented_dataset",
         train_test_val_split_dir_address=Path(__file__).parent / "dataset_train_test_val"
     )
 
     obj = BitVision(train_test_val_dir=Path(__file__).parent / "dataset_train_test_val")
     print(obj.categories)
     print(obj.data_details)
     obj.plot_image_category()
     obj.compile_model()
-
+    #
     model_name = "model_epoch_{epoch:02d}_loss_{loss:.2f}_acc_{accuracy:.2f}_val_acc_{val_accuracy:.2f}_.h5"
     obj.train_model(
+        epochs=8,
         model_save_address=Path(__file__).parent / "deep_model",
-        model_name=model_name,
-        epochs=40,
+        model_name=model_name
     )
     obj.plot_history(fig_folder_address=Path(__file__).parent / "figures")
 
+    best_model = obj.return_best_model_name(directory="deep_model")
+
     obj.predict(
         fig_save_address=Path(__file__).parent / "figures",
-        model_path=Path(__file__).parent / "deep_model" / model_name,
+        model_path=Path(__file__).parent / "deep_model" / best_model,
         test_folder_address=Path(__file__).parent / "dataset_train_test_val" / "test"
     )
 
     # find list of images in the Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     directory_path = Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     list_of_images = [str(x) for x in directory_path.glob("*.jpeg")]
+
     obj.grad_cam_viz(
-        model_path=Path(__file__).parent / "deep_model" / model_name,
+        model_path=Path(__file__).parent / "deep_model" / best_model,
         fig_to_save_address=Path(__file__).parent / "figures",
         img_to_be_applied_path=Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit" / list_of_images[0],
         output_gradcam_fig_name="gradcam.png"
     )
+```
 
+## Using TransferLearning Module
+```python
+from neural_network_model.transfer_learning import TransferModel
+from pathlib import Path
+
+
+transfer_model = TransferModel(
+        dataset_address=Path(__file__).parent / "dataset"
+    )
 
+transfer_model.plot_classes_number()
+transfer_model.analyze_image_names()
+transfer_model.plot_data_images(num_rows=3, num_cols=3)
+transfer_model.train_model()
+transfer_model.plot_metrics_results()
+transfer_model.results()
+transfer_model.predcit_test()
+transfer_model.grad_cam_viz(num_rows=3, num_cols=2)
+```
+
+Note that the dataset structure should be as follows:
+```
+├── dataset
+│   ├── class 1
+│   └── class 2
+│   └── class 3
+│   └── class .
+│   └── class .
+│   └── class .
+│   └── class N      
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `drillvision-0.0.5/drillvision.egg-info/SOURCES.txt` & `drillvision-0.0.6/drillvision.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,21 +5,26 @@
 requirements.txt
 setup.py
 ./requirements-test.txt
 ./requirements.txt
 ./neural_network_model/VERSION
 ./neural_network_model/__init__.py
 ./neural_network_model/bit_vision.py
+./neural_network_model/cam.jpg
 ./neural_network_model/model.py
 ./neural_network_model/process_data.py
 ./neural_network_model/s3.py
+./neural_network_model/script_run_all.py
+./neural_network_model/transfer_learning.py
 drillvision.egg-info/PKG-INFO
 drillvision.egg-info/SOURCES.txt
 drillvision.egg-info/dependency_links.txt
 drillvision.egg-info/requires.txt
 drillvision.egg-info/top_level.txt
 neural_network_model/VERSION
 neural_network_model/__init__.py
 neural_network_model/bit_vision.py
 neural_network_model/model.py
 neural_network_model/process_data.py
-neural_network_model/s3.py
+neural_network_model/s3.py
+neural_network_model/script_run_all.py
+neural_network_model/transfer_learning.py
```

### Comparing `drillvision-0.0.5/neural_network_model/bit_vision.py` & `drillvision-0.0.6/neural_network_model/bit_vision.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,37 @@
 import math
 import os
 import random
 import warnings
 from pathlib import Path
 from typing import Dict, List
 
-import numpy as np
-import tensorflow
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
+import numpy as np
+import tensorflow
 import tensorflow as tf
+from keras import Sequential
+from keras.callbacks import ModelCheckpoint
+from keras.layers import (
+    BatchNormalization,
+    Conv2D,
+    Dense,
+    Dropout,
+    Flatten,
+    MaxPooling2D,
+)
 from tensorflow import keras
 from tensorflow.keras.applications.resnet50 import decode_predictions, preprocess_input
 from tensorflow.keras.preprocessing import image
-from tensorflow.keras.preprocessing.image import ImageDataGenerator, img_to_array, load_img
-from keras import Sequential
-from keras.callbacks import ModelCheckpoint
-from keras.layers import BatchNormalization, Conv2D, Dense, Dropout, Flatten, MaxPooling2D
+from tensorflow.keras.preprocessing.image import (
+    ImageDataGenerator,
+    img_to_array,
+    load_img,
+)
 
 from neural_network_model.model import SETTING
 
 # Set seed to get the same random numbers each time
 random.seed(1)
 
 # Initialize the logger
@@ -45,19 +56,21 @@
 
 class BitVision:
     """
     This class is used to train a neural network model for bit vision.
     """
 
     def __init__(self, *args, **kwargs):
+        self.layer_names: Dict[str, List] = {}
         self.train_test_val_dir: str = kwargs.get(
             "train_test_val_dir",
             SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS,
         )
         self.model: tensorflow.keras.models.Sequential = None
+        # by default the following model is assembled
         self.assemble_deep_net_model()
         self.train_val_gens = {}
         self.model_history = None
         self.model_class_indices: Dict[str, int] = {}
 
     @property
     def categories(self) -> List[str]:
@@ -107,19 +120,26 @@
                 data[subdir][category] = num_files
         return data
 
     def assemble_deep_net_model(self) -> tensorflow.keras.models.Sequential:
         """
         This function is used to assemble the deep net model.
         """
+        image_size = SETTING.FLOW_FROM_DIRECTORY_SETTING.IMAGE_SIZE
+
         model = Sequential()
         activ = "relu"
 
         model.add(
-            Conv2D(32, kernel_size=(3, 3), activation=activ, input_shape=(224, 224, 3))
+            Conv2D(
+                32,
+                kernel_size=(3, 3),
+                activation=activ,
+                input_shape=(image_size, image_size, 3),
+            )
         )
         model.add(BatchNormalization())
 
         model.add(Conv2D(64, kernel_size=(3, 3), activation=activ))
         model.add(BatchNormalization())
         model.add(MaxPooling2D(pool_size=(2, 2)))
         model.add(Dropout(0.5))
@@ -132,48 +152,116 @@
         model.add(Flatten())
         model.add(Dense(64, activation=activ))
         model.add(Dropout(0.5))
         model.add(Dense(len(self.categories), activation="softmax"))
         self.model = model
         return self.model
 
+    def assemble_deep_net_model_2(self) -> tensorflow.keras.models.Sequential:
+        """
+        This function is used to assemble the deep net model.
+        """
+
+        image_size = SETTING.FLOW_FROM_DIRECTORY_SETTING.IMAGE_SIZE
+
+        kernel_size = (3, 3)
+        pool_size = (2, 2)
+        first_filters = 32
+        second_filters = 64
+        third_filters = 128
+
+        dropout_conv = 0.3
+        dropout_dense = 0.3
+
+        model = Sequential()
+        model.add(
+            Conv2D(
+                first_filters,
+                kernel_size,
+                activation="relu",
+                input_shape=(image_size, image_size, 3),
+            )
+        )
+        model.add(Conv2D(first_filters, kernel_size, activation="relu"))
+        model.add((MaxPooling2D(pool_size=pool_size)))
+        model.add(Dropout(dropout_conv))
+
+        model.add(Conv2D(second_filters, kernel_size, activation="relu"))
+        model.add(Conv2D(second_filters, kernel_size, activation="relu"))
+        model.add((MaxPooling2D(pool_size=pool_size)))
+        model.add(Dropout(dropout_conv))
+
+        model.add(Conv2D(third_filters, kernel_size, activation="relu"))
+        model.add(Conv2D(third_filters, kernel_size, activation="relu"))
+        model.add((MaxPooling2D(pool_size=pool_size)))
+        model.add(Dropout(dropout_conv))
+
+        model.add(Flatten())
+        model.add(Dense(256, activation="relu"))
+        model.add(Dropout(dropout_dense))
+        model.add(Dense(len(self.categories), activation="softmax"))
+
+        self.model = model
+        return self.model
+
     def compile_model(self, *args, **kwargs) -> None:
         """
         This function is used to compile the model.
         :return:
         """
         self.model.compile(
             optimizer=keras.optimizers.Adam(1e-3),
             loss=SETTING.MODEL_SETTING.LOSS,
             metrics=SETTING.MODEL_SETTING.METRICS,
         )
 
         self.model.summary()
 
+        # Initialize the dictionary
+        layer_names = {"conv_layer": [], "other_layer": []}
+
+        # Iterate over the model layers and store the names
+        for idx in range(len(self.model.layers)):
+            layer_name = self.model.get_layer(index=idx).name
+
+            # Check if the layer name contains 'conv' substring
+            if "conv" in layer_name.lower():
+                layer_names["conv_layer"].append(layer_name)
+            else:
+                layer_names["other_layer"].append(layer_name)
+
+        self.layer_names = layer_names
+
     def plot_image_category(self, *args, **kwargs) -> None:
-        """
-        This function is used to plot images.
-        :param images: list of images
-        :param labels: list of labels
-        :return:
-        """
         nrows = kwargs.get("nrows", 1)
         number_of_categories = len(self.categories)
         ncols = kwargs.get("ncols", number_of_categories)
         subdir = kwargs.get("subdir", "train")
         fig_size = kwargs.get("fig_size", (17, 10))
 
-        # get one image for each category in train data and plot them
+        # Get one image for each category in train data and plot them
         fig, axs = plt.subplots(nrows, ncols, figsize=fig_size)
-        for category in self.categories:
+
+        if nrows == 1 and ncols > 1:
+            axs = axs.reshape(
+                (ncols,)
+            )  # Reshape axs to handle 1 row and multiple columns
+
+        for i, category in enumerate(self.categories):
             category_path = self.train_test_val_dir / subdir / category
             image_path = category_path / os.listdir(category_path)[1]
             img = load_img(image_path)
-            axs[self.categories.index(category)].imshow(img)
-            axs[self.categories.index(category)].set_title(category)
+
+            if nrows == 1 and ncols > 1:
+                axs[i].imshow(img)  # Use 1D indexing for 1 row and multiple columns
+                axs[i].set_title(category)
+            else:
+                axs[i // ncols, i % ncols].imshow(img)  # Adjusted indexing
+                axs[i // ncols, i % ncols].set_title(category)  # Adjusted indexing
+
         plt.show()
 
     def _rescaling(self) -> None:
         """
         This function is used to rescale the images.
         The images were augmented before in the preprocessing step.
         Here we just rescale them.
@@ -213,23 +301,40 @@
         check_point = ModelCheckpoint(
             model_save_address / model_name,
             monitor=SETTING.MODEL_SETTING.MONITOR,
             verbose=SETTING.MODEL_SETTING.CHECK_POINT_VERBOSE,
             save_best_only=SETTING.MODEL_SETTING.SAVE_BEST_ONLY,
             mode=SETTING.MODEL_SETTING.MODE,
             period=SETTING.MODEL_SETTING.PERIOD,
+            metrics=SETTING.MODEL_SETTING.METRICS,
         )
         return check_point
 
     def _calculate_number_from_dict(self, my_dict: dict) -> int:
         total = sum(my_dict.values())
         return total
 
+    def _calculate_class_weight(self, class_counts: dict) -> dict:
+        class_labels = list(class_counts.keys())
+        class_indices = {label: index for index, label in enumerate(class_labels)}
+
+        total_samples = sum(class_counts.values())
+        class_weight = {}
+        for class_label, count in class_counts.items():
+            class_index = class_indices[class_label]
+            class_weight[class_index] = total_samples / (len(class_counts) * count)
+
+        # Normalize the class weights
+        class_weight_sum = sum(class_weight.values())
+        for class_index in class_weight:
+            class_weight[class_index] /= class_weight_sum
+        return class_weight
+
     def train_model(
-        self, model_save_address: str = SETTING.MODEL_SETTING.MODEL_PATH, **kwargs
+        self, model_save_address: Path = SETTING.MODEL_SETTING.MODEL_PATH, **kwargs
     ) -> None:
         """
         This function is used to train the model.
         :param model_save_address:
         :param kwargs: model_name, epochs, verbose, class_weight, workers, use_multiprocessing, shuffle
         :return:
         """
@@ -244,41 +349,40 @@
         )
         shuffle = kwargs.get("shuffle", SETTING.MODEL_SETTING.SHUFFLE)
 
         # calculate validation_steps
         BATCH_SIZE = SETTING.FLOW_FROM_DIRECTORY_SETTING.BATCH_SIZE
         TRAINING_SIZE = self._calculate_number_from_dict(self.data_details["train"])
         VALIDATION_SIZE = self._calculate_number_from_dict(self.data_details["val"])
+
+        if not class_weight:
+            class_weight = self._calculate_class_weight(self.data_details["train"])
+
         # We take the ceiling because we do not drop the remainder of the batch
         compute_steps_per_epoch = lambda x: int(math.ceil(1.0 * x / BATCH_SIZE))
         steps_per_epoch = compute_steps_per_epoch(TRAINING_SIZE)
         val_steps = compute_steps_per_epoch(VALIDATION_SIZE)
 
         self._rescaling()
         self.model_history = self.model.fit_generator(
             steps_per_epoch=steps_per_epoch,
             generator=self.train_val_gens["train"],
-            epochs=epochs or SETTING.MODEL_SETTING.EPOCHS,
-            verbose=verbose or SETTING.MODEL_SETTING.FIT_GEN_VERBOSE,
+            epochs=epochs,
+            verbose=verbose,
             validation_data=self.train_val_gens["val"],
-            validation_steps=val_steps or SETTING.MODEL_SETTING.VALIDATION_STEPS,
-            class_weight=class_weight or SETTING.MODEL_SETTING.CLASS_WEIGHT,
+            validation_steps=val_steps,
+            class_weight=class_weight,
             max_queue_size=SETTING.MODEL_SETTING.MAX_QUEUE_SIZE,
-            workers=workers or SETTING.MODEL_SETTING.WORKERS,
-            use_multiprocessing=use_multiprocessing
-            or SETTING.MODEL_SETTING.USE_MULTIPROCESSING,
-            shuffle=shuffle or SETTING.MODEL_SETTING.SHUFFLE,
+            workers=workers,
+            use_multiprocessing=use_multiprocessing,
+            shuffle=shuffle,
             initial_epoch=SETTING.MODEL_SETTING.INITIAL_EPOCH,
             callbacks=[self._check_points(model_save_address, model_name)],
         )
 
-        self.model.save(
-            model_save_address / model_name
-            or SETTING.MODEL_SETTING.MODEL_PATH / SETTING.MODEL_SETTING.MODEL_NAME
-        )
         logger.info(f"Model saved to {SETTING.MODEL_SETTING.MODEL_PATH}")
 
     def plot_history(self, *args, **kwargs):
         """
         This function is used to plot the history of the model.
         :param fig_folder_address: the address of the folder to save the figure
         :return:
@@ -318,15 +422,16 @@
             if case in list_to_be_edited:
                 list_to_be_edited.remove(case)
         return list_to_be_edited
 
     def predict(self, *args, **kwargs):
         """
         This function is used to predict the test data.
-        :param args:
+        :param args: test_folder_dir needs to have a suborder called test and there needs to have categories folders
+        same structure as train_test_val directory
         :param kwargs: fig_save_address: the address of the folder to save the figure,
         model_path: the path of the model to be used for prediction
         :return:
         """
         fig_save_address = kwargs.get(
             "fig_save_address", SETTING.FIGURE_SETTING.FIG_PRED_OUT_DIR_ADDRESS
         )
@@ -336,44 +441,45 @@
         model_path = kwargs.get(
             "model_path",
             SETTING.MODEL_SETTING.MODEL_PATH / SETTING.MODEL_SETTING.MODEL_NAME,
         )
         if model_path is None:
             logger.info(f"model_path from SETTING is was used - {model_path}")
 
-        test_folder_address = kwargs.get(
-            "test_folder_address", SETTING.DATA_ADDRESS_SETTING.TEST_DIR_ADDRESS
-        )
-        if test_folder_address is None:
-            raise ValueError("test_folder_address is None")
-
         model = keras.models.load_model(model_path)
         logger.info(f"Model loaded from {model_path}")
 
+        # Default settings
+        default_num_rows = SETTING.FIGURE_SETTING.NUM_ROWS_IN_PRED_MODEL
+        default_num_cols = SETTING.FIGURE_SETTING.NUM_COLS_IN_PRED_MODEL
+        default_figsize = SETTING.FIGURE_SETTING.FIGURE_SIZE_IN_PRED_MODEL
+
+        # Extract details from kwargs or use default settings
+        num_rows = kwargs.get("num_rows", default_num_rows)
+        num_cols = kwargs.get("num_cols", default_num_cols)
+        figure_size = kwargs.get("figure_size", default_figsize)
+
         for category in self.categories:
-            plt.figure(figsize=SETTING.FIGURE_SETTING.FIGURE_SIZE_IN_PRED_MODEL)
-            number_of_cols = SETTING.FIGURE_SETTING.NUM_COLS_IN_PRED_MODEL
-            number_of_rows = SETTING.FIGURE_SETTING.NUM_ROWS_IN_PRED_MODEL
+            plt.figure(figsize=figure_size)
+            number_of_cols = num_cols
+            number_of_rows = num_rows
             number_of_test_to_pred = SETTING.MODEL_SETTING.NUMBER_OF_TEST_TO_PRED
-            train_test_val_dir = (
-                self.train_test_val_dir
-                or SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
-            )
+
             # get the list of test images
             test_images_list = os.listdir(
-                train_test_val_dir
+                self.train_test_val_dir
                 / SETTING.PREPROCESSING_SETTING.TRAIN_TEST_SPLIT_DIR_NAMES[1]
                 / category
             )
             # check if .DS_Store is in the list if so remove it
             test_images_list = self._filter_out_list(list_to_be_edited=test_images_list)
 
             for i, img in enumerate(test_images_list[0:number_of_test_to_pred]):
                 path_to_img = (
-                    train_test_val_dir
+                    self.train_test_val_dir
                     / SETTING.PREPROCESSING_SETTING.TRAIN_TEST_SPLIT_DIR_NAMES[1]
                     / category
                     / str(img)
                 ).resolve()
 
                 img = load_img(
                     path_to_img,
@@ -410,15 +516,15 @@
                 os.makedirs(fig_path.parent)
             plt.savefig(fig_path)
             plt.show()
             plt.tight_layout()
 
         datagen = image.ImageDataGenerator(SETTING.DATA_GEN_SETTING.RESCALE)
         DoubleCheck_generator = datagen.flow_from_directory(
-            directory=test_folder_address,
+            directory=self.train_test_val_dir / "test",
             target_size=SETTING.FLOW_FROM_DIRECTORY_SETTING.TARGET_SIZE,
             color_mode=SETTING.FLOW_FROM_DIRECTORY_SETTING.COLOR_MODE,
             classes=None,
             class_mode=SETTING.FLOW_FROM_DIRECTORY_SETTING.CLASS_MODE,
             batch_size=SETTING.FLOW_FROM_DIRECTORY_SETTING.BATCH_SIZE,
             shuffle=SETTING.FLOW_FROM_DIRECTORY_SETTING.SHUFFLE,
             seed=SETTING.FLOW_FROM_DIRECTORY_SETTING.SEED,
@@ -445,30 +551,35 @@
             "output_gradcam_fig_name", SETTING.GRAD_CAM_SETTING.GRAD_CAM_FIG_NAME
         )
 
         img_to_be_applied_path = kwargs.get(
             "img_to_be_applied_path", SETTING.GRAD_CAM_SETTING.IMG_PATH
         )
 
+        print_layer_names = kwargs.get("print_layer_names", False)
+
         fig_address = fig_to_save_address / gradcam_fig_name
         if model_path is None:
             raise ValueError("model_path is None")
 
         model = keras.models.load_model(model_path)
         logger.info(f"Model loaded from {model_path}")
 
-        # print the model layers
-        for idx in range(len(model.layers)):
-            print(model.get_layer(index=idx).name)
+        if print_layer_names:
+            # print the model layers
+            for idx in range(len(model.layers)):
+                print(model.get_layer(index=idx).name)
 
         # model_builder = keras.applications.xception.Xception
         preprocess_input = keras.applications.xception.preprocess_input
         # decode_predictions = keras.applications.xception.decode_predictions
 
-        last_conv_layer_name = SETTING.GRAD_CAM_SETTING.LAST_CONV_LAYER_NAME
+        conv_layer_name_tobe_used = kwargs.get(
+            "layer_name", SETTING.GRAD_CAM_SETTING.LAST_CONV_LAYER_NAME
+        )
 
         # The local path to our target image
         img_path = img_to_be_applied_path
 
         # load the image and show it
         img = load_img(
             img_path, target_size=SETTING.FLOW_FROM_DIRECTORY_SETTING.TARGET_SIZE
@@ -483,23 +594,24 @@
             )
         )
         # Make model
         # model = model_builder(weights="imagenet")
         # Remove last layer's softmax
         model.layers[-1].activation = None
         # Print what the top predicted class is
-        preds = model.predict(img_array)
         # print("Predicted:", decode_predictions(preds, top=1)[0])
         # Generate class activation heatmap
         heatmap = BitVision._make_gradcam_heatmap(
-            img_array, model, last_conv_layer_name
+            img_array, model, conv_layer_name_tobe_used
         )
 
         # Display heatmap
         plt.matshow(heatmap)
+        # add the title layer name
+        plt.title(conv_layer_name_tobe_used)
         plt.show()
         BitVision._save_and_display_gradcam(img_path, heatmap, cam_path=fig_address)
 
     @staticmethod
     def _get_img_array(img_path, size):
         # `img` is a PIL image of size 299x299
         img = keras.preprocessing.image.load_img(img_path, target_size=size)
@@ -556,15 +668,15 @@
         img = keras.preprocessing.image.load_img(img_path)
         img = keras.preprocessing.image.img_to_array(img)
 
         # Rescale heatmap to a range 0-255
         heatmap = np.uint8((1 / SETTING.DATA_GEN_SETTING.RESCALE) * heatmap)
 
         # Use jet colormap to colorize heatmap
-        jet = cm.get_cmap("plasma")
+        jet = cm.get_cmap("hot")
 
         # Use RGB values of the colormap
         jet_colors = jet(np.arange(256))[:, :3]
         jet_heatmap = jet_colors[heatmap]
 
         # Create an image with RGB colorized heatmap
         jet_heatmap = keras.preprocessing.image.array_to_img(jet_heatmap)
@@ -576,47 +688,62 @@
         superimposed_img = keras.preprocessing.image.array_to_img(superimposed_img)
 
         # Save the superimposed image
         superimposed_img.save(cam_path)
 
     @staticmethod
     def return_best_model_name(
-        directory: str = SETTING.MODEL_SETTING.MODEL_PATH,
+        directory: Path = SETTING.MODEL_SETTING.MODEL_PATH,
     ) -> str:
         """
         Return the best model name
         :param directory:
         :return:
         """
 
         best_model = None
         best_val_acc = 0.0
 
         for filename in os.listdir(directory):
             if (
                 filename.endswith(".h5")
                 and "val_acc" in filename
-                and not "val_accuracy" in filename
+                and "val_accuracy" not in filename
             ):
                 # Extract the validation accuracy from the filename
                 print(filename.split("_val_acc_")[1].split("_.h5")[0])
                 val_acc = float(filename.split("_val_acc_")[1].split("_.h5")[0])
 
                 if val_acc > best_val_acc:
                     best_val_acc = val_acc
                     best_model = filename
 
         return best_model
 
+    @staticmethod
+    def print_deepnet_project_metadata():
+        SETTING.load_settings_from_json()
+
 
 if __name__ == "__main__":
     obj = BitVision(
         train_test_val_dir=Path(__file__).parent / ".." / "dataset_train_test_val"
     )
     print(obj.categories)
     print(obj.data_details)
-    obj.plot_image_category()
+    obj.plot_image_category(nrows=3, ncols=3)
+    obj.assemble_deep_net_model_2()
     obj.compile_model()
-    obj.train_model()
+    obj.train_model(epochs=5)
     obj.plot_history()
-    obj.predict()
-    obj.grad_cam_viz(gradcam_fig_name="test.png")
+    obj.predict(num_rows=2, num_cols=2, figsize=(4, 10))
+    print(obj.layer_names)
+    for conv_layer in obj.layer_names["conv_layer"]:
+        obj.grad_cam_viz(
+            gradcam_fig_name="test.png",
+            print_layer_names=False,
+            test_folder_dir=Path(__file__).parent
+            / ".."
+            / "dataset_train_test_val"
+            / "test",
+            layer_name=conv_layer,
+        )
```

### Comparing `drillvision-0.0.5/neural_network_model/model.py` & `drillvision-0.0.6/neural_network_model/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import json
 import os
 from pathlib import Path
+from pprint import pprint
 from typing import List
 
 from dotenv import load_dotenv
 from pydantic import BaseModel
 from tensorflow import keras
 
 # Load environment variables from .env file
@@ -12,29 +14,29 @@
 
 class DataAddressSetting(BaseModel):
     MAIN_DATA_DIR_ADDRESS: str = (Path(__file__).parent / ".." / "dataset").resolve()
     TEST_DIR_ADDRESS: str = (
         Path(__file__).parent
         / ".."
         / "dataset_train_test_val"
-        / "test"  # check the TRAIN_TEST_SPLIT_DIR_NAMES in
+        # / "test"  # check the TRAIN_TEST_SPLIT_DIR_NAMES in
         # the PreprocessingSetting make sure test is in the list
     )
 
 
 class DownloadImageSetting(BaseModel):
     LIMIT: int = 5
 
 
 class AugmentationSetting(BaseModel):
-    ROTATION_RANGE: int = 25
-    WIDTH_SHIFT_RANGE: float = 0.0
-    HEIGHT_SHIFT_RANGE: float = 0.0
-    SHEAR_RANGE: float = 0.2
-    ZOOM_RANGE: float = 0.5
+    ROTATION_RANGE: int = 30
+    WIDTH_SHIFT_RANGE: float = 0.2
+    HEIGHT_SHIFT_RANGE: float = 0.2
+    SHEAR_RANGE: float = 0.15
+    ZOOM_RANGE: float = 0.15
     HORIZONTAL_FLIP: bool = True
     FILL_MODE: str = "nearest"
 
     BATCH_SIZE: int = 1
 
     # Address to save augmented images
     AUGMENTED_IMAGES_DIR_ADDRESS: Path = (
@@ -67,19 +69,24 @@
 class ModelSetting(BaseModel):
     MODEL_PATH: str = (Path(__file__).parent / ".." / "deep_model").resolve()
 
     MODEL_NAME: str = "model_.h5"
 
     # compile
     LOSS: str = "categorical_crossentropy"
-    METRICS: List = ["accuracy"]
+    METRICS: List = [
+        "accuracy",
+        # 'precision',
+        # 'recall',
+        # 'f1_score'
+    ]
 
     # fit generator
     EPOCHS: int = 3
-    FIT_GEN_VERBOSE: int = 1
+    FIT_GEN_VERBOSE: int = 0
     VALIDATION_STEPS: int = 4
     CLASS_WEIGHT: dict = None
     MAX_QUEUE_SIZE: int = 10
     WORKERS: int = 1
     SHUFFLE: bool = True
     INITIAL_EPOCH: int = 1
     USE_MULTIPROCESSING: bool = False
@@ -108,14 +115,15 @@
 
 
 class RandomSeedSetting(BaseModel):
     SEED: int = 1
 
 
 class FlowFromDirectorySetting(BaseModel):
+    IMAGE_SIZE: int = 224
     TARGET_SIZE: tuple = (224, 224)
     COLOR_MODE: str = "rgb"
     CLASS_MODE: str = "categorical"
     BATCH_SIZE: int = 32
     SHUFFLE: bool = True
     SEED: int = 1234
 
@@ -131,15 +139,15 @@
     IMAGE_NEW_NAME: str = (Path(__file__).parent / ".." / "figures").resolve()
     GRAD_CAM_FIG_NAME: str = "grad_cam_pdc_Image_1.png"
 
     ALPHA: float = 0.7
 
 
 class S3BucketSetting(BaseModel):
-    BUCKET_NAME: str = "bitimages123"
+    BUCKET_NAME: str = os.getenv("BUCKET_NAME")
     PARENT_FOLDER_NAME: str = "dataset"
     SUBFOLDER_NAME: list = ["dataset/pdc_bit", "dataset/rollercone_bit"]
     DOWNLOAD_LOCATION: str = (Path(__file__).parent / ".." / "s3_dataset").resolve()
     REGION_NAME: str = "us-east-2"
     # s3 access credentials
     AWS_S3_SECRET_KEY: str = os.getenv("S3_AWS_SECRET_ACCESS_KEY")
     AWS_S3_ACCESS_KEY: str = os.getenv("S3_AWS_ACCESS_KEY")
@@ -187,13 +195,69 @@
     DATA_GEN_SETTING: DataGenSetting = DataGenSetting()
     DOWNLOAD_IMAGE_SETTING: DownloadImageSetting = DownloadImageSetting()
     GRAD_CAM_SETTING: GradCamSetting = GradCamSetting()
     S3_BUCKET_SETTING: S3BucketSetting = S3BucketSetting()
     EC2_SETTING: Ec2Setting = Ec2Setting()
     GITHUB_SETTING: GitHubSetting = GitHubSetting()
 
+    @staticmethod
+    def save_settings_to_json(filename: str = "settings.json"):
+        def convert_paths(obj):
+            if isinstance(obj, (Path, tuple)):
+                return str(obj)
+            return obj
+
+        with open(filename, "w") as f:
+            json.dump(SETTING.dict(), f, indent=4, default=convert_paths)
+
+    @staticmethod
+    def load_settings_from_json(filename: str = "settings.json") -> json:
+        with open(filename, "r") as f:
+            data = json.load(f)
+        pprint(Setting(**data))
+        return Setting(**data)
+
+
+class TransferLearnignSetting(Setting):
+    # prepare data frame in pandas
+    DF_X_COL_NAME: str = "Filepath"
+    DF_Y_COL_NAME: str = "Label"
 
-SETTING = Setting()
+    TRAIN_SIZE: float = 0.9
+    SHUFFLE: bool = True
+    RANDOM_STATE: int = 1
+
+    # training
+    VALIDATION_SPLIT: float = 0.1
+
+    # MobileNetV2 network details
+    WEIGHTS: str = "imagenet"
+    POOLING: str = "avg"
+    INCLUDE_TOP: bool = False
 
+    DENSE_LAYER_ACTIVATION: str = "relu"
+
+    DENSE_LAYER_1_UNITS: int = 128
+    DENSE_LAYER_2_UNITS: int = 128
+
+    LAST_LAYER_ACTIVATION: str = "softmax"
+
+    OPTIMIZER: str = "adam"
+    LOSS: str = "categorical_crossentropy"
+    METRICS: list = ["accuracy"]
+
+    MONITOR: str = "val_loss"
+    PATIENCE: int = 5
+    RESTORE_BEST_WEIGHTS: bool = True
+
+
+SETTING = Setting()
+TRANSFER_LEARNING_SETTING = TransferLearnignSetting()
 
 if __name__ == "__main__":
-    print(SETTING.EC2_SETTING.SECURITY_GROUP_ID)
+    # print(SETTING.EC2_SETTING.SECURITY_GROUP_ID)
+    # Save the settings to a JSON file
+    # SETTING.save_settings_to_json("settings.json")
+    SETTING.load_settings_from_json("settings.json")
+
+    # Load the settings from a JSON file
+    # loaded_settings = load_settings_from_json("settings.json")
```

### Comparing `drillvision-0.0.5/neural_network_model/process_data.py` & `drillvision-0.0.6/neural_network_model/process_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import logging
 import os
 import random
 import shutil
+import warnings
 from pathlib import Path
+from pprint import pprint
 from typing import Any, Dict, List
-import warnings
 
 from bing_image_downloader import downloader
 from tensorflow.keras.preprocessing import image
-from tensorflow.keras.preprocessing.image import ImageDataGenerator, img_to_array, load_img
+from tensorflow.keras.preprocessing.image import (
+    ImageDataGenerator,
+    img_to_array,
+    load_img,
+)
 from tqdm import tqdm
 
 from neural_network_model.model import SETTING
 from neural_network_model.s3 import MyS3
 
 # Set seed to get the same random numbers each time
 random.seed(SETTING.RANDOM_SEED_SETTING.SEED)
@@ -72,58 +77,58 @@
             download_location_address = (
                 self.dataset_address or SETTING.S3_BUCKET_SETTING.DOWNLOAD_LOCATION
             )
 
             s3.download_files_from_subfolders(
                 bucket_name, subfolders, download_location_address
             )
-            logger.info("Downloaded images from S3 bucket")
+            logger.debug("Downloaded images from S3 bucket")
             return
 
         if category_list is None:
             category_list = SETTING.CATEGORY_SETTING.CATEGORIES
         for category in category_list:
             downloader.download(
                 category,
                 limit=limit or SETTING.DOWNLOAD_IMAGE_SETTING.LIMIT,
                 output_dir=self.dataset_address
                 or SETTING.DATA_ADDRESS_SETTING.MAIN_DATA_DIR_ADDRESS,
                 adult_filter_off=True,
                 force_replace=False,
                 timeout=120,
             )
-        logger.info("Downloaded images")
+        logger.debug("Downloaded images")
 
     @property
     def categorie_name(self) -> List[str]:
         """
         This function is used to find the categories name.
         :return:
         """
         self.categories_name_folders = os.listdir(self.dataset_address)
         list_to_ignore = SETTING.IGNORE_SETTING.IGNORE_LIST
         self.categories_name_folders = [
             x for x in self.categories_name_folders if x not in list_to_ignore
         ]
-        logger.info(self.categories_name_folders)
-        logger.info(f"Categories name: {self.categories_name_folders}")
+        logger.debug(self.categories_name_folders)
+        logger.debug(f"Categories name: {self.categories_name_folders}")
 
         # for images in each category dir, check if the image is in list_to_ignore, if yes remove from dir
         for category_folder in self.categories_name_folders:
             # read the files in the dataset folder
             main_dataset_folder = (
                 self.dataset_address
                 or SETTING.DATA_ADDRESS_SETTING.MAIN_DATA_DIR_ADDRESS
             )
             data_address = main_dataset_folder / category_folder
 
             for file in os.listdir(data_address):
                 if file in list_to_ignore:
                     os.remove(data_address / file)
-                    logger.info(f"Removed {file} from {category_folder}")
+                    logger.debug(f"Removed {file} from {category_folder}")
 
         return self.categories_name_folders
 
     @property
     def image_dict(self) -> Dict[str, Dict[str, Any]]:
         """
         This function reads the data from the dataset folder.
@@ -198,21 +203,21 @@
                 rand_img_num = int(random.random() * number_of_images)
 
                 img_address = self.image_dict[image_category]["image_list"][
                     rand_img_num
                 ]
                 for case in SETTING.IGNORE_SETTING.IGNORE_LIST:
                     if case == img_address.name:
-                        logger.info(f"Found {case} in {image_category} folder")
+                        logger.debug(f"Found {case} in {image_category} folder")
                         continue
                 # check if the image name is in the ignore list, if so continue
                 if img_address in SETTING.IGNORE_SETTING.IGNORE_LIST:
                     continue
 
-                logger.info(f"Image address: {img_address}")
+                logger.debug(f"Image address: {img_address}")
 
                 img = load_img(img_address)
 
                 x = img_to_array(img)
                 x = x.reshape((1,) + x.shape)
 
                 for _ in Augment_data_gen.flow(
@@ -240,33 +245,33 @@
         )
         train_test_val_split_dir_address = (
             kwargs.get("train_test_val_split_dir_address")
             or SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
         )
         # get the list of dirs in the AUGMENTED_IMAGES_DIR_ADDRESS
         augmented_images_dir_list = os.listdir(augmented_data_address)
-        logger.info(f"Augmented images dir list: {augmented_images_dir_list}")
+        logger.debug(f"Augmented images dir list: {augmented_images_dir_list}")
 
         # make a new dir for train and test and validation data
         if not os.path.exists(train_test_val_split_dir_address):
             os.makedirs(train_test_val_split_dir_address)
         # make 3 dirs for train, test and validation under AUGMENTATION_SETTING.TRAIN_TEST_SPLIT_DIR_ADDRESS
         for dir_name in SETTING.PREPROCESSING_SETTING.TRAIN_TEST_SPLIT_DIR_NAMES:
             if not os.path.exists(train_test_val_split_dir_address / dir_name):
                 os.makedirs(train_test_val_split_dir_address / dir_name)
-        logger.info(f"Created train, test and validation dirs")
+        logger.debug("Created train, test and validation dirs")
 
         # under each train, test and validation dir make a dir for each category
         for dir_name in SETTING.PREPROCESSING_SETTING.TRAIN_TEST_SPLIT_DIR_NAMES:
             for category in augmented_images_dir_list:
                 if not os.path.exists(
                     train_test_val_split_dir_address / dir_name / category
                 ):
                     os.makedirs(train_test_val_split_dir_address / dir_name / category)
-        logger.info(f"Created category dirs under train, test and validation dirs")
+        logger.debug("Created category dirs under train, test and validation dirs")
 
         self._populated_augmented_images_into_train_test_val_dirs(
             augmented_data_address, train_test_val_split_dir_address
         )
 
     def _populated_augmented_images_into_train_test_val_dirs(self, *arges, **kwargs):
         dataset_augmented_dir_address = arges[0]
@@ -279,23 +284,22 @@
             # Number of items to select for each new list
             num_train = int(
                 len(original_list) * SETTING.PREPROCESSING_SETTING.TRAIN_FRACTION
             )
             num_test = int(
                 len(original_list) * SETTING.PREPROCESSING_SETTING.TEST_FRACTION
             )
-            num_val = len(original_list) - num_train - num_test
 
             # Randomly select items from the original list without replacement
             selected_items = random.sample(original_list, len(original_list))
 
             # Create three new lists containing 70%, 20%, and 10% of the original list
             train_list = selected_items[:num_train]
-            test_list = selected_items[num_train : num_train + num_test]
-            val_list = selected_items[num_train + num_test :]
+            test_list = selected_items[num_train : num_train + num_test]  # noqa: E203
+            val_list = selected_items[num_train + num_test :]  # noqa: E203
             # copy the images from the dataset_augmented pdc_bit folder to the train, test and validation folders
             self._copy_images(
                 train_list,
                 category,
                 "train",
                 dataset_augmented_dir_address,
                 train_test_val_split_dir_address,
@@ -330,38 +334,43 @@
         dataset_augmented_dir_address = (
             dataset_augmented_dir_address
             or SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
         )
 
         # check if the dir is empty, if not delete all the files
         if os.listdir(train_test_val_split_dir_address / dest_folder / categ):
-            logger.info(
+            logger.debug(
                 f"Deleting all the files in {train_test_val_split_dir_address / dest_folder / categ}"
             )
             for file in os.listdir(
                 train_test_val_split_dir_address / dest_folder / categ
             ):
                 os.remove(train_test_val_split_dir_address / dest_folder / categ / file)
 
-        for image in images:
+        for _image in images:
             shutil.copy(
-                dataset_augmented_dir_address / categ / image,
-                train_test_val_split_dir_address / dest_folder / categ / image,
+                dataset_augmented_dir_address / categ / _image,
+                train_test_val_split_dir_address / dest_folder / categ / _image,
             )
-        logger.info(
+        logger.debug(
             f"copied {len(images)} images for category {categ} to {dest_folder}"
         )
 
+    @staticmethod
+    def print_deepnet_project_metadata():
+        return SETTING.load_settings_from_json()
+
 
 if __name__ == "__main__":
     obj = Preprocessing(dataset_address=Path(__file__).parent / ".." / "dataset")
-    # obj.download_images()
+    obj.download_images()
 
     # or download the data from s3. this is after you have downloaded the data
     # using Process.download_images() and uploaded it to s3
     # this way the data would be consistent across all the users
     # obj = Preprocessing(dataset_address=Path(__file__).parent / ".." / "s3_dataset")
     # obj.download_images(from_s3=True)
 
     print(obj.image_dict)
     obj.augment_data(number_of_images_tobe_gen=10)
     obj.train_test_split()
+    obj.print_deepnet_project_metadata()
```

### Comparing `drillvision-0.0.5/neural_network_model/s3.py` & `drillvision-0.0.6/neural_network_model/s3.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.5/pyproject.toml` & `drillvision-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.5/setup.py` & `drillvision-0.0.6/setup.py`

 * *Files identical despite different names*

