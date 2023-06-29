# Comparing `tmp/RecruitmentCurveFitting-1.1.0-py2.py3-none-any.whl.zip` & `tmp/RecruitmentCurveFitting-1.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 106261 bytes, number of entries: 12
+Zip file size: 106314 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    35821 b- defN 23-May-27 05:45 RecruitmentCurveFitting/COPYING
 -rw-r--r--  2.0 unx    18750 b- defN 23-May-30 15:02 RecruitmentCurveFitting/CurveFitting.py
--rw-r--r--  2.0 unx    28108 b- defN 23-May-27 05:02 RecruitmentCurveFitting/RecruitmentCurves.py
--rw-r--r--  2.0 unx     4153 b- defN 23-May-30 15:02 RecruitmentCurveFitting/__init__.py
--rw-r--r--  2.0 unx     7760 b- defN 23-May-30 15:02 RecruitmentCurveFitting/__main__.py
+-rw-r--r--  2.0 unx    28502 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting/RecruitmentCurves.py
+-rw-r--r--  2.0 unx     4110 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting/__init__.py
+-rw-r--r--  2.0 unx     7820 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting/__main__.py
 -rw-r--r--  2.0 unx     1491 b- defN 23-May-27 02:43 RecruitmentCurveFitting/example-data1.txt
 -rw-r--r--  2.0 unx     2291 b- defN 23-May-27 02:24 RecruitmentCurveFitting/example-data2.txt
 -rw-r--r--  2.0 unx   208425 b- defN 23-May-27 02:24 RecruitmentCurveFitting/example-waveforms.csv
--rw-r--r--  2.0 unx     2602 b- defN 23-May-30 15:02 RecruitmentCurveFitting-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-30 15:02 RecruitmentCurveFitting-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-May-30 15:02 RecruitmentCurveFitting-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1135 b- defN 23-May-30 15:02 RecruitmentCurveFitting-1.1.0.dist-info/RECORD
-12 files, 310670 bytes uncompressed, 104321 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx     2559 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1135 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting-1.1.1.dist-info/RECORD
+12 files, 311038 bytes uncompressed, 104374 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: RecruitmentCurveFitting/example-data2.txt
 Comment: 
 
 Filename: RecruitmentCurveFitting/example-waveforms.csv
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.0.dist-info/METADATA
+Filename: RecruitmentCurveFitting-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.0.dist-info/WHEEL
+Filename: RecruitmentCurveFitting-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.0.dist-info/top_level.txt
+Filename: RecruitmentCurveFitting-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.0.dist-info/RECORD
+Filename: RecruitmentCurveFitting-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RecruitmentCurveFitting/RecruitmentCurves.py

