# Comparing `tmp/python-tgpt-0.6.0.tar.gz` & `tmp/python_tgpt-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-tgpt-0.6.0.tar", last modified: Fri Apr 12 03:30:10 2024, max compression
+gzip compressed data, was "python_tgpt-0.6.1.tar", last modified: Fri Apr 12 19:24:22 2024, max compression
```

## Comparing `python-tgpt-0.6.0.tar` & `python_tgpt-0.6.1.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.082981 python-tgpt-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19438 2024-04-12 03:30:10.082981 python-tgpt-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-04-12 03:30:09.000000 python-tgpt-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:30:10.082981 python-tgpt-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.066980 python-tgpt-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.066980 python-tgpt-0.6.0/src/pytgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/api/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/blackboxai/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/blackboxai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/blackboxai/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    78689 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gemini/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/gpt4all/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gpt4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gpt4all/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gpt4free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gpt4free/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gpt4free/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/groq/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/groq/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/imager/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/imager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/imager/imager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/koboldai/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/koboldai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/koboldai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/leo/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/leo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/leo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/llama2/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/llama2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/llama2/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/openai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/opengpt/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/opengpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/opengpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/perplexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/perplexity/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/phind/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/phind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/phind/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/poe/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/poe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/poe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    23471 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/webchatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/webchatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/webchatgpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.078981 python-tgpt-0.6.0/src/python_tgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19438 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.078981 python-tgpt-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_blackboxai.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_imager.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_koboldai.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_leo.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_opengpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_phind.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_webchatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.169216 python_tgpt-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19566 2024-04-12 19:24:22.169216 python_tgpt-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-04-12 19:24:21.000000 python_tgpt-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:24:22.173216 python_tgpt-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.157216 python_tgpt-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.161216 python_tgpt-0.6.1/src/pytgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.161216 python_tgpt-0.6.1/src/pytgpt/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12999 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/api/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.161216 python_tgpt-0.6.1/src/pytgpt/blackboxai/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/blackboxai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/blackboxai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78689 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.161216 python_tgpt-0.6.1/src/pytgpt/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/gemini/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.161216 python_tgpt-0.6.1/src/pytgpt/gpt4all/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/gpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/gpt4all/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.161216 python_tgpt-0.6.1/src/pytgpt/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/gpt4free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/gpt4free/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/gpt4free/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.161216 python_tgpt-0.6.1/src/pytgpt/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/groq/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.161216 python_tgpt-0.6.1/src/pytgpt/imager/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/imager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/imager/imager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.161216 python_tgpt-0.6.1/src/pytgpt/koboldai/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/koboldai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/koboldai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.161216 python_tgpt-0.6.1/src/pytgpt/leo/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/leo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/leo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.161216 python_tgpt-0.6.1/src/pytgpt/llama2/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/llama2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/llama2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.165216 python_tgpt-0.6.1/src/pytgpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/openai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.165216 python_tgpt-0.6.1/src/pytgpt/opengpt/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/opengpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/opengpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.165216 python_tgpt-0.6.1/src/pytgpt/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/perplexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/perplexity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.165216 python_tgpt-0.6.1/src/pytgpt/phind/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/phind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/phind/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.165216 python_tgpt-0.6.1/src/pytgpt/poe/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/poe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/poe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23825 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.165216 python_tgpt-0.6.1/src/pytgpt/webchatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/webchatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/src/pytgpt/webchatgpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.169216 python_tgpt-0.6.1/src/python_tgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19566 2024-04-12 19:24:22.000000 python_tgpt-0.6.1/src/python_tgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-12 19:24:22.000000 python_tgpt-0.6.1/src/python_tgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:24:22.000000 python_tgpt-0.6.1/src/python_tgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 19:24:22.000000 python_tgpt-0.6.1/src/python_tgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-12 19:24:22.000000 python_tgpt-0.6.1/src/python_tgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 19:24:22.000000 python_tgpt-0.6.1/src/python_tgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:24:22.169216 python_tgpt-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_blackboxai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_koboldai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_leo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_opengpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 19:23:52.000000 python_tgpt-0.6.1/tests/test_webchatgpt.py
```

### Comparing `python-tgpt-0.6.0/LICENSE` & `python_tgpt-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/PKG-INFO` & `python_tgpt-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.0
+Version: 0.6.1
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: webchatgpt==0.2.9
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: poe-api-wrapper==1.3.6
 Requires-Dist: brotli==1.1.0
 Requires-Dist: g4f>=0.2.6.1
