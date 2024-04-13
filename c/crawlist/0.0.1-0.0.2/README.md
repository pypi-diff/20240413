# Comparing `tmp/crawlist-0.0.1.tar.gz` & `tmp/crawlist-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlist-0.0.1.tar", last modified: Tue Apr  9 06:32:32 2024, max compression
+gzip compressed data, was "crawlist-0.0.2.tar", last modified: Fri Apr 12 09:23:31 2024, max compression
```

## Comparing `crawlist-0.0.1.tar` & `crawlist-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 06:32:32.838123 crawlist-0.0.1/
--rw-rw-rw-   0        0        0     1084 2024-04-09 06:19:04.000000 crawlist-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-09 06:17:13.000000 crawlist-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      766 2024-04-09 06:32:32.837123 crawlist-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       57 2024-04-09 06:22:24.000000 crawlist-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 06:32:32.813984 crawlist-0.0.1/crawlist/
--rw-rw-rw-   0        0        0       21 2024-04-09 06:17:13.000000 crawlist-0.0.1/crawlist/__init__.py
--rw-rw-rw-   0        0        0      360 2024-04-09 06:27:42.000000 crawlist-0.0.1/crawlist/__version__.py
--rw-rw-rw-   0        0        0    17592 2024-04-09 06:19:04.000000 crawlist-0.0.1/crawlist/advanced_analyzer.py
--rw-rw-rw-   0        0        0     1330 2024-04-09 06:19:04.000000 crawlist-0.0.1/crawlist/analyzer.py
--rw-rw-rw-   0        0        0     5623 2024-04-09 06:19:04.000000 crawlist-0.0.1/crawlist/analyzer_pre_processing.py
--rw-rw-rw-   0        0        0    16777 2024-04-09 06:30:25.000000 crawlist-0.0.1/crawlist/analyzer_util.py
--rw-rw-rw-   0        0        0       27 2024-04-09 06:17:13.000000 crawlist-0.0.1/crawlist/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 06:32:32.836143 crawlist-0.0.1/crawlist.egg-info/
--rw-rw-rw-   0        0        0      766 2024-04-09 06:32:32.000000 crawlist-0.0.1/crawlist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-04-09 06:32:32.000000 crawlist-0.0.1/crawlist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 06:32:32.000000 crawlist-0.0.1/crawlist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-09 06:32:32.000000 crawlist-0.0.1/crawlist.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-09 06:32:32.000000 crawlist-0.0.1/crawlist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 06:32:32.838123 crawlist-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3952 2024-04-09 06:31:41.000000 crawlist-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:23:31.658490 crawlist-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 09:23:24.000000 crawlist-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 09:23:24.000000 crawlist-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-12 09:23:31.658490 crawlist-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-04-12 09:23:24.000000 crawlist-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:23:31.658490 crawlist-0.0.2/crawlist/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:23:31.658490 crawlist-0.0.2/crawlist/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10660 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/dynamic_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/static_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/valid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:23:31.658490 crawlist-0.0.2/crawlist/processings/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/processings/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:23:31.658490 crawlist-0.0.2/crawlist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-12 09:23:31.000000 crawlist-0.0.2/crawlist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-12 09:23:31.000000 crawlist-0.0.2/crawlist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:23:31.000000 crawlist-0.0.2/crawlist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 09:23:31.000000 crawlist-0.0.2/crawlist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 09:23:31.000000 crawlist-0.0.2/crawlist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:23:31.658490 crawlist-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-12 09:23:24.000000 crawlist-0.0.2/setup.py
```

### Comparing `crawlist-0.0.1/setup.py` & `crawlist-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,132 +1,131 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Note: To use the 'upload' functionality of this file, you must:
-#   $ pipenv install twine --dev
-
-import io
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import find_packages, setup, Command
-
-# Package meta-data.
-NAME = 'crawlist'
-DESCRIPTION = 'A universal solution for web crawling lists'
-URL = 'https://github.com/WwwwwyDev/crawlist'
-EMAIL = 'wwy20001014@foxmail.com'
-AUTHOR = 'WwyDev'
-REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.1'
-
-# What packages are required for this module to be executed?
-REQUIRED = [
-    # 'requests', 'maya', 'records',
-    'parsel', 'selenium'
-]
-
-# What packages are optional?
-EXTRAS = {
-    # 'fancy feature': ['django'],
-}
-
-# The rest you shouldn't have to touch too much :)
-# ------------------------------------------------
-# Except, perhaps the License and Trove Classifiers!
-# If you do change the License, remember to change the Trove Classifier for that!
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
-        exec(f.read(), about)
-else:
-    about['__version__'] = VERSION
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = 'Build and publish the package.'
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
-        except OSError:
-            pass
-
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
-
-        sys.exit()
-
-
-# Where the magic happens:
-setup(
-    name=NAME,
-    version=about['__version__'],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    # If your package is a single module, use this instead of 'packages':
-    # py_modules=['mypackage'],
-
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
-    install_requires=REQUIRED,
-    extras_require=EXTRAS,
-    include_package_data=True,
-    license='MIT',
-    classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
-    ],
-    # $ setup.py publish support.
-    cmdclass={
-        'upload': UploadCommand,
-    },
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Note: To use the 'upload' functionality of this file, you must:
+#   $ pipenv install twine --dev
+
+import io
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import find_packages, setup, Command
+
+# Package meta-data.
+NAME = 'crawlist'
+DESCRIPTION = 'A universal solution for web crawling lists'
+URL = 'https://github.com/WwwwwyDev/crawlist'
+EMAIL = 'wwy20001014@foxmail.com'
+AUTHOR = 'WwyDev'
+REQUIRES_PYTHON = '>=3.6.0'
+VERSION = '0.0.2'
+
+# What packages are required for this module to be executed?
+REQUIRED = [
+    'parsel', 'selenium>=4.0.0', 'cssselect', 'lxml', 'requests', 'webdriver-manager'
+]
+
+# What packages are optional?
+EXTRAS = {
+    # 'fancy feature': ['django'],
+}
+
+# The rest you shouldn't have to touch too much :)
+# ------------------------------------------------
+# Except, perhaps the License and Trove Classifiers!
+# If you do change the License, remember to change the Trove Classifier for that!
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
+try:
+    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+        long_description = '\n' + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package's __version__.py module as a dictionary.
+about = {}
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+        exec(f.read(), about)
+else:
+    about['__version__'] = VERSION
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = 'Build and publish the package.'
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print('\033[1m{0}\033[0m'.format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status('Removing previous builds…')
+            rmtree(os.path.join(here, 'dist'))
+        except OSError:
+            pass
+
+        self.status('Building Source and Wheel (universal) distribution…')
+        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+
+        self.status('Uploading the package to PyPI via Twine…')
+        os.system('twine upload dist/*')
+
+        self.status('Pushing git tags…')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
+
+        sys.exit()
+
+
+# Where the magic happens:
+setup(
+    name=NAME,
+    version=about['__version__'],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    # If your package is a single module, use this instead of 'packages':
+    # py_modules=['mypackage'],
+
+    # entry_points={
+    #     'console_scripts': ['mycli=mymodule:cli'],
+    # },
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    include_package_data=True,
+    license='MIT',
+    classifiers=[
+        # Trove classifiers
+        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy'
+    ],
+    # $ setup.py publish support.
+    cmdclass={
+        'upload': UploadCommand,
+    },
+)
```

