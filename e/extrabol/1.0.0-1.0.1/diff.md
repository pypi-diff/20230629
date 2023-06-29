# Comparing `tmp/extrabol-1.0.0.tar.gz` & `tmp/extrabol-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/extrabol-1.0.0.tar", last modified: Thu Oct 20 17:32:55 2022, max compression
+gzip compressed data, was "extrabol-1.0.1.tar", last modified: Thu Jun 29 17:17:41 2023, max compression
```

## Comparing `extrabol-1.0.0.tar` & `extrabol-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2022-10-20 17:32:55.000000 extrabol-1.0.0/
--rw-r--r--   0 ian       (1000) ian       (1000)     3776 2022-10-20 17:32:55.000000 extrabol-1.0.0/PKG-INFO
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2022-10-20 17:32:55.000000 extrabol-1.0.0/extrabol/
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2022-10-20 17:30:32.000000 extrabol-1.0.0/extrabol/__init__.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2022-10-20 17:32:55.000000 extrabol-1.0.0/extrabol/example/
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2022-10-20 17:30:32.000000 extrabol-1.0.0/extrabol/example/__init__.py
--rw-r--r--   0 ian       (1000) ian       (1000)    36285 2022-10-20 17:30:32.000000 extrabol-1.0.0/extrabol/extrabol.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2022-10-20 17:32:55.000000 extrabol-1.0.0/extrabol/template_bank/
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2022-10-20 17:30:32.000000 extrabol-1.0.0/extrabol/template_bank/__init__.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2022-10-20 17:32:55.000000 extrabol-1.0.0/extrabol.egg-info/
--rw-r--r--   0 ian       (1000) ian       (1000)     3776 2022-10-20 17:32:55.000000 extrabol-1.0.0/extrabol.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)      318 2022-10-20 17:32:55.000000 extrabol-1.0.0/extrabol.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2022-10-20 17:32:55.000000 extrabol-1.0.0/extrabol.egg-info/dependency_links.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       53 2022-10-20 17:32:55.000000 extrabol-1.0.0/extrabol.egg-info/entry_points.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       74 2022-10-20 17:32:55.000000 extrabol-1.0.0/extrabol.egg-info/requires.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        9 2022-10-20 17:32:55.000000 extrabol-1.0.0/extrabol.egg-info/top_level.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       84 2022-10-20 17:32:55.000000 extrabol-1.0.0/setup.cfg
--rw-r--r--   0 ian       (1000) ian       (1000)     1257 2022-10-20 17:30:32.000000 extrabol-1.0.0/setup.py
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 17:17:41.835362 extrabol-1.0.1/
+-rw-r--r--   0 ian       (1000) ian       (1000)     1058 2023-06-29 17:17:27.000000 extrabol-1.0.1/LICENSE
+-rw-r--r--   0 ian       (1000) ian       (1000)     3921 2023-06-29 17:17:41.835362 extrabol-1.0.1/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)     3411 2023-06-29 17:17:27.000000 extrabol-1.0.1/README.md
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 17:17:41.825362 extrabol-1.0.1/extrabol/
+-rw-r--r--   0 ian       (1000) ian       (1000)        0 2023-06-29 17:17:27.000000 extrabol-1.0.1/extrabol/__init__.py
+-rw-r--r--   0 ian       (1000) ian       (1000)    36969 2023-06-29 17:17:27.000000 extrabol-1.0.1/extrabol/extrabol.py
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 17:17:41.835362 extrabol-1.0.1/extrabol.egg-info/
+-rw-r--r--   0 ian       (1000) ian       (1000)     3921 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)      268 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/SOURCES.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/dependency_links.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       52 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/entry_points.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       74 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/requires.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        9 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/top_level.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)      928 2023-06-29 17:17:27.000000 extrabol-1.0.1/pyproject.toml
+-rw-r--r--   0 ian       (1000) ian       (1000)       38 2023-06-29 17:17:41.835362 extrabol-1.0.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `extrabol-1.0.0/PKG-INFO` & `extrabol-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,122 @@
 Metadata-Version: 2.1
 Name: extrabol
-Version: 1.0.0
+Version: 1.0.1
 Summary: Estimate SN bolometric light curves
-Home-page: https://github.com/villrv/extrabol
-Author: Ian M. Thornton
-Author-email: iot5037@psu.edu
-License: UNKNOWN
-Description: Generate bolometric estimates of Supernovae
-        
-        Author: Ian Thornton
-        
-        Install with pip:
-        
-        ```bash
-        pip install extrabol
-        ```
-        # Usage
-        
-        ```
-        extrabol 'filename.dat' ARGUMENTS
-        ```
-        Optional Arguments:
-        ```
-        --verbose
-            Increase output verbosity
-        
-        -m MEAN, --mean MEAN
-            Use a supernova template as the mean function for the GP; Choose \'1a\',\'1bc\', \'2l\', \'2p\', or \'0\' (for no template)
-            Default = 0
-        
-        -t, --show-template
-            Shows supernova template on plots as dotted lines
-        
-        -d DIST, --dist DIST
-            Object luminosity distance in Mpc
-        
-        -z REDSHIFT, --redshift REDSHIFT
-            Object redshift
-            If no argument is provided, redshift will be read from the input file
-        
-        --dm DM
-            Object distance modulus
-        
-        --plot BOOL
-            Output plots, Default is TRUE
-        
-        --outdir OUTDIR
-            A file location for outputs to be written to
-        
-        --ebv EBV
-            Milky Way extinction E(B-V) value, if known
-            If no argument is probided the extinction will be read from the input file
-        
-        --hostebv HOSTEBV
-            Host extinction E(B-V)
-        
-        -s START, --start START
-            Start time of analysis window relative to peak luminosity
-            Default = -50 days
-        
-        -e END, --end END
-            End time of analysis window relative to peak luminosity
-            Default = 150 days
-        
-        -snr SNR
-            Minimum signal to noise ratio for observations
-            Default = 4.0
-        
-        -wc, --wvcorr
-            Use the redshift-corrected wavelength values for extinction calculations
-        
-        -mc, --use-mcmc
-            Use a Markov Chain Monte Carlo to fit black bodies instead of curve_fit.
-            This provides better error estimates but takes much longer.
-        
-        --T_max T_MAX
-            Modify the prior on temperature for blackbody fits by specifying a maximum temperature.
-            Default = 40,000K
-        ```
-        # Input Files
-        
-        Inputs to extrabol must be .dat files that conform to the following format.
-        
-        The first two lines must contain redshift and Milky Way extinction E(b-v) respectively. If these values are unknown, simply put 0.0.
-        The following lines contain observational data in 5 columns as shown below:
-        
-        ```
-        Time(MJD)   Apparent Magnitude   Error(in magnitudes)   Filter SVO ID   Type of magnitude (AB or Vega)
-        ```
-        Any white space can be used as the column delimiter. NaNs, non-detections, and data points with no error bars should not be included.
-        An example input file can be found under extrabol/example.
-        
-        # Example Input
-        
-        ```python
-        extrabol ./example/PSc000174_extrabol.dat --verbose -m 1a
-        ```
-        
-        This example may take a minute the first time you run it as astroquery fetches filter information!
-        
-        Filters must be specified by their [SVO](http://svo2.cab.inta-csic.es/svo/theory/fps3/) ID.
-        
-        
-Platform: UNKNOWN
+Author-email: "Ian M. Thornton" <iot5037@psu.edu>
+Project-URL: Repository, https://github.com/villrv/extrabol
+Project-URL: Documentation, https://extrabol.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![DOI](https://zenodo.org/badge/283353973.svg)](https://zenodo.org/badge/latestdoi/283353973)
+
+
+# extrabol
+
+`extrabol` is a Python 3.x package for rapidly and systematicaly estimating the bolometric luminosity and black body properties of (thermal) extragalactic transients from broadband UVONIR data. `extrabol` is broken down into three main steps:
+
+- Read in and pre-process a data file holding observations of a supernova or other transient event over time, through any number of broadband filters.
+- Interpolate this data using a Gaussian Process(GP), a non-physical, statistical model utilizing covariance.
+- Fit a series of blackbody curves to the interpolated data to estimate the bolometric luminosity, temperature, and radius of the transient over time.
+
+Author: Ian Thornton
+
+## Installation and Documentation
+
+Install with pip:
+
+```bash
+pip install extrabol
+```
+
+The latest documentation is available [here](https://extrabol.readthedocs.io/en/latest/).
+
+## Usage
+
+```
+extrabol 'filename.dat' ARGUMENTS
+```
+Optional Arguments:
+```
+--verbose
+    Increase output verbosity
+
+-m MEAN, --mean MEAN
+    Use a supernova template as the mean function for the GP; Choose \'1a\',\'1bc\', \'2l\', \'2p\', or \'0\' (for no template)
+    Default = 0
+
+-t, --show-template
+    Shows supernova template on plots as dotted lines
+
+-d DIST, --dist DIST
+    Object luminosity distance in Mpc
+
+-z REDSHIFT, --redshift REDSHIFT
+    Object redshift
+    If no argument is provided, redshift will be read from the input file
+
+--dm DM
+    Object distance modulus
+
+--plot BOOL
+    Output plots, Default is TRUE
+
+--outdir OUTDIR
+    A file location for outputs to be written to
+
+--ebv EBV
+    Milky Way extinction E(B-V) value, if known
+    If no argument is probided the extinction will be read from the input file
+
+--hostebv HOSTEBV
+    Host extinction E(B-V)
+
+-s START, --start START
+    Start time of analysis window relative to peak luminosity
+    Default = -50 days
+
+-e END, --end END
+    End time of analysis window relative to peak luminosity
+    Default = 150 days
+
+-snr SNR
+    Minimum signal to noise ratio for observations
+    Default = 4.0
+
+-wc, --wvcorr
+    Use the redshift-corrected wavelength values for extinction calculations
+
+-mc, --use-mcmc
+    Use a Markov Chain Monte Carlo to fit black bodies instead of curve_fit.
+    This provides better error estimates but takes much longer.
+
+--T_max T_MAX
+    Modify the prior on temperature for blackbody fits by specifying a maximum temperature.
+    Default = 40,000K
+```
+## Input Files
+
+Inputs to extrabol must be .dat files that conform to the following format.
+
+The first two lines must contain redshift and Milky Way extinction E(b-v) respectively. If these values are unknown, simply put 0.0.
+The following lines contain observational data in 5 columns as shown below:
+
+```
+Time(MJD)   Apparent Magnitude   Error(in magnitudes)   Filter SVO ID   Type of magnitude (AB or Vega)
+```
+Any white space can be used as the column delimiter. NaNs, non-detections, and data points with no error bars should not be included.
+An example input file can be found under extrabol/example.
+
+## Example Input
+
+```python
+extrabol ./example/PSc000174_extrabol.dat --verbose -m 1a
+```
+
+This example may take a minute the first time you run it as astroquery fetches filter information!
+
+Filters must be specified by their [SVO](http://svo2.cab.inta-csic.es/svo/theory/fps3/) ID.
```

