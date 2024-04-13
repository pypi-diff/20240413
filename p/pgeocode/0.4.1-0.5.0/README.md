# Comparing `tmp/pgeocode-0.4.1.tar.gz` & `tmp/pgeocode-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgeocode-0.4.1.tar", last modified: Thu Sep  7 18:16:07 2023, max compression
+gzip compressed data, was "pgeocode-0.5.0.tar", last modified: Sat Apr 13 06:45:47 2024, max compression
```

## Comparing `pgeocode-0.4.1.tar` & `pgeocode-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rth       (1000) rth       (1000)        0 2023-09-07 18:16:07.545078 pgeocode-0.4.1/
--rw-rw-r--   0 rth       (1000) rth       (1000)     1507 2022-12-13 20:27:13.000000 pgeocode-0.4.1/LICENSE
--rw-r--r--   0 rth       (1000) rth       (1000)     8371 2023-09-07 18:16:07.545078 pgeocode-0.4.1/PKG-INFO
--rw-rw-r--   0 rth       (1000) rth       (1000)     7684 2022-12-13 23:23:25.000000 pgeocode-0.4.1/README.rst
-drwxrwxr-x   0 rth       (1000) rth       (1000)        0 2023-09-07 18:16:07.545078 pgeocode-0.4.1/pgeocode.egg-info/
--rw-r--r--   0 rth       (1000) rth       (1000)     8371 2023-09-07 18:16:07.000000 pgeocode-0.4.1/pgeocode.egg-info/PKG-INFO
--rw-rw-r--   0 rth       (1000) rth       (1000)      213 2023-09-07 18:16:07.000000 pgeocode-0.4.1/pgeocode.egg-info/SOURCES.txt
--rw-rw-r--   0 rth       (1000) rth       (1000)        1 2023-09-07 18:16:07.000000 pgeocode-0.4.1/pgeocode.egg-info/dependency_links.txt
--rw-rw-r--   0 rth       (1000) rth       (1000)       39 2023-09-07 18:16:07.000000 pgeocode-0.4.1/pgeocode.egg-info/requires.txt
--rw-rw-r--   0 rth       (1000) rth       (1000)        9 2023-09-07 18:16:07.000000 pgeocode-0.4.1/pgeocode.egg-info/top_level.txt
--rw-rw-r--   0 rth       (1000) rth       (1000)    14440 2023-09-07 18:15:15.000000 pgeocode-0.4.1/pgeocode.py
--rw-rw-r--   0 rth       (1000) rth       (1000)      907 2022-12-13 22:03:09.000000 pgeocode-0.4.1/pyproject.toml
--rw-rw-r--   0 rth       (1000) rth       (1000)       38 2023-09-07 18:16:07.545078 pgeocode-0.4.1/setup.cfg
--rw-rw-r--   0 rth       (1000) rth       (1000)     1322 2022-12-13 22:15:27.000000 pgeocode-0.4.1/setup.py
+drwxrwxr-x   0 rth       (1000) rth       (1000)        0 2024-04-13 06:45:47.148501 pgeocode-0.5.0/
+-rw-rw-r--   0 rth       (1000) rth       (1000)     1507 2022-12-13 20:27:13.000000 pgeocode-0.5.0/LICENSE
+-rw-r--r--   0 rth       (1000) rth       (1000)     7888 2024-04-13 06:45:47.148501 pgeocode-0.5.0/PKG-INFO
+-rw-rw-r--   0 rth       (1000) rth       (1000)     7160 2024-04-12 09:44:06.000000 pgeocode-0.5.0/README.md
+drwxrwxr-x   0 rth       (1000) rth       (1000)        0 2024-04-13 06:45:47.148501 pgeocode-0.5.0/pgeocode.egg-info/
+-rw-r--r--   0 rth       (1000) rth       (1000)     7888 2024-04-13 06:45:47.000000 pgeocode-0.5.0/pgeocode.egg-info/PKG-INFO
+-rw-rw-r--   0 rth       (1000) rth       (1000)      212 2024-04-13 06:45:47.000000 pgeocode-0.5.0/pgeocode.egg-info/SOURCES.txt
+-rw-rw-r--   0 rth       (1000) rth       (1000)        1 2024-04-13 06:45:47.000000 pgeocode-0.5.0/pgeocode.egg-info/dependency_links.txt
+-rw-rw-r--   0 rth       (1000) rth       (1000)       39 2024-04-13 06:45:47.000000 pgeocode-0.5.0/pgeocode.egg-info/requires.txt
+-rw-rw-r--   0 rth       (1000) rth       (1000)        9 2024-04-13 06:45:47.000000 pgeocode-0.5.0/pgeocode.egg-info/top_level.txt
+-rw-rw-r--   0 rth       (1000) rth       (1000)    14240 2024-04-13 06:44:17.000000 pgeocode-0.5.0/pgeocode.py
+-rw-rw-r--   0 rth       (1000) rth       (1000)     1310 2024-04-12 09:44:06.000000 pgeocode-0.5.0/pyproject.toml
+-rw-rw-r--   0 rth       (1000) rth       (1000)       38 2024-04-13 06:45:47.148501 pgeocode-0.5.0/setup.cfg
+-rw-rw-r--   0 rth       (1000) rth       (1000)     1349 2024-04-12 09:44:06.000000 pgeocode-0.5.0/setup.py
```

### Comparing `pgeocode-0.4.1/LICENSE` & `pgeocode-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgeocode-0.4.1/PKG-INFO` & `pgeocode-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,190 +1,196 @@
 Metadata-Version: 2.1
 Name: pgeocode
-Version: 0.4.1
-Summary: Approximate geocoding
+Version: 0.5.0
+Summary: Postal code geocoding
 Author: Roman Yurchak
 Author-email: roman.yurchak@symerio.com
 License: BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Requires-Python: >=3.8
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: pandas
 Provides-Extra: fuzzy
 Requires-Dist: thefuzz; extra == "fuzzy"
 
-pgeocode
-========
-
-|pypi| |condaforge| |rdfd| |GHactions|
-
-.. |pypi| image:: https://img.shields.io/pypi/v/pgeocode.svg
-   :target: https://pypi.org/project/pgeocode/
-
-.. |condaforge| image:: https://img.shields.io/conda/vn/conda-forge/pgeocode.svg
-   :target: https://anaconda.org/conda-forge/pgeocode
-
-.. |rdfd| image:: https://readthedocs.org/projects/pgeocode/badge/?version=latest
-    :target: http://pgeocode.readthedocs.io/
-
-.. |GHactions| image:: https://github.com/symerio/pgeocode/workflows/Test/badge.svg
-   :target: https://github.com/symerio/pgeocode/actions?query=branch%3Amaster+
+# pgeocode
 
