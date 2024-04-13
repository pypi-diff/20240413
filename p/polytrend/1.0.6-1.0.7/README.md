# Comparing `tmp/polytrend-1.0.6.tar.gz` & `tmp/polytrend-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polytrend-1.0.6.tar", last modified: Thu Apr 11 21:13:48 2024, max compression
+gzip compressed data, was "polytrend-1.0.7.tar", last modified: Sat Apr 13 10:55:03 2024, max compression
```

## Comparing `polytrend-1.0.6.tar` & `polytrend-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 21:13:48.035953 polytrend-1.0.6/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.6/LICENSE
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3458 2024-04-11 21:13:48.035953 polytrend-1.0.6/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.6/README.md
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      963 2024-04-11 21:12:19.000000 polytrend-1.0.6/pyproject.toml
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 21:13:48.035953 polytrend-1.0.6/setup.cfg
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 21:08:44.000000 polytrend-1.0.6/setup.py
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 21:13:48.025953 polytrend-1.0.6/src/
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 21:13:48.025953 polytrend-1.0.6/src/polytrend/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      694 2024-04-11 20:21:39.000000 polytrend-1.0.6/src/polytrend/__init__.py
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    10445 2024-04-11 20:20:38.000000 polytrend-1.0.6/src/polytrend/polytrend.py
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 21:13:48.035953 polytrend-1.0.6/src/polytrend.egg-info/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3458 2024-04-11 21:13:48.000000 polytrend-1.0.6/src/polytrend.egg-info/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      278 2024-04-11 21:13:48.000000 polytrend-1.0.6/src/polytrend.egg-info/SOURCES.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 21:13:48.000000 polytrend-1.0.6/src/polytrend.egg-info/dependency_links.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      141 2024-04-11 21:13:48.000000 polytrend-1.0.6/src/polytrend.egg-info/requires.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       10 2024-04-11 21:13:48.000000 polytrend-1.0.6/src/polytrend.egg-info/top_level.txt
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 10:55:03.470687 polytrend-1.0.7/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.7/LICENSE
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3458 2024-04-13 10:55:03.470687 polytrend-1.0.7/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.7/README.md
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      963 2024-04-13 10:54:26.000000 polytrend-1.0.7/pyproject.toml
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-13 10:55:03.470687 polytrend-1.0.7/setup.cfg
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 21:08:44.000000 polytrend-1.0.7/setup.py
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 10:55:03.470687 polytrend-1.0.7/src/
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 10:55:03.470687 polytrend-1.0.7/src/polytrend/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      780 2024-04-13 10:52:00.000000 polytrend-1.0.7/src/polytrend/__init__.py
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    10445 2024-04-11 20:20:38.000000 polytrend-1.0.7/src/polytrend/polytrend.py
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 10:55:03.470687 polytrend-1.0.7/src/polytrend.egg-info/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3458 2024-04-13 10:55:03.000000 polytrend-1.0.7/src/polytrend.egg-info/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      278 2024-04-13 10:55:03.000000 polytrend-1.0.7/src/polytrend.egg-info/SOURCES.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-13 10:55:03.000000 polytrend-1.0.7/src/polytrend.egg-info/dependency_links.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      141 2024-04-13 10:55:03.000000 polytrend-1.0.7/src/polytrend.egg-info/requires.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       10 2024-04-13 10:55:03.000000 polytrend-1.0.7/src/polytrend.egg-info/top_level.txt
```

### Comparing `polytrend-1.0.6/LICENSE` & `polytrend-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.6/PKG-INFO` & `polytrend-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.6
+Version: 1.0.7
 Summary: PolyTrend is a regression tool that fits polynomial curves to noisy data.
 Author-email: Emmanuel Asiimwe <asiimwemmanuel47@gmail.com>
 Project-URL: Homepage, https://github.com/asiimwemmanuel/polytrend
 Project-URL: Issues, https://github.com/asiimwemmanuel/polytrend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `polytrend-1.0.6/README.md` & `polytrend-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.6/pyproject.toml` & `polytrend-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "polytrend"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Emmanuel Asiimwe", email="asiimwemmanuel47@gmail.com" },
 ]
 description = "PolyTrend is a regression tool that fits polynomial curves to noisy data."
 readme = "README.md"
 requires-python = ">= 3.11.8"
 dependencies = [
```

### Comparing `polytrend-1.0.6/src/polytrend/__init__.py` & `polytrend-1.0.7/src/polytrend/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,7 +10,10 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with PolyTrend. If not, see <https://www.gnu.org/licenses/>.
 
 from .polytrend import PolyTrend
+
+# Define what gets imported when someone imports the package
+__all__ = ['PolyTrend']
```

### Comparing `polytrend-1.0.6/src/polytrend/polytrend.py` & `polytrend-1.0.7/src/polytrend/polytrend.py`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.6/src/polytrend.egg-info/PKG-INFO` & `polytrend-1.0.7/src/polytrend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.6
+Version: 1.0.7
 Summary: PolyTrend is a regression tool that fits polynomial curves to noisy data.
 Author-email: Emmanuel Asiimwe <asiimwemmanuel47@gmail.com>
 Project-URL: Homepage, https://github.com/asiimwemmanuel/polytrend
 Project-URL: Issues, https://github.com/asiimwemmanuel/polytrend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

