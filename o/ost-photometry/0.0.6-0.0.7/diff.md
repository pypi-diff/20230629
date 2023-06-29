# Comparing `tmp/ost_photometry-0.0.6.tar.gz` & `tmp/ost_photometry-0.0.7.tar.gz`

## Comparing `ost_photometry-0.0.6.tar` & `ost_photometry-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/__init__.py
--rwxr-xr-x   0        0        0    21964 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/aux.py
--rwxr-xr-x   0        0        0     6453 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/calibration_data.py
--rwxr-xr-x   0        0        0     5281 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/checks.py
--rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/style.py
--rwxr-xr-x   0        0        0     1761 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/terminal_output.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/analyze/__init__.py
--rwxr-xr-x   0        0        0   166982 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/analyze/analyze.py
--rwxr-xr-x   0        0        0    82799 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/analyze/aux.py
--rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/analyze/calib.py
--rwxr-xr-x   0        0        0    32008 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/analyze/correlate.py
--rwxr-xr-x   0        0        0    65772 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/analyze/plot.py
--rwxr-xr-x   0        0        0    60779 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/analyze/trans.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/reduce/__init__.py
--rwxr-xr-x   0        0        0    67568 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/reduce/aux.py
--rwxr-xr-x   0        0        0    10487 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/reduce/plot.py
--rwxr-xr-x   0        0        0    75694 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/src/ost_photometry/reduce/redu.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/LICENSE
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/README.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 ost_photometry-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/__init__.py
+-rwxr-xr-x   0        0        0    21964 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/aux.py
+-rwxr-xr-x   0        0        0     6453 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/calibration_data.py
+-rwxr-xr-x   0        0        0     5281 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/checks.py
+-rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/style.py
+-rwxr-xr-x   0        0        0     1761 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/terminal_output.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/__init__.py
+-rwxr-xr-x   0        0        0   166982 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/analyze.py
+-rwxr-xr-x   0        0        0    84313 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/aux.py
+-rwxr-xr-x   0        0        0    30838 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/calib.py
+-rwxr-xr-x   0        0        0    32008 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/correlate.py
+-rwxr-xr-x   0        0        0    66907 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/plot.py
+-rwxr-xr-x   0        0        0    60779 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/trans.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/reduce/__init__.py
+-rwxr-xr-x   0        0        0    67568 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/reduce/aux.py
+-rwxr-xr-x   0        0        0    10487 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/reduce/plot.py
+-rwxr-xr-x   0        0        0    76037 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/reduce/redu.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/LICENSE
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/README.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/PKG-INFO
```

### Comparing `ost_photometry-0.0.6/src/ost_photometry/aux.py` & `ost_photometry-0.0.7/src/ost_photometry/aux.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.6/src/ost_photometry/calibration_data.py` & `ost_photometry-0.0.7/src/ost_photometry/calibration_data.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.6/src/ost_photometry/checks.py` & `ost_photometry-0.0.7/src/ost_photometry/checks.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.6/src/ost_photometry/terminal_output.py` & `ost_photometry-0.0.7/src/ost_photometry/terminal_output.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.6/src/ost_photometry/analyze/analyze.py` & `ost_photometry-0.0.7/src/ost_photometry/analyze/analyze.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.6/src/ost_photometry/analyze/aux.py` & `ost_photometry-0.0.7/src/ost_photometry/analyze/aux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1375,18 +1375,20 @@
             +' coefficients.',
             style_name='WARNING',
             )
 
     return None, None, None
 
 
-def check_variable(filename, filetype, filt_1, filt_2, cali, ISOcolumntype,
-                   ISOcolumn):
+def check_variable(filename, filetype, filt_1, filt_2, cali,
+                   ISOcolumntype, ISOcolumn):
     '''
-        Check variables and set defaults
+        Check variables and set defaults for CMDs and isochrone plots
+
+        This function exists for backwards compatibility.
 
         Parameters
         ----------
         filename            : `string`
             Specified file name - can also be empty -> set default
 
 
@@ -1404,14 +1406,50 @@
 
         ISOcolumntype       : `dictionary`
             Keys = filter - Values = type
 
         ISOcolumn           : `dictionary`
             Keys = filter - Values = column
     '''
