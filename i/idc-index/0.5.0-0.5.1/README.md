# Comparing `tmp/idc_index-0.5.0.tar.gz` & `tmp/idc_index-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Apr 11 03:00:31 2024, max compression
+gzip compressed data, last modified: Sat Apr 13 01:32:19 2024, max compression
```

## Comparing `idc_index-0.5.0.tar` & `idc_index-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0      125 2024-04-11 03:00:31.000000 idc_index-0.5.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-11 03:00:31.000000 idc_index-0.5.0/.gitattributes
--rw-r--r--   0        0        0     2357 2024-04-11 03:00:31.000000 idc_index-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-11 03:00:31.000000 idc_index-0.5.0/.readthedocs.yaml
--rw-r--r--   0        0        0     2742 2024-04-11 03:00:31.000000 idc_index-0.5.0/noxfile.py
--rw-r--r--   0        0        0     2394 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0      847 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1581 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      355 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/workflows/keep-alive.yaml
--rw-r--r--   0        0        0      851 2024-04-11 03:00:31.000000 idc_index-0.5.0/docs/conf.py
--rw-r--r--   0        0        0      196 2024-04-11 03:00:31.000000 idc_index-0.5.0/docs/index.md
--rw-r--r--   0        0        0      263 2024-04-11 03:00:31.000000 idc_index-0.5.0/idc_index/__init__.py
--rw-r--r--   0        0        0      411 2024-04-11 03:00:31.000000 idc_index-0.5.0/idc_index/_version.py
--rw-r--r--   0        0        0      118 2024-04-11 03:00:31.000000 idc_index-0.5.0/idc_index/_version.pyi
--rw-r--r--   0        0        0    25127 2024-04-11 03:00:31.000000 idc_index-0.5.0/idc_index/index.py
--rw-r--r--   0        0        0        0 2024-04-11 03:00:31.000000 idc_index-0.5.0/idc_index/py.typed
--rw-r--r--   0        0        0     1383 2024-04-11 03:00:31.000000 idc_index-0.5.0/queries/idc_index.sql
--rw-r--r--   0        0        0        0 2024-04-11 03:00:31.000000 idc_index-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     3779 2024-04-11 03:00:31.000000 idc_index-0.5.0/tests/idcindex.py
--rw-r--r--   0        0        0      413 2024-04-11 03:00:31.000000 idc_index-0.5.0/tests/study_manifest_aws.s5cmd
--rw-r--r--   0        0        0      437 2024-04-11 03:00:31.000000 idc_index-0.5.0/tests/study_manifest_gcs.s5cmd
--rw-r--r--   0        0        0      175 2024-04-11 03:00:31.000000 idc_index-0.5.0/tests/test_package.py
--rw-r--r--   0        0        0     2265 2024-04-11 03:00:31.000000 idc_index-0.5.0/.gitignore
--rw-r--r--   0        0        0     1077 2024-04-11 03:00:31.000000 idc_index-0.5.0/LICENSE
--rw-r--r--   0        0        0     4290 2024-04-11 03:00:31.000000 idc_index-0.5.0/README.md
--rw-r--r--   0        0        0     6173 2024-04-11 03:00:31.000000 idc_index-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7617 2024-04-11 03:00:31.000000 idc_index-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-04-13 01:32:19.000000 idc_index-0.5.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-13 01:32:19.000000 idc_index-0.5.1/.gitattributes
+-rw-r--r--   0        0        0     2357 2024-04-13 01:32:19.000000 idc_index-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-13 01:32:19.000000 idc_index-0.5.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2024-04-13 01:32:19.000000 idc_index-0.5.1/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      847 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1581 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      355 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/workflows/keep-alive.yaml
+-rw-r--r--   0        0        0      851 2024-04-13 01:32:19.000000 idc_index-0.5.1/docs/conf.py
+-rw-r--r--   0        0        0      196 2024-04-13 01:32:19.000000 idc_index-0.5.1/docs/index.md
+-rw-r--r--   0        0        0      263 2024-04-13 01:32:19.000000 idc_index-0.5.1/idc_index/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-13 01:32:19.000000 idc_index-0.5.1/idc_index/_version.py
+-rw-r--r--   0        0        0      118 2024-04-13 01:32:19.000000 idc_index-0.5.1/idc_index/_version.pyi
+-rw-r--r--   0        0        0    27954 2024-04-13 01:32:19.000000 idc_index-0.5.1/idc_index/index.py
+-rw-r--r--   0        0        0        0 2024-04-13 01:32:19.000000 idc_index-0.5.1/idc_index/py.typed
+-rw-r--r--   0        0        0        0 2024-04-13 01:32:19.000000 idc_index-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     3779 2024-04-13 01:32:19.000000 idc_index-0.5.1/tests/idcindex.py
+-rw-r--r--   0        0        0      413 2024-04-13 01:32:19.000000 idc_index-0.5.1/tests/study_manifest_aws.s5cmd
+-rw-r--r--   0        0        0      437 2024-04-13 01:32:19.000000 idc_index-0.5.1/tests/study_manifest_gcs.s5cmd
+-rw-r--r--   0        0        0      175 2024-04-13 01:32:19.000000 idc_index-0.5.1/tests/test_package.py
+-rw-r--r--   0        0        0     2265 2024-04-13 01:32:19.000000 idc_index-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1077 2024-04-13 01:32:19.000000 idc_index-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4290 2024-04-13 01:32:19.000000 idc_index-0.5.1/README.md
+-rw-r--r--   0        0        0     6121 2024-04-13 01:32:19.000000 idc_index-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7531 2024-04-13 01:32:19.000000 idc_index-0.5.1/PKG-INFO
```

### Comparing `idc_index-0.5.0/.pre-commit-config.yaml` & `idc_index-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.0/noxfile.py` & `idc_index-0.5.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.0/.github/CONTRIBUTING.md` & `idc_index-0.5.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.0/.github/matchers/pylint.json` & `idc_index-0.5.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.0/.github/workflows/cd.yml` & `idc_index-0.5.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.0/.github/workflows/ci.yml` & `idc_index-0.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.0/docs/conf.py` & `idc_index-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.0/idc_index/index.py` & `idc_index-0.5.1/idc_index/index.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from __future__ import annotations
 
 import logging
 import os
 import re
 import shutil
 import subprocess