### Comparing `extrabol-1.0.0/extrabol/extrabol.py` & `extrabol-1.0.1/extrabol/extrabol.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,39 +52,14 @@
     blam = ((2.*np.pi*h*c**2) / (lam_cm**5)) / (np.exp(exponential)-1.)
     area = 4. * np.pi * R**2
     lum = blam * area
 
     return lum
 
 
-def chi_square(dat, model, uncertainty):
-    '''
-    Calculate the chi squared of a model given a set of data
-
-    Parameters
-    ----------
-    dat : numpy.array
-        Experimental data for the model to be tested against
-    model : numpy.array
-        Model data being tested
-    uncertainty : numpy.array
-        Error on experimental data
-
-    Output
-    ------
-    chi2 : float
-        the chi sqaured value of the model
-    '''
-
-    chi2 = 0.
-    for i in np.arange(len(dat)):
-        chi2 += ((model[i]-dat[i]) / uncertainty[i])**2.
-
-    return chi2
-
 
 def read_in_photometry(filename, dm, redshift, start, end, snr, mwebv,
                        use_wc, verbose):
     '''
     Read in SN file
 
     Parameters
@@ -114,22 +89,26 @@
         Mean of wavelengths, used in GP pre-processing
     flux_corr : float
         Flux correction, used in GP pre-processing
     my_filters : list
         List of filter names
     '''
 