+
+    filename, filetype = check_variable_apparent_cmd(
+        filename,
+        filetype,
+        filt_1,
+        filt_2,
+        cali,
+        )
+
+    check_variable_absolute_cmd(filt_1, filt_2, ISOcolumntype, ISOcolumn)
+
+    return filename, filetype
+
+
+def check_variable_apparent_cmd(filename, filetype, filt_1, filt_2, cali):
+    '''
+        Check variables and set defaults for CMDs and isochrone plots
+
+        Parameters
+        ----------
+        filename            : `string`
+            Specified file name - can also be empty -> set default
+
+
+        filetype            : `string`
+            Specified file type - can also be empty -> set default
+
+        filt_1              : `string`
+            First filter
+
+        filt_2              : `string`
+            Second filter
+
+        cali                : `dictionary`
+            Keys = filter - Values = zero points
+    '''
     #   Set figure type
     if filename == "?" or filename =="":
         terminal_output.print_terminal(
             indent=1,
             string='[Warning] No filename given, us default (cmd)',
             style_name='WARNING',
             )
@@ -1432,20 +1470,18 @@
             indent=1,
             string='[Warning] Unknown filetype given, use default instead '\
                   +'(pdf)',
             style_name='WARNING',
             )
         filetype = 'pdf'
 
-    return filename, filetype
-
     #   Check if calibration parameter is consistent with the number of
     #   filter
-    if len(filt_2) != len(cali):
-        if len(filt_2) > len(cali):
+    if len(filt_2) + len(filt_1) != len(cali):
+        if len(filt_2) + len(filt_1) > len(cali):
             terminal_output.print_terminal(
                 indent=1,
                 string="[Error] More filter ('filt_2') specified than zero"\
                 +" points ('cali')",
                 style_name='WARNING',
             )
             sys.exit()
@@ -1454,14 +1490,35 @@
                 indent=1,
                 string="[Error] More zero points ('cali') specified than "\
                 +"filter ('filt_2')",
                 style_name='WARNING',
             )
             sys.exit()
 
+    return filename, filetype
+
+
+def check_variable_absolute_cmd(filt_1, filt_2, ISOcolumntype, ISOcolumn):
+    '''
+        Check variables and set defaults for CMDs and isochrone plots
+
+        Parameters
+        ----------
+        filt_1              : `string`
+            First filter
+
+        filt_2              : `string`
+            Second filter
+
+        ISOcolumntype       : `dictionary`
+            Keys = filter - Values = type
+
+        ISOcolumn           : `dictionary`
+            Keys = filter - Values = column
+    '''
     #   Check if the column declaration for the isochrones fits to the
     #   specified filter
     for fil in filt_2:
         if fil not in ISOcolumntype.keys():
             terminal_output.print_terminal(
                 fil,
                 indent=1,
```

### Comparing `ost_photometry-0.0.6/src/ost_photometry/analyze/calib.py` & `ost_photometry-0.0.7/src/ost_photometry/analyze/calib.py`

 * *Files 0% similar despite different names*

```diff
@@ -536,16 +536,16 @@
             arr = calib_tbl[col_names['mag'+band]]
             if hasattr(arr, 'mask'):
                 ind_rm = np.where(arr.mask)
                 calib_tbl.remove_rows(ind_rm)
 
     if not calib_tbl:
         raise RuntimeError(
-            f"{style.bcolors.FAIL} \nNo calibration star with {band} "
-            f"magnitude found. -> EXIT {style.bcolors.ENDC}"
+            f"{style.bcolors.FAIL} \nNo calibration star with {band_list} "
+            f"magnitudes found. -> EXIT {style.bcolors.ENDC}"
             )
     terminal_output.print_terminal(
         len(calib_tbl),
         indent=indent+2,
         string="Of these {} are useful",
         style_name='OKBLUE',
         )
```

### Comparing `ost_photometry-0.0.6/src/ost_photometry/analyze/correlate.py` & `ost_photometry-0.0.7/src/ost_photometry/analyze/correlate.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.6/src/ost_photometry/analyze/plot.py` & `ost_photometry-0.0.7/src/ost_photometry/analyze/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     #   Save the plot
     plt.savefig(outdir+'/img_comparison.pdf', bbox_inches='tight',format='pdf')
     plt.close()
 
 
 def starmap(outdir, image, band, tbl, indent=2, tbl_2=None,
             label='Identified stars', label_2='Identified stars (set 2)',
-            rts=None, mode=None, nameobj='', condense=False):
+            rts=None, mode=None, nameobj=None, condense=False):
     '''
         Plot star maps  -> overlays of the determined star positions on FITS
                         -> supports different versions
 
         Parameters
         ----------
         outdir          : `string`
@@ -119,15 +119,15 @@
 
         mode            : `string`, optional
             String used to switch between different plot modes
             Default is ``None``
 
         nameobj         : `string`, optional
             Name of the object
-            Default is ````
+            Default is ``None``
 
         condense        : `boolean`, optional
             If True pass the console output to the calling function.
             Default is ``False``.
     '''
     #   Check output directories
     checks.check_out(
@@ -176,24 +176,24 @@
                 f"table 2. {style.bcolors.ENDC}"
                 )
 
     #   Set layout of image
     fig = plt.figure(figsize=(20,9))
 
     #   Set title of the complete plot