+[![pypi](https://img.shields.io/pypi/v/pgeocode.svg)](https://pypi.org/project/pgeocode/)
+[![rdfd](https://readthedocs.org/projects/pgeocode/badge/?version=latest)](http://pgeocode.readthedocs.io/)
+[![GHactions](https://github.com/symerio/pgeocode/workflows/Test/badge.svg)](https://github.com/symerio/pgeocode/actions?query=branch%3Amaster+)
 
 Postal code geocoding and distance calculations
 
-pgeocode is a Python library for high performance off-line querying of GPS coordinates, region name and municipality name
-from postal codes. Distances between postal codes as well as general
-distance queries are also supported.
-The used `GeoNames <http://download.geonames.org/export/zip/>`_ database includes postal codes for 83 countries.
+pgeocode is a Python library for high performance off-line querying of
+GPS coordinates, region name and municipality name from postal codes.
+Distances between postal codes as well as general distance queries are
+also supported. The used
+[GeoNames](http://download.geonames.org/export/zip/) database includes
+postal codes for 83 countries.
 
 Currently, only queries within the same country are supported.
 
-For additional documentation see `pgeocode.readthedocs.io <https://pgeocode.readthedocs.io>`_.
-
-
-Installation
-------------
-
-pgeocode requires Python 3.8+ as well as ``numpy`` and ``pandas`` packages. It can be installed with,
+For additional documentation see
+[pgeocode.readthedocs.io](https://pgeocode.readthedocs.io).
 
-.. code::
+# Installation
 
-    pip install pgeocode
+pgeocode requires Python 3.10+ as well as `numpy` and `pandas` packages.
+It can be installed with,
 
-or
+```
+pip install pgeocode
+```
 
-.. code::
 
-    conda install -c conda-forge pgeocode
-
-Quickstart
-----------
+# Quickstart
 
 **Postal code queries**
 
-.. code:: python
-
-    >>> import pgeocode
+```python
+>>> import pgeocode
 
-    >>> nomi = pgeocode.Nominatim('fr')
-    >>> nomi.query_postal_code("75013")
-    postal_code               75013
-    country_code                 FR
-    place_name             Paris 13
-    state_name        Île-de-France
-    state_code                   11
-    county_name               Paris
-    county_code                  75
-    community_name            Paris
-    community_code              751
-    latitude                48.8322
-    longitude                2.3561
-    accuracy                      5
-
-    >>> nomi.query_postal_code(["75013", "69006"])
-          postal_code place_name            state_name  latitude  longitude
-    0       75013   Paris 13         Île-de-France   48.8322     2.3561
-    1       69006    Lyon 06  Auvergne-Rhône-Alpes   45.7679     4.8506
+>>> nomi = pgeocode.Nominatim('fr')
+>>> nomi.query_postal_code("75013")
+postal_code               75013
+country_code                 FR
+place_name             Paris 13
+state_name        Île-de-France
+state_code                   11
+county_name               Paris
+county_code                  75
+community_name            Paris
+community_code              751
+latitude                48.8322
+longitude                2.3561
+accuracy                      5
+
+>>> nomi.query_postal_code(["75013", "69006"])
+      postal_code place_name            state_name  latitude  longitude
+0       75013   Paris 13         Île-de-France   48.8322     2.3561
+1       69006    Lyon 06  Auvergne-Rhône-Alpes   45.7679     4.8506
+```
 
 **Place name queries**
 
-.. code:: python
+```python
+>>> import pgeocode
 
-    >>> import pgeocode
-
-    >>> nomi = pgeocode.Nominatim('fr')
-    >>> nomi.query_location("Antibes", top_k=3)
-        country_code  postal_code place_name                  state_name  state_code  ... community_name community_code latitude longitude  accuracy
-    49553           FR        06160    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
-    49787           FR        06600    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
-    49788           FR  06601 CEDEX    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
-
-    >>> nomi.query_location("Straassborg", top_k=3, fuzzy_threshold=80)
-        country_code  postal_code  place_name state_name  state_code  ... community_name community_code latitude longitude  accuracy
-    25461           FR        67000  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
-    25462           FR  67001 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
-    25463           FR  67002 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+>>> nomi = pgeocode.Nominatim('fr')
+>>> nomi.query_location("Antibes", top_k=3)
+    country_code  postal_code place_name                  state_name  state_code  ... community_name community_code latitude longitude  accuracy
+49553           FR        06160    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
+49787           FR        06600    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
+49788           FR  06601 CEDEX    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
+
+>>> nomi.query_location("Straassborg", top_k=3, fuzzy_threshold=80)
+    country_code  postal_code  place_name state_name  state_code  ... community_name community_code latitude longitude  accuracy
+25461           FR        67000  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+25462           FR  67001 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+25463           FR  67002 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+```
 
 **Distance calculations**
 
-.. code:: python
-
-    >>> dist = pgeocode.GeoDistance('fr')
-    >>> dist.query_postal_code("75013", "69006")
-    389.156
-    >>> dist.query_postal_code(["75013", "75014", "75015"], ["69006", "69005", "69004"])
-    array([ 389.15648697,  390.12577967,  390.49857655])
-
-
-Geocoding format
-----------------
-
-The result of a geo-localistion query is a ``pandas.DataFrame`` with the following columns,
-
-* ``country_code``: iso country code, 2 characters
-* ``postal_code`` : postal code
-* ``place_name``  : place name (e.g. town, city etc)
-* ``state_name`` : 1. order subdivision (state)
-* ``state_code`` : 1. order subdivision (state)
-* ``county_name`` : 2. order subdivision (county/province)
-* ``county_code`` : 2. order subdivision (county/province)
-* ``community_name`` : 3. order subdivision (community)
-* ``community_code`` : 3. order subdivision (community)
-* ``latitude``    : estimated latitude (wgs84)
-* ``longitude``   : estimated longitude (wgs84)
-* ``accuracy``    : accuracy of lat/lng from 1=estimated to 6=centroid
+```python
+>>> dist = pgeocode.GeoDistance('fr')
+>>> dist.query_postal_code("75013", "69006")
+389.156
+>>> dist.query_postal_code(["75013", "75014", "75015"], ["69006", "69005", "69004"])
+array([ 389.15648697,  390.12577967,  390.49857655])
+```
+
+# Geocoding format
+
+The result of a geo-localistion query is a `pandas.DataFrame` with the
+following columns,
+
+-   `country_code`: iso country code, 2 characters
+-   `postal_code` : postal code
+-   `place_name` : place name (e.g. town, city etc)
+-   `state_name` : 1. order subdivision (state)
+-   `state_code` : 1. order subdivision (state)
+-   `county_name` : 2. order subdivision (county/province)
+-   `county_code` : 2. order subdivision (county/province)
+-   `community_name` : 3. order subdivision (community)
+-   `community_code` : 3. order subdivision (community)
+-   `latitude` : estimated latitude (wgs84)
+-   `longitude` : estimated longitude (wgs84)
+-   `accuracy` : accuracy of lat/lng from 1=estimated to 6=centroid
 
-
-Configuration and defaults
---------------------------
+# Configuration and defaults
 
 **Storage directory**
 
-Defaults to ``~/.cache/pgeocode``, it is the directory where data is downloaded
-for later consumption. It can be changed using the environment variable
-``PGEOCODE_DATA_DIR``, i.e. ``export PGEOCODE_DATA_DIR=/tmp/pgeocode_data``.
+Defaults to `~/.cache/pgeocode`, it is the directory where data is
+downloaded for later consumption. It can be changed using the
+environment variable `PGEOCODE_DATA_DIR`, i.e.
+`export PGEOCODE_DATA_DIR=/tmp/pgeocode_data`.
 
 **Data sources**
 
-Data sources are provided as a list in the ``pgeocode.DOWNLOAD_URL`` variable.
-The default value is,
-
-.. code:: python
+Data sources are provided as a list in the `pgeocode.DOWNLOAD_URL`
+variable. The default value is,
 
-    DOWNLOAD_URL = [
-        "https://download.geonames.org/export/zip/{country}.zip",
-        "https://symerio.github.io/postal-codes-data/data/geonames/{country}.txt",
-    ]
-
-Data sources are tried from first to last until one works. Here the second link is a mirror
-of the first.
-
-It is also possible to extend this variable with third party data sources, as
-long as they follow the same format. See for instance
-`postal-codes-data <https://github.com/symerio/postal-codes-data/tree/master/data/geonames>`_
+``` python
+DOWNLOAD_URL = [
+    "https://download.geonames.org/export/zip/{country}.zip",
+    "https://symerio.github.io/postal-codes-data/data/geonames/{country}.txt",
+]
+```
+
+Data sources are tried from first to last until one works. Here the
+second link is a mirror of the first.
+
+It is also possible to extend this variable with third party data
+sources, as long as they follow the same format. See for instance
+[postal-codes-data](https://github.com/symerio/postal-codes-data/tree/master/data/geonames)
 repository for examples of data files.
 
-
-License
--------
+# License
 
 The pgeocode package is distributed under the 3-clause BSD license.
 
+The pgeocode package is maintained by [Symerio](https://www.symerio.com).
 
-Supported countries
--------------------
+# Supported countries
 
-The list of countries available in the GeoNames database, with the corresponding country codes, are given below,
+The list of countries available in the GeoNames database, with the
+corresponding country codes, are given below,
 
-Andorra (AD), Argentina (AR), American Samoa (AS), Austria (AT), Australia (AU), Åland Islands (AX), Azerbaijan (AZ), Bangladesh (BD), Belgium (BE), Bulgaria (BG), Bermuda (BM), Brazil (BR), Belarus (BY), Canada (CA), Switzerland (CH), Chile (CL), Colombia (CO), Costa Rica (CR), Cyprus (CY), Czechia (CZ), Germany (DE), Denmark (DK), Dominican Republic (DO), Algeria (DZ), Estonia (EE), Spain (ES), Finland (FI), Federated States of Micronesia (FM), Faroe Islands (FO), France (FR), United Kingdom of Great Britain and Northern Ireland (GB), French Guiana (GF), Guernsey (GG), Greenland (GL), Guadeloupe (GP), Guatemala (GT), Guam (GU), Croatia (HR), Haiti (HT), Hungary (HU), Ireland (IE), Isle of Man (IM), India (IN), Iceland (IS), Italy (IT), Jersey (JE), Japan (JP), Republic of Korea (KR), Liechtenstein (LI), Sri Lanka (LK), Lithuania (LT), Luxembourg (LU), Latvia (LV), Monaco (MC), Republic of Moldova (MD), Marshall Islands (MH), The former Yugoslav Republic of Macedonia (MK), Northern Mariana Islands (MP), Martinique (MQ), Malta (MT), Malawi (MW), Mexico (MX), Malaysia (MY), New Caledonia (NC), Netherlands (NL), Norway (NO), New Zealand (NZ), Peru (PE), Philippines (PH), Pakistan (PK), Poland (PL), Saint Pierre and Miquelon (PM), Puerto Rico (PR), Portugal (PT), Palau (PW), Réunion (RE), Romania (RO), Serbia (RS), Russian Federation (RU), Sweden (SE), Singapore (SG), Slovenia (SI), Svalbard and Jan Mayen Islands (SJ), Slovakia (SK), San Marino (SM), Thailand (TH), Turkey (TR), Ukraine (UA), United States of America (US), Uruguay (UY), Holy See (VA), United States Virgin Islands (VI), Wallis and Futuna Islands (WF), Mayotte (YT), South Africa (ZA)
+Andorra (AD), Argentina (AR), American Samoa (AS), Austria (AT),
+Australia (AU), Åland Islands (AX), Azerbaijan (AZ), Bangladesh (BD),
+Belgium (BE), Bulgaria (BG), Bermuda (BM), Brazil (BR), Belarus (BY),
+Canada (CA), Switzerland (CH), Chile (CL), Colombia (CO), Costa Rica
+(CR), Cyprus (CY), Czechia (CZ), Germany (DE), Denmark (DK), Dominican
+Republic (DO), Algeria (DZ), Estonia (EE), Spain (ES), Finland (FI),
+Federated States of Micronesia (FM), Faroe Islands (FO), France (FR),
+United Kingdom of Great Britain and Northern Ireland (GB), French Guiana
+(GF), Guernsey (GG), Greenland (GL), Guadeloupe (GP), Guatemala (GT),
+Guam (GU), Croatia (HR), Haiti (HT), Hungary (HU), Ireland (IE), Isle of
+Man (IM), India (IN), Iceland (IS), Italy (IT), Jersey (JE), Japan (JP),
+Republic of Korea (KR), Liechtenstein (LI), Sri Lanka (LK), Lithuania
+(LT), Luxembourg (LU), Latvia (LV), Monaco (MC), Republic of Moldova
+(MD), Marshall Islands (MH), The former Yugoslav Republic of Macedonia
+(MK), Northern Mariana Islands (MP), Martinique (MQ), Malta (MT), Malawi
+(MW), Mexico (MX), Malaysia (MY), New Caledonia (NC), Netherlands (NL),
+Norway (NO), New Zealand (NZ), Peru (PE), Philippines (PH), Pakistan
+(PK), Poland (PL), Saint Pierre and Miquelon (PM), Puerto Rico (PR),
+Portugal (PT), Palau (PW), Réunion (RE), Romania (RO), Serbia (RS),
+Russian Federation (RU), Sweden (SE), Singapore (SG), Slovenia (SI),
+Svalbard and Jan Mayen Islands (SJ), Slovakia (SK), San Marino (SM),
+Thailand (TH), Turkey (TR), Ukraine (UA), United States of America (US),
+Uruguay (UY), Holy See (VA), United States Virgin Islands (VI), Wallis
+and Futuna Islands (WF), Mayotte (YT), South Africa (ZA)
 
-See `GeoNames database <http://download.geonames.org/export/zip/>`_ for more information.
+See [GeoNames database](http://download.geonames.org/export/zip/) for
+more information.
```

### Comparing `pgeocode-0.4.1/README.rst` & `pgeocode-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,167 +1,172 @@
-pgeocode
-========
-
-|pypi| |condaforge| |rdfd| |GHactions|
-
-.. |pypi| image:: https://img.shields.io/pypi/v/pgeocode.svg
-   :target: https://pypi.org/project/pgeocode/
-
-.. |condaforge| image:: https://img.shields.io/conda/vn/conda-forge/pgeocode.svg
-   :target: https://anaconda.org/conda-forge/pgeocode
-
-.. |rdfd| image:: https://readthedocs.org/projects/pgeocode/badge/?version=latest
-    :target: http://pgeocode.readthedocs.io/
-
-.. |GHactions| image:: https://github.com/symerio/pgeocode/workflows/Test/badge.svg
-   :target: https://github.com/symerio/pgeocode/actions?query=branch%3Amaster+
+# pgeocode
 
+[![pypi](https://img.shields.io/pypi/v/pgeocode.svg)](https://pypi.org/project/pgeocode/)
+[![rdfd](https://readthedocs.org/projects/pgeocode/badge/?version=latest)](http://pgeocode.readthedocs.io/)
+[![GHactions](https://github.com/symerio/pgeocode/workflows/Test/badge.svg)](https://github.com/symerio/pgeocode/actions?query=branch%3Amaster+)
 
 Postal code geocoding and distance calculations
 
-pgeocode is a Python library for high performance off-line querying of GPS coordinates, region name and municipality name
-from postal codes. Distances between postal codes as well as general
-distance queries are also supported.
-The used `GeoNames <http://download.geonames.org/export/zip/>`_ database includes postal codes for 83 countries.
+pgeocode is a Python library for high performance off-line querying of
+GPS coordinates, region name and municipality name from postal codes.
+Distances between postal codes as well as general distance queries are
+also supported. The used
+[GeoNames](http://download.geonames.org/export/zip/) database includes
+postal codes for 83 countries.
 
 Currently, only queries within the same country are supported.
 
-For additional documentation see `pgeocode.readthedocs.io <https://pgeocode.readthedocs.io>`_.
-
-
-Installation
-------------
-
-pgeocode requires Python 3.8+ as well as ``numpy`` and ``pandas`` packages. It can be installed with,
+For additional documentation see
+[pgeocode.readthedocs.io](https://pgeocode.readthedocs.io).
 
-.. code::
+# Installation
 
-    pip install pgeocode
+pgeocode requires Python 3.10+ as well as `numpy` and `pandas` packages.
+It can be installed with,
 
-or
+```
+pip install pgeocode
+```
 
-.. code::
 
-    conda install -c conda-forge pgeocode
-
-Quickstart
-----------
+# Quickstart
 
 **Postal code queries**
 
-.. code:: python
-
-    >>> import pgeocode
+```python
+>>> import pgeocode
 
-    >>> nomi = pgeocode.Nominatim('fr')
-    >>> nomi.query_postal_code("75013")
-    postal_code               75013
-    country_code                 FR
-    place_name             Paris 13
-    state_name        Île-de-France
-    state_code                   11
-    county_name               Paris
-    county_code                  75
-    community_name            Paris
-    community_code              751
-    latitude                48.8322
-    longitude                2.3561
-    accuracy                      5
-
-    >>> nomi.query_postal_code(["75013", "69006"])
-          postal_code place_name            state_name  latitude  longitude
-    0       75013   Paris 13         Île-de-France   48.8322     2.3561
-    1       69006    Lyon 06  Auvergne-Rhône-Alpes   45.7679     4.8506
+>>> nomi = pgeocode.Nominatim('fr')
+>>> nomi.query_postal_code("75013")
+postal_code               75013
+country_code                 FR
+place_name             Paris 13
+state_name        Île-de-France
+state_code                   11
+county_name               Paris
+county_code                  75
+community_name            Paris
+community_code              751
+latitude                48.8322
+longitude                2.3561
+accuracy                      5
+
+>>> nomi.query_postal_code(["75013", "69006"])
+      postal_code place_name            state_name  latitude  longitude
+0       75013   Paris 13         Île-de-France   48.8322     2.3561
+1       69006    Lyon 06  Auvergne-Rhône-Alpes   45.7679     4.8506
+```
 
 **Place name queries**
 
-.. code:: python
+```python
+>>> import pgeocode
 
-    >>> import pgeocode
-
-    >>> nomi = pgeocode.Nominatim('fr')
-    >>> nomi.query_location("Antibes", top_k=3)
-        country_code  postal_code place_name                  state_name  state_code  ... community_name community_code latitude longitude  accuracy
-    49553           FR        06160    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
-    49787           FR        06600    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
-    49788           FR  06601 CEDEX    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
-
-    >>> nomi.query_location("Straassborg", top_k=3, fuzzy_threshold=80)
-        country_code  postal_code  place_name state_name  state_code  ... community_name community_code latitude longitude  accuracy
-    25461           FR        67000  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
-    25462           FR  67001 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
-    25463           FR  67002 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+>>> nomi = pgeocode.Nominatim('fr')
+>>> nomi.query_location("Antibes", top_k=3)
+    country_code  postal_code place_name                  state_name  state_code  ... community_name community_code latitude longitude  accuracy
+49553           FR        06160    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
+49787           FR        06600    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
+49788           FR  06601 CEDEX    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
+
+>>> nomi.query_location("Straassborg", top_k=3, fuzzy_threshold=80)
+    country_code  postal_code  place_name state_name  state_code  ... community_name community_code latitude longitude  accuracy
+25461           FR        67000  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+25462           FR  67001 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+25463           FR  67002 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+```
 
 **Distance calculations**
 
-.. code:: python
-
-    >>> dist = pgeocode.GeoDistance('fr')
-    >>> dist.query_postal_code("75013", "69006")
-    389.156
-    >>> dist.query_postal_code(["75013", "75014", "75015"], ["69006", "69005", "69004"])
-    array([ 389.15648697,  390.12577967,  390.49857655])
-
-
-Geocoding format
-----------------
-
-The result of a geo-localistion query is a ``pandas.DataFrame`` with the following columns,
-
-* ``country_code``: iso country code, 2 characters
-* ``postal_code`` : postal code
-* ``place_name``  : place name (e.g. town, city etc)
-* ``state_name`` : 1. order subdivision (state)
-* ``state_code`` : 1. order subdivision (state)
-* ``county_name`` : 2. order subdivision (county/province)
-* ``county_code`` : 2. order subdivision (county/province)
-* ``community_name`` : 3. order subdivision (community)
-* ``community_code`` : 3. order subdivision (community)
-* ``latitude``    : estimated latitude (wgs84)
-* ``longitude``   : estimated longitude (wgs84)
-* ``accuracy``    : accuracy of lat/lng from 1=estimated to 6=centroid
+```python
+>>> dist = pgeocode.GeoDistance('fr')
+>>> dist.query_postal_code("75013", "69006")
+389.156
+>>> dist.query_postal_code(["75013", "75014", "75015"], ["69006", "69005", "69004"])
+array([ 389.15648697,  390.12577967,  390.49857655])
+```
+
+# Geocoding format
+
+The result of a geo-localistion query is a `pandas.DataFrame` with the
+following columns,
+
+-   `country_code`: iso country code, 2 characters
+-   `postal_code` : postal code
+-   `place_name` : place name (e.g. town, city etc)
+-   `state_name` : 1. order subdivision (state)
+-   `state_code` : 1. order subdivision (state)
+-   `county_name` : 2. order subdivision (county/province)
+-   `county_code` : 2. order subdivision (county/province)
+-   `community_name` : 3. order subdivision (community)
+-   `community_code` : 3. order subdivision (community)
+-   `latitude` : estimated latitude (wgs84)
+-   `longitude` : estimated longitude (wgs84)
+-   `accuracy` : accuracy of lat/lng from 1=estimated to 6=centroid
 
-
-Configuration and defaults
---------------------------
+# Configuration and defaults
 
 **Storage directory**
 
-Defaults to ``~/.cache/pgeocode``, it is the directory where data is downloaded
-for later consumption. It can be changed using the environment variable
-``PGEOCODE_DATA_DIR``, i.e. ``export PGEOCODE_DATA_DIR=/tmp/pgeocode_data``.
+Defaults to `~/.cache/pgeocode`, it is the directory where data is
+downloaded for later consumption. It can be changed using the
+environment variable `PGEOCODE_DATA_DIR`, i.e.
+`export PGEOCODE_DATA_DIR=/tmp/pgeocode_data`.
 
 **Data sources**
 
-Data sources are provided as a list in the ``pgeocode.DOWNLOAD_URL`` variable.
-The default value is,
-
-.. code:: python
+Data sources are provided as a list in the `pgeocode.DOWNLOAD_URL`
+variable. The default value is,
 
-    DOWNLOAD_URL = [
-        "https://download.geonames.org/export/zip/{country}.zip",
-        "https://symerio.github.io/postal-codes-data/data/geonames/{country}.txt",
-    ]
-
-Data sources are tried from first to last until one works. Here the second link is a mirror
-of the first.
-
-It is also possible to extend this variable with third party data sources, as
-long as they follow the same format. See for instance
-`postal-codes-data <https://github.com/symerio/postal-codes-data/tree/master/data/geonames>`_
+``` python
+DOWNLOAD_URL = [
+    "https://download.geonames.org/export/zip/{country}.zip",
+    "https://symerio.github.io/postal-codes-data/data/geonames/{country}.txt",
+]
+```
+
+Data sources are tried from first to last until one works. Here the
+second link is a mirror of the first.
+
+It is also possible to extend this variable with third party data
+sources, as long as they follow the same format. See for instance
+[postal-codes-data](https://github.com/symerio/postal-codes-data/tree/master/data/geonames)
 repository for examples of data files.
 
-
-License
--------
+# License
 
 The pgeocode package is distributed under the 3-clause BSD license.
 
+The pgeocode package is maintained by [Symerio](https://www.symerio.com).
 
-Supported countries
--------------------
+# Supported countries
 
-The list of countries available in the GeoNames database, with the corresponding country codes, are given below,
+The list of countries available in the GeoNames database, with the
+corresponding country codes, are given below,
 
-Andorra (AD), Argentina (AR), American Samoa (AS), Austria (AT), Australia (AU), Åland Islands (AX), Azerbaijan (AZ), Bangladesh (BD), Belgium (BE), Bulgaria (BG), Bermuda (BM), Brazil (BR), Belarus (BY), Canada (CA), Switzerland (CH), Chile (CL), Colombia (CO), Costa Rica (CR), Cyprus (CY), Czechia (CZ), Germany (DE), Denmark (DK), Dominican Republic (DO), Algeria (DZ), Estonia (EE), Spain (ES), Finland (FI), Federated States of Micronesia (FM), Faroe Islands (FO), France (FR), United Kingdom of Great Britain and Northern Ireland (GB), French Guiana (GF), Guernsey (GG), Greenland (GL), Guadeloupe (GP), Guatemala (GT), Guam (GU), Croatia (HR), Haiti (HT), Hungary (HU), Ireland (IE), Isle of Man (IM), India (IN), Iceland (IS), Italy (IT), Jersey (JE), Japan (JP), Republic of Korea (KR), Liechtenstein (LI), Sri Lanka (LK), Lithuania (LT), Luxembourg (LU), Latvia (LV), Monaco (MC), Republic of Moldova (MD), Marshall Islands (MH), The former Yugoslav Republic of Macedonia (MK), Northern Mariana Islands (MP), Martinique (MQ), Malta (MT), Malawi (MW), Mexico (MX), Malaysia (MY), New Caledonia (NC), Netherlands (NL), Norway (NO), New Zealand (NZ), Peru (PE), Philippines (PH), Pakistan (PK), Poland (PL), Saint Pierre and Miquelon (PM), Puerto Rico (PR), Portugal (PT), Palau (PW), Réunion (RE), Romania (RO), Serbia (RS), Russian Federation (RU), Sweden (SE), Singapore (SG), Slovenia (SI), Svalbard and Jan Mayen Islands (SJ), Slovakia (SK), San Marino (SM), Thailand (TH), Turkey (TR), Ukraine (UA), United States of America (US), Uruguay (UY), Holy See (VA), United States Virgin Islands (VI), Wallis and Futuna Islands (WF), Mayotte (YT), South Africa (ZA)
+Andorra (AD), Argentina (AR), American Samoa (AS), Austria (AT),
+Australia (AU), Åland Islands (AX), Azerbaijan (AZ), Bangladesh (BD),
+Belgium (BE), Bulgaria (BG), Bermuda (BM), Brazil (BR), Belarus (BY),
+Canada (CA), Switzerland (CH), Chile (CL), Colombia (CO), Costa Rica
+(CR), Cyprus (CY), Czechia (CZ), Germany (DE), Denmark (DK), Dominican
+Republic (DO), Algeria (DZ), Estonia (EE), Spain (ES), Finland (FI),
+Federated States of Micronesia (FM), Faroe Islands (FO), France (FR),
+United Kingdom of Great Britain and Northern Ireland (GB), French Guiana
+(GF), Guernsey (GG), Greenland (GL), Guadeloupe (GP), Guatemala (GT),
+Guam (GU), Croatia (HR), Haiti (HT), Hungary (HU), Ireland (IE), Isle of
+Man (IM), India (IN), Iceland (IS), Italy (IT), Jersey (JE), Japan (JP),
+Republic of Korea (KR), Liechtenstein (LI), Sri Lanka (LK), Lithuania
+(LT), Luxembourg (LU), Latvia (LV), Monaco (MC), Republic of Moldova
+(MD), Marshall Islands (MH), The former Yugoslav Republic of Macedonia
+(MK), Northern Mariana Islands (MP), Martinique (MQ), Malta (MT), Malawi
+(MW), Mexico (MX), Malaysia (MY), New Caledonia (NC), Netherlands (NL),
+Norway (NO), New Zealand (NZ), Peru (PE), Philippines (PH), Pakistan
+(PK), Poland (PL), Saint Pierre and Miquelon (PM), Puerto Rico (PR),
+Portugal (PT), Palau (PW), Réunion (RE), Romania (RO), Serbia (RS),
+Russian Federation (RU), Sweden (SE), Singapore (SG), Slovenia (SI),
+Svalbard and Jan Mayen Islands (SJ), Slovakia (SK), San Marino (SM),
+Thailand (TH), Turkey (TR), Ukraine (UA), United States of America (US),
+Uruguay (UY), Holy See (VA), United States Virgin Islands (VI), Wallis
+and Futuna Islands (WF), Mayotte (YT), South Africa (ZA)
 
-See `GeoNames database <http://download.geonames.org/export/zip/>`_ for more information.
+See [GeoNames database](http://download.geonames.org/export/zip/) for
+more information.
```

### Comparing `pgeocode-0.4.1/pgeocode.egg-info/PKG-INFO` & `pgeocode-0.5.0/pgeocode.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,190 +1,196 @@
 Metadata-Version: 2.1
 Name: pgeocode
-Version: 0.4.1
-Summary: Approximate geocoding
+Version: 0.5.0
+Summary: Postal code geocoding
 Author: Roman Yurchak
 Author-email: roman.yurchak@symerio.com
 License: BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Requires-Python: >=3.8
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: pandas
 Provides-Extra: fuzzy
 Requires-Dist: thefuzz; extra == "fuzzy"
 
-pgeocode
-========
-
-|pypi| |condaforge| |rdfd| |GHactions|
-
-.. |pypi| image:: https://img.shields.io/pypi/v/pgeocode.svg
-   :target: https://pypi.org/project/pgeocode/
-
-.. |condaforge| image:: https://img.shields.io/conda/vn/conda-forge/pgeocode.svg
-   :target: https://anaconda.org/conda-forge/pgeocode
-
-.. |rdfd| image:: https://readthedocs.org/projects/pgeocode/badge/?version=latest
-    :target: http://pgeocode.readthedocs.io/
-
-.. |GHactions| image:: https://github.com/symerio/pgeocode/workflows/Test/badge.svg
-   :target: https://github.com/symerio/pgeocode/actions?query=branch%3Amaster+
+# pgeocode
 
+[![pypi](https://img.shields.io/pypi/v/pgeocode.svg)](https://pypi.org/project/pgeocode/)
+[![rdfd](https://readthedocs.org/projects/pgeocode/badge/?version=latest)](http://pgeocode.readthedocs.io/)
+[![GHactions](https://github.com/symerio/pgeocode/workflows/Test/badge.svg)](https://github.com/symerio/pgeocode/actions?query=branch%3Amaster+)
 
 Postal code geocoding and distance calculations
 
-pgeocode is a Python library for high performance off-line querying of GPS coordinates, region name and municipality name
-from postal codes. Distances between postal codes as well as general
-distance queries are also supported.
-The used `GeoNames <http://download.geonames.org/export/zip/>`_ database includes postal codes for 83 countries.
+pgeocode is a Python library for high performance off-line querying of
+GPS coordinates, region name and municipality name from postal codes.
+Distances between postal codes as well as general distance queries are
+also supported. The used
+[GeoNames](http://download.geonames.org/export/zip/) database includes
+postal codes for 83 countries.
 
 Currently, only queries within the same country are supported.
 
-For additional documentation see `pgeocode.readthedocs.io <https://pgeocode.readthedocs.io>`_.
-
-
-Installation
-------------
-
-pgeocode requires Python 3.8+ as well as ``numpy`` and ``pandas`` packages. It can be installed with,
+For additional documentation see
+[pgeocode.readthedocs.io](https://pgeocode.readthedocs.io).
 
-.. code::
+# Installation
 
-    pip install pgeocode
+pgeocode requires Python 3.10+ as well as `numpy` and `pandas` packages.
+It can be installed with,
 
-or
+```
+pip install pgeocode
+```
 
-.. code::
 
-    conda install -c conda-forge pgeocode
-
-Quickstart
-----------
+# Quickstart
 
 **Postal code queries**
 
-.. code:: python
-
-    >>> import pgeocode
+```python
+>>> import pgeocode
 
-    >>> nomi = pgeocode.Nominatim('fr')
-    >>> nomi.query_postal_code("75013")
-    postal_code               75013
-    country_code                 FR
-    place_name             Paris 13
-    state_name        Île-de-France
-    state_code                   11
-    county_name               Paris
-    county_code                  75
-    community_name            Paris
-    community_code              751
-    latitude                48.8322
-    longitude                2.3561
-    accuracy                      5
-
-    >>> nomi.query_postal_code(["75013", "69006"])
-          postal_code place_name            state_name  latitude  longitude
-    0       75013   Paris 13         Île-de-France   48.8322     2.3561
-    1       69006    Lyon 06  Auvergne-Rhône-Alpes   45.7679     4.8506
+>>> nomi = pgeocode.Nominatim('fr')
+>>> nomi.query_postal_code("75013")
+postal_code               75013
+country_code                 FR
+place_name             Paris 13
+state_name        Île-de-France
+state_code                   11
+county_name               Paris
+county_code                  75
+community_name            Paris
+community_code              751
+latitude                48.8322
+longitude                2.3561
+accuracy                      5
+
+>>> nomi.query_postal_code(["75013", "69006"])
+      postal_code place_name            state_name  latitude  longitude
+0       75013   Paris 13         Île-de-France   48.8322     2.3561
+1       69006    Lyon 06  Auvergne-Rhône-Alpes   45.7679     4.8506
+```
 
 **Place name queries**
 
-.. code:: python
+```python
+>>> import pgeocode
 
-    >>> import pgeocode
-
-    >>> nomi = pgeocode.Nominatim('fr')
-    >>> nomi.query_location("Antibes", top_k=3)
-        country_code  postal_code place_name                  state_name  state_code  ... community_name community_code latitude longitude  accuracy
-    49553           FR        06160    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
-    49787           FR        06600    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
-    49788           FR  06601 CEDEX    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
-
-    >>> nomi.query_location("Straassborg", top_k=3, fuzzy_threshold=80)
-        country_code  postal_code  place_name state_name  state_code  ... community_name community_code latitude longitude  accuracy
-    25461           FR        67000  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
-    25462           FR  67001 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
-    25463           FR  67002 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+>>> nomi = pgeocode.Nominatim('fr')
+>>> nomi.query_location("Antibes", top_k=3)
+    country_code  postal_code place_name                  state_name  state_code  ... community_name community_code latitude longitude  accuracy
+49553           FR        06160    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
+49787           FR        06600    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
+49788           FR  06601 CEDEX    Antibes  Provence-Alpes-Côte d'Azur        93.0  ...         Grasse            061  43.5858    7.1083         5
+
+>>> nomi.query_location("Straassborg", top_k=3, fuzzy_threshold=80)
+    country_code  postal_code  place_name state_name  state_code  ... community_name community_code latitude longitude  accuracy
+25461           FR        67000  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+25462           FR  67001 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+25463           FR  67002 CEDEX  Strasbourg  Grand Est        44.0  ...     Strasbourg            678  48.5839    7.7455         5
+```
 
 **Distance calculations**
 
-.. code:: python
-
-    >>> dist = pgeocode.GeoDistance('fr')
-    >>> dist.query_postal_code("75013", "69006")
-    389.156
-    >>> dist.query_postal_code(["75013", "75014", "75015"], ["69006", "69005", "69004"])
-    array([ 389.15648697,  390.12577967,  390.49857655])
-
-
-Geocoding format
-----------------
-
-The result of a geo-localistion query is a ``pandas.DataFrame`` with the following columns,
-
-* ``country_code``: iso country code, 2 characters
-* ``postal_code`` : postal code
-* ``place_name``  : place name (e.g. town, city etc)
-* ``state_name`` : 1. order subdivision (state)
-* ``state_code`` : 1. order subdivision (state)
-* ``county_name`` : 2. order subdivision (county/province)
-* ``county_code`` : 2. order subdivision (county/province)
-* ``community_name`` : 3. order subdivision (community)
-* ``community_code`` : 3. order subdivision (community)
-* ``latitude``    : estimated latitude (wgs84)
-* ``longitude``   : estimated longitude (wgs84)
-* ``accuracy``    : accuracy of lat/lng from 1=estimated to 6=centroid
+```python
+>>> dist = pgeocode.GeoDistance('fr')
+>>> dist.query_postal_code("75013", "69006")
+389.156
+>>> dist.query_postal_code(["75013", "75014", "75015"], ["69006", "69005", "69004"])
+array([ 389.15648697,  390.12577967,  390.49857655])
+```
+
+# Geocoding format
+
+The result of a geo-localistion query is a `pandas.DataFrame` with the
+following columns,
+
+-   `country_code`: iso country code, 2 characters
+-   `postal_code` : postal code
+-   `place_name` : place name (e.g. town, city etc)
+-   `state_name` : 1. order subdivision (state)
+-   `state_code` : 1. order subdivision (state)
+-   `county_name` : 2. order subdivision (county/province)
+-   `county_code` : 2. order subdivision (county/province)
+-   `community_name` : 3. order subdivision (community)
+-   `community_code` : 3. order subdivision (community)
+-   `latitude` : estimated latitude (wgs84)
+-   `longitude` : estimated longitude (wgs84)
+-   `accuracy` : accuracy of lat/lng from 1=estimated to 6=centroid
 
-
-Configuration and defaults
---------------------------
+# Configuration and defaults
 
 **Storage directory**
 
-Defaults to ``~/.cache/pgeocode``, it is the directory where data is downloaded
-for later consumption. It can be changed using the environment variable
-``PGEOCODE_DATA_DIR``, i.e. ``export PGEOCODE_DATA_DIR=/tmp/pgeocode_data``.
+Defaults to `~/.cache/pgeocode`, it is the directory where data is
+downloaded for later consumption. It can be changed using the
+environment variable `PGEOCODE_DATA_DIR`, i.e.
+`export PGEOCODE_DATA_DIR=/tmp/pgeocode_data`.
 
 **Data sources**
 
-Data sources are provided as a list in the ``pgeocode.DOWNLOAD_URL`` variable.
-The default value is,
-
-.. code:: python
+Data sources are provided as a list in the `pgeocode.DOWNLOAD_URL`
+variable. The default value is,
 
-    DOWNLOAD_URL = [
-        "https://download.geonames.org/export/zip/{country}.zip",
-        "https://symerio.github.io/postal-codes-data/data/geonames/{country}.txt",
-    ]
-
-Data sources are tried from first to last until one works. Here the second link is a mirror
-of the first.
-
-It is also possible to extend this variable with third party data sources, as
-long as they follow the same format. See for instance
-`postal-codes-data <https://github.com/symerio/postal-codes-data/tree/master/data/geonames>`_
+``` python
+DOWNLOAD_URL = [
+    "https://download.geonames.org/export/zip/{country}.zip",
+    "https://symerio.github.io/postal-codes-data/data/geonames/{country}.txt",
+]
+```
+
+Data sources are tried from first to last until one works. Here the
+second link is a mirror of the first.
+
+It is also possible to extend this variable with third party data
+sources, as long as they follow the same format. See for instance
+[postal-codes-data](https://github.com/symerio/postal-codes-data/tree/master/data/geonames)
 repository for examples of data files.
 
-
-License
--------
+# License
 
 The pgeocode package is distributed under the 3-clause BSD license.
 
+The pgeocode package is maintained by [Symerio](https://www.symerio.com).
 
-Supported countries
--------------------
+# Supported countries
 
-The list of countries available in the GeoNames database, with the corresponding country codes, are given below,
+The list of countries available in the GeoNames database, with the
+corresponding country codes, are given below,
 
-Andorra (AD), Argentina (AR), American Samoa (AS), Austria (AT), Australia (AU), Åland Islands (AX), Azerbaijan (AZ), Bangladesh (BD), Belgium (BE), Bulgaria (BG), Bermuda (BM), Brazil (BR), Belarus (BY), Canada (CA), Switzerland (CH), Chile (CL), Colombia (CO), Costa Rica (CR), Cyprus (CY), Czechia (CZ), Germany (DE), Denmark (DK), Dominican Republic (DO), Algeria (DZ), Estonia (EE), Spain (ES), Finland (FI), Federated States of Micronesia (FM), Faroe Islands (FO), France (FR), United Kingdom of Great Britain and Northern Ireland (GB), French Guiana (GF), Guernsey (GG), Greenland (GL), Guadeloupe (GP), Guatemala (GT), Guam (GU), Croatia (HR), Haiti (HT), Hungary (HU), Ireland (IE), Isle of Man (IM), India (IN), Iceland (IS), Italy (IT), Jersey (JE), Japan (JP), Republic of Korea (KR), Liechtenstein (LI), Sri Lanka (LK), Lithuania (LT), Luxembourg (LU), Latvia (LV), Monaco (MC), Republic of Moldova (MD), Marshall Islands (MH), The former Yugoslav Republic of Macedonia (MK), Northern Mariana Islands (MP), Martinique (MQ), Malta (MT), Malawi (MW), Mexico (MX), Malaysia (MY), New Caledonia (NC), Netherlands (NL), Norway (NO), New Zealand (NZ), Peru (PE), Philippines (PH), Pakistan (PK), Poland (PL), Saint Pierre and Miquelon (PM), Puerto Rico (PR), Portugal (PT), Palau (PW), Réunion (RE), Romania (RO), Serbia (RS), Russian Federation (RU), Sweden (SE), Singapore (SG), Slovenia (SI), Svalbard and Jan Mayen Islands (SJ), Slovakia (SK), San Marino (SM), Thailand (TH), Turkey (TR), Ukraine (UA), United States of America (US), Uruguay (UY), Holy See (VA), United States Virgin Islands (VI), Wallis and Futuna Islands (WF), Mayotte (YT), South Africa (ZA)
+Andorra (AD), Argentina (AR), American Samoa (AS), Austria (AT),
+Australia (AU), Åland Islands (AX), Azerbaijan (AZ), Bangladesh (BD),
+Belgium (BE), Bulgaria (BG), Bermuda (BM), Brazil (BR), Belarus (BY),
+Canada (CA), Switzerland (CH), Chile (CL), Colombia (CO), Costa Rica
+(CR), Cyprus (CY), Czechia (CZ), Germany (DE), Denmark (DK), Dominican
+Republic (DO), Algeria (DZ), Estonia (EE), Spain (ES), Finland (FI),
+Federated States of Micronesia (FM), Faroe Islands (FO), France (FR),
+United Kingdom of Great Britain and Northern Ireland (GB), French Guiana
+(GF), Guernsey (GG), Greenland (GL), Guadeloupe (GP), Guatemala (GT),
+Guam (GU), Croatia (HR), Haiti (HT), Hungary (HU), Ireland (IE), Isle of
+Man (IM), India (IN), Iceland (IS), Italy (IT), Jersey (JE), Japan (JP),
+Republic of Korea (KR), Liechtenstein (LI), Sri Lanka (LK), Lithuania
+(LT), Luxembourg (LU), Latvia (LV), Monaco (MC), Republic of Moldova
+(MD), Marshall Islands (MH), The former Yugoslav Republic of Macedonia
+(MK), Northern Mariana Islands (MP), Martinique (MQ), Malta (MT), Malawi
+(MW), Mexico (MX), Malaysia (MY), New Caledonia (NC), Netherlands (NL),
+Norway (NO), New Zealand (NZ), Peru (PE), Philippines (PH), Pakistan
+(PK), Poland (PL), Saint Pierre and Miquelon (PM), Puerto Rico (PR),
+Portugal (PT), Palau (PW), Réunion (RE), Romania (RO), Serbia (RS),
+Russian Federation (RU), Sweden (SE), Singapore (SG), Slovenia (SI),
+Svalbard and Jan Mayen Islands (SJ), Slovakia (SK), San Marino (SM),
+Thailand (TH), Turkey (TR), Ukraine (UA), United States of America (US),
+Uruguay (UY), Holy See (VA), United States Virgin Islands (VI), Wallis
+and Futuna Islands (WF), Mayotte (YT), South Africa (ZA)
 
-See `GeoNames database <http://download.geonames.org/export/zip/>`_ for more information.
+See [GeoNames database](http://download.geonames.org/export/zip/) for
+more information.
```

### Comparing `pgeocode-0.4.1/pgeocode.py` & `pgeocode-0.5.0/pgeocode.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 # Authors: Roman Yurchak <roman.yurchak@symerio.com>
 
 import contextlib
 import os
 import urllib.request
 import warnings
 from io import BytesIO
-from typing import Any, Tuple, List, Optional
+from typing import Any
 from zipfile import ZipFile
 
 import numpy as np
 import pandas as pd
 
-__version__ = "0.4.1"
+__version__ = "0.5.0"
 
 STORAGE_DIR = os.environ.get(
     "PGEOCODE_DATA_DIR",
     os.path.join(os.path.expanduser("~"), ".cache", "pgeocode"),
 )
 
 # A list of download locations. If the first URL fails, following ones will
@@ -178,15 +178,15 @@
                     with fh_zip.open(country.upper() + ".txt") as fh:
                         yield fh
             else:
                 yield reader
 
 
 @contextlib.contextmanager
-def _open_extract_cycle_url(urls: List[str], country: str) -> Any:
+def _open_extract_cycle_url(urls: list[str], country: str) -> Any:
     """Same as _open_extract_url but cycle through URLs until one works
 
     We start by opening the first URL in the list, and if fails
     move to the next, until one works or the end of list is reached.
     """
     if not isinstance(urls, list) or not len(urls):
         raise ValueError(f"urls={urls} must be a list with at least one URL")
@@ -222,19 +222,17 @@
         into a single entry
     """
 
     def __init__(self, country: str = "fr", unique: bool = True):
         country = country.upper()
         if country not in COUNTRIES_VALID:
             raise ValueError(
-                (
-                    "country={} is not a known country code. "
-                    "See the README for a list of supported "
-                    "countries"
-                ).format(country)
+                f"country={country} is not a known country code. "
+                "See the README for a list of supported "
+                "countries"
             )
         if country == "AR":
             warnings.warn(
                 "The Argentina data file contains 4-digit postal "
                 "codes which were replaced with a new system "
                 "in 1999."
             )
@@ -243,29 +241,27 @@
         if unique:
             self._data_frame = self._index_postal_codes()
         else:
             self._data_frame = self._data
         self.unique = unique
 
     @staticmethod
-    def _get_data(country: str) -> Tuple[str, pd.DataFrame]:
+    def _get_data(country: str) -> tuple[str, pd.DataFrame]:
         """Load the data from disk; otherwise download and save it"""
 
         data_path = os.path.join(STORAGE_DIR, country.upper() + ".txt")
         if os.path.exists(data_path):
             data = pd.read_csv(
                 data_path,
                 dtype={"postal_code": str},
                 na_values=NA_VALUES,
                 keep_default_na=False,
             )
         else:
-            download_urls = [
-                val.format(country=country) for val in DOWNLOAD_URL
-            ]
+            download_urls = [val.format(country=country) for val in DOWNLOAD_URL]
             with _open_extract_cycle_url(download_urls, country) as fh:
                 data = pd.read_csv(
                     fh,
                     sep="\t",
                     header=None,
                     names=DATA_FIELDS,
                     dtype={"postal_code": str},
@@ -340,26 +336,24 @@
         else:
             single_entry = False
 
         if not isinstance(codes, pd.DataFrame):
             codes = pd.DataFrame(codes, columns=["postal_code"])
 
         codes = self._normalize_postal_code(codes)
-        response = pd.merge(
-            codes, self._data_frame, on="postal_code", how="left"
-        )
+        response = pd.merge(codes, self._data_frame, on="postal_code", how="left")
         if self.unique and single_entry:
             response = response.iloc[0]
         return response
 
     def query_location(
         self,
         name: str,
         top_k: int = 100,
-        fuzzy_threshold: Optional[int] = None,
+        fuzzy_threshold: int | None = None,
         col: str = "place_name",
     ) -> pd.DataFrame:
         """Get location information from a place name
 
         Parameters
         ----------
         name: str
@@ -383,43 +377,37 @@
           names (or empty if no match was found)
         """
         contains_matches = self._str_contains_search(name, col)
         if len(contains_matches) > 0:
             return contains_matches.iloc[:top_k]
 
         if fuzzy_threshold is not None:
-            fuzzy_matches = self._fuzzy_search(
-                name, col, threshold=fuzzy_threshold
-            )
+            fuzzy_matches = self._fuzzy_search(name, col, threshold=fuzzy_threshold)
             if len(fuzzy_matches) > 0:
                 return fuzzy_matches.iloc[:top_k]
 
         return pd.DataFrame(columns=self._data.columns)
 
     def _str_contains_search(self, text: str, col: str) -> pd.DataFrame:
         match_mask = self._data[col].str.lower().str.contains(text.lower())
         match_mask.fillna(False, inplace=True)
         return self._data[match_mask]
 
-    def _fuzzy_search(
-        self, text: str, col: str, threshold: float = 80
-    ) -> pd.DataFrame:
+    def _fuzzy_search(self, text: str, col: str, threshold: float = 80) -> pd.DataFrame:
         try:
             # thefuzz is not required to install pgeocode,
             # it is an optional dependency for enabling fuzzy search
             from thefuzz import fuzz
         except ModuleNotFoundError as err:
             raise ModuleNotFoundError(
                 "Cannot use fuzzy search without 'thefuzz' package. "
                 "It can be installed with: pip install thefuzz[speedup]"
             ) from err
 
-        fuzzy_scores = self._data[col].apply(
-            lambda x: fuzz.ratio(str(x), text)
-        )
+        fuzzy_scores = self._data[col].apply(lambda x: fuzz.ratio(str(x), text))
         return self._data[fuzzy_scores >= threshold]
 
 
 class GeoDistance(Nominatim):
     """Distance calculation from a city name or a postal code
 
     Parameters
```

### Comparing `pgeocode-0.4.1/setup.py` & `pgeocode-0.5.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import io
 import os
 import re
 
 from setuptools import setup
 
 
 # https://packaging.python.org/guides/single-sourcing-package-version/
@@ -12,17 +11,15 @@
         encoding=kwargs.get("encoding", "utf8"),
     ) as fp:
         return fp.read()
 
 
 def find_version(*file_paths):
     version_file = read(*file_paths)
-    version_match = re.search(
-        r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M
-    )
+    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
     if version_match:
         return version_match.group(1)
 
 
 CLASSIFIERS = """\
 Intended Audience :: Science/Research
 Intended Audience :: Developers
@@ -33,21 +30,22 @@
 Operating System :: POSIX
 Operating System :: Unix
 
 """
 
 setup(
     name="pgeocode",
-    description="Approximate geocoding",
-    long_description=open("README.rst").read(),
+    description="Postal code geocoding",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
     version=find_version("pgeocode.py"),
     author="Roman Yurchak",
     author_email="roman.yurchak@symerio.com",
     py_modules=["pgeocode"],
-    python_requires=">=3.8",
+    python_requires=">=3.10",
     install_requires=["requests", "numpy", "pandas"],
     extras_require={
         "fuzzy": ["thefuzz"],
     },
     classifiers=[_f for _f in CLASSIFIERS.split("\n") if _f],
     license="BSD",
 )
```

