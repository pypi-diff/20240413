# Comparing `tmp/alana-0.0.1.tar.gz` & `tmp/alana-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alana-0.0.1.tar", last modified: Thu Apr 11 14:36:20 2024, max compression
+gzip compressed data, was "alana-0.0.2.tar", last modified: Sat Apr 13 09:24:23 2024, max compression
```

## Comparing `alana-0.0.1.tar` & `alana-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:36:20.848222 alana-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-11 14:36:15.000000 alana-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-11 14:36:20.848222 alana-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-11 14:36:15.000000 alana-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:36:20.848222 alana-0.0.1/alana/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:36:15.000000 alana-0.0.1/alana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-11 14:36:15.000000 alana-0.0.1/alana/alana.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-11 14:36:15.000000 alana-0.0.1/alana/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-11 14:36:15.000000 alana-0.0.1/alana/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:36:20.848222 alana-0.0.1/alana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-11 14:36:20.000000 alana-0.0.1/alana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 14:36:20.000000 alana-0.0.1/alana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:36:20.000000 alana-0.0.1/alana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 14:36:20.000000 alana-0.0.1/alana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 14:36:20.000000 alana-0.0.1/alana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:36:20.848222 alana-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-11 14:36:15.000000 alana-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:24:23.558023 alana-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-13 09:24:19.000000 alana-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-13 09:24:23.558023 alana-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-13 09:24:19.000000 alana-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:24:23.558023 alana-0.0.2/alana/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-13 09:24:19.000000 alana-0.0.2/alana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-13 09:24:19.000000 alana-0.0.2/alana/alana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-13 09:24:19.000000 alana-0.0.2/alana/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-13 09:24:19.000000 alana-0.0.2/alana/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:24:23.558023 alana-0.0.2/alana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-13 09:24:23.000000 alana-0.0.2/alana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 09:24:23.000000 alana-0.0.2/alana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 09:24:23.000000 alana-0.0.2/alana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 09:24:23.000000 alana-0.0.2/alana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 09:24:23.000000 alana-0.0.2/alana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 09:24:23.558023 alana-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-13 09:24:19.000000 alana-0.0.2/setup.py
```

### Comparing `alana-0.0.1/LICENSE` & `alana-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alana-0.0.1/PKG-INFO` & `alana-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alana
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.
 Home-page: https://github.com/alat-rights/alana-utilities
 Author: Alana
 Author-email: hi@alana.computer
 Keywords: LLM,utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,26 +15,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: anthropic
 Requires-Dist: colorama
-Requires-Dist: typing
 
 # alana-utilities
 Quick utilities for myself, mostly geared toward interacting with LLMs.
 
+Install Instructions
+```
+pip install alana
+```
+
 - Easy color print: red, green, blue, yellow, cyan
 - Make it easier to use the Anthropic API:
   - gen, for easy Claude generations
   - gen_examples, gen_examples_list for generating few-shot examples
   - get_xml, for using regex to get XML tag contents
 - A bunch of aliases
 
 TODO:
 - Easy prompt generation (meta-prompt) and alternative prompts given prompt
 - OpenAI model support
 - Support for automatic "are you sure"/"are you confused" multi-turn prompting
 - Support for multi-turn model interactions
 - Automatic error checking (are there mistakes in this code, sanity checking of model outputs)
 - Automatic model-switching on rate limit
+- Prompt test case generation and easy prompt testing
```

### Comparing `alana-0.0.1/README.md` & `alana-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # alana-utilities
 Quick utilities for myself, mostly geared toward interacting with LLMs.
 
+Install Instructions
+```
+pip install alana
+```
+
 - Easy color print: red, green, blue, yellow, cyan
 - Make it easier to use the Anthropic API:
   - gen, for easy Claude generations
   - gen_examples, gen_examples_list for generating few-shot examples
   - get_xml, for using regex to get XML tag contents
 - A bunch of aliases
 
 TODO:
 - Easy prompt generation (meta-prompt) and alternative prompts given prompt
 - OpenAI model support
 - Support for automatic "are you sure"/"are you confused" multi-turn prompting
 - Support for multi-turn model interactions
 - Automatic error checking (are there mistakes in this code, sanity checking of model outputs)
 - Automatic model-switching on rate limit
+- Prompt test case generation and easy prompt testing
```

### Comparing `alana-0.0.1/alana/color.py` & `alana-0.0.2/alana/color.py`

 * *Files identical despite different names*

### Comparing `alana-0.0.1/alana.egg-info/PKG-INFO` & `alana-0.0.2/alana.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alana
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.
 Home-page: https://github.com/alat-rights/alana-utilities
 Author: Alana
 Author-email: hi@alana.computer
 Keywords: LLM,utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,26 +15,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: anthropic
 Requires-Dist: colorama
-Requires-Dist: typing
 
 # alana-utilities
 Quick utilities for myself, mostly geared toward interacting with LLMs.
 
+Install Instructions
+```
+pip install alana
+```
+
 - Easy color print: red, green, blue, yellow, cyan
 - Make it easier to use the Anthropic API:
   - gen, for easy Claude generations
   - gen_examples, gen_examples_list for generating few-shot examples
   - get_xml, for using regex to get XML tag contents
 - A bunch of aliases
 
 TODO:
 - Easy prompt generation (meta-prompt) and alternative prompts given prompt
 - OpenAI model support
 - Support for automatic "are you sure"/"are you confused" multi-turn prompting
 - Support for multi-turn model interactions
 - Automatic error checking (are there mistakes in this code, sanity checking of model outputs)
 - Automatic model-switching on rate limit
+- Prompt test case generation and easy prompt testing
```

### Comparing `alana-0.0.1/setup.py` & `alana-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
    name='alana',
-   version='0.0.1',  # Update the version number as needed
+   version='0.0.2',  # Update the version number as needed
    author='Alana',
    author_email='hi@alana.computer',
    description='Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.',
    long_description=long_description,
    long_description_content_type="text/markdown",
-   url='https://github.com/alat-rights/alana-utilities',  # Replace with your repository URL
+   url='https://github.com/alat-rights/alana-utilities',
    packages=find_packages(),
    classifiers=[
          'Development Status :: 3 - Alpha',
          'Intended Audience :: Developers',
          'License :: OSI Approved :: MIT License',
          'Programming Language :: Python :: 3',
          'Programming Language :: Python :: 3.6',
@@ -25,10 +25,9 @@
          'Programming Language :: Python :: 3.9',
    ],
    keywords='LLM, utilities',  # Add relevant keywords
    python_requires='>=3.6',
    install_requires=[
       'anthropic',
       'colorama',
-      'typing',
    ],
 )
```