-    if rts is not None:
-        fig.suptitle(
-            'Star map ('+str(band)+' band, '+rts+') - '+nameobj,
-            fontsize=20,
-            )
+    if rts is None and nameobj is None:
+        sub_titel = f'Star map ({band} band)'
+    elif rts is None:
+        sub_titel = f'Star map ({band} band) - {nameobj}'
+    elif nameobj is None:
+        sub_titel = f'Star map ({band} band, {rts})'
     else:
-        fig.suptitle(
-            'Star map ('+str(band)+' band) - '+nameobj,
-            fontsize=20,
-            )
+        sub_titel = f'Star map ({band} band, {rts}) - {nameobj}'
+
+    fig.suptitle(sub_titel, fontsize=20)
 
     #   Set up normalization for the image
     norm = ImageNormalize(image, interval=ZScaleInterval())
 
     #   Display the actual image
     plt.imshow(image, cmap='Greys', origin='lower', norm=norm,
                interpolation='nearest')
@@ -378,15 +378,15 @@
         bbox_inches='tight',
         format='pdf',
         )
     plt.close()
 
 
 def plot_cutouts(outdir, stars, string, condense=False, max_plot_stars=25,
-                 nameobj='', indent=2):
+                 nameobj=None, indent=2):
     '''
         Plot the cutouts of the stars used to estimated the ePSF
 
         Parameters
         ----------
         outdir          : `string`
             Output directory
@@ -403,15 +403,15 @@
 
         max_plot_stars  : `integer`, optional
             Maximum number of cutouts to plot
             Default is ``25``.
 
         nameobj         : `string`, optional
             Name of the object
-            Default is ````.
+            Default is ``None``.
 
         indent          : `integer`, optional
             Indentation for the console output lines.
             Default is ``2``.
     '''
     #   Check output directories
     checks.check_out(
@@ -440,19 +440,19 @@
     #   Prepare plot
     fig, ax = plt.subplots(nrows=nrows, ncols=ncols, figsize=(20, 15),
                            squeeze=True)
     plt.subplots_adjust(left=None, bottom=None, right=None, top=None,
                         wspace=None, hspace=0.25)
 
     #   Set title of the complete plot
-    fig.suptitle(
-        'Cutouts of the '+str(n_cutouts)+' faintest stars ('
-        +str(string)+') - '+nameobj,
-        fontsize=20,
-        )
+    if nameobj is None:
+        sub_titel = f'Cutouts of the {n_cutouts} faintest stars ({string})'
+    else:
+        sub_titel = f'Cutouts of the {n_cutouts} faintest stars ({string}) - {nameobj}'
+    fig.suptitle(sub_titel, fontsize=20)
 
     ax = ax.ravel()                             # flatten the image?
 
     #   Loop over the cutouts (default: 25)
     for i in range(n_cutouts):
         # Remove bad pixels that would spoil the image normalization
         data_image = np.where(stars[i].data<=0, 1E-7, stars[i].data)
@@ -467,15 +467,15 @@
     # plt.show()
     plt.close()
 
     if condense:
         return outstr
 
 
-def plot_epsf(outdir, epsf, condense=False, nameobj='', indent=1):
+def plot_epsf(outdir, epsf, condense=False, nameobj=None, indent=1):
     '''
         Plot the ePSF image of all filters
 
         Parameters
         ----------
         outdir          : `string`
             Output directory
@@ -485,15 +485,15 @@
 
         condense        : `boolean`, optional
             If True pass the console output to the calling function
             Default is ``False``.
 
         nameobj         : `string`, optional
             Name of the object
-            Default is ````.
+            Default is ``None``.
 
         indent          : `integer`, optional
             Indentation for the console output lines
             Default is ``1``.
     '''
     #   Check output directories
     checks.check_out(
@@ -517,15 +517,18 @@
     elif nplots == 2:
         fig = plt.figure(figsize=(13,5))
     else:
         fig = plt.figure(figsize=(20,15))
 
 
     #   Set title of the complete plot
-    fig.suptitle('ePSF ('+nameobj+')', fontsize=20)
+    if nameobj is None:
+        fig.suptitle('ePSF', fontsize=20)
+    else:
+        fig.suptitle(f'ePSF ({nameobj})', fontsize=20)
 
     #   Plot individual subplots
     for i, (band, eps) in enumerate(epsf.items()):
         #   Remove bad pixels that would spoil the image normalization
         epsf_clean = np.where(eps.data<=0, 1E-7, eps.data)
         #   Set up normalization for the image
         norm = simple_norm(epsf_clean, 'log', percent=99.)
@@ -568,15 +571,15 @@
     plt.close()
 
     if condense:
         return outstr
 
 
 def plot_residual(name, image_orig, residual_image, outdir,
-                  condense=False, nameobj='', indent=1):
+                  condense=False, nameobj=None, indent=1):
     '''
         Plot the original and the residual image
 
         Parameters
         ----------
         name            : `string`
             Name of the plot, can be name of the object
@@ -592,15 +595,15 @@
 
         condense        : `boolean`, optional
             If True pass the console output to the calling function
             Default is ``False``.
 
         nameobj         : `string`, optional
             Name of the object
-            Default is ````.
+            Default is ``None``.
 
         indent          : `integer`, optional
             Indentation for the console output lines
             Default is ``1``.
     '''
     #   Check output directories
     checks.check_out(
@@ -632,15 +635,18 @@
         right=None,
         top=None,
         wspace=None,
         hspace=0.25,
         )
 
     #   Set title of the complete plot
-    fig.suptitle(name+' ('+nameobj+')', fontsize=20)
+    if nameobj is None:
+        fig.suptitle(name, fontsize=20)
+    else:
+        fig.suptitle(f'{name} ({nameobj})', fontsize=20)
 
     i = 1
     for band, image in image_orig.items():
         ##  Plot original image
         #   Set up normalization for the image
         norm = ImageNormalize(image, interval=ZScaleInterval())
 
@@ -718,15 +724,15 @@
     plt.close()
 
     if condense:
         return outstr
 
 
 def plot_mags(mag1, name1, mag2, name2, rts, outdir, err1=None, err2=None,
-              nameobj='', fit=None):
+              nameobj=None, fit=None):
     '''
         Plot magnitudes
 
         Parameters
         ----------
         mag1        : `numpy.ndarray`
             Magnitudes of filter 1
@@ -752,25 +758,25 @@
 
         err2        : `numpy.ndarray' or ``None``, optional
             Error of the filter 1 magnitudes
             Default is ``None``.
 
         nameobj     : `string`, optional
             Name of the object
-            Default is ````
+            Default is ``None``
 
         fit             : ` astropy.modeling.fitting` instance, optional
             Fit to plot
             Default is ``None``.
     '''
     scatter(mag1, name1+" [mag]", mag2, name2+" [mag]", rts, outdir, err1=err1,
               err2=err2, nameobj=nameobj, fit=fit)
 
 
