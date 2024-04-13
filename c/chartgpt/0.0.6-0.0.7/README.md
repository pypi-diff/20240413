# Comparing `tmp/chartgpt-0.0.6.tar.gz` & `tmp/chartgpt-0.0.7.tar.gz`

## Comparing `chartgpt-0.0.6.tar` & `chartgpt-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 chartgpt-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 chartgpt-0.0.6/mkdocs.yml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 chartgpt-0.0.6/requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 chartgpt-0.0.6/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chartgpt-0.0.6/.github/workflows/test.yml
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 chartgpt-0.0.6/chartgpt/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 chartgpt-0.0.6/chartgpt/__main__.py
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 chartgpt-0.0.6/chartgpt/chartgpt.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 chartgpt-0.0.6/chartgpt/constants.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 chartgpt-0.0.6/chartgpt/llm.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 chartgpt-0.0.6/chartgpt/prompts/base.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 chartgpt-0.0.6/chartgpt/prompts/generate_python_code.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 chartgpt-0.0.6/docs/api-generated.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 chartgpt-0.0.6/docs/index.md
--rw-r--r--   0        0        0    80099 2020-02-02 00:00:00.000000 chartgpt-0.0.6/docs/assets/chart.png
--rw-r--r--   0        0        0    11450 2020-02-02 00:00:00.000000 chartgpt-0.0.6/docs/assets/chartgpt_logo.svg
--rw-r--r--   0        0        0   925601 2020-02-02 00:00:00.000000 chartgpt-0.0.6/docs/assets/dash.png
--rw-r--r--   0        0        0   746570 2020-02-02 00:00:00.000000 chartgpt-0.0.6/docs/assets/notebook.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chartgpt-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 chartgpt-0.0.6/tests/test_run_code.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 chartgpt-0.0.6/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.6/LICENSE
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 chartgpt-0.0.6/README.md
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 chartgpt-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 chartgpt-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 chartgpt-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 chartgpt-0.0.7/mkdocs.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 chartgpt-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 chartgpt-0.0.7/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chartgpt-0.0.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 chartgpt-0.0.7/chartgpt/__init__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 chartgpt-0.0.7/chartgpt/__main__.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 chartgpt-0.0.7/chartgpt/chartgpt.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 chartgpt-0.0.7/chartgpt/constants.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 chartgpt-0.0.7/chartgpt/llm.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 chartgpt-0.0.7/chartgpt/prompts/base.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 chartgpt-0.0.7/chartgpt/prompts/generate_python_code.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 chartgpt-0.0.7/docs/api-generated.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 chartgpt-0.0.7/docs/index.md
+-rw-r--r--   0        0        0    80099 2020-02-02 00:00:00.000000 chartgpt-0.0.7/docs/assets/chart.png
+-rw-r--r--   0        0        0    11450 2020-02-02 00:00:00.000000 chartgpt-0.0.7/docs/assets/chartgpt_logo.svg
+-rw-r--r--   0        0        0   925601 2020-02-02 00:00:00.000000 chartgpt-0.0.7/docs/assets/dash.png
+-rw-r--r--   0        0        0   746570 2020-02-02 00:00:00.000000 chartgpt-0.0.7/docs/assets/notebook.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chartgpt-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 chartgpt-0.0.7/tests/test_run_code.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 chartgpt-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 chartgpt-0.0.7/README.md
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 chartgpt-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 chartgpt-0.0.7/PKG-INFO
```

### Comparing `chartgpt-0.0.6/.pre-commit-config.yaml` & `chartgpt-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/mkdocs.yml` & `chartgpt-0.0.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/.devcontainer/devcontainer.json` & `chartgpt-0.0.7/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/.github/workflows/publish.yml` & `chartgpt-0.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/.github/workflows/test.yml` & `chartgpt-0.0.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/chartgpt/__init__.py` & `chartgpt-0.0.7/chartgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/chartgpt/chartgpt.py` & `chartgpt-0.0.7/chartgpt/chartgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import io
 from contextlib import redirect_stdout
 from typing import Optional
 
+import numpy as np
 import pandas as pd
 from dotenv import load_dotenv
 from plotly import express as px
 from plotly import graph_objects as go
 from plotly.graph_objects import Figure
 
 from .llm import LLM
