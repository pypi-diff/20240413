# Comparing `tmp/mdformat_mkdocs-2.0.7.tar.gz` & `tmp/mdformat_mkdocs-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_mkdocs-2.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mdformat_mkdocs-2.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_mkdocs-2.0.7.tar` & `mdformat_mkdocs-2.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      600 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/.copier-answers.yml
--rw-r--r--   0        0        0     1819 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/.gitignore
--rw-r--r--   0        0        0     1592 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1085 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/.pre-commit-test.yaml
--rw-r--r--   0        0        0     2882 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/.ruff.toml
--rw-r--r--   0        0        0       21 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/.tool-versions
--rw-r--r--   0        0        0      276 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/.yamllint.yaml
--rw-r--r--   0        0        0     1366 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/LICENSE
--rw-r--r--   0        0        0     4366 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/README.md
--rw-r--r--   0        0        0      303 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/mdformat_mkdocs/__init__.py
--rw-r--r--   0        0        0      914 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/mdformat_mkdocs/_helpers.py
--rw-r--r--   0        0        0    11281 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/mdformat_mkdocs/_normalize_list.py
--rw-r--r--   0        0        0     2416 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/mdformat_mkdocs/_postprocess_inline.py
--rw-r--r--   0        0        0      317 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/mdformat_mkdocs/mdit_plugins/__init__.py
--rw-r--r--   0        0        0     2368 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/mdformat_mkdocs/mdit_plugins/_content_tabs.py
--rw-r--r--   0        0        0     2843 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py
--rw-r--r--   0        0        0      785 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py
--rw-r--r--   0        0        0     3966 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/mdformat_mkdocs/plugin.py
--rw-r--r--   0        0        0     1698 2024-03-30 21:12:14.079224 mdformat_mkdocs-2.0.7/pyproject.toml
--rw-r--r--   0        0        0      895 2024-03-30 21:12:14.083224 mdformat_mkdocs-2.0.7/tox.ini
--rw-r--r--   0        0        0     6023 1970-01-01 00:00:00.000000 mdformat_mkdocs-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0      600 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.copier-answers.yml
+-rw-r--r--   0        0        0     1819 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.gitignore
+-rw-r--r--   0        0        0     1592 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1085 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.pre-commit-test.yaml
+-rw-r--r--   0        0        0     2882 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.ruff.toml
+-rw-r--r--   0        0        0       21 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.tool-versions
+-rw-r--r--   0        0        0      276 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.yamllint.yaml
+-rw-r--r--   0        0        0     1366 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/LICENSE
+-rw-r--r--   0        0        0     4366 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/README.md
+-rw-r--r--   0        0        0      303 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/__init__.py
+-rw-r--r--   0        0        0      914 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/_helpers.py
+-rw-r--r--   0        0        0    11592 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/_normalize_list.py
+-rw-r--r--   0        0        0     2416 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/_postprocess_inline.py
+-rw-r--r--   0        0        0      317 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/__init__.py
+-rw-r--r--   0        0        0     2368 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_content_tabs.py
+-rw-r--r--   0        0        0     2843 2024-04-13 20:01:44.702604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py
+-rw-r--r--   0        0        0      785 2024-04-13 20:01:44.702604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py
+-rw-r--r--   0        0        0     3966 2024-04-13 20:01:44.702604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/plugin.py
+-rw-r--r--   0        0        0     1698 2024-04-13 20:01:44.702604 mdformat_mkdocs-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0      895 2024-04-13 20:01:44.702604 mdformat_mkdocs-2.0.8/tox.ini
+-rw-r--r--   0        0        0     6023 1970-01-01 00:00:00.000000 mdformat_mkdocs-2.0.8/PKG-INFO
```

### Comparing `mdformat_mkdocs-2.0.7/.copier-answers.yml` & `mdformat_mkdocs-2.0.8/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/.gitignore` & `mdformat_mkdocs-2.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/.pre-commit-config.yaml` & `mdformat_mkdocs-2.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/.pre-commit-test.yaml` & `mdformat_mkdocs-2.0.8/.pre-commit-test.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/.ruff.toml` & `mdformat_mkdocs-2.0.8/.ruff.toml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/CONTRIBUTING.md` & `mdformat_mkdocs-2.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/LICENSE` & `mdformat_mkdocs-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/README.md` & `mdformat_mkdocs-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/mdformat_mkdocs/_helpers.py` & `mdformat_mkdocs-2.0.8/mdformat_mkdocs/_helpers.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/mdformat_mkdocs/_normalize_list.py` & `mdformat_mkdocs-2.0.8/mdformat_mkdocs/_normalize_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,17 +234,20 @@
 
     lines: list[LineResult]
     new_lines: list[tuple[str, str]]
     # Used only for debugging purposes
     debug_block_indents: list[BlockIndent | None]
 
 
