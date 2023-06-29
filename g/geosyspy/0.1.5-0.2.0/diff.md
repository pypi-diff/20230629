# Comparing `tmp/geosyspy-0.1.5.tar.gz` & `tmp/geosyspy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosyspy-0.1.5.tar", last modified: Wed May 31 08:19:48 2023, max compression
+gzip compressed data, was "geosyspy-0.2.0.tar", last modified: Thu Jun 29 13:26:42 2023, max compression
```

## Comparing `geosyspy-0.1.5.tar` & `geosyspy-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:19:48.964245 geosyspy-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-31 08:19:48.964245 geosyspy-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-31 08:18:02.000000 geosyspy-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 08:18:02.000000 geosyspy-0.1.5/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:19:48.960245 geosyspy-0.1.5/geosyspy/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/geosys.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/image_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:19:48.964245 geosyspy-0.1.5/geosyspy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/geosys_platform_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/oauth2_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:19:48.964245 geosyspy-0.1.5/geosyspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-31 08:19:48.000000 geosyspy-0.1.5/geosyspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-31 08:19:48.000000 geosyspy-0.1.5/geosyspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:19:48.000000 geosyspy-0.1.5/geosyspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-31 08:19:48.000000 geosyspy-0.1.5/geosyspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 08:19:48.000000 geosyspy-0.1.5/geosyspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 08:19:48.964245 geosyspy-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-31 08:18:02.000000 geosyspy-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:19:48.964245 geosyspy-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/test_int_geosys.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/test_unit_geosys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/test_unit_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/test_unit_oauth2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:26:42.783020 geosyspy-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-06-29 13:26:42.783020 geosyspy-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-06-29 13:24:19.000000 geosyspy-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 13:24:19.000000 geosyspy-0.2.0/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:26:42.779020 geosyspy-0.2.0/geosyspy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43451 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/geosys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/image_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:26:42.779020 geosyspy-0.2.0/geosyspy/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/services/agriquest_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/services/analytics_fabric_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/services/analytics_processor_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/services/gis_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/services/map_product_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/services/master_data_management_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/services/service_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/services/vegetation_time_series_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/services/weather_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:26:42.783020 geosyspy-0.2.0/geosyspy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/utils/geosys_platform_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-29 13:24:19.000000 geosyspy-0.2.0/geosyspy/utils/oauth2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:26:42.779020 geosyspy-0.2.0/geosyspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-06-29 13:26:42.000000 geosyspy-0.2.0/geosyspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-29 13:26:42.000000 geosyspy-0.2.0/geosyspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:26:42.000000 geosyspy-0.2.0/geosyspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 13:26:42.000000 geosyspy-0.2.0/geosyspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 13:26:42.000000 geosyspy-0.2.0/geosyspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 13:26:42.783020 geosyspy-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-29 13:24:19.000000 geosyspy-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:26:42.783020 geosyspy-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_int_geosys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_unit_agriquest_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_unit_analytics_fabric_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_unit_analytics_processor_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_unit_geosys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_unit_gis_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_unit_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_unit_map_product_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_unit_master_data_management_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_unit_oauth2_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_unit_vegetation_time_series_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-29 13:24:19.000000 geosyspy-0.2.0/tests/test_unit_weather_service.py
```

### Comparing `geosyspy-0.1.5/PKG-INFO` & `geosyspy-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: geosyspy
-Version: 0.1.5
-Summary: Easy-to-use python wrapper for Geosys APIs (time series, imagery products)
-Author: Geosys
-Description-Content-Type: text/markdown
-
 <div id="top"></div>
 <!-- PROJECT SHIELDS -->
 <!--
 *** See the bottom of this document for the declaration of the reference variables
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
 