+    #if '.json' in filename:
+    #    # FOR ME: phases, mag, errs, filter
+    #else:
     photometry_data = np.loadtxt(filename, dtype=str, skiprows=2)
-
     # Extract key information into seperate arrays
     phases = np.asarray(photometry_data[:, 0], dtype=float)
     errs = np.asarray(photometry_data[:, 2], dtype=float)
     if verbose:
         print('Getting Filter Data...')
-    index = SvoFps.get_filter_index(timeout=3600)
+    index = SvoFps.get_filter_index(wavelength_eff_min=100*u.angstrom,
+                                    wavelength_eff_max=30000*u.angstrom,
+                                    timeout=3600)
     filterIDs = np.asarray(index['filterID'].data, dtype=str)
     wavelengthEffs = np.asarray(index['WavelengthEff'].data, dtype=float)
     widthEffs = np.asarray(index['WidthEff'].data, dtype=float)
     zpts_all = np.asarray(index['ZeroPoint'].data, dtype=str)
 
     # Extract filter names and effective wavelengths
     wv_effs = []
@@ -182,25 +161,28 @@
     # Eliminate any data points bellow threshold snr
     gis = []
     for i in np.arange(len(phases)):
         if (1/errs[i]) >= snr:
             gis.append(i)
     gis = np.asarray(gis, dtype=int)
 
