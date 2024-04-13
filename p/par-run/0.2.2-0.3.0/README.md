# Comparing `tmp/par_run-0.2.2.tar.gz` & `tmp/par_run-0.3.0.tar.gz`

## Comparing `par_run-0.2.2.tar` & `par_run-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.2.2/.python-version
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 par_run-0.2.2/commands.ini
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 par_run-0.2.2/requirements-dev.lock
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 par_run-0.2.2/requirements.lock
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/coverage_html.js
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/d_417a353b6036f046___init___py.html
--rw-r--r--   0        0        0    88534 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/d_417a353b6036f046_cli_py.html
--rw-r--r--   0        0        0   134028 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/d_417a353b6036f046_executor_py.html
--rw-r--r--   0        0        0    46396 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/d_417a353b6036f046_web_cli_py.html
--rw-r--r--   0        0        0    23925 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/d_417a353b6036f046_web_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/favicon_32.png
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/keybd_open.png
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/status.json
--rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 par_run-0.2.2/.reports/html/style.css
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 par_run-0.2.2/.vscode/launch.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 par_run-0.2.2/py_tests/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 par_run-0.2.2/py_tests/conftest.py
--rw-r--r--   0        0        0    14105 2020-02-02 00:00:00.000000 par_run-0.2.2/py_tests/test_cli.py
--rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 par_run-0.2.2/py_tests/test_executor.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 par_run-0.2.2/py_tests/test_main.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 par_run-0.2.2/py_tests/test_web.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.2.2/src/par_run/__init__.py
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 par_run-0.2.2/src/par_run/cli.py
--rw-r--r--   0        0        0    14943 2020-02-02 00:00:00.000000 par_run-0.2.2/src/par_run/executor.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 par_run-0.2.2/src/par_run/web.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.2.2/src/par_run/static/css/style.css
--rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.2.2/src/par_run/static/js/app.js
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.2.2/src/par_run/templates/index.html
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.2.2/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.2.2/LICENSE
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 par_run-0.2.2/README.md
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 par_run-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 par_run-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.3.0/.python-version
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 par_run-0.3.0/commands.ini
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 par_run-0.3.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 par_run-0.3.0/requirements.lock
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/coverage_html.js
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/d_417a353b6036f046___init___py.html
+-rw-r--r--   0        0        0   109310 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/d_417a353b6036f046_cli_py.html
+-rw-r--r--   0        0        0   146586 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/d_417a353b6036f046_executor_py.html
+-rw-r--r--   0        0        0    46396 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/d_417a353b6036f046_web_cli_py.html
+-rw-r--r--   0        0        0    23112 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/d_417a353b6036f046_web_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/favicon_32.png
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/keybd_open.png
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/style.css
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 par_run-0.3.0/.vscode/launch.json
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/conftest.py
+-rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/test_cli.py
+-rw-r--r--   0        0        0    13957 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/test_executor.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/test_main.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/test_web.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/__init__.py
+-rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/cli.py
+-rw-r--r--   0        0        0    16427 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/executor.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/web.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/static/css/style.css
+-rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/static/js/app.js
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/templates/index.html
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 par_run-0.3.0/README.md
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 par_run-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 par_run-0.3.0/PKG-INFO
```

### Comparing `par_run-0.2.2/requirements-dev.lock` & `par_run-0.3.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/requirements.lock` & `par_run-0.3.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/.reports/html/coverage_html.js` & `par_run-0.3.0/.reports/html/coverage_html.js`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/.reports/html/d_417a353b6036f046___init___py.html` & `par_run-0.3.0/.reports/html/d_417a353b6036f046___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 08:48 -0400
+            created at 2024-04-12 11:37 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -78,23 +78,23 @@
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Main module for the py_runner package."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.2.0"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.2.2"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 08:48 -0400
+            created at 2024-04-12 11:37 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,13 +6,13 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 11 ssttaatteemmeennttss ?  11 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-12 08:48 -0400
+12 11:37 -0400
 _1"""Main module for the py_runner package.""" 
 _2 
-_3__version__ = "0.2.0" 
+_3__version__ = "0.2.2" 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-12 08:48 -0400
+12 11:37 -0400
```

### Comparing `par_run-0.2.2/.reports/html/d_417a353b6036f046_cli_py.html` & `par_run-0.3.0/.reports/html/d_417a353b6036f046_cli_py.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/par_run/cli.py: 91%</title>
+    <title>Coverage for src/par_run/cli.py: 90%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/par_run/cli.py</b>:
-            <span class="pc_cov">91%</span>
+            <span class="pc_cov">90%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">180 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">163<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">17<span class="text"> missing</span></button>
+            <span class="text">219 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">197<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">22<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">2<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_executor_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 10:21 -0400
+            created at 2024-04-13 15:27 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -78,326 +78,379 @@
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""CLI for running commands in parallel"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">OrderedDict</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">enum</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">rich</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">typer</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">executor</span> <span class="key">import</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">CommandStatus</span><span class="op">,</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span> <span class="nam">read_commands_toml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="nam">PID_FILE</span> <span class="op">=</span> <span class="str">".par-run.uvicorn.pid"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="nam">cli_app</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Typer</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">contextlib</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">enum</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">OrderedDict</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Annotated</span><span class="op">,</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">rich</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">import</span> <span class="nam">typer</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">executor</span> <span class="key">import</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">CommandGroup</span><span class="op">,</span> <span class="nam">CommandStatus</span><span class="op">,</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span> <span class="nam">read_commands_toml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="nam">PID_FILE</span> <span class="op">=</span> <span class="str">".par-run.uvicorn.pid"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="nam">cli_app</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Typer</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="com"># Web only functions</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">def</span> <span class="nam">clean_up</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">    Clean up by removing the PID file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="nam">os</span><span class="op">.</span><span class="nam">remove</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"Cleaned up PID file."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="com"># Web only functions</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">def</span> <span class="nam">clean_up</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="str">"""Clean up by removing the PID file."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="nam">Path</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">)</span><span class="op">.</span><span class="nam">unlink</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"Cleaned up PID file."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="key">def</span> <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="str">"""Start the web server"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">if</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">isfile</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"UVicorn server is already running."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">sys</span><span class="op">.</span><span class="nam">exit</span><span class="op">(</span><span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">,</span> <span class="str">"w"</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="str">"utf-8"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">pid_file</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"Starting UVicorn server on port {port}..."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">uvicorn_command</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">            <span class="str">"uvicorn"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="str">"par_run.web:ws_app"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">            <span class="str">"--host"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="str">"0.0.0.0"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">            <span class="str">"--port"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">            <span class="nam">str</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="nam">process</span> <span class="op">=</span> <span class="nam">subprocess</span><span class="op">.</span><span class="nam">Popen</span><span class="op">(</span><span class="nam">uvicorn_command</span><span class="op">,</span> <span class="nam">stdout</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">DEVNULL</span><span class="op">,</span> <span class="nam">stderr</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">DEVNULL</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">pid_file</span><span class="op">.</span><span class="nam">write</span><span class="op">(</span><span class="nam">str</span><span class="op">(</span><span class="nam">process</span><span class="op">.</span><span class="nam">pid</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="com"># Wait for UVicorn to start</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="nam">wait_time</span> <span class="op">=</span> <span class="num">3</span> <span class="op">*</span> <span class="num">10</span><span class="op">**</span><span class="num">9</span>  <span class="com"># 3 seconds</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="nam">start_time</span> <span class="op">=</span> <span class="nam">time</span><span class="op">.</span><span class="nam">time_ns</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">while</span> <span class="nam">time</span><span class="op">.</span><span class="nam">time_ns</span><span class="op">(</span><span class="op">)</span> <span class="op">-</span> <span class="nam">start_time</span> <span class="op">&lt;</span> <span class="nam">wait_time</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="nam">test_port</span> <span class="op">=</span> <span class="nam">get_process_port</span><span class="op">(</span><span class="nam">process</span><span class="op">.</span><span class="nam">pid</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">            <span class="key">if</span> <span class="nam">port</span> <span class="op">==</span> <span class="nam">test_port</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">                <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"UVicorn server is running on port {port} in {(time.time_ns() - start_time)/10**6:.2f} ms."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">            <span class="nam">time</span><span class="op">.</span><span class="nam">sleep</span><span class="op">(</span><span class="num">0.1</span><span class="op">)</span>  <span class="com"># Poll every 0.1 seconds</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"UVicorn server did not respond within {wait_time} seconds."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"run 'par-run web status' to check the status."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="key">def</span> <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="str">"""Start the web server"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="key">if</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">)</span><span class="op">.</span><span class="nam">is_file</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"UVicorn server is already running."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">sys</span><span class="op">.</span><span class="nam">exit</span><span class="op">(</span><span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="key">with</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">)</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"w"</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="str">"utf-8"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">pid_file</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"Starting UVicorn server on port {port}..."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">uvicorn_command</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">            <span class="str">"uvicorn"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">            <span class="str">"par_run.web:ws_app"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="str">"--host"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">            <span class="str">"0.0.0.0"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="str">"--port"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">            <span class="nam">str</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="nam">process</span> <span class="op">=</span> <span class="nam">subprocess</span><span class="op">.</span><span class="nam">Popen</span><span class="op">(</span><span class="nam">uvicorn_command</span><span class="op">,</span> <span class="nam">stdout</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">DEVNULL</span><span class="op">,</span> <span class="nam">stderr</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">DEVNULL</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="nam">pid_file</span><span class="op">.</span><span class="nam">write</span><span class="op">(</span><span class="nam">str</span><span class="op">(</span><span class="nam">process</span><span class="op">.</span><span class="nam">pid</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="com"># Wait for UVicorn to start</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="nam">wait_time</span> <span class="op">=</span> <span class="num">3</span> <span class="op">*</span> <span class="num">10</span><span class="op">**</span><span class="num">9</span>  <span class="com"># 3 seconds</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="nam">start_time</span> <span class="op">=</span> <span class="nam">time</span><span class="op">.</span><span class="nam">time_ns</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">        <span class="key">while</span> <span class="nam">time</span><span class="op">.</span><span class="nam">time_ns</span><span class="op">(</span><span class="op">)</span> <span class="op">-</span> <span class="nam">start_time</span> <span class="op">&lt;</span> <span class="nam">wait_time</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">            <span class="nam">test_port</span> <span class="op">=</span> <span class="nam">get_process_port</span><span class="op">(</span><span class="nam">process</span><span class="op">.</span><span class="nam">pid</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="key">if</span> <span class="nam">port</span> <span class="op">==</span> <span class="nam">test_port</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">                <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"UVicorn server is running on port {port} in {(time.time_ns() - start_time)/10**6:.2f} ms."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">            <span class="nam">time</span><span class="op">.</span><span class="nam">sleep</span><span class="op">(</span><span class="num">0.1</span><span class="op">)</span>  <span class="com"># Poll every 0.1 seconds</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"UVicorn server did not respond within {wait_time} seconds."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"run 'par-run web status' to check the status."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="key">def</span> <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">    Stop the UVicorn server by reading its PID from the PID file and sending a termination signal.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">)</span><span class="op">.</span><span class="nam">is_file</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"UVicorn server is not running."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="key">def</span> <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="str">"""Stop the UVicorn server by reading its PID from the PID file and sending a termination signal."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">)</span><span class="op">.</span><span class="nam">is_file</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"UVicorn server is not running."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="key">with</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">)</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="op">)</span> <span class="key">as</span> <span class="nam">pid_file</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="nam">pid</span> <span class="op">=</span> <span class="nam">int</span><span class="op">(</span><span class="nam">pid_file</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">,</span> <span class="str">"r"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">pid_file</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">pid</span> <span class="op">=</span> <span class="nam">int</span><span class="op">(</span><span class="nam">pid_file</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"Stopping UVicorn server with {pid=:}..."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="nam">os</span><span class="op">.</span><span class="nam">kill</span><span class="op">(</span><span class="nam">pid</span><span class="op">,</span> <span class="nam">signal</span><span class="op">.</span><span class="nam">SIGTERM</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="key">except</span> <span class="nam">ProcessLookupError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="nam">clean_up</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t"><span class="key">def</span> <span class="nam">get_process_port</span><span class="op">(</span><span class="nam">pid</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="nam">process</span> <span class="op">=</span> <span class="nam">psutil</span><span class="op">.</span><span class="nam">Process</span><span class="op">(</span><span class="nam">pid</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="nam">connections</span> <span class="op">=</span> <span class="nam">process</span><span class="op">.</span><span class="nam">connections</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="key">if</span> <span class="nam">connections</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="nam">port</span> <span class="op">=</span> <span class="nam">connections</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">.</span><span class="nam">laddr</span><span class="op">.</span><span class="nam">port</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="key">return</span> <span class="nam">port</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t"><span class="key">def</span> <span class="nam">list_uvicorn_processes</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="str">"""Check for other UVicorn processes and list them"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">    <span class="nam">uvicorn_processes</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">    <span class="key">for</span> <span class="nam">process</span> <span class="key">in</span> <span class="nam">psutil</span><span class="op">.</span><span class="nam">process_iter</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">            <span class="nam">process_name</span> <span class="op">=</span> <span class="nam">process</span><span class="op">.</span><span class="nam">name</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">            <span class="key">if</span> <span class="str">"uvicorn"</span> <span class="key">in</span> <span class="nam">process_name</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">                <span class="nam">uvicorn_processes</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">process</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="key">except</span> <span class="op">(</span><span class="nam">psutil</span><span class="op">.</span><span class="nam">NoSuchProcess</span><span class="op">,</span> <span class="nam">psutil</span><span class="op">.</span><span class="nam">AccessDenied</span><span class="op">,</span> <span class="nam">psutil</span><span class="op">.</span><span class="nam">ZombieProcess</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">            <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">    <span class="key">if</span> <span class="nam">uvicorn_processes</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"Other UVicorn processes:"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="key">for</span> <span class="nam">process</span> <span class="key">in</span> <span class="nam">uvicorn_processes</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"PID: {process.pid}, Name: {process.name()}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"No other UVicorn processes found."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="key">def</span> <span class="nam">get_web_server_status</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t"><span class="str">    Get the status of the UVicorn server by reading its PID from the PID file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">isfile</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"No pid file found. Server likely not running."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">        <span class="nam">list_uvicorn_processes</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">    <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">,</span> <span class="str">"r"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">pid_file</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="nam">pid</span> <span class="op">=</span> <span class="nam">int</span><span class="op">(</span><span class="nam">pid_file</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">if</span> <span class="nam">psutil</span><span class="op">.</span><span class="nam">pid_exists</span><span class="op">(</span><span class="nam">pid</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">            <span class="nam">port</span> <span class="op">=</span> <span class="nam">get_process_port</span><span class="op">(</span><span class="nam">pid</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">            <span class="key">if</span> <span class="nam">port</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">                <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"UVicorn server is running with {pid=}, {port=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">                <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"UVicorn server is running with {pid=:}, couldn't determine port."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"UVicorn server is not running but pid files exists, deleting it."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">            <span class="nam">clean_up</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"Stopping UVicorn server with {pid=:}..."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="key">with</span> <span class="nam">contextlib</span><span class="op">.</span><span class="nam">suppress</span><span class="op">(</span><span class="nam">ProcessLookupError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">os</span><span class="op">.</span><span class="nam">kill</span><span class="op">(</span><span class="nam">pid</span><span class="op">,</span> <span class="nam">signal</span><span class="op">.</span><span class="nam">SIGTERM</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="nam">clean_up</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="key">def</span> <span class="nam">get_process_port</span><span class="op">(</span><span class="nam">pid</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="nam">process</span> <span class="op">=</span> <span class="nam">psutil</span><span class="op">.</span><span class="nam">Process</span><span class="op">(</span><span class="nam">pid</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="nam">connections</span> <span class="op">=</span> <span class="nam">process</span><span class="op">.</span><span class="nam">connections</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="key">if</span> <span class="nam">connections</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="nam">port</span> <span class="op">=</span> <span class="nam">connections</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">.</span><span class="nam">laddr</span><span class="op">.</span><span class="nam">port</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">        <span class="key">return</span> <span class="nam">port</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t"><span class="key">def</span> <span class="nam">list_uvicorn_processes</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="str">"""Check for other UVicorn processes and list them"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="nam">uvicorn_processes</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="key">with</span> <span class="nam">contextlib</span><span class="op">.</span><span class="nam">suppress</span><span class="op">(</span><span class="nam">psutil</span><span class="op">.</span><span class="nam">NoSuchProcess</span><span class="op">,</span> <span class="nam">psutil</span><span class="op">.</span><span class="nam">AccessDenied</span><span class="op">,</span> <span class="nam">psutil</span><span class="op">.</span><span class="nam">ZombieProcess</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="key">for</span> <span class="nam">process</span> <span class="key">in</span> <span class="nam">psutil</span><span class="op">.</span><span class="nam">process_iter</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">            <span class="nam">process_name</span> <span class="op">=</span> <span class="nam">process</span><span class="op">.</span><span class="nam">name</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">            <span class="key">if</span> <span class="str">"uvicorn"</span> <span class="key">in</span> <span class="nam">process_name</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">                <span class="nam">uvicorn_processes</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">process</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="key">if</span> <span class="nam">uvicorn_processes</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"Other UVicorn processes:"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="key">for</span> <span class="nam">process</span> <span class="key">in</span> <span class="nam">uvicorn_processes</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"PID: {process.pid}, Name: {process.name()}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"No other UVicorn processes found."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t"><span class="key">def</span> <span class="nam">get_web_server_status</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="str">"""Get the status of the UVicorn server by reading its PID from the PID file."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">)</span><span class="op">.</span><span class="nam">is_file</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">        <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"No pid file found. Server likely not running."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="nam">list_uvicorn_processes</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="key">with</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">PID_FILE</span><span class="op">)</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="op">)</span> <span class="key">as</span> <span class="nam">pid_file</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="nam">pid</span> <span class="op">=</span> <span class="nam">int</span><span class="op">(</span><span class="nam">pid_file</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="key">if</span> <span class="nam">psutil</span><span class="op">.</span><span class="nam">pid_exists</span><span class="op">(</span><span class="nam">pid</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">            <span class="nam">port</span> <span class="op">=</span> <span class="nam">get_process_port</span><span class="op">(</span><span class="nam">pid</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">            <span class="key">if</span> <span class="nam">port</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">                <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"UVicorn server is running with {pid=}, {port=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">                <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"UVicorn server is running with {pid=:}, couldn't determine port."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">"UVicorn server is not running but pid files exists, deleting it."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">            <span class="nam">clean_up</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t"><span class="key">class</span> <span class="nam">WebCommand</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">    <span class="str">"""Web command enumeration."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">    <span class="nam">START</span> <span class="op">=</span> <span class="str">"start"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">    <span class="nam">STOP</span> <span class="op">=</span> <span class="str">"stop"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">    <span class="nam">RESTART</span> <span class="op">=</span> <span class="str">"restart"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">    <span class="nam">STATUS</span> <span class="op">=</span> <span class="str">"status"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t"><span class="key">class</span> <span class="nam">WebCommand</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">    <span class="str">"""Web command enumeration."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="nam">START</span> <span class="op">=</span> <span class="str">"start"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="nam">STOP</span> <span class="op">=</span> <span class="str">"stop"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="nam">RESTART</span> <span class="op">=</span> <span class="str">"restart"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">    <span class="nam">STATUS</span> <span class="op">=</span> <span class="str">"status"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t"><span class="key">class</span> <span class="nam">CLICommandCBOnComp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Completed command {cmd.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="nam">output</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t"><span class="key">class</span> <span class="nam">CLICommandCBOnComp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Completed command {cmd.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="nam">output</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="str">"""Callback function for when a command receives output"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]Command {cmd.name} finished[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="key">elif</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[red bold]Command {cmd.name} failed, {exit_code=:}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="str">"""Callback function for when a command receives output"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">        <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]Command {cmd.name} finished[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">        <span class="key">elif</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[red bold]Command {cmd.name} failed, {exit_code=:}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t"><span class="key">class</span> <span class="nam">CLICommandCBOnRecv</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]{cmd.name}: Started[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"{cmd.name}: {output}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t"><span class="key">class</span> <span class="nam">CLICommandCBOnRecv</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]{cmd.name}: Started[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"{cmd.name}: {output}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="str">"""Callback function for when a command receives output"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]{cmd.name}: Finished[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="key">elif</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[red bold]{cmd.name}: Failed, {exit_code=:}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="str">"""Callback function for when a command receives output"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]{cmd.name}: Finished[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="key">elif</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[red bold]{cmd.name}: Failed, {exit_code=:}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t"><span class="key">def</span> <span class="nam">format_elapsed_time</span><span class="op">(</span><span class="nam">seconds</span><span class="op">:</span> <span class="nam">float</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">    <span class="str">"""Converts a number of seconds into a human-readable time format of HH:MM:SS.xxx</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t"><span class="str">    ----</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t"><span class="str">    seconds (float): The number of seconds elapsed.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t"><span class="key">def</span> <span class="nam">format_elapsed_time</span><span class="op">(</span><span class="nam">seconds</span><span class="op">:</span> <span class="nam">float</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t"><span class="str">    Converts a number of seconds into a human-readable time format of HH:MM:SS.xxx</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t"><span class="str">    seconds (float): The number of seconds elapsed.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t"><span class="str">    str: The formatted time string.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="nam">hours</span> <span class="op">=</span> <span class="nam">int</span><span class="op">(</span><span class="nam">seconds</span><span class="op">)</span> <span class="op">//</span> <span class="num">3600</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">    <span class="nam">minutes</span> <span class="op">=</span> <span class="op">(</span><span class="nam">int</span><span class="op">(</span><span class="nam">seconds</span><span class="op">)</span> <span class="op">%</span> <span class="num">3600</span><span class="op">)</span> <span class="op">//</span> <span class="num">60</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">    <span class="nam">seconds</span> <span class="op">=</span> <span class="nam">seconds</span> <span class="op">%</span> <span class="num">60</span>  <span class="com"># Keeping the fractional part of seconds</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">    <span class="com"># Return formatted string with seconds rounded to 2 d.p.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="key">return</span> <span class="str">f"{hours:02}:{minutes:02}:{seconds:06.3f}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t"><span class="op">@</span><span class="nam">cli_app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t"><span class="key">def</span> <span class="nam">run</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">    <span class="nam">style</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Processing strategy"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="str">"comp"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">    <span class="nam">show</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Show available groups and commands"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">    <span class="nam">file</span><span class="op">:</span> <span class="nam">Path</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"The commands.ini file to use"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">Path</span><span class="op">(</span><span class="str">"pyproject.toml"</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">    <span class="nam">groups</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="key">None</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Run a specific group of commands, comma spearated"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">    <span class="nam">cmds</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="key">None</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Run a specific commands, comma spearated"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">    <span class="str">"""Run commands in parallel"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">    <span class="com"># Overall exit code, need to track all command exit codes to update this</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">    <span class="nam">exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">    <span class="nam">st_all</span> <span class="op">=</span> <span class="nam">time</span><span class="op">.</span><span class="nam">perf_counter</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">    <span class="com"># console = rich.console.Console()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">    <span class="nam">master_groups</span> <span class="op">=</span> <span class="nam">read_commands_toml</span><span class="op">(</span><span class="nam">file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">    <span class="key">if</span> <span class="nam">show</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">        <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Group: {grp.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]{cmd.name}[/]: {cmd.cmd}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">    <span class="key">if</span> <span class="nam">groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">        <span class="nam">master_groups</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">g</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">g</span> <span class="key">in</span> <span class="nam">groups</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="key">if</span> <span class="nam">cmds</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">        <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">            <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">                <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">                    <span class="nam">cmd_name</span><span class="op">:</span> <span class="nam">cmd</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">                    <span class="key">for</span> <span class="nam">cmd_name</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">                    <span class="key">if</span> <span class="nam">cmd_name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">c</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">cmds</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">                <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="nam">master_groups</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]No groups or commands found.[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">        <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">        <span class="key">if</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnComp</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">        <span class="key">elif</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnRecv</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">BadParameter</span><span class="op">(</span><span class="str">"Invalid processing strategy"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="com"># Summarise the results</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">    <span class="nam">console</span> <span class="op">=</span> <span class="nam">rich</span><span class="op">.</span><span class="nam">console</span><span class="op">.</span><span class="nam">Console</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">        <span class="nam">console</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Group: {grp.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">        <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">            <span class="nam">elap_str</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">            <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">elapsed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">                <span class="nam">elap_str</span> <span class="op">=</span> <span class="str">f", {format_elapsed_time(cmd.elapsed)}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">                <span class="nam">elap_str</span> <span class="op">=</span> <span class="str">", XX:XX:XX.xxx"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">            <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">                <span class="nam">left_seg</span> <span class="op">=</span> <span class="str">f"[green bold]Command {cmd.name} succeeded "</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">                <span class="nam">left_seg</span> <span class="op">=</span> <span class="str">f"[red bold]Command {cmd.name} failed "</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">            <span class="nam">right_seg</span> <span class="op">=</span> <span class="str">f"({cmd.num_non_empty_lines}{elap_str})[/]"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">            <span class="com"># Adjust total line width dynamically based on max width and other content</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">            <span class="nam">pad_length</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">                <span class="num">100</span> <span class="op">-</span> <span class="nam">len</span><span class="op">(</span><span class="nam">left_seg</span><span class="op">)</span> <span class="op">-</span> <span class="nam">len</span><span class="op">(</span><span class="nam">right_seg</span><span class="op">)</span> <span class="op">-</span> <span class="num">10</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">                <span class="key">if</span> <span class="str">"succeeded"</span> <span class="key">in</span> <span class="nam">left_seg</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">                <span class="key">else</span> <span class="num">100</span> <span class="op">-</span> <span class="nam">len</span><span class="op">(</span><span class="nam">left_seg</span><span class="op">)</span> <span class="op">-</span> <span class="nam">len</span><span class="op">(</span><span class="nam">right_seg</span><span class="op">)</span> <span class="op">-</span> <span class="num">12</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"{left_seg}{' ' * pad_length}{right_seg}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">    <span class="nam">end_style</span> <span class="op">=</span> <span class="str">"[green bold]"</span> <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">==</span> <span class="num">0</span> <span class="key">else</span> <span class="str">"[red bold]"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">    <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"\n{end_style}Total elapsed time: {format_elapsed_time(time.perf_counter() - st_all)}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t"><span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">    <span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">    <span class="key">import</span> <span class="nam">signal</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">    <span class="key">import</span> <span class="nam">subprocess</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">    <span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">    <span class="key">import</span> <span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">    <span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">    <span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">    <span class="key">import</span> <span class="nam">psutil</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">    <span class="key">import</span> <span class="nam">typer</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">    <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]Web commands loaded[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">    <span class="nam">PID_FILE</span> <span class="op">=</span> <span class="str">".par-run.uvicorn.pid"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">    <span class="op">@</span><span class="nam">cli_app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">    <span class="key">def</span> <span class="nam">web</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">        <span class="nam">command</span><span class="op">:</span> <span class="nam">WebCommand</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Argument</span><span class="op">(</span><span class="op">...</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"command to control/interract with the web server"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">        <span class="nam">port</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="num">8001</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Port to run the web server"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">        <span class="str">"""Run the web server"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">        <span class="key">if</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">START</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STOP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">RESTART</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STATUS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">            <span class="nam">get_web_server_status</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"Not a valid command '{command}'"</span><span class="op">,</span> <span class="nam">err</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Abort</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t"><span class="str">    -------</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t"><span class="str">    str: The formatted time string.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="nam">hours</span> <span class="op">=</span> <span class="nam">int</span><span class="op">(</span><span class="nam">seconds</span><span class="op">)</span> <span class="op">//</span> <span class="num">3600</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">    <span class="nam">minutes</span> <span class="op">=</span> <span class="op">(</span><span class="nam">int</span><span class="op">(</span><span class="nam">seconds</span><span class="op">)</span> <span class="op">%</span> <span class="num">3600</span><span class="op">)</span> <span class="op">//</span> <span class="num">60</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">    <span class="nam">seconds</span> <span class="op">=</span> <span class="nam">seconds</span> <span class="op">%</span> <span class="num">60</span>  <span class="com"># Keeping the fractional part of seconds</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">    <span class="com"># Return formatted string with seconds rounded to 2 d.p.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">    <span class="key">return</span> <span class="str">f"{hours:02}:{minutes:02}:{seconds:06.3f}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t"><span class="key">def</span> <span class="nam">show_commands</span><span class="op">(</span><span class="nam">groups</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Group: {grp.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">            <span class="str">f"Params: cont_on_fail={grp.cont_on_fail}, serial={grp.serial}, timeout={grp.timeout}, retries={grp.retries}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="key">for</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]{cmd.name}[/]: {cmd.cmd}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t"><span class="key">def</span> <span class="nam">filter_groups</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">    <span class="nam">group_list</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">,</span> <span class="nam">filter_groups</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">filter_cmds</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">    <span class="key">if</span> <span class="nam">filter_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">        <span class="nam">group_list</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">group_list</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">g</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">g</span> <span class="key">in</span> <span class="nam">filter_groups</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">    <span class="key">if</span> <span class="nam">filter_cmds</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">        <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">group_list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">            <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">                <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">                    <span class="nam">cmd_name</span><span class="op">:</span> <span class="nam">cmd</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">                    <span class="key">for</span> <span class="nam">cmd_name</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">                    <span class="key">if</span> <span class="nam">cmd_name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">c</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">filter_cmds</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">                <span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">        <span class="nam">group_list</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">group_list</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">    <span class="key">return</span> <span class="nam">group_list</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t"><span class="key">def</span> <span class="nam">add_table_break</span><span class="op">(</span><span class="nam">tbl</span><span class="op">:</span> <span class="nam">rich</span><span class="op">.</span><span class="nam">table</span><span class="op">.</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">break_ch</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"-"</span><span class="op">,</span> <span class="nam">break_style</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">rich</span><span class="op">.</span><span class="nam">table</span><span class="op">.</span><span class="nam">Table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="nam">break_data</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span><span class="nam">break_ch</span> <span class="op">*</span> <span class="nam">int</span><span class="op">(</span><span class="nam">col</span><span class="op">.</span><span class="nam">width</span><span class="op">)</span> <span class="key">for</span> <span class="nam">col</span> <span class="key">in</span> <span class="nam">tbl</span><span class="op">.</span><span class="nam">columns</span> <span class="key">if</span> <span class="nam">col</span><span class="op">.</span><span class="nam">width</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">    <span class="nam">tbl</span><span class="op">.</span><span class="nam">add_row</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">        <span class="op">*</span><span class="nam">break_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">        <span class="nam">style</span><span class="op">=</span><span class="nam">break_style</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">    <span class="key">return</span> <span class="nam">tbl</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t"><span class="key">def</span> <span class="nam">build_results_tbl</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="nam">rich</span><span class="op">.</span><span class="nam">table</span><span class="op">.</span><span class="nam">Table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">    <span class="nam">res_tbl</span> <span class="op">=</span> <span class="nam">rich</span><span class="op">.</span><span class="nam">table</span><span class="op">.</span><span class="nam">Table</span><span class="op">(</span><span class="nam">title</span><span class="op">=</span><span class="str">"Results"</span><span class="op">,</span> <span class="nam">show_header</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">header_style</span><span class="op">=</span><span class="str">"bold blue"</span><span class="op">,</span> <span class="nam">box</span><span class="op">=</span><span class="nam">rich</span><span class="op">.</span><span class="nam">box</span><span class="op">.</span><span class="nam">ROUNDED</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">    <span class="nam">group_w</span><span class="op">,</span> <span class="nam">name_w</span><span class="op">,</span> <span class="nam">cmd_w</span><span class="op">,</span> <span class="nam">status_w</span><span class="op">,</span> <span class="nam">elap_w</span> <span class="op">=</span> <span class="op">(</span><span class="num">10</span><span class="op">,</span> <span class="num">15</span><span class="op">,</span> <span class="num">50</span><span class="op">,</span> <span class="num">6</span><span class="op">,</span> <span class="num">12</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">    <span class="nam">res_tbl</span><span class="op">.</span><span class="nam">add_column</span><span class="op">(</span><span class="str">"Group"</span><span class="op">,</span> <span class="nam">style</span><span class="op">=</span><span class="str">"bold blue"</span><span class="op">,</span> <span class="nam">width</span><span class="op">=</span><span class="nam">group_w</span><span class="op">,</span> <span class="nam">no_wrap</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">    <span class="nam">res_tbl</span><span class="op">.</span><span class="nam">add_column</span><span class="op">(</span><span class="str">"Name"</span><span class="op">,</span> <span class="nam">style</span><span class="op">=</span><span class="str">"bold blue"</span><span class="op">,</span> <span class="nam">width</span><span class="op">=</span><span class="nam">name_w</span><span class="op">,</span> <span class="nam">no_wrap</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">    <span class="nam">res_tbl</span><span class="op">.</span><span class="nam">add_column</span><span class="op">(</span><span class="str">"Command"</span><span class="op">,</span> <span class="nam">style</span><span class="op">=</span><span class="str">"bold blue"</span><span class="op">,</span> <span class="nam">width</span><span class="op">=</span><span class="nam">cmd_w</span><span class="op">,</span> <span class="nam">no_wrap</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="nam">res_tbl</span><span class="op">.</span><span class="nam">add_column</span><span class="op">(</span><span class="str">"Status"</span><span class="op">,</span> <span class="nam">style</span><span class="op">=</span><span class="str">"bold blue"</span><span class="op">,</span> <span class="nam">width</span><span class="op">=</span><span class="nam">status_w</span><span class="op">,</span> <span class="nam">no_wrap</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">    <span class="nam">res_tbl</span><span class="op">.</span><span class="nam">add_column</span><span class="op">(</span><span class="str">"Elapsed"</span><span class="op">,</span> <span class="nam">style</span><span class="op">=</span><span class="str">"bold blue"</span><span class="op">,</span> <span class="nam">width</span><span class="op">=</span><span class="nam">elap_w</span><span class="op">,</span> <span class="nam">no_wrap</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">    <span class="key">return</span> <span class="nam">res_tbl</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="key">def</span> <span class="nam">add_command_row</span><span class="op">(</span><span class="nam">tbl</span><span class="op">:</span> <span class="nam">rich</span><span class="op">.</span><span class="nam">table</span><span class="op">.</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">group_name</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">rich</span><span class="op">.</span><span class="nam">table</span><span class="op">.</span><span class="nam">Table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">    <span class="nam">elap_str</span> <span class="op">=</span> <span class="nam">format_elapsed_time</span><span class="op">(</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">elapsed</span><span class="op">)</span> <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">elapsed</span> <span class="key">else</span> <span class="str">"XX:XX:XX.xxx"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">    <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">        <span class="nam">cmd_status</span> <span class="op">=</span> <span class="str">"&#9989;"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="nam">row_style</span> <span class="op">=</span> <span class="str">"green"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">    <span class="key">elif</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">        <span class="nam">cmd_status</span> <span class="op">=</span> <span class="str">"&#10060;"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">        <span class="nam">row_style</span> <span class="op">=</span> <span class="str">"red"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">        <span class="nam">cmd_status</span> <span class="op">=</span> <span class="str">"&#9203;"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">        <span class="nam">row_style</span> <span class="op">=</span> <span class="str">"yellow"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">    <span class="nam">tbl</span><span class="op">.</span><span class="nam">add_row</span><span class="op">(</span><span class="nam">group_name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">cmd_status</span><span class="op">,</span> <span class="nam">elap_str</span><span class="op">,</span> <span class="nam">style</span><span class="op">=</span><span class="nam">row_style</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">    <span class="key">return</span> <span class="nam">tbl</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t"><span class="key">def</span> <span class="nam">fmt_group_name</span><span class="op">(</span><span class="nam">cmd_group</span><span class="op">:</span> <span class="nam">CommandGroup</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">    <span class="key">if</span> <span class="nam">cmd_group</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">        <span class="key">return</span> <span class="str">f"[green]{cmd_group.name}[/]"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">    <span class="key">elif</span> <span class="nam">cmd_group</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">        <span class="key">return</span> <span class="str">f"[red]{cmd_group.name}[/]"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">        <span class="key">return</span> <span class="str">f"[yellow]{cmd_group.name}[/]"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t"><span class="nam">style_default</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Processing strategy"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="str">"comp"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t"><span class="nam">show_default</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Show available groups and commands"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t"><span class="nam">pyproj_default</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"The default toml file to use"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">Path</span><span class="op">(</span><span class="str">"pyproject.toml"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t"><span class="nam">groups_default</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Run a specific group of commands, comma spearated"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t"><span class="nam">cmds_default</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Run specific commands, comma separated"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t"><span class="op">@</span><span class="nam">cli_app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t"><span class="key">def</span> <span class="nam">run</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">    <span class="nam">style</span><span class="op">:</span> <span class="nam">Annotated</span><span class="op">[</span><span class="nam">ProcessingStrategy</span><span class="op">,</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">]</span> <span class="op">=</span> <span class="nam">style_default</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">    <span class="nam">show</span><span class="op">:</span> <span class="nam">Annotated</span><span class="op">[</span><span class="nam">bool</span><span class="op">,</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">]</span> <span class="op">=</span> <span class="nam">show_default</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">    <span class="nam">file</span><span class="op">:</span> <span class="nam">Annotated</span><span class="op">[</span><span class="nam">Path</span><span class="op">,</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">]</span> <span class="op">=</span> <span class="nam">pyproj_default</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">    <span class="nam">groups</span><span class="op">:</span> <span class="nam">Annotated</span><span class="op">[</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">]</span> <span class="op">=</span> <span class="nam">groups_default</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">    <span class="nam">cmds</span><span class="op">:</span> <span class="nam">Annotated</span><span class="op">[</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">]</span> <span class="op">=</span> <span class="nam">cmds_default</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">    <span class="str">"""Run commands in parallel"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">    <span class="com"># Overall exit code, need to track all command exit codes to update this</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">    <span class="nam">exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">    <span class="nam">st_all</span> <span class="op">=</span> <span class="nam">time</span><span class="op">.</span><span class="nam">perf_counter</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">    <span class="nam">master_groups</span> <span class="op">=</span> <span class="nam">read_commands_toml</span><span class="op">(</span><span class="nam">file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">    <span class="key">if</span> <span class="nam">show</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">        <span class="key">return</span> <span class="nam">show_commands</span><span class="op">(</span><span class="nam">master_groups</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">    <span class="nam">master_groups</span> <span class="op">=</span> <span class="nam">filter_groups</span><span class="op">(</span><span class="nam">master_groups</span><span class="op">,</span> <span class="nam">groups</span><span class="op">,</span> <span class="nam">cmds</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]No groups or commands found.[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">        <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">        <span class="key">if</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnComp</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">        <span class="key">elif</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnRecv</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">BadParameter</span><span class="op">(</span><span class="str">"Invalid processing strategy"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">        <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cont_on_fail</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">            <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">    <span class="com"># Summarise the results</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">    <span class="nam">console</span> <span class="op">=</span> <span class="nam">rich</span><span class="op">.</span><span class="nam">console</span><span class="op">.</span><span class="nam">Console</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">    <span class="nam">res_tbl</span> <span class="op">=</span> <span class="nam">build_results_tbl</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t"><span class="key">except</span> <span class="nam">ImportError</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">    <span class="key">pass</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">    <span class="nam">cli_app</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp_ix</span><span class="op">,</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">enumerate</span><span class="op">(</span><span class="nam">master_groups</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">        <span class="key">for</span> <span class="nam">ix</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">enumerate</span><span class="op">(</span><span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">            <span class="key">if</span> <span class="nam">grp_ix</span> <span class="op">></span> <span class="num">0</span> <span class="key">and</span> <span class="nam">ix</span> <span class="op">==</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">                <span class="nam">add_table_break</span><span class="op">(</span><span class="nam">res_tbl</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">            <span class="nam">grp_name</span> <span class="op">=</span> <span class="nam">fmt_group_name</span><span class="op">(</span><span class="nam">grp</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">            <span class="key">if</span> <span class="nam">ix</span> <span class="op">></span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">                <span class="nam">grp_name</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">            <span class="nam">add_command_row</span><span class="op">(</span><span class="nam">res_tbl</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">,</span> <span class="nam">grp_name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">    <span class="nam">console</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="nam">res_tbl</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">    <span class="nam">end_style</span> <span class="op">=</span> <span class="str">"[green bold]"</span> <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">==</span> <span class="num">0</span> <span class="key">else</span> <span class="str">"[red bold]"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">    <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"\n{end_style}Total elapsed time: {format_elapsed_time(time.perf_counter() - st_all)}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">    <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t"><span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">    <span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">    <span class="key">import</span> <span class="nam">signal</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">    <span class="key">import</span> <span class="nam">subprocess</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">    <span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">    <span class="key">import</span> <span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">    <span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">    <span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">    <span class="key">import</span> <span class="nam">psutil</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">    <span class="key">import</span> <span class="nam">typer</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">    <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]Web commands loaded[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="nam">PID_FILE</span> <span class="op">=</span> <span class="str">".par-run.uvicorn.pid"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">    <span class="nam">command_default</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Argument</span><span class="op">(</span><span class="op">...</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"command to control/interract with the web server"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">    <span class="nam">port_default</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="num">8001</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Port to run the web server"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="op">@</span><span class="nam">cli_app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="key">def</span> <span class="nam">web</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">        <span class="nam">command</span><span class="op">:</span> <span class="nam">WebCommand</span> <span class="op">=</span> <span class="nam">command_default</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">        <span class="nam">port</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">port_default</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">        <span class="str">"""Run the web server"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">        <span class="key">if</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">START</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STOP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">RESTART</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STATUS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">            <span class="nam">get_web_server_status</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"Not a valid command '{command}'"</span><span class="op">,</span> <span class="nam">err</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Abort</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t"><span class="key">except</span> <span class="nam">ImportError</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">    <span class="key">pass</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">    <span class="nam">cli_app</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_executor_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 10:21 -0400
+            created at 2024-04-13 15:27 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,336 +1,402 @@
-************ CCoovveerraaggee ffoorr ssrrcc//ppaarr__rruunn//ccllii..ppyy:: 9911%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//ppaarr__rruunn//ccllii..ppyy:: 9900%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 118800 ssttaatteemmeennttss ?  116633 rruunn 1177 mmiissssiinngg 22 eexxcclluuddeedd **********
+********** 221199 ssttaatteemmeennttss ?  119977 rruunn 2222 mmiissssiinngg 22 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-12 10:21 -0400
+13 15:27 -0400
 _1"""CLI for running commands in parallel""" 
 _2 