-import sys
 import tempfile
-
-if sys.version_info < (3, 10):
-    from importlib_metadata import distribution
-else:
-    from importlib.metadata import distribution
+from importlib.metadata import distribution
 
 import duckdb
 import idc_index_data
 import pandas as pd
 import psutil
 from packaging.version import Version
 
@@ -63,15 +58,19 @@
         subprocess.check_call([self.s5cmdPath, "--help"], stdout=subprocess.DEVNULL)
 
     @staticmethod
     def _filter_dataframe_by_id(key, dataframe, _id):
         values = _id
         if isinstance(_id, str):
             values = [_id]
-        return dataframe[dataframe[key].isin(values)].copy()
+        filtered_df = dataframe[dataframe[key].isin(values)].copy()
+        if filtered_df.empty:
+            error_message = f"No data found for the {key} with the values {values}."
+            raise ValueError(error_message)
+        return filtered_df
 
     @staticmethod
     def _filter_by_collection_id(df_index, collection_id):
         return IDCClient._filter_dataframe_by_id(
             "collection_id", df_index, collection_id
         )
 
@@ -89,28 +88,57 @@
     def _filter_by_dicom_series_uid(df_index, dicom_series_uid):
         return IDCClient._filter_dataframe_by_id(
             "SeriesInstanceUID", df_index, dicom_series_uid
         )
 
     @staticmethod
     def get_idc_version():
+        """
+        Returns the version of IDC data used in idc-index
+        """
         idc_version = Version(idc_index_data.__version__).major
         return f"v{idc_version}"
 
     def get_collections(self):
+        """
+        Returns the collections present in IDC
+        """
         unique_collections = self.index["collection_id"].unique()
         return unique_collections.tolist()
 
     def get_series_size(self, seriesInstanceUID):
+        """
+        Gets cumulative size (MB) of the DICOM instances in a given SeriesInstanceUID.
+        Args:
+            seriesInstanceUID (str): The DICOM SeriesInstanceUID.
+        Returns:
+            float: The cumulative size of the DICOM instances in the given SeriesInstanceUID rounded to two digits, in MB.
+        Raises:
+            ValueError: If the `seriesInstanceUID` does not exist.
+        """
+
         resp = self.index[["SeriesInstanceUID"] == seriesInstanceUID][
             "series_size_MB"
         ].iloc[0]
         return resp
 
     def get_patients(self, collection_id, outputFormat="dict"):