```diff
@@ -57,15 +57,15 @@
 milliseconds::
     
     from RecruitmentCurveFitting import RecruitmentCurve, UnpackExamples
 
     UnpackExamples() # writes assorted example files to the current directory
 
     z = RecruitmentCurve('example-waveforms.csv') # that's one of the files
-    z.Fit( boundsM=[8.1, 15.3], boundsH=[34.6, 42.1] )
+    z.Fit( boundsM=[8.1, 15.9], boundsH=[34.6, 42.4] )
     z.Plot() # try hovering the mouse pointer over each data-point, it's fun
 	
 This module can also be run as a standalone command-line utility. Input files
 should be formatted as comma- or space-delimited numeric tables where the last
 three columns are stimulation intensity, M-wave size and H-reflex size. Prior
 columns, if present, are used to separate different conditions from each other
 (each condition generates one pair of curve fits, and one figure if requested)
@@ -378,15 +378,15 @@
 class RecruitmentCurve( object ):
 	"""
 	An object that takes EMG time-series (one per trial) and provides
 	a `.Fit()` method that extracts M-wave and H-reflex magnitudes (given
 	the bounds of these waveform components in milliseconds) and fits the
 	two respective recruitment curves.
 	"""
-	def __init__( self, waveforms, timeBase=None, stimulationIntensities=None, excuses=None, **descriptors ):
+	def __init__( self, waveforms, timeBase=None, stimulationIntensities=None, excuses=None, samplesPerSecond=None, **descriptors ):
 		"""				
 		Args:
 		    waveforms (2D `numpy.array`, or sequence of sequences of values):
 		        a two-dimensional array of voltage values: one row per
 		        time sample, one column per trial. It is assumed that you
 		        have preprocessed the waveforms appropriately, including
 		        removal of the stimulation artifact (this module does not
@@ -400,17 +400,21 @@
 		        first row (all but the first element) will be taken as
 		        `stimulationIntensities`. This format is saved by
 		        `.SaveArray()`.
 		    
 		    timeBase (float, or a 1D `numpy.array` or sequence of values):
 		        if expressed as a scalar, this should simply be the
 		        sampling frequency in Hz. If expressed as a sequence of
-		        time values, the number of values should be equal to the
-		        number of rows in `waveforms`.
+		        time values in milliseconds, the number of values should
+		        be equal to the number of rows in `waveforms`.
 		    
+		    samplesPerSecond (float):
+		        a more-intuitively-named alias for `timeBase` when all you
+		        have is a scalar sampling-frequency value.
+		        
 		    stimulationIntensities (1D `numpy.array` or sequence of values):
 		        one stimulation-intensity value per column of `waveforms`.
 		    
 		    excuses (list, tuple):
 		        an optional sequence of strings detailing reasons why
 		        this dataset is disqualified from ordinary analysis. If
 		        non-empty, curve-fitting will be skipped for this dataset.
@@ -441,16 +445,17 @@
 			self.descriptors = copy.deepcopy( other.descriptors )
 			for attrName, fit in other.clients.values():
 				fit = fit() # de-reference weakref.ref
 				if fit is not None: self.Associate( **{ attrName : fit.__class__( fit ) } )
 		else:
 			self.waveforms = numpy.asarray( waveforms, dtype=float )
 			nSamples, nWaveforms = self.waveforms.shape
-			if timeBase is None: raise ValueError( 'must supply timeBase' )
 			if stimulationIntensities is None: raise ValueError( 'must supply stimulationIntensities' )
+			if timeBase is None: timeBase = samplesPerSecond
+			if timeBase is None: raise ValueError( 'must supply timeBase' )
 			if isinstance( timeBase, ( int, float ) ):
 				samplesPerSecond = float( timeBase )
 				timeBase = 1000.0 * numpy.arange( nSamples )[ :, None ] / samplesPerSecond
 			self.timeBase = numpy.asarray( timeBase, dtype=float ).ravel()
 			self.stimulationIntensities = numpy.asarray( stimulationIntensities, dtype=float ).ravel()
 			self.excuses = list( excuses ) if excuses else []
 			self.descriptors = dict( descriptors )
@@ -623,26 +628,29 @@
 		"""
 		Experimental method for inferring M-wave bounds given H-wave
 		bounds and the assumption of isomorphism (NB: requires prior
 		removal of stimulation artifact).
 		"""
 		if boundsH is None: boundsH = self.boundsH
 		boundsH = numpy.asarray( boundsH, dtype=float ).ravel()
+		hStartInSamples = numpy.nonzero( self.timeBase >= min( boundsH ) )[ 0 ][ 0 ]
+		finesse = min( boundsH ) - self.timeBase[ hStartInSamples ]
+		
 		hWaveforms = self.Excerpt( boundsH )
 		# TODO: at this point we could do some ICA or something to isolate the H from contaminants
 		#       For now, let's just sort the trials in descending order of magnitude and average the first few
 		hReordering = numpy.argsort( -numpy.abs( hWaveforms ).mean( axis=0 ) )
 		firstOrderedHWaveformToAverage = 2
 		numberOfHWaveformsToAverage = 8
 		canonicalH = hWaveforms[ :, hReordering[ firstOrderedHWaveformToAverage : firstOrderedHWaveformToAverage + numberOfHWaveformsToAverage ] ].mean( axis=1 )
 		numberOfMWaveformsToAverage = 8
 		mReordering = numpy.argsort( self.stimulationIntensities )
 		fullWaveformAtMMax = self.waveforms[ :, mReordering[ -numberOfMWaveformsToAverage: ] ].mean( axis=1 )
 		mStartInSamples = numpy.argmax( numpy.correlate( fullWaveformAtMMax, canonicalH ) )
-		boundsM = self.timeBase[ [ mStartInSamples, mStartInSamples + canonicalH.size - 1 ] ]
+		boundsM = self.timeBase[ [ mStartInSamples ] ] + [ 0, boundsH.ptp() ] + finesse
 		if plot:
 			mmask = self.Excerpt( boundsM, 'mask' )
 			#magnitude = lambda x: numpy.abs( x ).mean()
 			magnitude = numpy.ptp
 			factor = magnitude( fullWaveformAtMMax[ mmask ] ) / magnitude( canonicalH )
 			import matplotlib.pyplot as plt
 			axes = plt.gcf() if isinstance( plot, bool ) else plt.figure( plot ) if isinstance( plot, int ) else plot
```

