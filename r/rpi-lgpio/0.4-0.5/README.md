# Comparing `tmp/rpi-lgpio-0.4.tar.gz` & `tmp/rpi-lgpio-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi-lgpio-0.4.tar", last modified: Tue Oct  3 13:53:44 2023, max compression
+gzip compressed data, was "rpi-lgpio-0.5.tar", last modified: Fri Apr 12 22:52:01 2024, max compression
```

## Comparing `rpi-lgpio-0.4.tar` & `rpi-lgpio-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-10-03 13:53:44.474616 rpi-lgpio-0.4/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1130 2022-10-14 16:04:33.000000 rpi-lgpio-0.4/LICENSE.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     1885 2023-10-03 13:53:44.474616 rpi-lgpio-0.4/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      772 2022-10-14 16:04:33.000000 rpi-lgpio-0.4/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-10-03 13:53:44.474616 rpi-lgpio-0.4/RPi/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-10-03 13:53:44.474616 rpi-lgpio-0.4/RPi/GPIO/
--rw-rw-r--   0 dave      (1000) dave      (1000)    29006 2023-10-03 13:42:16.000000 rpi-lgpio-0.4/RPi/GPIO/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2022-10-14 16:04:33.000000 rpi-lgpio-0.4/RPi/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-10-03 13:53:44.474616 rpi-lgpio-0.4/rpi_lgpio.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1885 2023-10-03 13:53:44.000000 rpi-lgpio-0.4/rpi_lgpio.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      242 2023-10-03 13:53:44.000000 rpi-lgpio-0.4/rpi_lgpio.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-10-03 13:53:44.000000 rpi-lgpio-0.4/rpi_lgpio.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       57 2023-10-03 13:53:44.000000 rpi-lgpio-0.4/rpi_lgpio.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        4 2023-10-03 13:53:44.000000 rpi-lgpio-0.4/rpi_lgpio.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     1560 2023-10-03 13:53:44.474616 rpi-lgpio-0.4/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2022-10-14 16:04:33.000000 rpi-lgpio-0.4/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-04-12 22:52:01.433484 rpi-lgpio-0.5/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1130 2024-04-10 08:01:37.000000 rpi-lgpio-0.5/LICENSE.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2251 2024-04-12 22:52:01.433484 rpi-lgpio-0.5/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1138 2024-04-10 08:01:37.000000 rpi-lgpio-0.5/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-04-12 22:52:01.430484 rpi-lgpio-0.5/RPi/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-04-12 22:52:01.431484 rpi-lgpio-0.5/RPi/GPIO/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    29014 2024-04-10 08:01:37.000000 rpi-lgpio-0.5/RPi/GPIO/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2024-04-10 08:01:37.000000 rpi-lgpio-0.5/RPi/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-04-12 22:52:01.433484 rpi-lgpio-0.5/rpi_lgpio.egg-info/
+-rw-r--r--   0 dave      (1000) dave      (1000)     2251 2024-04-12 22:52:01.000000 rpi-lgpio-0.5/rpi_lgpio.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      242 2024-04-12 22:52:01.000000 rpi-lgpio-0.5/rpi_lgpio.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2024-04-12 22:52:01.000000 rpi-lgpio-0.5/rpi_lgpio.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       63 2024-04-12 22:52:01.000000 rpi-lgpio-0.5/rpi_lgpio.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        4 2024-04-12 22:52:01.000000 rpi-lgpio-0.5/rpi_lgpio.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1587 2024-04-12 22:52:01.434484 rpi-lgpio-0.5/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2024-04-10 08:01:37.000000 rpi-lgpio-0.5/setup.py
```

### Comparing `rpi-lgpio-0.4/LICENSE.txt` & `rpi-lgpio-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rpi-lgpio-0.4/PKG-INFO` & `rpi-lgpio-0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-lgpio
-Version: 0.4
+Version: 0.5
 Summary: A compatibility shim between RPi.GPIO and lgpio
 Home-page: https://rpi-lgpio.readthedocs.io/
 Author: Dave Jones
 Author-email: dave@waveform.org.uk
 License: BSD-3-Clause
 Project-URL: Documentation, https://rpi-lgpio.readthedocs.io/
 Project-URL: Source Code, https://github.com/waveform80/rpi-lgpio
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: test
 License-File: LICENSE.txt
 
 ======
 README
 ======
 
 rpi-lgpio is a compatibility package intended to provide compatibility with
@@ -38,10 +38,23 @@
 .. warning::
 
     You *cannot* install rpi-lgpio and `rpi-gpio`_ (aka RPi.GPIO, the library
     it emulates) at the same time, in the same Python environment. Both
     packages attempt to install a module named ``RPi.GPIO`` and obviously this
     will not work.
 