@@ -116,15 +116,15 @@
 
 The name *python-tgpt* draws inspiration from its parent project [tgpt](https://github.com/aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this Python adaptation, users can effortlessly engage with a number of free LLMs available, fostering a smoother AI interaction experience.
 
 
 ### Features
 
 - 🐍 Python package
-- 🌐 FastAPI for web integration
+- [🌐 FastAPI for web integration](https://python-tgpt.onrender.com)
 - ⌨️ Command-line interface
 - 🧠 Multiple LLM providers - **45+**
 - 🌊 Stream and non-stream response
 - 🚀 Ready to use (No API key required)
 - 🎯 Customizable script generation and execution
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
@@ -538,15 +538,16 @@
 > To load previous conversations from a `.txt` file, use the `-fp` or `--filepath` flag. If no flag is passed, the default one will be used. To load context from a file without altering its content, use the `--retain-file` flag.
 
 ## Dynamic Provider
 
 Version **0.4.6** also introduces dynamic provider called `g4fauto`, which represents the fastest working g4f-based provider.
 
 > [!TIP]
-> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
+> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. 
+> `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
 
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
@@ -568,13 +569,15 @@
   interactive  Chat with AI interactively (Default)
   utils        Utility endpoint for pytgpt
   webchatgpt   Reverse Engineered ChatGPT Web-Version
 ```
 
 </details>
 
+REST-API is up and running on https://python-tgpt.onrender.com - *(unreliable)*.
+
 ## [CHANGELOG](https://github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md)
 
 ## Acknowledgements
 
 1. [x] [tgpt](https://github.com/aandrew-me/tgpt)
 2. [x] [gpt4free](https://github.com/xtekky/gpt4free)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.0 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.1 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -16,31 +16,31 @@
 Programming Language :: Python Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests==2.31.0 Requires-Dist: appdirs==1.4.4 Requires-Dist: pyyaml==6.0.1
-Requires-Dist: webchatgpt==0.2.9 Requires-Dist: GoogleBard1>=2.1.4 Requires-
-Dist: poe-api-wrapper==1.3.6 Requires-Dist: brotli==1.1.0 Requires-Dist:
-g4f>=0.2.6.1 Requires-Dist: Helpingai-T2==0.3 Provides-Extra: cli Requires-
-Dist: click==8.1.3; extra == "cli" Requires-Dist: rich==13.3.4; extra == "cli"
-Requires-Dist: clipman==3.1.0; extra == "cli" Requires-Dist: pyperclip==1.8.2;
-extra == "cli" Requires-Dist: colorama==0.4.6; extra == "cli" Requires-Dist:
-g4f>=0.2.6.1; extra == "cli" Requires-Dist: python-dotenv==1.0.0; extra ==
-"cli" Provides-Extra: api Requires-Dist: fastapi[all]==0.110.1; extra == "api"
-Provides-Extra: all Requires-Dist: g4f[all]>=0.2.6.1; extra == "all" Requires-
-Dist: matplotlib; extra == "all" Requires-Dist: gpt4all==2.2.0; extra == "all"
-Requires-Dist: click==8.1.3; extra == "all" Requires-Dist: rich==13.3.4; extra
-== "all" Requires-Dist: clipman==3.1.0; extra == "all" Requires-Dist:
-pyperclip==1.8.2; extra == "all" Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: g4f>=0.2.6.1; extra == "all" Requires-Dist: python-
-dotenv==1.0.0; extra == "all" Requires-Dist: fastapi[all]==0.110.1; extra ==
-"all"
+requests[socks]==2.31.0 Requires-Dist: appdirs==1.4.4 Requires-Dist:
+pyyaml==6.0.1 Requires-Dist: webchatgpt==0.2.9 Requires-Dist:
+GoogleBard1>=2.1.4 Requires-Dist: poe-api-wrapper==1.3.6 Requires-Dist:
+brotli==1.1.0 Requires-Dist: g4f>=0.2.6.1 Requires-Dist: Helpingai-T2==0.3
+Provides-Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
+rich==13.3.4; extra == "cli" Requires-Dist: clipman==3.1.0; extra == "cli"
+Requires-Dist: pyperclip==1.8.2; extra == "cli" Requires-Dist: colorama==0.4.6;
+extra == "cli" Requires-Dist: g4f>=0.2.6.1; extra == "cli" Requires-Dist:
+python-dotenv==1.0.0; extra == "cli" Provides-Extra: api Requires-Dist: fastapi
+[all]==0.110.1; extra == "api" Provides-Extra: all Requires-Dist: g4f
+[all]>=0.2.6.1; extra == "all" Requires-Dist: matplotlib; extra == "all"
+Requires-Dist: gpt4all==2.2.0; extra == "all" Requires-Dist: click==8.1.3;
+extra == "all" Requires-Dist: rich==13.3.4; extra == "all" Requires-Dist:
+clipman==3.1.0; extra == "all" Requires-Dist: pyperclip==1.8.2; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.2.6.1;
+extra == "all" Requires-Dist: python-dotenv==1.0.0; extra == "all" Requires-
+Dist: fastapi[all]==0.110.1; extra == "all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]_[_c_o_v_e_r_a_g_e_]
    _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
   _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
                         _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
@@ -50,56 +50,56 @@
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
 without requiring an API Key and generating images as well. The name *python-
 tgpt* draws inspiration from its parent project [tgpt](https://github.com/
 aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this
 Python adaptation, users can effortlessly engage with a number of free LLMs
 available, fostering a smoother AI interaction experience. ### Features - ð
-Python package - ð FastAPI for web integration - â¨ï¸ Command-line
-interface - ð§  Multiple LLM providers - **45+** - ð Stream and non-stream
-response - ð Ready to use (No API key required) - ð¯ Customizable script
-generation and execution - ð Offline support for Large Language Models -
-ð¨ Image generation capabilities - âï¸ Chained requests via proxy -
-ð¨ï¸ Enhanced conversational chat experience - ð¾ Capability to save
-prompts and responses (Conversation) - ð Ability to load previous
-conversations - ð¤ Pass [awesome-chatgpt prompts](https://github.com/f/
-awesome-chatgpt-prompts) easily ## Providers These are simply the hosts of the
-LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave** 2. [Koboldai]
-(https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs](https://
-opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com)
-*(API key required)* 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) -
-**OpenAI** *(Session ID required)* 6. [Gemini](https://github.com/Simatwa/bard)
-- **Google** *(Session ID required)* 9. [Phind](https://www.phind.com) -
-*default* 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
-www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
-//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
-console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
-www.perplexity.ai) 41+ providers proudly offered by [gpt4free](https://
-github.com/xtekky/gpt4free). - To list working providers run: ```sh $ pytgpt
-gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10](https://python.org)
-*(Optional)* ## Installation and Usage ### Installation Download binaries for
-your system from [here.](https://github.com/Simatwa/python-tgpt/releases/
-latest/) Alternatively, you can install non-binaries. *(Recommended)* 1.
-Developers: ```sh pip install --upgrade python-tgpt ``` 2. Commandline: ```sh
-pip install --upgrade "python-tgpt[cli]" ``` 3. Full installation: ```sh pip
-install --upgrade "python-tgpt[all]" ``` > `pip install -U "python-tgt[api]"`
-will install REST API dependencies. ## Usage This package offers a convenient
-command-line interface. > [!NOTE] > `phind` is the default *provider*. - For a
-quick response: ```bash python -m pytgpt generate "" ``` - For interactive
-mode: ```bash python -m pytgpt interactive "" ``` Make use of flag `--provider`
-followed by the provider name of your choice. e.g `--provider koboldai` > To
-list all providers offered by gpt4free, use following commands: ```pytgpt
-gpt4free list providers``` You can also simply use `pytgpt` instead of `python
--m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without any other
-command or option will automatically enter the `interactive` mode. Otherwise,
-you'll need to explicitly declare the desired action, for example, by running
-`$ pytgpt generate`. ### Developer Docs 1. Generate a quick response ```python
-from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output
-: How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
-import LEO bot = LEO() resp = bot.ask('
+Python package - [ð FastAPI for web integration](https://python-
+tgpt.onrender.com) - â¨ï¸ Command-line interface - ð§  Multiple LLM
+providers - **45+** - ð Stream and non-stream response - ð Ready to use
+(No API key required) - ð¯ Customizable script generation and execution -
+ð Offline support for Large Language Models - ð¨ Image generation
+capabilities - âï¸ Chained requests via proxy - ð¨ï¸ Enhanced
+conversational chat experience - ð¾ Capability to save prompts and responses
+(Conversation) - ð Ability to load previous conversations - ð¤ Pass
+[awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
+## Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
+(https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
+tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
+uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
+[WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
+required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
+ID required)* 9. [Phind](https://www.phind.com) - *default* 10. [Llama2](https:
+//www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https:
+//gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
+required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
+15. [Perplexity](https://www.perplexity.ai) 41+ providers proudly offered by
+[gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
+run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
+(https://python.org) *(Optional)* ## Installation and Usage ### Installation
+Download binaries for your system from [here.](https://github.com/Simatwa/
+python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
+(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
+Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
+installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
+-U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
+offers a convenient command-line interface. > [!NOTE] > `phind` is the default
+*provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
+For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
+flag `--provider` followed by the provider name of your choice. e.g `--provider
+koboldai` > To list all providers offered by gpt4free, use following commands:
+```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
+of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
+any other command or option will automatically enter the `interactive` mode.
+Otherwise, you'll need to explicitly declare the desired action, for example,
+by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick response
+```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print
+(resp) # Output : How may I help you. ``` 2. Get back whole response ```python
+from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -194,19 +194,20 @@
 a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--
 filepath` flag. If no flag is passed, the default one will be used. To load
 context from a file without altering its content, use the `--retain-file` flag.
 ## Dynamic Provider Version **0.4.6** also introduces dynamic provider called
 `g4fauto`, which represents the fastest working g4f-based provider. > [!TIP] >
 To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free
-gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
+gui`. > `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
 docs* and */redoc* respectively. For more usage info run `$ pytgpt --help` ```
 Usage: pytgpt [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the
 version and exit. -h, --help Show this message and exit. Commands: api FastAPI
 control endpoint awesome Perform CRUD operations on awesome-prompts generate
 Generate a quick response with AI gpt4free Discover gpt4free models, providers
 etc imager Generate images with pollinations.ai interactive Chat with AI
 interactively (Default) utils Utility endpoint for pytgpt webchatgpt Reverse
-Engineered ChatGPT Web-Version ``` ## [CHANGELOG](https://github.com/Simatwa/
-python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
-(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
-xtekky/gpt4free)
+Engineered ChatGPT Web-Version ``` REST-API is up and running on https://
+python-tgpt.onrender.com - *(unreliable)*. ## [CHANGELOG](https://github.com/
+Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x]
+[tgpt](https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://
+github.com/xtekky/gpt4free)
```

### Comparing `python-tgpt-0.6.0/README.md` & `python_tgpt-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 The name *python-tgpt* draws inspiration from its parent project [tgpt](https://github.com/aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this Python adaptation, users can effortlessly engage with a number of free LLMs available, fostering a smoother AI interaction experience.
 
 
 ### Features
 
 - 🐍 Python package
-- 🌐 FastAPI for web integration
+- [🌐 FastAPI for web integration](https://python-tgpt.onrender.com)
 - ⌨️ Command-line interface
 - 🧠 Multiple LLM providers - **45+**
 - 🌊 Stream and non-stream response
 - 🚀 Ready to use (No API key required)
 - 🎯 Customizable script generation and execution
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
@@ -473,15 +473,16 @@
 > To load previous conversations from a `.txt` file, use the `-fp` or `--filepath` flag. If no flag is passed, the default one will be used. To load context from a file without altering its content, use the `--retain-file` flag.
 
 ## Dynamic Provider
 
 Version **0.4.6** also introduces dynamic provider called `g4fauto`, which represents the fastest working g4f-based provider.
 
 > [!TIP]
-> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
+> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. 
+> `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
 
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
@@ -503,13 +504,15 @@
   interactive  Chat with AI interactively (Default)
   utils        Utility endpoint for pytgpt
   webchatgpt   Reverse Engineered ChatGPT Web-Version
 ```
 
 </details>
 
+REST-API is up and running on https://python-tgpt.onrender.com - *(unreliable)*.
+
 ## [CHANGELOG](https://github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md)
 
 ## Acknowledgements
 
 1. [x] [tgpt](https://github.com/aandrew-me/tgpt)
 2. [x] [gpt4free](https://github.com/xtekky/gpt4free)
```

#### html2text {}

```diff
@@ -11,56 +11,56 @@
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
 without requiring an API Key and generating images as well. The name *python-
 tgpt* draws inspiration from its parent project [tgpt](https://github.com/
 aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this
 Python adaptation, users can effortlessly engage with a number of free LLMs
 available, fostering a smoother AI interaction experience. ### Features - ð
-Python package - ð FastAPI for web integration - â¨ï¸ Command-line
-interface - ð§  Multiple LLM providers - **45+** - ð Stream and non-stream
-response - ð Ready to use (No API key required) - ð¯ Customizable script
-generation and execution - ð Offline support for Large Language Models -
-ð¨ Image generation capabilities - âï¸ Chained requests via proxy -
-ð¨ï¸ Enhanced conversational chat experience - ð¾ Capability to save
-prompts and responses (Conversation) - ð Ability to load previous
-conversations - ð¤ Pass [awesome-chatgpt prompts](https://github.com/f/
-awesome-chatgpt-prompts) easily ## Providers These are simply the hosts of the
-LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave** 2. [Koboldai]
-(https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs](https://
-opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com)
-*(API key required)* 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) -
-**OpenAI** *(Session ID required)* 6. [Gemini](https://github.com/Simatwa/bard)
-- **Google** *(Session ID required)* 9. [Phind](https://www.phind.com) -
-*default* 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
-www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
-//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
-console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
-www.perplexity.ai) 41+ providers proudly offered by [gpt4free](https://
-github.com/xtekky/gpt4free). - To list working providers run: ```sh $ pytgpt
-gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10](https://python.org)
-*(Optional)* ## Installation and Usage ### Installation Download binaries for
-your system from [here.](https://github.com/Simatwa/python-tgpt/releases/
-latest/) Alternatively, you can install non-binaries. *(Recommended)* 1.
-Developers: ```sh pip install --upgrade python-tgpt ``` 2. Commandline: ```sh
-pip install --upgrade "python-tgpt[cli]" ``` 3. Full installation: ```sh pip
-install --upgrade "python-tgpt[all]" ``` > `pip install -U "python-tgt[api]"`
-will install REST API dependencies. ## Usage This package offers a convenient
-command-line interface. > [!NOTE] > `phind` is the default *provider*. - For a
-quick response: ```bash python -m pytgpt generate "" ``` - For interactive
-mode: ```bash python -m pytgpt interactive "" ``` Make use of flag `--provider`
-followed by the provider name of your choice. e.g `--provider koboldai` > To
-list all providers offered by gpt4free, use following commands: ```pytgpt
-gpt4free list providers``` You can also simply use `pytgpt` instead of `python
--m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without any other
-command or option will automatically enter the `interactive` mode. Otherwise,
-you'll need to explicitly declare the desired action, for example, by running
-`$ pytgpt generate`. ### Developer Docs 1. Generate a quick response ```python
-from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output
-: How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
-import LEO bot = LEO() resp = bot.ask('
+Python package - [ð FastAPI for web integration](https://python-
+tgpt.onrender.com) - â¨ï¸ Command-line interface - ð§  Multiple LLM
+providers - **45+** - ð Stream and non-stream response - ð Ready to use
+(No API key required) - ð¯ Customizable script generation and execution -
+ð Offline support for Large Language Models - ð¨ Image generation
+capabilities - âï¸ Chained requests via proxy - ð¨ï¸ Enhanced
+conversational chat experience - ð¾ Capability to save prompts and responses
+(Conversation) - ð Ability to load previous conversations - ð¤ Pass
+[awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
+## Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
+(https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
+tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
+uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
+[WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
+required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
+ID required)* 9. [Phind](https://www.phind.com) - *default* 10. [Llama2](https:
+//www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https:
+//gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
+required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
+15. [Perplexity](https://www.perplexity.ai) 41+ providers proudly offered by
+[gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
+run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
+(https://python.org) *(Optional)* ## Installation and Usage ### Installation
+Download binaries for your system from [here.](https://github.com/Simatwa/
+python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
+(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
+Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
+installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
+-U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
+offers a convenient command-line interface. > [!NOTE] > `phind` is the default
+*provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
+For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
+flag `--provider` followed by the provider name of your choice. e.g `--provider
+koboldai` > To list all providers offered by gpt4free, use following commands:
+```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
+of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
+any other command or option will automatically enter the `interactive` mode.
+Otherwise, you'll need to explicitly declare the desired action, for example,
+by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick response
+```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print
+(resp) # Output : How may I help you. ``` 2. Get back whole response ```python
+from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -155,19 +155,20 @@
 a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--
 filepath` flag. If no flag is passed, the default one will be used. To load
 context from a file without altering its content, use the `--retain-file` flag.
 ## Dynamic Provider Version **0.4.6** also introduces dynamic provider called
 `g4fauto`, which represents the fastest working g4f-based provider. > [!TIP] >
 To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free
-gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
+gui`. > `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
 docs* and */redoc* respectively. For more usage info run `$ pytgpt --help` ```
 Usage: pytgpt [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the
 version and exit. -h, --help Show this message and exit. Commands: api FastAPI
 control endpoint awesome Perform CRUD operations on awesome-prompts generate
 Generate a quick response with AI gpt4free Discover gpt4free models, providers
 etc imager Generate images with pollinations.ai interactive Chat with AI
 interactively (Default) utils Utility endpoint for pytgpt webchatgpt Reverse
-Engineered ChatGPT Web-Version ``` ## [CHANGELOG](https://github.com/Simatwa/
-python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
-(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
-xtekky/gpt4free)
+Engineered ChatGPT Web-Version ``` REST-API is up and running on https://
+python-tgpt.onrender.com - *(unreliable)*. ## [CHANGELOG](https://github.com/
+Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x]
+[tgpt](https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://
+github.com/xtekky/gpt4free)
```

### Comparing `python-tgpt-0.6.0/setup.py` & `python_tgpt-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 from setuptools import find_packages
 
 
 INSTALL_REQUIRE = [
-    "requests==2.31.0",
+    "requests[socks]==2.31.0",
     "appdirs==1.4.4",
     "pyyaml==6.0.1",
     "webchatgpt==0.2.9",
     "GoogleBard1>=2.1.4",
     "poe-api-wrapper==1.3.6",
     "brotli==1.1.0",
     "g4f>=0.2.6.1",
@@ -42,15 +42,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="python-tgpt",
-    version="0.6.0",
+    version="0.6.1",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Interact with AI without API key",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `python-tgpt-0.6.0/src/pytgpt/__init__.py` & `python_tgpt-0.6.1/src/pytgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/base.py` & `python_tgpt-0.6.1/src/pytgpt/base.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/blackboxai/main.py` & `python_tgpt-0.6.1/src/pytgpt/blackboxai/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/console.py` & `python_tgpt-0.6.1/src/pytgpt/console.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/gemini/main.py` & `python_tgpt-0.6.1/src/pytgpt/gemini/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/gpt4all/main.py` & `python_tgpt-0.6.1/src/pytgpt/gpt4all/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/gpt4free/main.py` & `python_tgpt-0.6.1/src/pytgpt/gpt4free/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/gpt4free/utils.py` & `python_tgpt-0.6.1/src/pytgpt/gpt4free/utils.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/groq/main.py` & `python_tgpt-0.6.1/src/pytgpt/groq/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/imager/imager.py` & `python_tgpt-0.6.1/src/pytgpt/imager/imager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 import os
-from typing import Generator
+from typing import Generator, Union
 from string import punctuation
 from random import choice
 
 session = requests.Session()
 
 
 class Imager:
@@ -23,15 +23,15 @@
         self.headers = {
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
             "Accept-Language": "en-US,en;q=0.5",
             "Accept-Encoding": "gzip, deflate",
             "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:122.0) Gecko/20100101 Firefox/122.0",
         }
         session.proxies = proxies
-        session.timeout = timeout
+        self.timeout = timeout
         self.__prompt: str = "AI-generated image - pytgpt"
 
     def generate(
         self, prompt: str, amount: int = 1, stream: bool = False, additives: bool = True
     ) -> list[bytes]:
         """Generat image from prompt
 
@@ -57,15 +57,16 @@
             + choice(punctuation)
             + choice(punctuation)
         )
 
         def for_stream():
             for _ in range(amount):
                 resp = session.get(
-                    url=self.image_gen_endpoint % dict(prompt=prompt + ads())
+                    url=self.image_gen_endpoint % dict(prompt=prompt + ads()),
+                    timeout=self.timeout,
                 )
                 resp.raise_for_status()
                 yield resp.content
 
         def for_non_stream():
             response = []
 
@@ -73,38 +74,50 @@
                 response.append(image)
             return response
 
         self.__prompt = prompt
         return for_stream() if stream else for_non_stream()
 
     def save(
-        self, response: list[bytes], name: str = None, dir: str = os.getcwd()
-    ) -> None:
+        self,
+        response: list[bytes],
+        name: str = None,
+        dir: str = os.getcwd(),
+        filenames_prefix: str = "",
+    ) -> list[str]:
         """Save generated images
 
         Args:
             response (list[bytes]|Generator): Response of Imager.generate
             name (str):  Filename for the images. Defaults to last prompt.
             dir (str, optional): Directory for saving images. Defaults to os.getcwd().
+            filenames_prefix (str, optional): String to be prefixed at each filename to be returned.
         """
         assert isinstance(
             response, (list, Generator)
         ), f"Response should be of {list} or {Generator} types"
         name = self.__prompt if name is None else name
 
+        filenames: list = []
+
         for count, image in enumerate(response):
 
             def complete_path():
                 count_value = "" if count == 0 else f"_{count}"
                 return os.path.join(dir, name + count_value + "." + "jpeg")
 
             while os.path.isfile(complete_path()):
                 count += 1
 
-            with open(complete_path(), "wb") as fh:
+            absolute_path_to_file = complete_path()
+            filenames.append(filenames_prefix + os.path.split(absolute_path_to_file)[1])
+
+            with open(absolute_path_to_file, "wb") as fh:
                 fh.write(image)
 
+        return filenames
+
 
 if __name__ == "__main__":
     bot = Imager()
     resp = bot.generate("Coding bot ", 3, stream=True)
     bot.save(resp)
```

### Comparing `python-tgpt-0.6.0/src/pytgpt/koboldai/main.py` & `python_tgpt-0.6.1/src/pytgpt/koboldai/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/leo/main.py` & `python_tgpt-0.6.1/src/pytgpt/leo/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/llama2/main.py` & `python_tgpt-0.6.1/src/pytgpt/llama2/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/openai/main.py` & `python_tgpt-0.6.1/src/pytgpt/openai/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/opengpt/main.py` & `python_tgpt-0.6.1/src/pytgpt/opengpt/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/perplexity/main.py` & `python_tgpt-0.6.1/src/pytgpt/perplexity/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/phind/main.py` & `python_tgpt-0.6.1/src/pytgpt/phind/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/poe/main.py` & `python_tgpt-0.6.1/src/pytgpt/poe/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/pytgpt/utils.py` & `python_tgpt-0.6.1/src/pytgpt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,33 @@
 import appdirs
 import datetime
 import re
 import sys
 import click
 from rich.markdown import Markdown
 from rich.console import Console
+from pathlib import Path
+import os
+import shutil
 
 appdir = appdirs.AppDirs("pytgpt", "Smartwa")
 
 default_path = appdir.user_cache_dir
 
-if not os.path.exists(default_path):
-    os.makedirs(default_path)
+api_static_dir = Path(default_path) / "api"
+
+api_static_image_dir = api_static_dir / "images"
+
+if api_static_image_dir.exists():
+    # Remove static images
+    shutil.rmtree(api_static_image_dir, ignore_errors=True)
+
+os.makedirs(default_path, exist_ok=True)
+os.makedirs(api_static_dir.as_posix(), exist_ok=True)
+os.makedirs(api_static_image_dir.as_posix(), exist_ok=True)
 
 
 def run_system_command(
     command: str,
     exit_on_error: bool = True,
     stdout_error: bool = True,
     help: str = None,
```

### Comparing `python-tgpt-0.6.0/src/pytgpt/webchatgpt/main.py` & `python_tgpt-0.6.1/src/pytgpt/webchatgpt/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/src/python_tgpt.egg-info/PKG-INFO` & `python_tgpt-0.6.1/src/python_tgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.0
+Version: 0.6.1
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: webchatgpt==0.2.9
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: poe-api-wrapper==1.3.6
 Requires-Dist: brotli==1.1.0
 Requires-Dist: g4f>=0.2.6.1
@@ -116,15 +116,15 @@
 
 The name *python-tgpt* draws inspiration from its parent project [tgpt](https://github.com/aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this Python adaptation, users can effortlessly engage with a number of free LLMs available, fostering a smoother AI interaction experience.
 
 
 ### Features
 
 - 🐍 Python package
-- 🌐 FastAPI for web integration
+- [🌐 FastAPI for web integration](https://python-tgpt.onrender.com)
 - ⌨️ Command-line interface
 - 🧠 Multiple LLM providers - **45+**
 - 🌊 Stream and non-stream response
 - 🚀 Ready to use (No API key required)
 - 🎯 Customizable script generation and execution
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
@@ -538,15 +538,16 @@
 > To load previous conversations from a `.txt` file, use the `-fp` or `--filepath` flag. If no flag is passed, the default one will be used. To load context from a file without altering its content, use the `--retain-file` flag.
 
 ## Dynamic Provider
 
 Version **0.4.6** also introduces dynamic provider called `g4fauto`, which represents the fastest working g4f-based provider.
 
 > [!TIP]
-> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
+> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. 
+> `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
 
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
@@ -568,13 +569,15 @@
   interactive  Chat with AI interactively (Default)
   utils        Utility endpoint for pytgpt
   webchatgpt   Reverse Engineered ChatGPT Web-Version
 ```
 
 </details>
 
+REST-API is up and running on https://python-tgpt.onrender.com - *(unreliable)*.
+
 ## [CHANGELOG](https://github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md)
 
 ## Acknowledgements
 
 1. [x] [tgpt](https://github.com/aandrew-me/tgpt)
 2. [x] [gpt4free](https://github.com/xtekky/gpt4free)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.0 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.1 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -16,31 +16,31 @@
 Programming Language :: Python Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests==2.31.0 Requires-Dist: appdirs==1.4.4 Requires-Dist: pyyaml==6.0.1
-Requires-Dist: webchatgpt==0.2.9 Requires-Dist: GoogleBard1>=2.1.4 Requires-
-Dist: poe-api-wrapper==1.3.6 Requires-Dist: brotli==1.1.0 Requires-Dist:
-g4f>=0.2.6.1 Requires-Dist: Helpingai-T2==0.3 Provides-Extra: cli Requires-
-Dist: click==8.1.3; extra == "cli" Requires-Dist: rich==13.3.4; extra == "cli"
-Requires-Dist: clipman==3.1.0; extra == "cli" Requires-Dist: pyperclip==1.8.2;
-extra == "cli" Requires-Dist: colorama==0.4.6; extra == "cli" Requires-Dist:
-g4f>=0.2.6.1; extra == "cli" Requires-Dist: python-dotenv==1.0.0; extra ==
-"cli" Provides-Extra: api Requires-Dist: fastapi[all]==0.110.1; extra == "api"
-Provides-Extra: all Requires-Dist: g4f[all]>=0.2.6.1; extra == "all" Requires-
-Dist: matplotlib; extra == "all" Requires-Dist: gpt4all==2.2.0; extra == "all"
-Requires-Dist: click==8.1.3; extra == "all" Requires-Dist: rich==13.3.4; extra
-== "all" Requires-Dist: clipman==3.1.0; extra == "all" Requires-Dist:
-pyperclip==1.8.2; extra == "all" Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: g4f>=0.2.6.1; extra == "all" Requires-Dist: python-
-dotenv==1.0.0; extra == "all" Requires-Dist: fastapi[all]==0.110.1; extra ==
-"all"
+requests[socks]==2.31.0 Requires-Dist: appdirs==1.4.4 Requires-Dist:
+pyyaml==6.0.1 Requires-Dist: webchatgpt==0.2.9 Requires-Dist:
+GoogleBard1>=2.1.4 Requires-Dist: poe-api-wrapper==1.3.6 Requires-Dist:
+brotli==1.1.0 Requires-Dist: g4f>=0.2.6.1 Requires-Dist: Helpingai-T2==0.3
+Provides-Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
+rich==13.3.4; extra == "cli" Requires-Dist: clipman==3.1.0; extra == "cli"
+Requires-Dist: pyperclip==1.8.2; extra == "cli" Requires-Dist: colorama==0.4.6;
+extra == "cli" Requires-Dist: g4f>=0.2.6.1; extra == "cli" Requires-Dist:
+python-dotenv==1.0.0; extra == "cli" Provides-Extra: api Requires-Dist: fastapi
+[all]==0.110.1; extra == "api" Provides-Extra: all Requires-Dist: g4f
+[all]>=0.2.6.1; extra == "all" Requires-Dist: matplotlib; extra == "all"
+Requires-Dist: gpt4all==2.2.0; extra == "all" Requires-Dist: click==8.1.3;
+extra == "all" Requires-Dist: rich==13.3.4; extra == "all" Requires-Dist:
+clipman==3.1.0; extra == "all" Requires-Dist: pyperclip==1.8.2; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.2.6.1;
+extra == "all" Requires-Dist: python-dotenv==1.0.0; extra == "all" Requires-
+Dist: fastapi[all]==0.110.1; extra == "all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]_[_c_o_v_e_r_a_g_e_]
    _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
   _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
                         _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
@@ -50,56 +50,56 @@
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
 without requiring an API Key and generating images as well. The name *python-
 tgpt* draws inspiration from its parent project [tgpt](https://github.com/
 aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this
 Python adaptation, users can effortlessly engage with a number of free LLMs
 available, fostering a smoother AI interaction experience. ### Features - ð
-Python package - ð FastAPI for web integration - â¨ï¸ Command-line
-interface - ð§  Multiple LLM providers - **45+** - ð Stream and non-stream
-response - ð Ready to use (No API key required) - ð¯ Customizable script
-generation and execution - ð Offline support for Large Language Models -
-ð¨ Image generation capabilities - âï¸ Chained requests via proxy -
-ð¨ï¸ Enhanced conversational chat experience - ð¾ Capability to save
-prompts and responses (Conversation) - ð Ability to load previous
-conversations - ð¤ Pass [awesome-chatgpt prompts](https://github.com/f/
-awesome-chatgpt-prompts) easily ## Providers These are simply the hosts of the
-LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave** 2. [Koboldai]
-(https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs](https://
-opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com)
-*(API key required)* 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) -
-**OpenAI** *(Session ID required)* 6. [Gemini](https://github.com/Simatwa/bard)
-- **Google** *(Session ID required)* 9. [Phind](https://www.phind.com) -
-*default* 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
-www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
-//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
-console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
-www.perplexity.ai) 41+ providers proudly offered by [gpt4free](https://
-github.com/xtekky/gpt4free). - To list working providers run: ```sh $ pytgpt
-gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10](https://python.org)
-*(Optional)* ## Installation and Usage ### Installation Download binaries for
-your system from [here.](https://github.com/Simatwa/python-tgpt/releases/
-latest/) Alternatively, you can install non-binaries. *(Recommended)* 1.
-Developers: ```sh pip install --upgrade python-tgpt ``` 2. Commandline: ```sh
-pip install --upgrade "python-tgpt[cli]" ``` 3. Full installation: ```sh pip
-install --upgrade "python-tgpt[all]" ``` > `pip install -U "python-tgt[api]"`
-will install REST API dependencies. ## Usage This package offers a convenient
-command-line interface. > [!NOTE] > `phind` is the default *provider*. - For a
-quick response: ```bash python -m pytgpt generate "" ``` - For interactive
-mode: ```bash python -m pytgpt interactive "" ``` Make use of flag `--provider`
-followed by the provider name of your choice. e.g `--provider koboldai` > To
-list all providers offered by gpt4free, use following commands: ```pytgpt
-gpt4free list providers``` You can also simply use `pytgpt` instead of `python
--m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without any other
-command or option will automatically enter the `interactive` mode. Otherwise,
-you'll need to explicitly declare the desired action, for example, by running
-`$ pytgpt generate`. ### Developer Docs 1. Generate a quick response ```python
-from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output
-: How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
-import LEO bot = LEO() resp = bot.ask('
+Python package - [ð FastAPI for web integration](https://python-
+tgpt.onrender.com) - â¨ï¸ Command-line interface - ð§  Multiple LLM
+providers - **45+** - ð Stream and non-stream response - ð Ready to use
+(No API key required) - ð¯ Customizable script generation and execution -
+ð Offline support for Large Language Models - ð¨ Image generation
+capabilities - âï¸ Chained requests via proxy - ð¨ï¸ Enhanced
+conversational chat experience - ð¾ Capability to save prompts and responses
+(Conversation) - ð Ability to load previous conversations - ð¤ Pass
+[awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
+## Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
+(https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
+tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
+uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
+[WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
+required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
+ID required)* 9. [Phind](https://www.phind.com) - *default* 10. [Llama2](https:
+//www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https:
+//gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
+required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
+15. [Perplexity](https://www.perplexity.ai) 41+ providers proudly offered by
+[gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
+run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
+(https://python.org) *(Optional)* ## Installation and Usage ### Installation
+Download binaries for your system from [here.](https://github.com/Simatwa/
+python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
+(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
+Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
+installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
+-U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
+offers a convenient command-line interface. > [!NOTE] > `phind` is the default
+*provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
+For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
+flag `--provider` followed by the provider name of your choice. e.g `--provider
+koboldai` > To list all providers offered by gpt4free, use following commands:
+```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
+of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
+any other command or option will automatically enter the `interactive` mode.
+Otherwise, you'll need to explicitly declare the desired action, for example,
+by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick response
+```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print
+(resp) # Output : How may I help you. ``` 2. Get back whole response ```python
+from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -194,19 +194,20 @@
 a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--
 filepath` flag. If no flag is passed, the default one will be used. To load
 context from a file without altering its content, use the `--retain-file` flag.
 ## Dynamic Provider Version **0.4.6** also introduces dynamic provider called
 `g4fauto`, which represents the fastest working g4f-based provider. > [!TIP] >
 To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free
-gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
+gui`. > `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
 docs* and */redoc* respectively. For more usage info run `$ pytgpt --help` ```
 Usage: pytgpt [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the
 version and exit. -h, --help Show this message and exit. Commands: api FastAPI
 control endpoint awesome Perform CRUD operations on awesome-prompts generate
 Generate a quick response with AI gpt4free Discover gpt4free models, providers
 etc imager Generate images with pollinations.ai interactive Chat with AI
 interactively (Default) utils Utility endpoint for pytgpt webchatgpt Reverse
-Engineered ChatGPT Web-Version ``` ## [CHANGELOG](https://github.com/Simatwa/
-python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
-(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
-xtekky/gpt4free)
+Engineered ChatGPT Web-Version ``` REST-API is up and running on https://
+python-tgpt.onrender.com - *(unreliable)*. ## [CHANGELOG](https://github.com/
+Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x]
+[tgpt](https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://
+github.com/xtekky/gpt4free)
```

### Comparing `python-tgpt-0.6.0/src/python_tgpt.egg-info/SOURCES.txt` & `python_tgpt-0.6.1/src/python_tgpt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 src/pytgpt/webchatgpt/main.py
 src/python_tgpt.egg-info/PKG-INFO
 src/python_tgpt.egg-info/SOURCES.txt
 src/python_tgpt.egg-info/dependency_links.txt
 src/python_tgpt.egg-info/entry_points.txt
 src/python_tgpt.egg-info/requires.txt
 src/python_tgpt.egg-info/top_level.txt
+tests/test_api.py
 tests/test_blackboxai.py
 tests/test_gemini.py
 tests/test_gpt4all.py
 tests/test_gpt4free.py
 tests/test_groq.py
 tests/test_imager.py
 tests/test_koboldai.py
```

### Comparing `python-tgpt-0.6.0/tests/test_imager.py` & `python_tgpt-0.6.1/tests/test_imager.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.6.0/tests/test_utils.py` & `python_tgpt-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