-def sigma_plot(bv, mags, bands, band, nr, outdir, nameobj='', fit=None):
+def sigma_plot(bv, mags, bands, band, nr, outdir, nameobj=None, fit=None):
     '''
         Illustrate sigma clipping of magnitudes
 
         Parameters
         ----------
         bv          : `numpy.ndarray`
             Delta color - (mag_2-mag_1)_observed - (mag_2-mag_1)_literature
@@ -788,15 +794,15 @@
             Number of the star to plot
 
         outdir      : `string`
             Output directory
 
         nameobj     : `string`, optional
             Name of the object
-            Default is ````.
+            Default is ``None``.
 
         fit             : ` astropy.modeling.fitting` instance, optional
             Fit to plot
             Default is ``None``.
     '''
     #   Check output directories
     checks.check_out(
@@ -811,18 +817,19 @@
     mag_clip = mags[mask]
 
 
     #   Plot sigma clipped magnitudes
     fig = plt.figure(figsize=(8,8))
 
     #   Set title
-    fig.suptitle(
-        'Sigma clipped magnitudes -- star: '+str(nr)+' ('+nameobj+')',
-        fontsize=20,
-        )
+    if nameobj is None:
+        sub_titel = f'Sigma clipped magnitudes -- star: {nr}'
+    else:
+        sub_titel = f'Sigma clipped magnitudes -- star: {nr} ({nameobj})'
+    fig.suptitle(sub_titel, fontsize=20)
 
     #   Plot data
     plt.plot(mags,bv,color='blue',marker='.',linestyle='none')
     plt.plot(mag_clip,clip_bv,color='red',marker='.',linestyle='none')
 
 
     #   Plot fit
@@ -844,15 +851,15 @@
     plt.savefig(outdir+'/sigmag/'+str(nr)+'_'+str(band)
                 +'.png',bbox_inches='tight',format='png')
     plt.close()
     #plt.show()
 
 
 def light_curve_jd(ts, data_column, err_column, outdir, error_bars=True,
-                   nameobj=''):
+                   nameobj=None):
     '''
         Plot the light curve over Julian Date
 
         Parameters
         ----------
         ts          : `astropy.timeseries.TimeSeries`
             Time series
@@ -868,15 +875,15 @@
 
         error_bars  : `boolean`, optional
             If True error bars will be plotted.
             Default is ``False``.
 
         nameobj     : `string`, optional
             Name of the object
-            Default is ````.
+            Default is ``None``.
     '''
     #   Check output directories
     checks.check_out(
         outdir,
         os.path.join(outdir, 'lightcurve'),
         )
 