+        """
+        Gets the patients in a collection.
+        Args:
+            collection_id (str or a list of str): The collection id or list of collection ids. This should be in lower case separated by underscores.
+                                For example, 'pdmr_texture_analysis'. or ['pdmr_texture_analysis','nlst']
+            outputFormat (str, optional): The format in which to return the patient IDs. Available options are 'dict',
+                                        'df', and 'list'. Default is 'dict'.
+        Returns:
+            dict or pandas.DataFrame or list: Patient IDs in the requested output format. By default, it returns a dictionary.
+        Raises:
+            ValueError: If `outputFormat` is not one of 'dict', 'df', 'list'.
+        """
+
         if not isinstance(collection_id, str) and not isinstance(collection_id, list):
             raise TypeError("collection_id must be a string or list of strings")
 
         if outputFormat not in ["dict", "df", "list"]:
             raise ValueError("outputFormat must be either 'dict', 'df', or 'list")
 
         patient_df = self._filter_by_collection_id(self.index, collection_id)
@@ -139,15 +167,26 @@
                 response = patient_df
 
         logger.debug("Get patient response: %s", str(response))
 
         return response
 
     def get_dicom_studies(self, patientId, outputFormat="dict"):
-        """returns one row per distinct value of StudyInstanceUID"""
+        """
+        Returns Studies for a given patient or list of patients.
+        Args:
+            patientId (str or list of str): The patient Id or a list of patient Ids.
+            outputFormat (str, optional): The format in which to return the studies. Available options are 'dict',
+                                        'df', and 'list'. Default is 'dict'.
+        Returns:
+            dict or pandas.DataFrame or list: Studies in the requested output format. By default, it returns a dictionary.
+        Raises:
+            ValueError: If `outputFormat` is not one of 'dict', 'df', 'list'.
+            ValueError: If any of the `patientId` does not exist.
+        """
 
         if not isinstance(patientId, str) and not isinstance(patientId, list):
             raise TypeError("patientId must be a string or list of strings")
 
         if outputFormat not in ["dict", "df", "list"]:
             raise ValueError("outputFormat must be either 'dict' or 'df' or 'list'")
 
@@ -201,15 +240,28 @@
             else:
                 response = studies_df
 
         logger.debug("Get patient study response: %s", str(response))
 
         return response
 
-    def get_dicom_series(self, studyInstanceUID=None, outputFormat="dict"):
+    def get_dicom_series(self, studyInstanceUID, outputFormat="dict"):
+        """
+        Returns Series for a given study or list of studies.
+        Args:
+            studyInstanceUID (str or list of str): The DICOM StudyInstanceUID or a list of StudyInstanceUIDs.
+            outputFormat (str, optional): The format in which to return the series. Available options are 'dict',
+                                        'df', and 'list'. Default is 'dict'.
+        Returns:
+            dict or pandas.DataFrame or list: Series in the requested output format. By default, it returns a dictionary.
+        Raises:
+            ValueError: If `outputFormat` is not one of 'dict', 'df', 'list'.
+            ValueError: If any of the `studyInstanceUID` does not exist.
+        """
+
         if not isinstance(studyInstanceUID, str) and not isinstance(
             studyInstanceUID, list
         ):
             raise TypeError("studyInstanceUID must be a string or list of strings")
 
         if outputFormat not in ["dict", "df", "list"]:
             raise ValueError("outputFormat must be either 'dict' or 'df' or 'list'")