-def format_new_content(line: LineResult, inc_numbers: bool) -> str:
+def format_new_content(line: LineResult, inc_numbers: bool, is_code: bool) -> str:
     new_content = line.parsed.content
-    if line.parsed.syntax in {Syntax.LIST_BULLETED, Syntax.LIST_NUMBERED}:
+    if not is_code and line.parsed.syntax in {
+        Syntax.LIST_BULLETED,
+        Syntax.LIST_NUMBERED,
+    }:
         list_match = RE_LIST_ITEM.fullmatch(line.parsed.content)
         assert list_match is not None  # for pyright # noqa: S101
         new_bullet = "-"
         if line.parsed.syntax == Syntax.LIST_NUMBERED:
             counter = len(line.prev_list_peers) + 1 if inc_numbers else 1
             new_bullet = f"{counter}."
         new_content = f'{new_bullet} {list_match["item"]}'
@@ -259,36 +262,42 @@
 
     # `code_block_indents` take precedence to ignore contents of an HTML code block
     code_indents = map_lookback(parse_code_block, lines, None)
     html_indents = map_lookback(parse_html_line, lines, None)
     block_indents = [_c or _h for _c, _h in zip_equal(code_indents, html_indents)]
     new_indents = list(starmap(format_new_indent, zip_equal(lines, block_indents)))
 
-    new_contents = [format_new_content(line, inc_numbers) for line in lines]
+    new_contents = [
+        format_new_content(line, inc_numbers, ci is not None)
+        for line, ci in zip_equal(lines, code_indents)
+    ]
     return ParsedText(
         lines=lines,
         new_lines=[*zip_equal(new_indents, new_contents)],
         debug_block_indents=block_indents,
     )
 
 
 # ======================================================================================
 # Join Operations
 
 
 class SemanticIndent(Enum):
+    """Possible states for evaluating semantic indents. The values aren't relevant."""
+
     INITIAL = "Hack for MyPy and map_lookack, which returns initial..."
     EMPTY = ""
     ONE_LESS_ON_NEXT = "⤓(←)"
     ONE_LESS_SPACE = "←"
     TWO_LESS_ON_NEXT = "⤓(←←)"  # Bulleted
     TWO_LESS_SPACE = "←←"
 
 
 def parse_semantic_indent(last: SemanticIndent, line: LineResult) -> SemanticIndent:
+    """Conditionally evaluate when semantic indents are necessary."""
     # TODO: This works, but is very confusing
     if not line.parsed.content:
         result = SemanticIndent.EMPTY
 
     elif line.parsed.syntax == Syntax.LIST_BULLETED:
         result = SemanticIndent.TWO_LESS_ON_NEXT
     elif line.parsed.syntax == Syntax.LIST_NUMBERED:
@@ -342,14 +351,15 @@
 @rstrip_result
 def normalize_list(
     text: str,
     node: RenderTreeNode,
     context: RenderContext,
     check_if_align_semantic_breaks_in_lists: Callable[[], bool],  # Attach with partial
 ) -> str:
+    """Format markdown list."""
     # FIXME: Is this filter working correctly?
     #   If it is, the test for "Formats non-root lists" should be failing
     if node.level > 1:
         # Note: this function is called recursively,
         #   so only process the top-level item
         return text
```

### Comparing `mdformat_mkdocs-2.0.7/mdformat_mkdocs/_postprocess_inline.py` & `mdformat_mkdocs-2.0.8/mdformat_mkdocs/_postprocess_inline.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/mdformat_mkdocs/mdit_plugins/_content_tabs.py` & `mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_content_tabs.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py` & `mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py` & `mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/mdformat_mkdocs/plugin.py` & `mdformat_mkdocs-2.0.8/mdformat_mkdocs/plugin.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/pyproject.toml` & `mdformat_mkdocs-2.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/tox.ini` & `mdformat_mkdocs-2.0.8/tox.ini`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.7/PKG-INFO` & `mdformat_mkdocs-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdformat_mkdocs
-Version: 2.0.7
+Version: 2.0.8
 Summary: An mdformat plugin for mkdocs.
 Keywords: markdown,markdown-it,mdformat
 Author-email: kyleking <dev.act.kyle@gmail.com>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