+
     phases = phases[gis]
     fluxes = fluxes[gis]
     wv_effs = wv_effs[gis]
     errs = errs[gis]
     width_effs = np.asarray(width_effs)
     width_effs = width_effs[gis]
     my_filters = np.asarray(my_filters)
     my_filters = my_filters[gis]
 
     # Set the peak flux to t=0
     peak_i = np.argmax(fluxes)
+    if verbose:
+        print('Peak Luminosity occurrs at MJD',phases[peak_i])
     phases = np.asarray(phases) - phases[peak_i]
 
     # Eliminate any data points outside of specified range
     # With respect to first data point
     gis = []
     for i in np.arange(len(phases)):
         if phases[i] <= end and phases[i] >= start:
@@ -215,14 +197,39 @@
     my_filters = my_filters[gis]
 
     lc = np.vstack((phases, fluxes, wv_effs / 1000., errs, width_effs))
 
     return lc, wv_corr, flux_corr, my_filters
 
 
+def chi_square(dat, model, uncertainty):
+    '''
+    Calculate the chi squared of a model given a set of data
+
+    Parameters
+    ----------
+    dat : numpy.array
+        Experimental data for the model to be tested against
+    model : numpy.array
+        Model data being tested
+    uncertainty : numpy.array
+        Error on experimental data
+
+    Output
+    ------
+    chi2 : float
+        the chi sqaured value of the model
+    '''
+
+    chi2 = 0.
+    for i in np.arange(len(dat)):
+        chi2 += ((model[i]-dat[i]) / uncertainty[i])**2.
+
+    return chi2
+
 def generate_template(filter_wv, sn_type):
     '''
     Prepare and interpolate SN1a Template
 
     Parameters
     ----------
     fiter_wv : numpy.array
@@ -487,20 +494,19 @@
     fluxes = lc[:, 1]
     wv_effs = lc[:, 2]
     errs = lc[:, 3]
     stacked_data = np.vstack([times, wv_effs]).T
     ufilts = np.unique(lc[:, 2])
     ufilts_in_angstrom = ufilts*1000.0 + wv_corr
     nfilts = len(ufilts)
-    x_pred = np.zeros((int((np.ceil(np.max(times)) -
-                            np.floor(np.min(times)))+1)*nfilts, 2))
-    dense_fluxes = np.zeros((int((np.ceil(np.max(times)) -
-                                  np.floor(np.min(times)))+1), nfilts))
-    dense_errs = np.zeros((int((np.ceil(np.max(times)) -
-                                np.floor(np.min(times)))+1), nfilts))
+    length_of_times = len(np.arange(int(np.floor(np.min(lc[:, 0]))),
+                           (int(np.ceil(np.max(lc[:, 0])))+1),0.1))
+    x_pred = np.zeros((length_of_times*nfilts, 2))
+    dense_fluxes = np.zeros((length_of_times, nfilts))
+    dense_errs = np.zeros((length_of_times, nfilts))
 
     # test_y is only used if mean = True
     # but I still need it to exist either way
     test_y = []
     test_times = []
     if use_mean:
         template = generate_template(ufilts_in_angstrom, sn_type)
@@ -519,25 +525,24 @@
                 wv = param[:, 1]
                 return np.asarray([template(*p)[0] for p in zip(t, wv)]) \
                     + f_stretch
 
         # Get Test data so that the template can be plotted
         mean = snModel()
         for i in ufilts_in_angstrom:
-            test_wv = np.full((1, int((np.ceil(np.max(times)) -
-                                       np.floor(np.min(times))))), i)
-            test_times = np.arange(int(np.floor(np.min(times))+1),
-                                   int(np.ceil(np.max(times))+1))
+            test_wv = np.full((1, length_of_times), i)
+            test_times = np.arange(int(np.floor(np.min(times))),
+                                   int(np.ceil(np.max(times))+1), 0.1)
             test_x = np.vstack((test_times, test_wv)).T
             test_y.append(mean.get_value(test_x))
         test_y = np.asarray(test_y)
 
     # Set up gp
     kernel = np.var(lc[:, 1]) \
-        * george.kernels.ExpSquaredKernel([50, 0.5], ndim=2)
+        * george.kernels.Matern32Kernel([12, 0.1], ndim=2)
     if not use_mean:
         gp = george.GP(kernel, mean=0)
     else:
         gp = george.GP(kernel, mean=snModel())
     gp.compute(stacked_data, lc[:, -2])
 
     def neg_ln_like(p):
@@ -545,22 +550,24 @@
         return -gp.log_likelihood(lc[:, 1])
 
     def grad_neg_ln_like(p):
         gp.set_parameter_vector(p)
         return -gp.grad_log_likelihood(lc[:, 1])
 
     # Optomize gp parameters
+    bnds = ((None, None), (None, None), (None, None))
     result = minimize(neg_ln_like,
                       gp.get_parameter_vector(),
-                      jac=grad_neg_ln_like)
+                      jac=grad_neg_ln_like,
+                      bounds = bnds)
     gp.set_parameter_vector(result.x)
 
     # Populate arrays with time and wavelength values to be fed into gp
     for jj, time in enumerate(np.arange(int(np.floor(np.min(times))),
-                                        int(np.ceil(np.max(times)))+1)):
+                                        int(np.ceil(np.max(times)))+1, 0.1)):
         x_pred[jj*nfilts: jj*nfilts+nfilts, 0] = [time] * nfilts
         x_pred[jj*nfilts: jj*nfilts+nfilts, 1] = ufilts
 
     # Run gp to estimate interpolation
     pred, pred_var = gp.predict(lc[:, 1], x_pred, return_var=True)
 
     # Populate dense_lc with newly gp-predicted values
@@ -597,14 +604,16 @@
         BB temperature error array (cm)
     '''
 
     T_arr = np.zeros(len(dense_lc))
     R_arr = np.zeros(len(dense_lc))
     Terr_arr = np.zeros(len(dense_lc))
     Rerr_arr = np.zeros(len(dense_lc))