@@ -886,15 +893,18 @@
     #
     fig = plt.figure(figsize=(20,9))
 
     #   Plot grid
     plt.grid(True)
 
     #   Set title
-    fig.suptitle(f'Light curve - {nameobj}', fontsize=30)
+    if nameobj is None:
+        fig.suptitle(f'Light curve', fontsize=30)
+    else:
+        fig.suptitle(f'Light curve - {nameobj}', fontsize=30)
 
     #   Plot data with or without error bars
     if not error_bars:
         plt.plot(ts.time.jd, ts[data_column], 'k.', markersize=3)
     else:
         plt.errorbar(
             ts.time.jd,
@@ -942,15 +952,15 @@
         bbox_inches='tight',
         format='pdf',
         )
     plt.close()
 
 
 def light_curve_fold(ts, data_column, err_column, outdir, transit_time,
-                     period, binn=None, error_bars=True, nameobj=''):
+                     period, binn=None, error_bars=True, nameobj=None):
     '''
         Plot a folded light curve
 
         Parameters
         ----------
         ts              : `astropy.timeseries.TimeSeries`
             Time series
@@ -976,15 +986,15 @@
 
         error_bars  : `boolean`, optional
             If True error bars will be plotted.
             Default is ``False``.
 
         nameobj     : `string`, optional
             Name of the object
-            Default is ````.
+            Default is ``None``.
     '''
     #   Check output directories
     checks.check_out(
         outdir,
         os.path.join(outdir, 'lightcurve'),
         )
 
@@ -997,15 +1007,18 @@
 
     ###
     #   Make plot
     #
     fig = plt.figure(figsize=(20,9))
 
     #   Set title
-    fig.suptitle('Folded light curve - '+nameobj, fontsize=30)
+    if nameobj is None:
+        fig.suptitle('Folded light curve', fontsize=30)
+    else:
+        fig.suptitle(f'Folded light curve - {nameobj}', fontsize=30)
 
     #   Calculate binned lightcurve
     if binn is not None:
         ts_binned = aggregate_downsample(
             ts_folded,
             time_bin_size=binn * u.day,
             )
@@ -1086,15 +1099,15 @@
     plt.savefig(outdir+'/lightcurve/lightcurve_folded_'+str(data_column)
                 +'.pdf', bbox_inches='tight', format='pdf')
     plt.close()
 
 
 def plot_transform(outdir, color1, color2, color_lit, fit_var, a, b, b_err,
                    fit_func, airmass, filt=None, color_lit_err=None,
-                   fit_var_err=None, nameobj=''):
+                   fit_var_err=None, nameobj=None):
     '''
         Make the plots to determine the calibration factors for the
         magnitude transformation
 
         Parameters
         ----------
         outdir          : `string`
@@ -1139,15 +1152,15 @@
 
         fit_var_err     : `numpy.ndarray`, optional
             Fit varaiable errors
             Default is ``None``.
 
         nameobj         : `string`
             Name of the object
-            Default is ````.
+            Default is ``None``.
     '''
     #   Check output directories
     checks.check_out(
         outdir,
         os.path.join(outdir, 'trans_plots'),
         )
 