@@ -340,60 +392,63 @@
         # Parse the output to get the file names
         lines = output.split("\n")
         file_names = [s3_url + line.split()[-1] for line in lines if line]
 
         return file_names
 
     def get_viewer_URL(
-        self, seriesInstanceUID, studyInstanceUID=None, viewer_selector=None
+        self, seriesInstanceUID=None, studyInstanceUID=None, viewer_selector=None
     ):
         """
         Get the URL of the IDC viewer for the given series or study in IDC based on
         the provided SeriesInstanceUID or StudyInstanceUID. If StudyInstanceUID is not provided,
         it will be automatically deduced. If viewer_selector is not provided, default viewers
-        will be used (OHIF v2 for radiology modalities, and Slim for SM).
+        will be used (OHIF v2 or v3 for radiology modalities, and Slim for SM).
 
         This function will validate the provided SeriesInstanceUID or StudyInstanceUID against IDC
         index to ensure that the series or study is available in IDC.
 
         Args:
             SeriesInstanceUID: string containing the value of DICOM SeriesInstanceUID for a series
             available in IDC
 
             StudyInstanceUID: string containing the value of DICOM SeriesInstanceUID for a series
             available in IDC
 
             viewer_selector: string containing the name of the viewer to use. Must be one of the following:
-            ohif_v2, ohif_v2, or slim. If not provided, default viewers will be used.
+            ohif_v2, ohif_v3 or slim. If not provided, default viewers will be used.
 
         Returns:
             string containing the IDC viewer URL for the given SeriesInstanceUID
         """
 
         if seriesInstanceUID is None and studyInstanceUID is None:
             raise ValueError(
                 "Either SeriesInstanceUID or StudyInstanceUID, or both, must be provided."
             )
 
-        if seriesInstanceUID not in self.index["SeriesInstanceUID"].values:
+        if (
+            seriesInstanceUID is not None
+            and seriesInstanceUID not in self.index["SeriesInstanceUID"].values
+        ):
             raise ValueError("SeriesInstanceUID not found in IDC index.")
 
         if (
             studyInstanceUID is not None
             and studyInstanceUID not in self.index["StudyInstanceUID"].values
         ):
             raise ValueError("StudyInstanceUID not found in IDC index.")
 
         if viewer_selector is not None and viewer_selector not in [
             "ohif_v2",
             "ohif_v3",
             "slim",
         ]:
             raise ValueError(
-                "viewer_selector must be one of 'ohif_v2', 'ohif_v3' or 'slim'."
+                "viewer_selector must be one of 'ohif_v2', 'ohif_v3',  or 'slim'."
             )
 
         modality = None
 
         if studyInstanceUID is None:
             query = f"""
             SELECT
```

### Comparing `idc_index-0.5.0/tests/idcindex.py` & `idc_index-0.5.1/tests/idcindex.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,16 +66,16 @@
             outputFormat="list",
         )
 
         self.assertIsNotNone(series)
 
         series = self.client.get_dicom_series(
             studyInstanceUID=[
-                "1.3.6.1.4.1.14519.5.2.1.6279.6001.141365756818074696859567662357",
-                "1.3.6.1.4.1.14519.5.2.1.6279.6001.239368516910061467349404750170",
+                "1.3.6.1.4.1.14519.5.2.1.1239.1759.691327824408089993476361149761",
+                "1.3.6.1.4.1.14519.5.2.1.1239.1759.272272273744698671736205545239",
             ],
             outputFormat="list",
         )
 
         self.assertIsNotNone(series)
 
     def test_download_dicom_series(self):
```

### Comparing `idc_index-0.5.0/.gitignore` & `idc_index-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.0/LICENSE` & `idc_index-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.0/README.md` & `idc_index-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.0/pyproject.toml` & `idc_index-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
   "psutil",
   "pyarrow",
   "s5cmd",
 ]
 
 [project.optional-dependencies]
 test = [
-  "importlib_metadata>=2.0; python_version<'3.10'",
   "pytest >=6",
   "pytest-cov >=3",
 ]
 dev = [
   "pytest >=6",
   "pytest-cov >=3",
 ]
```

### Comparing `idc_index-0.5.0/PKG-INFO` & `idc_index-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idc-index
-Version: 0.5.0
+Version: 0.5.1
 Summary: Package to query and download data from an index of ImagingDataCommons
 Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
 Project-URL: Bug Tracker, https://github.com/ImagingDataCommons/idc-index/issues
 Project-URL: Discussions, https://discourse.canceridc.dev/
 Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
 Author-email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
 License: MIT License
@@ -58,15 +58,14 @@
 Provides-Extra: docs
 Requires-Dist: furo>=2023.08.17; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx>=7.0; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: importlib-metadata>=2.0; (python_version < '3.10') and extra == 'test'
 Requires-Dist: pytest-cov>=3; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
 # idc-index
 
 [![Actions Status][actions-badge]][actions-link]
```