+    covar_arr = np.zeros(len(dense_lc))
+
     prior_fit = (9000, 1e15)
 
     for i, datapoint in enumerate(dense_lc):
         fnu = 10.**((-datapoint[:, 0]+48.6) / -2.5)
         ferr = datapoint[:, 1]
         fnu = fnu * 4. * np.pi * (3.086e19)**2
         fnu_err = np.abs(0.921034 * 10.**(0.4*datapoint[:, 0] - 19.44)) \
@@ -635,46 +644,48 @@
             ndim = 2
             sampler = emcee.EnsembleSampler(nwalkers, ndim, log_probability,
                                             args=[wvs, flam, flam_err])
             T0 = 9000 + 1000*np.random.rand(nwalkers)
             R0 = 1e15 + 1e14*np.random.rand(nwalkers)
             p0 = np.vstack([T0, R0])
             p0 = p0.T
-
             burn_in_state = sampler.run_mcmc(p0, 100)
             sampler.reset()
             sampler.run_mcmc(burn_in_state, 4000)
             flat_samples = sampler.get_chain(discard=100, thin=1, flat=True)
-
+            covar_arr[i] = np.cov(flat_samples.T)[0,1]
             T_arr[i] = np.median(flat_samples[:, 0])
             R_arr[i] = np.median(flat_samples[:, 1])
             Terr_arr[i] = (np.percentile(flat_samples[:, 0], 84) -
                            np.percentile(flat_samples[:, 0], 16)) / 2.
             Rerr_arr[i] = (np.percentile(flat_samples[:, 1], 84) -
                            np.percentile(flat_samples[:, 1], 16)) / 2.
 
         else:
 
             try:
                 BBparams, covar = curve_fit(bbody, wvs, flam, maxfev=10000,
                                             p0=prior_fit, sigma=flam_err,
                                             bounds=(0, [T_max, np.inf]))
+
                 # Get temperature and radius, with errors, from fit
                 T_arr[i] = BBparams[0]
                 Terr_arr[i] = np.sqrt(np.diag(covar))[0]
                 R_arr[i] = np.abs(BBparams[1])
                 Rerr_arr[i] = np.sqrt(np.diag(covar))[1]
+                covar_arr[i] = covar[0,1]
                 prior_fit = BBparams
             except RuntimeWarning:
                 T_arr[i] = np.nan
                 R_arr[i] = np.nan
                 Terr_arr[i] = np.nan
                 Rerr_arr[i] = np.nan