@@ -1155,35 +1168,42 @@
     x_lin = np.sort(color_lit)
     y_lin = fit_func(x_lin,a,b)
 
     #   Set labels etc.
     airmass = round(airmass,2)
     if filt == None:
         #   coeff  = 1./b
-        titel  = 'Color transform ('+color1.lower()+'-'+color2.lower()\
-                 +' vs. '+color1+'-'+color2+') - '+nameobj\
-                 +' (X = '+str(airmass)+')'
-        ylabel = color1.lower()+'-'+color2.lower()+' [mag]'
-        path   = outdir+'/trans_plots/'+color1.lower()+color2.lower()\
-                 +'_'+color1+color2+'.pdf'
-        plabel = 'slope = '+str(b)+', T'+color1.lower()+color2.lower()\
-                 +' = '+str(1./b)+' +/- '+str(b_err)
+        if nameobj is None:
+            titel  = f'Color transform ({color1.lower()}-{color2.lower()}'\
+                    +f' vs. {color1}-{color2}) (X = {airmass})'
+        else:
+            titel  = f'Color transform ({color1.lower()}-{color2.lower()}'\
+                    +f' vs. {color1}-{color2}) - {nameobj} (X = {airmass})'
+        ylabel = f'{color1.lower()}-{color2.lower()} [mag]'
+        path   = f'{outdir}/trans_plots/{color1.lower()+color2.lower()}'\
+                 +f'_{color1+color2}.pdf'
+        plabel = f'slope = {b}, T{color1.lower()}{color2.lower()}'\
+                 +f' = {1./b} +/- {b_err}'
     else:
         #   coeff  = b
-        titel  = filt+color1.lower()+color2.lower()\
-                 +'-mag transform ('+filt+'-'+filt.lower()\
-                 +' vs. '+color1+'-'+color2+') - '+nameobj\
-                 +' (X = '+str(airmass)+')'
-        ylabel = filt+'-'+filt.lower()+' [mag]'
-        path   = outdir+'/trans_plots/'+filt+filt.lower()\
-                 +'_'+color1+color2+'.pdf'
-        plabel = 'slope = '+str(b)+', C'+filt.lower()+'_'\
-                 +color1.lower()+color2.lower()+' = '+str(b)\
-                 +' +/- '+str(b_err)
-    xlabel = color1+'-'+color2+' [mag]'
+        if nameobj is None:
+            titel  = f'{filt}{color1.lower()}{color2.lower()}'\
+                    +f'-mag transform ({filt}-{filt.lower()}'\
+                    +f' vs. {color1}-{color2}) (X = {airmass})'
+        else:
+            titel  = f'{filt}{color1.lower()}{color2.lower()}'\
+                    +f'-mag transform ({filt}-{filt.lower()}'\
+                    +f' vs. {color1}-{color2}) - {nameobj}'\
+                    +f' (X = {airmass})'
+        ylabel = f'{filt}-{filt.lower()} [mag]'
+        path   = f'{outdir}/trans_plots/{filt}{filt.lower()}'\
+                 +f'_{color1}{color2}.pdf'
+        plabel = f'slope = {b}, C{filt.lower()}_'\
+                 +f'{color1.lower()}{color2.lower()} = {b} +/- {b_err}'
+    xlabel = f'{color1}-{color2} [mag]'
 
     #   Make plot
     fig = plt.figure(figsize=(20,9))
 
     #   Set title
     fig.suptitle(titel, fontsize=30)
 
@@ -2279,15 +2299,15 @@
             bbox_inches='tight',
             format='pdf',
             )
         plt.close()
 
 
 def scatter(value1, name1, value2, name2, rts, outdir, err1=None, err2=None,
-            nameobj='', fit=None):
+            nameobj=None, fit=None):
     '''
         Plot magnitudes
 
         Parameters
         ----------
         value1      : `numpy.ndarray`
             Magnitudes of filter 1
@@ -2313,15 +2333,15 @@
 
         err2        : `numpy.ndarray' or ``None``, optional
             Error of value 2
             Default is ``None``.
 
         nameobj     : `string`, optional
             Name of the object
-            Default is ````
+            Default is ``None``
 
         fit             : ` astropy.modeling.fitting` instance, optional
             Fit to plot
             Default is ``None``.
     '''
     #   Check output directories
     checks.check_out(
@@ -2329,16 +2349,20 @@
         os.path.join(outdir, 'scatter'),
         )
 
     #   Plot magnitudes
     fig = plt.figure(figsize=(8,8))
 
     #   Set title