-_3from collections import OrderedDict 
-_4from pathlib import Path 
-_5from typing import Optional 
-_6import enum 
-_7 
-_8import rich 
-_9import typer 
-_1_0 
-_1_1from .executor import Command, CommandStatus, ProcessingStrategy,
-read_commands_toml 
-_1_2 
-_1_3PID_FILE = ".par-run.uvicorn.pid" 
-_1_4 
-_1_5cli_app = typer.Typer() 
-_1_6 
+_3import contextlib 
+_4import enum 
+_5from collections import OrderedDict 
+_6from pathlib import Path 
+_7from typing import Annotated, Optional 
+_8 
+_9import rich 
+_1_0import typer 
+_1_1 
+_1_2from .executor import Command, CommandGroup, CommandStatus,
+ProcessingStrategy, read_commands_toml 
+_1_3 
+_1_4PID_FILE = ".par-run.uvicorn.pid" 
+_1_5 
+_1_6cli_app = typer.Typer() 
 _1_7 
-_1_8# Web only functions 
-_1_9def clean_up(): 
-_2_0 """ 
-_2_1 Clean up by removing the PID file. 
-_2_2 """ 
-_2_3 os.remove(PID_FILE) 
-_2_4 typer.echo("Cleaned up PID file.") 
+_1_8 
+_1_9# Web only functions 
+_2_0def clean_up(): 
+_2_1 """Clean up by removing the PID file.""" 
+_2_2 Path(PID_FILE).unlink() 
+_2_3 typer.echo("Cleaned up PID file.") 
+_2_4 
 _2_5 