+Useful Links
+============
+
+* `Source code <https://github.com/waveform80/rpi-lgpio>`_
+
+* `Bug reports <https://github.com/waveform80/rpi-lgpio/issues>`_
+
+* `Documentation <https://rpi-lgpio.readthedocs.io/>`_
+
+* `Ubuntu packaging <https://launchpad.net/ubuntu/+source/rpi-lgpio>`_
+
+.. * `Debian packaging <https://salsa.debian.org/python-team/packages/rpi-lgpio>`_
+
 .. _rpi-gpio: https://pypi.org/project/RPi.GPIO/
 .. _gpiochip device: https://embeddedbits.org/new-linux-kernel-gpio-user-space-interface/
 .. _deprecated sysfs GPIO interface: https://waldorf.waveform.org.uk/2021/the-pins-they-are-a-changin.html
```

### Comparing `rpi-lgpio-0.4/RPi/GPIO/__init__.py` & `rpi-lgpio-0.5/RPi/GPIO/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -652,15 +652,15 @@
 
     for gpio in _gpio_list(chanlist):
         # We don't bother with warnings about GPIOs already in use here because
         # if we try to *use* a GPIO already in use, things are going to blow up
         # shortly anyway. We do deal with the pull-up warning, but only for
         # GPIO2 and GPIO3 because we're not supporting the original RPi so we
         # don't need to worry about the GPIO0 and GPIO1 discrepancy
-        if _warnings and gpio in (2, 3) and pull in (PUD_UP, PUD_DOWN):
+        if _warnings and gpio in (2, 3) and pull_up_down in (PUD_UP, PUD_DOWN):
             warnings.warn(Warning(
                 'A physical pull up resistor is fitted on this channel!'))
         if direction == IN:
             # This gpio_free may seem redundant, but is required when changing
             # the line-flags of an already acquired input line
             try:
                 lgpio.gpio_free(_chip, gpio)
```

### Comparing `rpi-lgpio-0.4/rpi_lgpio.egg-info/PKG-INFO` & `rpi-lgpio-0.5/rpi_lgpio.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-lgpio
-Version: 0.4
+Version: 0.5
 Summary: A compatibility shim between RPi.GPIO and lgpio
 Home-page: https://rpi-lgpio.readthedocs.io/
 Author: Dave Jones
 Author-email: dave@waveform.org.uk
 License: BSD-3-Clause
 Project-URL: Documentation, https://rpi-lgpio.readthedocs.io/
 Project-URL: Source Code, https://github.com/waveform80/rpi-lgpio
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: test
 License-File: LICENSE.txt
 
 ======
 README
 ======
 
 rpi-lgpio is a compatibility package intended to provide compatibility with
@@ -38,10 +38,23 @@
 .. warning::
 
     You *cannot* install rpi-lgpio and `rpi-gpio`_ (aka RPi.GPIO, the library
     it emulates) at the same time, in the same Python environment. Both
     packages attempt to install a module named ``RPi.GPIO`` and obviously this
     will not work.
 
+Useful Links
+============
+
+* `Source code <https://github.com/waveform80/rpi-lgpio>`_
+
+* `Bug reports <https://github.com/waveform80/rpi-lgpio/issues>`_
+
+* `Documentation <https://rpi-lgpio.readthedocs.io/>`_
+
+* `Ubuntu packaging <https://launchpad.net/ubuntu/+source/rpi-lgpio>`_
+
+.. * `Debian packaging <https://salsa.debian.org/python-team/packages/rpi-lgpio>`_
+
 .. _rpi-gpio: https://pypi.org/project/RPi.GPIO/
 .. _gpiochip device: https://embeddedbits.org/new-linux-kernel-gpio-user-space-interface/
 .. _deprecated sysfs GPIO interface: https://waldorf.waveform.org.uk/2021/the-pins-they-are-a-changin.html
```

### Comparing `rpi-lgpio-0.4/setup.cfg` & `rpi-lgpio-0.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rpi-lgpio
-version = 0.4
+version = 0.5
 description = A compatibility shim between RPi.GPIO and lgpio
 long_description = file:README.rst
 author = Dave Jones
 author_email = dave@waveform.org.uk
 url = https://rpi-lgpio.readthedocs.io/
 project_urls = 
 	Documentation = https://rpi-lgpio.readthedocs.io/
@@ -24,14 +24,16 @@
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 packages = find:
 python_requires = >=3.7
+install_requires = 
+	lgpio
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 doc = 
 	sphinx
```