+    if nameobj is None:
+        sub_titel = f'{name1} vs. {name2}:'
+    else:
+        sub_titel = f'{name1} vs. {name2} ({nameobj}):'
     fig.suptitle(
-        name1+' vs. '+name2+' ('+nameobj+'):',
+        sub_titel,
         fontsize=20,
         )
 
     #   Plot data
     plt.errorbar(
         value1,
         value2,
```

### Comparing `ost_photometry-0.0.6/src/ost_photometry/analyze/trans.py` & `ost_photometry-0.0.7/src/ost_photometry/analyze/trans.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.6/src/ost_photometry/reduce/aux.py` & `ost_photometry-0.0.7/src/ost_photometry/reduce/aux.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.6/src/ost_photometry/reduce/plot.py` & `ost_photometry-0.0.7/src/ost_photometry/reduce/plot.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.6/src/ost_photometry/reduce/redu.py` & `ost_photometry-0.0.7/src/ost_photometry/reduce/redu.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 def reduce_main(path, outdir, img_type=None, gain=None, readnoise=None,
                 dr=None, cosmics=True, mask_cosmics=False, satlevel=None,
                 objlim=5., sigclip=4.0, scale_expo=True, ref_img=0,
                 bias_enforce=False, verbose=False, addmask=True,
                 shift_method='skimage', stack=True, estimate_fwhm=False,
                 shift_all=False, tolerance=0.5, stack_method='average',
                 target=None, find_wcs=True, wcs_method='astrometry',
-                wcs_all=False, rm_outliers_shift=True, filter_window_shift=8,
-                threshold_shift=10., debug=False):
+                wcs_all=False, force_wcs_determ=False, rm_outliers_shift=True,
+                filter_window_shift=8, threshold_shift=10., debug=False):
     '''
         Main reduction routine: Creates master images for bias, darks,
                                 flats, reduces the science images and trims
                                 them to the same filed of view.
 
 
         Reduce the science images
@@ -172,14 +172,19 @@
             Default is ``astrometry``.
 
         wcs_all             : `boolean`, optional
             If `True` the WCS will be calculated for each image
             individually.
             Default is ``False``.
 
+        force_wcs_determ    : `boolean`, optional
+            If ``True`` a new WCS determination will be calculated even if
+            a WCS is already present in the FITS Header.
+            Default is ``False``.
+
         rm_outliers_shift   : `boolean`, optional
             If True outliers in the image shifts will be detected and removed.
             Default is ``True``.
 
         filter_window_shift : `integer`, optional
             Width of the median filter window
             Default is ``8``.
@@ -472,21 +477,23 @@
         #
         terminal_output.print_terminal(string="Determine WCS ...", indent=1)
         if wcs_all:
             aux.find_wcs_all_imgs(
                 out_path / 'cut',
                 out_path / 'cut',
                 method=wcs_method,
+                force_wcs_determ=force_wcs_determ,
                 )
         else:
             aux.find_wcs(
                 out_path / 'cut',
                 out_path / 'cut',
                 ref_id=ref_img,
                 method=wcs_method,
+                force_wcs_determ=force_wcs_determ,
                 )
 
     if estimate_fwhm:
         ###
         #   Estimate FWHM
         #
         terminal_output.print_terminal(string="Estimate FWHM ...", indent=1)
```

### Comparing `ost_photometry-0.0.6/LICENSE` & `ost_photometry-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.6/pyproject.toml` & `ost_photometry-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ost_photometry"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Rainer Hainich", email="rhainich@astro.physik.uni-potsdam.de" },
 ]
 description = "Phtometry reduction and analysis package for the OST observatory"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `ost_photometry-0.0.6/PKG-INFO` & `ost_photometry-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ost_photometry
-Version: 0.0.6
+Version: 0.0.7
 Summary: Phtometry reduction and analysis package for the OST observatory
 Project-URL: Homepage, https://github.com/OST-Observatory/ost_photometry_package
 Project-URL: Bug Tracker, https://github.com/OST-Observatory/ost_photometry_package/issues
 Author-email: Rainer Hainich <rhainich@astro.physik.uni-potsdam.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

