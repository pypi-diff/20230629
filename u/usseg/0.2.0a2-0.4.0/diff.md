# Comparing `tmp/usseg-0.2.0a2.tar.gz` & `tmp/usseg-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usseg-0.2.0a2.tar", max compression
+gzip compressed data, was "usseg-0.4.0.tar", max compression
```

## Comparing `usseg-0.2.0a2.tar` & `usseg-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     2831 2023-05-17 14:48:09.714561 usseg-0.2.0a2/README.md
--rw-r--r--   0        0        0      703 2023-05-18 10:26:45.709016 usseg-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0    53504 2023-05-17 12:58:04.630200 usseg-0.2.0a2/usseg/General_functions.py
--rw-r--r--   0        0        0     4115 2023-05-17 14:37:14.323870 usseg-0.2.0a2/usseg/Organise_files.py
--rw-r--r--   0        0        0    11405 2023-05-17 19:40:16.094684 usseg-0.2.0a2/usseg/Refined_anon_2_html.py
--rw-r--r--   0        0        0      303 2023-05-17 12:40:36.083145 usseg-0.2.0a2/usseg/__init__.py
--rw-r--r--   0        0        0      857 2023-05-18 10:07:46.451007 usseg-0.2.0a2/usseg/main.py
--rw-r--r--   0        0        0     4914 2023-05-17 14:12:40.206489 usseg-0.2.0a2/usseg/visualisation_html.py
--rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 usseg-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0     3203 2023-05-18 17:29:24.569730 usseg-0.4.0/README.md
+-rw-r--r--   0        0        0      710 2023-06-29 13:02:56.462211 usseg-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    54798 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/General_functions.py
+-rw-r--r--   0        0        0     4117 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/Organise_files.py
+-rw-r--r--   0        0        0    11591 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/Refined_anon_2_html.py
+-rw-r--r--   0        0        0     5240 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/Single_image_processing.py
+-rw-r--r--   0        0        0      361 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/__init__.py
+-rw-r--r--   0        0        0      771 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/example.py
+-rw-r--r--   0        0        0      878 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/main.py
+-rw-r--r--   0        0        0     4993 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/visualisation_html.py
+-rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 usseg-0.4.0/PKG-INFO
```

### Comparing `usseg-0.2.0a2/README.md` & `usseg-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,31 @@
   - [Plot\_correction](#plot_correction)
   - [Annotate](#annotate)
   - [Contributing](#contributing)
   - [License](#license)
 
 ## Installation
 
+- To install as a dependency for your project:
+
+``` 
+pip install usseg
+```
+
+or
+
+``` sh
+poetry add usseg
+```
+
+
+### Development Environment
+
+To install the development environment follow the following steps.
+
 - Clone this repository and change into the directory.
 - Install [poetry](https://python-poetry.org/docs/) as per the installation instructions.
 - Install [tesseract](https://github.com/tesseract-ocr/tesseract) as per the intallation instructions.
 - Install the package dependencies with:
 ```
 poetry install
 
@@ -34,14 +51,16 @@
 ```
 poetry shell
 ```
 
 - You are now in the development environment!
 - Copy `config_example.toml` to `config.toml` and change the variables for your local set up (e.g. path to your data etc.).
 - The main script can now be run in one complete run with `python usseg/main.py`.
+- If debugging in vscode, ensure the python interpreter is set to the virtual environment created poetry. This path can be found using ```poetry env info --path```
+
 
 # Functions
 
 Provide instructions on how to use your project.
 
 ## Initial_segmentation
```

### Comparing `usseg-0.2.0a2/usseg/General_functions.py` & `usseg-0.4.0/usseg/General_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,38 +13,39 @@
 from scipy.ndimage.filters import gaussian_filter
 import math
 from scipy import signal
 from scipy.spatial.distance import cdist
 from scipy.signal import find_peaks, peak_widths
 import statistics
 import scipy.linalg
+from sklearn.cluster import DBSCAN
 
 # from matplotlib import path
 # import nibabel as nib
 # from mpl_toolkits.mplot3d import Axes3D
 import pandas as pd
 import re
 import pytesseract
 from pytesseract import Output
 
-def Initial_segmentation(input_image_filename):
+def Initial_segmentation(input_image_obj):
     """Perform an initial corse segmentation of the waveform.
 
     Args:
         input_image_filename (str) : Name of file within current directory, or path to a file.
 
     Returns:
         segmentation_mask (ndarray) : A binary array mask showing the corse segmentation of waveform (1) against background (0).
         Xmin (float) : Minimum X coordinate of the segmentation.
         Xmax (float) : Maximum X coordinate of the segmentation.
         Ymin (float) : Minimum Y coordinate of the segmentation.
         Ymax (float) : Maximum Y coordinate of the segmentation.
     """
-    img_RGBA = Image.open(input_image_filename)  # These images are in RGBA form
-    img_RGB = img_RGBA.convert("RGB")  # We need RGB, so convert here.
+    # img_RGBA = Image.open(input_image_filename)  # These images are in RGBA form
+    img_RGB = input_image_obj
     pixel_data = img_RGB.load()  # Loads a pixel access object, where pixel values can be edited
     # gry = img_RGB.convert("L")  # (returns grayscale version)
 
     # To threshold the ROI,
     for y in range(img_RGB.size[1]):
         for x in range(img_RGB.size[0]):
             r = pixel_data[x, y][0]  # red component
@@ -109,15 +110,14 @@
         np.max(xmax_list),
         np.min(ymin_list),
         np.max(ymax_list),
     )  # find max and min withing the lists.
 
     return segmentation_mask, Xmin, Xmax, Ymin, Ymax
 
-
 def Define_end_ROIs(segmentation_mask, Xmin, Xmax, Ymin, Ymax):
     """
     Function to define regions adjacent to the corse waveform in which to search for axes info.
 
     Args:
         segmentation_mask (ndarray) : A binary array mask showing the corse segmentation of waveform (1) against background (0).
         Xmin (float) : Minimum X coordinate of the segmentation.
@@ -155,15 +155,35 @@
         Ymax_R = Ylim - 70
     else:
         Ymax_R = Ylim
 
     Right_dimensions = [Xmin_R, Xmax_R, Ymin_R, Ymax_R]
     return Left_dimensions, Right_dimensions
 
-def Segment_refinement(input_image_filename, Xmin, Xmax, Ymin, Ymax):
+def check_inverted_curve(top_curve_mask, Ymax, Ymin, tol=.25):
+    """Checks to see if top curve mask is of an inverted waveform
+
+    Args:
+        top_curve_mask (ndarray) : A binary array showing a curve along the top of the refined waveform.
+        Ymax (float) : Maximum Y coordinate of the segmentation in pixels.
+        Ymin (float) : Minimum Y coordinate of the segmentation in pixels.
+        tol (float, optional) : If the top curve occupies less than tol * (Ymax - Ymin) rows, then
+            the curve is assumed to be inverted (that is True is returned). If the top curve occupies more than
+            or equal to this number of rows, the False is returned and the curve is assumed to be non-inverted.
+            Defaults to 0.45.
+
+    Returns:
+        return value (bool) : True if the top curve is of an inverted waveform, False is the top curve is of a non-inverted waveform.
+    """
+    c_rows = np.where(np.sum(top_curve_mask, axis=1))   # Curve rows
+    c_range = np.max(c_rows) - np.min(c_rows)           # Y range of top curve
+    #print(c_range / (Ymax - Ymin), tol)
+    return c_range / (Ymax - Ymin) < tol
+
+def Segment_refinement(input_image_obj, Xmin, Xmax, Ymin, Ymax):
     """
     Function to refine the waveform segmentation within the bounds of the corse waveform ROI.
 
     Args:
         input_image_filename (str) : Name of file within current directory, or path to a file.
         Xmin (float) : Minimum X coordinate of the segmentation in pixels.
         Xmax (float) : Maximum X coordinate of the segmentation in pixels.
@@ -173,15 +193,15 @@
         refined_segmentation_mask (ndarray) :  A binary array mask showing the refined segmentation of waveform (1) against background (0).
         top_curve_mask (ndarray) : A binary array showing a curve along the top of the refined waveform.
     """
 
     # Refine segmentation to increase smoothing
     # Save output to .txt file to load later.
 
-    image = cv2.imread(input_image_filename)
+    image = input_image_obj
     input_image_gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
     ret, thresholded_image = cv2.threshold(input_image_gray, 30, 255, 0)
     thresholded_image[:, int(Xmax) : -1] = 0
     thresholded_image[:, 0 : int(Xmin) - 1] = 0
     thresholded_image[0 : int(Ymin) - 50, :] = 0
     thresholded_image[int(Ymax) : -1, :] = 0
     main_ROI = thresholded_image  # Main ROI
@@ -232,20 +252,26 @@
 
     ws = morphology.binary_erosion(refined_segmentation_mask)
     ws = ws.astype(float)
     top_curve_mask = refined_segmentation_mask - ws
     for x in range(int(rp[0].centroid[0]), top_curve_mask.shape[0]):
         top_curve_mask[x, :] = 0
 
+    # Checks if waveforms are inverted, if so gets the bottom of the curve
+    if check_inverted_curve(top_curve_mask, Ymax, Ymin):
+        top_curve_mask = refined_segmentation_mask - ws
+        for x in range(0, int(rp[0].centroid[0])):
+            top_curve_mask[x, :] = 0
+
     o = list(zip(*np.nonzero(top_curve_mask)))
     np.savetxt("test1.txt", o, fmt="%d")
 
     return refined_segmentation_mask, top_curve_mask
 
-def Search_for_ticks(input_image_filename, Side, Left_dimensions, Right_dimensions):
+def Search_for_ticks(input_image_obj, Side, Left_dimensions, Right_dimensions):
     """
     Function to search for the ticks in either of the axes ROIs
 
     Args:
         input_image_filename (str) : Name of file within current directory, or path to a file.
         Side (str) : Indicates the 'Left' or 'Right' axes.
         Left_dimensions (list) : edge points for the left axes ROI [Xmin, Xmax, Ymin, Ymax].
@@ -262,15 +288,15 @@
         Side (str) : Indicates the 'Left' or 'Right' axes.
         Left_dimensions (list) : edge points for the left axes ROI [Xmin, Xmax, Ymin, Ymax].
         Right_dimensions (list) : edge points for the left axes ROI [Xmin, Xmax, Ymin, Ymax].
         ROI2
         ROI3
     """
 
-    image = cv2.imread(input_image_filename)
+    image = input_image_obj
     thresholded_image = image
 
     if Side == "Left":
         ROIAX = thresholded_image[
             int(Left_dimensions[2]) : int(Left_dimensions[3]),
             int(Left_dimensions[0]) : int(Left_dimensions[1]),
         ]  # Right ROI
@@ -287,15 +313,15 @@
 
     binary_image = BinaryNP
     pixel_sum = binary_image  # .sum(-1)  # sum over color (last) axis
     nonzero_pixels = (pixel_sum > 0).astype(bool)
     W = morphology.remove_small_objects(nonzero_pixels, 20, connectivity=2)
     W = W.astype(float)
 
-    im = cv2.imread(input_image_filename)
+    im = input_image_obj
     input_image_gray = cv2.cvtColor(im, cv2.COLOR_BGR2GRAY)
     ret, thresholded_image = cv2.threshold(input_image_gray, 127, 255, 0)
 
     if Side == "Left":
         ROIAX = thresholded_image[
             int(Left_dimensions[2]) : int(Left_dimensions[3]),
             int(Left_dimensions[0]) : int(Left_dimensions[1]),
@@ -498,20 +524,20 @@
     CenPoints,
     onY,
     BCs,
     TYLshift,
     Side,
     Left_dimensions,
     Right_dimensions,
-    input_image_filename,
+    input_image_obj,
     ROI2,
     ROI3,
 ):
     for thresh_value in np.arange(100, 190, 5): # Threshold to optimise the resulting text extraction.
-        image = cv2.imread(input_image_filename)
+        image = input_image_obj
         input_image_gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
         ret, thresholded_image = cv2.threshold(input_image_gray, thresh_value, 255, 0)
         if Side == "Left":
             ROIAX = thresholded_image[
                 int(Left_dimensions[2]) : int(Left_dimensions[3]),
                 int(Left_dimensions[0]) : int(Left_dimensions[0] + TYLshift),
             ]  # Right ROI
@@ -539,15 +565,15 @@
                     retry += 1
             except Exception:
                 pass
 
         if retry == 0:
             break
 
-    print(number)
+    # print(number)
 
     # d = pytesseract.image_to_data(
     #     ROIAX,
     #     output_type=Output.DICT,
     #     config="--psm 11 -c tessedit_char_whitelist=-0123456789",
     # )
     n_boxes = len(extracted_text_data["level"])
@@ -710,15 +736,15 @@
                 diff = lst.index(0) - lst.index(i)
                 dist.append(diff)
             elif lst.index(0) < lst.index(i):
                 diff = abs(lst.index(i)) - abs(lst.index(0))
                 dist.append(diff)
             elif lst.index(0) == lst.index(i):
                 dist.append(0)
-        print(dist)
+        # print(dist)
 
         dist_divided = []
         for i in range(0, length):
             dist_divided.append(lst[i] / dist[i])
 
         return dist_divided
 
@@ -746,99 +772,103 @@
         ] = ROI3  # Right ROI
     elif Side == "Right":
         empty_to_fill[
             int(Right_dimensions[2]) : int(Right_dimensions[3]),
             int(Right_dimensions[0]) : int(Right_dimensions[1]),
         ] = ROI3  # Left ROI
 
-    print(number)
-    print(positions)
+    # print(number)
+    # print(positions)
 
     return ROIAX, number, positions, empty_to_fill
 
 
 def Plot_Digitized_data(Rticks, Rlocs, Lticks, Llocs):
     # Function to digitize the segmetned data:
 
     Rticks = list(map(int, Rticks))
     XmaxtickR = max(Rticks)
-    print("Max tick R:", XmaxtickR)
+    # print("Max tick R:", XmaxtickR)
     XmaxidR = Rticks.index(XmaxtickR)
     XmaxR = Rlocs[XmaxidR][0]
     YmaxR = Rlocs[XmaxidR][1]
-    print("X max R:", XmaxR)
+    # print("X max R:", XmaxR)
     XMintickR = min(Rticks)
-    print("Min tick R:", XMintickR)
+    # print("Min tick R:", XMintickR)
     XMinidR = Rticks.index(XMintickR)
     XminR = Rlocs[XMinidR][0]
-    print("X min R:", XminR)
+    # print("X min R:", XminR)
     #
     Lticks = list(map(int, Lticks))
     XmaxtickL = max(Lticks)
-    print("Max tick L:", XmaxtickL)
+    # print("Max tick L:", XmaxtickL)
     XmaxidL = Lticks.index(XmaxtickL)
     XmaxL = Llocs[XmaxidL][0]
-    print("X max L:", XmaxL)
+    # print("X max L:", XmaxL)
     XMintickL = min(Lticks)
-    print("Min tick L:", XMintickL)
+    # print("Min tick L:", XMintickL)
     XminidL = Lticks.index(XMintickL)
     XminL = Llocs[XminidL][0]
     YminL = Llocs[XminidL][1]
-    print("X min L:", XminL)
+    # print("X min L:", XminL)
 
     # Yplots = [Llocs[XmaxidL][0], Llocs[XminidL][0], Rlocs[XmaxidR][0]]
     # Xplots = [Llocs[XmaxidL][1], Llocs[XminidL][1], Rlocs[XmaxidR][1]]
 
     Xmin = 0
     Xmax = 1
     Ymin = XMintickL
     Ymax = XmaxtickL
 
-    b = np.loadtxt("test1.txt", dtype=float)
+    b = np.loadtxt("test1.txt", dtype=float) # Loading in data from Segment_refinement
     b = sorted(b, key=lambda k: [k[1], k[0]])
 
     b = [B.tolist() for B in b]
     b = [x[::-1] for x in b]
 
     b = pd.DataFrame(b).groupby(0, as_index=False)[1].mean().values.tolist()
     b = [x[::-1] for x in b]
 
-    X = [XminL, XmaxR]  # ,231,429,620,820,1011,0]
-    Y = [YminL, YmaxR]  # ,558,554,554,558,566,0]
+    X = [XminL, XmaxR]  
+    Y = [YminL, YmaxR] 
 
     for i in range(0, len(b)):
         if b[i][1] >= XminL + 20 and b[i][1] <= XmaxR - 20:
             X.append(b[i][1])
             Y.append(b[i][0])
 
     origin = [X[0], Y[0]]
     topRight = [X[1], Y[1]]
     XminScale = origin[0]
     XmaxScale = topRight[0]
     YminScale = origin[1]
     YmaxScale = topRight[1]
 
+    Ynought = [(0 - YminScale) / (YmaxScale - YminScale) * (Ymax - Ymin) + Ymin]
+
     X = X[2:-1]
     Y = Y[2:-1]
 
     Xplot = [
         (i - XminScale) / (XmaxScale - XminScale) * (Xmax - Xmin) + Xmin for i in X
     ]
     Yplot = [
         (i - YminScale) / (YmaxScale - YminScale) * (Ymax - Ymin) + Ymin for i in Y
     ]
 
-    print(Xmin, Xmax)
+    # Inverts the waveform if need be
+    if np.mean(Yplot) < 0:
+        Yplot = [ y * (-1) for y in Yplot]
+
+    # print(Xmin, Xmax)
     plt.figure(2)
     plt.plot(Xplot, Yplot, "-")
-    plt.xlim((Xmin, Xmax))
-    plt.ylim((0, max(Yplot) + 10))
     plt.xlabel("Arbitrary time scale")
     plt.ylabel("Flowrate (cm/s)")
-    return Xplot, Yplot
+    return Xplot, Yplot, Ynought
 
 
 def Plot_correction(Xplot, Yplot, df):
     """
     Use data from text extraction to correct the plot
     """
 
@@ -929,15 +959,15 @@
     except Exception:
         pass
 
     return df
 
 
 def Annotate(
-    input_image_filename,
+    input_image_obj,
     refined_segmentation_mask,
     Left_dimensions,
     Right_dimensions,
     Waveform_dimensions,
     Left_axis,
     Right_axis,
 ):
@@ -958,16 +988,16 @@
     r = [Xmin, Xmax, Xmax, Xmin, Xmin]
     c = [Ymax, Ymax, Ymin, Ymin, Ymax]
     rr, cc = polygon_perimeter(c, r, refined_segmentation_mask.shape)
 
     refined_segmentation_mask[rr, cc] = 2  # set color white
     refined_segmentation_mask[rrL, ccL] = 2
     refined_segmentation_mask[rrR, ccR] = 2
-    img_RGBA = Image.open(input_image_filename)
-    img_RGB = img_RGBA  # .convert('RGB')
+
+    img_RGB = input_image_obj  # .convert('RGB')
     pixel_data = img_RGB.load()
     # gry = img_RGB.convert("L")  # returns grayscale version.
 
     for y in range(img_RGB.size[1]):
         for x in range(img_RGB.size[0]):
             # r = pixel_data[x, y][0]
             # g = pixel_data[x, y][1]
@@ -991,30 +1021,30 @@
             elif Right_axis[y, x] == 255:
                 pixel_data[x, y] = (255, 0, 255, 255)  # Set ROIs to blue
             else:
                 pixel_data[x, y] = pixel_data[x, y]
     return img_RGB
 
 
-def Colour_extract(input_image_filename, TargetRGB, cyl_length, cyl_radius):
+def Colour_extract(input_image_obj, TargetRGB, cyl_length, cyl_radius):
     """Function for extracing target colours from image
     converts image to RGB space and find coordinates of pixels within a
     cylinder whose center is the target triplet. You can visualise this
     by removing commented plot statements throughout this function.
 
     Args:
         input_image_filename (str) : Name of file within current directory, or path to a file.
         TargetRGB (list) : triplet of target Red Green Blue colour [Red,Green,Blue].
         cyl_length (int) : length of cylinder.
         cyl_radius (int) : radius of cylinder.
 
     Returns:
         COL (JpegImageFile) : PIL JpegImageFile of the filtered image highlighting yellow text.
     """
-    col4 = Image.open(input_image_filename)
+    col4 = input_image_obj
     pix4 = col4.load()
 
     # DEFINE END POINTS OF CYLINDER
     np.set_printoptions(suppress=True)
 
     def appendSpherical_1point(xyz):
         ptsnew = np.hstack(
@@ -1149,15 +1179,15 @@
             logi = 1
         else:
             # print("not inside")
             logi = 0
 
         return logi
 
-    col4 = Image.open(input_image_filename)
+    col4 = input_image_obj
     pix4 = col4.load()
     gry4 = col4.convert("L")  # returns grayscale version.
 
     Rmat = []
     Gmat = []
     Bmat = []
     Xs = []
@@ -1191,15 +1221,15 @@
     Xs = np.array(Xs)
     Ys = np.array(Ys)
     #ax.scatter(Rmat[ids],Gmat[ids],Bmat[ids],c = C[ids]/255) # plot the select points in RGB coords
     #ax.scatter(Rmat,Gmat,Bmat,c = C/255)
     #plt.show()
 
     ## COMBINE
-    COL = Image.open(input_image_filename)
+    COL = input_image_obj
     COL = COL.convert("RGB")  # We need RGB, so convert here.
     PIX = COL.load()
 
     for id in ids[0]:
         PIX[Xs[id], Ys[id]] = (255, 255, 255)  # (Rmat[id],Gmat[id],Bmat[id])
 
     for y in range(COL.size[1]):
@@ -1209,43 +1239,42 @@
 
     # plt.figure(2)
     # plt.imshow(COL)
     # plt.show()
     return COL
 
 
-def Text_from_greyscale(input_image_filename, COL):
+def Text_from_greyscale(input_image_obj, COL):
     """
     Function for extracting text from the yellow filtered image.
 
     Args:
         input_image_filename (str) : Name of file within current directory, or path to a file.
         COL (JpegImageFile) : PIL JpegImageFile of the filtered image highlighting yellow text.
     Returns:
         Fail (int) : Checks if the function has failed (1), or passed (0).
         df (DataFrame) : Dataframe with columns 'Line', 'Word', 'Value', 'Unit'.
         populated with data extracted from the image with tesseract.
 
     """
 
     PIX = COL.load()
-    img = cv2.imread(input_image_filename)
+    img = input_image_obj
     for y in range(
         int(COL.size[1] * 0.45), COL.size[1]
     ):  # Exclude bottom 3rd of image - these are fails
         for x in range(COL.size[0]):
             PIX[x, y] = (0, 0, 0)
 
-    import numpy as np
 
     pixels = np.array(COL)
     data = pytesseract.image_to_data(
         pixels, output_type=Output.DICT, lang="eng", config="--psm 3 "
     )
-    print(len(data["text"]))
+    # print(len(data["text"]))
     if (
         len(data["text"]) < 30
     ):  # This is rough, if more than 30 objects found then highly likley it is a waveform scan.
         Fail = 1  # logical, keep scan or not
         # print("not enough text found - wrong scan type")
     else:
         Fail = 0
@@ -1262,15 +1291,14 @@
                 cv2.rectangle(img, (x, y), (x + w, y + h), (0, 0, 255), 2)
                 y_center[i] = y + (h/2)
             else:
                 y_center[i] = 0  
         else:
             y_center[i] = 0
         
-    from sklearn.cluster import DBSCAN
 
     def group_similar_numbers(array, tolerance, words):
         # This function groups indexes of words with similar y-coordinate center
         # Assuming that this is an indicator of words being part of the same line
         # Prepare the data for clustering
         data = np.array(array).reshape(-1, 1)
 
@@ -1293,19 +1321,19 @@
             grouped_words.append(' '.join(group_words))
 
         return grouped_words
 
     tolerance = 3  # Adjust the tolerance value - the max difference between y-coords considered on the same line
     grouped_words = group_similar_numbers(y_center, tolerance, data["text"])
 
-    for group in grouped_words:
-        print(group)
+    # for group in grouped_words:
+    #     # print(group)
 
     # Display image
-    cv2.imshow('img', img)
+    plt.imshow(img)
 
     # Analyze the OCR output
     target_words = [
         "Lt Ut-PS",
         "Lt Ut-ED",
         "Lt Ut-S/D",
         "Lt Ut-PI",
@@ -1344,29 +1372,29 @@
             # Look for word in line
             if word in line:
                 # Extract value and unit
                 match = re.search(r"(\-?\d+\.\d+|\-?\d+)\s*([^\d\s]+)?$", line)
                 if match:
                     value = float(match.group(1))
                     unit = match.group(2) if match.group(2) else ""
-                    df = df.append(
+                    df = df._append(
                         {"Line": i + 1, "Word": word, "Value": value, "Unit": unit},
                         ignore_index=True,
                     )
                 else:
                     print("couldn't find numeric data for line")
-                    df = df.append(
+                    df = df._append(
                         {"Line": i + 1, "Word": word, "Value": 0, "Unit": 0},
                         ignore_index=True,
                     )
                     pass
 
     # Print DataFrame
-    print(input_image_filename)
-    print(df)
+    # print(input_image_obj)
+    # print(df)
 
     # # Display the result
     # cv2.imshow('Result', img)
 
     return Fail, df
 
 def Scan_type_test(input_image_filename):
@@ -1448,14 +1476,14 @@
     # Initialize DataFrame
     df = pd.DataFrame(columns=["Line", "Word", "Value", "Unit"])
 
     Fail = 1  # initialise fail variable
     for target in target_words:
         for word in lines:
             if target in word:
-                print(f"{target} found in {word}")
+                # print(f"{target} found in {word}")
                 Fail = 0 # If any of the words are found, then no fail.
         # Print DataFrame
-    print(input_image_filename) # Print the file name just processed
+    # print(input_image_filename) # Print the file name just processed
 
     return Fail, df  # Return the fail variable and dataframe contraining extracted text.
```

### Comparing `usseg-0.2.0a2/usseg/Organise_files.py` & `usseg-0.4.0/usseg/Organise_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,13 +86,13 @@
     if pickle_path is not False:
         if pickle_path is None:
             pickle_path = toml.load("config.toml")["pickle"]["likely_us_images"]
 
         with open(pickle_path, 'wb') as f:
             pickle.dump(patient_paths, f)
 
-    return patient_paths
-
+    return pickle_path
+    
 if __name__ == "__main__":
 
     root_dir = toml.load("config.toml")["root_dir"]
     get_likely_us(root_dir)
```

### Comparing `usseg-0.2.0a2/usseg/Refined_anon_2_html.py` & `usseg-0.4.0/usseg/Refined_anon_2_html.py`

 * *Files 16% similar despite different names*

```diff
@@ -111,78 +111,69 @@
             "Excepted either a string or a list"
         )
 
 
     if output_dir is None:
         output_dir = toml.load("config.toml")["output_dir"]
     os.makedirs(output_dir, exist_ok=True)
-    xcel_file = output_dir + "sample3_processed_data"
+    # xcel_file = output_dir + "sample3_processed_data"
     Text_data = []  # text data extracted from image
     Annotated_scans = []
     Digitized_scans = []
 
     for input_image_filename in filenames:  # Iterare through all file names and populate excel file
         # input_image_filename = "E:/us-data-anon/0000/IHE_PDI/00003511/AA3A43F2/AAD8766D/0000371E\\EEEAE224.JPG"
         image_name = os.path.basename(input_image_filename)
         print(input_image_filename)
 
-        try:  # Try initial segmentation
+        try:  # Try text extraction
             colRGBA = Image.open(input_image_filename)  # These images are in RGBA form
-            col = colRGBA.convert("RGB")  # We need RGB, so convert here.
-            pix = (
-                col.load()
-            )  # Loads a pixel access object, where pixel values can be edited
+            PIL_col = colRGBA.convert("RGB")  # We need RGB, so convert here. with PIL
+            cv2_img = cv2.imread(input_image_filename) # with cv2.
+            # pix = (
+            #     col.load()
+            # )  # Loads a pixel access object, where pixel values can be edited
 
             # from General_functions import Colour_extract, Text_from_greyscale
-            COL = General_functions.Colour_extract(input_image_filename, [255, 255, 100], 80, 80)
+            COL = General_functions.Colour_extract(PIL_col, [255, 255, 100], 80, 80)
             print("Done Colour extract")
 
-            Fail, df = General_functions.Text_from_greyscale(input_image_filename, COL)
+            Fail, df = General_functions.Text_from_greyscale(cv2_img, COL)
         except Exception:  # flat fail on 1
             traceback.print_exc()  # prints the error message and traceback
             print("Failed Text extraction")
             Text_data.append(None)
             Fail = 0
             pass
 
         try:  # Try initial segmentation
             segmentation_mask, Xmin, Xmax, Ymin, Ymax = General_functions.Initial_segmentation(
-                input_image_filename=input_image_filename
+                input_image_obj=PIL_col
             )
-        except:  # flat fail on 1
+        except Exception:  # flat fail on 1
             print("Failed Initial segmentation")
             Fail = Fail + 1
             pass
 
         try:  # define end ROIs
             Left_dimensions, Right_dimensions = General_functions.Define_end_ROIs(
                 segmentation_mask, Xmin, Xmax, Ymin, Ymax
             )
-        except:
+        except Exception:
             print("Failed Defining ROI")
             Fail = Fail + 1
             pass
 
         try:
             Waveform_dimensions = [Xmin, Xmax, Ymin, Ymax]
-        except:
+        except Exception:
             print("Failed Waveform dimensions")
             Fail = Fail + 1
             pass
 
-        try:  # Refine segmentation
-            refined_segmentation_mask, top_curve_mask = General_functions.Segment_refinement(
-                input_image_filename, Xmin, Xmax, Ymin, Ymax
-            )
-        except:
-            traceback.print_exc()  # prints the error message and traceback
-            print("Failed Segment refinement")
-            Fail = Fail + 1
-            pass
-
         try:  # Search for ticks and labels
             (
                 Cs,
                 ROIAX,
                 CenPoints,
                 onY,
                 BCs,
@@ -190,27 +181,27 @@
                 thresholded_image,
                 Side,
                 Left_dimensions,
                 Right_dimensions,
                 ROI2,
                 ROI3,
             ) = General_functions.Search_for_ticks(
-                input_image_filename,"Left", Left_dimensions, Right_dimensions
+                cv2_img, "Left", Left_dimensions, Right_dimensions
             )
             ROIAX, Lnumber, Lpositions, ROIL = General_functions.Search_for_labels(
                 Cs,
                 ROIAX,
                 CenPoints,
                 onY,
                 BCs,
                 TYLshift,
                 Side,
                 Left_dimensions,
                 Right_dimensions,
-                input_image_filename,
+                cv2_img,
                 ROI2,
                 ROI3,
             )
 
             (
                 Cs,
                 ROIAX,
@@ -221,32 +212,54 @@
                 thresholded_image,
                 Side,
                 Left_dimensions,
                 Right_dimensions,
                 ROI2,
                 ROI3,
             ) = General_functions.Search_for_ticks(
-                input_image_filename,"Right", Left_dimensions, Right_dimensions
+                cv2_img, "Right", Left_dimensions, Right_dimensions
             )
             ROIAX, Rnumber, Rpositions, ROIR = General_functions.Search_for_labels(
                 Cs,
                 ROIAX,
                 CenPoints,
                 onY,
                 BCs,
                 TYLshift,
                 Side,
                 Left_dimensions,
                 Right_dimensions,
-                input_image_filename,
+                cv2_img,
                 ROI2,
                 ROI3,
             )
+        except Exception:
+            traceback.print_exc()  # prints the error message and traceback
+            print("Failed Axes search")
+            
+            Fail = Fail + 1
+            pass
+
+        try:
+            Xplot, Yplot, Ynought = General_functions.Plot_Digitized_data(
+                Rticks=Rnumber, Rlocs=Rpositions, Lticks=Lnumber, Llocs=Lpositions
+            )
+            
+            try:  # Refine segmentation
+                refined_segmentation_mask, top_curve_mask = General_functions.Segment_refinement(
+                    cv2_img, Xmin, Xmax, Ymin, Ymax
+                )
+            except Exception:
+                traceback.print_exc()  # prints the error message and traceback
+                print("Failed Segment refinement")
+                Fail = Fail + 1
+                pass
+
             col = General_functions.Annotate(
-                input_image_filename=input_image_filename,
+                input_image_obj=colRGBA,
                 refined_segmentation_mask=refined_segmentation_mask,
                 Left_dimensions=Left_dimensions,
                 Right_dimensions=Right_dimensions,
                 Waveform_dimensions=Waveform_dimensions,
                 Left_axis=ROIL,
                 Right_axis=ROIR,
             )
@@ -254,38 +267,29 @@
             fig1, ax1 = plt.subplots(1)
             ax1.imshow(col)
             ax1.set_xticks([])
             ax1.set_yticks([])
             ax1.tick_params(axis="both", which="both", length=0)
             fig1.savefig(Annotated_path, dpi=900, bbox_inches="tight", pad_inches=0)
             Annotated_scans.append(Annotated_path)
-        except Exception:
-            traceback.print_exc()  # prints the error message and traceback
-            print("Failed Axes search")
-            Annotated_scans.append(None)
-            Fail = Fail + 1
-            pass
 
-        try:
-            Xplot, Yplot = General_functions.Plot_Digitized_data(
-                Rticks=Rnumber, Rlocs=Rpositions, Lticks=Lnumber, Llocs=Lpositions
-            )
             try:
                 df = General_functions.Plot_correction(Xplot, Yplot, df)
                 Text_data.append(df)
             except Exception:
                 traceback.print_exc()
                 print("Failed correction")
                 continue
             Digitized_path = output_dir + image_name.partition(".")[0] + "_Digitized.png"
             plt.figure(2)
             plt.savefig(Digitized_path, dpi=900, bbox_inches="tight", pad_inches=0)
             Digitized_scans.append(Digitized_path)
         except Exception:
             print("Failed Digitization")
+            Annotated_scans.append(None)
             traceback.print_exc()
             try:
                 Text_data.append(df)
             except Exception:
                 traceback.print_exc()
                 Text_data.append(None)
             Digitized_scans.append(None)
@@ -324,8 +328,10 @@
             pickle_path = toml.load("config.toml")["pickle"]["segmented_data"]
         with open(pickle_path, "wb") as f:
             pickle.dump([filenames, Digitized_scans, Annotated_scans, Text_data], f)
     i = 0
     return (filenames, Digitized_scans, Annotated_scans, Text_data)
 
 if __name__ == "__main__":
-    segment()
+    setup_tesseract()
+    pickle_file = toml.load("config.toml")["pickle"]["likely_us_images"]
+    segment(filenames=pickle_file)
```

### Comparing `usseg-0.2.0a2/usseg/main.py` & `usseg-0.4.0/usseg/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 def main(root_dir):
     """Main function that performs all of the segmentation on a root directory"""
 
     # Checks and sets up the tesseract environment
     usseg.setup_tesseract()
 
     # Gets a list of likely ultrasound images from root dir and saves them to a pickle file.
-    usseg.get_likely_us(root_dir)
+    filenames = usseg.get_likely_us(root_dir)
 
     # Segments and digitises the pre-selected ultrasound images.
-    usseg.segment()
+    usseg.segment(filenames)
 
     # Generates an output.html of the segmented output
     usseg.generate_html_from_pkl()
 
 if __name__ == "__main__":
     root_dir = toml.load("config.toml")["root_dir"]
     main(root_dir)
```

### Comparing `usseg-0.2.0a2/usseg/visualisation_html.py` & `usseg-0.4.0/usseg/visualisation_html.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pickle
 from PIL import Image
 
 # Module imports
 import plotly.graph_objs as go
 import plotly.offline as pyo
 import pandas as pd
+import toml
 
 def generate_html(scans, Annotated_scans, Digitized_scans, tables):
     # Check if the number of scan paths and data tables match
     if len(scans) != len(tables):
         raise ValueError("The number of scan paths and data tables do not match.")
     
     # Start building the HTML string
@@ -99,15 +100,16 @@
     
     return html_str
 
 def generate_html_from_pkl():
     """Generates a html file from the previously processed pickle files"""
 
     # Loading lists from the saved file
-    with open('lists3.pickle', 'rb') as f:
+    pickle_file = toml.load("config.toml")["pickle"]["segmented_data"]
+    with open(pickle_file, 'rb') as f:
         scan_paths,Digitized_scans, Annotated_scans,Text_data = pickle.load(f)
 
     html_str = generate_html(scan_paths, Annotated_scans, Digitized_scans, Text_data)
     with open('output.html', 'w') as f:
         f.write(html_str)
 
 if __name__ == "__main__":
```

### Comparing `usseg-0.2.0a2/PKG-INFO` & `usseg-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: usseg
-Version: 0.2.0a2
+Version: 0.4.0
 Summary: Tools to segment doppler ultrasound signals from scan images.
 License: GPL-v3-or-later
 Author: Dale Kernot
 Author-email: 874043@swansea.ac.uk
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: nibabel (>=5.1.0,<6.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
+Requires-Dist: opencv-contrib-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
-Requires-Dist: sklearn (>=0.0.post5,<0.1)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Doppler Segmetnations
 
 These codes make up the framework for segmenting the doppler ultrasound scans.
 
@@ -43,14 +43,31 @@
   - [Plot\_correction](#plot_correction)
   - [Annotate](#annotate)
   - [Contributing](#contributing)
   - [License](#license)
 
 ## Installation
 
+- To install as a dependency for your project:
+
+``` 
+pip install usseg
+```
+
+or
+
+``` sh
+poetry add usseg
+```
+
+
+### Development Environment
+
+To install the development environment follow the following steps.
+
 - Clone this repository and change into the directory.
 - Install [poetry](https://python-poetry.org/docs/) as per the installation instructions.
 - Install [tesseract](https://github.com/tesseract-ocr/tesseract) as per the intallation instructions.
 - Install the package dependencies with:
 ```
 poetry install
 
@@ -60,14 +77,16 @@
 ```
 poetry shell
 ```
 
 - You are now in the development environment!
 - Copy `config_example.toml` to `config.toml` and change the variables for your local set up (e.g. path to your data etc.).
 - The main script can now be run in one complete run with `python usseg/main.py`.
+- If debugging in vscode, ensure the python interpreter is set to the virtual environment created poetry. This path can be found using ```poetry env info --path```
+
 
 # Functions
 
 Provide instructions on how to use your project.
 
 ## Initial_segmentation
```