@@ -118,14 +111,23 @@
 Make sure you have valid credentials. If you need to get trial access, please register [here](https://earthdailyagro.com/geosys-api/#get-started).
 
 This package has been tested on Python 3.10.11.
 
 
 ### Installing
 
+#### Conda
+
+If you are using Conda, there are the steps to follow to create a virtual environment:
+
+```
+conda create --name demo
+conda activate demo
+```
+
 #### For Linux / Mac OS
 ```
 pip install geosyspy
 ```
 
 #### For Windows
 
@@ -152,15 +154,31 @@
 ```
 API_CLIENT_ID=
 API_CLIENT_SECRET=
 API_USERNAME=
 API_PASSWORD=
 ```
 
-3. Run the Jupyter notebook
+
+3. Install Jupyter notebook [Examples](examples.ipynb) dependencies 
+
+```
+conda install --file requirements-notebook.txt
+```
+or
+```
+pip install -r requirements-notebook.txt
+```
+
+4. Set up the Jupyter Notebook kernel
+```
+python -m ipykernel install --user --name demo
+```
+
+5. Run the Jupyter notebook
 
 
 ### Run the package inside a Docker container
 
 Build the image locally :
 
 `docker build --tag geosyspy .`
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_pco8wkpm_/tmpiojrysof_TarContainer/0/1", line 25, column 4: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_pco8wkpm_/tmpiojrysof_TarContainer/0/1", line 25, column 4: Levels of opening and closing headings don't match*

```diff
@@ -1,10 +1,7 @@
-Metadata-Version: 2.1 Name: geosyspy Version: 0.1.5 Summary: Easy-to-use python
-wrapper for Geosys APIs (time series, imagery products) Author: Geosys
-Description-Content-Type: text/markdown
 
                                     [Logo]
                             ****** GeosysPy ******
   To be able to discover, request and use imagery products based on  virtual
                    constellation using the &ltgeosys/> API.
                                   Who_we_are
 
@@ -53,29 +50,34 @@
 images time series in [xarray](https://docs.xarray.dev/en/stable/) format *
 Analytic publication: * Save and retrieve custom data in Analytics Fabrik See
 [documentation](https://geosys.github.io/GeosysPy/) and [Examples]
 (examples.ipynb) notebook for more information ## Getting started ###
 Prerequisites Make sure you have valid credentials. If you need to get trial
 access, please register [here](https://earthdailyagro.com/geosys-api/#get-
 started). This package has been tested on Python 3.10.11. ### Installing ####
-For Linux / Mac OS ``` pip install geosyspy ``` #### For Windows Please refer
-to the [install.md](install.md) file. ### Run the package from source 1.
-Install dependencies ``` conda config --add channels conda-forge conda install
---file requirements.txt ``` or ``` pip install -r requirements.txt ``` 2.
-Create .env file You need a .env file with your credentials to run the
-[Examples](examples.ipynb) Jupyter notebook. ``` API_CLIENT_ID=
-API_CLIENT_SECRET= API_USERNAME= API_PASSWORD= ``` 3. Run the Jupyter notebook
-### Run the package inside a Docker container Build the image locally : `docker
-build --tag geosyspy .` Run it : `docker run -it --env-file .env geosyspy` or,
-without .env file : `docker run -it -e API_CLIENT_ID='...' -
-e API_CLIENT_SECRET='...' -e API_USERNAME='...' -e API_PASSWORD='...' geosyspy`
-Then : ```python >>> from geosyspy import Geosys >>> from
-geosyspy.utils.constants import * >>> import os >>> client = Geosys(os.getenv
-('API_CLIENT_ID'), os.getenv('API_CLIENT_SECRET'), os.getenv('API_USERNAME'),
-os.getenv('API_PASSWORD'), Env.PREPROD, Region.NA) ```
+Conda If you are using Conda, there are the steps to follow to create a virtual
+environment: ``` conda create --name demo conda activate demo ``` #### For
+Linux / Mac OS ``` pip install geosyspy ``` #### For Windows Please refer to
+the [install.md](install.md) file. ### Run the package from source 1. Install
+dependencies ``` conda config --add channels conda-forge conda install --file
+requirements.txt ``` or ``` pip install -r requirements.txt ``` 2. Create .env
+file You need a .env file with your credentials to run the [Examples]
+(examples.ipynb) Jupyter notebook. ``` API_CLIENT_ID= API_CLIENT_SECRET=
+API_USERNAME= API_PASSWORD= ``` 3. Install Jupyter notebook [Examples]
+(examples.ipynb) dependencies ``` conda install --file requirements-
+notebook.txt ``` or ``` pip install -r requirements-notebook.txt ``` 4. Set up
+the Jupyter Notebook kernel ``` python -m ipykernel install --user --name demo
+``` 5. Run the Jupyter notebook ### Run the package inside a Docker container
+Build the image locally : `docker build --tag geosyspy .` Run it : `docker run
+-it --env-file .env geosyspy` or, without .env file : `docker run -it -
+e API_CLIENT_ID='...' -e API_CLIENT_SECRET='...' -e API_USERNAME='...' -
+e API_PASSWORD='...' geosyspy` Then : ```python >>> from geosyspy import Geosys
+>>> from geosyspy.utils.constants import * >>> import os >>> client = Geosys
+(os.getenv('API_CLIENT_ID'), os.getenv('API_CLIENT_SECRET'), os.getenv
+('API_USERNAME'), os.getenv('API_PASSWORD'), Env.PREPROD, Region.NA) ```
                                                                   (back_to_top)
 ## Usage Initialize client: ```python from geosyspy import Geosys from
 geosyspy.utils.constants import * client = Geosys("API_CLIENT_ID",
 "API_CLIENT_SECRET", "API_USERNAME", "API_PASSWORD", Env.PREPROD, Region.NA)
 ``` Query data: ```python polygon = "POLYGON((...))" today = dt.date.today()
 year_ago = dt.date.today() + relativedelta(months=-12) dataframe =
 client.get_time_series(polygon, year_ago, today,
```

### Comparing `geosyspy-0.1.5/README.md` & `geosyspy-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: geosyspy
+Version: 0.2.0
+Summary: Easy-to-use python wrapper for Geosys APIs (time series, imagery products)
+Author: Geosys
+Description-Content-Type: text/markdown
+
 <div id="top"></div>
 <!-- PROJECT SHIELDS -->
 <!--
 *** See the bottom of this document for the declaration of the reference variables
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
 
@@ -111,14 +118,23 @@
 Make sure you have valid credentials. If you need to get trial access, please register [here](https://earthdailyagro.com/geosys-api/#get-started).
 
 This package has been tested on Python 3.10.11.
 
 
 ### Installing
 
+#### Conda
+
+If you are using Conda, there are the steps to follow to create a virtual environment:
+
+```
+conda create --name demo
+conda activate demo
+```
+
 #### For Linux / Mac OS
 ```
 pip install geosyspy
 ```
 
 #### For Windows
 
@@ -145,15 +161,31 @@
 ```
 API_CLIENT_ID=
 API_CLIENT_SECRET=
 API_USERNAME=
 API_PASSWORD=
 ```
 
-3. Run the Jupyter notebook
+
+3. Install Jupyter notebook [Examples](examples.ipynb) dependencies 
+
+```
+conda install --file requirements-notebook.txt
+```
+or
+```
+pip install -r requirements-notebook.txt
+```
+
+4. Set up the Jupyter Notebook kernel
+```
+python -m ipykernel install --user --name demo
+```
+
+5. Run the Jupyter notebook
 
 
 ### Run the package inside a Docker container
 
 Build the image locally :
 
 `docker build --tag geosyspy .`
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_pco8wkpm_/tmpiojrysof_TarContainer/0/2.md", line 18, column 4: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_pco8wkpm_/tmpiojrysof_TarContainer/0/2.md", line 18, column 4: Levels of opening and closing headings don't match*

```diff
@@ -1,7 +1,10 @@
+Metadata-Version: 2.1 Name: geosyspy Version: 0.2.0 Summary: Easy-to-use python
+wrapper for Geosys APIs (time series, imagery products) Author: Geosys
+Description-Content-Type: text/markdown
 
                                     [Logo]
                             ****** GeosysPy ******
   To be able to discover, request and use imagery products based on  virtual
                    constellation using the &ltgeosys/> API.
                                   Who_we_are
 
@@ -50,29 +53,34 @@
 images time series in [xarray](https://docs.xarray.dev/en/stable/) format *
 Analytic publication: * Save and retrieve custom data in Analytics Fabrik See
 [documentation](https://geosys.github.io/GeosysPy/) and [Examples]
 (examples.ipynb) notebook for more information ## Getting started ###
 Prerequisites Make sure you have valid credentials. If you need to get trial
 access, please register [here](https://earthdailyagro.com/geosys-api/#get-
 started). This package has been tested on Python 3.10.11. ### Installing ####
-For Linux / Mac OS ``` pip install geosyspy ``` #### For Windows Please refer
-to the [install.md](install.md) file. ### Run the package from source 1.
-Install dependencies ``` conda config --add channels conda-forge conda install
---file requirements.txt ``` or ``` pip install -r requirements.txt ``` 2.
-Create .env file You need a .env file with your credentials to run the
-[Examples](examples.ipynb) Jupyter notebook. ``` API_CLIENT_ID=
-API_CLIENT_SECRET= API_USERNAME= API_PASSWORD= ``` 3. Run the Jupyter notebook
-### Run the package inside a Docker container Build the image locally : `docker
-build --tag geosyspy .` Run it : `docker run -it --env-file .env geosyspy` or,
-without .env file : `docker run -it -e API_CLIENT_ID='...' -
-e API_CLIENT_SECRET='...' -e API_USERNAME='...' -e API_PASSWORD='...' geosyspy`
-Then : ```python >>> from geosyspy import Geosys >>> from
-geosyspy.utils.constants import * >>> import os >>> client = Geosys(os.getenv
-('API_CLIENT_ID'), os.getenv('API_CLIENT_SECRET'), os.getenv('API_USERNAME'),
-os.getenv('API_PASSWORD'), Env.PREPROD, Region.NA) ```
+Conda If you are using Conda, there are the steps to follow to create a virtual
+environment: ``` conda create --name demo conda activate demo ``` #### For
+Linux / Mac OS ``` pip install geosyspy ``` #### For Windows Please refer to
+the [install.md](install.md) file. ### Run the package from source 1. Install
+dependencies ``` conda config --add channels conda-forge conda install --file
+requirements.txt ``` or ``` pip install -r requirements.txt ``` 2. Create .env
+file You need a .env file with your credentials to run the [Examples]
+(examples.ipynb) Jupyter notebook. ``` API_CLIENT_ID= API_CLIENT_SECRET=
+API_USERNAME= API_PASSWORD= ``` 3. Install Jupyter notebook [Examples]
+(examples.ipynb) dependencies ``` conda install --file requirements-
+notebook.txt ``` or ``` pip install -r requirements-notebook.txt ``` 4. Set up
+the Jupyter Notebook kernel ``` python -m ipykernel install --user --name demo
+``` 5. Run the Jupyter notebook ### Run the package inside a Docker container
+Build the image locally : `docker build --tag geosyspy .` Run it : `docker run
+-it --env-file .env geosyspy` or, without .env file : `docker run -it -
+e API_CLIENT_ID='...' -e API_CLIENT_SECRET='...' -e API_USERNAME='...' -
+e API_PASSWORD='...' geosyspy` Then : ```python >>> from geosyspy import Geosys
+>>> from geosyspy.utils.constants import * >>> import os >>> client = Geosys
+(os.getenv('API_CLIENT_ID'), os.getenv('API_CLIENT_SECRET'), os.getenv
+('API_USERNAME'), os.getenv('API_PASSWORD'), Env.PREPROD, Region.NA) ```
                                                                   (back_to_top)
 ## Usage Initialize client: ```python from geosyspy import Geosys from
 geosyspy.utils.constants import * client = Geosys("API_CLIENT_ID",
 "API_CLIENT_SECRET", "API_USERNAME", "API_PASSWORD", Env.PREPROD, Region.NA)
 ``` Query data: ```python polygon = "POLYGON((...))" today = dt.date.today()
 year_ago = dt.date.today() + relativedelta(months=-12) dataframe =
 client.get_time_series(polygon, year_ago, today,
```

### Comparing `geosyspy-0.1.5/geosyspy/utils/http_client.py` & `geosyspy-0.2.0/geosyspy/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.5/geosyspy/utils/oauth2_client.py` & `geosyspy-0.2.0/geosyspy/utils/oauth2_client.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.5/geosyspy.egg-info/PKG-INFO` & `geosyspy-0.2.0/geosyspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geosyspy
-Version: 0.1.5
+Version: 0.2.0
 Summary: Easy-to-use python wrapper for Geosys APIs (time series, imagery products)
 Author: Geosys
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
 <!-- PROJECT SHIELDS -->
 <!--
@@ -118,14 +118,23 @@
 Make sure you have valid credentials. If you need to get trial access, please register [here](https://earthdailyagro.com/geosys-api/#get-started).
 
 This package has been tested on Python 3.10.11.
 
 
 ### Installing
 
+#### Conda
+
+If you are using Conda, there are the steps to follow to create a virtual environment:
+
+```
+conda create --name demo
+conda activate demo
+```
+
 #### For Linux / Mac OS
 ```
 pip install geosyspy
 ```
 
 #### For Windows
 
@@ -152,15 +161,31 @@
 ```
 API_CLIENT_ID=
 API_CLIENT_SECRET=
 API_USERNAME=
 API_PASSWORD=
 ```
 
-3. Run the Jupyter notebook
+
+3. Install Jupyter notebook [Examples](examples.ipynb) dependencies 
+
+```
+conda install --file requirements-notebook.txt
+```
+or
+```
+pip install -r requirements-notebook.txt
+```
+
+4. Set up the Jupyter Notebook kernel
+```
+python -m ipykernel install --user --name demo
+```
+
+5. Run the Jupyter notebook
 
 
 ### Run the package inside a Docker container
 
 Build the image locally :
 
 `docker build --tag geosyspy .`
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_pco8wkpm_/tmpiojrysof_TarContainer/0/16", line 25, column 4: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_pco8wkpm_/tmpiojrysof_TarContainer/0/16", line 25, column 4: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geosyspy Version: 0.1.5 Summary: Easy-to-use python
+Metadata-Version: 2.1 Name: geosyspy Version: 0.2.0 Summary: Easy-to-use python
 wrapper for Geosys APIs (time series, imagery products) Author: Geosys
 Description-Content-Type: text/markdown
 
                                     [Logo]
                             ****** GeosysPy ******
   To be able to discover, request and use imagery products based on  virtual
                    constellation using the &ltgeosys/> API.
@@ -53,29 +53,34 @@
 images time series in [xarray](https://docs.xarray.dev/en/stable/) format *
 Analytic publication: * Save and retrieve custom data in Analytics Fabrik See
 [documentation](https://geosys.github.io/GeosysPy/) and [Examples]
 (examples.ipynb) notebook for more information ## Getting started ###
 Prerequisites Make sure you have valid credentials. If you need to get trial
 access, please register [here](https://earthdailyagro.com/geosys-api/#get-
 started). This package has been tested on Python 3.10.11. ### Installing ####
-For Linux / Mac OS ``` pip install geosyspy ``` #### For Windows Please refer
-to the [install.md](install.md) file. ### Run the package from source 1.
-Install dependencies ``` conda config --add channels conda-forge conda install
---file requirements.txt ``` or ``` pip install -r requirements.txt ``` 2.
-Create .env file You need a .env file with your credentials to run the
-[Examples](examples.ipynb) Jupyter notebook. ``` API_CLIENT_ID=
-API_CLIENT_SECRET= API_USERNAME= API_PASSWORD= ``` 3. Run the Jupyter notebook
-### Run the package inside a Docker container Build the image locally : `docker
-build --tag geosyspy .` Run it : `docker run -it --env-file .env geosyspy` or,
-without .env file : `docker run -it -e API_CLIENT_ID='...' -
-e API_CLIENT_SECRET='...' -e API_USERNAME='...' -e API_PASSWORD='...' geosyspy`
-Then : ```python >>> from geosyspy import Geosys >>> from
-geosyspy.utils.constants import * >>> import os >>> client = Geosys(os.getenv
-('API_CLIENT_ID'), os.getenv('API_CLIENT_SECRET'), os.getenv('API_USERNAME'),
-os.getenv('API_PASSWORD'), Env.PREPROD, Region.NA) ```
+Conda If you are using Conda, there are the steps to follow to create a virtual
+environment: ``` conda create --name demo conda activate demo ``` #### For
+Linux / Mac OS ``` pip install geosyspy ``` #### For Windows Please refer to
+the [install.md](install.md) file. ### Run the package from source 1. Install
+dependencies ``` conda config --add channels conda-forge conda install --file
+requirements.txt ``` or ``` pip install -r requirements.txt ``` 2. Create .env
+file You need a .env file with your credentials to run the [Examples]
+(examples.ipynb) Jupyter notebook. ``` API_CLIENT_ID= API_CLIENT_SECRET=
+API_USERNAME= API_PASSWORD= ``` 3. Install Jupyter notebook [Examples]
+(examples.ipynb) dependencies ``` conda install --file requirements-
+notebook.txt ``` or ``` pip install -r requirements-notebook.txt ``` 4. Set up
+the Jupyter Notebook kernel ``` python -m ipykernel install --user --name demo
+``` 5. Run the Jupyter notebook ### Run the package inside a Docker container
+Build the image locally : `docker build --tag geosyspy .` Run it : `docker run
+-it --env-file .env geosyspy` or, without .env file : `docker run -it -
+e API_CLIENT_ID='...' -e API_CLIENT_SECRET='...' -e API_USERNAME='...' -
+e API_PASSWORD='...' geosyspy` Then : ```python >>> from geosyspy import Geosys
+>>> from geosyspy.utils.constants import * >>> import os >>> client = Geosys
+(os.getenv('API_CLIENT_ID'), os.getenv('API_CLIENT_SECRET'), os.getenv
+('API_USERNAME'), os.getenv('API_PASSWORD'), Env.PREPROD, Region.NA) ```
                                                                   (back_to_top)
 ## Usage Initialize client: ```python from geosyspy import Geosys from
 geosyspy.utils.constants import * client = Geosys("API_CLIENT_ID",
 "API_CLIENT_SECRET", "API_USERNAME", "API_PASSWORD", Env.PREPROD, Region.NA)
 ``` Query data: ```python polygon = "POLYGON((...))" today = dt.date.today()
 year_ago = dt.date.today() + relativedelta(months=-12) dataframe =
 client.get_time_series(polygon, year_ago, today,
```

### Comparing `geosyspy-0.1.5/setup.py` & `geosyspy-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,9 +21,9 @@
     description="Easy-to-use python wrapper for Geosys APIs (time series, imagery products)",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Geosys",
     packages=find_packages(),
     include_package_data=True,
     data_files=[('', ['VERSION.txt'])],
-    install_requires=["requests", "requests-oauthlib", "oauthlib", "scipy", "pandas==1.3.5", "shapely", "rasterio", "xarray"]
+    install_requires=["requests", "requests-oauthlib", "oauthlib", "scipy", "pandas==1.3.5", "shapely", "rasterio", "xarray", "retrying"]
 )
```

### Comparing `geosyspy-0.1.5/tests/test_unit_geosys.py` & `geosyspy-0.2.0/tests/test_unit_geosys.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,72 +34,14 @@
                 "refresh_token"}.issubset(set(credentials.keys()))
         assert credentials['access_token'] is not None
         assert credentials['refresh_token'] is not None
         assert credentials['expires_at'] > datetime.today().timestamp()
 
 
     @patch('geosyspy.utils.http_client.HttpClient.get')
-    def test_get_time_series_modis_ndvi(self, get_response):
-        get_response.return_value = mock_http_response_text_content("GET", load_data_from_textfile(
-            "time_series_modis_ndvi_mock_http_response"))
-        start_date = dt.datetime.strptime("2020-01-01", "%Y-%m-%d")
-        end_date = dt.datetime.strptime("2020-01-07", "%Y-%m-%d")
-        df = self.client.get_time_series(
-            POLYGON, start_date, end_date, SatelliteImageryCollection.MODIS, ["NDVI"]
-        )
-
-        assert df.index.name == "date"
-        assert "value" in df.columns
-        assert "index" in df.columns
-        assert len(df.index) == 7
-        date_range = list(map(lambda x: x.strftime("%Y-%m-%d"), df.index))
-        assert {"2020-01-01", "2020-01-02", "2020-01-03", "2020-01-04", "2020-01-05", "2020-01-06",
-                "2020-01-07"}.issubset(set(date_range))
-
-    @patch('geosyspy.utils.http_client.HttpClient.get')
-    def test_get_satellite_image_time_series_modis_ndvi(self, get_response):
-        get_response.return_value = mock_http_response_text_content("GET", load_data_from_textfile(
-            "satellite_image_time_series_modis_ndvi_mock_http_response"))
-        start_date = dt.datetime.strptime("2020-01-01", "%Y-%m-%d")
-        end_date = dt.datetime.strptime("2020-01-07", "%Y-%m-%d")
-
-        df = self.client.get_satellite_image_time_series(
-            POLYGON, start_date, end_date, [SatelliteImageryCollection.MODIS], ["NDVI"]
-        )
-        assert df.index.name == "date"
-        assert {"value", "index", "pixel.id"}.issubset(set(df.columns))
-        assert np.all((df["index"].values == "NDVI"))
-        assert len(df.index) == 14
-
-        assert {"2020-01-01", "2020-01-02", "2020-01-03", "2020-01-04", "2020-01-05", "2020-01-06",
-                "2020-01-07"}.issubset(set(df.index))
-
-        assert {"mh11v4i225j4612", "mh11v4i226j4612"}.issubset(set(df["pixel.id"]))
-
-    @patch('geosyspy.utils.http_client.HttpClient.get')
-    def test_get_satellite_coverage_image_references(self, get_response):
-        get_response.return_value = mock_http_response_text_content("GET", load_data_from_textfile(
-            "satellite_coverage_image_references_mock_http_response"))
-        start_date = dt.datetime.strptime("2022-01-01", "%Y-%m-%d")
-        end_date = dt.datetime.strptime("2023-01-01", "%Y-%m-%d")
-        info, images_references = self.client.get_satellite_coverage_image_references(
-            POLYGON, start_date, end_date, [SatelliteImageryCollection.SENTINEL_2]
-        )
-
-        assert {"coverageType", "image.id", "image.availableBands", "image.sensor", "image.soilMaterial",
-                "image.spatialResolution", "image.weather", "image.date", "seasonField.id"}.issubset(set(info.columns))
-
-        assert len(info) == len(images_references)
-        for i, image_info in info.iterrows():
-            assert (
-                       image_info["image.date"],
-                       image_info["image.sensor"],
-                   ) in images_references
-
-    @patch('geosyspy.utils.http_client.HttpClient.get')
     def test_get_time_series_weather_historical_daily(self, get_response):
         get_response.return_value = mock_http_response_text_content("GET", load_data_from_textfile(
             "time_series_weather_historical_daily_mock_http_response"))
         start_date = dt.datetime.strptime("2021-01-01", "%Y-%m-%d")
         end_date = dt.datetime.strptime("2022-01-01", "%Y-%m-%d")
         indicators = [
 
@@ -123,16 +65,21 @@
         assert {"precipitation.cumulative", "temperature.standard", "temperature.standardMax",
                 "Location"}.issubset(set(df.columns))
         assert df.index.name == "date"
         assert df["weatherType"].iloc[1] == "HISTORICAL_DAILY"
 
     @patch('geosyspy.utils.http_client.HttpClient.get')
     def test_get_metrics(self, get_response):
-        get_response.return_value = mock_http_response_text_content("GET", load_data_from_textfile(
+
+        fake_master_data_management_response = mock_http_response_text_content("GET", load_data_from_textfile(
+            "master_data_management_get_unique_id_mock_http_response"))
+        fake_analytics_fabric_response = mock_http_response_text_content("GET", load_data_from_textfile(
             "metrics_lai_radar_mock_http_response"))
+        get_response.side_effect= [fake_master_data_management_response, fake_analytics_fabric_response]
+
 
         lai_radar_polygon = "POLYGON((-52.72591542 -18.7395779,-52.72604885 -18.73951122,-52.72603114 -18.73908689,-52.71556835 -18.72490316,-52.71391916 -18.72612966,-52.71362802 -18.72623726,-52.71086473 -18.72804231,-52.72083542 -18.74173696,-52.72118937 -18.74159174,-52.72139229 -18.7418552,-52.72600257 -18.73969719,-52.72591542 -18.7395779))"
         schema_id = "LAI_RADAR"
         start_date = dt.datetime.strptime("2023-01-02", "%Y-%m-%d")
         end_date = dt.datetime.strptime("2023-05-02", "%Y-%m-%d")
         df = self.client.get_metrics(lai_radar_polygon, schema_id, start_date, end_date)
 
@@ -181,7 +128,36 @@
             POLYGON,
             start_date,
             end_date,
             collections=[SatelliteImageryCollection.SENTINEL_2, SatelliteImageryCollection.LANDSAT_8],
             indicators=["Reflectance"],
         )
         assert dict(dataset.dims) == {'band': 4, 'y': 80, 'x': 81, 'time': 2}
+
+
+    @patch('geosyspy.utils.http_client.HttpClient.post')
+    def test_get_agriquest_weather_block_data(self, get_response):
+        get_response.return_value =  mock_http_response_text_content("POST", load_data_from_textfile(
+           "agriquest_weather_data_mock_http_response"))
+        start_date = "2022-05-01"
+        end_date = "2023-04-28"
+        dataset = self.client.get_agriquest_weather_block_data(
+            start_date=start_date,
+            end_date=end_date,
+            block_code=AgriquestBlocks.FRA_DEPARTEMENTS,
+            weather_type=AgriquestWeatherType.CUMULATIVE_PRECIPITATION
+        )
+        assert dataset.keys()[0] == "AMU"
+        assert len(dataset["AMU"]) == 97
+
+    @patch('geosyspy.utils.http_client.HttpClient.post')
+    def test_get_agriquest_ndvi_block_data(self, get_response):
+        get_response.return_value =  mock_http_response_text_content("POST", load_data_from_textfile(
+           "agriquest_ndvi_data_mock_http_response"))
+        date = "2023-06-05"
+        dataset = self.client.get_agriquest_ndvi_block_data(
+            day_of_measure=date,
+            commodity_code=AgriquestCommodityCode.ALL_VEGETATION,
+            block_code=AgriquestBlocks.AMU_NORTH_AMERICA,
+        )
+        assert dataset.keys()[0] == "AMU"
+        assert dataset.keys()[-1] == "NDVI"
```

### Comparing `geosyspy-0.1.5/tests/test_unit_http_client.py` & `geosyspy-0.2.0/tests/test_unit_http_client.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.5/tests/test_unit_oauth2_client.py` & `geosyspy-0.2.0/tests/test_unit_oauth2_client.py`

 * *Files identical despite different names*

