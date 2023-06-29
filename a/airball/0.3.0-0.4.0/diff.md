# Comparing `tmp/airball-0.3.0.tar.gz` & `tmp/airball-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airball-0.3.0.tar", last modified: Thu Feb  9 06:22:19 2023, max compression
+gzip compressed data, was "airball-0.4.0.tar", last modified: Thu Jun 29 09:10:59 2023, max compression
```

## Comparing `airball-0.3.0.tar` & `airball-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-02-09 06:22:19.807668 airball-0.3.0/
--rw-r--r--   0 zyrxvo     (501) staff       (20)    35149 2022-05-02 19:30:08.000000 airball-0.3.0/LICENSE
--rw-r--r--   0 zyrxvo     (501) staff       (20)      988 2023-02-09 06:22:19.807532 airball-0.3.0/PKG-INFO
--rw-r--r--   0 zyrxvo     (501) staff       (20)      437 2022-10-13 00:46:55.000000 airball-0.3.0/README.md
--rw-r--r--   0 zyrxvo     (501) staff       (20)       85 2022-06-02 19:07:19.000000 airball-0.3.0/pyproject.toml
--rw-r--r--   0 zyrxvo     (501) staff       (20)       38 2023-02-09 06:22:19.807705 airball-0.3.0/setup.cfg
--rw-r--r--   0 zyrxvo     (501) staff       (20)      922 2023-02-09 02:42:29.000000 airball-0.3.0/setup.py
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-02-09 06:22:19.803832 airball-0.3.0/src/
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-02-09 06:22:19.806549 airball-0.3.0/src/airball/
--rw-r--r--   0 zyrxvo     (501) staff       (20)      243 2023-02-09 02:42:53.000000 airball-0.3.0/src/airball/__init__.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    13205 2023-02-09 01:44:59.000000 airball-0.3.0/src/airball/analytic.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)     9349 2023-02-09 06:00:24.000000 airball-0.3.0/src/airball/environments.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    11507 2023-02-09 06:18:07.000000 airball-0.3.0/src/airball/flybys.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    15000 2023-02-09 02:16:12.000000 airball-0.3.0/src/airball/particle.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)     7088 2023-02-09 03:40:54.000000 airball-0.3.0/src/airball/tools.py
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-02-09 06:22:19.807375 airball-0.3.0/src/airball.egg-info/
--rw-r--r--   0 zyrxvo     (501) staff       (20)      988 2023-02-09 06:22:19.000000 airball-0.3.0/src/airball.egg-info/PKG-INFO
--rw-r--r--   0 zyrxvo     (501) staff       (20)      358 2023-02-09 06:22:19.000000 airball-0.3.0/src/airball.egg-info/SOURCES.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)        1 2023-02-09 06:22:19.000000 airball-0.3.0/src/airball.egg-info/dependency_links.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)       35 2023-02-09 06:22:19.000000 airball-0.3.0/src/airball.egg-info/requires.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)        8 2023-02-09 06:22:19.000000 airball-0.3.0/src/airball.egg-info/top_level.txt
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-29 09:10:59.726911 airball-0.4.0/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    35149 2022-05-02 19:30:08.000000 airball-0.4.0/LICENSE
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     1023 2023-06-29 09:10:59.726792 airball-0.4.0/PKG-INFO
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      472 2023-02-16 19:20:04.000000 airball-0.4.0/README.md
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       85 2022-06-02 19:07:19.000000 airball-0.4.0/pyproject.toml
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       38 2023-06-29 09:10:59.726954 airball-0.4.0/setup.cfg
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      922 2023-06-29 09:03:54.000000 airball-0.4.0/setup.py
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-29 09:10:59.724420 airball-0.4.0/src/
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-29 09:10:59.725823 airball-0.4.0/src/airball/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      243 2023-06-23 02:16:23.000000 airball-0.4.0/src/airball/__init__.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     8979 2023-06-27 13:19:02.000000 airball-0.4.0/src/airball/analytic.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    43811 2023-06-29 09:01:58.000000 airball-0.4.0/src/airball/environments.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    11157 2023-06-29 08:34:54.000000 airball-0.4.0/src/airball/flybys.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    15000 2023-02-09 02:16:12.000000 airball-0.4.0/src/airball/particle.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     8475 2023-06-29 07:55:57.000000 airball-0.4.0/src/airball/tools.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      181 2023-06-29 01:38:57.000000 airball-0.4.0/src/airball/units.py
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-29 09:10:59.726608 airball-0.4.0/src/airball.egg-info/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     1023 2023-06-29 09:10:59.000000 airball-0.4.0/src/airball.egg-info/PKG-INFO
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      379 2023-06-29 09:10:59.000000 airball-0.4.0/src/airball.egg-info/SOURCES.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)        1 2023-06-29 09:10:59.000000 airball-0.4.0/src/airball.egg-info/dependency_links.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       35 2023-06-29 09:10:59.000000 airball-0.4.0/src/airball.egg-info/requires.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)        8 2023-06-29 09:10:59.000000 airball-0.4.0/src/airball.egg-info/top_level.txt
```

### Comparing `airball-0.3.0/LICENSE` & `airball-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airball-0.3.0/setup.py` & `airball-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="airball",
-    version="0.3.0",
+    version="0.4.0",
     author="Garett Brown",
     author_email="garett.brown@mail.utoronto.ca",
     description="A package for implementing flybys in hannorein/rebound",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zyrxvo/airball/",
     project_urls={
```

### Comparing `airball-0.3.0/src/airball/particle.py` & `airball-0.4.0/src/airball/particle.py`

 * *Files identical despite different names*

### Comparing `airball-0.3.0/src/airball/tools.py` & `airball-0.4.0/src/airball/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,94 @@
 from lib2to3.pytree import convert
 import numpy as _numpy
+import rebound as _rebound
 
 from scipy.special import erfinv as _erfinv
 from scipy.stats import uniform as _uniform
-# import astropy.constants as const
-# import astropy.units as u
+import astropy.constants as const
+from . import units
 
 ################################
 ###### Useful Constants ########
 ################################
 
 twopi = 2.*_numpy.pi
+# yr2pi = u.def_unit('yrtwopi', u.yr/twopi, format={'latex': r'(yr/2\pi)'})
 
-convert_kms_to_auyr2pi = 0.03357365989646266 # 1 km/s to AU/Yr2Pi
-convert_kms_to_auyr = 0.2109495265696987 # 1 km/s to AU/Yr
-convert_auyr2pi_to_kms = 1.0/convert_kms_to_auyr2pi
+# convert_kms_to_auyr2pi = 0.03357365989646266 # 1 km/s to AU/Yr2Pi
+# convert_kms_to_auyr = 0.2109495265696987 # 1 km/s to AU/Yr
+# convert_auyr2pi_to_kms = 1.0/convert_kms_to_auyr2pi
 
-convert_pc3_to_au3 = ((_numpy.pi**3)/272097792000000000) # 1 parsec^-3 to AU^-3
-convert_au3_to_pc3 = 1.0/convert_pc3_to_au3
+# convert_pc3_to_au3 = ((_numpy.pi**3)/272097792000000000) # 1 parsec^-3 to AU^-3
+# convert_au3_to_pc3 = 1.0/convert_pc3_to_au3
 
 ############################################################
 ### Stellar Mass generators using Initial Mass Functions ###
 ############################################################
 
-def imf_gen_1(size):
-    '''
-        Generate stellar mass samples for single star systems between 0.01 and 1.0 Solar Mass.
+# def imf_gen_1(size):
+#     '''
+#         Generate stellar mass samples for single star systems between 0.01 and 1.0 Solar Mass.
         
-        Computed using the inverted cumulative probability distribution (CDF) from the initial mass function (IMF) given in equation (17) by Chabrier (2003) https://ui.adsabs.harvard.edu/abs/2003PASP..115..763C/abstract
-
-        Parameters
-        ----------
-        size: the number of samples to draw.
-    '''
-    n = int(size)
-    u = _uniform.rvs(size=n)
-    return 0.08*_numpy.exp(2.246879476250902 * _erfinv(-0.8094067254228074 + 1.6975098420629455*u))
+#         Computed using the inverted cumulative probability distribution (CDF) from the initial mass function (IMF) given in equation (17) by Chabrier (2003) https://ui.adsabs.harvard.edu/abs/2003PASP..115..763C/abstract
 
-def imf_gen_10(size):
-    '''
-        Generate stellar mass samples for single star systems between 0.01 and 10.0 Solar Masses.
+#         Parameters
+#         ----------
+#         size: the number of samples to draw.
+#     '''
+#     n = int(size)
+#     u = _uniform.rvs(size=n)
+#     return 0.08*_numpy.exp(2.246879476250902 * _erfinv(-0.8094067254228074 + 1.6975098420629455*u))
+
+# def imf_gen_10(size):
+#     '''
+#         Generate stellar mass samples for single star systems between 0.01 and 10.0 Solar Masses.
         
-        Computed using the inverted cumulative probability distribution (CDF) by smoothly combining the initial mass function (IMF) given in equation (17) by Chabrier (2003) https://ui.adsabs.harvard.edu/abs/2003PASP..115..763C/abstract for stars less than 1.0 Solar Mass with the standard power-law IMF from Salpeter (1955) https://ui.adsabs.harvard.edu/abs/1955ApJ...121..161S/abstract for stars more than 1.0 Solar Mass.
+#         Computed using the inverted cumulative probability distribution (CDF) by smoothly combining the initial mass function (IMF) given in equation (17) by Chabrier (2003) https://ui.adsabs.harvard.edu/abs/2003PASP..115..763C/abstract for stars less than 1.0 Solar Mass with the standard power-law IMF from Salpeter (1955) https://ui.adsabs.harvard.edu/abs/1955ApJ...121..161S/abstract for stars more than 1.0 Solar Mass.
 
-        Parameters
-        ----------
-        size: the number of samples to draw.
-    '''
-    n = int(size)
-    u = _uniform.rvs(size=n)
-    return _numpy.where(u > 0.9424222533172513, 0.11575164791201686 / (1.0030379829867349 - u)**(10/13.), 0.08*_numpy.exp(2.246879476250902 * _erfinv(-0.8094067254228074 + 1.801220032833315*u)))
-
-def imf_gen_100(size):
-    '''
-        Generate stellar mass samples for single star systems between 0.01 and 100.0 Solar Masses.
+#         Parameters
+#         ----------
+#         size: the number of samples to draw.
+#     '''
+#     n = int(size)
+#     u = _uniform.rvs(size=n)
+#     return _numpy.where(u > 0.9424222533172513, 0.11575164791201686 / (1.0030379829867349 - u)**(10/13.), 0.08*_numpy.exp(2.246879476250902 * _erfinv(-0.8094067254228074 + 1.801220032833315*u)))
+
+# def imf_gen_100(size):
+#     '''
+#         Generate stellar mass samples for single star systems between 0.01 and 100.0 Solar Masses.
         
-        Computed using the inverted cumulative probability distribution (CDF) by smoothly combining the initial mass function (IMF) given in equation (17) by Chabrier (2003) https://ui.adsabs.harvard.edu/abs/2003PASP..115..763C/abstract for stars less than 1.0 Solar Mass with the standard power-law IMF from Salpeter (1955) https://ui.adsabs.harvard.edu/abs/1955ApJ...121..161S/abstract for stars more than 1.0 Solar Mass.
+#         Computed using the inverted cumulative probability distribution (CDF) by smoothly combining the initial mass function (IMF) given in equation (17) by Chabrier (2003) https://ui.adsabs.harvard.edu/abs/2003PASP..115..763C/abstract for stars less than 1.0 Solar Mass with the standard power-law IMF from Salpeter (1955) https://ui.adsabs.harvard.edu/abs/1955ApJ...121..161S/abstract for stars more than 1.0 Solar Mass.
 
-        Parameters
-        ----------
-        size: the number of samples to draw.
-    '''
-    n = int(size)
-    u = _uniform.rvs(size=n)
-    return _numpy.where(u > 0.9397105089399359, 0.11549535807627886 / (1.0001518217134586 - u)**(10/13.), 0.08*_numpy.exp(2.246879476250902 * _erfinv(-0.8094067254228074 + 1.8064178551944312*u)))
+#         Parameters
+#         ----------
+#         size: the number of samples to draw.
+#     '''
+#     n = int(size)
+#     u = _uniform.rvs(size=n)
+#     return _numpy.where(u > 0.9397105089399359, 0.11549535807627886 / (1.0001518217134586 - u)**(10/13.), 0.08*_numpy.exp(2.246879476250902 * _erfinv(-0.8094067254228074 + 1.8064178551944312*u)))
 
 
 
 
 ############################################################
 ################### Helper Functions #######################
 ############################################################
 
+def rebound_units(sim):
+    defrebunits = {'length': units.au, 'mass': units.solMass, 'time': units.yr2pi}
+    siunits = {'length': units.m, 'mass': units.kg, 'time': units.s}
+    rebunitset = {'length': _rebound.units.lengths_SI, 'mass': _rebound.units.masses_SI, 'time': _rebound.units.times_SI}
+    simunits = sim.units
+    
+    for unit in simunits:
+        if simunits[unit] == None: simunits[unit] = defrebunits[unit]
+        else: simunits[unit] = rebunitset[unit][simunits[unit]] * siunits[unit]
+    return simunits
+
 # Implemented from StackOverflow: https://stackoverflow.com/a/14314054
 def moving_average(a, n=3) :
     '''Compute the moving average of an array of numbers using the nearest n elements.'''
     ret = _numpy.cumsum(a)
     ret[n:] = ret[n:] - ret[:-n]
     return ret[n - 1:] / n
 
@@ -83,76 +96,81 @@
 def vinf_and_b_to_e(mu, star_b, star_vinf):
     '''
         Using the impact parameter to convert from the relative velocity at infinity between the two stars to the eccentricity of the flyby star.
         Equation (2) from Spurzem et al. (2009) https://ui.adsabs.harvard.edu/abs/2009ApJ...697..458S/abstract
 
         Parameters
         ----------
-        mu : the total mass of the system (Sun, planets, and flyby star) times the gravitational constant G in units where G = 1, Msun, AU, Yr2Pi
-        b :  impact parameter of the flyby star in units of AU
-        vinf : the relative velocity at infinity between the central star and the flyby star (hyperbolic excess velocity) in units of km/s
-    '''
-    G = 1 # Newton's gravitational constant in units of Msun, AU, and Yr2Pi
-    v = star_vinf*convert_kms_to_auyr2pi # Convert velocity units from km/s to AU/Yr2Pi
-    # mu = G
-    numerator = star_b * v**2.
+        mu : the total mass of the system (Sun, planets, and flyby star) times the gravitational constant G
+        b :  impact parameter of the flyby star
+        vinf : the relative velocity at infinity between the central star and the flyby star (hyperbolic excess velocity)
+    '''
+
+    star_b = star_b.to(units.au) if isQuantity(star_b) else star_b * units.au
+    star_vinf = star_vinf.to(units.km/units.s) if isQuantity(star_vinf) else star_vinf * units.km/units.s
+
+    numerator = star_b * star_vinf**2.
     return _numpy.sqrt(1 + (numerator/mu)**2.)
 
 def determine_eccentricity(sim, star_mass, star_b, star_v=None, star_e=None):
-    # Calculate the eccentricity of the flyby star.
-    mu = sim.G * (_numpy.sum([p.m for p in sim.particles]) + star_mass)
+    '''Calculate the eccentricity of the flyby star. '''
+    # Convert the units of the REBOUND Simulation into Astropy Units.
+    units = rebound_units(sim)
+    G = (sim.G * units['length']**3 / units['mass'] / units['time']**2)
+    star_mass = star_mass.to(units['mass']) if isQuantity(star_mass) else star_mass * units['mass']
+    star_b = star_b.to(units['length']) if isQuantity(star_b) else star_b * units['length']
+    star_v = star_v.to(units['length']/units['time']) if isQuantity(star_v) else star_v * units['length']/units['time']
+
+    mu = G * (_numpy.sum([p.m for p in sim.particles]) * units['mass'] + star_mass)
     if star_e is not None and star_v is not None: raise AssertionError('Overdetermined. Cannot specify an eccentricity and a velocity for the perturbing star.')
     elif star_e is not None and star_v is None:
         # Simply use the eccentricity if it is defined.
         return star_e
     elif star_e is None and star_v is not None:
         # If `star_v` is defined convert it to eccentricity.
         # Assumes that `star_v` is in units of km/s.
-        sun_mass = sim.particles[0].m
-        planet_mass = sim.particles[1].m
         return vinf_and_b_to_e(mu=mu, star_b=star_b, star_vinf=star_v)
     else: raise AssertionError('Undetermined. Specify either an eccentricity or a velocity for the perturbing star.')
 
 def cross_section(star_mass, R, v):
     '''
         The cross-section with gravitational focusing.
         
         Parameters
         ----------
         star_mass : the mass of flyby star in units of Msun
         R : the maximum interaction radius in units of AU
         v : the typical velocity from the distribution in units of AU/Yr
     '''
-    
-    G = twopi**2 # Newton's gravitational constant in units of Msun, AU, and Years
-    sun_mass = 1 # mass of the Sun in units of Msun
+    G = const.G.decompose([units.AU, units.yr, units.solMass]) # Newton's gravitational constant in units of Msun, AU, and Years (G ~ 4π^2).
+    sun_mass = 1 * units.solMass # mass of the Sun in units of Msun
     return (_numpy.pi * R**2) * (1 + 2*G*(sun_mass + star_mass)/(R * v**2))
 
-def encounter_rate(n, vbar, R, star_mass=1):
+def encounter_rate(n, vbar, R, star_mass=(1 * units.solMass)):
     '''
         The expected flyby encounter rate within an stellar environment
         
         Parameters
         ----------
         n : stellar number density in units of AU^{-3}
         vbar : velocity dispersion in units of km/s
         R : interaction radius in units of AU
         star_mass : mass of a typical flyby star in units of Msun
     '''
-    vv = vbar*convert_kms_to_auyr # Convert from km/s to AU/yr
+    # vv = vbar*convert_kms_to_auyr # Convert from km/s to AU/yr
     # Include factor of sqrt(2) in cross-section to account for relative velocities at infinity.
-    return n * vv * cross_section(star_mass, R, _numpy.sqrt(2.)*vv)
+    return n * vbar * cross_section(star_mass, R, _numpy.sqrt(2.)*vbar)
 
 
 def isList(l):
+    '''Determines if an object is a list or numpy array. Used for flyby parallelization.'''
     if isinstance(l,(list,_numpy.ndarray)): return True
     else: return False
 
 
-
-
-# UNIT_SYSTEM = [u.AU, u.yr, u.solMass]
-# G_REBOUND = const.G.decompose(UNIT_SYSTEM).value
-# def convertUnits(x):
-#   return [xnew.decompose(UNIT_SYSTEM).value for xnew in x]
-
-# numberdensity, velocity = convertUnits([numberdensity, velocity])
+def isQuantity(var):
+    '''Determines if an object is an Astropy Quantity. Used for Stellar Environment initializations.'''
+    return isinstance(var, units.quantity.Quantity)
+
+def isUnit(var):
+    '''Determines if an object is an Astropy Quantity. Used for Stellar Environment initializations.'''
+    return isinstance(var, (units.core.IrreducibleUnit, units.core.CompositeUnit))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