## RecruitmentCurveFitting/__init__.py

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 
 # $BEGIN_RECRUITMENTCURVEFITTING_LICENSE$
 # 
 # This file is part of the RecruitmentCurveFitting project, a Python
 # package for fitting sigmoid and bell-shaped functions to EMG
 # recruitment-curve measurements.
 # 
@@ -33,28 +33,28 @@
 from .RecruitmentCurves import *
 
 CITATION_INFO = """
 If you use this software in your research, your report should cite the article
 in which this approach was introduced, as follows:
 
 - McKinnon ML, Hill NJ, Carp JS, Dellenbach B & Thompson AK (2023).
-  Automated identification of EMG responses evoked by peripheral nerve
-  stimulation: quantitative effects on critical parameters of diagnostic and
-  closed-loop therapeutic applications.
+  Methods for automated delineation and assessment of EMG responses evoked by
+  peripheral nerve stimulation in diagnostic and closed-loop therapeutic
+  applications.
   @JOURNAL@ @NUMBER@(@VOLUME@):@PAGES@
   @DOI@
     
 The corresponding BibTeX entry is::
 
     @article{mckinnonhill2023,
       author  = {McKinnon, Michael L. and Hill, N. Jeremy and Carp, Jonathan S.
                  and Dellenbach, Blair and Thompson, Aiko K.},
-      title   = {Automated Identification of {EMG} Responses Evoked by Peripheral
-                 Nerve Stimulation: Quantitative Effects on Critical Parameters 
-                 of Diagnostic and Closed-Loop Therapeutic Applications},
+      title   = {Methods for Automated Delineation and Assessment of {EMG}
+                 Responses Evoked by Peripheral Nerve Stimulation in Diagnostic
+                 and Closed-Loop Therapeutic Applications},
       journal = {TBD},
       volume  = {TBD},
       number  = {TBD},
       pages   = {TBD--TBD},
       month   = {TBD},
       year    = {2023},
       date    = {2023-TBD-TBD},
```

## RecruitmentCurveFitting/__main__.py

```diff
@@ -38,48 +38,46 @@
 import argparse
 
 def OneOrTwoNumbers( s ):
 	seq = ast.literal_eval( s.strip( ' [](),' ) + ',' )
 	try: x, = seq
 	except: x = a, b = seq
 	return x
-		
 
 class HelpFormatter( argparse.RawDescriptionHelpFormatter ): pass
 #class HelpFormatter( argparse.RawDescriptionHelpFormatter, argparse.ArgumentDefaultsHelpFormatter ): pass
 parser = argparse.ArgumentParser( description=__doc__, formatter_class=HelpFormatter, prog='python -m RecruitmentCurveFitting', )
-parser.add_argument(         "filenames",    metavar='FILENAME',    nargs='*', help='one or more text files to load (use a dash to denote stdin)' )
-parser.add_argument( "-s", "--saveas",       metavar='PDFFILENAME', default='', help='name of pdf file in which to save figures (one per page)' )
-parser.add_argument( "-p", "--plot",         action='store_true',   help='whether to show figures on-screen' )
-parser.add_argument( "-g", "--grid",         action='store_true',   help='whether to use a grid for the plot' )
-parser.add_argument( "-x", "--xlabel",       metavar='XLABEL',      default='Stimulation Intensity (mA)', help='x-axis label text for the plot' )
-parser.add_argument( "-y", "--ylabel",       metavar='YLABEL',      default='Response ($\\mu$V)', help='y-axis label text for the plot' )
-parser.add_argument(       "--title",        metavar='TITLE',       default=None, help='override automatically-generated plot titles' )
-parser.add_argument(       "--xlim",         metavar='XMIN,XMAX',   default=None, type=OneOrTwoNumbers, help='x-axis limits for the plot' )
-parser.add_argument(       "--ylim",         metavar='YMIN,YMAX',   default=None, type=OneOrTwoNumbers, help='y-axis limits for the plot' )
-parser.add_argument(       "--mark-mmax",    action='store_true',   help='whether to mark M_max' )
-parser.add_argument(       "--mark-hmax",    action='store_true',   help='whether to mark H_max' )
-parser.add_argument( "-t", "--threshold",    metavar='MTHRESHOLD',  default=0, type=float, help='unscaled proportion of Mmax (between 0 and 1) to mark as "threshold" for the M-wave curve (set to 0 to leave it unmarked)' )
-parser.add_argument(       "--unpack-examples", action='store_true', help='write example files to the current directory (do not overwrite) and quit' )
-parser.add_argument(       "--help-module",  action='store_true', help='display the main package docstring' )
+parser.add_argument(       "filenames",         metavar='FILENAME',    nargs='*', help='one or more text files to load (use a dash to denote stdin)' )
+parser.add_argument(       "--help-module",     action='store_true',   help='display the docstring for the main package (Python API)' )
+parser.add_argument(       "--unpack-examples", action='store_true',   help='write example files to the current directory (do not overwrite) and quit' )
+parser.add_argument( "-p", "--plot",            action='store_true',   help='whether to show figures on-screen' )
+parser.add_argument( "-g", "--grid",            action='store_true',   help='whether to use a grid for the plots' )
+parser.add_argument( "-x", "--xlabel",          metavar='XLABEL',      default='Stimulation Intensity (mA)', help='x-axis label text for the plots' )
+parser.add_argument( "-y", "--ylabel",          metavar='YLABEL',      default='Response ($\\mu$V)', help='y-axis label text for the plots' )
+parser.add_argument( "-t", "--title",           metavar='TITLE',       default=None, help='override automatically-generated plot titles' )
+parser.add_argument(       "--xlim",            metavar='XMIN,XMAX',   default=None, type=OneOrTwoNumbers, help='x-axis limits for the plots' )
+parser.add_argument(       "--ylim",            metavar='YMIN,YMAX',   default=None, type=OneOrTwoNumbers, help='y-axis limits for the plots' )
+parser.add_argument(       "--mark-mmax",       action='store_true',   help='whether to mark M_max on plots' )
+parser.add_argument(       "--mark-hmax",       action='store_true',   help='whether to mark H_max on plots' )
+parser.add_argument(       "--threshold",       metavar='MTHRESHOLD',  default=0, type=float, help='unscaled proportion of Mmax (between 0 and 1) to mark as "threshold" for the M-wave curve (set to 0 to leave it unmarked)' )
+parser.add_argument( "-s", "--saveas",          metavar='PDFFILENAME', default='', help='name of pdf file in which to save figures (one per page)' )
 opts = parser.parse_args()
 
-
 import numpy
 
 import RecruitmentCurveFitting
 from RecruitmentCurveFitting import *
 
 if opts.unpack_examples:
 	UnpackExamples()
 	if not opts.filenames: raise SystemExit( 'done' )		
 
 if opts.help_module:
 	print( RecruitmentCurveFitting.__doc__ )
-	if not opts.filenames: raise SystemExit()
+	raise SystemExit()
 
 def tryeval(x):
 	try: return ast.literal_eval( x )
 	except: return x
 	
 filenames = opts.filenames if opts.filenames else [ '-' ]
 def myglob( pattern ):
```

## Comparing `RecruitmentCurveFitting-1.1.0.dist-info/METADATA` & `RecruitmentCurveFitting-1.1.1.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecruitmentCurveFitting
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package for fitting sigmoid and bell-shaped functions to EMG recruitment-curve measurements
 Home-page: UNKNOWN
 Author: Jeremy Hill
 Author-email: jezhill@gmail.com
 License: GPL v3+
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, <4
@@ -34,28 +34,28 @@
     
 
 
 If you use this software in your research, your report should cite the article
 in which this approach was introduced, as follows:
 
 - McKinnon ML, Hill NJ, Carp JS, Dellenbach B & Thompson AK (2023).
-  Automated identification of EMG responses evoked by peripheral nerve
-  stimulation: quantitative effects on critical parameters of diagnostic and
-  closed-loop therapeutic applications.
+  Methods for automated delineation and assessment of EMG responses evoked by
+  peripheral nerve stimulation in diagnostic and closed-loop therapeutic
+  applications.
   @JOURNAL@ @NUMBER@(@VOLUME@):@PAGES@
   @DOI@
     
 The corresponding BibTeX entry is::
 
     @article{mckinnonhill2023,
       author  = {McKinnon, Michael L. and Hill, N. Jeremy and Carp, Jonathan S.
                  and Dellenbach, Blair and Thompson, Aiko K.},
-      title   = {Automated Identification of {EMG} Responses Evoked by Peripheral
-                 Nerve Stimulation: Quantitative Effects on Critical Parameters 
-                 of Diagnostic and Closed-Loop Therapeutic Applications},
+      title   = {Methods for Automated Delineation and Assessment of {EMG}
+                 Responses Evoked by Peripheral Nerve Stimulation in Diagnostic
+                 and Closed-Loop Therapeutic Applications},
       journal = {TBD},
       volume  = {TBD},
       number  = {TBD},
       pages   = {TBD--TBD},
       month   = {TBD},
       year    = {2023},
       date    = {2023-TBD-TBD},
```

## Comparing `RecruitmentCurveFitting-1.1.0.dist-info/RECORD` & `RecruitmentCurveFitting-1.1.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 RecruitmentCurveFitting/COPYING,sha256=Czg9WmPaZE9ijZnDOXbqZIftiaqlnwsyV5kt6sEXHms,35821
 RecruitmentCurveFitting/CurveFitting.py,sha256=80RF2UuoP9KUl-pydCIwa_FHD9k8-J7OFvefHWRfL2A,18750
-RecruitmentCurveFitting/RecruitmentCurves.py,sha256=Glpy6G3ttJ1gBnIv0ITVPr4MtSTLslWauWRZbqOFK8g,28108
-RecruitmentCurveFitting/__init__.py,sha256=peOEQXA8V176MhvCWwFqLxkv4coU7H70YOjM5Lc3RCo,4153
-RecruitmentCurveFitting/__main__.py,sha256=Itk6SIM0iEb1UY_RsRH9yNHAxMjz-GGFuLe8yhjNivg,7760
+RecruitmentCurveFitting/RecruitmentCurves.py,sha256=UPeHS19jOlkMuvKRp8sMT_5zyEXE5KONCznWG-QWLmg,28502
+RecruitmentCurveFitting/__init__.py,sha256=Tb-5fhd6Rpicm1qs9l3eoe6jj0IH7UiG3HjeDDTpeGc,4110
+RecruitmentCurveFitting/__main__.py,sha256=515xY1F8yjh3qF-hpvkFFMnAbFcDeKSTJWkrL3XEhUE,7820
 RecruitmentCurveFitting/example-data1.txt,sha256=FeaYwnAMGemLQKM9Kj1IPi_3fey7gyY9SLOJYttZcXc,1491
 RecruitmentCurveFitting/example-data2.txt,sha256=SBv6zHDxt1YOhylfZSMMHSCsDNwL1brHpTgAdH8esvg,2291
 RecruitmentCurveFitting/example-waveforms.csv,sha256=eWF7HtChJAv5uHfiQ1Pg__l-d9eYKtGWr8PlYp7-kis,208425
-RecruitmentCurveFitting-1.1.0.dist-info/METADATA,sha256=msRPJiVYu-EJisdOWMJKTEw-OYeN2dr6VwcsObCbrmE,2602
-RecruitmentCurveFitting-1.1.0.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
-RecruitmentCurveFitting-1.1.0.dist-info/top_level.txt,sha256=GaYHShtnr9zJ_unau13fDnezLMr3kyCH0-KQN_Go6WM,24
-RecruitmentCurveFitting-1.1.0.dist-info/RECORD,,
+RecruitmentCurveFitting-1.1.1.dist-info/METADATA,sha256=beBgHI4rbQ0tD68qxbAkmujUdELSWrigafelDoPUBMs,2559
+RecruitmentCurveFitting-1.1.1.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
+RecruitmentCurveFitting-1.1.1.dist-info/top_level.txt,sha256=GaYHShtnr9zJ_unau13fDnezLMr3kyCH0-KQN_Go6WM,24
+RecruitmentCurveFitting-1.1.1.dist-info/RECORD,,
```