@@ -23,15 +24,15 @@
         """_summary_
 
         Args:
             llm (Optional[str], optional): _description_. Defaults to "openai".
             conversational (bool, optional): _description_. Defaults to True.
             verbose (bool, optional): _description_. Defaults to False.
         """
-        self.llm = LLM(api_key=api_key, **kwargs)
+        self.llm = LLM(**kwargs)
         self.fig = None
         self.last_run_code = None
         self.variables_payload = {}
 
     def load(self, df: pd.DataFrame) -> None:
         """Load a DataFrame.
 
@@ -105,15 +106,15 @@
             Default to True
 
         Returns:
 
         """
         self.last_run_code = code
 
-        environment: dict = {"pd": pd, "go": go, "px": px, "df": df}
+        environment: dict = {"pd": pd, "go": go, "px": px, "df": df, "np": np}
 
         with redirect_stdout(io.StringIO()) as output:
             n_retries = 0
             while n_retries < 2:
                 try:
                     exec(code, environment)
                     code_ran = code
```

### Comparing `chartgpt-0.0.6/chartgpt/constants.py` & `chartgpt-0.0.7/chartgpt/constants.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/chartgpt/prompts/base.py` & `chartgpt-0.0.7/chartgpt/prompts/base.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/chartgpt/prompts/generate_python_code.py` & `chartgpt-0.0.7/chartgpt/prompts/generate_python_code.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,28 +2,24 @@
 
 from chartgpt.constants import END_CODE_TAG, START_CODE_TAG
 
 from .base import Prompt
 
 
 class GeneratePythonCodePrompt(Prompt):
-    context: str = """
-You are ChartGPT, a data scientist working at a startup. You are asked to analyze a \
-dataset and create a chart.
-Today is {today_date}.
-You are given a dataset `df` with the following columns: {df_columns}.
-
+    context: str = """You are ChartGPT, a Python software developer expert in data visualization using Plotly. \
+Today is {today_date}. \
+You are given a dataset `df` with the following columns: {df_columns}. \
 When asked about the data, your response must include a python code that uses the \
 library Plotly to make a chart using the dataframe `df`. If necessary, you can filter \
-the dataframe `df`. You can use any chart type you want.
+the dataframe `df` using any pandas operations, as long as it works. \
 Using the provided dataframe, df, return the python code and make sure to prefix the \
 requested python code with {START_CODE_TAG} exactly and suffix the code with \
 {END_CODE_TAG} exactly to get the answer to the following question:
-{user_prompt}
-"""
+{user_prompt}. Code:"""
 
     def __init__(self, **kwargs):
         super().__init__(
             today_date=date.today(),
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
             **kwargs,
```

### Comparing `chartgpt-0.0.6/docs/index.md` & `chartgpt-0.0.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/docs/assets/chart.png` & `chartgpt-0.0.7/docs/assets/chart.png`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/docs/assets/chartgpt_logo.svg` & `chartgpt-0.0.7/docs/assets/chartgpt_logo.svg`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/docs/assets/dash.png` & `chartgpt-0.0.7/docs/assets/dash.png`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/docs/assets/notebook.png` & `chartgpt-0.0.7/docs/assets/notebook.png`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/tests/test_run_code.py` & `chartgpt-0.0.7/tests/test_run_code.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/LICENSE` & `chartgpt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/README.md` & `chartgpt-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.6/pyproject.toml` & `chartgpt-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chartgpt"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Elie Brosset", email="eliebrosset@gmail.com" },
 ]
 description = "ChartGPT is a library for generating charts from text"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -17,14 +17,15 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pandas>=2.0.0",
     "plotly>=4.0.0",
     "openai>=0.2.0",
     "python-dotenv>=1.0.0",
+    "litellm>=1.34.25",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest >=7.1.3,<8.0.0",
     "coverage[toml] >= 6.5.0,< 8.0",
     "mypy ==0.982",
```

### Comparing `chartgpt-0.0.6/PKG-INFO` & `chartgpt-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: chartgpt
-Version: 0.0.6
+Version: 0.0.7
 Summary: ChartGPT is a library for generating charts from text
 Project-URL: Homepage, https://github.com/chatgpt/chart
 Author-email: Elie Brosset <eliebrosset@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: litellm>=1.34.25
 Requires-Dist: openai>=0.2.0
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: plotly>=4.0.0
 Requires-Dist: python-dotenv>=1.0.0
 Provides-Extra: dev
 Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: ruff==0.0.138; extra == 'dev'
```