+                covar_arr[i] = np.nan
 
-    return T_arr, R_arr, Terr_arr, Rerr_arr
+    return T_arr, R_arr, Terr_arr, Rerr_arr, covar_arr
 
 
 def plot_gp(lc, dense_lc, snname, flux_corr, my_filters, wvs, test_data,
             outdir, sn_type, test_times, mean, show_template):
     '''
     Plot the GP-interpolate LC and save
 
@@ -703,15 +714,15 @@
     show_template : bool
         Whether or not the sn template is plotted
 
     Output
     ------
     '''
     plot_times = np.arange(int(np.floor(np.min(lc[:, 0]))),
-                           (int(np.ceil(np.max(lc[:, 0])))+1))
+                           (int(np.ceil(np.max(lc[:, 0])))+1),0.1)
 
     # Import a color map to make the plots look pretty
     cm = plt.get_cmap('rainbow')
     wv_colors = (wvs-np.min(wvs)) / (np.max(wvs)-np.min(wvs))
 
     # Plot interpolation, template, and error (shaded areas)
     for jj in np.arange(len(wv_colors)):
@@ -776,15 +787,15 @@
     sn_type : string
         The type of sn template used for the gp
 
     Output
     ------
     '''
     interp_times = np.arange(int(np.floor(np.min(lc[:, 0]))),
-                             int(np.ceil(np.max(lc[:, 0])))+1)
+                             int(np.ceil(np.max(lc[:, 0])))+1, 0.1)
     fig, axarr = plt.subplots(2, 1, sharex=True)
 
     axarr[0].plot(interp_times, Tarr / 1.e3, color='k')
     axarr[0].fill_between(interp_times, Tarr/1.e3 - Terr_arr/1.e3,
                           Tarr/1.e3 + Terr_arr/1.e3, color='k', alpha=0.2)
     axarr[0].set_ylabel('Temp. (1000 K)')
 
@@ -821,15 +832,15 @@
     sn_type : string
         The type of sn template used in the gp
 
     Output
     ------
     '''
     plot_times = np.arange(int(np.floor(np.min(lc[:, 0]))),
-                           int(np.ceil(np.max(lc[:, 0])))+1)
+                           int(np.ceil(np.max(lc[:, 0])))+1, 0.1)
 
     plt.plot(plot_times, bol_lum, color='k')
     plt.fill_between(plot_times, bol_lum-bol_err, bol_lum+bol_err,
                      color='k', alpha=0.2)
 
     plt.title(snname + ' Bolometric Luminosity')
     plt.xlabel('Time (Days)')