-_2_6 
-_2_7def start_web_server(port: int): 
-_2_8 """Start the web server""" 
-_2_9 if os.path.isfile(PID_FILE): 
-_3_0 typer.echo("UVicorn server is already running.") 
-_3_1 sys.exit(1) 
-_3_2 with open(PID_FILE, "w", encoding="utf-8") as pid_file: 
-_3_3 typer.echo(f"Starting UVicorn server on port {port}...") 
-_3_4 uvicorn_command = [ 
-_3_5 "uvicorn", 
-_3_6 "par_run.web:ws_app", 
-_3_7 "--host", 
-_3_8 "0.0.0.0", 
-_3_9 "--port", 
-_4_0 str(port), 
-_4_1 ] 
-_4_2 process = subprocess.Popen(uvicorn_command, stdout=subprocess.DEVNULL,
+_2_6def start_web_server(port: int): 
+_2_7 """Start the web server""" 
+_2_8 if Path(PID_FILE).is_file(): 
+_2_9 typer.echo("UVicorn server is already running.") 
+_3_0 sys.exit(1) 
+_3_1 with Path(PID_FILE).open("w", encoding="utf-8") as pid_file: 
+_3_2 typer.echo(f"Starting UVicorn server on port {port}...") 
+_3_3 uvicorn_command = [ 
+_3_4 "uvicorn", 
+_3_5 "par_run.web:ws_app", 
+_3_6 "--host", 
+_3_7 "0.0.0.0", 
+_3_8 "--port", 
+_3_9 str(port), 
+_4_0 ] 
+_4_1 process = subprocess.Popen(uvicorn_command, stdout=subprocess.DEVNULL,
 stderr=subprocess.DEVNULL) 
-_4_3 pid_file.write(str(process.pid)) 
-_4_4 
-_4_5 # Wait for UVicorn to start 
-_4_6 wait_time = 3 * 10**9 # 3 seconds 
-_4_7 start_time = time.time_ns() 
-_4_8 
-_4_9 while time.time_ns() - start_time < wait_time: 
-_5_0 test_port = get_process_port(process.pid) 
-_5_1 if port == test_port: 
-_5_2 typer.echo(f"UVicorn server is running on port {port} in {(time.time_ns() -
+_4_2 pid_file.write(str(process.pid)) 
+_4_3 
+_4_4 # Wait for UVicorn to start 
+_4_5 wait_time = 3 * 10**9 # 3 seconds 
+_4_6 start_time = time.time_ns() 
+_4_7 
+_4_8 while time.time_ns() - start_time < wait_time: 
+_4_9 test_port = get_process_port(process.pid) 
+_5_0 if port == test_port: 
+_5_1 typer.echo(f"UVicorn server is running on port {port} in {(time.time_ns() -
 start_time)/10**6:.2f} ms.") 
-_5_3 break 
-_5_4 time.sleep(0.1) # Poll every 0.1 seconds 
-_5_5 
-_5_6 else: 
-_5_7 typer.echo(f"UVicorn server did not respond within {wait_time} seconds.") 
-_5_8 typer.echo("run 'par-run web status' to check the status.") 
+_5_2 break 
+_5_3 time.sleep(0.1) # Poll every 0.1 seconds 
+_5_4 
+_5_5 else: 
+_5_6 typer.echo(f"UVicorn server did not respond within {wait_time} seconds.") 
+_5_7 typer.echo("run 'par-run web status' to check the status.") 
+_5_8 
 _5_9 
-_6_0 
-_6_1def stop_web_server(): 
-_6_2 """ 
-_6_3 Stop the UVicorn server by reading its PID from the PID file and sending a
-termination signal. 
-_6_4 """ 
-_6_5 if not Path(PID_FILE).is_file(): 
-_6_6 typer.echo("UVicorn server is not running.") 
-_6_7 return 
+_6_0def stop_web_server(): 
+_6_1 """Stop the UVicorn server by reading its PID from the PID file and sending
+a termination signal.""" 
+_6_2 if not Path(PID_FILE).is_file(): 
+_6_3 typer.echo("UVicorn server is not running.") 
+_6_4 return 
+_6_5 
+_6_6 with Path(PID_FILE).open() as pid_file: 
+_6_7 pid = int(pid_file.read().strip()) 
 _6_8 
-_6_9 with open(PID_FILE, "r") as pid_file: 
-_7_0 pid = int(pid_file.read().strip()) 
-_7_1 
-_7_2 typer.echo(f"Stopping UVicorn server with {pid=:}...") 
-_7_3 try: 
-_7_4 os.kill(pid, signal.SIGTERM) 
-_7_5 except ProcessLookupError: 
-_7_6 pass 
-_7_7 clean_up() 
-_7_8 
-_7_9 
-_8_0def get_process_port(pid: int) -> Optional[int]: 
-_8_1 process = psutil.Process(pid) 
-_8_2 connections = process.connections() 
-_8_3 if connections: 
-_8_4 port = connections[0].laddr.port 
-_8_5 return port 
-_8_6 return None 
-_8_7 
-_8_8 
-_8_9def list_uvicorn_processes(): 
-_9_0 """Check for other UVicorn processes and list them""" 
-_9_1 uvicorn_processes = [] 
-_9_2 for process in psutil.process_iter(): 
-_9_3 try: 
-_9_4 process_name = process.name() 
-_9_5 if "uvicorn" in process_name.lower(): 
-_9_6 uvicorn_processes.append(process) 
-_9_7 except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess): 
-_9_8 pass 
-_9_9 if uvicorn_processes: 
-_1_0_0 typer.echo("Other UVicorn processes:") 
-_1_0_1 for process in uvicorn_processes: 
-_1_0_2 typer.echo(f"PID: {process.pid}, Name: {process.name()}") 
-_1_0_3 else: 
-_1_0_4 typer.echo("No other UVicorn processes found.") 
-_1_0_5 
-_1_0_6 
-_1_0_7def get_web_server_status(): 
-_1_0_8 """ 
-_1_0_9 Get the status of the UVicorn server by reading its PID from the PID file. 
-_1_1_0 """ 
-_1_1_1 if not os.path.isfile(PID_FILE): 
-_1_1_2 typer.echo("No pid file found. Server likely not running.") 
-_1_1_3 list_uvicorn_processes() 
-_1_1_4 return 
-_1_1_5 
-_1_1_6 with open(PID_FILE, "r") as pid_file: 
-_1_1_7 pid = int(pid_file.read().strip()) 
-_1_1_8 if psutil.pid_exists(pid): 
-_1_1_9 port = get_process_port(pid) 
-_1_2_0 if port: 
-_1_2_1 typer.echo(f"UVicorn server is running with {pid=}, {port=}") 
-_1_2_2 else: 
-_1_2_3 typer.echo(f"UVicorn server is running with {pid=:}, couldn't determine
+_6_9 typer.echo(f"Stopping UVicorn server with {pid=:}...") 
+_7_0 with contextlib.suppress(ProcessLookupError): 
+_7_1 os.kill(pid, signal.SIGTERM) 
+_7_2 clean_up() 
+_7_3 
+_7_4 
+_7_5def get_process_port(pid: int) -> Optional[int]: 
+_7_6 process = psutil.Process(pid) 
+_7_7 connections = process.connections() 
+_7_8 if connections: 
+_7_9 port = connections[0].laddr.port 
+_8_0 return port 
+_8_1 return None 
+_8_2 
+_8_3 
+_8_4def list_uvicorn_processes(): 
+_8_5 """Check for other UVicorn processes and list them""" 
+_8_6 uvicorn_processes = [] 
+_8_7 with contextlib.suppress(psutil.NoSuchProcess, psutil.AccessDenied,
+psutil.ZombieProcess): 
+_8_8 for process in psutil.process_iter(): 
+_8_9 process_name = process.name() 
+_9_0 if "uvicorn" in process_name.lower(): 
+_9_1 uvicorn_processes.append(process) 
+_9_2 
+_9_3 if uvicorn_processes: 
+_9_4 typer.echo("Other UVicorn processes:") 
+_9_5 for process in uvicorn_processes: 
+_9_6 typer.echo(f"PID: {process.pid}, Name: {process.name()}") 
+_9_7 else: 
+_9_8 typer.echo("No other UVicorn processes found.") 
+_9_9 
+_1_0_0 
+_1_0_1def get_web_server_status(): 
+_1_0_2 """Get the status of the UVicorn server by reading its PID from the PID
+file.""" 
+_1_0_3 if not Path(PID_FILE).is_file(): 
+_1_0_4 typer.echo("No pid file found. Server likely not running.") 
+_1_0_5 list_uvicorn_processes() 
+_1_0_6 return 
+_1_0_7 
+_1_0_8 with Path(PID_FILE).open() as pid_file: 
+_1_0_9 pid = int(pid_file.read().strip()) 
+_1_1_0 if psutil.pid_exists(pid): 
+_1_1_1 port = get_process_port(pid) 
+_1_1_2 if port: 
+_1_1_3 typer.echo(f"UVicorn server is running with {pid=}, {port=}") 
+_1_1_4 else: 
+_1_1_5 typer.echo(f"UVicorn server is running with {pid=:}, couldn't determine
 port.") 
-_1_2_4 else: 
-_1_2_5 typer.echo("UVicorn server is not running but pid files exists, deleting
+_1_1_6 else: 
+_1_1_7 typer.echo("UVicorn server is not running but pid files exists, deleting
 it.") 
-_1_2_6 clean_up() 
-_1_2_7 
+_1_1_8 clean_up() 
+_1_1_9 
+_1_2_0 
+_1_2_1class WebCommand(enum.Enum): 
+_1_2_2 """Web command enumeration.""" 
+_1_2_3 
+_1_2_4 START = "start" 
+_1_2_5 STOP = "stop" 
+_1_2_6 RESTART = "restart" 
+_1_2_7 STATUS = "status" 
 _1_2_8 
-_1_2_9class WebCommand(enum.Enum): 
-_1_3_0 """Web command enumeration.""" 
+_1_2_9 def __str__(self): 
+_1_3_0 return self.value 
 _1_3_1 
-_1_3_2 START = "start" 
-_1_3_3 STOP = "stop" 
-_1_3_4 RESTART = "restart" 
-_1_3_5 STATUS = "status" 
+_1_3_2 
+_1_3_3class CLICommandCBOnComp: 
+_1_3_4 def on_start(self, cmd: Command): 
+_1_3_5 rich.print(f"[blue bold]Completed command {cmd.name}[/]") 
 _1_3_6 
-_1_3_7 def __str__(self): 
-_1_3_8 return self.value 
+_1_3_7 def on_recv(self, _: Command, output: str): 
+_1_3_8 rich.print(output) 
 _1_3_9 
-_1_4_0 
-_1_4_1class CLICommandCBOnComp: 
-_1_4_2 def on_start(self, cmd: Command): 
-_1_4_3 rich.print(f"[blue bold]Completed command {cmd.name}[/]") 
-_1_4_4 
-_1_4_5 def on_recv(self, _: Command, output: str): 
-_1_4_6 rich.print(output) 
+_1_4_0 def on_term(self, cmd: Command, exit_code: int): 
+_1_4_1 """Callback function for when a command receives output""" 
+_1_4_2 if cmd.status == CommandStatus.SUCCESS: 
+_1_4_3 rich.print(f"[green bold]Command {cmd.name} finished[/]") 
+_1_4_4 elif cmd.status == CommandStatus.FAILURE: 
+_1_4_5 rich.print(f"[red bold]Command {cmd.name} failed, {exit_code=:}[/]") 
+_1_4_6 
 _1_4_7 
-_1_4_8 def on_term(self, cmd: Command, exit_code: int): 
-_1_4_9 """Callback function for when a command receives output""" 
-_1_5_0 if cmd.status == CommandStatus.SUCCESS: 
-_1_5_1 rich.print(f"[green bold]Command {cmd.name} finished[/]") 
-_1_5_2 elif cmd.status == CommandStatus.FAILURE: 
-_1_5_3 rich.print(f"[red bold]Command {cmd.name} failed, {exit_code=:}[/]") 
+_1_4_8class CLICommandCBOnRecv: 
+_1_4_9 def on_start(self, cmd: Command): 
+_1_5_0 rich.print(f"[blue bold]{cmd.name}: Started[/]") 
+_1_5_1 
+_1_5_2 def on_recv(self, cmd: Command, output: str): 
+_1_5_3 rich.print(f"{cmd.name}: {output}") 
 _1_5_4 
-_1_5_5 
-_1_5_6class CLICommandCBOnRecv: 
-_1_5_7 def on_start(self, cmd: Command): 
-_1_5_8 rich.print(f"[blue bold]{cmd.name}: Started[/]") 
-_1_5_9 
-_1_6_0 def on_recv(self, cmd: Command, output: str): 
-_1_6_1 rich.print(f"{cmd.name}: {output}") 
+_1_5_5 def on_term(self, cmd: Command, exit_code: int): 
+_1_5_6 """Callback function for when a command receives output""" 
+_1_5_7 if cmd.status == CommandStatus.SUCCESS: 
+_1_5_8 rich.print(f"[green bold]{cmd.name}: Finished[/]") 
+_1_5_9 elif cmd.status == CommandStatus.FAILURE: 
+_1_6_0 rich.print(f"[red bold]{cmd.name}: Failed, {exit_code=:}[/]") 
+_1_6_1 
 _1_6_2 
-_1_6_3 def on_term(self, cmd: Command, exit_code: int): 
-_1_6_4 """Callback function for when a command receives output""" 
-_1_6_5 if cmd.status == CommandStatus.SUCCESS: 
-_1_6_6 rich.print(f"[green bold]{cmd.name}: Finished[/]") 
-_1_6_7 elif cmd.status == CommandStatus.FAILURE: 
-_1_6_8 rich.print(f"[red bold]{cmd.name}: Failed, {exit_code=:}[/]") 
-_1_6_9 
-_1_7_0 
-_1_7_1def format_elapsed_time(seconds: float) -> str: 
-_1_7_2 """ 
-_1_7_3 Converts a number of seconds into a human-readable time format of HH:MM:
+_1_6_3def format_elapsed_time(seconds: float) -> str: 
+_1_6_4 """Converts a number of seconds into a human-readable time format of HH:MM:
 SS.xxx 
-_1_7_4 
-_1_7_5 Args: 
-_1_7_6 seconds (float): The number of seconds elapsed. 
-_1_7_7 
-_1_7_8 Returns: 
-_1_7_9 str: The formatted time string. 
-_1_8_0 """ 
-_1_8_1 hours = int(seconds) // 3600 
-_1_8_2 minutes = (int(seconds) % 3600) // 60 
-_1_8_3 seconds = seconds % 60 # Keeping the fractional part of seconds 
-_1_8_4 
-_1_8_5 # Return formatted string with seconds rounded to 2 d.p. 
-_1_8_6 return f"{hours:02}:{minutes:02}:{seconds:06.3f}" 
-_1_8_7 
-_1_8_8 
-_1_8_9@cli_app.command() 
-_1_9_0def run( 
-_1_9_1 style: ProcessingStrategy = typer.Option(help="Processing strategy",
-default="comp"), 
-_1_9_2 show: bool = typer.Option(help="Show available groups and commands",
-default=False), 
-_1_9_3 file: Path = typer.Option(help="The commands.ini file to use", default=Path
-("pyproject.toml")), 
-_1_9_4 groups: Optional[str] = typer.Option(None, help="Run a specific group of
-commands, comma spearated"), 
-_1_9_5 cmds: Optional[str] = typer.Option(None, help="Run a specific commands,
-comma spearated"), 
-_1_9_6): 
-_1_9_7 """Run commands in parallel""" 
-_1_9_8 # Overall exit code, need to track all command exit codes to update this 
-_1_9_9 exit_code = 0 
-_2_0_0 st_all = time.perf_counter() 
-_2_0_1 # console = rich.console.Console() 
-_2_0_2 master_groups = read_commands_toml(file) 
-_2_0_3 if show: 
-_2_0_4 for grp in master_groups: 
-_2_0_5 rich.print(f"[blue bold]Group: {grp.name}[/]") 
-_2_0_6 for _, cmd in grp.cmds.items(): 
-_2_0_7 rich.print(f"[green bold]{cmd.name}[/]: {cmd.cmd}") 
-_2_0_8 return 
-_2_0_9 
-_2_1_0 if groups: 
-_2_1_1 master_groups = [grp for grp in master_groups if grp.name in [g.strip() for
-g in groups.split(",")]] 
-_2_1_2 
-_2_1_3 if cmds: 
-_2_1_4 for grp in master_groups: 
-_2_1_5 grp.cmds = OrderedDict( 
-_2_1_6 { 
-_2_1_7 cmd_name: cmd 
-_2_1_8 for cmd_name, cmd in grp.cmds.items() 
-_2_1_9 if cmd_name in [c.strip() for c in cmds.split(",")] 
-_2_2_0 } 
-_2_2_1 ) 
-_2_2_2 master_groups = [grp for grp in master_groups if grp.cmds] 
-_2_2_3 
-_2_2_4 if not master_groups: 
-_2_2_5 rich.print("[blue]No groups or commands found.[/]") 
-_2_2_6 raise typer.Exit(0) 
-_2_2_7 
-_2_2_8 for grp in master_groups: 
-_2_2_9 if style == ProcessingStrategy.ON_COMP: 
-_2_3_0 exit_code = exit_code or grp.run(style, CLICommandCBOnComp()) 
-_2_3_1 elif style == ProcessingStrategy.ON_RECV: 
-_2_3_2 exit_code = exit_code or grp.run(style, CLICommandCBOnRecv()) 
-_2_3_3 else: 
-_2_3_4 raise typer.BadParameter("Invalid processing strategy") 
-_2_3_5 
-_2_3_6 # Summarise the results 
-_2_3_7 console = rich.console.Console() 
-_2_3_8 for grp in master_groups: 
-_2_3_9 console.print(f"[blue bold]Group: {grp.name}[/]") 
-_2_4_0 for _, cmd in grp.cmds.items(): 
-_2_4_1 elap_str = "" 
-_2_4_2 if cmd.elapsed: 
-_2_4_3 elap_str = f", {format_elapsed_time(cmd.elapsed)}" 
-_2_4_4 else: 
-_2_4_5 elap_str = ", XX:XX:XX.xxx" 
-_2_4_6 
-_2_4_7 if cmd.status == CommandStatus.SUCCESS: 
-_2_4_8 left_seg = f"[green bold]Command {cmd.name} succeeded " 
-_2_4_9 else: 
-_2_5_0 left_seg = f"[red bold]Command {cmd.name} failed " 
-_2_5_1 
-_2_5_2 right_seg = f"({cmd.num_non_empty_lines}{elap_str})[/]" 
-_2_5_3 
-_2_5_4 # Adjust total line width dynamically based on max width and other content 
-_2_5_5 pad_length = ( 
-_2_5_6 100 - len(left_seg) - len(right_seg) - 10 
-_2_5_7 if "succeeded" in left_seg 
-_2_5_8 else 100 - len(left_seg) - len(right_seg) - 12 
-_2_5_9 ) 
-_2_6_0 
-_2_6_1 rich.print(f"{left_seg}{' ' * pad_length}{right_seg}") 
-_2_6_2 end_style = "[green bold]" if exit_code == 0 else "[red bold]" 
-_2_6_3 rich.print(f"\n{end_style}Total elapsed time: {format_elapsed_time
-(time.perf_counter() - st_all)}[/]") 
-_2_6_4 raise typer.Exit(exit_code) 
-_2_6_5 
-_2_6_6 
-_2_6_7try: 
-_2_6_8 import os 
-_2_6_9 import signal 
-_2_7_0 import subprocess 
-_2_7_1 import sys 
-_2_7_2 import time 
-_2_7_3 from pathlib import Path 
-_2_7_4 from typing import Optional 
-_2_7_5 
-_2_7_6 import psutil 
-_2_7_7 import typer 
-_2_7_8 
-_2_7_9 rich.print("[blue]Web commands loaded[/]") 
-_2_8_0 
-_2_8_1 PID_FILE = ".par-run.uvicorn.pid" 
-_2_8_2 
-_2_8_3 @cli_app.command() 
-_2_8_4 def web( 
-_2_8_5 command: WebCommand = typer.Argument(..., help="command to control/
-interract with the web server"), 
-_2_8_6 port: int = typer.Option(8001, help="Port to run the web server"), 
-_2_8_7 ): 
-_2_8_8 """Run the web server""" 
-_2_8_9 if command == WebCommand.START: 
-_2_9_0 start_web_server(port) 
-_2_9_1 elif command == WebCommand.STOP: 
-_2_9_2 stop_web_server() 
-_2_9_3 elif command == WebCommand.RESTART: 
-_2_9_4 stop_web_server() 
-_2_9_5 start_web_server(port) 
-_2_9_6 elif command == WebCommand.STATUS: 
-_2_9_7 get_web_server_status() 
-_2_9_8 else: 
-_2_9_9 typer.echo(f"Not a valid command '{command}'", err=True) 
-_3_0_0 raise typer.Abort() 
+_1_6_5 
+_1_6_6 Args: 
+_1_6_7 ---- 
+_1_6_8 seconds (float): The number of seconds elapsed. 
+_1_6_9 
+_1_7_0 Returns: 
+_1_7_1 ------- 
+_1_7_2 str: The formatted time string. 
+_1_7_3 
+_1_7_4 """ 
+_1_7_5 hours = int(seconds) // 3600 
+_1_7_6 minutes = (int(seconds) % 3600) // 60 
+_1_7_7 seconds = seconds % 60 # Keeping the fractional part of seconds 
+_1_7_8 
+_1_7_9 # Return formatted string with seconds rounded to 2 d.p. 
+_1_8_0 return f"{hours:02}:{minutes:02}:{seconds:06.3f}" 
+_1_8_1 
+_1_8_2 
+_1_8_3def show_commands(groups: list[CommandGroup]): 
+_1_8_4 for grp in groups: 
+_1_8_5 rich.print(f"[blue bold]Group: {grp.name}[/]") 
+_1_8_6 rich.print( 
+_1_8_7 f"Params: cont_on_fail={grp.cont_on_fail}, serial={grp.serial}, timeout=
+{grp.timeout}, retries={grp.retries}" 
+_1_8_8 ) 
+_1_8_9 for cmd in grp.cmds.values(): 
+_1_9_0 rich.print(f"[green bold]{cmd.name}[/]: {cmd.cmd}") 
+_1_9_1 
+_1_9_2 
+_1_9_3def filter_groups( 
+_1_9_4 group_list: list[CommandGroup], filter_groups: Optional[str], filter_cmds:
+Optional[str] 
+_1_9_5) -> list[CommandGroup]: 
+_1_9_6 if filter_groups: 
+_1_9_7 group_list = [grp for grp in group_list if grp.name in [g.strip() for g in
+filter_groups.split(",")]] 
+_1_9_8 
+_1_9_9 if filter_cmds: 
+_2_0_0 for grp in group_list: 
+_2_0_1 grp.cmds = OrderedDict( 
+_2_0_2 { 
+_2_0_3 cmd_name: cmd 
+_2_0_4 for cmd_name, cmd in grp.cmds.items() 
+_2_0_5 if cmd_name in [c.strip() for c in filter_cmds.split(",")] 
+_2_0_6 }, 
+_2_0_7 ) 
+_2_0_8 group_list = [grp for grp in group_list if grp.cmds] 
+_2_0_9 return group_list 
+_2_1_0 
+_2_1_1 
+_2_1_2def add_table_break(tbl: rich.table.Table, break_ch: str = "-", break_style:
+Optional[str] = None) -> rich.table.Table: 
+_2_1_3 break_data: list[str] = [break_ch * int(col.width) for col in tbl.columns
+if col.width is not None] 
+_2_1_4 tbl.add_row( 
+_2_1_5 *break_data, 
+_2_1_6 style=break_style, 
+_2_1_7 ) 
+_2_1_8 return tbl 
+_2_1_9 
+_2_2_0 
+_2_2_1def build_results_tbl() -> rich.table.Table: 
+_2_2_2 res_tbl = rich.table.Table(title="Results", show_header=True,
+header_style="bold blue", box=rich.box.ROUNDED) 
+_2_2_3 group_w, name_w, cmd_w, status_w, elap_w = (10, 15, 50, 6, 12) 
+_2_2_4 res_tbl.add_column("Group", style="bold blue", width=group_w,
+no_wrap=True) 
+_2_2_5 res_tbl.add_column("Name", style="bold blue", width=name_w, no_wrap=True) 
+_2_2_6 res_tbl.add_column("Command", style="bold blue", width=cmd_w,
+no_wrap=True) 
+_2_2_7 res_tbl.add_column("Status", style="bold blue", width=status_w,
+no_wrap=True) 
+_2_2_8 res_tbl.add_column("Elapsed", style="bold blue", width=elap_w,
+no_wrap=True) 
+_2_2_9 return res_tbl 
+_2_3_0 
+_2_3_1 
+_2_3_2def add_command_row(tbl: rich.table.Table, cmd: Command, group_name: str) -
+> rich.table.Table: 
+_2_3_3 elap_str = format_elapsed_time(cmd.elapsed) if cmd.elapsed else "XX:XX:
+XX.xxx" 
+_2_3_4 
+_2_3_5 if cmd.status == CommandStatus.SUCCESS: 
+_2_3_6 cmd_status = "✅" 
+_2_3_7 row_style = "green" 
+_2_3_8 elif cmd.status == CommandStatus.FAILURE: 
+_2_3_9 cmd_status = "❌" 
+_2_4_0 row_style = "red" 
+_2_4_1 else: 
+_2_4_2 cmd_status = "⏳" 
+_2_4_3 row_style = "yellow" 
+_2_4_4 
+_2_4_5 tbl.add_row(group_name, cmd.name, cmd.cmd, cmd_status, elap_str,
+style=row_style) 
+_2_4_6 return tbl 
+_2_4_7 
+_2_4_8 
+_2_4_9def fmt_group_name(cmd_group: CommandGroup) -> str: 
+_2_5_0 if cmd_group.status == CommandStatus.SUCCESS: 
+_2_5_1 return f"[green]{cmd_group.name}[/]" 
+_2_5_2 elif cmd_group.status == CommandStatus.FAILURE: 
+_2_5_3 return f"[red]{cmd_group.name}[/]" 
+_2_5_4 else: 
+_2_5_5 return f"[yellow]{cmd_group.name}[/]" 
+_2_5_6 
+_2_5_7 
+_2_5_8style_default = typer.Option(help="Processing strategy", default="comp") 
+_2_5_9show_default = typer.Option(help="Show available groups and commands",
+default=False) 
+_2_6_0pyproj_default = typer.Option(help="The default toml file to use",
+default=Path("pyproject.toml")) 
+_2_6_1groups_default = typer.Option(help="Run a specific group of commands, comma
+spearated", default=None) 
+_2_6_2cmds_default = typer.Option(help="Run specific commands, comma separated",
+default=None) 
+_2_6_3 
+_2_6_4 
+_2_6_5@cli_app.command() 
+_2_6_6def run( 
+_2_6_7 style: Annotated[ProcessingStrategy, typer.Option] = style_default, 
+_2_6_8 show: Annotated[bool, typer.Option] = show_default, 
+_2_6_9 file: Annotated[Path, typer.Option] = pyproj_default, 
+_2_7_0 groups: Annotated[Optional[str], typer.Option] = groups_default, 
+_2_7_1 cmds: Annotated[Optional[str], typer.Option] = cmds_default, 
+_2_7_2): 
+_2_7_3 """Run commands in parallel""" 
+_2_7_4 # Overall exit code, need to track all command exit codes to update this 
+_2_7_5 exit_code = 0 
+_2_7_6 st_all = time.perf_counter() 
+_2_7_7 
+_2_7_8 master_groups = read_commands_toml(file) 
+_2_7_9 if show: 
+_2_8_0 return show_commands(master_groups) 
+_2_8_1 
+_2_8_2 master_groups = filter_groups(master_groups, groups, cmds) 
+_2_8_3 
+_2_8_4 if not master_groups: 
+_2_8_5 rich.print("[blue]No groups or commands found.[/]") 
+_2_8_6 raise typer.Exit(0) 
+_2_8_7 
+_2_8_8 for grp in master_groups: 
+_2_8_9 if style == ProcessingStrategy.ON_COMP: 
+_2_9_0 exit_code = grp.run(style, CLICommandCBOnComp()) 
+_2_9_1 elif style == ProcessingStrategy.ON_RECV: 
+_2_9_2 exit_code = grp.run(style, CLICommandCBOnRecv()) 
+_2_9_3 else: 
+_2_9_4 raise typer.BadParameter("Invalid processing strategy") 
+_2_9_5 if exit_code != 0 and not grp.cont_on_fail: 
+_2_9_6 break 
+_2_9_7 
+_2_9_8 # Summarise the results 
+_2_9_9 console = rich.console.Console() 
+_3_0_0 res_tbl = build_results_tbl() 
 _3_0_1 
-_3_0_2except ImportError: # pragma: no cover 
-_3_0_3 pass # pragma: no cover 
-_3_0_4 
-_3_0_5if __name__ == "__main__": 
-_3_0_6 cli_app() 
+_3_0_2 for grp_ix, grp in enumerate(master_groups): 
+_3_0_3 for ix, cmd in enumerate(grp.cmds.values()): 
+_3_0_4 if grp_ix > 0 and ix == 0: 
+_3_0_5 add_table_break(res_tbl) 
+_3_0_6 grp_name = fmt_group_name(grp) 
+_3_0_7 if ix > 0: 
+_3_0_8 grp_name = "" 
+_3_0_9 add_command_row(res_tbl, cmd, grp_name) 
+_3_1_0 
+_3_1_1 console.print(res_tbl) 
+_3_1_2 end_style = "[green bold]" if exit_code == 0 else "[red bold]" 
+_3_1_3 rich.print(f"\n{end_style}Total elapsed time: {format_elapsed_time
+(time.perf_counter() - st_all)}[/]") 
+_3_1_4 raise typer.Exit(exit_code) 
+_3_1_5 
+_3_1_6 
+_3_1_7try: 
+_3_1_8 import os 
+_3_1_9 import signal 
+_3_2_0 import subprocess 
+_3_2_1 import sys 
+_3_2_2 import time 
+_3_2_3 from pathlib import Path 
+_3_2_4 from typing import Optional 
+_3_2_5 
+_3_2_6 import psutil 
+_3_2_7 import typer 
+_3_2_8 
+_3_2_9 rich.print("[blue]Web commands loaded[/]") 
+_3_3_0 
+_3_3_1 PID_FILE = ".par-run.uvicorn.pid" 
+_3_3_2 
+_3_3_3 command_default = typer.Argument(..., help="command to control/interract
+with the web server") 
+_3_3_4 port_default = typer.Option(8001, help="Port to run the web server") 
+_3_3_5 
+_3_3_6 @cli_app.command() 
+_3_3_7 def web( 
+_3_3_8 command: WebCommand = command_default, 
+_3_3_9 port: int = port_default, 
+_3_4_0 ): 
+_3_4_1 """Run the web server""" 
+_3_4_2 if command == WebCommand.START: 
+_3_4_3 start_web_server(port) 
+_3_4_4 elif command == WebCommand.STOP: 
+_3_4_5 stop_web_server() 
+_3_4_6 elif command == WebCommand.RESTART: 
+_3_4_7 stop_web_server() 
+_3_4_8 start_web_server(port) 
+_3_4_9 elif command == WebCommand.STATUS: 
+_3_5_0 get_web_server_status() 
+_3_5_1 else: 
+_3_5_2 typer.echo(f"Not a valid command '{command}'", err=True) 
+_3_5_3 raise typer.Abort() 
+_3_5_4 
+_3_5_5except ImportError: # pragma: no cover 
+_3_5_6 pass # pragma: no cover 
+_3_5_7 
+_3_5_8if __name__ == "__main__": 
+_3_5_9 cli_app() 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-12 10:21 -0400
+13 15:27 -0400
```

### Comparing `par_run-0.2.2/.reports/html/d_417a353b6036f046_executor_py.html` & `par_run-0.3.0/.reports/html/d_417a353b6036f046_executor_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">251 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">213<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">38<span class="text"> missing</span></button>
+            <span class="text">271 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">229<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">42<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">7<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_web_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 08:32 -0400
+            created at 2024-04-13 15:32 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,438 +85,484 @@
     <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">asyncio</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">configparser</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">enum</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">multiprocessing</span> <span class="key">as</span> <span class="nam">mp</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">queue</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">subprocess</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">OrderedDict</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">concurrent</span><span class="op">.</span><span class="nam">futures</span> <span class="key">import</span> <span class="nam">Future</span><span class="op">,</span> <span class="nam">ProcessPoolExecutor</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">queue</span> <span class="key">import</span> <span class="nam">Queue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">import</span> <span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">List</span><span class="op">,</span> <span class="nam">Optional</span><span class="op">,</span> <span class="nam">Protocol</span><span class="op">,</span> <span class="nam">TypeVar</span><span class="op">,</span> <span class="nam">Union</span><span class="op">,</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="nam">pydantic</span> <span class="key">import</span> <span class="nam">BaseModel</span><span class="op">,</span> <span class="nam">Field</span><span class="op">,</span> <span class="nam">ConfigDict</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">import</span> <span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">OrderedDict</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">concurrent</span><span class="op">.</span><span class="nam">futures</span> <span class="key">import</span> <span class="nam">Future</span><span class="op">,</span> <span class="nam">ProcessPoolExecutor</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">from</span> <span class="nam">queue</span> <span class="key">import</span> <span class="nam">Queue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">Optional</span><span class="op">,</span> <span class="nam">Protocol</span><span class="op">,</span> <span class="nam">TypeVar</span><span class="op">,</span> <span class="nam">Union</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">import</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="com"># Type alias for a generic future.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="nam">GenFuture</span> <span class="op">=</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">Future</span><span class="op">,</span> <span class="nam">asyncio</span><span class="op">.</span><span class="nam">Future</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">ContextT</span> <span class="op">=</span> <span class="nam">TypeVar</span><span class="op">(</span><span class="str">"ContextT"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="nam">pydantic</span> <span class="key">import</span> <span class="nam">BaseModel</span><span class="op">,</span> <span class="nam">ConfigDict</span><span class="op">,</span> <span class="nam">Field</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="com"># Type alias for a generic future.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="nam">GenFuture</span> <span class="op">=</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">Future</span><span class="op">,</span> <span class="nam">asyncio</span><span class="op">.</span><span class="nam">Future</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="nam">ContextT</span> <span class="op">=</span> <span class="nam">TypeVar</span><span class="op">(</span><span class="str">"ContextT"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">class</span> <span class="nam">ProcessingStrategy</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"""Enum for processing strategies."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="nam">ON_COMP</span> <span class="op">=</span> <span class="str">"comp"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="nam">ON_RECV</span> <span class="op">=</span> <span class="str">"recv"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="key">class</span> <span class="nam">ProcessingStrategy</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="str">"""Enum for processing strategies."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="nam">ON_COMP</span> <span class="op">=</span> <span class="str">"comp"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="nam">ON_RECV</span> <span class="op">=</span> <span class="str">"recv"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandStatus</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"""Enum for command status."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">NOT_STARTED</span> <span class="op">=</span> <span class="str">"Not Started"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">RUNNING</span> <span class="op">=</span> <span class="str">"Running"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="nam">SUCCESS</span> <span class="op">=</span> <span class="str">"Success"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="nam">FAILURE</span> <span class="op">=</span> <span class="str">"Failure"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="key">def</span> <span class="nam">completed</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="str">"""Return True if the command has completed."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span> <span class="key">in</span> <span class="op">[</span><span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">,</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandStatus</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"""Enum for command status."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">NOT_STARTED</span> <span class="op">=</span> <span class="str">"Not Started"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="nam">RUNNING</span> <span class="op">=</span> <span class="str">"Running"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="nam">SUCCESS</span> <span class="op">=</span> <span class="str">"Success"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="nam">FAILURE</span> <span class="op">=</span> <span class="str">"Failure"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="key">def</span> <span class="nam">completed</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="str">"""Return True if the command has completed."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span> <span class="key">in</span> <span class="op">[</span><span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">,</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="key">class</span> <span class="nam">Command</span><span class="op">(</span><span class="nam">BaseModel</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="str">"""Holder for a command and its name."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="nam">model_config</span> <span class="op">=</span> <span class="nam">ConfigDict</span><span class="op">(</span><span class="nam">arbitrary_types_allowed</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="nam">cmd</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">passenv</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="nam">setenv</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="nam">status</span><span class="op">:</span> <span class="nam">CommandStatus</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">NOT_STARTED</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="nam">unflushed</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="op">[</span><span class="op">]</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="nam">num_non_empty_lines</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="num">0</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="nam">ret_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="nam">fut</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">GenFuture</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="nam">start_time</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">float</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">elapsed</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">float</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="key">def</span> <span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">line</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="str">"""Increment the non-empty line count."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="key">if</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">num_non_empty_lines</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="key">def</span> <span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">line</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="str">"""Append a line to the output and increment the non-empty line count."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="key">def</span> <span class="nam">clear_unflushed</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="str">"""Clear the unflushed output."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">.</span><span class="nam">clear</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="key">def</span> <span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">ret_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="str">"""Set the return code and status of the command."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">start_time</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">elapsed</span> <span class="op">=</span> <span class="nam">time</span><span class="op">.</span><span class="nam">perf_counter</span><span class="op">(</span><span class="op">)</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">start_time</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">ret_code</span> <span class="op">=</span> <span class="nam">ret_code</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span><span class="op">.</span><span class="nam">cancel</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="key">if</span> <span class="nam">ret_code</span> <span class="op">==</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="key">def</span> <span class="nam">set_running</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="str">"""Set the command status to running."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">start_time</span> <span class="op">=</span> <span class="nam">time</span><span class="op">.</span><span class="nam">perf_counter</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">RUNNING</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="key">class</span> <span class="nam">Command</span><span class="op">(</span><span class="nam">BaseModel</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="str">"""Holder for a command and its name."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="nam">model_config</span> <span class="op">=</span> <span class="nam">ConfigDict</span><span class="op">(</span><span class="nam">arbitrary_types_allowed</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">cmd</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="nam">passenv</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="nam">setenv</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="nam">status</span><span class="op">:</span> <span class="nam">CommandStatus</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">NOT_STARTED</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="nam">unflushed</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="op">[</span><span class="op">]</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="nam">num_non_empty_lines</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="num">0</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="nam">ret_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="nam">fut</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">GenFuture</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">start_time</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">float</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">elapsed</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">float</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">def</span> <span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">line</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="str">"""Increment the non-empty line count."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="key">if</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">num_non_empty_lines</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="key">def</span> <span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">line</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="str">"""Append a line to the output and increment the non-empty line count."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="key">def</span> <span class="nam">clear_unflushed</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="str">"""Clear the unflushed output."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">.</span><span class="nam">clear</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="key">def</span> <span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">ret_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="str">"""Set the return code and status of the command."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">start_time</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">elapsed</span> <span class="op">=</span> <span class="nam">time</span><span class="op">.</span><span class="nam">perf_counter</span><span class="op">(</span><span class="op">)</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">start_time</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">ret_code</span> <span class="op">=</span> <span class="nam">ret_code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span><span class="op">.</span><span class="nam">cancel</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="key">if</span> <span class="nam">ret_code</span> <span class="op">==</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">def</span> <span class="nam">set_running</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="str">"""Set the command status to running."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">start_time</span> <span class="op">=</span> <span class="nam">time</span><span class="op">.</span><span class="nam">perf_counter</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">RUNNING</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandCB</span><span class="op">(</span><span class="nam">Protocol</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandCB</span><span class="op">(</span><span class="nam">Protocol</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandAsyncCB</span><span class="op">(</span><span class="nam">Protocol</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandAsyncCB</span><span class="op">(</span><span class="nam">Protocol</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t"><span class="key">class</span> <span class="nam">QRetriever</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">retries</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">q</span> <span class="op">=</span> <span class="nam">q</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span> <span class="op">=</span> <span class="nam">timeout</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span> <span class="op">=</span> <span class="nam">retries</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">    <span class="key">def</span> <span class="nam">get</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">        <span class="nam">retry_count</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">            <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">                <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">q</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">block</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">            <span class="key">except</span> <span class="nam">queue</span><span class="op">.</span><span class="nam">Empty</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">                <span class="key">if</span> <span class="nam">retry_count</span> <span class="op">&lt;</span> <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">                    <span class="nam">retry_count</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">                    <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">TimeoutError</span><span class="op">(</span><span class="str">"Timeout waiting for command output"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="key">return</span> <span class="str">f"QRetriever(timeout={self.timeout}, retries={self.retries})"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="key">class</span> <span class="nam">QRetriever</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">retries</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">q</span> <span class="op">=</span> <span class="nam">q</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span> <span class="op">=</span> <span class="nam">timeout</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span> <span class="op">=</span> <span class="nam">retries</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">    <span class="key">def</span> <span class="nam">get</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="nam">retry_count</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">            <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">                <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">q</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">block</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">            <span class="key">except</span> <span class="nam">queue</span><span class="op">.</span><span class="nam">Empty</span><span class="op">:</span>  <span class="com"># noqa: PERF203</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">                <span class="key">if</span> <span class="nam">retry_count</span> <span class="op">&lt;</span> <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">                    <span class="nam">retry_count</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">                    <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">TimeoutError</span><span class="op">(</span><span class="str">"Timeout waiting for command output"</span><span class="op">)</span> <span class="key">from</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="key">return</span> <span class="str">f"QRetriever(timeout={self.timeout}, retries={self.retries})"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandGroup</span><span class="op">(</span><span class="nam">BaseModel</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">    <span class="str">"""Holder for a group of commands."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">    <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="nam">desc</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="nam">cmds</span><span class="op">:</span> <span class="nam">OrderedDict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Command</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default_factory</span><span class="op">=</span><span class="nam">OrderedDict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="nam">timeout</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="num">30</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">    <span class="nam">retries</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="num">3</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">run_async</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandAsyncCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="nam">q</span> <span class="op">=</span> <span class="nam">mp</span><span class="op">.</span><span class="nam">Manager</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">Queue</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="nam">pool</span> <span class="op">=</span> <span class="nam">ProcessPoolExecutor</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="nam">futs</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">            <span class="nam">asyncio</span><span class="op">.</span><span class="nam">get_event_loop</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">run_in_executor</span><span class="op">(</span><span class="nam">pool</span><span class="op">,</span> <span class="nam">run_command</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">setenv</span><span class="op">,</span> <span class="nam">q</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="key">for</span> <span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">)</span><span class="op">,</span> <span class="nam">fut</span> <span class="key">in</span> <span class="nam">zip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">futs</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="nam">fut</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_running</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_process_q_async</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">strategy</span><span class="op">,</span> <span class="nam">callbacks</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">    <span class="key">def</span> <span class="nam">run</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span> <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandCB</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="nam">q</span> <span class="op">=</span> <span class="nam">mp</span><span class="op">.</span><span class="nam">Manager</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">Queue</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="nam">pool</span> <span class="op">=</span> <span class="nam">ProcessPoolExecutor</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="nam">futs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">pool</span><span class="op">.</span><span class="nam">submit</span><span class="op">(</span><span class="nam">run_command</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">setenv</span><span class="op">,</span> <span class="nam">q</span><span class="op">)</span> <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="key">for</span> <span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">)</span><span class="op">,</span> <span class="nam">fut</span> <span class="key">in</span> <span class="nam">zip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">futs</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="nam">fut</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_running</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_process_q</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">strategy</span><span class="op">,</span> <span class="nam">callbacks</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandGroup</span><span class="op">(</span><span class="nam">BaseModel</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">    <span class="str">"""Holder for a group of commands."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="nam">desc</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="nam">cmds</span><span class="op">:</span> <span class="nam">OrderedDict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Command</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default_factory</span><span class="op">=</span><span class="nam">OrderedDict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">    <span class="nam">timeout</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="num">30</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">    <span class="nam">retries</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="num">3</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">    <span class="nam">cont_on_fail</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="nam">serial</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">    <span class="nam">status</span><span class="op">:</span> <span class="nam">CommandStatus</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">NOT_STARTED</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="key">def</span> <span class="nam">update_status</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmds</span><span class="op">:</span> <span class="nam">OrderedDict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Command</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="str">"""Update the status of the command group."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="key">if</span> <span class="nam">all</span><span class="op">(</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span> <span class="key">for</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">cmds</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">run_async</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandAsyncCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">        <span class="nam">q</span> <span class="op">=</span> <span class="nam">mp</span><span class="op">.</span><span class="nam">Manager</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">Queue</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">        <span class="nam">pool</span> <span class="op">=</span> <span class="nam">ProcessPoolExecutor</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">        <span class="nam">futs</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">            <span class="nam">asyncio</span><span class="op">.</span><span class="nam">get_event_loop</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">run_in_executor</span><span class="op">(</span><span class="nam">pool</span><span class="op">,</span> <span class="nam">run_command</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">setenv</span><span class="op">,</span> <span class="nam">q</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">        <span class="key">for</span> <span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">)</span><span class="op">,</span> <span class="nam">fut</span> <span class="key">in</span> <span class="nam">zip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">futs</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="nam">fut</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_running</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">    <span class="key">def</span> <span class="nam">_process_q</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_process_q_async</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">strategy</span><span class="op">,</span> <span class="nam">callbacks</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">    <span class="key">def</span> <span class="nam">run</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span> <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandCB</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="nam">q</span> <span class="op">=</span> <span class="nam">mp</span><span class="op">.</span><span class="nam">Manager</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">Queue</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="nam">pool</span> <span class="op">=</span> <span class="nam">ProcessPoolExecutor</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">        <span class="nam">cmd_series</span> <span class="op">=</span> <span class="op">[</span><span class="nam">OrderedDict</span><span class="op">(</span><span class="op">[</span><span class="op">(</span><span class="nam">k</span><span class="op">,</span> <span class="nam">v</span><span class="op">)</span><span class="op">]</span><span class="op">)</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">]</span> <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">serial</span> <span class="key">else</span> <span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">        <span class="nam">group_exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">        <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">                <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">        <span class="nam">q_ret</span> <span class="op">=</span> <span class="nam">QRetriever</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">            <span class="nam">q_result</span> <span class="op">=</span> <span class="nam">q_ret</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">            <span class="com"># Can only get here with a valid message from the Q</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">            <span class="nam">cmd_name</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">            <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">            <span class="nam">output_line</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">            <span class="key">if</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">            <span class="nam">cmd</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">[</span><span class="nam">cmd_name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">                    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">                        <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">clear_unflushed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">            <span class="key">if</span> <span class="nam">all</span><span class="op">(</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span><span class="op">.</span><span class="nam">completed</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="key">return</span> <span class="nam">grp_exit_code</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">_process_q_async</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandAsyncCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">                <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="nam">q_ret</span> <span class="op">=</span> <span class="nam">QRetriever</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">            <span class="key">await</span> <span class="nam">asyncio</span><span class="op">.</span><span class="nam">sleep</span><span class="op">(</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">            <span class="nam">q_result</span> <span class="op">=</span> <span class="nam">q_ret</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">        <span class="key">for</span> <span class="nam">cmd_entries</span> <span class="key">in</span> <span class="nam">cmd_series</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">            <span class="nam">futs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">pool</span><span class="op">.</span><span class="nam">submit</span><span class="op">(</span><span class="nam">run_command</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">setenv</span><span class="op">,</span> <span class="nam">q</span><span class="op">)</span> <span class="key">for</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">cmd_entries</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">            <span class="key">for</span> <span class="nam">cmd</span><span class="op">,</span> <span class="nam">fut</span> <span class="key">in</span> <span class="nam">zip</span><span class="op">(</span><span class="nam">cmd_entries</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">futs</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">                <span class="nam">cmd</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="nam">fut</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">                <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_running</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_process_q</span><span class="op">(</span><span class="nam">cmd_entries</span><span class="op">,</span> <span class="nam">q</span><span class="op">,</span> <span class="nam">strategy</span><span class="op">,</span> <span class="nam">callbacks</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">            <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">                <span class="nam">group_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">                <span class="key">if</span> <span class="key">not</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cont_on_fail</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">                    <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">        <span class="key">return</span> <span class="nam">group_exit_code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">    <span class="key">def</span> <span class="nam">_process_q</span><span class="op">(</span>  <span class="com"># noqa: PLR0912</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="nam">cmds</span><span class="op">:</span> <span class="nam">OrderedDict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Command</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">        <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">        <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">            <span class="key">for</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">cmds</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">                <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">        <span class="nam">q_ret</span> <span class="op">=</span> <span class="nam">QRetriever</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">            <span class="nam">q_result</span> <span class="op">=</span> <span class="nam">q_ret</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">            <span class="com"># Can only get here with a valid message from the Q</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">            <span class="nam">cmd_name</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">            <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">            <span class="nam">output_line</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">            <span class="key">if</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">            <span class="nam">cmd</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">[</span><span class="nam">cmd_name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">                    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">                        <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">clear_unflushed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">            <span class="com"># Can only get here with a valid message from the Q</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">            <span class="nam">cmd_name</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">            <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">            <span class="nam">output_line</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">            <span class="key">if</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">            <span class="nam">cmd</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">[</span><span class="nam">cmd_name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">                    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">                        <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">clear_unflushed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">            <span class="key">if</span> <span class="nam">all</span><span class="op">(</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span><span class="op">.</span><span class="nam">completed</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">        <span class="key">return</span> <span class="nam">grp_exit_code</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t"><span class="key">def</span> <span class="nam">read_commands_ini</span><span class="op">(</span><span class="nam">filename</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">    <span class="str">"""Read a commands.ini file and return a list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t"><span class="str">        filename (Union[str, Path]): The filename of the commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t"><span class="str">        list[CommandGroup]: A list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">configparser</span><span class="op">.</span><span class="nam">ConfigParser</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">    <span class="nam">config</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="nam">filename</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">    <span class="nam">command_groups</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">    <span class="key">for</span> <span class="nam">section</span> <span class="key">in</span> <span class="nam">config</span><span class="op">.</span><span class="nam">sections</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">        <span class="key">if</span> <span class="nam">section</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"group."</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">            <span class="nam">group_name</span> <span class="op">=</span> <span class="nam">section</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"group."</span><span class="op">,</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">            <span class="nam">commands</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">            <span class="key">for</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">config</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="nam">section</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">                <span class="nam">name</span> <span class="op">=</span> <span class="nam">name</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">                <span class="nam">commands</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">=</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">            <span class="nam">command_group</span> <span class="op">=</span> <span class="nam">CommandGroup</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">group_name</span><span class="op">,</span> <span class="nam">cmds</span><span class="op">=</span><span class="nam">commands</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">            <span class="nam">command_groups</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">command_group</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">    <span class="key">return</span> <span class="nam">command_groups</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">            <span class="key">if</span> <span class="nam">all</span><span class="op">(</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span><span class="op">.</span><span class="nam">completed</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">cmds</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">update_status</span><span class="op">(</span><span class="nam">cmds</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">        <span class="key">return</span> <span class="nam">grp_exit_code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">_process_q_async</span><span class="op">(</span>  <span class="com"># noqa: PLR0912</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">        <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandAsyncCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">        <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">            <span class="key">for</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">                <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">        <span class="nam">q_ret</span> <span class="op">=</span> <span class="nam">QRetriever</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">            <span class="key">await</span> <span class="nam">asyncio</span><span class="op">.</span><span class="nam">sleep</span><span class="op">(</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">            <span class="nam">q_result</span> <span class="op">=</span> <span class="nam">q_ret</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">            <span class="com"># Can only get here with a valid message from the Q</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">            <span class="nam">cmd_name</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">            <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">            <span class="nam">output_line</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">            <span class="key">if</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">            <span class="nam">cmd</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">[</span><span class="nam">cmd_name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">                    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">                        <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">clear_unflushed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">            <span class="key">if</span> <span class="nam">all</span><span class="op">(</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span><span class="op">.</span><span class="nam">completed</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">        <span class="key">return</span> <span class="nam">grp_exit_code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t"><span class="key">def</span> <span class="nam">read_commands_ini</span><span class="op">(</span><span class="nam">filename</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">    <span class="str">"""Read a commands.ini file and return a list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t"><span class="key">def</span> <span class="nam">write_commands_ini</span><span class="op">(</span><span class="nam">filename</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">]</span><span class="op">,</span> <span class="nam">command_groups</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">    <span class="str">"""Write a list of CommandGroup objects to a commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t"><span class="str">    ----</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t"><span class="str">        filename (Union[str, Path]): The filename of the commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t"><span class="str">        filename (Union[str, Path]): The filename of the commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t"><span class="str">        command_groups (list[CommandGroup]): A list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">configparser</span><span class="op">.</span><span class="nam">ConfigParser</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">    <span class="key">for</span> <span class="nam">group</span> <span class="key">in</span> <span class="nam">command_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">        <span class="nam">section_name</span> <span class="op">=</span> <span class="str">f"group.{group.name}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">        <span class="nam">config</span><span class="op">[</span><span class="nam">section_name</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">        <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">command</span> <span class="key">in</span> <span class="nam">group</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">            <span class="nam">config</span><span class="op">[</span><span class="nam">section_name</span><span class="op">]</span><span class="op">[</span><span class="nam">command</span><span class="op">.</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">command</span><span class="op">.</span><span class="nam">cmd</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">    <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">filename</span><span class="op">,</span> <span class="str">"w"</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="str">"utf-8"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">configfile</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">        <span class="nam">config</span><span class="op">.</span><span class="nam">write</span><span class="op">(</span><span class="nam">configfile</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t"><span class="key">def</span> <span class="nam">_validate_mandatory_keys</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">items</span><span class="op">.</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">keys</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">context</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">,</span> <span class="op">...</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">    <span class="str">"""Validate that the mandatory keys are present in the data.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t"><span class="str">    -------</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t"><span class="str">        list[CommandGroup]: A list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">configparser</span><span class="op">.</span><span class="nam">ConfigParser</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">    <span class="nam">config</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="nam">filename</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">    <span class="nam">command_groups</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">    <span class="key">for</span> <span class="nam">section</span> <span class="key">in</span> <span class="nam">config</span><span class="op">.</span><span class="nam">sections</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">        <span class="key">if</span> <span class="nam">section</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"group."</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">            <span class="nam">group_name</span> <span class="op">=</span> <span class="nam">section</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"group."</span><span class="op">,</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">            <span class="nam">commands</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">            <span class="key">for</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">config</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="nam">section</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">                <span class="nam">clean_name</span> <span class="op">=</span> <span class="nam">name</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">                <span class="nam">commands</span><span class="op">[</span><span class="nam">clean_name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">clean_name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">=</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">            <span class="nam">command_group</span> <span class="op">=</span> <span class="nam">CommandGroup</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">group_name</span><span class="op">,</span> <span class="nam">cmds</span><span class="op">=</span><span class="nam">commands</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">            <span class="nam">command_groups</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">command_group</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t"><span class="str">        data (tomlkit.items.Table): The data to validate.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="str">        keys (list[str]): The mandatory keys.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">    <span class="nam">vals</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span> <span class="key">in</span> <span class="nam">keys</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">        <span class="nam">val</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">val</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">f"{key} is mandatory, not found in {context}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">        <span class="nam">vals</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">val</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="key">return</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">vals</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t"><span class="key">def</span> <span class="nam">_get_optional_keys</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">items</span><span class="op">.</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">keys</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="op">...</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">    <span class="str">"""Get Optional keys or default.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t"><span class="str">        data (tomlkit.items.Table): The data to use as source</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t"><span class="str">        keys (list[str]): The optional keys.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="key">return</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">default</span><span class="op">)</span> <span class="key">for</span> <span class="nam">key</span> <span class="key">in</span> <span class="nam">keys</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">    <span class="key">return</span> <span class="nam">command_groups</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t"><span class="key">def</span> <span class="nam">write_commands_ini</span><span class="op">(</span><span class="nam">filename</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">]</span><span class="op">,</span> <span class="nam">command_groups</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">    <span class="str">"""Write a list of CommandGroup objects to a commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t"><span class="str">    ----</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t"><span class="str">        filename (Union[str, Path]): The filename of the commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t"><span class="str">        command_groups (list[CommandGroup]): A list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">configparser</span><span class="op">.</span><span class="nam">ConfigParser</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">    <span class="key">for</span> <span class="nam">group</span> <span class="key">in</span> <span class="nam">command_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">        <span class="nam">section_name</span> <span class="op">=</span> <span class="str">f"group.{group.name}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">        <span class="nam">config</span><span class="op">[</span><span class="nam">section_name</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">        <span class="key">for</span> <span class="nam">command</span> <span class="key">in</span> <span class="nam">group</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">            <span class="nam">config</span><span class="op">[</span><span class="nam">section_name</span><span class="op">]</span><span class="op">[</span><span class="nam">command</span><span class="op">.</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">command</span><span class="op">.</span><span class="nam">cmd</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="key">with</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">filename</span><span class="op">)</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"w"</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="str">"utf-8"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">configfile</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">        <span class="nam">config</span><span class="op">.</span><span class="nam">write</span><span class="op">(</span><span class="nam">configfile</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t"><span class="key">def</span> <span class="nam">read_commands_toml</span><span class="op">(</span><span class="nam">filename</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">    <span class="str">"""Read a commands.toml file and return a list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t"><span class="str">        filename (Union[str, Path]): The filename of the commands.toml file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t"><span class="str">        list[CommandGroup]: A list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">    <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">filename</span><span class="op">,</span> <span class="str">"r"</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="str">"utf-8"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">toml_file</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">        <span class="nam">toml_data</span> <span class="op">=</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">toml_file</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="nam">cmd_groups_data</span> <span class="op">=</span> <span class="nam">toml_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"tool"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"par-run"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">cmd_groups_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"No par-run data found in toml file"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">    <span class="nam">_</span> <span class="op">=</span> <span class="nam">cmd_groups_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"description"</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t"><span class="key">def</span> <span class="nam">_validate_mandatory_keys</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">items</span><span class="op">.</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">keys</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">context</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">,</span> <span class="op">...</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="str">"""Validate that the mandatory keys are present in the data.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="str">    ----</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t"><span class="str">        data (tomlkit.items.Table): The data to validate.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t"><span class="str">        keys (list[str]): The mandatory keys.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">    <span class="nam">vals</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span> <span class="key">in</span> <span class="nam">keys</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">        <span class="nam">val</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">val</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">f"{key} is mandatory, not found in {context}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">        <span class="nam">vals</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">val</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">    <span class="key">return</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">vals</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">    <span class="nam">command_groups</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="key">for</span> <span class="nam">group_data</span> <span class="key">in</span> <span class="nam">cmd_groups_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"groups"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">        <span class="op">(</span><span class="nam">group_name</span><span class="op">,</span><span class="op">)</span> <span class="op">=</span> <span class="nam">_validate_mandatory_keys</span><span class="op">(</span><span class="nam">group_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"name"</span><span class="op">]</span><span class="op">,</span> <span class="str">"top level par-run group"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">        <span class="nam">group_desc</span><span class="op">,</span> <span class="nam">group_timeout</span><span class="op">,</span> <span class="nam">group_retries</span> <span class="op">=</span> <span class="nam">_get_optional_keys</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">            <span class="nam">group_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"desc"</span><span class="op">,</span> <span class="str">"timeout"</span><span class="op">,</span> <span class="str">"retries"</span><span class="op">]</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">group_timeout</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">            <span class="nam">group_timeout</span> <span class="op">=</span> <span class="num">30</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">group_retries</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">            <span class="nam">group_retries</span> <span class="op">=</span> <span class="num">3</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">        <span class="nam">commands</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">        <span class="key">for</span> <span class="nam">cmd_data</span> <span class="key">in</span> <span class="nam">group_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"commands"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">            <span class="nam">name</span><span class="op">,</span> <span class="nam">exec</span> <span class="op">=</span> <span class="nam">_validate_mandatory_keys</span><span class="op">(</span><span class="nam">cmd_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"name"</span><span class="op">,</span> <span class="str">"exec"</span><span class="op">]</span><span class="op">,</span> <span class="str">f"command group {group_name}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">            <span class="nam">setenv</span><span class="op">,</span> <span class="nam">passenv</span> <span class="op">=</span> <span class="nam">_get_optional_keys</span><span class="op">(</span><span class="nam">cmd_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"setenv"</span><span class="op">,</span> <span class="str">"passenv"</span><span class="op">]</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t"><span class="key">def</span> <span class="nam">_get_optional_keys</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">items</span><span class="op">.</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">keys</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="op">...</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">    <span class="str">"""Get Optional keys or default.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t"><span class="str">    ----</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t"><span class="str">        data (tomlkit.items.Table): The data to use as source</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t"><span class="str">        keys (list[str]): The optional keys.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">    <span class="nam">res</span> <span class="op">=</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">default</span><span class="op">)</span> <span class="key">for</span> <span class="nam">key</span> <span class="key">in</span> <span class="nam">keys</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">    <span class="key">return</span> <span class="nam">res</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t"><span class="key">def</span> <span class="nam">read_commands_toml</span><span class="op">(</span><span class="nam">filename</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">    <span class="str">"""Read a commands.toml file and return a list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">            <span class="nam">commands</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">=</span><span class="nam">exec</span><span class="op">,</span> <span class="nam">setenv</span><span class="op">=</span><span class="nam">setenv</span><span class="op">,</span> <span class="nam">passenv</span><span class="op">=</span><span class="nam">passenv</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">        <span class="nam">command_group</span> <span class="op">=</span> <span class="nam">CommandGroup</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">            <span class="nam">name</span><span class="op">=</span><span class="nam">group_name</span><span class="op">,</span> <span class="nam">desc</span><span class="op">=</span><span class="nam">group_desc</span><span class="op">,</span> <span class="nam">cmds</span><span class="op">=</span><span class="nam">commands</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">=</span><span class="nam">group_timeout</span><span class="op">,</span> <span class="nam">retries</span><span class="op">=</span><span class="nam">group_retries</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">        <span class="nam">command_groups</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">command_group</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">    <span class="key">return</span> <span class="nam">command_groups</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t"><span class="str">    ----</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t"><span class="str">        filename (Union[str, Path]): The filename of the commands.toml file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t"><span class="str">    -------</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t"><span class="str">        list[CommandGroup]: A list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t"><span class="key">def</span> <span class="nam">run_command</span><span class="op">(</span><span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">command</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">setenv</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">]</span><span class="op">,</span> <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">    <span class="str">"""Run a command and put the output into a queue. The output is a tuple of the command</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t"><span class="str">    name and the output line. The final output is a tuple of the command name and a dictionary</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t"><span class="str">    with the return code.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t"><span class="str">        name (Command): Command to run.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t"><span class="str">        q (Queue): Queue to put the output into.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">    <span class="nam">new_env</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">    <span class="key">if</span> <span class="nam">setenv</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">        <span class="nam">new_env</span> <span class="op">=</span> <span class="nam">os</span><span class="op">.</span><span class="nam">environ</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">        <span class="nam">new_env</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">setenv</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">    <span class="key">with</span> <span class="nam">subprocess</span><span class="op">.</span><span class="nam">Popen</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">        <span class="nam">command</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">        <span class="nam">shell</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">        <span class="nam">env</span><span class="op">=</span><span class="nam">new_env</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">        <span class="nam">stdout</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">PIPE</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">        <span class="nam">stderr</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">STDOUT</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">        <span class="nam">text</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">    <span class="op">)</span> <span class="key">as</span> <span class="nam">process</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">        <span class="key">if</span> <span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">            <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">iter</span><span class="op">(</span><span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">.</span><span class="nam">readline</span><span class="op">,</span> <span class="str">""</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">                <span class="nam">q</span><span class="op">.</span><span class="nam">put</span><span class="op">(</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">            <span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">.</span><span class="nam">close</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">            <span class="nam">process</span><span class="op">.</span><span class="nam">wait</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">            <span class="nam">ret_code</span> <span class="op">=</span> <span class="nam">process</span><span class="op">.</span><span class="nam">returncode</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">            <span class="key">if</span> <span class="nam">ret_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">                <span class="nam">q</span><span class="op">.</span><span class="nam">put</span><span class="op">(</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">int</span><span class="op">(</span><span class="nam">ret_code</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Process has no return code"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">    <span class="key">with</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">filename</span><span class="op">)</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="nam">encoding</span><span class="op">=</span><span class="str">"utf-8"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">toml_file</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">        <span class="nam">toml_data</span> <span class="op">=</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">toml_file</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="nam">cmd_groups_data</span> <span class="op">=</span> <span class="nam">toml_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"tool"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"par-run"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">cmd_groups_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"No par-run data found in toml file"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">    <span class="nam">_</span> <span class="op">=</span> <span class="nam">cmd_groups_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"description"</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">    <span class="nam">command_groups</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">    <span class="key">for</span> <span class="nam">group_data</span> <span class="key">in</span> <span class="nam">cmd_groups_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"groups"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">        <span class="op">(</span><span class="nam">group_name</span><span class="op">,</span><span class="op">)</span> <span class="op">=</span> <span class="nam">_validate_mandatory_keys</span><span class="op">(</span><span class="nam">group_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"name"</span><span class="op">]</span><span class="op">,</span> <span class="str">"top level par-run group"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">        <span class="nam">group_desc</span><span class="op">,</span> <span class="nam">group_timeout</span><span class="op">,</span> <span class="nam">group_retries</span> <span class="op">=</span> <span class="nam">_get_optional_keys</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">            <span class="nam">group_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">            <span class="op">[</span><span class="str">"desc"</span><span class="op">,</span> <span class="str">"timeout"</span><span class="op">,</span> <span class="str">"retries"</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">            <span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">        <span class="op">(</span><span class="nam">group_cont_on_fail</span><span class="op">,</span> <span class="nam">group_serial</span><span class="op">)</span> <span class="op">=</span> <span class="nam">_get_optional_keys</span><span class="op">(</span><span class="nam">group_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"cont_on_fail"</span><span class="op">,</span> <span class="str">"serial"</span><span class="op">]</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">group_timeout</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">            <span class="nam">group_timeout</span> <span class="op">=</span> <span class="num">30</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">group_retries</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">            <span class="nam">group_retries</span> <span class="op">=</span> <span class="num">3</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">        <span class="nam">group_cont_on_fail</span> <span class="op">=</span> <span class="nam">bool</span><span class="op">(</span><span class="nam">group_cont_on_fail</span> <span class="key">and</span> <span class="nam">group_cont_on_fail</span> <span class="key">is</span> <span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">        <span class="nam">group_serial</span> <span class="op">=</span> <span class="nam">bool</span><span class="op">(</span><span class="nam">group_serial</span> <span class="key">and</span> <span class="nam">group_serial</span> <span class="key">is</span> <span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">        <span class="nam">commands</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">        <span class="key">for</span> <span class="nam">cmd_data</span> <span class="key">in</span> <span class="nam">group_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"commands"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">            <span class="nam">name</span><span class="op">,</span> <span class="nam">exec</span> <span class="op">=</span> <span class="nam">_validate_mandatory_keys</span><span class="op">(</span><span class="nam">cmd_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"name"</span><span class="op">,</span> <span class="str">"exec"</span><span class="op">]</span><span class="op">,</span> <span class="str">f"command group {group_name}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">            <span class="nam">setenv</span><span class="op">,</span> <span class="nam">passenv</span> <span class="op">=</span> <span class="nam">_get_optional_keys</span><span class="op">(</span><span class="nam">cmd_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"setenv"</span><span class="op">,</span> <span class="str">"passenv"</span><span class="op">]</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">            <span class="nam">commands</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">=</span><span class="nam">exec</span><span class="op">,</span> <span class="nam">setenv</span><span class="op">=</span><span class="nam">setenv</span><span class="op">,</span> <span class="nam">passenv</span><span class="op">=</span><span class="nam">passenv</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">        <span class="nam">command_group</span> <span class="op">=</span> <span class="nam">CommandGroup</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">            <span class="nam">name</span><span class="op">=</span><span class="nam">group_name</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">            <span class="nam">desc</span><span class="op">=</span><span class="nam">group_desc</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">            <span class="nam">cmds</span><span class="op">=</span><span class="nam">commands</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">            <span class="nam">timeout</span><span class="op">=</span><span class="nam">group_timeout</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">            <span class="nam">retries</span><span class="op">=</span><span class="nam">group_retries</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t">            <span class="nam">cont_on_fail</span><span class="op">=</span><span class="nam">group_cont_on_fail</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">            <span class="nam">serial</span><span class="op">=</span><span class="nam">group_serial</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">        <span class="nam">command_groups</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">command_group</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">    <span class="key">return</span> <span class="nam">command_groups</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t"><span class="key">def</span> <span class="nam">run_command</span><span class="op">(</span><span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">command</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">setenv</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">]</span><span class="op">,</span> <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">    <span class="str">"""Run a command and put the output into a queue. The output is a tuple of the command</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t"><span class="str">    name and the output line. The final output is a tuple of the command name and a dictionary</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t"><span class="str">    with the return code.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t"><span class="str">    ----</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t"><span class="str">        name (Command): Command to run.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t"><span class="str">        q (Queue): Queue to put the output into.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">    <span class="nam">new_env</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t">    <span class="key">if</span> <span class="nam">setenv</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">        <span class="nam">new_env</span> <span class="op">=</span> <span class="nam">os</span><span class="op">.</span><span class="nam">environ</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t">        <span class="nam">new_env</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">setenv</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t">    <span class="key">with</span> <span class="nam">subprocess</span><span class="op">.</span><span class="nam">Popen</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">        <span class="nam">command</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">        <span class="nam">shell</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">        <span class="nam">env</span><span class="op">=</span><span class="nam">new_env</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">        <span class="nam">stdout</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">PIPE</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">        <span class="nam">stderr</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">STDOUT</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t">        <span class="nam">text</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">    <span class="op">)</span> <span class="key">as</span> <span class="nam">process</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">        <span class="key">if</span> <span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t">            <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">iter</span><span class="op">(</span><span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">.</span><span class="nam">readline</span><span class="op">,</span> <span class="str">""</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t">                <span class="nam">q</span><span class="op">.</span><span class="nam">put</span><span class="op">(</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t">            <span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">.</span><span class="nam">close</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t">            <span class="nam">process</span><span class="op">.</span><span class="nam">wait</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t">            <span class="nam">ret_code</span> <span class="op">=</span> <span class="nam">process</span><span class="op">.</span><span class="nam">returncode</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t468" href="#t468">468</a></span><span class="t">            <span class="key">if</span> <span class="nam">ret_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t469" href="#t469">469</a></span><span class="t">                <span class="nam">q</span><span class="op">.</span><span class="nam">put</span><span class="op">(</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">int</span><span class="op">(</span><span class="nam">ret_code</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t470" href="#t470">470</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t471" href="#t471">471</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Process has no return code"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_web_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 08:32 -0400
+            created at 2024-04-13 15:32 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -4,454 +4,502 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 225511 ssttaatteemmeennttss ?  221133 rruunn 3388 mmiissssiinngg 77 eexxcclluuddeedd **********
+********** 227711 ssttaatteemmeennttss ?  222299 rruunn 4422 mmiissssiinngg 77 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-12 08:32 -0400
+13 15:32 -0400
 _1"""Todo""" 
 _2 
 _3import asyncio 
 _4import configparser 
 _5import enum 
 _6import multiprocessing as mp 
 _7import os 
 _8import queue 
 _9import subprocess 
-_1_0from collections import OrderedDict 
-_1_1from concurrent.futures import Future, ProcessPoolExecutor 
-_1_2from pathlib import Path 
-_1_3from queue import Queue 
-_1_4import time 
-_1_5from typing import List, Optional, Protocol, TypeVar, Union, Any 
-_1_6from pydantic import BaseModel, Field, ConfigDict 
+_1_0import time 
+_1_1from collections import OrderedDict 
+_1_2from concurrent.futures import Future, ProcessPoolExecutor 
+_1_3from pathlib import Path 
+_1_4from queue import Queue 
+_1_5from typing import Any, Optional, Protocol, TypeVar, Union 
+_1_6 
 _1_7import tomlkit 
-_1_8 
-_1_9# Type alias for a generic future. 
-_2_0GenFuture = Union[Future, asyncio.Future] 
-_2_1 
-_2_2ContextT = TypeVar("ContextT") 
-_2_3 
+_1_8from pydantic import BaseModel, ConfigDict, Field 
+_1_9 
+_2_0# Type alias for a generic future. 
+_2_1GenFuture = Union[Future, asyncio.Future] 
+_2_2 
+_2_3ContextT = TypeVar("ContextT") 
 _2_4 
-_2_5class ProcessingStrategy(enum.Enum): 
-_2_6 """Enum for processing strategies.""" 
-_2_7 
-_2_8 ON_COMP = "comp" 
-_2_9 ON_RECV = "recv" 
-_3_0 
+_2_5 
+_2_6class ProcessingStrategy(enum.Enum): 
+_2_7 """Enum for processing strategies.""" 
+_2_8 
+_2_9 ON_COMP = "comp" 
+_3_0 ON_RECV = "recv" 
 _3_1 
-_3_2class CommandStatus(enum.Enum): 
-_3_3 """Enum for command status.""" 
-_3_4 
-_3_5 NOT_STARTED = "Not Started" 
-_3_6 RUNNING = "Running" 
-_3_7 SUCCESS = "Success" 
-_3_8 FAILURE = "Failure" 
-_3_9 
-_4_0 def completed(self) -> bool: 
-_4_1 """Return True if the command has completed.""" 
-_4_2 return self in [CommandStatus.SUCCESS, CommandStatus.FAILURE] 
-_4_3 
+_3_2 
+_3_3class CommandStatus(enum.Enum): 
+_3_4 """Enum for command status.""" 
+_3_5 
+_3_6 NOT_STARTED = "Not Started" 
+_3_7 RUNNING = "Running" 
+_3_8 SUCCESS = "Success" 
+_3_9 FAILURE = "Failure" 
+_4_0 
+_4_1 def completed(self) -> bool: 
+_4_2 """Return True if the command has completed.""" 
+_4_3 return self in [CommandStatus.SUCCESS, CommandStatus.FAILURE] 
 _4_4 
-_4_5class Command(BaseModel): 
-_4_6 """Holder for a command and its name.""" 
-_4_7 
-_4_8 model_config = ConfigDict(arbitrary_types_allowed=True) 
-_4_9 
-_5_0 name: str 
-_5_1 cmd: str 
-_5_2 passenv: Optional[list[str]] = Field(default=None) 
-_5_3 setenv: Optional[dict[str, str]] = Field(default=None) 
-_5_4 status: CommandStatus = CommandStatus.NOT_STARTED 
-_5_5 unflushed: List[str] = Field(default=[], exclude=True) 
-_5_6 num_non_empty_lines: int = Field(default=0, exclude=True) 
-_5_7 ret_code: Optional[int] = Field(default=None, exclude=True) 
-_5_8 fut: Optional[GenFuture] = Field(default=None, exclude=True) 
-_5_9 start_time: Optional[float] = Field(default=None, exclude=True) 
-_6_0 elapsed: Optional[float] = Field(default=None, exclude=True) 
-_6_1 
-_6_2 def incr_line_count(self, line: str) -> None: 
-_6_3 """Increment the non-empty line count.""" 
-_6_4 if line.strip(): 
-_6_5 self.num_non_empty_lines += 1 
-_6_6 
-_6_7 def append_unflushed(self, line: str) -> None: 
-_6_8 """Append a line to the output and increment the non-empty line count.""" 
-_6_9 self.unflushed.append(line) 
-_7_0 
-_7_1 def clear_unflushed(self) -> None: 
-_7_2 """Clear the unflushed output.""" 
-_7_3 self.unflushed.clear() 
-_7_4 
-_7_5 def set_ret_code(self, ret_code: int): 
-_7_6 """Set the return code and status of the command.""" 
-_7_7 if self.start_time: 
-_7_8 self.elapsed = time.perf_counter() - self.start_time 
-_7_9 self.ret_code = ret_code 
-_8_0 if self.fut: 
-_8_1 self.fut.cancel() 
-_8_2 self.fut = None 
-_8_3 if ret_code == 0: 
-_8_4 self.status = CommandStatus.SUCCESS 
-_8_5 else: 
-_8_6 self.status = CommandStatus.FAILURE 
-_8_7 
-_8_8 def set_running(self): 
-_8_9 """Set the command status to running.""" 
-_9_0 self.start_time = time.perf_counter() 
-_9_1 self.status = CommandStatus.RUNNING 
-_9_2 
+_4_5 
+_4_6class Command(BaseModel): 
+_4_7 """Holder for a command and its name.""" 
+_4_8 
+_4_9 model_config = ConfigDict(arbitrary_types_allowed=True) 
+_5_0 
+_5_1 name: str 
+_5_2 cmd: str 
+_5_3 passenv: Optional[list[str]] = Field(default=None) 
+_5_4 setenv: Optional[dict[str, str]] = Field(default=None) 
+_5_5 status: CommandStatus = CommandStatus.NOT_STARTED 
+_5_6 unflushed: list[str] = Field(default=[], exclude=True) 
+_5_7 num_non_empty_lines: int = Field(default=0, exclude=True) 
+_5_8 ret_code: Optional[int] = Field(default=None, exclude=True) 
+_5_9 fut: Optional[GenFuture] = Field(default=None, exclude=True) 
+_6_0 start_time: Optional[float] = Field(default=None, exclude=True) 
+_6_1 elapsed: Optional[float] = Field(default=None, exclude=True) 
+_6_2 
+_6_3 def incr_line_count(self, line: str) -> None: 
+_6_4 """Increment the non-empty line count.""" 
+_6_5 if line.strip(): 
+_6_6 self.num_non_empty_lines += 1 
+_6_7 
+_6_8 def append_unflushed(self, line: str) -> None: 
+_6_9 """Append a line to the output and increment the non-empty line count.""" 
+_7_0 self.unflushed.append(line) 
+_7_1 
+_7_2 def clear_unflushed(self) -> None: 
+_7_3 """Clear the unflushed output.""" 
+_7_4 self.unflushed.clear() 
+_7_5 
+_7_6 def set_ret_code(self, ret_code: int): 
+_7_7 """Set the return code and status of the command.""" 
+_7_8 if self.start_time: 
+_7_9 self.elapsed = time.perf_counter() - self.start_time 
+_8_0 self.ret_code = ret_code 
+_8_1 if self.fut: 
+_8_2 self.fut.cancel() 
+_8_3 self.fut = None 
+_8_4 if ret_code == 0: 
+_8_5 self.status = CommandStatus.SUCCESS 
+_8_6 else: 
+_8_7 self.status = CommandStatus.FAILURE 
+_8_8 
+_8_9 def set_running(self): 
+_9_0 """Set the command status to running.""" 
+_9_1 self.start_time = time.perf_counter() 
+_9_2 self.status = CommandStatus.RUNNING 
 _9_3 
-_9_4class CommandCB(Protocol): 
-_9_5 def on_start(self, cmd: Command) -> None: ... 
-_9_6 def on_recv(self, cmd: Command, output: str) -> None: ... 
-_9_7 def on_term(self, cmd: Command, exit_code: int) -> None: ... 
-_9_8 
+_9_4 
+_9_5class CommandCB(Protocol): 
+_9_6 def on_start(self, cmd: Command) -> None: ... 
+_9_7 def on_recv(self, cmd: Command, output: str) -> None: ... 
+_9_8 def on_term(self, cmd: Command, exit_code: int) -> None: ... 
 _9_9 
-_1_0_0class CommandAsyncCB(Protocol): 
-_1_0_1 async def on_start(self, cmd: Command) -> None: ... 
-_1_0_2 async def on_recv(self, cmd: Command, output: str) -> None: ... 
-_1_0_3 async def on_term(self, cmd: Command, exit_code: int) -> None: ... 
-_1_0_4 
+_1_0_0 
+_1_0_1class CommandAsyncCB(Protocol): 
+_1_0_2 async def on_start(self, cmd: Command) -> None: ... 
+_1_0_3 async def on_recv(self, cmd: Command, output: str) -> None: ... 
+_1_0_4 async def on_term(self, cmd: Command, exit_code: int) -> None: ... 
 _1_0_5 
-_1_0_6class QRetriever: 
-_1_0_7 def __init__(self, q: Queue, timeout: int, retries: int): 
-_1_0_8 self.q = q 
-_1_0_9 self.timeout = timeout 
-_1_1_0 self.retries = retries 
-_1_1_1 
-_1_1_2 def get(self): 
-_1_1_3 retry_count = 0 
-_1_1_4 while True: 
-_1_1_5 try: 
-_1_1_6 return self.q.get(block=True, timeout=self.timeout) 
-_1_1_7 except queue.Empty: 
-_1_1_8 if retry_count < self.retries: 
-_1_1_9 retry_count += 1 
-_1_2_0 continue 
-_1_2_1 else: 
-_1_2_2 raise TimeoutError("Timeout waiting for command output") 
-_1_2_3 
-_1_2_4 def __str__(self) -> str: 
-_1_2_5 return f"QRetriever(timeout={self.timeout}, retries={self.retries})" 
-_1_2_6 
+_1_0_6 
+_1_0_7class QRetriever: 
+_1_0_8 def __init__(self, q: Queue, timeout: int, retries: int): 
+_1_0_9 self.q = q 
+_1_1_0 self.timeout = timeout 
+_1_1_1 self.retries = retries 
+_1_1_2 
+_1_1_3 def get(self): 
+_1_1_4 retry_count = 0 
+_1_1_5 while True: 
+_1_1_6 try: 
+_1_1_7 return self.q.get(block=True, timeout=self.timeout) 
+_1_1_8 except queue.Empty: # noqa: PERF203 
+_1_1_9 if retry_count < self.retries: 
+_1_2_0 retry_count += 1 
+_1_2_1 continue 
+_1_2_2 else: 
+_1_2_3 raise TimeoutError("Timeout waiting for command output") from None 
+_1_2_4 
+_1_2_5 def __str__(self) -> str: 
+_1_2_6 return f"QRetriever(timeout={self.timeout}, retries={self.retries})" 
 _1_2_7 
-_1_2_8class CommandGroup(BaseModel): 
-_1_2_9 """Holder for a group of commands.""" 
-_1_3_0 
-_1_3_1 name: str 
-_1_3_2 desc: Optional[str] = None 
-_1_3_3 cmds: OrderedDict[str, Command] = Field(default_factory=OrderedDict) 
-_1_3_4 timeout: int = Field(default=30) 
-_1_3_5 retries: int = Field(default=3) 
-_1_3_6 
-_1_3_7 async def run_async( 
-_1_3_8 self, 
-_1_3_9 strategy: ProcessingStrategy, 
-_1_4_0 callbacks: CommandAsyncCB, 
-_1_4_1 ): 
-_1_4_2 q = mp.Manager().Queue() 
-_1_4_3 pool = ProcessPoolExecutor() 
-_1_4_4 futs = [ 
-_1_4_5 asyncio.get_event_loop().run_in_executor(pool, run_command, cmd.name,
+_1_2_8 
+_1_2_9class CommandGroup(BaseModel): 
+_1_3_0 """Holder for a group of commands.""" 
+_1_3_1 
+_1_3_2 name: str 
+_1_3_3 desc: Optional[str] = None 
+_1_3_4 cmds: OrderedDict[str, Command] = Field(default_factory=OrderedDict) 
+_1_3_5 timeout: int = Field(default=30) 
+_1_3_6 retries: int = Field(default=3) 
+_1_3_7 cont_on_fail: bool = Field(default=False) 
+_1_3_8 serial: bool = Field(default=False) 
+_1_3_9 status: CommandStatus = CommandStatus.NOT_STARTED 
+_1_4_0 
+_1_4_1 def update_status(self, cmds: OrderedDict[str, Command]): 
+_1_4_2 """Update the status of the command group.""" 
+_1_4_3 if all(cmd.status == CommandStatus.SUCCESS for cmd in cmds.values()): 
+_1_4_4 self.status = CommandStatus.SUCCESS 
+_1_4_5 else: 
+_1_4_6 self.status = CommandStatus.FAILURE 
+_1_4_7 
+_1_4_8 async def run_async( 
+_1_4_9 self, 
+_1_5_0 strategy: ProcessingStrategy, 
+_1_5_1 callbacks: CommandAsyncCB, 
+_1_5_2 ): 
+_1_5_3 q = mp.Manager().Queue() 
+_1_5_4 pool = ProcessPoolExecutor() 
+_1_5_5 futs = [ 
+_1_5_6 asyncio.get_event_loop().run_in_executor(pool, run_command, cmd.name,
 cmd.cmd, cmd.setenv, q) 
-_1_4_6 for _, cmd in self.cmds.items() 
-_1_4_7 ] 
-_1_4_8 
-_1_4_9 for (_, cmd), fut in zip(self.cmds.items(), futs): 
-_1_5_0 cmd.fut = fut 
-_1_5_1 cmd.set_running() 
-_1_5_2 
-_1_5_3 return await self._process_q_async(q, strategy, callbacks) 
-_1_5_4 
-_1_5_5 def run(self, strategy: ProcessingStrategy, callbacks: CommandCB): 
-_1_5_6 q = mp.Manager().Queue() 
-_1_5_7 pool = ProcessPoolExecutor() 
-_1_5_8 futs = [pool.submit(run_command, cmd.name, cmd.cmd, cmd.setenv, q) for _,
-cmd in self.cmds.items()] 
-_1_5_9 for (_, cmd), fut in zip(self.cmds.items(), futs): 
-_1_6_0 cmd.fut = fut 
-_1_6_1 cmd.set_running() 
-_1_6_2 return self._process_q(q, strategy, callbacks) 
+_1_5_7 for _, cmd in self.cmds.items() 
+_1_5_8 ] 
+_1_5_9 
+_1_6_0 for (_, cmd), fut in zip(self.cmds.items(), futs): 
+_1_6_1 cmd.fut = fut 
+_1_6_2 cmd.set_running() 
 _1_6_3 
-_1_6_4 def _process_q( 
-_1_6_5 self, 
-_1_6_6 q: Queue, 
-_1_6_7 strategy: ProcessingStrategy, 
-_1_6_8 callbacks: CommandCB, 
-_1_6_9 ) -> int: 
-_1_7_0 grp_exit_code = 0 
+_1_6_4 return await self._process_q_async(q, strategy, callbacks) 
+_1_6_5 
+_1_6_6 def run(self, strategy: ProcessingStrategy, callbacks: CommandCB): 
+_1_6_7 q = mp.Manager().Queue() 
+_1_6_8 pool = ProcessPoolExecutor() 
+_1_6_9 cmd_series = [OrderedDict([(k, v)]) for k, v in self.cmds.items()] if
+self.serial else [self.cmds] 
+_1_7_0 group_exit_code = 0 
 _1_7_1 
-_1_7_2 if strategy == ProcessingStrategy.ON_RECV: 
-_1_7_3 for _, cmd in self.cmds.items(): 
-_1_7_4 callbacks.on_start(cmd) 
-_1_7_5 
-_1_7_6 q_ret = QRetriever(q, self.timeout, self.retries) 
-_1_7_7 while True: 
-_1_7_8 q_result = q_ret.get() 
-_1_7_9 
-_1_8_0 # Can only get here with a valid message from the Q 
-_1_8_1 cmd_name = q_result[0] 
-_1_8_2 exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else
+_1_7_2 for cmd_entries in cmd_series: 
+_1_7_3 futs = [pool.submit(run_command, cmd.name, cmd.cmd, cmd.setenv, q) for cmd
+in cmd_entries.values()] 
+_1_7_4 for cmd, fut in zip(cmd_entries.values(), futs): 
+_1_7_5 cmd.fut = fut 
+_1_7_6 cmd.set_running() 
+_1_7_7 exit_code = self._process_q(cmd_entries, q, strategy, callbacks) 
+_1_7_8 if exit_code != 0: 
+_1_7_9 group_exit_code = 1 
+_1_8_0 if not self.cont_on_fail: 
+_1_8_1 break 
+_1_8_2 return group_exit_code 
+_1_8_3 
+_1_8_4 def _process_q( # noqa: PLR0912 
+_1_8_5 self, 
+_1_8_6 cmds: OrderedDict[str, Command], 
+_1_8_7 q: Queue, 
+_1_8_8 strategy: ProcessingStrategy, 
+_1_8_9 callbacks: CommandCB, 
+_1_9_0 ) -> int: 
+_1_9_1 grp_exit_code = 0 
+_1_9_2 
+_1_9_3 if strategy == ProcessingStrategy.ON_RECV: 
+_1_9_4 for cmd in cmds.values(): 
+_1_9_5 callbacks.on_start(cmd) 
+_1_9_6 
+_1_9_7 q_ret = QRetriever(q, self.timeout, self.retries) 
+_1_9_8 while True: 
+_1_9_9 q_result = q_ret.get() 
+_2_0_0 
+_2_0_1 # Can only get here with a valid message from the Q 
+_2_0_2 cmd_name = q_result[0] 
+_2_0_3 exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else
 None 
-_1_8_3 output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str)
+_2_0_4 output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str)
 else None 
-_1_8_4 if exit_code is None and output_line is None: 
-_1_8_5 raise ValueError("Invalid Q message") # pragma: no cover 
-_1_8_6 
-_1_8_7 cmd = self.cmds[cmd_name] 
-_1_8_8 if strategy == ProcessingStrategy.ON_RECV: 
-_1_8_9 if output_line is not None: 
-_1_9_0 cmd.incr_line_count(output_line) 
-_1_9_1 callbacks.on_recv(cmd, output_line) 
-_1_9_2 elif exit_code is not None: 
-_1_9_3 cmd.set_ret_code(exit_code) 
-_1_9_4 callbacks.on_term(cmd, exit_code) 
-_1_9_5 if exit_code != 0: 
-_1_9_6 grp_exit_code = 1 
-_1_9_7 else: 
-_1_9_8 raise ValueError("Invalid Q message") # pragma: no cover 
-_1_9_9 
-_2_0_0 if strategy == ProcessingStrategy.ON_COMP: 
-_2_0_1 if output_line is not None: 
-_2_0_2 cmd.incr_line_count(output_line) 
-_2_0_3 cmd.append_unflushed(output_line) 
-_2_0_4 elif exit_code is not None: 
-_2_0_5 callbacks.on_start(cmd) 
-_2_0_6 for line in cmd.unflushed: 
-_2_0_7 callbacks.on_recv(cmd, line) 
-_2_0_8 cmd.clear_unflushed() 
-_2_0_9 callbacks.on_term(cmd, exit_code) 
-_2_1_0 cmd.set_ret_code(exit_code) 
-_2_1_1 if exit_code != 0: 
-_2_1_2 grp_exit_code = 1 
-_2_1_3 else: 
-_2_1_4 raise ValueError("Invalid Q message") # pragma: no cover 
-_2_1_5 
-_2_1_6 if all(cmd.status.completed() for _, cmd in self.cmds.items()): 
-_2_1_7 break 
-_2_1_8 return grp_exit_code 
-_2_1_9 
-_2_2_0 async def _process_q_async( 
-_2_2_1 self, 
-_2_2_2 q: Queue, 
-_2_2_3 strategy: ProcessingStrategy, 
-_2_2_4 callbacks: CommandAsyncCB, 
-_2_2_5 ) -> int: 
-_2_2_6 grp_exit_code = 0 
-_2_2_7 
-_2_2_8 if strategy == ProcessingStrategy.ON_RECV: 
-_2_2_9 for _, cmd in self.cmds.items(): 
-_2_3_0 await callbacks.on_start(cmd) 
-_2_3_1 
-_2_3_2 q_ret = QRetriever(q, self.timeout, self.retries) 
-_2_3_3 while True: 
-_2_3_4 await asyncio.sleep(0) 
-_2_3_5 q_result = q_ret.get() 
+_2_0_5 if exit_code is None and output_line is None: 
+_2_0_6 raise ValueError("Invalid Q message") # pragma: no cover 
+_2_0_7 
+_2_0_8 cmd = self.cmds[cmd_name] 
+_2_0_9 if strategy == ProcessingStrategy.ON_RECV: 
+_2_1_0 if output_line is not None: 
+_2_1_1 cmd.incr_line_count(output_line) 
+_2_1_2 callbacks.on_recv(cmd, output_line) 
+_2_1_3 elif exit_code is not None: 
+_2_1_4 cmd.set_ret_code(exit_code) 
+_2_1_5 callbacks.on_term(cmd, exit_code) 
+_2_1_6 if exit_code != 0: 
+_2_1_7 grp_exit_code = 1 
+_2_1_8 else: 
+_2_1_9 raise ValueError("Invalid Q message") # pragma: no cover 
+_2_2_0 
+_2_2_1 if strategy == ProcessingStrategy.ON_COMP: 
+_2_2_2 if output_line is not None: 
+_2_2_3 cmd.incr_line_count(output_line) 
+_2_2_4 cmd.append_unflushed(output_line) 
+_2_2_5 elif exit_code is not None: 
+_2_2_6 callbacks.on_start(cmd) 
+_2_2_7 for line in cmd.unflushed: 
+_2_2_8 callbacks.on_recv(cmd, line) 
+_2_2_9 cmd.clear_unflushed() 
+_2_3_0 callbacks.on_term(cmd, exit_code) 
+_2_3_1 cmd.set_ret_code(exit_code) 
+_2_3_2 if exit_code != 0: 
+_2_3_3 grp_exit_code = 1 
+_2_3_4 else: 
+_2_3_5 raise ValueError("Invalid Q message") # pragma: no cover 
 _2_3_6 
-_2_3_7 # Can only get here with a valid message from the Q 
-_2_3_8 cmd_name = q_result[0] 
-_2_3_9 exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else
+_2_3_7 if all(cmd.status.completed() for cmd in cmds.values()): 
+_2_3_8 self.update_status(cmds) 
+_2_3_9 break 
+_2_4_0 return grp_exit_code 
+_2_4_1 
+_2_4_2 async def _process_q_async( # noqa: PLR0912 
+_2_4_3 self, 
+_2_4_4 q: Queue, 
+_2_4_5 strategy: ProcessingStrategy, 
+_2_4_6 callbacks: CommandAsyncCB, 
+_2_4_7 ) -> int: 
+_2_4_8 grp_exit_code = 0 
+_2_4_9 
+_2_5_0 if strategy == ProcessingStrategy.ON_RECV: 
+_2_5_1 for cmd in self.cmds.values(): 
+_2_5_2 await callbacks.on_start(cmd) 
+_2_5_3 
+_2_5_4 q_ret = QRetriever(q, self.timeout, self.retries) 
+_2_5_5 while True: 
+_2_5_6 await asyncio.sleep(0) 
+_2_5_7 q_result = q_ret.get() 
+_2_5_8 
+_2_5_9 # Can only get here with a valid message from the Q 
+_2_6_0 cmd_name = q_result[0] 
+_2_6_1 exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else
 None 
-_2_4_0 output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str)
+_2_6_2 output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str)
 else None 
-_2_4_1 if exit_code is None and output_line is None: 
-_2_4_2 raise ValueError("Invalid Q message") # pragma: no cover 
-_2_4_3 
-_2_4_4 cmd = self.cmds[cmd_name] 
-_2_4_5 if strategy == ProcessingStrategy.ON_RECV: 
-_2_4_6 if output_line is not None: 
-_2_4_7 cmd.incr_line_count(output_line) 
-_2_4_8 await callbacks.on_recv(cmd, output_line) 
-_2_4_9 elif exit_code is not None: 
-_2_5_0 cmd.set_ret_code(exit_code) 
-_2_5_1 await callbacks.on_term(cmd, exit_code) 
-_2_5_2 if exit_code != 0: 
-_2_5_3 grp_exit_code = 1 
-_2_5_4 else: 
-_2_5_5 raise ValueError("Invalid Q message") # pragma: no cover 
-_2_5_6 
-_2_5_7 if strategy == ProcessingStrategy.ON_COMP: 
-_2_5_8 if output_line is not None: 
-_2_5_9 cmd.incr_line_count(output_line) 
-_2_6_0 cmd.append_unflushed(output_line) 
-_2_6_1 elif exit_code is not None: 
-_2_6_2 await callbacks.on_start(cmd) 
-_2_6_3 for line in cmd.unflushed: 
-_2_6_4 await callbacks.on_recv(cmd, line) 
-_2_6_5 cmd.clear_unflushed() 
-_2_6_6 await callbacks.on_term(cmd, exit_code) 
-_2_6_7 cmd.set_ret_code(exit_code) 
-_2_6_8 if exit_code != 0: 
-_2_6_9 grp_exit_code = 1 
-_2_7_0 else: 
-_2_7_1 raise ValueError("Invalid Q message") # pragma: no cover 
-_2_7_2 
-_2_7_3 if all(cmd.status.completed() for _, cmd in self.cmds.items()): 
-_2_7_4 break 
-_2_7_5 return grp_exit_code 
-_2_7_6 
-_2_7_7 
-_2_7_8def read_commands_ini(filename: Union[str, Path]) -> list[CommandGroup]: 
-_2_7_9 """Read a commands.ini file and return a list of CommandGroup objects. 
-_2_8_0 
-_2_8_1 Args: 
-_2_8_2 filename (Union[str, Path]): The filename of the commands.ini file. 
-_2_8_3 
-_2_8_4 Returns: 
-_2_8_5 list[CommandGroup]: A list of CommandGroup objects. 
-_2_8_6 """ 
-_2_8_7 config = configparser.ConfigParser() 
-_2_8_8 config.read(filename) 
-_2_8_9 
-_2_9_0 command_groups = [] 
-_2_9_1 for section in config.sections(): 
-_2_9_2 if section.startswith("group."): 
-_2_9_3 group_name = section.replace("group.", "") 
-_2_9_4 commands = OrderedDict() 
-_2_9_5 for name, cmd in config.items(section): 
-_2_9_6 name = name.strip() 
-_2_9_7 commands[name] = Command(name=name, cmd=cmd.strip()) 
-_2_9_8 command_group = CommandGroup(name=group_name, cmds=commands) 
-_2_9_9 command_groups.append(command_group) 
-_3_0_0 
-_3_0_1 return command_groups 
+_2_6_3 if exit_code is None and output_line is None: 
+_2_6_4 raise ValueError("Invalid Q message") # pragma: no cover 
+_2_6_5 
+_2_6_6 cmd = self.cmds[cmd_name] 
+_2_6_7 if strategy == ProcessingStrategy.ON_RECV: 
+_2_6_8 if output_line is not None: 
+_2_6_9 cmd.incr_line_count(output_line) 
+_2_7_0 await callbacks.on_recv(cmd, output_line) 
+_2_7_1 elif exit_code is not None: 
+_2_7_2 cmd.set_ret_code(exit_code) 
+_2_7_3 await callbacks.on_term(cmd, exit_code) 
+_2_7_4 if exit_code != 0: 
+_2_7_5 grp_exit_code = 1 
+_2_7_6 else: 
+_2_7_7 raise ValueError("Invalid Q message") # pragma: no cover 
+_2_7_8 
+_2_7_9 if strategy == ProcessingStrategy.ON_COMP: 
+_2_8_0 if output_line is not None: 
+_2_8_1 cmd.incr_line_count(output_line) 
+_2_8_2 cmd.append_unflushed(output_line) 
+_2_8_3 elif exit_code is not None: 
+_2_8_4 await callbacks.on_start(cmd) 
+_2_8_5 for line in cmd.unflushed: 
+_2_8_6 await callbacks.on_recv(cmd, line) 
+_2_8_7 cmd.clear_unflushed() 
+_2_8_8 await callbacks.on_term(cmd, exit_code) 
+_2_8_9 cmd.set_ret_code(exit_code) 
+_2_9_0 if exit_code != 0: 
+_2_9_1 grp_exit_code = 1 
+_2_9_2 else: 
+_2_9_3 raise ValueError("Invalid Q message") # pragma: no cover 
+_2_9_4 
+_2_9_5 if all(cmd.status.completed() for _, cmd in self.cmds.items()): 
+_2_9_6 break 
+_2_9_7 return grp_exit_code 
+_2_9_8 
+_2_9_9 
+_3_0_0def read_commands_ini(filename: Union[str, Path]) -> list[CommandGroup]: 
+_3_0_1 """Read a commands.ini file and return a list of CommandGroup objects. 
 _3_0_2 
-_3_0_3 
-_3_0_4def write_commands_ini(filename: Union[str, Path], command_groups: list
-[CommandGroup]): 
-_3_0_5 """Write a list of CommandGroup objects to a commands.ini file. 
+_3_0_3 Args: 
+_3_0_4 ---- 
+_3_0_5 filename (Union[str, Path]): The filename of the commands.ini file. 
 _3_0_6 
-_3_0_7 Args: 
-_3_0_8 filename (Union[str, Path]): The filename of the commands.ini file. 
-_3_0_9 command_groups (list[CommandGroup]): A list of CommandGroup objects. 
-_3_1_0 """ 
-_3_1_1 config = configparser.ConfigParser() 
-_3_1_2 
-_3_1_3 for group in command_groups: 
-_3_1_4 section_name = f"group.{group.name}" 
-_3_1_5 config[section_name] = {} 
-_3_1_6 for _, command in group.cmds.items(): 
-_3_1_7 config[section_name][command.name] = command.cmd 
-_3_1_8 
-_3_1_9 with open(filename, "w", encoding="utf-8") as configfile: 
-_3_2_0 config.write(configfile) 
-_3_2_1 
-_3_2_2 
-_3_2_3def _validate_mandatory_keys(data: tomlkit.items.Table, keys: list[str],
-context: str) -> tuple[Any, ...]: 
-_3_2_4 """Validate that the mandatory keys are present in the data. 
+_3_0_7 Returns: 
+_3_0_8 ------- 
+_3_0_9 list[CommandGroup]: A list of CommandGroup objects. 
+_3_1_0 
+_3_1_1 """ 
+_3_1_2 config = configparser.ConfigParser() 
+_3_1_3 config.read(filename) 
+_3_1_4 
+_3_1_5 command_groups = [] 
+_3_1_6 for section in config.sections(): 
+_3_1_7 if section.startswith("group."): 
+_3_1_8 group_name = section.replace("group.", "") 
+_3_1_9 commands = OrderedDict() 
+_3_2_0 for name, cmd in config.items(section): 
+_3_2_1 clean_name = name.strip() 
+_3_2_2 commands[clean_name] = Command(name=clean_name, cmd=cmd.strip()) 
+_3_2_3 command_group = CommandGroup(name=group_name, cmds=commands) 
+_3_2_4 command_groups.append(command_group) 
 _3_2_5 
-_3_2_6 Args: 
-_3_2_7 data (tomlkit.items.Table): The data to validate. 
-_3_2_8 keys (list[str]): The mandatory keys. 
-_3_2_9 """ 
-_3_3_0 vals = [] 
-_3_3_1 for key in keys: 
-_3_3_2 val = data.get(key, None) 
-_3_3_3 if not val: 
-_3_3_4 raise ValueError(f"{key} is mandatory, not found in {context}") 
-_3_3_5 vals.append(val) 
-_3_3_6 return tuple(vals) 
-_3_3_7 
-_3_3_8 
-_3_3_9def _get_optional_keys(data: tomlkit.items.Table, keys: list[str],
-default=None) -> tuple[Optional[Any], ...]: 
-_3_4_0 """Get Optional keys or default. 
-_3_4_1 
-_3_4_2 Args: 
-_3_4_3 data (tomlkit.items.Table): The data to use as source 
-_3_4_4 keys (list[str]): The optional keys. 
-_3_4_5 """ 
-_3_4_6 return tuple(data.get(key, default) for key in keys) 
-_3_4_7 
+_3_2_6 return command_groups 
+_3_2_7 
+_3_2_8 
+_3_2_9def write_commands_ini(filename: Union[str, Path], command_groups: list
+[CommandGroup]): 
+_3_3_0 """Write a list of CommandGroup objects to a commands.ini file. 
+_3_3_1 
+_3_3_2 Args: 
+_3_3_3 ---- 
+_3_3_4 filename (Union[str, Path]): The filename of the commands.ini file. 
+_3_3_5 command_groups (list[CommandGroup]): A list of CommandGroup objects. 
+_3_3_6 
+_3_3_7 """ 
+_3_3_8 config = configparser.ConfigParser() 
+_3_3_9 
+_3_4_0 for group in command_groups: 
+_3_4_1 section_name = f"group.{group.name}" 
+_3_4_2 config[section_name] = {} 
+_3_4_3 for command in group.cmds.values(): 
+_3_4_4 config[section_name][command.name] = command.cmd 
+_3_4_5 
+_3_4_6 with Path(filename).open("w", encoding="utf-8") as configfile: 
+_3_4_7 config.write(configfile) 
 _3_4_8 
-_3_4_9def read_commands_toml(filename: Union[str, Path]) -> list[CommandGroup]: 
-_3_5_0 """Read a commands.toml file and return a list of CommandGroup objects. 
-_3_5_1 
-_3_5_2 Args: 
-_3_5_3 filename (Union[str, Path]): The filename of the commands.toml file. 
-_3_5_4 
-_3_5_5 Returns: 
-_3_5_6 list[CommandGroup]: A list of CommandGroup objects. 
-_3_5_7 """ 
-_3_5_8 
-_3_5_9 with open(filename, "r", encoding="utf-8") as toml_file: 
-_3_6_0 toml_data = tomlkit.parse(toml_file.read()) 
-_3_6_1 
-_3_6_2 cmd_groups_data = toml_data.get("tool", {}).get("par-run", {}) 
-_3_6_3 if not cmd_groups_data: 
-_3_6_4 raise ValueError("No par-run data found in toml file") 
-_3_6_5 _ = cmd_groups_data.get("description", None) 
+_3_4_9 
+_3_5_0def _validate_mandatory_keys(data: tomlkit.items.Table, keys: list[str],
+context: str) -> tuple[Any, ...]: 
+_3_5_1 """Validate that the mandatory keys are present in the data. 
+_3_5_2 
+_3_5_3 Args: 
+_3_5_4 ---- 
+_3_5_5 data (tomlkit.items.Table): The data to validate. 
+_3_5_6 keys (list[str]): The mandatory keys. 
+_3_5_7 
+_3_5_8 """ 
+_3_5_9 vals = [] 
+_3_6_0 for key in keys: 
+_3_6_1 val = data.get(key, None) 
+_3_6_2 if not val: 
+_3_6_3 raise ValueError(f"{key} is mandatory, not found in {context}") 
+_3_6_4 vals.append(val) 
+_3_6_5 return tuple(vals) 
 _3_6_6 
-_3_6_7 command_groups = [] 
-_3_6_8 for group_data in cmd_groups_data.get("groups", []): 
-_3_6_9 (group_name,) = _validate_mandatory_keys(group_data, ["name"], "top level
+_3_6_7 
+_3_6_8def _get_optional_keys(data: tomlkit.items.Table, keys: list[str],
+default=None) -> tuple[Optional[Any], ...]: 
+_3_6_9 """Get Optional keys or default. 
+_3_7_0 
+_3_7_1 Args: 
+_3_7_2 ---- 
+_3_7_3 data (tomlkit.items.Table): The data to use as source 
+_3_7_4 keys (list[str]): The optional keys. 
+_3_7_5 
+_3_7_6 """ 
+_3_7_7 res = tuple(data.get(key, default) for key in keys) 
+_3_7_8 return res 
+_3_7_9 
+_3_8_0 
+_3_8_1def read_commands_toml(filename: Union[str, Path]) -> list[CommandGroup]: 
+_3_8_2 """Read a commands.toml file and return a list of CommandGroup objects. 
+_3_8_3 
+_3_8_4 Args: 
+_3_8_5 ---- 
+_3_8_6 filename (Union[str, Path]): The filename of the commands.toml file. 
+_3_8_7 
+_3_8_8 Returns: 
+_3_8_9 ------- 
+_3_9_0 list[CommandGroup]: A list of CommandGroup objects. 
+_3_9_1 
+_3_9_2 """ 
+_3_9_3 with Path(filename).open(encoding="utf-8") as toml_file: 
+_3_9_4 toml_data = tomlkit.parse(toml_file.read()) 
+_3_9_5 
+_3_9_6 cmd_groups_data = toml_data.get("tool", {}).get("par-run", {}) 
+_3_9_7 if not cmd_groups_data: 
+_3_9_8 raise ValueError("No par-run data found in toml file") 
+_3_9_9 _ = cmd_groups_data.get("description", None) 
+_4_0_0 
+_4_0_1 command_groups = [] 
+_4_0_2 for group_data in cmd_groups_data.get("groups", []): 
+_4_0_3 (group_name,) = _validate_mandatory_keys(group_data, ["name"], "top level
 par-run group") 
-_3_7_0 group_desc, group_timeout, group_retries = _get_optional_keys( 
-_3_7_1 group_data, ["desc", "timeout", "retries"], default=None 
-_3_7_2 ) 
-_3_7_3 
-_3_7_4 if not group_timeout: 
-_3_7_5 group_timeout = 30 
-_3_7_6 if not group_retries: 
-_3_7_7 group_retries = 3 
-_3_7_8 
-_3_7_9 commands = OrderedDict() 
-_3_8_0 for cmd_data in group_data.get("commands", []): 
-_3_8_1 name, exec = _validate_mandatory_keys(cmd_data, ["name", "exec"], f"command
+_4_0_4 group_desc, group_timeout, group_retries = _get_optional_keys( 
+_4_0_5 group_data, 
+_4_0_6 ["desc", "timeout", "retries"], 
+_4_0_7 default=None, 
+_4_0_8 ) 
+_4_0_9 (group_cont_on_fail, group_serial) = _get_optional_keys(group_data,
+["cont_on_fail", "serial"], default=False) 
+_4_1_0 
+_4_1_1 if not group_timeout: 
+_4_1_2 group_timeout = 30 
+_4_1_3 if not group_retries: 
+_4_1_4 group_retries = 3 
+_4_1_5 group_cont_on_fail = bool(group_cont_on_fail and group_cont_on_fail is
+True) 
+_4_1_6 group_serial = bool(group_serial and group_serial is True) 
+_4_1_7 
+_4_1_8 commands = OrderedDict() 
+_4_1_9 for cmd_data in group_data.get("commands", []): 
+_4_2_0 name, exec = _validate_mandatory_keys(cmd_data, ["name", "exec"], f"command
 group {group_name}") 
-_3_8_2 setenv, passenv = _get_optional_keys(cmd_data, ["setenv", "passenv"],
+_4_2_1 setenv, passenv = _get_optional_keys(cmd_data, ["setenv", "passenv"],
 default=None) 
-_3_8_3 
-_3_8_4 commands[name] = Command(name=name, cmd=exec, setenv=setenv,
+_4_2_2 
+_4_2_3 commands[name] = Command(name=name, cmd=exec, setenv=setenv,
 passenv=passenv) 
-_3_8_5 command_group = CommandGroup( 
-_3_8_6 name=group_name, desc=group_desc, cmds=commands, timeout=group_timeout,
-retries=group_retries 
-_3_8_7 ) 
-_3_8_8 command_groups.append(command_group) 
-_3_8_9 
-_3_9_0 return command_groups 
-_3_9_1 
-_3_9_2 
-_3_9_3def run_command(name: str, command: str, setenv: Optional[dict[str, str]],
+_4_2_4 command_group = CommandGroup( 
+_4_2_5 name=group_name, 
+_4_2_6 desc=group_desc, 
+_4_2_7 cmds=commands, 
+_4_2_8 timeout=group_timeout, 
+_4_2_9 retries=group_retries, 
+_4_3_0 cont_on_fail=group_cont_on_fail, 
+_4_3_1 serial=group_serial, 
+_4_3_2 ) 
+_4_3_3 command_groups.append(command_group) 
+_4_3_4 
+_4_3_5 return command_groups 
+_4_3_6 
+_4_3_7 
+_4_3_8def run_command(name: str, command: str, setenv: Optional[dict[str, str]],
 q: Queue) -> None: 
-_3_9_4 """Run a command and put the output into a queue. The output is a tuple of
+_4_3_9 """Run a command and put the output into a queue. The output is a tuple of
 the command 
-_3_9_5 name and the output line. The final output is a tuple of the command name
+_4_4_0 name and the output line. The final output is a tuple of the command name
 and a dictionary 
-_3_9_6 with the return code. 
-_3_9_7 
-_3_9_8 Args: 
-_3_9_9 name (Command): Command to run. 
-_4_0_0 q (Queue): Queue to put the output into. 
-_4_0_1 """ 
-_4_0_2 
-_4_0_3 new_env = None 
-_4_0_4 if setenv: 
-_4_0_5 new_env = os.environ.copy() 
-_4_0_6 new_env.update(setenv) 
-_4_0_7 
-_4_0_8 with subprocess.Popen( 
-_4_0_9 command, 
-_4_1_0 shell=True, 
-_4_1_1 env=new_env, 
-_4_1_2 stdout=subprocess.PIPE, 
-_4_1_3 stderr=subprocess.STDOUT, 
-_4_1_4 text=True, 
-_4_1_5 ) as process: 
-_4_1_6 if process.stdout: 
-_4_1_7 for line in iter(process.stdout.readline, ""): 
-_4_1_8 q.put((name, line.strip())) 
-_4_1_9 process.stdout.close() 
-_4_2_0 process.wait() 
-_4_2_1 ret_code = process.returncode 
-_4_2_2 if ret_code is not None: 
-_4_2_3 q.put((name, int(ret_code))) 
-_4_2_4 else: 
-_4_2_5 raise ValueError("Process has no return code") # pragma: no cover 
+_4_4_1 with the return code. 
+_4_4_2 
+_4_4_3 Args: 
+_4_4_4 ---- 
+_4_4_5 name (Command): Command to run. 
+_4_4_6 q (Queue): Queue to put the output into. 
+_4_4_7 
+_4_4_8 """ 
+_4_4_9 new_env = None 
+_4_5_0 if setenv: 
+_4_5_1 new_env = os.environ.copy() 
+_4_5_2 new_env.update(setenv) 
+_4_5_3 
+_4_5_4 with subprocess.Popen( 
+_4_5_5 command, 
+_4_5_6 shell=True, 
+_4_5_7 env=new_env, 
+_4_5_8 stdout=subprocess.PIPE, 
+_4_5_9 stderr=subprocess.STDOUT, 
+_4_6_0 text=True, 
+_4_6_1 ) as process: 
+_4_6_2 if process.stdout: 
+_4_6_3 for line in iter(process.stdout.readline, ""): 
+_4_6_4 q.put((name, line.strip())) 
+_4_6_5 process.stdout.close() 
+_4_6_6 process.wait() 
+_4_6_7 ret_code = process.returncode 
+_4_6_8 if ret_code is not None: 
+_4_6_9 q.put((name, int(ret_code))) 
+_4_7_0 else: 
+_4_7_1 raise ValueError("Process has no return code") # pragma: no cover 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-12 08:32 -0400
+13 15:32 -0400
```

### Comparing `par_run-0.2.2/.reports/html/d_417a353b6036f046_web_cli_py.html` & `par_run-0.3.0/.reports/html/d_417a353b6036f046_web_cli_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/.reports/html/d_417a353b6036f046_web_py.html` & `par_run-0.3.0/.reports/html/d_417a353b6036f046_web_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/par_run/web.py: 71%</title>
+    <title>Coverage for src/par_run/web.py: 74%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/par_run/web.py</b>:
-            <span class="pc_cov">71%</span>
+            <span class="pc_cov">74%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">41 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">29<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">12<span class="text"> missing</span></button>
+            <span class="text">38 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">28<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">10<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046_executor_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 07:35 -0400
+            created at 2024-04-13 13:09 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -79,43 +79,43 @@
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Web UI Module"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">rich</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span> <span class="key">import</span> <span class="nam">Body</span><span class="op">,</span> <span class="nam">FastAPI</span><span class="op">,</span> <span class="nam">Request</span><span class="op">,</span> <span class="nam">WebSocket</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span><span class="op">.</span><span class="nam">staticfiles</span> <span class="key">import</span> <span class="nam">StaticFiles</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span><span class="op">.</span><span class="nam">templating</span> <span class="key">import</span> <span class="nam">Jinja2Templates</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">executor</span> <span class="key">import</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">CommandGroup</span><span class="op">,</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span> <span class="nam">read_commands_ini</span><span class="op">,</span> <span class="nam">write_commands_ini</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="nam">BASE_PATH</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">__file__</span><span class="op">)</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">parent</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="nam">ws_app</span> <span class="op">=</span> <span class="nam">FastAPI</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="nam">ws_app</span><span class="op">.</span><span class="nam">mount</span><span class="op">(</span><span class="str">"/static"</span><span class="op">,</span> <span class="nam">StaticFiles</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">str</span><span class="op">(</span><span class="nam">BASE_PATH</span> <span class="op">/</span> <span class="str">"static"</span><span class="op">)</span><span class="op">)</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="str">"static"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="nam">templates</span> <span class="op">=</span> <span class="nam">Jinja2Templates</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">str</span><span class="op">(</span><span class="nam">BASE_PATH</span> <span class="op">/</span> <span class="str">"templates"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">rich</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span> <span class="key">import</span> <span class="nam">Body</span><span class="op">,</span> <span class="nam">FastAPI</span><span class="op">,</span> <span class="nam">Request</span><span class="op">,</span> <span class="nam">WebSocket</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span><span class="op">.</span><span class="nam">staticfiles</span> <span class="key">import</span> <span class="nam">StaticFiles</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span><span class="op">.</span><span class="nam">templating</span> <span class="key">import</span> <span class="nam">Jinja2Templates</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">executor</span> <span class="key">import</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span> <span class="nam">read_commands_ini</span><span class="op">,</span> <span class="nam">write_commands_ini</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="nam">BASE_PATH</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">__file__</span><span class="op">)</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">parent</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="nam">ws_app</span> <span class="op">=</span> <span class="nam">FastAPI</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="nam">ws_app</span><span class="op">.</span><span class="nam">mount</span><span class="op">(</span><span class="str">"/static"</span><span class="op">,</span> <span class="nam">StaticFiles</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">str</span><span class="op">(</span><span class="nam">BASE_PATH</span> <span class="op">/</span> <span class="str">"static"</span><span class="op">)</span><span class="op">)</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="str">"static"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="nam">templates</span> <span class="op">=</span> <span class="nam">Jinja2Templates</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">str</span><span class="op">(</span><span class="nam">BASE_PATH</span> <span class="op">/</span> <span class="str">"templates"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="op">@</span><span class="nam">ws_app</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"/"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">ws_main</span><span class="op">(</span><span class="nam">request</span><span class="op">:</span> <span class="nam">Request</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="str">"""Get the main page."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">"Main page"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="op">@</span><span class="nam">ws_app</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"/"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">ws_main</span><span class="op">(</span><span class="nam">request</span><span class="op">:</span> <span class="nam">Request</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="str">"""Get the main page."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="key">return</span> <span class="nam">templates</span><span class="op">.</span><span class="nam">TemplateResponse</span><span class="op">(</span><span class="str">"index.html"</span><span class="op">,</span> <span class="op">{</span><span class="str">"request"</span><span class="op">:</span> <span class="nam">request</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="op">@</span><span class="nam">ws_app</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"/get-commands-config"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">get_commands_config</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="str">"""Get the commands configuration."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="key">return</span> <span class="nam">read_commands_ini</span><span class="op">(</span><span class="str">"commands.ini"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="op">@</span><span class="nam">ws_app</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span><span class="str">"/update-commands-config"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">update_commands_config</span><span class="op">(</span><span class="nam">updated_config</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Body</span><span class="op">(</span><span class="op">...</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">update_commands_config</span><span class="op">(</span><span class="nam">updated_config</span><span class="op">=</span><span class="nam">Body</span><span class="op">(</span><span class="op">...</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>  <span class="com"># noqa: B008</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"""Update the commands configuration."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">write_commands_ini</span><span class="op">(</span><span class="str">"commands.ini"</span><span class="op">,</span> <span class="nam">updated_config</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="str">"message"</span><span class="op">:</span> <span class="str">"Configuration updated successfully"</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="key">class</span> <span class="nam">WebCommandCB</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="str">"""Websocket command callbacks."""</span>&nbsp;</span><span class="r"></span></p>
@@ -134,29 +134,27 @@
     <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t"><span class="op">@</span><span class="nam">ws_app</span><span class="op">.</span><span class="nam">websocket_route</span><span class="op">(</span><span class="str">"/ws"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">websocket_endpoint</span><span class="op">(</span><span class="nam">websocket</span><span class="op">:</span> <span class="nam">WebSocket</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="str">"""Websocket endpoint to run commands."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"Websocket connection"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="nam">master_groups</span> <span class="op">=</span> <span class="nam">read_commands_ini</span><span class="op">(</span><span class="str">"commands.ini"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="nam">master_groups</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="key">await</span> <span class="nam">websocket</span><span class="op">.</span><span class="nam">accept</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">cb</span> <span class="op">=</span> <span class="nam">WebCommandCB</span><span class="op">(</span><span class="nam">websocket</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">"Running commands"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="nam">exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="key">await</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run_async</span><span class="op">(</span><span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">,</span> <span class="nam">cb</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="key">await</span> <span class="nam">websocket</span><span class="op">.</span><span class="nam">accept</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">cb</span> <span class="op">=</span> <span class="nam">WebCommandCB</span><span class="op">(</span><span class="nam">websocket</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="key">await</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run_async</span><span class="op">(</span><span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">,</span> <span class="nam">cb</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046_executor_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 07:35 -0400
+            created at 2024-04-13 13:09 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,55 +1,54 @@
-************ CCoovveerraaggee ffoorr ssrrcc//ppaarr__rruunn//wweebb..ppyy:: 7711%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//ppaarr__rruunn//wweebb..ppyy:: 7744%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 4411 ssttaatteemmeennttss ?  2299 rruunn 1122 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 3388 ssttaatteemmeennttss ?  2288 rruunn 1100 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-12 07:35 -0400
+13 13:09 -0400
 _1"""Web UI Module""" 
 _2 
 _3from pathlib import Path 
-_4import rich 
-_5from fastapi import Body, FastAPI, Request, WebSocket 
-_6from fastapi.staticfiles import StaticFiles 
-_7from fastapi.templating import Jinja2Templates 
-_8 
-_9from .executor import Command, CommandGroup, ProcessingStrategy,
-read_commands_ini, write_commands_ini 
-_1_0 
-_1_1BASE_PATH = Path(__file__).resolve().parent 
-_1_2 
-_1_3ws_app = FastAPI() 
-_1_4ws_app.mount("/static", StaticFiles(directory=str(BASE_PATH / "static")),
+_4 
+_5import rich 
+_6from fastapi import Body, FastAPI, Request, WebSocket 
+_7from fastapi.staticfiles import StaticFiles 
+_8from fastapi.templating import Jinja2Templates 
+_9 
+_1_0from .executor import Command, ProcessingStrategy, read_commands_ini,
+write_commands_ini 
+_1_1 
+_1_2BASE_PATH = Path(__file__).resolve().parent 
+_1_3 
+_1_4ws_app = FastAPI() 
+_1_5ws_app.mount("/static", StaticFiles(directory=str(BASE_PATH / "static")),
 name="static") 
-_1_5templates = Jinja2Templates(directory=str(BASE_PATH / "templates")) 
-_1_6 
+_1_6templates = Jinja2Templates(directory=str(BASE_PATH / "templates")) 
 _1_7 
-_1_8@ws_app.get("/") 
-_1_9async def ws_main(request: Request): 
-_2_0 """Get the main page.""" 
-_2_1 print("Main page") 
+_1_8 
+_1_9@ws_app.get("/") 
+_2_0async def ws_main(request: Request): 
+_2_1 """Get the main page.""" 
 _2_2 return templates.TemplateResponse("index.html", {"request": request}) 
 _2_3 
 _2_4 
 _2_5@ws_app.get("/get-commands-config") 
 _2_6async def get_commands_config(): 
 _2_7 """Get the commands configuration.""" 
 _2_8 return read_commands_ini("commands.ini") 
 _2_9 
 _3_0 
 _3_1@ws_app.post("/update-commands-config") 
-_3_2async def update_commands_config(updated_config: list[CommandGroup] = Body
-(...)): 
+_3_2async def update_commands_config(updated_config=Body(...)): # noqa: B008 
 _3_3 """Update the commands configuration.""" 
 _3_4 write_commands_ini("commands.ini", updated_config) 
 _3_5 return {"message": "Configuration updated successfully"} 
 _3_6 
 _3_7 
 _3_8class WebCommandCB: 
 _3_9 """Websocket command callbacks.""" 
@@ -69,17 +68,15 @@
 _5_2 
 _5_3 
 _5_4@ws_app.websocket_route("/ws") 
 _5_5async def websocket_endpoint(websocket: WebSocket): 
 _5_6 """Websocket endpoint to run commands.""" 
 _5_7 rich.print("Websocket connection") 
 _5_8 master_groups = read_commands_ini("commands.ini") 
-_5_9 print(master_groups) 
-_6_0 await websocket.accept() 
-_6_1 cb = WebCommandCB(websocket) 
-_6_2 print("Running commands") 
-_6_3 exit_code = 0 
-_6_4 for grp in master_groups: 
-_6_5 exit_code = exit_code or await grp.run_async(ProcessingStrategy.ON_RECV,
+_5_9 await websocket.accept() 
+_6_0 cb = WebCommandCB(websocket) 
+_6_1 exit_code = 0 
+_6_2 for grp in master_groups: 
+_6_3 exit_code = exit_code or await grp.run_async(ProcessingStrategy.ON_RECV,
 cb) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-12 07:35 -0400
+13 13:09 -0400
```

### Comparing `par_run-0.2.2/.reports/html/favicon_32.png` & `par_run-0.3.0/.reports/html/favicon_32.png`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/.reports/html/index.html` & `par_run-0.3.0/.reports/html/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 10:21 -0400
+            created at 2024-04-13 15:32 -0400
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -66,53 +66,53 @@
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_417a353b6036f046_cli_py.html">src/par_run/cli.py</a></td>
-                <td>180</td>
-                <td>17</td>
+                <td>219</td>
+                <td>22</td>
                 <td>2</td>
-                <td class="right" data-ratio="163 180">91%</td>
+                <td class="right" data-ratio="197 219">90%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_417a353b6036f046_executor_py.html">src/par_run/executor.py</a></td>
-                <td>251</td>
-                <td>38</td>
+                <td>271</td>
+                <td>42</td>
                 <td>7</td>
-                <td class="right" data-ratio="213 251">85%</td>
+                <td class="right" data-ratio="229 271">85%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_417a353b6036f046_web_py.html">src/par_run/web.py</a></td>
-                <td>41</td>
-                <td>12</td>
+                <td>38</td>
+                <td>10</td>
                 <td>0</td>
-                <td class="right" data-ratio="29 41">71%</td>
+                <td class="right" data-ratio="28 38">74%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>473</td>
-                <td>67</td>
+                <td>529</td>
+                <td>74</td>
                 <td>9</td>
-                <td class="right" data-ratio="406 473">86%</td>
+                <td class="right" data-ratio="455 529">86%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 10:21 -0400
+            created at 2024-04-13 15:32 -0400
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_417a353b6036f046_web_py.html"/>
         <a id="nextFileLink" class="nav" href="d_417a353b6036f046___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 ************ CCoovveerraaggee rreeppoorrtt:: 8866%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-12 10:21 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-13 15:32 -0400
 MMoodduullee                  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _s_r_c_/_p_a_r___r_u_n_/_____i_n_i_t_____._p_y 1          0       0        100%
-_s_r_c_/_p_a_r___r_u_n_/_c_l_i_._p_y      180        17      2        91%
-_s_r_c_/_p_a_r___r_u_n_/_e_x_e_c_u_t_o_r_._p_y 251        38      7        85%
-_s_r_c_/_p_a_r___r_u_n_/_w_e_b_._p_y      41         12      0        71%
-Total                   473        67      9        86%
+_s_r_c_/_p_a_r___r_u_n_/_c_l_i_._p_y      219        22      2        90%
+_s_r_c_/_p_a_r___r_u_n_/_e_x_e_c_u_t_o_r_._p_y 271        42      7        85%
+_s_r_c_/_p_a_r___r_u_n_/_w_e_b_._p_y      38         10      0        74%
+Total                   529        74      9        86%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-12 10:21 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-13 15:32 -0400
```

### Comparing `par_run-0.2.2/.reports/html/keybd_closed.png` & `par_run-0.3.0/.reports/html/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/.reports/html/keybd_open.png` & `par_run-0.3.0/.reports/html/keybd_open.png`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/.reports/html/status.json` & `par_run-0.3.0/.reports/html/status.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9894999999999999%*

 * *Differences: {"'files'": "{'d_417a353b6036f046___init___py': {'hash': '789c313adf999ffc277fcac08e19c2c1'}, "*

 * *            "'d_417a353b6036f046_cli_py': {'hash': '7e679eab98e618a11daba9ba54fcd51b', 'index': "*

 * *            "{'nums': {insert: [(2, 219), (4, 22)], delete: [4, 2]}}}, "*

 * *            "'d_417a353b6036f046_executor_py': {'hash': 'a7d12c01d3dcb30db4f9fe13e4e0e92c', "*

 * *            "'index': {'nums': {insert: [(2, 271), (4, 42)], delete: [4, 2]}}}, "*

 * *            "'d_417a353b6036f046_web_py': {'hash': '1b830066e8f21110b […]*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "d_417a353b6036f046___init___py": {
-            "hash": "2acd0f3f7d187411f827058d2663ad25",
+            "hash": "789c313adf999ffc277fcac08e19c2c1",
             "index": {
                 "html_filename": "d_417a353b6036f046___init___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -14,40 +14,40 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/par_run/__init__.py"
             }
         },
         "d_417a353b6036f046_cli_py": {
-            "hash": "0ccfe317a36b4e9ad5cd9d8c055c4c9e",
+            "hash": "7e679eab98e618a11daba9ba54fcd51b",
             "index": {
                 "html_filename": "d_417a353b6036f046_cli_py.html",
                 "nums": [
                     0,
                     1,
-                    180,
+                    219,
                     2,
-                    17,
+                    22,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/par_run/cli.py"
             }
         },
         "d_417a353b6036f046_executor_py": {
-            "hash": "30a2e8e096771c03bce574b222368cf2",
+            "hash": "a7d12c01d3dcb30db4f9fe13e4e0e92c",
             "index": {
                 "html_filename": "d_417a353b6036f046_executor_py.html",
                 "nums": [
                     0,
                     1,
-                    251,
+                    271,
                     7,
-                    38,
+                    42,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/par_run/executor.py"
             }
         },
@@ -65,23 +65,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/par_run/web_cli.py"
             }
         },
         "d_417a353b6036f046_web_py": {
-            "hash": "1fb2ef0b6f77c855d0607135ad5ff66f",
+            "hash": "1b830066e8f21110b1894eec46b2950f",
             "index": {
                 "html_filename": "d_417a353b6036f046_web_py.html",
                 "nums": [
                     0,
                     1,
-                    41,
+                    38,
                     0,
-                    12,
+                    10,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/par_run/web.py"
             }
         }
```

### Comparing `par_run-0.2.2/.reports/html/style.css` & `par_run-0.3.0/.reports/html/style.css`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/.vscode/launch.json` & `par_run-0.3.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/py_tests/test_cli.py` & `par_run-0.3.0/py_tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     stop_web_server,
 )
 from par_run.executor import Command, CommandGroup, CommandStatus
 
 runner = CliRunner()
 
 
-@pytest.fixture
+@pytest.fixture()
 def mock_command_group():
     command1 = Command(name="cmd1", cmd="echo 'Hello, World!'")
     command2 = Command(name="cmd2", cmd="echo 'Goodbye, World!'")
     commands = {"cmd1": command1, "cmd2": command2}
     return CommandGroup(name="group1", cmds=commands)
 
 
-@pytest.fixture
+@pytest.fixture()
 def mock_command_group_part_fail():
     command1 = Command(name="cmd1", cmd="echo 'Hello, World!'")
     command2 = Command(name="cmd2", cmd="exit 1")
     commands = {"cmd1": command1, "cmd2": command2}
     return CommandGroup(name="group1", cmds=commands)
 
 
@@ -115,15 +115,16 @@
     # Setup: Mock time.time_ns to control the loop timing, ensuring it doesn't run out of values
     start_ns = 1000000
     time_ns_side_effect = itertools.chain([start_ns, start_ns + 1], itertools.repeat(start_ns + 2 * 10**9))
     mocker.patch("par_run.cli.time.time_ns", side_effect=time_ns_side_effect)
 
     # Setup: Mock get_process_port to return the correct port after the first loop iteration, ensuring it doesn't run out of values
     get_process_port_side_effect = itertools.chain(
-        [None, 8000], itertools.repeat(8000)
+        [None, 8000],
+        itertools.repeat(8000),
     )  # First call: None, subsequent calls: 8000 (port number)
     mocker.patch("par_run.cli.get_process_port", side_effect=get_process_port_side_effect)
 
     # Setup: Mock typer.echo to capture output
     mock_echo = mocker.patch("par_run.cli.typer.echo")
 
     # Setup: Temporary PID file location
@@ -254,19 +255,21 @@
         stop_web_server()
 
 
 def test_get_process_port(mocker):
     # Mock psutil.Process and its connections method
     mock_process = mocker.patch("par_run.cli.psutil.Process")
     mock_conn = mocker.MagicMock()
-    mock_conn.laddr.port = 8000  # Example port number
+    run_port = 8000
+    mock_conn.laddr.port = run_port
     mock_process.return_value.connections.return_value = [mock_conn]
 
-    port = get_process_port(1234)  # Example PID
-    assert port == 8000
+    example_pid = 1234
+    port = get_process_port(example_pid)
+    assert port == run_port
 
 
 def test_get_process_port_no_connections(mocker):
     # Mock psutil.Process to return no connections
     mock_process = mocker.patch("par_run.cli.psutil.Process")
     mock_process.return_value.connections.return_value = []
```

### Comparing `par_run-0.2.2/py_tests/test_executor.py` & `par_run-0.3.0/py_tests/test_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,16 @@
     fut = pool.submit(run_command, command.name, command.cmd, {}, q)
     command.fut = fut
     command.set_running()
     _ = fut.result()
 
     msg = q.get()
     assert isinstance(msg, tuple)
-    assert len(msg) == 2
+    exp_msg_len = 2
+    assert len(msg) == exp_msg_len
     assert msg[0] == command.name
     assert msg[1] == "Hello, World!"
     exit_code = q.get()[1]
 
     command.set_ret_code(exit_code)
     assert command.ret_code == 0
     assert command.status == CommandStatus.SUCCESS
@@ -71,15 +72,16 @@
     fut = pool.submit(run_command, command.name, command.cmd, {}, q)
     command.set_running()
     command.fut = fut
     _ = fut.result()
     msg = q.get()
 
     assert isinstance(msg, tuple)
-    assert len(msg) == 2
+    exp_msg_len = 2
+    assert len(msg) == exp_msg_len
     assert msg[0] == command.name
     exit_code = msg[1]
     command.set_ret_code(exit_code)
     assert command.ret_code == exit_code
     assert command.status == CommandStatus.FAILURE
     assert command.fut is None
     assert command.status.completed()
@@ -205,15 +207,15 @@
     assert all(cmd.unflushed == [] for cmd in group.cmds.values())
     assert all(cmd.fut is None for cmd in group.cmds.values())
     assert all(cmd.status in [CommandStatus.SUCCESS, CommandStatus.FAILURE] for cmd in group.cmds.values())
     assert all(cmd.ret_code in [0, 1] for cmd in group.cmds.values())
     assert group_exit == 1
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_command_group_async():
     command1 = Command(name="test1", cmd="echo 'Hello, World!'")
     command2 = Command(name="test2", cmd="echo 'World, Hey!'")
     commands = OrderedDict()
     commands[command1.name] = command1
     commands[command2.name] = command2
     group = CommandGroup(name="test_group", cmds=commands)
@@ -238,15 +240,15 @@
     assert all(cmd.num_non_empty_lines == 1 for cmd in group.cmds.values())
     assert all(cmd.unflushed == [] for cmd in group.cmds.values())
     assert all(cmd.fut is None for cmd in group.cmds.values())
     assert all(cmd.status == CommandStatus.SUCCESS for cmd in group.cmds.values())
     assert all(cmd.ret_code == 0 for cmd in group.cmds.values())
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_command_group_async_part_fail():
     command1 = Command(name="test1", cmd="echo 'Hello, World!'")
     command2 = Command(name="test2", cmd="echo 'World, Hey!'; exit 1")
     commands = OrderedDict()
     commands[command1.name] = command1
     commands[command2.name] = command2
     group = CommandGroup(name="test_group", cmds=commands)
@@ -279,15 +281,16 @@
 
 def test_run_command():
     q = mp.Manager().Queue()
     run_command("Test", "echo 'Hello, World!'", {}, q)
 
     msg = q.get()
     assert isinstance(msg, tuple)
-    assert len(msg) == 2
+    exp_msg_len = 2
+    assert len(msg) == exp_msg_len
     assert msg[0] == "Test"
     assert msg[1] == "Hello, World!"
     exit_code = q.get()[1]
     assert exit_code == 0
 
 
 def test_read_commands_ini(mocker, command_data, expected_command_groups):
```

### Comparing `par_run-0.2.2/py_tests/test_web.py` & `par_run-0.3.0/py_tests/test_web.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,39 +3,41 @@
 import pytest
 from fastapi.testclient import TestClient
 
 from par_run.executor import Command, CommandStatus
 from par_run.web import WebCommandCB, ws_app
 
 
-@pytest.fixture
+@pytest.fixture()
 def async_mock():
     """Creates an async version of MagicMock."""
 
     class AsyncMock(MagicMock):
         async def __call__(self, *args, **kwargs):
-            return super(AsyncMock, self).__call__(*args, **kwargs)
+            return super().__call__(*args, **kwargs)
 
     return AsyncMock
 
 
 client = TestClient(ws_app)
 
 
 def test_ws_main():
     response = client.get("/")
-    assert response.status_code == 200
+    http_ok = 200
+    assert response.status_code == http_ok
 
 
 def test_get_commands_config(mocker):
     # Mock read_commands_ini to return a known value
     mock_read = mocker.patch("par_run.web.read_commands_ini", return_value=[{"name": "test", "cmds": []}])
 
     response = client.get("/get-commands-config")
-    assert response.status_code == 200
+    http_ok = 200
+    assert response.status_code == http_ok
     assert response.json() == [{"name": "test", "cmds": []}]
     mock_read.assert_called_once_with("commands.ini")
 
 
 @pytest.mark.skip(reason="Need to align pydantic models")
 def test_update_commands_config(mocker):
     # Mock write_commands_ini to do nothing
@@ -44,62 +46,61 @@
     command_group_payload = [
         {
             "name": "test_group",
             "cmds": [
                 {"name": "command1", "cmd": "echo Hello World"},
                 {"name": "command2", "cmd": "echo Goodbye World"},
             ],
-        }
+        },
     ]
 
     response = client.post("/update-commands-config", json=command_group_payload)
-    assert response.status_code == 200
+    http_ok = 200
+    assert response.status_code == http_ok
 
 
 @pytest.mark.skip(reason="WebSocket testing is not yet implemented")
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_websocket_endpoint(mocker):
     # Mock read_commands_ini and CommandGroup.run_async if necessary
     mocker.patch("par_run.web.read_commands_ini", return_value=[])
     mock_run_async = mocker.patch("par_run.executor.CommandGroup.run_async", return_value=0)
 
-    print("websocket_endpoint1")
     # Connect to the WebSocket endpoint
     with client.websocket_connect("/ws") as websocket:
         # Send a message to initiate command execution or any other interaction
         # Adjust this part based on how your WebSocket endpoint is supposed to be used
         while True:
             response = websocket.receive_json()
-            print(response)  # Print each response for inspection
 
             # Add a condition to break the loop when all responses are received
             # This condition depends on your WebSocket server's implementation
             if "ret_code" in response:  # Example condition, adjust as necessary
                 break
 
     # Verify that run_async was called if it's part of the WebSocket interaction
     mock_run_async.assert_awaited()
 
 
 @pytest.mark.skip(reason="WebSocket testing is not yet implemented")
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_webcommandcb_on_start(async_mock):
     ws = MagicMock()
     ws.send_json = async_mock()
 
     cmd = Command(name="test_cmd", cmd="echo 'Hello World'", status=CommandStatus.NOT_STARTED)
 
     cb = WebCommandCB(ws)
     await cb.on_start(cmd)
 
     # Since ws.send_json is an async mock, you should check if it's awaited with the expected arguments
     ws.send_json.assert_awaited_with({"commandName": cmd.name, "output": "[blue bold]Started command test_cmd[/]"})
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_webcommandcb_on_recv(async_mock):
     # Mock WebSocket with async send_json
     ws = MagicMock()
     ws.send_json = async_mock()
 
     cmd = Command(name="test_cmd", cmd="echo 'Hello World'")
 
@@ -113,15 +114,15 @@
     assert ws.send_json.called
     assert ws.send_json.call_args[0][0] == {
         "commandName": "test_cmd",
         "output": "Hello World",
     }
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_webcommandcb_on_term(async_mock):
     # Mock WebSocket with async send_json
     ws = MagicMock()
     ws.send_json = async_mock()
 
     cmd = Command(name="test_cmd", cmd="echo 'Goodbye World'")
```

### Comparing `par_run-0.2.2/src/par_run/cli.py` & `par_run-0.3.0/src/par_run/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 """CLI for running commands in parallel"""
 
+import contextlib
+import enum
 from collections import OrderedDict
 from pathlib import Path
-from typing import Optional
-import enum
+from typing import Annotated, Optional
 
 import rich
 import typer
 
-from .executor import Command, CommandStatus, ProcessingStrategy, read_commands_toml
+from .executor import Command, CommandGroup, CommandStatus, ProcessingStrategy, read_commands_toml
 
 PID_FILE = ".par-run.uvicorn.pid"
 
 cli_app = typer.Typer()
 
 
 # Web only functions
 def clean_up():
-    """
-    Clean up by removing the PID file.
-    """
-    os.remove(PID_FILE)
+    """Clean up by removing the PID file."""
+    Path(PID_FILE).unlink()
     typer.echo("Cleaned up PID file.")
 
 
 def start_web_server(port: int):
     """Start the web server"""
-    if os.path.isfile(PID_FILE):
+    if Path(PID_FILE).is_file():
         typer.echo("UVicorn server is already running.")
         sys.exit(1)
-    with open(PID_FILE, "w", encoding="utf-8") as pid_file:
+    with Path(PID_FILE).open("w", encoding="utf-8") as pid_file:
         typer.echo(f"Starting UVicorn server on port {port}...")
         uvicorn_command = [
             "uvicorn",
             "par_run.web:ws_app",
             "--host",
             "0.0.0.0",
             "--port",
@@ -55,29 +54,25 @@
 
         else:
             typer.echo(f"UVicorn server did not respond within {wait_time} seconds.")
             typer.echo("run 'par-run web status' to check the status.")
 
 
 def stop_web_server():
-    """
-    Stop the UVicorn server by reading its PID from the PID file and sending a termination signal.
-    """
+    """Stop the UVicorn server by reading its PID from the PID file and sending a termination signal."""
     if not Path(PID_FILE).is_file():
         typer.echo("UVicorn server is not running.")
         return
 
-    with open(PID_FILE, "r") as pid_file:
+    with Path(PID_FILE).open() as pid_file:
         pid = int(pid_file.read().strip())
 
     typer.echo(f"Stopping UVicorn server with {pid=:}...")
-    try:
+    with contextlib.suppress(ProcessLookupError):
         os.kill(pid, signal.SIGTERM)
-    except ProcessLookupError:
-        pass
     clean_up()
 
 
 def get_process_port(pid: int) -> Optional[int]:
     process = psutil.Process(pid)
     connections = process.connections()
     if connections:
@@ -85,39 +80,36 @@
         return port
     return None
 
 
 def list_uvicorn_processes():
     """Check for other UVicorn processes and list them"""
     uvicorn_processes = []
-    for process in psutil.process_iter():
-        try:
+    with contextlib.suppress(psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
+        for process in psutil.process_iter():
             process_name = process.name()
             if "uvicorn" in process_name.lower():
                 uvicorn_processes.append(process)
-        except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
-            pass
+
     if uvicorn_processes:
         typer.echo("Other UVicorn processes:")
         for process in uvicorn_processes:
             typer.echo(f"PID: {process.pid}, Name: {process.name()}")
     else:
         typer.echo("No other UVicorn processes found.")
 
 
 def get_web_server_status():
-    """
-    Get the status of the UVicorn server by reading its PID from the PID file.
-    """
-    if not os.path.isfile(PID_FILE):
+    """Get the status of the UVicorn server by reading its PID from the PID file."""
+    if not Path(PID_FILE).is_file():
         typer.echo("No pid file found. Server likely not running.")
         list_uvicorn_processes()
         return
 
-    with open(PID_FILE, "r") as pid_file:
+    with Path(PID_FILE).open() as pid_file:
         pid = int(pid_file.read().strip())
         if psutil.pid_exists(pid):
             port = get_process_port(pid)
             if port:
                 typer.echo(f"UVicorn server is running with {pid=}, {port=}")
             else:
                 typer.echo(f"UVicorn server is running with {pid=:}, couldn't determine port.")
@@ -165,104 +157,162 @@
         if cmd.status == CommandStatus.SUCCESS:
             rich.print(f"[green bold]{cmd.name}: Finished[/]")
         elif cmd.status == CommandStatus.FAILURE:
             rich.print(f"[red bold]{cmd.name}: Failed, {exit_code=:}[/]")
 
 
 def format_elapsed_time(seconds: float) -> str:
-    """
-    Converts a number of seconds into a human-readable time format of HH:MM:SS.xxx
+    """Converts a number of seconds into a human-readable time format of HH:MM:SS.xxx
 
     Args:
+    ----
     seconds (float): The number of seconds elapsed.
 
     Returns:
+    -------
     str: The formatted time string.
+
     """
     hours = int(seconds) // 3600
     minutes = (int(seconds) % 3600) // 60
     seconds = seconds % 60  # Keeping the fractional part of seconds
 
     # Return formatted string with seconds rounded to 2 d.p.
     return f"{hours:02}:{minutes:02}:{seconds:06.3f}"
 
 
+def show_commands(groups: list[CommandGroup]):
+    for grp in groups:
+        rich.print(f"[blue bold]Group: {grp.name}[/]")
+        rich.print(
+            f"Params: cont_on_fail={grp.cont_on_fail}, serial={grp.serial}, timeout={grp.timeout}, retries={grp.retries}"
+        )
+        for cmd in grp.cmds.values():
+            rich.print(f"[green bold]{cmd.name}[/]: {cmd.cmd}")
+
+
+def filter_groups(
+    group_list: list[CommandGroup], filter_groups: Optional[str], filter_cmds: Optional[str]
+) -> list[CommandGroup]:
+    if filter_groups:
+        group_list = [grp for grp in group_list if grp.name in [g.strip() for g in filter_groups.split(",")]]
+
+    if filter_cmds:
+        for grp in group_list:
+            grp.cmds = OrderedDict(
+                {
+                    cmd_name: cmd
+                    for cmd_name, cmd in grp.cmds.items()
+                    if cmd_name in [c.strip() for c in filter_cmds.split(",")]
+                },
+            )
+        group_list = [grp for grp in group_list if grp.cmds]
+    return group_list
+
+
+def add_table_break(tbl: rich.table.Table, break_ch: str = "-", break_style: Optional[str] = None) -> rich.table.Table:
+    break_data: list[str] = [break_ch * int(col.width) for col in tbl.columns if col.width is not None]
+    tbl.add_row(
+        *break_data,
+        style=break_style,
+    )
+    return tbl
+
+
+def build_results_tbl() -> rich.table.Table:
+    res_tbl = rich.table.Table(title="Results", show_header=True, header_style="bold blue", box=rich.box.ROUNDED)
+    group_w, name_w, cmd_w, status_w, elap_w = (10, 15, 50, 6, 12)
+    res_tbl.add_column("Group", style="bold blue", width=group_w, no_wrap=True)
+    res_tbl.add_column("Name", style="bold blue", width=name_w, no_wrap=True)
+    res_tbl.add_column("Command", style="bold blue", width=cmd_w, no_wrap=True)
+    res_tbl.add_column("Status", style="bold blue", width=status_w, no_wrap=True)
+    res_tbl.add_column("Elapsed", style="bold blue", width=elap_w, no_wrap=True)
+    return res_tbl
+
+
+def add_command_row(tbl: rich.table.Table, cmd: Command, group_name: str) -> rich.table.Table:
+    elap_str = format_elapsed_time(cmd.elapsed) if cmd.elapsed else "XX:XX:XX.xxx"
+
+    if cmd.status == CommandStatus.SUCCESS:
+        cmd_status = "✅"
+        row_style = "green"
+    elif cmd.status == CommandStatus.FAILURE:
+        cmd_status = "❌"
+        row_style = "red"
+    else:
+        cmd_status = "⏳"
+        row_style = "yellow"
+
+    tbl.add_row(group_name, cmd.name, cmd.cmd, cmd_status, elap_str, style=row_style)
+    return tbl
+
+
+def fmt_group_name(cmd_group: CommandGroup) -> str:
+    if cmd_group.status == CommandStatus.SUCCESS:
+        return f"[green]{cmd_group.name}[/]"
+    elif cmd_group.status == CommandStatus.FAILURE:
+        return f"[red]{cmd_group.name}[/]"
+    else:
+        return f"[yellow]{cmd_group.name}[/]"
+
+
+style_default = typer.Option(help="Processing strategy", default="comp")
+show_default = typer.Option(help="Show available groups and commands", default=False)
+pyproj_default = typer.Option(help="The default toml file to use", default=Path("pyproject.toml"))
+groups_default = typer.Option(help="Run a specific group of commands, comma spearated", default=None)
+cmds_default = typer.Option(help="Run specific commands, comma separated", default=None)
+
+
 @cli_app.command()
 def run(
-    style: ProcessingStrategy = typer.Option(help="Processing strategy", default="comp"),
-    show: bool = typer.Option(help="Show available groups and commands", default=False),
-    file: Path = typer.Option(help="The commands.ini file to use", default=Path("pyproject.toml")),
-    groups: Optional[str] = typer.Option(None, help="Run a specific group of commands, comma spearated"),
-    cmds: Optional[str] = typer.Option(None, help="Run a specific commands, comma spearated"),
+    style: Annotated[ProcessingStrategy, typer.Option] = style_default,
+    show: Annotated[bool, typer.Option] = show_default,
+    file: Annotated[Path, typer.Option] = pyproj_default,
+    groups: Annotated[Optional[str], typer.Option] = groups_default,
+    cmds: Annotated[Optional[str], typer.Option] = cmds_default,
 ):
     """Run commands in parallel"""
     # Overall exit code, need to track all command exit codes to update this
     exit_code = 0
     st_all = time.perf_counter()
-    # console = rich.console.Console()
+
     master_groups = read_commands_toml(file)
     if show:
-        for grp in master_groups:
-            rich.print(f"[blue bold]Group: {grp.name}[/]")
-            for _, cmd in grp.cmds.items():
-                rich.print(f"[green bold]{cmd.name}[/]: {cmd.cmd}")
-        return
+        return show_commands(master_groups)
 
-    if groups:
-        master_groups = [grp for grp in master_groups if grp.name in [g.strip() for g in groups.split(",")]]
-
-    if cmds:
-        for grp in master_groups:
-            grp.cmds = OrderedDict(
-                {
-                    cmd_name: cmd
-                    for cmd_name, cmd in grp.cmds.items()
-                    if cmd_name in [c.strip() for c in cmds.split(",")]
-                }
-            )
-        master_groups = [grp for grp in master_groups if grp.cmds]
+    master_groups = filter_groups(master_groups, groups, cmds)
 
     if not master_groups:
         rich.print("[blue]No groups or commands found.[/]")
         raise typer.Exit(0)
 
     for grp in master_groups:
         if style == ProcessingStrategy.ON_COMP:
-            exit_code = exit_code or grp.run(style, CLICommandCBOnComp())
+            exit_code = grp.run(style, CLICommandCBOnComp())
         elif style == ProcessingStrategy.ON_RECV:
-            exit_code = exit_code or grp.run(style, CLICommandCBOnRecv())
+            exit_code = grp.run(style, CLICommandCBOnRecv())
         else:
             raise typer.BadParameter("Invalid processing strategy")
+        if exit_code != 0 and not grp.cont_on_fail:
+            break
 
     # Summarise the results
     console = rich.console.Console()
-    for grp in master_groups:
-        console.print(f"[blue bold]Group: {grp.name}[/]")
-        for _, cmd in grp.cmds.items():
-            elap_str = ""
-            if cmd.elapsed:
-                elap_str = f", {format_elapsed_time(cmd.elapsed)}"
-            else:
-                elap_str = ", XX:XX:XX.xxx"
+    res_tbl = build_results_tbl()
 
-            if cmd.status == CommandStatus.SUCCESS:
-                left_seg = f"[green bold]Command {cmd.name} succeeded "
-            else:
-                left_seg = f"[red bold]Command {cmd.name} failed "
-
-            right_seg = f"({cmd.num_non_empty_lines}{elap_str})[/]"
+    for grp_ix, grp in enumerate(master_groups):
+        for ix, cmd in enumerate(grp.cmds.values()):
+            if grp_ix > 0 and ix == 0:
+                add_table_break(res_tbl)
+            grp_name = fmt_group_name(grp)
+            if ix > 0:
+                grp_name = ""
+            add_command_row(res_tbl, cmd, grp_name)
 
-            # Adjust total line width dynamically based on max width and other content
-            pad_length = (
-                100 - len(left_seg) - len(right_seg) - 10
-                if "succeeded" in left_seg
-                else 100 - len(left_seg) - len(right_seg) - 12
-            )
-
-            rich.print(f"{left_seg}{' ' * pad_length}{right_seg}")
+    console.print(res_tbl)
     end_style = "[green bold]" if exit_code == 0 else "[red bold]"
     rich.print(f"\n{end_style}Total elapsed time: {format_elapsed_time(time.perf_counter() - st_all)}[/]")
     raise typer.Exit(exit_code)
 
 
 try:
     import os
@@ -276,18 +326,21 @@
     import psutil
     import typer
 
     rich.print("[blue]Web commands loaded[/]")
 
     PID_FILE = ".par-run.uvicorn.pid"
 
+    command_default = typer.Argument(..., help="command to control/interract with the web server")
+    port_default = typer.Option(8001, help="Port to run the web server")
+
     @cli_app.command()
     def web(
-        command: WebCommand = typer.Argument(..., help="command to control/interract with the web server"),
-        port: int = typer.Option(8001, help="Port to run the web server"),
+        command: WebCommand = command_default,
+        port: int = port_default,
     ):
         """Run the web server"""
         if command == WebCommand.START:
             start_web_server(port)
         elif command == WebCommand.STOP:
             stop_web_server()
         elif command == WebCommand.RESTART:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `par_run-0.2.2/src/par_run/executor.py` & `par_run-0.3.0/src/par_run/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import asyncio
 import configparser
 import enum
 import multiprocessing as mp
 import os
 import queue
 import subprocess
+import time
 from collections import OrderedDict
 from concurrent.futures import Future, ProcessPoolExecutor
 from pathlib import Path
 from queue import Queue
-import time
-from typing import List, Optional, Protocol, TypeVar, Union, Any
-from pydantic import BaseModel, Field, ConfigDict
+from typing import Any, Optional, Protocol, TypeVar, Union
+
 import tomlkit
+from pydantic import BaseModel, ConfigDict, Field
 
 # Type alias for a generic future.
 GenFuture = Union[Future, asyncio.Future]
 
 ContextT = TypeVar("ContextT")
 
 
@@ -48,15 +49,15 @@
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     name: str
     cmd: str
     passenv: Optional[list[str]] = Field(default=None)
     setenv: Optional[dict[str, str]] = Field(default=None)
     status: CommandStatus = CommandStatus.NOT_STARTED
-    unflushed: List[str] = Field(default=[], exclude=True)
+    unflushed: list[str] = Field(default=[], exclude=True)
     num_non_empty_lines: int = Field(default=0, exclude=True)
     ret_code: Optional[int] = Field(default=None, exclude=True)
     fut: Optional[GenFuture] = Field(default=None, exclude=True)
     start_time: Optional[float] = Field(default=None, exclude=True)
     elapsed: Optional[float] = Field(default=None, exclude=True)
 
     def incr_line_count(self, line: str) -> None:
@@ -110,33 +111,43 @@
         self.retries = retries
 
     def get(self):
         retry_count = 0
         while True:
             try:
                 return self.q.get(block=True, timeout=self.timeout)
-            except queue.Empty:
+            except queue.Empty:  # noqa: PERF203
                 if retry_count < self.retries:
                     retry_count += 1
                     continue
                 else:
-                    raise TimeoutError("Timeout waiting for command output")
+                    raise TimeoutError("Timeout waiting for command output") from None
 
     def __str__(self) -> str:
         return f"QRetriever(timeout={self.timeout}, retries={self.retries})"
 
 
 class CommandGroup(BaseModel):
     """Holder for a group of commands."""
 
     name: str
     desc: Optional[str] = None
     cmds: OrderedDict[str, Command] = Field(default_factory=OrderedDict)
     timeout: int = Field(default=30)
     retries: int = Field(default=3)
+    cont_on_fail: bool = Field(default=False)
+    serial: bool = Field(default=False)
+    status: CommandStatus = CommandStatus.NOT_STARTED
+
+    def update_status(self, cmds: OrderedDict[str, Command]):
+        """Update the status of the command group."""
+        if all(cmd.status == CommandStatus.SUCCESS for cmd in cmds.values()):
+            self.status = CommandStatus.SUCCESS
+        else:
+            self.status = CommandStatus.FAILURE
 
     async def run_async(
         self,
         strategy: ProcessingStrategy,
         callbacks: CommandAsyncCB,
     ):
         q = mp.Manager().Queue()
@@ -151,30 +162,40 @@
             cmd.set_running()
 
         return await self._process_q_async(q, strategy, callbacks)
 
     def run(self, strategy: ProcessingStrategy, callbacks: CommandCB):
         q = mp.Manager().Queue()
         pool = ProcessPoolExecutor()
-        futs = [pool.submit(run_command, cmd.name, cmd.cmd, cmd.setenv, q) for _, cmd in self.cmds.items()]
-        for (_, cmd), fut in zip(self.cmds.items(), futs):
-            cmd.fut = fut
-            cmd.set_running()
-        return self._process_q(q, strategy, callbacks)
+        cmd_series = [OrderedDict([(k, v)]) for k, v in self.cmds.items()] if self.serial else [self.cmds]
+        group_exit_code = 0
 
-    def _process_q(
+        for cmd_entries in cmd_series:
+            futs = [pool.submit(run_command, cmd.name, cmd.cmd, cmd.setenv, q) for cmd in cmd_entries.values()]
+            for cmd, fut in zip(cmd_entries.values(), futs):
+                cmd.fut = fut
+                cmd.set_running()
+            exit_code = self._process_q(cmd_entries, q, strategy, callbacks)
+            if exit_code != 0:
+                group_exit_code = 1
+                if not self.cont_on_fail:
+                    break
+        return group_exit_code
+
+    def _process_q(  # noqa: PLR0912
         self,
+        cmds: OrderedDict[str, Command],
         q: Queue,
         strategy: ProcessingStrategy,
         callbacks: CommandCB,
     ) -> int:
         grp_exit_code = 0
 
         if strategy == ProcessingStrategy.ON_RECV:
-            for _, cmd in self.cmds.items():
+            for cmd in cmds.values():
                 callbacks.on_start(cmd)
 
         q_ret = QRetriever(q, self.timeout, self.retries)
         while True:
             q_result = q_ret.get()
 
             # Can only get here with a valid message from the Q
@@ -209,28 +230,29 @@
                     callbacks.on_term(cmd, exit_code)
                     cmd.set_ret_code(exit_code)
                     if exit_code != 0:
                         grp_exit_code = 1
                 else:
                     raise ValueError("Invalid Q message")  # pragma: no cover
 
-            if all(cmd.status.completed() for _, cmd in self.cmds.items()):
+            if all(cmd.status.completed() for cmd in cmds.values()):
+                self.update_status(cmds)
                 break
         return grp_exit_code
 
-    async def _process_q_async(
+    async def _process_q_async(  # noqa: PLR0912
         self,
         q: Queue,
         strategy: ProcessingStrategy,
         callbacks: CommandAsyncCB,
     ) -> int:
         grp_exit_code = 0
 
         if strategy == ProcessingStrategy.ON_RECV:
-            for _, cmd in self.cmds.items():
+            for cmd in self.cmds.values():
                 await callbacks.on_start(cmd)
 
         q_ret = QRetriever(q, self.timeout, self.retries)
         while True:
             await asyncio.sleep(0)
             q_result = q_ret.get()
 
@@ -275,135 +297,159 @@
         return grp_exit_code
 
 
 def read_commands_ini(filename: Union[str, Path]) -> list[CommandGroup]:
     """Read a commands.ini file and return a list of CommandGroup objects.
 
     Args:
+    ----
         filename (Union[str, Path]): The filename of the commands.ini file.
 
     Returns:
+    -------
         list[CommandGroup]: A list of CommandGroup objects.
+
     """
     config = configparser.ConfigParser()
     config.read(filename)
 
     command_groups = []
     for section in config.sections():
         if section.startswith("group."):
             group_name = section.replace("group.", "")
             commands = OrderedDict()
             for name, cmd in config.items(section):
-                name = name.strip()
-                commands[name] = Command(name=name, cmd=cmd.strip())
+                clean_name = name.strip()
+                commands[clean_name] = Command(name=clean_name, cmd=cmd.strip())
             command_group = CommandGroup(name=group_name, cmds=commands)
             command_groups.append(command_group)
 
     return command_groups
 
 
 def write_commands_ini(filename: Union[str, Path], command_groups: list[CommandGroup]):
     """Write a list of CommandGroup objects to a commands.ini file.
 
     Args:
+    ----
         filename (Union[str, Path]): The filename of the commands.ini file.
         command_groups (list[CommandGroup]): A list of CommandGroup objects.
+
     """
     config = configparser.ConfigParser()
 
     for group in command_groups:
         section_name = f"group.{group.name}"
         config[section_name] = {}
-        for _, command in group.cmds.items():
+        for command in group.cmds.values():
             config[section_name][command.name] = command.cmd
 
-    with open(filename, "w", encoding="utf-8") as configfile:
+    with Path(filename).open("w", encoding="utf-8") as configfile:
         config.write(configfile)
 
 
 def _validate_mandatory_keys(data: tomlkit.items.Table, keys: list[str], context: str) -> tuple[Any, ...]:
     """Validate that the mandatory keys are present in the data.
 
     Args:
+    ----
         data (tomlkit.items.Table): The data to validate.
         keys (list[str]): The mandatory keys.
+
     """
     vals = []
     for key in keys:
         val = data.get(key, None)
         if not val:
             raise ValueError(f"{key} is mandatory, not found in {context}")
         vals.append(val)
     return tuple(vals)
 
 
 def _get_optional_keys(data: tomlkit.items.Table, keys: list[str], default=None) -> tuple[Optional[Any], ...]:
     """Get Optional keys or default.
 
     Args:
+    ----
         data (tomlkit.items.Table): The data to use as source
         keys (list[str]): The optional keys.
+
     """
-    return tuple(data.get(key, default) for key in keys)
+    res = tuple(data.get(key, default) for key in keys)
+    return res
 
 
 def read_commands_toml(filename: Union[str, Path]) -> list[CommandGroup]:
     """Read a commands.toml file and return a list of CommandGroup objects.
 
     Args:
+    ----
         filename (Union[str, Path]): The filename of the commands.toml file.
 
     Returns:
+    -------
         list[CommandGroup]: A list of CommandGroup objects.
-    """
 
-    with open(filename, "r", encoding="utf-8") as toml_file:
+    """
+    with Path(filename).open(encoding="utf-8") as toml_file:
         toml_data = tomlkit.parse(toml_file.read())
 
     cmd_groups_data = toml_data.get("tool", {}).get("par-run", {})
     if not cmd_groups_data:
         raise ValueError("No par-run data found in toml file")
     _ = cmd_groups_data.get("description", None)
 
     command_groups = []
     for group_data in cmd_groups_data.get("groups", []):
         (group_name,) = _validate_mandatory_keys(group_data, ["name"], "top level par-run group")
         group_desc, group_timeout, group_retries = _get_optional_keys(
-            group_data, ["desc", "timeout", "retries"], default=None
+            group_data,
+            ["desc", "timeout", "retries"],
+            default=None,
         )
+        (group_cont_on_fail, group_serial) = _get_optional_keys(group_data, ["cont_on_fail", "serial"], default=False)
 
         if not group_timeout:
             group_timeout = 30
         if not group_retries:
             group_retries = 3
+        group_cont_on_fail = bool(group_cont_on_fail and group_cont_on_fail is True)
+        group_serial = bool(group_serial and group_serial is True)
 
         commands = OrderedDict()
         for cmd_data in group_data.get("commands", []):
             name, exec = _validate_mandatory_keys(cmd_data, ["name", "exec"], f"command group {group_name}")
             setenv, passenv = _get_optional_keys(cmd_data, ["setenv", "passenv"], default=None)
 
             commands[name] = Command(name=name, cmd=exec, setenv=setenv, passenv=passenv)
         command_group = CommandGroup(
-            name=group_name, desc=group_desc, cmds=commands, timeout=group_timeout, retries=group_retries
+            name=group_name,
+            desc=group_desc,
+            cmds=commands,
+            timeout=group_timeout,
+            retries=group_retries,
+            cont_on_fail=group_cont_on_fail,
+            serial=group_serial,
         )
         command_groups.append(command_group)
 
     return command_groups
 
 
 def run_command(name: str, command: str, setenv: Optional[dict[str, str]], q: Queue) -> None:
     """Run a command and put the output into a queue. The output is a tuple of the command
     name and the output line. The final output is a tuple of the command name and a dictionary
     with the return code.
 
     Args:
+    ----
         name (Command): Command to run.
         q (Queue): Queue to put the output into.
-    """
 
+    """
     new_env = None
     if setenv:
         new_env = os.environ.copy()
         new_env.update(setenv)
 
     with subprocess.Popen(
         command,
```

### Comparing `par_run-0.2.2/src/par_run/web.py` & `par_run-0.3.0/src/par_run/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """Web UI Module"""
 
 from pathlib import Path
+
 import rich
 from fastapi import Body, FastAPI, Request, WebSocket
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 
-from .executor import Command, CommandGroup, ProcessingStrategy, read_commands_ini, write_commands_ini
+from .executor import Command, ProcessingStrategy, read_commands_ini, write_commands_ini
 
 BASE_PATH = Path(__file__).resolve().parent
 
 ws_app = FastAPI()
 ws_app.mount("/static", StaticFiles(directory=str(BASE_PATH / "static")), name="static")
 templates = Jinja2Templates(directory=str(BASE_PATH / "templates"))
 
 
 @ws_app.get("/")
 async def ws_main(request: Request):
     """Get the main page."""
-    print("Main page")
     return templates.TemplateResponse("index.html", {"request": request})
 
 
 @ws_app.get("/get-commands-config")
 async def get_commands_config():
     """Get the commands configuration."""
     return read_commands_ini("commands.ini")
 
 
 @ws_app.post("/update-commands-config")
-async def update_commands_config(updated_config: list[CommandGroup] = Body(...)):
+async def update_commands_config(updated_config=Body(...)):  # noqa: B008
     """Update the commands configuration."""
     write_commands_ini("commands.ini", updated_config)
     return {"message": "Configuration updated successfully"}
 
 
 class WebCommandCB:
     """Websocket command callbacks."""
@@ -52,14 +52,12 @@
 
 
 @ws_app.websocket_route("/ws")
 async def websocket_endpoint(websocket: WebSocket):
     """Websocket endpoint to run commands."""
     rich.print("Websocket connection")
     master_groups = read_commands_ini("commands.ini")
-    print(master_groups)
     await websocket.accept()
     cb = WebCommandCB(websocket)
-    print("Running commands")
     exit_code = 0
     for grp in master_groups:
         exit_code = exit_code or await grp.run_async(ProcessingStrategy.ON_RECV, cb)
```

### Comparing `par_run-0.2.2/src/par_run/static/css/style.css` & `par_run-0.3.0/src/par_run/static/css/style.css`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/src/par_run/static/js/app.js` & `par_run-0.3.0/src/par_run/static/js/app.js`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/src/par_run/templates/index.html` & `par_run-0.3.0/src/par_run/templates/index.html`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/.gitignore` & `par_run-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/LICENSE` & `par_run-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/README.md` & `par_run-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `par_run-0.2.2/pyproject.toml` & `par_run-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "par-run"
-version = "0.2.2"
+version = "0.3.0"
 description = "Parallel command runner"
 license = "MIT"
 authors = [
     { name = "Naz Quadri", email = "naz.quadri@gmail.com" }
 ]
 classifiers = [
     'Development Status :: 4 - Beta',
@@ -75,15 +75,15 @@
 packages = [
     "src/par_run",
     "static",
     "templates",
 ]
 
 [tool.bumpversion]
-current_version = "0.2.2"
+current_version = "0.3.0"
 commit = true
 tag = true
 tag_name = "{new_version}"
 tag_message = "Version {new_version}"
 message = "Bump version: {current_version} → {new_version}"
 allow_dirty = true
 parse = """(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"""
@@ -98,14 +98,38 @@
 filename = "pyproject.toml"
 
 [tool.ruff]
 line-length = 120
 indent-width = 4
 target-version = "py39"
 
+[tool.ruff.lint]
+extend-select = [
+    'Q',
+    'B',
+    'UP',
+    'I',
+    'F',
+    'PTH',
+    'PIE',
+    'TID',
+    'ERA',
+    'ARG',
+    'PL',
+    #'ANN',
+    'SIM',
+    'PERF',
+    'T20',
+]
+extend-ignore = ["S101", "FA100"]
+
+[tool.ruff.lint.isort]
+known-first-party = ["par_run"]
+
+
 [tool.pytest.ini_options]
 addopts = "--cov src --cov-report html:.reports/html --cov-report term --random-order -p no:warnings -v"
 minversion = "8.0"
 pythonpath = ["src", "py_tests"]
 testpaths = "py_tests"
 pythonfiles = "test_*.py"
 
@@ -114,14 +138,16 @@
 desc = "par-run from pyproject.toml"
 
 [[tool.par-run.groups]]
 name = "Formatting"
 desc = "Code formatting commands."
 timeout = 5
 retries = 3 
+cont_on_fail = true # default is false
+serial = false # default is false
 
   [[tool.par-run.groups.commands]]
   name = "ruff_fmt"
   exec = "ruff format src py_tests"
   # Define an empty extras using standard table notation, or simply omit it if it's always empty
 
   [[tool.par-run.groups.commands]]
@@ -131,14 +157,15 @@
 
 
 [[tool.par-run.groups]]
 name = "Quality"
 desc = "Code Quality Tools. No code mutation"
 timeout = 5
 retries = 3
+cont_on_fail = true # default is false
 
   [[tool.par-run.groups.commands]]
   name = "ruff_lint"
   exec = "ruff check src py_tests"
   # extras omitted as it's empty
 
   [[tool.par-run.groups.commands]]
@@ -153,17 +180,36 @@
 
 
 [[tool.par-run.groups]]
 name = "ENV"
 desc = "Code Quality Tools. No code mutation"
 timeout = 5
 retries = 3
+cont_on_fail = true # default is false
+
 
   [[tool.par-run.groups.commands]]
   name = "full_env"
   exec = "env"
   setenv = {MY_VAR = "production", ENABLE_LOGS = "true"}
 
   [[tool.par-run.groups.commands]]
   name = "my_var"
   exec = "echo \"MY_VAR=$MY_VAR\", \"ENABLE_LOGS=$ENABLE_LOGS\""
   setenv = {MY_VAR = "production", ENABLE_LOGS = "true"}
+
+
+[[tool.par-run.groups]]
+name = "Serial"
+desc = "Must run serially"
+timeout = 5
+retries = 3
+cont_on_fail = true # default is false
+serial = true
+
+  [[tool.par-run.groups.commands]]
+  name = "sleep then create file"
+  exec = "sleep 2 && touch /tmp/test.pr"
+
+  [[tool.par-run.groups.commands]]
+  name = "try delete file"
+  exec = "rm /tmp/test.pr"
```

### Comparing `par_run-0.2.2/PKG-INFO` & `par_run-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: par-run
-Version: 0.2.2
+Version: 0.3.0
 Summary: Parallel command runner
 Project-URL: Homepage, https://github.com/nazq/par-run
 Project-URL: Documentation, https://github.com/nazq/par-run
 Project-URL: Repository, https://github.com/nazq/par-run
 Project-URL: Issues, https://github.com/nazq/par-run/issues
 Project-URL: Changelog, https://github.com/nazq/par-run
 Author-email: Naz Quadri <naz.quadri@gmail.com>
```