@@ -875,15 +886,15 @@
         Type of sn template used for the gp
 
     Output
     ------
     '''
 
     times = np.arange(int(np.floor(np.min(lc[:, 0]))),
-                      int(np.ceil(np.max(lc[:, 0])))+1)
+                      int(np.ceil(np.max(lc[:, 0])))+1, 0.1)
     dense_lc = np.reshape(dense_lc, (len(dense_lc), -1))
     dense_lc = np.hstack((np.reshape(-times, (len(times), 1)), dense_lc))
     tabledata = np.stack((Tarr / 1e3, Terr_arr / 1e3, Rarr / 1e15,
                           Rerr_arr / 1e15, np.log10(bol_lum),
                           np.log10(bol_err))).T
     tabledata = np.hstack((-dense_lc, tabledata)).T
 
@@ -908,14 +919,15 @@
 
 
 def main():
 
     default_data = pkg_resources.resource_filename(
                    'extrabol.example', 'SN2010bc.dat'
                    )
+
     # Define all arguments
     parser = argparse.ArgumentParser(description='extrabol helpers')
     parser.add_argument('snfile', nargs='?',
                         default=default_data,
                         type=str, help='Give name of SN file')
     parser.add_argument('-m', '--mean', dest='mean', type=str, default='0',
                         help="Template function for gp.\
@@ -1036,33 +1048,36 @@
     if args.verbose:
         print('Using ' + str(sn_type) + ' template.')
 
     dense_lc, test_data, test_times = interpolate(lc, wv_corr, sn_type,
                                                   mean, args.redshift,
                                                   args.verbose)
     lc = lc.T
-
     wvs, wvind = np.unique(lc[:, 2], return_index=True)
     wvs = wvs*1000.0 + wv_corr
     my_filters = np.asarray(my_filters)
     ufilts = my_filters[wvind]
 
     # Converts to AB magnitudes
     dense_lc[:, :, 0] += flux_corr
 
     if args.verbose:
         print('Fitting Blackbodies, this may take a few minutes...')
-    Tarr, Rarr, Terr_arr, Rerr_arr = fit_bb(dense_lc, wvs, args.mc, args.T_max)
+    Tarr, Rarr, Terr_arr, Rerr_arr, covar_arr = fit_bb(dense_lc, wvs, args.mc,
+                                                       args.T_max)
 
     # Calculate bolometric luminosity and error
     bol_lum = 4. * np.pi * Rarr**2 * sigsb * Tarr**4
+    covar_err = 2. * (4. * np.pi * sigsb)**2 * (2 * Rarr * Tarr**4) * \
+                (4 * Rarr**2 * Tarr**3) * covar_arr
     bol_err = 4. * np.pi * sigsb * np.sqrt(
                 (2. * Rarr * Tarr**4 * Rerr_arr)**2
                 + (4. * Tarr**3 * Rarr**2 * Terr_arr)**2
                 )
+    bol_err = np.sqrt(bol_err**2 + covar_err)
 
     if args.plot:
         if args.verbose:
             print('Making plots in ' + args.outdir)
         plot_gp(lc, dense_lc, snname, flux_corr, ufilts, wvs, test_data,
                 args.outdir, sn_type, test_times, mean, args.template)
         plot_bb_ev(lc, Tarr, Rarr, Terr_arr, Rerr_arr, snname,
```

### Comparing `extrabol-1.0.0/extrabol.egg-info/PKG-INFO` & `extrabol-1.0.1/extrabol.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,122 @@
 Metadata-Version: 2.1
 Name: extrabol
-Version: 1.0.0
+Version: 1.0.1
 Summary: Estimate SN bolometric light curves
-Home-page: https://github.com/villrv/extrabol
-Author: Ian M. Thornton
-Author-email: iot5037@psu.edu
-License: UNKNOWN
-Description: Generate bolometric estimates of Supernovae
-        
-        Author: Ian Thornton
-        
-        Install with pip:
-        
-        ```bash
-        pip install extrabol
-        ```
-        # Usage
-        
-        ```
-        extrabol 'filename.dat' ARGUMENTS
-        ```
-        Optional Arguments:
-        ```
-        --verbose
-            Increase output verbosity
-        
-        -m MEAN, --mean MEAN
-            Use a supernova template as the mean function for the GP; Choose \'1a\',\'1bc\', \'2l\', \'2p\', or \'0\' (for no template)
-            Default = 0
-        
-        -t, --show-template
-            Shows supernova template on plots as dotted lines
-        
-        -d DIST, --dist DIST
-            Object luminosity distance in Mpc
-        
-        -z REDSHIFT, --redshift REDSHIFT
-            Object redshift
-            If no argument is provided, redshift will be read from the input file
-        
-        --dm DM
-            Object distance modulus
-        
-        --plot BOOL
-            Output plots, Default is TRUE
-        
-        --outdir OUTDIR
-            A file location for outputs to be written to
-        
-        --ebv EBV
-            Milky Way extinction E(B-V) value, if known
-            If no argument is probided the extinction will be read from the input file
-        
-        --hostebv HOSTEBV
-            Host extinction E(B-V)
-        
-        -s START, --start START
-            Start time of analysis window relative to peak luminosity
-            Default = -50 days
-        
-        -e END, --end END
-            End time of analysis window relative to peak luminosity
-            Default = 150 days
-        
-        -snr SNR
-            Minimum signal to noise ratio for observations
-            Default = 4.0
-        
-        -wc, --wvcorr
-            Use the redshift-corrected wavelength values for extinction calculations
-        
-        -mc, --use-mcmc
-            Use a Markov Chain Monte Carlo to fit black bodies instead of curve_fit.
-            This provides better error estimates but takes much longer.
-        
-        --T_max T_MAX
-            Modify the prior on temperature for blackbody fits by specifying a maximum temperature.
-            Default = 40,000K
-        ```
-        # Input Files
-        
-        Inputs to extrabol must be .dat files that conform to the following format.
-        
-        The first two lines must contain redshift and Milky Way extinction E(b-v) respectively. If these values are unknown, simply put 0.0.
-        The following lines contain observational data in 5 columns as shown below:
-        
-        ```
-        Time(MJD)   Apparent Magnitude   Error(in magnitudes)   Filter SVO ID   Type of magnitude (AB or Vega)
-        ```
-        Any white space can be used as the column delimiter. NaNs, non-detections, and data points with no error bars should not be included.
-        An example input file can be found under extrabol/example.
-        
-        # Example Input
-        
-        ```python
-        extrabol ./example/PSc000174_extrabol.dat --verbose -m 1a
-        ```
-        
-        This example may take a minute the first time you run it as astroquery fetches filter information!
-        
-        Filters must be specified by their [SVO](http://svo2.cab.inta-csic.es/svo/theory/fps3/) ID.
-        
-        
-Platform: UNKNOWN
+Author-email: "Ian M. Thornton" <iot5037@psu.edu>
+Project-URL: Repository, https://github.com/villrv/extrabol
+Project-URL: Documentation, https://extrabol.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![DOI](https://zenodo.org/badge/283353973.svg)](https://zenodo.org/badge/latestdoi/283353973)
+
+
+# extrabol
+
+`extrabol` is a Python 3.x package for rapidly and systematicaly estimating the bolometric luminosity and black body properties of (thermal) extragalactic transients from broadband UVONIR data. `extrabol` is broken down into three main steps:
+
+- Read in and pre-process a data file holding observations of a supernova or other transient event over time, through any number of broadband filters.
+- Interpolate this data using a Gaussian Process(GP), a non-physical, statistical model utilizing covariance.
+- Fit a series of blackbody curves to the interpolated data to estimate the bolometric luminosity, temperature, and radius of the transient over time.
+
+Author: Ian Thornton
+
+## Installation and Documentation
+
+Install with pip:
+
+```bash
+pip install extrabol
+```
+
+The latest documentation is available [here](https://extrabol.readthedocs.io/en/latest/).
+
+## Usage
+
+```
+extrabol 'filename.dat' ARGUMENTS
+```
+Optional Arguments:
+```
+--verbose
+    Increase output verbosity
+
+-m MEAN, --mean MEAN
+    Use a supernova template as the mean function for the GP; Choose \'1a\',\'1bc\', \'2l\', \'2p\', or \'0\' (for no template)
+    Default = 0
+
+-t, --show-template
+    Shows supernova template on plots as dotted lines
+
+-d DIST, --dist DIST
+    Object luminosity distance in Mpc
+
+-z REDSHIFT, --redshift REDSHIFT
+    Object redshift
+    If no argument is provided, redshift will be read from the input file
+
+--dm DM
+    Object distance modulus
+
+--plot BOOL
+    Output plots, Default is TRUE
+
+--outdir OUTDIR
+    A file location for outputs to be written to
+
+--ebv EBV
+    Milky Way extinction E(B-V) value, if known
+    If no argument is probided the extinction will be read from the input file
+
+--hostebv HOSTEBV
+    Host extinction E(B-V)
+
+-s START, --start START
+    Start time of analysis window relative to peak luminosity
+    Default = -50 days
+
+-e END, --end END
+    End time of analysis window relative to peak luminosity
+    Default = 150 days
+
+-snr SNR
+    Minimum signal to noise ratio for observations
+    Default = 4.0
+
+-wc, --wvcorr
+    Use the redshift-corrected wavelength values for extinction calculations
+
+-mc, --use-mcmc
+    Use a Markov Chain Monte Carlo to fit black bodies instead of curve_fit.
+    This provides better error estimates but takes much longer.
+
+--T_max T_MAX
+    Modify the prior on temperature for blackbody fits by specifying a maximum temperature.
+    Default = 40,000K
+```
+## Input Files
+
+Inputs to extrabol must be .dat files that conform to the following format.
+
+The first two lines must contain redshift and Milky Way extinction E(b-v) respectively. If these values are unknown, simply put 0.0.
+The following lines contain observational data in 5 columns as shown below:
+
+```
+Time(MJD)   Apparent Magnitude   Error(in magnitudes)   Filter SVO ID   Type of magnitude (AB or Vega)
+```
+Any white space can be used as the column delimiter. NaNs, non-detections, and data points with no error bars should not be included.
+An example input file can be found under extrabol/example.
+
+## Example Input
+
+```python
+extrabol ./example/PSc000174_extrabol.dat --verbose -m 1a
+```
+
+This example may take a minute the first time you run it as astroquery fetches filter information!
+
+Filters must be specified by their [SVO](http://svo2.cab.inta-csic.es/svo/theory/fps3/) ID.
```

